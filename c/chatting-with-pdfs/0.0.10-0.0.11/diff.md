# Comparing `tmp/chatting_with_pdfs-0.0.10.tar.gz` & `tmp/chatting_with_pdfs-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatting_with_pdfs-0.0.10.tar", last modified: Fri Jul 14 07:26:06 2023, max compression
+gzip compressed data, was "chatting_with_pdfs-0.0.11.tar", last modified: Mon Jul 17 08:18:18 2023, max compression
```

## Comparing `chatting_with_pdfs-0.0.10.tar` & `chatting_with_pdfs-0.0.11.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 07:26:06.090435 chatting_with_pdfs-0.0.10/
--rw-rw-rw-   0        0        0     1086 2023-07-13 15:51:36.000000 chatting_with_pdfs-0.0.10/LICENSE
--rw-rw-rw-   0        0        0     3135 2023-07-14 07:26:06.088592 chatting_with_pdfs-0.0.10/PKG-INFO
--rw-rw-rw-   0        0        0     2705 2023-07-13 16:12:42.000000 chatting_with_pdfs-0.0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 07:26:06.033596 chatting_with_pdfs-0.0.10/app/
-drwxrwxrwx   0        0        0        0 2023-07-14 07:26:06.083361 chatting_with_pdfs-0.0.10/app/chatting_with_pdfs.egg-info/
--rw-rw-rw-   0        0        0     3135 2023-07-14 07:26:05.000000 chatting_with_pdfs-0.0.10/app/chatting_with_pdfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-07-14 07:26:05.000000 chatting_with_pdfs-0.0.10/app/chatting_with_pdfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 07:26:05.000000 chatting_with_pdfs-0.0.10/app/chatting_with_pdfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-14 07:26:05.000000 chatting_with_pdfs-0.0.10/app/chatting_with_pdfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 07:26:05.000000 chatting_with_pdfs-0.0.10/app/chatting_with_pdfs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 07:26:06.091482 chatting_with_pdfs-0.0.10/setup.cfg
--rw-rw-rw-   0        0        0      816 2023-07-14 07:23:09.000000 chatting_with_pdfs-0.0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 08:18:18.741321 chatting_with_pdfs-0.0.11/
+-rw-rw-rw-   0        0        0     1086 2023-07-13 15:51:36.000000 chatting_with_pdfs-0.0.11/LICENSE
+-rw-rw-rw-   0        0        0     3135 2023-07-17 08:18:18.741321 chatting_with_pdfs-0.0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2705 2023-07-13 16:12:42.000000 chatting_with_pdfs-0.0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 08:18:18.728170 chatting_with_pdfs-0.0.11/app/
+drwxrwxrwx   0        0        0        0 2023-07-17 08:18:18.739543 chatting_with_pdfs-0.0.11/app/chatting_with_pdfs.egg-info/
+-rw-rw-rw-   0        0        0     3135 2023-07-17 08:18:18.000000 chatting_with_pdfs-0.0.11/app/chatting_with_pdfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-07-17 08:18:18.000000 chatting_with_pdfs-0.0.11/app/chatting_with_pdfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 08:18:18.000000 chatting_with_pdfs-0.0.11/app/chatting_with_pdfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-17 08:18:18.000000 chatting_with_pdfs-0.0.11/app/chatting_with_pdfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 08:18:18.000000 chatting_with_pdfs-0.0.11/app/chatting_with_pdfs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 08:18:18.742319 chatting_with_pdfs-0.0.11/setup.cfg
+-rw-rw-rw-   0        0        0      816 2023-07-17 08:17:41.000000 chatting_with_pdfs-0.0.11/setup.py
```

### Comparing `chatting_with_pdfs-0.0.10/LICENSE` & `chatting_with_pdfs-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `chatting_with_pdfs-0.0.10/PKG-INFO` & `chatting_with_pdfs-0.0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatting_with_pdfs
-Version: 0.0.10
+Version: 0.0.11
 Summary: Load a PDF file and ask questions via llama_index and GPT.
 Author: Morne
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `chatting_with_pdfs-0.0.10/README.md` & `chatting_with_pdfs-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `chatting_with_pdfs-0.0.10/app/chatting_with_pdfs.egg-info/PKG-INFO` & `chatting_with_pdfs-0.0.11/app/chatting_with_pdfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatting-with-pdfs
-Version: 0.0.10
+Version: 0.0.11
 Summary: Load a PDF file and ask questions via llama_index and GPT.
 Author: Morne
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `chatting_with_pdfs-0.0.10/setup.py` & `chatting_with_pdfs-0.0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r", encoding="utf8") as f:
     long_description = f.read()
 
 setup(
     name="chatting_with_pdfs",
-    version="0.0.10",
+    version="0.0.11",
     description="Load a PDF file and ask questions via llama_index and GPT.",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Morne",
     license="MIT",
```

