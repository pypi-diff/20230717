# Comparing `tmp/retrival-1.0.1.tar.gz` & `tmp/retrival-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retrival-1.0.1.tar", last modified: Wed Feb 22 10:07:43 2023, max compression
+gzip compressed data, was "retrival-1.0.2.tar", last modified: Mon Jul 17 03:36:00 2023, max compression
```

## Comparing `retrival-1.0.1.tar` & `retrival-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 10:07:43.986437 retrival-1.0.1/
--rw-r--r--   0 root         (0) root         (0)    11558 2023-02-17 16:57:32.000000 retrival-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1094 2023-02-22 10:07:43.986437 retrival-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1068 2023-02-22 06:20:22.000000 retrival-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 10:07:43.985437 retrival-1.0.1/retrival/
--rw-r--r--   0 root         (0) root         (0)      105 2023-02-22 10:06:20.000000 retrival-1.0.1/retrival/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8834 2023-02-22 06:50:13.000000 retrival-1.0.1/retrival/search_engine.py
--rw-r--r--   0 root         (0) root         (0)     3822 2023-02-21 07:08:43.000000 retrival-1.0.1/retrival/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 10:07:43.986437 retrival-1.0.1/retrival.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1094 2023-02-22 10:07:43.000000 retrival-1.0.1/retrival.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      250 2023-02-22 10:07:43.000000 retrival-1.0.1/retrival.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-22 10:07:43.000000 retrival-1.0.1/retrival.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-02-22 10:07:43.000000 retrival-1.0.1/retrival.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-02-22 10:07:43.000000 retrival-1.0.1/retrival.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-22 10:07:43.986437 retrival-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1539 2023-02-22 05:52:25.000000 retrival-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 03:36:00.943925 retrival-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)    11558 2023-07-17 01:22:52.000000 retrival-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-07-17 03:36:00.943925 retrival-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-07-17 01:22:52.000000 retrival-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 03:36:00.942925 retrival-1.0.2/retrival/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-17 01:24:05.000000 retrival-1.0.2/retrival/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9070 2023-07-17 01:51:57.000000 retrival-1.0.2/retrival/search_engine.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2023-07-17 01:22:52.000000 retrival-1.0.2/retrival/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 03:36:00.942925 retrival-1.0.2/retrival.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-07-17 03:36:00.000000 retrival-1.0.2/retrival.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      250 2023-07-17 03:36:00.000000 retrival-1.0.2/retrival.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 03:36:00.000000 retrival-1.0.2/retrival.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-17 03:36:00.000000 retrival-1.0.2/retrival.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-17 03:36:00.000000 retrival-1.0.2/retrival.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 03:36:00.943925 retrival-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-07-17 02:02:27.000000 retrival-1.0.2/setup.py
```

### Comparing `retrival-1.0.1/LICENSE` & `retrival-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `retrival-1.0.1/PKG-INFO` & `retrival-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retrival
-Version: 1.0.1
+Version: 1.0.2
 Summary: Just for BM25
 Home-page: https://github.com/skykiseki/retrival
 Author: Wei, Zhihui
 Author-email: evelinesdd@qq.com
 License: MIT
 Keywords: retrival
 Platform: UNKNOWN
```

### Comparing `retrival-1.0.1/README.md` & `retrival-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `retrival-1.0.1/retrival/search_engine.py` & `retrival-1.0.2/retrival/search_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import jieba
 import numba as nb
 import json
 import numpy as np
 import jsonlines
 import os
+import fcntl
 from indxr import Indxr
 from numba.typed import List as TypedList
 from collections import defaultdict
 from sklearn.feature_extraction.text import CountVectorizer
 from typing import List, Iterable, Dict
 from .utils import bm25
 
@@ -224,28 +225,32 @@
         ----------
 
         Returns:
         -------
 
         """
         # 先删除原始文件
-        if os.path.isfile(self.path_jsonl):
+        if os.path.exists(self.path_jsonl):
             os.remove(self.path_jsonl)
 
         # 再开始生成jsonl文件
         if self.corpus is None:
             raise NotImplementedError('No corpus data found')
 
         else:
-            corpus_writer = jsonlines.open(self.path_jsonl, mode='a')
-            for d in self.corpus:
-                corpus_writer.write(d)
-
-            corpus_writer.close()
-
+            with jsonlines.open(self.path_jsonl, mode='a') as writer:
+                # 加文件锁
+                fcntl.flock(writer._fp.fileno(), fcntl.LOCK_EX)
+
+                try:
+                    for d in self.corpus:
+                        writer.write(d)
+                finally:
+                    # 解锁文件
+                    fcntl.flock(writer._fp.fileno(), fcntl.LOCK_UN)
 
     def get_docs(self, doc_ids: List[str]) -> List[dict]:
         """
         基于原始id获取原始docs
 
         Parameters:
         ----------
```

### Comparing `retrival-1.0.1/retrival/utils.py` & `retrival-1.0.2/retrival/utils.py`

 * *Files identical despite different names*

### Comparing `retrival-1.0.1/retrival.egg-info/PKG-INFO` & `retrival-1.0.2/retrival.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retrival
-Version: 1.0.1
+Version: 1.0.2
 Summary: Just for BM25
 Home-page: https://github.com/skykiseki/retrival
 Author: Wei, Zhihui
 Author-email: evelinesdd@qq.com
 License: MIT
 Keywords: retrival
 Platform: UNKNOWN
```

### Comparing `retrival-1.0.1/setup.py` & `retrival-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 完整文档见 ``README.md``
 
 GitHub: https://github.com/skykiseki/retrival
 """
 
 setup(name='retrival',
-      version='1.0.1',
+      version='1.0.2',
       description='Just for BM25',
       long_description=LONGDOC,
       long_description_content_type="text/markdown",
       author='Wei, Zhihui',
       author_email='evelinesdd@qq.com',
       url='https://github.com/skykiseki/retrival',
       license="MIT",
```

