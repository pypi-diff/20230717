# Comparing `tmp/autohooks_plugin_black-23.4.0.tar.gz` & `tmp/autohooks_plugin_black-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autohooks_plugin_black-23.4.0.tar", max compression
+gzip compressed data, was "autohooks_plugin_black-23.7.0.tar", max compression
```

## Comparing `autohooks_plugin_black-23.4.0.tar` & `autohooks_plugin_black-23.7.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-04-20 08:00:09.716838 autohooks_plugin_black-23.4.0/LICENSE
--rw-r--r--   0        0        0     2368 2023-04-20 08:00:09.716838 autohooks_plugin_black-23.4.0/README.md
--rw-r--r--   0        0        0      751 2023-04-20 08:00:09.716838 autohooks_plugin_black-23.4.0/autohooks/plugins/black/__init__.py
--rw-r--r--   0        0        0      103 2023-04-20 08:00:09.716838 autohooks_plugin_black-23.4.0/autohooks/plugins/black/__version__.py
--rw-r--r--   0        0        0     3357 2023-04-20 08:00:09.716838 autohooks_plugin_black-23.4.0/autohooks/plugins/black/black.py
--rw-r--r--   0        0        0    62339 2023-04-20 08:00:09.716838 autohooks_plugin_black-23.4.0/poetry.lock
--rw-r--r--   0        0        0       31 2023-04-20 08:00:09.716838 autohooks_plugin_black-23.4.0/poetry.toml
--rw-r--r--   0        0        0     2054 2023-04-20 08:00:09.716838 autohooks_plugin_black-23.4.0/pyproject.toml
--rw-r--r--   0        0        0     3750 1970-01-01 00:00:00.000000 autohooks_plugin_black-23.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-17 11:18:41.156167 autohooks_plugin_black-23.7.0/LICENSE
+-rw-r--r--   0        0        0     2243 2023-07-17 11:18:41.156167 autohooks_plugin_black-23.7.0/README.md
+-rw-r--r--   0        0        0      777 2023-07-17 11:18:41.156167 autohooks_plugin_black-23.7.0/autohooks/plugins/black/__init__.py
+-rw-r--r--   0        0        0      103 2023-07-17 11:18:41.156167 autohooks_plugin_black-23.7.0/autohooks/plugins/black/__version__.py
+-rw-r--r--   0        0        0     3375 2023-07-17 11:18:41.156167 autohooks_plugin_black-23.7.0/autohooks/plugins/black/black.py
+-rw-r--r--   0        0        0    39169 2023-07-17 11:18:41.156167 autohooks_plugin_black-23.7.0/poetry.lock
+-rw-r--r--   0        0        0     2088 2023-07-17 11:18:41.156167 autohooks_plugin_black-23.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3369 1970-01-01 00:00:00.000000 autohooks_plugin_black-23.7.0/PKG-INFO
```

### Comparing `autohooks_plugin_black-23.4.0/LICENSE` & `autohooks_plugin_black-23.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autohooks_plugin_black-23.4.0/README.md` & `autohooks_plugin_black-23.7.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -10,18 +10,15 @@
 ## Installation
 
 ### Install using pip
 
 You can install the latest stable release of autohooks-plugin-black from the
 Python Package Index using [pip](https://pip.pypa.io/):
 
-    pip install autohooks-plugin-black
-
-Note the `pip` refers to the Python 3 package manager. In a environment where
-Python 2 is also available the correct command may be `pip3`.
+    python3 -m pip install autohooks-plugin-black
 
 ### Install using poetry
 
 It is highly encouraged to use [poetry](https://python-poetry.org) for
 maintaining your project's dependencies. Normally autohooks-plugin-black is
 installed as a development dependency.
 
@@ -70,10 +67,10 @@
 [create a pull request](https://github.com/greenbone/autohooks-plugin-black/pulls)
 on GitHub. Bigger changes need to be discussed with the development team via the
 [issues section at GitHub](https://github.com/greenbone/autohooks-plugin-black/issues)
 first.
 
 ## License
 
-Copyright (C) 2019 [Greenbone AG](https://www.greenbone.net/)
+Copyright (C) 2019-2023 [Greenbone AG](https://www.greenbone.net/)
 
 Licensed under the [GNU General Public License v3.0 or later](LICENSE).
```

### Comparing `autohooks_plugin_black-23.4.0/autohooks/plugins/black/__init__.py` & `autohooks_plugin_black-23.7.0/autohooks/plugins/black/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,7 +12,9 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from .black import precommit
+
+__all__ = ("precommit",)
```

### Comparing `autohooks_plugin_black-23.4.0/autohooks/plugins/black/black.py` & `autohooks_plugin_black-23.7.0/autohooks/plugins/black/black.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 DEFAULT_INCLUDE = ("*.py",)
 DEFAULT_ARGUMENTS = ("-q",)
 
 
 def check_black_installed() -> None:
     try:
-        import black  # pylint: disable=unused-import, import-outside-toplevel
+        import black  # pylint: disable=unused-import, import-outside-toplevel # noqa: F401,E501
     except ImportError:
         raise RuntimeError(
             "Could not find black. "
             "Please add black to your python environment."
         ) from None
```

### Comparing `autohooks_plugin_black-23.4.0/pyproject.toml` & `autohooks_plugin_black-23.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,62 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "autohooks-plugin-black"
-version = "23.4.0"
+version = "23.7.0"
 description = "An autohooks plugin for python code formatting via black"
 license = "GPL-3.0-or-later"
 authors = ["Greenbone AG <info@greenbone.net>"]
 readme = "README.md"
 homepage = "https://github.com/greenbone/autohooks-plugin-black"
 repository = "https://github.com/greenbone/autohooks-plugin-black"
 documentation = ""
 # Full list: https://pypi.org/pypi?%3Aaction=list_classifiers
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Environment :: Console",
   "Intended Audience :: Developers",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [
   { include = "autohooks" },
   { include = "poetry.lock", format = "sdist"},
-  { include = "poetry.toml", format = "sdist"},
 ]
 keywords = [
   "git",
   "formatting",
   "linting",
   "hooks",
   "black",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7.2"
+python = "^3.8"
 black = ">=20.8"
 autohooks = ">=21.6.0"
 
 [tool.poetry.dev-dependencies]
-autohooks-plugin-pylint = ">=21.6.0"
+autohooks-plugin-ruff = ">=23.6.0"
 autohooks-plugin-isort = ">=22.3.0"
-coverage = "^7.2.3"
-mypy = "^1.2"
+autohooks-plugin-mypy = ">=23.3.0"
+coverage = ">=7.2.7"
+mypy = ">=1.4"
 pontos = ">=22.5.0"
 
 [tool.black]
 line-length = 80
-target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
+target-version = ['py38', 'py39', 'py310', 'py311']
 exclude = '''
 /(
     \.git
   | \.venv
   | \.github
   | \.vscode
   | _build
@@ -68,19 +67,25 @@
 '''
 
 [tool.autohooks]
 mode = "poetry"
 pre-commit = [
   'autohooks.plugins.isort',
   'autohooks.plugins.black',
-  'autohooks.plugins.pylint',
+  'autohooks.plugins.ruff',
+  'autohooks.plugins.mypy',
 ]
 
 [tool.pontos.version]
 version-module-file = "autohooks/plugins/black/__version__.py"
 
 [tool.isort]
 profile = "black"
 line_length = 80
 
 [tool.mypy]
+files = "autohooks"
 ignore_missing_imports = true
+
+[tool.ruff]
+line-length = 80
+target-version = "py38"
```

### Comparing `autohooks_plugin_black-23.4.0/PKG-INFO` & `autohooks_plugin_black-23.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 Metadata-Version: 2.1
 Name: autohooks-plugin-black
-Version: 23.4.0
+Version: 23.7.0
 Summary: An autohooks plugin for python code formatting via black
 Home-page: https://github.com/greenbone/autohooks-plugin-black
 License: GPL-3.0-or-later
 Keywords: git,formatting,linting,hooks,black
 Author: Greenbone AG
 Author-email: info@greenbone.net
-Requires-Python: >=3.7.2,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: autohooks (>=21.6.0)
 Requires-Dist: black (>=20.8)
 Project-URL: Repository, https://github.com/greenbone/autohooks-plugin-black
 Description-Content-Type: text/markdown
 
 ![Greenbone Logo](https://www.greenbone.net/wp-content/uploads/gb_new-logo_horizontal_rgb_small.png)
@@ -41,18 +36,15 @@
 ## Installation
 
 ### Install using pip
 
 You can install the latest stable release of autohooks-plugin-black from the
 Python Package Index using [pip](https://pip.pypa.io/):
 
-    pip install autohooks-plugin-black
-
-Note the `pip` refers to the Python 3 package manager. In a environment where
-Python 2 is also available the correct command may be `pip3`.
+    python3 -m pip install autohooks-plugin-black
 
 ### Install using poetry
 
 It is highly encouraged to use [poetry](https://python-poetry.org) for
 maintaining your project's dependencies. Normally autohooks-plugin-black is
 installed as a development dependency.
 
@@ -101,11 +93,11 @@
 [create a pull request](https://github.com/greenbone/autohooks-plugin-black/pulls)
 on GitHub. Bigger changes need to be discussed with the development team via the
 [issues section at GitHub](https://github.com/greenbone/autohooks-plugin-black/issues)
 first.
 
 ## License
 
-Copyright (C) 2019 [Greenbone AG](https://www.greenbone.net/)
+Copyright (C) 2019-2023 [Greenbone AG](https://www.greenbone.net/)
 
 Licensed under the [GNU General Public License v3.0 or later](LICENSE).
```

