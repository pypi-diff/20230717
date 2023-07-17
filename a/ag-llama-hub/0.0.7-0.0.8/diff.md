# Comparing `tmp/ag_llama_hub-0.0.7.tar.gz` & `tmp/ag_llama_hub-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama_hub-0.0.7.tar", last modified: Mon Jul 17 11:48:35 2023, max compression
+gzip compressed data, was "dist\ag_llama_hub-0.0.8.tar", last modified: Mon Jul 17 13:33:58 2023, max compression
```

## Comparing `ag_llama_hub-0.0.7.tar` & `ag_llama_hub-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 11:48:35.291793 ag_llama_hub-0.0.7/
--rw-rw-rw-   0        0        0      832 2023-07-17 11:48:35.290795 ag_llama_hub-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-17 11:48:35.274763 ag_llama_hub-0.0.7/ag_llama_hub/
--rw-rw-rw-   0        0        0     2105 2023-07-12 14:53:21.000000 ag_llama_hub-0.0.7/ag_llama_hub/__init__.py
--rw-rw-rw-   0        0        0     4794 2023-07-17 11:48:25.000000 ag_llama_hub-0.0.7/ag_llama_hub/__main__.py
--rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.7/ag_llama_hub/choice.py
--rw-rw-rw-   0        0        0    16256 2023-07-04 11:44:01.000000 ag_llama_hub-0.0.7/ag_llama_hub/model.py
--rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.7/ag_llama_hub/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-17 11:48:35.285809 ag_llama_hub-0.0.7/ag_llama_hub.egg-info/
--rw-rw-rw-   0        0        0      832 2023-07-17 11:48:35.000000 ag_llama_hub-0.0.7/ag_llama_hub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-07-17 11:48:35.000000 ag_llama_hub-0.0.7/ag_llama_hub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 11:48:35.000000 ag_llama_hub-0.0.7/ag_llama_hub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-07-17 11:48:35.000000 ag_llama_hub-0.0.7/ag_llama_hub.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-17 11:48:35.000000 ag_llama_hub-0.0.7/ag_llama_hub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 11:48:35.291793 ag_llama_hub-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2567 2023-07-12 13:13:29.000000 ag_llama_hub-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 11:48:35.288801 ag_llama_hub-0.0.7/utils/
--rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.7/utils/download.py
--rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.7/utils/render.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:33:58.163577 ag_llama_hub-0.0.8/
+-rw-rw-rw-   0        0        0      832 2023-07-17 13:33:58.162581 ag_llama_hub-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-17 13:33:58.149615 ag_llama_hub-0.0.8/ag_llama_hub/
+-rw-rw-rw-   0        0        0     2105 2023-07-12 14:53:21.000000 ag_llama_hub-0.0.8/ag_llama_hub/__init__.py
+-rw-rw-rw-   0        0        0     4794 2023-07-17 11:48:25.000000 ag_llama_hub-0.0.8/ag_llama_hub/__main__.py
+-rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.8/ag_llama_hub/choice.py
+-rw-rw-rw-   0        0        0    16470 2023-07-17 13:33:49.000000 ag_llama_hub-0.0.8/ag_llama_hub/model.py
+-rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.8/ag_llama_hub/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:33:58.158592 ag_llama_hub-0.0.8/ag_llama_hub.egg-info/
+-rw-rw-rw-   0        0        0      832 2023-07-17 13:33:58.000000 ag_llama_hub-0.0.8/ag_llama_hub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-07-17 13:33:58.000000 ag_llama_hub-0.0.8/ag_llama_hub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 13:33:58.000000 ag_llama_hub-0.0.8/ag_llama_hub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-07-17 13:33:58.000000 ag_llama_hub-0.0.8/ag_llama_hub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-17 13:33:58.000000 ag_llama_hub-0.0.8/ag_llama_hub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 13:33:58.164576 ag_llama_hub-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2567 2023-07-12 13:13:29.000000 ag_llama_hub-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:33:58.161584 ag_llama_hub-0.0.8/utils/
+-rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.8/utils/download.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.8/utils/render.py
```

### Comparing `ag_llama_hub-0.0.7/PKG-INFO` & `ag_llama_hub-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag_llama_hub
-Version: 0.0.7
+Version: 0.0.8
 Summary: ag_llama_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama_hub-0.0.7/ag_llama_hub/__init__.py` & `ag_llama_hub-0.0.8/ag_llama_hub/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.7/ag_llama_hub/__main__.py` & `ag_llama_hub-0.0.8/ag_llama_hub/__main__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.7/ag_llama_hub/choice.py` & `ag_llama_hub-0.0.8/ag_llama_hub/choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.7/ag_llama_hub/model.py` & `ag_llama_hub-0.0.8/ag_llama_hub/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,20 +173,23 @@
             processor.append(TopPLogitsWarper(config.top_p))
 
         return processor
 
     def tokenize(self, text,trim_to=2048):
         """Tokenize a string into a tensor of token IDs."""
         num_tokens = self.get_tokens_count(text)            
+        if num_tokens>trim_to:
+            raise ValueError(f"Tokenized original text:{num_tokens} tokens, trimed:{trim_to} tokens. Some tokens are lost, please try to reduce the length of the input text.")
         self.wait_and_clear_gpu()
         with torch.inference_mode():
             batch = self.tokenizer.encode(text,truncation=True,max_length=trim_to,return_tensors="pt")
             logger.debug(f"Sending tokenized text to device {self.device}")
             res=batch[0].to(self.device)
         logger.debug(f"Tokenized original text:{num_tokens} tokens, trimed:{batch.shape[-1]} tokens")
+        
         return res
 
     def generate(self, input_ids, logprobs=0, **kwargs):
         """Generate a stream of predicted tokens using the language model."""
 
         # Store the original batch size and input length.
         batch_size = input_ids.shape[0]
@@ -423,9 +426,9 @@
     return StreamModel(model, tokenizer,path=name_or_path)
 
 def gpu_sum(info):
     bytes_gib = 1024.0 ** 3
     s=""        
     s+='used:'+f"{int(info.used / bytes_gib)} GiB | "
     s+='free:'+ f"{int(info.free / bytes_gib)} GiB | "
-    s+='total:'+f"{int(info.total / bytes_gib)} GiB |"
+    s+='total:'+f"{int(info.total / bytes_gib)} GiB"
     return s
```

### Comparing `ag_llama_hub-0.0.7/ag_llama_hub/tokenizer.py` & `ag_llama_hub-0.0.8/ag_llama_hub/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.7/ag_llama_hub.egg-info/PKG-INFO` & `ag_llama_hub-0.0.8/ag_llama_hub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag-llama-hub
-Version: 0.0.7
+Version: 0.0.8
 Summary: ag_llama_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama_hub-0.0.7/setup.py` & `ag_llama_hub-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.7/utils/download.py` & `ag_llama_hub-0.0.8/utils/download.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.7/utils/render.py` & `ag_llama_hub-0.0.8/utils/render.py`

 * *Files identical despite different names*

