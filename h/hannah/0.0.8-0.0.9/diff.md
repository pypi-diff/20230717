# Comparing `tmp/hannah-0.0.8.tar.gz` & `tmp/hannah-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hannah-0.0.8.tar", max compression
+gzip compressed data, was "hannah-0.0.9.tar", max compression
```

## Comparing `hannah-0.0.8.tar` & `hannah-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1077 2023-02-26 06:56:27.199180 hannah-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0      460 2023-02-26 06:56:27.199245 hannah-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-02-26 06:56:27.199309 hannah-0.0.8/hannah/__init__.py
--rw-r--r--   0        0        0       45 2023-02-26 06:56:27.199389 hannah-0.0.8/hannah/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-26 06:56:27.199456 hannah-0.0.8/hannah/http/__init__.py
--rw-r--r--   0        0        0     1931 2023-02-26 06:56:27.199538 hannah-0.0.8/hannah/http/mappings.py
--rw-r--r--   0        0        0     1983 2023-02-26 06:56:27.199630 hannah-0.0.8/hannah/http/session.py
--rw-r--r--   0        0        0     2444 2023-02-26 07:27:30.913690 hannah-0.0.8/hannah/models.py
--rw-r--r--   0        0        0     1274 2023-02-26 06:56:27.199776 hannah-0.0.8/hannah/parsers.py
--rw-r--r--   0        0        0        0 2023-02-26 06:56:27.199842 hannah-0.0.8/hannah/tests/__init__.py
--rw-r--r--   0        0        0     1162 2023-02-26 06:56:27.199926 hannah-0.0.8/hannah/tests/test_http.py
--rw-r--r--   0        0        0      387 2023-02-26 06:56:27.199999 hannah-0.0.8/hannah/tests/test_swagger.py
--rw-r--r--   0        0        0      504 2023-02-26 07:21:51.907082 hannah-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1171 1970-01-01 00:00:00.000000 hannah-0.0.8/setup.py
--rw-r--r--   0        0        0     1218 1970-01-01 00:00:00.000000 hannah-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-02-26 06:56:27.199180 hannah-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0      460 2023-02-26 06:56:27.199245 hannah-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-02-26 06:56:27.199309 hannah-0.0.9/hannah/__init__.py
+-rw-r--r--   0        0        0       45 2023-02-26 06:56:27.199389 hannah-0.0.9/hannah/exceptions.py
+-rw-r--r--   0        0        0        0 2023-02-26 06:56:27.199456 hannah-0.0.9/hannah/http/__init__.py
+-rw-r--r--   0        0        0     1931 2023-02-26 06:56:27.199538 hannah-0.0.9/hannah/http/mappings.py
+-rw-r--r--   0        0        0     1983 2023-02-26 06:56:27.199630 hannah-0.0.9/hannah/http/session.py
+-rw-r--r--   0        0        0     2444 2023-02-26 07:27:30.913690 hannah-0.0.9/hannah/models.py
+-rw-r--r--   0        0        0     1274 2023-02-26 06:56:27.199776 hannah-0.0.9/hannah/parsers.py
+-rw-r--r--   0        0        0        0 2023-02-26 06:56:27.199842 hannah-0.0.9/hannah/tests/__init__.py
+-rw-r--r--   0        0        0     1162 2023-02-26 06:56:27.199926 hannah-0.0.9/hannah/tests/test_http.py
+-rw-r--r--   0        0        0      387 2023-02-26 06:56:27.199999 hannah-0.0.9/hannah/tests/test_swagger.py
+-rw-r--r--   0        0        0      504 2023-07-17 13:19:26.216511 hannah-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1218 1970-01-01 00:00:00.000000 hannah-0.0.9/PKG-INFO
```

### Comparing `hannah-0.0.8/LICENSE.txt` & `hannah-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hannah-0.0.8/hannah/http/mappings.py` & `hannah-0.0.9/hannah/http/mappings.py`

 * *Files identical despite different names*

### Comparing `hannah-0.0.8/hannah/http/session.py` & `hannah-0.0.9/hannah/http/session.py`

 * *Files identical despite different names*

### Comparing `hannah-0.0.8/hannah/models.py` & `hannah-0.0.9/hannah/models.py`

 * *Files identical despite different names*

### Comparing `hannah-0.0.8/hannah/parsers.py` & `hannah-0.0.9/hannah/parsers.py`

 * *Files identical despite different names*

### Comparing `hannah-0.0.8/hannah/tests/test_http.py` & `hannah-0.0.9/hannah/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `hannah-0.0.8/PKG-INFO` & `hannah-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hannah
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Home-page: https://github.com/suganthsundar/hannah
 License: MIT
 Author: suganthsundar
 Author-email: suganthsundar@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

