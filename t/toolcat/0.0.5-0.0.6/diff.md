# Comparing `tmp/toolcat-0.0.5.tar.gz` & `tmp/toolcat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolcat-0.0.5.tar", max compression
+gzip compressed data, was "toolcat-0.0.6.tar", max compression
```

## Comparing `toolcat-0.0.5.tar` & `toolcat-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1211 2023-06-03 18:15:32.691464 toolcat-0.0.5/LICENSE
--rw-r--r--   0        0        0      182 2023-06-03 20:00:15.609596 toolcat-0.0.5/README.md
--rw-r--r--   0        0        0     1086 2023-07-01 08:43:26.072517 toolcat-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       24 2023-06-03 18:15:32.694245 toolcat-0.0.5/src/toolcat/__init__.py
--rw-r--r--   0        0        0     2382 2023-06-03 23:01:48.937333 toolcat-0.0.5/src/toolcat/database.py
--rw-r--r--   0        0        0     1400 2023-06-03 23:01:51.316471 toolcat-0.0.5/src/toolcat/database_test.py
--rw-r--r--   0        0        0      831 2023-07-01 08:42:42.223538 toolcat-0.0.5/src/toolcat/project.py
--rw-r--r--   0        0        0     1096 2023-06-03 19:12:14.817042 toolcat-0.0.5/src/toolcat/projects_test.py
--rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 toolcat-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-06-03 18:15:32.691464 toolcat-0.0.6/LICENSE
+-rw-r--r--   0        0        0      182 2023-06-03 20:00:15.609596 toolcat-0.0.6/README.md
+-rw-r--r--   0        0        0     1085 2023-07-17 09:00:02.481521 toolcat-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-06-03 18:15:32.694245 toolcat-0.0.6/src/toolcat/__init__.py
+-rw-r--r--   0        0        0     2382 2023-06-03 23:01:48.937333 toolcat-0.0.6/src/toolcat/database.py
+-rw-r--r--   0        0        0     1400 2023-06-03 23:01:51.316471 toolcat-0.0.6/src/toolcat/database_test.py
+-rw-r--r--   0        0        0      831 2023-07-01 08:42:42.223538 toolcat-0.0.6/src/toolcat/project.py
+-rw-r--r--   0        0        0     1096 2023-06-03 19:12:14.817042 toolcat-0.0.6/src/toolcat/projects_test.py
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 toolcat-0.0.6/PKG-INFO
```

### Comparing `toolcat-0.0.5/LICENSE` & `toolcat-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `toolcat-0.0.5/pyproject.toml` & `toolcat-0.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,34 +12,34 @@
 [tool.mypy]
 ignore_missing_imports = true
 # https://stackoverflow.com/questions/62265366/does-mypy-only-type-check-a-function-if-it-declares-a-return-type
 check_untyped_defs = true
 
 [tool.poetry]
 name = "toolcat"
-version = "0.0.5"
+version = "0.0.6"
 description = "Essential Libraries and Tools for Streamlined Development"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicence"
 readme = "README.md"
 packages = [{ include = "toolcat", from = "src" }]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 toml = "^0.10.2"
-sqlalchemy = "^2.0.15"
+sqlalchemy = "^2.0.19"
 
 [tool.poetry.group.dev.dependencies]
 bandit = { extras = ["toml"], version = "^1.7.5" }
-black = "^23.3.0"
+black = "^23.7.0"
 coverage = "^7.2.7"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
-mypy = "^1.3.0"
+mypy = "^1.4.1"
 nox = "^2023.4.22"
-pre-commit = "^3.3.2"
-pytest = "^7.3.1"
+pre-commit = "^3.3.3"
+pytest = "^7.4.0"
 pytest-xdist = "^3.3.1"
 types-toml = "^0.10.8.6"
 
 [tool.pytest.ini_options]
 markers = ["integration: tags a test as integration tests"]
```

### Comparing `toolcat-0.0.5/src/toolcat/database.py` & `toolcat-0.0.6/src/toolcat/database.py`

 * *Files identical despite different names*

### Comparing `toolcat-0.0.5/src/toolcat/database_test.py` & `toolcat-0.0.6/src/toolcat/database_test.py`

 * *Files identical despite different names*

### Comparing `toolcat-0.0.5/src/toolcat/project.py` & `toolcat-0.0.6/src/toolcat/project.py`

 * *Files identical despite different names*

### Comparing `toolcat-0.0.5/src/toolcat/projects_test.py` & `toolcat-0.0.6/src/toolcat/projects_test.py`

 * *Files identical despite different names*

