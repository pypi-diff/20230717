# Comparing `tmp/fastembed-0.0.1a1.tar.gz` & `tmp/fastembed-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastembed-0.0.1a1.tar", max compression
+gzip compressed data, was "fastembed-0.0.1a2.tar", max compression
```

## Comparing `fastembed-0.0.1a1.tar` & `fastembed-0.0.1a2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-07-14 05:55:44.593141 fastembed-0.0.1a1/LICENSE
--rw-r--r--   0        0        0     1380 2023-07-14 05:55:44.593290 fastembed-0.0.1a1/README.md
--rw-r--r--   0        0        0      882 2023-07-14 05:55:44.593496 fastembed-0.0.1a1/fastembed/embedding.py
--rw-r--r--   0        0        0      624 2023-07-14 05:55:44.593623 fastembed-0.0.1a1/fastembed/qdrant_client.py
--rw-r--r--   0        0        0     5787 2023-07-14 05:55:44.593784 fastembed-0.0.1a1/fastembed/qdrant_mixin.py
--rw-r--r--   0        0        0      965 2023-07-17 09:26:30.782978 fastembed-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     2287 1970-01-01 00:00:00.000000 fastembed-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-14 05:55:44.593141 fastembed-0.0.1a2/LICENSE
+-rw-r--r--   0        0        0     1376 2023-07-17 09:27:57.029707 fastembed-0.0.1a2/README.md
+-rw-r--r--   0        0        0      882 2023-07-14 05:55:44.593496 fastembed-0.0.1a2/fastembed/embedding.py
+-rw-r--r--   0        0        0      623 2023-07-17 09:28:52.510023 fastembed-0.0.1a2/fastembed/qdrant_client.py
+-rw-r--r--   0        0        0     5787 2023-07-14 05:55:44.593784 fastembed-0.0.1a2/fastembed/qdrant_mixin.py
+-rw-r--r--   0        0        0      965 2023-07-17 09:30:25.246186 fastembed-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0     2283 1970-01-01 00:00:00.000000 fastembed-0.0.1a2/PKG-INFO
```

### Comparing `fastembed-0.0.1a1/LICENSE` & `fastembed-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastembed-0.0.1a1/README.md` & `fastembed-0.0.1a2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# FastVector Library
+# FastEmbed Library
 
-FastVector is a Python library that provides convenient methods for indexing and searching text documents using Qdrant, a high-dimensional vector indexing and search system.
+FastEmbed is a Python library that provides convenient methods for indexing and searching text documents using Qdrant, a high-dimensional vector indexing and search system.
 
 ## Features
 
 - Batch document insertion with automatic embedding using SentenceTransformers. With support for OpenAI and custom embeddings.
 - Efficient batch searching with support for filtering by metadata.
 - Automatic generation of unique IDs for documents.
 - Convenient alias methods for adding documents and performing queries.
 
 ## Installation
 
-To install the FastVector library, we install Qdrant client as well with pip:
+To install the FastEmbed library, we install Qdrant client as well with pip:
 
 ```bash
-pip install fastvector qdrant-client
+pip install fastembed qdrant-client
 ```
 
 ## Usage
 
 Here's a simple usage example, which works as is:
 
 ```python
```

### Comparing `fastembed-0.0.1a1/fastembed/embedding.py` & `fastembed-0.0.1a2/fastembed/embedding.py`

 * *Files identical despite different names*

### Comparing `fastembed-0.0.1a1/fastembed/qdrant_client.py` & `fastembed-0.0.1a2/fastembed/qdrant_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     # Existing QdrantClient implementation...
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # Check if fastvector is installed
         try:
-            from fastvector.qdrant_mixin import QdrantClientMixin
+            from fastembed.qdrant_mixin import QdrantClientMixin
 
             # If it is, add the mixin methods to this instance
             for name, method in QdrantClientMixin.__dict__.items():
                 if callable(method):
                     setattr(self, name, method.__get__(self, self.__class__))
         except ImportError:
             # If it's not, do nothing
```

### Comparing `fastembed-0.0.1a1/fastembed/qdrant_mixin.py` & `fastembed-0.0.1a2/fastembed/qdrant_mixin.py`

 * *Files identical despite different names*

### Comparing `fastembed-0.0.1a1/pyproject.toml` & `fastembed-0.0.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastembed"
-version = "0.0.1.alpha1"
+version = "0.0.1.alpha2"
 description = "Fast embedding alternative to Sentence transformers"
 authors = ["NirantK <nirant.bits@gmail.com>"]
 license = "Apache License"
 readme = "README.md"
 packages = [{include = "fastembed"}]
 homepage = "https://github.com/qdrant/qdrant-client"
 repository = "https://github.com/qdrant/qdrant-client"
```

### Comparing `fastembed-0.0.1a1/PKG-INFO` & `fastembed-0.0.1a2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastembed
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: Fast embedding alternative to Sentence transformers
 Home-page: https://github.com/qdrant/qdrant-client
 License: Apache License
 Keywords: vector,embedding,neural,search,qdrant
 Author: NirantK
 Author-email: nirant.bits@gmail.com
 Requires-Python: >=3.8.0,<3.12
@@ -16,31 +16,31 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: onnxruntime (>=1.15.1,<2.0.0)
 Requires-Dist: onnxruntime-silicon (>=1.15.0,<2.0.0) ; sys_platform == "darwin"
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Project-URL: Repository, https://github.com/qdrant/qdrant-client
 Description-Content-Type: text/markdown
 
-# FastVector Library
+# FastEmbed Library
 
-FastVector is a Python library that provides convenient methods for indexing and searching text documents using Qdrant, a high-dimensional vector indexing and search system.
+FastEmbed is a Python library that provides convenient methods for indexing and searching text documents using Qdrant, a high-dimensional vector indexing and search system.
 
 ## Features
 
 - Batch document insertion with automatic embedding using SentenceTransformers. With support for OpenAI and custom embeddings.
 - Efficient batch searching with support for filtering by metadata.
 - Automatic generation of unique IDs for documents.
 - Convenient alias methods for adding documents and performing queries.
 
 ## Installation
 
-To install the FastVector library, we install Qdrant client as well with pip:
+To install the FastEmbed library, we install Qdrant client as well with pip:
 
 ```bash
-pip install fastvector qdrant-client
+pip install fastembed qdrant-client
 ```
 
 ## Usage
 
 Here's a simple usage example, which works as is:
 
 ```python
```

