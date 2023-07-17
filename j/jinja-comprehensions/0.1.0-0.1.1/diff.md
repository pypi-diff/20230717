# Comparing `tmp/jinja_comprehensions-0.1.0.tar.gz` & `tmp/jinja_comprehensions-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja_comprehensions-0.1.0.tar", max compression
+gzip compressed data, was "jinja_comprehensions-0.1.1.tar", max compression
```

## Comparing `jinja_comprehensions-0.1.0.tar` & `jinja_comprehensions-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      443 2023-07-17 07:19:16.262588 jinja_comprehensions-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1067 2023-07-17 05:22:37.767004 jinja_comprehensions-0.1.0/LICENSE
--rw-r--r--   0        0        0     1694 2023-07-17 07:10:13.527721 jinja_comprehensions-0.1.0/README.md
--rw-r--r--   0        0        0      200 2023-07-17 06:08:25.029318 jinja_comprehensions-0.1.0/jinja_comprehensions/__init__.py
--rw-r--r--   0        0        0     4260 2023-07-17 06:02:53.730766 jinja_comprehensions-0.1.0/jinja_comprehensions/compiler.py
--rw-r--r--   0        0        0      493 2023-07-17 06:08:25.013318 jinja_comprehensions-0.1.0/jinja_comprehensions/environment.py
--rw-r--r--   0        0        0     5126 2023-07-17 06:08:25.025318 jinja_comprehensions-0.1.0/jinja_comprehensions/nativetypes.py
--rw-r--r--   0        0        0     5459 2023-07-17 05:55:27.073928 jinja_comprehensions-0.1.0/jinja_comprehensions/nodes.py
--rw-r--r--   0        0        0     8131 2023-07-17 06:49:03.849863 jinja_comprehensions-0.1.0/jinja_comprehensions/parser.py
--rw-r--r--   0        0        0      544 2023-07-17 06:00:18.239690 jinja_comprehensions-0.1.0/jinja_comprehensions/runtime.py
--rw-r--r--   0        0        0     1942 2023-07-03 18:12:07.917024 jinja_comprehensions-0.1.0/jinja_comprehensions/util.py
--rw-r--r--   0        0        0     2274 2023-07-17 06:04:43.652940 jinja_comprehensions-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-17 05:22:37.767004 jinja_comprehensions-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1412 2023-07-17 06:41:58.397284 jinja_comprehensions-0.1.0/tests/base.py
--rw-r--r--   0        0        0     1925 2023-07-17 06:50:02.595096 jinja_comprehensions-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1955 2023-07-17 06:21:43.805199 jinja_comprehensions-0.1.0/tests/test_collections.py
--rw-r--r--   0        0        0     2378 2023-07-17 06:21:04.256413 jinja_comprehensions-0.1.0/tests/test_comprehensions.py
--rw-r--r--   0        0        0     2749 1970-01-01 00:00:00.000000 jinja_comprehensions-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      531 2023-07-17 07:28:00.585271 jinja_comprehensions-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1067 2023-07-17 05:22:37.767004 jinja_comprehensions-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1781 2023-07-17 07:26:34.291514 jinja_comprehensions-0.1.1/README.md
+-rw-r--r--   0        0        0      200 2023-07-17 06:08:25.029318 jinja_comprehensions-0.1.1/jinja_comprehensions/__init__.py
+-rw-r--r--   0        0        0     4260 2023-07-17 06:02:53.730766 jinja_comprehensions-0.1.1/jinja_comprehensions/compiler.py
+-rw-r--r--   0        0        0      493 2023-07-17 06:08:25.013318 jinja_comprehensions-0.1.1/jinja_comprehensions/environment.py
+-rw-r--r--   0        0        0     5126 2023-07-17 06:08:25.025318 jinja_comprehensions-0.1.1/jinja_comprehensions/nativetypes.py
+-rw-r--r--   0        0        0     5459 2023-07-17 05:55:27.073928 jinja_comprehensions-0.1.1/jinja_comprehensions/nodes.py
+-rw-r--r--   0        0        0     8131 2023-07-17 06:49:03.849863 jinja_comprehensions-0.1.1/jinja_comprehensions/parser.py
+-rw-r--r--   0        0        0      544 2023-07-17 06:00:18.239690 jinja_comprehensions-0.1.1/jinja_comprehensions/runtime.py
+-rw-r--r--   0        0        0     1942 2023-07-03 18:12:07.917024 jinja_comprehensions-0.1.1/jinja_comprehensions/util.py
+-rw-r--r--   0        0        0     2274 2023-07-17 07:28:00.317266 jinja_comprehensions-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-17 05:22:37.767004 jinja_comprehensions-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1412 2023-07-17 06:41:58.397284 jinja_comprehensions-0.1.1/tests/base.py
+-rw-r--r--   0        0        0     1925 2023-07-17 06:50:02.595096 jinja_comprehensions-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     1955 2023-07-17 06:21:43.805199 jinja_comprehensions-0.1.1/tests/test_collections.py
+-rw-r--r--   0        0        0     2378 2023-07-17 06:21:04.256413 jinja_comprehensions-0.1.1/tests/test_comprehensions.py
+-rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 jinja_comprehensions-0.1.1/PKG-INFO
```

### Comparing `jinja_comprehensions-0.1.0/LICENSE` & `jinja_comprehensions-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja_comprehensions-0.1.0/README.md` & `jinja_comprehensions-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 # jinja-comprehensions
 Jinja2 environments providing support for list/dict comprehensions, set literals/comprehensions, generator expressions, and list/dict spreading.
 
+
+### Set literals
 ```jinja
 {{ {'set', 'set', 'literal', 'literal'} }}
 ```
 ```
 {'literal', 'set'}
 ```
 
+### Comprehensions
 ```jinja
 list: {{ [n // 2 for n in range(10)] }}
 set:  {{ {n // 2 for n in range(10)} }}
 dict: {{ {n: n // 2 for n in range(10)} }}
 ```
 ```
 list: [0, 0, 1, 1, 2, 2, 3, 3, 4, 4]
 set:  {0, 1, 2, 3, 4}
 dict: {0: 0, 1: 0, 2: 1, 3: 1, 4: 2, 5: 2, 6: 3, 7: 3, 8: 4, 9: 4}
 ```
 
+### Generator expressions
 ```jinja
 {{ (n // 2 for n in range(10)) | join(', ') }}
 ```
 ```
 0, 0, 1, 1, 2, 2, 3, 3, 4, 4
 ```
 
+### List/dict spreading
 ```jinja
 {% set stuff = {'b': 98, 'c': 99, 'd': 100} -%}
 {{ {'a': 97, **stuff, 'e': 101} }}
 {{ [97, *stuff.values(), 101] }}
 ```
 ```
 {'a': 97, 'b': 98, 'c': 99, 'd': 100, 'e': 101}
```

### Comparing `jinja_comprehensions-0.1.0/jinja_comprehensions/compiler.py` & `jinja_comprehensions-0.1.1/jinja_comprehensions/compiler.py`

 * *Files identical despite different names*

### Comparing `jinja_comprehensions-0.1.0/jinja_comprehensions/nativetypes.py` & `jinja_comprehensions-0.1.1/jinja_comprehensions/nativetypes.py`

 * *Files identical despite different names*

### Comparing `jinja_comprehensions-0.1.0/jinja_comprehensions/nodes.py` & `jinja_comprehensions-0.1.1/jinja_comprehensions/nodes.py`

 * *Files identical despite different names*

### Comparing `jinja_comprehensions-0.1.0/jinja_comprehensions/parser.py` & `jinja_comprehensions-0.1.1/jinja_comprehensions/parser.py`

 * *Files identical despite different names*

### Comparing `jinja_comprehensions-0.1.0/jinja_comprehensions/runtime.py` & `jinja_comprehensions-0.1.1/jinja_comprehensions/runtime.py`

 * *Files identical despite different names*

### Comparing `jinja_comprehensions-0.1.0/jinja_comprehensions/util.py` & `jinja_comprehensions-0.1.1/jinja_comprehensions/util.py`

 * *Files identical despite different names*

### Comparing `jinja_comprehensions-0.1.0/pyproject.toml` & `jinja_comprehensions-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jinja-comprehensions"
-version = "0.1.0"
+version = "0.1.1"
 description = "Jinja2 environment supporting Python comprehensions"
 authors = ["Zach Kanzler <zach@rewst.io>"]
 repository = "https://github.com/RewstApp/jinja-comprehensions"
 homepage = "https://github.com/RewstApp/jinja-comprehensions"
 license = "MIT"
 readme = "README.md"
 packages = [
```

### Comparing `jinja_comprehensions-0.1.0/tests/base.py` & `jinja_comprehensions-0.1.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `jinja_comprehensions-0.1.0/tests/conftest.py` & `jinja_comprehensions-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jinja_comprehensions-0.1.0/tests/test_collections.py` & `jinja_comprehensions-0.1.1/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `jinja_comprehensions-0.1.0/tests/test_comprehensions.py` & `jinja_comprehensions-0.1.1/tests/test_comprehensions.py`

 * *Files identical despite different names*

### Comparing `jinja_comprehensions-0.1.0/PKG-INFO` & `jinja_comprehensions-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinja-comprehensions
-Version: 0.1.0
+Version: 0.1.1
 Summary: Jinja2 environment supporting Python comprehensions
 Home-page: https://github.com/RewstApp/jinja-comprehensions
 License: MIT
 Author: Zach Kanzler
 Author-email: zach@rewst.io
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -23,39 +23,44 @@
 Requires-Dist: asyncstdlib (>=3.10.8,<4.0.0)
 Project-URL: Repository, https://github.com/RewstApp/jinja-comprehensions
 Description-Content-Type: text/markdown
 
 # jinja-comprehensions
 Jinja2 environments providing support for list/dict comprehensions, set literals/comprehensions, generator expressions, and list/dict spreading.
 
+
+### Set literals
 ```jinja
 {{ {'set', 'set', 'literal', 'literal'} }}
 ```
 ```
 {'literal', 'set'}
 ```
 
+### Comprehensions
 ```jinja
 list: {{ [n // 2 for n in range(10)] }}
 set:  {{ {n // 2 for n in range(10)} }}
 dict: {{ {n: n // 2 for n in range(10)} }}
 ```
 ```
 list: [0, 0, 1, 1, 2, 2, 3, 3, 4, 4]
 set:  {0, 1, 2, 3, 4}
 dict: {0: 0, 1: 0, 2: 1, 3: 1, 4: 2, 5: 2, 6: 3, 7: 3, 8: 4, 9: 4}
 ```
 
+### Generator expressions
 ```jinja
 {{ (n // 2 for n in range(10)) | join(', ') }}
 ```
 ```
 0, 0, 1, 1, 2, 2, 3, 3, 4, 4
 ```
 
+### List/dict spreading
 ```jinja
 {% set stuff = {'b': 98, 'c': 99, 'd': 100} -%}
 {{ {'a': 97, **stuff, 'e': 101} }}
 {{ [97, *stuff.values(), 101] }}
 ```
 ```
 {'a': 97, 'b': 98, 'c': 99, 'd': 100, 'e': 101}
```

