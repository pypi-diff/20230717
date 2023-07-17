# Comparing `tmp/sc_cc_ng_sdk_python-0.1.8.tar.gz` & `tmp/sc_cc_ng_sdk_python-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc_cc_ng_sdk_python-0.1.8.tar", max compression
+gzip compressed data, was "sc_cc_ng_sdk_python-0.1.9.tar", max compression
```

## Comparing `sc_cc_ng_sdk_python-0.1.8.tar` & `sc_cc_ng_sdk_python-0.1.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-26 13:45:09.675633 sc_cc_ng_sdk_python-0.1.8/README.md
--rw-r--r--   0        0        0      530 2023-07-07 09:06:14.671219 sc_cc_ng_sdk_python-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    16277 2023-06-28 12:50:17.041509 sc_cc_ng_sdk_python-0.1.8/sc_cc_ng_sdk_python/__init__.py
--rw-r--r--   0        0        0      497 1970-01-01 00:00:00.000000 sc_cc_ng_sdk_python-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-26 13:45:09.675633 sc_cc_ng_sdk_python-0.1.9/README.md
+-rw-r--r--   0        0        0      530 2023-07-17 11:41:40.447560 sc_cc_ng_sdk_python-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    16277 2023-06-28 12:50:17.041509 sc_cc_ng_sdk_python-0.1.9/sc_cc_ng_sdk_python/__init__.py
+-rw-r--r--   0        0        0      497 1970-01-01 00:00:00.000000 sc_cc_ng_sdk_python-0.1.9/PKG-INFO
```

### Comparing `sc_cc_ng_sdk_python-0.1.8/pyproject.toml` & `sc_cc_ng_sdk_python-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "sc-cc-ng-sdk-python"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Rikard Olsson <rikard@thryselius.se>"]
 readme = "README.md"
 packages = [{include = "sc_cc_ng_sdk_python"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-sc-cc-ng-models-python = "^0.1.6"
+sc-cc-ng-models-python = "^0.1.7"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.0.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `sc_cc_ng_sdk_python-0.1.8/sc_cc_ng_sdk_python/__init__.py` & `sc_cc_ng_sdk_python-0.1.9/sc_cc_ng_sdk_python/__init__.py`

 * *Files identical despite different names*

