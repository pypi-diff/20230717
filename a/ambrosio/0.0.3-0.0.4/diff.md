# Comparing `tmp/ambrosio-0.0.3.tar.gz` & `tmp/ambrosio-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambrosio-0.0.3.tar", max compression
+gzip compressed data, was "ambrosio-0.0.4.tar", max compression
```

## Comparing `ambrosio-0.0.3.tar` & `ambrosio-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1211 2023-07-01 06:56:26.474970 ambrosio-0.0.3/LICENSE
--rw-r--r--   0        0        0      447 2023-07-01 07:47:27.856863 ambrosio-0.0.3/README.md
--rw-r--r--   0        0        0     1052 2023-07-01 10:45:21.280733 ambrosio-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       24 2023-07-01 07:47:27.859411 ambrosio-0.0.3/src/ambrosio/__init__.py
--rw-r--r--   0        0        0       48 2023-07-01 07:47:27.861735 ambrosio-0.0.3/src/ambrosio/ui/__init__.py
--rw-r--r--   0        0        0       81 2023-07-01 07:47:27.862068 ambrosio-0.0.3/src/ambrosio/ui/cli/__init__.py
--rw-r--r--   0        0        0      633 2023-07-01 10:24:19.630149 ambrosio-0.0.3/src/ambrosio/ui/cli/main.py
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 ambrosio-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-01 06:56:26.474970 ambrosio-0.0.4/LICENSE
+-rw-r--r--   0        0        0      447 2023-07-01 07:47:27.856863 ambrosio-0.0.4/README.md
+-rw-r--r--   0        0        0     1051 2023-07-17 09:30:47.089602 ambrosio-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-07-01 07:47:27.859411 ambrosio-0.0.4/src/ambrosio/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-01 07:47:27.861735 ambrosio-0.0.4/src/ambrosio/ui/__init__.py
+-rw-r--r--   0        0        0       81 2023-07-01 07:47:27.862068 ambrosio-0.0.4/src/ambrosio/ui/cli/__init__.py
+-rw-r--r--   0        0        0      633 2023-07-01 10:24:19.630149 ambrosio-0.0.4/src/ambrosio/ui/cli/main.py
+-rw-r--r--   0        0        0     1083 1970-01-01 00:00:00.000000 ambrosio-0.0.4/PKG-INFO
```

### Comparing `ambrosio-0.0.3/LICENSE` & `ambrosio-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ambrosio-0.0.3/pyproject.toml` & `ambrosio-0.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.poetry]
 name = "ambrosio"
-version = "0.0.3"
+version = "0.0.4"
 description = "Ambrosio helps accomplish tasks in the command line."
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicence"
 readme = "README.md"
 packages = [{ include = "ambrosio", from = "src" }]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 awesome-slugify = "^1.6.5"
-toolcat = "^0.0.5"
+toolcat = "^0.0.6"
 typer = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
 bandit = { extras = ["toml"], version = "^1.7.5" }
 behave = "^1.2.6"
-black = "^23.3.0"
+black = "^23.7.0"
 coverage = "^7.2.7"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 nox = "^2023.4.22"
 pre-commit = "^3.3.3"
 pytest = "^7.4.0"
 pytest-bdd = "^6.1.1"
```

### Comparing `ambrosio-0.0.3/src/ambrosio/ui/cli/main.py` & `ambrosio-0.0.4/src/ambrosio/ui/cli/main.py`

 * *Files identical despite different names*

### Comparing `ambrosio-0.0.3/PKG-INFO` & `ambrosio-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ambrosio
-Version: 0.0.3
+Version: 0.0.4
 Summary: Ambrosio helps accomplish tasks in the command line.
 License: The Unlicence
 Author: Luís Miranda
 Author-email: luistm@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: awesome-slugify (>=1.6.5,<2.0.0)
-Requires-Dist: toolcat (>=0.0.5,<0.0.6)
+Requires-Dist: toolcat (>=0.0.6,<0.0.7)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Ambrosio
 
 Ambrosio helps accomplish tasks in the command line
```

