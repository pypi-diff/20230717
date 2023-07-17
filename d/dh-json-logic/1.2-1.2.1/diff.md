# Comparing `tmp/dh_json_logic-1.2.tar.gz` & `tmp/dh_json_logic-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dh_json_logic-1.2.tar", max compression
+gzip compressed data, was "dh_json_logic-1.2.1.tar", max compression
```

## Comparing `dh_json_logic-1.2.tar` & `dh_json_logic-1.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2023-07-14 12:48:30.491825 dh_json_logic-1.2/LICENSE
--rw-r--r--   0        0        0     3168 2023-07-14 12:48:30.491825 dh_json_logic-1.2/README.md
--rw-r--r--   0        0        0    31272 2023-07-14 12:48:30.491825 dh_json_logic-1.2/dh_json_logic/__init__.py
--rw-r--r--   0        0        0     1272 2023-07-14 12:48:30.491825 dh_json_logic-1.2/pyproject.toml
--rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 dh_json_logic-1.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-17 09:49:23.707630 dh_json_logic-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3169 2023-07-17 09:49:23.707630 dh_json_logic-1.2.1/README.md
+-rw-r--r--   0        0        0    31272 2023-07-17 09:49:23.707630 dh_json_logic-1.2.1/dh_json_logic/__init__.py
+-rw-r--r--   0        0        0     1274 2023-07-17 09:49:23.707630 dh_json_logic-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3658 1970-01-01 00:00:00.000000 dh_json_logic-1.2.1/PKG-INFO
```

### Comparing `dh_json_logic-1.2/LICENSE` & `dh_json_logic-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dh_json_logic-1.2/README.md` & `dh_json_logic-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # json-logic-py
 **NOTE:** This is fork of https://github.com/YaraslauZhylko/json-logic-py/ created for use in our internal projects.
 
 
+
 ## Introduction
 This parser accepts [JsonLogic](http://jsonlogic.com) rules and executes them in Python.
 
 This is a Python porting of the excellent GitHub project by [jwadhams](https://github.com/jwadhams) for JavaScript: [json-logic-js](https://github.com/jwadhams/json-logic-js).
 
 All credit goes to him, this is simply an implementation of the same logic in Python (small differences below).
```

### Comparing `dh_json_logic-1.2/dh_json_logic/__init__.py` & `dh_json_logic-1.2.1/dh_json_logic/__init__.py`

 * *Files identical despite different names*

### Comparing `dh_json_logic-1.2/pyproject.toml` & `dh_json_logic-1.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = [ "poetry_core>=1.6.1" ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dh-json-logic"
-version = "1.2"
+version = "1.2.1"
 description = "A fork of https://github.com/YaraslauZhylko/json-logic-py/"
 readme="README.md"
 authors = [ "dearhealth" ]
 homepage = "https://github.com/dearhealth/json-logic-py"
 repository = "https://github.com/dearhealth/json-logic-py"
 
   [tool.poetry.dependencies]
```

### Comparing `dh_json_logic-1.2/PKG-INFO` & `dh_json_logic-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dh-json-logic
-Version: 1.2
+Version: 1.2.1
 Summary: A fork of https://github.com/YaraslauZhylko/json-logic-py/
 Home-page: https://github.com/dearhealth/json-logic-py
 Author: dearhealth
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/dearhealth/json-logic-py
 Description-Content-Type: text/markdown
 
 # json-logic-py
 **NOTE:** This is fork of https://github.com/YaraslauZhylko/json-logic-py/ created for use in our internal projects.
 
 
+
 ## Introduction
 This parser accepts [JsonLogic](http://jsonlogic.com) rules and executes them in Python.
 
 This is a Python porting of the excellent GitHub project by [jwadhams](https://github.com/jwadhams) for JavaScript: [json-logic-js](https://github.com/jwadhams/json-logic-js).
 
 All credit goes to him, this is simply an implementation of the same logic in Python (small differences below).
```

