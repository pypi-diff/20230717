# Comparing `tmp/su6_plugin_svelte_check-0.2.2.tar.gz` & `tmp/su6_plugin_svelte_check-0.3.0.tar.gz`

## Comparing `su6_plugin_svelte_check-0.2.2.tar` & `su6_plugin_svelte_check-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/coverage.svg
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/.github/workflows/su6.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/htmlcov/d_a80ff4318293920f___about___py.html
--rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/htmlcov/d_a80ff4318293920f___init___py.html
--rw-r--r--   0        0        0    15560 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/htmlcov/d_a80ff4318293920f_cli_py.html
--rw-r--r--   0        0        0    19618 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/htmlcov/d_a80ff4318293920f_find_project_root_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/htmlcov/style.css
--rw-r--r--   0        0        0    32741 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/pytest_examples/package-lock.json
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/pytest_examples/package.json
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/pytest_examples/tsconfig-issues.json
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/pytest_examples/tsconfig-no_issues.json
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/pytest_examples/tsconfig-warnings.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/pytest_examples/issues/index.svelte
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/pytest_examples/no_issues/index.svelte
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/pytest_examples/warnings/index.svelte
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/src/su6_plugin_svelte_check/__about__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/src/su6_plugin_svelte_check/__init__.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/src/su6_plugin_svelte_check/cli.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/src/su6_plugin_svelte_check/find_project_root.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/tests/test_about.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/tests/test_find_project_root.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/tests/test_plugin.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/LICENSE.txt
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/README.md
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/coverage.svg
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/.github/workflows/su6.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/d_a80ff4318293920f___about___py.html
+-rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/d_a80ff4318293920f___init___py.html
+-rw-r--r--   0        0        0    15560 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/d_a80ff4318293920f_cli_py.html
+-rw-r--r--   0        0        0    19618 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/d_a80ff4318293920f_find_project_root_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/style.css
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/.gitignore
+-rw-r--r--   0        0        0    32309 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/package-lock.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/package.json
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/tsconfig-issues.json
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/tsconfig-no_issues.json
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/tsconfig-warnings.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/issues/index.svelte
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/no_issues/index.svelte
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/warnings/index.svelte
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/src/su6_plugin_svelte_check/__about__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/src/su6_plugin_svelte_check/__init__.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/src/su6_plugin_svelte_check/cli.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/src/su6_plugin_svelte_check/find_project_root.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/tests/test_about.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/tests/test_find_project_root.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/tests/test_plugin.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/README.md
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/PKG-INFO
```

### Comparing `su6_plugin_svelte_check-0.2.2/CHANGELOG.md` & `su6_plugin_svelte_check-0.3.0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.3.0 (2023-07-17)
+### Feature
+* Allow specifying a custom --node-modules directory which should have `svelte-check` ([`db1dc42`](https://github.com/robinvandernoord/su6-plugin-svelte-check/commit/db1dc42720e7f94020249b6859097b3cb541cda0))
+
 ## v0.2.2 (2023-07-17)
 ### Fix
 * Don't include node modules in git!! ([`360325c`](https://github.com/robinvandernoord/su6-plugin-svelte-check/commit/360325c02ed99fb34519941061e9b78679601d61))
 
 ## v0.2.1 (2023-07-17)
 
 ### Fix
```

### Comparing `su6_plugin_svelte_check-0.2.2/coverage.svg` & `su6_plugin_svelte_check-0.3.0/coverage.svg`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/htmlcov/coverage_html.js` & `su6_plugin_svelte_check-0.3.0/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/htmlcov/d_a80ff4318293920f___about___py.html` & `su6_plugin_svelte_check-0.3.0/htmlcov/d_a80ff4318293920f___about___py.html`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/htmlcov/d_a80ff4318293920f___init___py.html` & `su6_plugin_svelte_check-0.3.0/htmlcov/d_a80ff4318293920f___init___py.html`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/htmlcov/d_a80ff4318293920f_cli_py.html` & `su6_plugin_svelte_check-0.3.0/htmlcov/d_a80ff4318293920f_cli_py.html`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/htmlcov/d_a80ff4318293920f_find_project_root_py.html` & `su6_plugin_svelte_check-0.3.0/htmlcov/d_a80ff4318293920f_find_project_root_py.html`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/htmlcov/favicon_32.png` & `su6_plugin_svelte_check-0.3.0/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/htmlcov/index.html` & `su6_plugin_svelte_check-0.3.0/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/htmlcov/keybd_closed.png` & `su6_plugin_svelte_check-0.3.0/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/htmlcov/keybd_open.png` & `su6_plugin_svelte_check-0.3.0/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/htmlcov/status.json` & `su6_plugin_svelte_check-0.3.0/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/htmlcov/style.css` & `su6_plugin_svelte_check-0.3.0/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/pytest_examples/package-lock.json` & `su6_plugin_svelte_check-0.3.0/pytest_examples/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984756097560976%*

 * *Differences: {"'packages'": "{delete: ['node_modules/fsevents']}"}*

```diff
@@ -327,27 +327,14 @@
             "version": "7.0.1"
         },
         "node_modules/fs.realpath": {
             "integrity": "sha512-OO0pH2lK6a0hZnAdau5ItzHPI6pUlvI7jMVnxUQRtw4owF2wk8lOSabtGDCTP4Ggrg2MbGnWO9X8K1t4+fGMDw==",
             "resolved": "https://registry.npmjs.org/fs.realpath/-/fs.realpath-1.0.0.tgz",
             "version": "1.0.0"
         },
-        "node_modules/fsevents": {
-            "engines": {
-                "node": "^8.16.0 || ^10.6.0 || >=11.0.0"
-            },
-            "hasInstallScript": true,
-            "integrity": "sha512-xiqMQR4xAeHTuB9uWm+fFRcIOgKBMiOBP+eXiyT7jsgVCq1bkVygt00oASowB7EdtpOHaaPgKt812P9ab+DDKA==",
-            "optional": true,
-            "os": [
-                "darwin"
-            ],
-            "resolved": "https://registry.npmjs.org/fsevents/-/fsevents-2.3.2.tgz",
-            "version": "2.3.2"
-        },
         "node_modules/glob": {
             "dependencies": {
                 "fs.realpath": "^1.0.0",
                 "inflight": "^1.0.4",
                 "inherits": "2",
                 "minimatch": "^3.1.1",
                 "once": "^1.3.0",
```

### Comparing `su6_plugin_svelte_check-0.2.2/pytest_examples/tsconfig-issues.json` & `su6_plugin_svelte_check-0.3.0/pytest_examples/tsconfig-issues.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/pytest_examples/tsconfig-no_issues.json` & `su6_plugin_svelte_check-0.3.0/pytest_examples/tsconfig-no_issues.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/pytest_examples/tsconfig-warnings.json` & `su6_plugin_svelte_check-0.3.0/pytest_examples/tsconfig-warnings.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/src/su6_plugin_svelte_check/cli.py` & `su6_plugin_svelte_check-0.3.0/src/su6_plugin_svelte_check/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,23 +18,25 @@
     tsconfig: str = "./tsconfig.json"
 
 
 config = SvelteCheckPluginConfig()
 
 
 @register(add_to_all=True)
-def svelte_check(strict: bool = None, tsconfig: str = None) -> int:
+def svelte_check(strict: bool = None, tsconfig: str = None, node_modules: str = None) -> int:
     """
     Register a top-level command.
 
     @register works without ()
     """
     config.update(strict=strict, tsconfig=tsconfig)
     # svelte-check --tsconfig ./tsconfig.json --threshold error
-    root, _ = find_project_root(("node_modules",))
+
+    node_modules = node_modules or "node_modules"
+    root, _ = find_project_root((node_modules,))
     executable = str(root / "node_modules/svelte-check/bin/svelte-check")
 
     args = []
     if config.strict:
         args.append("--fail-on-warnings")
     else:
         args.extend(["--threshold", "error"])
```

### Comparing `su6_plugin_svelte_check-0.2.2/src/su6_plugin_svelte_check/find_project_root.py` & `su6_plugin_svelte_check-0.3.0/src/su6_plugin_svelte_check/find_project_root.py`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/tests/test_find_project_root.py` & `su6_plugin_svelte_check-0.3.0/tests/test_find_project_root.py`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/tests/test_plugin.py` & `su6_plugin_svelte_check-0.3.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/LICENSE.txt` & `su6_plugin_svelte_check-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/pyproject.toml` & `su6_plugin_svelte_check-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.2.2/PKG-INFO` & `su6_plugin_svelte_check-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: su6-plugin-svelte-check
-Version: 0.2.2
+Version: 0.3.0
 Summary: Svelte-check plugin for `su6`
 Project-URL: Documentation, https://github.com/robinvandernoord/su6-plugin-svelte-check#readme
 Project-URL: Issues, https://github.com/robinvandernoord/su6-plugin-svelte-check/issues
 Project-URL: Source, https://github.com/robinvandernoord/su6-plugin-svelte-check
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

