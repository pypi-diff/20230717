# Comparing `tmp/fgen-0.1.1.tar.gz` & `tmp/fgen-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgen-0.1.1.tar", max compression
+gzip compressed data, was "fgen-0.1.2.tar", max compression
```

## Comparing `fgen-0.1.1.tar` & `fgen-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1461 2023-07-14 04:41:25.452781 fgen-0.1.1/LICENSE
--rw-r--r--   0        0        0     2094 2023-07-14 04:41:25.452781 fgen-0.1.1/README.md
--rw-r--r--   0        0        0     5211 2023-07-14 04:41:25.454781 fgen-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      316 2023-07-14 04:41:25.454781 fgen-0.1.1/src/fgen/__init__.py
--rw-r--r--   0        0        0      103 2023-07-14 04:41:25.454781 fgen-0.1.1/src/fgen/commands/__init__.py
--rw-r--r--   0        0        0      429 2023-07-14 04:41:25.454781 fgen-0.1.1/src/fgen/commands/base.py
--rw-r--r--   0        0        0     2450 2023-07-14 04:41:25.454781 fgen-0.1.1/src/fgen/commands/generate.py
--rw-r--r--   0        0        0     4619 2023-07-14 04:41:25.454781 fgen-0.1.1/src/fgen/fortran_parsing.py
--rw-r--r--   0        0        0      165 2023-07-14 04:41:25.454781 fgen-0.1.1/src/fgen/main.py
--rw-r--r--   0        0        0        0 2023-07-14 04:41:25.481781 fgen-0.1.1/src/fgen/py.typed
--rw-r--r--   0        0        0    11287 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen/schema.py
--rw-r--r--   0        0        0     2119 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen/templates/calculator_manager.f90.jinja
--rw-r--r--   0        0        0     3798 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen/templates/python_module.py.jinja
--rw-r--r--   0        0        0     3937 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen/templates/wrap_module.f90.jinja
--rw-r--r--   0        0        0     4889 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen/templator.py
--rw-r--r--   0        0        0      111 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen_runtime/__init__.py
--rw-r--r--   0        0        0     4414 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen_runtime/base.py
--rw-r--r--   0        0        0      130 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen_runtime/common.py
--rw-r--r--   0        0        0      543 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen_runtime/exceptions.py
--rw-r--r--   0        0        0     3240 1970-01-01 00:00:00.000000 fgen-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1461 2023-07-17 02:05:29.812434 fgen-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2094 2023-07-17 02:05:29.812434 fgen-0.1.2/README.md
+-rw-r--r--   0        0        0     5245 2023-07-17 02:05:29.814433 fgen-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      316 2023-07-17 02:05:29.814433 fgen-0.1.2/src/fgen/__init__.py
+-rw-r--r--   0        0        0      103 2023-07-17 02:05:29.814433 fgen-0.1.2/src/fgen/commands/__init__.py
+-rw-r--r--   0        0        0      429 2023-07-17 02:05:29.814433 fgen-0.1.2/src/fgen/commands/base.py
+-rw-r--r--   0        0        0     2450 2023-07-17 02:05:29.814433 fgen-0.1.2/src/fgen/commands/generate.py
+-rw-r--r--   0        0        0     2806 2023-07-17 02:05:29.814433 fgen-0.1.2/src/fgen/f2py.py
+-rw-r--r--   0        0        0     4619 2023-07-17 02:05:29.814433 fgen-0.1.2/src/fgen/fortran_parsing.py
+-rw-r--r--   0        0        0      165 2023-07-17 02:05:29.814433 fgen-0.1.2/src/fgen/main.py
+-rw-r--r--   0        0        0        0 2023-07-17 02:05:29.840433 fgen-0.1.2/src/fgen/py.typed
+-rw-r--r--   0        0        0    11287 2023-07-17 02:05:29.814433 fgen-0.1.2/src/fgen/schema.py
+-rw-r--r--   0        0        0     2119 2023-07-17 02:05:29.815434 fgen-0.1.2/src/fgen/templates/calculator_manager.f90.jinja
+-rw-r--r--   0        0        0     3798 2023-07-17 02:05:29.815434 fgen-0.1.2/src/fgen/templates/python_module.py.jinja
+-rw-r--r--   0        0        0     3937 2023-07-17 02:05:29.815434 fgen-0.1.2/src/fgen/templates/wrap_module.f90.jinja
+-rw-r--r--   0        0        0     4889 2023-07-17 02:05:29.815434 fgen-0.1.2/src/fgen/templator.py
+-rw-r--r--   0        0        0      111 2023-07-17 02:05:29.815434 fgen-0.1.2/src/fgen_runtime/__init__.py
+-rw-r--r--   0        0        0     4414 2023-07-17 02:05:29.815434 fgen-0.1.2/src/fgen_runtime/base.py
+-rw-r--r--   0        0        0      130 2023-07-17 02:05:29.815434 fgen-0.1.2/src/fgen_runtime/common.py
+-rw-r--r--   0        0        0      543 2023-07-17 02:05:29.815434 fgen-0.1.2/src/fgen_runtime/exceptions.py
+-rw-r--r--   0        0        0     3240 1970-01-01 00:00:00.000000 fgen-0.1.2/PKG-INFO
```

### Comparing `fgen-0.1.1/LICENSE` & `fgen-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fgen-0.1.1/README.md` & `fgen-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fgen-0.1.1/pyproject.toml` & `fgen-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgen"
-version = "0.1.1"
+version = "0.1.2"
 description = "Automatically generate wrapper to integrate Fortran and Python"
 authors = ["Jared Lewis <jared.lewis@climate-energy-college.org>"]
 readme = "README.md"
 packages = [
     {include = "fgen", from = "src"},
     {include = "fgen_runtime", from = "src"},
 ]
@@ -67,14 +67,17 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.run]
 source = ["src/fgen"]
+omit = [
+    "src/fgen/f2py.py"
+]
 branch = true
 
 [tool.coverage.report]
 fail_under = 95
 skip_empty = true
 show_missing = true
 # Regexes for lines to exclude from consideration in addition to the defaults
```

### Comparing `fgen-0.1.1/src/fgen/commands/generate.py` & `fgen-0.1.2/src/fgen/commands/generate.py`

 * *Files identical despite different names*

### Comparing `fgen-0.1.1/src/fgen/fortran_parsing.py` & `fgen-0.1.2/src/fgen/fortran_parsing.py`

 * *Files identical despite different names*

### Comparing `fgen-0.1.1/src/fgen/schema.py` & `fgen-0.1.2/src/fgen/schema.py`

 * *Files identical despite different names*

### Comparing `fgen-0.1.1/src/fgen/templates/calculator_manager.f90.jinja` & `fgen-0.1.2/src/fgen/templates/calculator_manager.f90.jinja`

 * *Files identical despite different names*

### Comparing `fgen-0.1.1/src/fgen/templates/python_module.py.jinja` & `fgen-0.1.2/src/fgen/templates/python_module.py.jinja`

 * *Files identical despite different names*

### Comparing `fgen-0.1.1/src/fgen/templates/wrap_module.f90.jinja` & `fgen-0.1.2/src/fgen/templates/wrap_module.f90.jinja`

 * *Files identical despite different names*

### Comparing `fgen-0.1.1/src/fgen/templator.py` & `fgen-0.1.2/src/fgen/templator.py`

 * *Files identical despite different names*

### Comparing `fgen-0.1.1/src/fgen_runtime/base.py` & `fgen-0.1.2/src/fgen_runtime/base.py`

 * *Files identical despite different names*

### Comparing `fgen-0.1.1/src/fgen_runtime/exceptions.py` & `fgen-0.1.2/src/fgen_runtime/exceptions.py`

 * *Files identical despite different names*

### Comparing `fgen-0.1.1/PKG-INFO` & `fgen-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgen
-Version: 0.1.1
+Version: 0.1.2
 Summary: Automatically generate wrapper to integrate Fortran and Python
 Home-page: https://gitlab.com/magicc/fgen
 License: BSD-3-Clause
 Keywords: fortran
 Author: Jared Lewis
 Author-email: jared.lewis@climate-energy-college.org
 Requires-Python: >=3.9,<4.0
```

