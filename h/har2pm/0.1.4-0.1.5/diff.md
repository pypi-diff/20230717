# Comparing `tmp/har2pm-0.1.4.tar.gz` & `tmp/har2pm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2pm-0.1.4.tar", max compression
+gzip compressed data, was "har2pm-0.1.5.tar", max compression
```

## Comparing `har2pm-0.1.4.tar` & `har2pm-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       50 2023-07-14 10:20:04.533135 har2pm-0.1.4/har2pm/__init__.py
--rw-r--r--   0        0        0     1116 2023-07-14 10:20:04.533135 har2pm-0.1.4/har2pm/cli.py
--rw-r--r--   0        0        0     3681 2023-07-14 10:46:12.280974 har2pm-0.1.4/har2pm/common.py
--rw-r--r--   0        0        0     1856 2023-07-14 10:20:04.534134 har2pm-0.1.4/har2pm/har2postman.py
--rw-r--r--   0        0        0     1083 2023-07-14 10:20:04.532132 har2pm-0.1.4/LICENSE
--rw-r--r--   0        0        0      689 2023-07-17 03:33:17.489150 har2pm-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      604 2023-07-14 10:20:04.532132 har2pm-0.1.4/README.md
--rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 har2pm-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-07-14 10:20:04.533135 har2pm-0.1.5/har2pm/__init__.py
+-rw-r--r--   0        0        0     1106 2023-07-17 03:34:06.940299 har2pm-0.1.5/har2pm/cli.py
+-rw-r--r--   0        0        0     3680 2023-07-17 09:57:27.197777 har2pm-0.1.5/har2pm/common.py
+-rw-r--r--   0        0        0     1851 2023-07-17 03:34:06.940299 har2pm-0.1.5/har2pm/har2postman.py
+-rw-r--r--   0        0        0     1083 2023-07-14 10:20:04.532132 har2pm-0.1.5/LICENSE
+-rw-r--r--   0        0        0      689 2023-07-17 09:57:43.827275 har2pm-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      604 2023-07-14 10:20:04.532132 har2pm-0.1.5/README.md
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 har2pm-0.1.5/PKG-INFO
```

### Comparing `har2pm-0.1.4/har2pm/cli.py` & `har2pm-0.1.5/har2pm/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 import sys
 import logging
-from har2postman.har2postman import Har2Postman
-from har2postman import __version__
+from har2pm.har2postman import Har2Postman
+from har2pm import __version__
 
 
 def main():
     parser = argparse.ArgumentParser(description='har to postman collection')
     parser.add_argument(
         '-V', '--version', dest='version', action='store_true',
         help="show version")
```

### Comparing `har2pm-0.1.4/har2pm/common.py` & `har2pm-0.1.5/har2pm/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """
     with open(har_path, 'r', encoding='utf-8') as har:
         return json.load(har)
 
 
 def save_postman_collection(file_path, postman_json):
     with open(file_path, 'w') as postman:
-        postman.write(json.dumps(postman_json, indent=4, ensure_ascii=False))
+        postman.write(json.dumps(postman_json, indent=4, ensure_ascii=True))
 
 
 def extract_params(query):
     """
     :param query: (str) eg: q=testerhome&encoding=utf-8
     :return:
         [
```

### Comparing `har2pm-0.1.4/har2pm/har2postman.py` & `har2pm-0.1.5/har2pm/har2postman.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 import os
 
 import jmespath
 
-from har2postman.common import (convert_url, load_har, save_postman_collection, convert_body, convert_headers)
+from har2pm.common import (convert_url, load_har, save_postman_collection, convert_body, convert_headers)
 
 
 class Har2Postman:
 
     def __init__(self, har_path):
         self.har_path = har_path
         self.postman_collection = {
```

### Comparing `har2pm-0.1.4/LICENSE` & `har2pm-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `har2pm-0.1.4/pyproject.toml` & `har2pm-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "har2pm"
-version = "0.1.4"
+version = "0.1.5"
 description = "Convert HAR(HTTP Archive) to Postman Collection"
 authors = ["ysansan"]
 license = "MIT"
 homepage = "https://github.com/whitexie/Har2Postman"
 repository = "https://github.com/whitexie/Har2Postman"
 keywords = ["har", "postman"]
 readme = "README.md"
```

### Comparing `har2pm-0.1.4/README.md` & `har2pm-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `har2pm-0.1.4/PKG-INFO` & `har2pm-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har2pm
-Version: 0.1.4
+Version: 0.1.5
 Summary: Convert HAR(HTTP Archive) to Postman Collection
 Home-page: https://github.com/whitexie/Har2Postman
 License: MIT
 Keywords: har,postman
 Author: ysansan
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

