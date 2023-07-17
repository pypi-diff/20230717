# Comparing `tmp/llm-toys-0.1.0.tar.gz` & `tmp/llm-toys-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-toys-0.1.0.tar", last modified: Mon Jul 17 11:24:36 2023, max compression
+gzip compressed data, was "llm-toys-0.1.1.tar", last modified: Mon Jul 17 11:27:36 2023, max compression
```

## Comparing `llm-toys-0.1.0.tar` & `llm-toys-0.1.1.tar`

### file list

```diff
@@ -1,1628 +1,1628 @@
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:36.012431 llm-toys-0.1.0/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6908 2023-07-17 11:24:36.012431 llm-toys-0.1.0/PKG-INFO
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6545 2023-07-17 11:03:23.000000 llm-toys-0.1.0/README.md
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.848430 llm-toys-0.1.0/llm_toys/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      518 2023-07-17 11:24:23.000000 llm-toys-0.1.0/llm_toys/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1762 2023-07-17 10:05:14.000000 llm-toys-0.1.0/llm_toys/config.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3879 2023-07-17 09:13:47.000000 llm-toys-0.1.0/llm_toys/eval.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.848430 llm-toys-0.1.0/llm_toys/hf/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 14:32:56.000000 llm-toys-0.1.0/llm_toys/hf/__init__.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.848430 llm-toys-0.1.0/llm_toys/hf/peft/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2163 2023-07-15 14:04:38.000000 llm-toys-0.1.0/llm_toys/hf/peft/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5535 2023-07-15 14:04:38.000000 llm-toys-0.1.0/llm_toys/hf/peft/auto.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      877 2023-07-15 14:04:38.000000 llm-toys-0.1.0/llm_toys/hf/peft/import_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3224 2023-07-15 14:04:38.000000 llm-toys-0.1.0/llm_toys/hf/peft/mapping.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    74724 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/peft/peft_model.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.852430 llm-toys-0.1.0/llm_toys/hf/peft/tuners/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1217 2023-07-15 14:04:38.000000 llm-toys-0.1.0/llm_toys/hf/peft/tuners/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    33370 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/peft/tuners/adalora.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16325 2023-07-15 14:04:38.000000 llm-toys-0.1.0/llm_toys/hf/peft/tuners/adaption_prompt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    22782 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/peft/tuners/ia3.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    48122 2023-07-15 14:04:38.000000 llm-toys-0.1.0/llm_toys/hf/peft/tuners/lora.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6755 2023-07-15 14:04:38.000000 llm-toys-0.1.0/llm_toys/hf/peft/tuners/p_tuning.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3785 2023-07-15 14:04:38.000000 llm-toys-0.1.0/llm_toys/hf/peft/tuners/prefix_tuning.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4935 2023-07-15 14:04:38.000000 llm-toys-0.1.0/llm_toys/hf/peft/tuners/prompt_tuning.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.852430 llm-toys-0.1.0/llm_toys/hf/peft/utils/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1734 2023-07-15 14:04:38.000000 llm-toys-0.1.0/llm_toys/hf/peft/utils/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8845 2023-07-15 14:04:38.000000 llm-toys-0.1.0/llm_toys/hf/peft/utils/config.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1118 2023-07-15 14:04:38.000000 llm-toys-0.1.0/llm_toys/hf/peft/utils/hub_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13087 2023-07-15 14:04:38.000000 llm-toys-0.1.0/llm_toys/hf/peft/utils/other.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6098 2023-07-15 14:04:38.000000 llm-toys-0.1.0/llm_toys/hf/peft/utils/save_and_load.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.860430 llm-toys-0.1.0/llm_toys/hf/transformers/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   279202 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8783 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/activations.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4313 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/activations_tf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    30854 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/audio_utils.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.860430 llm-toys-0.1.0/llm_toys/hf/transformers/benchmark/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/benchmark/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10752 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/benchmark/benchmark.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3890 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/benchmark/benchmark_args.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4735 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/benchmark/benchmark_args_tf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6475 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/benchmark/benchmark_args_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13251 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/benchmark/benchmark_tf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    37600 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/benchmark/benchmark_utils.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.860430 llm-toys-0.1.0/llm_toys/hf/transformers/commands/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      923 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/commands/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11062 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/commands/add_new_model.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    70769 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/commands/add_new_model_like.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7852 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/commands/convert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2373 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/commands/download.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5316 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/commands/env.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8001 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/commands/lfs.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20540 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/commands/pt_to_tf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4249 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/commands/run.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8026 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/commands/serving.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6307 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/commands/train.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2047 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/commands/transformers_cli.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7124 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/commands/user.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    51951 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/configuration_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20903 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/convert_graph_to_onnx.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    16631 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/convert_pytorch_checkpoint_to_tf2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    52391 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/convert_slow_tokenizer.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     4982 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/convert_slow_tokenizers_checkpoints_to_fast.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2899 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/convert_tf_hub_seq_to_seq_bert_to_pytorch.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.860430 llm-toys-0.1.0/llm_toys/hf/transformers/data/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1423 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/data/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    76822 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/data/data_collator.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.864430 llm-toys-0.1.0/llm_toys/hf/transformers/data/datasets/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      909 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/data/datasets/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6149 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/data/datasets/glue.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23675 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/data/datasets/language_modeling.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9205 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/data/datasets/squad.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.864430 llm-toys-0.1.0/llm_toys/hf/transformers/data/metrics/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3632 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/data/metrics/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    29676 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/data/metrics/squad_metrics.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.864430 llm-toys-0.1.0/llm_toys/hf/transformers/data/processors/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1014 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/data/processors/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23219 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/data/processors/glue.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    33153 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/data/processors/squad.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13829 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/data/processors/utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3489 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/data/processors/xnli.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12907 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/debug_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16966 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/deepspeed.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2115 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/dependency_versions_check.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3167 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/dependency_versions_table.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24465 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/dynamic_module_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18215 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/feature_extraction_sequence_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28136 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/feature_extraction_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3574 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/file_utils.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.864430 llm-toys-0.1.0/llm_toys/hf/transformers/generation/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9515 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/generation/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19089 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/generation/beam_constraints.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    45955 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/generation/beam_search.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40270 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/generation/configuration_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19218 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/generation/flax_logits_process.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    49014 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/generation/flax_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    54715 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/generation/logits_process.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6373 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/generation/stopping_criteria.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9145 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/generation/streamers.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28136 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/generation/tf_logits_process.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   177842 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/generation/tf_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   251955 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/generation/utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1118 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/generation_flax_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1109 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/generation_tf_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1126 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/generation_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19745 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/hf_argparser.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4161 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/hyperparameter_search.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    26885 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/image_processing_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    30960 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/image_transforms.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24006 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/image_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    71566 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/integrations.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20843 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/keras_callbacks.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    35232 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/modelcard.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    41961 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/modeling_flax_outputs.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19529 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/modeling_flax_pytorch_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    56460 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/modeling_flax_utils.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   106127 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/modeling_outputs.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    56074 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/modeling_tf_outputs.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24772 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/modeling_tf_pytorch_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   160782 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/modeling_tf_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   191059 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/modeling_utils.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.864430 llm-toys-0.1.0/llm_toys/hf/transformers/models/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3559 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/__init__.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.868430 llm-toys-0.1.0/llm_toys/hf/transformers/models/albert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5482 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/albert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8568 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/albert/configuration_albert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2162 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/albert/convert_albert_original_tf_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    60616 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/albert/modeling_albert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40772 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/albert/modeling_flax_albert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    61857 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/albert/modeling_tf_albert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15429 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/albert/tokenization_albert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10815 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/albert/tokenization_albert_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.868430 llm-toys-0.1.0/llm_toys/hf/transformers/models/align/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2064 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/align/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18805 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/align/configuration_align.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15524 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/align/convert_align_tf_to_hf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    72060 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/align/modeling_align.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6216 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/align/processing_align.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.868430 llm-toys-0.1.0/llm_toys/hf/transformers/models/altclip/
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2126 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/altclip/__init__.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    19664 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/altclip/configuration_altclip.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    78788 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/altclip/modeling_altclip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6477 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/altclip/processing_altclip.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.868430 llm-toys-0.1.0/llm_toys/hf/transformers/models/audio_spectrogram_transformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2507 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/audio_spectrogram_transformer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5650 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/audio_spectrogram_transformer/configuration_audio_spectrogram_transformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11052 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/audio_spectrogram_transformer/convert_audio_spectrogram_transformer_original_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8614 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/audio_spectrogram_transformer/feature_extraction_audio_spectrogram_transformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    26449 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/audio_spectrogram_transformer/modeling_audio_spectrogram_transformer.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.868430 llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15846 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40272 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/auto_factory.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    44362 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/configuration_auto.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18500 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/feature_extraction_auto.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19917 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/image_processing_auto.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    57917 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/modeling_auto.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14128 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/modeling_flax_auto.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    27835 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/modeling_tf_auto.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15201 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/processing_auto.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    39830 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/tokenization_auto.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.868430 llm-toys-0.1.0/llm_toys/hf/transformers/models/autoformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1914 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/autoformer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12325 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/autoformer/configuration_autoformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   109505 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/autoformer/modeling_autoformer.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.872430 llm-toys-0.1.0/llm_toys/hf/transformers/models/bart/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4333 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bart/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18993 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bart/configuration_bart.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6055 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bart/convert_bart_original_pytorch_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    90105 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bart/modeling_bart.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    82723 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bart/modeling_flax_bart.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    74717 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bart/modeling_tf_bart.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17981 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bart/tokenization_bart.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13812 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bart/tokenization_bart_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.872430 llm-toys-0.1.0/llm_toys/hf/transformers/models/barthez/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1848 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/barthez/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13193 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/barthez/tokenization_barthez.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8900 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/barthez/tokenization_barthez_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.872430 llm-toys-0.1.0/llm_toys/hf/transformers/models/bartpho/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1362 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bartpho/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14219 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bartpho/tokenization_bartpho.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.872430 llm-toys-0.1.0/llm_toys/hf/transformers/models/beit/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3289 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/beit/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9641 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/beit/configuration_beit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16480 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/beit/convert_beit_unilm_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1172 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/beit/feature_extraction_beit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24407 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/beit/image_processing_beit.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    54268 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/beit/modeling_beit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    36989 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/beit/modeling_flax_beit.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.872430 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6057 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10150 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/configuration_bert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10490 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/convert_bert_original_tf2_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2159 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/convert_bert_original_tf_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4098 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/convert_bert_pytorch_checkpoint_to_original_tf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7606 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/convert_bert_token_dropping_original_tf2_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    83947 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/modeling_bert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    63604 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/modeling_flax_bert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    85690 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/modeling_tf_bert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    25078 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/tokenization_bert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14871 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/tokenization_bert_fast.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11798 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/tokenization_bert_tf.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.876430 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert_generation/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2275 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert_generation/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6228 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert_generation/configuration_bert_generation.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    47874 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert_generation/modeling_bert_generation.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7140 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert_generation/tokenization_bert_generation.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.876430 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert_japanese/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1053 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert_japanese/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40187 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bert_japanese/tokenization_bert_japanese.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.876430 llm-toys-0.1.0/llm_toys/hf/transformers/models/bertweet/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      959 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bertweet/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    27220 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bertweet/tokenization_bertweet.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.876430 llm-toys-0.1.0/llm_toys/hf/transformers/models/big_bird/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4574 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/big_bird/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8306 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/big_bird/configuration_big_bird.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2493 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/big_bird/convert_bigbird_original_tf_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   142285 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/big_bird/modeling_big_bird.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   109507 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/big_bird/modeling_flax_big_bird.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14885 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/big_bird/tokenization_big_bird.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11355 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/big_bird/tokenization_big_bird_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.876430 llm-toys-0.1.0/llm_toys/hf/transformers/models/bigbird_pegasus/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2316 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bigbird_pegasus/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19802 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bigbird_pegasus/configuration_bigbird_pegasus.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6288 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bigbird_pegasus/convert_bigbird_pegasus_tf_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   147915 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bigbird_pegasus/modeling_bigbird_pegasus.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.876430 llm-toys-0.1.0/llm_toys/hf/transformers/models/biogpt/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2058 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/biogpt/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6390 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/biogpt/configuration_biogpt.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    10578 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/biogpt/convert_biogpt_original_pytorch_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    43239 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/biogpt/modeling_biogpt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13723 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/biogpt/tokenization_biogpt.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.876430 llm-toys-0.1.0/llm_toys/hf/transformers/models/bit/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2244 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bit/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6236 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bit/configuration_bit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5955 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bit/convert_bit_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16108 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bit/image_processing_bit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    32019 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bit/modeling_bit.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.880430 llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4031 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19016 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot/configuration_blenderbot.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3702 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot/convert_blenderbot_original_pytorch_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    77177 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot/modeling_blenderbot.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    65012 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot/modeling_flax_blenderbot.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    67823 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot/modeling_tf_blenderbot.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19488 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot/tokenization_blenderbot.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14205 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot/tokenization_blenderbot_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.880430 llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot_small/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4263 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot_small/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18479 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot_small/configuration_blenderbot_small.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    75970 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot_small/modeling_blenderbot_small.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    65958 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot_small/modeling_flax_blenderbot_small.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    67121 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot_small/modeling_tf_blenderbot_small.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8641 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot_small/tokenization_blenderbot_small.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4058 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot_small/tokenization_blenderbot_small_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.880430 llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3692 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17118 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/configuration_blip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6980 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/convert_blip_original_pytorch_to_hf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14112 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/image_processing_blip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    61776 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/modeling_blip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    43338 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/modeling_blip_text.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    65275 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/modeling_tf_blip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    42406 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/modeling_tf_blip_text.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6204 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/processing_blip.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.880430 llm-toys-0.1.0/llm_toys/hf/transformers/models/blip_2/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2153 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blip_2/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17275 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blip_2/configuration_blip_2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12330 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blip_2/convert_blip_2_original_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    81996 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blip_2/modeling_blip_2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6698 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/blip_2/processing_blip_2.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.884430 llm-toys-0.1.0/llm_toys/hf/transformers/models/bloom/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2499 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bloom/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10758 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bloom/configuration_bloom.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10302 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bloom/convert_bloom_original_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    56945 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bloom/modeling_bloom.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7389 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bloom/tokenization_bloom_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.884430 llm-toys-0.1.0/llm_toys/hf/transformers/models/bridgetower/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2864 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bridgetower/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17056 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bridgetower/configuration_bridgetower.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    22800 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bridgetower/image_processing_bridgetower.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    88379 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bridgetower/modeling_bridgetower.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5056 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/bridgetower/processing_bridgetower.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.884430 llm-toys-0.1.0/llm_toys/hf/transformers/models/byt5/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      942 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/byt5/__init__.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2120 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/byt5/convert_byt5_original_tf_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10727 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/byt5/tokenization_byt5.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.884430 llm-toys-0.1.0/llm_toys/hf/transformers/models/camembert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4443 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/camembert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7735 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/camembert/configuration_camembert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    72469 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/camembert/modeling_camembert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    73463 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/camembert/modeling_tf_camembert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13581 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/camembert/tokenization_camembert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8658 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/camembert/tokenization_camembert_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.884430 llm-toys-0.1.0/llm_toys/hf/transformers/models/canine/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2272 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/canine/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6478 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/canine/configuration_canine.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2117 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/canine/convert_canine_original_tf_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    73763 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/canine/modeling_canine.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9276 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/canine/tokenization_canine.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.884430 llm-toys-0.1.0/llm_toys/hf/transformers/models/chinese_clip/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2919 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/chinese_clip/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    22588 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/chinese_clip/configuration_chinese_clip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5069 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/chinese_clip/convert_chinese_clip_original_pytorch_to_hf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1247 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/chinese_clip/feature_extraction_chinese_clip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15758 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/chinese_clip/image_processing_chinese_clip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    73599 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/chinese_clip/modeling_chinese_clip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6787 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/chinese_clip/processing_chinese_clip.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.888430 llm-toys-0.1.0/llm_toys/hf/transformers/models/clap/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2322 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clap/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21201 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clap/configuration_clap.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4695 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clap/convert_clap_original_pytorch_to_hf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18653 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clap/feature_extraction_clap.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   105313 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clap/modeling_clap.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5704 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clap/processing_clap.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.888430 llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5027 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21049 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/configuration_clip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5306 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/convert_clip_original_pytorch_to_hf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1172 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/feature_extraction_clip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16139 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/image_processing_clip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57071 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/modeling_clip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    45844 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/modeling_flax_clip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    53459 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/modeling_tf_clip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6854 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/processing_clip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21029 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/tokenization_clip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6956 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/tokenization_clip_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.888430 llm-toys-0.1.0/llm_toys/hf/transformers/models/clipseg/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2179 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clipseg/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21241 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clipseg/configuration_clipseg.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11114 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clipseg/convert_clipseg_original_pytorch_to_hf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    65133 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clipseg/modeling_clipseg.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7871 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/clipseg/processing_clipseg.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.888430 llm-toys-0.1.0/llm_toys/hf/transformers/models/codegen/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2443 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/codegen/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10324 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/codegen/configuration_codegen.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    31450 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/codegen/modeling_codegen.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15219 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/codegen/tokenization_codegen.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10614 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/codegen/tokenization_codegen_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.888430 llm-toys-0.1.0/llm_toys/hf/transformers/models/conditional_detr/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2828 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/conditional_detr/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12973 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/conditional_detr/configuration_conditional_detr.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15930 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/conditional_detr/convert_conditional_detr_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1251 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/conditional_detr/feature_extraction_conditional_detr.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    70534 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/conditional_detr/image_processing_conditional_detr.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   127751 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/conditional_detr/modeling_conditional_detr.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.892430 llm-toys-0.1.0/llm_toys/hf/transformers/models/convbert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4069 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convbert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7311 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convbert/configuration_convbert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2108 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convbert/convert_convbert_original_tf1_checkpoint_to_pytorch_and_tf2.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    58732 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convbert/modeling_convbert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    52625 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convbert/modeling_tf_convbert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21870 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convbert/tokenization_convbert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8765 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convbert/tokenization_convbert_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.892430 llm-toys-0.1.0/llm_toys/hf/transformers/models/convnext/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3150 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convnext/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6201 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convnext/configuration_convnext.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10220 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convnext/convert_convnext_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1200 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convnext/feature_extraction_convnext.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15054 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convnext/image_processing_convnext.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    22149 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convnext/modeling_convnext.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23306 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convnext/modeling_tf_convnext.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.892430 llm-toys-0.1.0/llm_toys/hf/transformers/models/convnextv2/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2159 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convnextv2/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5430 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convnextv2/configuration_convnextv2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12473 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convnextv2/convert_convnextv2_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23932 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/convnextv2/modeling_convnextv2.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.892430 llm-toys-0.1.0/llm_toys/hf/transformers/models/cpm/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1816 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/cpm/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15154 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/cpm/tokenization_cpm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10680 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/cpm/tokenization_cpm_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.892430 llm-toys-0.1.0/llm_toys/hf/transformers/models/cpmant/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2117 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/cpmant/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5329 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/cpmant/configuration_cpmant.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    37709 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/cpmant/modeling_cpmant.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10079 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/cpmant/tokenization_cpmant.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.892430 llm-toys-0.1.0/llm_toys/hf/transformers/models/ctrl/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2688 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/ctrl/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4738 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/ctrl/configuration_ctrl.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    34910 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/ctrl/modeling_ctrl.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    36036 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/ctrl/modeling_tf_ctrl.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8491 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/ctrl/tokenization_ctrl.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.896430 llm-toys-0.1.0/llm_toys/hf/transformers/models/cvt/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2434 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/cvt/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6860 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/cvt/configuration_cvt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13570 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/cvt/convert_cvt_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28913 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/cvt/modeling_cvt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    36051 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/cvt/modeling_tf_cvt.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.896430 llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4933 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16436 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/configuration_data2vec_audio.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7420 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/configuration_data2vec_text.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9432 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/configuration_data2vec_vision.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10858 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/convert_data2vec_audio_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9580 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/convert_data2vec_text_original_pytorch_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    15340 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/convert_data2vec_vision_original_pytorch_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    65709 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/modeling_data2vec_audio.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    71169 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/modeling_data2vec_text.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    53184 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/modeling_data2vec_vision.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    60423 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/modeling_tf_data2vec_vision.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.896430 llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3677 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9389 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta/configuration_deberta.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    58332 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta/modeling_deberta.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    60370 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta/modeling_tf_deberta.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19801 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta/tokenization_deberta.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13437 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta/tokenization_deberta_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.900430 llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta_v2/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3899 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta_v2/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9175 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta_v2/configuration_deberta_v2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    67935 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta_v2/modeling_deberta_v2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    66544 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta_v2/modeling_tf_deberta_v2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21720 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta_v2/tokenization_deberta_v2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10997 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta_v2/tokenization_deberta_v2_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.900430 llm-toys-0.1.0/llm_toys/hf/transformers/models/decision_transformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2124 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/decision_transformer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7321 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/decision_transformer/configuration_decision_transformer.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    43327 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/decision_transformer/modeling_decision_transformer.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.900430 llm-toys-0.1.0/llm_toys/hf/transformers/models/deformable_detr/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2599 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deformable_detr/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14244 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deformable_detr/configuration_deformable_detr.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9477 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deformable_detr/convert_deformable_detr_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1244 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deformable_detr/feature_extraction_deformable_detr.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57980 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deformable_detr/image_processing_deformable_detr.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1559 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deformable_detr/load_custom.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   119564 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deformable_detr/modeling_deformable_detr.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.900430 llm-toys-0.1.0/llm_toys/hf/transformers/models/deit/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3486 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deit/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5961 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deit/configuration_deit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9217 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deit/convert_deit_timm_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1172 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deit/feature_extraction_deit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14866 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deit/image_processing_deit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    38581 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deit/modeling_deit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    42421 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deit/modeling_tf_deit.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.900430 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/__init__.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.900430 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/bort/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/bort/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14057 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/bort/convert_bort_original_gluonnlp_checkpoint_to_pytorch.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.900430 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mctct/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1892 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mctct/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9308 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mctct/configuration_mctct.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13460 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mctct/feature_extraction_mctct.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    33784 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mctct/modeling_mctct.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5929 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mctct/processing_mctct.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.900430 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mmbt/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1480 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mmbt/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1606 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mmbt/configuration_mmbt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18890 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mmbt/modeling_mmbt.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.904430 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/retribert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2351 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/retribert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5407 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/retribert/configuration_retribert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9465 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/retribert/modeling_retribert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    22586 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/retribert/tokenization_retribert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9017 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/retribert/tokenization_retribert_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.904430 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/tapex/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      926 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/tapex/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    65003 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/tapex/tokenization_tapex.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.904430 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2077 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7413 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/configuration_trajectory_transformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3139 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/convert_trajectory_transformer_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    26203 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/modeling_trajectory_transformer.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.904430 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/van/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1728 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/van/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4837 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/van/configuration_van.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10363 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/van/convert_van_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21576 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/van/modeling_van.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.904430 llm-toys-0.1.0/llm_toys/hf/transformers/models/deta/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2205 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deta/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11931 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deta/configuration_deta.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16833 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deta/convert_deta_resnet_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19031 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deta/convert_deta_swin_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    42393 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deta/image_processing_deta.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   135049 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/deta/modeling_deta.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.904430 llm-toys-0.1.0/llm_toys/hf/transformers/models/detr/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2438 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/detr/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13243 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/detr/configuration_detr.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13561 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/detr/convert_detr_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18993 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/detr/convert_detr_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1172 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/detr/feature_extraction_detr.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    78319 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/detr/image_processing_detr.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   111497 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/detr/modeling_detr.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.904430 llm-toys-0.1.0/llm_toys/hf/transformers/models/dialogpt/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dialogpt/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1537 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dialogpt/convert_dialogpt_original_pytorch_checkpoint_to_pytorch.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.904430 llm-toys-0.1.0/llm_toys/hf/transformers/models/dinat/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1812 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dinat/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7399 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dinat/configuration_dinat.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    41810 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dinat/modeling_dinat.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.904430 llm-toys-0.1.0/llm_toys/hf/transformers/models/distilbert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5167 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/distilbert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6978 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/distilbert/configuration_distilbert.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    51793 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/distilbert/modeling_distilbert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    32621 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/distilbert/modeling_flax_distilbert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    42933 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/distilbert/modeling_tf_distilbert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23599 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/distilbert/tokenization_distilbert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10708 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/distilbert/tokenization_distilbert_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.908430 llm-toys-0.1.0/llm_toys/hf/transformers/models/dit/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dit/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9420 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dit/convert_dit_unilm_to_pytorch.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.908430 llm-toys-0.1.0/llm_toys/hf/transformers/models/donut/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2455 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/donut/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5981 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/donut/configuration_donut_swin.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9316 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/donut/convert_donut_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1179 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/donut/feature_extraction_donut.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19857 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/donut/image_processing_donut.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    43709 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/donut/modeling_donut_swin.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8095 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/donut/processing_donut.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.908430 llm-toys-0.1.0/llm_toys/hf/transformers/models/dpr/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4535 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dpr/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7262 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dpr/configuration_dpr.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6096 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dpr/convert_dpr_original_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28581 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dpr/modeling_dpr.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    31966 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dpr/modeling_tf_dpr.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19789 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dpr/tokenization_dpr.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20175 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dpr/tokenization_dpr_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.908430 llm-toys-0.1.0/llm_toys/hf/transformers/models/dpt/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2444 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dpt/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11302 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dpt/configuration_dpt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12994 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dpt/convert_dpt_hybrid_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11781 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dpt/convert_dpt_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1165 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dpt/feature_extraction_dpt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18212 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dpt/image_processing_dpt.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    54912 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/dpt/modeling_dpt.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.908430 llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3550 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientformer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7919 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientformer/configuration_efficientformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9381 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientformer/convert_efficientformer_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16416 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientformer/image_processing_efficientformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    33848 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientformer/modeling_efficientformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40444 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientformer/modeling_tf_efficientformer.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.908430 llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientnet/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2670 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientnet/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7750 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientnet/configuration_efficientnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12756 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientnet/convert_efficientnet_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16724 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientnet/image_processing_efficientnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24389 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientnet/modeling_efficientnet.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.912430 llm-toys-0.1.0/llm_toys/hf/transformers/models/electra/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5257 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/electra/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9927 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/electra/configuration_electra.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2862 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/electra/convert_electra_original_tf_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    75769 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/electra/modeling_electra.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    62265 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/electra/modeling_flax_electra.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    69406 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/electra/modeling_tf_electra.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    22677 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/electra/tokenization_electra.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10495 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/electra/tokenization_electra_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.912430 llm-toys-0.1.0/llm_toys/hf/transformers/models/encodec/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1910 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/encodec/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8749 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/encodec/configuration_encodec.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15253 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/encodec/convert_encodec_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9873 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/encodec/feature_extraction_encodec.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    33479 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/encodec/modeling_encodec.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.912430 llm-toys-0.1.0/llm_toys/hf/transformers/models/encoder_decoder/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2451 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/encoder_decoder/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4840 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/encoder_decoder/configuration_encoder_decoder.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    35803 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/encoder_decoder/modeling_encoder_decoder.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    43812 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/encoder_decoder/modeling_flax_encoder_decoder.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    34302 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/encoder_decoder/modeling_tf_encoder_decoder.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.912430 llm-toys-0.1.0/llm_toys/hf/transformers/models/ernie/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2331 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/ernie/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8884 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/ernie/configuration_ernie.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    84083 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/ernie/modeling_ernie.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.912430 llm-toys-0.1.0/llm_toys/hf/transformers/models/ernie_m/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2637 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/ernie_m/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6190 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/ernie_m/configuration_ernie_m.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    47827 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/ernie_m/modeling_ernie_m.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17113 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/ernie_m/tokenization_ernie_m.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.912430 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2978 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14558 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/configuration_esm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18476 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/convert_esm.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    55911 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/modeling_esm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    86749 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/modeling_esmfold.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    60870 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/modeling_tf_esm.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.912430 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      446 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14392 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/chunk_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3764 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/data_transforms.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8376 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/feats.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3705 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/loss.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11490 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/protein.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    37993 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/residue_constants.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    41122 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/rigid_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4798 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/tensor_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6015 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/tokenization_esm.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.912430 llm-toys-0.1.0/llm_toys/hf/transformers/models/falcon/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2067 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/falcon/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6683 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/falcon/configuration_falcon.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    56890 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/falcon/modeling_falcon.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.916430 llm-toys-0.1.0/llm_toys/hf/transformers/models/flaubert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3488 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/flaubert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11706 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/flaubert/configuration_flaubert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57659 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/flaubert/modeling_flaubert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    52304 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/flaubert/modeling_tf_flaubert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24019 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/flaubert/tokenization_flaubert.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.916430 llm-toys-0.1.0/llm_toys/hf/transformers/models/flava/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3030 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/flava/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    37956 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/flava/configuration_flava.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3428 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/flava/convert_dalle_to_flava_codebook.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4372 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/flava/convert_flava_original_pytorch_to_hf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1201 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/flava/feature_extraction_flava.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    36878 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/flava/image_processing_flava.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    96717 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/flava/modeling_flava.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6807 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/flava/processing_flava.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.916430 llm-toys-0.1.0/llm_toys/hf/transformers/models/fnet/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3179 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/fnet/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5839 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/fnet/configuration_fnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6912 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/fnet/convert_fnet_original_flax_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    49473 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/fnet/modeling_fnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15847 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/fnet/tokenization_fnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8558 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/fnet/tokenization_fnet_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.916430 llm-toys-0.1.0/llm_toys/hf/transformers/models/focalnet/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1989 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/focalnet/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8013 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/focalnet/configuration_focalnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9450 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/focalnet/convert_focalnet_to_hf_format.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    43585 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/focalnet/modeling_focalnet.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.916430 llm-toys-0.1.0/llm_toys/hf/transformers/models/fsmt/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1675 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/fsmt/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10579 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/fsmt/configuration_fsmt.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    11264 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/fsmt/convert_fsmt_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    58083 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/fsmt/modeling_fsmt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20127 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/fsmt/tokenization_fsmt.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.916430 llm-toys-0.1.0/llm_toys/hf/transformers/models/funnel/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4126 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/funnel/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8894 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/funnel/configuration_funnel.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2335 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/funnel/convert_funnel_original_tf_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    69831 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/funnel/modeling_funnel.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    73093 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/funnel/modeling_tf_funnel.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24023 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/funnel/tokenization_funnel.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11794 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/funnel/tokenization_funnel_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.920431 llm-toys-0.1.0/llm_toys/hf/transformers/models/git/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1888 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/git/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11822 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/git/configuration_git.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21976 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/git/convert_git_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    69494 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/git/modeling_git.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5486 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/git/processing_git.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.920431 llm-toys-0.1.0/llm_toys/hf/transformers/models/glpn/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2384 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/glpn/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6183 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/glpn/configuration_glpn.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8558 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/glpn/convert_glpn_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1172 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/glpn/feature_extraction_glpn.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8864 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/glpn/image_processing_glpn.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    31527 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/glpn/modeling_glpn.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.920431 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4674 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12134 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/configuration_gpt2.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2532 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/convert_gpt2_original_tf_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    31960 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/modeling_flax_gpt2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    76173 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/modeling_gpt2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    51678 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/modeling_tf_gpt2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14425 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/tokenization_gpt2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8054 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/tokenization_gpt2_fast.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3763 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/tokenization_gpt2_tf.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.920431 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_bigcode/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2037 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_bigcode/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6448 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_bigcode/configuration_gpt_bigcode.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    48056 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_bigcode/modeling_gpt_bigcode.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.920431 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neo/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2718 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neo/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12058 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neo/configuration_gpt_neo.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2589 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neo/convert_gpt_neo_mesh_tf_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28080 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neo/modeling_flax_gpt_neo.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    47983 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neo/modeling_gpt_neo.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.920431 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2595 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8824 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox/configuration_gpt_neox.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    51180 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox/modeling_gpt_neox.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5797 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox/tokenization_gpt_neox_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.924430 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox_japanese/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2154 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox_japanese/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5729 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox_japanese/configuration_gpt_neox_japanese.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    32308 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox_japanese/modeling_gpt_neox_japanese.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17328 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox_japanese/tokenization_gpt_neox_japanese.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.924430 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_sw3/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1361 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_sw3/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8156 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_sw3/convert_megatron_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14759 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_sw3/tokenization_gpt_sw3.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.924430 llm-toys-0.1.0/llm_toys/hf/transformers/models/gptj/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3280 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gptj/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8996 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gptj/configuration_gptj.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28517 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gptj/modeling_flax_gptj.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    49873 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gptj/modeling_gptj.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    44030 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gptj/modeling_tf_gptj.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.924430 llm-toys-0.1.0/llm_toys/hf/transformers/models/gptsan_japanese/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2294 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gptsan_japanese/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7329 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gptsan_japanese/configuration_gptsan_japanese.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9793 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gptsan_japanese/convert_gptsan_tf_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    67099 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gptsan_japanese/modeling_gptsan_japanese.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24556 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/gptsan_japanese/tokenization_gptsan_japanese.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.924430 llm-toys-0.1.0/llm_toys/hf/transformers/models/graphormer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1873 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/graphormer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6086 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/graphormer/collating_graphormer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10401 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/graphormer/configuration_graphormer.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    37407 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/graphormer/modeling_graphormer.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.924430 llm-toys-0.1.0/llm_toys/hf/transformers/models/groupvit/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2875 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/groupvit/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21413 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/groupvit/configuration_groupvit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9775 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/groupvit/convert_groupvit_nvlab_to_hf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    68613 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/groupvit/modeling_groupvit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    77841 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/groupvit/modeling_tf_groupvit.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.924430 llm-toys-0.1.0/llm_toys/hf/transformers/models/herbert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1472 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/herbert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    25665 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/herbert/tokenization_herbert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6549 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/herbert/tokenization_herbert_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.928430 llm-toys-0.1.0/llm_toys/hf/transformers/models/hubert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2536 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/hubert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14760 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/hubert/configuration_hubert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8942 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/hubert/convert_distilhubert_original_s3prl_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10380 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/hubert/convert_hubert_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2895 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/hubert/convert_hubert_original_s3prl_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    60942 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/hubert/modeling_hubert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    63209 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/hubert/modeling_tf_hubert.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.928430 llm-toys-0.1.0/llm_toys/hf/transformers/models/ibert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2086 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/ibert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7462 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/ibert/configuration_ibert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    56703 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/ibert/modeling_ibert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    30072 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/ibert/quant_modules.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.928430 llm-toys-0.1.0/llm_toys/hf/transformers/models/imagegpt/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2658 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/imagegpt/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8866 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/imagegpt/configuration_imagegpt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2691 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/imagegpt/convert_imagegpt_original_tf2_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1200 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/imagegpt/feature_extraction_imagegpt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10808 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/imagegpt/image_processing_imagegpt.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    53849 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/imagegpt/modeling_imagegpt.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.928430 llm-toys-0.1.0/llm_toys/hf/transformers/models/informer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1857 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/informer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12684 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/informer/configuration_informer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   103554 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/informer/modeling_informer.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.928430 llm-toys-0.1.0/llm_toys/hf/transformers/models/instructblip/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2279 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/instructblip/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17867 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/instructblip/configuration_instructblip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13387 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/instructblip/convert_instructblip_original_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    70206 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/instructblip/modeling_instructblip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7855 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/instructblip/processing_instructblip.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.928430 llm-toys-0.1.0/llm_toys/hf/transformers/models/jukebox/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2084 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/jukebox/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    27873 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/jukebox/configuration_jukebox.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11789 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/jukebox/convert_jukebox.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   119653 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/jukebox/modeling_jukebox.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17740 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/jukebox/tokenization_jukebox.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.928430 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlm/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3787 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlm/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9513 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlm/configuration_layoutlm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    61080 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlm/modeling_layoutlm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    65594 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlm/modeling_tf_layoutlm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21698 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlm/tokenization_layoutlm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8967 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlm/tokenization_layoutlm_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.932431 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv2/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3439 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv2/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11247 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv2/configuration_layoutlmv2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1195 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv2/feature_extraction_layoutlmv2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11287 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv2/image_processing_layoutlmv2.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    61575 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv2/modeling_layoutlmv2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9267 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv2/processing_layoutlmv2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    72412 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv2/tokenization_layoutlmv2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    38073 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv2/tokenization_layoutlmv2_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.932431 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4512 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13363 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/configuration_layoutlmv3.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1195 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/feature_extraction_layoutlmv3.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16742 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/image_processing_layoutlmv3.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    60927 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/modeling_layoutlmv3.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    67864 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/modeling_tf_layoutlmv3.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9118 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/processing_layoutlmv3.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    72788 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/tokenization_layoutlmv3.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40311 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/tokenization_layoutlmv3_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.932431 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutxlm/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2037 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutxlm/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9218 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutxlm/processing_layoutxlm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57669 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutxlm/tokenization_layoutxlm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    39911 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutxlm/tokenization_layoutxlm_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.932431 llm-toys-0.1.0/llm_toys/hf/transformers/models/led/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3008 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/led/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7633 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/led/configuration_led.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   139950 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/led/modeling_led.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   116584 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/led/modeling_tf_led.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20406 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/led/tokenization_led.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14871 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/led/tokenization_led_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.932431 llm-toys-0.1.0/llm_toys/hf/transformers/models/levit/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2508 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/levit/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5930 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/levit/configuration_levit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6258 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/levit/convert_levit_timm_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1204 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/levit/feature_extraction_levit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17200 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/levit/image_processing_levit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    29663 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/levit/modeling_levit.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.936431 llm-toys-0.1.0/llm_toys/hf/transformers/models/lilt/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1909 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/lilt/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6878 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/lilt/configuration_lilt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    53140 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/lilt/modeling_lilt.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.936431 llm-toys-0.1.0/llm_toys/hf/transformers/models/llama/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2665 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/llama/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6998 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/llama/configuration_llama.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10917 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/llama/convert_llama_weights_to_hf.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    42064 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/llama/modeling_llama.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12954 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/llama/tokenization_llama.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6491 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/llama/tokenization_llama_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.936431 llm-toys-0.1.0/llm_toys/hf/transformers/models/longformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4196 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/longformer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9564 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/longformer/configuration_longformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3026 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/longformer/convert_longformer_original_pytorch_lightning_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   114361 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/longformer/modeling_longformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   121690 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/longformer/modeling_tf_longformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18736 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/longformer/tokenization_longformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14530 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/longformer/tokenization_longformer_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.936431 llm-toys-0.1.0/llm_toys/hf/transformers/models/longt5/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2546 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/longt5/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8481 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/longt5/configuration_longt5.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11089 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/longt5/convert_longt5x_checkpoint_to_flax.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   105640 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/longt5/modeling_flax_longt5.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   105418 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/longt5/modeling_longt5.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.936431 llm-toys-0.1.0/llm_toys/hf/transformers/models/luke/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2383 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/luke/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6554 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/luke/configuration_luke.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7467 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/luke/convert_luke_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   104043 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/luke/modeling_luke.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    85386 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/luke/tokenization_luke.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.936431 llm-toys-0.1.0/llm_toys/hf/transformers/models/lxmert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3396 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/lxmert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9510 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/lxmert/configuration_lxmert.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2109 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/lxmert/convert_lxmert_original_tf_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    64955 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/lxmert/modeling_lxmert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    61404 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/lxmert/modeling_tf_lxmert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21421 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/lxmert/tokenization_lxmert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8437 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/lxmert/tokenization_lxmert_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.936431 llm-toys-0.1.0/llm_toys/hf/transformers/models/m2m_100/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1992 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/m2m_100/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13582 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/m2m_100/configuration_m2m_100.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3159 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/m2m_100/convert_m2m100_original_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    65535 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/m2m_100/modeling_m2m_100.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17257 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/m2m_100/tokenization_m2m_100.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.940431 llm-toys-0.1.0/llm_toys/hf/transformers/models/marian/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3444 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/marian/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18558 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/marian/configuration_marian.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    36254 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/marian/convert_marian_tatoeba_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    26757 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/marian/convert_marian_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    64272 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/marian/modeling_flax_marian.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    83338 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/marian/modeling_marian.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    69040 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/marian/modeling_tf_marian.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17662 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/marian/tokenization_marian.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.940431 llm-toys-0.1.0/llm_toys/hf/transformers/models/markuplm/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2806 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/markuplm/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7571 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/markuplm/configuration_markuplm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6400 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/markuplm/feature_extraction_markuplm.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    57944 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/markuplm/modeling_markuplm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6347 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/markuplm/processing_markuplm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    69705 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/markuplm/tokenization_markuplm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    42808 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/markuplm/tokenization_markuplm_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.940431 llm-toys-0.1.0/llm_toys/hf/transformers/models/mask2former/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2357 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mask2former/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11404 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mask2former/configuration_mask2former.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    45688 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mask2former/convert_mask2former_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    50612 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mask2former/image_processing_mask2former.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   120588 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mask2former/modeling_mask2former.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.940431 llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2945 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9360 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/configuration_maskformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7054 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/configuration_maskformer_swin.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    32237 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/convert_maskformer_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20732 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/convert_maskformer_resnet_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20321 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/convert_maskformer_swin_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1214 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/feature_extraction_maskformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    53010 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/image_processing_maskformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    89023 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/modeling_maskformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    41045 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/modeling_maskformer_swin.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.944431 llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4403 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18387 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart/configuration_mbart.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3035 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart/convert_mbart_original_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    75102 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart/modeling_flax_mbart.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    89498 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart/modeling_mbart.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    68919 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart/modeling_tf_mbart.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14713 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart/tokenization_mbart.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11916 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart/tokenization_mbart_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.944431 llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart50/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1847 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart50/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16666 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart50/tokenization_mbart50.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12199 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart50/tokenization_mbart50_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.944431 llm-toys-0.1.0/llm_toys/hf/transformers/models/mega/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2140 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mega/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12738 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mega/configuration_mega.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13154 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mega/convert_mega_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   109288 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mega/modeling_mega.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.944431 llm-toys-0.1.0/llm_toys/hf/transformers/models/megatron_bert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2506 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/megatron_bert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6573 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/megatron_bert/configuration_megatron_bert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13686 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/megatron_bert/convert_megatron_bert_checkpoint.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    83194 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/megatron_bert/modeling_megatron_bert.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.944431 llm-toys-0.1.0/llm_toys/hf/transformers/models/megatron_gpt2/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      630 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/megatron_gpt2/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    36651 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/megatron_gpt2/checkpoint_reshaping_and_interoperability.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13627 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/megatron_gpt2/convert_megatron_gpt2_checkpoint.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.944431 llm-toys-0.1.0/llm_toys/hf/transformers/models/mgp_str/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2164 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mgp_str/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5935 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mgp_str/configuration_mgp_str.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21898 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mgp_str/modeling_mgp_str.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9244 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mgp_str/processing_mgp_str.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4068 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mgp_str/tokenization_mgp_str.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.944431 llm-toys-0.1.0/llm_toys/hf/transformers/models/mluke/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1356 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mluke/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10185 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mluke/convert_mluke_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    81133 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mluke/tokenization_mluke.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.944431 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilebert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4604 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilebert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8586 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilebert/configuration_mobilebert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2200 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilebert/convert_mobilebert_original_tf_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    70458 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilebert/modeling_mobilebert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    70944 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilebert/modeling_tf_mobilebert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21304 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilebert/tokenization_mobilebert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8377 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilebert/tokenization_mobilebert_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.948431 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v1/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2735 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v1/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5237 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v1/configuration_mobilenet_v1.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4932 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v1/convert_original_tf_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1222 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v1/feature_extraction_mobilenet_v1.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16159 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v1/image_processing_mobilenet_v1.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    18777 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v1/modeling_mobilenet_v1.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.948431 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v2/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2830 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v2/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7361 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v2/configuration_mobilenet_v2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6402 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v2/convert_original_tf_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1222 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v2/feature_extraction_mobilenet_v2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18576 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v2/image_processing_mobilenet_v2.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    34752 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v2/modeling_mobilenet_v2.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.948431 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevit/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3492 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevit/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8400 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevit/configuration_mobilevit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12402 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevit/convert_mlcvnets_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1207 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevit/feature_extraction_mobilevit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15713 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevit/image_processing_mobilevit.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    40528 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevit/modeling_mobilevit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    44632 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevit/modeling_tf_mobilevit.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.948431 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevitv2/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2111 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevitv2/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7237 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevitv2/configuration_mobilevitv2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12557 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevitv2/convert_mlcvnets_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    38738 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevitv2/modeling_mobilevitv2.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.948431 llm-toys-0.1.0/llm_toys/hf/transformers/models/mpnet/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3875 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mpnet/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5442 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mpnet/configuration_mpnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    42548 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mpnet/modeling_mpnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    48395 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mpnet/modeling_tf_mpnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    22583 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mpnet/tokenization_mpnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8930 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mpnet/tokenization_mpnet_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.948431 llm-toys-0.1.0/llm_toys/hf/transformers/models/mra/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2254 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mra/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6662 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mra/configuration_mra.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4247 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mra/convert_mra_pytorch_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    62339 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mra/modeling_mra.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.948431 llm-toys-0.1.0/llm_toys/hf/transformers/models/mt5/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3439 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mt5/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7588 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mt5/configuration_mt5.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4239 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mt5/modeling_flax_mt5.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   102044 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mt5/modeling_mt5.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3325 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mt5/modeling_tf_mt5.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.952431 llm-toys-0.1.0/llm_toys/hf/transformers/models/musicgen/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2099 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/musicgen/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10772 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/musicgen/configuration_musicgen.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8128 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/musicgen/convert_musicgen_transformers.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   123160 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/musicgen/modeling_musicgen.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5665 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/musicgen/processing_musicgen.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.952431 llm-toys-0.1.0/llm_toys/hf/transformers/models/mvp/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2536 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mvp/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8533 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mvp/configuration_mvp.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    95123 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mvp/modeling_mvp.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16823 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mvp/tokenization_mvp.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12088 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/mvp/tokenization_mvp_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.952431 llm-toys-0.1.0/llm_toys/hf/transformers/models/nat/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1776 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/nat/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7033 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/nat/configuration_nat.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40045 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/nat/modeling_nat.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.952431 llm-toys-0.1.0/llm_toys/hf/transformers/models/nezha/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2233 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/nezha/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5033 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/nezha/configuration_nezha.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    75081 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/nezha/modeling_nezha.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.952431 llm-toys-0.1.0/llm_toys/hf/transformers/models/nllb/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1868 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/nllb/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19976 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/nllb/tokenization_nllb.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16966 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/nllb/tokenization_nllb_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.952431 llm-toys-0.1.0/llm_toys/hf/transformers/models/nllb_moe/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1978 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/nllb_moe/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11315 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/nllb_moe/configuration_nllb_moe.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6477 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/nllb_moe/convert_nllb_moe_sharded_original_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    86841 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/nllb_moe/modeling_nllb_moe.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.952431 llm-toys-0.1.0/llm_toys/hf/transformers/models/nystromformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2337 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/nystromformer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6623 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/nystromformer/configuration_nystromformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4197 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/nystromformer/convert_nystromformer_original_pytorch_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    49086 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/nystromformer/modeling_nystromformer.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.952431 llm-toys-0.1.0/llm_toys/hf/transformers/models/oneformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2402 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/oneformer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12423 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/oneformer/configuration_oneformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    50690 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/oneformer/convert_to_hf_oneformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    55915 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/oneformer/image_processing_oneformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   143392 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/oneformer/modeling_oneformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9482 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/oneformer/processing_oneformer.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.956431 llm-toys-0.1.0/llm_toys/hf/transformers/models/open_llama/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2787 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/open_llama/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7858 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/open_llama/configuration_open_llama.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    44924 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/open_llama/modeling_open_llama.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.956431 llm-toys-0.1.0/llm_toys/hf/transformers/models/openai/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3658 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/openai/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7332 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/openai/configuration_openai.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2666 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/openai/convert_openai_original_tf_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    38004 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/openai/modeling_openai.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    37783 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/openai/modeling_tf_openai.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15582 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/openai/tokenization_openai.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3046 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/openai/tokenization_openai_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.956431 llm-toys-0.1.0/llm_toys/hf/transformers/models/opt/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2977 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/opt/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7244 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/opt/configuration_opt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3858 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/opt/convert_opt_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    31547 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/opt/modeling_flax_opt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57855 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/opt/modeling_opt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    45560 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/opt/modeling_tf_opt.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.956431 llm-toys-0.1.0/llm_toys/hf/transformers/models/owlvit/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2915 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/owlvit/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17054 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/owlvit/configuration_owlvit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13988 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/owlvit/convert_owlvit_original_flax_to_hf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1186 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/owlvit/feature_extraction_owlvit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23870 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/owlvit/image_processing_owlvit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    77705 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/owlvit/modeling_owlvit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11123 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/owlvit/processing_owlvit.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.956431 llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4111 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7693 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus/configuration_pegasus.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5359 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus/convert_pegasus_tf_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    66067 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus/modeling_flax_pegasus.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    82118 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus/modeling_pegasus.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    69379 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus/modeling_tf_pegasus.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13709 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus/tokenization_pegasus.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9937 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus/tokenization_pegasus_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.956431 llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus_x/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1828 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus_x/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8419 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus_x/configuration_pegasus_x.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    79396 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus_x/modeling_pegasus_x.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.960431 llm-toys-0.1.0/llm_toys/hf/transformers/models/perceiver/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3293 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/perceiver/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12055 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/perceiver/configuration_perceiver.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21286 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/perceiver/convert_perceiver_haiku_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1207 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/perceiver/feature_extraction_perceiver.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15537 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/perceiver/image_processing_perceiver.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   146469 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/perceiver/modeling_perceiver.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8945 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/perceiver/tokenization_perceiver.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.960431 llm-toys-0.1.0/llm_toys/hf/transformers/models/phobert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      955 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/phobert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13551 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/phobert/tokenization_phobert.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.960431 llm-toys-0.1.0/llm_toys/hf/transformers/models/pix2struct/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2701 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/pix2struct/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18040 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/pix2struct/configuration_pix2struct.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5886 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/pix2struct/convert_pix2struct_original_pytorch_to_hf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17854 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/pix2struct/image_processing_pix2struct.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    83362 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/pix2struct/modeling_pix2struct.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6959 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/pix2struct/processing_pix2struct.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.960431 llm-toys-0.1.0/llm_toys/hf/transformers/models/plbart/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2429 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/plbart/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8719 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/plbart/configuration_plbart.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3553 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/plbart/convert_plbart_original_checkpoint_to_torch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    82983 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/plbart/modeling_plbart.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21656 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/plbart/tokenization_plbart.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.960431 llm-toys-0.1.0/llm_toys/hf/transformers/models/poolformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2586 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/poolformer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5802 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/poolformer/configuration_poolformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7947 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/poolformer/convert_poolformer_original_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1214 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/poolformer/feature_extraction_poolformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18310 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/poolformer/image_processing_poolformer.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    18074 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/poolformer/modeling_poolformer.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.960431 llm-toys-0.1.0/llm_toys/hf/transformers/models/prophetnet/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2157 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/prophetnet/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9062 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/prophetnet/configuration_prophetnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7055 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/prophetnet/convert_prophetnet_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   114949 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/prophetnet/modeling_prophetnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21847 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/prophetnet/tokenization_prophetnet.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.960431 llm-toys-0.1.0/llm_toys/hf/transformers/models/qdqbert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2402 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/qdqbert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5895 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/qdqbert/configuration_qdqbert.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    77045 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/qdqbert/modeling_qdqbert.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.964431 llm-toys-0.1.0/llm_toys/hf/transformers/models/rag/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2426 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/rag/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8800 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/rag/configuration_rag.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    86080 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/rag/modeling_rag.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    87921 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/rag/modeling_tf_rag.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28510 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/rag/retrieval_rag.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4576 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/rag/tokenization_rag.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.964431 llm-toys-0.1.0/llm_toys/hf/transformers/models/realm/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2675 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/realm/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8743 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/realm/configuration_realm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    84492 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/realm/modeling_realm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6370 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/realm/retrieval_realm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    25477 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/realm/tokenization_realm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14575 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/realm/tokenization_realm_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.964431 llm-toys-0.1.0/llm_toys/hf/transformers/models/reformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3139 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/reformer/__init__.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    13463 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/reformer/configuration_reformer.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     7818 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/reformer/convert_reformer_trax_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   115179 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/reformer/modeling_reformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7315 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/reformer/tokenization_reformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4825 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/reformer/tokenization_reformer_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.964431 llm-toys-0.1.0/llm_toys/hf/transformers/models/regnet/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3168 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/regnet/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4088 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/regnet/configuration_regnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11770 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/regnet/convert_regnet_seer_10b_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18715 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/regnet/convert_regnet_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28403 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/regnet/modeling_flax_regnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17533 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/regnet/modeling_regnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19479 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/regnet/modeling_tf_regnet.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.964431 llm-toys-0.1.0/llm_toys/hf/transformers/models/rembert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4514 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/rembert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7450 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/rembert/configuration_rembert.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2208 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/rembert/convert_rembert_tf_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    68091 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/rembert/modeling_rembert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    69600 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/rembert/modeling_tf_rembert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10481 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/rembert/tokenization_rembert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10422 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/rembert/tokenization_rembert_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.964431 llm-toys-0.1.0/llm_toys/hf/transformers/models/resnet/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3216 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/resnet/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5697 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/resnet/configuration_resnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7287 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/resnet/convert_resnet_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24640 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/resnet/modeling_flax_resnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19025 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/resnet/modeling_resnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19121 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/resnet/modeling_tf_resnet.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.968431 llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5091 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7878 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta/configuration_roberta.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8002 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta/convert_roberta_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    56957 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta/modeling_flax_roberta.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    71162 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta/modeling_roberta.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    71893 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta/modeling_tf_roberta.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17960 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta/tokenization_roberta.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13678 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta/tokenization_roberta_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.968431 llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta_prelayernorm/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5391 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta_prelayernorm/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8024 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta_prelayernorm/configuration_roberta_prelayernorm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2975 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta_prelayernorm/convert_roberta_prelayernorm_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    60529 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta_prelayernorm/modeling_flax_roberta_prelayernorm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    73898 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta_prelayernorm/modeling_roberta_prelayernorm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    74866 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta_prelayernorm/modeling_tf_roberta_prelayernorm.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.968431 llm-toys-0.1.0/llm_toys/hf/transformers/models/roc_bert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2875 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roc_bert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8657 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roc_bert/configuration_roc_bert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    92854 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roc_bert/modeling_roc_bert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    50992 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roc_bert/tokenization_roc_bert.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.968431 llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5333 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7711 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/configuration_roformer.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2240 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/convert_roformer_original_tf_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    39460 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/modeling_flax_roformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    69287 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/modeling_roformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57616 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/modeling_tf_roformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23835 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/tokenization_roformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8276 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/tokenization_roformer_fast.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2652 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/tokenization_utils.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.968431 llm-toys-0.1.0/llm_toys/hf/transformers/models/rwkv/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1780 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/rwkv/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6204 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/rwkv/configuration_rwkv.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6994 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/rwkv/convert_rwkv_checkpoint_to_hf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    35605 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/rwkv/modeling_rwkv.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.968431 llm-toys-0.1.0/llm_toys/hf/transformers/models/sam/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2980 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/sam/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14784 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/sam/configuration_sam.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6958 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/sam/convert_sam_original_to_hf_format.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57242 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/sam/image_processing_sam.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    65035 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/sam/modeling_sam.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    66857 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/sam/modeling_tf_sam.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10848 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/sam/processing_sam.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.972431 llm-toys-0.1.0/llm_toys/hf/transformers/models/segformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3676 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/segformer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7636 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/segformer/configuration_segformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17092 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/segformer/convert_segformer_original_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1207 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/segformer/feature_extraction_segformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21100 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/segformer/image_processing_segformer.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    35488 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/segformer/modeling_segformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    36138 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/segformer/modeling_tf_segformer.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.972431 llm-toys-0.1.0/llm_toys/hf/transformers/models/sew/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1778 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/sew/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14239 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/sew/configuration_sew.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12745 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/sew/convert_sew_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    53927 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/sew/modeling_sew.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.972431 llm-toys-0.1.0/llm_toys/hf/transformers/models/sew_d/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1804 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/sew_d/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15981 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/sew_d/configuration_sew_d.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13575 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/sew_d/convert_sew_d_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    74626 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/sew_d/modeling_sew_d.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.972431 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_encoder_decoder/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2037 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_encoder_decoder/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5087 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_encoder_decoder/configuration_speech_encoder_decoder.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14760 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_encoder_decoder/convert_mbart_wav2vec2_seq2seq_original_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11971 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_encoder_decoder/convert_speech_to_text_wav2vec2_seq2seq_original_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    45067 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_encoder_decoder/modeling_flax_speech_encoder_decoder.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    32945 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_encoder_decoder/modeling_speech_encoder_decoder.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.972431 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3845 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9312 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text/configuration_speech_to_text.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4478 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text/convert_s2t_fairseq_to_tfms.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11798 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text/feature_extraction_speech_to_text.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    66955 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text/modeling_speech_to_text.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    68086 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text/modeling_tf_speech_to_text.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4817 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text/processing_speech_to_text.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11653 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text/tokenization_speech_to_text.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.972431 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text_2/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2166 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text_2/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6281 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text_2/configuration_speech_to_text_2.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    46328 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text_2/modeling_speech_to_text_2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4789 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text_2/processing_speech_to_text_2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9211 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text_2/tokenization_speech_to_text_2.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.976431 llm-toys-0.1.0/llm_toys/hf/transformers/models/speecht5/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2971 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speecht5/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23899 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speecht5/configuration_speecht5.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4241 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speecht5/convert_hifigan.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17194 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speecht5/convert_speecht5_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17809 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speecht5/feature_extraction_speecht5.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   144023 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speecht5/modeling_speecht5.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7561 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speecht5/processing_speecht5.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8390 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/speecht5/tokenization_speecht5.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.976431 llm-toys-0.1.0/llm_toys/hf/transformers/models/splinter/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2532 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/splinter/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6120 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/splinter/configuration_splinter.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    53633 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/splinter/modeling_splinter.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    22013 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/splinter/tokenization_splinter.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9657 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/splinter/tokenization_splinter_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.976431 llm-toys-0.1.0/llm_toys/hf/transformers/models/squeezebert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2996 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/squeezebert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7910 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/squeezebert/configuration_squeezebert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    45011 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/squeezebert/modeling_squeezebert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21889 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/squeezebert/tokenization_squeezebert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9397 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/squeezebert/tokenization_squeezebert_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.976431 llm-toys-0.1.0/llm_toys/hf/transformers/models/swiftformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1990 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swiftformer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5346 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swiftformer/configuration_swiftformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6239 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swiftformer/convert_swiftformer_original_to_hf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23318 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swiftformer/modeling_swiftformer.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.976431 llm-toys-0.1.0/llm_toys/hf/transformers/models/swin/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2703 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swin/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7999 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swin/configuration_swin.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6627 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swin/convert_swin_simmim_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5805 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swin/convert_swin_timm_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    60019 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swin/modeling_swin.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    63770 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swin/modeling_tf_swin.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.976431 llm-toys-0.1.0/llm_toys/hf/transformers/models/swin2sr/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2277 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swin2sr/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6706 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swin2sr/configuration_swin2sr.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11355 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swin2sr/convert_swin2sr_original_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7713 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swin2sr/image_processing_swin2sr.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    51704 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swin2sr/modeling_swin2sr.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.976431 llm-toys-0.1.0/llm_toys/hf/transformers/models/swinv2/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1867 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swinv2/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6323 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swinv2/configuration_swinv2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7687 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swinv2/convert_swinv2_timm_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    61510 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/swinv2/modeling_swinv2.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.980431 llm-toys-0.1.0/llm_toys/hf/transformers/models/switch_transformers/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2484 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/switch_transformers/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10011 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/switch_transformers/configuration_switch_transformers.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7649 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/switch_transformers/convert_big_switch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7593 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/switch_transformers/convert_switch_transformers_original_flax_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    89411 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/switch_transformers/modeling_switch_transformers.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.980431 llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4338 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7460 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/configuration_t5.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2120 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/convert_t5_original_tf_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10538 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/convert_t5x_checkpoint_to_flax.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    10365 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/convert_t5x_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    74074 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/modeling_flax_t5.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    97295 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/modeling_t5.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    71842 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/modeling_tf_t5.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17968 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/tokenization_t5.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10587 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/tokenization_t5_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.980431 llm-toys-0.1.0/llm_toys/hf/transformers/models/table_transformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2065 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/table_transformer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12520 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/table_transformer/configuration_table_transformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15076 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/table_transformer/convert_table_transformer_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    92597 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/table_transformer/modeling_table_transformer.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.980431 llm-toys-0.1.0/llm_toys/hf/transformers/models/tapas/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2952 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/tapas/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12900 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/tapas/configuration_tapas.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5049 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/tapas/convert_tapas_original_tf_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   111736 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/tapas/modeling_tapas.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   105769 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/tapas/modeling_tf_tapas.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   121112 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/tapas/tokenization_tapas.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.980431 llm-toys-0.1.0/llm_toys/hf/transformers/models/time_series_transformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2069 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/time_series_transformer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12003 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/time_series_transformer/configuration_time_series_transformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    90470 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/time_series_transformer/modeling_time_series_transformer.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.980431 llm-toys-0.1.0/llm_toys/hf/transformers/models/timesformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1862 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/timesformer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5683 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/timesformer/configuration_timesformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10176 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/timesformer/convert_timesformer_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    34650 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/timesformer/modeling_timesformer.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.980431 llm-toys-0.1.0/llm_toys/hf/transformers/models/timm_backbone/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1624 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/timm_backbone/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2876 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/timm_backbone/configuration_timm_backbone.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5991 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/timm_backbone/modeling_timm_backbone.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.984431 llm-toys-0.1.0/llm_toys/hf/transformers/models/transfo_xl/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3182 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/transfo_xl/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7895 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/transfo_xl/configuration_transfo_xl.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     4916 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/transfo_xl/convert_transfo_xl_original_tf_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    45094 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/transfo_xl/modeling_tf_transfo_xl.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7597 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/transfo_xl/modeling_tf_transfo_xl_utilities.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    55720 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/transfo_xl/modeling_transfo_xl.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10861 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/transfo_xl/modeling_transfo_xl_utilities.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    30487 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/transfo_xl/tokenization_transfo_xl.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.984431 llm-toys-0.1.0/llm_toys/hf/transformers/models/trocr/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1818 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/trocr/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6778 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/trocr/configuration_trocr.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10155 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/trocr/convert_trocr_unilm_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    47542 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/trocr/modeling_trocr.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5720 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/trocr/processing_trocr.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.984431 llm-toys-0.1.0/llm_toys/hf/transformers/models/tvlt/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2687 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/tvlt/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8760 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/tvlt/configuration_tvlt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10507 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/tvlt/feature_extraction_tvlt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20730 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/tvlt/image_processing_tvlt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57262 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/tvlt/modeling_tvlt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3505 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/tvlt/processing_tvlt.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.984431 llm-toys-0.1.0/llm_toys/hf/transformers/models/umt5/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1746 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/umt5/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7753 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/umt5/configuration_umt5.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12070 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/umt5/convert_umt5_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    73907 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/umt5/modeling_umt5.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.984431 llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2018 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17161 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech/configuration_unispeech.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11340 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech/convert_unispeech_original_pytorch_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    73175 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech/modeling_unispeech.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.984431 llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech_sat/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2267 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech_sat/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18584 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech_sat/configuration_unispeech_sat.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4870 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech_sat/convert_unispeech_original_s3prl_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9289 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech_sat/convert_unispeech_sat_original_pytorch_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    86770 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech_sat/modeling_unispeech_sat.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.984431 llm-toys-0.1.0/llm_toys/hf/transformers/models/upernet/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1535 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/upernet/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5439 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/upernet/configuration_upernet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10271 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/upernet/convert_convnext_upernet_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14026 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/upernet/convert_swin_upernet_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17414 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/upernet/modeling_upernet.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.988431 llm-toys-0.1.0/llm_toys/hf/transformers/models/videomae/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2519 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/videomae/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6718 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/videomae/configuration_videomae.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13989 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/videomae/convert_videomae_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1200 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/videomae/feature_extraction_videomae.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17262 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/videomae/image_processing_videomae.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    46972 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/videomae/modeling_videomae.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.988431 llm-toys-0.1.0/llm_toys/hf/transformers/models/vilt/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2788 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vilt/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6929 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vilt/configuration_vilt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12870 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vilt/convert_vilt_original_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1172 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vilt/feature_extraction_vilt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21090 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vilt/image_processing_vilt.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    65187 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vilt/modeling_vilt.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6054 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vilt/processing_vilt.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.988431 llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_encoder_decoder/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2627 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_encoder_decoder/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8785 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_encoder_decoder/configuration_vision_encoder_decoder.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    41661 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_encoder_decoder/modeling_flax_vision_encoder_decoder.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    36960 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_encoder_decoder/modeling_tf_vision_encoder_decoder.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    35040 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_encoder_decoder/modeling_vision_encoder_decoder.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.988431 llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_text_dual_encoder/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2730 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_text_dual_encoder/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5289 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_text_dual_encoder/configuration_vision_text_dual_encoder.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    26682 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_text_dual_encoder/modeling_flax_vision_text_dual_encoder.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28773 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_text_dual_encoder/modeling_tf_vision_text_dual_encoder.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    25315 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_text_dual_encoder/modeling_vision_text_dual_encoder.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7010 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_text_dual_encoder/processing_vision_text_dual_encoder.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.988431 llm-toys-0.1.0/llm_toys/hf/transformers/models/visual_bert/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2235 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/visual_bert/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7942 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/visual_bert/configuration_visual_bert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5158 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/visual_bert/convert_visual_bert_original_pytorch_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    69820 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/visual_bert/modeling_visual_bert.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.988431 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3598 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5835 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/configuration_vit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8854 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/convert_dino_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10184 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/convert_vit_timm_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1165 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/feature_extraction_vit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13287 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/image_processing_vit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    25333 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/modeling_flax_vit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    31869 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/modeling_tf_vit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    35989 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/modeling_vit.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.992431 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_hybrid/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2316 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_hybrid/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7223 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_hybrid/configuration_vit_hybrid.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13413 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_hybrid/convert_vit_hybrid_timm_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16128 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_hybrid/image_processing_vit_hybrid.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    32287 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_hybrid/modeling_vit_hybrid.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.992431 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_mae/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2428 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_mae/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6568 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_mae/configuration_vit_mae.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7516 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_mae/convert_vit_mae_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    47226 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_mae/modeling_tf_vit_mae.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    43355 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_mae/modeling_vit_mae.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.992431 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_msn/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1783 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_msn/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5062 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_msn/configuration_vit_msn.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9841 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_msn/convert_msn_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    30091 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_msn/modeling_vit_msn.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.992431 llm-toys-0.1.0/llm_toys/hf/transformers/models/vivit/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2441 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vivit/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5368 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vivit/configuration_vivit.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9145 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vivit/convert_vivit_flax_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18469 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vivit/image_processing_vivit.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    28976 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/vivit/modeling_vivit.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.992431 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4139 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20142 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/configuration_wav2vec2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14293 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/convert_wav2vec2_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4838 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/convert_wav2vec2_original_s3prl_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11511 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/feature_extraction_wav2vec2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57331 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/modeling_flax_wav2vec2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    70405 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/modeling_tf_wav2vec2.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   106131 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/modeling_wav2vec2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7136 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/processing_wav2vec2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    41063 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/tokenization_wav2vec2.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.992431 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_conformer/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2375 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_conformer/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20919 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_conformer/configuration_wav2vec2_conformer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13382 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_conformer/convert_wav2vec2_conformer_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    95737 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_conformer/modeling_wav2vec2_conformer.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.992431 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_phoneme/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      993 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_phoneme/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    26089 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_phoneme/tokenization_wav2vec2_phoneme.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.992431 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_with_lm/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      981 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_with_lm/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    29648 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_with_lm/processing_wav2vec2_with_lm.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.996431 llm-toys-0.1.0/llm_toys/hf/transformers/models/wavlm/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1959 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wavlm/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18605 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wavlm/configuration_wavlm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8580 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wavlm/convert_wavlm_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4814 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wavlm/convert_wavlm_original_s3prl_checkpoint_to_pytorch.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    78999 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/wavlm/modeling_wavlm.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.996431 llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4284 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17052 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/configuration_whisper.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7602 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/convert_openai_to_hf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    22822 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/english_normalizer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12240 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/feature_extraction_whisper.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    72572 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/modeling_flax_whisper.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    77654 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/modeling_tf_whisper.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    93218 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/modeling_whisper.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3890 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/processing_whisper.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    49340 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/tokenization_whisper.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    26137 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/tokenization_whisper_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.996431 llm-toys-0.1.0/llm_toys/hf/transformers/models/x_clip/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2053 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/x_clip/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21041 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/x_clip/configuration_x_clip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18066 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/x_clip/convert_x_clip_original_pytorch_to_hf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    70568 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/x_clip/modeling_x_clip.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6872 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/x_clip/processing_x_clip.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.996431 llm-toys-0.1.0/llm_toys/hf/transformers/models/xglm/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3871 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xglm/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6055 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xglm/configuration_xglm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2325 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xglm/convert_xglm_original_ckpt_to_trfms.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    33123 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xglm/modeling_flax_xglm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    41806 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xglm/modeling_tf_xglm.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    40819 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xglm/modeling_xglm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13277 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xglm/tokenization_xglm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8033 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xglm/tokenization_xglm_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:36.000431 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3292 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11975 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm/configuration_xlm.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2934 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm/convert_xlm_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    51632 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm/modeling_tf_xlm.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    54911 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm/modeling_xlm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    34960 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm/tokenization_xlm.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:36.000431 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_prophetnet/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2615 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_prophetnet/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9125 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_prophetnet/configuration_xlm_prophetnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   118980 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_prophetnet/modeling_xlm_prophetnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13908 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_prophetnet/tokenization_xlm_prophetnet.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:36.000431 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5825 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8346 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta/configuration_xlm_roberta.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    58614 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta/modeling_flax_xlm_roberta.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    73898 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta/modeling_tf_xlm_roberta.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    72944 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta/modeling_xlm_roberta.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14285 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta/tokenization_xlm_roberta.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10264 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta/tokenization_xlm_roberta_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:36.000431 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta_xl/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2405 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta_xl/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7595 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta_xl/configuration_xlm_roberta_xl.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8228 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta_xl/convert_xlm_roberta_xl_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    68793 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta_xl/modeling_xlm_roberta_xl.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:36.000431 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlnet/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4288 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlnet/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11143 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlnet/configuration_xlnet.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     3688 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlnet/convert_xlnet_original_tf_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    73071 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlnet/modeling_tf_xlnet.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    92846 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlnet/modeling_xlnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16191 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlnet/tokenization_xlnet.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10026 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xlnet/tokenization_xlnet_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:36.000431 llm-toys-0.1.0/llm_toys/hf/transformers/models/xmod/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2325 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xmod/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10145 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xmod/configuration_xmod.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9859 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xmod/convert_xmod_original_pytorch_checkpoint_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    76513 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/xmod/modeling_xmod.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:36.000431 llm-toys-0.1.0/llm_toys/hf/transformers/models/yolos/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2400 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/yolos/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7790 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/yolos/configuration_yolos.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11259 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/yolos/convert_yolos_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1179 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/yolos/feature_extraction_yolos.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    52795 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/yolos/image_processing_yolos.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    58800 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/yolos/modeling_yolos.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:36.004431 llm-toys-0.1.0/llm_toys/hf/transformers/models/yoso/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2074 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/yoso/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6902 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/yoso/configuration_yoso.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4115 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/yoso/convert_yoso_pytorch_to_pytorch.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    55064 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/models/yoso/modeling_yoso.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:36.004431 llm-toys-0.1.0/llm_toys/hf/transformers/onnx/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1548 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/onnx/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9519 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/onnx/__main__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    32490 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/onnx/config.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21182 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/onnx/convert.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28264 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/onnx/features.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3625 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/onnx/utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    31638 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/optimization.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16583 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/optimization_tf.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:36.004431 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    46315 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8769 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/audio_classification.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8094 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/audio_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    35232 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/automatic_speech_recognition.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    51408 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/base.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13594 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/conversational.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4258 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/depth_estimation.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23079 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/document_question_answering.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4822 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/feature_extraction.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10691 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/fill_mask.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4940 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/image_classification.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8731 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/image_segmentation.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7138 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/image_to_text.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13291 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/mask_generation.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7441 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/object_detection.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12613 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/pt_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    29474 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/question_answering.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19892 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/table_question_answering.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16875 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/text2text_generation.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10043 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/text_classification.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15183 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/text_generation.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    26627 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/token_classification.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5008 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/video_classification.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5968 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/visual_question_answering.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6501 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/zero_shot_audio_classification.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11983 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/zero_shot_classification.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6075 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/zero_shot_image_classification.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9029 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/zero_shot_object_detection.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11968 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/processing_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11445 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/pytorch_utils.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:36.008431 llm-toys-0.1.0/llm_toys/hf/transformers/sagemaker/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      730 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/sagemaker/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1044 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/sagemaker/trainer_sm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5389 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/sagemaker/training_args_sm.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    68116 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/testing_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9571 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tf_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7520 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/time_series_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40143 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tokenization_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   182321 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tokenization_utils_base.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    33446 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tokenization_utils_fast.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:36.008431 llm-toys-0.1.0/llm_toys/hf/transformers/tools/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2955 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tools/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9093 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tools/agent_types.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    30304 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tools/agents.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    29957 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tools/base.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3337 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tools/document_question_answering.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24739 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tools/evaluate_agent.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1745 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tools/image_captioning.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1969 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tools/image_question_answering.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2102 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tools/image_segmentation.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1558 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tools/prompts.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9959 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tools/python_interpreter.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1482 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tools/speech_to_text.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2475 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tools/text_classification.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1967 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tools/text_question_answering.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1691 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tools/text_summarization.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2424 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tools/text_to_speech.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8493 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/tools/translation.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   185736 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/trainer.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24051 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/trainer_callback.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    47809 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/trainer_pt_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15722 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/trainer_seq2seq.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    34629 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/trainer_tf.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24147 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/trainer_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   126983 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/training_args.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4484 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/training_args_seq2seq.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14388 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/training_args_tf.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:36.012431 llm-toys-0.1.0/llm_toys/hf/transformers/utils/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6572 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12027 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/backbone_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13391 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/bitsandbytes.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      282 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/constants.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40011 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/doc.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      391 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/dummy_detectron2_objects.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    30740 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/dummy_flax_objects.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      294 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/dummy_keras_nlp_objects.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   193887 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/dummy_pt_objects.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      286 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/dummy_sentencepiece_and_tokenizers_objects.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5575 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/dummy_sentencepiece_objects.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      465 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/dummy_speech_objects.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      306 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/dummy_tensorflow_text_objects.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    67038 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/dummy_tf_objects.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10241 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/dummy_tokenizers_objects.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12566 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/dummy_vision_objects.py
--rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    47792 2023-07-16 03:26:07.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/fx.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18320 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/generic.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4979 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/hp_naming.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    49100 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/hub.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    39906 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/import_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10168 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/logging.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2272 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/model_parallel_utils.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14831 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/notebook.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12238 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/quantization_config.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    50671 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/sentencepiece_model_pb2.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6621 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/sentencepiece_model_pb2_new.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4333 2023-07-15 14:04:29.000000 llm-toys-0.1.0/llm_toys/hf/transformers/utils/versions.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      935 2023-07-16 13:26:36.000000 llm-toys-0.1.0/llm_toys/prompts.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:36.012431 llm-toys-0.1.0/llm_toys/tasks/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      210 2023-07-17 10:11:26.000000 llm-toys-0.1.0/llm_toys/tasks/__init__.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5749 2023-07-17 10:44:34.000000 llm-toys-0.1.0/llm_toys/tasks/all_tasks.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3281 2023-07-17 10:45:38.000000 llm-toys-0.1.0/llm_toys/tasks/paraphrase.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3893 2023-07-16 13:17:26.000000 llm-toys-0.1.0/llm_toys/tasks/predict.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4416 2023-07-17 10:47:13.000000 llm-toys-0.1.0/llm_toys/tasks/summary_topic.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8968 2023-07-17 09:26:46.000000 llm-toys-0.1.0/llm_toys/train.py
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3126 2023-07-17 04:11:06.000000 llm-toys-0.1.0/llm_toys/utils.py
-drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:24:35.848430 llm-toys-0.1.0/llm_toys.egg-info/
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6908 2023-07-17 11:24:35.000000 llm-toys-0.1.0/llm_toys.egg-info/PKG-INFO
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    87698 2023-07-17 11:24:35.000000 llm-toys-0.1.0/llm_toys.egg-info/SOURCES.txt
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        1 2023-07-17 11:24:35.000000 llm-toys-0.1.0/llm_toys.egg-info/dependency_links.txt
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1514 2023-07-17 11:24:35.000000 llm-toys-0.1.0/llm_toys.egg-info/requires.txt
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        9 2023-07-17 11:24:35.000000 llm-toys-0.1.0/llm_toys.egg-info/top_level.txt
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)       89 2023-07-15 06:02:36.000000 llm-toys-0.1.0/pyproject.toml
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)       38 2023-07-17 11:24:36.012431 llm-toys-0.1.0/setup.cfg
--rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1431 2023-07-17 11:08:43.000000 llm-toys-0.1.0/setup.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.473569 llm-toys-0.1.1/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6908 2023-07-17 11:27:36.473569 llm-toys-0.1.1/PKG-INFO
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6545 2023-07-17 11:03:23.000000 llm-toys-0.1.1/README.md
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.325568 llm-toys-0.1.1/llm_toys/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      518 2023-07-17 11:27:22.000000 llm-toys-0.1.1/llm_toys/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1762 2023-07-17 10:05:14.000000 llm-toys-0.1.1/llm_toys/config.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3879 2023-07-17 09:13:47.000000 llm-toys-0.1.1/llm_toys/eval.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.329568 llm-toys-0.1.1/llm_toys/hf/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 14:32:56.000000 llm-toys-0.1.1/llm_toys/hf/__init__.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.329568 llm-toys-0.1.1/llm_toys/hf/peft/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2163 2023-07-15 14:04:38.000000 llm-toys-0.1.1/llm_toys/hf/peft/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5535 2023-07-15 14:04:38.000000 llm-toys-0.1.1/llm_toys/hf/peft/auto.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      877 2023-07-15 14:04:38.000000 llm-toys-0.1.1/llm_toys/hf/peft/import_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3224 2023-07-15 14:04:38.000000 llm-toys-0.1.1/llm_toys/hf/peft/mapping.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    74724 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/peft/peft_model.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.329568 llm-toys-0.1.1/llm_toys/hf/peft/tuners/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1217 2023-07-15 14:04:38.000000 llm-toys-0.1.1/llm_toys/hf/peft/tuners/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    33370 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/peft/tuners/adalora.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16325 2023-07-15 14:04:38.000000 llm-toys-0.1.1/llm_toys/hf/peft/tuners/adaption_prompt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    22782 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/peft/tuners/ia3.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    48122 2023-07-15 14:04:38.000000 llm-toys-0.1.1/llm_toys/hf/peft/tuners/lora.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6755 2023-07-15 14:04:38.000000 llm-toys-0.1.1/llm_toys/hf/peft/tuners/p_tuning.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3785 2023-07-15 14:04:38.000000 llm-toys-0.1.1/llm_toys/hf/peft/tuners/prefix_tuning.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4935 2023-07-15 14:04:38.000000 llm-toys-0.1.1/llm_toys/hf/peft/tuners/prompt_tuning.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.329568 llm-toys-0.1.1/llm_toys/hf/peft/utils/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1734 2023-07-15 14:04:38.000000 llm-toys-0.1.1/llm_toys/hf/peft/utils/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8845 2023-07-15 14:04:38.000000 llm-toys-0.1.1/llm_toys/hf/peft/utils/config.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1118 2023-07-15 14:04:38.000000 llm-toys-0.1.1/llm_toys/hf/peft/utils/hub_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13087 2023-07-15 14:04:38.000000 llm-toys-0.1.1/llm_toys/hf/peft/utils/other.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6098 2023-07-15 14:04:38.000000 llm-toys-0.1.1/llm_toys/hf/peft/utils/save_and_load.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.337568 llm-toys-0.1.1/llm_toys/hf/transformers/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   279202 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8783 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/activations.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4313 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/activations_tf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    30854 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/audio_utils.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.337568 llm-toys-0.1.1/llm_toys/hf/transformers/benchmark/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/benchmark/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10752 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/benchmark/benchmark.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3890 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/benchmark/benchmark_args.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4735 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/benchmark/benchmark_args_tf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6475 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/benchmark/benchmark_args_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13251 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/benchmark/benchmark_tf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    37600 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/benchmark/benchmark_utils.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.337568 llm-toys-0.1.1/llm_toys/hf/transformers/commands/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      923 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/commands/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11062 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/commands/add_new_model.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    70769 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/commands/add_new_model_like.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7852 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/commands/convert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2373 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/commands/download.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5316 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/commands/env.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8001 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/commands/lfs.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20540 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/commands/pt_to_tf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4249 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/commands/run.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8026 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/commands/serving.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6307 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/commands/train.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2047 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/commands/transformers_cli.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7124 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/commands/user.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    51951 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/configuration_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20903 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/convert_graph_to_onnx.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    16631 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/convert_pytorch_checkpoint_to_tf2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    52391 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/convert_slow_tokenizer.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     4982 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/convert_slow_tokenizers_checkpoints_to_fast.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2899 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/convert_tf_hub_seq_to_seq_bert_to_pytorch.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.337568 llm-toys-0.1.1/llm_toys/hf/transformers/data/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1423 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/data/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    76822 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/data/data_collator.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.337568 llm-toys-0.1.1/llm_toys/hf/transformers/data/datasets/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      909 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/data/datasets/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6149 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/data/datasets/glue.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23675 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/data/datasets/language_modeling.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9205 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/data/datasets/squad.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.337568 llm-toys-0.1.1/llm_toys/hf/transformers/data/metrics/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3632 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/data/metrics/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    29676 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/data/metrics/squad_metrics.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.341568 llm-toys-0.1.1/llm_toys/hf/transformers/data/processors/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1014 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/data/processors/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23219 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/data/processors/glue.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    33153 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/data/processors/squad.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13829 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/data/processors/utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3489 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/data/processors/xnli.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12907 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/debug_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16966 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/deepspeed.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2115 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/dependency_versions_check.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3167 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/dependency_versions_table.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24465 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/dynamic_module_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18215 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/feature_extraction_sequence_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28136 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/feature_extraction_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3574 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/file_utils.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.341568 llm-toys-0.1.1/llm_toys/hf/transformers/generation/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9515 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/generation/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19089 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/generation/beam_constraints.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    45955 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/generation/beam_search.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40270 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/generation/configuration_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19218 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/generation/flax_logits_process.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    49014 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/generation/flax_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    54715 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/generation/logits_process.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6373 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/generation/stopping_criteria.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9145 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/generation/streamers.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28136 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/generation/tf_logits_process.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   177842 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/generation/tf_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   251955 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/generation/utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1118 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/generation_flax_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1109 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/generation_tf_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1126 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/generation_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19745 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/hf_argparser.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4161 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/hyperparameter_search.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    26885 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/image_processing_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    30960 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/image_transforms.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24006 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/image_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    71566 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/integrations.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20843 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/keras_callbacks.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    35232 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/modelcard.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    41961 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/modeling_flax_outputs.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19529 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/modeling_flax_pytorch_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    56460 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/modeling_flax_utils.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   106127 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/modeling_outputs.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    56074 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/modeling_tf_outputs.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24772 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/modeling_tf_pytorch_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   160782 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/modeling_tf_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   191059 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/modeling_utils.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.341568 llm-toys-0.1.1/llm_toys/hf/transformers/models/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3559 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/__init__.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.341568 llm-toys-0.1.1/llm_toys/hf/transformers/models/albert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5482 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/albert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8568 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/albert/configuration_albert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2162 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/albert/convert_albert_original_tf_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    60616 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/albert/modeling_albert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40772 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/albert/modeling_flax_albert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    61857 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/albert/modeling_tf_albert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15429 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/albert/tokenization_albert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10815 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/albert/tokenization_albert_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.341568 llm-toys-0.1.1/llm_toys/hf/transformers/models/align/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2064 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/align/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18805 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/align/configuration_align.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15524 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/align/convert_align_tf_to_hf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    72060 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/align/modeling_align.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6216 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/align/processing_align.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.341568 llm-toys-0.1.1/llm_toys/hf/transformers/models/altclip/
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2126 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/altclip/__init__.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    19664 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/altclip/configuration_altclip.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    78788 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/altclip/modeling_altclip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6477 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/altclip/processing_altclip.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.341568 llm-toys-0.1.1/llm_toys/hf/transformers/models/audio_spectrogram_transformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2507 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/audio_spectrogram_transformer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5650 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/audio_spectrogram_transformer/configuration_audio_spectrogram_transformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11052 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/audio_spectrogram_transformer/convert_audio_spectrogram_transformer_original_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8614 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/audio_spectrogram_transformer/feature_extraction_audio_spectrogram_transformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    26449 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/audio_spectrogram_transformer/modeling_audio_spectrogram_transformer.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.345568 llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15846 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40272 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/auto_factory.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    44362 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/configuration_auto.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18500 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/feature_extraction_auto.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19917 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/image_processing_auto.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    57917 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/modeling_auto.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14128 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/modeling_flax_auto.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    27835 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/modeling_tf_auto.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15201 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/processing_auto.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    39830 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/tokenization_auto.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.345568 llm-toys-0.1.1/llm_toys/hf/transformers/models/autoformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1914 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/autoformer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12325 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/autoformer/configuration_autoformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   109505 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/autoformer/modeling_autoformer.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.345568 llm-toys-0.1.1/llm_toys/hf/transformers/models/bart/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4333 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bart/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18993 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bart/configuration_bart.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6055 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bart/convert_bart_original_pytorch_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    90105 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bart/modeling_bart.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    82723 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bart/modeling_flax_bart.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    74717 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bart/modeling_tf_bart.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17981 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bart/tokenization_bart.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13812 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bart/tokenization_bart_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.345568 llm-toys-0.1.1/llm_toys/hf/transformers/models/barthez/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1848 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/barthez/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13193 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/barthez/tokenization_barthez.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8900 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/barthez/tokenization_barthez_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.345568 llm-toys-0.1.1/llm_toys/hf/transformers/models/bartpho/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1362 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bartpho/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14219 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bartpho/tokenization_bartpho.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.345568 llm-toys-0.1.1/llm_toys/hf/transformers/models/beit/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3289 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/beit/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9641 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/beit/configuration_beit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16480 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/beit/convert_beit_unilm_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1172 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/beit/feature_extraction_beit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24407 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/beit/image_processing_beit.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    54268 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/beit/modeling_beit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    36989 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/beit/modeling_flax_beit.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.349568 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6057 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10150 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/configuration_bert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10490 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/convert_bert_original_tf2_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2159 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/convert_bert_original_tf_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4098 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/convert_bert_pytorch_checkpoint_to_original_tf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7606 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/convert_bert_token_dropping_original_tf2_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    83947 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/modeling_bert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    63604 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/modeling_flax_bert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    85690 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/modeling_tf_bert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    25078 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/tokenization_bert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14871 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/tokenization_bert_fast.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11798 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/tokenization_bert_tf.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.349568 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert_generation/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2275 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert_generation/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6228 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert_generation/configuration_bert_generation.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    47874 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert_generation/modeling_bert_generation.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7140 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert_generation/tokenization_bert_generation.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.349568 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert_japanese/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1053 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert_japanese/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40187 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bert_japanese/tokenization_bert_japanese.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.349568 llm-toys-0.1.1/llm_toys/hf/transformers/models/bertweet/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      959 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bertweet/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    27220 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bertweet/tokenization_bertweet.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.349568 llm-toys-0.1.1/llm_toys/hf/transformers/models/big_bird/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4574 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/big_bird/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8306 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/big_bird/configuration_big_bird.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2493 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/big_bird/convert_bigbird_original_tf_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   142285 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/big_bird/modeling_big_bird.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   109507 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/big_bird/modeling_flax_big_bird.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14885 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/big_bird/tokenization_big_bird.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11355 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/big_bird/tokenization_big_bird_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.349568 llm-toys-0.1.1/llm_toys/hf/transformers/models/bigbird_pegasus/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2316 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bigbird_pegasus/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19802 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bigbird_pegasus/configuration_bigbird_pegasus.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6288 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bigbird_pegasus/convert_bigbird_pegasus_tf_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   147915 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bigbird_pegasus/modeling_bigbird_pegasus.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.349568 llm-toys-0.1.1/llm_toys/hf/transformers/models/biogpt/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2058 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/biogpt/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6390 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/biogpt/configuration_biogpt.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    10578 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/biogpt/convert_biogpt_original_pytorch_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    43239 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/biogpt/modeling_biogpt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13723 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/biogpt/tokenization_biogpt.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.349568 llm-toys-0.1.1/llm_toys/hf/transformers/models/bit/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2244 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bit/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6236 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bit/configuration_bit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5955 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bit/convert_bit_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16108 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bit/image_processing_bit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    32019 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bit/modeling_bit.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.349568 llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4031 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19016 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot/configuration_blenderbot.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3702 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot/convert_blenderbot_original_pytorch_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    77177 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot/modeling_blenderbot.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    65012 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot/modeling_flax_blenderbot.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    67823 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot/modeling_tf_blenderbot.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19488 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot/tokenization_blenderbot.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14205 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot/tokenization_blenderbot_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.353568 llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot_small/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4263 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot_small/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18479 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot_small/configuration_blenderbot_small.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    75970 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot_small/modeling_blenderbot_small.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    65958 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot_small/modeling_flax_blenderbot_small.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    67121 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot_small/modeling_tf_blenderbot_small.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8641 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot_small/tokenization_blenderbot_small.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4058 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot_small/tokenization_blenderbot_small_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.353568 llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3692 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17118 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/configuration_blip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6980 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/convert_blip_original_pytorch_to_hf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14112 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/image_processing_blip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    61776 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/modeling_blip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    43338 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/modeling_blip_text.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    65275 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/modeling_tf_blip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    42406 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/modeling_tf_blip_text.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6204 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/processing_blip.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.353568 llm-toys-0.1.1/llm_toys/hf/transformers/models/blip_2/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2153 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blip_2/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17275 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blip_2/configuration_blip_2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12330 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blip_2/convert_blip_2_original_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    81996 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blip_2/modeling_blip_2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6698 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/blip_2/processing_blip_2.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.353568 llm-toys-0.1.1/llm_toys/hf/transformers/models/bloom/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2499 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bloom/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10758 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bloom/configuration_bloom.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10302 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bloom/convert_bloom_original_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    56945 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bloom/modeling_bloom.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7389 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bloom/tokenization_bloom_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.353568 llm-toys-0.1.1/llm_toys/hf/transformers/models/bridgetower/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2864 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bridgetower/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17056 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bridgetower/configuration_bridgetower.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    22800 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bridgetower/image_processing_bridgetower.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    88379 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bridgetower/modeling_bridgetower.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5056 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/bridgetower/processing_bridgetower.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.353568 llm-toys-0.1.1/llm_toys/hf/transformers/models/byt5/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      942 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/byt5/__init__.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2120 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/byt5/convert_byt5_original_tf_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10727 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/byt5/tokenization_byt5.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.353568 llm-toys-0.1.1/llm_toys/hf/transformers/models/camembert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4443 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/camembert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7735 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/camembert/configuration_camembert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    72469 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/camembert/modeling_camembert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    73463 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/camembert/modeling_tf_camembert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13581 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/camembert/tokenization_camembert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8658 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/camembert/tokenization_camembert_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.357568 llm-toys-0.1.1/llm_toys/hf/transformers/models/canine/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2272 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/canine/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6478 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/canine/configuration_canine.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2117 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/canine/convert_canine_original_tf_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    73763 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/canine/modeling_canine.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9276 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/canine/tokenization_canine.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.357568 llm-toys-0.1.1/llm_toys/hf/transformers/models/chinese_clip/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2919 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/chinese_clip/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    22588 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/chinese_clip/configuration_chinese_clip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5069 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/chinese_clip/convert_chinese_clip_original_pytorch_to_hf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1247 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/chinese_clip/feature_extraction_chinese_clip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15758 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/chinese_clip/image_processing_chinese_clip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    73599 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/chinese_clip/modeling_chinese_clip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6787 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/chinese_clip/processing_chinese_clip.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.357568 llm-toys-0.1.1/llm_toys/hf/transformers/models/clap/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2322 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clap/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21201 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clap/configuration_clap.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4695 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clap/convert_clap_original_pytorch_to_hf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18653 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clap/feature_extraction_clap.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   105313 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clap/modeling_clap.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5704 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clap/processing_clap.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.357568 llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5027 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21049 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/configuration_clip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5306 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/convert_clip_original_pytorch_to_hf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1172 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/feature_extraction_clip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16139 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/image_processing_clip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57071 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/modeling_clip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    45844 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/modeling_flax_clip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    53459 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/modeling_tf_clip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6854 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/processing_clip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21029 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/tokenization_clip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6956 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/tokenization_clip_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.357568 llm-toys-0.1.1/llm_toys/hf/transformers/models/clipseg/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2179 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clipseg/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21241 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clipseg/configuration_clipseg.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11114 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clipseg/convert_clipseg_original_pytorch_to_hf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    65133 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clipseg/modeling_clipseg.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7871 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/clipseg/processing_clipseg.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.357568 llm-toys-0.1.1/llm_toys/hf/transformers/models/codegen/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2443 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/codegen/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10324 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/codegen/configuration_codegen.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    31450 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/codegen/modeling_codegen.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15219 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/codegen/tokenization_codegen.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10614 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/codegen/tokenization_codegen_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.361568 llm-toys-0.1.1/llm_toys/hf/transformers/models/conditional_detr/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2828 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/conditional_detr/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12973 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/conditional_detr/configuration_conditional_detr.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15930 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/conditional_detr/convert_conditional_detr_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1251 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/conditional_detr/feature_extraction_conditional_detr.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    70534 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/conditional_detr/image_processing_conditional_detr.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   127751 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/conditional_detr/modeling_conditional_detr.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.361568 llm-toys-0.1.1/llm_toys/hf/transformers/models/convbert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4069 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convbert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7311 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convbert/configuration_convbert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2108 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convbert/convert_convbert_original_tf1_checkpoint_to_pytorch_and_tf2.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    58732 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convbert/modeling_convbert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    52625 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convbert/modeling_tf_convbert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21870 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convbert/tokenization_convbert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8765 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convbert/tokenization_convbert_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.361568 llm-toys-0.1.1/llm_toys/hf/transformers/models/convnext/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3150 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convnext/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6201 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convnext/configuration_convnext.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10220 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convnext/convert_convnext_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1200 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convnext/feature_extraction_convnext.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15054 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convnext/image_processing_convnext.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    22149 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convnext/modeling_convnext.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23306 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convnext/modeling_tf_convnext.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.361568 llm-toys-0.1.1/llm_toys/hf/transformers/models/convnextv2/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2159 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convnextv2/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5430 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convnextv2/configuration_convnextv2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12473 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convnextv2/convert_convnextv2_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23932 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/convnextv2/modeling_convnextv2.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.361568 llm-toys-0.1.1/llm_toys/hf/transformers/models/cpm/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1816 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/cpm/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15154 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/cpm/tokenization_cpm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10680 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/cpm/tokenization_cpm_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.361568 llm-toys-0.1.1/llm_toys/hf/transformers/models/cpmant/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2117 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/cpmant/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5329 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/cpmant/configuration_cpmant.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    37709 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/cpmant/modeling_cpmant.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10079 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/cpmant/tokenization_cpmant.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.361568 llm-toys-0.1.1/llm_toys/hf/transformers/models/ctrl/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2688 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/ctrl/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4738 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/ctrl/configuration_ctrl.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    34910 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/ctrl/modeling_ctrl.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    36036 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/ctrl/modeling_tf_ctrl.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8491 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/ctrl/tokenization_ctrl.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.361568 llm-toys-0.1.1/llm_toys/hf/transformers/models/cvt/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2434 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/cvt/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6860 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/cvt/configuration_cvt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13570 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/cvt/convert_cvt_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28913 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/cvt/modeling_cvt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    36051 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/cvt/modeling_tf_cvt.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.365568 llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4933 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16436 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/configuration_data2vec_audio.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7420 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/configuration_data2vec_text.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9432 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/configuration_data2vec_vision.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10858 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/convert_data2vec_audio_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9580 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/convert_data2vec_text_original_pytorch_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    15340 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/convert_data2vec_vision_original_pytorch_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    65709 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/modeling_data2vec_audio.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    71169 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/modeling_data2vec_text.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    53184 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/modeling_data2vec_vision.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    60423 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/modeling_tf_data2vec_vision.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.365568 llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3677 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9389 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta/configuration_deberta.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    58332 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta/modeling_deberta.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    60370 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta/modeling_tf_deberta.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19801 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta/tokenization_deberta.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13437 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta/tokenization_deberta_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.365568 llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta_v2/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3899 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta_v2/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9175 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta_v2/configuration_deberta_v2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    67935 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta_v2/modeling_deberta_v2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    66544 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta_v2/modeling_tf_deberta_v2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21720 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta_v2/tokenization_deberta_v2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10997 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta_v2/tokenization_deberta_v2_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.365568 llm-toys-0.1.1/llm_toys/hf/transformers/models/decision_transformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2124 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/decision_transformer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7321 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/decision_transformer/configuration_decision_transformer.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    43327 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/decision_transformer/modeling_decision_transformer.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.365568 llm-toys-0.1.1/llm_toys/hf/transformers/models/deformable_detr/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2599 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deformable_detr/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14244 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deformable_detr/configuration_deformable_detr.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9477 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deformable_detr/convert_deformable_detr_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1244 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deformable_detr/feature_extraction_deformable_detr.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57980 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deformable_detr/image_processing_deformable_detr.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1559 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deformable_detr/load_custom.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   119564 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deformable_detr/modeling_deformable_detr.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.365568 llm-toys-0.1.1/llm_toys/hf/transformers/models/deit/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3486 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deit/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5961 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deit/configuration_deit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9217 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deit/convert_deit_timm_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1172 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deit/feature_extraction_deit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14866 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deit/image_processing_deit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    38581 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deit/modeling_deit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    42421 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deit/modeling_tf_deit.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.365568 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/__init__.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.365568 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/bort/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/bort/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14057 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/bort/convert_bort_original_gluonnlp_checkpoint_to_pytorch.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.369568 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mctct/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1892 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mctct/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9308 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mctct/configuration_mctct.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13460 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mctct/feature_extraction_mctct.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    33784 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mctct/modeling_mctct.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5929 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mctct/processing_mctct.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.369568 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mmbt/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1480 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mmbt/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1606 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mmbt/configuration_mmbt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18890 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mmbt/modeling_mmbt.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.369568 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/retribert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2351 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/retribert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5407 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/retribert/configuration_retribert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9465 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/retribert/modeling_retribert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    22586 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/retribert/tokenization_retribert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9017 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/retribert/tokenization_retribert_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.369568 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/tapex/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      926 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/tapex/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    65003 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/tapex/tokenization_tapex.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.369568 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2077 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7413 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/configuration_trajectory_transformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3139 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/convert_trajectory_transformer_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    26203 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/modeling_trajectory_transformer.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.369568 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/van/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1728 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/van/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4837 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/van/configuration_van.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10363 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/van/convert_van_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21576 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/van/modeling_van.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.369568 llm-toys-0.1.1/llm_toys/hf/transformers/models/deta/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2205 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deta/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11931 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deta/configuration_deta.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16833 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deta/convert_deta_resnet_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19031 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deta/convert_deta_swin_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    42393 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deta/image_processing_deta.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   135049 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/deta/modeling_deta.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.369568 llm-toys-0.1.1/llm_toys/hf/transformers/models/detr/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2438 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/detr/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13243 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/detr/configuration_detr.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13561 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/detr/convert_detr_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18993 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/detr/convert_detr_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1172 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/detr/feature_extraction_detr.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    78319 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/detr/image_processing_detr.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   111497 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/detr/modeling_detr.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.369568 llm-toys-0.1.1/llm_toys/hf/transformers/models/dialogpt/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dialogpt/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1537 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dialogpt/convert_dialogpt_original_pytorch_checkpoint_to_pytorch.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.369568 llm-toys-0.1.1/llm_toys/hf/transformers/models/dinat/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1812 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dinat/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7399 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dinat/configuration_dinat.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    41810 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dinat/modeling_dinat.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.373568 llm-toys-0.1.1/llm_toys/hf/transformers/models/distilbert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5167 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/distilbert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6978 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/distilbert/configuration_distilbert.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    51793 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/distilbert/modeling_distilbert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    32621 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/distilbert/modeling_flax_distilbert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    42933 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/distilbert/modeling_tf_distilbert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23599 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/distilbert/tokenization_distilbert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10708 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/distilbert/tokenization_distilbert_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.373568 llm-toys-0.1.1/llm_toys/hf/transformers/models/dit/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        0 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dit/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9420 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dit/convert_dit_unilm_to_pytorch.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.373568 llm-toys-0.1.1/llm_toys/hf/transformers/models/donut/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2455 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/donut/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5981 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/donut/configuration_donut_swin.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9316 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/donut/convert_donut_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1179 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/donut/feature_extraction_donut.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19857 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/donut/image_processing_donut.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    43709 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/donut/modeling_donut_swin.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8095 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/donut/processing_donut.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.373568 llm-toys-0.1.1/llm_toys/hf/transformers/models/dpr/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4535 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dpr/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7262 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dpr/configuration_dpr.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6096 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dpr/convert_dpr_original_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28581 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dpr/modeling_dpr.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    31966 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dpr/modeling_tf_dpr.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19789 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dpr/tokenization_dpr.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20175 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dpr/tokenization_dpr_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.373568 llm-toys-0.1.1/llm_toys/hf/transformers/models/dpt/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2444 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dpt/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11302 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dpt/configuration_dpt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12994 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dpt/convert_dpt_hybrid_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11781 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dpt/convert_dpt_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1165 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dpt/feature_extraction_dpt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18212 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dpt/image_processing_dpt.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    54912 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/dpt/modeling_dpt.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.373568 llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3550 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientformer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7919 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientformer/configuration_efficientformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9381 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientformer/convert_efficientformer_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16416 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientformer/image_processing_efficientformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    33848 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientformer/modeling_efficientformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40444 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientformer/modeling_tf_efficientformer.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.373568 llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientnet/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2670 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientnet/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7750 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientnet/configuration_efficientnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12756 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientnet/convert_efficientnet_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16724 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientnet/image_processing_efficientnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24389 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientnet/modeling_efficientnet.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.377568 llm-toys-0.1.1/llm_toys/hf/transformers/models/electra/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5257 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/electra/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9927 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/electra/configuration_electra.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2862 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/electra/convert_electra_original_tf_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    75769 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/electra/modeling_electra.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    62265 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/electra/modeling_flax_electra.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    69406 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/electra/modeling_tf_electra.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    22677 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/electra/tokenization_electra.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10495 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/electra/tokenization_electra_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.377568 llm-toys-0.1.1/llm_toys/hf/transformers/models/encodec/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1910 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/encodec/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8749 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/encodec/configuration_encodec.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15253 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/encodec/convert_encodec_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9873 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/encodec/feature_extraction_encodec.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    33479 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/encodec/modeling_encodec.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.377568 llm-toys-0.1.1/llm_toys/hf/transformers/models/encoder_decoder/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2451 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/encoder_decoder/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4840 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/encoder_decoder/configuration_encoder_decoder.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    35803 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/encoder_decoder/modeling_encoder_decoder.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    43812 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/encoder_decoder/modeling_flax_encoder_decoder.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    34302 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/encoder_decoder/modeling_tf_encoder_decoder.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.377568 llm-toys-0.1.1/llm_toys/hf/transformers/models/ernie/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2331 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/ernie/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8884 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/ernie/configuration_ernie.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    84083 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/ernie/modeling_ernie.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.377568 llm-toys-0.1.1/llm_toys/hf/transformers/models/ernie_m/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2637 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/ernie_m/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6190 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/ernie_m/configuration_ernie_m.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    47827 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/ernie_m/modeling_ernie_m.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17113 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/ernie_m/tokenization_ernie_m.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.377568 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2978 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14558 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/configuration_esm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18476 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/convert_esm.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    55911 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/modeling_esm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    86749 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/modeling_esmfold.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    60870 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/modeling_tf_esm.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.381568 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      446 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14392 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/chunk_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3764 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/data_transforms.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8376 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/feats.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3705 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/loss.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11490 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/protein.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    37993 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/residue_constants.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    41122 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/rigid_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4798 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/tensor_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6015 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/tokenization_esm.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.381568 llm-toys-0.1.1/llm_toys/hf/transformers/models/falcon/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2067 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/falcon/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6683 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/falcon/configuration_falcon.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    56890 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/falcon/modeling_falcon.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.381568 llm-toys-0.1.1/llm_toys/hf/transformers/models/flaubert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3488 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/flaubert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11706 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/flaubert/configuration_flaubert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57659 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/flaubert/modeling_flaubert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    52304 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/flaubert/modeling_tf_flaubert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24019 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/flaubert/tokenization_flaubert.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.381568 llm-toys-0.1.1/llm_toys/hf/transformers/models/flava/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3030 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/flava/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    37956 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/flava/configuration_flava.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3428 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/flava/convert_dalle_to_flava_codebook.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4372 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/flava/convert_flava_original_pytorch_to_hf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1201 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/flava/feature_extraction_flava.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    36878 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/flava/image_processing_flava.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    96717 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/flava/modeling_flava.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6807 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/flava/processing_flava.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.381568 llm-toys-0.1.1/llm_toys/hf/transformers/models/fnet/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3179 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/fnet/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5839 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/fnet/configuration_fnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6912 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/fnet/convert_fnet_original_flax_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    49473 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/fnet/modeling_fnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15847 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/fnet/tokenization_fnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8558 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/fnet/tokenization_fnet_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.381568 llm-toys-0.1.1/llm_toys/hf/transformers/models/focalnet/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1989 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/focalnet/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8013 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/focalnet/configuration_focalnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9450 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/focalnet/convert_focalnet_to_hf_format.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    43585 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/focalnet/modeling_focalnet.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.381568 llm-toys-0.1.1/llm_toys/hf/transformers/models/fsmt/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1675 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/fsmt/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10579 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/fsmt/configuration_fsmt.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    11264 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/fsmt/convert_fsmt_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    58083 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/fsmt/modeling_fsmt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20127 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/fsmt/tokenization_fsmt.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.385568 llm-toys-0.1.1/llm_toys/hf/transformers/models/funnel/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4126 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/funnel/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8894 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/funnel/configuration_funnel.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2335 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/funnel/convert_funnel_original_tf_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    69831 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/funnel/modeling_funnel.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    73093 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/funnel/modeling_tf_funnel.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24023 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/funnel/tokenization_funnel.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11794 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/funnel/tokenization_funnel_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.385568 llm-toys-0.1.1/llm_toys/hf/transformers/models/git/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1888 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/git/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11822 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/git/configuration_git.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21976 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/git/convert_git_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    69494 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/git/modeling_git.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5486 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/git/processing_git.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.385568 llm-toys-0.1.1/llm_toys/hf/transformers/models/glpn/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2384 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/glpn/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6183 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/glpn/configuration_glpn.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8558 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/glpn/convert_glpn_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1172 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/glpn/feature_extraction_glpn.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8864 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/glpn/image_processing_glpn.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    31527 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/glpn/modeling_glpn.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.385568 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4674 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12134 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/configuration_gpt2.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2532 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/convert_gpt2_original_tf_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    31960 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/modeling_flax_gpt2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    76173 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/modeling_gpt2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    51678 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/modeling_tf_gpt2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14425 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/tokenization_gpt2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8054 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/tokenization_gpt2_fast.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3763 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/tokenization_gpt2_tf.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.385568 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_bigcode/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2037 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_bigcode/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6448 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_bigcode/configuration_gpt_bigcode.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    48056 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_bigcode/modeling_gpt_bigcode.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.385568 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neo/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2718 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neo/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12058 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neo/configuration_gpt_neo.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2589 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neo/convert_gpt_neo_mesh_tf_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28080 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neo/modeling_flax_gpt_neo.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    47983 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neo/modeling_gpt_neo.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.385568 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2595 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8824 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox/configuration_gpt_neox.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    51180 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox/modeling_gpt_neox.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5797 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox/tokenization_gpt_neox_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.385568 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox_japanese/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2154 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox_japanese/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5729 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox_japanese/configuration_gpt_neox_japanese.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    32308 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox_japanese/modeling_gpt_neox_japanese.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17328 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox_japanese/tokenization_gpt_neox_japanese.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.385568 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_sw3/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1361 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_sw3/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8156 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_sw3/convert_megatron_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14759 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_sw3/tokenization_gpt_sw3.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.389568 llm-toys-0.1.1/llm_toys/hf/transformers/models/gptj/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3280 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gptj/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8996 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gptj/configuration_gptj.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28517 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gptj/modeling_flax_gptj.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    49873 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gptj/modeling_gptj.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    44030 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gptj/modeling_tf_gptj.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.389568 llm-toys-0.1.1/llm_toys/hf/transformers/models/gptsan_japanese/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2294 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gptsan_japanese/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7329 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gptsan_japanese/configuration_gptsan_japanese.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9793 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gptsan_japanese/convert_gptsan_tf_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    67099 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gptsan_japanese/modeling_gptsan_japanese.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24556 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/gptsan_japanese/tokenization_gptsan_japanese.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.389568 llm-toys-0.1.1/llm_toys/hf/transformers/models/graphormer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1873 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/graphormer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6086 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/graphormer/collating_graphormer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10401 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/graphormer/configuration_graphormer.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    37407 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/graphormer/modeling_graphormer.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.389568 llm-toys-0.1.1/llm_toys/hf/transformers/models/groupvit/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2875 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/groupvit/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21413 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/groupvit/configuration_groupvit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9775 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/groupvit/convert_groupvit_nvlab_to_hf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    68613 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/groupvit/modeling_groupvit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    77841 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/groupvit/modeling_tf_groupvit.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.389568 llm-toys-0.1.1/llm_toys/hf/transformers/models/herbert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1472 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/herbert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    25665 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/herbert/tokenization_herbert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6549 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/herbert/tokenization_herbert_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.389568 llm-toys-0.1.1/llm_toys/hf/transformers/models/hubert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2536 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/hubert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14760 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/hubert/configuration_hubert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8942 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/hubert/convert_distilhubert_original_s3prl_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10380 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/hubert/convert_hubert_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2895 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/hubert/convert_hubert_original_s3prl_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    60942 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/hubert/modeling_hubert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    63209 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/hubert/modeling_tf_hubert.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.389568 llm-toys-0.1.1/llm_toys/hf/transformers/models/ibert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2086 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/ibert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7462 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/ibert/configuration_ibert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    56703 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/ibert/modeling_ibert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    30072 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/ibert/quant_modules.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.389568 llm-toys-0.1.1/llm_toys/hf/transformers/models/imagegpt/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2658 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/imagegpt/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8866 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/imagegpt/configuration_imagegpt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2691 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/imagegpt/convert_imagegpt_original_tf2_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1200 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/imagegpt/feature_extraction_imagegpt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10808 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/imagegpt/image_processing_imagegpt.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    53849 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/imagegpt/modeling_imagegpt.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.389568 llm-toys-0.1.1/llm_toys/hf/transformers/models/informer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1857 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/informer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12684 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/informer/configuration_informer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   103554 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/informer/modeling_informer.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.393568 llm-toys-0.1.1/llm_toys/hf/transformers/models/instructblip/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2279 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/instructblip/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17867 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/instructblip/configuration_instructblip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13387 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/instructblip/convert_instructblip_original_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    70206 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/instructblip/modeling_instructblip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7855 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/instructblip/processing_instructblip.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.393568 llm-toys-0.1.1/llm_toys/hf/transformers/models/jukebox/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2084 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/jukebox/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    27873 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/jukebox/configuration_jukebox.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11789 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/jukebox/convert_jukebox.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   119653 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/jukebox/modeling_jukebox.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17740 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/jukebox/tokenization_jukebox.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.393568 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlm/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3787 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlm/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9513 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlm/configuration_layoutlm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    61080 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlm/modeling_layoutlm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    65594 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlm/modeling_tf_layoutlm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21698 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlm/tokenization_layoutlm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8967 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlm/tokenization_layoutlm_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.393568 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv2/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3439 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv2/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11247 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv2/configuration_layoutlmv2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1195 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv2/feature_extraction_layoutlmv2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11287 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv2/image_processing_layoutlmv2.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    61575 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv2/modeling_layoutlmv2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9267 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv2/processing_layoutlmv2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    72412 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv2/tokenization_layoutlmv2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    38073 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv2/tokenization_layoutlmv2_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.393568 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4512 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13363 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/configuration_layoutlmv3.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1195 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/feature_extraction_layoutlmv3.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16742 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/image_processing_layoutlmv3.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    60927 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/modeling_layoutlmv3.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    67864 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/modeling_tf_layoutlmv3.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9118 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/processing_layoutlmv3.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    72788 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/tokenization_layoutlmv3.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40311 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/tokenization_layoutlmv3_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.393568 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutxlm/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2037 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutxlm/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9218 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutxlm/processing_layoutxlm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57669 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutxlm/tokenization_layoutxlm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    39911 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutxlm/tokenization_layoutxlm_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.397568 llm-toys-0.1.1/llm_toys/hf/transformers/models/led/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3008 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/led/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7633 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/led/configuration_led.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   139950 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/led/modeling_led.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   116584 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/led/modeling_tf_led.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20406 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/led/tokenization_led.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14871 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/led/tokenization_led_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.397568 llm-toys-0.1.1/llm_toys/hf/transformers/models/levit/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2508 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/levit/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5930 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/levit/configuration_levit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6258 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/levit/convert_levit_timm_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1204 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/levit/feature_extraction_levit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17200 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/levit/image_processing_levit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    29663 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/levit/modeling_levit.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.397568 llm-toys-0.1.1/llm_toys/hf/transformers/models/lilt/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1909 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/lilt/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6878 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/lilt/configuration_lilt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    53140 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/lilt/modeling_lilt.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.397568 llm-toys-0.1.1/llm_toys/hf/transformers/models/llama/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2665 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/llama/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6998 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/llama/configuration_llama.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10917 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/llama/convert_llama_weights_to_hf.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    42064 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/llama/modeling_llama.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12954 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/llama/tokenization_llama.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6491 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/llama/tokenization_llama_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.397568 llm-toys-0.1.1/llm_toys/hf/transformers/models/longformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4196 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/longformer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9564 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/longformer/configuration_longformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3026 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/longformer/convert_longformer_original_pytorch_lightning_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   114361 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/longformer/modeling_longformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   121690 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/longformer/modeling_tf_longformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18736 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/longformer/tokenization_longformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14530 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/longformer/tokenization_longformer_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.397568 llm-toys-0.1.1/llm_toys/hf/transformers/models/longt5/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2546 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/longt5/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8481 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/longt5/configuration_longt5.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11089 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/longt5/convert_longt5x_checkpoint_to_flax.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   105640 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/longt5/modeling_flax_longt5.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   105418 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/longt5/modeling_longt5.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.401568 llm-toys-0.1.1/llm_toys/hf/transformers/models/luke/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2383 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/luke/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6554 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/luke/configuration_luke.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7467 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/luke/convert_luke_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   104043 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/luke/modeling_luke.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    85386 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/luke/tokenization_luke.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.401568 llm-toys-0.1.1/llm_toys/hf/transformers/models/lxmert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3396 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/lxmert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9510 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/lxmert/configuration_lxmert.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2109 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/lxmert/convert_lxmert_original_tf_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    64955 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/lxmert/modeling_lxmert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    61404 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/lxmert/modeling_tf_lxmert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21421 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/lxmert/tokenization_lxmert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8437 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/lxmert/tokenization_lxmert_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.401568 llm-toys-0.1.1/llm_toys/hf/transformers/models/m2m_100/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1992 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/m2m_100/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13582 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/m2m_100/configuration_m2m_100.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3159 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/m2m_100/convert_m2m100_original_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    65535 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/m2m_100/modeling_m2m_100.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17257 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/m2m_100/tokenization_m2m_100.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.401568 llm-toys-0.1.1/llm_toys/hf/transformers/models/marian/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3444 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/marian/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18558 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/marian/configuration_marian.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    36254 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/marian/convert_marian_tatoeba_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    26757 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/marian/convert_marian_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    64272 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/marian/modeling_flax_marian.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    83338 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/marian/modeling_marian.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    69040 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/marian/modeling_tf_marian.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17662 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/marian/tokenization_marian.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.405568 llm-toys-0.1.1/llm_toys/hf/transformers/models/markuplm/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2806 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/markuplm/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7571 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/markuplm/configuration_markuplm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6400 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/markuplm/feature_extraction_markuplm.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    57944 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/markuplm/modeling_markuplm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6347 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/markuplm/processing_markuplm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    69705 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/markuplm/tokenization_markuplm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    42808 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/markuplm/tokenization_markuplm_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.405568 llm-toys-0.1.1/llm_toys/hf/transformers/models/mask2former/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2357 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mask2former/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11404 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mask2former/configuration_mask2former.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    45688 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mask2former/convert_mask2former_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    50612 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mask2former/image_processing_mask2former.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   120588 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mask2former/modeling_mask2former.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.405568 llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2945 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9360 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/configuration_maskformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7054 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/configuration_maskformer_swin.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    32237 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/convert_maskformer_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20732 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/convert_maskformer_resnet_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20321 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/convert_maskformer_swin_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1214 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/feature_extraction_maskformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    53010 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/image_processing_maskformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    89023 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/modeling_maskformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    41045 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/modeling_maskformer_swin.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.405568 llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4403 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18387 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart/configuration_mbart.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3035 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart/convert_mbart_original_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    75102 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart/modeling_flax_mbart.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    89498 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart/modeling_mbart.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    68919 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart/modeling_tf_mbart.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14713 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart/tokenization_mbart.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11916 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart/tokenization_mbart_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.405568 llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart50/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1847 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart50/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16666 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart50/tokenization_mbart50.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12199 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart50/tokenization_mbart50_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.405568 llm-toys-0.1.1/llm_toys/hf/transformers/models/mega/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2140 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mega/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12738 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mega/configuration_mega.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13154 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mega/convert_mega_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   109288 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mega/modeling_mega.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.405568 llm-toys-0.1.1/llm_toys/hf/transformers/models/megatron_bert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2506 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/megatron_bert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6573 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/megatron_bert/configuration_megatron_bert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13686 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/megatron_bert/convert_megatron_bert_checkpoint.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    83194 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/megatron_bert/modeling_megatron_bert.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.409568 llm-toys-0.1.1/llm_toys/hf/transformers/models/megatron_gpt2/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      630 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/megatron_gpt2/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    36651 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/megatron_gpt2/checkpoint_reshaping_and_interoperability.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13627 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/megatron_gpt2/convert_megatron_gpt2_checkpoint.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.409568 llm-toys-0.1.1/llm_toys/hf/transformers/models/mgp_str/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2164 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mgp_str/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5935 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mgp_str/configuration_mgp_str.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21898 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mgp_str/modeling_mgp_str.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9244 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mgp_str/processing_mgp_str.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4068 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mgp_str/tokenization_mgp_str.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.409568 llm-toys-0.1.1/llm_toys/hf/transformers/models/mluke/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1356 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mluke/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10185 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mluke/convert_mluke_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    81133 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mluke/tokenization_mluke.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.409568 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilebert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4604 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilebert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8586 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilebert/configuration_mobilebert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2200 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilebert/convert_mobilebert_original_tf_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    70458 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilebert/modeling_mobilebert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    70944 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilebert/modeling_tf_mobilebert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21304 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilebert/tokenization_mobilebert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8377 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilebert/tokenization_mobilebert_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.409568 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v1/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2735 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v1/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5237 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v1/configuration_mobilenet_v1.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4932 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v1/convert_original_tf_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1222 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v1/feature_extraction_mobilenet_v1.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16159 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v1/image_processing_mobilenet_v1.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    18777 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v1/modeling_mobilenet_v1.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.409568 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v2/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2830 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v2/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7361 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v2/configuration_mobilenet_v2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6402 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v2/convert_original_tf_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1222 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v2/feature_extraction_mobilenet_v2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18576 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v2/image_processing_mobilenet_v2.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    34752 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v2/modeling_mobilenet_v2.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.413568 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevit/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3492 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevit/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8400 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevit/configuration_mobilevit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12402 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevit/convert_mlcvnets_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1207 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevit/feature_extraction_mobilevit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15713 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevit/image_processing_mobilevit.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    40528 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevit/modeling_mobilevit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    44632 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevit/modeling_tf_mobilevit.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.413568 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevitv2/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2111 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevitv2/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7237 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevitv2/configuration_mobilevitv2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12557 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevitv2/convert_mlcvnets_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    38738 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevitv2/modeling_mobilevitv2.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.413568 llm-toys-0.1.1/llm_toys/hf/transformers/models/mpnet/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3875 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mpnet/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5442 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mpnet/configuration_mpnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    42548 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mpnet/modeling_mpnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    48395 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mpnet/modeling_tf_mpnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    22583 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mpnet/tokenization_mpnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8930 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mpnet/tokenization_mpnet_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.413568 llm-toys-0.1.1/llm_toys/hf/transformers/models/mra/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2254 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mra/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6662 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mra/configuration_mra.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4247 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mra/convert_mra_pytorch_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    62339 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mra/modeling_mra.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.413568 llm-toys-0.1.1/llm_toys/hf/transformers/models/mt5/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3439 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mt5/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7588 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mt5/configuration_mt5.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4239 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mt5/modeling_flax_mt5.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   102044 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mt5/modeling_mt5.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3325 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mt5/modeling_tf_mt5.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.413568 llm-toys-0.1.1/llm_toys/hf/transformers/models/musicgen/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2099 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/musicgen/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10772 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/musicgen/configuration_musicgen.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8128 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/musicgen/convert_musicgen_transformers.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   123160 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/musicgen/modeling_musicgen.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5665 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/musicgen/processing_musicgen.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.413568 llm-toys-0.1.1/llm_toys/hf/transformers/models/mvp/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2536 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mvp/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8533 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mvp/configuration_mvp.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    95123 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mvp/modeling_mvp.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16823 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mvp/tokenization_mvp.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12088 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/mvp/tokenization_mvp_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.417569 llm-toys-0.1.1/llm_toys/hf/transformers/models/nat/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1776 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/nat/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7033 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/nat/configuration_nat.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40045 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/nat/modeling_nat.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.417569 llm-toys-0.1.1/llm_toys/hf/transformers/models/nezha/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2233 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/nezha/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5033 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/nezha/configuration_nezha.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    75081 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/nezha/modeling_nezha.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.417569 llm-toys-0.1.1/llm_toys/hf/transformers/models/nllb/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1868 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/nllb/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19976 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/nllb/tokenization_nllb.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16966 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/nllb/tokenization_nllb_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.417569 llm-toys-0.1.1/llm_toys/hf/transformers/models/nllb_moe/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1978 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/nllb_moe/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11315 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/nllb_moe/configuration_nllb_moe.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6477 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/nllb_moe/convert_nllb_moe_sharded_original_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    86841 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/nllb_moe/modeling_nllb_moe.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.417569 llm-toys-0.1.1/llm_toys/hf/transformers/models/nystromformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2337 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/nystromformer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6623 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/nystromformer/configuration_nystromformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4197 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/nystromformer/convert_nystromformer_original_pytorch_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    49086 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/nystromformer/modeling_nystromformer.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.417569 llm-toys-0.1.1/llm_toys/hf/transformers/models/oneformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2402 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/oneformer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12423 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/oneformer/configuration_oneformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    50690 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/oneformer/convert_to_hf_oneformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    55915 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/oneformer/image_processing_oneformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   143392 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/oneformer/modeling_oneformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9482 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/oneformer/processing_oneformer.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.417569 llm-toys-0.1.1/llm_toys/hf/transformers/models/open_llama/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2787 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/open_llama/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7858 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/open_llama/configuration_open_llama.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    44924 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/open_llama/modeling_open_llama.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.417569 llm-toys-0.1.1/llm_toys/hf/transformers/models/openai/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3658 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/openai/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7332 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/openai/configuration_openai.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2666 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/openai/convert_openai_original_tf_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    38004 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/openai/modeling_openai.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    37783 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/openai/modeling_tf_openai.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15582 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/openai/tokenization_openai.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3046 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/openai/tokenization_openai_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.421568 llm-toys-0.1.1/llm_toys/hf/transformers/models/opt/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2977 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/opt/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7244 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/opt/configuration_opt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3858 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/opt/convert_opt_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    31547 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/opt/modeling_flax_opt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57855 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/opt/modeling_opt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    45560 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/opt/modeling_tf_opt.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.421568 llm-toys-0.1.1/llm_toys/hf/transformers/models/owlvit/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2915 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/owlvit/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17054 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/owlvit/configuration_owlvit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13988 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/owlvit/convert_owlvit_original_flax_to_hf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1186 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/owlvit/feature_extraction_owlvit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23870 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/owlvit/image_processing_owlvit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    77705 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/owlvit/modeling_owlvit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11123 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/owlvit/processing_owlvit.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.421568 llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4111 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7693 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus/configuration_pegasus.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5359 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus/convert_pegasus_tf_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    66067 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus/modeling_flax_pegasus.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    82118 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus/modeling_pegasus.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    69379 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus/modeling_tf_pegasus.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13709 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus/tokenization_pegasus.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9937 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus/tokenization_pegasus_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.421568 llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus_x/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1828 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus_x/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8419 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus_x/configuration_pegasus_x.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    79396 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus_x/modeling_pegasus_x.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.421568 llm-toys-0.1.1/llm_toys/hf/transformers/models/perceiver/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3293 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/perceiver/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12055 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/perceiver/configuration_perceiver.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21286 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/perceiver/convert_perceiver_haiku_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1207 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/perceiver/feature_extraction_perceiver.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15537 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/perceiver/image_processing_perceiver.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   146469 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/perceiver/modeling_perceiver.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8945 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/perceiver/tokenization_perceiver.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.421568 llm-toys-0.1.1/llm_toys/hf/transformers/models/phobert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      955 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/phobert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13551 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/phobert/tokenization_phobert.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.425568 llm-toys-0.1.1/llm_toys/hf/transformers/models/pix2struct/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2701 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/pix2struct/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18040 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/pix2struct/configuration_pix2struct.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5886 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/pix2struct/convert_pix2struct_original_pytorch_to_hf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17854 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/pix2struct/image_processing_pix2struct.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    83362 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/pix2struct/modeling_pix2struct.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6959 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/pix2struct/processing_pix2struct.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.425568 llm-toys-0.1.1/llm_toys/hf/transformers/models/plbart/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2429 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/plbart/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8719 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/plbart/configuration_plbart.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3553 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/plbart/convert_plbart_original_checkpoint_to_torch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    82983 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/plbart/modeling_plbart.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21656 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/plbart/tokenization_plbart.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.425568 llm-toys-0.1.1/llm_toys/hf/transformers/models/poolformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2586 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/poolformer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5802 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/poolformer/configuration_poolformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7947 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/poolformer/convert_poolformer_original_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1214 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/poolformer/feature_extraction_poolformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18310 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/poolformer/image_processing_poolformer.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    18074 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/poolformer/modeling_poolformer.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.425568 llm-toys-0.1.1/llm_toys/hf/transformers/models/prophetnet/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2157 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/prophetnet/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9062 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/prophetnet/configuration_prophetnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7055 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/prophetnet/convert_prophetnet_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   114949 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/prophetnet/modeling_prophetnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21847 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/prophetnet/tokenization_prophetnet.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.425568 llm-toys-0.1.1/llm_toys/hf/transformers/models/qdqbert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2402 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/qdqbert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5895 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/qdqbert/configuration_qdqbert.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    77045 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/qdqbert/modeling_qdqbert.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.425568 llm-toys-0.1.1/llm_toys/hf/transformers/models/rag/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2426 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/rag/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8800 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/rag/configuration_rag.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    86080 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/rag/modeling_rag.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    87921 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/rag/modeling_tf_rag.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28510 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/rag/retrieval_rag.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4576 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/rag/tokenization_rag.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.425568 llm-toys-0.1.1/llm_toys/hf/transformers/models/realm/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2675 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/realm/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8743 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/realm/configuration_realm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    84492 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/realm/modeling_realm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6370 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/realm/retrieval_realm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    25477 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/realm/tokenization_realm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14575 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/realm/tokenization_realm_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.425568 llm-toys-0.1.1/llm_toys/hf/transformers/models/reformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3139 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/reformer/__init__.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    13463 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/reformer/configuration_reformer.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     7818 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/reformer/convert_reformer_trax_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   115179 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/reformer/modeling_reformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7315 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/reformer/tokenization_reformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4825 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/reformer/tokenization_reformer_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.429569 llm-toys-0.1.1/llm_toys/hf/transformers/models/regnet/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3168 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/regnet/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4088 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/regnet/configuration_regnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11770 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/regnet/convert_regnet_seer_10b_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18715 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/regnet/convert_regnet_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28403 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/regnet/modeling_flax_regnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17533 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/regnet/modeling_regnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19479 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/regnet/modeling_tf_regnet.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.429569 llm-toys-0.1.1/llm_toys/hf/transformers/models/rembert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4514 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/rembert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7450 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/rembert/configuration_rembert.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2208 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/rembert/convert_rembert_tf_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    68091 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/rembert/modeling_rembert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    69600 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/rembert/modeling_tf_rembert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10481 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/rembert/tokenization_rembert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10422 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/rembert/tokenization_rembert_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.429569 llm-toys-0.1.1/llm_toys/hf/transformers/models/resnet/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3216 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/resnet/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5697 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/resnet/configuration_resnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7287 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/resnet/convert_resnet_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24640 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/resnet/modeling_flax_resnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19025 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/resnet/modeling_resnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19121 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/resnet/modeling_tf_resnet.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.429569 llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5091 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7878 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta/configuration_roberta.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8002 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta/convert_roberta_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    56957 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta/modeling_flax_roberta.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    71162 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta/modeling_roberta.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    71893 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta/modeling_tf_roberta.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17960 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta/tokenization_roberta.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13678 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta/tokenization_roberta_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.429569 llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta_prelayernorm/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5391 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta_prelayernorm/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8024 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta_prelayernorm/configuration_roberta_prelayernorm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2975 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta_prelayernorm/convert_roberta_prelayernorm_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    60529 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta_prelayernorm/modeling_flax_roberta_prelayernorm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    73898 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta_prelayernorm/modeling_roberta_prelayernorm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    74866 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta_prelayernorm/modeling_tf_roberta_prelayernorm.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.429569 llm-toys-0.1.1/llm_toys/hf/transformers/models/roc_bert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2875 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roc_bert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8657 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roc_bert/configuration_roc_bert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    92854 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roc_bert/modeling_roc_bert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    50992 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roc_bert/tokenization_roc_bert.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.433569 llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5333 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7711 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/configuration_roformer.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2240 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/convert_roformer_original_tf_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    39460 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/modeling_flax_roformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    69287 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/modeling_roformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57616 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/modeling_tf_roformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23835 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/tokenization_roformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8276 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/tokenization_roformer_fast.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2652 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/tokenization_utils.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.433569 llm-toys-0.1.1/llm_toys/hf/transformers/models/rwkv/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1780 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/rwkv/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6204 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/rwkv/configuration_rwkv.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6994 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/rwkv/convert_rwkv_checkpoint_to_hf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    35605 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/rwkv/modeling_rwkv.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.433569 llm-toys-0.1.1/llm_toys/hf/transformers/models/sam/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2980 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/sam/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14784 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/sam/configuration_sam.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6958 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/sam/convert_sam_original_to_hf_format.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57242 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/sam/image_processing_sam.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    65035 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/sam/modeling_sam.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    66857 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/sam/modeling_tf_sam.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10848 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/sam/processing_sam.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.433569 llm-toys-0.1.1/llm_toys/hf/transformers/models/segformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3676 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/segformer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7636 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/segformer/configuration_segformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17092 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/segformer/convert_segformer_original_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1207 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/segformer/feature_extraction_segformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21100 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/segformer/image_processing_segformer.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    35488 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/segformer/modeling_segformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    36138 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/segformer/modeling_tf_segformer.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.433569 llm-toys-0.1.1/llm_toys/hf/transformers/models/sew/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1778 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/sew/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14239 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/sew/configuration_sew.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12745 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/sew/convert_sew_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    53927 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/sew/modeling_sew.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.433569 llm-toys-0.1.1/llm_toys/hf/transformers/models/sew_d/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1804 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/sew_d/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15981 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/sew_d/configuration_sew_d.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13575 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/sew_d/convert_sew_d_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    74626 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/sew_d/modeling_sew_d.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.433569 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_encoder_decoder/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2037 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_encoder_decoder/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5087 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_encoder_decoder/configuration_speech_encoder_decoder.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14760 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_encoder_decoder/convert_mbart_wav2vec2_seq2seq_original_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11971 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_encoder_decoder/convert_speech_to_text_wav2vec2_seq2seq_original_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    45067 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_encoder_decoder/modeling_flax_speech_encoder_decoder.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    32945 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_encoder_decoder/modeling_speech_encoder_decoder.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.437569 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3845 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9312 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text/configuration_speech_to_text.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4478 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text/convert_s2t_fairseq_to_tfms.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11798 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text/feature_extraction_speech_to_text.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    66955 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text/modeling_speech_to_text.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    68086 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text/modeling_tf_speech_to_text.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4817 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text/processing_speech_to_text.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11653 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text/tokenization_speech_to_text.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.437569 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text_2/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2166 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text_2/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6281 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text_2/configuration_speech_to_text_2.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    46328 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text_2/modeling_speech_to_text_2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4789 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text_2/processing_speech_to_text_2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9211 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text_2/tokenization_speech_to_text_2.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.437569 llm-toys-0.1.1/llm_toys/hf/transformers/models/speecht5/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2971 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speecht5/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23899 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speecht5/configuration_speecht5.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4241 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speecht5/convert_hifigan.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17194 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speecht5/convert_speecht5_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17809 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speecht5/feature_extraction_speecht5.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   144023 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speecht5/modeling_speecht5.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7561 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speecht5/processing_speecht5.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8390 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/speecht5/tokenization_speecht5.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.437569 llm-toys-0.1.1/llm_toys/hf/transformers/models/splinter/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2532 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/splinter/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6120 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/splinter/configuration_splinter.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    53633 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/splinter/modeling_splinter.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    22013 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/splinter/tokenization_splinter.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9657 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/splinter/tokenization_splinter_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.437569 llm-toys-0.1.1/llm_toys/hf/transformers/models/squeezebert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2996 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/squeezebert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7910 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/squeezebert/configuration_squeezebert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    45011 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/squeezebert/modeling_squeezebert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21889 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/squeezebert/tokenization_squeezebert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9397 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/squeezebert/tokenization_squeezebert_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.437569 llm-toys-0.1.1/llm_toys/hf/transformers/models/swiftformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1990 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swiftformer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5346 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swiftformer/configuration_swiftformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6239 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swiftformer/convert_swiftformer_original_to_hf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23318 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swiftformer/modeling_swiftformer.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.437569 llm-toys-0.1.1/llm_toys/hf/transformers/models/swin/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2703 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swin/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7999 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swin/configuration_swin.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6627 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swin/convert_swin_simmim_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5805 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swin/convert_swin_timm_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    60019 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swin/modeling_swin.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    63770 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swin/modeling_tf_swin.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.441568 llm-toys-0.1.1/llm_toys/hf/transformers/models/swin2sr/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2277 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swin2sr/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6706 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swin2sr/configuration_swin2sr.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11355 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swin2sr/convert_swin2sr_original_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7713 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swin2sr/image_processing_swin2sr.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    51704 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swin2sr/modeling_swin2sr.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.441568 llm-toys-0.1.1/llm_toys/hf/transformers/models/swinv2/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1867 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swinv2/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6323 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swinv2/configuration_swinv2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7687 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swinv2/convert_swinv2_timm_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    61510 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/swinv2/modeling_swinv2.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.441568 llm-toys-0.1.1/llm_toys/hf/transformers/models/switch_transformers/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2484 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/switch_transformers/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10011 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/switch_transformers/configuration_switch_transformers.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7649 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/switch_transformers/convert_big_switch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7593 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/switch_transformers/convert_switch_transformers_original_flax_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    89411 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/switch_transformers/modeling_switch_transformers.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.441568 llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4338 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7460 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/configuration_t5.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2120 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/convert_t5_original_tf_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10538 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/convert_t5x_checkpoint_to_flax.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    10365 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/convert_t5x_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    74074 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/modeling_flax_t5.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    97295 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/modeling_t5.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    71842 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/modeling_tf_t5.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17968 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/tokenization_t5.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10587 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/tokenization_t5_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.441568 llm-toys-0.1.1/llm_toys/hf/transformers/models/table_transformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2065 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/table_transformer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12520 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/table_transformer/configuration_table_transformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15076 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/table_transformer/convert_table_transformer_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    92597 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/table_transformer/modeling_table_transformer.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.441568 llm-toys-0.1.1/llm_toys/hf/transformers/models/tapas/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2952 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/tapas/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12900 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/tapas/configuration_tapas.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5049 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/tapas/convert_tapas_original_tf_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   111736 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/tapas/modeling_tapas.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   105769 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/tapas/modeling_tf_tapas.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   121112 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/tapas/tokenization_tapas.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.441568 llm-toys-0.1.1/llm_toys/hf/transformers/models/time_series_transformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2069 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/time_series_transformer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12003 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/time_series_transformer/configuration_time_series_transformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    90470 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/time_series_transformer/modeling_time_series_transformer.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.445569 llm-toys-0.1.1/llm_toys/hf/transformers/models/timesformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1862 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/timesformer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5683 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/timesformer/configuration_timesformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10176 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/timesformer/convert_timesformer_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    34650 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/timesformer/modeling_timesformer.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.445569 llm-toys-0.1.1/llm_toys/hf/transformers/models/timm_backbone/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1624 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/timm_backbone/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2876 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/timm_backbone/configuration_timm_backbone.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5991 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/timm_backbone/modeling_timm_backbone.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.445569 llm-toys-0.1.1/llm_toys/hf/transformers/models/transfo_xl/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3182 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/transfo_xl/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7895 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/transfo_xl/configuration_transfo_xl.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     4916 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/transfo_xl/convert_transfo_xl_original_tf_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    45094 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/transfo_xl/modeling_tf_transfo_xl.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7597 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/transfo_xl/modeling_tf_transfo_xl_utilities.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    55720 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/transfo_xl/modeling_transfo_xl.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10861 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/transfo_xl/modeling_transfo_xl_utilities.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    30487 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/transfo_xl/tokenization_transfo_xl.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.445569 llm-toys-0.1.1/llm_toys/hf/transformers/models/trocr/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1818 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/trocr/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6778 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/trocr/configuration_trocr.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10155 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/trocr/convert_trocr_unilm_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    47542 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/trocr/modeling_trocr.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5720 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/trocr/processing_trocr.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.445569 llm-toys-0.1.1/llm_toys/hf/transformers/models/tvlt/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2687 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/tvlt/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8760 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/tvlt/configuration_tvlt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10507 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/tvlt/feature_extraction_tvlt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20730 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/tvlt/image_processing_tvlt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57262 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/tvlt/modeling_tvlt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3505 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/tvlt/processing_tvlt.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.445569 llm-toys-0.1.1/llm_toys/hf/transformers/models/umt5/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1746 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/umt5/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7753 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/umt5/configuration_umt5.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12070 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/umt5/convert_umt5_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    73907 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/umt5/modeling_umt5.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.445569 llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2018 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17161 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech/configuration_unispeech.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11340 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech/convert_unispeech_original_pytorch_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    73175 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech/modeling_unispeech.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.445569 llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech_sat/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2267 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech_sat/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18584 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech_sat/configuration_unispeech_sat.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4870 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech_sat/convert_unispeech_original_s3prl_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9289 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech_sat/convert_unispeech_sat_original_pytorch_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    86770 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech_sat/modeling_unispeech_sat.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.449569 llm-toys-0.1.1/llm_toys/hf/transformers/models/upernet/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1535 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/upernet/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5439 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/upernet/configuration_upernet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10271 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/upernet/convert_convnext_upernet_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14026 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/upernet/convert_swin_upernet_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17414 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/upernet/modeling_upernet.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.449569 llm-toys-0.1.1/llm_toys/hf/transformers/models/videomae/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2519 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/videomae/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6718 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/videomae/configuration_videomae.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13989 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/videomae/convert_videomae_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1200 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/videomae/feature_extraction_videomae.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17262 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/videomae/image_processing_videomae.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    46972 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/videomae/modeling_videomae.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.449569 llm-toys-0.1.1/llm_toys/hf/transformers/models/vilt/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2788 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vilt/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6929 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vilt/configuration_vilt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12870 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vilt/convert_vilt_original_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1172 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vilt/feature_extraction_vilt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21090 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vilt/image_processing_vilt.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    65187 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vilt/modeling_vilt.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6054 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vilt/processing_vilt.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.449569 llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_encoder_decoder/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2627 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_encoder_decoder/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8785 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_encoder_decoder/configuration_vision_encoder_decoder.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    41661 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_encoder_decoder/modeling_flax_vision_encoder_decoder.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    36960 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_encoder_decoder/modeling_tf_vision_encoder_decoder.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    35040 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_encoder_decoder/modeling_vision_encoder_decoder.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.449569 llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_text_dual_encoder/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2730 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_text_dual_encoder/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5289 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_text_dual_encoder/configuration_vision_text_dual_encoder.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    26682 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_text_dual_encoder/modeling_flax_vision_text_dual_encoder.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28773 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_text_dual_encoder/modeling_tf_vision_text_dual_encoder.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    25315 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_text_dual_encoder/modeling_vision_text_dual_encoder.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7010 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_text_dual_encoder/processing_vision_text_dual_encoder.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.449569 llm-toys-0.1.1/llm_toys/hf/transformers/models/visual_bert/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2235 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/visual_bert/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7942 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/visual_bert/configuration_visual_bert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5158 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/visual_bert/convert_visual_bert_original_pytorch_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    69820 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/visual_bert/modeling_visual_bert.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.449569 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3598 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5835 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/configuration_vit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8854 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/convert_dino_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10184 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/convert_vit_timm_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1165 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/feature_extraction_vit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13287 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/image_processing_vit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    25333 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/modeling_flax_vit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    31869 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/modeling_tf_vit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    35989 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/modeling_vit.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.453569 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_hybrid/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2316 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_hybrid/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7223 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_hybrid/configuration_vit_hybrid.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13413 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_hybrid/convert_vit_hybrid_timm_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16128 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_hybrid/image_processing_vit_hybrid.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    32287 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_hybrid/modeling_vit_hybrid.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.453569 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_mae/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2428 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_mae/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6568 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_mae/configuration_vit_mae.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7516 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_mae/convert_vit_mae_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    47226 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_mae/modeling_tf_vit_mae.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    43355 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_mae/modeling_vit_mae.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.453569 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_msn/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1783 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_msn/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5062 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_msn/configuration_vit_msn.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9841 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_msn/convert_msn_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    30091 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_msn/modeling_vit_msn.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.453569 llm-toys-0.1.1/llm_toys/hf/transformers/models/vivit/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2441 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vivit/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5368 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vivit/configuration_vivit.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9145 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vivit/convert_vivit_flax_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18469 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vivit/image_processing_vivit.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    28976 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/vivit/modeling_vivit.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.453569 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4139 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20142 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/configuration_wav2vec2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14293 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/convert_wav2vec2_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4838 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/convert_wav2vec2_original_s3prl_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11511 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/feature_extraction_wav2vec2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    57331 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/modeling_flax_wav2vec2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    70405 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/modeling_tf_wav2vec2.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   106131 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/modeling_wav2vec2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7136 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/processing_wav2vec2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    41063 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/tokenization_wav2vec2.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.453569 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_conformer/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2375 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_conformer/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    20919 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_conformer/configuration_wav2vec2_conformer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13382 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_conformer/convert_wav2vec2_conformer_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    95737 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_conformer/modeling_wav2vec2_conformer.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.453569 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_phoneme/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      993 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_phoneme/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    26089 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_phoneme/tokenization_wav2vec2_phoneme.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.453569 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_with_lm/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      981 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_with_lm/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    29648 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_with_lm/processing_wav2vec2_with_lm.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.457569 llm-toys-0.1.1/llm_toys/hf/transformers/models/wavlm/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1959 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wavlm/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18605 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wavlm/configuration_wavlm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8580 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wavlm/convert_wavlm_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4814 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wavlm/convert_wavlm_original_s3prl_checkpoint_to_pytorch.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    78999 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/wavlm/modeling_wavlm.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.457569 llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4284 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    17052 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/configuration_whisper.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7602 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/convert_openai_to_hf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    22822 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/english_normalizer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12240 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/feature_extraction_whisper.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    72572 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/modeling_flax_whisper.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    77654 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/modeling_tf_whisper.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    93218 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/modeling_whisper.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3890 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/processing_whisper.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    49340 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/tokenization_whisper.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    26137 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/tokenization_whisper_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.457569 llm-toys-0.1.1/llm_toys/hf/transformers/models/x_clip/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2053 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/x_clip/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21041 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/x_clip/configuration_x_clip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18066 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/x_clip/convert_x_clip_original_pytorch_to_hf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    70568 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/x_clip/modeling_x_clip.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6872 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/x_clip/processing_x_clip.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.457569 llm-toys-0.1.1/llm_toys/hf/transformers/models/xglm/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3871 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xglm/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6055 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xglm/configuration_xglm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2325 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xglm/convert_xglm_original_ckpt_to_trfms.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    33123 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xglm/modeling_flax_xglm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    41806 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xglm/modeling_tf_xglm.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    40819 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xglm/modeling_xglm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13277 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xglm/tokenization_xglm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8033 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xglm/tokenization_xglm_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.461569 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3292 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11975 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm/configuration_xlm.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     2934 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm/convert_xlm_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    51632 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm/modeling_tf_xlm.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    54911 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm/modeling_xlm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    34960 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm/tokenization_xlm.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.461569 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_prophetnet/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2615 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_prophetnet/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9125 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_prophetnet/configuration_xlm_prophetnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   118980 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_prophetnet/modeling_xlm_prophetnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13908 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_prophetnet/tokenization_xlm_prophetnet.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.461569 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5825 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8346 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta/configuration_xlm_roberta.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    58614 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta/modeling_flax_xlm_roberta.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    73898 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta/modeling_tf_xlm_roberta.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    72944 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta/modeling_xlm_roberta.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14285 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta/tokenization_xlm_roberta.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10264 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta/tokenization_xlm_roberta_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.461569 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta_xl/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2405 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta_xl/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7595 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta_xl/configuration_xlm_roberta_xl.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8228 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta_xl/convert_xlm_roberta_xl_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    68793 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta_xl/modeling_xlm_roberta_xl.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.461569 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlnet/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4288 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlnet/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11143 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlnet/configuration_xlnet.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)     3688 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlnet/convert_xlnet_original_tf_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    73071 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlnet/modeling_tf_xlnet.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    92846 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlnet/modeling_xlnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16191 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlnet/tokenization_xlnet.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10026 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xlnet/tokenization_xlnet_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.461569 llm-toys-0.1.1/llm_toys/hf/transformers/models/xmod/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2325 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xmod/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10145 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xmod/configuration_xmod.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9859 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xmod/convert_xmod_original_pytorch_checkpoint_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    76513 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/xmod/modeling_xmod.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.465569 llm-toys-0.1.1/llm_toys/hf/transformers/models/yolos/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2400 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/yolos/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7790 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/yolos/configuration_yolos.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11259 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/yolos/convert_yolos_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1179 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/yolos/feature_extraction_yolos.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    52795 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/yolos/image_processing_yolos.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    58800 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/yolos/modeling_yolos.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.465569 llm-toys-0.1.1/llm_toys/hf/transformers/models/yoso/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2074 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/yoso/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6902 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/yoso/configuration_yoso.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4115 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/yoso/convert_yoso_pytorch_to_pytorch.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    55064 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/models/yoso/modeling_yoso.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.465569 llm-toys-0.1.1/llm_toys/hf/transformers/onnx/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1548 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/onnx/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9519 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/onnx/__main__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    32490 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/onnx/config.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    21182 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/onnx/convert.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    28264 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/onnx/features.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3625 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/onnx/utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    31638 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/optimization.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16583 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/optimization_tf.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.469569 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    46315 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8769 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/audio_classification.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8094 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/audio_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    35232 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/automatic_speech_recognition.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    51408 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/base.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13594 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/conversational.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4258 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/depth_estimation.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    23079 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/document_question_answering.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4822 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/feature_extraction.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10691 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/fill_mask.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4940 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/image_classification.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8731 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/image_segmentation.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7138 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/image_to_text.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13291 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/mask_generation.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7441 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/object_detection.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12613 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/pt_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    29474 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/question_answering.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    19892 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/table_question_answering.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    16875 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/text2text_generation.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10043 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/text_classification.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15183 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/text_generation.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    26627 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/token_classification.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5008 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/video_classification.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5968 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/visual_question_answering.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6501 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/zero_shot_audio_classification.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11983 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/zero_shot_classification.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6075 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/zero_shot_image_classification.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9029 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/zero_shot_object_detection.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11968 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/processing_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    11445 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/pytorch_utils.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.469569 llm-toys-0.1.1/llm_toys/hf/transformers/sagemaker/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      730 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/sagemaker/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1044 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/sagemaker/trainer_sm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5389 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/sagemaker/training_args_sm.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    68116 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/testing_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9571 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tf_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     7520 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/time_series_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40143 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tokenization_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   182321 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tokenization_utils_base.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    33446 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tokenization_utils_fast.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.469569 llm-toys-0.1.1/llm_toys/hf/transformers/tools/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2955 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tools/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9093 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tools/agent_types.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    30304 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tools/agents.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    29957 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tools/base.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3337 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tools/document_question_answering.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24739 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tools/evaluate_agent.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1745 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tools/image_captioning.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1969 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tools/image_question_answering.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2102 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tools/image_segmentation.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1558 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tools/prompts.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     9959 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tools/python_interpreter.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1482 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tools/speech_to_text.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2475 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tools/text_classification.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1967 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tools/text_question_answering.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1691 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tools/text_summarization.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2424 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tools/text_to_speech.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8493 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/tools/translation.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)   185736 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/trainer.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24051 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/trainer_callback.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    47809 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/trainer_pt_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    15722 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/trainer_seq2seq.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    34629 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/trainer_tf.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    24147 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/trainer_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   126983 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/training_args.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4484 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/training_args_seq2seq.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14388 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/training_args_tf.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.473569 llm-toys-0.1.1/llm_toys/hf/transformers/utils/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6572 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12027 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/backbone_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    13391 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/bitsandbytes.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      282 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/constants.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    40011 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/doc.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      391 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/dummy_detectron2_objects.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    30740 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/dummy_flax_objects.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      294 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/dummy_keras_nlp_objects.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)   193887 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/dummy_pt_objects.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      286 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/dummy_sentencepiece_and_tokenizers_objects.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5575 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/dummy_sentencepiece_objects.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      465 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/dummy_speech_objects.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      306 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/dummy_tensorflow_text_objects.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    67038 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/dummy_tf_objects.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10241 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/dummy_tokenizers_objects.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12566 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/dummy_vision_objects.py
+-rwxrwxr-x   0 tarnished  (1000) tarnished  (1000)    47792 2023-07-16 03:26:07.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/fx.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    18320 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/generic.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4979 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/hp_naming.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    49100 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/hub.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    39906 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/import_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    10168 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/logging.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     2272 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/model_parallel_utils.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    14831 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/notebook.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    12238 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/quantization_config.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    50671 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/sentencepiece_model_pb2.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6621 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/sentencepiece_model_pb2_new.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4333 2023-07-15 14:04:29.000000 llm-toys-0.1.1/llm_toys/hf/transformers/utils/versions.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      935 2023-07-16 13:26:36.000000 llm-toys-0.1.1/llm_toys/prompts.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.473569 llm-toys-0.1.1/llm_toys/tasks/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)      210 2023-07-17 10:11:26.000000 llm-toys-0.1.1/llm_toys/tasks/__init__.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     5749 2023-07-17 10:44:34.000000 llm-toys-0.1.1/llm_toys/tasks/all_tasks.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3281 2023-07-17 10:45:38.000000 llm-toys-0.1.1/llm_toys/tasks/paraphrase.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3893 2023-07-16 13:17:26.000000 llm-toys-0.1.1/llm_toys/tasks/predict.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     4416 2023-07-17 10:47:13.000000 llm-toys-0.1.1/llm_toys/tasks/summary_topic.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     8968 2023-07-17 09:26:46.000000 llm-toys-0.1.1/llm_toys/train.py
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     3126 2023-07-17 04:11:06.000000 llm-toys-0.1.1/llm_toys/utils.py
+drwxrwxr-x   0 tarnished  (1000) tarnished  (1000)        0 2023-07-17 11:27:36.325568 llm-toys-0.1.1/llm_toys.egg-info/
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     6908 2023-07-17 11:27:36.000000 llm-toys-0.1.1/llm_toys.egg-info/PKG-INFO
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)    87698 2023-07-17 11:27:36.000000 llm-toys-0.1.1/llm_toys.egg-info/SOURCES.txt
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        1 2023-07-17 11:27:36.000000 llm-toys-0.1.1/llm_toys.egg-info/dependency_links.txt
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1498 2023-07-17 11:27:36.000000 llm-toys-0.1.1/llm_toys.egg-info/requires.txt
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)        9 2023-07-17 11:27:36.000000 llm-toys-0.1.1/llm_toys.egg-info/top_level.txt
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)       89 2023-07-15 06:02:36.000000 llm-toys-0.1.1/pyproject.toml
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)       38 2023-07-17 11:27:36.473569 llm-toys-0.1.1/setup.cfg
+-rw-rw-r--   0 tarnished  (1000) tarnished  (1000)     1431 2023-07-17 11:08:43.000000 llm-toys-0.1.1/setup.py
```

### Comparing `llm-toys-0.1.0/PKG-INFO` & `llm-toys-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-toys
-Version: 0.1.0
+Version: 0.1.1
 Summary: Small(7B and below), production-ready finetuned LLMs for a diverse set of useful tasks.
 Home-page: https://github.com/kuutsav/llm-toys
 Author: Kumar Utsav
 Author-email: krum.utsav@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
```

### Comparing `llm-toys-0.1.0/README.md` & `llm-toys-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/__init__.py` & `llm-toys-0.1.1/llm_toys/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 
 from pathlib import Path
 import sys
 
 from llm_toys.utils import print_warning
```

### Comparing `llm-toys-0.1.0/llm_toys/config.py` & `llm-toys-0.1.1/llm_toys/config.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/eval.py` & `llm-toys-0.1.1/llm_toys/eval.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/peft/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/auto.py` & `llm-toys-0.1.1/llm_toys/hf/peft/auto.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/import_utils.py` & `llm-toys-0.1.1/llm_toys/hf/peft/import_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/mapping.py` & `llm-toys-0.1.1/llm_toys/hf/peft/mapping.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/peft_model.py` & `llm-toys-0.1.1/llm_toys/hf/peft/peft_model.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/tuners/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/peft/tuners/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/tuners/adalora.py` & `llm-toys-0.1.1/llm_toys/hf/peft/tuners/adalora.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/tuners/adaption_prompt.py` & `llm-toys-0.1.1/llm_toys/hf/peft/tuners/adaption_prompt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/tuners/ia3.py` & `llm-toys-0.1.1/llm_toys/hf/peft/tuners/ia3.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/tuners/lora.py` & `llm-toys-0.1.1/llm_toys/hf/peft/tuners/lora.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/tuners/p_tuning.py` & `llm-toys-0.1.1/llm_toys/hf/peft/tuners/p_tuning.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/tuners/prefix_tuning.py` & `llm-toys-0.1.1/llm_toys/hf/peft/tuners/prefix_tuning.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/tuners/prompt_tuning.py` & `llm-toys-0.1.1/llm_toys/hf/peft/tuners/prompt_tuning.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/utils/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/peft/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/utils/config.py` & `llm-toys-0.1.1/llm_toys/hf/peft/utils/config.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/utils/hub_utils.py` & `llm-toys-0.1.1/llm_toys/hf/peft/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/utils/other.py` & `llm-toys-0.1.1/llm_toys/hf/peft/utils/other.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/peft/utils/save_and_load.py` & `llm-toys-0.1.1/llm_toys/hf/peft/utils/save_and_load.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/activations.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/activations.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/activations_tf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/activations_tf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/audio_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/audio_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/benchmark/benchmark.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/benchmark/benchmark_args.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/benchmark/benchmark_args.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/benchmark/benchmark_args_tf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/benchmark/benchmark_args_tf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/benchmark/benchmark_args_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/benchmark/benchmark_args_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/benchmark/benchmark_tf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/benchmark/benchmark_tf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/benchmark/benchmark_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/commands/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/commands/add_new_model.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/commands/add_new_model.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/commands/add_new_model_like.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/commands/add_new_model_like.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/commands/convert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/commands/convert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/commands/download.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/commands/download.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/commands/env.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/commands/env.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/commands/lfs.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/commands/lfs.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/commands/pt_to_tf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/commands/pt_to_tf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/commands/run.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/commands/run.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/commands/serving.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/commands/serving.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/commands/train.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/commands/train.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/commands/transformers_cli.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/commands/transformers_cli.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/commands/user.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/commands/user.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/configuration_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/convert_graph_to_onnx.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/convert_graph_to_onnx.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/convert_pytorch_checkpoint_to_tf2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/convert_pytorch_checkpoint_to_tf2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/convert_slow_tokenizer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/convert_slow_tokenizer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/convert_slow_tokenizers_checkpoints_to_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/convert_slow_tokenizers_checkpoints_to_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/convert_tf_hub_seq_to_seq_bert_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/convert_tf_hub_seq_to_seq_bert_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/data/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/data/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/data/data_collator.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/data/data_collator.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/data/datasets/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/data/datasets/glue.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/data/datasets/glue.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/data/datasets/language_modeling.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/data/datasets/language_modeling.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/data/datasets/squad.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/data/datasets/squad.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/data/metrics/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/data/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/data/metrics/squad_metrics.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/data/metrics/squad_metrics.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/data/processors/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/data/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/data/processors/glue.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/data/processors/glue.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/data/processors/squad.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/data/processors/squad.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/data/processors/utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/data/processors/utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/data/processors/xnli.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/data/processors/xnli.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/debug_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/debug_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/deepspeed.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/deepspeed.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/dependency_versions_check.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/dependency_versions_check.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/dependency_versions_table.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/dependency_versions_table.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/dynamic_module_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/dynamic_module_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/feature_extraction_sequence_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/feature_extraction_sequence_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/feature_extraction_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/feature_extraction_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/file_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/file_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/generation/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/generation/beam_constraints.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/generation/beam_constraints.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/generation/beam_search.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/generation/beam_search.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/generation/configuration_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/generation/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/generation/flax_logits_process.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/generation/flax_logits_process.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/generation/flax_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/generation/flax_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/generation/logits_process.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/generation/logits_process.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/generation/stopping_criteria.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/generation/stopping_criteria.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/generation/streamers.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/generation/streamers.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/generation/tf_logits_process.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/generation/tf_logits_process.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/generation/tf_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/generation/tf_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/generation/utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/generation/utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/generation_flax_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/generation_flax_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/generation_tf_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/generation_tf_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/generation_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/generation_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/hf_argparser.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/hf_argparser.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/hyperparameter_search.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/hyperparameter_search.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/image_processing_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/image_processing_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/image_transforms.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/image_transforms.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/image_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/image_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/integrations.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/integrations.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/keras_callbacks.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/keras_callbacks.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/modelcard.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/modelcard.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/modeling_flax_outputs.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/modeling_flax_outputs.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/modeling_flax_pytorch_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/modeling_flax_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/modeling_flax_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/modeling_flax_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/modeling_outputs.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/modeling_outputs.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/modeling_tf_outputs.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/modeling_tf_outputs.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/modeling_tf_pytorch_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/modeling_tf_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/modeling_tf_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/modeling_tf_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/modeling_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/albert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/albert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/albert/configuration_albert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/albert/configuration_albert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/albert/convert_albert_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/albert/convert_albert_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/albert/modeling_albert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/albert/modeling_albert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/albert/modeling_flax_albert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/albert/modeling_flax_albert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/albert/modeling_tf_albert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/albert/modeling_tf_albert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/albert/tokenization_albert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/albert/tokenization_albert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/albert/tokenization_albert_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/albert/tokenization_albert_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/align/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/align/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/align/configuration_align.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/align/configuration_align.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/align/convert_align_tf_to_hf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/align/convert_align_tf_to_hf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/align/modeling_align.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/align/modeling_align.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/align/processing_align.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/align/processing_align.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/altclip/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/altclip/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/altclip/configuration_altclip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/altclip/configuration_altclip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/altclip/modeling_altclip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/altclip/modeling_altclip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/altclip/processing_altclip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/altclip/processing_altclip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/audio_spectrogram_transformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/audio_spectrogram_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/audio_spectrogram_transformer/configuration_audio_spectrogram_transformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/audio_spectrogram_transformer/configuration_audio_spectrogram_transformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/audio_spectrogram_transformer/convert_audio_spectrogram_transformer_original_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/audio_spectrogram_transformer/convert_audio_spectrogram_transformer_original_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/audio_spectrogram_transformer/feature_extraction_audio_spectrogram_transformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/audio_spectrogram_transformer/feature_extraction_audio_spectrogram_transformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/audio_spectrogram_transformer/modeling_audio_spectrogram_transformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/audio_spectrogram_transformer/modeling_audio_spectrogram_transformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/auto_factory.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/auto_factory.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/configuration_auto.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/configuration_auto.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/feature_extraction_auto.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/feature_extraction_auto.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/image_processing_auto.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/image_processing_auto.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/modeling_auto.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/modeling_auto.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/modeling_flax_auto.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/modeling_flax_auto.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/modeling_tf_auto.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/modeling_tf_auto.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/processing_auto.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/processing_auto.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/auto/tokenization_auto.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/auto/tokenization_auto.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/autoformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/autoformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/autoformer/configuration_autoformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/autoformer/configuration_autoformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/autoformer/modeling_autoformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/autoformer/modeling_autoformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bart/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bart/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bart/configuration_bart.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bart/configuration_bart.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bart/convert_bart_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bart/convert_bart_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bart/modeling_bart.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bart/modeling_bart.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bart/modeling_flax_bart.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bart/modeling_flax_bart.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bart/modeling_tf_bart.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bart/modeling_tf_bart.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bart/tokenization_bart.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bart/tokenization_bart.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bart/tokenization_bart_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bart/tokenization_bart_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/barthez/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/barthez/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/barthez/tokenization_barthez.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/barthez/tokenization_barthez.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/barthez/tokenization_barthez_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/barthez/tokenization_barthez_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bartpho/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bartpho/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bartpho/tokenization_bartpho.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bartpho/tokenization_bartpho.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/beit/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/beit/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/beit/configuration_beit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/beit/configuration_beit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/beit/convert_beit_unilm_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/beit/convert_beit_unilm_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/beit/feature_extraction_beit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/beit/feature_extraction_beit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/beit/image_processing_beit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/beit/image_processing_beit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/beit/modeling_beit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/beit/modeling_beit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/beit/modeling_flax_beit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/beit/modeling_flax_beit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/configuration_bert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/configuration_bert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/convert_bert_original_tf2_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/convert_bert_original_tf2_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/convert_bert_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/convert_bert_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/convert_bert_pytorch_checkpoint_to_original_tf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/convert_bert_pytorch_checkpoint_to_original_tf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/convert_bert_token_dropping_original_tf2_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/convert_bert_token_dropping_original_tf2_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/modeling_bert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/modeling_bert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/modeling_flax_bert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/modeling_flax_bert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/modeling_tf_bert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/modeling_tf_bert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/tokenization_bert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/tokenization_bert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/tokenization_bert_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/tokenization_bert_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert/tokenization_bert_tf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert/tokenization_bert_tf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert_generation/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert_generation/configuration_bert_generation.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert_generation/configuration_bert_generation.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert_generation/modeling_bert_generation.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert_generation/modeling_bert_generation.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert_generation/tokenization_bert_generation.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert_generation/tokenization_bert_generation.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert_japanese/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert_japanese/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bert_japanese/tokenization_bert_japanese.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bert_japanese/tokenization_bert_japanese.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bertweet/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bertweet/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bertweet/tokenization_bertweet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bertweet/tokenization_bertweet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/big_bird/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/big_bird/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/big_bird/configuration_big_bird.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/big_bird/configuration_big_bird.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/big_bird/convert_bigbird_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/big_bird/convert_bigbird_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/big_bird/modeling_big_bird.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/big_bird/modeling_big_bird.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/big_bird/modeling_flax_big_bird.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/big_bird/modeling_flax_big_bird.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/big_bird/tokenization_big_bird.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/big_bird/tokenization_big_bird.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/big_bird/tokenization_big_bird_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/big_bird/tokenization_big_bird_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bigbird_pegasus/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bigbird_pegasus/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bigbird_pegasus/configuration_bigbird_pegasus.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bigbird_pegasus/configuration_bigbird_pegasus.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bigbird_pegasus/convert_bigbird_pegasus_tf_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bigbird_pegasus/convert_bigbird_pegasus_tf_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bigbird_pegasus/modeling_bigbird_pegasus.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bigbird_pegasus/modeling_bigbird_pegasus.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/biogpt/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/biogpt/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/biogpt/configuration_biogpt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/biogpt/configuration_biogpt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/biogpt/convert_biogpt_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/biogpt/convert_biogpt_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/biogpt/modeling_biogpt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/biogpt/modeling_biogpt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/biogpt/tokenization_biogpt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/biogpt/tokenization_biogpt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bit/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bit/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bit/configuration_bit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bit/configuration_bit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bit/convert_bit_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bit/convert_bit_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bit/image_processing_bit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bit/image_processing_bit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bit/modeling_bit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bit/modeling_bit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot/configuration_blenderbot.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot/configuration_blenderbot.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot/convert_blenderbot_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot/convert_blenderbot_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot/modeling_blenderbot.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot/modeling_blenderbot.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot/modeling_flax_blenderbot.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot/modeling_flax_blenderbot.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot/modeling_tf_blenderbot.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot/modeling_tf_blenderbot.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot/tokenization_blenderbot.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot/tokenization_blenderbot.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot/tokenization_blenderbot_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot/tokenization_blenderbot_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot_small/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot_small/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot_small/configuration_blenderbot_small.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot_small/configuration_blenderbot_small.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot_small/modeling_blenderbot_small.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot_small/modeling_blenderbot_small.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot_small/modeling_flax_blenderbot_small.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot_small/modeling_flax_blenderbot_small.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot_small/modeling_tf_blenderbot_small.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot_small/modeling_tf_blenderbot_small.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot_small/tokenization_blenderbot_small.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot_small/tokenization_blenderbot_small.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blenderbot_small/tokenization_blenderbot_small_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blenderbot_small/tokenization_blenderbot_small_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/configuration_blip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/configuration_blip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/convert_blip_original_pytorch_to_hf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/convert_blip_original_pytorch_to_hf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/image_processing_blip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/image_processing_blip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/modeling_blip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/modeling_blip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/modeling_blip_text.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/modeling_blip_text.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/modeling_tf_blip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/modeling_tf_blip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/modeling_tf_blip_text.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/modeling_tf_blip_text.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blip/processing_blip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blip/processing_blip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blip_2/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blip_2/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blip_2/configuration_blip_2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blip_2/configuration_blip_2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blip_2/convert_blip_2_original_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blip_2/convert_blip_2_original_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blip_2/modeling_blip_2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blip_2/modeling_blip_2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/blip_2/processing_blip_2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/blip_2/processing_blip_2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bloom/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bloom/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bloom/configuration_bloom.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bloom/configuration_bloom.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bloom/convert_bloom_original_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bloom/convert_bloom_original_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bloom/modeling_bloom.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bloom/modeling_bloom.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bloom/tokenization_bloom_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bloom/tokenization_bloom_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bridgetower/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bridgetower/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bridgetower/configuration_bridgetower.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bridgetower/configuration_bridgetower.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bridgetower/image_processing_bridgetower.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bridgetower/image_processing_bridgetower.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bridgetower/modeling_bridgetower.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bridgetower/modeling_bridgetower.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/bridgetower/processing_bridgetower.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/bridgetower/processing_bridgetower.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/byt5/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/byt5/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/byt5/convert_byt5_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/byt5/convert_byt5_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/byt5/tokenization_byt5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/byt5/tokenization_byt5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/camembert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/camembert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/camembert/configuration_camembert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/camembert/configuration_camembert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/camembert/modeling_camembert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/camembert/modeling_camembert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/camembert/modeling_tf_camembert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/camembert/modeling_tf_camembert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/camembert/tokenization_camembert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/camembert/tokenization_camembert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/camembert/tokenization_camembert_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/camembert/tokenization_camembert_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/canine/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/canine/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/canine/configuration_canine.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/canine/configuration_canine.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/canine/convert_canine_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/canine/convert_canine_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/canine/modeling_canine.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/canine/modeling_canine.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/canine/tokenization_canine.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/canine/tokenization_canine.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/chinese_clip/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/chinese_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/chinese_clip/configuration_chinese_clip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/chinese_clip/configuration_chinese_clip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/chinese_clip/convert_chinese_clip_original_pytorch_to_hf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/chinese_clip/convert_chinese_clip_original_pytorch_to_hf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/chinese_clip/feature_extraction_chinese_clip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/chinese_clip/feature_extraction_chinese_clip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/chinese_clip/image_processing_chinese_clip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/chinese_clip/image_processing_chinese_clip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/chinese_clip/modeling_chinese_clip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/chinese_clip/modeling_chinese_clip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/chinese_clip/processing_chinese_clip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/chinese_clip/processing_chinese_clip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clap/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clap/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clap/configuration_clap.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clap/configuration_clap.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clap/convert_clap_original_pytorch_to_hf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clap/convert_clap_original_pytorch_to_hf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clap/feature_extraction_clap.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clap/feature_extraction_clap.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clap/modeling_clap.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clap/modeling_clap.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clap/processing_clap.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clap/processing_clap.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/configuration_clip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/configuration_clip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/convert_clip_original_pytorch_to_hf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/convert_clip_original_pytorch_to_hf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/feature_extraction_clip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/feature_extraction_clip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/image_processing_clip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/image_processing_clip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/modeling_clip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/modeling_clip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/modeling_flax_clip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/modeling_flax_clip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/modeling_tf_clip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/modeling_tf_clip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/processing_clip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/processing_clip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/tokenization_clip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/tokenization_clip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clip/tokenization_clip_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clip/tokenization_clip_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clipseg/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clipseg/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clipseg/configuration_clipseg.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clipseg/configuration_clipseg.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clipseg/convert_clipseg_original_pytorch_to_hf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clipseg/convert_clipseg_original_pytorch_to_hf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clipseg/modeling_clipseg.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clipseg/modeling_clipseg.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/clipseg/processing_clipseg.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/clipseg/processing_clipseg.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/codegen/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/codegen/configuration_codegen.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/codegen/configuration_codegen.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/codegen/modeling_codegen.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/codegen/modeling_codegen.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/codegen/tokenization_codegen.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/codegen/tokenization_codegen.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/codegen/tokenization_codegen_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/codegen/tokenization_codegen_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/conditional_detr/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/conditional_detr/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/conditional_detr/configuration_conditional_detr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/conditional_detr/configuration_conditional_detr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/conditional_detr/convert_conditional_detr_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/conditional_detr/convert_conditional_detr_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/conditional_detr/feature_extraction_conditional_detr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/conditional_detr/feature_extraction_conditional_detr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/conditional_detr/image_processing_conditional_detr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/conditional_detr/image_processing_conditional_detr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/conditional_detr/modeling_conditional_detr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/conditional_detr/modeling_conditional_detr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convbert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convbert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convbert/configuration_convbert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convbert/configuration_convbert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convbert/convert_convbert_original_tf1_checkpoint_to_pytorch_and_tf2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convbert/convert_convbert_original_tf1_checkpoint_to_pytorch_and_tf2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convbert/modeling_convbert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convbert/modeling_convbert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convbert/modeling_tf_convbert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convbert/modeling_tf_convbert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convbert/tokenization_convbert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convbert/tokenization_convbert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convbert/tokenization_convbert_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convbert/tokenization_convbert_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convnext/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convnext/configuration_convnext.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convnext/configuration_convnext.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convnext/convert_convnext_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convnext/convert_convnext_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convnext/feature_extraction_convnext.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convnext/feature_extraction_convnext.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convnext/image_processing_convnext.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convnext/image_processing_convnext.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convnext/modeling_convnext.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convnext/modeling_convnext.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convnext/modeling_tf_convnext.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convnext/modeling_tf_convnext.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convnextv2/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convnextv2/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convnextv2/configuration_convnextv2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convnextv2/configuration_convnextv2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convnextv2/convert_convnextv2_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convnextv2/convert_convnextv2_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/convnextv2/modeling_convnextv2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/convnextv2/modeling_convnextv2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/cpm/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/cpm/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/cpm/tokenization_cpm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/cpm/tokenization_cpm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/cpm/tokenization_cpm_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/cpm/tokenization_cpm_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/cpmant/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/cpmant/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/cpmant/configuration_cpmant.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/cpmant/configuration_cpmant.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/cpmant/modeling_cpmant.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/cpmant/modeling_cpmant.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/cpmant/tokenization_cpmant.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/cpmant/tokenization_cpmant.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/ctrl/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/ctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/ctrl/configuration_ctrl.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/ctrl/configuration_ctrl.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/ctrl/modeling_ctrl.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/ctrl/modeling_ctrl.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/ctrl/modeling_tf_ctrl.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/ctrl/modeling_tf_ctrl.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/ctrl/tokenization_ctrl.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/ctrl/tokenization_ctrl.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/cvt/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/cvt/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/cvt/configuration_cvt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/cvt/configuration_cvt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/cvt/convert_cvt_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/cvt/convert_cvt_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/cvt/modeling_cvt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/cvt/modeling_cvt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/cvt/modeling_tf_cvt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/cvt/modeling_tf_cvt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/configuration_data2vec_audio.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/configuration_data2vec_audio.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/configuration_data2vec_text.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/configuration_data2vec_text.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/configuration_data2vec_vision.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/configuration_data2vec_vision.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/convert_data2vec_audio_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/convert_data2vec_audio_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/convert_data2vec_text_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/convert_data2vec_text_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/convert_data2vec_vision_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/convert_data2vec_vision_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/modeling_data2vec_audio.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/modeling_data2vec_audio.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/modeling_data2vec_text.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/modeling_data2vec_text.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/modeling_data2vec_vision.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/modeling_data2vec_vision.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/data2vec/modeling_tf_data2vec_vision.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/data2vec/modeling_tf_data2vec_vision.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta/configuration_deberta.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta/configuration_deberta.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta/modeling_deberta.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta/modeling_deberta.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta/modeling_tf_deberta.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta/modeling_tf_deberta.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta/tokenization_deberta.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta/tokenization_deberta.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta/tokenization_deberta_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta/tokenization_deberta_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta_v2/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta_v2/configuration_deberta_v2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta_v2/configuration_deberta_v2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta_v2/modeling_deberta_v2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta_v2/modeling_deberta_v2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta_v2/modeling_tf_deberta_v2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta_v2/modeling_tf_deberta_v2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta_v2/tokenization_deberta_v2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta_v2/tokenization_deberta_v2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deberta_v2/tokenization_deberta_v2_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deberta_v2/tokenization_deberta_v2_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/decision_transformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/decision_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/decision_transformer/configuration_decision_transformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/decision_transformer/configuration_decision_transformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/decision_transformer/modeling_decision_transformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/decision_transformer/modeling_decision_transformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deformable_detr/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deformable_detr/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deformable_detr/configuration_deformable_detr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deformable_detr/configuration_deformable_detr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deformable_detr/convert_deformable_detr_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deformable_detr/convert_deformable_detr_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deformable_detr/feature_extraction_deformable_detr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deformable_detr/feature_extraction_deformable_detr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deformable_detr/image_processing_deformable_detr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deformable_detr/image_processing_deformable_detr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deformable_detr/load_custom.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deformable_detr/load_custom.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deformable_detr/modeling_deformable_detr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deformable_detr/modeling_deformable_detr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deit/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deit/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deit/configuration_deit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deit/configuration_deit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deit/convert_deit_timm_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deit/convert_deit_timm_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deit/feature_extraction_deit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deit/feature_extraction_deit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deit/image_processing_deit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deit/image_processing_deit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deit/modeling_deit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deit/modeling_deit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deit/modeling_tf_deit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deit/modeling_tf_deit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/bort/convert_bort_original_gluonnlp_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/bort/convert_bort_original_gluonnlp_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mctct/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mctct/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mctct/configuration_mctct.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mctct/configuration_mctct.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mctct/feature_extraction_mctct.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mctct/feature_extraction_mctct.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mctct/modeling_mctct.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mctct/modeling_mctct.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mctct/processing_mctct.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mctct/processing_mctct.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mmbt/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mmbt/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mmbt/configuration_mmbt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mmbt/configuration_mmbt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/mmbt/modeling_mmbt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/mmbt/modeling_mmbt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/retribert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/retribert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/retribert/configuration_retribert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/retribert/configuration_retribert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/retribert/modeling_retribert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/retribert/modeling_retribert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/retribert/tokenization_retribert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/retribert/tokenization_retribert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/retribert/tokenization_retribert_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/retribert/tokenization_retribert_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/tapex/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/tapex/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/tapex/tokenization_tapex.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/tapex/tokenization_tapex.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/configuration_trajectory_transformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/configuration_trajectory_transformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/convert_trajectory_transformer_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/convert_trajectory_transformer_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/modeling_trajectory_transformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/trajectory_transformer/modeling_trajectory_transformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/van/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/van/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/van/configuration_van.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/van/configuration_van.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/van/convert_van_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/van/convert_van_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deprecated/van/modeling_van.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deprecated/van/modeling_van.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deta/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deta/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deta/configuration_deta.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deta/configuration_deta.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deta/convert_deta_resnet_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deta/convert_deta_resnet_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deta/convert_deta_swin_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deta/convert_deta_swin_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deta/image_processing_deta.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deta/image_processing_deta.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/deta/modeling_deta.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/deta/modeling_deta.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/detr/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/detr/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/detr/configuration_detr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/detr/configuration_detr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/detr/convert_detr_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/detr/convert_detr_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/detr/convert_detr_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/detr/convert_detr_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/detr/feature_extraction_detr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/detr/feature_extraction_detr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/detr/image_processing_detr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/detr/image_processing_detr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/detr/modeling_detr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/detr/modeling_detr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dialogpt/convert_dialogpt_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dialogpt/convert_dialogpt_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dinat/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dinat/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dinat/configuration_dinat.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dinat/configuration_dinat.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dinat/modeling_dinat.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dinat/modeling_dinat.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/distilbert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/distilbert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/distilbert/configuration_distilbert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/distilbert/configuration_distilbert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/distilbert/modeling_distilbert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/distilbert/modeling_distilbert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/distilbert/modeling_flax_distilbert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/distilbert/modeling_flax_distilbert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/distilbert/modeling_tf_distilbert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/distilbert/modeling_tf_distilbert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/distilbert/tokenization_distilbert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/distilbert/tokenization_distilbert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/distilbert/tokenization_distilbert_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/distilbert/tokenization_distilbert_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dit/convert_dit_unilm_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dit/convert_dit_unilm_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/donut/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/donut/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/donut/configuration_donut_swin.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/donut/configuration_donut_swin.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/donut/convert_donut_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/donut/convert_donut_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/donut/feature_extraction_donut.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/donut/feature_extraction_donut.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/donut/image_processing_donut.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/donut/image_processing_donut.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/donut/modeling_donut_swin.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/donut/modeling_donut_swin.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/donut/processing_donut.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/donut/processing_donut.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dpr/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dpr/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dpr/configuration_dpr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dpr/configuration_dpr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dpr/convert_dpr_original_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dpr/convert_dpr_original_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dpr/modeling_dpr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dpr/modeling_dpr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dpr/modeling_tf_dpr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dpr/modeling_tf_dpr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dpr/tokenization_dpr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dpr/tokenization_dpr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dpr/tokenization_dpr_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dpr/tokenization_dpr_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dpt/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dpt/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dpt/configuration_dpt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dpt/configuration_dpt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dpt/convert_dpt_hybrid_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dpt/convert_dpt_hybrid_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dpt/convert_dpt_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dpt/convert_dpt_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dpt/feature_extraction_dpt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dpt/feature_extraction_dpt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dpt/image_processing_dpt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dpt/image_processing_dpt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/dpt/modeling_dpt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/dpt/modeling_dpt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientformer/configuration_efficientformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientformer/configuration_efficientformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientformer/convert_efficientformer_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientformer/convert_efficientformer_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientformer/image_processing_efficientformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientformer/image_processing_efficientformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientformer/modeling_efficientformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientformer/modeling_efficientformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientformer/modeling_tf_efficientformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientformer/modeling_tf_efficientformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientnet/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientnet/configuration_efficientnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientnet/configuration_efficientnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientnet/convert_efficientnet_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientnet/convert_efficientnet_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientnet/image_processing_efficientnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientnet/image_processing_efficientnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/efficientnet/modeling_efficientnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/efficientnet/modeling_efficientnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/electra/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/electra/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/electra/configuration_electra.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/electra/configuration_electra.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/electra/convert_electra_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/electra/convert_electra_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/electra/modeling_electra.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/electra/modeling_electra.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/electra/modeling_flax_electra.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/electra/modeling_flax_electra.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/electra/modeling_tf_electra.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/electra/modeling_tf_electra.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/electra/tokenization_electra.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/electra/tokenization_electra.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/electra/tokenization_electra_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/electra/tokenization_electra_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/encodec/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/encodec/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/encodec/configuration_encodec.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/encodec/configuration_encodec.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/encodec/convert_encodec_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/encodec/convert_encodec_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/encodec/feature_extraction_encodec.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/encodec/feature_extraction_encodec.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/encodec/modeling_encodec.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/encodec/modeling_encodec.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/encoder_decoder/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/encoder_decoder/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/encoder_decoder/configuration_encoder_decoder.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/encoder_decoder/configuration_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/encoder_decoder/modeling_encoder_decoder.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/encoder_decoder/modeling_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/encoder_decoder/modeling_flax_encoder_decoder.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/encoder_decoder/modeling_flax_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/encoder_decoder/modeling_tf_encoder_decoder.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/encoder_decoder/modeling_tf_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/ernie/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/ernie/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/ernie/configuration_ernie.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/ernie/configuration_ernie.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/ernie/modeling_ernie.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/ernie/modeling_ernie.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/ernie_m/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/ernie_m/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/ernie_m/configuration_ernie_m.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/ernie_m/configuration_ernie_m.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/ernie_m/modeling_ernie_m.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/ernie_m/modeling_ernie_m.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/ernie_m/tokenization_ernie_m.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/ernie_m/tokenization_ernie_m.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/configuration_esm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/configuration_esm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/convert_esm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/convert_esm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/modeling_esm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/modeling_esm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/modeling_esmfold.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/modeling_esmfold.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/modeling_tf_esm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/modeling_tf_esm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/chunk_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/chunk_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/data_transforms.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/data_transforms.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/feats.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/feats.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/loss.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/loss.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/protein.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/protein.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/residue_constants.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/residue_constants.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/rigid_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/rigid_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/openfold_utils/tensor_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/openfold_utils/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/esm/tokenization_esm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/esm/tokenization_esm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/falcon/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/falcon/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/falcon/configuration_falcon.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/falcon/configuration_falcon.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/falcon/modeling_falcon.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/falcon/modeling_falcon.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/flaubert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/flaubert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/flaubert/configuration_flaubert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/flaubert/configuration_flaubert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/flaubert/modeling_flaubert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/flaubert/modeling_flaubert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/flaubert/modeling_tf_flaubert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/flaubert/modeling_tf_flaubert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/flaubert/tokenization_flaubert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/flaubert/tokenization_flaubert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/flava/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/flava/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/flava/configuration_flava.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/flava/configuration_flava.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/flava/convert_dalle_to_flava_codebook.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/flava/convert_dalle_to_flava_codebook.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/flava/convert_flava_original_pytorch_to_hf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/flava/convert_flava_original_pytorch_to_hf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/flava/feature_extraction_flava.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/flava/feature_extraction_flava.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/flava/image_processing_flava.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/flava/image_processing_flava.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/flava/modeling_flava.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/flava/modeling_flava.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/flava/processing_flava.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/flava/processing_flava.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/fnet/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/fnet/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/fnet/configuration_fnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/fnet/configuration_fnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/fnet/convert_fnet_original_flax_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/fnet/convert_fnet_original_flax_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/fnet/modeling_fnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/fnet/modeling_fnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/fnet/tokenization_fnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/fnet/tokenization_fnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/fnet/tokenization_fnet_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/fnet/tokenization_fnet_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/focalnet/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/focalnet/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/focalnet/configuration_focalnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/focalnet/configuration_focalnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/focalnet/convert_focalnet_to_hf_format.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/focalnet/convert_focalnet_to_hf_format.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/focalnet/modeling_focalnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/focalnet/modeling_focalnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/fsmt/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/fsmt/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/fsmt/configuration_fsmt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/fsmt/configuration_fsmt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/fsmt/convert_fsmt_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/fsmt/convert_fsmt_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/fsmt/modeling_fsmt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/fsmt/modeling_fsmt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/fsmt/tokenization_fsmt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/fsmt/tokenization_fsmt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/funnel/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/funnel/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/funnel/configuration_funnel.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/funnel/configuration_funnel.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/funnel/convert_funnel_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/funnel/convert_funnel_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/funnel/modeling_funnel.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/funnel/modeling_funnel.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/funnel/modeling_tf_funnel.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/funnel/modeling_tf_funnel.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/funnel/tokenization_funnel.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/funnel/tokenization_funnel.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/funnel/tokenization_funnel_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/funnel/tokenization_funnel_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/git/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/git/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/git/configuration_git.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/git/configuration_git.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/git/convert_git_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/git/convert_git_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/git/modeling_git.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/git/modeling_git.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/git/processing_git.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/git/processing_git.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/glpn/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/glpn/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/glpn/configuration_glpn.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/glpn/configuration_glpn.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/glpn/convert_glpn_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/glpn/convert_glpn_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/glpn/feature_extraction_glpn.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/glpn/feature_extraction_glpn.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/glpn/image_processing_glpn.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/glpn/image_processing_glpn.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/glpn/modeling_glpn.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/glpn/modeling_glpn.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/configuration_gpt2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/configuration_gpt2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/convert_gpt2_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/convert_gpt2_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/modeling_flax_gpt2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/modeling_flax_gpt2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/modeling_gpt2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/modeling_gpt2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/modeling_tf_gpt2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/modeling_tf_gpt2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/tokenization_gpt2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/tokenization_gpt2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/tokenization_gpt2_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/tokenization_gpt2_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt2/tokenization_gpt2_tf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt2/tokenization_gpt2_tf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_bigcode/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_bigcode/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_bigcode/configuration_gpt_bigcode.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_bigcode/configuration_gpt_bigcode.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_bigcode/modeling_gpt_bigcode.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_bigcode/modeling_gpt_bigcode.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neo/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neo/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neo/configuration_gpt_neo.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neo/configuration_gpt_neo.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neo/convert_gpt_neo_mesh_tf_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neo/convert_gpt_neo_mesh_tf_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neo/modeling_flax_gpt_neo.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neo/modeling_flax_gpt_neo.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neo/modeling_gpt_neo.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neo/modeling_gpt_neo.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox/configuration_gpt_neox.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox/configuration_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox/modeling_gpt_neox.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox/modeling_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox/tokenization_gpt_neox_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox/tokenization_gpt_neox_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox_japanese/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox_japanese/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox_japanese/configuration_gpt_neox_japanese.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox_japanese/configuration_gpt_neox_japanese.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox_japanese/modeling_gpt_neox_japanese.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox_japanese/modeling_gpt_neox_japanese.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_neox_japanese/tokenization_gpt_neox_japanese.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_neox_japanese/tokenization_gpt_neox_japanese.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_sw3/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_sw3/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_sw3/convert_megatron_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_sw3/convert_megatron_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gpt_sw3/tokenization_gpt_sw3.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gpt_sw3/tokenization_gpt_sw3.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gptj/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gptj/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gptj/configuration_gptj.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gptj/configuration_gptj.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gptj/modeling_flax_gptj.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gptj/modeling_flax_gptj.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gptj/modeling_gptj.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gptj/modeling_gptj.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gptj/modeling_tf_gptj.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gptj/modeling_tf_gptj.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gptsan_japanese/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gptsan_japanese/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gptsan_japanese/configuration_gptsan_japanese.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gptsan_japanese/configuration_gptsan_japanese.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gptsan_japanese/convert_gptsan_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gptsan_japanese/convert_gptsan_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gptsan_japanese/modeling_gptsan_japanese.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gptsan_japanese/modeling_gptsan_japanese.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/gptsan_japanese/tokenization_gptsan_japanese.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/gptsan_japanese/tokenization_gptsan_japanese.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/graphormer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/graphormer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/graphormer/collating_graphormer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/graphormer/collating_graphormer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/graphormer/configuration_graphormer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/graphormer/configuration_graphormer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/graphormer/modeling_graphormer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/graphormer/modeling_graphormer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/groupvit/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/groupvit/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/groupvit/configuration_groupvit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/groupvit/configuration_groupvit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/groupvit/convert_groupvit_nvlab_to_hf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/groupvit/convert_groupvit_nvlab_to_hf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/groupvit/modeling_groupvit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/groupvit/modeling_groupvit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/groupvit/modeling_tf_groupvit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/groupvit/modeling_tf_groupvit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/herbert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/herbert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/herbert/tokenization_herbert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/herbert/tokenization_herbert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/herbert/tokenization_herbert_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/herbert/tokenization_herbert_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/hubert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/hubert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/hubert/configuration_hubert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/hubert/configuration_hubert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/hubert/convert_distilhubert_original_s3prl_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/hubert/convert_distilhubert_original_s3prl_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/hubert/convert_hubert_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/hubert/convert_hubert_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/hubert/convert_hubert_original_s3prl_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/hubert/convert_hubert_original_s3prl_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/hubert/modeling_hubert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/hubert/modeling_hubert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/hubert/modeling_tf_hubert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/hubert/modeling_tf_hubert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/ibert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/ibert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/ibert/configuration_ibert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/ibert/configuration_ibert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/ibert/modeling_ibert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/ibert/modeling_ibert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/ibert/quant_modules.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/ibert/quant_modules.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/imagegpt/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/imagegpt/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/imagegpt/configuration_imagegpt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/imagegpt/configuration_imagegpt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/imagegpt/convert_imagegpt_original_tf2_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/imagegpt/convert_imagegpt_original_tf2_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/imagegpt/feature_extraction_imagegpt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/imagegpt/feature_extraction_imagegpt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/imagegpt/image_processing_imagegpt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/imagegpt/image_processing_imagegpt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/imagegpt/modeling_imagegpt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/imagegpt/modeling_imagegpt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/informer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/informer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/informer/configuration_informer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/informer/configuration_informer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/informer/modeling_informer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/informer/modeling_informer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/instructblip/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/instructblip/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/instructblip/configuration_instructblip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/instructblip/configuration_instructblip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/instructblip/convert_instructblip_original_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/instructblip/convert_instructblip_original_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/instructblip/modeling_instructblip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/instructblip/modeling_instructblip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/instructblip/processing_instructblip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/instructblip/processing_instructblip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/jukebox/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/jukebox/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/jukebox/configuration_jukebox.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/jukebox/configuration_jukebox.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/jukebox/convert_jukebox.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/jukebox/convert_jukebox.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/jukebox/modeling_jukebox.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/jukebox/modeling_jukebox.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/jukebox/tokenization_jukebox.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/jukebox/tokenization_jukebox.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlm/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlm/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlm/configuration_layoutlm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlm/configuration_layoutlm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlm/modeling_layoutlm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlm/modeling_layoutlm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlm/modeling_tf_layoutlm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlm/modeling_tf_layoutlm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlm/tokenization_layoutlm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlm/tokenization_layoutlm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlm/tokenization_layoutlm_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlm/tokenization_layoutlm_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv2/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv2/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv2/configuration_layoutlmv2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv2/configuration_layoutlmv2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv2/feature_extraction_layoutlmv2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv2/feature_extraction_layoutlmv2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv2/image_processing_layoutlmv2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv2/image_processing_layoutlmv2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv2/modeling_layoutlmv2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv2/modeling_layoutlmv2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv2/processing_layoutlmv2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv2/processing_layoutlmv2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv2/tokenization_layoutlmv2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv2/tokenization_layoutlmv2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv2/tokenization_layoutlmv2_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv2/tokenization_layoutlmv2_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/configuration_layoutlmv3.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/configuration_layoutlmv3.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/feature_extraction_layoutlmv3.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/feature_extraction_layoutlmv3.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/image_processing_layoutlmv3.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/image_processing_layoutlmv3.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/modeling_layoutlmv3.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/modeling_layoutlmv3.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/modeling_tf_layoutlmv3.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/modeling_tf_layoutlmv3.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/processing_layoutlmv3.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/processing_layoutlmv3.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/tokenization_layoutlmv3.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/tokenization_layoutlmv3.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutlmv3/tokenization_layoutlmv3_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutlmv3/tokenization_layoutlmv3_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutxlm/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutxlm/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutxlm/processing_layoutxlm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutxlm/processing_layoutxlm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutxlm/tokenization_layoutxlm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutxlm/tokenization_layoutxlm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/layoutxlm/tokenization_layoutxlm_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/layoutxlm/tokenization_layoutxlm_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/led/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/led/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/led/configuration_led.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/led/configuration_led.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/led/modeling_led.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/led/modeling_led.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/led/modeling_tf_led.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/led/modeling_tf_led.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/led/tokenization_led.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/led/tokenization_led.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/led/tokenization_led_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/led/tokenization_led_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/levit/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/levit/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/levit/configuration_levit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/levit/configuration_levit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/levit/convert_levit_timm_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/levit/convert_levit_timm_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/levit/feature_extraction_levit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/levit/feature_extraction_levit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/levit/image_processing_levit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/levit/image_processing_levit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/levit/modeling_levit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/levit/modeling_levit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/lilt/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/lilt/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/lilt/configuration_lilt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/lilt/configuration_lilt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/lilt/modeling_lilt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/lilt/modeling_lilt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/llama/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/llama/configuration_llama.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/llama/configuration_llama.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/llama/convert_llama_weights_to_hf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/llama/convert_llama_weights_to_hf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/llama/modeling_llama.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/llama/modeling_llama.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/llama/tokenization_llama.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/llama/tokenization_llama.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/llama/tokenization_llama_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/llama/tokenization_llama_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/longformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/longformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/longformer/configuration_longformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/longformer/configuration_longformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/longformer/convert_longformer_original_pytorch_lightning_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/longformer/convert_longformer_original_pytorch_lightning_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/longformer/modeling_longformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/longformer/modeling_longformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/longformer/modeling_tf_longformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/longformer/modeling_tf_longformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/longformer/tokenization_longformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/longformer/tokenization_longformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/longformer/tokenization_longformer_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/longformer/tokenization_longformer_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/longt5/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/longt5/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/longt5/configuration_longt5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/longt5/configuration_longt5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/longt5/convert_longt5x_checkpoint_to_flax.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/longt5/convert_longt5x_checkpoint_to_flax.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/longt5/modeling_flax_longt5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/longt5/modeling_flax_longt5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/longt5/modeling_longt5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/longt5/modeling_longt5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/luke/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/luke/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/luke/configuration_luke.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/luke/configuration_luke.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/luke/convert_luke_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/luke/convert_luke_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/luke/modeling_luke.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/luke/modeling_luke.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/luke/tokenization_luke.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/luke/tokenization_luke.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/lxmert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/lxmert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/lxmert/configuration_lxmert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/lxmert/configuration_lxmert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/lxmert/convert_lxmert_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/lxmert/convert_lxmert_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/lxmert/modeling_lxmert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/lxmert/modeling_lxmert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/lxmert/modeling_tf_lxmert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/lxmert/modeling_tf_lxmert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/lxmert/tokenization_lxmert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/lxmert/tokenization_lxmert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/lxmert/tokenization_lxmert_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/lxmert/tokenization_lxmert_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/m2m_100/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/m2m_100/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/m2m_100/configuration_m2m_100.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/m2m_100/configuration_m2m_100.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/m2m_100/convert_m2m100_original_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/m2m_100/convert_m2m100_original_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/m2m_100/modeling_m2m_100.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/m2m_100/modeling_m2m_100.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/m2m_100/tokenization_m2m_100.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/m2m_100/tokenization_m2m_100.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/marian/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/marian/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/marian/configuration_marian.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/marian/configuration_marian.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/marian/convert_marian_tatoeba_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/marian/convert_marian_tatoeba_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/marian/convert_marian_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/marian/convert_marian_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/marian/modeling_flax_marian.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/marian/modeling_flax_marian.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/marian/modeling_marian.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/marian/modeling_marian.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/marian/modeling_tf_marian.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/marian/modeling_tf_marian.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/marian/tokenization_marian.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/marian/tokenization_marian.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/markuplm/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/markuplm/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/markuplm/configuration_markuplm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/markuplm/configuration_markuplm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/markuplm/feature_extraction_markuplm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/markuplm/feature_extraction_markuplm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/markuplm/modeling_markuplm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/markuplm/modeling_markuplm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/markuplm/processing_markuplm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/markuplm/processing_markuplm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/markuplm/tokenization_markuplm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/markuplm/tokenization_markuplm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/markuplm/tokenization_markuplm_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/markuplm/tokenization_markuplm_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mask2former/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mask2former/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mask2former/configuration_mask2former.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mask2former/configuration_mask2former.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mask2former/convert_mask2former_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mask2former/convert_mask2former_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mask2former/image_processing_mask2former.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mask2former/image_processing_mask2former.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mask2former/modeling_mask2former.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mask2former/modeling_mask2former.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/configuration_maskformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/configuration_maskformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/configuration_maskformer_swin.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/configuration_maskformer_swin.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/convert_maskformer_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/convert_maskformer_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/convert_maskformer_resnet_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/convert_maskformer_resnet_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/convert_maskformer_swin_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/convert_maskformer_swin_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/feature_extraction_maskformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/feature_extraction_maskformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/image_processing_maskformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/image_processing_maskformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/modeling_maskformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/modeling_maskformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/maskformer/modeling_maskformer_swin.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/maskformer/modeling_maskformer_swin.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart/configuration_mbart.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart/configuration_mbart.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart/convert_mbart_original_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart/convert_mbart_original_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart/modeling_flax_mbart.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart/modeling_flax_mbart.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart/modeling_mbart.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart/modeling_mbart.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart/modeling_tf_mbart.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart/modeling_tf_mbart.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart/tokenization_mbart.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart/tokenization_mbart.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart/tokenization_mbart_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart/tokenization_mbart_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart50/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart50/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart50/tokenization_mbart50.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart50/tokenization_mbart50.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mbart50/tokenization_mbart50_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mbart50/tokenization_mbart50_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mega/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mega/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mega/configuration_mega.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mega/configuration_mega.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mega/convert_mega_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mega/convert_mega_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mega/modeling_mega.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mega/modeling_mega.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/megatron_bert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/megatron_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/megatron_bert/configuration_megatron_bert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/megatron_bert/configuration_megatron_bert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/megatron_bert/convert_megatron_bert_checkpoint.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/megatron_bert/convert_megatron_bert_checkpoint.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/megatron_bert/modeling_megatron_bert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/megatron_bert/modeling_megatron_bert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/megatron_gpt2/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/megatron_gpt2/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/megatron_gpt2/checkpoint_reshaping_and_interoperability.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/megatron_gpt2/checkpoint_reshaping_and_interoperability.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/megatron_gpt2/convert_megatron_gpt2_checkpoint.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/megatron_gpt2/convert_megatron_gpt2_checkpoint.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mgp_str/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mgp_str/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mgp_str/configuration_mgp_str.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mgp_str/configuration_mgp_str.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mgp_str/modeling_mgp_str.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mgp_str/modeling_mgp_str.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mgp_str/processing_mgp_str.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mgp_str/processing_mgp_str.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mgp_str/tokenization_mgp_str.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mgp_str/tokenization_mgp_str.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mluke/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mluke/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mluke/convert_mluke_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mluke/convert_mluke_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mluke/tokenization_mluke.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mluke/tokenization_mluke.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilebert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilebert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilebert/configuration_mobilebert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilebert/configuration_mobilebert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilebert/convert_mobilebert_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilebert/convert_mobilebert_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilebert/modeling_mobilebert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilebert/modeling_mobilebert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilebert/modeling_tf_mobilebert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilebert/modeling_tf_mobilebert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilebert/tokenization_mobilebert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilebert/tokenization_mobilebert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilebert/tokenization_mobilebert_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilebert/tokenization_mobilebert_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v1/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v1/configuration_mobilenet_v1.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v1/configuration_mobilenet_v1.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v1/convert_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v1/convert_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v1/feature_extraction_mobilenet_v1.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v1/feature_extraction_mobilenet_v1.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v1/image_processing_mobilenet_v1.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v1/image_processing_mobilenet_v1.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v1/modeling_mobilenet_v1.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v1/modeling_mobilenet_v1.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v2/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v2/configuration_mobilenet_v2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v2/configuration_mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v2/convert_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v2/convert_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v2/feature_extraction_mobilenet_v2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v2/feature_extraction_mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v2/image_processing_mobilenet_v2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v2/image_processing_mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilenet_v2/modeling_mobilenet_v2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilenet_v2/modeling_mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevit/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevit/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevit/configuration_mobilevit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevit/configuration_mobilevit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevit/convert_mlcvnets_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevit/convert_mlcvnets_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevit/feature_extraction_mobilevit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevit/feature_extraction_mobilevit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevit/image_processing_mobilevit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevit/image_processing_mobilevit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevit/modeling_mobilevit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevit/modeling_mobilevit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevit/modeling_tf_mobilevit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevit/modeling_tf_mobilevit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevitv2/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevitv2/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevitv2/configuration_mobilevitv2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevitv2/configuration_mobilevitv2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevitv2/convert_mlcvnets_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevitv2/convert_mlcvnets_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mobilevitv2/modeling_mobilevitv2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mobilevitv2/modeling_mobilevitv2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mpnet/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mpnet/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mpnet/configuration_mpnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mpnet/configuration_mpnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mpnet/modeling_mpnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mpnet/modeling_mpnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mpnet/modeling_tf_mpnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mpnet/modeling_tf_mpnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mpnet/tokenization_mpnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mpnet/tokenization_mpnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mpnet/tokenization_mpnet_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mpnet/tokenization_mpnet_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mra/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mra/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mra/configuration_mra.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mra/configuration_mra.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mra/convert_mra_pytorch_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mra/convert_mra_pytorch_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mra/modeling_mra.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mra/modeling_mra.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mt5/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mt5/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mt5/configuration_mt5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mt5/configuration_mt5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mt5/modeling_flax_mt5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mt5/modeling_flax_mt5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mt5/modeling_mt5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mt5/modeling_mt5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mt5/modeling_tf_mt5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mt5/modeling_tf_mt5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/musicgen/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/musicgen/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/musicgen/configuration_musicgen.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/musicgen/configuration_musicgen.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/musicgen/convert_musicgen_transformers.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/musicgen/convert_musicgen_transformers.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/musicgen/modeling_musicgen.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/musicgen/modeling_musicgen.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/musicgen/processing_musicgen.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/musicgen/processing_musicgen.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mvp/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mvp/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mvp/configuration_mvp.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mvp/configuration_mvp.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mvp/modeling_mvp.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mvp/modeling_mvp.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mvp/tokenization_mvp.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mvp/tokenization_mvp.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/mvp/tokenization_mvp_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/mvp/tokenization_mvp_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/nat/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/nat/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/nat/configuration_nat.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/nat/configuration_nat.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/nat/modeling_nat.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/nat/modeling_nat.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/nezha/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/nezha/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/nezha/configuration_nezha.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/nezha/configuration_nezha.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/nezha/modeling_nezha.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/nezha/modeling_nezha.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/nllb/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/nllb/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/nllb/tokenization_nllb.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/nllb/tokenization_nllb.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/nllb/tokenization_nllb_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/nllb/tokenization_nllb_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/nllb_moe/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/nllb_moe/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/nllb_moe/configuration_nllb_moe.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/nllb_moe/configuration_nllb_moe.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/nllb_moe/convert_nllb_moe_sharded_original_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/nllb_moe/convert_nllb_moe_sharded_original_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/nllb_moe/modeling_nllb_moe.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/nllb_moe/modeling_nllb_moe.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/nystromformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/nystromformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/nystromformer/configuration_nystromformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/nystromformer/configuration_nystromformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/nystromformer/convert_nystromformer_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/nystromformer/convert_nystromformer_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/nystromformer/modeling_nystromformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/nystromformer/modeling_nystromformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/oneformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/oneformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/oneformer/configuration_oneformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/oneformer/configuration_oneformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/oneformer/convert_to_hf_oneformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/oneformer/convert_to_hf_oneformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/oneformer/image_processing_oneformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/oneformer/image_processing_oneformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/oneformer/modeling_oneformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/oneformer/modeling_oneformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/oneformer/processing_oneformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/oneformer/processing_oneformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/open_llama/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/open_llama/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/open_llama/configuration_open_llama.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/open_llama/configuration_open_llama.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/open_llama/modeling_open_llama.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/open_llama/modeling_open_llama.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/openai/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/openai/configuration_openai.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/openai/configuration_openai.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/openai/convert_openai_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/openai/convert_openai_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/openai/modeling_openai.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/openai/modeling_openai.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/openai/modeling_tf_openai.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/openai/modeling_tf_openai.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/openai/tokenization_openai.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/openai/tokenization_openai.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/openai/tokenization_openai_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/openai/tokenization_openai_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/opt/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/opt/configuration_opt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/opt/configuration_opt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/opt/convert_opt_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/opt/convert_opt_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/opt/modeling_flax_opt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/opt/modeling_flax_opt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/opt/modeling_opt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/opt/modeling_opt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/opt/modeling_tf_opt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/opt/modeling_tf_opt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/owlvit/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/owlvit/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/owlvit/configuration_owlvit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/owlvit/configuration_owlvit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/owlvit/convert_owlvit_original_flax_to_hf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/owlvit/convert_owlvit_original_flax_to_hf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/owlvit/feature_extraction_owlvit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/owlvit/feature_extraction_owlvit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/owlvit/image_processing_owlvit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/owlvit/image_processing_owlvit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/owlvit/modeling_owlvit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/owlvit/modeling_owlvit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/owlvit/processing_owlvit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/owlvit/processing_owlvit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus/configuration_pegasus.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus/configuration_pegasus.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus/convert_pegasus_tf_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus/convert_pegasus_tf_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus/modeling_flax_pegasus.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus/modeling_flax_pegasus.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus/modeling_pegasus.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus/modeling_pegasus.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus/modeling_tf_pegasus.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus/modeling_tf_pegasus.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus/tokenization_pegasus.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus/tokenization_pegasus.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus/tokenization_pegasus_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus/tokenization_pegasus_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus_x/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus_x/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus_x/configuration_pegasus_x.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus_x/configuration_pegasus_x.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/pegasus_x/modeling_pegasus_x.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/pegasus_x/modeling_pegasus_x.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/perceiver/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/perceiver/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/perceiver/configuration_perceiver.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/perceiver/configuration_perceiver.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/perceiver/convert_perceiver_haiku_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/perceiver/convert_perceiver_haiku_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/perceiver/feature_extraction_perceiver.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/perceiver/feature_extraction_perceiver.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/perceiver/image_processing_perceiver.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/perceiver/image_processing_perceiver.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/perceiver/modeling_perceiver.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/perceiver/modeling_perceiver.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/perceiver/tokenization_perceiver.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/perceiver/tokenization_perceiver.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/phobert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/phobert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/phobert/tokenization_phobert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/phobert/tokenization_phobert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/pix2struct/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/pix2struct/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/pix2struct/configuration_pix2struct.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/pix2struct/configuration_pix2struct.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/pix2struct/convert_pix2struct_original_pytorch_to_hf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/pix2struct/convert_pix2struct_original_pytorch_to_hf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/pix2struct/image_processing_pix2struct.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/pix2struct/image_processing_pix2struct.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/pix2struct/modeling_pix2struct.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/pix2struct/modeling_pix2struct.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/pix2struct/processing_pix2struct.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/pix2struct/processing_pix2struct.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/plbart/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/plbart/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/plbart/configuration_plbart.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/plbart/configuration_plbart.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/plbart/convert_plbart_original_checkpoint_to_torch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/plbart/convert_plbart_original_checkpoint_to_torch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/plbart/modeling_plbart.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/plbart/modeling_plbart.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/plbart/tokenization_plbart.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/plbart/tokenization_plbart.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/poolformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/poolformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/poolformer/configuration_poolformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/poolformer/configuration_poolformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/poolformer/convert_poolformer_original_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/poolformer/convert_poolformer_original_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/poolformer/feature_extraction_poolformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/poolformer/feature_extraction_poolformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/poolformer/image_processing_poolformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/poolformer/image_processing_poolformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/poolformer/modeling_poolformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/poolformer/modeling_poolformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/prophetnet/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/prophetnet/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/prophetnet/configuration_prophetnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/prophetnet/configuration_prophetnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/prophetnet/convert_prophetnet_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/prophetnet/convert_prophetnet_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/prophetnet/modeling_prophetnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/prophetnet/modeling_prophetnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/prophetnet/tokenization_prophetnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/prophetnet/tokenization_prophetnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/qdqbert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/qdqbert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/qdqbert/configuration_qdqbert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/qdqbert/configuration_qdqbert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/qdqbert/modeling_qdqbert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/qdqbert/modeling_qdqbert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/rag/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/rag/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/rag/configuration_rag.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/rag/configuration_rag.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/rag/modeling_rag.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/rag/modeling_rag.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/rag/modeling_tf_rag.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/rag/modeling_tf_rag.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/rag/retrieval_rag.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/rag/retrieval_rag.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/rag/tokenization_rag.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/rag/tokenization_rag.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/realm/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/realm/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/realm/configuration_realm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/realm/configuration_realm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/realm/modeling_realm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/realm/modeling_realm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/realm/retrieval_realm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/realm/retrieval_realm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/realm/tokenization_realm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/realm/tokenization_realm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/realm/tokenization_realm_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/realm/tokenization_realm_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/reformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/reformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/reformer/configuration_reformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/reformer/configuration_reformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/reformer/convert_reformer_trax_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/reformer/convert_reformer_trax_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/reformer/modeling_reformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/reformer/modeling_reformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/reformer/tokenization_reformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/reformer/tokenization_reformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/reformer/tokenization_reformer_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/reformer/tokenization_reformer_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/regnet/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/regnet/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/regnet/configuration_regnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/regnet/configuration_regnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/regnet/convert_regnet_seer_10b_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/regnet/convert_regnet_seer_10b_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/regnet/convert_regnet_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/regnet/convert_regnet_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/regnet/modeling_flax_regnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/regnet/modeling_flax_regnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/regnet/modeling_regnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/regnet/modeling_regnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/regnet/modeling_tf_regnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/regnet/modeling_tf_regnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/rembert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/rembert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/rembert/configuration_rembert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/rembert/configuration_rembert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/rembert/convert_rembert_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/rembert/convert_rembert_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/rembert/modeling_rembert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/rembert/modeling_rembert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/rembert/modeling_tf_rembert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/rembert/modeling_tf_rembert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/rembert/tokenization_rembert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/rembert/tokenization_rembert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/rembert/tokenization_rembert_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/rembert/tokenization_rembert_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/resnet/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/resnet/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/resnet/configuration_resnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/resnet/configuration_resnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/resnet/convert_resnet_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/resnet/convert_resnet_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/resnet/modeling_flax_resnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/resnet/modeling_flax_resnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/resnet/modeling_resnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/resnet/modeling_resnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/resnet/modeling_tf_resnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/resnet/modeling_tf_resnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta/configuration_roberta.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta/configuration_roberta.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta/convert_roberta_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta/convert_roberta_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta/modeling_flax_roberta.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta/modeling_flax_roberta.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta/modeling_roberta.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta/modeling_roberta.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta/modeling_tf_roberta.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta/modeling_tf_roberta.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta/tokenization_roberta.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta/tokenization_roberta.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta/tokenization_roberta_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta/tokenization_roberta_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta_prelayernorm/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta_prelayernorm/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta_prelayernorm/configuration_roberta_prelayernorm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta_prelayernorm/configuration_roberta_prelayernorm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta_prelayernorm/convert_roberta_prelayernorm_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta_prelayernorm/convert_roberta_prelayernorm_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta_prelayernorm/modeling_flax_roberta_prelayernorm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta_prelayernorm/modeling_flax_roberta_prelayernorm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta_prelayernorm/modeling_roberta_prelayernorm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta_prelayernorm/modeling_roberta_prelayernorm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roberta_prelayernorm/modeling_tf_roberta_prelayernorm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roberta_prelayernorm/modeling_tf_roberta_prelayernorm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roc_bert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roc_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roc_bert/configuration_roc_bert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roc_bert/configuration_roc_bert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roc_bert/modeling_roc_bert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roc_bert/modeling_roc_bert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roc_bert/tokenization_roc_bert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roc_bert/tokenization_roc_bert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/configuration_roformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/configuration_roformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/convert_roformer_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/convert_roformer_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/modeling_flax_roformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/modeling_flax_roformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/modeling_roformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/modeling_roformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/modeling_tf_roformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/modeling_tf_roformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/tokenization_roformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/tokenization_roformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/tokenization_roformer_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/tokenization_roformer_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/roformer/tokenization_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/roformer/tokenization_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/rwkv/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/rwkv/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/rwkv/configuration_rwkv.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/rwkv/configuration_rwkv.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/rwkv/convert_rwkv_checkpoint_to_hf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/rwkv/convert_rwkv_checkpoint_to_hf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/rwkv/modeling_rwkv.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/rwkv/modeling_rwkv.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/sam/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/sam/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/sam/configuration_sam.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/sam/configuration_sam.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/sam/convert_sam_original_to_hf_format.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/sam/convert_sam_original_to_hf_format.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/sam/image_processing_sam.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/sam/image_processing_sam.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/sam/modeling_sam.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/sam/modeling_sam.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/sam/modeling_tf_sam.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/sam/modeling_tf_sam.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/sam/processing_sam.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/sam/processing_sam.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/segformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/segformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/segformer/configuration_segformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/segformer/configuration_segformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/segformer/convert_segformer_original_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/segformer/convert_segformer_original_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/segformer/feature_extraction_segformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/segformer/feature_extraction_segformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/segformer/image_processing_segformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/segformer/image_processing_segformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/segformer/modeling_segformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/segformer/modeling_segformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/segformer/modeling_tf_segformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/segformer/modeling_tf_segformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/sew/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/sew/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/sew/configuration_sew.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/sew/configuration_sew.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/sew/convert_sew_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/sew/convert_sew_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/sew/modeling_sew.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/sew/modeling_sew.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/sew_d/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/sew_d/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/sew_d/configuration_sew_d.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/sew_d/configuration_sew_d.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/sew_d/convert_sew_d_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/sew_d/convert_sew_d_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/sew_d/modeling_sew_d.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/sew_d/modeling_sew_d.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_encoder_decoder/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_encoder_decoder/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_encoder_decoder/configuration_speech_encoder_decoder.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_encoder_decoder/configuration_speech_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_encoder_decoder/convert_mbart_wav2vec2_seq2seq_original_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_encoder_decoder/convert_mbart_wav2vec2_seq2seq_original_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_encoder_decoder/convert_speech_to_text_wav2vec2_seq2seq_original_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_encoder_decoder/convert_speech_to_text_wav2vec2_seq2seq_original_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_encoder_decoder/modeling_flax_speech_encoder_decoder.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_encoder_decoder/modeling_flax_speech_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_encoder_decoder/modeling_speech_encoder_decoder.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_encoder_decoder/modeling_speech_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text/configuration_speech_to_text.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text/configuration_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text/convert_s2t_fairseq_to_tfms.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text/convert_s2t_fairseq_to_tfms.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text/feature_extraction_speech_to_text.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text/feature_extraction_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text/modeling_speech_to_text.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text/modeling_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text/modeling_tf_speech_to_text.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text/modeling_tf_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text/processing_speech_to_text.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text/processing_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text/tokenization_speech_to_text.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text/tokenization_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text_2/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text_2/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text_2/configuration_speech_to_text_2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text_2/configuration_speech_to_text_2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text_2/modeling_speech_to_text_2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text_2/modeling_speech_to_text_2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text_2/processing_speech_to_text_2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text_2/processing_speech_to_text_2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speech_to_text_2/tokenization_speech_to_text_2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speech_to_text_2/tokenization_speech_to_text_2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speecht5/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speecht5/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speecht5/configuration_speecht5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speecht5/configuration_speecht5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speecht5/convert_hifigan.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speecht5/convert_hifigan.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speecht5/convert_speecht5_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speecht5/convert_speecht5_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speecht5/feature_extraction_speecht5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speecht5/feature_extraction_speecht5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speecht5/modeling_speecht5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speecht5/modeling_speecht5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speecht5/processing_speecht5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speecht5/processing_speecht5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/speecht5/tokenization_speecht5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/speecht5/tokenization_speecht5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/splinter/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/splinter/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/splinter/configuration_splinter.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/splinter/configuration_splinter.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/splinter/modeling_splinter.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/splinter/modeling_splinter.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/splinter/tokenization_splinter.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/splinter/tokenization_splinter.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/splinter/tokenization_splinter_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/splinter/tokenization_splinter_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/squeezebert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/squeezebert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/squeezebert/configuration_squeezebert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/squeezebert/configuration_squeezebert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/squeezebert/modeling_squeezebert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/squeezebert/modeling_squeezebert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/squeezebert/tokenization_squeezebert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/squeezebert/tokenization_squeezebert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/squeezebert/tokenization_squeezebert_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/squeezebert/tokenization_squeezebert_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swiftformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swiftformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swiftformer/configuration_swiftformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swiftformer/configuration_swiftformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swiftformer/convert_swiftformer_original_to_hf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swiftformer/convert_swiftformer_original_to_hf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swiftformer/modeling_swiftformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swiftformer/modeling_swiftformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swin/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swin/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swin/configuration_swin.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swin/configuration_swin.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swin/convert_swin_simmim_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swin/convert_swin_simmim_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swin/convert_swin_timm_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swin/convert_swin_timm_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swin/modeling_swin.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swin/modeling_swin.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swin/modeling_tf_swin.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swin/modeling_tf_swin.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swin2sr/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swin2sr/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swin2sr/configuration_swin2sr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swin2sr/configuration_swin2sr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swin2sr/convert_swin2sr_original_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swin2sr/convert_swin2sr_original_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swin2sr/image_processing_swin2sr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swin2sr/image_processing_swin2sr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swin2sr/modeling_swin2sr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swin2sr/modeling_swin2sr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swinv2/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swinv2/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swinv2/configuration_swinv2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swinv2/configuration_swinv2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swinv2/convert_swinv2_timm_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swinv2/convert_swinv2_timm_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/swinv2/modeling_swinv2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/swinv2/modeling_swinv2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/switch_transformers/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/switch_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/switch_transformers/configuration_switch_transformers.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/switch_transformers/configuration_switch_transformers.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/switch_transformers/convert_big_switch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/switch_transformers/convert_big_switch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/switch_transformers/convert_switch_transformers_original_flax_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/switch_transformers/convert_switch_transformers_original_flax_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/switch_transformers/modeling_switch_transformers.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/switch_transformers/modeling_switch_transformers.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/configuration_t5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/configuration_t5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/convert_t5_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/convert_t5_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/convert_t5x_checkpoint_to_flax.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/convert_t5x_checkpoint_to_flax.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/convert_t5x_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/convert_t5x_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/modeling_flax_t5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/modeling_flax_t5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/modeling_t5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/modeling_t5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/modeling_tf_t5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/modeling_tf_t5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/tokenization_t5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/tokenization_t5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/t5/tokenization_t5_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/t5/tokenization_t5_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/table_transformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/table_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/table_transformer/configuration_table_transformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/table_transformer/configuration_table_transformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/table_transformer/convert_table_transformer_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/table_transformer/convert_table_transformer_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/table_transformer/modeling_table_transformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/table_transformer/modeling_table_transformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/tapas/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/tapas/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/tapas/configuration_tapas.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/tapas/configuration_tapas.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/tapas/convert_tapas_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/tapas/convert_tapas_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/tapas/modeling_tapas.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/tapas/modeling_tapas.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/tapas/modeling_tf_tapas.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/tapas/modeling_tf_tapas.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/tapas/tokenization_tapas.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/tapas/tokenization_tapas.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/time_series_transformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/time_series_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/time_series_transformer/configuration_time_series_transformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/time_series_transformer/configuration_time_series_transformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/time_series_transformer/modeling_time_series_transformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/time_series_transformer/modeling_time_series_transformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/timesformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/timesformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/timesformer/configuration_timesformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/timesformer/configuration_timesformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/timesformer/convert_timesformer_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/timesformer/convert_timesformer_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/timesformer/modeling_timesformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/timesformer/modeling_timesformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/timm_backbone/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/timm_backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/timm_backbone/configuration_timm_backbone.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/timm_backbone/configuration_timm_backbone.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/timm_backbone/modeling_timm_backbone.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/timm_backbone/modeling_timm_backbone.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/transfo_xl/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/transfo_xl/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/transfo_xl/configuration_transfo_xl.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/transfo_xl/configuration_transfo_xl.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/transfo_xl/convert_transfo_xl_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/transfo_xl/convert_transfo_xl_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/transfo_xl/modeling_tf_transfo_xl.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/transfo_xl/modeling_tf_transfo_xl.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/transfo_xl/modeling_tf_transfo_xl_utilities.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/transfo_xl/modeling_tf_transfo_xl_utilities.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/transfo_xl/modeling_transfo_xl.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/transfo_xl/modeling_transfo_xl.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/transfo_xl/modeling_transfo_xl_utilities.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/transfo_xl/modeling_transfo_xl_utilities.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/transfo_xl/tokenization_transfo_xl.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/transfo_xl/tokenization_transfo_xl.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/trocr/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/trocr/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/trocr/configuration_trocr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/trocr/configuration_trocr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/trocr/convert_trocr_unilm_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/trocr/convert_trocr_unilm_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/trocr/modeling_trocr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/trocr/modeling_trocr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/trocr/processing_trocr.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/trocr/processing_trocr.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/tvlt/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/tvlt/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/tvlt/configuration_tvlt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/tvlt/configuration_tvlt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/tvlt/feature_extraction_tvlt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/tvlt/feature_extraction_tvlt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/tvlt/image_processing_tvlt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/tvlt/image_processing_tvlt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/tvlt/modeling_tvlt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/tvlt/modeling_tvlt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/tvlt/processing_tvlt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/tvlt/processing_tvlt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/umt5/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/umt5/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/umt5/configuration_umt5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/umt5/configuration_umt5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/umt5/convert_umt5_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/umt5/convert_umt5_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/umt5/modeling_umt5.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/umt5/modeling_umt5.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech/configuration_unispeech.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech/configuration_unispeech.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech/convert_unispeech_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech/convert_unispeech_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech/modeling_unispeech.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech/modeling_unispeech.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech_sat/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech_sat/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech_sat/configuration_unispeech_sat.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech_sat/configuration_unispeech_sat.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech_sat/convert_unispeech_original_s3prl_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech_sat/convert_unispeech_original_s3prl_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech_sat/convert_unispeech_sat_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech_sat/convert_unispeech_sat_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/unispeech_sat/modeling_unispeech_sat.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/unispeech_sat/modeling_unispeech_sat.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/upernet/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/upernet/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/upernet/configuration_upernet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/upernet/configuration_upernet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/upernet/convert_convnext_upernet_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/upernet/convert_convnext_upernet_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/upernet/convert_swin_upernet_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/upernet/convert_swin_upernet_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/upernet/modeling_upernet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/upernet/modeling_upernet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/videomae/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/videomae/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/videomae/configuration_videomae.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/videomae/configuration_videomae.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/videomae/convert_videomae_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/videomae/convert_videomae_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/videomae/feature_extraction_videomae.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/videomae/feature_extraction_videomae.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/videomae/image_processing_videomae.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/videomae/image_processing_videomae.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/videomae/modeling_videomae.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/videomae/modeling_videomae.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vilt/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vilt/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vilt/configuration_vilt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vilt/configuration_vilt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vilt/convert_vilt_original_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vilt/convert_vilt_original_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vilt/feature_extraction_vilt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vilt/feature_extraction_vilt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vilt/image_processing_vilt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vilt/image_processing_vilt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vilt/modeling_vilt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vilt/modeling_vilt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vilt/processing_vilt.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vilt/processing_vilt.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_encoder_decoder/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_encoder_decoder/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_encoder_decoder/configuration_vision_encoder_decoder.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_encoder_decoder/configuration_vision_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_encoder_decoder/modeling_flax_vision_encoder_decoder.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_encoder_decoder/modeling_flax_vision_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_encoder_decoder/modeling_tf_vision_encoder_decoder.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_encoder_decoder/modeling_tf_vision_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_encoder_decoder/modeling_vision_encoder_decoder.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_encoder_decoder/modeling_vision_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_text_dual_encoder/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_text_dual_encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_text_dual_encoder/configuration_vision_text_dual_encoder.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_text_dual_encoder/configuration_vision_text_dual_encoder.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_text_dual_encoder/modeling_flax_vision_text_dual_encoder.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_text_dual_encoder/modeling_flax_vision_text_dual_encoder.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_text_dual_encoder/modeling_tf_vision_text_dual_encoder.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_text_dual_encoder/modeling_tf_vision_text_dual_encoder.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_text_dual_encoder/modeling_vision_text_dual_encoder.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_text_dual_encoder/modeling_vision_text_dual_encoder.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vision_text_dual_encoder/processing_vision_text_dual_encoder.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vision_text_dual_encoder/processing_vision_text_dual_encoder.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/visual_bert/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/visual_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/visual_bert/configuration_visual_bert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/visual_bert/configuration_visual_bert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/visual_bert/convert_visual_bert_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/visual_bert/convert_visual_bert_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/visual_bert/modeling_visual_bert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/visual_bert/modeling_visual_bert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/configuration_vit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/configuration_vit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/convert_dino_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/convert_dino_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/convert_vit_timm_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/convert_vit_timm_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/feature_extraction_vit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/feature_extraction_vit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/image_processing_vit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/image_processing_vit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/modeling_flax_vit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/modeling_flax_vit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/modeling_tf_vit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/modeling_tf_vit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit/modeling_vit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit/modeling_vit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_hybrid/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_hybrid/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_hybrid/configuration_vit_hybrid.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_hybrid/configuration_vit_hybrid.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_hybrid/convert_vit_hybrid_timm_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_hybrid/convert_vit_hybrid_timm_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_hybrid/image_processing_vit_hybrid.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_hybrid/image_processing_vit_hybrid.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_hybrid/modeling_vit_hybrid.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_hybrid/modeling_vit_hybrid.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_mae/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_mae/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_mae/configuration_vit_mae.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_mae/configuration_vit_mae.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_mae/convert_vit_mae_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_mae/convert_vit_mae_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_mae/modeling_tf_vit_mae.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_mae/modeling_tf_vit_mae.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_mae/modeling_vit_mae.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_mae/modeling_vit_mae.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_msn/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_msn/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_msn/configuration_vit_msn.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_msn/configuration_vit_msn.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_msn/convert_msn_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_msn/convert_msn_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vit_msn/modeling_vit_msn.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vit_msn/modeling_vit_msn.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vivit/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vivit/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vivit/configuration_vivit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vivit/configuration_vivit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vivit/convert_vivit_flax_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vivit/convert_vivit_flax_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vivit/image_processing_vivit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vivit/image_processing_vivit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/vivit/modeling_vivit.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/vivit/modeling_vivit.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/configuration_wav2vec2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/configuration_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/convert_wav2vec2_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/convert_wav2vec2_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/convert_wav2vec2_original_s3prl_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/convert_wav2vec2_original_s3prl_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/feature_extraction_wav2vec2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/feature_extraction_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/modeling_flax_wav2vec2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/modeling_flax_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/modeling_tf_wav2vec2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/modeling_tf_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/modeling_wav2vec2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/modeling_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/processing_wav2vec2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/processing_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2/tokenization_wav2vec2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2/tokenization_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_conformer/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_conformer/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_conformer/configuration_wav2vec2_conformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_conformer/configuration_wav2vec2_conformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_conformer/convert_wav2vec2_conformer_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_conformer/convert_wav2vec2_conformer_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_conformer/modeling_wav2vec2_conformer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_conformer/modeling_wav2vec2_conformer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_phoneme/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_phoneme/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_phoneme/tokenization_wav2vec2_phoneme.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_phoneme/tokenization_wav2vec2_phoneme.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_with_lm/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_with_lm/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wav2vec2_with_lm/processing_wav2vec2_with_lm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wav2vec2_with_lm/processing_wav2vec2_with_lm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wavlm/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wavlm/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wavlm/configuration_wavlm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wavlm/configuration_wavlm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wavlm/convert_wavlm_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wavlm/convert_wavlm_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wavlm/convert_wavlm_original_s3prl_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wavlm/convert_wavlm_original_s3prl_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/wavlm/modeling_wavlm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/wavlm/modeling_wavlm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/configuration_whisper.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/configuration_whisper.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/convert_openai_to_hf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/convert_openai_to_hf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/english_normalizer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/english_normalizer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/feature_extraction_whisper.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/feature_extraction_whisper.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/modeling_flax_whisper.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/modeling_flax_whisper.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/modeling_tf_whisper.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/modeling_tf_whisper.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/modeling_whisper.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/modeling_whisper.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/processing_whisper.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/processing_whisper.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/tokenization_whisper.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/tokenization_whisper.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/whisper/tokenization_whisper_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/whisper/tokenization_whisper_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/x_clip/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/x_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/x_clip/configuration_x_clip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/x_clip/configuration_x_clip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/x_clip/convert_x_clip_original_pytorch_to_hf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/x_clip/convert_x_clip_original_pytorch_to_hf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/x_clip/modeling_x_clip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/x_clip/modeling_x_clip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/x_clip/processing_x_clip.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/x_clip/processing_x_clip.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xglm/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xglm/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xglm/configuration_xglm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xglm/configuration_xglm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xglm/convert_xglm_original_ckpt_to_trfms.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xglm/convert_xglm_original_ckpt_to_trfms.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xglm/modeling_flax_xglm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xglm/modeling_flax_xglm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xglm/modeling_tf_xglm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xglm/modeling_tf_xglm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xglm/modeling_xglm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xglm/modeling_xglm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xglm/tokenization_xglm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xglm/tokenization_xglm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xglm/tokenization_xglm_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xglm/tokenization_xglm_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm/configuration_xlm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm/configuration_xlm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm/convert_xlm_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm/convert_xlm_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm/modeling_tf_xlm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm/modeling_tf_xlm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm/modeling_xlm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm/modeling_xlm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm/tokenization_xlm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm/tokenization_xlm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_prophetnet/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_prophetnet/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_prophetnet/configuration_xlm_prophetnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_prophetnet/configuration_xlm_prophetnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_prophetnet/modeling_xlm_prophetnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_prophetnet/modeling_xlm_prophetnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_prophetnet/tokenization_xlm_prophetnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_prophetnet/tokenization_xlm_prophetnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta/configuration_xlm_roberta.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta/configuration_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta/modeling_flax_xlm_roberta.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta/modeling_flax_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta/modeling_tf_xlm_roberta.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta/modeling_tf_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta/modeling_xlm_roberta.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta/modeling_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta/tokenization_xlm_roberta.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta/tokenization_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta/tokenization_xlm_roberta_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta/tokenization_xlm_roberta_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta_xl/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta_xl/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta_xl/configuration_xlm_roberta_xl.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta_xl/configuration_xlm_roberta_xl.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta_xl/convert_xlm_roberta_xl_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta_xl/convert_xlm_roberta_xl_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlm_roberta_xl/modeling_xlm_roberta_xl.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlm_roberta_xl/modeling_xlm_roberta_xl.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlnet/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlnet/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlnet/configuration_xlnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlnet/configuration_xlnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlnet/convert_xlnet_original_tf_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlnet/convert_xlnet_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlnet/modeling_tf_xlnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlnet/modeling_tf_xlnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlnet/modeling_xlnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlnet/modeling_xlnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlnet/tokenization_xlnet.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlnet/tokenization_xlnet.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xlnet/tokenization_xlnet_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xlnet/tokenization_xlnet_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xmod/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xmod/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xmod/configuration_xmod.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xmod/configuration_xmod.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xmod/convert_xmod_original_pytorch_checkpoint_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xmod/convert_xmod_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/xmod/modeling_xmod.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/xmod/modeling_xmod.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/yolos/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/yolos/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/yolos/configuration_yolos.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/yolos/configuration_yolos.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/yolos/convert_yolos_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/yolos/convert_yolos_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/yolos/feature_extraction_yolos.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/yolos/feature_extraction_yolos.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/yolos/image_processing_yolos.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/yolos/image_processing_yolos.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/yolos/modeling_yolos.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/yolos/modeling_yolos.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/yoso/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/yoso/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/yoso/configuration_yoso.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/yoso/configuration_yoso.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/yoso/convert_yoso_pytorch_to_pytorch.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/yoso/convert_yoso_pytorch_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/models/yoso/modeling_yoso.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/models/yoso/modeling_yoso.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/onnx/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/onnx/__main__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/onnx/__main__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/onnx/config.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/onnx/config.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/onnx/convert.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/onnx/convert.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/onnx/features.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/onnx/features.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/onnx/utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/onnx/utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/optimization.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/optimization.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/optimization_tf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/optimization_tf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/audio_classification.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/audio_classification.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/audio_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/audio_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/automatic_speech_recognition.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/automatic_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/base.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/conversational.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/conversational.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/depth_estimation.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/depth_estimation.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/document_question_answering.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/document_question_answering.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/feature_extraction.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/fill_mask.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/fill_mask.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/image_classification.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/image_classification.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/image_segmentation.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/image_segmentation.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/image_to_text.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/image_to_text.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/mask_generation.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/mask_generation.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/object_detection.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/object_detection.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/pt_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/pt_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/question_answering.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/question_answering.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/table_question_answering.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/table_question_answering.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/text2text_generation.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/text2text_generation.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/text_classification.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/text_classification.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/text_generation.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/text_generation.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/token_classification.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/token_classification.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/video_classification.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/video_classification.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/visual_question_answering.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/visual_question_answering.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/zero_shot_audio_classification.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/zero_shot_audio_classification.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/zero_shot_classification.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/zero_shot_classification.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/zero_shot_image_classification.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/zero_shot_image_classification.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pipelines/zero_shot_object_detection.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pipelines/zero_shot_object_detection.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/processing_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/processing_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/pytorch_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/sagemaker/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/sagemaker/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/sagemaker/trainer_sm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/sagemaker/trainer_sm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/sagemaker/training_args_sm.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/sagemaker/training_args_sm.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/testing_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/testing_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tf_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tf_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/time_series_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/time_series_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tokenization_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tokenization_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tokenization_utils_base.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tokenization_utils_base.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tokenization_utils_fast.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tokenization_utils_fast.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tools/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tools/agent_types.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tools/agent_types.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tools/agents.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tools/agents.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tools/base.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tools/base.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tools/document_question_answering.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tools/document_question_answering.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tools/evaluate_agent.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tools/evaluate_agent.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tools/image_captioning.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tools/image_captioning.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tools/image_question_answering.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tools/image_question_answering.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tools/image_segmentation.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tools/image_segmentation.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tools/prompts.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tools/python_interpreter.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tools/python_interpreter.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tools/speech_to_text.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tools/speech_to_text.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tools/text_classification.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tools/text_classification.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tools/text_question_answering.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tools/text_question_answering.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tools/text_summarization.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tools/text_summarization.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tools/text_to_speech.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tools/text_to_speech.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/tools/translation.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/tools/translation.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/trainer.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/trainer.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/trainer_callback.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/trainer_callback.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/trainer_pt_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/trainer_pt_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/trainer_seq2seq.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/trainer_tf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/trainer_tf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/trainer_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/training_args.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/training_args.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/training_args_seq2seq.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/training_args_seq2seq.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/training_args_tf.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/training_args_tf.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/__init__.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/backbone_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/backbone_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/bitsandbytes.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/bitsandbytes.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/doc.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/doc.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/dummy_flax_objects.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/dummy_flax_objects.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/dummy_pt_objects.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/dummy_pt_objects.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/dummy_sentencepiece_objects.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/dummy_sentencepiece_objects.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/dummy_tf_objects.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/dummy_tf_objects.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/dummy_tokenizers_objects.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/dummy_tokenizers_objects.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/dummy_vision_objects.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/dummy_vision_objects.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/fx.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/fx.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/generic.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/generic.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/hp_naming.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/hp_naming.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/hub.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/hub.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/import_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/logging.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/logging.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/model_parallel_utils.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/model_parallel_utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/notebook.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/quantization_config.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/quantization_config.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/sentencepiece_model_pb2.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/sentencepiece_model_pb2.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/sentencepiece_model_pb2_new.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/sentencepiece_model_pb2_new.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/hf/transformers/utils/versions.py` & `llm-toys-0.1.1/llm_toys/hf/transformers/utils/versions.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/prompts.py` & `llm-toys-0.1.1/llm_toys/prompts.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/tasks/all_tasks.py` & `llm-toys-0.1.1/llm_toys/tasks/all_tasks.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/tasks/paraphrase.py` & `llm-toys-0.1.1/llm_toys/tasks/paraphrase.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/tasks/predict.py` & `llm-toys-0.1.1/llm_toys/tasks/predict.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/tasks/summary_topic.py` & `llm-toys-0.1.1/llm_toys/tasks/summary_topic.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/train.py` & `llm-toys-0.1.1/llm_toys/train.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys/utils.py` & `llm-toys-0.1.1/llm_toys/utils.py`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys.egg-info/PKG-INFO` & `llm-toys-0.1.1/llm_toys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-toys
-Version: 0.1.0
+Version: 0.1.1
 Summary: Small(7B and below), production-ready finetuned LLMs for a diverse set of useful tasks.
 Home-page: https://github.com/kuutsav/llm-toys
 Author: Kumar Utsav
 Author-email: krum.utsav@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
```

### Comparing `llm-toys-0.1.0/llm_toys.egg-info/SOURCES.txt` & `llm-toys-0.1.1/llm_toys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm-toys-0.1.0/llm_toys.egg-info/requires.txt` & `llm-toys-0.1.1/llm_toys.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 grpcio==1.56.0
 h11==0.14.0
 huggingface-hub==0.16.4
 idna==3.4
 Jinja2==3.1.2
 joblib==1.3.1
 lit==16.0.6
-llm-toys==0.0.7
 Mako==1.2.4
 MarkupSafe==2.1.3
 monotonic==1.6
 mpmath==1.3.0
 networkx==3.1
 nltk==3.8.1
 numpy==1.25.1
```

### Comparing `llm-toys-0.1.0/setup.py` & `llm-toys-0.1.1/setup.py`

 * *Files identical despite different names*

