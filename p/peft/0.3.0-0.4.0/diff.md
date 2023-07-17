# Comparing `tmp/peft-0.3.0.tar.gz` & `tmp/peft-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peft-0.3.0.tar", last modified: Wed May  3 19:45:13 2023, max compression
+gzip compressed data, was "peft-0.4.0.tar", last modified: Mon Jul 17 10:04:03 2023, max compression
```

## Comparing `peft-0.3.0.tar` & `peft-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,46 @@
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-05-03 19:45:13.266616 peft-0.3.0/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    11357 2022-11-25 03:51:31.000000 peft-0.3.0/LICENSE
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    20550 2023-05-03 19:45:13.266499 peft-0.3.0/PKG-INFO
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    19627 2023-05-03 19:37:00.000000 peft-0.3.0/README.md
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      665 2023-03-07 08:32:29.000000 peft-0.3.0/pyproject.toml
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)       38 2023-05-03 19:45:13.266649 peft-0.3.0/setup.cfg
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     3134 2023-05-03 19:42:54.000000 peft-0.3.0/setup.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-05-03 19:45:13.262706 peft-0.3.0/src/
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-05-03 19:45:13.264205 peft-0.3.0/src/peft/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1757 2023-05-03 19:42:47.000000 peft-0.3.0/src/peft/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      720 2023-04-17 11:31:49.000000 peft-0.3.0/src/peft/import_utils.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     4427 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/mapping.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    52633 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/peft_model.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-05-03 19:45:13.265878 peft-0.3.0/src/peft/tuners/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1180 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/tuners/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    29964 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/tuners/adalora.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    15972 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/tuners/adaption_prompt.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    31010 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/tuners/lora.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     6755 2023-04-17 11:31:49.000000 peft-0.3.0/src/peft/tuners/p_tuning.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     3785 2023-04-17 11:31:49.000000 peft-0.3.0/src/peft/tuners/prefix_tuning.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     4935 2023-04-17 11:31:49.000000 peft-0.3.0/src/peft/tuners/prompt_tuning.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-05-03 19:45:13.266325 peft-0.3.0/src/peft/utils/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1398 2023-04-17 11:33:24.000000 peft-0.3.0/src/peft/utils/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     6823 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/utils/config.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     8356 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/utils/other.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     5829 2023-05-03 19:37:00.000000 peft-0.3.0/src/peft/utils/save_and_load.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-05-03 19:45:13.264772 peft-0.3.0/src/peft.egg-info/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    20550 2023-05-03 19:45:13.000000 peft-0.3.0/src/peft.egg-info/PKG-INFO
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      605 2023-05-03 19:45:13.000000 peft-0.3.0/src/peft.egg-info/SOURCES.txt
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)        1 2023-05-03 19:45:13.000000 peft-0.3.0/src/peft.egg-info/dependency_links.txt
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      289 2023-05-03 19:45:13.000000 peft-0.3.0/src/peft.egg-info/requires.txt
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)        5 2023-05-03 19:45:13.000000 peft-0.3.0/src/peft.egg-info/top_level.txt
+drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-07-17 10:04:03.364333 peft-0.4.0/
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    11357 2022-11-25 03:51:31.000000 peft-0.4.0/LICENSE
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    20578 2023-07-17 10:04:03.364100 peft-0.4.0/PKG-INFO
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    19655 2023-07-17 09:47:00.000000 peft-0.4.0/README.md
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      872 2023-07-17 10:00:38.000000 peft-0.4.0/pyproject.toml
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)       38 2023-07-17 10:04:03.364400 peft-0.4.0/setup.cfg
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     3202 2023-07-17 10:02:29.000000 peft-0.4.0/setup.py
+drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-07-17 10:04:03.356177 peft-0.4.0/src/
+drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-07-17 10:04:03.358170 peft-0.4.0/src/peft/
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     2158 2023-07-17 10:02:18.000000 peft-0.4.0/src/peft/__init__.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     5535 2023-07-17 09:47:00.000000 peft-0.4.0/src/peft/auto.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      877 2023-06-22 10:46:29.000000 peft-0.4.0/src/peft/import_utils.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     3286 2023-07-17 09:47:00.000000 peft-0.4.0/src/peft/mapping.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    74771 2023-07-17 10:00:38.000000 peft-0.4.0/src/peft/peft_model.py
+drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-07-17 10:04:03.361285 peft-0.4.0/src/peft/tuners/
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1217 2023-07-17 09:47:00.000000 peft-0.4.0/src/peft/tuners/__init__.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    33418 2023-07-10 07:46:53.000000 peft-0.4.0/src/peft/tuners/adalora.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    16325 2023-07-10 07:46:53.000000 peft-0.4.0/src/peft/tuners/adaption_prompt.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    22812 2023-07-17 09:47:00.000000 peft-0.4.0/src/peft/tuners/ia3.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    48579 2023-07-17 09:47:00.000000 peft-0.4.0/src/peft/tuners/lora.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     6755 2023-04-17 11:31:49.000000 peft-0.4.0/src/peft/tuners/p_tuning.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     3785 2023-04-17 11:31:49.000000 peft-0.4.0/src/peft/tuners/prefix_tuning.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     4935 2023-04-17 11:31:49.000000 peft-0.4.0/src/peft/tuners/prompt_tuning.py
+drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-07-17 10:04:03.362222 peft-0.4.0/src/peft/utils/
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1734 2023-07-17 09:47:00.000000 peft-0.4.0/src/peft/utils/__init__.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     8830 2023-07-17 10:00:38.000000 peft-0.4.0/src/peft/utils/config.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1118 2023-06-16 09:17:11.000000 peft-0.4.0/src/peft/utils/hub_utils.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    13087 2023-07-17 09:47:00.000000 peft-0.4.0/src/peft/utils/other.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     6098 2023-07-17 09:47:00.000000 peft-0.4.0/src/peft/utils/save_and_load.py
+drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-07-17 10:04:03.359092 peft-0.4.0/src/peft.egg-info/
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    20578 2023-07-17 10:04:03.000000 peft-0.4.0/src/peft.egg-info/PKG-INFO
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      959 2023-07-17 10:04:03.000000 peft-0.4.0/src/peft.egg-info/SOURCES.txt
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)        1 2023-07-17 10:04:03.000000 peft-0.4.0/src/peft.egg-info/dependency_links.txt
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      367 2023-07-17 10:04:03.000000 peft-0.4.0/src/peft.egg-info/requires.txt
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)        5 2023-07-17 10:04:03.000000 peft-0.4.0/src/peft.egg-info/top_level.txt
+drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2023-07-17 10:04:03.363801 peft-0.4.0/tests/
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    18208 2023-07-17 09:47:00.000000 peft-0.4.0/tests/test_adaption_prompt.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     9771 2023-07-10 07:46:53.000000 peft-0.4.0/tests/test_common_gpu.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     5924 2023-07-17 09:47:00.000000 peft-0.4.0/tests/test_config.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     8425 2023-07-17 09:47:00.000000 peft-0.4.0/tests/test_decoder_models.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     8062 2023-07-17 09:47:00.000000 peft-0.4.0/tests/test_encoder_decoder_models.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     7252 2023-07-17 09:47:00.000000 peft-0.4.0/tests/test_feature_extraction_models.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    19874 2023-07-10 07:46:53.000000 peft-0.4.0/tests/test_gpu_examples.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     6079 2023-07-17 09:47:00.000000 peft-0.4.0/tests/test_stablediffusion.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    33027 2023-07-17 09:47:00.000000 peft-0.4.0/tests/testing_common.py
+-rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     2307 2023-07-10 07:46:53.000000 peft-0.4.0/tests/testing_utils.py
```

### Comparing `peft-0.3.0/LICENSE` & `peft-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peft-0.3.0/PKG-INFO` & `peft-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: peft
-Version: 0.3.0
+Version: 0.4.0
 Summary: Parameter-Efficient Fine-Tuning (PEFT)
 Home-page: https://github.com/huggingface/peft
 Author: The HuggingFace team
 Author-email: sourab@huggingface.co
 License: Apache
 Keywords: deep learning
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: quality
 Provides-Extra: docs_specific
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
@@ -53,14 +53,15 @@
 Supported methods:
 
 1. LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685)
 2. Prefix Tuning: [Prefix-Tuning: Optimizing Continuous Prompts for Generation](https://aclanthology.org/2021.acl-long.353/), [P-Tuning v2: Prompt Tuning Can Be Comparable to Fine-tuning Universally Across Scales and Tasks](https://arxiv.org/pdf/2110.07602.pdf)
 3. P-Tuning: [GPT Understands, Too](https://arxiv.org/abs/2103.10385)
 4. Prompt Tuning: [The Power of Scale for Parameter-Efficient Prompt Tuning](https://arxiv.org/abs/2104.08691)
 5. AdaLoRA: [Adaptive Budget Allocation for Parameter-Efficient Fine-Tuning](https://arxiv.org/abs/2303.10512)  
+6. $(IA)^3$ : [Infused Adapter by Inhibiting and Amplifying Inner Activations](https://arxiv.org/abs/2205.05638)
 
 ## Getting started
 
 ```python
 from transformers import AutoModelForSeq2SeqLM
 from peft import get_peft_config, get_peft_model, LoraConfig, TaskType
 model_name_or_path = "bigscience/mt0-large"
@@ -162,15 +163,15 @@
 - Here is an example in [trl](https://github.com/lvwerra/trl) library using PEFT+INT8 for tuning policy model: [gpt2-sentiment_peft.py](https://github.com/lvwerra/trl/blob/main/examples/sentiment/scripts/gpt2-sentiment_peft.py) and corresponding [Blog](https://huggingface.co/blog/trl-peft)
 - Example using PEFT for Instrction finetuning, reward model and policy : [stack_llama](https://github.com/lvwerra/trl/tree/main/examples/stack_llama/scripts) and corresponding [Blog](https://huggingface.co/blog/stackllama) 
 
 ### INT8 training of large models in Colab using PEFT LoRA and bits_and_bytes
 
 - Here is now a demo on how to fine tune [OPT-6.7b](https://huggingface.co/facebook/opt-6.7b) (14GB in fp16) in a Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jCkpikz0J2o20FBQmYmAGdiKmJGOMo-o?usp=sharing)
 
-- Here is now a demo on how to fine tune [whishper-large](openai/whisper-large-v2) (1.5B params) (14GB in fp16) in a Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1DOkD_5OUjFa0r5Ik3SgywJLJtEo2qLxO?usp=sharing) and [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vhF8yueFqha3Y3CpTHN6q9EVcII9EYzs?usp=sharing)
+- Here is now a demo on how to fine tune [whisper-large](https://huggingface.co/openai/whisper-large-v2) (1.5B params) (14GB in fp16) in a Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1DOkD_5OUjFa0r5Ik3SgywJLJtEo2qLxO?usp=sharing) and [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vhF8yueFqha3Y3CpTHN6q9EVcII9EYzs?usp=sharing)
 
 ### Save compute and storage even for medium and small models
 
 Save storage by avoiding full finetuning of models on each of the downstream tasks/datasets,
 With PEFT methods, users only need to store tiny checkpoints in the order of `MBs` all the while retaining 
 performance comparable to full finetuning.
 
@@ -246,87 +247,87 @@
 ### Example of PEFT model inference using 🤗 Accelerate's Big Model Inferencing capabilities
 An example is provided in `~examples/causal_language_modeling/peft_lora_clm_accelerate_big_model_inference.ipynb`. 
 
 
 ## Models support matrix
 
 ### Causal Language Modeling
-| Model        | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  |
-|--------------| ---- | ---- | ---- | ----  |
-| GPT-2        | ✅  | ✅  | ✅  | ✅  |
-| Bloom        | ✅  | ✅  | ✅  | ✅  |
-| OPT          | ✅  | ✅  | ✅  | ✅  |
-| GPT-Neo      | ✅  | ✅  | ✅  | ✅  |
-| GPT-J        | ✅  | ✅  | ✅  | ✅  |
-| GPT-NeoX-20B | ✅  | ✅  | ✅  | ✅  |
-| LLaMA        | ✅  | ✅  | ✅  | ✅  |
-| ChatGLM      | ✅  | ✅  | ✅  | ✅  |
+| Model        | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+|--------------| ---- | ---- | ---- | ----  | ----  |
+| GPT-2        | ✅  | ✅  | ✅  | ✅  | ✅  |
+| Bloom        | ✅  | ✅  | ✅  | ✅  | ✅  |
+| OPT          | ✅  | ✅  | ✅  | ✅  | ✅  |
+| GPT-Neo      | ✅  | ✅  | ✅  | ✅  | ✅  |
+| GPT-J        | ✅  | ✅  | ✅  | ✅  | ✅  |
+| GPT-NeoX-20B | ✅  | ✅  | ✅  | ✅  | ✅  |
+| LLaMA        | ✅  | ✅  | ✅  | ✅  | ✅  |
+| ChatGLM      | ✅  | ✅  | ✅  | ✅  | ✅  |
 
 ### Conditional Generation
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ---- |
-| T5        | ✅   | ✅   | ✅   | ✅   |
-| BART      | ✅   | ✅   | ✅   | ✅   |
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ---- | ---- |
+| T5        | ✅   | ✅   | ✅   | ✅   | ✅   |
+| BART      | ✅   | ✅   | ✅   | ✅   | ✅   |
 
 ### Sequence Classification
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| BERT           | ✅  | ✅  | ✅  | ✅  |  
-| RoBERTa        | ✅  | ✅  | ✅  | ✅  |
-| GPT-2          | ✅  | ✅  | ✅  | ✅  | 
-| Bloom          | ✅  | ✅  | ✅  | ✅  |   
-| OPT            | ✅  | ✅  | ✅  | ✅  |
-| GPT-Neo        | ✅  | ✅  | ✅  | ✅  |
-| GPT-J          | ✅  | ✅  | ✅  | ✅  |
-| Deberta        | ✅  |     | ✅  | ✅  |     
-| Deberta-v2     | ✅  |     | ✅  | ✅  |    
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| BERT           | ✅  | ✅  | ✅  | ✅  |  ✅  |  
+| RoBERTa        | ✅  | ✅  | ✅  | ✅  | ✅  |
+| GPT-2          | ✅  | ✅  | ✅  | ✅  |   |
+| Bloom          | ✅  | ✅  | ✅  | ✅  |   |
+| OPT            | ✅  | ✅  | ✅  | ✅  |   |
+| GPT-Neo        | ✅  | ✅  | ✅  | ✅  |   |
+| GPT-J          | ✅  | ✅  | ✅  | ✅  |   |
+| Deberta        | ✅  |     | ✅  | ✅  |   | 
+| Deberta-v2     | ✅  |     | ✅  | ✅  |   |
 
 ### Token Classification
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| BERT           | ✅  | ✅  |   |   |  
-| RoBERTa        | ✅  | ✅  |   |   |
-| GPT-2          | ✅  | ✅  |   |   | 
-| Bloom          | ✅  | ✅  |   |   |   
-| OPT            | ✅  | ✅  |   |   |
-| GPT-Neo        | ✅  | ✅  |   |   |
-| GPT-J          | ✅  | ✅  |   |   |
-| Deberta        | ✅  |     |   |   | 
-| Deberta-v2     | ✅  |     |   |   |
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| BERT           | ✅  | ✅  |   |   |   |  
+| RoBERTa        | ✅  | ✅  |   |   |   |
+| GPT-2          | ✅  | ✅  |   |   |   |
+| Bloom          | ✅  | ✅  |   |   |   |
+| OPT            | ✅  | ✅  |   |   |   |
+| GPT-Neo        | ✅  | ✅  |   |   |   |
+| GPT-J          | ✅  | ✅  |   |   |   |
+| Deberta        | ✅  |     |   |   |   |
+| Deberta-v2     | ✅  |     |   |   |   |
 
 ### Text-to-Image Generation
 
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| Stable Diffusion           | ✅  |   |   |   |  
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| Stable Diffusion           | ✅  |   |   |   |   |  
 
 
 ### Image Classification
 
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| ViT           | ✅  |   |   |   | 
-| Swin           | ✅  |   |   |   | 
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| ViT           | ✅  |   |   |   |    | 
+| Swin           | ✅  |   |   |   |   |  
 
 ### Image to text (Multi-modal models)
 
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| Blip-2           | ✅  |   |   |   | 
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| Blip-2           | ✅  |   |   |   |   |
 
 ___Note that we have tested LoRA for [ViT](https://huggingface.co/docs/transformers/model_doc/vit) and [Swin](https://huggingface.co/docs/transformers/model_doc/swin) for fine-tuning on image classification. However, it should be possible to use LoRA for any compatible model [provided](https://huggingface.co/models?pipeline_tag=image-classification&sort=downloads&search=vit) by 🤗 Transformers. Check out the respective
 examples to learn more. If you run into problems, please open an issue.___
 
 The same principle applies to our [segmentation models](https://huggingface.co/models?pipeline_tag=image-segmentation&sort=downloads) as well. 
 
 ### Semantic Segmentation
 
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| SegFormer           | ✅  |   |   |   | 
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| SegFormer           | ✅  |   |   |   |   | 
 
 
 ## Caveats:
 
 1. Below is an example of using PyTorch FSDP for training. However, it doesn't lead to 
 any GPU memory savings. Please refer issue [[FSDP] FSDP with CPU offload consumes 1.65X more GPU memory when training models with most of the params frozen](https://github.com/pytorch/pytorch/issues/91165). 
 
@@ -375,35 +376,30 @@
   use_cpu: false
   ```
   b. run the below command to launch the example script
   ```bash
   accelerate launch --config_file fsdp_config.yaml examples/peft_lora_seq2seq_accelerate_fsdp.py
   ```
 
-2. When using `P_TUNING` or `PROMPT_TUNING` with `SEQ_2_SEQ` task, remember to remove the `num_virtual_token` virtual prompt predictions from the left side of the model outputs during evaluations. 
-
-3. For encoder-decoder models, `P_TUNING` or `PROMPT_TUNING` doesn't support `generate` functionality of transformers because `generate` strictly requires `decoder_input_ids` but 
-`P_TUNING`/`PROMPT_TUNING` appends soft prompt embeddings to `input_embeds` to create
-new `input_embeds` to be given to the model. Therefore, `generate` doesn't support this yet.
-
-4. When using ZeRO3 with zero3_init_flag=True, if you find the gpu memory increase with training steps. we might need to set zero3_init_flag=false in accelerate config.yaml. The related issue is [[BUG] memory leak under zero.Init](https://github.com/microsoft/DeepSpeed/issues/2637)
+2. When using ZeRO3 with zero3_init_flag=True, if you find the gpu memory increase with training steps. we might need to update deepspeed after [deepspeed commit 42858a9891422abc](https://github.com/microsoft/DeepSpeed/commit/42858a9891422abcecaa12c1bd432d28d33eb0d4) . The related issue is [[BUG] Peft Training with Zero.Init() and Zero3 will increase GPU memory every forward step ](https://github.com/microsoft/DeepSpeed/issues/3002)
 
 ## Backlog:
 - [x] Add tests
 - [x] Multi Adapter training and inference support
 - [x] Add more use cases and examples
-- [ ] Explore and possibly integrate `Bottleneck Adapters`, `(IA)^3`, `AdaptionPrompt` ...
+- [x] Integrate`(IA)^3`, `AdaptionPrompt`
+- [ ] Explore and possibly integrate methods like `Bottleneck Adapters`,  ...
 
 ## Citing 🤗 PEFT
 
 If you use 🤗 PEFT in your publication, please cite it by using the following BibTeX entry.
 
 ```bibtex
 @Misc{peft,
   title =        {PEFT: State-of-the-art Parameter-Efficient Fine-Tuning methods},
-  author =       {Sourab Mangrulkar, Sylvain Gugger, Lysandre Debut, Younes Belkada, Sayak Paul},
+  author =       {Sourab Mangrulkar and Sylvain Gugger and Lysandre Debut and Younes Belkada and Sayak Paul},
   howpublished = {\url{https://github.com/huggingface/peft}},
   year =         {2022}
 }
 ```
```

### Comparing `peft-0.3.0/README.md` & `peft-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 Supported methods:
 
 1. LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685)
 2. Prefix Tuning: [Prefix-Tuning: Optimizing Continuous Prompts for Generation](https://aclanthology.org/2021.acl-long.353/), [P-Tuning v2: Prompt Tuning Can Be Comparable to Fine-tuning Universally Across Scales and Tasks](https://arxiv.org/pdf/2110.07602.pdf)
 3. P-Tuning: [GPT Understands, Too](https://arxiv.org/abs/2103.10385)
 4. Prompt Tuning: [The Power of Scale for Parameter-Efficient Prompt Tuning](https://arxiv.org/abs/2104.08691)
 5. AdaLoRA: [Adaptive Budget Allocation for Parameter-Efficient Fine-Tuning](https://arxiv.org/abs/2303.10512)  
+6. $(IA)^3$ : [Infused Adapter by Inhibiting and Amplifying Inner Activations](https://arxiv.org/abs/2205.05638)
 
 ## Getting started
 
 ```python
 from transformers import AutoModelForSeq2SeqLM
 from peft import get_peft_config, get_peft_model, LoraConfig, TaskType
 model_name_or_path = "bigscience/mt0-large"
@@ -135,15 +136,15 @@
 - Here is an example in [trl](https://github.com/lvwerra/trl) library using PEFT+INT8 for tuning policy model: [gpt2-sentiment_peft.py](https://github.com/lvwerra/trl/blob/main/examples/sentiment/scripts/gpt2-sentiment_peft.py) and corresponding [Blog](https://huggingface.co/blog/trl-peft)
 - Example using PEFT for Instrction finetuning, reward model and policy : [stack_llama](https://github.com/lvwerra/trl/tree/main/examples/stack_llama/scripts) and corresponding [Blog](https://huggingface.co/blog/stackllama) 
 
 ### INT8 training of large models in Colab using PEFT LoRA and bits_and_bytes
 
 - Here is now a demo on how to fine tune [OPT-6.7b](https://huggingface.co/facebook/opt-6.7b) (14GB in fp16) in a Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jCkpikz0J2o20FBQmYmAGdiKmJGOMo-o?usp=sharing)
 
-- Here is now a demo on how to fine tune [whishper-large](openai/whisper-large-v2) (1.5B params) (14GB in fp16) in a Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1DOkD_5OUjFa0r5Ik3SgywJLJtEo2qLxO?usp=sharing) and [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vhF8yueFqha3Y3CpTHN6q9EVcII9EYzs?usp=sharing)
+- Here is now a demo on how to fine tune [whisper-large](https://huggingface.co/openai/whisper-large-v2) (1.5B params) (14GB in fp16) in a Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1DOkD_5OUjFa0r5Ik3SgywJLJtEo2qLxO?usp=sharing) and [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vhF8yueFqha3Y3CpTHN6q9EVcII9EYzs?usp=sharing)
 
 ### Save compute and storage even for medium and small models
 
 Save storage by avoiding full finetuning of models on each of the downstream tasks/datasets,
 With PEFT methods, users only need to store tiny checkpoints in the order of `MBs` all the while retaining 
 performance comparable to full finetuning.
 
@@ -219,87 +220,87 @@
 ### Example of PEFT model inference using 🤗 Accelerate's Big Model Inferencing capabilities
 An example is provided in `~examples/causal_language_modeling/peft_lora_clm_accelerate_big_model_inference.ipynb`. 
 
 
 ## Models support matrix
 
 ### Causal Language Modeling
-| Model        | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  |
-|--------------| ---- | ---- | ---- | ----  |
-| GPT-2        | ✅  | ✅  | ✅  | ✅  |
-| Bloom        | ✅  | ✅  | ✅  | ✅  |
-| OPT          | ✅  | ✅  | ✅  | ✅  |
-| GPT-Neo      | ✅  | ✅  | ✅  | ✅  |
-| GPT-J        | ✅  | ✅  | ✅  | ✅  |
-| GPT-NeoX-20B | ✅  | ✅  | ✅  | ✅  |
-| LLaMA        | ✅  | ✅  | ✅  | ✅  |
-| ChatGLM      | ✅  | ✅  | ✅  | ✅  |
+| Model        | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+|--------------| ---- | ---- | ---- | ----  | ----  |
+| GPT-2        | ✅  | ✅  | ✅  | ✅  | ✅  |
+| Bloom        | ✅  | ✅  | ✅  | ✅  | ✅  |
+| OPT          | ✅  | ✅  | ✅  | ✅  | ✅  |
+| GPT-Neo      | ✅  | ✅  | ✅  | ✅  | ✅  |
+| GPT-J        | ✅  | ✅  | ✅  | ✅  | ✅  |
+| GPT-NeoX-20B | ✅  | ✅  | ✅  | ✅  | ✅  |
+| LLaMA        | ✅  | ✅  | ✅  | ✅  | ✅  |
+| ChatGLM      | ✅  | ✅  | ✅  | ✅  | ✅  |
 
 ### Conditional Generation
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ---- |
-| T5        | ✅   | ✅   | ✅   | ✅   |
-| BART      | ✅   | ✅   | ✅   | ✅   |
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ---- | ---- |
+| T5        | ✅   | ✅   | ✅   | ✅   | ✅   |
+| BART      | ✅   | ✅   | ✅   | ✅   | ✅   |
 
 ### Sequence Classification
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| BERT           | ✅  | ✅  | ✅  | ✅  |  
-| RoBERTa        | ✅  | ✅  | ✅  | ✅  |
-| GPT-2          | ✅  | ✅  | ✅  | ✅  | 
-| Bloom          | ✅  | ✅  | ✅  | ✅  |   
-| OPT            | ✅  | ✅  | ✅  | ✅  |
-| GPT-Neo        | ✅  | ✅  | ✅  | ✅  |
-| GPT-J          | ✅  | ✅  | ✅  | ✅  |
-| Deberta        | ✅  |     | ✅  | ✅  |     
-| Deberta-v2     | ✅  |     | ✅  | ✅  |    
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| BERT           | ✅  | ✅  | ✅  | ✅  |  ✅  |  
+| RoBERTa        | ✅  | ✅  | ✅  | ✅  | ✅  |
+| GPT-2          | ✅  | ✅  | ✅  | ✅  |   |
+| Bloom          | ✅  | ✅  | ✅  | ✅  |   |
+| OPT            | ✅  | ✅  | ✅  | ✅  |   |
+| GPT-Neo        | ✅  | ✅  | ✅  | ✅  |   |
+| GPT-J          | ✅  | ✅  | ✅  | ✅  |   |
+| Deberta        | ✅  |     | ✅  | ✅  |   | 
+| Deberta-v2     | ✅  |     | ✅  | ✅  |   |
 
 ### Token Classification
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| BERT           | ✅  | ✅  |   |   |  
-| RoBERTa        | ✅  | ✅  |   |   |
-| GPT-2          | ✅  | ✅  |   |   | 
-| Bloom          | ✅  | ✅  |   |   |   
-| OPT            | ✅  | ✅  |   |   |
-| GPT-Neo        | ✅  | ✅  |   |   |
-| GPT-J          | ✅  | ✅  |   |   |
-| Deberta        | ✅  |     |   |   | 
-| Deberta-v2     | ✅  |     |   |   |
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| BERT           | ✅  | ✅  |   |   |   |  
+| RoBERTa        | ✅  | ✅  |   |   |   |
+| GPT-2          | ✅  | ✅  |   |   |   |
+| Bloom          | ✅  | ✅  |   |   |   |
+| OPT            | ✅  | ✅  |   |   |   |
+| GPT-Neo        | ✅  | ✅  |   |   |   |
+| GPT-J          | ✅  | ✅  |   |   |   |
+| Deberta        | ✅  |     |   |   |   |
+| Deberta-v2     | ✅  |     |   |   |   |
 
 ### Text-to-Image Generation
 
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| Stable Diffusion           | ✅  |   |   |   |  
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| Stable Diffusion           | ✅  |   |   |   |   |  
 
 
 ### Image Classification
 
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| ViT           | ✅  |   |   |   | 
-| Swin           | ✅  |   |   |   | 
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| ViT           | ✅  |   |   |   |    | 
+| Swin           | ✅  |   |   |   |   |  
 
 ### Image to text (Multi-modal models)
 
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| Blip-2           | ✅  |   |   |   | 
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| Blip-2           | ✅  |   |   |   |   |
 
 ___Note that we have tested LoRA for [ViT](https://huggingface.co/docs/transformers/model_doc/vit) and [Swin](https://huggingface.co/docs/transformers/model_doc/swin) for fine-tuning on image classification. However, it should be possible to use LoRA for any compatible model [provided](https://huggingface.co/models?pipeline_tag=image-classification&sort=downloads&search=vit) by 🤗 Transformers. Check out the respective
 examples to learn more. If you run into problems, please open an issue.___
 
 The same principle applies to our [segmentation models](https://huggingface.co/models?pipeline_tag=image-segmentation&sort=downloads) as well. 
 
 ### Semantic Segmentation
 
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| SegFormer           | ✅  |   |   |   | 
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| SegFormer           | ✅  |   |   |   |   | 
 
 
 ## Caveats:
 
 1. Below is an example of using PyTorch FSDP for training. However, it doesn't lead to 
 any GPU memory savings. Please refer issue [[FSDP] FSDP with CPU offload consumes 1.65X more GPU memory when training models with most of the params frozen](https://github.com/pytorch/pytorch/issues/91165). 
 
@@ -348,33 +349,28 @@
   use_cpu: false
   ```
   b. run the below command to launch the example script
   ```bash
   accelerate launch --config_file fsdp_config.yaml examples/peft_lora_seq2seq_accelerate_fsdp.py
   ```
 
-2. When using `P_TUNING` or `PROMPT_TUNING` with `SEQ_2_SEQ` task, remember to remove the `num_virtual_token` virtual prompt predictions from the left side of the model outputs during evaluations. 
-
-3. For encoder-decoder models, `P_TUNING` or `PROMPT_TUNING` doesn't support `generate` functionality of transformers because `generate` strictly requires `decoder_input_ids` but 
-`P_TUNING`/`PROMPT_TUNING` appends soft prompt embeddings to `input_embeds` to create
-new `input_embeds` to be given to the model. Therefore, `generate` doesn't support this yet.
-
-4. When using ZeRO3 with zero3_init_flag=True, if you find the gpu memory increase with training steps. we might need to set zero3_init_flag=false in accelerate config.yaml. The related issue is [[BUG] memory leak under zero.Init](https://github.com/microsoft/DeepSpeed/issues/2637)
+2. When using ZeRO3 with zero3_init_flag=True, if you find the gpu memory increase with training steps. we might need to update deepspeed after [deepspeed commit 42858a9891422abc](https://github.com/microsoft/DeepSpeed/commit/42858a9891422abcecaa12c1bd432d28d33eb0d4) . The related issue is [[BUG] Peft Training with Zero.Init() and Zero3 will increase GPU memory every forward step ](https://github.com/microsoft/DeepSpeed/issues/3002)
 
 ## Backlog:
 - [x] Add tests
 - [x] Multi Adapter training and inference support
 - [x] Add more use cases and examples
-- [ ] Explore and possibly integrate `Bottleneck Adapters`, `(IA)^3`, `AdaptionPrompt` ...
+- [x] Integrate`(IA)^3`, `AdaptionPrompt`
+- [ ] Explore and possibly integrate methods like `Bottleneck Adapters`,  ...
 
 ## Citing 🤗 PEFT
 
 If you use 🤗 PEFT in your publication, please cite it by using the following BibTeX entry.
 
 ```bibtex
 @Misc{peft,
   title =        {PEFT: State-of-the-art Parameter-Efficient Fine-Tuning methods},
-  author =       {Sourab Mangrulkar, Sylvain Gugger, Lysandre Debut, Younes Belkada, Sayak Paul},
+  author =       {Sourab Mangrulkar and Sylvain Gugger and Lysandre Debut and Younes Belkada and Sayak Paul},
   howpublished = {\url{https://github.com/huggingface/peft}},
   year =         {2022}
 }
 ```
```

### Comparing `peft-0.3.0/pyproject.toml` & `peft-0.4.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -29,8 +29,15 @@
 ensure_newline_before_comments = true
 
 [tool.pytest]
 doctest_optionflags = [
     "NORMALIZE_WHITESPACE",
     "ELLIPSIS",
     "NUMBER",
-]
+]
+
+[tool.pytest.ini_options]
+addopts = "--cov=src/peft --cov-report=term-missing"
+markers = [
+    "single_gpu_tests: tests that run on a single GPU",
+    "multi_gpu_tests: tests that run on multiple GPUs",
+]
```

### Comparing `peft-0.3.0/setup.py` & `peft-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,54 +11,55 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import find_packages, setup
 
 extras = {}
-extras["quality"] = ["black ~= 22.0", "ruff>=0.0.241"]
+extras["quality"] = ["black ~= 22.0", "ruff>=0.0.241", "urllib3<=2.0.0"]
 extras["docs_specific"] = ["hf-doc-builder"]
 extras["dev"] = extras["quality"] + extras["docs_specific"]
-extras["test"] = extras["dev"] + ["pytest", "pytest-xdist", "parameterized", "datasets"]
+extras["test"] = extras["dev"] + ["pytest", "pytest-cov", "pytest-xdist", "parameterized", "datasets", "diffusers"]
 
 setup(
     name="peft",
-    version="0.3.0",
+    version="0.4.0",
     description="Parameter-Efficient Fine-Tuning (PEFT)",
     license_files=["LICENSE"],
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="Apache",
     author="The HuggingFace team",
     author_email="sourab@huggingface.co",
     url="https://github.com/huggingface/peft",
     package_dir={"": "src"},
     packages=find_packages("src"),
     entry_points={},
-    python_requires=">=3.7.0",
+    python_requires=">=3.8.0",
     install_requires=[
         "numpy>=1.17",
         "packaging>=20.0",
         "psutil",
         "pyyaml",
         "torch>=1.13.0",
         "transformers",
         "accelerate",
+        "safetensors",
     ],
     extras_require=extras,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
 )
 
 # Release checklist
 # 1. Change the version in __init__.py and setup.py.
 # 2. Commit these changes with the message: "Release: VERSION"
```

### Comparing `peft-0.3.0/src/peft/__init__.py` & `peft-0.4.0/src/peft/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,29 +13,42 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
+from .auto import (
+    AutoPeftModel,
+    AutoPeftModelForCausalLM,
+    AutoPeftModelForSequenceClassification,
+    AutoPeftModelForSeq2SeqLM,
+    AutoPeftModelForTokenClassification,
+    AutoPeftModelForQuestionAnswering,
+    AutoPeftModelForFeatureExtraction,
+)
 from .mapping import MODEL_TYPE_TO_PEFT_MODEL_MAPPING, PEFT_TYPE_TO_CONFIG_MAPPING, get_peft_config, get_peft_model
 from .peft_model import (
     PeftModel,
     PeftModelForCausalLM,
     PeftModelForSeq2SeqLM,
     PeftModelForSequenceClassification,
     PeftModelForTokenClassification,
+    PeftModelForQuestionAnswering,
+    PeftModelForFeatureExtraction,
 )
 from .tuners import (
     AdaptionPromptConfig,
     AdaptionPromptModel,
     LoraConfig,
     LoraModel,
+    IA3Config,
+    IA3Model,
     AdaLoraConfig,
     AdaLoraModel,
     PrefixEncoder,
     PrefixTuningConfig,
     PromptEmbedding,
     PromptEncoder,
     PromptEncoderConfig,
@@ -48,10 +61,11 @@
     PeftConfig,
     PeftType,
     PromptLearningConfig,
     TaskType,
     bloom_model_postprocess_past_key_value,
     get_peft_model_state_dict,
     prepare_model_for_int8_training,
+    prepare_model_for_kbit_training,
     set_peft_model_state_dict,
     shift_tokens_right,
 )
```

### Comparing `peft-0.3.0/src/peft/import_utils.py` & `peft-0.4.0/src/peft/import_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,7 +13,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import importlib
 
 
 def is_bnb_available():
     return importlib.util.find_spec("bitsandbytes") is not None
+
+
+def is_bnb_4bit_available():
+    if not is_bnb_available():
+        return False
+
+    import bitsandbytes as bnb
+
+    return hasattr(bnb.nn, "Linear4bit")
```

### Comparing `peft-0.3.0/src/peft/peft_model.py` & `peft-0.4.0/src/peft/peft_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,59 +9,73 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from __future__ import annotations
+
 import inspect
 import os
 import warnings
 from contextlib import contextmanager
+from copy import deepcopy
+from typing import Any, Dict, List, Optional, Union
 
 import torch
 from accelerate import dispatch_model, infer_auto_device_map
 from accelerate.hooks import AlignDevicesHook, add_hook_to_module, remove_hook_from_submodules
 from accelerate.utils import get_balanced_memory
 from huggingface_hub import hf_hub_download
+from huggingface_hub.utils import EntryNotFoundError
+from safetensors.torch import load_file as safe_load_file
+from safetensors.torch import save_file as safe_save_file
 from torch.nn import BCEWithLogitsLoss, CrossEntropyLoss, MSELoss
 from transformers import PreTrainedModel
-from transformers.modeling_outputs import SequenceClassifierOutput, TokenClassifierOutput
+from transformers.modeling_outputs import QuestionAnsweringModelOutput, SequenceClassifierOutput, TokenClassifierOutput
 from transformers.utils import PushToHubMixin
 
+from . import __version__
 from .tuners import (
     AdaLoraModel,
     AdaptionPromptModel,
+    IA3Model,
     LoraModel,
     PrefixEncoder,
     PromptEmbedding,
     PromptEncoder,
 )
 from .utils import (
+    SAFETENSORS_WEIGHTS_NAME,
     TRANSFORMERS_MODELS_TO_PREFIX_TUNING_POSTPROCESS_MAPPING,
     WEIGHTS_NAME,
     PeftConfig,
     PeftType,
     PromptLearningConfig,
     TaskType,
+    _prepare_prompt_learning_config,
     _set_adapter,
     _set_trainable,
+    add_library_to_model_card,
     get_peft_model_state_dict,
+    hub_file_exists,
     set_peft_model_state_dict,
     shift_tokens_right,
 )
 
 
 PEFT_TYPE_TO_MODEL_MAPPING = {
     PeftType.LORA: LoraModel,
     PeftType.PROMPT_TUNING: PromptEmbedding,
     PeftType.P_TUNING: PromptEncoder,
     PeftType.PREFIX_TUNING: PrefixEncoder,
     PeftType.ADALORA: AdaLoraModel,
     PeftType.ADAPTION_PROMPT: AdaptionPromptModel,
+    PeftType.IA3: IA3Model,
 }
 
 
 class PeftModel(PushToHubMixin, torch.nn.Module):
     """
     Base model encompassing various Peft methods.
 
@@ -81,92 +95,168 @@
         using [`PromptLearningConfig`].
         - **transformer_backbone_name** (`str`) -- The name of the transformer
         backbone in the base model if using [`PromptLearningConfig`].
         - **word_embeddings** (`torch.nn.Embedding`) -- The word embeddings of the transformer backbone
         in the base model if using [`PromptLearningConfig`].
     """
 
-    def __init__(self, model, peft_config: PeftConfig, adapter_name="default"):
+    def __init__(self, model: PreTrainedModel, peft_config: PeftConfig, adapter_name: str = "default"):
         super().__init__()
         self.base_model = model
-        self.config = self.base_model.config
+        self.config = getattr(self.base_model, "config", {"model_type": "custom"})
         self.modules_to_save = None
         self.peft_config = {}
         self.active_adapter = adapter_name
         self.peft_type = peft_config.peft_type
-        self.base_model_torch_dtype = getattr(model, "dtype", None)
         if not isinstance(peft_config, PromptLearningConfig):
             self.peft_config[adapter_name] = peft_config
             self.base_model = PEFT_TYPE_TO_MODEL_MAPPING[peft_config.peft_type](
                 self.base_model, self.peft_config, adapter_name
             )
             self.set_additional_trainable_modules(peft_config, adapter_name)
         else:
             self.add_adapter(adapter_name, peft_config)
 
-    def save_pretrained(self, save_directory, **kwargs):
+        if getattr(model, "is_gradient_checkpointing", True):
+            model = self._prepare_model_for_gradient_checkpointing(model)
+
+    def save_pretrained(
+        self,
+        save_directory: str,
+        safe_serialization: bool = False,
+        selected_adapters: Optional[List[str]] = None,
+        **kwargs: Any,
+    ):
         r"""
         This function saves the adapter model and the adapter configuration files to a directory, so that it can be
         reloaded using the [`LoraModel.from_pretrained`] class method, and also used by the [`LoraModel.push_to_hub`]
         method.
 
         Args:
             save_directory (`str`):
                 Directory where the adapter model and configuration files will be saved (will be created if it does not
                 exist).
             kwargs (additional keyword arguments, *optional*):
                 Additional keyword arguments passed along to the `push_to_hub` method.
         """
         if os.path.isfile(save_directory):
             raise ValueError(f"Provided path ({save_directory}) should be a directory, not a file")
+
+        if selected_adapters is None:
+            selected_adapters = list(self.peft_config.keys())
+        else:
+            if any(
+                selected_adapter_name not in list(self.peft_config.keys())
+                for selected_adapter_name in selected_adapters
+            ):
+                raise ValueError(
+                    f"You passed an invalid `selected_adapters` arguments, current supported adapter names are"
+                    f" {list(self.peft_config.keys())} - got {selected_adapters}."
+                )
+
         os.makedirs(save_directory, exist_ok=True)
+        self.create_or_update_model_card(save_directory)
 
-        for adapter_name, peft_config in self.peft_config.items():
+        for adapter_name in selected_adapters:
+            peft_config = self.peft_config[adapter_name]
             # save only the trainable weights
             output_state_dict = get_peft_model_state_dict(
                 self, state_dict=kwargs.get("state_dict", None), adapter_name=adapter_name
             )
             output_dir = os.path.join(save_directory, adapter_name) if adapter_name != "default" else save_directory
             os.makedirs(output_dir, exist_ok=True)
-            torch.save(output_state_dict, os.path.join(output_dir, WEIGHTS_NAME))
+
+            if safe_serialization:
+                safe_save_file(
+                    output_state_dict,
+                    os.path.join(output_dir, SAFETENSORS_WEIGHTS_NAME),
+                    metadata={"format": "pt"},
+                )
+            else:
+                torch.save(output_state_dict, os.path.join(output_dir, WEIGHTS_NAME))
 
             # save the config and change the inference mode to `True`
             if peft_config.base_model_name_or_path is None:
                 peft_config.base_model_name_or_path = (
                     self.base_model.__dict__.get("name_or_path", None)
                     if isinstance(peft_config, PromptLearningConfig)
                     else self.base_model.model.__dict__.get("name_or_path", None)
                 )
             inference_mode = peft_config.inference_mode
             peft_config.inference_mode = True
-            peft_config.save_pretrained(output_dir)
+
+            if peft_config.task_type is None:
+                # deal with auto mapping
+                base_model_class = self._get_base_model_class(
+                    is_prompt_tuning=isinstance(peft_config, PromptLearningConfig)
+                )
+                parent_library = base_model_class.__module__
+
+                auto_mapping_dict = {
+                    "base_model_class": base_model_class.__name__,
+                    "parent_library": parent_library,
+                }
+            else:
+                auto_mapping_dict = None
+
+            peft_config.save_pretrained(output_dir, auto_mapping_dict=auto_mapping_dict)
             peft_config.inference_mode = inference_mode
 
     @classmethod
-    def from_pretrained(cls, model, model_id, adapter_name="default", is_trainable=False, **kwargs):
+    def from_pretrained(
+        cls,
+        model: PreTrainedModel,
+        model_id: Union[str, os.PathLike],
+        adapter_name: str = "default",
+        is_trainable: bool = False,
+        config: Optional[PeftConfig] = None,
+        **kwargs: Any,
+    ):
         r"""
         Instantiate a [`LoraModel`] from a pretrained Lora configuration and weights.
 
         Args:
             model ([`~transformers.PreTrainedModel`]):
                 The model to be adapted. The model should be initialized with the
                 [`~transformers.PreTrainedModel.from_pretrained`] method from the 🤗 Transformers library.
             model_id (`str` or `os.PathLike`):
                 The name of the Lora configuration to use. Can be either:
                     - A string, the `model id` of a Lora configuration hosted inside a model repo on the Hugging Face
                       Hub.
                     - A path to a directory containing a Lora configuration file saved using the `save_pretrained`
                       method (`./my_lora_config_directory/`).
+            adapter_name (`str`, *optional*, defaults to `"default"`):
+                The name of the adapter to be loaded. This is useful for loading multiple adapters.
+            is_trainable (`bool`, *optional*, defaults to `False`):
+                Whether the adapter should be trainable or not. If `False`, the adapter will be frozen and use for
+                inference
+            config ([`~peft.PeftConfig`], *optional*):
+                The configuration object to use instead of an automatically loaded configuation. This configuration
+                object is mutually exclusive with `model_id` and `kwargs`. This is useful when configuration is already
+                loaded before calling `from_pretrained`.
+            kwargs: (`optional`):
+                Additional keyword arguments passed along to the specific Lora configuration class.
         """
         from .mapping import MODEL_TYPE_TO_PEFT_MODEL_MAPPING, PEFT_TYPE_TO_CONFIG_MAPPING
 
         # load the config
-        config = PEFT_TYPE_TO_CONFIG_MAPPING[
-            PeftConfig.from_pretrained(model_id, subfolder=kwargs.get("subfolder", None)).peft_type
-        ].from_pretrained(model_id, subfolder=kwargs.get("subfolder", None))
+        if config is None:
+            config = PEFT_TYPE_TO_CONFIG_MAPPING[
+                PeftConfig._get_peft_type(
+                    model_id,
+                    subfolder=kwargs.get("subfolder", None),
+                    revision=kwargs.get("revision", None),
+                    cache_dir=kwargs.get("cache_dir", None),
+                    use_auth_token=kwargs.get("use_auth_token", None),
+                )
+            ].from_pretrained(model_id, **kwargs)
+        elif isinstance(config, PeftConfig):
+            config.inference_mode = not is_trainable
+        else:
+            raise ValueError(f"The input config must be a PeftConfig, got {config.__class__}")
 
         if (getattr(model, "hf_device_map", None) is not None) and len(
             set(model.hf_device_map.values()).intersection({"cpu", "disk"})
         ) > 0:
             remove_hook_from_submodules(model)
 
         if isinstance(config, PromptLearningConfig) and is_trainable:
@@ -174,30 +264,33 @@
         else:
             config.inference_mode = not is_trainable
 
         if config.task_type not in MODEL_TYPE_TO_PEFT_MODEL_MAPPING.keys():
             model = cls(model, config, adapter_name)
         else:
             model = MODEL_TYPE_TO_PEFT_MODEL_MAPPING[config.task_type](model, config, adapter_name)
-        model.load_adapter(model_id, adapter_name, **kwargs)
+        model.load_adapter(model_id, adapter_name, is_trainable=is_trainable, **kwargs)
         return model
 
-    def _setup_prompt_encoder(self, adapter_name):
+    def _setup_prompt_encoder(self, adapter_name: str):
         config = self.peft_config[adapter_name]
-        self.prompt_encoder = torch.nn.ModuleDict({})
-        self.prompt_tokens = {}
+        if not hasattr(self, "prompt_encoder"):
+            self.prompt_encoder = torch.nn.ModuleDict({})
+            self.prompt_tokens = {}
         transformer_backbone = None
         for name, module in self.base_model.named_children():
             for param in module.parameters():
                 param.requires_grad = False
             if isinstance(module, PreTrainedModel):
                 # Make sure to freeze Tranformers model
                 if transformer_backbone is None:
                     transformer_backbone = module
                     self.transformer_backbone_name = name
+        if transformer_backbone is None:
+            transformer_backbone = self.base_model
 
         if config.num_transformer_submodules is None:
             config.num_transformer_submodules = 2 if config.task_type == TaskType.SEQ_2_SEQ_LM else 1
 
         for named_param, value in list(transformer_backbone.named_parameters()):
             if value.shape[0] == self.base_model.config.vocab_size:
                 self.word_embeddings = transformer_backbone.get_submodule(named_param.replace(".weight", ""))
@@ -207,43 +300,70 @@
             prompt_encoder = PromptEmbedding(config, self.word_embeddings)
         elif config.peft_type == PeftType.P_TUNING:
             prompt_encoder = PromptEncoder(config)
         elif config.peft_type == PeftType.PREFIX_TUNING:
             prompt_encoder = PrefixEncoder(config)
         else:
             raise ValueError("Not supported")
+
+        prompt_encoder = prompt_encoder.to(self.device)
         self.prompt_encoder.update(torch.nn.ModuleDict({adapter_name: prompt_encoder}))
         self.prompt_tokens[adapter_name] = torch.arange(
             config.num_virtual_tokens * config.num_transformer_submodules
         ).long()
 
-    def get_prompt_embedding_to_save(self, adapter_name):
+    def _prepare_model_for_gradient_checkpointing(self, model: PreTrainedModel):
+        r"""
+        Prepares the model for gradient checkpointing if necessary
+        """
+        if not (getattr(model, "is_loaded_in_8bit", False) or getattr(model, "is_loaded_in_4bit", False)):
+            if hasattr(model, "enable_input_require_grads"):
+                model.enable_input_require_grads()
+            elif hasattr(model, "get_input_embeddings"):
+
+                def make_inputs_require_grad(module, input, output):
+                    output.requires_grad_(True)
+
+                model.get_input_embeddings().register_forward_hook(make_inputs_require_grad)
+        return model
+
+    def get_prompt_embedding_to_save(self, adapter_name: str):
         """
         Returns the prompt embedding to save when saving the model. Only applicable when `peft_config.peft_type !=
         PeftType.LORA`.
         """
-        prompt_tokens = self.prompt_tokens[adapter_name].unsqueeze(0).expand(1, -1).to(self.device)
+        prompt_encoder = self.prompt_encoder[adapter_name]
+        prompt_tokens = (
+            self.prompt_tokens[adapter_name].unsqueeze(0).expand(1, -1).to(prompt_encoder.embedding.weight.device)
+        )
         if self.peft_config[adapter_name].peft_type == PeftType.PREFIX_TUNING:
             prompt_tokens = prompt_tokens[:, : self.peft_config[adapter_name].num_virtual_tokens]
-        prompt_embeddings = self.prompt_encoder[adapter_name](prompt_tokens)
+        prompt_embeddings = prompt_encoder(prompt_tokens)
         return prompt_embeddings[0].detach().cpu()
 
-    def get_prompt(self, batch_size):
+    def get_prompt(self, batch_size: int):
         """
         Returns the virtual prompts to use for Peft. Only applicable when `peft_config.peft_type != PeftType.LORA`.
         """
         peft_config = self.active_peft_config
         prompt_encoder = self.prompt_encoder[self.active_adapter]
-        prompt_tokens = self.prompt_tokens[self.active_adapter].unsqueeze(0).expand(batch_size, -1).to(self.device)
+        prompt_tokens = (
+            self.prompt_tokens[self.active_adapter]
+            .unsqueeze(0)
+            .expand(batch_size, -1)
+            .to(prompt_encoder.embedding.weight.device)
+        )
         if peft_config.peft_type == PeftType.PREFIX_TUNING:
             prompt_tokens = prompt_tokens[:, : peft_config.num_virtual_tokens]
             if peft_config.inference_mode:
                 past_key_values = prompt_encoder.embedding.weight.repeat(batch_size, 1, 1)
             else:
                 past_key_values = prompt_encoder(prompt_tokens)
+            if self.base_model_torch_dtype is not None:
+                past_key_values = past_key_values.to(self.base_model_torch_dtype)
             past_key_values = past_key_values.view(
                 batch_size,
                 peft_config.num_virtual_tokens,
                 peft_config.num_layers * 2,
                 peft_config.num_attention_heads,
                 peft_config.token_dim // peft_config.num_attention_heads,
             )
@@ -275,109 +395,174 @@
             if num_params == 0 and hasattr(param, "ds_numel"):
                 num_params = param.ds_numel
 
             all_param += num_params
             if param.requires_grad:
                 trainable_params += num_params
         print(
-            f"trainable params: {trainable_params} || all params: {all_param} || trainable%: {100 * trainable_params / all_param}"
+            f"trainable params: {trainable_params:,d} || all params: {all_param:,d} || trainable%: {100 * trainable_params / all_param}"
         )
 
     def __getattr__(self, name: str):
         """Forward missing attributes to the wrapped module."""
         try:
             return super().__getattr__(name)  # defer to nn.Module's logic
         except AttributeError:
             return getattr(self.base_model, name)
 
-    def forward(self, *args, **kwargs):
+    def forward(self, *args: Any, **kwargs: Any):
         """
         Forward pass of the model.
         """
         return self.get_base_model()(*args, **kwargs)
 
+    def _get_base_model_class(self, is_prompt_tuning=False):
+        """
+        Returns the base model class.
+        """
+        if not is_prompt_tuning:
+            return self.base_model.model.__class__
+        return self.base_model.__class__
+
     @contextmanager
     def disable_adapter(self):
         """
         Disables the adapter module.
         """
         try:
-            if isinstance(self.peft_config, PromptLearningConfig):
+            if isinstance(self.peft_config[self.active_adapter], PromptLearningConfig):
+                # TODO: consider replacing this patching of methods with a more robust mechanism: setting a flag and
+                # letting the underyling methods deal with it, same as how LoRA does it.
                 old_forward = self.forward
                 self.forward = self.base_model.forward
+                old_prepare_inputs_for_generation = self.prepare_inputs_for_generation
+                self.prepare_inputs_for_generation = self.base_model.prepare_inputs_for_generation
             else:
                 self.base_model.disable_adapter_layers()
             yield
         finally:
-            if isinstance(self.peft_config, PromptLearningConfig):
+            if isinstance(self.peft_config[self.active_adapter], PromptLearningConfig):
                 self.forward = old_forward
+                self.old_prepare_inputs_for_generation = old_prepare_inputs_for_generation
             else:
                 self.base_model.enable_adapter_layers()
 
     def get_base_model(self):
         """
         Returns the base model.
         """
         return self.base_model if isinstance(self.active_peft_config, PromptLearningConfig) else self.base_model.model
 
-    def add_adapter(self, adapter_name, peft_config):
+    def add_adapter(self, adapter_name: str, peft_config: PeftConfig):
         if peft_config.peft_type != self.peft_type:
             raise ValueError(
                 f"Cannot combine adapters with different peft types. "
                 f"Found {self.peft_type} and {peft_config.peft_type}."
             )
         self.peft_config[adapter_name] = peft_config
         if isinstance(peft_config, PromptLearningConfig):
+            if hasattr(self.config, "to_dict"):
+                dict_config = self.config.to_dict()
+            else:
+                dict_config = self.config
+
+            peft_config = _prepare_prompt_learning_config(peft_config, dict_config)
             self._setup_prompt_encoder(adapter_name)
         else:
             self.base_model.add_adapter(adapter_name, peft_config)
 
         self.set_additional_trainable_modules(peft_config, adapter_name)
 
     def set_additional_trainable_modules(self, peft_config, adapter_name):
         if getattr(peft_config, "modules_to_save", None) is not None:
             if self.modules_to_save is None:
                 self.modules_to_save = set(peft_config.modules_to_save)
             else:
                 self.modules_to_save.update(peft_config.modules_to_save)
             _set_trainable(self, adapter_name)
 
-    def load_adapter(self, model_id, adapter_name, is_trainable=False, **kwargs):
+    @classmethod
+    def _split_kwargs(cls, kwargs: Dict[str, Any]):
+        _kwargs_not_in_hf_hub_download_signature = ("use_auth_token",)
+        hf_hub_download_kwargs = {}
+        other_kwargs = {}
+
+        for key, value in kwargs.items():
+            if key in inspect.signature(hf_hub_download).parameters or key in _kwargs_not_in_hf_hub_download_signature:
+                hf_hub_download_kwargs[key] = value
+            else:
+                other_kwargs[key] = value
+
+        return hf_hub_download_kwargs, other_kwargs
+
+    def load_adapter(self, model_id: str, adapter_name: str, is_trainable: bool = False, **kwargs: Any):
         from .mapping import PEFT_TYPE_TO_CONFIG_MAPPING
 
+        hf_hub_download_kwargs, kwargs = self._split_kwargs(kwargs)
+
         if adapter_name not in self.peft_config:
             # load the config
             peft_config = PEFT_TYPE_TO_CONFIG_MAPPING[
-                PeftConfig.from_pretrained(model_id, subfolder=kwargs.get("subfolder", None)).peft_type
-            ].from_pretrained(model_id, subfolder=kwargs.get("subfolder", None))
+                PeftConfig._get_peft_type(
+                    model_id,
+                    **hf_hub_download_kwargs,
+                )
+            ].from_pretrained(
+                model_id,
+                **hf_hub_download_kwargs,
+            )
             if isinstance(peft_config, PromptLearningConfig) and is_trainable:
                 raise ValueError("Cannot set a prompt learning adapter to trainable when loading pretrained adapter.")
             else:
                 peft_config.inference_mode = not is_trainable
             self.add_adapter(adapter_name, peft_config)
 
         # load weights if any
         path = os.path.join(model_id, kwargs["subfolder"]) if kwargs.get("subfolder", None) is not None else model_id
 
-        if os.path.exists(os.path.join(path, WEIGHTS_NAME)):
+        if os.path.exists(os.path.join(path, SAFETENSORS_WEIGHTS_NAME)):
+            filename = os.path.join(path, SAFETENSORS_WEIGHTS_NAME)
+            use_safetensors = True
+        elif os.path.exists(os.path.join(path, WEIGHTS_NAME)):
             filename = os.path.join(path, WEIGHTS_NAME)
+            use_safetensors = False
         else:
-            try:
-                filename = hf_hub_download(model_id, WEIGHTS_NAME, subfolder=kwargs.get("subfolder", None))
-            except:  # noqa
-                raise ValueError(
-                    f"Can't find weights for {model_id} in {model_id} or in the Hugging Face Hub. "
-                    f"Please check that the file {WEIGHTS_NAME} is present at {model_id}."
+            has_remote_safetensors_file = hub_file_exists(
+                model_id,
+                SAFETENSORS_WEIGHTS_NAME,
+                revision=hf_hub_download_kwargs.get("revision", None),
+                repo_type=hf_hub_download_kwargs.get("repo_type", None),
+            )
+            use_safetensors = has_remote_safetensors_file
+
+            if has_remote_safetensors_file:
+                # Priority 1: load safetensors weights
+                filename = hf_hub_download(
+                    model_id,
+                    SAFETENSORS_WEIGHTS_NAME,
+                    **hf_hub_download_kwargs,
                 )
+            else:
+                try:
+                    filename = hf_hub_download(model_id, WEIGHTS_NAME, **hf_hub_download_kwargs)
+                except EntryNotFoundError:
+                    raise ValueError(
+                        f"Can't find weights for {model_id} in {model_id} or in the Hugging Face Hub. "
+                        f"Please check that the file {WEIGHTS_NAME} or {SAFETENSORS_WEIGHTS_NAME} is present at {model_id}."
+                    )
+
+        if use_safetensors:
+            adapters_weights = safe_load_file(filename, device="cuda" if torch.cuda.is_available() else "cpu")
+        else:
+            adapters_weights = torch.load(
+                filename, map_location=torch.device("cuda" if torch.cuda.is_available() else "cpu")
+            )
 
-        adapters_weights = torch.load(
-            filename, map_location=torch.device("cuda" if torch.cuda.is_available() else "cpu")
-        )
         # load the weights into the model
-        set_peft_model_state_dict(self, adapters_weights, adapter_name=adapter_name)
+        load_result = set_peft_model_state_dict(self, adapters_weights, adapter_name=adapter_name)
         if (
             (getattr(self, "hf_device_map", None) is not None)
             and (len(set(self.hf_device_map.values()).intersection({"cpu", "disk"})) > 0)
             and len(self.peft_config) == 1
         ):
             device_map = kwargs.get("device_map", "auto")
             max_memory = kwargs.get("max_memory", None)
@@ -411,31 +596,77 @@
             )
             hook = AlignDevicesHook(io_same_device=True)
             if isinstance(self.peft_config[adapter_name], PromptLearningConfig):
                 remove_hook_from_submodules(self.prompt_encoder)
             add_hook_to_module(self.get_base_model(), hook)
 
         # Set model in evaluation mode to deactivate Dropout modules by default
-        self.eval()
+        if not is_trainable:
+            self.eval()
+        return load_result
 
-    def set_adapter(self, adapter_name):
+    def set_adapter(self, adapter_name: str):
         """
         Sets the active adapter.
         """
         if adapter_name not in self.peft_config:
             raise ValueError(f"Adapter {adapter_name} not found.")
         self.active_adapter = adapter_name
         if not isinstance(self.peft_config[adapter_name], PromptLearningConfig):
             self.base_model.set_adapter(adapter_name)
         _set_adapter(self, adapter_name)
 
     @property
+    def base_model_torch_dtype(self):
+        return getattr(self.base_model, "dtype", None)
+
+    @property
     def active_peft_config(self):
         return self.peft_config[self.active_adapter]
 
+    def create_or_update_model_card(self, output_dir: str):
+        """
+        Updates or create model card to include information about peft:
+        1. Adds `peft` library tag
+        2. Adds peft version
+        3. Adds quantization information if it was used
+        """
+        # Adds `peft` library tag
+        add_library_to_model_card(output_dir)
+
+        with open(os.path.join(output_dir, "README.md"), "r") as f:
+            lines = f.readlines()
+
+        quantization_config = None
+        if hasattr(self.config, "quantization_config"):
+            quantization_config = self.config.quantization_config.to_dict()
+        training_config_text = ""
+        # Adds quantization information if it was used
+        if quantization_config is not None:
+            training_config_text += "\nThe following `bitsandbytes` quantization config was used during training:\n"
+            training_config_text += "\n".join([f"- {name}: {value}" for name, value in quantization_config.items()])
+            training_config_text += "\n"
+
+        training_procedure_heading = "## Training procedure\n"
+        if training_procedure_heading in lines:
+            lines.insert(lines.index(training_procedure_heading) + 2, training_config_text)
+        else:
+            lines.append(f"{training_procedure_heading}\n{training_config_text}")
+
+        # Adds peft version
+        framework_block_heading = "### Framework versions\n"
+        if framework_block_heading in lines:
+            lines.insert(lines.index(framework_block_heading) + 2, f"- PEFT {__version__}\n")
+        else:
+            lines.append(f"{framework_block_heading}\n\n- PEFT {__version__}\n")
+
+        # write the lines back to README.md
+        with open(os.path.join(output_dir, "README.md"), "w") as f:
+            f.writelines(lines)
+
 
 class PeftModelForSequenceClassification(PeftModel):
     """
     Peft model for sequence classification tasks.
 
     Args:
         model ([`~transformers.PreTrainedModel`]): Base transformer model.
@@ -512,15 +743,15 @@
                 return_dict=return_dict,
                 **kwargs,
             )
 
         batch_size = input_ids.shape[0]
         if attention_mask is not None:
             # concat prompt attention mask
-            prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(self.device)
+            prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(attention_mask.device)
             attention_mask = torch.cat((prefix_attention_mask, attention_mask), dim=1)
         if kwargs.get("position_ids", None) is not None:
             warnings.warn("Position ids are not supported for parameter efficient tuning. Ignoring position ids.")
             kwargs["position_ids"] = None
         kwargs.update(
             {
                 "attention_mask": attention_mask,
@@ -533,15 +764,15 @@
 
         if peft_config.peft_type == PeftType.PREFIX_TUNING:
             return self._prefix_tuning_forward(input_ids=input_ids, **kwargs)
         else:
             if kwargs.get("token_type_ids", None) is not None:
                 kwargs["token_type_ids"] = torch.cat(
                     (
-                        torch.zeros(batch_size, peft_config.num_virtual_tokens).to(self.device),
+                        torch.zeros(batch_size, peft_config.num_virtual_tokens).to(self.word_embeddings.weight.device),
                         kwargs["token_type_ids"],
                     ),
                     dim=1,
                 ).long()
             if inputs_embeds is None:
                 inputs_embeds = self.word_embeddings(input_ids)
             prompts = self.get_prompt(batch_size=batch_size)
@@ -671,29 +902,42 @@
         output_attentions=None,
         output_hidden_states=None,
         return_dict=None,
         **kwargs,
     ):
         peft_config = self.active_peft_config
         if not isinstance(peft_config, PromptLearningConfig):
+            if self.base_model.config.model_type == "mpt":
+                if inputs_embeds is not None:
+                    raise AssertionError("forward in MPTForCausalLM does not support inputs_embeds")
+                return self.base_model(
+                    input_ids=input_ids,
+                    attention_mask=attention_mask,
+                    labels=labels,
+                    output_attentions=output_attentions,
+                    output_hidden_states=output_hidden_states,
+                    return_dict=return_dict,
+                    **kwargs,
+                )
+
             return self.base_model(
                 input_ids=input_ids,
                 attention_mask=attention_mask,
                 inputs_embeds=inputs_embeds,
                 labels=labels,
                 output_attentions=output_attentions,
                 output_hidden_states=output_hidden_states,
                 return_dict=return_dict,
                 **kwargs,
             )
 
         batch_size = input_ids.shape[0]
         if attention_mask is not None:
             # concat prompt attention mask
-            prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(self.device)
+            prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(attention_mask.device)
             attention_mask = torch.cat((prefix_attention_mask, attention_mask), dim=1)
 
         if kwargs.get("position_ids", None) is not None:
             warnings.warn("Position ids are not supported for parameter efficient tuning. Ignoring position ids.")
             kwargs["position_ids"] = None
         if kwargs.get("token_type_ids", None) is not None:
             warnings.warn("Token type ids are not supported for parameter efficient tuning. Ignoring token type ids")
@@ -712,92 +956,60 @@
             past_key_values = self.get_prompt(batch_size)
             return self.base_model(input_ids=input_ids, past_key_values=past_key_values, **kwargs)
         else:
             if inputs_embeds is None:
                 inputs_embeds = self.word_embeddings(input_ids)
             # concat prompt labels
             if labels is not None:
-                prefix_labels = torch.full((batch_size, peft_config.num_virtual_tokens), -100).to(self.device)
+                prefix_labels = torch.full((batch_size, peft_config.num_virtual_tokens), -100).to(labels.device)
                 kwargs["labels"] = torch.cat((prefix_labels, labels), dim=1)
             prompts = self.get_prompt(batch_size=batch_size)
             prompts = prompts.to(inputs_embeds.dtype)
             inputs_embeds = torch.cat((prompts, inputs_embeds), dim=1)
             return self.base_model(inputs_embeds=inputs_embeds, **kwargs)
 
     def generate(self, **kwargs):
-        peft_config = self.active_peft_config
         self.base_model.prepare_inputs_for_generation = self.prepare_inputs_for_generation
+        if hasattr(self.base_model, "model"):
+            self.base_model.model.generation_config = self.generation_config
+        else:
+            self.base_model.generation_config = self.generation_config
         try:
-            if not isinstance(peft_config, PromptLearningConfig):
-                outputs = self.base_model.generate(**kwargs)
-            else:
-                if "input_ids" not in kwargs:
-                    raise ValueError("input_ids must be provided for Peft model generation")
-                # For gpt2 models, we construct postion_ids on the fly by using attention mask, and position ids need to match input_shape.
-                # for prefix tuning, input shape is determined using `input_ids`. Thus we should not expand 'attention_mask' here
-                # for prompt tuning input_ids is not passed but a concatenated input_embeds is passed. Thus attention_mask needs to be of same size of num_virtual_tokens + input_ids
-                if kwargs.get("attention_mask", None) is not None and peft_config.peft_type in [
-                    PeftType.PROMPT_TUNING,
-                    PeftType.P_TUNING,
-                ]:
-                    # concat prompt attention mask
-                    prefix_attention_mask = torch.ones(
-                        kwargs["input_ids"].shape[0], peft_config.num_virtual_tokens
-                    ).to(kwargs["input_ids"].device)
-                    kwargs["attention_mask"] = torch.cat((prefix_attention_mask, kwargs["attention_mask"]), dim=1)
-
-                if kwargs.get("position_ids", None) is not None:
-                    warnings.warn(
-                        "Position ids are not supported for parameter efficient tuning. Ignoring position ids."
-                    )
-                    kwargs["position_ids"] = None
-                if kwargs.get("token_type_ids", None) is not None:
-                    warnings.warn(
-                        "Token type ids are not supported for parameter efficient tuning. Ignoring token type ids"
-                    )
-                    kwargs["token_type_ids"] = None
-
-                outputs = self.base_model.generate(**kwargs)
+            outputs = self.base_model.generate(**kwargs)
         except:
             self.base_model.prepare_inputs_for_generation = self.base_model_prepare_inputs_for_generation
             raise
         else:
             self.base_model.prepare_inputs_for_generation = self.base_model_prepare_inputs_for_generation
             return outputs
 
     def prepare_inputs_for_generation(self, *args, **kwargs):
         peft_config = self.active_peft_config
         model_kwargs = self.base_model_prepare_inputs_for_generation(*args, **kwargs)
         if isinstance(peft_config, PromptLearningConfig):
-            if peft_config.peft_type == PeftType.PREFIX_TUNING:
+            if model_kwargs.get("attention_mask", None) is not None:
                 prefix_attention_mask = torch.ones(
                     model_kwargs["input_ids"].shape[0], peft_config.num_virtual_tokens
                 ).to(model_kwargs["input_ids"].device)
                 model_kwargs["attention_mask"] = torch.cat(
                     (prefix_attention_mask, model_kwargs["attention_mask"]), dim=1
                 )
 
-            if model_kwargs["past_key_values"] is None and peft_config.peft_type == PeftType.PREFIX_TUNING:
-                past_key_values = self.get_prompt(batch_size=model_kwargs["input_ids"].shape[0])
+            if model_kwargs.get("position_ids", None) is not None:
+                warnings.warn("Position ids are not supported for parameter efficient tuning. Ignoring position ids.")
+                model_kwargs["position_ids"] = None
 
-                if self.base_model_torch_dtype is not None:
-                    # handle the case for Bloom where it outputs tuple of tuples
-                    if isinstance(past_key_values[0], tuple):
-                        past_key_values = tuple(
-                            tuple(
-                                past_key_value.to(self.base_model_torch_dtype)
-                                for past_key_value in past_key_value_tuple
-                            )
-                            for past_key_value_tuple in past_key_values
-                        )
-                    else:
-                        past_key_values = tuple(
-                            past_key_value.to(self.base_model_torch_dtype) for past_key_value in past_key_values
-                        )
+            if kwargs.get("token_type_ids", None) is not None:
+                warnings.warn(
+                    "Token type ids are not supported for parameter efficient tuning. Ignoring token type ids"
+                )
+                kwargs["token_type_ids"] = None
 
+            if model_kwargs["past_key_values"] is None and peft_config.peft_type == PeftType.PREFIX_TUNING:
+                past_key_values = self.get_prompt(batch_size=model_kwargs["input_ids"].shape[0])
                 model_kwargs["past_key_values"] = past_key_values
             else:
                 if model_kwargs["past_key_values"] is None:
                     inputs_embeds = self.word_embeddings(model_kwargs["input_ids"])
                     prompts = self.get_prompt(batch_size=model_kwargs["input_ids"].shape[0])
                     prompts = prompts.to(inputs_embeds.dtype)
                     model_kwargs["inputs_embeds"] = torch.cat((prompts, inputs_embeds), dim=1)
@@ -825,15 +1037,14 @@
         ...     "peft_type": "LORA",
         ...     "task_type": "SEQ_2_SEQ_LM",
         ...     "inference_mode": False,
         ...     "r": 8,
         ...     "target_modules": ["q", "v"],
         ...     "lora_alpha": 32,
         ...     "lora_dropout": 0.1,
-        ...     "merge_weights": False,
         ...     "fan_in_fan_out": False,
         ...     "enable_lora": None,
         ...     "bias": "none",
         ... }
 
         >>> peft_config = get_peft_config(config)
         >>> model = AutoModelForSeq2SeqLM.from_pretrained("t5-base")
@@ -879,15 +1090,17 @@
                 return_dict=return_dict,
                 **kwargs,
             )
 
         batch_size = input_ids.shape[0]
         if decoder_attention_mask is not None:
             # concat prompt attention mask
-            prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(self.device)
+            prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(
+                decoder_attention_mask.device
+            )
             decoder_attention_mask = torch.cat((prefix_attention_mask, decoder_attention_mask), dim=1)
 
         if kwargs.get("position_ids", None) is not None:
             warnings.warn("Position ids are not supported for parameter efficient tuning. Ignoring position ids.")
             kwargs["position_ids"] = None
         if kwargs.get("token_type_ids", None) is not None:
             warnings.warn("Token type ids are not supported for parameter efficient tuning. Ignoring token type ids")
@@ -902,35 +1115,62 @@
                 "return_dict": return_dict,
             }
         )
 
         if peft_config.peft_type == PeftType.PREFIX_TUNING:
             past_key_values = self.get_prompt(batch_size)
             return self.base_model(
-                input_ids=input_ids, decoder_input_ids=decoder_input_ids, past_key_values=past_key_values, **kwargs
+                input_ids=input_ids,
+                decoder_input_ids=decoder_input_ids,
+                decoder_inputs_embeds=decoder_inputs_embeds,
+                past_key_values=past_key_values,
+                **kwargs,
+            )
+        elif peft_config.peft_type in [PeftType.PROMPT_TUNING, PeftType.P_TUNING]:
+            if inputs_embeds is None:
+                inputs_embeds = self.word_embeddings(input_ids)
+
+            if attention_mask is not None:
+                # concat prompt attention mask
+                prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(
+                    attention_mask.device
+                )
+                kwargs["attention_mask"] = torch.cat((prefix_attention_mask, attention_mask), dim=1)
+
+            prompts = self.get_prompt(batch_size=batch_size)
+            prompts = prompts.to(inputs_embeds.dtype)
+            inputs_embeds = torch.cat((prompts[:, : peft_config.num_virtual_tokens], inputs_embeds), dim=1)
+
+            return self.base_model(
+                inputs_embeds=inputs_embeds,
+                decoder_input_ids=decoder_input_ids,
+                decoder_inputs_embeds=decoder_inputs_embeds,
+                **kwargs,
             )
         else:
             if inputs_embeds is None:
                 inputs_embeds = self.word_embeddings(input_ids)
             if decoder_inputs_embeds is None and decoder_input_ids is None:
                 decoder_input_ids = shift_tokens_right(
                     labels, self.config.pad_token_id, self.config.decoder_start_token_id
                 )
                 decoder_inputs_embeds = self.word_embeddings(decoder_input_ids)
 
             if attention_mask is not None:
                 # concat prompt attention mask
-                prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(self.device)
+                prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(
+                    attention_mask.device
+                )
                 kwargs["attention_mask"] = torch.cat((prefix_attention_mask, attention_mask), dim=1)
             # concat prompt labels
             if labels is not None:
                 if peft_config.num_transformer_submodules == 1:
                     kwargs["labels"] = labels
                 elif peft_config.num_transformer_submodules == 2:
-                    prefix_labels = torch.full((batch_size, peft_config.num_virtual_tokens), -100).to(self.device)
+                    prefix_labels = torch.full((batch_size, peft_config.num_virtual_tokens), -100).to(labels.device)
                     kwargs["labels"] = torch.cat((prefix_labels, labels), dim=1)
             prompts = self.get_prompt(batch_size=batch_size)
             prompts = prompts.to(inputs_embeds.dtype)
             inputs_embeds = torch.cat((prompts[:, : peft_config.num_virtual_tokens], inputs_embeds), dim=1)
             if peft_config.num_transformer_submodules == 1:
                 return self.base_model(inputs_embeds=inputs_embeds, **kwargs)
             elif peft_config.num_transformer_submodules == 2:
@@ -962,14 +1202,39 @@
                     warnings.warn(
                         "Token type ids are not supported for parameter efficient tuning. Ignoring token type ids"
                     )
                     kwargs["token_type_ids"] = None
 
                 if peft_config.peft_type == PeftType.PREFIX_TUNING:
                     outputs = self.base_model.generate(**kwargs)
+                elif peft_config.peft_type in [PeftType.PROMPT_TUNING, PeftType.P_TUNING]:
+                    kwargs = deepcopy(kwargs)
+
+                    if "encoder_outputs" in kwargs:
+                        del kwargs["encoder_ouputs"]
+                        warnings.warn(
+                            "`encoder_outputs` should not be passed to `generate` when using prompt tuning. Ignoring it."
+                        )
+
+                    input_ids = kwargs.pop("input_ids")
+                    inputs_embeds = self.word_embeddings(input_ids)
+                    batch_size = inputs_embeds.shape[0]
+                    prompts = self.get_prompt(batch_size=batch_size)
+                    prompts = prompts.to(inputs_embeds.dtype)
+
+                    inputs_embeds = torch.cat((prompts[:, : peft_config.num_virtual_tokens], inputs_embeds), dim=1)
+                    kwargs["inputs_embeds"] = inputs_embeds
+
+                    if "attention_mask" in kwargs:
+                        prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(
+                            kwargs["attention_mask"].device
+                        )
+                        kwargs["attention_mask"] = torch.cat((prefix_attention_mask, kwargs["attention_mask"]), dim=1)
+
+                    return self.base_model.generate(**kwargs)
                 else:
                     raise NotImplementedError
         except:
             self.base_model.prepare_inputs_for_generation = self.base_model_prepare_inputs_for_generation
             self.base_model._prepare_encoder_decoder_kwargs_for_generation = (
                 self.base_model_prepare_encoder_decoder_kwargs_for_generation
             )
@@ -983,27 +1248,14 @@
 
     def prepare_inputs_for_generation(self, *args, **kwargs):
         peft_config = self.active_peft_config
         model_kwargs = self.base_model_prepare_inputs_for_generation(*args, **kwargs)
         if model_kwargs["past_key_values"] is None and peft_config.peft_type == PeftType.PREFIX_TUNING:
             batch_size = model_kwargs["decoder_input_ids"].shape[0]
             past_key_values = self.get_prompt(batch_size)
-            if self.base_model_torch_dtype is not None:
-                # handle the case for Bloom where it outputs tuple of tuples
-                if isinstance(past_key_values[0], tuple):
-                    past_key_values = tuple(
-                        tuple(
-                            past_key_value.to(self.base_model_torch_dtype) for past_key_value in past_key_value_tuple
-                        )
-                        for past_key_value_tuple in past_key_values
-                    )
-                else:
-                    past_key_values = tuple(
-                        past_key_value.to(self.base_model_torch_dtype) for past_key_value in past_key_values
-                    )
             model_kwargs["past_key_values"] = past_key_values
 
         return model_kwargs
 
 
 class PeftModelForTokenClassification(PeftModel):
     """
@@ -1085,15 +1337,15 @@
                 return_dict=return_dict,
                 **kwargs,
             )
 
         batch_size = input_ids.shape[0]
         if attention_mask is not None:
             # concat prompt attention mask
-            prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(self.device)
+            prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(attention_mask.device)
             attention_mask = torch.cat((prefix_attention_mask, attention_mask), dim=1)
         if kwargs.get("position_ids", None) is not None:
             warnings.warn("Position ids are not supported for parameter efficient tuning. Ignoring position ids.")
             kwargs["position_ids"] = None
         kwargs.update(
             {
                 "attention_mask": attention_mask,
@@ -1106,15 +1358,15 @@
 
         if peft_config.peft_type == PeftType.PREFIX_TUNING:
             return self._prefix_tuning_forward(input_ids=input_ids, **kwargs)
         else:
             if kwargs.get("token_type_ids", None) is not None:
                 kwargs["token_type_ids"] = torch.cat(
                     (
-                        torch.zeros(batch_size, peft_config.num_virtual_tokens).to(self.device),
+                        torch.zeros(batch_size, peft_config.num_virtual_tokens).to(self.word_embeddings.weight.device),
                         kwargs["token_type_ids"],
                     ),
                     dim=1,
                 ).long()
             if inputs_embeds is None:
                 inputs_embeds = self.word_embeddings(input_ids)
             prompts = self.get_prompt(batch_size=batch_size)
@@ -1157,22 +1409,306 @@
             outputs = transformer_backbone_name(**kwargs)
             sequence_output = outputs[0]
             if "dropout" in [name for name, _ in list(self.base_model.named_children())]:
                 sequence_output = self.base_model.dropout(sequence_output)
             logits = self.base_model.get_submodule(self.cls_layer_name)(sequence_output)
 
             loss = None
-            loss = None
             if labels is not None:
                 loss_fct = CrossEntropyLoss()
                 loss = loss_fct(logits.view(-1, self.num_labels), labels.view(-1))
 
             if not return_dict:
                 output = (logits,) + outputs[2:]
                 return ((loss,) + output) if loss is not None else output
 
             return TokenClassifierOutput(
                 loss=loss,
                 logits=logits,
                 hidden_states=outputs.hidden_states,
                 attentions=outputs.attentions,
             )
+
+
+class PeftModelForQuestionAnswering(PeftModel):
+    """
+    Peft model for extractive question answering.
+
+    Args:
+        model ([`~transformers.PreTrainedModel`]): Base transformer model.
+        peft_config ([`PeftConfig`]): Peft config.
+
+    **Attributes**:
+        - **config** ([`~transformers.PretrainedConfig`]) -- The configuration object of the base model.
+        - **cls_layer_name** (`str`) -- The name of the classification layer.
+
+    Example:
+
+        ```py
+        >>> from transformers import AutoModelForQuestionAnswering
+        >>> from peft import PeftModelForQuestionAnswering, get_peft_config
+
+        >>> config = {
+        ...     "peft_type": "LORA",
+        ...     "task_type": "QUESTION_ANS",
+        ...     "inference_mode": False,
+        ...     "r": 16,
+        ...     "target_modules": ["query", "value"],
+        ...     "lora_alpha": 32,
+        ...     "lora_dropout": 0.05,
+        ...     "fan_in_fan_out": False,
+        ...     "bias": "none",
+        ... }
+
+        >>> peft_config = get_peft_config(config)
+        >>> model = AutoModelForQuestionAnswering.from_pretrained("bert-base-cased")
+        >>> peft_model = PeftModelForQuestionAnswering(model, peft_config)
+        >>> peft_model.print_trainable_parameters()
+        trainable params: 592900 || all params: 108312580 || trainable%: 0.5473971721475013
+        ```
+    """
+
+    def __init__(self, model, peft_config: PeftConfig = None, adapter_name="default"):
+        super().__init__(model, peft_config, adapter_name)
+        if self.modules_to_save is None:
+            self.modules_to_save = {"qa_outputs"}
+        else:
+            self.modules_to_save.update({"qa_outputs"})
+
+        for name, _ in self.base_model.named_children():
+            if any(module_name in name for module_name in self.modules_to_save):
+                self.cls_layer_name = name
+                break
+
+        # to make sure classifier layer is trainable
+        _set_trainable(self, adapter_name)
+
+    def forward(
+        self,
+        input_ids=None,
+        attention_mask=None,
+        token_type_ids=None,
+        position_ids=None,
+        inputs_embeds=None,
+        start_positions=None,
+        end_positions=None,
+        output_attentions=None,
+        output_hidden_states=None,
+        return_dict=None,
+        **kwargs,
+    ):
+        peft_config = self.active_peft_config
+        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+
+        if not isinstance(peft_config, PromptLearningConfig):
+            return self.base_model(
+                input_ids=input_ids,
+                attention_mask=attention_mask,
+                inputs_embeds=inputs_embeds,
+                start_positions=start_positions,
+                end_positions=end_positions,
+                output_attentions=output_attentions,
+                output_hidden_states=output_hidden_states,
+                return_dict=return_dict,
+                **kwargs,
+            )
+
+        batch_size = input_ids.shape[0]
+        if attention_mask is not None:
+            # concat prompt attention mask
+            prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(attention_mask.device)
+            attention_mask = torch.cat((prefix_attention_mask, attention_mask), dim=1)
+        if kwargs.get("position_ids", None) is not None:
+            warnings.warn("Position ids are not supported for parameter efficient tuning. Ignoring position ids.")
+            kwargs["position_ids"] = None
+        kwargs.update(
+            {
+                "attention_mask": attention_mask,
+                "start_positions": start_positions,
+                "end_positions": end_positions,
+                "output_attentions": output_attentions,
+                "output_hidden_states": output_hidden_states,
+                "return_dict": return_dict,
+            }
+        )
+
+        if peft_config.peft_type == PeftType.PREFIX_TUNING:
+            return self._prefix_tuning_forward(input_ids=input_ids, **kwargs)
+        else:
+            if kwargs.get("token_type_ids", None) is not None:
+                kwargs["token_type_ids"] = torch.cat(
+                    (
+                        torch.zeros(batch_size, peft_config.num_virtual_tokens).to(self.word_embeddings.weight.device),
+                        kwargs["token_type_ids"],
+                    ),
+                    dim=1,
+                ).long()
+            if inputs_embeds is None:
+                inputs_embeds = self.word_embeddings(input_ids)
+            prompts = self.get_prompt(batch_size=batch_size)
+            prompts = prompts.to(inputs_embeds.dtype)
+            inputs_embeds = torch.cat((prompts, inputs_embeds), dim=1)
+            return self.base_model(inputs_embeds=inputs_embeds, **kwargs)
+
+    def _prefix_tuning_forward(
+        self,
+        input_ids=None,
+        attention_mask=None,
+        inputs_embeds=None,
+        start_positions=None,
+        end_positions=None,
+        output_attentions=None,
+        output_hidden_states=None,
+        return_dict=None,
+        **kwargs,
+    ):
+        batch_size = input_ids.shape[0]
+        past_key_values = self.get_prompt(batch_size)
+        fwd_params = list(inspect.signature(self.base_model.forward).parameters.keys())
+        kwargs.update(
+            {
+                "input_ids": input_ids,
+                "attention_mask": attention_mask,
+                "inputs_embeds": inputs_embeds,
+                "output_attentions": output_attentions,
+                "output_hidden_states": output_hidden_states,
+                "return_dict": return_dict,
+                "past_key_values": past_key_values,
+            }
+        )
+        if "past_key_values" in fwd_params:
+            return self.base_model(start_positions=start_positions, end_positions=end_positions, **kwargs)
+        else:
+            transformer_backbone_name = self.base_model.get_submodule(self.transformer_backbone_name)
+            fwd_params = list(inspect.signature(transformer_backbone_name.forward).parameters.keys())
+            if "past_key_values" not in fwd_params:
+                raise ValueError("Model does not support past key values which are required for prefix tuning.")
+            outputs = transformer_backbone_name(**kwargs)
+            sequence_output = outputs[0]
+            if "dropout" in [name for name, _ in list(self.base_model.named_children())]:
+                sequence_output = self.base_model.dropout(sequence_output)
+            logits = self.base_model.get_submodule(self.cls_layer_name)(sequence_output)
+            start_logits, end_logits = logits.split(1, dim=-1)
+            start_logits = start_logits.squeeze(-1).contiguous()
+            end_logits = end_logits.squeeze(-1).contiguous()
+
+            total_loss = None
+            if start_positions is not None and end_positions is not None:
+                # If we are on multi-GPU, split add a dimension
+                if len(start_positions.size()) > 1:
+                    start_positions = start_positions.squeeze(-1)
+                if len(end_positions.size()) > 1:
+                    end_positions = end_positions.squeeze(-1)
+                # sometimes the start/end positions are outside our model inputs, we ignore these terms
+                ignored_index = start_logits.size(1)
+                start_positions = start_positions.clamp(0, ignored_index)
+                end_positions = end_positions.clamp(0, ignored_index)
+
+                loss_fct = CrossEntropyLoss(ignore_index=ignored_index)
+                start_loss = loss_fct(start_logits, start_positions)
+                end_loss = loss_fct(end_logits, end_positions)
+                total_loss = (start_loss + end_loss) / 2
+
+            if not return_dict:
+                output = (start_logits, end_logits) + outputs[2:]
+                return ((total_loss,) + output) if total_loss is not None else output
+
+            return QuestionAnsweringModelOutput(
+                loss=total_loss,
+                start_logits=start_logits,
+                end_logits=end_logits,
+                hidden_states=outputs.hidden_states,
+                attentions=outputs.attentions,
+            )
+
+
+class PeftModelForFeatureExtraction(PeftModel):
+    """
+    Peft model for extracting features/embeddings from transformer models
+
+    Args:
+        model ([`~transformers.PreTrainedModel`]): Base transformer model.
+        peft_config ([`PeftConfig`]): Peft config.
+
+    **Attributes**:
+        - **config** ([`~transformers.PretrainedConfig`]) -- The configuration object of the base model.
+
+    Example:
+
+        ```py
+        >>> from transformers import AutoModel
+        >>> from peft import PeftModelForFeatureExtraction, get_peft_config
+
+        >>> config = {
+        ...     "peft_type": "LORA",
+        ...     "task_type": "FEATURE_EXTRACTION",
+        ...     "inference_mode": False,
+        ...     "r": 16,
+        ...     "target_modules": ["query", "value"],
+        ...     "lora_alpha": 32,
+        ...     "lora_dropout": 0.05,
+        ...     "fan_in_fan_out": False,
+        ...     "bias": "none",
+        ... }
+        >>> peft_config = get_peft_config(config)
+        >>> model = AutoModel.from_pretrained("bert-base-cased")
+        >>> peft_model = PeftModelForFeatureExtraction(model, peft_config)
+        >>> peft_model.print_trainable_parameters()
+        ```
+    """
+
+    def __init__(self, model, peft_config: PeftConfig = None, adapter_name="default"):
+        super().__init__(model, peft_config, adapter_name)
+
+    def forward(
+        self,
+        input_ids=None,
+        attention_mask=None,
+        inputs_embeds=None,
+        output_attentions=None,
+        output_hidden_states=None,
+        return_dict=None,
+        **kwargs,
+    ):
+        peft_config = self.active_peft_config
+        if not isinstance(peft_config, PromptLearningConfig):
+            return self.base_model(
+                input_ids=input_ids,
+                attention_mask=attention_mask,
+                inputs_embeds=inputs_embeds,
+                output_attentions=output_attentions,
+                output_hidden_states=output_hidden_states,
+                return_dict=return_dict,
+                **kwargs,
+            )
+
+        batch_size = input_ids.shape[0]
+        if attention_mask is not None:
+            # concat prompt attention mask
+            prefix_attention_mask = torch.ones(batch_size, peft_config.num_virtual_tokens).to(attention_mask.device)
+            attention_mask = torch.cat((prefix_attention_mask, attention_mask), dim=1)
+
+        if kwargs.get("position_ids", None) is not None:
+            warnings.warn("Position ids are not supported for parameter efficient tuning. Ignoring position ids.")
+            kwargs["position_ids"] = None
+        if kwargs.get("token_type_ids", None) is not None:
+            warnings.warn("Token type ids are not supported for parameter efficient tuning. Ignoring token type ids")
+            kwargs["token_type_ids"] = None
+        kwargs.update(
+            {
+                "attention_mask": attention_mask,
+                "output_attentions": output_attentions,
+                "output_hidden_states": output_hidden_states,
+                "return_dict": return_dict,
+            }
+        )
+
+        if peft_config.peft_type == PeftType.PREFIX_TUNING:
+            past_key_values = self.get_prompt(batch_size)
+            return self.base_model(input_ids=input_ids, past_key_values=past_key_values, **kwargs)
+        else:
+            if inputs_embeds is None:
+                inputs_embeds = self.word_embeddings(input_ids)
+            prompts = self.get_prompt(batch_size=batch_size)
+            prompts = prompts.to(inputs_embeds.dtype)
+            inputs_embeds = torch.cat((prompts, inputs_embeds), dim=1)
+            return self.base_model(inputs_embeds=inputs_embeds, **kwargs)
```

### Comparing `peft-0.3.0/src/peft/tuners/__init__.py` & `peft-0.4.0/src/peft/tuners/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,11 +15,12 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .adaption_prompt import AdaptionPromptConfig, AdaptionPromptModel
 from .lora import LoraConfig, LoraModel
+from .ia3 import IA3Config, IA3Model
 from .adalora import AdaLoraConfig, AdaLoraModel
 from .p_tuning import PromptEncoder, PromptEncoderConfig, PromptEncoderReparameterizationType
 from .prefix_tuning import PrefixEncoder, PrefixTuningConfig
 from .prompt_tuning import PromptEmbedding, PromptTuningConfig, PromptTuningInit
```

### Comparing `peft-0.3.0/src/peft/tuners/adalora.py` & `peft-0.4.0/src/peft/tuners/adalora.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import importlib
 import re
 import warnings
 from dataclasses import dataclass, field
 from typing import Optional
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from transformers.pytorch_utils import Conv1D
 
+from ..import_utils import is_bnb_4bit_available, is_bnb_available
 from ..utils import (
     TRANSFORMERS_MODELS_TO_ADALORA_TARGET_MODULES_MAPPING,
     PeftType,
     _freeze_adapter,
     _get_submodules,
     transpose,
 )
@@ -20,18 +20,14 @@
     LoraConfig,
     LoraLayer,
     LoraModel,
     mark_only_lora_as_trainable,
 )
 
 
-def is_bnb_available():
-    return importlib.util.find_spec("bitsandbytes") is not None
-
-
 if is_bnb_available():
     import bitsandbytes as bnb
 
 
 @dataclass
 class AdaLoraConfig(LoraConfig):
     """
@@ -124,15 +120,17 @@
         else:
             self.trainable_adapter_name = adapter_name
             self.rankallocator = RankAllocator(self.model, self.peft_config[adapter_name], self.trainable_adapter_name)
 
     def _find_and_replace(self, adapter_name):
         lora_config = self.peft_config[adapter_name]
         loaded_in_8bit = getattr(self.model, "is_loaded_in_8bit", False)
-        if loaded_in_8bit and not is_bnb_available():
+        loaded_in_4bit = getattr(self.model, "is_loaded_in_4bit", False)
+
+        if (loaded_in_8bit or loaded_in_4bit) and not is_bnb_available():
             raise ImportError(
                 "To use Lora with 8-bit quantization, please install the `bitsandbytes` package. "
                 "You can install it with `pip install bitsandbytes`."
             )
         is_target_modules_in_base_model = False
         kwargs = {
             "r": lora_config.init_r,
@@ -169,14 +167,26 @@
                                 "threshold": target.state.threshold,
                                 "index": target.index,
                             }
                         )
                         new_module = SVDLinear8bitLt(
                             adapter_name, target.in_features, target.out_features, bias=bias, **kwargs
                         )
+                    elif loaded_in_4bit and is_bnb_4bit_available() and isinstance(target, bnb.nn.Linear4bit):
+                        fourbit_kwargs = kwargs.copy()
+                        fourbit_kwargs.update(
+                            {
+                                "compute_dtype": target.compute_dtype,
+                                "compress_statistics": target.weight.compress_statistics,
+                                "quant_type": target.weight.quant_type,
+                            }
+                        )
+                        new_module = SVDLinear4bit(
+                            adapter_name, target.in_features, target.out_features, bias=bias, **fourbit_kwargs
+                        )
                     else:
                         if isinstance(target, torch.nn.Linear):
                             in_features, out_features = target.in_features, target.out_features
                             if kwargs["fan_in_fan_out"]:
                                 warnings.warn(
                                     "fan_in_fan_out is set to True but the target module is `torch.nn.Linear`. "
                                     "Setting fan_in_fan_out to False."
@@ -226,15 +236,18 @@
             for n, p in self.model.named_parameters():
                 if ("lora_A" in n or "lora_B" in n) and self.trainable_adapter_name in n:
                     para_cov = p @ p.T if "lora_A" in n else p.T @ p
                     I = torch.eye(*para_cov.size(), out=torch.empty_like(para_cov))
                     I.requires_grad = False
                     num_param += 1
                     regu_loss += torch.norm(para_cov - I, p="fro")
-            regu_loss = regu_loss / num_param
+            if num_param > 0:
+                regu_loss = regu_loss / num_param
+            else:
+                regu_loss = 0
             outputs.loss += orth_reg_weight * regu_loss
         return outputs
 
     def resize_modules_by_rank_pattern(self, rank_pattern, adapter_name):
         lora_config = self.peft_config[adapter_name]
         for name, rank_idx in rank_pattern.items():
             if isinstance(rank_idx, list):
@@ -307,16 +320,14 @@
     def _prepare_adalora_config(peft_config, model_config):
         if peft_config.target_modules is None:
             if model_config["model_type"] not in TRANSFORMERS_MODELS_TO_ADALORA_TARGET_MODULES_MAPPING:
                 raise ValueError("Please specify `target_modules` in `peft_config`")
             peft_config.target_modules = TRANSFORMERS_MODELS_TO_ADALORA_TARGET_MODULES_MAPPING[
                 model_config["model_type"]
             ]
-        if peft_config.inference_mode:
-            peft_config.merge_weights = True
         return peft_config
 
 
 class AdaLoraLayer(LoraLayer):
     def __init__(
         self,
         in_features: int,
@@ -505,15 +516,80 @@
                             self.lora_dropout[self.active_adapter](x)
                             @ (self.lora_A[self.active_adapter] * self.lora_E[self.active_adapter]).T
                             @ self.lora_B[self.active_adapter].T
                         )
                         * self.scaling[self.active_adapter]
                         / (self.ranknum[self.active_adapter] + 1e-5)
                     )
-                result += output
+                result = result + output
+            return result
+
+
+if is_bnb_4bit_available():
+
+    class SVDLinear4bit(bnb.nn.Linear4bit, AdaLoraLayer):
+        # Low-rank matrix for SVD-based adaptation
+        def __init__(
+            self,
+            adapter_name,
+            in_features,
+            out_features,
+            r: int = 0,
+            lora_alpha: int = 1,
+            lora_dropout: float = 0.0,
+            **kwargs,
+        ):
+            bnb.nn.Linear4bit.__init__(
+                self,
+                in_features,
+                out_features,
+                bias=kwargs.get("bias", True),
+                compute_dtype=kwargs.get("compute_dtype", torch.float32),
+                compress_statistics=kwargs.get("compress_statistics", True),
+                quant_type=kwargs.get("quant_type", "nf4"),
+            )
+            AdaLoraLayer.__init__(self, in_features=in_features, out_features=out_features)
+            # Freezing the pre-trained weight matrix
+            self.weight.requires_grad = False
+
+            init_lora_weights = kwargs.pop("init_lora_weights", True)
+            self.update_layer(adapter_name, r, lora_alpha, lora_dropout, init_lora_weights)
+            self.active_adapter = adapter_name
+
+        def forward(self, x: torch.Tensor):
+            result = super().forward(x)
+
+            if self.disable_adapters or self.active_adapter not in self.lora_A.keys():
+                return result
+            elif self.r[self.active_adapter] > 0:
+                if not torch.is_autocast_enabled():
+                    expected_dtype = result.dtype
+
+                    if x.dtype != torch.float32:
+                        x = x.float()
+                    output = (
+                        (
+                            self.lora_dropout[self.active_adapter](x)
+                            @ (self.lora_A[self.active_adapter] * self.lora_E[self.active_adapter]).T
+                            @ self.lora_B[self.active_adapter].T
+                        ).to(expected_dtype)
+                        * self.scaling[self.active_adapter]
+                        / (self.ranknum[self.active_adapter] + 1e-5)
+                    )
+                else:
+                    output = (
+                        (
+                            self.lora_dropout[self.active_adapter](x)
+                            @ (self.lora_A[self.active_adapter] * self.lora_E[self.active_adapter]).T
+                            @ self.lora_B[self.active_adapter].T
+                        )
+                        * self.scaling[self.active_adapter]
+                        / (self.ranknum[self.active_adapter] + 1e-5)
+                    )
+                result = result + output
             return result
 
 
 class RankAllocator(object):
     """
     The RankAllocator for AdaLoraModel. Paper: https://openreview.net/pdf?id=lq62uWRJjiY
```

### Comparing `peft-0.3.0/src/peft/tuners/adaption_prompt.py` & `peft-0.4.0/src/peft/tuners/adaption_prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,19 +289,22 @@
         self.adapter_len = adapter_len
         # Assume all parameters of the attention model we are wrapping are on the same device.
         device = next(model.parameters()).device
         # Don't think this was specified in the paper, but we follow the official repo which used an Embedding
         # which initializes the tokens with standard normal values.
         # https://github.com/ZrrSkywalker/LLaMA-Adapter/blob/41c3546fe1997ab8a65809dc8d8f9252b19d9faf/llama/model.py#L234
         # (bsz, adapter_len, hidden_size)
+        target_dtype = (
+            model.q_proj.weight.dtype if model.q_proj.weight.dtype not in [torch.int8, torch.uint8] else torch.float32
+        )
         self.adaption_prompt = nn.Parameter(
-            torch.empty(1, adapter_len, self.model.hidden_size, device=device).normal_()
+            torch.empty(1, adapter_len, self.model.hidden_size, device=device, dtype=target_dtype).normal_()
         )
         # Initialize the gate to 0 as this is "zero-init".
-        self.adaption_gate = nn.Parameter(torch.zeros(1, device=device))
+        self.adaption_gate = nn.Parameter(torch.zeros(1, device=device, dtype=target_dtype))
 
     def forward(self, **kwargs):
         """
         Forward pass for the adapter which wraps the original LlamaAttention module.
 
         "Official" paper implementation:
         https://github.com/ZrrSkywalker/LLaMA-Adapter/blob/41c3546fe1997ab8a65809dc8d8f9252b19d9faf/llama/model.py#L141
@@ -339,21 +342,27 @@
         )
 
         # Recompute query states.
         compute_query_states = TRANSFORMERS_MODEL_CONFIG[self.model_type].compute_query_states
         # (bsz, num_heads, q_len, head_dim)
         query_states = compute_query_states(model=self.model, **kwargs)
 
+        previous_dtype = query_states.dtype
         # (bsz, num_heads, q_len, adapter_len)
-        scores = torch.matmul(query_states, adapter_k.transpose(2, 3)) / math.sqrt(self.model.head_dim)
+        scores = torch.matmul(query_states, adapter_k.transpose(2, 3).to(previous_dtype)) / math.sqrt(
+            self.model.head_dim
+        )
         # Upcast attention to fp32
         # (bsz, num_heads, q_len, adapter_len)
-        scores = self.adaption_gate * F.softmax(scores, dim=-1, dtype=torch.float32).to(query_states.dtype)
+        scores = self.adaption_gate * F.softmax(scores, dim=-1, dtype=torch.float32).to(previous_dtype)
         # (bsz, q_len, num_heads * head_dim)
         adapter_output = torch.matmul(scores, adapter_v).transpose(1, 2).reshape(bsz, q_len, -1)
         # (bsz, q_len, hidden_size)
         if o_proj_layer is not None:
             adapter_output = getattr(self.model, o_proj_layer)(adapter_output)
 
         # Add adaption prompt output to original output.
         output = output + adapter_output
+
+        # Restore original dtype.
+        output = output.to(previous_dtype)
         return output, None, past_key_value
```

### Comparing `peft-0.3.0/src/peft/tuners/lora.py` & `peft-0.4.0/src/peft/tuners/ia3.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,272 +8,283 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import math
 import re
 import warnings
 from dataclasses import asdict, dataclass, field
 from enum import Enum
 from typing import List, Optional, Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from transformers.pytorch_utils import Conv1D
 
 from ..import_utils import is_bnb_available
 from ..utils import (
-    TRANSFORMERS_MODELS_TO_LORA_TARGET_MODULES_MAPPING,
+    TRANSFORMERS_MODELS_TO_IA3_FEEDFORWARD_MODULES_MAPPING,
+    TRANSFORMERS_MODELS_TO_IA3_TARGET_MODULES_MAPPING,
     ModulesToSaveWrapper,
     PeftConfig,
     PeftType,
     _freeze_adapter,
     _get_submodules,
     transpose,
 )
 
 
 if is_bnb_available():
     import bitsandbytes as bnb
 
 
 @dataclass
-class LoraConfig(PeftConfig):
+class IA3Config(PeftConfig):
     """
-    This is the configuration class to store the configuration of a [`LoraModel`].
+    This is the configuration class to store the configuration of a [`IA3Model`].
 
     Args:
-        r (`int`): Lora attention dimension.
-        target_modules (`Union[List[str],str]`): The names of the modules to apply Lora to.
-        lora_alpha (`float`): The alpha parameter for Lora scaling.
-        lora_dropout (`float`): The dropout probability for Lora layers.
+        target_modules (`Union[List[str],str]`): The names of the modules to apply (IA)^3 to.
+        feedforward_modules (`Union[List[str],str]`): The names of the modules to be treated as feedforward modules
+        as in the original paper.
         fan_in_fan_out (`bool`): Set this to True if the layer to replace stores weight like (fan_in, fan_out).
         For example, gpt-2 uses `Conv1D` which stores weights like (fan_in, fan_out) and hence this should be set to `True`.:
-        bias (`str`): Bias type for Lora. Can be 'none', 'all' or 'lora_only'
-        modules_to_save (`List[str]`):List of modules apart from LoRA layers to be set as trainable
+        modules_to_save (`List[str]`):List of modules apart from (IA)^3 layers to be set as trainable
             and saved in the final checkpoint.
+        init_ia3_weights (`bool`): Whether to initialize the vectors in the (IA)^3 layers, defaults to `True`.
     """
 
-    r: int = field(default=8, metadata={"help": "Lora attention dimension"})
     target_modules: Optional[Union[List[str], str]] = field(
         default=None,
         metadata={
-            "help": "List of module names or regex expression of the module names to replace with Lora."
+            "help": "List of module names or regex expression of the module names to replace with ia3."
             "For example, ['q', 'v'] or '.*decoder.*(SelfAttention|EncDecAttention).*(q|v)$' "
         },
     )
-    lora_alpha: int = field(default=None, metadata={"help": "Lora alpha"})
-    lora_dropout: float = field(default=None, metadata={"help": "Lora dropout"})
+    feedforward_modules: Optional[Union[List[str], str]] = field(
+        default=None,
+        metadata={
+            "help": "List of module names or a regex expression of module names which are feedforward"
+            "For example, ['output.dense']"
+        },
+    )
     fan_in_fan_out: bool = field(
         default=False,
         metadata={"help": "Set this to True if the layer to replace stores weight like (fan_in, fan_out)"},
     )
-    bias: str = field(default="none", metadata={"help": "Bias type for Lora. Can be 'none', 'all' or 'lora_only'"})
     modules_to_save: Optional[List[str]] = field(
         default=None,
         metadata={
-            "help": "List of modules apart from LoRA layers to be set as trainable and saved in the final checkpoint. "
+            "help": "List of modules apart from (IA)^3 layers to be set as trainable and saved in the final checkpoint. "
             "For example, in Sequence Classification or Token Classification tasks, "
             "the final layer `classifier/score` are randomly initialized and as such need to be trainable and saved."
         },
     )
-    init_lora_weights: bool = field(
+    init_ia3_weights: bool = field(
         default=True,
-        metadata={"help": "Whether to initialize the weights of the Lora layers."},
+        metadata={"help": "Whether to initialize the vectors in the (IA)^3 layers."},
     )
 
     def __post_init__(self):
-        self.peft_type = PeftType.LORA
+        self.peft_type = PeftType.IA3
 
 
-class LoraModel(torch.nn.Module):
+class IA3Model(torch.nn.Module):
     """
-    Creates Low Rank Adapter (Lora) model from a pretrained transformers model.
+    Creates a Infused Adapter by Inhibiting and Amplifying Inner Activations ((IA)^3) model from a pretrained
+    transformers model. The method is described in detail in https://arxiv.org/abs/2205.05638
 
     Args:
         model ([`~transformers.PreTrainedModel`]): The model to be adapted.
-        config ([`LoraConfig`]): The configuration of the Lora model.
+        config ([`IA3Config`]): The configuration of the (IA)^3 model.
 
     Returns:
-        `torch.nn.Module`: The Lora model.
+        `torch.nn.Module`: The (IA)^3 model.
 
     Example:
 
         ```py
-        >>> from transformers import AutoModelForSeq2SeqLM, LoraConfig
-        >>> from peft import LoraModel, LoraConfig
+        >>> from transformers import AutoModelForSeq2SeqLM, ia3Config
+        >>> from peft import IA3Model, IA3Config
 
-        >>> config = LoraConfig(
-        ...     peft_type="LORA",
+        >>> config = IA3Config(
+        ...     peft_type="IA3",
         ...     task_type="SEQ_2_SEQ_LM",
-        ...     r=8,
-        ...     lora_alpha=32,
-        ...     target_modules=["q", "v"],
-        ...     lora_dropout=0.01,
+        ...     target_modules=["k", "v", "w0"],
+        ...     feedforward_modules=["w0"],
         ... )
 
         >>> model = AutoModelForSeq2SeqLM.from_pretrained("t5-base")
-        >>> lora_model = LoraModel(config, model)
-        ```
-
-        ```py
-        >>> import transformers
-        >>> from peft import LoraConfig, PeftModel, get_peft_model, prepare_model_for_int8_training
-
-        >>> target_modules = ["q_proj", "k_proj", "v_proj", "out_proj", "fc_in", "fc_out", "wte"]
-        >>> config = LoraConfig(
-        ...     r=4, lora_alpha=16, target_modules=target_modules, lora_dropout=0.1, bias="none", task_type="CAUSAL_LM"
-        ... )
-
-        >>> model = transformers.GPTJForCausalLM.from_pretrained(
-        ...     "kakaobrain/kogpt",
-        ...     revision="KoGPT6B-ryan1.5b-float16",  # or float32 version: revision=KoGPT6B-ryan1.5b
-        ...     pad_token_id=tokenizer.eos_token_id,
-        ...     use_cache=False,
-        ...     device_map={"": rank},
-        ...     torch_dtype=torch.float16,
-        ...     load_in_8bit=True,
-        ... )
-        >>> model = prepare_model_for_int8_training(model)
-        >>> lora_model = get_peft_model(model, config)
+        >>> ia3_model = IA3Model(config, model)
         ```
 
     **Attributes**:
         - **model** ([`~transformers.PreTrainedModel`]) -- The model to be adapted.
-        - **peft_config** ([`LoraConfig`]): The configuration of the Lora model.
+        - **peft_config** ([`ia3Config`]): The configuration of the (IA)^3 model.
     """
 
     def __init__(self, model, config, adapter_name):
         super().__init__()
         self.model = model
         self.forward = self.model.forward
         self.peft_config = config
         self.add_adapter(adapter_name, self.peft_config[adapter_name])
 
     def add_adapter(self, adapter_name, config=None):
         if config is not None:
             model_config = self.model.config.to_dict() if hasattr(self.model.config, "to_dict") else self.model.config
-            config = self._prepare_lora_config(config, model_config)
+            config = self._prepare_ia3_config(config, model_config)
             self.peft_config[adapter_name] = config
         self._find_and_replace(adapter_name)
-        if len(self.peft_config) > 1 and self.peft_config[adapter_name].bias != "none":
-            raise ValueError(
-                "LoraModel supports only 1 adapter with bias. When using multiple adapters, set bias to 'none' for all adapters."
-            )
-        mark_only_lora_as_trainable(self.model, self.peft_config[adapter_name].bias)
+
+        mark_only_ia3_as_trainable(self.model)
         if self.peft_config[adapter_name].inference_mode:
             _freeze_adapter(self.model, adapter_name)
 
-    def _find_and_replace(self, adapter_name):
-        lora_config = self.peft_config[adapter_name]
+    def _check_quantization_dependency(self):
+        loaded_in_4bit = getattr(self.model, "is_loaded_in_4bit", False)
+        if loaded_in_4bit:
+            raise NotImplementedError(
+                "4-bit quantization is not supported for IA3 yet, 8-bit quantization can be used instead."
+            )
         loaded_in_8bit = getattr(self.model, "is_loaded_in_8bit", False)
         if loaded_in_8bit and not is_bnb_available():
             raise ImportError(
-                "To use Lora with 8-bit quantization, please install the `bitsandbytes` package. "
+                "To use (IA)^3 with 8-bit quantization, please install the `bitsandbytes` package. "
                 "You can install it with `pip install bitsandbytes`."
             )
-        is_target_modules_in_base_model = False
+
+    def _create_new_module(self, ia3_config, adapter_name, target, is_feedforward):
         kwargs = {
-            "r": lora_config.r,
-            "lora_alpha": lora_config.lora_alpha,
-            "lora_dropout": lora_config.lora_dropout,
-            "fan_in_fan_out": lora_config.fan_in_fan_out,
-            "init_lora_weights": lora_config.init_lora_weights,
+            "fan_in_fan_out": ia3_config.fan_in_fan_out,
+            "init_ia3_weights": ia3_config.init_ia3_weights,
         }
+        bias = hasattr(target, "bias") and target.bias is not None
+        loaded_in_8bit = getattr(self.model, "is_loaded_in_8bit", False)
+
+        if loaded_in_8bit and isinstance(target, bnb.nn.Linear8bitLt):
+            eightbit_kwargs = kwargs.copy()
+            eightbit_kwargs.update(
+                {
+                    "has_fp16_weights": target.state.has_fp16_weights,
+                    "memory_efficient_backward": target.state.memory_efficient_backward,
+                    "threshold": target.state.threshold,
+                    "index": target.index,
+                }
+            )
+            new_module = Linear8bitLt(
+                adapter_name,
+                target.in_features,
+                target.out_features,
+                is_feedforward,
+                bias=bias,
+                **eightbit_kwargs,
+            )
+        else:
+            #  Create a new Linear module with (IA)^3 parameters for torch.nn.Linear
+            # or Conv1D modules
+            if isinstance(target, torch.nn.Linear):
+                in_features, out_features = target.in_features, target.out_features
+                if kwargs["fan_in_fan_out"]:
+                    warnings.warn(
+                        "fan_in_fan_out is set to True but the target module is `torch.nn.Linear`. "
+                        "Setting fan_in_fan_out to False."
+                    )
+                    kwargs["fan_in_fan_out"] = ia3_config.fan_in_fan_out = False
+            elif isinstance(target, Conv1D):
+                in_features, out_features = (
+                    target.weight.ds_shape if hasattr(target.weight, "ds_shape") else target.weight.shape
+                )
+                if not kwargs["fan_in_fan_out"]:
+                    warnings.warn(
+                        "fan_in_fan_out is set to False but the target module is `Conv1D`. "
+                        "Setting fan_in_fan_out to True."
+                    )
+                    kwargs["fan_in_fan_out"] = ia3_config.fan_in_fan_out = True
+            else:
+                raise ValueError(
+                    f"Target module {target} is not supported. "
+                    f"Currently, only `torch.nn.Linear` and `Conv1D` are supported."
+                )
+            new_module = Linear(
+                adapter_name, in_features, out_features, is_feedforward=is_feedforward, bias=bias, **kwargs
+            )
+        return new_module
+
+    def _check_target_module_exists(self, ia3_config, key):
+        if isinstance(ia3_config.target_modules, str):
+            target_module_found = re.fullmatch(ia3_config.target_modules, key)
+        else:
+            target_module_found = any(
+                self._is_valid_match(key, target_key) for target_key in ia3_config.target_modules
+            )
+        return target_module_found
+
+    def _find_and_replace(self, adapter_name):
+        ia3_config = self.peft_config[adapter_name]
+        if not ia3_config.feedforward_modules:
+            ia3_config.feedforward_modules = []  # convert to list if None
+        self._check_quantization_dependency()
+        is_target_modules_in_base_model = False
+
         key_list = [key for key, _ in self.model.named_modules()]
         for key in key_list:
-            if isinstance(lora_config.target_modules, str):
-                target_module_found = re.fullmatch(lora_config.target_modules, key)
+            if not self._check_target_module_exists(ia3_config, key):
+                continue
+            # check if target module is in feedforward_modules
+            if isinstance(ia3_config.feedforward_modules, str):
+                is_feedforward = re.fullmatch(ia3_config.feedforward_modules, key)
             else:
-                target_module_found = any(key.endswith(target_key) for target_key in lora_config.target_modules)
-            if target_module_found:
-                if not is_target_modules_in_base_model:
-                    is_target_modules_in_base_model = True
-                parent, target, target_name = _get_submodules(self.model, key)
-                if hasattr(target, "bias"):
-                    bias = target.bias is not None
+                is_feedforward = any(key.endswith(target_key) for target_key in ia3_config.feedforward_modules)
 
-                if isinstance(target, LoraLayer):
-                    target.update_layer(
-                        adapter_name,
-                        lora_config.r,
-                        lora_config.lora_alpha,
-                        lora_config.lora_dropout,
-                        lora_config.init_lora_weights,
-                    )
-                else:
-                    if loaded_in_8bit and isinstance(target, bnb.nn.Linear8bitLt):
-                        eightbit_kwargs = kwargs.copy()
-                        eightbit_kwargs.update(
-                            {
-                                "has_fp16_weights": target.state.has_fp16_weights,
-                                "memory_efficient_backward": target.state.memory_efficient_backward,
-                                "threshold": target.state.threshold,
-                                "index": target.index,
-                            }
-                        )
-                        new_module = Linear8bitLt(
-                            adapter_name, target.in_features, target.out_features, bias=bias, **eightbit_kwargs
-                        )
-                    elif isinstance(target, torch.nn.Embedding):
-                        embedding_kwargs = kwargs.copy()
-                        embedding_kwargs.pop("fan_in_fan_out", None)
-                        in_features, out_features = target.num_embeddings, target.embedding_dim
-                        new_module = Embedding(adapter_name, in_features, out_features, **embedding_kwargs)
-                    else:
-                        if isinstance(target, torch.nn.Linear):
-                            in_features, out_features = target.in_features, target.out_features
-                            if kwargs["fan_in_fan_out"]:
-                                warnings.warn(
-                                    "fan_in_fan_out is set to True but the target module is `torch.nn.Linear`. "
-                                    "Setting fan_in_fan_out to False."
-                                )
-                                kwargs["fan_in_fan_out"] = lora_config.fan_in_fan_out = False
-                        elif isinstance(target, Conv1D):
-                            in_features, out_features = (
-                                target.weight.ds_shape if hasattr(target.weight, "ds_shape") else target.weight.shape
-                            )
-                            if not kwargs["fan_in_fan_out"]:
-                                warnings.warn(
-                                    "fan_in_fan_out is set to False but the target module is `Conv1D`. "
-                                    "Setting fan_in_fan_out to True."
-                                )
-                                kwargs["fan_in_fan_out"] = lora_config.fan_in_fan_out = True
-                        else:
-                            raise ValueError(
-                                f"Target module {target} is not supported. "
-                                f"Currently, only `torch.nn.Linear` and `Conv1D` are supported."
-                            )
-                        new_module = Linear(adapter_name, in_features, out_features, bias=bias, **kwargs)
-
-                    self._replace_module(parent, target_name, new_module, target)
+            if not is_target_modules_in_base_model:
+                is_target_modules_in_base_model = True
+            parent, target, target_name = _get_submodules(self.model, key)
+
+            if isinstance(target, IA3Layer):
+                target.update_layer(
+                    adapter_name,
+                    ia3_config.init_ia3_weights,
+                )
+            else:
+                new_module = self._create_new_module(ia3_config, adapter_name, target, is_feedforward)
+                self._replace_module(parent, target_name, new_module, target)
         if not is_target_modules_in_base_model:
             raise ValueError(
-                f"Target modules {lora_config.target_modules} not found in the base model. "
+                f"Target modules {ia3_config.target_modules} not found in the base model. "
                 f"Please check the target modules and try again."
             )
 
+    @staticmethod
+    def _is_valid_match(key: str, target_key: str):
+        """
+        Helper function to match module names target_key and key. Makes sure that either the key is exactly the
+        target_key or the target_key is a submodule of key
+        """
+        if key.endswith(target_key):
+            if len(key) > len(target_key):
+                return key.endswith("." + target_key)  # must be a sub module
+            return True
+        return False
+
     def _replace_module(self, parent_module, child_name, new_module, old_module):
         setattr(parent_module, child_name, new_module)
         new_module.weight = old_module.weight
-        if hasattr(old_module, "bias"):
-            if old_module.bias is not None:
-                new_module.bias = old_module.bias
-
+        if old_module.bias is not None:
+            new_module.bias = old_module.bias
         if getattr(old_module, "state", None) is not None:
             new_module.state = old_module.state
             new_module.to(old_module.weight.device)
 
         # dispatch to correct device
         for name, module in new_module.named_modules():
-            if "lora_" in name:
+            if "ia3_" in name:
                 module.to(old_module.weight.device)
 
     def __getattr__(self, name: str):
         """Forward missing attributes to the wrapped module."""
         try:
             return super().__getattr__(name)  # defer to nn.Module's logic
         except AttributeError:
@@ -286,437 +297,254 @@
             if inference:
                 config["inference_mode"] = True
         config_dict[key] = config
         return config
 
     def _set_adapter_layers(self, enabled=True):
         for module in self.model.modules():
-            if isinstance(module, LoraLayer):
+            if isinstance(module, IA3Layer):
                 module.disable_adapters = False if enabled else True
 
     def enable_adapter_layers(self):
         self._set_adapter_layers(enabled=True)
 
     def disable_adapter_layers(self):
         self._set_adapter_layers(enabled=False)
 
     def set_adapter(self, adapter_name):
         for module in self.model.modules():
-            if isinstance(module, LoraLayer):
+            if isinstance(module, IA3Layer):
                 if module.merged:
                     warnings.warn("Adapter cannot be set when the model is merged. Unmerging the model first.")
                     module.unmerge()
                 module.active_adapter = adapter_name
 
-    def merge_adapter(self):
-        for module in self.model.modules():
-            if isinstance(module, LoraLayer):
-                module.merge()
-
-    def unmerge_adapter(self):
-        for module in self.model.modules():
-            if isinstance(module, LoraLayer):
-                module.unmerge()
-
     @staticmethod
-    def _prepare_lora_config(peft_config, model_config):
+    def _prepare_ia3_config(peft_config, model_config):
         if peft_config.target_modules is None:
-            if model_config["model_type"] not in TRANSFORMERS_MODELS_TO_LORA_TARGET_MODULES_MAPPING:
+            if model_config["model_type"] not in TRANSFORMERS_MODELS_TO_IA3_TARGET_MODULES_MAPPING:
                 raise ValueError("Please specify `target_modules` in `peft_config`")
-            peft_config.target_modules = TRANSFORMERS_MODELS_TO_LORA_TARGET_MODULES_MAPPING[model_config["model_type"]]
-        if peft_config.inference_mode:
-            peft_config.merge_weights = True
+            peft_config.target_modules = TRANSFORMERS_MODELS_TO_IA3_TARGET_MODULES_MAPPING[model_config["model_type"]]
+        if peft_config.feedforward_modules is None:
+            if model_config["model_type"] not in TRANSFORMERS_MODELS_TO_IA3_FEEDFORWARD_MODULES_MAPPING:
+                raise ValueError("Please specify `feedforward_modules` in `peft_config`")
+            peft_config.feedforward_modules = TRANSFORMERS_MODELS_TO_IA3_FEEDFORWARD_MODULES_MAPPING[
+                model_config["model_type"]
+            ]
         return peft_config
 
     def merge_and_unload(self):
         r"""
-        This method merges the LoRa layers into the base model. This is needed if someone wants to use the base model
+        This method merges the (IA)^3 layers into the base model. This is needed if someone wants to use the base model
         as a standalone model.
         """
         if getattr(self.config, "model_type", None) == "gpt2":
-            raise ValueError("GPT2 models are not supported for merging LORA layers")
+            raise ValueError("GPT2 models are not supported for merging ia3 layers")
 
         if getattr(self.model, "is_loaded_in_8bit", False):
-            raise ValueError("Cannot merge LORA layers when the model is loaded in 8-bit mode")
+            raise ValueError("Cannot merge ia3 layers when the model is loaded in 8-bit mode")
 
-        key_list = [key for key, _ in self.model.named_modules() if "lora" not in key]
+        key_list = [key for key, _ in self.model.named_modules() if "ia3" not in key]
         for key in key_list:
             try:
                 parent, target, target_name = _get_submodules(self.model, key)
             except AttributeError:
                 continue
-            if isinstance(target, LoraLayer):
+            if isinstance(target, IA3Layer):
                 bias = target.bias is not None
                 new_module = torch.nn.Linear(target.in_features, target.out_features, bias=bias)
                 target.merge()
                 self._replace_module(parent, target_name, new_module, target)
 
             # save any additional trainable modules part of `modules_to_save`
             if isinstance(target, ModulesToSaveWrapper):
                 setattr(parent, target_name, target.modules_to_save[target.active_adapter])
 
         return self.model
 
-    def add_weighted_adapter(self, adapters, weights, adapter_name):
-        if len({self.peft_config[adapter].r for adapter in adapters}) != 1:
-            raise ValueError("All adapters must have the same r value")
-        self.peft_config[adapter_name] = self.peft_config[adapters[0]]
-        self.peft_config[adapter_name].lora_alpha = self.peft_config[adapters[0]].r
-        self._find_and_replace(adapter_name)
-        mark_only_lora_as_trainable(self.model, self.peft_config[adapter_name].bias)
-        _freeze_adapter(self.model, adapter_name)
-        key_list = [key for key, _ in self.model.named_modules() if "lora" not in key]
-        for key in key_list:
-            _, target, _ = _get_submodules(self.model, key)
-            if isinstance(target, LoraLayer):
-                if adapter_name in target.lora_A:
-                    target.lora_A[adapter_name].weight.data = target.lora_A[adapter_name].weight.data * 0.0
-                    target.lora_B[adapter_name].weight.data = target.lora_B[adapter_name].weight.data * 0.0
-                    for adapter, weight in zip(adapters, weights):
-                        if adapter not in target.lora_A:
-                            continue
-                        target.lora_A[adapter_name].weight.data += (
-                            target.lora_A[adapter].weight.data * weight * target.scaling[adapter]
-                        )
-                        target.lora_B[adapter_name].weight.data += target.lora_B[adapter].weight.data * weight
-
-                elif adapter_name in target.lora_embedding_A:
-                    target.lora_embedding_A[adapter_name].data = target.lora_embedding_A[adapter_name].data * 0.0
-                    target.lora_embedding_B[adapter_name].data = target.lora_embedding_B[adapter_name].data * 0.0
-                    for adapter, weight in zip(adapters, weights):
-                        if adapter not in target.lora_embedding_A:
-                            continue
-                        target.lora_embedding_A[adapter_name].data += (
-                            target.lora_embedding_A[adapter].data * weight * target.scaling[adapter]
-                        )
-                        target.lora_embedding_B[adapter_name].data += target.lora_embedding_B[adapter].data * weight
-
 
-# Below code is based on https://github.com/microsoft/LoRA/blob/main/loralib/layers.py
+# Below code is based on https://github.com/microsoft/lora/blob/main/loralib/layers.py
 # and modified to work with PyTorch FSDP
 
 
 #  ------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  ------------------------------------------------------------------------------------------
 
 
-# had to adapt it for `lora_only` to work
-def mark_only_lora_as_trainable(model: nn.Module, bias: str = "none") -> None:
+def mark_only_ia3_as_trainable(model: nn.Module) -> None:
     for n, p in model.named_parameters():
-        if "lora_" not in n:
+        if "ia3_" not in n:
             p.requires_grad = False
-    if bias == "none":
-        return
-    elif bias == "all":
-        for n, p in model.named_parameters():
-            if "bias" in n:
-                p.requires_grad = True
-    elif bias == "lora_only":
-        for m in model.modules():
-            if isinstance(m, LoraLayer) and hasattr(m, "bias") and m.bias is not None:
-                m.bias.requires_grad = True
-    else:
-        raise NotImplementedError
 
 
-class LoraLayer:
+class IA3Layer:
     def __init__(
         self,
         in_features: int,
         out_features: int,
+        is_feedforward: bool,
     ):
-        self.r = {}
-        self.lora_alpha = {}
         self.scaling = {}
-        self.lora_dropout = nn.ModuleDict({})
-        self.lora_A = nn.ModuleDict({})
-        self.lora_B = nn.ModuleDict({})
-        # For Embedding layer
-        self.lora_embedding_A = nn.ParameterDict({})
-        self.lora_embedding_B = nn.ParameterDict({})
+        self.ia3_l = nn.ParameterDict({})
         # Mark the weight as unmerged
         self.merged = False
         self.disable_adapters = False
         self.in_features = in_features
         self.out_features = out_features
+        self.is_feedforward = is_feedforward
 
-    def update_layer(self, adapter_name, r, lora_alpha, lora_dropout, init_lora_weights):
-        self.r[adapter_name] = r
-        self.lora_alpha[adapter_name] = lora_alpha
-        if lora_dropout > 0.0:
-            lora_dropout_layer = nn.Dropout(p=lora_dropout)
-        else:
-            lora_dropout_layer = nn.Identity()
-
-        self.lora_dropout.update(nn.ModuleDict({adapter_name: lora_dropout_layer}))
+    def update_layer(self, adapter_name, init_ia3_weights):
         # Actual trainable parameters
-        if r > 0:
-            self.lora_A.update(nn.ModuleDict({adapter_name: nn.Linear(self.in_features, r, bias=False)}))
-            self.lora_B.update(nn.ModuleDict({adapter_name: nn.Linear(r, self.out_features, bias=False)}))
-            self.scaling[adapter_name] = lora_alpha / r
-        if init_lora_weights:
-            self.reset_lora_parameters(adapter_name)
-        self.to(self.weight.device)
-
-    def update_layer_embedding(self, adapter_name, r, lora_alpha, lora_dropout, init_lora_weights):
-        self.r[adapter_name] = r
-        self.lora_alpha[adapter_name] = lora_alpha
-        if lora_dropout > 0.0:
-            lora_dropout_layer = nn.Dropout(p=lora_dropout)
+        if self.is_feedforward:
+            weight = torch.randn((1, self.in_features))
         else:
-            lora_dropout_layer = nn.Identity()
-
-        self.lora_dropout.update(nn.ModuleDict({adapter_name: lora_dropout_layer}))
-        # Actual trainable parameters
-        if r > 0:
-            self.lora_embedding_A.update(
-                nn.ParameterDict({adapter_name: nn.Parameter(self.weight.new_zeros((r, self.in_features)))})
-            )
-            self.lora_embedding_B.update(
-                nn.ParameterDict({adapter_name: nn.Parameter(self.weight.new_zeros((self.out_features, r)))})
-            )
-            self.scaling[adapter_name] = lora_alpha / r
-        if init_lora_weights:
-            self.reset_lora_parameters(adapter_name)
+            weight = torch.randn((self.out_features, 1))
+        self.ia3_l.update(nn.ParameterDict({adapter_name: nn.Parameter(weight)}))
+        if init_ia3_weights:
+            self.reset_ia3_parameters(adapter_name)
         self.to(self.weight.device)
 
-    def reset_lora_parameters(self, adapter_name):
-        if adapter_name in self.lora_A.keys():
-            # initialize A the same way as the default for nn.Linear and B to zero
-            nn.init.kaiming_uniform_(self.lora_A[adapter_name].weight, a=math.sqrt(5))
-            nn.init.zeros_(self.lora_B[adapter_name].weight)
-        if adapter_name in self.lora_embedding_A.keys():
-            # initialize a the same way as the default for nn.linear and b to zero
-            nn.init.zeros_(self.lora_embedding_A[adapter_name])
-            nn.init.normal_(self.lora_embedding_B[adapter_name])
+    def reset_ia3_parameters(self, adapter_name):
+        if adapter_name in self.ia3_l.keys():
+            # initialize learned vector with torch.ones
+            nn.init.constant_(self.ia3_l[adapter_name], 1.0)
 
 
-class Linear(nn.Linear, LoraLayer):
-    # Lora implemented in a dense layer
+class Linear(nn.Linear, IA3Layer):
+    # (IA)^3 implemented in a dense layer
     def __init__(
         self,
         adapter_name: str,
         in_features: int,
         out_features: int,
-        r: int = 0,
-        lora_alpha: int = 1,
-        lora_dropout: float = 0.0,
         fan_in_fan_out: bool = False,  # Set this to True if the layer to replace stores weight like (fan_in, fan_out)
+        is_feedforward: bool = False,  # Set to True if the layer is treated as a feedforward layer
         **kwargs,
     ):
-        init_lora_weights = kwargs.pop("init_lora_weights", True)
+        init_ia3_weights = kwargs.pop("init_ia3_weights", True)
 
         nn.Linear.__init__(self, in_features, out_features, **kwargs)
-        LoraLayer.__init__(self, in_features=in_features, out_features=out_features)
+        IA3Layer.__init__(self, in_features=in_features, out_features=out_features, is_feedforward=is_feedforward)
         # Freezing the pre-trained weight matrix
         self.weight.requires_grad = False
 
         self.fan_in_fan_out = fan_in_fan_out
         if fan_in_fan_out:
             self.weight.data = self.weight.data.T
 
         nn.Linear.reset_parameters(self)
-        self.update_layer(adapter_name, r, lora_alpha, lora_dropout, init_lora_weights)
+        self.update_layer(adapter_name, init_ia3_weights)
         self.active_adapter = adapter_name
 
+        self.is_feedforward = is_feedforward
+
     def merge(self):
-        if self.active_adapter not in self.lora_A.keys():
+        if self.active_adapter not in self.ia3_l.keys():
             return
         if self.merged:
             warnings.warn("Already merged. Nothing to do.")
             return
-        if self.r[self.active_adapter] > 0:
-            self.weight.data += (
-                transpose(
-                    self.lora_B[self.active_adapter].weight @ self.lora_A[self.active_adapter].weight,
-                    self.fan_in_fan_out,
-                )
-                * self.scaling[self.active_adapter]
-            )
-            self.merged = True
+
+        self.weight = transpose(self.weight, self.fan_in_fan_out)
+        self.weight.data = torch.mul(self.weight.data, self.ia3_l[self.active_adapter].data)
+        self.weight = transpose(self.weight, self.fan_in_fan_out)
+
+        self.merged = True
 
     def unmerge(self):
-        if self.active_adapter not in self.lora_A.keys():
+        if self.active_adapter not in self.ia3_l.keys():
             return
         if not self.merged:
             warnings.warn("Already unmerged. Nothing to do.")
             return
-        if self.r[self.active_adapter] > 0:
-            self.weight.data -= (
-                transpose(
-                    self.lora_B[self.active_adapter].weight @ self.lora_A[self.active_adapter].weight,
-                    self.fan_in_fan_out,
-                )
-                * self.scaling[self.active_adapter]
-            )
-            self.merged = False
+
+        warnings.warn("Unmerge result can be inaccurate for (IA)^3.")
+        self.weight = transpose(self.weight, self.fan_in_fan_out)
+        # divide by (IA)^3 vector. Add tolerace to avoid division by zero
+        self.weight.data = torch.div(self.weight.data, self.ia3_l[self.active_adapter].data + 1e-8)
+        self.weight = transpose(self.weight, self.fan_in_fan_out)
+
+        self.merged = False
 
     def forward(self, x: torch.Tensor):
         previous_dtype = x.dtype
 
-        if self.active_adapter not in self.lora_A.keys():
+        if self.active_adapter not in self.ia3_l.keys():
             return F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
+
         if self.disable_adapters:
-            if self.r[self.active_adapter] > 0 and self.merged:
+            if self.merged:
                 self.unmerge()
             result = F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
-        elif self.r[self.active_adapter] > 0 and not self.merged:
-            result = F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
-
-            x = x.to(self.lora_A[self.active_adapter].weight.dtype)
-
-            result += (
-                self.lora_B[self.active_adapter](
-                    self.lora_A[self.active_adapter](self.lora_dropout[self.active_adapter](x))
+        elif not self.merged:
+            if self.is_feedforward:
+                x = x.to(self.ia3_l[self.active_adapter].dtype)
+                interm = x * self.ia3_l[self.active_adapter].flatten()
+                result = F.linear(
+                    interm.to(self.weight.dtype),
+                    transpose(self.weight, self.fan_in_fan_out),
+                    bias=self.bias,
                 )
-                * self.scaling[self.active_adapter]
-            )
+            else:
+                result = F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
+                result = result.to(self.ia3_l[self.active_adapter].dtype) * self.ia3_l[self.active_adapter].flatten()
         else:
             result = F.linear(x, transpose(self.weight, self.fan_in_fan_out), bias=self.bias)
 
         result = result.to(previous_dtype)
 
         return result
 
 
-class Embedding(nn.Embedding, LoraLayer):
-    # LoRA implemented in a Embedding layer
-    def __init__(
-        self,
-        adapter_name: str,
-        num_embeddings: int,
-        embedding_dim: int,
-        r: int = 0,
-        lora_alpha: int = 1,
-        lora_dropout: float = 0.0,
-        **kwargs,
-    ):
-        init_lora_weights = kwargs.pop("init_lora_weights", True)
-
-        nn.Embedding.__init__(self, num_embeddings, embedding_dim, **kwargs)
-        LoraLayer.__init__(self, in_features=num_embeddings, out_features=embedding_dim)
-
-        self.weight.requires_grad = False
-
-        nn.Embedding.reset_parameters(self)
-        self.update_layer_embedding(adapter_name, r, lora_alpha, lora_dropout, init_lora_weights)
-        self.active_adapter = adapter_name
-
-    def unmerge(self, mode: bool = True):
-        if not self.merged:
-            warnings.warn("Already unmerged. Nothing to do.")
-            return
-        if self.r[self.active_adapter] > 0:
-            self.weight.data -= (
-                transpose(
-                    self.lora_embedding_B[self.active_adapter] @ self.lora_embedding_A[self.active_adapter], True
-                )
-                * self.scaling[self.active_adapter]
-            )
-            self.merged = False
-
-    def merge(self):
-        if self.merged:
-            warnings.warn("Already merged. Nothing to do.")
-            return
-        if self.r[self.active_adapter] > 0:
-            self.weight.data += (
-                transpose(
-                    self.lora_embedding_B[self.active_adapter] @ self.lora_embedding_A[self.active_adapter], True
-                )
-                * self.scaling[self.active_adapter]
-            )
-            self.merged = True
-
-    def forward(self, x: torch.Tensor):
-        if self.disable_adapters:
-            if self.r[self.active.adapter] > 0 and self.merged:
-                self.weight.data -= (
-                    transpose(
-                        self.lora_embedding_B[self.active_adapter].weight
-                        @ self.lora_embedding_A[self.active_adapter].weight,
-                        True,
-                    )
-                    * self.scaling[self.active_adapter]
-                )
-                self.merged = False
-            return nn.Embedding.forward(self, x)
-
-        elif self.r[self.active_adapter] > 0 and not self.merged:
-            result = nn.Embedding.forward(self, x)
-            if self.r[self.active_adapter] > 0:
-                after_A = F.embedding(
-                    x,
-                    self.lora_embedding_A[self.active_adapter].T,
-                    self.padding_idx,
-                    self.max_norm,
-                    self.norm_type,
-                    self.scale_grad_by_freq,
-                    self.sparse,
-                )
-                result += (after_A @ self.lora_embedding_B[self.active_adapter].T) * self.scaling[self.active_adapter]
-            return result
-        else:
-            return nn.Embedding.forward(self, x)
-
-
 if is_bnb_available():
 
-    class Linear8bitLt(bnb.nn.Linear8bitLt, LoraLayer):
-        # Lora implemented in a dense layer
+    class Linear8bitLt(bnb.nn.Linear8bitLt, IA3Layer):
+        # (IA)^3 implemented in a dense layer
         def __init__(
             self,
             adapter_name,
             in_features,
             out_features,
-            r: int = 0,
-            lora_alpha: int = 1,
-            lora_dropout: float = 0.0,
+            is_feedforward,
             **kwargs,
         ):
             bnb.nn.Linear8bitLt.__init__(
                 self,
                 in_features,
                 out_features,
                 bias=kwargs.get("bias", True),
                 has_fp16_weights=kwargs.get("has_fp16_weights", True),
                 memory_efficient_backward=kwargs.get("memory_efficient_backward", False),
                 threshold=kwargs.get("threshold", 0.0),
                 index=kwargs.get("index", None),
             )
-            LoraLayer.__init__(self, in_features=in_features, out_features=out_features)
+            IA3Layer.__init__(self, in_features=in_features, out_features=out_features, is_feedforward=is_feedforward)
 
             # Freezing the pre-trained weight matrix
             self.weight.requires_grad = False
 
-            init_lora_weights = kwargs.pop("init_lora_weights", True)
-            self.update_layer(adapter_name, r, lora_alpha, lora_dropout, init_lora_weights)
+            init_ia3_weights = kwargs.pop("init_ia3_weights", True)
+            self.update_layer(adapter_name, init_ia3_weights)
             self.active_adapter = adapter_name
+            self.is_feedforward = is_feedforward
 
         def forward(self, x: torch.Tensor):
-            result = super().forward(x)
-
-            if self.disable_adapters or self.active_adapter not in self.lora_A.keys():
-                return result
-            elif self.r[self.active_adapter] > 0:
+            if self.disable_adapters or self.active_adapter not in self.ia3_l.keys():
+                return super().forward(x)
+            else:
                 if not torch.is_autocast_enabled():
-                    expected_dtype = result.dtype
-
                     if x.dtype != torch.float32:
                         x = x.float()
-                    output = (
-                        self.lora_B[self.active_adapter](
-                            self.lora_A[self.active_adapter](self.lora_dropout[self.active_adapter](x))
-                        ).to(expected_dtype)
-                        * self.scaling[self.active_adapter]
-                    )
+                    if self.is_feedforward:
+                        result = super().forward(x * self.ia3_l[self.active_adapter].flatten())
+                    else:
+                        result = super().forward(x)
+                        expected_dtype = result.dtype
+                        result = (result * self.ia3_l[self.active_adapter].flatten()).to(expected_dtype)
                 else:
-                    output = (
-                        self.lora_B[self.active_adapter](
-                            self.lora_A[self.active_adapter](self.lora_dropout[self.active_adapter](x))
-                        )
-                        * self.scaling[self.active_adapter]
-                    )
-                result += output
+                    if self.is_feedforward:
+                        result = super().forward(x * self.ia3_l[self.active_adapter].flatten())
+                    else:
+                        result = result * self.ia3_l[self.active_adapter].flatten()
             return result
```

### Comparing `peft-0.3.0/src/peft/tuners/p_tuning.py` & `peft-0.4.0/src/peft/tuners/p_tuning.py`

 * *Files identical despite different names*

### Comparing `peft-0.3.0/src/peft/tuners/prefix_tuning.py` & `peft-0.4.0/src/peft/tuners/prefix_tuning.py`

 * *Files identical despite different names*

### Comparing `peft-0.3.0/src/peft/tuners/prompt_tuning.py` & `peft-0.4.0/src/peft/tuners/prompt_tuning.py`

 * *Files identical despite different names*

### Comparing `peft-0.3.0/src/peft/utils/__init__.py` & `peft-0.4.0/src/peft/utils/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,20 +18,29 @@
 # limitations under the License.
 
 from .config import PeftConfig, PeftType, PromptLearningConfig, TaskType
 from .other import (
     TRANSFORMERS_MODELS_TO_PREFIX_TUNING_POSTPROCESS_MAPPING,
     TRANSFORMERS_MODELS_TO_LORA_TARGET_MODULES_MAPPING,
     TRANSFORMERS_MODELS_TO_ADALORA_TARGET_MODULES_MAPPING,
+    TRANSFORMERS_MODELS_TO_IA3_TARGET_MODULES_MAPPING,
+    TRANSFORMERS_MODELS_TO_IA3_FEEDFORWARD_MODULES_MAPPING,
+    COMMON_LAYERS_PATTERN,
     CONFIG_NAME,
     WEIGHTS_NAME,
+    SAFETENSORS_WEIGHTS_NAME,
+    CLAMP_QUANTILE,
     _set_trainable,
+    add_library_to_model_card,
     bloom_model_postprocess_past_key_value,
     prepare_model_for_int8_training,
+    prepare_model_for_kbit_training,
     shift_tokens_right,
     transpose,
     _get_submodules,
     _set_adapter,
     _freeze_adapter,
     ModulesToSaveWrapper,
+    _prepare_prompt_learning_config,
 )
+from .hub_utils import hub_file_exists
 from .save_and_load import get_peft_model_state_dict, set_peft_model_state_dict
```

### Comparing `peft-0.3.0/src/peft/utils/config.py` & `peft-0.4.0/src/peft/utils/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import enum
+import inspect
 import json
 import os
 from dataclasses import asdict, dataclass, field
 from typing import Optional, Union
 
 from huggingface_hub import hf_hub_download
 from transformers.utils import PushToHubMixin
@@ -27,42 +28,44 @@
 class PeftType(str, enum.Enum):
     PROMPT_TUNING = "PROMPT_TUNING"
     P_TUNING = "P_TUNING"
     PREFIX_TUNING = "PREFIX_TUNING"
     LORA = "LORA"
     ADALORA = "ADALORA"
     ADAPTION_PROMPT = "ADAPTION_PROMPT"
+    IA3 = "IA3"
 
 
 class TaskType(str, enum.Enum):
     SEQ_CLS = "SEQ_CLS"
     SEQ_2_SEQ_LM = "SEQ_2_SEQ_LM"
     CAUSAL_LM = "CAUSAL_LM"
     TOKEN_CLS = "TOKEN_CLS"
+    QUESTION_ANS = "QUESTION_ANS"
+    FEATURE_EXTRACTION = "FEATURE_EXTRACTION"
 
 
 @dataclass
 class PeftConfigMixin(PushToHubMixin):
     r"""
     This is the base configuration class for PEFT adapter models. It contains all the methods that are common to all
     PEFT adapter models. This class inherits from [`~transformers.utils.PushToHubMixin`] which contains the methods to
     push your model to the Hub. The method `save_pretrained` will save the configuration of your adapter model in a
     directory. The method `from_pretrained` will load the configuration of your adapter model from a directory.
 
     Args:
         peft_type (Union[[`~peft.utils.config.PeftType`], `str`]): The type of Peft method to use.
     """
     peft_type: Optional[PeftType] = field(default=None, metadata={"help": "The type of PEFT model."})
-
-    @property
-    def __dict__(self):
-        return asdict(self)
+    auto_mapping: Optional[dict] = field(
+        default=None, metadata={"help": "An auto mapping dict to help retrieve the base model class if needed."}
+    )
 
     def to_dict(self):
-        return self.__dict__
+        return asdict(self)
 
     def save_pretrained(self, save_directory, **kwargs):
         r"""
         This method saves the configuration of your adapter model in a directory.
 
         Args:
             save_directory (`str`):
@@ -71,18 +74,23 @@
                 Additional keyword arguments passed along to the [`~transformers.utils.PushToHubMixin.push_to_hub`]
                 method.
         """
         if os.path.isfile(save_directory):
             raise AssertionError(f"Provided path ({save_directory}) should be a directory, not a file")
 
         os.makedirs(save_directory, exist_ok=True)
+        auto_mapping_dict = kwargs.pop("auto_mapping_dict", None)
 
-        output_dict = self.__dict__
+        output_dict = asdict(self)
         output_path = os.path.join(save_directory, CONFIG_NAME)
 
+        # Add auto mapping details for custom models.
+        if auto_mapping_dict is not None:
+            output_dict["auto_mapping"] = auto_mapping_dict
+
         # save it
         with open(output_path, "w") as writer:
             writer.write(json.dumps(output_dict, indent=2, sort_keys=True))
 
     @classmethod
     def from_pretrained(cls, pretrained_model_name_or_path, subfolder=None, **kwargs):
         r"""
@@ -95,25 +103,30 @@
                 Additional keyword arguments passed along to the child class initialization.
         """
         path = (
             os.path.join(pretrained_model_name_or_path, subfolder)
             if subfolder is not None
             else pretrained_model_name_or_path
         )
+
+        hf_hub_download_kwargs, class_kwargs, _ = cls._split_kwargs(kwargs)
+
         if os.path.isfile(os.path.join(path, CONFIG_NAME)):
             config_file = os.path.join(path, CONFIG_NAME)
         else:
             try:
-                config_file = hf_hub_download(pretrained_model_name_or_path, CONFIG_NAME, subfolder=subfolder)
+                config_file = hf_hub_download(
+                    pretrained_model_name_or_path, CONFIG_NAME, subfolder=subfolder, **hf_hub_download_kwargs
+                )
             except Exception:
                 raise ValueError(f"Can't find '{CONFIG_NAME}' at '{pretrained_model_name_or_path}'")
 
         loaded_attributes = cls.from_json_file(config_file)
 
-        config = cls(**kwargs)
+        config = cls(**class_kwargs)
 
         for key, value in loaded_attributes.items():
             if hasattr(config, key):
                 setattr(config, key, value)
 
         return config
 
@@ -127,27 +140,69 @@
                 The path to the json file.
         """
         with open(path_json_file, "r") as file:
             json_object = json.load(file)
 
         return json_object
 
+    @classmethod
+    def _split_kwargs(cls, kwargs):
+        hf_hub_download_kwargs = {}
+        class_kwargs = {}
+        other_kwargs = {}
+
+        for key, value in kwargs.items():
+            if key in inspect.signature(hf_hub_download).parameters:
+                hf_hub_download_kwargs[key] = value
+            elif key in list(cls.__annotations__):
+                class_kwargs[key] = value
+            else:
+                other_kwargs[key] = value
+
+        return hf_hub_download_kwargs, class_kwargs, other_kwargs
+
+    @classmethod
+    def _get_peft_type(
+        cls,
+        model_id,
+        **hf_hub_download_kwargs,
+    ):
+        subfolder = hf_hub_download_kwargs.get("subfolder", None)
+
+        path = os.path.join(model_id, subfolder) if subfolder is not None else model_id
+
+        if os.path.isfile(os.path.join(path, CONFIG_NAME)):
+            config_file = os.path.join(path, CONFIG_NAME)
+        else:
+            try:
+                config_file = hf_hub_download(
+                    model_id,
+                    CONFIG_NAME,
+                    **hf_hub_download_kwargs,
+                )
+            except Exception:
+                raise ValueError(f"Can't find '{CONFIG_NAME}' at '{model_id}'")
+
+        loaded_attributes = cls.from_json_file(config_file)
+        return loaded_attributes["peft_type"]
+
 
 @dataclass
 class PeftConfig(PeftConfigMixin):
     """
     This is the base configuration class to store the configuration of a [`PeftModel`].
 
     Args:
         peft_type (Union[[`~peft.utils.config.PeftType`], `str`]): The type of Peft method to use.
         task_type (Union[[`~peft.utils.config.TaskType`], `str`]): The type of task to perform.
         inference_mode (`bool`, defaults to `False`): Whether to use the Peft model in inference mode.
     """
 
     base_model_name_or_path: str = field(default=None, metadata={"help": "The name of the base model to use."})
+    revision: str = field(default=None, metadata={"help": "The specific model version to use."})
     peft_type: Union[str, PeftType] = field(default=None, metadata={"help": "Peft type"})
     task_type: Union[str, TaskType] = field(default=None, metadata={"help": "Task type"})
     inference_mode: bool = field(default=False, metadata={"help": "Whether to use inference mode"})
 
 
 @dataclass
 class PromptLearningConfig(PeftConfig):
```

### Comparing `peft-0.3.0/src/peft/utils/save_and_load.py` & `peft-0.4.0/src/peft/utils/save_and_load.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,16 @@
     elif isinstance(config, PromptLearningConfig):
         to_return = {}
         if config.inference_mode:
             prompt_embeddings = model.prompt_encoder[adapter_name].embedding.weight
         else:
             prompt_embeddings = model.get_prompt_embedding_to_save(adapter_name)
         to_return["prompt_embeddings"] = prompt_embeddings
+    elif config.peft_type == PeftType.IA3:
+        to_return = {k: state_dict[k] for k in state_dict if "ia3_" in k}
     else:
         raise NotImplementedError
     if model.modules_to_save is not None:
         for key, value in state_dict.items():
             if any(f"{module_name}.modules_to_save.{adapter_name}" in key for module_name in model.modules_to_save):
                 to_return[key.replace("modules_to_save.", "")] = value
 
@@ -94,19 +96,20 @@
                     if module_name in key:
                         key = key.replace(module_name, f"{module_name}.modules_to_save.{adapter_name}")
                         break
             state_dict[key] = value
     else:
         state_dict = peft_model_state_dict
 
-    if config.peft_type in (PeftType.LORA, PeftType.ADALORA):
+    if config.peft_type in (PeftType.LORA, PeftType.ADALORA, PeftType.IA3):
         peft_model_state_dict = {}
+        parameter_prefix = "ia3_" if config.peft_type == PeftType.IA3 else "lora_"
         for k, v in state_dict.items():
-            if "lora_" in k:
-                suffix = k.split("lora_")[1]
+            if parameter_prefix in k:
+                suffix = k.split(parameter_prefix)[1]
                 if "." in suffix:
                     suffix_to_replace = ".".join(suffix.split(".")[1:])
                     k = k.replace(suffix_to_replace, f"{adapter_name}.{suffix_to_replace}")
                 else:
                     k = f"{k}.{adapter_name}"
                 peft_model_state_dict[k] = v
             else:
@@ -116,12 +119,13 @@
             if rank_pattern is not None:
                 model.resize_modules_by_rank_pattern(rank_pattern, adapter_name)
     elif isinstance(config, PromptLearningConfig) or config.peft_type == PeftType.ADAPTION_PROMPT:
         peft_model_state_dict = state_dict
     else:
         raise NotImplementedError
 
-    model.load_state_dict(peft_model_state_dict, strict=False)
+    load_result = model.load_state_dict(peft_model_state_dict, strict=False)
     if isinstance(config, PromptLearningConfig):
         model.prompt_encoder[adapter_name].embedding.load_state_dict(
             {"weight": peft_model_state_dict["prompt_embeddings"]}, strict=True
         )
+    return load_result
```

### Comparing `peft-0.3.0/src/peft.egg-info/PKG-INFO` & `peft-0.4.0/src/peft.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: peft
-Version: 0.3.0
+Version: 0.4.0
 Summary: Parameter-Efficient Fine-Tuning (PEFT)
 Home-page: https://github.com/huggingface/peft
 Author: The HuggingFace team
 Author-email: sourab@huggingface.co
 License: Apache
 Keywords: deep learning
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: quality
 Provides-Extra: docs_specific
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
@@ -53,14 +53,15 @@
 Supported methods:
 
 1. LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685)
 2. Prefix Tuning: [Prefix-Tuning: Optimizing Continuous Prompts for Generation](https://aclanthology.org/2021.acl-long.353/), [P-Tuning v2: Prompt Tuning Can Be Comparable to Fine-tuning Universally Across Scales and Tasks](https://arxiv.org/pdf/2110.07602.pdf)
 3. P-Tuning: [GPT Understands, Too](https://arxiv.org/abs/2103.10385)
 4. Prompt Tuning: [The Power of Scale for Parameter-Efficient Prompt Tuning](https://arxiv.org/abs/2104.08691)
 5. AdaLoRA: [Adaptive Budget Allocation for Parameter-Efficient Fine-Tuning](https://arxiv.org/abs/2303.10512)  
+6. $(IA)^3$ : [Infused Adapter by Inhibiting and Amplifying Inner Activations](https://arxiv.org/abs/2205.05638)
 
 ## Getting started
 
 ```python
 from transformers import AutoModelForSeq2SeqLM
 from peft import get_peft_config, get_peft_model, LoraConfig, TaskType
 model_name_or_path = "bigscience/mt0-large"
@@ -162,15 +163,15 @@
 - Here is an example in [trl](https://github.com/lvwerra/trl) library using PEFT+INT8 for tuning policy model: [gpt2-sentiment_peft.py](https://github.com/lvwerra/trl/blob/main/examples/sentiment/scripts/gpt2-sentiment_peft.py) and corresponding [Blog](https://huggingface.co/blog/trl-peft)
 - Example using PEFT for Instrction finetuning, reward model and policy : [stack_llama](https://github.com/lvwerra/trl/tree/main/examples/stack_llama/scripts) and corresponding [Blog](https://huggingface.co/blog/stackllama) 
 
 ### INT8 training of large models in Colab using PEFT LoRA and bits_and_bytes
 
 - Here is now a demo on how to fine tune [OPT-6.7b](https://huggingface.co/facebook/opt-6.7b) (14GB in fp16) in a Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jCkpikz0J2o20FBQmYmAGdiKmJGOMo-o?usp=sharing)
 
-- Here is now a demo on how to fine tune [whishper-large](openai/whisper-large-v2) (1.5B params) (14GB in fp16) in a Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1DOkD_5OUjFa0r5Ik3SgywJLJtEo2qLxO?usp=sharing) and [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vhF8yueFqha3Y3CpTHN6q9EVcII9EYzs?usp=sharing)
+- Here is now a demo on how to fine tune [whisper-large](https://huggingface.co/openai/whisper-large-v2) (1.5B params) (14GB in fp16) in a Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1DOkD_5OUjFa0r5Ik3SgywJLJtEo2qLxO?usp=sharing) and [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vhF8yueFqha3Y3CpTHN6q9EVcII9EYzs?usp=sharing)
 
 ### Save compute and storage even for medium and small models
 
 Save storage by avoiding full finetuning of models on each of the downstream tasks/datasets,
 With PEFT methods, users only need to store tiny checkpoints in the order of `MBs` all the while retaining 
 performance comparable to full finetuning.
 
@@ -246,87 +247,87 @@
 ### Example of PEFT model inference using 🤗 Accelerate's Big Model Inferencing capabilities
 An example is provided in `~examples/causal_language_modeling/peft_lora_clm_accelerate_big_model_inference.ipynb`. 
 
 
 ## Models support matrix
 
 ### Causal Language Modeling
-| Model        | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  |
-|--------------| ---- | ---- | ---- | ----  |
-| GPT-2        | ✅  | ✅  | ✅  | ✅  |
-| Bloom        | ✅  | ✅  | ✅  | ✅  |
-| OPT          | ✅  | ✅  | ✅  | ✅  |
-| GPT-Neo      | ✅  | ✅  | ✅  | ✅  |
-| GPT-J        | ✅  | ✅  | ✅  | ✅  |
-| GPT-NeoX-20B | ✅  | ✅  | ✅  | ✅  |
-| LLaMA        | ✅  | ✅  | ✅  | ✅  |
-| ChatGLM      | ✅  | ✅  | ✅  | ✅  |
+| Model        | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+|--------------| ---- | ---- | ---- | ----  | ----  |
+| GPT-2        | ✅  | ✅  | ✅  | ✅  | ✅  |
+| Bloom        | ✅  | ✅  | ✅  | ✅  | ✅  |
+| OPT          | ✅  | ✅  | ✅  | ✅  | ✅  |
+| GPT-Neo      | ✅  | ✅  | ✅  | ✅  | ✅  |
+| GPT-J        | ✅  | ✅  | ✅  | ✅  | ✅  |
+| GPT-NeoX-20B | ✅  | ✅  | ✅  | ✅  | ✅  |
+| LLaMA        | ✅  | ✅  | ✅  | ✅  | ✅  |
+| ChatGLM      | ✅  | ✅  | ✅  | ✅  | ✅  |
 
 ### Conditional Generation
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ---- |
-| T5        | ✅   | ✅   | ✅   | ✅   |
-| BART      | ✅   | ✅   | ✅   | ✅   |
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ---- | ---- |
+| T5        | ✅   | ✅   | ✅   | ✅   | ✅   |
+| BART      | ✅   | ✅   | ✅   | ✅   | ✅   |
 
 ### Sequence Classification
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| BERT           | ✅  | ✅  | ✅  | ✅  |  
-| RoBERTa        | ✅  | ✅  | ✅  | ✅  |
-| GPT-2          | ✅  | ✅  | ✅  | ✅  | 
-| Bloom          | ✅  | ✅  | ✅  | ✅  |   
-| OPT            | ✅  | ✅  | ✅  | ✅  |
-| GPT-Neo        | ✅  | ✅  | ✅  | ✅  |
-| GPT-J          | ✅  | ✅  | ✅  | ✅  |
-| Deberta        | ✅  |     | ✅  | ✅  |     
-| Deberta-v2     | ✅  |     | ✅  | ✅  |    
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| BERT           | ✅  | ✅  | ✅  | ✅  |  ✅  |  
+| RoBERTa        | ✅  | ✅  | ✅  | ✅  | ✅  |
+| GPT-2          | ✅  | ✅  | ✅  | ✅  |   |
+| Bloom          | ✅  | ✅  | ✅  | ✅  |   |
+| OPT            | ✅  | ✅  | ✅  | ✅  |   |
+| GPT-Neo        | ✅  | ✅  | ✅  | ✅  |   |
+| GPT-J          | ✅  | ✅  | ✅  | ✅  |   |
+| Deberta        | ✅  |     | ✅  | ✅  |   | 
+| Deberta-v2     | ✅  |     | ✅  | ✅  |   |
 
 ### Token Classification
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| BERT           | ✅  | ✅  |   |   |  
-| RoBERTa        | ✅  | ✅  |   |   |
-| GPT-2          | ✅  | ✅  |   |   | 
-| Bloom          | ✅  | ✅  |   |   |   
-| OPT            | ✅  | ✅  |   |   |
-| GPT-Neo        | ✅  | ✅  |   |   |
-| GPT-J          | ✅  | ✅  |   |   |
-| Deberta        | ✅  |     |   |   | 
-| Deberta-v2     | ✅  |     |   |   |
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| BERT           | ✅  | ✅  |   |   |   |  
+| RoBERTa        | ✅  | ✅  |   |   |   |
+| GPT-2          | ✅  | ✅  |   |   |   |
+| Bloom          | ✅  | ✅  |   |   |   |
+| OPT            | ✅  | ✅  |   |   |   |
+| GPT-Neo        | ✅  | ✅  |   |   |   |
+| GPT-J          | ✅  | ✅  |   |   |   |
+| Deberta        | ✅  |     |   |   |   |
+| Deberta-v2     | ✅  |     |   |   |   |
 
 ### Text-to-Image Generation
 
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| Stable Diffusion           | ✅  |   |   |   |  
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| Stable Diffusion           | ✅  |   |   |   |   |  
 
 
 ### Image Classification
 
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| ViT           | ✅  |   |   |   | 
-| Swin           | ✅  |   |   |   | 
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| ViT           | ✅  |   |   |   |    | 
+| Swin           | ✅  |   |   |   |   |  
 
 ### Image to text (Multi-modal models)
 
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| Blip-2           | ✅  |   |   |   | 
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| Blip-2           | ✅  |   |   |   |   |
 
 ___Note that we have tested LoRA for [ViT](https://huggingface.co/docs/transformers/model_doc/vit) and [Swin](https://huggingface.co/docs/transformers/model_doc/swin) for fine-tuning on image classification. However, it should be possible to use LoRA for any compatible model [provided](https://huggingface.co/models?pipeline_tag=image-classification&sort=downloads&search=vit) by 🤗 Transformers. Check out the respective
 examples to learn more. If you run into problems, please open an issue.___
 
 The same principle applies to our [segmentation models](https://huggingface.co/models?pipeline_tag=image-segmentation&sort=downloads) as well. 
 
 ### Semantic Segmentation
 
-|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | 
-| --------- | ---- | ---- | ---- | ----  |
-| SegFormer           | ✅  |   |   |   | 
+|   Model         | LoRA | Prefix Tuning  | P-Tuning | Prompt Tuning  | IA3 |
+| --------- | ---- | ---- | ---- | ----  | ----  |
+| SegFormer           | ✅  |   |   |   |   | 
 
 
 ## Caveats:
 
 1. Below is an example of using PyTorch FSDP for training. However, it doesn't lead to 
 any GPU memory savings. Please refer issue [[FSDP] FSDP with CPU offload consumes 1.65X more GPU memory when training models with most of the params frozen](https://github.com/pytorch/pytorch/issues/91165). 
 
@@ -375,35 +376,30 @@
   use_cpu: false
   ```
   b. run the below command to launch the example script
   ```bash
   accelerate launch --config_file fsdp_config.yaml examples/peft_lora_seq2seq_accelerate_fsdp.py
   ```
 
-2. When using `P_TUNING` or `PROMPT_TUNING` with `SEQ_2_SEQ` task, remember to remove the `num_virtual_token` virtual prompt predictions from the left side of the model outputs during evaluations. 
-
-3. For encoder-decoder models, `P_TUNING` or `PROMPT_TUNING` doesn't support `generate` functionality of transformers because `generate` strictly requires `decoder_input_ids` but 
-`P_TUNING`/`PROMPT_TUNING` appends soft prompt embeddings to `input_embeds` to create
-new `input_embeds` to be given to the model. Therefore, `generate` doesn't support this yet.
-
-4. When using ZeRO3 with zero3_init_flag=True, if you find the gpu memory increase with training steps. we might need to set zero3_init_flag=false in accelerate config.yaml. The related issue is [[BUG] memory leak under zero.Init](https://github.com/microsoft/DeepSpeed/issues/2637)
+2. When using ZeRO3 with zero3_init_flag=True, if you find the gpu memory increase with training steps. we might need to update deepspeed after [deepspeed commit 42858a9891422abc](https://github.com/microsoft/DeepSpeed/commit/42858a9891422abcecaa12c1bd432d28d33eb0d4) . The related issue is [[BUG] Peft Training with Zero.Init() and Zero3 will increase GPU memory every forward step ](https://github.com/microsoft/DeepSpeed/issues/3002)
 
 ## Backlog:
 - [x] Add tests
 - [x] Multi Adapter training and inference support
 - [x] Add more use cases and examples
-- [ ] Explore and possibly integrate `Bottleneck Adapters`, `(IA)^3`, `AdaptionPrompt` ...
+- [x] Integrate`(IA)^3`, `AdaptionPrompt`
+- [ ] Explore and possibly integrate methods like `Bottleneck Adapters`,  ...
 
 ## Citing 🤗 PEFT
 
 If you use 🤗 PEFT in your publication, please cite it by using the following BibTeX entry.
 
 ```bibtex
 @Misc{peft,
   title =        {PEFT: State-of-the-art Parameter-Efficient Fine-Tuning methods},
-  author =       {Sourab Mangrulkar, Sylvain Gugger, Lysandre Debut, Younes Belkada, Sayak Paul},
+  author =       {Sourab Mangrulkar and Sylvain Gugger and Lysandre Debut and Younes Belkada and Sayak Paul},
   howpublished = {\url{https://github.com/huggingface/peft}},
   year =         {2022}
 }
 ```
```

