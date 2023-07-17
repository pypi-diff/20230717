# Comparing `tmp/llmtuner-0.0.9.tar.gz` & `tmp/llmtuner-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmtuner-0.0.9.tar", last modified: Sat Jul 15 09:18:28 2023, max compression
+gzip compressed data, was "llmtuner-0.1.0.tar", last modified: Mon Jul 17 16:33:17 2023, max compression
```

## Comparing `llmtuner-0.0.9.tar` & `llmtuner-0.1.0.tar`

### file list

```diff
@@ -1,68 +1,89 @@
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.413016 llmtuner-0.0.9/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-15 09:06:30.000000 llmtuner-0.0.9/LICENSE
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    13532 2023-07-15 09:18:28.413016 llmtuner-0.0.9/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    12888 2023-07-15 09:06:30.000000 llmtuner-0.0.9/README.md
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-15 09:06:30.000000 llmtuner-0.0.9/pyproject.toml
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-15 09:18:28.413016 llmtuner-0.0.9/setup.cfg
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2033 2023-07-15 09:06:30.000000 llmtuner-0.0.9/setup.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.285015 llmtuner-0.0.9/src/
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.309016 llmtuner-0.0.9/src/llmtuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      285 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.317016 llmtuner-0.0.9/src/llmtuner/api/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       41 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/api/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5783 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/api/app.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2053 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/api/protocol.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.341016 llmtuner-0.0.9/src/llmtuner/dsets/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      105 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/dsets/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2565 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/dsets/callbacks.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4294 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/dsets/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8194 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/dsets/preprocess.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.349016 llmtuner-0.0.9/src/llmtuner/extras/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/extras/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3101 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/extras/callbacks.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      211 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/extras/constants.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      443 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/extras/logging.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3884 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/extras/misc.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1716 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/extras/ploting.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2172 2023-07-15 09:06:27.000000 llmtuner-0.0.9/src/llmtuner/extras/save_and_load.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6433 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/extras/template.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.353016 llmtuner-0.0.9/src/llmtuner/hparams/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      222 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/hparams/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5012 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/hparams/data_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3738 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/hparams/finetuning_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      388 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/hparams/general_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1973 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/hparams/generating_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3053 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/hparams/model_args.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.357016 llmtuner-0.0.9/src/llmtuner/tuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      241 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.393016 llmtuner-0.0.9/src/llmtuner/tuner/core/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/core/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3839 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/tuner/core/adapter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6975 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/tuner/core/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6400 2023-07-15 09:06:28.000000 llmtuner-0.0.9/src/llmtuner/tuner/core/parser.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4113 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/core/trainer.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.401016 llmtuner-0.0.9/src/llmtuner/tuner/ppo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/ppo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8765 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/ppo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1673 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/ppo/utils.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2926 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/ppo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.401016 llmtuner-0.0.9/src/llmtuner/tuner/pt/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/pt/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2884 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/pt/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.409016 llmtuner-0.0.9/src/llmtuner/tuner/rm/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/rm/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      722 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/rm/collator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/rm/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1482 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/rm/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2741 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/rm/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.409016 llmtuner-0.0.9/src/llmtuner/tuner/sft/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-15 09:06:30.000000 llmtuner-0.0.9/src/llmtuner/tuner/sft/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2069 2023-07-15 09:06:29.000000 llmtuner-0.0.9/src/llmtuner/tuner/sft/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3059 2023-07-15 09:06:30.000000 llmtuner-0.0.9/src/llmtuner/tuner/sft/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4264 2023-07-15 09:06:30.000000 llmtuner-0.0.9/src/llmtuner/tuner/sft/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 09:18:28.313016 llmtuner-0.0.9/src/llmtuner.egg-info/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    13532 2023-07-15 09:18:27.000000 llmtuner-0.0.9/src/llmtuner.egg-info/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1641 2023-07-15 09:18:27.000000 llmtuner-0.0.9/src/llmtuner.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-15 09:18:27.000000 llmtuner-0.0.9/src/llmtuner.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      206 2023-07-15 09:18:27.000000 llmtuner-0.0.9/src/llmtuner.egg-info/requires.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-15 09:18:27.000000 llmtuner-0.0.9/src/llmtuner.egg-info/top_level.txt
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:33:17.272834 llmtuner-0.1.0/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-17 16:32:51.000000 llmtuner-0.1.0/LICENSE
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    14082 2023-07-17 16:33:17.272834 llmtuner-0.1.0/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    13447 2023-07-17 16:32:57.000000 llmtuner-0.1.0/README.md
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-17 16:32:57.000000 llmtuner-0.1.0/pyproject.toml
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-17 16:33:17.272834 llmtuner-0.1.0/setup.cfg
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2033 2023-07-17 16:32:57.000000 llmtuner-0.1.0/setup.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:33:16.980834 llmtuner-0.1.0/src/
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:33:16.992834 llmtuner-0.1.0/src/llmtuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      258 2023-07-17 16:32:55.000000 llmtuner-0.1.0/src/llmtuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:33:17.028834 llmtuner-0.1.0/src/llmtuner/api/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       41 2023-07-17 16:32:52.000000 llmtuner-0.1.0/src/llmtuner/api/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4624 2023-07-17 16:32:51.000000 llmtuner-0.1.0/src/llmtuner/api/app.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2053 2023-07-17 16:32:52.000000 llmtuner-0.1.0/src/llmtuner/api/protocol.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:33:17.032834 llmtuner-0.1.0/src/llmtuner/chat/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-17 16:32:52.000000 llmtuner-0.1.0/src/llmtuner/chat/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3737 2023-07-17 16:32:52.000000 llmtuner-0.1.0/src/llmtuner/chat/stream_chat.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:33:17.040834 llmtuner-0.1.0/src/llmtuner/dsets/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      105 2023-07-17 16:32:52.000000 llmtuner-0.1.0/src/llmtuner/dsets/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2565 2023-07-17 16:32:52.000000 llmtuner-0.1.0/src/llmtuner/dsets/callbacks.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4294 2023-07-17 16:32:52.000000 llmtuner-0.1.0/src/llmtuner/dsets/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8194 2023-07-17 16:32:52.000000 llmtuner-0.1.0/src/llmtuner/dsets/preprocess.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:33:17.104834 llmtuner-0.1.0/src/llmtuner/extras/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:32:53.000000 llmtuner-0.1.0/src/llmtuner/extras/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3071 2023-07-17 16:32:53.000000 llmtuner-0.1.0/src/llmtuner/extras/callbacks.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1410 2023-07-17 16:32:53.000000 llmtuner-0.1.0/src/llmtuner/extras/constants.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      751 2023-07-17 16:32:53.000000 llmtuner-0.1.0/src/llmtuner/extras/logging.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3884 2023-07-17 16:32:53.000000 llmtuner-0.1.0/src/llmtuner/extras/misc.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1788 2023-07-17 16:32:53.000000 llmtuner-0.1.0/src/llmtuner/extras/ploting.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2172 2023-07-17 16:32:53.000000 llmtuner-0.1.0/src/llmtuner/extras/save_and_load.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5453 2023-07-17 16:32:53.000000 llmtuner-0.1.0/src/llmtuner/extras/template.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:33:17.120834 llmtuner-0.1.0/src/llmtuner/hparams/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      222 2023-07-17 16:32:54.000000 llmtuner-0.1.0/src/llmtuner/hparams/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5013 2023-07-17 16:32:53.000000 llmtuner-0.1.0/src/llmtuner/hparams/data_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3739 2023-07-17 16:32:53.000000 llmtuner-0.1.0/src/llmtuner/hparams/finetuning_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      388 2023-07-17 16:32:53.000000 llmtuner-0.1.0/src/llmtuner/hparams/general_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1973 2023-07-17 16:32:54.000000 llmtuner-0.1.0/src/llmtuner/hparams/generating_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3053 2023-07-17 16:32:54.000000 llmtuner-0.1.0/src/llmtuner/hparams/model_args.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:33:17.120834 llmtuner-0.1.0/src/llmtuner/tuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      241 2023-07-17 16:32:55.000000 llmtuner-0.1.0/src/llmtuner/tuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:33:17.184834 llmtuner-0.1.0/src/llmtuner/tuner/core/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-07-17 16:32:54.000000 llmtuner-0.1.0/src/llmtuner/tuner/core/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3839 2023-07-17 16:32:54.000000 llmtuner-0.1.0/src/llmtuner/tuner/core/adapter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7094 2023-07-17 16:32:54.000000 llmtuner-0.1.0/src/llmtuner/tuner/core/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6400 2023-07-17 16:32:54.000000 llmtuner-0.1.0/src/llmtuner/tuner/core/parser.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4113 2023-07-17 16:32:54.000000 llmtuner-0.1.0/src/llmtuner/tuner/core/trainer.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:33:17.192834 llmtuner-0.1.0/src/llmtuner/tuner/ppo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-17 16:32:54.000000 llmtuner-0.1.0/src/llmtuner/tuner/ppo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8091 2023-07-17 16:32:54.000000 llmtuner-0.1.0/src/llmtuner/tuner/ppo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1673 2023-07-17 16:32:54.000000 llmtuner-0.1.0/src/llmtuner/tuner/ppo/utils.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3083 2023-07-17 16:32:54.000000 llmtuner-0.1.0/src/llmtuner/tuner/ppo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:33:17.196834 llmtuner-0.1.0/src/llmtuner/tuner/pt/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-17 16:32:55.000000 llmtuner-0.1.0/src/llmtuner/tuner/pt/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2884 2023-07-17 16:32:55.000000 llmtuner-0.1.0/src/llmtuner/tuner/pt/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:33:17.216834 llmtuner-0.1.0/src/llmtuner/tuner/rm/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-17 16:32:55.000000 llmtuner-0.1.0/src/llmtuner/tuner/rm/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      722 2023-07-17 16:32:55.000000 llmtuner-0.1.0/src/llmtuner/tuner/rm/collator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-07-17 16:32:55.000000 llmtuner-0.1.0/src/llmtuner/tuner/rm/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1482 2023-07-17 16:32:55.000000 llmtuner-0.1.0/src/llmtuner/tuner/rm/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2854 2023-07-17 16:32:55.000000 llmtuner-0.1.0/src/llmtuner/tuner/rm/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:33:17.224834 llmtuner-0.1.0/src/llmtuner/tuner/sft/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-17 16:32:55.000000 llmtuner-0.1.0/src/llmtuner/tuner/sft/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2069 2023-07-17 16:32:55.000000 llmtuner-0.1.0/src/llmtuner/tuner/sft/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4162 2023-07-17 16:32:55.000000 llmtuner-0.1.0/src/llmtuner/tuner/sft/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4264 2023-07-17 16:32:55.000000 llmtuner-0.1.0/src/llmtuner/tuner/sft/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:33:17.244834 llmtuner-0.1.0/src/llmtuner/webui/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       48 2023-07-17 16:32:57.000000 llmtuner-0.1.0/src/llmtuner/webui/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2546 2023-07-17 16:32:55.000000 llmtuner-0.1.0/src/llmtuner/webui/chat.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2564 2023-07-17 16:32:56.000000 llmtuner-0.1.0/src/llmtuner/webui/common.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:33:17.268834 llmtuner-0.1.0/src/llmtuner/webui/components/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      234 2023-07-17 16:32:56.000000 llmtuner-0.1.0/src/llmtuner/webui/components/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1809 2023-07-17 16:32:56.000000 llmtuner-0.1.0/src/llmtuner/webui/components/chatbot.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      625 2023-07-17 16:32:56.000000 llmtuner-0.1.0/src/llmtuner/webui/components/data.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2227 2023-07-17 16:32:56.000000 llmtuner-0.1.0/src/llmtuner/webui/components/eval.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1389 2023-07-17 16:32:56.000000 llmtuner-0.1.0/src/llmtuner/webui/components/infer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3730 2023-07-17 16:32:56.000000 llmtuner-0.1.0/src/llmtuner/webui/components/sft.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1677 2023-07-17 16:32:56.000000 llmtuner-0.1.0/src/llmtuner/webui/components/top.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      387 2023-07-17 16:32:56.000000 llmtuner-0.1.0/src/llmtuner/webui/css.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1461 2023-07-17 16:32:57.000000 llmtuner-0.1.0/src/llmtuner/webui/interface.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     9155 2023-07-17 16:32:57.000000 llmtuner-0.1.0/src/llmtuner/webui/locales.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1224 2023-07-17 16:32:57.000000 llmtuner-0.1.0/src/llmtuner/webui/manager.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6820 2023-07-17 16:32:57.000000 llmtuner-0.1.0/src/llmtuner/webui/runner.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2606 2023-07-17 16:32:57.000000 llmtuner-0.1.0/src/llmtuner/webui/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 16:33:16.996834 llmtuner-0.1.0/src/llmtuner.egg-info/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    14082 2023-07-17 16:33:16.000000 llmtuner-0.1.0/src/llmtuner.egg-info/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2238 2023-07-17 16:33:16.000000 llmtuner-0.1.0/src/llmtuner.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-17 16:33:16.000000 llmtuner-0.1.0/src/llmtuner.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      198 2023-07-17 16:33:16.000000 llmtuner-0.1.0/src/llmtuner.egg-info/requires.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-17 16:33:16.000000 llmtuner-0.1.0/src/llmtuner.egg-info/top_level.txt
```

### Comparing `llmtuner-0.0.9/LICENSE` & `llmtuner-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/PKG-INFO` & `llmtuner-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.0.9
+Version: 0.1.0
 Summary: Easy-to-use fine-tuning framework using PEFT
 Home-page: https://github.com/hiyouga/LLaMA-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -20,24 +20,27 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LLaMA Efficient Tuning
 
-![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Efficient-Tuning?style=social)
-![GitHub Code License](https://img.shields.io/github/license/hiyouga/LLaMA-Efficient-Tuning)
-![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Efficient-Tuning)
-![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)
+[![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Efficient-Tuning?style=social)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/stargazers)
+[![GitHub Code License](https://img.shields.io/github/license/hiyouga/LLaMA-Efficient-Tuning)](LICENSE)
+[![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Efficient-Tuning)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/commits/main)
+[![PyPI](https://img.shields.io/pypi/v/llmtuner)](https://pypi.org/project/llmtuner/)
+[![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/pulls)
 
 👋 Join our [WeChat](assets/wechat.jpg).
 
 ## Changelog
 
-[23/07/11] Now we support training the **Baichuan-13B** model in this repo. Try `--model_name_or_path baichuan-inc/Baichuan-13B-Base`, `--padding_side right` and `--lora_target W_pack` arguments to train the Baichuan-13B model. Remember to use `--prompt_template baichuan` argument when you are using the Baichuan-13B-Chat model.
+[23/07/18] Now we develop an all-in-one Web UI for training, evaluation and inference. Try `train_web.py` to fine-tune models in your Web browser. Thank [@KanadeSiina](https://github.com/KanadeSiina) and [@codemayq](https://github.com/codemayq) for their efforts in the development.
+
+[23/07/11] Now we support training the **Baichuan-13B** model in this repo. Please replace the Baichuan-13B model file with `tests/modeling_baichuan.py` and try `--model_name_or_path path_to_baichuan_model` and `--lora_target W_pack` arguments to train the Baichuan-13B model. Remember to use `--prompt_template baichuan` argument when you are using the Baichuan-13B-Chat model.
 
 [23/07/09] Now we release [FastEdit](https://github.com/hiyouga/FastEdit)⚡🩹, an easy-to-use package for editing the factual knowledge of large language models efficiently. Please follow [FastEdit](https://github.com/hiyouga/FastEdit) if you are interested.
 
 [23/07/07] Now we support training the **InternLM-7B** model in this repo. Try `--model_name_or_path internlm/internlm-7b` argument to use the InternLM model. Remember to use `--prompt_template intern` argument when you are using the InternLM-chat model.
 
 [23/07/05] Now we support training the **Falcon-7B/40B** models in this repo. Try `--model_name_or_path tiiuae/falcon-7b` and `--lora_target query_key_value` arguments to use the Falcon model.
 
@@ -144,22 +147,18 @@
 git clone https://github.com/hiyouga/LLaMA-Efficient-Tuning.git
 conda create -n llama_etuning python=3.10
 conda activate llama_etuning
 cd LLaMA-Efficient-Tuning
 pip install -r requirements.txt
 ```
 
-### LLaMA Weights Preparation (optional)
-
-1. Download the weights of the LLaMA models.
-2. Convert them to HF format using the following command.
+### All-in-one Web UI
 
 ```bash
-python -m transformers.models.llama.convert_llama_weights_to_hf \
-    --input_dir path_to_llama_weights --model_size 7B --output_dir path_to_llama_model
+python src/train_web.py
 ```
 
 ### (Continually) Pre-Training
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage pt \
@@ -294,18 +293,28 @@
     --per_device_eval_batch_size 8 \
     --max_samples 50 \
     --predict_with_generate
 ```
 
 We recommend using `--per_device_eval_batch_size=1` and `--max_target_length 128` at 4/8-bit evaluation.
 
-### API / CLI / Web Demo
+### API Demo
+
+```bash
+python src/api_demo.py \
+    --model_name_or_path path_to_your_model \
+    --checkpoint_dir path_to_checkpoint
+```
+
+See `http://localhost:8000/docs` for API documentation.
+
+### CLI Demo
 
 ```bash
-python src/xxx_demo.py \
+python src/cli_demo.py \
     --model_name_or_path path_to_your_model \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Export model
 
 ```bash
```

### Comparing `llmtuner-0.0.9/README.md` & `llmtuner-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # LLaMA Efficient Tuning
 
-![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Efficient-Tuning?style=social)
-![GitHub Code License](https://img.shields.io/github/license/hiyouga/LLaMA-Efficient-Tuning)
-![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Efficient-Tuning)
-![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)
+[![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Efficient-Tuning?style=social)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/stargazers)
+[![GitHub Code License](https://img.shields.io/github/license/hiyouga/LLaMA-Efficient-Tuning)](LICENSE)
+[![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Efficient-Tuning)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/commits/main)
+[![PyPI](https://img.shields.io/pypi/v/llmtuner)](https://pypi.org/project/llmtuner/)
+[![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/pulls)
 
 👋 Join our [WeChat](assets/wechat.jpg).
 
 ## Changelog
 
-[23/07/11] Now we support training the **Baichuan-13B** model in this repo. Try `--model_name_or_path baichuan-inc/Baichuan-13B-Base`, `--padding_side right` and `--lora_target W_pack` arguments to train the Baichuan-13B model. Remember to use `--prompt_template baichuan` argument when you are using the Baichuan-13B-Chat model.
+[23/07/18] Now we develop an all-in-one Web UI for training, evaluation and inference. Try `train_web.py` to fine-tune models in your Web browser. Thank [@KanadeSiina](https://github.com/KanadeSiina) and [@codemayq](https://github.com/codemayq) for their efforts in the development.
+
+[23/07/11] Now we support training the **Baichuan-13B** model in this repo. Please replace the Baichuan-13B model file with `tests/modeling_baichuan.py` and try `--model_name_or_path path_to_baichuan_model` and `--lora_target W_pack` arguments to train the Baichuan-13B model. Remember to use `--prompt_template baichuan` argument when you are using the Baichuan-13B-Chat model.
 
 [23/07/09] Now we release [FastEdit](https://github.com/hiyouga/FastEdit)⚡🩹, an easy-to-use package for editing the factual knowledge of large language models efficiently. Please follow [FastEdit](https://github.com/hiyouga/FastEdit) if you are interested.
 
 [23/07/07] Now we support training the **InternLM-7B** model in this repo. Try `--model_name_or_path internlm/internlm-7b` argument to use the InternLM model. Remember to use `--prompt_template intern` argument when you are using the InternLM-chat model.
 
 [23/07/05] Now we support training the **Falcon-7B/40B** models in this repo. Try `--model_name_or_path tiiuae/falcon-7b` and `--lora_target query_key_value` arguments to use the Falcon model.
 
@@ -120,22 +123,18 @@
 git clone https://github.com/hiyouga/LLaMA-Efficient-Tuning.git
 conda create -n llama_etuning python=3.10
 conda activate llama_etuning
 cd LLaMA-Efficient-Tuning
 pip install -r requirements.txt
 ```
 
-### LLaMA Weights Preparation (optional)
-
-1. Download the weights of the LLaMA models.
-2. Convert them to HF format using the following command.
+### All-in-one Web UI
 
 ```bash
-python -m transformers.models.llama.convert_llama_weights_to_hf \
-    --input_dir path_to_llama_weights --model_size 7B --output_dir path_to_llama_model
+python src/train_web.py
 ```
 
 ### (Continually) Pre-Training
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage pt \
@@ -270,18 +269,28 @@
     --per_device_eval_batch_size 8 \
     --max_samples 50 \
     --predict_with_generate
 ```
 
 We recommend using `--per_device_eval_batch_size=1` and `--max_target_length 128` at 4/8-bit evaluation.
 
-### API / CLI / Web Demo
+### API Demo
+
+```bash
+python src/api_demo.py \
+    --model_name_or_path path_to_your_model \
+    --checkpoint_dir path_to_checkpoint
+```
+
+See `http://localhost:8000/docs` for API documentation.
+
+### CLI Demo
 
 ```bash
-python src/xxx_demo.py \
+python src/cli_demo.py \
     --model_name_or_path path_to_your_model \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Export model
 
 ```bash
```

### Comparing `llmtuner-0.0.9/setup.py` & `llmtuner-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner/api/protocol.py` & `llmtuner-0.1.0/src/llmtuner/api/protocol.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner/dsets/callbacks.py` & `llmtuner-0.1.0/src/llmtuner/dsets/callbacks.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner/dsets/loader.py` & `llmtuner-0.1.0/src/llmtuner/dsets/loader.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner/dsets/preprocess.py` & `llmtuner-0.1.0/src/llmtuner/dsets/preprocess.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner/extras/callbacks.py` & `llmtuner-0.1.0/src/llmtuner/extras/callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from transformers.training_args import TrainingArguments
 
 
 class LogCallback(TrainerCallback):
 
     def __init__(self, runner=None):
         self.runner = runner
+        self.start_time = time.time()
         self.tracker = {}
 
     def on_train_begin(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
         r"""
         Event called at the beginning of training.
         """
         self.start_time = time.time()
@@ -42,16 +43,14 @@
             control.should_epoch_stop = True
             control.should_training_stop = True
 
     def on_log(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs) -> None:
         r"""
         Event called after logging the last logs.
         """
-        if "step" not in state.log_history[-1]:
-            return
         cur_time = time.time()
         cur_steps = state.log_history[-1].get("step")
         elapsed_time = cur_time - self.start_time
         avg_time_per_step = elapsed_time / cur_steps if cur_steps != 0 else 0
         remaining_steps = state.max_steps - cur_steps
         remaining_time = remaining_steps * avg_time_per_step
         self.tracker = {
```

### Comparing `llmtuner-0.0.9/src/llmtuner/extras/misc.py` & `llmtuner-0.1.0/src/llmtuner/extras/misc.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner/extras/ploting.py` & `llmtuner-0.1.0/src/llmtuner/extras/ploting.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import os
+import math
 import json
 import matplotlib.pyplot as plt
 from typing import List, Optional
 from transformers.trainer import TRAINER_STATE_NAME
 
 from llmtuner.extras.logging import get_logger
 
 
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

### Comparing `llmtuner-0.0.9/src/llmtuner/extras/save_and_load.py` & `llmtuner-0.1.0/src/llmtuner/extras/save_and_load.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner/hparams/data_args.py` & `llmtuner-0.1.0/src/llmtuner/hparams/data_args.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 @dataclass
 class DataArguments:
     """
     Arguments pertaining to what data we are going to input our model for training and evaluation.
     """
     dataset: Optional[str] = field(
         default="alpaca_zh",
-        metadata={"help": "The name of provided dataset(s) to use. Use comma to separate multiple datasets."}
+        metadata={"help": "The name of provided dataset(s) to use. Use commas to separate multiple datasets."}
     )
     dataset_dir: Optional[str] = field(
         default="data",
         metadata={"help": "The name of the folder containing datasets."}
     )
     split: Optional[str] = field(
         default="train",
```

### Comparing `llmtuner-0.0.9/src/llmtuner/hparams/finetuning_args.py` & `llmtuner-0.1.0/src/llmtuner/hparams/finetuning_args.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     )
     lora_dropout: Optional[float] = field(
         default=0.1,
         metadata={"help": "Dropout rate for the LoRA fine-tuning."}
     )
     lora_target: Optional[str] = field(
         default="q_proj,v_proj",
-        metadata={"help": "Name(s) of target modules to apply LoRA. Use comma to separate multiple modules. \
+        metadata={"help": "Name(s) of target modules to apply LoRA. Use commas to separate multiple modules. \
                   LLaMA choices: [\"q_proj\", \"k_proj\", \"v_proj\", \"o_proj\", \"gate_proj\", \"up_proj\", \"down_proj\"], \
                   BLOOM & Falcon choices: [\"query_key_value\", \"self_attention.dense\", \"mlp.dense\"], \
                   Baichuan choices: [\"W_pack\", \"o_proj\", \"gate_proj\", \"up_proj\", \"down_proj\"]"}
     )
 
     def __post_init__(self):
         if isinstance(self.lora_target, str): # support custom target modules/layers of LoRA
```

### Comparing `llmtuner-0.0.9/src/llmtuner/hparams/generating_args.py` & `llmtuner-0.1.0/src/llmtuner/hparams/generating_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner/hparams/model_args.py` & `llmtuner-0.1.0/src/llmtuner/hparams/model_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner/tuner/core/adapter.py` & `llmtuner-0.1.0/src/llmtuner/tuner/core/adapter.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner/tuner/core/loader.py` & `llmtuner-0.1.0/src/llmtuner/tuner/core/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     AutoConfig,
     AutoModelForCausalLM,
     AutoTokenizer,
     BitsAndBytesConfig
 )
 from transformers.utils import check_min_version
 from transformers.utils.versions import require_version
-from transformers.modeling_utils import PreTrainedModel
-from transformers.tokenization_utils import PreTrainedTokenizer
+from transformers.modeling_utils import PretrainedConfig, PreTrainedModel
+from transformers.tokenization_utils import PreTrainedTokenizerBase
 from trl import AutoModelForCausalLMWithValueHead
 
 from llmtuner.extras.logging import get_logger
 from llmtuner.extras.misc import prepare_model_for_training, print_trainable_params
 from llmtuner.extras.save_and_load import load_valuehead_params
 from llmtuner.hparams import ModelArguments, FinetuningArguments
 from llmtuner.tuner.core.adapter import init_adapter
@@ -24,23 +24,23 @@
 logger = get_logger(__name__)
 
 
 check_min_version("4.29.1")
 require_version("datasets>=2.12.0", "To fix: pip install datasets>=2.12.0")
 require_version("accelerate>=0.19.0", "To fix: pip install accelerate>=0.19.0")
 require_version("peft>=0.3.0", "To fix: pip install peft>=0.3.0")
-require_version("trl>=0.4.4", "To fix: pip install trl>=0.4.4")
+require_version("trl>=0.4.7", "To fix: pip install trl>=0.4.7")
 
 
 def load_model_and_tokenizer(
     model_args: ModelArguments,
     finetuning_args: FinetuningArguments,
     is_trainable: Optional[bool] = False,
     stage: Optional[Literal["pt", "sft", "rm", "ppo"]] = "sft"
-) -> Tuple[PreTrainedModel, PreTrainedTokenizer]:
+) -> Tuple[PreTrainedModel, PreTrainedTokenizerBase]:
     r"""
     Loads pretrained model and tokenizer.
 
     Support both training and inference.
     """
     if (not is_trainable) and model_args.checkpoint_dir is None:
         logger.warning("Checkpoint is not found at evaluation, load the original model.")
@@ -109,20 +109,20 @@
         config=config,
         torch_dtype=torch.bfloat16 if model_args.compute_dtype == torch.bfloat16 else torch.float16,
         low_cpu_mem_usage=True,
         **config_kwargs
     )
 
     # Register auto class to save the custom code files.
-    if hasattr(config, "auto_map") and "AutoConfig" in config.auto_map:
+    if isinstance(config, PretrainedConfig) and "AutoConfig" in getattr(config, "auto_map", {}):
         config.__class__.register_for_auto_class()
-    if hasattr(config, "auto_map") and "AutoTokenizer" in config.auto_map:
-        tokenizer.__class__.register_for_auto_class()
-    if hasattr(config, "auto_map") and "AutoModelForCausalLM" in config.auto_map:
+    if isinstance(model, PreTrainedModel) and "AutoModelForCausalLM" in getattr(config, "auto_map", {}):
         model.__class__.register_for_auto_class()
+    if isinstance(tokenizer, PreTrainedTokenizerBase) and "AutoTokenizer" in tokenizer.init_kwargs.get("auto_map", {}):
+        tokenizer.__class__.register_for_auto_class()
 
     # Initialize adapters
     model = prepare_model_for_training(model, finetuning_args.finetuning_type) if is_trainable else model
     model = init_adapter(model, model_args, finetuning_args, is_trainable, is_mergeable)
 
     if stage == "rm" or stage == "ppo": # add value head
         model = AutoModelForCausalLMWithValueHead.from_pretrained(model)
```

### Comparing `llmtuner-0.0.9/src/llmtuner/tuner/core/parser.py` & `llmtuner-0.1.0/src/llmtuner/tuner/core/parser.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner/tuner/core/trainer.py` & `llmtuner-0.1.0/src/llmtuner/tuner/core/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner/tuner/ppo/trainer.py` & `llmtuner-0.1.0/src/llmtuner/tuner/ppo/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 logger = get_logger(__name__)
 
 
 class PPOPeftTrainer(PPOTrainer, PeftTrainer):
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
@@ -42,121 +41,112 @@
         self.data_collator = self.accelerator.prepare(kwargs["data_collator"]) # override the data collator of PPOTrainer
         self._remove_log()
 
     def ppo_train(self, max_target_length: int) -> None:
         r"""
         Implements training loop for the PPO stage, like _inner_training_loop() in Huggingface's Trainer.
         """
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
-
-                unwrapped_model.gradient_checkpointing_disable()
-                unwrapped_model.config.use_cache = True
-
-                # Get response from model
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
+            unwrapped_model.gradient_checkpointing_disable()
+            unwrapped_model.config.use_cache = True
 
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
-                rewards = [reward for reward in values[:, -1].to(torch.float32)] # use float32 type
-                replace_model(unwrapped_model, target="default") # make sure the model is default at the end
+            rewards = [reward for reward in values[-1].to(torch.float32)] # use float32 type
+            replace_model(unwrapped_model, target="default")
 
-                # Run PPO step
-                unwrapped_model.gradient_checkpointing_enable()
-                unwrapped_model.config.use_cache = False
+            # Run PPO step
+            unwrapped_model.gradient_checkpointing_enable()
+            unwrapped_model.config.use_cache = False
+            stats = self.step(queries, responses, rewards)
 
-                stats = self.step(queries, responses, rewards)
-
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
```

### Comparing `llmtuner-0.0.9/src/llmtuner/tuner/ppo/utils.py` & `llmtuner-0.1.0/src/llmtuner/tuner/ppo/utils.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner/tuner/ppo/workflow.py` & `llmtuner-0.1.0/src/llmtuner/tuner/ppo/workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 # Inspired by:
 # https://github.com/lvwerra/trl/blob/main/examples/sentiment/scripts/gpt-neox-20b_peft/gpt-neo-20b_sentiment_peft.py
 
 import math
 from trl import PPOConfig
 from torch.optim import AdamW
-from transformers import DataCollatorForSeq2Seq, Seq2SeqTrainingArguments
+from typing import Optional, List
+from transformers import DataCollatorForSeq2Seq, Seq2SeqTrainingArguments, TrainerCallback
 from transformers.optimization import get_scheduler
 
 from llmtuner.dsets import get_dataset, preprocess_dataset
 from llmtuner.extras.callbacks import LogCallback
 from llmtuner.extras.ploting import plot_loss
 from llmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments
 from llmtuner.tuner.core import load_model_and_tokenizer
 from llmtuner.tuner.ppo.trainer import PPOPeftTrainer
 
 
 def run_ppo(
     model_args: ModelArguments,
     data_args: DataArguments,
     training_args: Seq2SeqTrainingArguments,
-    finetuning_args: FinetuningArguments
+    finetuning_args: FinetuningArguments,
+    callbacks: Optional[List[TrainerCallback]] = [LogCallback()]
 ):
     dataset = get_dataset(model_args, data_args)
     model, tokenizer = load_model_and_tokenizer(model_args, finetuning_args, training_args.do_train, stage="ppo")
     dataset = preprocess_dataset(dataset, tokenizer, data_args, training_args, stage="ppo")
     data_collator = DataCollatorForSeq2Seq(tokenizer=tokenizer, label_pad_token_id=tokenizer.pad_token_id)
 
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
@@ -46,15 +48,15 @@
         num_training_steps=(training_args.num_train_epochs * math.ceil(len(dataset) / total_train_batch_size))
     )
 
     # Initialize our Trainer
     ppo_trainer = PPOPeftTrainer(
         training_args=training_args,
         finetuning_args=finetuning_args,
-        callbacks=[LogCallback()],
+        callbacks=callbacks,
         config=ppo_config,
         model=model,
         ref_model=None,
         tokenizer=tokenizer,
         dataset=dataset,
         data_collator=data_collator,
         optimizer=optimizer,
```

### Comparing `llmtuner-0.0.9/src/llmtuner/tuner/pt/workflow.py` & `llmtuner-0.1.0/src/llmtuner/tuner/pt/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner/tuner/rm/collator.py` & `llmtuner-0.1.0/src/llmtuner/tuner/rm/collator.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner/tuner/rm/trainer.py` & `llmtuner-0.1.0/src/llmtuner/tuner/rm/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner/tuner/rm/workflow.py` & `llmtuner-0.1.0/src/llmtuner/tuner/rm/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Inspired by:
 # https://github.com/lvwerra/trl/blob/main/examples/summarization/scripts/reward_summarization.py
 # https://github.com/CarperAI/trlx/blob/main/examples/summarize_rlhf/reward_model/train_reward_model_gptj.py
 
-from transformers import Seq2SeqTrainingArguments
+from typing import Optional, List
+from transformers import Seq2SeqTrainingArguments, TrainerCallback
 
 from llmtuner.dsets import get_dataset, preprocess_dataset
 from llmtuner.extras.callbacks import LogCallback
 from llmtuner.extras.ploting import plot_loss
 from llmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments
 from llmtuner.tuner.core import load_model_and_tokenizer
 from llmtuner.tuner.rm.metric import compute_accuracy
@@ -14,15 +15,16 @@
 from llmtuner.tuner.rm.trainer import PairwisePeftTrainer
 
 
 def run_rm(
     model_args: ModelArguments,
     data_args: DataArguments,
     training_args: Seq2SeqTrainingArguments,
-    finetuning_args: FinetuningArguments
+    finetuning_args: FinetuningArguments,
+    callbacks: Optional[List[TrainerCallback]] = [LogCallback()]
 ):
     dataset = get_dataset(model_args, data_args)
     model, tokenizer = load_model_and_tokenizer(model_args, finetuning_args, training_args.do_train, stage="rm")
     dataset = preprocess_dataset(dataset, tokenizer, data_args, training_args, stage="rm")
     data_collator = PairwiseDataCollatorWithPadding(tokenizer)
 
     training_args.remove_unused_columns = False # important for pairwise dataset
@@ -40,15 +42,15 @@
     # Initialize our Trainer
     trainer = PairwisePeftTrainer(
         finetuning_args=finetuning_args,
         model=model,
         args=training_args,
         tokenizer=tokenizer,
         data_collator=data_collator,
-        callbacks=[LogCallback()],
+        callbacks=callbacks,
         compute_metrics=compute_accuracy,
         **trainer_kwargs
     )
 
     # Training
     if training_args.do_train:
         train_result = trainer.train()
```

### Comparing `llmtuner-0.0.9/src/llmtuner/tuner/sft/metric.py` & `llmtuner-0.1.0/src/llmtuner/tuner/sft/metric.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner/tuner/sft/trainer.py` & `llmtuner-0.1.0/src/llmtuner/tuner/sft/trainer.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,25 +28,48 @@
     ) -> Tuple[Optional[float], Optional[torch.Tensor], Optional[torch.Tensor]]:
         r"""
         Removes the prompt part in the generated tokens.
 
         Subclass and override to inject custom behavior.
         """
         prompt_len, label_len = inputs["input_ids"].size(-1), inputs["labels"].size(-1)
-        if self.tokenizer.padding_side == "right": # pads the labels to the same length as the inputs
-            inputs["labels"] = torch.cat((inputs["labels"], torch.zeros_like(inputs["input_ids"])[:, label_len:]), dim=-1)
-        else:
-            inputs["labels"] = torch.cat((torch.zeros_like(inputs["input_ids"])[:, label_len:], inputs["labels"]), dim=-1)
+        if prompt_len > label_len:
+            inputs["labels"] = self._pad_tensors_to_target_len(inputs["labels"], inputs["input_ids"])
+        if label_len > prompt_len:
+            inputs["input_ids"] = self._pad_tensors_to_target_len(inputs["input_ids"], inputs["labels"])
+
         loss, generated_tokens, labels = super().prediction_step(
             model, inputs, prediction_loss_only=prediction_loss_only, ignore_keys=ignore_keys
         )
-        generated_tokens = generated_tokens[:, prompt_len:] if generated_tokens is not None else None
+        generated_tokens = generated_tokens[:, max(prompt_len, label_len):] if generated_tokens is not None else None
 
         return (loss, generated_tokens, labels)
 
+    def _pad_tensors_to_target_len(self, src_tensor: torch.Tensor, tgt_tensor: torch.Tensor) -> torch.Tensor:
+        r"""
+        Pads the tensor to the same length as the target tensor.
+
+        Should only be called when predict_with_generate=True.
+        """
+        if self.tokenizer is not None and hasattr(self.tokenizer, "pad_token_id"):
+            assert self.tokenizer.padding_side == "left", "This method only accepts left-padded tensor."
+            # If PAD token is not defined at least EOS token has to be defined
+            pad_token_id = (
+                self.tokenizer.pad_token_id if self.tokenizer.pad_token_id is not None else self.tokenizer.eos_token_id
+            )
+        else:
+            if self.model.config.pad_token_id is not None:
+                pad_token_id = self.model.config.pad_token_id
+            else:
+                raise ValueError("Pad_token_id must be set in the configuration of the model, in order to pad tensors")
+
+        padded_tensor = pad_token_id * torch.ones_like(tgt_tensor)
+        padded_tensor[:, -src_tensor.shape[-1]:] = src_tensor # adopt left-padding
+        return padded_tensor
+
     def save_predictions(
         self,
         predict_results: PredictionOutput
     ) -> None:
         r"""
         Saves model predictions to `output_dir`.
```

### Comparing `llmtuner-0.0.9/src/llmtuner/tuner/sft/workflow.py` & `llmtuner-0.1.0/src/llmtuner/tuner/sft/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.0.9/src/llmtuner.egg-info/PKG-INFO` & `llmtuner-0.1.0/src/llmtuner.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.0.9
+Version: 0.1.0
 Summary: Easy-to-use fine-tuning framework using PEFT
 Home-page: https://github.com/hiyouga/LLaMA-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -20,24 +20,27 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LLaMA Efficient Tuning
 
-![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Efficient-Tuning?style=social)
-![GitHub Code License](https://img.shields.io/github/license/hiyouga/LLaMA-Efficient-Tuning)
-![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Efficient-Tuning)
-![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)
+[![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Efficient-Tuning?style=social)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/stargazers)
+[![GitHub Code License](https://img.shields.io/github/license/hiyouga/LLaMA-Efficient-Tuning)](LICENSE)
+[![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Efficient-Tuning)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/commits/main)
+[![PyPI](https://img.shields.io/pypi/v/llmtuner)](https://pypi.org/project/llmtuner/)
+[![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/pulls)
 
 👋 Join our [WeChat](assets/wechat.jpg).
 
 ## Changelog
 
-[23/07/11] Now we support training the **Baichuan-13B** model in this repo. Try `--model_name_or_path baichuan-inc/Baichuan-13B-Base`, `--padding_side right` and `--lora_target W_pack` arguments to train the Baichuan-13B model. Remember to use `--prompt_template baichuan` argument when you are using the Baichuan-13B-Chat model.
+[23/07/18] Now we develop an all-in-one Web UI for training, evaluation and inference. Try `train_web.py` to fine-tune models in your Web browser. Thank [@KanadeSiina](https://github.com/KanadeSiina) and [@codemayq](https://github.com/codemayq) for their efforts in the development.
+
+[23/07/11] Now we support training the **Baichuan-13B** model in this repo. Please replace the Baichuan-13B model file with `tests/modeling_baichuan.py` and try `--model_name_or_path path_to_baichuan_model` and `--lora_target W_pack` arguments to train the Baichuan-13B model. Remember to use `--prompt_template baichuan` argument when you are using the Baichuan-13B-Chat model.
 
 [23/07/09] Now we release [FastEdit](https://github.com/hiyouga/FastEdit)⚡🩹, an easy-to-use package for editing the factual knowledge of large language models efficiently. Please follow [FastEdit](https://github.com/hiyouga/FastEdit) if you are interested.
 
 [23/07/07] Now we support training the **InternLM-7B** model in this repo. Try `--model_name_or_path internlm/internlm-7b` argument to use the InternLM model. Remember to use `--prompt_template intern` argument when you are using the InternLM-chat model.
 
 [23/07/05] Now we support training the **Falcon-7B/40B** models in this repo. Try `--model_name_or_path tiiuae/falcon-7b` and `--lora_target query_key_value` arguments to use the Falcon model.
 
@@ -144,22 +147,18 @@
 git clone https://github.com/hiyouga/LLaMA-Efficient-Tuning.git
 conda create -n llama_etuning python=3.10
 conda activate llama_etuning
 cd LLaMA-Efficient-Tuning
 pip install -r requirements.txt
 ```
 
-### LLaMA Weights Preparation (optional)
-
-1. Download the weights of the LLaMA models.
-2. Convert them to HF format using the following command.
+### All-in-one Web UI
 
 ```bash
-python -m transformers.models.llama.convert_llama_weights_to_hf \
-    --input_dir path_to_llama_weights --model_size 7B --output_dir path_to_llama_model
+python src/train_web.py
 ```
 
 ### (Continually) Pre-Training
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage pt \
@@ -294,18 +293,28 @@
     --per_device_eval_batch_size 8 \
     --max_samples 50 \
     --predict_with_generate
 ```
 
 We recommend using `--per_device_eval_batch_size=1` and `--max_target_length 128` at 4/8-bit evaluation.
 
-### API / CLI / Web Demo
+### API Demo
+
+```bash
+python src/api_demo.py \
+    --model_name_or_path path_to_your_model \
+    --checkpoint_dir path_to_checkpoint
+```
+
+See `http://localhost:8000/docs` for API documentation.
+
+### CLI Demo
 
 ```bash
-python src/xxx_demo.py \
+python src/cli_demo.py \
     --model_name_or_path path_to_your_model \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Export model
 
 ```bash
```

### Comparing `llmtuner-0.0.9/src/llmtuner.egg-info/SOURCES.txt` & `llmtuner-0.1.0/src/llmtuner.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 src/llmtuner.egg-info/SOURCES.txt
 src/llmtuner.egg-info/dependency_links.txt
 src/llmtuner.egg-info/requires.txt
 src/llmtuner.egg-info/top_level.txt
 src/llmtuner/api/__init__.py
 src/llmtuner/api/app.py
 src/llmtuner/api/protocol.py
+src/llmtuner/chat/__init__.py
+src/llmtuner/chat/stream_chat.py
 src/llmtuner/dsets/__init__.py
 src/llmtuner/dsets/callbacks.py
 src/llmtuner/dsets/loader.py
 src/llmtuner/dsets/preprocess.py
 src/llmtuner/extras/__init__.py
 src/llmtuner/extras/callbacks.py
 src/llmtuner/extras/constants.py
@@ -45,8 +47,24 @@
 src/llmtuner/tuner/rm/collator.py
 src/llmtuner/tuner/rm/metric.py
 src/llmtuner/tuner/rm/trainer.py
 src/llmtuner/tuner/rm/workflow.py
 src/llmtuner/tuner/sft/__init__.py
 src/llmtuner/tuner/sft/metric.py
 src/llmtuner/tuner/sft/trainer.py
-src/llmtuner/tuner/sft/workflow.py
+src/llmtuner/tuner/sft/workflow.py
+src/llmtuner/webui/__init__.py
+src/llmtuner/webui/chat.py
+src/llmtuner/webui/common.py
+src/llmtuner/webui/css.py
+src/llmtuner/webui/interface.py
+src/llmtuner/webui/locales.py
+src/llmtuner/webui/manager.py
+src/llmtuner/webui/runner.py
+src/llmtuner/webui/utils.py
+src/llmtuner/webui/components/__init__.py
+src/llmtuner/webui/components/chatbot.py
+src/llmtuner/webui/components/data.py
+src/llmtuner/webui/components/eval.py
+src/llmtuner/webui/components/infer.py
+src/llmtuner/webui/components/sft.py
+src/llmtuner/webui/components/top.py
```

