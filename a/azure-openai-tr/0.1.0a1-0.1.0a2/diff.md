# Comparing `tmp/azure_openai_tr-0.1.0a1.tar.gz` & `tmp/azure_openai_tr-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_openai_tr-0.1.0a1.tar", max compression
+gzip compressed data, was "azure_openai_tr-0.1.0a2.tar", max compression
```

## Comparing `azure_openai_tr-0.1.0a1.tar` & `azure_openai_tr-0.1.0a2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      118 2023-07-17 12:26:10.035377 azure_openai_tr-0.1.0a1/azure_openai_tr/__init__.py
--rw-r--r--   0        0        0      971 2023-07-17 10:31:54.508010 azure_openai_tr-0.1.0a1/azure_openai_tr/__main__.py
--rw-r--r--   0        0        0     2184 2023-07-17 10:34:52.747734 azure_openai_tr-0.1.0a1/azure_openai_tr/azure_openai_tr.py
--rw-r--r--   0        0        0     1085 2023-07-17 10:31:54.320489 azure_openai_tr-0.1.0a1/LICENSE
--rw-r--r--   0        0        0     2071 2023-07-17 12:26:02.782384 azure_openai_tr-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     1827 2023-07-17 12:00:34.433425 azure_openai_tr-0.1.0a1/README.md
--rw-r--r--   0        0        0     2511 1970-01-01 00:00:00.000000 azure_openai_tr-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0      118 2023-07-17 12:41:17.743416 azure_openai_tr-0.1.0a2/azure_openai_tr/__init__.py
+-rw-r--r--   0        0        0      971 2023-07-17 10:31:54.508010 azure_openai_tr-0.1.0a2/azure_openai_tr/__main__.py
+-rw-r--r--   0        0        0     2184 2023-07-17 10:34:52.747734 azure_openai_tr-0.1.0a2/azure_openai_tr/azure_openai_tr.py
+-rw-r--r--   0        0        0     1085 2023-07-17 10:31:54.320489 azure_openai_tr-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0     2071 2023-07-17 12:41:11.570247 azure_openai_tr-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1832 2023-07-17 12:39:40.217115 azure_openai_tr-0.1.0a2/README.md
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 azure_openai_tr-0.1.0a2/PKG-INFO
```

### Comparing `azure_openai_tr-0.1.0a1/azure_openai_tr/__main__.py` & `azure_openai_tr-0.1.0a2/azure_openai_tr/__main__.py`

 * *Files identical despite different names*

### Comparing `azure_openai_tr-0.1.0a1/azure_openai_tr/azure_openai_tr.py` & `azure_openai_tr-0.1.0a2/azure_openai_tr/azure_openai_tr.py`

 * *Files identical despite different names*

### Comparing `azure_openai_tr-0.1.0a1/LICENSE` & `azure_openai_tr-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `azure_openai_tr-0.1.0a1/pyproject.toml` & `azure_openai_tr-0.1.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "azure-openai-tr"
-version = "0.1.0a1"
+version = "0.1.0a2"
 description = "Translate via Azure Openai"
 authors = ["ffreemt"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ffreemt/azure-openai-tr"
 
 [tool.poetry.dependencies]
```

### Comparing `azure_openai_tr-0.1.0a1/README.md` & `azure_openai_tr-0.1.0a2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # azure-openai-tr
-[![pytest](https://github.com/ffreemt/azure-openai-tr/actions/workflows/routine-tests.yml/badge.svg)](https://github.com/ffreemt/azure-openai-tr/actions)[![python](https://img.shields.io/static/v1?label=python+&message=3.8%2B&color=blue)](https://www.python.org/downloads/)[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)[![PyPI version](https://badge.fury.io/py/azure_openai_tr.svg)](https://badge.fury.io/py/azure_openai_tr)
+[![pytest](https://github.com/ffreemt/azure-openai-tr/actions/workflows/routine-tests.yml/badge.svg)](https://github.com/ffreemt/azure-openai-tr/actions)[![python](https://img.shields.io/static/v1?label=python+&message=3.10%2B&color=blue)](https://www.python.org/downloads/)[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)[![PyPI version](https://badge.fury.io/py/azure_openai_tr.svg)](https://badge.fury.io/py/azure_openai_tr)
 
 Translate via Azure Openai
 
 ## Install it
 
 ```shell
 pip install azure-openai-tr
@@ -19,18 +19,18 @@
 print(azure_openai_tr("test this and that")
 # '测试这个和那个。'
 
 print(azure_openai_tr("Hey ya", temperature=.2))
 # 嘿，你好
 
 print(azure_openai_tr("Hey ya", temperature=.8))
-嗨啊
+# 嗨啊
 
 print(azure_openai_tr("Hey ya", temperature=.8))
-嘿 ya
+# 嘿 ya
 
 print(azure_openai_tr("test this and that", to_lang='German', temperature=.8))
 # Teste dies und jenes.
 
 print(azure_openai_tr("test this and that", to_lang='German', temperature=.8))
 # Teste dies und das.
```

### Comparing `azure_openai_tr-0.1.0a1/PKG-INFO` & `azure_openai_tr-0.1.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-openai-tr
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Translate via Azure Openai
 Home-page: https://github.com/ffreemt/azure-openai-tr
 License: MIT
 Author: ffreemt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: set-loglevel (>=0.1.2,<0.2.0)
 Requires-Dist: typer (>=0.4.1,<0.5.0)
 Project-URL: Repository, https://github.com/ffreemt/azure-openai-tr
 Description-Content-Type: text/markdown
 
 # azure-openai-tr
-[![pytest](https://github.com/ffreemt/azure-openai-tr/actions/workflows/routine-tests.yml/badge.svg)](https://github.com/ffreemt/azure-openai-tr/actions)[![python](https://img.shields.io/static/v1?label=python+&message=3.8%2B&color=blue)](https://www.python.org/downloads/)[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)[![PyPI version](https://badge.fury.io/py/azure_openai_tr.svg)](https://badge.fury.io/py/azure_openai_tr)
+[![pytest](https://github.com/ffreemt/azure-openai-tr/actions/workflows/routine-tests.yml/badge.svg)](https://github.com/ffreemt/azure-openai-tr/actions)[![python](https://img.shields.io/static/v1?label=python+&message=3.10%2B&color=blue)](https://www.python.org/downloads/)[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)[![PyPI version](https://badge.fury.io/py/azure_openai_tr.svg)](https://badge.fury.io/py/azure_openai_tr)
 
 Translate via Azure Openai
 
 ## Install it
 
 ```shell
 pip install azure-openai-tr
@@ -39,18 +39,18 @@
 print(azure_openai_tr("test this and that")
 # '测试这个和那个。'
 
 print(azure_openai_tr("Hey ya", temperature=.2))
 # 嘿，你好
 
 print(azure_openai_tr("Hey ya", temperature=.8))
-嗨啊
+# 嗨啊
 
 print(azure_openai_tr("Hey ya", temperature=.8))
-嘿 ya
+# 嘿 ya
 
 print(azure_openai_tr("test this and that", to_lang='German', temperature=.8))
 # Teste dies und jenes.
 
 print(azure_openai_tr("test this and that", to_lang='German', temperature=.8))
 # Teste dies und das.
```

