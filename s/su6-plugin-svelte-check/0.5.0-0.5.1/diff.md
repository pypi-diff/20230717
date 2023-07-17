# Comparing `tmp/su6_plugin_svelte_check-0.5.0.tar.gz` & `tmp/su6_plugin_svelte_check-0.5.1.tar.gz`

## Comparing `su6_plugin_svelte_check-0.5.0.tar` & `su6_plugin_svelte_check-0.5.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/coverage.svg
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/.github/workflows/su6.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f___about___py.html
--rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f___init___py.html
--rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f_cli_py.html
--rw-r--r--   0        0        0    19618 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f_find_project_root_py.html
--rw-r--r--   0        0        0    22030 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f_helpers_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/style.css
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pytest_examples/.gitignore
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pytest_examples/custom_tsconfig.json
--rw-r--r--   0        0        0    32309 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pytest_examples/package-lock.json
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pytest_examples/package.json
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pytest_examples/pyproject.toml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pytest_examples/issues/index.svelte
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pytest_examples/no_issues/index.svelte
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pytest_examples/warnings/index.svelte
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/src/su6_plugin_svelte_check/__about__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/src/su6_plugin_svelte_check/__init__.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/src/su6_plugin_svelte_check/cli.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/src/su6_plugin_svelte_check/helpers.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/tests/test_about.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/tests/test_find_project_root.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/tests/test_plugin.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/README.md
--rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/coverage.svg
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/.github/workflows/su6.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/htmlcov/d_a80ff4318293920f___about___py.html
+-rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/htmlcov/d_a80ff4318293920f___init___py.html
+-rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/htmlcov/d_a80ff4318293920f_cli_py.html
+-rw-r--r--   0        0        0    19618 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/htmlcov/d_a80ff4318293920f_find_project_root_py.html
+-rw-r--r--   0        0        0    22030 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/htmlcov/d_a80ff4318293920f_helpers_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/htmlcov/style.css
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/pytest_examples/.gitignore
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/pytest_examples/custom_tsconfig.json
+-rw-r--r--   0        0        0    32309 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/pytest_examples/package-lock.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/pytest_examples/package.json
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/pytest_examples/pyproject.toml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/pytest_examples/issues/index.svelte
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/pytest_examples/no_issues/index.svelte
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/pytest_examples/warnings/index.svelte
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/src/su6_plugin_svelte_check/__about__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/src/su6_plugin_svelte_check/__init__.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/src/su6_plugin_svelte_check/cli.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/src/su6_plugin_svelte_check/helpers.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/tests/test_about.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/tests/test_find_project_root.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/tests/test_plugin.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/LICENSE.txt
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/README.md
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.1/PKG-INFO
```

### Comparing `su6_plugin_svelte_check-0.5.0/CHANGELOG.md` & `su6_plugin_svelte_check-0.5.1/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.5.1 (2023-07-17)
+### Documentation
+* **readme:** More informative ([`1c64ef6`](https://github.com/robinvandernoord/su6-plugin-svelte-check/commit/1c64ef6e75c26e3fe6f985b673444a158f0ee1d1))
+
 ## v0.5.0 (2023-07-17)
 ### Feature
 * Allow defining custom target ([`bcac570`](https://github.com/robinvandernoord/su6-plugin-svelte-check/commit/bcac57077b53d7c1b8a79d2100309b3448739fc3))
 
 ## v0.4.0 (2023-07-17)
 ### Feature
 * Add install-svelte-check command ([`84630d2`](https://github.com/robinvandernoord/su6-plugin-svelte-check/commit/84630d254fd1946d5789f50a427d29024f41b227))
```

### Comparing `su6_plugin_svelte_check-0.5.0/coverage.svg` & `su6_plugin_svelte_check-0.5.1/coverage.svg`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.5.0/htmlcov/coverage_html.js` & `su6_plugin_svelte_check-0.5.1/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f___about___py.html` & `su6_plugin_svelte_check-0.5.1/htmlcov/d_a80ff4318293920f___about___py.html`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f___init___py.html` & `su6_plugin_svelte_check-0.5.1/htmlcov/d_a80ff4318293920f___init___py.html`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f_cli_py.html` & `su6_plugin_svelte_check-0.5.1/htmlcov/d_a80ff4318293920f_cli_py.html`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f_find_project_root_py.html` & `su6_plugin_svelte_check-0.5.1/htmlcov/d_a80ff4318293920f_find_project_root_py.html`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f_helpers_py.html` & `su6_plugin_svelte_check-0.5.1/htmlcov/d_a80ff4318293920f_helpers_py.html`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.5.0/htmlcov/favicon_32.png` & `su6_plugin_svelte_check-0.5.1/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.5.0/htmlcov/index.html` & `su6_plugin_svelte_check-0.5.1/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.5.0/htmlcov/keybd_closed.png` & `su6_plugin_svelte_check-0.5.1/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.5.0/htmlcov/keybd_open.png` & `su6_plugin_svelte_check-0.5.1/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.5.0/htmlcov/status.json` & `su6_plugin_svelte_check-0.5.1/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.5.0/htmlcov/style.css` & `su6_plugin_svelte_check-0.5.1/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.5.0/pytest_examples/package-lock.json` & `su6_plugin_svelte_check-0.5.1/pytest_examples/package-lock.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.5.0/src/su6_plugin_svelte_check/cli.py` & `su6_plugin_svelte_check-0.5.1/src/su6_plugin_svelte_check/cli.py`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.5.0/src/su6_plugin_svelte_check/helpers.py` & `su6_plugin_svelte_check-0.5.1/src/su6_plugin_svelte_check/helpers.py`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.5.0/tests/test_find_project_root.py` & `su6_plugin_svelte_check-0.5.1/tests/test_find_project_root.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import contextlib
 from pathlib import Path
 
 from src.su6_plugin_svelte_check.helpers import find_project_root, chdir
 
 
 def test_find_project_root_node_modules():
     with chdir("./pytest_examples/no_issues"):
```

### Comparing `su6_plugin_svelte_check-0.5.0/tests/test_plugin.py` & `su6_plugin_svelte_check-0.5.1/tests/test_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-import contextlib
-import os
 import shutil
 from pathlib import Path
 
+from plumbum import local
 from su6 import app
 from typer.testing import CliRunner
-from plumbum import local
 
-try:
-    chdir = contextlib.chdir
-except AttributeError:
-    from contextlib_chdir import chdir
+from src.su6_plugin_svelte_check.helpers import chdir
 
 runner = CliRunner(mix_stderr=False)
 
 
 def prepare_env():
     local["npm"]("install", "svelte-check")
```

### Comparing `su6_plugin_svelte_check-0.5.0/LICENSE.txt` & `su6_plugin_svelte_check-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.5.0/pyproject.toml` & `su6_plugin_svelte_check-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 svelte-check = "su6_plugin_svelte_check.cli"  
 
 [template.plugins.default]
 src-layout = true
 
 [project.optional-dependencies]
 dev = [
-    "su6[all]"
+    "su6[all]",
+    "hatch",
 ]
 
 [project.urls]
 Documentation = "https://github.com/robinvandernoord/su6-plugin-svelte-check#readme" 
 Issues = "https://github.com/robinvandernoord/su6-plugin-svelte-check/issues" 
 Source = "https://github.com/robinvandernoord/su6-plugin-svelte-check"
```

### Comparing `su6_plugin_svelte_check-0.5.0/PKG-INFO` & `su6_plugin_svelte_check-0.5.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: su6-plugin-svelte-check
-Version: 0.5.0
+Version: 0.5.1
 Summary: Svelte-check plugin for `su6`
 Project-URL: Documentation, https://github.com/robinvandernoord/su6-plugin-svelte-check#readme
 Project-URL: Issues, https://github.com/robinvandernoord/su6-plugin-svelte-check/issues
 Project-URL: Source, https://github.com/robinvandernoord/su6-plugin-svelte-check
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -14,17 +14,46 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: su6>=1.6.0
 Provides-Extra: dev
+Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: su6[all]; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # su6-plugin-svelte-check
 
 Plugin for [su6](https://github.com/trialandsuccess/su6) that adds `svelte-check` functionality.
 
+## Installation
+```bash
+pip install su6-plugin-svelte-check
+# or
+pip install su6[svelte-check]
+```
+
+## Usage
+
+```bash
+# optionally, if svelte-check isn't installed yet:
+su6 install-svelte-check
+
+su6 svelte-check
+```
+
+### pyproject.toml
+(all keys are optional, and also usable as flags to `svelte-check` (e.g. `--strict` or `--target ./path/to/files`))
+```toml
+[tool.su6.prettier]
+target = "./path/to/svelte/files"
+node_modules = "./path/to/node_modules"
+
+strict = true | false
+tsconfig = "./path/to/tsconfig.json"
+```
+
+
 ## License
 
 `su6-plugin-svelte-check` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

