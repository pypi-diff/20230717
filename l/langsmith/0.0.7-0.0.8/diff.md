# Comparing `tmp/langsmith-0.0.7.tar.gz` & `tmp/langsmith-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langsmith-0.0.7.tar", max compression
+gzip compressed data, was "langsmith-0.0.8.tar", max compression
```

## Comparing `langsmith-0.0.7.tar` & `langsmith-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     8031 2023-07-12 19:19:22.829561 langsmith-0.0.7/README.md
--rw-r--r--   0        0        0      478 2023-07-10 20:55:19.191988 langsmith-0.0.7/langsmith/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 17:54:45.352774 langsmith-0.0.7/langsmith/cli/__init__.py
--rw-r--r--   0        0        0      363 2023-07-05 17:54:45.353156 langsmith-0.0.7/langsmith/cli/conf/nginx.conf
--rw-r--r--   0        0        0      143 2023-07-12 06:25:39.153595 langsmith-0.0.7/langsmith/cli/docker-compose.dev.yaml
--rw-r--r--   0        0        0      315 2023-07-05 17:54:45.353418 langsmith-0.0.7/langsmith/cli/docker-compose.ngrok.yaml
--rw-r--r--   0        0        0     1186 2023-07-12 00:52:45.305623 langsmith-0.0.7/langsmith/cli/docker-compose.yaml
--rw-r--r--   0        0        0    14420 2023-07-15 15:32:37.213445 langsmith-0.0.7/langsmith/cli/main.py
--rw-r--r--   0        0        0    31862 2023-07-15 15:34:27.624335 langsmith-0.0.7/langsmith/client.py
--rw-r--r--   0        0        0      234 2023-07-05 17:54:45.355050 langsmith-0.0.7/langsmith/evaluation/__init__.py
--rw-r--r--   0        0        0     1411 2023-07-05 17:54:45.355316 langsmith-0.0.7/langsmith/evaluation/evaluator.py
--rw-r--r--   0        0        0     1529 2023-07-05 17:54:45.355546 langsmith-0.0.7/langsmith/evaluation/string_evaluator.py
--rw-r--r--   0        0        0     9462 2023-07-05 17:54:45.355760 langsmith-0.0.7/langsmith/run_helpers.py
--rw-r--r--   0        0        0     6116 2023-07-12 00:52:45.306853 langsmith-0.0.7/langsmith/run_trees.py
--rw-r--r--   0        0        0     6499 2023-07-13 17:24:35.594023 langsmith-0.0.7/langsmith/schemas.py
--rw-r--r--   0        0        0     4180 2023-07-15 15:34:27.624819 langsmith-0.0.7/langsmith/utils.py
--rw-r--r--   0        0        0      858 2023-07-15 15:52:31.855998 langsmith-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     8593 1970-01-01 00:00:00.000000 langsmith-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     8107 2023-07-17 14:32:27.346477 langsmith-0.0.8/README.md
+-rw-r--r--   0        0        0      478 2023-07-10 20:55:19.191988 langsmith-0.0.8/langsmith/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:54:45.352774 langsmith-0.0.8/langsmith/cli/__init__.py
+-rw-r--r--   0        0        0      363 2023-07-05 17:54:45.353156 langsmith-0.0.8/langsmith/cli/conf/nginx.conf
+-rw-r--r--   0        0        0      143 2023-07-12 06:25:39.153595 langsmith-0.0.8/langsmith/cli/docker-compose.dev.yaml
+-rw-r--r--   0        0        0      315 2023-07-05 17:54:45.353418 langsmith-0.0.8/langsmith/cli/docker-compose.ngrok.yaml
+-rw-r--r--   0        0        0     1186 2023-07-12 00:52:45.305623 langsmith-0.0.8/langsmith/cli/docker-compose.yaml
+-rw-r--r--   0        0        0    14420 2023-07-15 15:32:37.213445 langsmith-0.0.8/langsmith/cli/main.py
+-rw-r--r--   0        0        0    45457 2023-07-17 14:32:27.347012 langsmith-0.0.8/langsmith/client.py
+-rw-r--r--   0        0        0      234 2023-07-05 17:54:45.355050 langsmith-0.0.8/langsmith/evaluation/__init__.py
+-rw-r--r--   0        0        0     1411 2023-07-05 17:54:45.355316 langsmith-0.0.8/langsmith/evaluation/evaluator.py
+-rw-r--r--   0        0        0     1529 2023-07-05 17:54:45.355546 langsmith-0.0.8/langsmith/evaluation/string_evaluator.py
+-rw-r--r--   0        0        0     9462 2023-07-05 17:54:45.355760 langsmith-0.0.8/langsmith/run_helpers.py
+-rw-r--r--   0        0        0     6116 2023-07-12 00:52:45.306853 langsmith-0.0.8/langsmith/run_trees.py
+-rw-r--r--   0        0        0     6499 2023-07-13 17:24:35.594023 langsmith-0.0.8/langsmith/schemas.py
+-rw-r--r--   0        0        0     4180 2023-07-15 15:34:27.624819 langsmith-0.0.8/langsmith/utils.py
+-rw-r--r--   0        0        0      858 2023-07-17 15:17:02.918787 langsmith-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     8669 1970-01-01 00:00:00.000000 langsmith-0.0.8/PKG-INFO
```

### Comparing `langsmith-0.0.7/README.md` & `langsmith-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 LangSmith helps you and your team develop and evaluate language models and intelligent agents. It is compatible with any LLM Application and provides seamless integration with [LangChain](https://github.com/hwchase17/langchain), a widely recognized open-source framework that simplifies the process for developers to create powerful language model applications.
 
 > **Note**: You can enjoy the benefits of LangSmith without using the LangChain open-source packages! To get started with your own proprietary framework, set up your account and then skip to [Logging Traces Outside LangChain](#logging-traces-outside-langchain).
 
 A typical workflow looks like:
 
-1. Set up an account with LangSmith or host your [local server](https://docs.smith.langchain.com/docs/additional-resources/local_installation).
+1. Set up an account with LangSmith.
 2. Log traces.
 3. Debug, Create Datasets, and Evaluate Runs.
 
 We'll walk through these steps in more detail below.
 
 ## 1. Connect to LangSmith
 
@@ -179,15 +179,17 @@
         outputs=run.outputs,
         dataset_id=dataset.id,
     )
 ```
 
 ## Evaluating Runs
 
-You can run evaluations directly using the LangSmith client.
+Check out the [LangSmith Testing & Evaluation dos](https://docs.smith.langchain.com/docs/evaluation/) for up-to-date workflows.
+
+For generating automated feedback on individual runs, you can run evaluations directly using the LangSmith client.
 
 ```python
 from typing import Optional
 from langsmith.evaluation import StringEvaluator
 
 
 def jaccard_chars(output: str, answer: str) -> float:
```

### Comparing `langsmith-0.0.7/langsmith/cli/docker-compose.yaml` & `langsmith-0.0.8/langsmith/cli/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.7/langsmith/cli/main.py` & `langsmith-0.0.8/langsmith/cli/main.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.7/langsmith/evaluation/evaluator.py` & `langsmith-0.0.8/langsmith/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.7/langsmith/evaluation/string_evaluator.py` & `langsmith-0.0.8/langsmith/evaluation/string_evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.7/langsmith/run_helpers.py` & `langsmith-0.0.8/langsmith/run_helpers.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.7/langsmith/run_trees.py` & `langsmith-0.0.8/langsmith/run_trees.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.7/langsmith/schemas.py` & `langsmith-0.0.8/langsmith/schemas.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.7/langsmith/utils.py` & `langsmith-0.0.8/langsmith/utils.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.7/pyproject.toml` & `langsmith-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langsmith"
-version = "0.0.7"
+version = "0.0.8"
 description = "Client library to connect to the LangSmith LLM Tracing and Evaluation Platform."
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "langsmith"}]
 
 [tool.poetry.scripts]
```

### Comparing `langsmith-0.0.7/PKG-INFO` & `langsmith-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langsmith
-Version: 0.0.7
+Version: 0.0.8
 Summary: Client library to connect to the LangSmith LLM Tracing and Evaluation Platform.
 License: MIT
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -26,15 +26,15 @@
 
 LangSmith helps you and your team develop and evaluate language models and intelligent agents. It is compatible with any LLM Application and provides seamless integration with [LangChain](https://github.com/hwchase17/langchain), a widely recognized open-source framework that simplifies the process for developers to create powerful language model applications.
 
 > **Note**: You can enjoy the benefits of LangSmith without using the LangChain open-source packages! To get started with your own proprietary framework, set up your account and then skip to [Logging Traces Outside LangChain](#logging-traces-outside-langchain).
 
 A typical workflow looks like:
 
-1. Set up an account with LangSmith or host your [local server](https://docs.smith.langchain.com/docs/additional-resources/local_installation).
+1. Set up an account with LangSmith.
 2. Log traces.
 3. Debug, Create Datasets, and Evaluate Runs.
 
 We'll walk through these steps in more detail below.
 
 ## 1. Connect to LangSmith
 
@@ -195,15 +195,17 @@
         outputs=run.outputs,
         dataset_id=dataset.id,
     )
 ```
 
 ## Evaluating Runs
 
-You can run evaluations directly using the LangSmith client.
+Check out the [LangSmith Testing & Evaluation dos](https://docs.smith.langchain.com/docs/evaluation/) for up-to-date workflows.
+
+For generating automated feedback on individual runs, you can run evaluations directly using the LangSmith client.
 
 ```python
 from typing import Optional
 from langsmith.evaluation import StringEvaluator
 
 
 def jaccard_chars(output: str, answer: str) -> float:
```

