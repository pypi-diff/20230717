# Comparing `tmp/opset-3.0.0.tar.gz` & `tmp/opset-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opset-3.0.0.tar", max compression
+gzip compressed data, was "opset-3.0.0a1.tar", max compression
```

## Comparing `opset-3.0.0.tar` & `opset-3.0.0a1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-07-17 16:21:49.415760 opset-3.0.0/LICENSE
--rw-r--r--   0        0        0    24719 2023-07-17 16:21:49.415760 opset-3.0.0/README.md
--rw-r--r--   0        0        0      328 2023-07-17 16:21:49.415760 opset-3.0.0/opset/__init__.py
--rw-r--r--   0        0        0    24214 2023-07-17 17:20:51.727956 opset-3.0.0/opset/configurator.py
--rw-r--r--   0        0        0        0 2023-07-17 16:21:49.415760 opset-3.0.0/opset/py.typed
--rw-r--r--   0        0        0     3981 2023-07-17 16:59:01.186916 opset-3.0.0/opset/utils.py
--rw-r--r--   0        0        0     1663 2023-07-17 18:31:12.176762 opset-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    25661 1970-01-01 00:00:00.000000 opset-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-17 16:21:49.415760 opset-3.0.0a1/LICENSE
+-rw-r--r--   0        0        0    24719 2023-07-17 16:21:49.415760 opset-3.0.0a1/README.md
+-rw-r--r--   0        0        0      328 2023-07-17 16:21:49.415760 opset-3.0.0a1/opset/__init__.py
+-rw-r--r--   0        0        0    24214 2023-07-17 17:20:51.727956 opset-3.0.0a1/opset/configurator.py
+-rw-r--r--   0        0        0        0 2023-07-17 16:21:49.415760 opset-3.0.0a1/opset/py.typed
+-rw-r--r--   0        0        0     3981 2023-07-17 16:59:01.186916 opset-3.0.0a1/opset/utils.py
+-rw-r--r--   0        0        0     1665 2023-07-17 18:27:53.372084 opset-3.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0    25663 1970-01-01 00:00:00.000000 opset-3.0.0a1/PKG-INFO
```

### Comparing `opset-3.0.0/LICENSE` & `opset-3.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `opset-3.0.0/README.md` & `opset-3.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `opset-3.0.0/opset/configurator.py` & `opset-3.0.0a1/opset/configurator.py`

 * *Files identical despite different names*

### Comparing `opset-3.0.0/opset/utils.py` & `opset-3.0.0a1/opset/utils.py`

 * *Files identical despite different names*

### Comparing `opset-3.0.0/pyproject.toml` & `opset-3.0.0a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opset"
-version = "3.0.0"
+version = "3.0.0a1"
 description = "A library for simplifying the configuration of Python applications at all stages of deployment."
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/MarcDufresne/opset"
 repository = "https://github.com/MarcDufresne/opset"
 documentation = "https://github.com/MarcDufresne/opset"
 keywords = ["config", "management", "configuration", "logging", "setup"]
```

### Comparing `opset-3.0.0/PKG-INFO` & `opset-3.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opset
-Version: 3.0.0
+Version: 3.0.0a1
 Summary: A library for simplifying the configuration of Python applications at all stages of deployment.
 Home-page: https://github.com/MarcDufresne/opset
 License: Apache-2.0
 Keywords: config,management,configuration,logging,setup
 Author: Marc-André Dufresne
 Author-email: marc.andre.dufresne@gmail.com
 Requires-Python: >=3.10,<4.0
```

