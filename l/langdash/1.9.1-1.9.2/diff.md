# Comparing `tmp/langdash-1.9.1.tar.gz` & `tmp/langdash-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.9.1.tar", last modified: Mon Jul 17 02:15:55 2023, max compression
+gzip compressed data, was "langdash-1.9.2.tar", last modified: Mon Jul 17 02:20:06 2023, max compression
```

## Comparing `langdash-1.9.1.tar` & `langdash-1.9.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.551742 langdash-1.9.1/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.9.1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.9.1/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3692 2023-07-17 02:15:55.547741 langdash-1.9.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2757 2023-07-15 21:14:06.000000 langdash-1.9.1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.543740 langdash-1.9.1/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-17 02:14:10.000000 langdash-1.9.1/langdash/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.547741 langdash-1.9.1/langdash/chains/
--rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.9.1/langdash/chains/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    16150 2023-07-17 00:39:55.000000 langdash-1.9.1/langdash/chains/chains.py
--rw-rw-r--   0 user      (1000) user      (1000)     9651 2023-07-17 02:03:07.000000 langdash-1.9.1/langdash/chains/nodes.py
--rw-rw-r--   0 user      (1000) user      (1000)      310 2023-07-14 19:48:15.000000 langdash-1.9.1/langdash/chains/typing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.543740 langdash-1.9.1/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.9.1/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.9.1/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     7148 2023-07-15 19:11:10.000000 langdash-1.9.1/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)     1359 2023-07-11 02:58:19.000000 langdash-1.9.1/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1677 2023-07-16 21:41:28.000000 langdash-1.9.1/langdash/llm.py
--rw-r--r--   0 user      (1000) user      (1000)      742 2023-07-14 18:46:03.000000 langdash-1.9.1/langdash/llm_config.py
--rw-rw-r--   0 user      (1000) user      (1000)    10255 2023-07-17 02:12:53.000000 langdash-1.9.1/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.547741 langdash-1.9.1/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.9.1/langdash/models/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.547741 langdash-1.9.1/langdash/models/_mixins/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.9.1/langdash/models/_mixins/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3900 2023-07-17 02:13:33.000000 langdash-1.9.1/langdash/models/_mixins/tensor_based_infer_mixin.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.547741 langdash-1.9.1/langdash/models/_tokenizer/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.9.1/langdash/models/_tokenizer/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.9.1/langdash/models/_tokenizer/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     1876 2023-07-17 01:59:42.000000 langdash-1.9.1/langdash/models/_tokenizer/bytes_dict_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     2331 2023-07-17 02:01:52.000000 langdash-1.9.1/langdash/models/_tokenizer/hf_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1601 2023-07-17 02:00:57.000000 langdash-1.9.1/langdash/models/_tokenizer/rwkv_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)      764 2023-07-17 02:01:26.000000 langdash-1.9.1/langdash/models/_tokenizer/tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     6321 2023-07-16 03:31:46.000000 langdash-1.9.1/langdash/models/ctransformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     6020 2023-07-16 03:31:55.000000 langdash-1.9.1/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.9.1/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)    14840 2023-07-17 02:10:15.000000 langdash-1.9.1/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)     1031 2023-07-16 21:47:08.000000 langdash-1.9.1/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5800 2023-07-17 02:12:00.000000 langdash-1.9.1/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      885 2023-07-15 18:57:17.000000 langdash-1.9.1/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.9.1/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.543740 langdash-1.9.1/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.9.1/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1133 2023-07-17 02:03:43.000000 langdash-1.9.1/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.9.1/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.9.1/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:15:55.547741 langdash-1.9.1/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3692 2023-07-17 02:15:55.000000 langdash-1.9.1/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1677 2023-07-17 02:15:55.000000 langdash-1.9.1/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-17 02:15:55.000000 langdash-1.9.1/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      199 2023-07-17 02:15:55.000000 langdash-1.9.1/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-17 02:15:55.000000 langdash-1.9.1/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-17 02:15:55.551742 langdash-1.9.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.9.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:20:06.902326 langdash-1.9.2/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.9.2/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.9.2/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3692 2023-07-17 02:20:06.902326 langdash-1.9.2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2757 2023-07-15 21:14:06.000000 langdash-1.9.2/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:20:06.898326 langdash-1.9.2/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-17 02:19:38.000000 langdash-1.9.2/langdash/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:20:06.898326 langdash-1.9.2/langdash/chains/
+-rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.9.2/langdash/chains/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16150 2023-07-17 00:39:55.000000 langdash-1.9.2/langdash/chains/chains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9651 2023-07-17 02:03:07.000000 langdash-1.9.2/langdash/chains/nodes.py
+-rw-rw-r--   0 user      (1000) user      (1000)      310 2023-07-14 19:48:15.000000 langdash-1.9.2/langdash/chains/typing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:20:06.894325 langdash-1.9.2/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.9.2/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.9.2/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7148 2023-07-15 19:11:10.000000 langdash-1.9.2/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1359 2023-07-11 02:58:19.000000 langdash-1.9.2/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1677 2023-07-16 21:41:28.000000 langdash-1.9.2/langdash/llm.py
+-rw-r--r--   0 user      (1000) user      (1000)      742 2023-07-14 18:46:03.000000 langdash-1.9.2/langdash/llm_config.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10255 2023-07-17 02:12:53.000000 langdash-1.9.2/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:20:06.898326 langdash-1.9.2/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.9.2/langdash/models/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:20:06.898326 langdash-1.9.2/langdash/models/_mixins/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.9.2/langdash/models/_mixins/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3931 2023-07-17 02:19:12.000000 langdash-1.9.2/langdash/models/_mixins/tensor_based_infer_mixin.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:20:06.902326 langdash-1.9.2/langdash/models/_tokenizer/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.9.2/langdash/models/_tokenizer/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.9.2/langdash/models/_tokenizer/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1876 2023-07-17 01:59:42.000000 langdash-1.9.2/langdash/models/_tokenizer/bytes_dict_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2331 2023-07-17 02:01:52.000000 langdash-1.9.2/langdash/models/_tokenizer/hf_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1601 2023-07-17 02:00:57.000000 langdash-1.9.2/langdash/models/_tokenizer/rwkv_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)      764 2023-07-17 02:01:26.000000 langdash-1.9.2/langdash/models/_tokenizer/tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6321 2023-07-16 03:31:46.000000 langdash-1.9.2/langdash/models/ctransformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6020 2023-07-16 03:31:55.000000 langdash-1.9.2/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.9.2/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14840 2023-07-17 02:10:15.000000 langdash-1.9.2/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1031 2023-07-16 21:47:08.000000 langdash-1.9.2/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5800 2023-07-17 02:12:00.000000 langdash-1.9.2/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      885 2023-07-15 18:57:17.000000 langdash-1.9.2/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.9.2/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:20:06.894325 langdash-1.9.2/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.9.2/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1133 2023-07-17 02:03:43.000000 langdash-1.9.2/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.9.2/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.9.2/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-17 02:20:06.898326 langdash-1.9.2/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3692 2023-07-17 02:20:06.000000 langdash-1.9.2/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1677 2023-07-17 02:20:06.000000 langdash-1.9.2/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-17 02:20:06.000000 langdash-1.9.2/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      199 2023-07-17 02:20:06.000000 langdash-1.9.2/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-17 02:20:06.000000 langdash-1.9.2/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-17 02:20:06.902326 langdash-1.9.2/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.9.2/setup.py
```

### Comparing `langdash-1.9.1/LICENSE.txt` & `langdash-1.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/PKG-INFO` & `langdash-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.9.1
+Version: 1.9.2
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langdash-1.9.1/README.md` & `langdash-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/chains/chains.py` & `langdash-1.9.2/langdash/chains/chains.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/chains/nodes.py` & `langdash-1.9.2/langdash/chains/nodes.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/classify/token_qa.py` & `langdash-1.9.2/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/core.py` & `langdash-1.9.2/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/infer.py` & `langdash-1.9.2/langdash/infer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/llm.py` & `langdash-1.9.2/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/llm_config.py` & `langdash-1.9.2/langdash/llm_config.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/llm_session.py` & `langdash-1.9.2/langdash/llm_session.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/models/_mixins/tensor_based_infer_mixin.py` & `langdash-1.9.2/langdash/models/_mixins/tensor_based_infer_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     if isinstance(end, str):
       if len(end) == 0:
         end = self._model.eos_token
       elif end_is_token or args.min_new_tokens > 0:
         endtoks = self.tokenize(end)
         assert len(endtoks) == 1
         end = endtoks[0]
-      assert isinstance(end, int)
 
     if self._logits is None:
       if self._next_token is not None:
         self._logits = self._eval(self._next_token[0])
         self._next_token = None
       else:
         raise ValueError(
@@ -68,15 +67,16 @@
           self._logits = self._eval(self._next_token[0])
         else:
           strip_left = self._next_token[1]
 
         self._next_token = None
 
       if args.min_new_tokens > 0 and i < args.min_new_tokens:
-        self._logits[end] = -inf
+        # FIXME: mypy doesn't infer end to be int
+        self._logits[end] = -inf # type: ignore
 
       if logit_preprocessors is not None:
         for pp in logit_preprocessors:
           # FIXME: mypy doesn't infer self._logits to be a sequence of ints
           pp(self._logits) # type: ignore
 
       tokid = sampling.sample(self._logits, args, ctx)
```

### Comparing `langdash-1.9.1/langdash/models/_tokenizer/_bpe.py` & `langdash-1.9.2/langdash/models/_tokenizer/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/models/_tokenizer/bytes_dict_tokenizer.py` & `langdash-1.9.2/langdash/models/_tokenizer/bytes_dict_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/models/_tokenizer/hf_tokenizer.py` & `langdash-1.9.2/langdash/models/_tokenizer/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/models/_tokenizer/rwkv_tokenizer.py` & `langdash-1.9.2/langdash/models/_tokenizer/rwkv_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/models/_tokenizer/tokenizer.py` & `langdash-1.9.2/langdash/models/_tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/models/ctransformers.py` & `langdash-1.9.2/langdash/models/ctransformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/models/llama_cpp.py` & `langdash-1.9.2/langdash/models/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/models/mock.py` & `langdash-1.9.2/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/models/rwkv_cpp.py` & `langdash-1.9.2/langdash/models/rwkv_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/models/sentence_transformers.py` & `langdash-1.9.2/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/models/transformers.py` & `langdash-1.9.2/langdash/models/transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/response.py` & `langdash-1.9.2/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/sampling.py` & `langdash-1.9.2/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/search/embedding_search.py` & `langdash-1.9.2/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/search/engine.py` & `langdash-1.9.2/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash/search/multichoice_search.py` & `langdash-1.9.2/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/langdash.egg-info/PKG-INFO` & `langdash-1.9.2/langdash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.9.1
+Version: 1.9.2
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langdash-1.9.1/langdash.egg-info/SOURCES.txt` & `langdash-1.9.2/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.9.1/setup.py` & `langdash-1.9.2/setup.py`

 * *Files identical despite different names*

