# Comparing `tmp/float_table-0.1.4.tar.gz` & `tmp/float_table-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "float_table-0.1.4.tar", max compression
+gzip compressed data, was "float_table-0.1.5.tar", max compression
```

## Comparing `float_table-0.1.4.tar` & `float_table-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        4 2023-07-16 18:30:44.357591 float_table-0.1.4/README.md
--rw-r--r--   0        0        0      165 2023-07-16 20:27:07.444635 float_table-0.1.4/float_table/__init__.py
--rw-r--r--   0        0        0     2910 2023-07-16 21:39:45.016397 float_table-0.1.4/float_table/fmt.py
--rw-r--r--   0        0        0      824 2023-07-16 21:40:10.951129 float_table-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-16 16:20:05.484880 float_table-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     2763 2023-07-16 21:39:25.227350 float_table-0.1.4/tests/test.py
--rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 float_table-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        4 2023-07-16 18:30:44.357591 float_table-0.1.5/README.md
+-rw-r--r--   0        0        0      165 2023-07-16 21:40:31.971112 float_table-0.1.5/float_table/__init__.py
+-rw-r--r--   0        0        0     2910 2023-07-16 21:40:33.067971 float_table-0.1.5/float_table/fmt.py
+-rw-r--r--   0        0        0      824 2023-07-16 21:43:50.236210 float_table-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-16 16:20:05.484880 float_table-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     2763 2023-07-16 21:40:33.068136 float_table-0.1.5/tests/test.py
+-rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 float_table-0.1.5/PKG-INFO
```

### Comparing `float_table-0.1.4/float_table/fmt.py` & `float_table-0.1.5/float_table/fmt.py`

 * *Files identical despite different names*

### Comparing `float_table-0.1.4/pyproject.toml` & `float_table-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "float-table"
-version = "0.1.4"
+version = "0.1.5"
 homepage = "https://github.com/tadamcz/float-table"
 description = "Top-level package for float-table."
 authors = ["Tom Adamczewski <tadamczewskipublic@gmail.com>"]
 readme = "README.md"
 classifiers=[
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
```

### Comparing `float_table-0.1.4/tests/test.py` & `float_table-0.1.5/tests/test.py`

 * *Files identical despite different names*

### Comparing `float_table-0.1.4/PKG-INFO` & `float_table-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: float-table
-Version: 0.1.4
+Version: 0.1.5
 Summary: Top-level package for float-table.
 Home-page: https://github.com/tadamcz/float-table
 Author: Tom Adamczewski
 Author-email: tadamczewskipublic@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

