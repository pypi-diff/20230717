# Comparing `tmp/langdash-1.9.0.tar.gz` & `tmp/langdash-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.9.0.tar", last modified: Mon Jul 17 00:13:15 2023, max compression
+gzip compressed data, was "langdash-1.9.1.tar", last modified: Mon Jul 17 02:15:55 2023, max compression
```

## Comparing `langdash-1.9.0.tar` & `langdash-1.9.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.677788 langdash-1.9.0/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.9.0/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.9.0/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3692 2023-07-17 00:13:15.677788 langdash-1.9.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2757 2023-07-15 21:14:06.000000 langdash-1.9.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.673788 langdash-1.9.0/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-17 00:12:51.000000 langdash-1.9.0/langdash/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.677788 langdash-1.9.0/langdash/chains/
--rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.9.0/langdash/chains/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    16150 2023-07-17 00:09:43.000000 langdash-1.9.0/langdash/chains/chains.py
--rw-rw-r--   0 user      (1000) user      (1000)     9610 2023-07-17 00:04:17.000000 langdash-1.9.0/langdash/chains/nodes.py
--rw-rw-r--   0 user      (1000) user      (1000)      310 2023-07-14 19:48:15.000000 langdash-1.9.0/langdash/chains/typing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.673788 langdash-1.9.0/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.9.0/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.9.0/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     7148 2023-07-15 19:11:10.000000 langdash-1.9.0/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)     1359 2023-07-11 02:58:19.000000 langdash-1.9.0/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1677 2023-07-16 21:41:28.000000 langdash-1.9.0/langdash/llm.py
--rw-r--r--   0 user      (1000) user      (1000)      742 2023-07-14 18:46:03.000000 langdash-1.9.0/langdash/llm_config.py
--rw-rw-r--   0 user      (1000) user      (1000)    10233 2023-07-16 21:47:08.000000 langdash-1.9.0/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.677788 langdash-1.9.0/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.9.0/langdash/models/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.677788 langdash-1.9.0/langdash/models/_mixins/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.9.0/langdash/models/_mixins/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3775 2023-07-15 19:49:38.000000 langdash-1.9.0/langdash/models/_mixins/tensor_based_infer_mixin.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.677788 langdash-1.9.0/langdash/models/_tokenizer/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.9.0/langdash/models/_tokenizer/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.9.0/langdash/models/_tokenizer/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     1610 2023-07-15 19:49:38.000000 langdash-1.9.0/langdash/models/_tokenizer/bytes_dict_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     2361 2023-07-15 19:49:38.000000 langdash-1.9.0/langdash/models/_tokenizer/hf_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1622 2023-07-15 19:25:51.000000 langdash-1.9.0/langdash/models/_tokenizer/rwkv_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)      745 2023-07-15 19:49:38.000000 langdash-1.9.0/langdash/models/_tokenizer/tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     6321 2023-07-16 03:31:46.000000 langdash-1.9.0/langdash/models/ctransformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     6020 2023-07-16 03:31:55.000000 langdash-1.9.0/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.9.0/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)    14583 2023-07-17 00:04:17.000000 langdash-1.9.0/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)     1031 2023-07-16 21:47:08.000000 langdash-1.9.0/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5799 2023-07-16 03:32:00.000000 langdash-1.9.0/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      885 2023-07-15 18:57:17.000000 langdash-1.9.0/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.9.0/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.673788 langdash-1.9.0/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.9.0/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.9.0/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.9.0/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.9.0/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 00:13:15.673788 langdash-1.9.0/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3692 2023-07-17 00:13:15.000000 langdash-1.9.0/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1677 2023-07-17 00:13:15.000000 langdash-1.9.0/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-17 00:13:15.000000 langdash-1.9.0/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      199 2023-07-17 00:13:15.000000 langdash-1.9.0/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-17 00:13:15.000000 langdash-1.9.0/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-17 00:13:15.677788 langdash-1.9.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.9.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.551742 langdash-1.9.1/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.9.1/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.9.1/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3692 2023-07-17 02:15:55.547741 langdash-1.9.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2757 2023-07-15 21:14:06.000000 langdash-1.9.1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.543740 langdash-1.9.1/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-17 02:14:10.000000 langdash-1.9.1/langdash/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.547741 langdash-1.9.1/langdash/chains/
+-rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.9.1/langdash/chains/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16150 2023-07-17 00:39:55.000000 langdash-1.9.1/langdash/chains/chains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9651 2023-07-17 02:03:07.000000 langdash-1.9.1/langdash/chains/nodes.py
+-rw-rw-r--   0 user      (1000) user      (1000)      310 2023-07-14 19:48:15.000000 langdash-1.9.1/langdash/chains/typing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.543740 langdash-1.9.1/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.9.1/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.9.1/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7148 2023-07-15 19:11:10.000000 langdash-1.9.1/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1359 2023-07-11 02:58:19.000000 langdash-1.9.1/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1677 2023-07-16 21:41:28.000000 langdash-1.9.1/langdash/llm.py
+-rw-r--r--   0 user      (1000) user      (1000)      742 2023-07-14 18:46:03.000000 langdash-1.9.1/langdash/llm_config.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10255 2023-07-17 02:12:53.000000 langdash-1.9.1/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.547741 langdash-1.9.1/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.9.1/langdash/models/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.547741 langdash-1.9.1/langdash/models/_mixins/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.9.1/langdash/models/_mixins/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3900 2023-07-17 02:13:33.000000 langdash-1.9.1/langdash/models/_mixins/tensor_based_infer_mixin.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.547741 langdash-1.9.1/langdash/models/_tokenizer/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.9.1/langdash/models/_tokenizer/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.9.1/langdash/models/_tokenizer/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1876 2023-07-17 01:59:42.000000 langdash-1.9.1/langdash/models/_tokenizer/bytes_dict_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2331 2023-07-17 02:01:52.000000 langdash-1.9.1/langdash/models/_tokenizer/hf_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1601 2023-07-17 02:00:57.000000 langdash-1.9.1/langdash/models/_tokenizer/rwkv_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)      764 2023-07-17 02:01:26.000000 langdash-1.9.1/langdash/models/_tokenizer/tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6321 2023-07-16 03:31:46.000000 langdash-1.9.1/langdash/models/ctransformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6020 2023-07-16 03:31:55.000000 langdash-1.9.1/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.9.1/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14840 2023-07-17 02:10:15.000000 langdash-1.9.1/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1031 2023-07-16 21:47:08.000000 langdash-1.9.1/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5800 2023-07-17 02:12:00.000000 langdash-1.9.1/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      885 2023-07-15 18:57:17.000000 langdash-1.9.1/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.9.1/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.543740 langdash-1.9.1/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.9.1/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1133 2023-07-17 02:03:43.000000 langdash-1.9.1/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.9.1/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.9.1/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.547741 langdash-1.9.1/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3692 2023-07-17 02:15:55.000000 langdash-1.9.1/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1677 2023-07-17 02:15:55.000000 langdash-1.9.1/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-17 02:15:55.000000 langdash-1.9.1/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      199 2023-07-17 02:15:55.000000 langdash-1.9.1/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-17 02:15:55.000000 langdash-1.9.1/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-17 02:15:55.551742 langdash-1.9.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.9.1/setup.py
```

### Comparing `langdash-1.9.0/LICENSE.txt` & `langdash-1.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/PKG-INFO` & `langdash-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.9.0
+Version: 1.9.1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langdash-1.9.0/README.md` & `langdash-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/langdash/chains/chains.py` & `langdash-1.9.1/langdash/chains/chains.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/langdash/chains/nodes.py` & `langdash-1.9.1/langdash/chains/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from langdash.infer import InferArgs
 
 if TYPE_CHECKING:
   from langdash.core import Langdash
   from langdash.llm_session import LLMGenerationSession
   from .chains import LDChain, LDNodeGenerator, LDNodeArgs
 
+LogitPreprocessor = Callable[[List[int]], None]
+
 
 class LDNode:
   """ Base class for langdash nodes. """
 
   def __init__(self, ld: "Langdash"):
     self._ld = ld
 
@@ -96,15 +98,15 @@
     self,
     ld: "Langdash",
     returns: str,
     end: Optional[Union[str, int]],
     padleft: str = "",
     infer_args: Optional[InferArgs] = None,
     end_is_token: bool = False,
-    logit_preprocessors: Optional[List[Callable[List[int], None]]] = None,
+    logit_preprocessors: Optional[List[LogitPreprocessor]] = None,
   ):
     super().__init__(ld)
     self._returns = returns
     self._end = end
     self._padleft = padleft
     self._infer_args = infer_args
     self._end_is_token = end_is_token
```

### Comparing `langdash-1.9.0/langdash/classify/token_qa.py` & `langdash-1.9.1/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/langdash/core.py` & `langdash-1.9.1/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/langdash/infer.py` & `langdash-1.9.1/langdash/infer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/langdash/llm.py` & `langdash-1.9.1/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/langdash/llm_config.py` & `langdash-1.9.1/langdash/llm_config.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/langdash/llm_session.py` & `langdash-1.9.1/langdash/llm_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from langdash.chains import CalledNode, LDNodeArgs, LDNode
 from langdash.infer import InferArgs
 from langdash.llm import LLM
 
 if TYPE_CHECKING:
   from langdash.core import Langdash
 
-LogitPreprocessorList = List[Callable[Sequence[int], None]]
+LogitPreprocessorList = List[Callable[[Sequence[int]], None]]
 
 T_LLM = TypeVar("T_LLM", bound=LLM)
 
 
 class LLMSession(Generic[T_LLM]):
   """
   Base class for a session for a language model.
@@ -190,15 +190,15 @@
     args: InferArgs,
     end_is_token: bool,
     logit_preprocessors: Optional[LogitPreprocessorList],
   ) -> Generator[RespInfer, None, None]:
     raise NotImplementedError("_infer")
 
   def infer(self,
-            args: InferArgs = None,
+            args: Optional[InferArgs] = None,
             **kwargs) -> Generator[RespInfer, None, None]:
     """
     Infer the next tokens from the input sequence.
 
     Args:
       end (Optional[Union[str, int]]):
         The end of the output sequence.
@@ -339,32 +339,32 @@
         num_toks += 1
       self._logits = self._eval_mult(tokens)
       num_toks += len(tokens)
 
     return num_toks
 
 
-T_Embedding = TypeVar("T_Embedding")
+T_EmbeddingList = TypeVar("T_EmbeddingList")
 
 
-class LLMEmbeddingSession(LLMSession, Generic[T_LLM, T_Embedding]):
+class LLMEmbeddingSession(LLMSession, Generic[T_LLM, T_EmbeddingList]):
   """ Session for a language model that outputs an embedding for raw text. """
 
   def __init__(self, llm: T_LLM, ld: "Langdash"):
     self._ld = ld
     self._llm = llm
 
   @property
   def embedding_size(self) -> int:
     """
     Returns the embedding size of the model.
     """
     raise NotImplementedError("embedding_size")
 
-  def embed(self, documents: List[str]) -> List[T_Embedding]:
+  def embed(self, documents: List[str]) -> T_EmbeddingList:
     """
     Infer the embedding of a list of text.
     
     Args:
       documents (List[str]): The text to be embedded.
       
     Returns:
```

### Comparing `langdash-1.9.0/langdash/models/_mixins/tensor_based_infer_mixin.py` & `langdash-1.9.1/langdash/models/_mixins/tensor_based_infer_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     if isinstance(end, str):
       if len(end) == 0:
         end = self._model.eos_token
       elif end_is_token or args.min_new_tokens > 0:
         endtoks = self.tokenize(end)
         assert len(endtoks) == 1
         end = endtoks[0]
+      assert isinstance(end, int)
 
     if self._logits is None:
       if self._next_token is not None:
         self._logits = self._eval(self._next_token[0])
         self._next_token = None
       else:
         raise ValueError(
@@ -71,15 +72,16 @@
         self._next_token = None
 
       if args.min_new_tokens > 0 and i < args.min_new_tokens:
         self._logits[end] = -inf
 
       if logit_preprocessors is not None:
         for pp in logit_preprocessors:
-          pp(self._logits)
+          # FIXME: mypy doesn't infer self._logits to be a sequence of ints
+          pp(self._logits) # type: ignore
 
       tokid = sampling.sample(self._logits, args, ctx)
       ctx.append(tokid)
 
       if tokid == self._model.eos_token:  # implies end is int
         break
```

### Comparing `langdash-1.9.0/langdash/models/_tokenizer/_bpe.py` & `langdash-1.9.1/langdash/models/_tokenizer/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/langdash/models/_tokenizer/bytes_dict_tokenizer.py` & `langdash-1.9.1/langdash/models/_tokenizer/bytes_dict_tokenizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-from typing import List, Union, Optional, Generator, Mapping
+from typing import List, Union, Optional, Generator, Dict, Callable
 from .tokenizer import Tokenizer, BufferedToken
 
 
 class BytesDictTokenizer(Tokenizer):
 
-  def __init__(self, encode_func, decode_func, mapping: List[bytes]):
+  def __init__(
+    self,
+    encode_func: Callable[..., List[int]],
+    decode_func: Callable[[List[int]], str],
+    mapping: List[bytes],
+  ):
     self.encode_func = encode_func
     self.decode_func = decode_func
     self.mapping = mapping
+    self.reverse_mapping: Optional[Dict[bytes, int]] = None
 
   def encode(self, text: str, add_special_tokens: bool = False) -> List[int]:
     return self.encode_func(text, add_special_tokens=add_special_tokens)
 
   def decode(self, tokens: List[int]) -> str:
     return self.decode_func(tokens)
 
@@ -24,16 +30,20 @@
 
   def tokens_starting_with(self, token_id: int) -> Generator[int, None, None]:
     tokstr = self.mapping[token_id]
     for logits_tokid, logits_tokstr in enumerate(self.mapping):
       if not logits_tokstr.startswith(tokstr):
         yield logits_tokid
 
-  def get_vocab(self) -> Mapping[str, int]:
-    return self.mapping
+  def get_vocab(self):
+    if self.reverse_mapping is None:
+      self.reverse_mapping = {
+        token: idx for idx, token in enumerate(self.mapping)
+      }
+    return self.reverse_mapping
 
 
 class BytesDictBufferedToken(BufferedToken):
 
   def __init__(self, tokenizer: BytesDictTokenizer, token_bytes: bytes):
     self.tokenizer = tokenizer
     self.token_bytes = token_bytes
```

### Comparing `langdash-1.9.0/langdash/models/_tokenizer/hf_tokenizer.py` & `langdash-1.9.1/langdash/models/_tokenizer/hf_tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union, Optional, Generator, Mapping
+from typing import List, Union, Optional, Generator
 import warnings
 from .tokenizer import Tokenizer, BufferedToken
 from ._bpe import decode as bpe_decode
 
 
 class HFTokenizer(Tokenizer):
   vocab: List[str]
@@ -48,15 +48,15 @@
       tokstr = self.tokenizer.decode(token_id)
       for logits_tokid, logits_tokstr in enumerate(self.vocab):
         if not logits_tokstr.startswith(tokstr):
           yield logits_tokid
     except UnicodeDecodeError:
       return
 
-  def get_vocab(self) -> Mapping[str, int]:
+  def get_vocab(self):
     return self.tokenizer.get_vocab()
 
 
 class HFBufferedToken(BufferedToken):
 
   def __init__(self, tokenizer: HFTokenizer, token_id: int):
     self.tokenizer = tokenizer
```

### Comparing `langdash-1.9.0/langdash/models/_tokenizer/rwkv_tokenizer.py` & `langdash-1.9.1/langdash/models/_tokenizer/rwkv_tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
   def tokens_starting_with(self, token_id: int) -> Generator[int, None, None]:
     tokstr = self.decode([token_id])
     for logits_tokstr, logits_tokid in self.vocab.items():
       if not logits_tokstr.startswith(tokstr):
         yield logits_tokid
 
-  def get_vocab(self) -> Mapping[str, int]:
+  def get_vocab(self):
     return self.vocab
 
 
 class RwkvBufferedToken(BufferedToken):
 
   def __init__(self, tokenizer: RwkvTokenizer, token_id: int):
     self.tokenizer = tokenizer
```

### Comparing `langdash-1.9.0/langdash/models/_tokenizer/tokenizer.py` & `langdash-1.9.1/langdash/models/_tokenizer/tokenizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union, Optional, Generator, Mapping
+from typing import List, Union, Optional, Generator, Dict
 from abc import ABC, abstractmethod
 
 
 class BufferedToken(ABC):
 
   @abstractmethod
   def add_token_id(self, token_id: int) -> Optional[str]:
@@ -28,9 +28,9 @@
     pass
 
   @abstractmethod
   def tokens_starting_with(self, token_id: int) -> Generator[int, None, None]:
     pass
 
   @abstractmethod
-  def get_vocab(self) -> Mapping[str, int]:
+  def get_vocab(self) -> Union[Dict[bytes, int], Dict[str, int]]:
     pass
```

### Comparing `langdash-1.9.0/langdash/models/ctransformers.py` & `langdash-1.9.1/langdash/models/ctransformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/langdash/models/llama_cpp.py` & `langdash-1.9.1/langdash/models/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/langdash/models/mock.py` & `langdash-1.9.1/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/langdash/models/rwkv_cpp.py` & `langdash-1.9.1/langdash/models/rwkv_cpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import tokenizers  # type: ignore
 
 from langdash.llm import LLM, LLMCapability
 from langdash.llm_config import LLMConfig
 from langdash.llm_session import LLMGenerationSession, LLMEmbeddingSession, LLMGenerationSessionForRawText, LLMState
 import langdash.sampling as sampling
 from ._mixins.tensor_based_infer_mixin import TensorBasedInferMixin
+from ._tokenizer.tokenizer import Tokenizer
 
 _rwkv_lib: Optional[str] = None
 _rwkv_cpp_folder: Optional[str] = None
 
 RWKV_CPP_COMMIT_DEFAULT = "84634c047a9831b16cdf1cc3f2626e0ef0b2373b"
 RWKV_CPP_COMMIT = os.environ.get(
   "LANGDASH_RWKV_CPP_COMMIT", RWKV_CPP_COMMIT_DEFAULT
@@ -161,14 +162,16 @@
   _logits: Optional[torch.Tensor] = None
   _state: Optional[torch.Tensor] = None
   _next_token: Optional[Tuple[int, str]] = None
 
 
 class RwkvCppWrapper:
 
+  tokenizer: Tokenizer
+
   def __init__(self, llm: "RwkvCppModel"):
     assert _rwkv_lib is not None
     self.model = rwkv_cpp_model.RWKVModel(
       rwkv_cpp_shared_library.RWKVSharedLibrary(_rwkv_lib), llm._model_path,
       **llm._model_kwargs
     )
     self.batch_size = llm._batch_size
@@ -210,28 +213,33 @@
     tokid: int,
     state: torch.Tensor,
     logits_out: Optional[torch.Tensor] = None
   ) -> Tuple[torch.Tensor, torch.Tensor]:
     return self.model.eval(tokid, state, state, logits_out)
 
   def eval_mult(
-    self, tokens: List[int], state: torch.Tensor, logits_out: torch.Tensor
+    self,
+    tokens: List[int],
+    state: Optional[torch.Tensor],
+    logits_out: Optional[torch.Tensor],
   ) -> Tuple[torch.Tensor, torch.Tensor]:
     if self.do_eval_sequence:
       batch_size = self.batch_size
       for i in _sequence_progress(range(0, len(tokens), batch_size)):
         logits_out, state = self.model.eval_sequence(
           tokens[i:i + batch_size], state, state, logits_out
         )
-      return logits_out, state
+    # FIXME: mypy does not infer self._logits to not be None
+      return logits_out, state  # type: ignore
     else:
       for tokid in _sequence_progress(tokens[:-1]):
         _, state = self.model.eval(tokid, state, state, None)
       logits_out, state = self.model.eval(tokens[-1], state, state, logits_out)
-      return logits_out, state
+      # FIXME: mypy does not infer self._logits to not be None
+      return logits_out, state  # type: ignore
 
   def embed(self, documents: List[str]) -> torch.Tensor:
     embeddings = torch.zeros((len(documents), self.embedding_size))
     for i, document in enumerate(documents):
       _, state = self.eval_mult(
         self.tokenizer.encode(document, add_special_tokens=False), None, None
       )
```

### Comparing `langdash-1.9.0/langdash/models/sentence_transformers.py` & `langdash-1.9.1/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/langdash/models/transformers.py` & `langdash-1.9.1/langdash/models/transformers.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
   def next_token_logits(self) -> List[float]:
     return self._next_token_logits_raw().tolist()
 
   def next_token_probs(self) -> List[float]:
     return sampling.logits_to_probs(self._next_token_logits_raw()).tolist()
 
   def get_context_length(self) -> int:
-    return self.model.get_context_length()
+    return self._model.get_context_length()
 
   def get_vocab(self) -> Mapping[str, int]:
     return self._model.tokenizer.get_vocab()
 
 
 class TransformersModel(LLM[TransformersSession]):
   """
```

### Comparing `langdash-1.9.0/langdash/response.py` & `langdash-1.9.1/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/langdash/sampling.py` & `langdash-1.9.1/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/langdash/search/embedding_search.py` & `langdash-1.9.1/langdash/search/embedding_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
   def __init__(
     self,
     embd_session: LLMEmbeddingSession,
   ):
     super().__init__()
     self._embd_session = embd_session
-    self._embds = faiss.IndexFlatIP(self._embd_session.embedding_size())
+    self._embds = faiss.IndexFlatIP(self._embd_session.embedding_size)
 
   def add(self, texts: Union[str, List[str]]):
     if isinstance(texts, str):
       self._documents.append(texts)
       self._embds.add(self._embd_session.embed([texts]))
     else:
       self._documents += texts
```

### Comparing `langdash-1.9.0/langdash/search/engine.py` & `langdash-1.9.1/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/langdash/search/multichoice_search.py` & `langdash-1.9.1/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/langdash.egg-info/PKG-INFO` & `langdash-1.9.1/langdash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.9.0
+Version: 1.9.1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langdash-1.9.0/langdash.egg-info/SOURCES.txt` & `langdash-1.9.1/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.9.0/setup.py` & `langdash-1.9.1/setup.py`

 * *Files identical despite different names*

