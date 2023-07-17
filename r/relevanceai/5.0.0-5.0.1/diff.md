# Comparing `tmp/relevanceai-5.0.0.tar.gz` & `tmp/relevanceai-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relevanceai-5.0.0.tar", last modified: Mon Jul 17 13:42:56 2023, max compression
+gzip compressed data, was "relevanceai-5.0.1.tar", last modified: Mon Jul 17 13:45:25 2023, max compression
```

## Comparing `relevanceai-5.0.0.tar` & `relevanceai-5.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 13:42:56.404912 relevanceai-5.0.0/
--rw-rw-rw-   0        0        0    11547 2023-07-17 13:38:32.000000 relevanceai-5.0.0/LICENSE
--rw-rw-rw-   0        0        0     1192 2023-07-17 13:42:56.403913 relevanceai-5.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      970 2023-07-17 13:38:32.000000 relevanceai-5.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 13:42:56.353330 relevanceai-5.0.0/relevanceai/
--rw-rw-rw-   0        0        0      342 2023-07-17 13:42:06.000000 relevanceai-5.0.0/relevanceai/__init__.py
--rw-rw-rw-   0        0        0      117 2023-07-17 13:38:32.000000 relevanceai-5.0.0/relevanceai/_request.py
--rw-rw-rw-   0        0        0     2158 2023-07-17 13:38:32.000000 relevanceai-5.0.0/relevanceai/auth.py
--rw-rw-rw-   0        0        0     6646 2023-07-17 13:38:32.000000 relevanceai-5.0.0/relevanceai/chain.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:42:56.377330 relevanceai-5.0.0/relevanceai/connect/
--rw-rw-rw-   0        0        0       83 2023-07-17 13:40:43.000000 relevanceai-5.0.0/relevanceai/connect/__init__.py
--rw-rw-rw-   0        0        0     4324 2023-07-17 13:41:18.000000 relevanceai-5.0.0/relevanceai/connect/chains.py
--rw-rw-rw-   0        0        0     3811 2023-07-17 13:39:31.000000 relevanceai-5.0.0/relevanceai/connect/steps.py
--rw-rw-rw-   0        0        0     3401 2023-07-17 13:38:32.000000 relevanceai-5.0.0/relevanceai/datasets.py
--rw-rw-rw-   0        0        0     1046 2023-07-17 13:38:32.000000 relevanceai-5.0.0/relevanceai/env.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:42:56.385333 relevanceai-5.0.0/relevanceai/frontend/
--rw-rw-rw-   0        0        0      104 2023-07-17 13:40:02.000000 relevanceai-5.0.0/relevanceai/frontend/__init__.py
--rw-rw-rw-   0        0        0      686 2023-07-17 06:16:31.000000 relevanceai-5.0.0/relevanceai/frontend/input_components.py
--rw-rw-rw-   0        0        0     1908 2023-07-17 13:39:59.000000 relevanceai-5.0.0/relevanceai/frontend/upload_file.py
--rw-rw-rw-   0        0        0     4586 2023-07-17 13:38:32.000000 relevanceai-5.0.0/relevanceai/params.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:42:56.403913 relevanceai-5.0.0/relevanceai/steps/
--rw-rw-rw-   0        0        0      600 2023-07-17 13:38:32.000000 relevanceai-5.0.0/relevanceai/steps/__init__.py
--rw-rw-rw-   0        0        0     2671 2023-07-17 13:38:32.000000 relevanceai-5.0.0/relevanceai/steps/_base.py
--rw-rw-rw-   0        0        0     1994 2023-07-17 13:38:32.000000 relevanceai-5.0.0/relevanceai/steps/api_call.py
--rw-rw-rw-   0        0        0     1150 2023-07-17 13:38:32.000000 relevanceai-5.0.0/relevanceai/steps/execute_javascript.py
--rw-rw-rw-   0        0        0     1285 2023-07-17 13:38:32.000000 relevanceai-5.0.0/relevanceai/steps/generate_vector_embedding.py
--rw-rw-rw-   0        0        0     3751 2023-07-17 13:38:32.000000 relevanceai-5.0.0/relevanceai/steps/prompt_completion.py
--rw-rw-rw-   0        0        0     1721 2023-07-17 13:38:32.000000 relevanceai-5.0.0/relevanceai/steps/redis_vector_search.py
--rw-rw-rw-   0        0        0     1018 2023-07-17 13:38:32.000000 relevanceai-5.0.0/relevanceai/steps/run_chain.py
--rw-rw-rw-   0        0        0     2829 2023-07-17 13:38:32.000000 relevanceai-5.0.0/relevanceai/steps/run_step.py
--rw-rw-rw-   0        0        0     2120 2023-07-17 13:38:32.000000 relevanceai-5.0.0/relevanceai/steps/vector_search.py
--rw-rw-rw-   0        0        0     1728 2023-07-17 13:38:32.000000 relevanceai-5.0.0/relevanceai/steps/vectorize_and_search.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:42:56.375332 relevanceai-5.0.0/relevanceai.egg-info/
--rw-rw-rw-   0        0        0     1192 2023-07-17 13:42:56.000000 relevanceai-5.0.0/relevanceai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      947 2023-07-17 13:42:56.000000 relevanceai-5.0.0/relevanceai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 13:42:56.000000 relevanceai-5.0.0/relevanceai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 13:42:56.000000 relevanceai-5.0.0/relevanceai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-17 13:42:56.000000 relevanceai-5.0.0/relevanceai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 13:42:56.404912 relevanceai-5.0.0/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-07-17 13:38:32.000000 relevanceai-5.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:45:25.672081 relevanceai-5.0.1/
+-rw-rw-rw-   0        0        0    11547 2023-07-17 13:38:32.000000 relevanceai-5.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1192 2023-07-17 13:45:25.671080 relevanceai-5.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      970 2023-07-17 13:38:32.000000 relevanceai-5.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 13:45:25.641941 relevanceai-5.0.1/relevanceai/
+-rw-rw-rw-   0        0        0      343 2023-07-17 13:45:23.000000 relevanceai-5.0.1/relevanceai/__init__.py
+-rw-rw-rw-   0        0        0      117 2023-07-17 13:38:32.000000 relevanceai-5.0.1/relevanceai/_request.py
+-rw-rw-rw-   0        0        0     2158 2023-07-17 13:38:32.000000 relevanceai-5.0.1/relevanceai/auth.py
+-rw-rw-rw-   0        0        0     6646 2023-07-17 13:38:32.000000 relevanceai-5.0.1/relevanceai/chain.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:45:25.650941 relevanceai-5.0.1/relevanceai/connect/
+-rw-rw-rw-   0        0        0       83 2023-07-17 13:40:43.000000 relevanceai-5.0.1/relevanceai/connect/__init__.py
+-rw-rw-rw-   0        0        0     4325 2023-07-17 13:44:35.000000 relevanceai-5.0.1/relevanceai/connect/chains.py
+-rw-rw-rw-   0        0        0     3812 2023-07-17 13:44:40.000000 relevanceai-5.0.1/relevanceai/connect/steps.py
+-rw-rw-rw-   0        0        0     3401 2023-07-17 13:38:32.000000 relevanceai-5.0.1/relevanceai/datasets.py
+-rw-rw-rw-   0        0        0     1046 2023-07-17 13:38:32.000000 relevanceai-5.0.1/relevanceai/env.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:45:25.656523 relevanceai-5.0.1/relevanceai/frontend/
+-rw-rw-rw-   0        0        0      104 2023-07-17 13:40:02.000000 relevanceai-5.0.1/relevanceai/frontend/__init__.py
+-rw-rw-rw-   0        0        0      686 2023-07-17 06:16:31.000000 relevanceai-5.0.1/relevanceai/frontend/input_components.py
+-rw-rw-rw-   0        0        0     1908 2023-07-17 13:39:59.000000 relevanceai-5.0.1/relevanceai/frontend/upload_file.py
+-rw-rw-rw-   0        0        0     4586 2023-07-17 13:38:32.000000 relevanceai-5.0.1/relevanceai/params.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:45:25.671080 relevanceai-5.0.1/relevanceai/steps/
+-rw-rw-rw-   0        0        0      600 2023-07-17 13:38:32.000000 relevanceai-5.0.1/relevanceai/steps/__init__.py
+-rw-rw-rw-   0        0        0     2671 2023-07-17 13:38:32.000000 relevanceai-5.0.1/relevanceai/steps/_base.py
+-rw-rw-rw-   0        0        0     1994 2023-07-17 13:38:32.000000 relevanceai-5.0.1/relevanceai/steps/api_call.py
+-rw-rw-rw-   0        0        0     1150 2023-07-17 13:38:32.000000 relevanceai-5.0.1/relevanceai/steps/execute_javascript.py
+-rw-rw-rw-   0        0        0     1285 2023-07-17 13:38:32.000000 relevanceai-5.0.1/relevanceai/steps/generate_vector_embedding.py
+-rw-rw-rw-   0        0        0     3751 2023-07-17 13:38:32.000000 relevanceai-5.0.1/relevanceai/steps/prompt_completion.py
+-rw-rw-rw-   0        0        0     1721 2023-07-17 13:38:32.000000 relevanceai-5.0.1/relevanceai/steps/redis_vector_search.py
+-rw-rw-rw-   0        0        0     1018 2023-07-17 13:38:32.000000 relevanceai-5.0.1/relevanceai/steps/run_chain.py
+-rw-rw-rw-   0        0        0     2829 2023-07-17 13:38:32.000000 relevanceai-5.0.1/relevanceai/steps/run_step.py
+-rw-rw-rw-   0        0        0     2120 2023-07-17 13:38:32.000000 relevanceai-5.0.1/relevanceai/steps/vector_search.py
+-rw-rw-rw-   0        0        0     1728 2023-07-17 13:38:32.000000 relevanceai-5.0.1/relevanceai/steps/vectorize_and_search.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:45:25.648942 relevanceai-5.0.1/relevanceai.egg-info/
+-rw-rw-rw-   0        0        0     1192 2023-07-17 13:45:25.000000 relevanceai-5.0.1/relevanceai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      947 2023-07-17 13:45:25.000000 relevanceai-5.0.1/relevanceai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 13:45:25.000000 relevanceai-5.0.1/relevanceai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 13:45:25.000000 relevanceai-5.0.1/relevanceai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-17 13:45:25.000000 relevanceai-5.0.1/relevanceai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 13:45:25.672081 relevanceai-5.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-07-17 13:38:32.000000 relevanceai-5.0.1/setup.py
```

### Comparing `relevanceai-5.0.0/LICENSE` & `relevanceai-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/PKG-INFO` & `relevanceai-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relevanceai
-Version: 5.0.0
+Version: 5.0.1
 Home-page: https://relevanceai.com/
 Author: Relevance AI
 Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Relevance AI - The platform for building and deploying AI chains and Agents
```

### Comparing `relevanceai-5.0.0/README.md` & `relevanceai-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/auth.py` & `relevanceai-5.0.1/relevanceai/auth.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/chain.py` & `relevanceai-5.0.1/relevanceai/chain.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/connect/chains.py` & `relevanceai-5.0.1/relevanceai/connect/chains.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         headers=config.auth.headers,
         json={"ids": chain_id_list},
     )
     print("Successfully deleted chains from cloud: ", results.json())
     print("Trace-id ", results.headers.get("x-trace-id"))
 
 
-def create_chains(api_routes, url, id_suffix="", cleanup=True, export_json=False):
+def connect_chains(api_routes, url, id_suffix="", cleanup=True, export_json=False):
     chains, chain_id_list = routes_to_chains(api_routes, url, id_suffix=id_suffix)
     if export_json:
         import json
 
         with open("chain_export.json", "w") as outfile:
             json.dump({"export": chains}, outfile)
     else:
```

### Comparing `relevanceai-5.0.0/relevanceai/connect/steps.py` & `relevanceai-5.0.1/relevanceai/connect/steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         headers=config.auth.headers,
         json={"updates": tfs},
     )
     print("Uploaded transformations: ", results.json())
     print("Trace-id ", results.headers.get("x-trace-id"))
 
 
-def create_steps(
+def connect_steps(
     api_routes, url, id_suffix="", cleanup=True, export_json=False
 ):
     tfs_list, id_list = routes_to_steps(api_routes, url, id_suffix=id_suffix)
     if export_json:
         import json
 
         with open("transformation_export.json", "w") as outfile:
```

### Comparing `relevanceai-5.0.0/relevanceai/datasets.py` & `relevanceai-5.0.1/relevanceai/datasets.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/env.py` & `relevanceai-5.0.1/relevanceai/env.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/frontend/input_components.py` & `relevanceai-5.0.1/relevanceai/frontend/input_components.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/frontend/upload_file.py` & `relevanceai-5.0.1/relevanceai/frontend/upload_file.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/params.py` & `relevanceai-5.0.1/relevanceai/params.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/steps/__init__.py` & `relevanceai-5.0.1/relevanceai/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/steps/_base.py` & `relevanceai-5.0.1/relevanceai/steps/_base.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/steps/api_call.py` & `relevanceai-5.0.1/relevanceai/steps/api_call.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/steps/execute_javascript.py` & `relevanceai-5.0.1/relevanceai/steps/execute_javascript.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/steps/generate_vector_embedding.py` & `relevanceai-5.0.1/relevanceai/steps/generate_vector_embedding.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/steps/prompt_completion.py` & `relevanceai-5.0.1/relevanceai/steps/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/steps/redis_vector_search.py` & `relevanceai-5.0.1/relevanceai/steps/redis_vector_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/steps/run_chain.py` & `relevanceai-5.0.1/relevanceai/steps/run_chain.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/steps/run_step.py` & `relevanceai-5.0.1/relevanceai/steps/run_step.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/steps/vector_search.py` & `relevanceai-5.0.1/relevanceai/steps/vector_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai/steps/vectorize_and_search.py` & `relevanceai-5.0.1/relevanceai/steps/vectorize_and_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/relevanceai.egg-info/PKG-INFO` & `relevanceai-5.0.1/relevanceai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relevanceai
-Version: 5.0.0
+Version: 5.0.1
 Home-page: https://relevanceai.com/
 Author: Relevance AI
 Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Relevance AI - The platform for building and deploying AI chains and Agents
```

### Comparing `relevanceai-5.0.0/relevanceai.egg-info/SOURCES.txt` & `relevanceai-5.0.1/relevanceai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `relevanceai-5.0.0/setup.py` & `relevanceai-5.0.1/setup.py`

 * *Files identical despite different names*

