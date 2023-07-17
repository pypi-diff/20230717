# Comparing `tmp/ag_llama_hub-0.0.6.tar.gz` & `tmp/ag_llama_hub-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama_hub-0.0.6.tar", last modified: Wed Jul 12 15:03:23 2023, max compression
+gzip compressed data, was "dist\ag_llama_hub-0.0.7.tar", last modified: Mon Jul 17 11:48:35 2023, max compression
```

## Comparing `ag_llama_hub-0.0.6.tar` & `ag_llama_hub-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 15:03:23.372624 ag_llama_hub-0.0.6/
--rw-rw-rw-   0        0        0      832 2023-07-12 15:03:23.371655 ag_llama_hub-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 15:03:23.354672 ag_llama_hub-0.0.6/ag_llama_hub/
--rw-rw-rw-   0        0        0     2105 2023-07-12 14:53:21.000000 ag_llama_hub-0.0.6/ag_llama_hub/__init__.py
--rw-rw-rw-   0        0        0     4728 2023-07-12 15:03:06.000000 ag_llama_hub-0.0.6/ag_llama_hub/__main__.py
--rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.6/ag_llama_hub/choice.py
--rw-rw-rw-   0        0        0    16256 2023-07-04 11:44:01.000000 ag_llama_hub-0.0.6/ag_llama_hub/model.py
--rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.6/ag_llama_hub/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:03:23.365642 ag_llama_hub-0.0.6/ag_llama_hub.egg-info/
--rw-rw-rw-   0        0        0      832 2023-07-12 15:03:23.000000 ag_llama_hub-0.0.6/ag_llama_hub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-07-12 15:03:23.000000 ag_llama_hub-0.0.6/ag_llama_hub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 15:03:23.000000 ag_llama_hub-0.0.6/ag_llama_hub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-07-12 15:03:23.000000 ag_llama_hub-0.0.6/ag_llama_hub.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-12 15:03:23.000000 ag_llama_hub-0.0.6/ag_llama_hub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 15:03:23.373621 ag_llama_hub-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2567 2023-07-12 13:13:29.000000 ag_llama_hub-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:03:23.368634 ag_llama_hub-0.0.6/utils/
--rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.6/utils/download.py
--rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.6/utils/render.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:48:35.291793 ag_llama_hub-0.0.7/
+-rw-rw-rw-   0        0        0      832 2023-07-17 11:48:35.290795 ag_llama_hub-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-17 11:48:35.274763 ag_llama_hub-0.0.7/ag_llama_hub/
+-rw-rw-rw-   0        0        0     2105 2023-07-12 14:53:21.000000 ag_llama_hub-0.0.7/ag_llama_hub/__init__.py
+-rw-rw-rw-   0        0        0     4794 2023-07-17 11:48:25.000000 ag_llama_hub-0.0.7/ag_llama_hub/__main__.py
+-rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.7/ag_llama_hub/choice.py
+-rw-rw-rw-   0        0        0    16256 2023-07-04 11:44:01.000000 ag_llama_hub-0.0.7/ag_llama_hub/model.py
+-rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.7/ag_llama_hub/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:48:35.285809 ag_llama_hub-0.0.7/ag_llama_hub.egg-info/
+-rw-rw-rw-   0        0        0      832 2023-07-17 11:48:35.000000 ag_llama_hub-0.0.7/ag_llama_hub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-07-17 11:48:35.000000 ag_llama_hub-0.0.7/ag_llama_hub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 11:48:35.000000 ag_llama_hub-0.0.7/ag_llama_hub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-07-17 11:48:35.000000 ag_llama_hub-0.0.7/ag_llama_hub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-17 11:48:35.000000 ag_llama_hub-0.0.7/ag_llama_hub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 11:48:35.291793 ag_llama_hub-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2567 2023-07-12 13:13:29.000000 ag_llama_hub-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:48:35.288801 ag_llama_hub-0.0.7/utils/
+-rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.7/utils/download.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.7/utils/render.py
```

### Comparing `ag_llama_hub-0.0.6/PKG-INFO` & `ag_llama_hub-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag_llama_hub
-Version: 0.0.6
+Version: 0.0.7
 Summary: ag_llama_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama_hub-0.0.6/ag_llama_hub/__init__.py` & `ag_llama_hub-0.0.7/ag_llama_hub/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.6/ag_llama_hub/__main__.py` & `ag_llama_hub-0.0.7/ag_llama_hub/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from . import COMPLETION_MAX_N
 from . import COMPLETION_MAX_LOGPROBS
 
 # Load the language model to be served.
 stream_model = None
 def load_stream_model(model=MODEL,load_in_8bit=MODEL_LOAD_IN_8BIT):
     global stream_model
+    logger.info(f"Loading model {MODEL} in 8bit: {load_in_8bit}")
     stream_model = load_model(
         name_or_path=model,
         revision=MODEL_REVISION,
         cache_dir=MODEL_CACHE_DIR,
         load_in_8bit=load_in_8bit,
         load_in_4bit=MODEL_LOAD_IN_4BIT,
         local_files_only=MODEL_LOCAL_FILES_ONLY,
```

### Comparing `ag_llama_hub-0.0.6/ag_llama_hub/choice.py` & `ag_llama_hub-0.0.7/ag_llama_hub/choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.6/ag_llama_hub/model.py` & `ag_llama_hub-0.0.7/ag_llama_hub/model.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.6/ag_llama_hub/tokenizer.py` & `ag_llama_hub-0.0.7/ag_llama_hub/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.6/ag_llama_hub.egg-info/PKG-INFO` & `ag_llama_hub-0.0.7/ag_llama_hub.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag-llama-hub
-Version: 0.0.6
+Version: 0.0.7
 Summary: ag_llama_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama_hub-0.0.6/setup.py` & `ag_llama_hub-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.6/utils/download.py` & `ag_llama_hub-0.0.7/utils/download.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.6/utils/render.py` & `ag_llama_hub-0.0.7/utils/render.py`

 * *Files identical despite different names*

