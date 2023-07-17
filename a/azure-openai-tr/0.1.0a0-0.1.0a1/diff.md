# Comparing `tmp/azure_openai_tr-0.1.0a0.tar.gz` & `tmp/azure_openai_tr-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_openai_tr-0.1.0a0.tar", max compression
+gzip compressed data, was "azure_openai_tr-0.1.0a1.tar", max compression
```

## Comparing `azure_openai_tr-0.1.0a0.tar` & `azure_openai_tr-0.1.0a1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      118 2023-07-17 10:31:54.492352 azure_openai_tr-0.1.0a0/azure_openai_tr/__init__.py
--rw-r--r--   0        0        0      971 2023-07-17 10:31:54.508010 azure_openai_tr-0.1.0a0/azure_openai_tr/__main__.py
--rw-r--r--   0        0        0     2184 2023-07-17 10:34:52.747734 azure_openai_tr-0.1.0a0/azure_openai_tr/azure_openai_tr.py
--rw-r--r--   0        0        0     1085 2023-07-17 10:31:54.320489 azure_openai_tr-0.1.0a0/LICENSE
--rw-r--r--   0        0        0     2077 2023-07-17 11:44:06.700284 azure_openai_tr-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0     1827 2023-07-17 12:00:34.433425 azure_openai_tr-0.1.0a0/README.md
--rw-r--r--   0        0        0     2511 1970-01-01 00:00:00.000000 azure_openai_tr-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0      118 2023-07-17 12:26:10.035377 azure_openai_tr-0.1.0a1/azure_openai_tr/__init__.py
+-rw-r--r--   0        0        0      971 2023-07-17 10:31:54.508010 azure_openai_tr-0.1.0a1/azure_openai_tr/__main__.py
+-rw-r--r--   0        0        0     2184 2023-07-17 10:34:52.747734 azure_openai_tr-0.1.0a1/azure_openai_tr/azure_openai_tr.py
+-rw-r--r--   0        0        0     1085 2023-07-17 10:31:54.320489 azure_openai_tr-0.1.0a1/LICENSE
+-rw-r--r--   0        0        0     2071 2023-07-17 12:26:02.782384 azure_openai_tr-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1827 2023-07-17 12:00:34.433425 azure_openai_tr-0.1.0a1/README.md
+-rw-r--r--   0        0        0     2511 1970-01-01 00:00:00.000000 azure_openai_tr-0.1.0a1/PKG-INFO
```

### Comparing `azure_openai_tr-0.1.0a0/azure_openai_tr/__main__.py` & `azure_openai_tr-0.1.0a1/azure_openai_tr/__main__.py`

 * *Files identical despite different names*

### Comparing `azure_openai_tr-0.1.0a0/azure_openai_tr/azure_openai_tr.py` & `azure_openai_tr-0.1.0a1/azure_openai_tr/azure_openai_tr.py`

 * *Files identical despite different names*

### Comparing `azure_openai_tr-0.1.0a0/LICENSE` & `azure_openai_tr-0.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `azure_openai_tr-0.1.0a0/pyproject.toml` & `azure_openai_tr-0.1.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "azure-openai-tr"
-version = "0.1.0-alpha.0"
+version = "0.1.0a1"
 description = "Translate via Azure Openai"
 authors = ["ffreemt"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ffreemt/azure-openai-tr"
 
 [tool.poetry.dependencies]
```

### Comparing `azure_openai_tr-0.1.0a0/README.md` & `azure_openai_tr-0.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `azure_openai_tr-0.1.0a0/PKG-INFO` & `azure_openai_tr-0.1.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-openai-tr
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Translate via Azure Openai
 Home-page: https://github.com/ffreemt/azure-openai-tr
 License: MIT
 Author: ffreemt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

