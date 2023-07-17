# Comparing `tmp/langroid-0.1.8.tar.gz` & `tmp/langroid-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langroid-0.1.8.tar", max compression
+gzip compressed data, was "langroid-0.1.9.tar", max compression
```

## Comparing `langroid-0.1.8.tar` & `langroid-0.1.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1065 2023-07-10 12:50:46.867380 langroid-0.1.8/LICENSE
--rw-r--r--   0        0        0     7640 2023-07-14 01:55:09.549026 langroid-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-07-10 12:50:46.945291 langroid-0.1.8/langroid/agent/__init__.py
--rw-r--r--   0        0        0    20661 2023-07-12 15:42:56.200970 langroid-0.1.8/langroid/agent/base.py
--rw-r--r--   0        0        0    21381 2023-07-12 19:26:13.244508 langroid-0.1.8/langroid/agent/chat_agent.py
--rw-r--r--   0        0        0     5745 2023-07-11 17:26:14.896756 langroid-0.1.8/langroid/agent/chat_document.py
--rw-r--r--   0        0        0        0 2023-07-10 12:50:46.945784 langroid-0.1.8/langroid/agent/special/__init__.py
--rw-r--r--   0        0        0    15600 2023-07-11 18:03:51.048963 langroid-0.1.8/langroid/agent/special/doc_chat_agent.py
--rw-r--r--   0        0        0     4495 2023-07-11 17:26:14.896869 langroid-0.1.8/langroid/agent/special/recipient_validator_agent.py
--rw-r--r--   0        0        0     6995 2023-07-11 18:16:03.238429 langroid-0.1.8/langroid/agent/special/retriever_agent.py
--rw-r--r--   0        0        0    24029 2023-07-12 14:10:13.319947 langroid-0.1.8/langroid/agent/task.py
--rw-r--r--   0        0        0     5339 2023-07-11 20:42:05.617741 langroid-0.1.8/langroid/agent/tool_message.py
--rw-r--r--   0        0        0        0 2023-07-10 12:50:46.946205 langroid-0.1.8/langroid/cachedb/__init__.py
--rw-r--r--   0        0        0      790 2023-07-10 12:50:46.946296 langroid-0.1.8/langroid/cachedb/base.py
--rw-r--r--   0        0        0     2335 2023-07-13 21:50:17.897232 langroid-0.1.8/langroid/cachedb/redis_cachedb.py
--rw-r--r--   0        0        0        0 2023-07-10 12:50:46.946452 langroid-0.1.8/langroid/embedding_models/__init__.py
--rw-r--r--   0        0        0      939 2023-07-10 12:50:46.946564 langroid-0.1.8/langroid/embedding_models/base.py
--rw-r--r--   0        0        0     2490 2023-07-10 12:50:46.946652 langroid-0.1.8/langroid/embedding_models/models.py
--rw-r--r--   0        0        0        0 2023-07-10 12:50:46.946780 langroid-0.1.8/langroid/language_models/__init__.py
--rw-r--r--   0        0        0    12539 2023-07-11 14:33:44.212106 langroid-0.1.8/langroid/language_models/base.py
--rw-r--r--   0        0        0    17329 2023-07-12 02:18:15.391645 langroid-0.1.8/langroid/language_models/openai_gpt.py
--rw-r--r--   0        0        0     4668 2023-07-10 12:50:46.947158 langroid-0.1.8/langroid/language_models/utils.py
--rw-r--r--   0        0        0     1434 2023-07-11 17:26:14.896978 langroid-0.1.8/langroid/mytypes.py
--rw-r--r--   0        0        0        0 2023-07-10 12:50:46.947322 langroid-0.1.8/langroid/parsing/__init__.py
--rw-r--r--   0        0        0     1068 2023-07-10 12:50:46.947420 langroid-0.1.8/langroid/parsing/agent_chats.py
--rw-r--r--   0        0        0     3727 2023-07-10 12:50:46.947504 langroid-0.1.8/langroid/parsing/code_parser.py
--rw-r--r--   0        0        0      981 2023-07-10 12:50:46.947580 langroid-0.1.8/langroid/parsing/json.py
--rw-r--r--   0        0        0     1829 2023-07-10 12:50:46.947651 langroid-0.1.8/langroid/parsing/para_sentence_split.py
--rw-r--r--   0        0        0     6831 2023-07-10 12:50:46.947734 langroid-0.1.8/langroid/parsing/parser.py
--rw-r--r--   0        0        0    26625 2023-07-10 12:50:46.947881 langroid-0.1.8/langroid/parsing/repo_loader.py
--rw-r--r--   0        0        0     1612 2023-07-10 12:50:46.947966 langroid-0.1.8/langroid/parsing/url_loader.py
--rw-r--r--   0        0        0     3709 2023-07-10 12:50:46.948046 langroid-0.1.8/langroid/parsing/urls.py
--rw-r--r--   0        0        0      683 2023-07-10 12:50:46.948121 langroid-0.1.8/langroid/parsing/utils.py
--rw-r--r--   0        0        0        0 2023-07-10 12:50:46.948229 langroid-0.1.8/langroid/prompts/__init__.py
--rw-r--r--   0        0        0      331 2023-07-10 12:50:46.948326 langroid-0.1.8/langroid/prompts/dialog.py
--rw-r--r--   0        0        0       98 2023-07-10 12:50:46.948390 langroid-0.1.8/langroid/prompts/prompts_config.py
--rw-r--r--   0        0        0     5850 2023-07-10 12:50:46.948476 langroid-0.1.8/langroid/prompts/templates.py
--rw-r--r--   0        0        0     8935 2023-07-10 12:50:46.948571 langroid-0.1.8/langroid/prompts/transforms.py
--rw-r--r--   0        0        0        0 2023-07-10 12:50:46.948656 langroid-0.1.8/langroid/scripts/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 12:50:46.948847 langroid-0.1.8/langroid/utils/__init__.py
--rw-r--r--   0        0        0     1498 2023-07-10 12:50:46.948961 langroid-0.1.8/langroid/utils/configuration.py
--rw-r--r--   0        0        0      485 2023-07-10 12:50:46.949032 langroid-0.1.8/langroid/utils/constants.py
--rw-r--r--   0        0        0     3875 2023-07-10 12:50:46.949116 langroid-0.1.8/langroid/utils/logging.py
--rw-r--r--   0        0        0        0 2023-07-10 12:50:46.949195 langroid-0.1.8/langroid/utils/output/__init__.py
--rw-r--r--   0        0        0     1311 2023-07-10 21:57:19.150301 langroid-0.1.8/langroid/utils/output/printing.py
--rw-r--r--   0        0        0     1138 2023-07-10 12:50:46.949375 langroid-0.1.8/langroid/utils/system.py
--rw-r--r--   0        0        0        0 2023-07-10 12:50:46.949448 langroid-0.1.8/langroid/vector_store/__init__.py
--rw-r--r--   0        0        0     3679 2023-07-11 17:29:58.775183 langroid-0.1.8/langroid/vector_store/base.py
--rw-r--r--   0        0        0     5200 2023-07-11 17:29:02.512412 langroid-0.1.8/langroid/vector_store/chromadb.py
--rw-r--r--   0        0        0     7731 2023-07-11 17:29:02.512859 langroid-0.1.8/langroid/vector_store/qdrantdb.py
--rw-r--r--   0        0        0     3045 2023-07-14 19:22:35.302348 langroid-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    10006 1970-01-01 00:00:00.000000 langroid-0.1.8/setup.py
--rw-r--r--   0        0        0    10055 1970-01-01 00:00:00.000000 langroid-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-10 12:50:46.867380 langroid-0.1.9/LICENSE
+-rw-r--r--   0        0        0     7640 2023-07-14 01:55:09.549026 langroid-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 12:50:46.945291 langroid-0.1.9/langroid/agent/__init__.py
+-rw-r--r--   0        0        0    20661 2023-07-12 15:42:56.200970 langroid-0.1.9/langroid/agent/base.py
+-rw-r--r--   0        0        0    21381 2023-07-12 19:26:13.244508 langroid-0.1.9/langroid/agent/chat_agent.py
+-rw-r--r--   0        0        0     5745 2023-07-11 17:26:14.896756 langroid-0.1.9/langroid/agent/chat_document.py
+-rw-r--r--   0        0        0        0 2023-07-10 12:50:46.945784 langroid-0.1.9/langroid/agent/special/__init__.py
+-rw-r--r--   0        0        0    15600 2023-07-11 18:03:51.048963 langroid-0.1.9/langroid/agent/special/doc_chat_agent.py
+-rw-r--r--   0        0        0     4495 2023-07-11 17:26:14.896869 langroid-0.1.9/langroid/agent/special/recipient_validator_agent.py
+-rw-r--r--   0        0        0     6995 2023-07-11 18:16:03.238429 langroid-0.1.9/langroid/agent/special/retriever_agent.py
+-rw-r--r--   0        0        0    24029 2023-07-12 14:10:13.319947 langroid-0.1.9/langroid/agent/task.py
+-rw-r--r--   0        0        0     5339 2023-07-11 20:42:05.617741 langroid-0.1.9/langroid/agent/tool_message.py
+-rw-r--r--   0        0        0        0 2023-07-10 12:50:46.946205 langroid-0.1.9/langroid/cachedb/__init__.py
+-rw-r--r--   0        0        0      790 2023-07-10 12:50:46.946296 langroid-0.1.9/langroid/cachedb/base.py
+-rw-r--r--   0        0        0     2335 2023-07-13 21:50:17.897232 langroid-0.1.9/langroid/cachedb/redis_cachedb.py
+-rw-r--r--   0        0        0        0 2023-07-10 12:50:46.946452 langroid-0.1.9/langroid/embedding_models/__init__.py
+-rw-r--r--   0        0        0      939 2023-07-10 12:50:46.946564 langroid-0.1.9/langroid/embedding_models/base.py
+-rw-r--r--   0        0        0     2490 2023-07-10 12:50:46.946652 langroid-0.1.9/langroid/embedding_models/models.py
+-rw-r--r--   0        0        0        0 2023-07-10 12:50:46.946780 langroid-0.1.9/langroid/language_models/__init__.py
+-rw-r--r--   0        0        0    12539 2023-07-11 14:33:44.212106 langroid-0.1.9/langroid/language_models/base.py
+-rw-r--r--   0        0        0    17329 2023-07-12 02:18:15.391645 langroid-0.1.9/langroid/language_models/openai_gpt.py
+-rw-r--r--   0        0        0     4668 2023-07-10 12:50:46.947158 langroid-0.1.9/langroid/language_models/utils.py
+-rw-r--r--   0        0        0     1434 2023-07-11 17:26:14.896978 langroid-0.1.9/langroid/mytypes.py
+-rw-r--r--   0        0        0        0 2023-07-10 12:50:46.947322 langroid-0.1.9/langroid/parsing/__init__.py
+-rw-r--r--   0        0        0     1068 2023-07-10 12:50:46.947420 langroid-0.1.9/langroid/parsing/agent_chats.py
+-rw-r--r--   0        0        0     3727 2023-07-10 12:50:46.947504 langroid-0.1.9/langroid/parsing/code_parser.py
+-rw-r--r--   0        0        0      981 2023-07-10 12:50:46.947580 langroid-0.1.9/langroid/parsing/json.py
+-rw-r--r--   0        0        0     1829 2023-07-10 12:50:46.947651 langroid-0.1.9/langroid/parsing/para_sentence_split.py
+-rw-r--r--   0        0        0     6831 2023-07-10 12:50:46.947734 langroid-0.1.9/langroid/parsing/parser.py
+-rw-r--r--   0        0        0    26625 2023-07-10 12:50:46.947881 langroid-0.1.9/langroid/parsing/repo_loader.py
+-rw-r--r--   0        0        0     1612 2023-07-10 12:50:46.947966 langroid-0.1.9/langroid/parsing/url_loader.py
+-rw-r--r--   0        0        0     3709 2023-07-10 12:50:46.948046 langroid-0.1.9/langroid/parsing/urls.py
+-rw-r--r--   0        0        0      683 2023-07-10 12:50:46.948121 langroid-0.1.9/langroid/parsing/utils.py
+-rw-r--r--   0        0        0        0 2023-07-10 12:50:46.948229 langroid-0.1.9/langroid/prompts/__init__.py
+-rw-r--r--   0        0        0      331 2023-07-10 12:50:46.948326 langroid-0.1.9/langroid/prompts/dialog.py
+-rw-r--r--   0        0        0       98 2023-07-10 12:50:46.948390 langroid-0.1.9/langroid/prompts/prompts_config.py
+-rw-r--r--   0        0        0     5850 2023-07-10 12:50:46.948476 langroid-0.1.9/langroid/prompts/templates.py
+-rw-r--r--   0        0        0     8935 2023-07-10 12:50:46.948571 langroid-0.1.9/langroid/prompts/transforms.py
+-rw-r--r--   0        0        0        0 2023-07-10 12:50:46.948656 langroid-0.1.9/langroid/scripts/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 12:50:46.948847 langroid-0.1.9/langroid/utils/__init__.py
+-rw-r--r--   0        0        0     1498 2023-07-10 12:50:46.948961 langroid-0.1.9/langroid/utils/configuration.py
+-rw-r--r--   0        0        0      485 2023-07-10 12:50:46.949032 langroid-0.1.9/langroid/utils/constants.py
+-rw-r--r--   0        0        0     3875 2023-07-10 12:50:46.949116 langroid-0.1.9/langroid/utils/logging.py
+-rw-r--r--   0        0        0        0 2023-07-10 12:50:46.949195 langroid-0.1.9/langroid/utils/output/__init__.py
+-rw-r--r--   0        0        0     1311 2023-07-10 21:57:19.150301 langroid-0.1.9/langroid/utils/output/printing.py
+-rw-r--r--   0        0        0     1138 2023-07-10 12:50:46.949375 langroid-0.1.9/langroid/utils/system.py
+-rw-r--r--   0        0        0        0 2023-07-10 12:50:46.949448 langroid-0.1.9/langroid/vector_store/__init__.py
+-rw-r--r--   0        0        0     3679 2023-07-11 17:29:58.775183 langroid-0.1.9/langroid/vector_store/base.py
+-rw-r--r--   0        0        0     5200 2023-07-11 17:29:02.512412 langroid-0.1.9/langroid/vector_store/chromadb.py
+-rw-r--r--   0        0        0     7731 2023-07-11 17:29:02.512859 langroid-0.1.9/langroid/vector_store/qdrantdb.py
+-rw-r--r--   0        0        0     3304 2023-07-14 22:00:35.052334 langroid-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     9876 1970-01-01 00:00:00.000000 langroid-0.1.9/setup.py
+-rw-r--r--   0        0        0     9884 1970-01-01 00:00:00.000000 langroid-0.1.9/PKG-INFO
```

### Comparing `langroid-0.1.8/LICENSE` & `langroid-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/README.md` & `langroid-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/agent/base.py` & `langroid-0.1.9/langroid/agent/base.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/agent/chat_agent.py` & `langroid-0.1.9/langroid/agent/chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/agent/chat_document.py` & `langroid-0.1.9/langroid/agent/chat_document.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/agent/special/doc_chat_agent.py` & `langroid-0.1.9/langroid/agent/special/doc_chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/agent/special/recipient_validator_agent.py` & `langroid-0.1.9/langroid/agent/special/recipient_validator_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/agent/special/retriever_agent.py` & `langroid-0.1.9/langroid/agent/special/retriever_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/agent/task.py` & `langroid-0.1.9/langroid/agent/task.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/agent/tool_message.py` & `langroid-0.1.9/langroid/agent/tool_message.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/cachedb/base.py` & `langroid-0.1.9/langroid/cachedb/base.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/cachedb/redis_cachedb.py` & `langroid-0.1.9/langroid/cachedb/redis_cachedb.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/embedding_models/base.py` & `langroid-0.1.9/langroid/embedding_models/base.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/embedding_models/models.py` & `langroid-0.1.9/langroid/embedding_models/models.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/language_models/base.py` & `langroid-0.1.9/langroid/language_models/base.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/language_models/openai_gpt.py` & `langroid-0.1.9/langroid/language_models/openai_gpt.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/language_models/utils.py` & `langroid-0.1.9/langroid/language_models/utils.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/mytypes.py` & `langroid-0.1.9/langroid/mytypes.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/parsing/agent_chats.py` & `langroid-0.1.9/langroid/parsing/agent_chats.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/parsing/code_parser.py` & `langroid-0.1.9/langroid/parsing/code_parser.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/parsing/json.py` & `langroid-0.1.9/langroid/parsing/json.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/parsing/para_sentence_split.py` & `langroid-0.1.9/langroid/parsing/para_sentence_split.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/parsing/parser.py` & `langroid-0.1.9/langroid/parsing/parser.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/parsing/repo_loader.py` & `langroid-0.1.9/langroid/parsing/repo_loader.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/parsing/url_loader.py` & `langroid-0.1.9/langroid/parsing/url_loader.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/parsing/urls.py` & `langroid-0.1.9/langroid/parsing/urls.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/parsing/utils.py` & `langroid-0.1.9/langroid/parsing/utils.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/prompts/templates.py` & `langroid-0.1.9/langroid/prompts/templates.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/prompts/transforms.py` & `langroid-0.1.9/langroid/prompts/transforms.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/utils/configuration.py` & `langroid-0.1.9/langroid/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/utils/logging.py` & `langroid-0.1.9/langroid/utils/logging.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/utils/output/printing.py` & `langroid-0.1.9/langroid/utils/output/printing.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/utils/system.py` & `langroid-0.1.9/langroid/utils/system.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/vector_store/base.py` & `langroid-0.1.9/langroid/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/vector_store/chromadb.py` & `langroid-0.1.9/langroid/vector_store/chromadb.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/langroid/vector_store/qdrantdb.py` & `langroid-0.1.9/langroid/vector_store/qdrantdb.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.8/pyproject.toml` & `langroid-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langroid"
-version = "0.1.8"
+version = "0.1.9"
 description = "Harness LLMs with Multi-Agent Programming"
 authors = ["Prasad Chalasani <pchalasani@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
@@ -42,36 +42,48 @@
 ruff = "^0.0.270"
 pre-commit = "^3.3.2"
 types-redis = "^4.5.5.2"
 types-requests = "^2.31.0.1"
 pyparsing = "^3.0.9"
 nltk = "^3.8.1"
 # optional; see extras section below
-sentence-transformers = {version="^2.2.2", optional=true}
-torch = {version="2.0.0", optional=true}
-docker = {version="^6.1.2", optional=true}
+#sentence-transformers = {version="^2.2.2", optional=true}
+#torch = {version="2.0.0", optional=true}
+#docker = {version="^6.1.2", optional=true}
 qdrant-client = "^1.3.1"
 pydantic = "1.10.11"
 
+[tool.poetry.group.hf-embeddings]
+optional = true
+
+[tool.poetry.group.hf-embeddings.dependencies]
+sentence-transformers = "^2.2.2"
+torch = "^2.0.0"
+
+[tool.poetry.group.docker]
+optional = true
+
+[tool.poetry.group.docker.dependencies]
+docker = "^6.1.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 coverage = "^7.2.5"
 
 [tool.poetry.extras]
 # install these using `poetry install -E hf-embeddings`
 hf-embeddings = ["sentence-transformer", "torch"]
 # install these using `poetry install -E docker`
 docker = ["docker"]
 
-[[tool.poetry.source]]
-name = "repositories.testpypi"
-url = "https://test.pypi.org/legacy/"
-default = false
-secondary = false
+#[[tool.poetry.source]]
+#name = "repositories.testpypi"
+#url = "https://test.pypi.org/legacy/"
+#default = false
+#secondary = false
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
```

### Comparing `langroid-0.1.8/setup.py` & `langroid-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,29 +55,25 @@
  'tiktoken>=0.3.3,<0.4.0',
  'trafilatura>=1.5.0,<2.0.0',
  'typer>=0.7.0,<0.8.0',
  'types-redis>=4.5.5.2,<5.0.0.0',
  'types-requests>=2.31.0.1,<3.0.0.0',
  'wget>=3.2,<4.0']
 
-extras_require = \
-{'docker': ['docker>=6.1.2,<7.0.0'], 'hf-embeddings': ['torch==2.0.0']}
-
 setup_kwargs = {
     'name': 'langroid',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Harness LLMs with Multi-Agent Programming',
     'long_description': '<div style="display: flex; align-items: center;">\n  <img src="docs/assets/orange-logo.png" alt="Logo" \n        width="80" height="80"align="left">\n  <h1>Langroid</h1>\n</div>\n\n[![Pytest](https://github.com/langroid/langroid/actions/workflows/pytest.yml/badge.svg)](https://github.com/langroid/langroid/actions/workflows/pytest.yml)\n[![Lint](https://github.com/langroid/langroid/actions/workflows/validate.yml/badge.svg)](https://github.com/langroid/langroid/actions/workflows/validate.yml)\n[![Docs](https://github.com/langroid/langroid/actions/workflows/mkdocs-deploy.yml/badge.svg)](https://github.com/langroid/langroid/actions/workflows/mkdocs-deploy.yml)\n\n\n## Contributors:\n- Prasad Chalasani (Independent ML Consultant)\n- Somesh Jha (Professor of CS, U Wisc at Madison)\n- Mohannad Alhanahnah (Research Associate, U Wisc at Madison)\n- Ashish Hooda (PhD Candidate, U Wisc at Madison)\n\n## Set up dev env\n\nWe use [`poetry`](https://python-poetry.org/docs/#installation) \nto manage dependencies, and `python 3.11` for development.\n\nFirst install `poetry`, then create virtual env and install dependencies:\n\n```bash\n# clone this repo and cd into repo root\ngit clone ...\ncd <repo_root>\n# create a virtual env under project root, .venv directory\npython3 -m venv .venv\n\n# activate the virtual env\n. .venv/bin/activate\n\n# use poetry to install dependencies (these go into .venv dir)\npoetry install\n\n# To be able to run `dockerchat` you need some extras:\npoetry install -E docker\n```\nTo add packages, use `poetry add <package-name>`. This will automatically \nfind the latest compatible version of the package and add it to `pyproject.\ntoml`. _Do not manually edit `pyproject.toml` to add packages._\n\n## Set up environment variables (API keys, etc\n\nCopy the `.env-template` file to a new file `.env` and \ninsert these secrets:\n- OpenAI API key, \n- GitHub Personal Access Token (needed by  PyGithub to analyze git repos; \n  token-based API calls are less rate-limited).\n- Redis Password (ask @pchalasani for this) for the redis cache.\n- Qdrant API key (ask @pchalasani for this) for the vector db.\n\n```bash\ncp .env-template .env\n# now edit the .env file, insert your secrets as above\n``` \n\nCurrently only OpenAI models are supported. Others will be added later.\n\n## Run tests\nTo verify your env is correctly setup, run all tests using `make tests`.\n\n## Generate docs (private only for now)\n\nGenerate docs: `make docs`, then go to the IP address shown at the end, like \n`http://127.0.0.1:8000/`\nNote this runs a docs server in the background.\nTo stop it, run `make nodocs`. Also, running `make docs` next time will kill \nany previously running `mkdocs` server.\n\n\n## Contributing, and Pull requests\n\nIn this Python repository, we prioritize code readability and maintainability.\nTo ensure this, please adhere to the following guidelines when contributing:\n\n1. **Type-Annotate Code:** Add type annotations to function signatures and\n   variables to make the code more self-explanatory and to help catch potential\n   issues early. For example, `def greet(name: str) -> str:`.\n\n2. **Google-Style Docstrings:** Use Google-style docstrings to clearly describe\n   the purpose, arguments, and return values of functions. For example:\n\n   ```python\n   def greet(name: str) -> str:\n       """Generate a greeting message.\n\n       Args:\n           name (str): The name of the person to greet.\n\n       Returns:\n           str: The greeting message.\n       """\n       return f"Hello, {name}!"\n   ```\n\n3. **PEP8-Compliant 80-Char Max per Line:** Follow the PEP8 style guide and keep\n   lines to a maximum of 80 characters. This improves readability and ensures\n   consistency across the codebase.\n\nIf you are using an LLM to write code for you, adding these \ninstructions will usually get you code compliant with the above:\n```\nuse type-annotations, google-style docstrings, and pep8 compliant max 80 \n     chars per line.\n```     \n\n\nBy following these practices, we can create a clean, consistent, and\neasy-to-understand codebase for all contributors. Thank you for your\ncooperation!\n\nTo check for issues locally, run `make check`, it runs linters `black`, `ruff`,\n`flake8` and type-checker `mypy`. Issues flagged by `black` can usually be \nauto-fixed using `black .`, and to fix `ruff issues`, do:\n```\npoetry run ruff . --fix\n```\n\n- When you run this, `black` may warn that some files _would_ be reformatted. \nIf so, you should just run `black .` to reformat them. Also,\n- `flake8` may warn about some issues; read about each one and fix those \n  issues.\n\nYou can also run `make lint` to (try to) auto-tix `black` and `ruff`\nissues. \n\nSo, typically when submitting a PR, you would do this sequence:\n- run `pytest tests -nc` (`-nc` means "no cache", i.e. do not use cached LLM \n  API call responses)\n- fix things so tests pass, then proceed to lint/style/type checks\n- `make check` to see what issues there are\n- `make lint` to auto-fix some of them\n- `make check` again to see what issues remain\n- possibly manually fix `flake8` issues, and any `mypy` issues flagged.\n- `make check` again to see if all issues are fixed.\n- repeat if needed, until all clean. \n\nWhen done with these, git-commit, push to github and submit the PR. If this \nis an ongoing PR, just push to github again and the PR will be updated. \n\nStrongly recommend to use the `gh` command-line utility when working with git.\nRead more [here](docs/development/github-cli.md).\n\n\n\n## Run some examples\n\nThere  are now several examples under `examples` and `examples_dev`. \nThey are typically run with `python3 examples/.../chat.py`, but sometimes \nthe app name may not be `chat.py`.\nGenerally speaking, these commands can take additional command-line options, \ne.g.: \n- `-nc` to disable using cached LLM responses (i.e. forces fresh response)\n- `-d` or `--debug` to see more output\n- `-f` to enable using OpenAI function-calling instead of Langroid tools.\n\nHere are some apps to try (others will be described later):\n\n### "Chat" with a set of URLs.\n\n```bash\npython3 examples/docqa/chat.py\n```\n\nAsk a question you want answered based on the URLs content. The default \nURLs are about various articles and discussions on LLM-based agents, \ncompression and intelligence. If you are using the default URLs, try asking:\n\n> who is Pattie Maes?\n\nand then a follow-up question:\n\n> what did she build?\n\n### "Chat" with a code repo, given the GitHub URL\n```bash\npython3 examples_dev/codechat/codechat.py\n```\nFor the default URL, try asking: \n\n> What version of python is used?\n\n### "chat"-based dockerfile creator. \nThis is a 3-agent system to generate a docker file for a (Python) github repo.\n\n\n```bash\npython3 examples_dev/dockerfile/chat.py\n```\n\n## Logs of multi-agent interactions\n\nWhen running a multi-agent chat, e.g. using `task.run()`, two types of logs \nare generated:\n- plain-text logs in `logs/<task_name>.log`\n- tsv logs in `logs/<task_name>.tsv`\n\nWe will go into details of inter-agent chat structure in another place, \nbut for now it is important to realize that the logs show _every attempt at \n  responding to the current pending message, even those that are not allowed_.\nThe ones marked with an asterisk (*) are the ones that are considered the \nresponses for a given `step()` (which is a "turn" in the conversation).\n\nThe plain text logs have color-coding ANSI chars to make them easier to read \nby doing `less <log_file>`. The format is:\n```\n(TaskName) Responder SenderEntity (EntityName) (=> Recipient) TOOL Content\n```\n\nThe structure of the `tsv` logs is similar. A great way to view these is to \ninstall and use `visidata` (https://www.visidata.org/):\n```bash\nvd logs/<task_name>.tsv\n```\n\n',
     'author': 'Prasad Chalasani',
     'author_email': 'pchalasani@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'extras_require': extras_require,
     'python_requires': '>=3.8.1,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `langroid-0.1.8/PKG-INFO` & `langroid-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langroid
-Version: 0.1.8
+Version: 0.1.9
 Summary: Harness LLMs with Multi-Agent Programming
 License: MIT
 Author: Prasad Chalasani
 Author-email: pchalasani@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,14 @@
 Provides-Extra: docker
 Provides-Extra: hf-embeddings
 Requires-Dist: autopep8 (>=2.0.2,<3.0.0)
 Requires-Dist: black[jupyter] (>=23.3.0,<24.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: chromadb (>=0.3.21,<0.4.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
-Requires-Dist: docker (>=6.1.2,<7.0.0) ; extra == "docker"
 Requires-Dist: faker (>=18.9.0,<19.0.0)
 Requires-Dist: fakeredis (>=2.12.1,<3.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: mkdocs (>=1.4.2,<2.0.0)
 Requires-Dist: mkdocs-awesome-pages-plugin (>=2.8.0,<3.0.0)
@@ -43,17 +42,15 @@
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: qdrant-client (>=1.3.1,<2.0.0)
 Requires-Dist: redis (>=4.5.5,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: requests-oauthlib (>=1.3.1,<2.0.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: ruff (>=0.0.270,<0.0.271)
-Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
-Requires-Dist: torch (==2.0.0) ; extra == "hf-embeddings"
 Requires-Dist: trafilatura (>=1.5.0,<2.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Requires-Dist: types-redis (>=4.5.5.2,<5.0.0.0)
 Requires-Dist: types-requests (>=2.31.0.1,<3.0.0.0)
 Requires-Dist: wget (>=3.2,<4.0)
 Description-Content-Type: text/markdown
```

