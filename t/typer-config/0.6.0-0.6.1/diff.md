# Comparing `tmp/typer_config-0.6.0.tar.gz` & `tmp/typer_config-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_config-0.6.0.tar", max compression
+gzip compressed data, was "typer_config-0.6.1.tar", max compression
```

## Comparing `typer_config-0.6.0.tar` & `typer_config-0.6.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-05-01 15:54:43.337757 typer_config-0.6.0/LICENSE
--rw-r--r--   0        0        0     2473 2023-07-17 16:12:30.477542 typer_config-0.6.0/README.md
--rw-r--r--   0        0        0     2651 2023-07-17 16:13:24.487598 typer_config-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      363 2023-07-17 15:34:49.905969 typer_config-0.6.0/typer_config/__init__.py
--rw-r--r--   0        0        0      819 2023-07-17 15:34:49.909791 typer_config-0.6.0/typer_config/__optional_imports.py
--rw-r--r--   0        0        0     1910 2023-07-17 15:34:49.913567 typer_config-0.6.0/typer_config/__typing.py
--rw-r--r--   0        0        0     4086 2023-07-17 15:34:49.917414 typer_config-0.6.0/typer_config/callbacks.py
--rw-r--r--   0        0        0     9482 2023-07-17 15:34:49.920773 typer_config-0.6.0/typer_config/decorators.py
--rw-r--r--   0        0        0     1611 2023-07-17 15:34:49.924143 typer_config-0.6.0/typer_config/dumpers.py
--rw-r--r--   0        0        0     8598 2023-07-17 15:34:49.928143 typer_config-0.6.0/typer_config/loaders.py
--rw-r--r--   0        0        0     4226 1970-01-01 00:00:00.000000 typer_config-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-17 16:24:03.224066 typer_config-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2473 2023-07-17 16:24:03.224809 typer_config-0.6.1/README.md
+-rw-r--r--   0        0        0     2651 2023-07-17 20:55:59.582462 typer_config-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      363 2023-07-17 16:24:03.264789 typer_config-0.6.1/typer_config/__init__.py
+-rw-r--r--   0        0        0      819 2023-07-17 16:24:03.272535 typer_config-0.6.1/typer_config/__optional_imports.py
+-rw-r--r--   0        0        0     1910 2023-07-17 16:24:03.279419 typer_config-0.6.1/typer_config/__typing.py
+-rw-r--r--   0        0        0     4086 2023-07-17 16:24:03.282926 typer_config-0.6.1/typer_config/callbacks.py
+-rw-r--r--   0        0        0     9482 2023-07-17 16:24:03.286842 typer_config-0.6.1/typer_config/decorators.py
+-rw-r--r--   0        0        0     1611 2023-07-17 16:24:03.293519 typer_config-0.6.1/typer_config/dumpers.py
+-rw-r--r--   0        0        0     8598 2023-07-17 16:24:03.332219 typer_config-0.6.1/typer_config/loaders.py
+-rw-r--r--   0        0        0     4226 1970-01-01 00:00:00.000000 typer_config-0.6.1/PKG-INFO
```

### Comparing `typer_config-0.6.0/LICENSE` & `typer_config-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_config-0.6.0/README.md` & `typer_config-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `typer_config-0.6.0/pyproject.toml` & `typer_config-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typer-config"
-version = "0.6.0"
+version = "0.6.1"
 description = "Utilities for working with configuration files in typer CLIs. "
 authors = ["Matt Anderson <matt@manderscience.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "typer_config"}]
 repository = "https://github.com/maxb2/typer-config"
 documentation = "https://maxb2.github.io/typer-config/"
```

### Comparing `typer_config-0.6.0/typer_config/__optional_imports.py` & `typer_config-0.6.1/typer_config/__optional_imports.py`

 * *Files identical despite different names*

### Comparing `typer_config-0.6.0/typer_config/__typing.py` & `typer_config-0.6.1/typer_config/__typing.py`

 * *Files identical despite different names*

### Comparing `typer_config-0.6.0/typer_config/callbacks.py` & `typer_config-0.6.1/typer_config/callbacks.py`

 * *Files identical despite different names*

### Comparing `typer_config-0.6.0/typer_config/decorators.py` & `typer_config-0.6.1/typer_config/decorators.py`

 * *Files identical despite different names*

### Comparing `typer_config-0.6.0/typer_config/dumpers.py` & `typer_config-0.6.1/typer_config/dumpers.py`

 * *Files identical despite different names*

### Comparing `typer_config-0.6.0/typer_config/loaders.py` & `typer_config-0.6.1/typer_config/loaders.py`

 * *Files identical despite different names*

### Comparing `typer_config-0.6.0/PKG-INFO` & `typer_config-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typer-config
-Version: 0.6.0
+Version: 0.6.1
 Summary: Utilities for working with configuration files in typer CLIs. 
 Home-page: https://maxb2.github.io/typer-config/
 License: MIT
 Keywords: typer,config,configuration,configuration-file,yaml,toml,json,dotenv,cli
 Author: Matt Anderson
 Author-email: matt@manderscience.com
 Requires-Python: >=3.8,<4.0
```

