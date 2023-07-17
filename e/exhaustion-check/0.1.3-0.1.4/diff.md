# Comparing `tmp/exhaustion_check-0.1.3.tar.gz` & `tmp/exhaustion_check-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exhaustion_check-0.1.3.tar", max compression
+gzip compressed data, was "exhaustion_check-0.1.4.tar", max compression
```

## Comparing `exhaustion_check-0.1.3.tar` & `exhaustion_check-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1075 2023-05-16 14:06:14.197256 exhaustion_check-0.1.3/LICENSE.md
--rw-r--r--   0        0        0     4217 2023-05-16 14:06:14.173256 exhaustion_check-0.1.3/README.md
--rw-r--r--   0        0        0     2319 2023-05-16 18:46:02.650612 exhaustion_check-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      112 2023-05-16 14:06:14.201256 exhaustion_check-0.1.3/src/exhaustion_check/__init__.py
--rw-r--r--   0        0        0     2238 2023-05-16 14:41:21.482373 exhaustion_check-0.1.3/src/exhaustion_check/exhaustion_check.py
--rw-r--r--   0        0        0     1080 2023-05-16 18:44:39.413299 exhaustion_check-0.1.3/src/exhaustion_check/pretty_sort_yaml.py
--rw-r--r--   0        0        0     4839 1970-01-01 00:00:00.000000 exhaustion_check-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-16 14:06:14.197256 exhaustion_check-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0     4217 2023-05-16 14:06:14.173256 exhaustion_check-0.1.4/README.md
+-rw-r--r--   0        0        0     2383 2023-07-17 14:24:31.581607 exhaustion_check-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-05-16 14:06:14.201256 exhaustion_check-0.1.4/src/exhaustion_check/__init__.py
+-rw-r--r--   0        0        0     2238 2023-05-16 14:41:21.482373 exhaustion_check-0.1.4/src/exhaustion_check/exhaustion_check.py
+-rw-r--r--   0        0        0     1377 2023-07-17 13:58:38.076817 exhaustion_check-0.1.4/src/exhaustion_check/get_first_of_first.py
+-rw-r--r--   0        0        0     1080 2023-05-16 18:44:39.413299 exhaustion_check-0.1.4/src/exhaustion_check/pretty_sort_yaml.py
+-rw-r--r--   0        0        0     4839 1970-01-01 00:00:00.000000 exhaustion_check-0.1.4/PKG-INFO
```

### Comparing `exhaustion_check-0.1.3/LICENSE.md` & `exhaustion_check-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exhaustion_check-0.1.3/README.md` & `exhaustion_check-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `exhaustion_check-0.1.3/pyproject.toml` & `exhaustion_check-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "exhaustion-check"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Mark Andrew Miller <MAM@lbl.gov>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/turbomam/exhaustion-check"
 repository = "https://github.com/turbomam/exhaustion-check"
 
@@ -99,8 +99,9 @@
 
 [tool.black]
 line_length = 88
 include = '\.pyi?$'
 
 [tool.poetry.scripts]
 exhaustion-check = "exhaustion_check.exhaustion_check:validate_instance"
-pretty-sort-yaml = "exhaustion_check.pretty_sort_yaml:load_yaml_file"
+pretty-sort-yaml = "exhaustion_check.pretty_sort_yaml:load_yaml_file"
+get-first-of-first = "exhaustion_check.get_first_of_first:cli"
```

### Comparing `exhaustion_check-0.1.3/src/exhaustion_check/exhaustion_check.py` & `exhaustion_check-0.1.4/src/exhaustion_check/exhaustion_check.py`

 * *Files identical despite different names*

### Comparing `exhaustion_check-0.1.3/src/exhaustion_check/pretty_sort_yaml.py` & `exhaustion_check-0.1.4/src/exhaustion_check/pretty_sort_yaml.py`

 * *Files identical despite different names*

### Comparing `exhaustion_check-0.1.3/PKG-INFO` & `exhaustion_check-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exhaustion-check
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Home-page: https://github.com/turbomam/exhaustion-check
 License: MIT
 Author: Mark Andrew Miller
 Author-email: MAM@lbl.gov
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exhaustion-check Version: 0.1.3 Summary: Home-page:
+Metadata-Version: 2.1 Name: exhaustion-check Version: 0.1.4 Summary: Home-page:
 https://github.com/turbomam/exhaustion-check License: MIT Author: Mark Andrew
 Miller Author-email: MAM@lbl.gov Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: linkml (>=1.5.2,<2.0.0) Project-URL: Repository,
 https://github.com/turbomam/exhaustion-check Description-Content-Type: text/
```

