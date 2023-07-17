# Comparing `tmp/decontext-0.1.1.tar.gz` & `tmp/decontext-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decontext-0.1.1.tar", last modified: Fri Jul 14 02:49:07 2023, max compression
+gzip compressed data, was "decontext-0.1.2.tar", last modified: Mon Jul 17 19:26:07 2023, max compression
```

## Comparing `decontext-0.1.1.tar` & `decontext-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,38 @@
-drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-14 02:49:07.214471 decontext-0.1.1/
--rw-r--r--   0 benjaminn  (5207) users      (100)    13576 2023-07-14 02:49:07.213471 decontext-0.1.1/PKG-INFO
--rw-r--r--   0 benjaminn  (5207) users      (100)    12456 2023-07-14 01:41:35.000000 decontext-0.1.1/README.md
--rw-r--r--   0 benjaminn  (5207) users      (100)     3078 2023-07-14 02:38:41.000000 decontext-0.1.1/pyproject.toml
--rw-r--r--   0 benjaminn  (5207) users      (100)       38 2023-07-14 02:49:07.215471 decontext-0.1.1/setup.cfg
-drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-14 02:49:07.112475 decontext-0.1.1/src/
-drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-14 02:49:07.156473 decontext-0.1.1/src/decontext/
--rw-r--r--   0 benjaminn  (5207) users      (100)      120 2023-07-14 01:43:45.000000 decontext-0.1.1/src/decontext/__init__.py
--rw-r--r--   0 benjaminn  (5207) users      (100)     6512 2023-07-12 22:06:39.000000 decontext-0.1.1/src/decontext/cache.py
--rw-r--r--   0 benjaminn  (5207) users      (100)     6503 2023-07-14 01:23:06.000000 decontext-0.1.1/src/decontext/data_types.py
--rw-r--r--   0 benjaminn  (5207) users      (100)      115 2023-07-13 17:38:14.000000 decontext-0.1.1/src/decontext/logging.py
--rw-r--r--   0 benjaminn  (5207) users      (100)    13289 2023-07-14 01:05:17.000000 decontext-0.1.1/src/decontext/model.py
--rw-r--r--   0 benjaminn  (5207) users      (100)     2650 2023-07-14 02:03:38.000000 decontext-0.1.1/src/decontext/pipeline.py
--rw-r--r--   0 benjaminn  (5207) users      (100)        0 2023-07-07 20:57:14.000000 decontext-0.1.1/src/decontext/py.typed
-drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-14 02:49:07.198472 decontext-0.1.1/src/decontext/step/
--rw-r--r--   0 benjaminn  (5207) users      (100)     5892 2023-07-14 00:52:27.000000 decontext-0.1.1/src/decontext/step/qa.py
--rw-r--r--   0 benjaminn  (5207) users      (100)      664 2023-07-13 17:38:14.000000 decontext-0.1.1/src/decontext/step/qgen.py
--rw-r--r--   0 benjaminn  (5207) users      (100)      969 2023-07-13 17:38:14.000000 decontext-0.1.1/src/decontext/step/step.py
--rw-r--r--   0 benjaminn  (5207) users      (100)      685 2023-07-13 17:38:14.000000 decontext-0.1.1/src/decontext/step/synth.py
--rw-r--r--   0 benjaminn  (5207) users      (100)     3840 2023-07-14 01:03:23.000000 decontext-0.1.1/src/decontext/template.py
--rw-r--r--   0 benjaminn  (5207) users      (100)      920 2023-07-14 00:52:27.000000 decontext-0.1.1/src/decontext/utils.py
-drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-14 02:49:07.183472 decontext-0.1.1/src/decontext.egg-info/
--rw-r--r--   0 benjaminn  (5207) users      (100)    13576 2023-07-14 02:49:07.000000 decontext-0.1.1/src/decontext.egg-info/PKG-INFO
--rw-r--r--   0 benjaminn  (5207) users      (100)      606 2023-07-14 02:49:07.000000 decontext-0.1.1/src/decontext.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminn  (5207) users      (100)        1 2023-07-14 02:49:07.000000 decontext-0.1.1/src/decontext.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminn  (5207) users      (100)      477 2023-07-14 02:49:07.000000 decontext-0.1.1/src/decontext.egg-info/requires.txt
--rw-r--r--   0 benjaminn  (5207) users      (100)       10 2023-07-14 02:49:07.000000 decontext-0.1.1/src/decontext.egg-info/top_level.txt
-drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-14 02:49:07.209471 decontext-0.1.1/tests/
--rw-r--r--   0 benjaminn  (5207) users      (100)     1052 2023-07-14 02:43:59.000000 decontext-0.1.1/tests/test_data_types.py
--rw-r--r--   0 benjaminn  (5207) users      (100)     8590 2023-07-14 00:56:27.000000 decontext-0.1.1/tests/test_pipeline.py
--rw-r--r--   0 benjaminn  (5207) users      (100)      348 2023-07-14 00:52:27.000000 decontext-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-17 19:26:07.788131 decontext-0.1.2/
+-rw-r--r--   0 benjaminn  (5207) users      (100)    13878 2023-07-17 19:26:07.786131 decontext-0.1.2/PKG-INFO
+-rw-r--r--   0 benjaminn  (5207) users      (100)    12758 2023-07-14 20:36:02.000000 decontext-0.1.2/README.md
+-rw-r--r--   0 benjaminn  (5207) users      (100)     3093 2023-07-17 19:25:34.000000 decontext-0.1.2/pyproject.toml
+-rw-r--r--   0 benjaminn  (5207) users      (100)       38 2023-07-17 19:26:07.788131 decontext-0.1.2/setup.cfg
+drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-17 19:26:07.651137 decontext-0.1.2/src/
+drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-17 19:26:07.703135 decontext-0.1.2/src/decontext/
+-rw-r--r--   0 benjaminn  (5207) users      (100)      120 2023-07-14 01:43:45.000000 decontext-0.1.2/src/decontext/__init__.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)     6676 2023-07-14 20:16:15.000000 decontext-0.1.2/src/decontext/cache.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)     6503 2023-07-14 01:23:06.000000 decontext-0.1.2/src/decontext/data_types.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)      115 2023-07-13 17:38:14.000000 decontext-0.1.2/src/decontext/logging.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)    13289 2023-07-14 01:05:17.000000 decontext-0.1.2/src/decontext/model.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)     2650 2023-07-14 02:03:38.000000 decontext-0.1.2/src/decontext/pipeline.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)        0 2023-07-07 20:57:14.000000 decontext-0.1.2/src/decontext/py.typed
+drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-17 19:26:07.744133 decontext-0.1.2/src/decontext/step/
+-rw-r--r--   0 benjaminn  (5207) users      (100)     6062 2023-07-16 15:46:42.000000 decontext-0.1.2/src/decontext/step/qa.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)      767 2023-07-16 15:53:33.000000 decontext-0.1.2/src/decontext/step/qgen.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)     1033 2023-07-14 15:49:13.000000 decontext-0.1.2/src/decontext/step/step.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)      788 2023-07-14 16:37:13.000000 decontext-0.1.2/src/decontext/step/synth.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)     4115 2023-07-16 15:54:26.000000 decontext-0.1.2/src/decontext/template.py
+drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-17 19:26:07.765132 decontext-0.1.2/src/decontext/templates/
+-rw-r--r--   0 benjaminn  (5207) users      (100)        0 2023-07-14 15:40:25.000000 decontext-0.1.2/src/decontext/templates/__init__.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)      624 2023-07-12 00:22:38.000000 decontext-0.1.2/src/decontext/templates/qa_fulltext.yaml
+-rw-r--r--   0 benjaminn  (5207) users      (100)      957 2023-07-12 20:55:22.000000 decontext-0.1.2/src/decontext/templates/qa_retrieval.yaml
+-rw-r--r--   0 benjaminn  (5207) users      (100)     1045 2023-07-12 00:21:41.000000 decontext-0.1.2/src/decontext/templates/qgen.yaml
+-rw-r--r--   0 benjaminn  (5207) users      (100)     1456 2023-07-12 00:19:47.000000 decontext-0.1.2/src/decontext/templates/synth.yaml
+-rw-r--r--   0 benjaminn  (5207) users      (100)      920 2023-07-14 00:52:27.000000 decontext-0.1.2/src/decontext/utils.py
+drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-17 19:26:07.727134 decontext-0.1.2/src/decontext.egg-info/
+-rw-r--r--   0 benjaminn  (5207) users      (100)    13878 2023-07-17 19:26:07.000000 decontext-0.1.2/src/decontext.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminn  (5207) users      (100)      814 2023-07-17 19:26:07.000000 decontext-0.1.2/src/decontext.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminn  (5207) users      (100)        1 2023-07-17 19:26:07.000000 decontext-0.1.2/src/decontext.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminn  (5207) users      (100)      477 2023-07-17 19:26:07.000000 decontext-0.1.2/src/decontext.egg-info/requires.txt
+-rw-r--r--   0 benjaminn  (5207) users      (100)       10 2023-07-17 19:26:07.000000 decontext-0.1.2/src/decontext.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-17 19:26:07.783131 decontext-0.1.2/tests/
+-rw-r--r--   0 benjaminn  (5207) users      (100)     1641 2023-07-16 15:53:55.000000 decontext-0.1.2/tests/test_cache.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)     1052 2023-07-14 02:43:59.000000 decontext-0.1.2/tests/test_data_types.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)     8590 2023-07-17 19:02:09.000000 decontext-0.1.2/tests/test_pipeline.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)      348 2023-07-14 00:52:27.000000 decontext-0.1.2/tests/test_utils.py
```

### Comparing `decontext-0.1.1/PKG-INFO` & `decontext-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decontext
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pipeline for decontextualization of scientific snippets.
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>, Benjamin Newman <bnewmancommercial@gmail.com>, Luca Soldaini <luca@soldaini.net>, Kyle Lo <kylel@allenai.org>
 Maintainer-email: Benjamin Newman <bnewmancommercial@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/bnewm0609/qa-decontextualization
 Project-URL: Repository, https://github.com/bnewm0609/qa-decontextualization
 Project-URL: Bug Tracker, https://github.com/bnewm0609/qa-decontextualization/issues
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # QA Decontextualization
 
 See `experiments` for description of how to run experiments investigating this method.
 
@@ -40,19 +40,22 @@
 ## Quick Start
 
 1. Set your OpenAI API key
 ```bash
 export OPENAI_API_KEY='yourkey'
 ```
 
+By default, all requests to APIs are cached at `$HOME/.cache/decontext`, but this can be changed by setting the environment variable `export DECONTEXT_CACHE_DIR=path/to/cache`.
+
 2. Decontextualize
 
 To decontextualize a snippet using some context, you can pass both the snippet and context to the decontextualization function.
 Currently, the expected format for the context is __entire full-text papers__.
 These include the title, abstract, and the sections of the paper.
+The title, abstract, and full text are all required fields.
 The `PaperContext` class, which holds these full-texts is a Pydantic model, so its values can be parsed from `json` strings as shown below.
 <!-- The decontextualization will be best if it includes certain parts of the paper: especially the title, abstract, and the paragraph surrounding the snippet. If these can't be found, a warning will be raised.
 ```python
 from decontext import decontext
 
 context_paragraph_1 = "Data collection. Subreddits are sub-communities on Reddit oriented around specific interests or topics, such as technology or politics. Sampling from Reddit as a whole would bias the model towards the most commonly discussed content. But by sampling posts from individual subreddits, we can control the kinds of posts we use to train our model. To collect a diverse training dataset, we have randomly sampled 1000 posts each from the subreddits politics, business, science, and AskReddit, and 1000 additional posts from the Reddit frontpage. All posts in our sample appeared between January 2007 and March 2015, and to control for length effects, contain between 300 and 400 characters. This results in a total training dataset of 5000 posts."
 
@@ -116,14 +119,15 @@
 Additionally, the `decontext` function also supports using multiple papers as context:
 ```python
 decontext(snippet=snippet, context=paper_1_context, additional_context=[paper_2_context])
 ```
 The argument `context` should be the one that contains the snippet. The argument `additional_context` can contain other potentially useful material (e.g. papers that are cited in the snippet).
 
 3. Debugging
+
 For debugging purposes, it's useful to have access to the intermediate outputs of the pipeline. To show these, set the `return_metadata` argument to `True`. The returned metadata is an instance of `decontext.PaperSnippet`, which contains these outputs along with the cost of the run.
 ```python
 new_snippet, metadata = decontext(snippet, paper_1, return_metadata=True)
 
 >   PaperSnippet({
         "idx": "<unique identifier for the snippet>" ,
         "snippet": "<original snippet>",
@@ -212,33 +216,32 @@
     TemplateQAStep(),
     TemplateSynthStep(),
 ])
 
 decontext(snippet=snippet, context=context, pipeline=pipeline)
 ```
 
-
+The templates used to prompt OpenAI models for the default Pipeline are `yaml` files defined in `src/decontext/templates`.
 
 ## Function Declaration
 ```python
 def decontext(
     snippet: str,
-    context: PaperContext, # Union[str, List[str], PaperContext, List[PaperContext]],
+    context: PaperContext,
     additional_contexts: Optional[List[PaperContext]] = None,
-    # config: Union[Config, str, Path] = "configs/default.yaml",
     pipeline: Optional[Pipeline] = None,
     return_metadata: bool = False,
 ) -> Union[str, Tuple[str, PaperSnippet]]:
     """Decontextualizes the snippet using the given context according to the given config.
 
     Args:
         snippet: The text snippet to decontextualize.
         context: The context to incorporate into the decontextualization. This context must include the snippet.
         additional_contexts: Additional context to use in the decontextualization (eg papers that are cited in the snippet).
-        pipeline: The pipeline to run on the snippet.
+        pipeline: The pipeline to run on the snippet. If not provided, a default retrieval-based pipeline will be run.
         return_metadata: Flag for returning the PaperSnippet object with intermediate outputs. (See below).
 
     Returns:
         string with the decontextualized version of the snippet.
 
         if `return_metadata = True`, additionally return the intermediate results for each step of the pipeline
         as described above.
```

### Comparing `decontext-0.1.1/README.md` & `decontext-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,19 +18,22 @@
 ## Quick Start
 
 1. Set your OpenAI API key
 ```bash
 export OPENAI_API_KEY='yourkey'
 ```
 
+By default, all requests to APIs are cached at `$HOME/.cache/decontext`, but this can be changed by setting the environment variable `export DECONTEXT_CACHE_DIR=path/to/cache`.
+
 2. Decontextualize
 
 To decontextualize a snippet using some context, you can pass both the snippet and context to the decontextualization function.
 Currently, the expected format for the context is __entire full-text papers__.
 These include the title, abstract, and the sections of the paper.
+The title, abstract, and full text are all required fields.
 The `PaperContext` class, which holds these full-texts is a Pydantic model, so its values can be parsed from `json` strings as shown below.
 <!-- The decontextualization will be best if it includes certain parts of the paper: especially the title, abstract, and the paragraph surrounding the snippet. If these can't be found, a warning will be raised.
 ```python
 from decontext import decontext
 
 context_paragraph_1 = "Data collection. Subreddits are sub-communities on Reddit oriented around specific interests or topics, such as technology or politics. Sampling from Reddit as a whole would bias the model towards the most commonly discussed content. But by sampling posts from individual subreddits, we can control the kinds of posts we use to train our model. To collect a diverse training dataset, we have randomly sampled 1000 posts each from the subreddits politics, business, science, and AskReddit, and 1000 additional posts from the Reddit frontpage. All posts in our sample appeared between January 2007 and March 2015, and to control for length effects, contain between 300 and 400 characters. This results in a total training dataset of 5000 posts."
 
@@ -94,14 +97,15 @@
 Additionally, the `decontext` function also supports using multiple papers as context:
 ```python
 decontext(snippet=snippet, context=paper_1_context, additional_context=[paper_2_context])
 ```
 The argument `context` should be the one that contains the snippet. The argument `additional_context` can contain other potentially useful material (e.g. papers that are cited in the snippet).
 
 3. Debugging
+
 For debugging purposes, it's useful to have access to the intermediate outputs of the pipeline. To show these, set the `return_metadata` argument to `True`. The returned metadata is an instance of `decontext.PaperSnippet`, which contains these outputs along with the cost of the run.
 ```python
 new_snippet, metadata = decontext(snippet, paper_1, return_metadata=True)
 
 >   PaperSnippet({
         "idx": "<unique identifier for the snippet>" ,
         "snippet": "<original snippet>",
@@ -190,33 +194,32 @@
     TemplateQAStep(),
     TemplateSynthStep(),
 ])
 
 decontext(snippet=snippet, context=context, pipeline=pipeline)
 ```
 
-
+The templates used to prompt OpenAI models for the default Pipeline are `yaml` files defined in `src/decontext/templates`.
 
 ## Function Declaration
 ```python
 def decontext(
     snippet: str,
-    context: PaperContext, # Union[str, List[str], PaperContext, List[PaperContext]],
+    context: PaperContext,
     additional_contexts: Optional[List[PaperContext]] = None,
-    # config: Union[Config, str, Path] = "configs/default.yaml",
     pipeline: Optional[Pipeline] = None,
     return_metadata: bool = False,
 ) -> Union[str, Tuple[str, PaperSnippet]]:
     """Decontextualizes the snippet using the given context according to the given config.
 
     Args:
         snippet: The text snippet to decontextualize.
         context: The context to incorporate into the decontextualization. This context must include the snippet.
         additional_contexts: Additional context to use in the decontextualization (eg papers that are cited in the snippet).
-        pipeline: The pipeline to run on the snippet.
+        pipeline: The pipeline to run on the snippet. If not provided, a default retrieval-based pipeline will be run.
         return_metadata: Flag for returning the PaperSnippet object with intermediate outputs. (See below).
 
     Returns:
         string with the decontextualized version of the snippet.
 
         if `return_metadata = True`, additionally return the intermediate results for each step of the pipeline
         as described above.
```

### Comparing `decontext-0.1.1/pyproject.toml` & `decontext-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "decontext"
-version = "0.1.1"
+version = "0.1.2"
 description = """\
 Pipeline for decontextualization of scientific snippets.
 """
 license = {text = "Apache-2.0"}
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dependencies = [
     "anthropic==0.2.10",
     "diskcache==5.6.1",
     "filelock==3.12.2",
     "Jinja2==3.1.2",
     "shadow-scholar==0.6.1",
     "omegaconf==2.2.3",
@@ -65,15 +65,15 @@
 "Bug Tracker" = "https://github.com/bnewm0609/qa-decontextualization/issues"
 
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-decontext = ["py.typed"]
+decontext = ["py.typed", "templates/*"]
 
 
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = [
     "setuptools >= 61.0.0",
     "pip >= 21.0.0",
```

### Comparing `decontext-0.1.1/src/decontext/cache.py` & `decontext-0.1.2/src/decontext/cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import json
+import os
 from pathlib import Path
 
 from diskcache import Index
 from filelock import FileLock
 
 
-OPENAI_CACHE_DIR = f"{Path.home()}/nfs/.cache/openai/"
-OPENAI_DISKCACHE_DIR = f"{Path.home()}/nfs/.cache/openai_diskcache/"
+CACHE_DIR = os.environ.get(
+    "DECONTEXT_CACHE_DIR", f"{Path.home()}/.cache/decontext"
+)
+OPENAI_CACHE_DIR = f"{CACHE_DIR}/jsoncache/"
+OPENAI_DISKCACHE_DIR = f"{CACHE_DIR}/diskcache/"
 
 
 class DiskCache:
     def __init__(
         self, cache: dict, cache_dir: str, enforce_cached: bool = False
     ) -> None:
         """Initialize the Cache.
@@ -55,14 +59,16 @@
         Args:
             key (str): The key to the cache.
             fn (Callable): The function to call upon a cache miss.
 
         Returns:
             The value stored at the key or the result of calling the function.
         """
+        # breakpoint()
+        # assert self.cache_dir == "~/nfs/.cache/decontext/diskcache"
         if key in self._cache:
             print("Found example in cache")
             return self._cache[key]
         else:
             if not self.enforce_cached:
                 self._cache[key] = fn()
                 # self.save()
```

### Comparing `decontext-0.1.1/src/decontext/data_types.py` & `decontext-0.1.2/src/decontext/data_types.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.1/src/decontext/model.py` & `decontext-0.1.2/src/decontext/model.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.1/src/decontext/pipeline.py` & `decontext-0.1.2/src/decontext/pipeline.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.1/src/decontext/step/qa.py` & `decontext-0.1.2/src/decontext/step/qa.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import json
 import os
 import tempfile
 from collections import defaultdict
 from contextlib import ExitStack
+from importlib import resources
 
 from shadow_scholar.app import pdod
 
 from decontext.data_types import PaperSnippet, Section
 from decontext.step.step import QAStep, TemplatePipelineStep
 from decontext.utils import none_check
 
 
 class TemplateRetrievalQAStep(QAStep, TemplatePipelineStep):
     """Template step that does retrieval"""
 
     def __init__(self):
-        super().__init__(
-            model_name="gpt-4", template="templates/qa_retrieval.yaml"
-        )
+        with resources.path("decontext.templates", "qa_retrieval.yaml") as f:
+            template_path = f
+        super().__init__(model_name="gpt-4", template=template_path)
 
     def retrieve(self, paper_snippet: PaperSnippet):
         # TODO: cache these
         additional_contexts = none_check(paper_snippet.additional_contexts, [])
         contexts = [paper_snippet.context] + additional_contexts
         # 1. create the doc(s)
 
@@ -98,15 +99,14 @@
             os.remove(query_file_name)
             os.remove(retrieval_output_file_name)
 
         return paper_retrieval_output_file
 
     def run(self, snippet: PaperSnippet):
         self.retrieve(snippet)
-
         for question in snippet.qae:
             unique_evidence = set(
                 [
                     ev.paragraph
                     for ev in (none_check(question.evidence, []))
                     if (
                         ev.paragraph != snippet.context.abstract
@@ -127,31 +127,30 @@
                     "title": snippet.context.title,
                     "abstract": snippet.context.abstract,
                     "section_with_snippet": section_with_snippet,
                     "paragraph_with_snippet": paragraph_with_snippet,
                     "unique_evidence": list(unique_evidence),
                 }
             )
-
             result = self.model(prompt)
             answer = self.model.extract_text(result)
             snippet.add_answer(qid=question.qid, answer=answer)
             snippet.add_cost(result.cost)
 
 
 class TemplateFullTextQAStep(QAStep, TemplatePipelineStep):
     """Runs the QA component of the decontextualization Pipeline using the whole context paper.
 
     All additional context papers are ignored.
     """
 
     def __init__(self):
-        super().__init__(
-            model_name="gpt-4", template="templates/qa_fulltext.yaml"
-        )
+        with resources.path("decontext.templates", "qa_fulltext.yaml") as f:
+            template_path = f
+        super().__init__(model_name="gpt-4", template=template_path)
 
     def run(self, snippet: PaperSnippet):
         for question in snippet.qae:
             prompt = self.template.fill(
                 {
                     "snippet": snippet.snippet,
                     "question": question.question,
```

### Comparing `decontext-0.1.1/src/decontext/step/qgen.py` & `decontext-0.1.2/src/decontext/step/synth.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+from importlib import resources
+
 from decontext.data_types import PaperSnippet
-from decontext.step.step import TemplatePipelineStep, QGenStep
+from .step import TemplatePipelineStep, SynthesisStep
 
 
-class TemplateQGenStep(QGenStep, TemplatePipelineStep):
+class TemplateSynthStep(SynthesisStep, TemplatePipelineStep):
     def __init__(self):
-        super().__init__(
-            model_name="text-davinci-003", template="templates/qgen.yaml"
-        )
+        with resources.path("decontext.templates", "synth.yaml") as f:
+            template_path = f
+        super().__init__(model_name="text-davinci-003", template=template_path)
 
     def run(self, snippet: PaperSnippet):
-        prompt = self.template.fill(snippet.dict())
+        prompt = self.template.fill(
+            {
+                "questions": snippet.qae,
+                "sentence": snippet.snippet,
+            }
+        )
+
         response = self.model(prompt)
-        text = self.model.extract_text(response)
-        for line in text.strip().splitlines():
-            question = line.lstrip(" -*")
-            snippet.add_question(question=question)
+        synth = self.model.extract_text(response)
+        snippet.add_decontextualized_snippet(synth)
         snippet.add_cost(response.cost)
```

### Comparing `decontext-0.1.1/src/decontext/step/step.py` & `decontext-0.1.2/src/decontext/step/step.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from pathlib import Path
+from typing import Union
+
 from decontext.data_types import PaperSnippet
 from decontext.model import load_model
 from decontext.template import Template
 
 
 class PipelineStep:
     """Base class for Pipeline components."""
@@ -25,15 +28,15 @@
 class SynthesisStep(PipelineStep):
     name = "synth"
 
 
 class TemplatePipelineStep(PipelineStep):
     """Base class for steps that use templates"""
 
-    def __init__(self, model_name: str, template: str):
+    def __init__(self, model_name: str, template: Union[str, Path]):
         """Initialize the Pipeline step by loading a model
 
         Args:
             model_name (str): name of the api model to use (e.g. 'text-davinci-003')
             template (str): template or path to template
         """
```

### Comparing `decontext-0.1.1/src/decontext/template.py` & `decontext-0.1.2/src/decontext/template.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 from jinja2 import Template as JTemplate
 import yaml
 
 from decontext.data_types import OpenAIChatMessage
 
 
 class Template:
-    def __init__(self, template: Union[str, List]):
+    def __init__(self, template: Union[Path, str, List]):
         self.template = self.load_template(template)
 
         if isinstance(self.template, str):
             self.template_type = "completion"
         else:
             self.template_type = "openai_chat"
 
     def load_template(
-        self, template: Union[str, List]
+        self, template: Union[Path, str, List]
     ) -> Union[List[OpenAIChatMessage], str]:
         """Load the template from the config.
 
         The passed template takes one of three forms:
         1. a list[dict[str, str]] (for the OpenAI Chat Endpoint). The keys are the role ("user", "system")
             and the values are the template for that message. The dict[str, str] is converted into an
             `OpenAIChatMessage`.
@@ -34,48 +34,53 @@
             template (Union[str, list]): The template or a path to a yaml file with template.
 
         Returns:
             list[OpenAIChatMessage] for the OpenAI Chat API case and a str for the Completion or Claude
             cases with the template. The template is not filled at this point.
         """
 
+        loaded_template: Union[List[OpenAIChatMessage], str] = ""
         # there are a few choices for template:
-        if (
+        if isinstance(template, Path) or (
             isinstance(template, str)
             and len(template) < 256
             and Path(template).is_file()
         ):
+            template = str(template)
             # the template is a path to a file - read the template from the file
             with open(template) as f:
                 if template.endswith("yaml"):
-                    template = yaml.safe_load(f)["template"]
-                    if isinstance(template, list):  # we're using OpenAI chat
-                        template = [
-                            OpenAIChatMessage(**item) for item in template
+                    loaded_template = yaml.safe_load(f)["template"]
+                    if isinstance(
+                        loaded_template, list
+                    ):  # we're using OpenAI chat
+                        loaded_template = [
+                            OpenAIChatMessage(**item)
+                            for item in loaded_template
                         ]
                 else:
-                    template = f.read()
+                    loaded_template = f.read()
         elif isinstance(template, str):
             # assume the template is for a non-chat model. It also could be a path that's misspelled.
             if template.endswith(".yaml") or template.endswith(".txt"):
                 raise FileNotFoundError(
                     f"Make sure path is correct. Unable to find this file: {template}"
                 )
-            template = template
+            loaded_template = template
         elif isinstance(
             template, list
         ):  # or isinstance(template, ListConfig):
             # assume that the passsed thing is the template dict itself
-            template = [OpenAIChatMessage(**item) for item in template]
+            loaded_template = [OpenAIChatMessage(**item) for item in template]
         else:
             raise ValueError(
                 "Template must be either a string, list or path to a valid file"
             )
 
-        return template
+        return loaded_template
 
     def fill(self, fields: dict) -> Union[List[OpenAIChatMessage], str]:
         result: Union[List[OpenAIChatMessage], str] = ""
         if self.template_type == "completion":
             result = JTemplate(
                 self.template, undefined=StrictUndefined
             ).render(fields)
```

### Comparing `decontext-0.1.1/src/decontext/utils.py` & `decontext-0.1.2/src/decontext/utils.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.1/src/decontext.egg-info/PKG-INFO` & `decontext-0.1.2/src/decontext.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decontext
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pipeline for decontextualization of scientific snippets.
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>, Benjamin Newman <bnewmancommercial@gmail.com>, Luca Soldaini <luca@soldaini.net>, Kyle Lo <kylel@allenai.org>
 Maintainer-email: Benjamin Newman <bnewmancommercial@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/bnewm0609/qa-decontextualization
 Project-URL: Repository, https://github.com/bnewm0609/qa-decontextualization
 Project-URL: Bug Tracker, https://github.com/bnewm0609/qa-decontextualization/issues
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # QA Decontextualization
 
 See `experiments` for description of how to run experiments investigating this method.
 
@@ -40,19 +40,22 @@
 ## Quick Start
 
 1. Set your OpenAI API key
 ```bash
 export OPENAI_API_KEY='yourkey'
 ```
 
+By default, all requests to APIs are cached at `$HOME/.cache/decontext`, but this can be changed by setting the environment variable `export DECONTEXT_CACHE_DIR=path/to/cache`.
+
 2. Decontextualize
 
 To decontextualize a snippet using some context, you can pass both the snippet and context to the decontextualization function.
 Currently, the expected format for the context is __entire full-text papers__.
 These include the title, abstract, and the sections of the paper.
+The title, abstract, and full text are all required fields.
 The `PaperContext` class, which holds these full-texts is a Pydantic model, so its values can be parsed from `json` strings as shown below.
 <!-- The decontextualization will be best if it includes certain parts of the paper: especially the title, abstract, and the paragraph surrounding the snippet. If these can't be found, a warning will be raised.
 ```python
 from decontext import decontext
 
 context_paragraph_1 = "Data collection. Subreddits are sub-communities on Reddit oriented around specific interests or topics, such as technology or politics. Sampling from Reddit as a whole would bias the model towards the most commonly discussed content. But by sampling posts from individual subreddits, we can control the kinds of posts we use to train our model. To collect a diverse training dataset, we have randomly sampled 1000 posts each from the subreddits politics, business, science, and AskReddit, and 1000 additional posts from the Reddit frontpage. All posts in our sample appeared between January 2007 and March 2015, and to control for length effects, contain between 300 and 400 characters. This results in a total training dataset of 5000 posts."
 
@@ -116,14 +119,15 @@
 Additionally, the `decontext` function also supports using multiple papers as context:
 ```python
 decontext(snippet=snippet, context=paper_1_context, additional_context=[paper_2_context])
 ```
 The argument `context` should be the one that contains the snippet. The argument `additional_context` can contain other potentially useful material (e.g. papers that are cited in the snippet).
 
 3. Debugging
+
 For debugging purposes, it's useful to have access to the intermediate outputs of the pipeline. To show these, set the `return_metadata` argument to `True`. The returned metadata is an instance of `decontext.PaperSnippet`, which contains these outputs along with the cost of the run.
 ```python
 new_snippet, metadata = decontext(snippet, paper_1, return_metadata=True)
 
 >   PaperSnippet({
         "idx": "<unique identifier for the snippet>" ,
         "snippet": "<original snippet>",
@@ -212,33 +216,32 @@
     TemplateQAStep(),
     TemplateSynthStep(),
 ])
 
 decontext(snippet=snippet, context=context, pipeline=pipeline)
 ```
 
-
+The templates used to prompt OpenAI models for the default Pipeline are `yaml` files defined in `src/decontext/templates`.
 
 ## Function Declaration
 ```python
 def decontext(
     snippet: str,
-    context: PaperContext, # Union[str, List[str], PaperContext, List[PaperContext]],
+    context: PaperContext,
     additional_contexts: Optional[List[PaperContext]] = None,
-    # config: Union[Config, str, Path] = "configs/default.yaml",
     pipeline: Optional[Pipeline] = None,
     return_metadata: bool = False,
 ) -> Union[str, Tuple[str, PaperSnippet]]:
     """Decontextualizes the snippet using the given context according to the given config.
 
     Args:
         snippet: The text snippet to decontextualize.
         context: The context to incorporate into the decontextualization. This context must include the snippet.
         additional_contexts: Additional context to use in the decontextualization (eg papers that are cited in the snippet).
-        pipeline: The pipeline to run on the snippet.
+        pipeline: The pipeline to run on the snippet. If not provided, a default retrieval-based pipeline will be run.
         return_metadata: Flag for returning the PaperSnippet object with intermediate outputs. (See below).
 
     Returns:
         string with the decontextualized version of the snippet.
 
         if `return_metadata = True`, additionally return the intermediate results for each step of the pipeline
         as described above.
```

### Comparing `decontext-0.1.1/src/decontext.egg-info/SOURCES.txt` & `decontext-0.1.2/src/decontext.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,10 +14,16 @@
 src/decontext.egg-info/dependency_links.txt
 src/decontext.egg-info/requires.txt
 src/decontext.egg-info/top_level.txt
 src/decontext/step/qa.py
 src/decontext/step/qgen.py
 src/decontext/step/step.py
 src/decontext/step/synth.py
+src/decontext/templates/__init__.py
+src/decontext/templates/qa_fulltext.yaml
+src/decontext/templates/qa_retrieval.yaml
+src/decontext/templates/qgen.yaml
+src/decontext/templates/synth.yaml
+tests/test_cache.py
 tests/test_data_types.py
 tests/test_pipeline.py
 tests/test_utils.py
```

### Comparing `decontext-0.1.1/tests/test_data_types.py` & `decontext-0.1.2/tests/test_data_types.py`

 * *Files identical despite different names*

### Comparing `decontext-0.1.1/tests/test_pipeline.py` & `decontext-0.1.2/tests/test_pipeline.py`

 * *Files identical despite different names*

