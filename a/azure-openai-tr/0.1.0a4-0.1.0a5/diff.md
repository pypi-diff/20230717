# Comparing `tmp/azure_openai_tr-0.1.0a4.tar.gz` & `tmp/azure_openai_tr-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_openai_tr-0.1.0a4.tar", max compression
+gzip compressed data, was "azure_openai_tr-0.1.0a5.tar", max compression
```

## Comparing `azure_openai_tr-0.1.0a4.tar` & `azure_openai_tr-0.1.0a5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      118 2023-07-17 12:49:27.042059 azure_openai_tr-0.1.0a4/azure_openai_tr/__init__.py
--rw-r--r--   0        0        0      971 2023-07-17 10:31:54.508010 azure_openai_tr-0.1.0a4/azure_openai_tr/__main__.py
--rw-r--r--   0        0        0     2184 2023-07-17 10:34:52.747734 azure_openai_tr-0.1.0a4/azure_openai_tr/azure_openai_tr.py
--rw-r--r--   0        0        0     1085 2023-07-17 10:31:54.320489 azure_openai_tr-0.1.0a4/LICENSE
--rw-r--r--   0        0        0     2071 2023-07-17 12:49:14.644925 azure_openai_tr-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0     2072 2023-07-17 12:48:03.849254 azure_openai_tr-0.1.0a4/README.md
--rw-r--r--   0        0        0     2745 1970-01-01 00:00:00.000000 azure_openai_tr-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0      118 2023-07-17 12:53:59.912767 azure_openai_tr-0.1.0a5/azure_openai_tr/__init__.py
+-rw-r--r--   0        0        0      971 2023-07-17 10:31:54.508010 azure_openai_tr-0.1.0a5/azure_openai_tr/__main__.py
+-rw-r--r--   0        0        0     2184 2023-07-17 10:34:52.747734 azure_openai_tr-0.1.0a5/azure_openai_tr/azure_openai_tr.py
+-rw-r--r--   0        0        0     1085 2023-07-17 10:31:54.320489 azure_openai_tr-0.1.0a5/LICENSE
+-rw-r--r--   0        0        0     2071 2023-07-17 12:53:51.389641 azure_openai_tr-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0     2072 2023-07-17 12:48:03.849254 azure_openai_tr-0.1.0a5/README.md
+-rw-r--r--   0        0        0     2745 1970-01-01 00:00:00.000000 azure_openai_tr-0.1.0a5/PKG-INFO
```

### Comparing `azure_openai_tr-0.1.0a4/azure_openai_tr/__main__.py` & `azure_openai_tr-0.1.0a5/azure_openai_tr/__main__.py`

 * *Files identical despite different names*

### Comparing `azure_openai_tr-0.1.0a4/azure_openai_tr/azure_openai_tr.py` & `azure_openai_tr-0.1.0a5/azure_openai_tr/azure_openai_tr.py`

 * *Files identical despite different names*

### Comparing `azure_openai_tr-0.1.0a4/LICENSE` & `azure_openai_tr-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `azure_openai_tr-0.1.0a4/pyproject.toml` & `azure_openai_tr-0.1.0a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "azure-openai-tr"
-version = "0.1.0a4"
+version = "0.1.0a5"
 description = "Translate via Azure Openai"
 authors = ["ffreemt"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ffreemt/azure-openai-tr"
 
 [tool.poetry.dependencies]
```

### Comparing `azure_openai_tr-0.1.0a4/README.md` & `azure_openai_tr-0.1.0a5/README.md`

 * *Files identical despite different names*

### Comparing `azure_openai_tr-0.1.0a4/PKG-INFO` & `azure_openai_tr-0.1.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-openai-tr
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Translate via Azure Openai
 Home-page: https://github.com/ffreemt/azure-openai-tr
 License: MIT
 Author: ffreemt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

