# Comparing `tmp/langdash-1.8.0.tar.gz` & `tmp/langdash-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.8.0.tar", last modified: Sat Jul 15 20:32:17 2023, max compression
+gzip compressed data, was "langdash-1.8.1.tar", last modified: Sun Jul 16 04:36:49 2023, max compression
```

## Comparing `langdash-1.8.0.tar` & `langdash-1.8.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.294276 langdash-1.8.0/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.8.0/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.8.0/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3647 2023-07-15 20:32:17.294276 langdash-1.8.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2712 2023-07-08 22:51:09.000000 langdash-1.8.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.286276 langdash-1.8.0/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-15 20:31:59.000000 langdash-1.8.0/langdash/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.290276 langdash-1.8.0/langdash/chains/
--rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.8.0/langdash/chains/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    15394 2023-07-15 19:43:23.000000 langdash-1.8.0/langdash/chains/chains.py
--rw-rw-r--   0 user      (1000) user      (1000)     9603 2023-07-15 19:44:32.000000 langdash-1.8.0/langdash/chains/nodes.py
--rw-rw-r--   0 user      (1000) user      (1000)      310 2023-07-14 19:48:15.000000 langdash-1.8.0/langdash/chains/typing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.282276 langdash-1.8.0/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.8.0/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.8.0/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     7148 2023-07-15 19:11:10.000000 langdash-1.8.0/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)     1359 2023-07-11 02:58:19.000000 langdash-1.8.0/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1661 2023-06-28 07:07:44.000000 langdash-1.8.0/langdash/llm.py
--rw-r--r--   0 user      (1000) user      (1000)      742 2023-07-14 18:46:03.000000 langdash-1.8.0/langdash/llm_config.py
--rw-rw-r--   0 user      (1000) user      (1000)    10076 2023-07-15 19:57:10.000000 langdash-1.8.0/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.290276 langdash-1.8.0/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.8.0/langdash/models/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.290276 langdash-1.8.0/langdash/models/_mixins/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.8.0/langdash/models/_mixins/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3775 2023-07-15 19:49:38.000000 langdash-1.8.0/langdash/models/_mixins/tensor_based_infer_mixin.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.294276 langdash-1.8.0/langdash/models/_tokenizer/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.8.0/langdash/models/_tokenizer/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.8.0/langdash/models/_tokenizer/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     1610 2023-07-15 19:49:38.000000 langdash-1.8.0/langdash/models/_tokenizer/bytes_dict_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     2361 2023-07-15 19:49:38.000000 langdash-1.8.0/langdash/models/_tokenizer/hf_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1622 2023-07-15 19:25:51.000000 langdash-1.8.0/langdash/models/_tokenizer/rwkv_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)      745 2023-07-15 19:49:38.000000 langdash-1.8.0/langdash/models/_tokenizer/tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     6211 2023-07-15 19:49:38.000000 langdash-1.8.0/langdash/models/ctransformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5910 2023-07-15 19:27:43.000000 langdash-1.8.0/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.8.0/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)    12084 2023-07-15 19:49:38.000000 langdash-1.8.0/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.8.0/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5731 2023-07-15 19:49:38.000000 langdash-1.8.0/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      885 2023-07-15 18:57:17.000000 langdash-1.8.0/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.8.0/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.286276 langdash-1.8.0/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.8.0/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.8.0/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.8.0/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.8.0/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-15 20:32:17.290276 langdash-1.8.0/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3647 2023-07-15 20:32:17.000000 langdash-1.8.0/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1677 2023-07-15 20:32:17.000000 langdash-1.8.0/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-15 20:32:17.000000 langdash-1.8.0/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      199 2023-07-15 20:32:17.000000 langdash-1.8.0/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-15 20:32:17.000000 langdash-1.8.0/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-15 20:32:17.294276 langdash-1.8.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.8.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.272795 langdash-1.8.1/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.8.1/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.8.1/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3692 2023-07-16 04:36:49.272795 langdash-1.8.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2757 2023-07-15 21:14:06.000000 langdash-1.8.1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.268795 langdash-1.8.1/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-16 04:36:31.000000 langdash-1.8.1/langdash/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.272795 langdash-1.8.1/langdash/chains/
+-rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.8.1/langdash/chains/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15535 2023-07-16 04:30:12.000000 langdash-1.8.1/langdash/chains/chains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9603 2023-07-15 19:44:32.000000 langdash-1.8.1/langdash/chains/nodes.py
+-rw-rw-r--   0 user      (1000) user      (1000)      310 2023-07-14 19:48:15.000000 langdash-1.8.1/langdash/chains/typing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.268795 langdash-1.8.1/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.8.1/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.8.1/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7148 2023-07-15 19:11:10.000000 langdash-1.8.1/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1359 2023-07-11 02:58:19.000000 langdash-1.8.1/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1661 2023-06-28 07:07:44.000000 langdash-1.8.1/langdash/llm.py
+-rw-r--r--   0 user      (1000) user      (1000)      742 2023-07-14 18:46:03.000000 langdash-1.8.1/langdash/llm_config.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10215 2023-07-16 03:36:19.000000 langdash-1.8.1/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.272795 langdash-1.8.1/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.8.1/langdash/models/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.272795 langdash-1.8.1/langdash/models/_mixins/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.8.1/langdash/models/_mixins/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3775 2023-07-15 19:49:38.000000 langdash-1.8.1/langdash/models/_mixins/tensor_based_infer_mixin.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.272795 langdash-1.8.1/langdash/models/_tokenizer/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.8.1/langdash/models/_tokenizer/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.8.1/langdash/models/_tokenizer/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1610 2023-07-15 19:49:38.000000 langdash-1.8.1/langdash/models/_tokenizer/bytes_dict_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2361 2023-07-15 19:49:38.000000 langdash-1.8.1/langdash/models/_tokenizer/hf_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1622 2023-07-15 19:25:51.000000 langdash-1.8.1/langdash/models/_tokenizer/rwkv_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)      745 2023-07-15 19:49:38.000000 langdash-1.8.1/langdash/models/_tokenizer/tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6321 2023-07-16 03:31:46.000000 langdash-1.8.1/langdash/models/ctransformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6020 2023-07-16 03:31:55.000000 langdash-1.8.1/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.8.1/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12152 2023-07-16 03:31:48.000000 langdash-1.8.1/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.8.1/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5799 2023-07-16 03:32:00.000000 langdash-1.8.1/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      885 2023-07-15 18:57:17.000000 langdash-1.8.1/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.8.1/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.268795 langdash-1.8.1/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.8.1/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.8.1/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.8.1/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.8.1/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.268795 langdash-1.8.1/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3692 2023-07-16 04:36:49.000000 langdash-1.8.1/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1677 2023-07-16 04:36:49.000000 langdash-1.8.1/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-16 04:36:49.000000 langdash-1.8.1/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      199 2023-07-16 04:36:49.000000 langdash-1.8.1/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-16 04:36:49.000000 langdash-1.8.1/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-16 04:36:49.272795 langdash-1.8.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.8.1/setup.py
```

### Comparing `langdash-1.8.0/LICENSE.txt` & `langdash-1.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/PKG-INFO` & `langdash-1.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.8.0
+Version: 1.8.1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
@@ -26,16 +26,16 @@
 # langdash
 
 A simple library for interfacing with language models.
 
 **Currently in beta!**
 
 **Features:**
-  
-  * Support for text generation, text classification (through prompting) and vector-based document searching.
+
+  * Support for guided text generation, text classification (through prompting) and vector-based document searching.
   * Lightweight, build-it-yourself-style prompt wrappers.
   * Token healing and transformers/RNN state reuse for fast inference, like in [Microsoft's guidance](https://github.com/microsoft/guidance).
   * First-class support for ggml backends.
 
 **Documentation:** [Read on readthedocs.io](https://langdash.readthedocs.io/en/latest/)
 
 **Repository:** [main](https://git.mysymphony.jp.net/nana/langdash/) / [Gitlab mirror](https://gitlab.com/nanamochizuki77/langdash)
@@ -49,15 +49,15 @@
 ```
 
 List of modules:
   
   * **core:**
     * *embeddings:* required for running searching through embeddings
   * **backends:**
-    * Generation backends: *rwkv_cpp*, *llama_cpp*, *ctransformers* (alpha), *transformers*
+    * Generation backends: *rwkv_cpp*, *llama_cpp*, *ctransformers*, *transformers*
     * Embedding backends: *sentence_transformers*
 
 **Note:** If running from source, initialize the git submodules in the `langdash/extern` folder to compile foreign backends.
     
 ## Usage
 
 Examples:
@@ -78,17 +78,19 @@
 
 You can specify additional model parameters using the `-ae` CLI argument, and passing a valid Python literal. For example, to run the chat example using the WizardLM model with context length of 4096, do:
 
 ```
 python examples/chat.py llama_cpp /path/to/ggml-wizardlm.bin -ae n_ctx 4096
 ```
 
-Some examples require you to specify the prompt format. Currently, two are implemented: `wizardlm` (shortened Alpaca format without the first prompt line and `# Instruction:`), and `alpaca` (the full format). You will need to specify it for most of the examples:
+Some examples require you to specify the prompt format. Formats include: `wizardlm` (shortened Alpaca format without the first prompt line and `# Instruction:`), and `alpaca` (the full format). You will need to specify it for most of the examples:
 
 ```
 python examples/instruct.py llama_cpp /path/to/ggml-wizardlm.bin -ae n_ctx 4096 --prompt-format wizardlm
 ```
 
+For a full list, see the `examples/_instruct_format.py` file.
+
 
 ## License
 
 Apache 2.0
```

### Comparing `langdash-1.8.0/README.md` & `langdash-1.8.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # langdash
 
 A simple library for interfacing with language models.
 
 **Currently in beta!**
 
 **Features:**
-  
-  * Support for text generation, text classification (through prompting) and vector-based document searching.
+
+  * Support for guided text generation, text classification (through prompting) and vector-based document searching.
   * Lightweight, build-it-yourself-style prompt wrappers.
   * Token healing and transformers/RNN state reuse for fast inference, like in [Microsoft's guidance](https://github.com/microsoft/guidance).
   * First-class support for ggml backends.
 
 **Documentation:** [Read on readthedocs.io](https://langdash.readthedocs.io/en/latest/)
 
 **Repository:** [main](https://git.mysymphony.jp.net/nana/langdash/) / [Gitlab mirror](https://gitlab.com/nanamochizuki77/langdash)
@@ -24,15 +24,15 @@
 ```
 
 List of modules:
   
   * **core:**
     * *embeddings:* required for running searching through embeddings
   * **backends:**
-    * Generation backends: *rwkv_cpp*, *llama_cpp*, *ctransformers* (alpha), *transformers*
+    * Generation backends: *rwkv_cpp*, *llama_cpp*, *ctransformers*, *transformers*
     * Embedding backends: *sentence_transformers*
 
 **Note:** If running from source, initialize the git submodules in the `langdash/extern` folder to compile foreign backends.
     
 ## Usage
 
 Examples:
@@ -53,17 +53,19 @@
 
 You can specify additional model parameters using the `-ae` CLI argument, and passing a valid Python literal. For example, to run the chat example using the WizardLM model with context length of 4096, do:
 
 ```
 python examples/chat.py llama_cpp /path/to/ggml-wizardlm.bin -ae n_ctx 4096
 ```
 
-Some examples require you to specify the prompt format. Currently, two are implemented: `wizardlm` (shortened Alpaca format without the first prompt line and `# Instruction:`), and `alpaca` (the full format). You will need to specify it for most of the examples:
+Some examples require you to specify the prompt format. Formats include: `wizardlm` (shortened Alpaca format without the first prompt line and `# Instruction:`), and `alpaca` (the full format). You will need to specify it for most of the examples:
 
 ```
 python examples/instruct.py llama_cpp /path/to/ggml-wizardlm.bin -ae n_ctx 4096 --prompt-format wizardlm
 ```
 
+For a full list, see the `examples/_instruct_format.py` file.
+
 
 ## License
 
 Apache 2.0
```

### Comparing `langdash-1.8.0/langdash/chains/chains.py` & `langdash-1.8.1/langdash/chains/chains.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,36 +202,42 @@
       if isinstance(node, LDReturns):
         text = ""
         for resp in generator:
           assert isinstance(resp, RespInfer)
           text = resp.running_infer
           if resp.tokid != -1:
             result.completion_tokens += 1
-        result.returns[node._returns] = text
+        result.returns[node._returns] = self._returns[node._returns](text)
 
       elif isinstance(node, LDChoice):
         resp = next(generator)
         assert isinstance(resp, RespInfer)
-        result.returns[node._returns] = resp.running_infer
+        result.returns[node._returns] = self._returns[node._returns](
+          resp.running_infer
+        )
 
         resp = next(generator)
         assert isinstance(resp, RespInject)
         result.completion_tokens += resp.tokens_counter
 
       elif isinstance(node, LDRepeat):
         text = ""
+        result_list = []
+
         for resp in generator:
           assert isinstance(resp, RespInfer)
           text = resp.running_infer
           if resp.tokid != -1:
             result.completion_tokens += 1
           else:
-            result.returns[node._append_target].append(text)
+            result_list.append(text)
             text = ""
 
+        result.returns[node._append_target] = result_list
+
       else:
         for resp in generator:
           if isinstance(resp, RespInject):
             result.prompt_tokens += resp.tokens_counter
           else:
             raise NotImplementedError(resp.__class__.__name__)
```

### Comparing `langdash-1.8.0/langdash/chains/nodes.py` & `langdash-1.8.1/langdash/chains/nodes.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/classify/token_qa.py` & `langdash-1.8.1/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/core.py` & `langdash-1.8.1/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/infer.py` & `langdash-1.8.1/langdash/infer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/llm.py` & `langdash-1.8.1/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/llm_config.py` & `langdash-1.8.1/langdash/llm_config.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/llm_session.py` & `langdash-1.8.1/langdash/llm_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,20 @@
     self.default_infer_args = default_infer_args
     self.called_nodes = ([] if track_called_nodes else None)
     self.token_healing = token_healing
     self._tokens_counter = 0
     self.tokens_used = 0
     self.event_handlers = event_handlers
 
+  def _reset_state(self):
+    if self.called_nodes:
+      self.called_nodes.clear()
+    self._tokens_counter = 0
+    self.tokens_used = 0
+
   def set_state(self, state: Optional[T_LLMState]):
     """
     Set the state of the language model.
 
     Args:
       state (Optional[T_LLMState]):
         The state of the language model, or None to clear the state.
```

### Comparing `langdash-1.8.0/langdash/models/_mixins/tensor_based_infer_mixin.py` & `langdash-1.8.1/langdash/models/_mixins/tensor_based_infer_mixin.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/models/_tokenizer/_bpe.py` & `langdash-1.8.1/langdash/models/_tokenizer/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/models/_tokenizer/bytes_dict_tokenizer.py` & `langdash-1.8.1/langdash/models/_tokenizer/bytes_dict_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/models/_tokenizer/hf_tokenizer.py` & `langdash-1.8.1/langdash/models/_tokenizer/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/models/_tokenizer/rwkv_tokenizer.py` & `langdash-1.8.1/langdash/models/_tokenizer/rwkv_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/models/_tokenizer/tokenizer.py` & `langdash-1.8.1/langdash/models/_tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/models/ctransformers.py` & `langdash-1.8.1/langdash/models/ctransformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Optional, Any, Mapping
 import weakref
 import torch
 
 from langdash.llm import LLM
 from langdash.llm_config import LLMConfig
-from langdash.llm_session import LLMGenerationSessionForRawText
+from langdash.llm_session import LLMGenerationSession, LLMGenerationSessionForRawText
 import langdash.sampling as sampling
 from ._tokenizer.tokenizer import Tokenizer
 from ._tokenizer.bytes_dict_tokenizer import BytesDictTokenizer
 from ._tokenizer.hf_tokenizer import HFTokenizer
 from ._mixins.tensor_based_infer_mixin import TensorBasedInferWithSessionMixin
 
 import ctransformers  # type: ignore
@@ -130,18 +130,20 @@
   def next_token_logits(self) -> List[float]:
     return self._next_token_logits_raw().tolist()
 
   def next_token_probs(self) -> List[float]:
     return sampling.logits_to_probs(self._next_token_logits_raw()).tolist()
 
   def set_state(self, state: Optional[CTransformersState]):
-    self._model.set_state(self, state)
     if state is None:
+      self._model.set_state(self, None)
       self._logits = None
+      LLMGenerationSession._reset_state(self)
     else:
+      self._model.set_state(self, state)
       self._logits = self._model.load_logits_from_model()
 
   def clone_state(self) -> CTransformersState:
     return self._model.clone_state(self)
 
   def get_context_length(self) -> int:
     return self._model.get_context_length(self)
```

### Comparing `langdash-1.8.0/langdash/models/llama_cpp.py` & `langdash-1.8.1/langdash/models/llama_cpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional, Mapping
 import weakref
 import torch
 from llama_cpp import Llama, LlamaState, llama_token_to_str  # type: ignore
 
 from langdash.llm import LLM
 from langdash.llm_config import LLMConfig
-from langdash.llm_session import LLMGenerationSessionForRawText
+from langdash.llm_session import LLMGenerationSession, LLMGenerationSessionForRawText
 import langdash.sampling as sampling
 from ._tokenizer.bytes_dict_tokenizer import BytesDictTokenizer
 from ._mixins.tensor_based_infer_mixin import TensorBasedInferWithSessionMixin
 
 
 class LlamaWrapper:
   model: Llama
@@ -108,18 +108,20 @@
   def next_token_logits(self) -> List[float]:
     return self._next_token_logits_raw().tolist()
 
   def next_token_probs(self) -> List[float]:
     return sampling.logits_to_probs(self._next_token_logits_raw()).tolist()
 
   def set_state(self, state: Optional[LlamaState]):
-    self._model.set_state(self, state)
     if state is None:
+      self._model.set_state(self, None)
       self._logits = None
+      LLMGenerationSession._reset_state(self)
     else:
+      self._model.set_state(self, state)
       self._logits = self._model.load_logits_from_llama()
 
   def clone_state(self) -> LlamaState:
     return self._model.clone_state(self)
 
   def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
     return self._model.tokenizer.encode(
```

### Comparing `langdash-1.8.0/langdash/models/mock.py` & `langdash-1.8.1/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/models/rwkv_cpp.py` & `langdash-1.8.1/langdash/models/rwkv_cpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import sys
 import torch
 import tokenizers  # type: ignore
 
 from langdash.llm import LLM
 from langdash.llm_config import LLMConfig
-from langdash.llm_session import LLMGenerationSessionForRawText, LLMState
+from langdash.llm_session import LLMGenerationSession, LLMGenerationSessionForRawText, LLMState
 import langdash.sampling as sampling
 from ._mixins.tensor_based_infer_mixin import TensorBasedInferMixin
 
 _rwkv_lib: Optional[str] = None
 _rwkv_cpp_folder: Optional[str] = None
 
 RWKV_CPP_COMMIT_DEFAULT = "84634c047a9831b16cdf1cc3f2626e0ef0b2373b"
@@ -255,14 +255,15 @@
     # FIXME: mypy does not infer self._logits to not be None
     return self._logits  # type: ignore
 
   def set_state(self, state: Optional[RwkvCppState]):
     if state is None:
       self._logits, self._state = None, None
       self._next_token = None
+      LLMGenerationSession._reset_state(self)
     else:
       self._logits = copy.deepcopy(state._logits)
       self._state = copy.deepcopy(state._state)
       self._next_token = state._next_token
 
   def clone_state(self) -> RwkvCppState:
     return RwkvCppState(
```

### Comparing `langdash-1.8.0/langdash/models/sentence_transformers.py` & `langdash-1.8.1/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/models/transformers.py` & `langdash-1.8.1/langdash/models/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Optional, Tuple, Union, Any, Mapping
 from dataclasses import dataclass
 import copy
 
 from langdash.llm import LLM
-from langdash.llm_session import LLMGenerationSessionForRawText, LLMState
+from langdash.llm_session import LLMGenerationSession, LLMGenerationSessionForRawText, LLMState
 import langdash.sampling as sampling
 from ._tokenizer.hf_tokenizer import HFTokenizer
 from ._mixins.tensor_based_infer_mixin import TensorBasedInferMixin
 
 import transformers  # type: ignore
 import torch
 
@@ -91,14 +91,15 @@
     self._next_token = None
 
   def set_state(self, state: Optional[TransformersState]):
     if state is None:
       self._logits = None
       self._state = None
       self._next_token = None
+      LLMGenerationSession._reset_state(self)
     else:
       self._logits = copy.deepcopy(state._logits)
       self._state = copy.deepcopy(state._state)
       self._next_token = state._next_token
 
   def clone_state(self) -> TransformersState:
     return TransformersState(
```

### Comparing `langdash-1.8.0/langdash/response.py` & `langdash-1.8.1/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/sampling.py` & `langdash-1.8.1/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/search/embedding_search.py` & `langdash-1.8.1/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/search/engine.py` & `langdash-1.8.1/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash/search/multichoice_search.py` & `langdash-1.8.1/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/langdash.egg-info/PKG-INFO` & `langdash-1.8.1/langdash.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.8.0
+Version: 1.8.1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
@@ -26,16 +26,16 @@
 # langdash
 
 A simple library for interfacing with language models.
 
 **Currently in beta!**
 
 **Features:**
-  
-  * Support for text generation, text classification (through prompting) and vector-based document searching.
+
+  * Support for guided text generation, text classification (through prompting) and vector-based document searching.
   * Lightweight, build-it-yourself-style prompt wrappers.
   * Token healing and transformers/RNN state reuse for fast inference, like in [Microsoft's guidance](https://github.com/microsoft/guidance).
   * First-class support for ggml backends.
 
 **Documentation:** [Read on readthedocs.io](https://langdash.readthedocs.io/en/latest/)
 
 **Repository:** [main](https://git.mysymphony.jp.net/nana/langdash/) / [Gitlab mirror](https://gitlab.com/nanamochizuki77/langdash)
@@ -49,15 +49,15 @@
 ```
 
 List of modules:
   
   * **core:**
     * *embeddings:* required for running searching through embeddings
   * **backends:**
-    * Generation backends: *rwkv_cpp*, *llama_cpp*, *ctransformers* (alpha), *transformers*
+    * Generation backends: *rwkv_cpp*, *llama_cpp*, *ctransformers*, *transformers*
     * Embedding backends: *sentence_transformers*
 
 **Note:** If running from source, initialize the git submodules in the `langdash/extern` folder to compile foreign backends.
     
 ## Usage
 
 Examples:
@@ -78,17 +78,19 @@
 
 You can specify additional model parameters using the `-ae` CLI argument, and passing a valid Python literal. For example, to run the chat example using the WizardLM model with context length of 4096, do:
 
 ```
 python examples/chat.py llama_cpp /path/to/ggml-wizardlm.bin -ae n_ctx 4096
 ```
 
-Some examples require you to specify the prompt format. Currently, two are implemented: `wizardlm` (shortened Alpaca format without the first prompt line and `# Instruction:`), and `alpaca` (the full format). You will need to specify it for most of the examples:
+Some examples require you to specify the prompt format. Formats include: `wizardlm` (shortened Alpaca format without the first prompt line and `# Instruction:`), and `alpaca` (the full format). You will need to specify it for most of the examples:
 
 ```
 python examples/instruct.py llama_cpp /path/to/ggml-wizardlm.bin -ae n_ctx 4096 --prompt-format wizardlm
 ```
 
+For a full list, see the `examples/_instruct_format.py` file.
+
 
 ## License
 
 Apache 2.0
```

### Comparing `langdash-1.8.0/langdash.egg-info/SOURCES.txt` & `langdash-1.8.1/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.8.0/setup.py` & `langdash-1.8.1/setup.py`

 * *Files identical despite different names*

