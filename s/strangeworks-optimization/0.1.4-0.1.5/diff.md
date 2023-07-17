# Comparing `tmp/strangeworks_optimization-0.1.4.tar.gz` & `tmp/strangeworks_optimization-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_optimization-0.1.4.tar", max compression
+gzip compressed data, was "strangeworks_optimization-0.1.5.tar", max compression
```

## Comparing `strangeworks_optimization-0.1.4.tar` & `strangeworks_optimization-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      196 2023-07-13 14:28:47.827502 strangeworks_optimization-0.1.4/README.md
--rw-r--r--   0        0        0      994 2023-07-13 14:29:02.019658 strangeworks_optimization-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      174 2023-07-13 14:28:47.827502 strangeworks_optimization-0.1.4/strangeworks_optimization/__init__.py
--rw-r--r--   0        0        0     2746 2023-07-13 14:28:47.827502 strangeworks_optimization-0.1.4/strangeworks_optimization/optimization.py
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 strangeworks_optimization-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      196 2023-07-17 14:44:56.645051 strangeworks_optimization-0.1.5/README.md
+-rw-r--r--   0        0        0     1016 2023-07-17 14:45:10.421563 strangeworks_optimization-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-07-17 14:44:56.649051 strangeworks_optimization-0.1.5/strangeworks_optimization/__init__.py
+-rw-r--r--   0        0        0     4438 2023-07-17 14:44:56.649051 strangeworks_optimization-0.1.5/strangeworks_optimization/optimization.py
+-rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 strangeworks_optimization-0.1.5/PKG-INFO
```

### Comparing `strangeworks_optimization-0.1.4/pyproject.toml` & `strangeworks_optimization-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-optimization"
-version = "0.1.4"
+version = "0.1.5"
 description = "This SDK extends the Strangeworks SDK to provide access to the Strangeworks Optimization API."
 authors = ["Strange Devs <hello@strangeworks.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "strangeworks_optimization"}]
 
 
@@ -18,14 +18,15 @@
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.23.2"
 python-dotenv = "^1.0.0"
 pytest = "^7.3.1"
 ruff = "^0.0.272"
 black = ">=22.10.0,<23.0.0"
+pre-commit = "^3.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 markers = [
     "integration_could_cost_money: marks tests as creating a job that could cost some money (deselect with '-m \"not integration_could_cost_money\"')",
```

### Comparing `strangeworks_optimization-0.1.4/PKG-INFO` & `strangeworks_optimization-0.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-optimization
-Version: 0.1.4
+Version: 0.1.5
 Summary: This SDK extends the Strangeworks SDK to provide access to the Strangeworks Optimization API.
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

