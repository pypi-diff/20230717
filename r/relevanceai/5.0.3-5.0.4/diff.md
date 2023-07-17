# Comparing `tmp/relevanceai-5.0.3.tar.gz` & `tmp/relevanceai-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relevanceai-5.0.3.tar", last modified: Mon Jul 17 13:54:04 2023, max compression
+gzip compressed data, was "relevanceai-5.0.4.tar", last modified: Mon Jul 17 13:57:12 2023, max compression
```

## Comparing `relevanceai-5.0.3.tar` & `relevanceai-5.0.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 13:54:04.452156 relevanceai-5.0.3/
--rw-rw-rw-   0        0        0    11547 2023-07-17 13:38:32.000000 relevanceai-5.0.3/LICENSE
--rw-rw-rw-   0        0        0     1192 2023-07-17 13:54:04.451157 relevanceai-5.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      970 2023-07-17 13:38:32.000000 relevanceai-5.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 13:54:04.423157 relevanceai-5.0.3/relevanceai/
--rw-rw-rw-   0        0        0      279 2023-07-17 13:54:01.000000 relevanceai-5.0.3/relevanceai/__init__.py
--rw-rw-rw-   0        0        0      117 2023-07-17 13:38:32.000000 relevanceai-5.0.3/relevanceai/_request.py
--rw-rw-rw-   0        0        0     2158 2023-07-17 13:38:32.000000 relevanceai-5.0.3/relevanceai/auth.py
--rw-rw-rw-   0        0        0     6646 2023-07-17 13:38:32.000000 relevanceai-5.0.3/relevanceai/chain.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:54:04.431157 relevanceai-5.0.3/relevanceai/connect/
--rw-rw-rw-   0        0        0        0 2023-07-17 13:53:04.000000 relevanceai-5.0.3/relevanceai/connect/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:54:04.434157 relevanceai-5.0.3/relevanceai/connect/fastapi/
--rw-rw-rw-   0        0        0       99 2023-07-17 13:49:37.000000 relevanceai-5.0.3/relevanceai/connect/fastapi/__init__.py
--rw-rw-rw-   0        0        0     4325 2023-07-17 13:44:35.000000 relevanceai-5.0.3/relevanceai/connect/fastapi/chains.py
--rw-rw-rw-   0        0        0     3812 2023-07-17 13:50:03.000000 relevanceai-5.0.3/relevanceai/connect/fastapi/steps.py
--rw-rw-rw-   0        0        0     3401 2023-07-17 13:38:32.000000 relevanceai-5.0.3/relevanceai/datasets.py
--rw-rw-rw-   0        0        0     1046 2023-07-17 13:38:32.000000 relevanceai-5.0.3/relevanceai/env.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:54:04.439157 relevanceai-5.0.3/relevanceai/frontend/
--rw-rw-rw-   0        0        0      104 2023-07-17 13:40:02.000000 relevanceai-5.0.3/relevanceai/frontend/__init__.py
--rw-rw-rw-   0        0        0      686 2023-07-17 06:16:31.000000 relevanceai-5.0.3/relevanceai/frontend/input_components.py
--rw-rw-rw-   0        0        0     1908 2023-07-17 13:39:59.000000 relevanceai-5.0.3/relevanceai/frontend/upload_file.py
--rw-rw-rw-   0        0        0     4586 2023-07-17 13:38:32.000000 relevanceai-5.0.3/relevanceai/params.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:54:04.450156 relevanceai-5.0.3/relevanceai/steps/
--rw-rw-rw-   0        0        0      600 2023-07-17 13:38:32.000000 relevanceai-5.0.3/relevanceai/steps/__init__.py
--rw-rw-rw-   0        0        0     2671 2023-07-17 13:38:32.000000 relevanceai-5.0.3/relevanceai/steps/_base.py
--rw-rw-rw-   0        0        0     1994 2023-07-17 13:38:32.000000 relevanceai-5.0.3/relevanceai/steps/api_call.py
--rw-rw-rw-   0        0        0     1150 2023-07-17 13:38:32.000000 relevanceai-5.0.3/relevanceai/steps/execute_javascript.py
--rw-rw-rw-   0        0        0     1285 2023-07-17 13:38:32.000000 relevanceai-5.0.3/relevanceai/steps/generate_vector_embedding.py
--rw-rw-rw-   0        0        0     3751 2023-07-17 13:38:32.000000 relevanceai-5.0.3/relevanceai/steps/prompt_completion.py
--rw-rw-rw-   0        0        0     1721 2023-07-17 13:38:32.000000 relevanceai-5.0.3/relevanceai/steps/redis_vector_search.py
--rw-rw-rw-   0        0        0     1018 2023-07-17 13:38:32.000000 relevanceai-5.0.3/relevanceai/steps/run_chain.py
--rw-rw-rw-   0        0        0     2829 2023-07-17 13:38:32.000000 relevanceai-5.0.3/relevanceai/steps/run_step.py
--rw-rw-rw-   0        0        0     2120 2023-07-17 13:38:32.000000 relevanceai-5.0.3/relevanceai/steps/vector_search.py
--rw-rw-rw-   0        0        0     1728 2023-07-17 13:38:32.000000 relevanceai-5.0.3/relevanceai/steps/vectorize_and_search.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:54:04.431157 relevanceai-5.0.3/relevanceai.egg-info/
--rw-rw-rw-   0        0        0     1192 2023-07-17 13:54:04.000000 relevanceai-5.0.3/relevanceai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1003 2023-07-17 13:54:04.000000 relevanceai-5.0.3/relevanceai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 13:54:04.000000 relevanceai-5.0.3/relevanceai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 13:54:04.000000 relevanceai-5.0.3/relevanceai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-17 13:54:04.000000 relevanceai-5.0.3/relevanceai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 13:54:04.452156 relevanceai-5.0.3/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-07-17 13:38:32.000000 relevanceai-5.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:57:12.676001 relevanceai-5.0.4/
+-rw-rw-rw-   0        0        0    11547 2023-07-17 13:38:32.000000 relevanceai-5.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1192 2023-07-17 13:57:12.675001 relevanceai-5.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      970 2023-07-17 13:38:32.000000 relevanceai-5.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 13:57:12.646989 relevanceai-5.0.4/relevanceai/
+-rw-rw-rw-   0        0        0      279 2023-07-17 13:57:03.000000 relevanceai-5.0.4/relevanceai/__init__.py
+-rw-rw-rw-   0        0        0      117 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/_request.py
+-rw-rw-rw-   0        0        0     2158 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/auth.py
+-rw-rw-rw-   0        0        0     6646 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/chain.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:57:12.656989 relevanceai-5.0.4/relevanceai/connect/
+-rw-rw-rw-   0        0        0        0 2023-07-17 13:53:04.000000 relevanceai-5.0.4/relevanceai/connect/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:57:12.658989 relevanceai-5.0.4/relevanceai/connect/fastapi/
+-rw-rw-rw-   0        0        0       99 2023-07-17 13:56:57.000000 relevanceai-5.0.4/relevanceai/connect/fastapi/__init__.py
+-rw-rw-rw-   0        0        0     4325 2023-07-17 13:44:35.000000 relevanceai-5.0.4/relevanceai/connect/fastapi/chains.py
+-rw-rw-rw-   0        0        0     3812 2023-07-17 13:50:03.000000 relevanceai-5.0.4/relevanceai/connect/fastapi/steps.py
+-rw-rw-rw-   0        0        0     3401 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/datasets.py
+-rw-rw-rw-   0        0        0     1046 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/env.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:57:12.660989 relevanceai-5.0.4/relevanceai/frontend/
+-rw-rw-rw-   0        0        0      104 2023-07-17 13:40:02.000000 relevanceai-5.0.4/relevanceai/frontend/__init__.py
+-rw-rw-rw-   0        0        0      686 2023-07-17 06:16:31.000000 relevanceai-5.0.4/relevanceai/frontend/input_components.py
+-rw-rw-rw-   0        0        0     1908 2023-07-17 13:39:59.000000 relevanceai-5.0.4/relevanceai/frontend/upload_file.py
+-rw-rw-rw-   0        0        0     4586 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/params.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:57:12.675001 relevanceai-5.0.4/relevanceai/steps/
+-rw-rw-rw-   0        0        0      600 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/__init__.py
+-rw-rw-rw-   0        0        0     2671 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/_base.py
+-rw-rw-rw-   0        0        0     1994 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/api_call.py
+-rw-rw-rw-   0        0        0     1150 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/execute_javascript.py
+-rw-rw-rw-   0        0        0     1285 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/generate_vector_embedding.py
+-rw-rw-rw-   0        0        0     3751 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/prompt_completion.py
+-rw-rw-rw-   0        0        0     1721 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/redis_vector_search.py
+-rw-rw-rw-   0        0        0     1018 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/run_chain.py
+-rw-rw-rw-   0        0        0     2829 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/run_step.py
+-rw-rw-rw-   0        0        0     2120 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/vector_search.py
+-rw-rw-rw-   0        0        0     1728 2023-07-17 13:38:32.000000 relevanceai-5.0.4/relevanceai/steps/vectorize_and_search.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:57:12.653989 relevanceai-5.0.4/relevanceai.egg-info/
+-rw-rw-rw-   0        0        0     1192 2023-07-17 13:57:12.000000 relevanceai-5.0.4/relevanceai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1003 2023-07-17 13:57:12.000000 relevanceai-5.0.4/relevanceai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 13:57:12.000000 relevanceai-5.0.4/relevanceai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 13:57:12.000000 relevanceai-5.0.4/relevanceai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-17 13:57:12.000000 relevanceai-5.0.4/relevanceai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 13:57:12.676001 relevanceai-5.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-07-17 13:38:32.000000 relevanceai-5.0.4/setup.py
```

### Comparing `relevanceai-5.0.3/LICENSE` & `relevanceai-5.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/PKG-INFO` & `relevanceai-5.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relevanceai
-Version: 5.0.3
+Version: 5.0.4
 Home-page: https://relevanceai.com/
 Author: Relevance AI
 Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Relevance AI - The platform for building and deploying AI chains and Agents
```

### Comparing `relevanceai-5.0.3/README.md` & `relevanceai-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/auth.py` & `relevanceai-5.0.4/relevanceai/auth.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/chain.py` & `relevanceai-5.0.4/relevanceai/chain.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/connect/fastapi/chains.py` & `relevanceai-5.0.4/relevanceai/connect/fastapi/chains.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/connect/fastapi/steps.py` & `relevanceai-5.0.4/relevanceai/connect/fastapi/steps.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/datasets.py` & `relevanceai-5.0.4/relevanceai/datasets.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/env.py` & `relevanceai-5.0.4/relevanceai/env.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/frontend/input_components.py` & `relevanceai-5.0.4/relevanceai/frontend/input_components.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/frontend/upload_file.py` & `relevanceai-5.0.4/relevanceai/frontend/upload_file.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/params.py` & `relevanceai-5.0.4/relevanceai/params.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/steps/__init__.py` & `relevanceai-5.0.4/relevanceai/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/steps/_base.py` & `relevanceai-5.0.4/relevanceai/steps/_base.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/steps/api_call.py` & `relevanceai-5.0.4/relevanceai/steps/api_call.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/steps/execute_javascript.py` & `relevanceai-5.0.4/relevanceai/steps/execute_javascript.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/steps/generate_vector_embedding.py` & `relevanceai-5.0.4/relevanceai/steps/generate_vector_embedding.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/steps/prompt_completion.py` & `relevanceai-5.0.4/relevanceai/steps/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/steps/redis_vector_search.py` & `relevanceai-5.0.4/relevanceai/steps/redis_vector_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/steps/run_chain.py` & `relevanceai-5.0.4/relevanceai/steps/run_chain.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/steps/run_step.py` & `relevanceai-5.0.4/relevanceai/steps/run_step.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/steps/vector_search.py` & `relevanceai-5.0.4/relevanceai/steps/vector_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai/steps/vectorize_and_search.py` & `relevanceai-5.0.4/relevanceai/steps/vectorize_and_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/relevanceai.egg-info/PKG-INFO` & `relevanceai-5.0.4/relevanceai.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relevanceai
-Version: 5.0.3
+Version: 5.0.4
 Home-page: https://relevanceai.com/
 Author: Relevance AI
 Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Relevance AI - The platform for building and deploying AI chains and Agents
```

### Comparing `relevanceai-5.0.3/relevanceai.egg-info/SOURCES.txt` & `relevanceai-5.0.4/relevanceai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.3/setup.py` & `relevanceai-5.0.4/setup.py`

 * *Files identical despite different names*

