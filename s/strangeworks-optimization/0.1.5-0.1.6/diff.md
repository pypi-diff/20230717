# Comparing `tmp/strangeworks_optimization-0.1.5.tar.gz` & `tmp/strangeworks_optimization-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_optimization-0.1.5.tar", max compression
+gzip compressed data, was "strangeworks_optimization-0.1.6.tar", max compression
```

## Comparing `strangeworks_optimization-0.1.5.tar` & `strangeworks_optimization-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      196 2023-07-17 14:44:56.645051 strangeworks_optimization-0.1.5/README.md
--rw-r--r--   0        0        0     1016 2023-07-17 14:45:10.421563 strangeworks_optimization-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      174 2023-07-17 14:44:56.649051 strangeworks_optimization-0.1.5/strangeworks_optimization/__init__.py
--rw-r--r--   0        0        0     4438 2023-07-17 14:44:56.649051 strangeworks_optimization-0.1.5/strangeworks_optimization/optimization.py
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 strangeworks_optimization-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      196 2023-07-17 21:42:14.320216 strangeworks_optimization-0.1.6/README.md
+-rw-r--r--   0        0        0     1009 2023-07-17 21:42:27.824425 strangeworks_optimization-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-07-17 21:42:14.320216 strangeworks_optimization-0.1.6/strangeworks_optimization/__init__.py
+-rw-r--r--   0        0        0     4438 2023-07-17 21:42:14.320216 strangeworks_optimization-0.1.6/strangeworks_optimization/optimization.py
+-rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 strangeworks_optimization-0.1.6/PKG-INFO
```

### Comparing `strangeworks_optimization-0.1.5/pyproject.toml` & `strangeworks_optimization-0.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "strangeworks-optimization"
-version = "0.1.5"
+version = "0.1.6"
 description = "This SDK extends the Strangeworks SDK to provide access to the Strangeworks Optimization API."
 authors = ["Strange Devs <hello@strangeworks.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "strangeworks_optimization"}]
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-strangeworks = "^0.4.2"
+strangeworks = "^0.4.4"
 dimod = "^0.12.7"
-strangeworks-python-core = "^0.1.7"
+strangeworks-core = "^0.2.3"
 pydantic = "^1.10.9"
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.23.2"
 python-dotenv = "^1.0.0"
 pytest = "^7.3.1"
```

### Comparing `strangeworks_optimization-0.1.5/strangeworks_optimization/optimization.py` & `strangeworks_optimization-0.1.6/strangeworks_optimization/optimization.py`

 * *Files identical despite different names*

### Comparing `strangeworks_optimization-0.1.5/PKG-INFO` & `strangeworks_optimization-0.1.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: strangeworks-optimization
-Version: 0.1.5
+Version: 0.1.6
 Summary: This SDK extends the Strangeworks SDK to provide access to the Strangeworks Optimization API.
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dimod (>=0.12.7,<0.13.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
-Requires-Dist: strangeworks (>=0.4.2,<0.5.0)
-Requires-Dist: strangeworks-python-core (>=0.1.7,<0.2.0)
+Requires-Dist: strangeworks (>=0.4.4,<0.5.0)
+Requires-Dist: strangeworks-core (>=0.2.3,<0.3.0)
 Description-Content-Type: text/markdown
 
 ![Tests](https://github.com/strangeworks/strangeworks-optimization/actions/workflows/cron_test.yml/badge.svg)
 
 # strangeworks-optimization
 
 [Docs](https://docs.strangeworks.com/apps/optimization)
```

