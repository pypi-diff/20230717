# Comparing `tmp/godoo_cli-0.5.2.tar.gz` & `tmp/godoo_cli-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godoo_cli-0.5.2.tar", max compression
+gzip compressed data, was "godoo_cli-0.6.0.tar", max compression
```

## Comparing `godoo_cli-0.5.2.tar` & `godoo_cli-0.6.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     7633 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/LICENSE
--rw-r--r--   0        0        0     7297 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/README.md
--rw-r--r--   0        0        0     5004 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/pyproject.toml
--rw-r--r--   0        0        0       61 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/__init__.py
--rw-r--r--   0        0        0       88 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/__main__.py
--rw-r--r--   0        0        0     1963 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/cli.py
--rw-r--r--   0        0        0     5397 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/cli_common.py
--rw-r--r--   0        0        0      293 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/__init__.py
--rw-r--r--   0        0        0     5811 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/bootstrap.py
--rw-r--r--   0        0        0     1173 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/config.py
--rw-r--r--   0        0        0       28 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/db/__init__.py
--rw-r--r--   0        0        0      311 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/db/cli.py
--rw-r--r--   0        0        0     1801 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/db/connection.py
--rw-r--r--   0        0        0     1325 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/db/passwords.py
--rw-r--r--   0        0        0    10339 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/launch.py
--rw-r--r--   0        0        0      177 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/rpc/__init__.py
--rw-r--r--   0        0        0      897 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/rpc/cli.py
--rw-r--r--   0        0        0     1484 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/rpc/config_parameters.py
--rw-r--r--   0        0        0     2278 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/rpc/importer.py
--rw-r--r--   0        0        0     4828 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/commands/rpc/modules.py
--rw-r--r--   0        0        0     4000 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/commands/rpc/translations.py
--rw-r--r--   0        0        0     1619 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/commands/shell.py
--rw-r--r--   0        0        0     8544 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/commands/source_get.py
--rw-r--r--   0        0        0     4437 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/commands/test.py
--rw-r--r--   0        0        0      161 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/git/__init__.py
--rw-r--r--   0        0        0     1299 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/git/git_odoo.py
--rw-r--r--   0        0        0     3296 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/git/git_odoo_addons.py
--rw-r--r--   0        0        0     6460 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/git/git_repo.py
--rw-r--r--   0        0        0     4585 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/git/git_url.py
--rw-r--r--   0        0        0     1575 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/git/zip_download.py
--rw-r--r--   0        0        0       49 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/helpers/__init__.py
--rw-r--r--   0        0        0     2225 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/helpers/bootstrap.py
--rw-r--r--   0        0        0      386 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/helpers/cli.py
--rw-r--r--   0        0        0     8895 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/helpers/odoo_files.py
--rw-r--r--   0        0        0     3277 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/helpers/odoo_manifest.py
--rw-r--r--   0        0        0     2766 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/helpers/system.py
--rw-r--r--   0        0        0       22 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/version.py
--rw-r--r--   0        0        0     9317 1970-01-01 00:00:00.000000 godoo_cli-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     7633 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7297 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/README.md
+-rw-r--r--   0        0        0     5070 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/__init__.py
+-rw-r--r--   0        0        0       88 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/__main__.py
+-rw-r--r--   0        0        0     1963 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/cli.py
+-rw-r--r--   0        0        0     5397 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/cli_common.py
+-rw-r--r--   0        0        0      293 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/__init__.py
+-rw-r--r--   0        0        0     5811 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/bootstrap.py
+-rw-r--r--   0        0        0     1173 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/config.py
+-rw-r--r--   0        0        0       28 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/db/__init__.py
+-rw-r--r--   0        0        0      311 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/db/cli.py
+-rw-r--r--   0        0        0     1801 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/db/connection.py
+-rw-r--r--   0        0        0     1325 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/db/passwords.py
+-rw-r--r--   0        0        0    10339 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/launch.py
+-rw-r--r--   0        0        0      177 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/rpc/__init__.py
+-rw-r--r--   0        0        0      897 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/rpc/cli.py
+-rw-r--r--   0        0        0     1484 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/rpc/config_parameters.py
+-rw-r--r--   0        0        0     2278 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/rpc/importer.py
+-rw-r--r--   0        0        0     4828 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/rpc/modules.py
+-rw-r--r--   0        0        0     4000 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/rpc/translations.py
+-rw-r--r--   0        0        0     1619 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/shell.py
+-rw-r--r--   0        0        0     8544 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/source_get.py
+-rw-r--r--   0        0        0     4437 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/commands/test.py
+-rw-r--r--   0        0        0      161 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/git/__init__.py
+-rw-r--r--   0        0        0     2688 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/git/git_odoo.py
+-rw-r--r--   0        0        0     3296 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/git/git_odoo_addons.py
+-rw-r--r--   0        0        0     6460 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/git/git_repo.py
+-rw-r--r--   0        0        0     4585 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/git/git_url.py
+-rw-r--r--   0        0        0     1575 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/git/zip_download.py
+-rw-r--r--   0        0        0       49 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/helpers/__init__.py
+-rw-r--r--   0        0        0     2225 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/helpers/bootstrap.py
+-rw-r--r--   0        0        0      386 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/helpers/cli.py
+-rw-r--r--   0        0        0     8895 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/helpers/odoo_files.py
+-rw-r--r--   0        0        0     3277 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/helpers/odoo_manifest.py
+-rw-r--r--   0        0        0     2766 2023-07-17 10:33:31.700929 godoo_cli-0.6.0/src/godoo_cli/helpers/system.py
+-rw-r--r--   0        0        0       22 2023-07-17 10:33:31.704929 godoo_cli-0.6.0/src/godoo_cli/version.py
+-rw-r--r--   0        0        0     9387 1970-01-01 00:00:00.000000 godoo_cli-0.6.0/PKG-INFO
```

### Comparing `godoo_cli-0.5.2/LICENSE` & `godoo_cli-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/README.md` & `godoo_cli-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/pyproject.toml` & `godoo_cli-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gOdoo-cli"
-version = "0.5.2"
+version = "0.6.0"
 description = "Wrapper around Odoo-Bin with some convinience RPC functions."
 authors = ["Joshua Kreuder <Joshua_Kreuder@outlook.com>"]
 license = "LGPL-3"
 readme = "README.md"
 packages = [{include = "godoo_cli",  from = "src"}]
 repository = "https://github.com/OpenJKSoftware/gOdoo"
 keywords = ["odoo", "godoo","devcontainer"]
@@ -35,25 +35,27 @@
 py-spy = { version="^0.3.11", optional = true}
 rope = { version="^0.23.0", optional = true}
 flake8 = { version="^5.0.4", optional = true}
 inotify = { version="^0.2.10",optional = true}
 mock = { version="^4.0.3", optional= true}
 pytest = { version="^7.2.1", optional= true}
 pytest-cov = {version="^4.0.0",optional=true}
+pydevd-odoo = { version="^1.2.1",optional=true}
 
 [tool.poetry.extras]
 devcontainer = [
     "ipdb",
     "debugpy",
     "pre-commit",
     "watchdog",
     "rope",
     "py-spy",
     "inotify",
     "mock",
+    "pydevd-odoo"
 ]
 codequality = [
     "pylint-odoo",
     "black",
     "isort",
     "flake8",
     "pytest",
```

### Comparing `godoo_cli-0.5.2/src/godoo_cli/cli.py` & `godoo_cli-0.6.0/src/godoo_cli/cli.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/cli_common.py` & `godoo_cli-0.6.0/src/godoo_cli/cli_common.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/commands/bootstrap.py` & `godoo_cli-0.6.0/src/godoo_cli/commands/bootstrap.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/commands/config.py` & `godoo_cli-0.6.0/src/godoo_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/commands/db/connection.py` & `godoo_cli-0.6.0/src/godoo_cli/commands/db/connection.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/commands/db/passwords.py` & `godoo_cli-0.6.0/src/godoo_cli/commands/db/passwords.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/commands/launch.py` & `godoo_cli-0.6.0/src/godoo_cli/commands/launch.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/commands/rpc/cli.py` & `godoo_cli-0.6.0/src/godoo_cli/commands/rpc/cli.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/commands/rpc/config_parameters.py` & `godoo_cli-0.6.0/src/godoo_cli/commands/rpc/config_parameters.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/commands/rpc/importer.py` & `godoo_cli-0.6.0/src/godoo_cli/commands/rpc/importer.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/commands/rpc/modules.py` & `godoo_cli-0.6.0/src/godoo_cli/commands/rpc/modules.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/commands/rpc/translations.py` & `godoo_cli-0.6.0/src/godoo_cli/commands/rpc/translations.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/commands/shell.py` & `godoo_cli-0.6.0/src/godoo_cli/commands/shell.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/commands/source_get.py` & `godoo_cli-0.6.0/src/godoo_cli/commands/source_get.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/commands/test.py` & `godoo_cli-0.6.0/src/godoo_cli/commands/test.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/git/git_odoo_addons.py` & `godoo_cli-0.6.0/src/godoo_cli/git/git_odoo_addons.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/git/git_repo.py` & `godoo_cli-0.6.0/src/godoo_cli/git/git_repo.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/git/git_url.py` & `godoo_cli-0.6.0/src/godoo_cli/git/git_url.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/git/zip_download.py` & `godoo_cli-0.6.0/src/godoo_cli/git/zip_download.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/helpers/bootstrap.py` & `godoo_cli-0.6.0/src/godoo_cli/helpers/bootstrap.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/helpers/odoo_files.py` & `godoo_cli-0.6.0/src/godoo_cli/helpers/odoo_files.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/helpers/odoo_manifest.py` & `godoo_cli-0.6.0/src/godoo_cli/helpers/odoo_manifest.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/src/godoo_cli/helpers/system.py` & `godoo_cli-0.6.0/src/godoo_cli/helpers/system.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.2/PKG-INFO` & `godoo_cli-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godoo-cli
-Version: 0.5.2
+Version: 0.6.0
 Summary: Wrapper around Odoo-Bin with some convinience RPC functions.
 Home-page: https://github.com/OpenJKSoftware/gOdoo
 License: LGPL-3
 Keywords: odoo,godoo,devcontainer
 Author: Joshua Kreuder
 Author-email: Joshua_Kreuder@outlook.com
 Requires-Python: >=3.8.1,<3.12
@@ -25,14 +25,15 @@
 Requires-Dist: isort (>=5.10.1,<6.0.0) ; extra == "codequality"
 Requires-Dist: mock (>=4.0.3,<5.0.0) ; extra == "devcontainer"
 Requires-Dist: openupgradelib (>=3.3.4,<4.0.0)
 Requires-Dist: passlib (>=1.7.3,<2.0.0)
 Requires-Dist: pre-commit (>=2.20.0,<3.0.0) ; extra == "devcontainer"
 Requires-Dist: psycopg2 (>=2.8.6,<3.0.0)
 Requires-Dist: py-spy (>=0.3.11,<0.4.0) ; extra == "devcontainer"
+Requires-Dist: pydevd-odoo (>=1.2.1,<2.0.0) ; extra == "devcontainer"
 Requires-Dist: pylint-odoo (>=8.0.16,<9.0.0) ; extra == "codequality"
 Requires-Dist: pytest (>=7.2.1,<8.0.0) ; extra == "codequality"
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0) ; extra == "codequality"
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: rope (>=0.23.0,<0.24.0) ; extra == "devcontainer"
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
 Requires-Dist: typer-common-functions (>=0.0.3,<0.0.4)
```

