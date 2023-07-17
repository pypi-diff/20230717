# Comparing `tmp/embedchain-0.0.8.tar.gz` & `tmp/embedchain-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedchain-0.0.8.tar", last modified: Fri Jun 23 17:19:43 2023, max compression
+gzip compressed data, was "embedchain-0.0.9.tar", last modified: Sat Jun 24 04:18:51 2023, max compression
```

## Comparing `embedchain-0.0.8.tar` & `embedchain-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 17:19:43.096723 embedchain-0.0.8/
--rw-r--r--   0 tj         (501) staff       (20)    11349 2023-06-20 11:57:43.000000 embedchain-0.0.8/LICENSE
--rw-r--r--   0 tj         (501) staff       (20)     7108 2023-06-23 17:19:43.096584 embedchain-0.0.8/PKG-INFO
--rw-r--r--   0 tj         (501) staff       (20)     6613 2023-06-23 17:14:59.000000 embedchain-0.0.8/README.md
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 17:19:43.093089 embedchain-0.0.8/embedchain/
--rw-r--r--   0 tj         (501) staff       (20)       27 2023-06-20 11:09:25.000000 embedchain-0.0.8/embedchain/__init__.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 17:19:43.095205 embedchain-0.0.8/embedchain/chunkers/
--rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.8/embedchain/chunkers/__init__.py
--rw-r--r--   0 tj         (501) staff       (20)      819 2023-06-23 11:36:20.000000 embedchain-0.0.8/embedchain/chunkers/base_chunker.py
--rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:09:25.000000 embedchain-0.0.8/embedchain/chunkers/pdf_file.py
--rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-23 17:14:59.000000 embedchain-0.0.8/embedchain/chunkers/qna_pair.py
--rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:23:20.000000 embedchain-0.0.8/embedchain/chunkers/web_page.py
--rw-r--r--   0 tj         (501) staff       (20)      426 2023-06-20 11:09:25.000000 embedchain-0.0.8/embedchain/chunkers/youtube_video.py
--rw-r--r--   0 tj         (501) staff       (20)     8154 2023-06-23 17:15:05.000000 embedchain-0.0.8/embedchain/embedchain.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 17:19:43.096355 embedchain-0.0.8/embedchain/loaders/
--rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.8/embedchain/loaders/__init__.py
--rw-r--r--   0 tj         (501) staff       (20)      301 2023-06-23 17:14:59.000000 embedchain-0.0.8/embedchain/loaders/local_qna_pair.py
--rw-r--r--   0 tj         (501) staff       (20)      639 2023-06-23 11:25:48.000000 embedchain-0.0.8/embedchain/loaders/pdf_file.py
--rw-r--r--   0 tj         (501) staff       (20)      731 2023-06-23 11:25:48.000000 embedchain-0.0.8/embedchain/loaders/web_page.py
--rw-r--r--   0 tj         (501) staff       (20)      618 2023-06-23 11:25:48.000000 embedchain-0.0.8/embedchain/loaders/youtube_video.py
--rw-r--r--   0 tj         (501) staff       (20)     1162 2023-06-23 17:15:05.000000 embedchain-0.0.8/embedchain/utils.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 17:19:43.093796 embedchain-0.0.8/embedchain.egg-info/
--rw-r--r--   0 tj         (501) staff       (20)     7108 2023-06-23 17:19:43.000000 embedchain-0.0.8/embedchain.egg-info/PKG-INFO
--rw-r--r--   0 tj         (501) staff       (20)      630 2023-06-23 17:19:43.000000 embedchain-0.0.8/embedchain.egg-info/SOURCES.txt
--rw-r--r--   0 tj         (501) staff       (20)        1 2023-06-23 17:19:43.000000 embedchain-0.0.8/embedchain.egg-info/dependency_links.txt
--rw-r--r--   0 tj         (501) staff       (20)      103 2023-06-23 17:19:43.000000 embedchain-0.0.8/embedchain.egg-info/requires.txt
--rw-r--r--   0 tj         (501) staff       (20)       11 2023-06-23 17:19:43.000000 embedchain-0.0.8/embedchain.egg-info/top_level.txt
--rw-r--r--   0 tj         (501) staff       (20)       38 2023-06-23 17:19:43.096756 embedchain-0.0.8/setup.cfg
--rw-r--r--   0 tj         (501) staff       (20)      979 2023-06-23 17:18:27.000000 embedchain-0.0.8/setup.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-24 04:18:51.509168 embedchain-0.0.9/
+-rw-r--r--   0 tj         (501) staff       (20)    11349 2023-06-20 11:57:43.000000 embedchain-0.0.9/LICENSE
+-rw-r--r--   0 tj         (501) staff       (20)     7108 2023-06-24 04:18:51.509036 embedchain-0.0.9/PKG-INFO
+-rw-r--r--   0 tj         (501) staff       (20)     6613 2023-06-23 17:14:59.000000 embedchain-0.0.9/README.md
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-24 04:18:51.505315 embedchain-0.0.9/embedchain/
+-rw-r--r--   0 tj         (501) staff       (20)       27 2023-06-20 11:09:25.000000 embedchain-0.0.9/embedchain/__init__.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-24 04:18:51.507212 embedchain-0.0.9/embedchain/chunkers/
+-rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.9/embedchain/chunkers/__init__.py
+-rw-r--r--   0 tj         (501) staff       (20)      819 2023-06-23 11:36:20.000000 embedchain-0.0.9/embedchain/chunkers/base_chunker.py
+-rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:09:25.000000 embedchain-0.0.9/embedchain/chunkers/pdf_file.py
+-rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-23 17:14:59.000000 embedchain-0.0.9/embedchain/chunkers/qna_pair.py
+-rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:23:20.000000 embedchain-0.0.9/embedchain/chunkers/web_page.py
+-rw-r--r--   0 tj         (501) staff       (20)      426 2023-06-20 11:09:25.000000 embedchain-0.0.9/embedchain/chunkers/youtube_video.py
+-rw-r--r--   0 tj         (501) staff       (20)     8154 2023-06-23 17:15:05.000000 embedchain-0.0.9/embedchain/embedchain.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-24 04:18:51.508279 embedchain-0.0.9/embedchain/loaders/
+-rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.9/embedchain/loaders/__init__.py
+-rw-r--r--   0 tj         (501) staff       (20)      301 2023-06-23 17:14:59.000000 embedchain-0.0.9/embedchain/loaders/local_qna_pair.py
+-rw-r--r--   0 tj         (501) staff       (20)      639 2023-06-23 11:25:48.000000 embedchain-0.0.9/embedchain/loaders/pdf_file.py
+-rw-r--r--   0 tj         (501) staff       (20)      731 2023-06-23 11:25:48.000000 embedchain-0.0.9/embedchain/loaders/web_page.py
+-rw-r--r--   0 tj         (501) staff       (20)      618 2023-06-23 11:25:48.000000 embedchain-0.0.9/embedchain/loaders/youtube_video.py
+-rw-r--r--   0 tj         (501) staff       (20)     1162 2023-06-23 17:15:05.000000 embedchain-0.0.9/embedchain/utils.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-24 04:18:51.508793 embedchain-0.0.9/embedchain/vectordb/
+-rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-24 04:16:39.000000 embedchain-0.0.9/embedchain/vectordb/__init__.py
+-rw-r--r--   0 tj         (501) staff       (20)      293 2023-06-23 06:44:10.000000 embedchain-0.0.9/embedchain/vectordb/base_vector_db.py
+-rw-r--r--   0 tj         (501) staff       (20)      866 2023-06-23 06:44:10.000000 embedchain-0.0.9/embedchain/vectordb/chroma_db.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-24 04:18:51.506040 embedchain-0.0.9/embedchain.egg-info/
+-rw-r--r--   0 tj         (501) staff       (20)     7108 2023-06-24 04:18:51.000000 embedchain-0.0.9/embedchain.egg-info/PKG-INFO
+-rw-r--r--   0 tj         (501) staff       (20)      733 2023-06-24 04:18:51.000000 embedchain-0.0.9/embedchain.egg-info/SOURCES.txt
+-rw-r--r--   0 tj         (501) staff       (20)        1 2023-06-24 04:18:51.000000 embedchain-0.0.9/embedchain.egg-info/dependency_links.txt
+-rw-r--r--   0 tj         (501) staff       (20)      103 2023-06-24 04:18:51.000000 embedchain-0.0.9/embedchain.egg-info/requires.txt
+-rw-r--r--   0 tj         (501) staff       (20)       11 2023-06-24 04:18:51.000000 embedchain-0.0.9/embedchain.egg-info/top_level.txt
+-rw-r--r--   0 tj         (501) staff       (20)       38 2023-06-24 04:18:51.509201 embedchain-0.0.9/setup.cfg
+-rw-r--r--   0 tj         (501) staff       (20)      979 2023-06-24 04:18:30.000000 embedchain-0.0.9/setup.py
```

### Comparing `embedchain-0.0.8/LICENSE` & `embedchain-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.8/PKG-INFO` & `embedchain-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedchain
-Version: 0.0.8
+Version: 0.0.9
 Summary: embedchain is a framework to easily create LLM powered bots over any dataset
 Home-page: https://github.com/embedchain/embedchain
 Author: Taranjeet Singh
 Author-email: reachtotj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `embedchain-0.0.8/README.md` & `embedchain-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.8/embedchain/chunkers/base_chunker.py` & `embedchain-0.0.9/embedchain/chunkers/base_chunker.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.8/embedchain/embedchain.py` & `embedchain-0.0.9/embedchain/embedchain.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.8/embedchain/loaders/pdf_file.py` & `embedchain-0.0.9/embedchain/loaders/pdf_file.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.8/embedchain/loaders/web_page.py` & `embedchain-0.0.9/embedchain/loaders/web_page.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.8/embedchain/loaders/youtube_video.py` & `embedchain-0.0.9/embedchain/loaders/youtube_video.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.8/embedchain/utils.py` & `embedchain-0.0.9/embedchain/utils.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.8/embedchain.egg-info/PKG-INFO` & `embedchain-0.0.9/embedchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedchain
-Version: 0.0.8
+Version: 0.0.9
 Summary: embedchain is a framework to easily create LLM powered bots over any dataset
 Home-page: https://github.com/embedchain/embedchain
 Author: Taranjeet Singh
 Author-email: reachtotj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `embedchain-0.0.8/embedchain.egg-info/SOURCES.txt` & `embedchain-0.0.9/embedchain.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,8 +15,11 @@
 embedchain/chunkers/qna_pair.py
 embedchain/chunkers/web_page.py
 embedchain/chunkers/youtube_video.py
 embedchain/loaders/__init__.py
 embedchain/loaders/local_qna_pair.py
 embedchain/loaders/pdf_file.py
 embedchain/loaders/web_page.py
-embedchain/loaders/youtube_video.py
+embedchain/loaders/youtube_video.py
+embedchain/vectordb/__init__.py
+embedchain/vectordb/base_vector_db.py
+embedchain/vectordb/chroma_db.py
```

### Comparing `embedchain-0.0.8/setup.py` & `embedchain-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="embedchain",
-    version="0.0.8",
+    version="0.0.9",
     author="Taranjeet Singh",
     author_email="reachtotj@gmail.com",
     description="embedchain is a framework to easily create LLM powered bots over any dataset",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/embedchain/embedchain",
     packages=setuptools.find_packages(),
```

