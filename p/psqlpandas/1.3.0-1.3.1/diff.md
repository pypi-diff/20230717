# Comparing `tmp/psqlpandas-1.3.0.tar.gz` & `tmp/psqlpandas-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psqlpandas-1.3.0.tar", max compression
+gzip compressed data, was "psqlpandas-1.3.1.tar", max compression
```

## Comparing `psqlpandas-1.3.0.tar` & `psqlpandas-1.3.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      900 2023-07-14 14:48:26.587735 psqlpandas-1.3.0/LICENSE
--rw-r--r--   0        0        0      199 2023-07-14 14:48:26.587735 psqlpandas-1.3.0/README.md
--rw-r--r--   0        0        0        0 2023-07-14 14:48:26.611734 psqlpandas-1.3.0/psqlpandas/__init__.py
--rw-r--r--   0        0        0       22 2023-07-14 14:48:26.588735 psqlpandas-1.3.0/psqlpandas/__version__.py
--rw-r--r--   0        0        0     8220 2023-07-14 14:48:26.588735 psqlpandas-1.3.0/psqlpandas/postgresql.py
--rw-r--r--   0        0        0       88 2023-07-14 14:48:26.588735 psqlpandas-1.3.0/psqlpandas/scripts/script.py
--rw-r--r--   0        0        0     3091 2023-07-14 14:48:26.588735 psqlpandas-1.3.0/psqlpandas/tables.py
--rw-r--r--   0        0        0     1886 2023-07-14 14:48:26.588735 psqlpandas-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 psqlpandas-1.3.0/setup.py
--rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 psqlpandas-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      900 2023-07-17 12:43:03.019858 psqlpandas-1.3.1/LICENSE
+-rw-r--r--   0        0        0      199 2023-07-17 12:43:03.019858 psqlpandas-1.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-17 12:43:03.044858 psqlpandas-1.3.1/psqlpandas/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-17 12:43:03.020858 psqlpandas-1.3.1/psqlpandas/__version__.py
+-rw-r--r--   0        0        0     8220 2023-07-17 12:43:03.020858 psqlpandas-1.3.1/psqlpandas/postgresql.py
+-rw-r--r--   0        0        0       88 2023-07-17 12:43:03.020858 psqlpandas-1.3.1/psqlpandas/scripts/script.py
+-rw-r--r--   0        0        0     3091 2023-07-17 12:43:03.020858 psqlpandas-1.3.1/psqlpandas/tables.py
+-rw-r--r--   0        0        0     2209 2023-07-17 12:43:03.020858 psqlpandas-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 psqlpandas-1.3.1/PKG-INFO
```

### Comparing `psqlpandas-1.3.0/LICENSE` & `psqlpandas-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `psqlpandas-1.3.0/psqlpandas/postgresql.py` & `psqlpandas-1.3.1/psqlpandas/postgresql.py`

 * *Files identical despite different names*

### Comparing `psqlpandas-1.3.0/psqlpandas/tables.py` & `psqlpandas-1.3.1/psqlpandas/tables.py`

 * *Files identical despite different names*

### Comparing `psqlpandas-1.3.0/pyproject.toml` & `psqlpandas-1.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psqlpandas"
-version = "1.3.0"
+version = "1.3.1"
 description = "Utilities to communicate with postgresql database through pandas dataframes."
 authors = ["Mattia Tantardini <mattia.tantardini@gmail.com>"]
 readme = "README.md"
 keywords = ["postgresql", "pandas"]
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Intended Audience :: Developers",
@@ -12,14 +12,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.0.0"
 psycopg2 = "^2.9.5"
 pandas = "^2.0.1"
+sqlalchemy = "^2.0.19"  # Needed to read_sql even though it is not explicitly used in the code
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20.0"
 commitizen = "^2.35.0"
 python-semantic-release = "^7.32.1"
 pytest = "^7.1.3"
 
@@ -49,14 +50,22 @@
     ["highlighted", "fg:#ff9d00 bold"],
     ["selected", "fg:#cc5454"],
     ["separator", "fg:#cc5454"],
     ["instruction", ""],
     ["text", ""],
     ["disabled", "fg:#858585 italic"]
 ]
+version = "1.3.1"
+version_files = [
+    "psqlpandas/__version__.py:__version__",
+    "pyproject.toml:version"
+]
+tag_format = "v$major.$minor.$patch"
+annotated_tag = true
+bump_message = "release $current_version -> $new_version"
 
 # --- Semantic release --- #
 [tool.semantic_release]
 # Reference: https://python-semantic-release.readthedocs.io/en/latest/index.html
 version_variable = [
     "psqlpandas/__version__.py:__version__",
     "pyproject.toml:version"
```

### Comparing `psqlpandas-1.3.0/PKG-INFO` & `psqlpandas-1.3.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: psqlpandas
-Version: 1.3.0
+Version: 1.3.1
 Summary: Utilities to communicate with postgresql database through pandas dataframes.
 Keywords: postgresql,pandas
 Author: Mattia Tantardini
 Author-email: mattia.tantardini@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: numpy (>=1.0.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
+Requires-Dist: sqlalchemy (>=2.0.19,<3.0.0)
 Description-Content-Type: text/markdown
 
 # psqlpandas
 Utilities to communicate with postgresql database through pandas dataframes.
 
 ## Installation
 ```
```

