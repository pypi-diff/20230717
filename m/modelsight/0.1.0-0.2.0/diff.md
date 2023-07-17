# Comparing `tmp/modelsight-0.1.0.tar.gz` & `tmp/modelsight-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelsight-0.1.0.tar", max compression
+gzip compressed data, was "modelsight-0.2.0.tar", max compression
```

## Comparing `modelsight-0.1.0.tar` & `modelsight-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rwxr-xr-x   0        0        0    35096 2023-06-20 15:21:00.584313 modelsight-0.1.0/LICENSE
--rw-r--r--   0        0        0     1839 2023-06-21 12:50:47.492956 modelsight-0.1.0/README.md
--rw-r--r--   0        0        0     1039 2023-06-23 10:23:01.009791 modelsight-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       43 2023-06-21 15:23:01.579723 modelsight-0.1.0/src/modelsight/.gitignore
--rw-r--r--   0        0        0      190 2023-06-21 15:26:39.332847 modelsight-0.1.0/src/modelsight/__init__.py
--rw-r--r--   0        0        0      370 2023-06-21 14:52:56.919136 modelsight-0.1.0/src/modelsight/_typing.py
--rw-r--r--   0        0        0      107 2023-06-21 15:00:47.791553 modelsight-0.1.0/src/modelsight/calibration/__init__.py
--rw-r--r--   0        0        0     6700 2023-06-21 14:59:06.524371 modelsight-0.1.0/src/modelsight/calibration/calib.py
--rw-r--r--   0        0        0      367 2023-06-21 15:24:16.582369 modelsight-0.1.0/src/modelsight/config.py
--rw-r--r--   0        0        0       19 2023-06-21 15:24:14.580553 modelsight-0.1.0/src/modelsight/settings.toml
--rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 modelsight-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0    35096 2023-06-20 15:21:00.584313 modelsight-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1346 2023-07-17 09:05:59.204004 modelsight-0.2.0/README.md
+-rw-r--r--   0        0        0     1062 2023-07-17 09:39:24.410524 modelsight-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-06-21 15:23:01.579723 modelsight-0.2.0/src/modelsight/.gitignore
+-rw-r--r--   0        0        0      190 2023-06-21 15:26:39.332847 modelsight-0.2.0/src/modelsight/__init__.py
+-rw-r--r--   0        0        0     1245 2023-07-16 21:12:07.850626 modelsight-0.2.0/src/modelsight/_typing.py
+-rw-r--r--   0        0        0      107 2023-06-21 15:00:47.791553 modelsight-0.2.0/src/modelsight/calibration/__init__.py
+-rw-r--r--   0        0        0     6700 2023-06-21 14:59:06.524371 modelsight-0.2.0/src/modelsight/calibration/calib.py
+-rw-r--r--   0        0        0      367 2023-06-21 15:24:16.582369 modelsight-0.2.0/src/modelsight/config.py
+-rw-r--r--   0        0        0       96 2023-07-16 20:26:13.479788 modelsight-0.2.0/src/modelsight/curves/__init__.py
+-rw-r--r--   0        0        0     7268 2023-07-16 21:43:10.127090 modelsight-0.2.0/src/modelsight/curves/roc.py
+-rw-r--r--   0        0        0       19 2023-07-16 20:51:42.241672 modelsight-0.2.0/src/modelsight/settings.toml
+-rw-r--r--   0        0        0     2224 1970-01-01 00:00:00.000000 modelsight-0.2.0/PKG-INFO
```

### Comparing `modelsight-0.1.0/LICENSE` & `modelsight-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modelsight-0.1.0/pyproject.toml` & `modelsight-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelsight"
-version = "0.1.0"
+version = "0.2.0"
 description = "Better insights into Machine Learning models performance"
 authors = ["Francesco Pisu"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules"
@@ -34,8 +34,9 @@
 sphinx-rtd-theme = "^1.2.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
-version_variable = "pyproject.toml:version"
+version_variable = "pyproject.toml:version"
+version_source = "tag"
```

### Comparing `modelsight-0.1.0/src/modelsight/calibration/calib.py` & `modelsight-0.2.0/src/modelsight/calibration/calib.py`

 * *Files identical despite different names*

