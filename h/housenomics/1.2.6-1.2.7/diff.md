# Comparing `tmp/housenomics-1.2.6.tar.gz` & `tmp/housenomics-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "housenomics-1.2.6.tar", max compression
+gzip compressed data, was "housenomics-1.2.7.tar", max compression
```

## Comparing `housenomics-1.2.6.tar` & `housenomics-1.2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1211 2023-04-05 20:39:03.022505 housenomics-1.2.6/LICENSE
--rw-r--r--   0        0        0     1331 2023-07-01 10:55:14.210014 housenomics-1.2.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-05 20:39:03.032709 housenomics-1.2.6/src/housenomics/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 20:39:03.033041 housenomics-1.2.6/src/housenomics/application/__init__.py
--rw-r--r--   0        0        0      787 2023-04-06 08:51:23.764662 housenomics-1.2.6/src/housenomics/application/import_transactions.py
--rw-r--r--   0        0        0      572 2023-05-28 21:46:38.921062 housenomics-1.2.6/src/housenomics/application/import_transactions_test.py
--rw-r--r--   0        0        0      758 2023-04-14 20:32:53.007626 housenomics-1.2.6/src/housenomics/application/repositories/transactions.py
--rw-r--r--   0        0        0     1803 2023-04-05 20:39:03.034847 housenomics-1.2.6/src/housenomics/application/views/transactions.py
--rw-r--r--   0        0        0     4981 2023-06-03 23:16:04.690593 housenomics-1.2.6/src/housenomics/application/views/transactions_test.py
--rw-r--r--   0        0        0     2983 2023-04-07 14:24:59.019481 housenomics-1.2.6/src/housenomics/infrastructure/gateway_cgd_file.py
--rw-r--r--   0        0        0     2045 2023-04-14 20:32:53.007236 housenomics-1.2.6/src/housenomics/infrastructure/gateway_cgd_file_test.py
--rw-r--r--   0        0        0      494 2023-06-03 23:13:55.270918 housenomics-1.2.6/src/housenomics/transaction.py
--rw-r--r--   0        0        0        0 2023-04-05 20:39:03.038982 housenomics-1.2.6/src/housenomics/ui/cli/__init__.py
--rw-r--r--   0        0        0     2451 2023-06-03 23:16:04.686939 housenomics-1.2.6/src/housenomics/ui/cli/main.py
--rw-r--r--   0        0        0      670 2023-06-03 23:16:04.691822 housenomics-1.2.6/src/housenomics/ui/cli/report.py
--rw-r--r--   0        0        0      323 2023-04-05 20:39:03.039911 housenomics-1.2.6/src/housenomics/ui/cli/version.py
--rw-r--r--   0        0        0      479 2023-04-05 20:39:03.041120 housenomics-1.2.6/src/toolbox/cli.py
--rw-r--r--   0        0        0       83 2023-06-03 23:15:36.706123 housenomics-1.2.6/src/toolbox/database.py
--rw-r--r--   0        0        0       64 2023-04-05 20:39:03.042194 housenomics-1.2.6/src/toolbox/views.py
--rw-r--r--   0        0        0      143 2023-04-05 20:39:03.042641 housenomics-1.2.6/src/toolbox/views_test.py
--rw-r--r--   0        0        0      632 1970-01-01 00:00:00.000000 housenomics-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-05 20:39:03.022505 housenomics-1.2.7/LICENSE
+-rw-r--r--   0        0        0     1331 2023-07-17 09:38:24.086497 housenomics-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-05 20:39:03.032709 housenomics-1.2.7/src/housenomics/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-05 20:39:03.033041 housenomics-1.2.7/src/housenomics/application/__init__.py
+-rw-r--r--   0        0        0      787 2023-04-06 08:51:23.764662 housenomics-1.2.7/src/housenomics/application/import_transactions.py
+-rw-r--r--   0        0        0      572 2023-05-28 21:46:38.921062 housenomics-1.2.7/src/housenomics/application/import_transactions_test.py
+-rw-r--r--   0        0        0      758 2023-04-14 20:32:53.007626 housenomics-1.2.7/src/housenomics/application/repositories/transactions.py
+-rw-r--r--   0        0        0     1803 2023-04-05 20:39:03.034847 housenomics-1.2.7/src/housenomics/application/views/transactions.py
+-rw-r--r--   0        0        0     4981 2023-06-03 23:16:04.690593 housenomics-1.2.7/src/housenomics/application/views/transactions_test.py
+-rw-r--r--   0        0        0     2983 2023-04-07 14:24:59.019481 housenomics-1.2.7/src/housenomics/infrastructure/gateway_cgd_file.py
+-rw-r--r--   0        0        0     2045 2023-04-14 20:32:53.007236 housenomics-1.2.7/src/housenomics/infrastructure/gateway_cgd_file_test.py
+-rw-r--r--   0        0        0      494 2023-06-03 23:13:55.270918 housenomics-1.2.7/src/housenomics/transaction.py
+-rw-r--r--   0        0        0        0 2023-04-05 20:39:03.038982 housenomics-1.2.7/src/housenomics/ui/cli/__init__.py
+-rw-r--r--   0        0        0     2451 2023-06-03 23:16:04.686939 housenomics-1.2.7/src/housenomics/ui/cli/main.py
+-rw-r--r--   0        0        0      670 2023-06-03 23:16:04.691822 housenomics-1.2.7/src/housenomics/ui/cli/report.py
+-rw-r--r--   0        0        0      323 2023-04-05 20:39:03.039911 housenomics-1.2.7/src/housenomics/ui/cli/version.py
+-rw-r--r--   0        0        0      479 2023-04-05 20:39:03.041120 housenomics-1.2.7/src/toolbox/cli.py
+-rw-r--r--   0        0        0       83 2023-06-03 23:15:36.706123 housenomics-1.2.7/src/toolbox/database.py
+-rw-r--r--   0        0        0       64 2023-04-05 20:39:03.042194 housenomics-1.2.7/src/toolbox/views.py
+-rw-r--r--   0        0        0      143 2023-04-05 20:39:03.042641 housenomics-1.2.7/src/toolbox/views_test.py
+-rw-r--r--   0        0        0      632 1970-01-01 00:00:00.000000 housenomics-1.2.7/PKG-INFO
```

### Comparing `housenomics-1.2.6/LICENSE` & `housenomics-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `housenomics-1.2.6/pyproject.toml` & `housenomics-1.2.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
 exclude_dirs = ["tests", "features"]
 
 [tool.poetry]
 name = "housenomics"
-version = "1.2.6"
+version = "1.2.7"
 description = "Manage your personal finances"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "MIT"
 
 [[tool.poetry.packages]]
 include = "toolbox"
 from = "src"
@@ -34,17 +34,17 @@
 [tool.poetry.scripts]
 housenomics = "housenomics.ui.cli.main:housenomics_cli.app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pendulum = "^2.1.2"
 rich = "^13.4.2"
-sqlalchemy = "^2.0.17"
+sqlalchemy = "^2.0.19"
 toml = "^0.10.2"
-toolcat = "^0.0.5"
+toolcat = "^0.0.6"
 typer = "^0.9.0"
 
 [tool.pytest.ini_options]
 markers = ["integration: tags a test as integration tests"]
 
 [tool.poetry.dev-dependencies.bandit]
 extras = ["toml"]
```

### Comparing `housenomics-1.2.6/src/housenomics/application/import_transactions.py` & `housenomics-1.2.7/src/housenomics/application/import_transactions.py`

 * *Files identical despite different names*

### Comparing `housenomics-1.2.6/src/housenomics/application/import_transactions_test.py` & `housenomics-1.2.7/src/housenomics/application/import_transactions_test.py`

 * *Files identical despite different names*

### Comparing `housenomics-1.2.6/src/housenomics/application/repositories/transactions.py` & `housenomics-1.2.7/src/housenomics/application/repositories/transactions.py`

 * *Files identical despite different names*

### Comparing `housenomics-1.2.6/src/housenomics/application/views/transactions.py` & `housenomics-1.2.7/src/housenomics/application/views/transactions.py`

 * *Files identical despite different names*

### Comparing `housenomics-1.2.6/src/housenomics/application/views/transactions_test.py` & `housenomics-1.2.7/src/housenomics/application/views/transactions_test.py`

 * *Files identical despite different names*

### Comparing `housenomics-1.2.6/src/housenomics/infrastructure/gateway_cgd_file.py` & `housenomics-1.2.7/src/housenomics/infrastructure/gateway_cgd_file.py`

 * *Files identical despite different names*

### Comparing `housenomics-1.2.6/src/housenomics/infrastructure/gateway_cgd_file_test.py` & `housenomics-1.2.7/src/housenomics/infrastructure/gateway_cgd_file_test.py`

 * *Files identical despite different names*

### Comparing `housenomics-1.2.6/src/housenomics/ui/cli/main.py` & `housenomics-1.2.7/src/housenomics/ui/cli/main.py`

 * *Files identical despite different names*

### Comparing `housenomics-1.2.6/src/housenomics/ui/cli/report.py` & `housenomics-1.2.7/src/housenomics/ui/cli/report.py`

 * *Files identical despite different names*

### Comparing `housenomics-1.2.6/PKG-INFO` & `housenomics-1.2.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: housenomics
-Version: 1.2.6
+Version: 1.2.7
 Summary: Manage your personal finances
 License: MIT
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
-Requires-Dist: sqlalchemy (>=2.0.17,<3.0.0)
+Requires-Dist: sqlalchemy (>=2.0.19,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: toolcat (>=0.0.5,<0.0.6)
+Requires-Dist: toolcat (>=0.0.6,<0.0.7)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
```

