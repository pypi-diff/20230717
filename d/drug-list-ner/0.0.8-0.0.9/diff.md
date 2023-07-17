# Comparing `tmp/drug_list_ner-0.0.8.tar.gz` & `tmp/drug_list_ner-0.0.9.tar.gz`

## Comparing `drug_list_ner-0.0.8.tar` & `drug_list_ner-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/.DS_Store
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/Pipfile
--rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/Pipfile.lock
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/pyvenv.cfg
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/requirements.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/src/drug_list_ner/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/src/drug_list_ner/__init__.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/src/drug_list_ner/example.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/src/drug_list_ner/model2/.DS_Store
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/src/drug_list_ner/model2/config.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/src/drug_list_ner/tokenizer2/special_tokens_map.json
--rw-r--r--   0        0        0   716830 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/src/drug_list_ner/tokenizer2/tokenizer.json
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/src/drug_list_ner/tokenizer2/tokenizer_config.json
--rw-r--r--   0        0        0   227845 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/src/drug_list_ner/tokenizer2/vocab.txt
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/LICENSE
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/README.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 drug_list_ner-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/.DS_Store
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/Pipfile
+-rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/Pipfile.lock
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/pyvenv.cfg
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/requirements.txt
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/src/drug_list_ner/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/src/drug_list_ner/__init__.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/src/drug_list_ner/example.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/src/drug_list_ner/model2/.DS_Store
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/src/drug_list_ner/model2/config.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/src/drug_list_ner/tokenizer2/special_tokens_map.json
+-rw-r--r--   0        0        0   716830 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/src/drug_list_ner/tokenizer2/tokenizer.json
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/src/drug_list_ner/tokenizer2/tokenizer_config.json
+-rw-r--r--   0        0        0   227845 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/src/drug_list_ner/tokenizer2/vocab.txt
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/LICENSE
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/README.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 drug_list_ner-0.0.9/PKG-INFO
```

### Comparing `drug_list_ner-0.0.8/.DS_Store` & `drug_list_ner-0.0.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.8/Pipfile.lock` & `drug_list_ner-0.0.9/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.8/requirements.txt` & `drug_list_ner-0.0.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.8/src/.DS_Store` & `drug_list_ner-0.0.9/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.8/src/drug_list_ner/.DS_Store` & `drug_list_ner-0.0.9/src/drug_list_ner/.DS_Store`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.8/src/drug_list_ner/example.py` & `drug_list_ner-0.0.9/src/drug_list_ner/example.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from transformers import AutoTokenizer, AutoModelForTokenClassification, pipeline
 import os
 from huggingface_hub import hf_hub_download
 
-tokenizer = AutoTokenizer.from_pretrained("./tokenizer2", model_max_length=10000000)
+
+tokenizer = AutoTokenizer.from_pretrained("/tokenizer2", model_max_length=10000000)
 model_path = "./model2"
 pytorch_model_url = "https://huggingface.co/ronoys/testDeploy/blob/main/pytorch_model.bin"
 
 
 def drug_search(sentence):
     
     if not os.path.exists(os.path.join(model_path, "pytorch_model.bin")):
```

### Comparing `drug_list_ner-0.0.8/src/drug_list_ner/model2/.DS_Store` & `drug_list_ner-0.0.9/src/drug_list_ner/model2/.DS_Store`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.8/src/drug_list_ner/model2/config.json` & `drug_list_ner-0.0.9/src/drug_list_ner/model2/config.json`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.8/src/drug_list_ner/tokenizer2/tokenizer.json` & `drug_list_ner-0.0.9/src/drug_list_ner/tokenizer2/tokenizer.json`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.8/src/drug_list_ner/tokenizer2/vocab.txt` & `drug_list_ner-0.0.9/src/drug_list_ner/tokenizer2/vocab.txt`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.8/LICENSE` & `drug_list_ner-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.8/pyproject.toml` & `drug_list_ner-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "drug_list_ner"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Ronoy Sarkar", email="ronoysarkar.mail@gmail.com" },
 ]
 description = "An NER model to identify prescription drugs in a text sample"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `drug_list_ner-0.0.8/PKG-INFO` & `drug_list_ner-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drug_list_ner
-Version: 0.0.8
+Version: 0.0.9
 Summary: An NER model to identify prescription drugs in a text sample
 Author-email: Ronoy Sarkar <ronoysarkar.mail@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

