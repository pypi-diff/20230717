# Comparing `tmp/camminapy-1.1.3.tar.gz` & `tmp/camminapy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camminapy-1.1.3.tar", max compression
+gzip compressed data, was "camminapy-1.1.4.tar", max compression
```

## Comparing `camminapy-1.1.3.tar` & `camminapy-1.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-05-25 18:22:20.279949 camminapy-1.1.3/LICENSE
--rw-r--r--   0        0        0      361 2023-05-26 10:37:06.478390 camminapy-1.1.3/README.md
--rw-r--r--   0        0        0      119 2023-05-26 10:37:06.478678 camminapy-1.1.3/camminapy/__init__.py
--rw-r--r--   0        0        0      343 2023-05-25 18:22:20.280553 camminapy-1.1.3/camminapy/data/__init__.py
--rw-r--r--   0        0        0     6597 2023-07-17 20:18:10.371016 camminapy-1.1.3/camminapy/data/resample.py
--rw-r--r--   0        0        0      163 2023-05-25 18:22:20.280877 camminapy-1.1.3/camminapy/plot/__init__.py
--rw-r--r--   0        0        0     1085 2023-05-25 18:22:20.280996 camminapy-1.1.3/camminapy/plot/altair_config.py
--rw-r--r--   0        0        0     6242 2023-05-25 18:43:33.297938 camminapy-1.1.3/camminapy/plot/altair_theme.py
--rw-r--r--   0        0        0     2633 2023-05-25 18:22:20.281263 camminapy-1.1.3/camminapy/plot/footer.py
--rw-r--r--   0        0        0        0 2023-05-25 18:22:20.281378 camminapy-1.1.3/camminapy/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-05-25 18:22:20.281505 camminapy-1.1.3/camminapy/utils/config.py
--rw-r--r--   0        0        0      734 2023-05-26 07:06:53.398496 camminapy-1.1.3/camminapy/utils/logger.py
--rw-r--r--   0        0        0     1138 2023-07-17 20:18:36.822958 camminapy-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 camminapy-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-25 18:22:20.279949 camminapy-1.1.4/LICENSE
+-rw-r--r--   0        0        0      361 2023-05-26 10:37:06.478390 camminapy-1.1.4/README.md
+-rw-r--r--   0        0        0      119 2023-05-26 10:37:06.478678 camminapy-1.1.4/camminapy/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-25 18:22:20.280553 camminapy-1.1.4/camminapy/data/__init__.py
+-rw-r--r--   0        0        0     6597 2023-07-17 20:18:10.371016 camminapy-1.1.4/camminapy/data/resample.py
+-rw-r--r--   0        0        0      163 2023-05-25 18:22:20.280877 camminapy-1.1.4/camminapy/plot/__init__.py
+-rw-r--r--   0        0        0     1085 2023-05-25 18:22:20.280996 camminapy-1.1.4/camminapy/plot/altair_config.py
+-rw-r--r--   0        0        0     6242 2023-05-25 18:43:33.297938 camminapy-1.1.4/camminapy/plot/altair_theme.py
+-rw-r--r--   0        0        0     2633 2023-05-25 18:22:20.281263 camminapy-1.1.4/camminapy/plot/footer.py
+-rw-r--r--   0        0        0        0 2023-05-25 18:22:20.281378 camminapy-1.1.4/camminapy/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-25 18:22:20.281505 camminapy-1.1.4/camminapy/utils/config.py
+-rw-r--r--   0        0        0      734 2023-05-26 07:06:53.398496 camminapy-1.1.4/camminapy/utils/logger.py
+-rw-r--r--   0        0        0     1137 2023-07-17 20:19:58.069606 camminapy-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1201 1970-01-01 00:00:00.000000 camminapy-1.1.4/PKG-INFO
```

### Comparing `camminapy-1.1.3/LICENSE` & `camminapy-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.3/camminapy/data/resample.py` & `camminapy-1.1.4/camminapy/data/resample.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.3/camminapy/plot/altair_config.py` & `camminapy-1.1.4/camminapy/plot/altair_config.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.3/camminapy/plot/altair_theme.py` & `camminapy-1.1.4/camminapy/plot/altair_theme.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.3/camminapy/plot/footer.py` & `camminapy-1.1.4/camminapy/plot/footer.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.3/camminapy/utils/config.py` & `camminapy-1.1.4/camminapy/utils/config.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.3/camminapy/utils/logger.py` & `camminapy-1.1.4/camminapy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.3/pyproject.toml` & `camminapy-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "camminapy"
-version = "1.1.3"
+version = "1.1.4"
 description = "My personal code collection."
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 readme = "README.md"
 repository = "https://github.com/thomascamminady/camminapy"
 homepage = "https://thomascamminady.github.io/camminapy/camminapy.html"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 altair = "^5.0.0"
 gitpython = "^3.1.31"
-polars = ">=0.17.15"
+polars = ">=0.18.0"
 pyarrow = "^12.0.0"
 rich = "^13.3.5"
 toolz = "^0.12.0"
 pdoc = "^13.1.1"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.0.1"
```

### Comparing `camminapy-1.1.3/PKG-INFO` & `camminapy-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: camminapy
-Version: 1.1.3
+Version: 1.1.4
 Summary: My personal code collection.
 Home-page: https://thomascamminady.github.io/camminapy/camminapy.html
 Author: Thomas Camminady
 Author-email: 0milieux_member@icloud.com
 Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: altair (>=5.0.0,<6.0.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: pdoc (>=13.1.1,<14.0.0)
-Requires-Dist: polars (>=0.17.15)
+Requires-Dist: polars (>=0.18.0)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: toolz (>=0.12.0,<0.13.0)
 Project-URL: Repository, https://github.com/thomascamminady/camminapy
 Description-Content-Type: text/markdown
 
 My personal code collection.
```

