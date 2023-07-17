# Comparing `tmp/langdash-1.8.1.tar.gz` & `tmp/langdash-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.8.1.tar", last modified: Sun Jul 16 04:36:49 2023, max compression
+gzip compressed data, was "langdash-1.9.0.tar", last modified: Mon Jul 17 00:13:15 2023, max compression
```

## Comparing `langdash-1.8.1.tar` & `langdash-1.9.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.272795 langdash-1.8.1/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.8.1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.8.1/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3692 2023-07-16 04:36:49.272795 langdash-1.8.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2757 2023-07-15 21:14:06.000000 langdash-1.8.1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.268795 langdash-1.8.1/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-16 04:36:31.000000 langdash-1.8.1/langdash/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.272795 langdash-1.8.1/langdash/chains/
--rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.8.1/langdash/chains/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    15535 2023-07-16 04:30:12.000000 langdash-1.8.1/langdash/chains/chains.py
--rw-rw-r--   0 user      (1000) user      (1000)     9603 2023-07-15 19:44:32.000000 langdash-1.8.1/langdash/chains/nodes.py
--rw-rw-r--   0 user      (1000) user      (1000)      310 2023-07-14 19:48:15.000000 langdash-1.8.1/langdash/chains/typing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.268795 langdash-1.8.1/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.8.1/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.8.1/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     7148 2023-07-15 19:11:10.000000 langdash-1.8.1/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)     1359 2023-07-11 02:58:19.000000 langdash-1.8.1/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1661 2023-06-28 07:07:44.000000 langdash-1.8.1/langdash/llm.py
--rw-r--r--   0 user      (1000) user      (1000)      742 2023-07-14 18:46:03.000000 langdash-1.8.1/langdash/llm_config.py
--rw-rw-r--   0 user      (1000) user      (1000)    10215 2023-07-16 03:36:19.000000 langdash-1.8.1/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.272795 langdash-1.8.1/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.8.1/langdash/models/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.272795 langdash-1.8.1/langdash/models/_mixins/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.8.1/langdash/models/_mixins/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3775 2023-07-15 19:49:38.000000 langdash-1.8.1/langdash/models/_mixins/tensor_based_infer_mixin.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.272795 langdash-1.8.1/langdash/models/_tokenizer/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.8.1/langdash/models/_tokenizer/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.8.1/langdash/models/_tokenizer/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     1610 2023-07-15 19:49:38.000000 langdash-1.8.1/langdash/models/_tokenizer/bytes_dict_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     2361 2023-07-15 19:49:38.000000 langdash-1.8.1/langdash/models/_tokenizer/hf_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1622 2023-07-15 19:25:51.000000 langdash-1.8.1/langdash/models/_tokenizer/rwkv_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)      745 2023-07-15 19:49:38.000000 langdash-1.8.1/langdash/models/_tokenizer/tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     6321 2023-07-16 03:31:46.000000 langdash-1.8.1/langdash/models/ctransformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     6020 2023-07-16 03:31:55.000000 langdash-1.8.1/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.8.1/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)    12152 2023-07-16 03:31:48.000000 langdash-1.8.1/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.8.1/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5799 2023-07-16 03:32:00.000000 langdash-1.8.1/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      885 2023-07-15 18:57:17.000000 langdash-1.8.1/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.8.1/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.268795 langdash-1.8.1/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.8.1/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.8.1/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.8.1/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.8.1/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-16 04:36:49.268795 langdash-1.8.1/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3692 2023-07-16 04:36:49.000000 langdash-1.8.1/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1677 2023-07-16 04:36:49.000000 langdash-1.8.1/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-16 04:36:49.000000 langdash-1.8.1/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      199 2023-07-16 04:36:49.000000 langdash-1.8.1/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-16 04:36:49.000000 langdash-1.8.1/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-16 04:36:49.272795 langdash-1.8.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.8.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.677788 langdash-1.9.0/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.9.0/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.9.0/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3692 2023-07-17 00:13:15.677788 langdash-1.9.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2757 2023-07-15 21:14:06.000000 langdash-1.9.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.673788 langdash-1.9.0/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-17 00:12:51.000000 langdash-1.9.0/langdash/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.677788 langdash-1.9.0/langdash/chains/
+-rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.9.0/langdash/chains/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16150 2023-07-17 00:09:43.000000 langdash-1.9.0/langdash/chains/chains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9610 2023-07-17 00:04:17.000000 langdash-1.9.0/langdash/chains/nodes.py
+-rw-rw-r--   0 user      (1000) user      (1000)      310 2023-07-14 19:48:15.000000 langdash-1.9.0/langdash/chains/typing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.673788 langdash-1.9.0/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.9.0/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.9.0/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7148 2023-07-15 19:11:10.000000 langdash-1.9.0/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1359 2023-07-11 02:58:19.000000 langdash-1.9.0/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1677 2023-07-16 21:41:28.000000 langdash-1.9.0/langdash/llm.py
+-rw-r--r--   0 user      (1000) user      (1000)      742 2023-07-14 18:46:03.000000 langdash-1.9.0/langdash/llm_config.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10233 2023-07-16 21:47:08.000000 langdash-1.9.0/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.677788 langdash-1.9.0/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.9.0/langdash/models/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.677788 langdash-1.9.0/langdash/models/_mixins/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.9.0/langdash/models/_mixins/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3775 2023-07-15 19:49:38.000000 langdash-1.9.0/langdash/models/_mixins/tensor_based_infer_mixin.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.677788 langdash-1.9.0/langdash/models/_tokenizer/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.9.0/langdash/models/_tokenizer/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.9.0/langdash/models/_tokenizer/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1610 2023-07-15 19:49:38.000000 langdash-1.9.0/langdash/models/_tokenizer/bytes_dict_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2361 2023-07-15 19:49:38.000000 langdash-1.9.0/langdash/models/_tokenizer/hf_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1622 2023-07-15 19:25:51.000000 langdash-1.9.0/langdash/models/_tokenizer/rwkv_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)      745 2023-07-15 19:49:38.000000 langdash-1.9.0/langdash/models/_tokenizer/tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6321 2023-07-16 03:31:46.000000 langdash-1.9.0/langdash/models/ctransformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6020 2023-07-16 03:31:55.000000 langdash-1.9.0/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.9.0/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14583 2023-07-17 00:04:17.000000 langdash-1.9.0/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1031 2023-07-16 21:47:08.000000 langdash-1.9.0/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5799 2023-07-16 03:32:00.000000 langdash-1.9.0/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      885 2023-07-15 18:57:17.000000 langdash-1.9.0/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.9.0/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.673788 langdash-1.9.0/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.9.0/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.9.0/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.9.0/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.9.0/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.673788 langdash-1.9.0/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3692 2023-07-17 00:13:15.000000 langdash-1.9.0/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1677 2023-07-17 00:13:15.000000 langdash-1.9.0/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-17 00:13:15.000000 langdash-1.9.0/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      199 2023-07-17 00:13:15.000000 langdash-1.9.0/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-17 00:13:15.000000 langdash-1.9.0/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-17 00:13:15.677788 langdash-1.9.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.9.0/setup.py
```

### Comparing `langdash-1.8.1/LICENSE.txt` & `langdash-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/PKG-INFO` & `langdash-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.8.1
+Version: 1.9.0
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langdash-1.8.1/README.md` & `langdash-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/chains/chains.py` & `langdash-1.9.0/langdash/chains/chains.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass
 from collections import OrderedDict
+import typing
 from typing import Generator, Dict, Any, List, Union, Optional, Tuple, FrozenSet, Set, TYPE_CHECKING, cast
 import re
 import copy
 import warnings
 
 from langdash.response import Response, RespInfer, RespInject, RespReturns
 from .nodes import LDNode, LDText, LDFormatArg, LDArg, LDReturns, LDChoice, LDRepeat
@@ -115,24 +116,34 @@
       if isinstance(node, str):
         pp_nodes.append(self._ld.text(node))
       elif isinstance(node, LDFormatArg):
         _preprocess_format_arg(node)
       else:
         pp_nodes.append(node)
 
-    # argument/return checking
+    # variable/type checking
     for node in nodes:
       if isinstance(node, LDArg):
         if node._arg not in self._args:
           raise ValueError(f"'{node._arg}' not found in argument declaration")
-      elif isinstance(node, (LDReturns, LDChoice)):
+      elif isinstance(node, LDChoice):
         if node._returns not in self._returns:
           raise ValueError(
             f"'{node._returns}' not found in return declaration"
           )
+      elif isinstance(node, LDRepeat):
+        if node._append_target not in self._returns:
+          raise ValueError(
+            f"'{node._append_target}' not found in return declaration"
+          )
+        rettype = self._returns[node._append_target]
+        if rettype is not list or typing.get_origin(rettype) is not list:
+          raise TypeError(
+            f"return type of '{node._append_target}' should be a list"
+          )
 
     # fuse text nodes
     for i in range(len(pp_nodes)):
       pp_node_i = pp_nodes[i]
       if isinstance(pp_node_i, LDText):
         for j in range(i + 1, len(pp_nodes)):
           pp_node_j = pp_nodes[j]
@@ -228,16 +239,19 @@
           text = resp.running_infer
           if resp.tokid != -1:
             result.completion_tokens += 1
           else:
             result_list.append(text)
             text = ""
 
-        result.returns[node._append_target] = result_list
-
+        rettype = self._returns[node._append_target]
+        if rettype is list:
+          result.returns[node._append_target] = result_list
+        else:
+          result.returns[node._append_target] = list(map(rettype, result_list))
       else:
         for resp in generator:
           if isinstance(resp, RespInject):
             result.prompt_tokens += resp.tokens_counter
           else:
             raise NotImplementedError(resp.__class__.__name__)
```

### Comparing `langdash-1.8.1/langdash/chains/nodes.py` & `langdash-1.9.0/langdash/chains/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,16 +220,17 @@
       try:
         choices = args[self._choices]
       except KeyError:
         raise KeyError(
           f"Expected \"{self._choices}\" argument to be passed into chain."
         )
 
-      if not isinstance(choices, list) or not all(
-        isinstance(choice, str) for choice in choices
+      if not (
+        isinstance(choices, list) and
+        all(isinstance(choice, str) for choice in choices)
       ):
         raise TypeError(f"Expected \"{self._choices}\" to be List[str]")
 
       cache = self._get_token_cache_once(
         session, heal_prefix, self._preprocess_choices(choices)
       )
     else:  # List[str]
```

### Comparing `langdash-1.8.1/langdash/classify/token_qa.py` & `langdash-1.9.0/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/core.py` & `langdash-1.9.0/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/infer.py` & `langdash-1.9.0/langdash/infer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/llm.py` & `langdash-1.9.0/langdash/llm.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,21 +42,23 @@
         Event handlers for prompt events. Defaults to `None`.
 
     Returns:
       A new session object.
     """
     return self.__class__.Session(llm=self, *args, **kwargs)
 
-  def get_capability(self) -> LLMCapability:
+  @property
+  def capability(self) -> LLMCapability:
     """
     Returns the capability of the language model.
     """
     return LLMCapability.Generative
 
 
 class EmbeddingLLM(LLM[T_LLMEmbeddingSession]):
   """
   A language model class for generating embeddings.
   """
 
-  def get_capability(self) -> LLMCapability:
+  @property
+  def capability(self) -> LLMCapability:
     return LLMCapability.Embedding
```

### Comparing `langdash-1.8.1/langdash/llm_config.py` & `langdash-1.9.0/langdash/llm_config.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/llm_session.py` & `langdash-1.9.0/langdash/llm_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,21 +349,22 @@
 class LLMEmbeddingSession(LLMSession, Generic[T_LLM, T_Embedding]):
   """ Session for a language model that outputs an embedding for raw text. """
 
   def __init__(self, llm: T_LLM, ld: "Langdash"):
     self._ld = ld
     self._llm = llm
 
+  @property
   def embedding_size(self) -> int:
     """
     Returns the embedding size of the model.
     """
     raise NotImplementedError("embedding_size")
 
-  def embed(self, documents: List[str]) -> T_Embedding:
+  def embed(self, documents: List[str]) -> List[T_Embedding]:
     """
     Infer the embedding of a list of text.
     
     Args:
       documents (List[str]): The text to be embedded.
       
     Returns:
```

### Comparing `langdash-1.8.1/langdash/models/_mixins/tensor_based_infer_mixin.py` & `langdash-1.9.0/langdash/models/_mixins/tensor_based_infer_mixin.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/models/_tokenizer/_bpe.py` & `langdash-1.9.0/langdash/models/_tokenizer/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/models/_tokenizer/bytes_dict_tokenizer.py` & `langdash-1.9.0/langdash/models/_tokenizer/bytes_dict_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/models/_tokenizer/hf_tokenizer.py` & `langdash-1.9.0/langdash/models/_tokenizer/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/models/_tokenizer/rwkv_tokenizer.py` & `langdash-1.9.0/langdash/models/_tokenizer/rwkv_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/models/_tokenizer/tokenizer.py` & `langdash-1.9.0/langdash/models/_tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/models/ctransformers.py` & `langdash-1.9.0/langdash/models/ctransformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/models/llama_cpp.py` & `langdash-1.9.0/langdash/models/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/models/mock.py` & `langdash-1.9.0/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/models/rwkv_cpp.py` & `langdash-1.9.0/langdash/models/rwkv_cpp.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from dataclasses import dataclass
 import copy
 import os
 import sys
 import torch
 import tokenizers  # type: ignore
 
-from langdash.llm import LLM
+from langdash.llm import LLM, LLMCapability
 from langdash.llm_config import LLMConfig
-from langdash.llm_session import LLMGenerationSession, LLMGenerationSessionForRawText, LLMState
+from langdash.llm_session import LLMGenerationSession, LLMEmbeddingSession, LLMGenerationSessionForRawText, LLMState
 import langdash.sampling as sampling
 from ._mixins.tensor_based_infer_mixin import TensorBasedInferMixin
 
 _rwkv_lib: Optional[str] = None
 _rwkv_cpp_folder: Optional[str] = None
 
 RWKV_CPP_COMMIT_DEFAULT = "84634c047a9831b16cdf1cc3f2626e0ef0b2373b"
@@ -132,14 +132,19 @@
 
 try:
   import rwkv_tokenizer  # type: ignore
   _rwkv_tokenizer_available = True
 except ModuleNotFoundError:
   _rwkv_tokenizer_available = False
 
+_RWKV_CAPABILITY = LLMCapability.Generative
+
+if hasattr(rwkv_cpp_model.RWKVModel, 'n_embed'):
+  _RWKV_CAPABILITY |= LLMCapability.Embedding
+
 sys.path.pop(0)
 
 try:
   from tqdm import tqdm
 
   def _sequence_progress(v):
     if len(v) < 2:
@@ -191,14 +196,19 @@
         ),
         mapping=mapping
       )
     else:
       raise ValueError(f"unknown tokenizer type {llm._tokenizer_type}")
     self.eos_token = 0
 
+    if LLMCapability.Embedding in _RWKV_CAPABILITY:
+      self.embedding_size = self.model.n_embed
+      self.state_shape = (self.model.n_layer, 5, self.model.n_embed)
+      self.embedding_position = (0, 0)
+
   def eval(
     self,
     tokid: int,
     state: torch.Tensor,
     logits_out: Optional[torch.Tensor] = None
   ) -> Tuple[torch.Tensor, torch.Tensor]:
     return self.model.eval(tokid, state, state, logits_out)
@@ -215,18 +225,29 @@
       return logits_out, state
     else:
       for tokid in _sequence_progress(tokens[:-1]):
         _, state = self.model.eval(tokid, state, state, None)
       logits_out, state = self.model.eval(tokens[-1], state, state, logits_out)
       return logits_out, state
 
+  def embed(self, documents: List[str]) -> torch.Tensor:
+    embeddings = torch.zeros((len(documents), self.embedding_size))
+    for i, document in enumerate(documents):
+      _, state = self.eval_mult(
+        self.tokenizer.encode(document, add_special_tokens=False), None, None
+      )
+      state = state.reshape(self.state_shape)
+      embeddings[i] = state[self.embedding_position]
+    return embeddings
+
 
 class RwkvCppSession(
   TensorBasedInferMixin,
-  LLMGenerationSessionForRawText["RwkvCppModel", RwkvCppState, torch.Tensor]
+  LLMGenerationSessionForRawText["RwkvCppModel", RwkvCppState, torch.Tensor],
+  LLMEmbeddingSession["RwkvCppModel", torch.Tensor],
 ):
   """
   Session for rwkv.cpp model.
   """
 
   _logits: Optional[torch.Tensor]
   _state: Optional[torch.Tensor]
@@ -294,14 +315,65 @@
 
   def next_token_probs(self) -> List[float]:
     return sampling.logits_to_probs(self._next_token_logits_raw()).tolist()
 
   def get_vocab(self) -> Mapping[str, int]:
     return self._model.tokenizer.get_vocab()
 
+  @property
+  def embedding_size(self) -> int:
+    return self._model.embedding_size
+
+  def embed(self, documents: List[str]) -> torch.Tensor:
+    return self._model.embed(documents)
+
+  @property
+  def embedding_position(self) -> Tuple[int, int]:
+    """
+    Gets the position of the state in which to get the embedding vector.
+    """
+    return self._model.embedding_position
+
+  @embedding_position.setter
+  def embedding_position(self, position: Tuple[int, int]):
+    """
+    Sets the position of the state in which to get the embedding vector.
+    
+    Args:
+      position (Tuple[int,int]):
+        This must be a tuple of `(layer, vector index)`.
+        
+        Layer may be a negative number. If it is a negative number then
+        it will be counted backwards from the total number of layers in model.
+        
+        Vector index must be between 0 and 4 (inclusive).
+    """
+    layer, vector_index = position
+
+    n_layer = self._model.model.n_layer
+    if layer < 0:
+      layer = n_layer + layer
+    if not (0 <= layer <= n_layer):
+      raise ValueError(
+        f"layer index must be between 0 and {n_layer} (inclusive)"
+      )
+
+    if not (0 <= vector_index <= 4):
+      raise ValueError("vector index must be between 0 and 4 (inclusive)")
+
+    self._model.embedding_position = (layer, vector_index)
+
+  @property
+  def model_layer_size(self) -> int:
+    return self._model.model.n_layer
+
+  @property
+  def model_embed_vec_size(self) -> int:
+    return self._model.model.n_embed
+
 
 class RwkvCppModel(LLM[RwkvCppSession]):
   """
   rwkv.cpp model
   """
 
   _model_path: str
@@ -380,7 +452,11 @@
       }
       assert _rwkv_cpp_folder is not None
       self._tokenizer_path = os.path.join(
         _rwkv_cpp_folder, builtin_tokenizer_paths[self._tokenizer_type]
       )
     else:
       self._tokenizer_path = tokenizer_path
+
+  @property
+  def capability(self) -> LLMCapability:
+    return _RWKV_CAPABILITY
```

### Comparing `langdash-1.8.1/langdash/models/sentence_transformers.py` & `langdash-1.9.0/langdash/models/sentence_transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,20 @@
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
 
     self._model = self._ld._get_model_internal(
       self._llm, lambda llm: SentenceTransformer(llm._model_name)
     )
 
+  @property
   def embedding_size(self) -> int:
     return self._model.get_sentence_embedding_dimension()
 
   def embed(self, documents: List[str]) -> torch.Tensor:
-    return self._model.encode(documents)
+    return torch.tensor(self._model.encode(documents))
 
 
 class SentenceTransformersModel(EmbeddingLLM[SentenceTransformersSession]):
   """
   sentence_transformers embedding model.
   """
   Session = SentenceTransformersSession
```

### Comparing `langdash-1.8.1/langdash/models/transformers.py` & `langdash-1.9.0/langdash/models/transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/response.py` & `langdash-1.9.0/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/sampling.py` & `langdash-1.9.0/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/search/embedding_search.py` & `langdash-1.9.0/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/search/engine.py` & `langdash-1.9.0/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash/search/multichoice_search.py` & `langdash-1.9.0/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/langdash.egg-info/PKG-INFO` & `langdash-1.9.0/langdash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.8.1
+Version: 1.9.0
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langdash-1.8.1/langdash.egg-info/SOURCES.txt` & `langdash-1.9.0/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.8.1/setup.py` & `langdash-1.9.0/setup.py`

 * *Files identical despite different names*

