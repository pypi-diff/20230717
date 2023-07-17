# Comparing `tmp/camminapy-1.1.5.tar.gz` & `tmp/camminapy-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camminapy-1.1.5.tar", max compression
+gzip compressed data, was "camminapy-1.1.6.tar", max compression
```

## Comparing `camminapy-1.1.5.tar` & `camminapy-1.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-05-25 18:22:20.279949 camminapy-1.1.5/LICENSE
--rw-r--r--   0        0        0      361 2023-05-26 10:37:06.478390 camminapy-1.1.5/README.md
--rw-r--r--   0        0        0      119 2023-05-26 10:37:06.478678 camminapy-1.1.5/camminapy/__init__.py
--rw-r--r--   0        0        0      343 2023-05-25 18:22:20.280553 camminapy-1.1.5/camminapy/data/__init__.py
--rw-r--r--   0        0        0     6597 2023-07-17 20:18:10.371016 camminapy-1.1.5/camminapy/data/resample.py
--rw-r--r--   0        0        0      163 2023-05-25 18:22:20.280877 camminapy-1.1.5/camminapy/plot/__init__.py
--rw-r--r--   0        0        0     1085 2023-05-25 18:22:20.280996 camminapy-1.1.5/camminapy/plot/altair_config.py
--rw-r--r--   0        0        0     6242 2023-05-25 18:43:33.297938 camminapy-1.1.5/camminapy/plot/altair_theme.py
--rw-r--r--   0        0        0     2633 2023-05-25 18:22:20.281263 camminapy-1.1.5/camminapy/plot/footer.py
--rw-r--r--   0        0        0        0 2023-05-25 18:22:20.281378 camminapy-1.1.5/camminapy/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-05-25 18:22:20.281505 camminapy-1.1.5/camminapy/utils/config.py
--rw-r--r--   0        0        0      734 2023-05-26 07:06:53.398496 camminapy-1.1.5/camminapy/utils/logger.py
--rw-r--r--   0        0        0     1141 2023-07-17 20:25:34.161860 camminapy-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 camminapy-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-25 18:22:20.279949 camminapy-1.1.6/LICENSE
+-rw-r--r--   0        0        0      361 2023-05-26 10:37:06.478390 camminapy-1.1.6/README.md
+-rw-r--r--   0        0        0      119 2023-05-26 10:37:06.478678 camminapy-1.1.6/camminapy/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-25 18:22:20.280553 camminapy-1.1.6/camminapy/data/__init__.py
+-rw-r--r--   0        0        0     6597 2023-07-17 20:18:10.371016 camminapy-1.1.6/camminapy/data/resample.py
+-rw-r--r--   0        0        0      163 2023-05-25 18:22:20.280877 camminapy-1.1.6/camminapy/plot/__init__.py
+-rw-r--r--   0        0        0     1085 2023-05-25 18:22:20.280996 camminapy-1.1.6/camminapy/plot/altair_config.py
+-rw-r--r--   0        0        0     6242 2023-05-25 18:43:33.297938 camminapy-1.1.6/camminapy/plot/altair_theme.py
+-rw-r--r--   0        0        0     2633 2023-05-25 18:22:20.281263 camminapy-1.1.6/camminapy/plot/footer.py
+-rw-r--r--   0        0        0        0 2023-05-25 18:22:20.281378 camminapy-1.1.6/camminapy/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-25 18:22:20.281505 camminapy-1.1.6/camminapy/utils/config.py
+-rw-r--r--   0        0        0      734 2023-05-26 07:06:53.398496 camminapy-1.1.6/camminapy/utils/logger.py
+-rw-r--r--   0        0        0     1141 2023-07-17 20:25:52.725473 camminapy-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 camminapy-1.1.6/PKG-INFO
```

### Comparing `camminapy-1.1.5/LICENSE` & `camminapy-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.5/camminapy/data/resample.py` & `camminapy-1.1.6/camminapy/data/resample.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.5/camminapy/plot/altair_config.py` & `camminapy-1.1.6/camminapy/plot/altair_config.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.5/camminapy/plot/altair_theme.py` & `camminapy-1.1.6/camminapy/plot/altair_theme.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.5/camminapy/plot/footer.py` & `camminapy-1.1.6/camminapy/plot/footer.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.5/camminapy/utils/config.py` & `camminapy-1.1.6/camminapy/utils/config.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.5/camminapy/utils/logger.py` & `camminapy-1.1.6/camminapy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.5/pyproject.toml` & `camminapy-1.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camminapy"
-version = "1.1.5"
+version = "1.1.6"
 description = "My personal code collection."
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 readme = "README.md"
 repository = "https://github.com/thomascamminady/camminapy"
 homepage = "https://thomascamminady.github.io/camminapy/camminapy.html"
 
 [tool.poetry.dependencies]
```

### Comparing `camminapy-1.1.5/PKG-INFO` & `camminapy-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camminapy
-Version: 1.1.5
+Version: 1.1.6
 Summary: My personal code collection.
 Home-page: https://thomascamminady.github.io/camminapy/camminapy.html
 Author: Thomas Camminady
 Author-email: 0milieux_member@icloud.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

