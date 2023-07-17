# Comparing `tmp/zeno_build-0.0.3.tar.gz` & `tmp/zeno_build-0.0.4.tar.gz`

## Comparing `zeno_build-0.0.3.tar` & `zeno_build-0.0.4.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/__init__.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/cache_utils.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/version.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/__init__.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/audio_metrics/__init__.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/audio_metrics/error.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/code_metrics/__init__.py
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/code_metrics/execution_accuracy.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/code_metrics/execution_accuracy_utils.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_features/__init__.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_features/capitalization.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_features/clustering.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_features/exact_match.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_features/frequency.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_features/length.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_features/numbers.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_metrics/__init__.py
--rw-r--r--   0        0        0    16437 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_metrics/critique.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_tokenizers/__init__.py
--rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_tokenizers/unicode.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/experiments/__init__.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/experiments/experiment_run.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/experiments/search_space.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/__init__.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/chat_generate.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/dataset_config.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/global_models.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/lm_config.py
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/text_generate.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/providers/__init__.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/providers/cohere_utils.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/providers/huggingface_utils.py
--rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/providers/openai_utils.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/optimizers/__init__.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/optimizers/base.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/optimizers/exhaustive.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/optimizers/random.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/optimizers/standard.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/optimizers/vizier.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/prompts/__init__.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/prompts/chat_prompt.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/prompts/prompt_utils.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/reporting/__init__.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/reporting/aggregate_results.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/reporting/reporting_utils.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/reporting/visualize.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 zeno_build-0.0.3/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zeno_build-0.0.3/LICENSE
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 zeno_build-0.0.3/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 zeno_build-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 zeno_build-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/__init__.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/cache_utils.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/version.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/__init__.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/audio_metrics/__init__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/audio_metrics/error.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/code_metrics/__init__.py
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/code_metrics/execution_accuracy.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/code_metrics/execution_accuracy_utils.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_features/__init__.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_features/capitalization.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_features/clustering.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_features/exact_match.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_features/frequency.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_features/length.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_features/numbers.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_metrics/__init__.py
+-rw-r--r--   0        0        0    16437 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_metrics/critique.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_tokenizers/__init__.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_tokenizers/unicode.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/experiments/__init__.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/experiments/experiment_run.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/experiments/search_space.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/__init__.py
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/chat_generate.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/dataset_config.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/global_models.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/lm_config.py
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/text_generate.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/providers/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/providers/cohere_utils.py
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/providers/huggingface_utils.py
+-rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/providers/openai_utils.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/providers/vllm_utils.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/optimizers/__init__.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/optimizers/base.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/optimizers/exhaustive.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/optimizers/random.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/optimizers/standard.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/optimizers/vizier.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/prompts/__init__.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/prompts/chat_prompt.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/prompts/prompt_utils.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/reporting/__init__.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/reporting/aggregate_results.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/reporting/reporting_utils.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/reporting/visualize.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 zeno_build-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zeno_build-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 zeno_build-0.0.4/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zeno_build-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 zeno_build-0.0.4/PKG-INFO
```

### Comparing `zeno_build-0.0.3/zeno_build/cache_utils.py` & `zeno_build-0.0.4/zeno_build/cache_utils.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/evaluation/audio_metrics/error.py` & `zeno_build-0.0.4/zeno_build/evaluation/audio_metrics/error.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/evaluation/code_metrics/execution_accuracy.py` & `zeno_build-0.0.4/zeno_build/evaluation/code_metrics/execution_accuracy.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/evaluation/code_metrics/execution_accuracy_utils.py` & `zeno_build-0.0.4/zeno_build/evaluation/code_metrics/execution_accuracy_utils.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/evaluation/text_features/capitalization.py` & `zeno_build-0.0.4/zeno_build/evaluation/text_features/capitalization.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/evaluation/text_features/clustering.py` & `zeno_build-0.0.4/zeno_build/evaluation/text_features/clustering.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     """Cluster the labels together to find similar sentences.
 
     Args:
         df: Zeno DataFrame
         ops: Zeno options
 
     Returns:
-        DistillReturn: Number of digits in the output
+        DistillReturn: Cluster IDs of each of the input data points
     """
     documents = [str(x) for x in df[ops.data_column]]
     # TODO(gneubig): having something like the sqrt of the number of documents seems
     #   like a good number of clusters, but more than 20 are not supported in Zeno:
     #   https://github.com/zeno-ml/zeno/issues/873
     # num_clusters = int(math.sqrt(len(documents)))
     num_clusters = 20
@@ -56,15 +56,15 @@
     """Cluster the labels together to find similar sentences.
 
     Args:
         df: Zeno DataFrame
         ops: Zeno options
 
     Returns:
-        DistillReturn: Number of digits in the output
+        DistillReturn: Cluster IDs of each of the labels
     """
     documents = [str(x) for x in df[ops.label_column]]
     # TODO(gneubig): having something like the sqrt of the number of documents seems
     #   like a good number of clusters, but more than 20 are not supported in Zeno:
     #   https://github.com/zeno-ml/zeno/issues/873
     # num_clusters = int(math.sqrt(len(documents)))
     num_clusters = 20
```

### Comparing `zeno_build-0.0.3/zeno_build/evaluation/text_features/exact_match.py` & `zeno_build-0.0.4/zeno_build/evaluation/text_features/exact_match.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/evaluation/text_features/frequency.py` & `zeno_build-0.0.4/zeno_build/evaluation/text_features/frequency.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/evaluation/text_features/length.py` & `zeno_build-0.0.4/zeno_build/evaluation/text_features/length.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/evaluation/text_features/numbers.py` & `zeno_build-0.0.4/zeno_build/evaluation/text_features/numbers.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/evaluation/text_metrics/critique.py` & `zeno_build-0.0.4/zeno_build/evaluation/text_metrics/critique.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/evaluation/text_tokenizers/unicode.py` & `zeno_build-0.0.4/zeno_build/evaluation/text_tokenizers/unicode.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/experiments/search_space.py` & `zeno_build-0.0.4/zeno_build/experiments/search_space.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/models/chat_generate.py` & `zeno_build-0.0.4/zeno_build/models/chat_generate.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,17 +4,33 @@
 from zeno_build.models import lm_config
 from zeno_build.models.providers.cohere_utils import generate_from_cohere
 from zeno_build.models.providers.huggingface_utils import generate_from_huggingface
 from zeno_build.models.providers.openai_utils import (
     generate_from_openai_chat_completion,
     generate_from_openai_completion,
 )
+from zeno_build.models.providers.vllm_utils import generate_from_vllm
 from zeno_build.prompts import chat_prompt
 
 
+def _contexts_to_prompts(
+    full_contexts: list[chat_prompt.ChatMessages],
+    prompt_template: chat_prompt.ChatMessages,
+    model_config: lm_config.LMConfig,
+    context_length: int,
+) -> list[str]:
+    return [
+        prompt_template.to_text_prompt(
+            full_context=full_context.limit_length(context_length),
+            name_replacements=model_config.name_replacements,
+        )
+        for full_context in full_contexts
+    ]
+
+
 def generate_from_chat_prompt(
     full_contexts: list[chat_prompt.ChatMessages],
     prompt_template: chat_prompt.ChatMessages,
     model_config: lm_config.LMConfig,
     temperature: float,
     max_tokens: int,
     top_p: float,
@@ -39,21 +55,21 @@
     print(
         f"Generating with {prompt_template=}, {model_config.model=}, "
         f"{temperature=}, {max_tokens=}, {top_p=}, {context_length=}..."
     )
     if model_config.provider == "openai":
         return asyncio.run(
             generate_from_openai_completion(
-                full_contexts,
-                prompt_template,
+                _contexts_to_prompts(
+                    full_contexts, prompt_template, model_config, context_length
+                ),
                 model_config,
                 temperature,
                 max_tokens,
                 top_p,
-                context_length,
                 requests_per_minute,
             )
         )
     elif model_config.provider == "openai_chat":
         return asyncio.run(
             generate_from_openai_chat_completion(
                 full_contexts,
@@ -65,29 +81,39 @@
                 context_length,
                 requests_per_minute,
             )
         )
     elif model_config.provider == "cohere":
         return asyncio.run(
             generate_from_cohere(
-                full_contexts,
-                prompt_template,
+                _contexts_to_prompts(
+                    full_contexts, prompt_template, model_config, context_length
+                ),
                 model_config,
                 temperature,
                 max_tokens,
                 top_p,
-                context_length,
                 requests_per_minute,
             )
         )
     elif model_config.provider == "huggingface":
         return generate_from_huggingface(
-            full_contexts,
-            prompt_template,
+            _contexts_to_prompts(
+                full_contexts, prompt_template, model_config, context_length
+            ),
+            model_config,
+            temperature,
+            max_tokens,
+            top_p,
+        )
+    elif model_config.provider == "vllm":
+        return generate_from_vllm(
+            _contexts_to_prompts(
+                full_contexts, prompt_template, model_config, context_length
+            ),
             model_config,
             temperature,
             max_tokens,
             top_p,
-            context_length,
         )
     else:
         raise ValueError("Unknown provider, but you can add your own!")
```

### Comparing `zeno_build-0.0.3/zeno_build/models/dataset_config.py` & `zeno_build-0.0.4/zeno_build/models/dataset_config.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/models/lm_config.py` & `zeno_build-0.0.4/zeno_build/models/lm_config.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/models/text_generate.py` & `zeno_build-0.0.4/zeno_build/models/text_generate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,84 +1,95 @@
 """Generate from a textual prompt."""
 
 import asyncio
 
-import openai
 import tqdm
 
 from zeno_build.models import global_models, lm_config
-from zeno_build.models.providers.huggingface_utils import text_generate_from_huggingface
+from zeno_build.models.providers.huggingface_utils import generate_from_huggingface
+from zeno_build.models.providers.openai_utils import (
+    generate_from_openai_chat_completion,
+    generate_from_openai_completion,
+)
+from zeno_build.prompts.chat_prompt import ChatMessages, ChatTurn
 from zeno_build.prompts.prompt_utils import replace_variables
 
 
-async def generate_from_text_prompt(
+def generate_from_text_prompt(
     variables: list[dict[str, str]],
     prompt_template: str,
     model_config: lm_config.LMConfig,
     temperature: float,
     max_tokens: int,
     top_p: float,
+    requests_per_minute: int = 150,
 ) -> list[str]:
     """Generate from a textual prompt.
 
     Args:
         variables: The source set of variables to consume.
         prompt_template: The template for the prompt.
         model_config: Configuration of the model.
         temperature: The temperature to use.
         max_tokens: The maximum number of tokens to generate.
         top_p: The top p value to use.
+        requests_per_minute: Limit on the number of OpenAI requests per minute.
 
     Returns:
         The generated text.
     """
     print(
         f"Generating with {prompt_template=}, {model_config.model=}, "
         f"{temperature=}, {max_tokens=}, {top_p=}..."
     )
     if model_config.provider == "huggingface":
-        return text_generate_from_huggingface(
-            variables,
-            prompt_template,
+        prompts = [replace_variables(prompt_template, vars) for vars in variables]
+        return generate_from_huggingface(
+            prompts,
             model_config,
             temperature,
             max_tokens,
             top_p,
         )
     elif model_config.provider == "openai":
-        async_responses = [
-            openai.Completion.acreate(
-                engine=model_config.model,
-                prompt=replace_variables(prompt_template, vars),
-                temperature=temperature,
-                max_tokens=max_tokens,
-                top_p=top_p,
+        prompts = [replace_variables(prompt_template, vars) for vars in variables]
+        return asyncio.run(
+            generate_from_openai_completion(
+                prompts,
+                model_config,
+                temperature,
+                max_tokens,
+                top_p,
+                requests_per_minute,
+            )
+        )
+    elif model_config.provider == "openai_chat":
+        full_contexts = [
+            ChatMessages(
+                [
+                    ChatTurn(
+                        role="user",
+                        content=replace_variables(prompt_template, vars),
+                    )
+                ]
             )
             for vars in variables
         ]
-        responses = await asyncio.gather(*async_responses)
-        return [x["choices"][0]["text"] for x in responses]
-    elif model_config.provider == "openai_chat":
-        async_responses = [
-            openai.ChatCompletion.acreate(
-                model=model_config.model,
-                messages=[
-                    {
-                        "role": "user",
-                        "content": replace_variables(prompt_template, vars),
-                    },
-                ],
+        return asyncio.run(
+            generate_from_openai_chat_completion(
+                full_contexts=full_contexts,
+                prompt_template=ChatMessages([]),
+                model_config=model_config,
                 temperature=temperature,
                 max_tokens=max_tokens,
                 top_p=top_p,
+                context_length=1,
+                requests_per_minute=requests_per_minute,
             )
-            for vars in variables
-        ]
-        responses = await asyncio.gather(*async_responses)
-        return [x["choices"][0]["message"]["content"] for x in responses]
+        )
     elif model_config.provider == "cohere":
         import cohere
 
         results = []
         for vars in tqdm.tqdm(variables, "Generating synchronously from Cohere"):
             try:
                 prompt = replace_variables(prompt_template, vars)
```

### Comparing `zeno_build-0.0.3/zeno_build/models/providers/openai_utils.py` & `zeno_build-0.0.4/zeno_build/models/providers/openai_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,33 +62,29 @@
             except openai.error.APIError as e:
                 logging.warning(f"OpenAI API error: {e}")
                 await asyncio.sleep(10)
         return {"choices": [{"message": {"content": ""}}]}
 
 
 async def generate_from_openai_completion(
-    full_contexts: list[chat_prompt.ChatMessages],
-    prompt_template: chat_prompt.ChatMessages,
+    prompts: list[str],
     model_config: lm_config.LMConfig,
     temperature: float,
     max_tokens: int,
     top_p: float,
-    context_length: int,
     requests_per_minute: int = 150,
 ) -> list[str]:
     """Generate from OpenAI Completion API.
 
     Args:
-        full_contexts: List of full contexts to generate from.
-        prompt_template: Prompt template to use.
+        prompts: List of prompts to generate from.
         model_config: Model configuration.
         temperature: Temperature to use.
         max_tokens: Maximum number of tokens to generate.
         top_p: Top p to use.
-        context_length: Length of context to use.
         requests_per_minute: Number of requests per minute to allow.
 
     Returns:
         List of generated responses.
     """
     if "OPENAI_API_KEY" not in os.environ:
         raise ValueError(
@@ -96,24 +92,21 @@
         )
     openai.api_key = os.environ["OPENAI_API_KEY"]
     openai.aiosession.set(ClientSession())
     limiter = aiolimiter.AsyncLimiter(requests_per_minute)
     async_responses = [
         _throttled_openai_completion_acreate(
             engine=model_config.model,
-            prompt=prompt_template.to_text_prompt(
-                full_context=full_context.limit_length(context_length),
-                name_replacements=model_config.name_replacements,
-            ),
+            prompt=prompt,
             temperature=temperature,
             max_tokens=max_tokens,
             top_p=top_p,
             limiter=limiter,
         )
-        for full_context in full_contexts
+        for prompt in prompts
     ]
     responses = await tqdm_asyncio.gather(*async_responses)
     # Note: will never be none because it's set, but mypy doesn't know that.
     await openai.aiosession.get().close()  # type: ignore
     return [x["choices"][0]["text"] for x in responses]
```

### Comparing `zeno_build-0.0.3/zeno_build/optimizers/base.py` & `zeno_build-0.0.4/zeno_build/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/optimizers/exhaustive.py` & `zeno_build-0.0.4/zeno_build/optimizers/exhaustive.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/optimizers/random.py` & `zeno_build-0.0.4/zeno_build/optimizers/random.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/optimizers/vizier.py` & `zeno_build-0.0.4/zeno_build/optimizers/vizier.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/prompts/chat_prompt.py` & `zeno_build-0.0.4/zeno_build/prompts/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/reporting/aggregate_results.py` & `zeno_build-0.0.4/zeno_build/reporting/aggregate_results.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/reporting/reporting_utils.py` & `zeno_build-0.0.4/zeno_build/reporting/reporting_utils.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/zeno_build/reporting/visualize.py` & `zeno_build-0.0.4/zeno_build/reporting/visualize.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/.gitignore` & `zeno_build-0.0.4/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -134,7 +134,8 @@
 
 # Apple stuff
 .DS_Store
 
 # Experimental results
 results*/
 .zeno_cache/
+zeno_cache/
```

### Comparing `zeno_build-0.0.3/LICENSE` & `zeno_build-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/README.md` & `zeno_build-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.3/pyproject.toml` & `zeno_build-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,20 @@
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 classifiers = [
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
-dependencies = ["aiolimiter>=1.0.0", "inspiredco>=0.0.2", "zenoml>=0.6.1"]
+dependencies = [
+  "aiolimiter>=1.0.0",
+  "inspiredco>=0.0.2",
+  "openai>=0.27.0",
+  "zenoml>=0.6.1",
+]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = ["mypy>=1.2.0", "pre-commit>=3.2.0", "pytest>=6.0.0", "black>=23.3.0"]
 
 [tool.hatch.build]
 include = ["*.py"]
```

### Comparing `zeno_build-0.0.3/PKG-INFO` & `zeno_build-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeno_build
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library for comparing multiple llm-based systems.
 Author-email: Ángel Alexander Cabrera <alex.cabrera@gmail.com>, Graham Neubig <neubig@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Zeno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,14 +27,15 @@
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Requires-Dist: aiolimiter>=1.0.0
 Requires-Dist: inspiredco>=0.0.2
+Requires-Dist: openai>=0.27.0
 Requires-Dist: zenoml>=0.6.1
 Provides-Extra: test
 Requires-Dist: black>=23.3.0; extra == 'test'
 Requires-Dist: mypy>=1.2.0; extra == 'test'
 Requires-Dist: pre-commit>=3.2.0; extra == 'test'
 Requires-Dist: pytest>=6.0.0; extra == 'test'
 Description-Content-Type: text/markdown
```

