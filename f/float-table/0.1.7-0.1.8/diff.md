# Comparing `tmp/float_table-0.1.7.tar.gz` & `tmp/float_table-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "float_table-0.1.7.tar", max compression
+gzip compressed data, was "float_table-0.1.8.tar", max compression
```

## Comparing `float_table-0.1.7.tar` & `float_table-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        4 2023-07-16 18:30:44.357591 float_table-0.1.7/README.md
--rw-r--r--   0        0        0      178 2023-07-17 09:50:19.103444 float_table-0.1.7/float_table/__init__.py
--rw-r--r--   0        0        0     4645 2023-07-17 11:39:05.920922 float_table-0.1.7/float_table/fmt.py
--rw-r--r--   0        0        0      844 2023-07-17 11:47:07.068481 float_table-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-16 16:20:05.484880 float_table-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0     2999 2023-07-17 11:23:41.558571 float_table-0.1.7/tests/test.py
--rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 float_table-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        4 2023-07-16 18:30:44.357591 float_table-0.1.8/README.md
+-rw-r--r--   0        0        0      178 2023-07-17 09:50:19.103444 float_table-0.1.8/float_table/__init__.py
+-rw-r--r--   0        0        0     4645 2023-07-17 11:39:05.920922 float_table-0.1.8/float_table/fmt.py
+-rw-r--r--   0        0        0      864 2023-07-17 17:14:40.471222 float_table-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-16 16:20:05.484880 float_table-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0     2999 2023-07-17 11:23:41.558571 float_table-0.1.8/tests/test.py
+-rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 float_table-0.1.8/PKG-INFO
```

### Comparing `float_table-0.1.7/float_table/fmt.py` & `float_table-0.1.8/float_table/fmt.py`

 * *Files identical despite different names*

### Comparing `float_table-0.1.7/pyproject.toml` & `float_table-0.1.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "float-table"
-version = "0.1.7"
+version = "0.1.8"
 homepage = "https://github.com/tadamcz/float-table"
 description = "Top-level package for float-table."
 authors = ["Tom Adamczewski <tadamczewskipublic@gmail.com>"]
 readme = "README.md"
 classifiers=[
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
@@ -15,14 +15,15 @@
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 numpy = "^1"
 pandas = "^2"
+tabulate = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
 bump2version = "*"
 coverage = "*"
 pytest = ">=7.2.0"
 pytest-pycharm = "*"
 sigfig = "*"
```

### Comparing `float_table-0.1.7/tests/test.py` & `float_table-0.1.8/tests/test.py`

 * *Files identical despite different names*

### Comparing `float_table-0.1.7/PKG-INFO` & `float_table-0.1.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: float-table
-Version: 0.1.7
+Version: 0.1.8
 Summary: Top-level package for float-table.
 Home-page: https://github.com/tadamcz/float-table
 Author: Tom Adamczewski
 Author-email: tadamczewskipublic@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1,<2)
 Requires-Dist: pandas (>=2,<3)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 TODO
```

