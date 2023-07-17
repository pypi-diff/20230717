# Comparing `tmp/su6_plugin_svelte_check-0.4.0.tar.gz` & `tmp/su6_plugin_svelte_check-0.5.0.tar.gz`

## Comparing `su6_plugin_svelte_check-0.4.0.tar` & `su6_plugin_svelte_check-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/coverage.svg
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/.github/workflows/su6.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f___about___py.html
--rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f___init___py.html
--rw-r--r--   0        0        0    18443 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f_cli_py.html
--rw-r--r--   0        0        0    19618 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f_find_project_root_py.html
--rw-r--r--   0        0        0    21967 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f_helpers_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/style.css
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/.gitignore
--rw-r--r--   0        0        0    32309 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/package-lock.json
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/package.json
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/tsconfig-issues.json
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/tsconfig-no_issues.json
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/tsconfig-warnings.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/issues/index.svelte
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/no_issues/index.svelte
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/warnings/index.svelte
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/src/su6_plugin_svelte_check/__about__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/src/su6_plugin_svelte_check/__init__.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/src/su6_plugin_svelte_check/cli.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/src/su6_plugin_svelte_check/helpers.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/tests/test_about.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/tests/test_find_project_root.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/tests/test_plugin.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/README.md
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/coverage.svg
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/.github/workflows/su6.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f___about___py.html
+-rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f___init___py.html
+-rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f_cli_py.html
+-rw-r--r--   0        0        0    19618 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f_find_project_root_py.html
+-rw-r--r--   0        0        0    22030 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f_helpers_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/htmlcov/style.css
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pytest_examples/.gitignore
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pytest_examples/custom_tsconfig.json
+-rw-r--r--   0        0        0    32309 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pytest_examples/package-lock.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pytest_examples/package.json
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pytest_examples/pyproject.toml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pytest_examples/issues/index.svelte
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pytest_examples/no_issues/index.svelte
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pytest_examples/warnings/index.svelte
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/src/su6_plugin_svelte_check/__about__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/src/su6_plugin_svelte_check/__init__.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/src/su6_plugin_svelte_check/cli.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/src/su6_plugin_svelte_check/helpers.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/tests/test_about.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/tests/test_find_project_root.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/tests/test_plugin.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/README.md
+-rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.5.0/PKG-INFO
```

### Comparing `su6_plugin_svelte_check-0.4.0/CHANGELOG.md` & `su6_plugin_svelte_check-0.5.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.5.0 (2023-07-17)
+### Feature
+* Allow defining custom target ([`bcac570`](https://github.com/robinvandernoord/su6-plugin-svelte-check/commit/bcac57077b53d7c1b8a79d2100309b3448739fc3))
+
 ## v0.4.0 (2023-07-17)
 ### Feature
 * Add install-svelte-check command ([`84630d2`](https://github.com/robinvandernoord/su6-plugin-svelte-check/commit/84630d254fd1946d5789f50a427d29024f41b227))
 
 ## v0.3.0 (2023-07-17)
 ### Feature
 * Allow specifying a custom --node-modules directory which should have `svelte-check` ([`db1dc42`](https://github.com/robinvandernoord/su6-plugin-svelte-check/commit/db1dc42720e7f94020249b6859097b3cb541cda0))
```

### Comparing `su6_plugin_svelte_check-0.4.0/coverage.svg` & `su6_plugin_svelte_check-0.5.0/coverage.svg`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.4.0/htmlcov/coverage_html.js` & `su6_plugin_svelte_check-0.5.0/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f___about___py.html` & `su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f___about___py.html`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f___init___py.html` & `su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f___init___py.html`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f_cli_py.html` & `su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f_find_project_root_py.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/su6_plugin_svelte_check/cli.py: 100%</title>
+    <title>Coverage for src/su6_plugin_svelte_check/find_project_root.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/su6_plugin_svelte_check/cli.py</b>:
+            <span class="text">Coverage for </span><b>src/su6_plugin_svelte_check/find_project_root.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">26 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">26<span class="text"> run</span></button>
+            <span class="text">18 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">18<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
-            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
+            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">4<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_a80ff4318293920f___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_a80ff4318293920f_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_a80ff4318293920f_helpers_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-17 17:28 +0200
+            created at 2023-07-17 14:04 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -77,77 +77,74 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">This module contains an example of both methods of adding commands to su6.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Modified from black.files.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">su6</span><span class="op">.</span><span class="nam">plugins</span> <span class="key">import</span> <span class="nam">PluginConfig</span><span class="op">,</span> <span class="nam">register</span><span class="op">,</span> <span class="nam">run_tool</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">functools</span> <span class="key">import</span> <span class="nam">lru_cache</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Optional</span><span class="op">,</span> <span class="nam">Sequence</span><span class="op">,</span> <span class="nam">Tuple</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">chdir</span><span class="op">,</span> <span class="nam">find_project_root</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="op">@</span><span class="nam">register</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">class</span> <span class="nam">SvelteCheckPluginConfig</span><span class="op">(</span><span class="nam">PluginConfig</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">    Config without state, loads [tool.su6.demo] from pyproject.toml into self.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="op">@</span><span class="nam">lru_cache</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">def</span> <span class="nam">find_project_root</span><span class="op">(</span><span class="nam">srcs</span><span class="op">:</span> <span class="nam">Sequence</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span> <span class="nam">stdin_filename</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Tuple</span><span class="op">[</span><span class="nam">Path</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="str">    Return a directory containing .git, .hg, or pyproject.toml.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">    That directory will be a common parent of all files and directories</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="str">    passed in `srcs`.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="nam">tsconfig</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"./tsconfig.json"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">    If no directory in the tree contains a marker that would specify it's the</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">    project root, the root of the file system is returned.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="nam">config</span> <span class="op">=</span> <span class="nam">SvelteCheckPluginConfig</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="op">@</span><span class="nam">register</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="key">def</span> <span class="nam">install_svelte_check</span><span class="op">(</span><span class="nam">target_dir</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="str">    Install the svelte-check tool using npm.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="nam">target_dir</span> <span class="op">=</span> <span class="nam">target_dir</span> <span class="key">or</span> <span class="str">"./"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="str">    Returns a two-tuple with the first element as the project root path and</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="str">    the second element as a string describing the method by which the</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="str">    project root was discovered.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="key">if</span> <span class="nam">stdin_filename</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="nam">srcs</span> <span class="op">=</span> <span class="nam">tuple</span><span class="op">(</span><span class="nam">stdin_filename</span> <span class="key">if</span> <span class="nam">s</span> <span class="op">==</span> <span class="str">"-"</span> <span class="key">else</span> <span class="nam">s</span> <span class="key">for</span> <span class="nam">s</span> <span class="key">in</span> <span class="nam">srcs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">srcs</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="nam">srcs</span> <span class="op">=</span> <span class="op">[</span><span class="nam">str</span><span class="op">(</span><span class="nam">Path</span><span class="op">.</span><span class="nam">cwd</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">resolve</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="nam">path_srcs</span> <span class="op">=</span> <span class="op">[</span><span class="nam">Path</span><span class="op">(</span><span class="nam">Path</span><span class="op">.</span><span class="nam">cwd</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">src</span><span class="op">)</span><span class="op">.</span><span class="nam">resolve</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">src</span> <span class="key">in</span> <span class="nam">srcs</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="key">with</span> <span class="nam">chdir</span><span class="op">(</span><span class="nam">target_dir</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="key">return</span> <span class="nam">run_tool</span><span class="op">(</span><span class="str">"npm"</span><span class="op">,</span> <span class="str">"install"</span><span class="op">,</span> <span class="str">"svelte-check"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="com"># A list of lists of parents for each 'src'. 'src' is included as a</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="com"># "parent" of itself if it is a directory</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="nam">src_parents</span> <span class="op">=</span> <span class="op">[</span><span class="nam">list</span><span class="op">(</span><span class="nam">path</span><span class="op">.</span><span class="nam">parents</span><span class="op">)</span> <span class="op">+</span> <span class="op">(</span><span class="op">[</span><span class="nam">path</span><span class="op">]</span> <span class="key">if</span> <span class="nam">path</span><span class="op">.</span><span class="nam">is_dir</span><span class="op">(</span><span class="op">)</span> <span class="key">else</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span> <span class="key">for</span> <span class="nam">path</span> <span class="key">in</span> <span class="nam">path_srcs</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t"><span class="op">@</span><span class="nam">register</span><span class="op">(</span><span class="nam">add_to_all</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t"><span class="key">def</span> <span class="nam">svelte_check</span><span class="op">(</span><span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">tsconfig</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">node_modules</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="str">    Run the svelte-check tool.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="nam">config</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">,</span> <span class="nam">tsconfig</span><span class="op">=</span><span class="nam">tsconfig</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="com"># svelte-check --tsconfig ./tsconfig.json --threshold error</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="nam">node_modules</span> <span class="op">=</span> <span class="nam">node_modules</span> <span class="key">or</span> <span class="str">"node_modules"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="nam">root</span><span class="op">,</span> <span class="nam">_</span> <span class="op">=</span> <span class="nam">find_project_root</span><span class="op">(</span><span class="op">(</span><span class="nam">node_modules</span><span class="op">,</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="nam">executable</span> <span class="op">=</span> <span class="nam">str</span><span class="op">(</span><span class="nam">root</span> <span class="op">/</span> <span class="str">"node_modules/svelte-check/bin/svelte-check"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">common_base</span> <span class="op">=</span> <span class="nam">max</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="nam">set</span><span class="op">.</span><span class="nam">intersection</span><span class="op">(</span><span class="op">*</span><span class="op">(</span><span class="nam">set</span><span class="op">(</span><span class="nam">parents</span><span class="op">)</span> <span class="key">for</span> <span class="nam">parents</span> <span class="key">in</span> <span class="nam">src_parents</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="nam">key</span><span class="op">=</span><span class="key">lambda</span> <span class="nam">path</span><span class="op">:</span> <span class="nam">path</span><span class="op">.</span><span class="nam">parts</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="key">for</span> <span class="nam">directory</span> <span class="key">in</span> <span class="op">(</span><span class="nam">common_base</span><span class="op">,</span> <span class="op">*</span><span class="nam">common_base</span><span class="op">.</span><span class="nam">parents</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">directory</span> <span class="op">/</span> <span class="str">"node_modules"</span><span class="op">)</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">            <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">"node_modules"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">directory</span> <span class="op">/</span> <span class="str">".git"</span><span class="op">)</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">            <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">".git directory"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="nam">args</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="key">if</span> <span class="nam">config</span><span class="op">.</span><span class="nam">strict</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="str">"--fail-on-warnings"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="op">[</span><span class="str">"--threshold"</span><span class="op">,</span> <span class="str">"error"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">directory</span> <span class="op">/</span> <span class="str">".hg"</span><span class="op">)</span><span class="op">.</span><span class="nam">is_dir</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">            <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">".hg directory"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">directory</span> <span class="op">/</span> <span class="str">"pyproject.toml"</span><span class="op">)</span><span class="op">.</span><span class="nam">is_file</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">            <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">"pyproject.toml"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="key">if</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">config</span><span class="op">.</span><span class="nam">tsconfig</span><span class="op">)</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="op">[</span><span class="str">"--tsconfig"</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">tsconfig</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="key">return</span> <span class="nam">run_tool</span><span class="op">(</span><span class="nam">executable</span><span class="op">,</span> <span class="op">*</span><span class="nam">args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">"file system root"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_a80ff4318293920f___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_a80ff4318293920f_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_a80ff4318293920f_helpers_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-17 17:28 +0200
+            created at 2023-07-17 14:04 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,76 +1,75 @@
 
-****** Coverage for src/su6_plugin_svelte_check/cli.py: 100% ******
+****** Coverage for src/su6_plugin_svelte_check/find_project_root.py: 100%
+******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 26 statements   26 run 0 missing 0 excluded *****
+***** 18 statements   18 run 0 missing 4 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-17 17:28 +0200
+at 2023-07-17 14:04 +0200
 
 
 1""" 
-2This module contains an example of both methods of adding commands to su6. 
+2Modified from black.files. 
 3""" 
-4from pathlib import Path 
-5 
-6from su6.plugins import PluginConfig, register, run_tool 
+4from functools import lru_cache 
+5from pathlib import Path 
+6from typing import Optional, Sequence, Tuple 
 7 
-8from .helpers import chdir, find_project_root 
-9 
-10 
-11@register 
-12class SvelteCheckPluginConfig(PluginConfig): 
-13 """ 
-14 Config without state, loads [tool.su6.demo] from pyproject.toml into self. 
-15 """ 
+8 
+9@lru_cache() 
+10def find_project_root(srcs: Sequence[str], stdin_filename: Optional[str] =
+None) -> Tuple[Path, str]: 
+11 """ 
+12 Return a directory containing .git, .hg, or pyproject.toml. 
+13 
+14 That directory will be a common parent of all files and directories 
+15 passed in `srcs`. 
 16 
-17 strict: bool = False 
-18 tsconfig: str = "./tsconfig.json" 
+17 If no directory in the tree contains a marker that would specify it's the 
+18 project root, the root of the file system is returned. 
 19 
-20 
-21config = SvelteCheckPluginConfig() 
-22 
-23 
-24@register 
-25def install_svelte_check(target_dir: str = None) -> int: 
-26 """ 
-27 Install the svelte-check tool using npm. 
-28 """ 
-29 target_dir = target_dir or "./" 
+20 Returns a two-tuple with the first element as the project root path and 
+21 the second element as a string describing the method by which the 
+22 project root was discovered. 
+23 """ 
+24 if stdin_filename is not None: 
+25 srcs = tuple(stdin_filename if s == "-" else s for s in srcs) 
+26 if not srcs: 
+27 srcs = [str(Path.cwd().resolve())] 
+28 
+29 path_srcs = [Path(Path.cwd(), src).resolve() for src in srcs] 
 30 
-31 with chdir(target_dir): 
-32 return run_tool("npm", "install", "svelte-check") 
-33 
+31 # A list of lists of parents for each 'src'. 'src' is included as a 
+32 # "parent" of itself if it is a directory 
+33 src_parents = [list(path.parents) + ([path] if path.is_dir() else []) for
+path in path_srcs] 
 34 
-35@register(add_to_all=True) 
-36def svelte_check(strict: bool = None, tsconfig: str = None, node_modules: str
-= None) -> int: 
-37 """ 
-38 Run the svelte-check tool. 
-39 """ 
-40 config.update(strict=strict, tsconfig=tsconfig) 
-41 # svelte-check --tsconfig ./tsconfig.json --threshold error 
-42 
-43 node_modules = node_modules or "node_modules" 
-44 root, _ = find_project_root((node_modules,)) 
-45 executable = str(root / "node_modules/svelte-check/bin/svelte-check") 
+35 common_base = max( 
+36 set.intersection(*(set(parents) for parents in src_parents)), 
+37 key=lambda path: path.parts, 
+38 ) 
+39 
+40 for directory in (common_base, *common_base.parents): 
+41 if (directory / "node_modules").exists(): 
+42 return directory, "node_modules" 
+43 
+44 if (directory / ".git").exists(): 
+45 return directory, ".git directory" 
 46 
-47 args = [] 
-48 if config.strict: 
-49 args.append("--fail-on-warnings") 
-50 else: 
-51 args.extend(["--threshold", "error"]) 
+47 if (directory / ".hg").is_dir(): # pragma: no cover 
+48 return directory, ".hg directory" 
+49 
+50 if (directory / "pyproject.toml").is_file(): # pragma: no cover 
+51 return directory, "pyproject.toml" 
 52 
-53 if Path(config.tsconfig).exists(): 
-54 args.extend(["--tsconfig", config.tsconfig]) 
-55 
-56 return run_tool(executable, *args) 
+53 return directory, "file system root" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-17 17:28 +0200
+at 2023-07-17 14:04 +0200
```

### Comparing `su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f_find_project_root_py.html` & `su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f_helpers_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/su6_plugin_svelte_check/find_project_root.py: 100%</title>
+    <title>Coverage for src/su6_plugin_svelte_check/helpers.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/su6_plugin_svelte_check/find_project_root.py</b>:
+            <span class="text">Coverage for </span><b>src/su6_plugin_svelte_check/helpers.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">18 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">18<span class="text"> run</span></button>
+            <span class="text">22 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">22<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
-            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">4<span class="text"> excluded</span></button>
+            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">6<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a80ff4318293920f_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-17 14:04 +0200
+            created at 2023-07-17 18:17 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -77,74 +77,86 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Modified from black.files.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Re-usable helpers for this project.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">functools</span> <span class="key">import</span> <span class="nam">lru_cache</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Optional</span><span class="op">,</span> <span class="nam">Sequence</span><span class="op">,</span> <span class="nam">Tuple</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="op">@</span><span class="nam">lru_cache</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">def</span> <span class="nam">find_project_root</span><span class="op">(</span><span class="nam">srcs</span><span class="op">:</span> <span class="nam">Sequence</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span> <span class="nam">stdin_filename</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Tuple</span><span class="op">[</span><span class="nam">Path</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="str">    Return a directory containing .git, .hg, or pyproject.toml.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">    That directory will be a common parent of all files and directories</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="str">    passed in `srcs`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">    If no directory in the tree contains a marker that would specify it's the</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">    project root, the root of the file system is returned.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="str">    Returns a two-tuple with the first element as the project root path and</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="str">    the second element as a string describing the method by which the</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="str">    project root was discovered.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="key">if</span> <span class="nam">stdin_filename</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="nam">srcs</span> <span class="op">=</span> <span class="nam">tuple</span><span class="op">(</span><span class="nam">stdin_filename</span> <span class="key">if</span> <span class="nam">s</span> <span class="op">==</span> <span class="str">"-"</span> <span class="key">else</span> <span class="nam">s</span> <span class="key">for</span> <span class="nam">s</span> <span class="key">in</span> <span class="nam">srcs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">srcs</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="nam">srcs</span> <span class="op">=</span> <span class="op">[</span><span class="nam">str</span><span class="op">(</span><span class="nam">Path</span><span class="op">.</span><span class="nam">cwd</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">resolve</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="nam">path_srcs</span> <span class="op">=</span> <span class="op">[</span><span class="nam">Path</span><span class="op">(</span><span class="nam">Path</span><span class="op">.</span><span class="nam">cwd</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">src</span><span class="op">)</span><span class="op">.</span><span class="nam">resolve</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">src</span> <span class="key">in</span> <span class="nam">srcs</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">contextlib</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">functools</span> <span class="key">import</span> <span class="nam">lru_cache</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Optional</span><span class="op">,</span> <span class="nam">Sequence</span><span class="op">,</span> <span class="nam">Tuple</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="nam">chdir</span> <span class="op">=</span> <span class="nam">contextlib</span><span class="op">.</span><span class="nam">chdir</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">except</span> <span class="nam">AttributeError</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="key">from</span> <span class="nam">contextlib_chdir</span> <span class="key">import</span> <span class="nam">chdir</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="op">@</span><span class="nam">lru_cache</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">def</span> <span class="nam">find_project_root</span><span class="op">(</span><span class="nam">srcs</span><span class="op">:</span> <span class="nam">Sequence</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span> <span class="nam">stdin_filename</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Tuple</span><span class="op">[</span><span class="nam">Path</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="str">    Return a directory containing .git, .hg, or pyproject.toml.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="str">    That directory will be a common parent of all files and directories</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="str">    passed in `srcs`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="str">    If no directory in the tree contains a marker that would specify it's the</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">    project root, the root of the file system is returned.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="str">    Returns a two-tuple with the first element as the project root path and</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="str">    the second element as a string describing the method by which the</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="str">    project root was discovered.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="com"># A list of lists of parents for each 'src'. 'src' is included as a</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="com"># "parent" of itself if it is a directory</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="nam">src_parents</span> <span class="op">=</span> <span class="op">[</span><span class="nam">list</span><span class="op">(</span><span class="nam">path</span><span class="op">.</span><span class="nam">parents</span><span class="op">)</span> <span class="op">+</span> <span class="op">(</span><span class="op">[</span><span class="nam">path</span><span class="op">]</span> <span class="key">if</span> <span class="nam">path</span><span class="op">.</span><span class="nam">is_dir</span><span class="op">(</span><span class="op">)</span> <span class="key">else</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span> <span class="key">for</span> <span class="nam">path</span> <span class="key">in</span> <span class="nam">path_srcs</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">common_base</span> <span class="op">=</span> <span class="nam">max</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="nam">set</span><span class="op">.</span><span class="nam">intersection</span><span class="op">(</span><span class="op">*</span><span class="op">(</span><span class="nam">set</span><span class="op">(</span><span class="nam">parents</span><span class="op">)</span> <span class="key">for</span> <span class="nam">parents</span> <span class="key">in</span> <span class="nam">src_parents</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="nam">key</span><span class="op">=</span><span class="key">lambda</span> <span class="nam">path</span><span class="op">:</span> <span class="nam">path</span><span class="op">.</span><span class="nam">parts</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="str">    Modified from black.files.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="key">if</span> <span class="nam">stdin_filename</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">srcs</span> <span class="op">=</span> <span class="nam">tuple</span><span class="op">(</span><span class="nam">stdin_filename</span> <span class="key">if</span> <span class="nam">s</span> <span class="op">==</span> <span class="str">"-"</span> <span class="key">else</span> <span class="nam">s</span> <span class="key">for</span> <span class="nam">s</span> <span class="key">in</span> <span class="nam">srcs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">srcs</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="nam">srcs</span> <span class="op">=</span> <span class="op">[</span><span class="nam">str</span><span class="op">(</span><span class="nam">Path</span><span class="op">.</span><span class="nam">cwd</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">resolve</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="nam">path_srcs</span> <span class="op">=</span> <span class="op">[</span><span class="nam">Path</span><span class="op">(</span><span class="nam">Path</span><span class="op">.</span><span class="nam">cwd</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">src</span><span class="op">)</span><span class="op">.</span><span class="nam">resolve</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">src</span> <span class="key">in</span> <span class="nam">srcs</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="key">for</span> <span class="nam">directory</span> <span class="key">in</span> <span class="op">(</span><span class="nam">common_base</span><span class="op">,</span> <span class="op">*</span><span class="nam">common_base</span><span class="op">.</span><span class="nam">parents</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">directory</span> <span class="op">/</span> <span class="str">"node_modules"</span><span class="op">)</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">            <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">"node_modules"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="com"># A list of lists of parents for each 'src'. 'src' is included as a</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="com"># "parent" of itself if it is a directory</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="nam">src_parents</span> <span class="op">=</span> <span class="op">[</span><span class="nam">list</span><span class="op">(</span><span class="nam">path</span><span class="op">.</span><span class="nam">parents</span><span class="op">)</span> <span class="op">+</span> <span class="op">(</span><span class="op">[</span><span class="nam">path</span><span class="op">]</span> <span class="key">if</span> <span class="nam">path</span><span class="op">.</span><span class="nam">is_dir</span><span class="op">(</span><span class="op">)</span> <span class="key">else</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span> <span class="key">for</span> <span class="nam">path</span> <span class="key">in</span> <span class="nam">path_srcs</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">directory</span> <span class="op">/</span> <span class="str">".git"</span><span class="op">)</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">            <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">".git directory"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">directory</span> <span class="op">/</span> <span class="str">".hg"</span><span class="op">)</span><span class="op">.</span><span class="nam">is_dir</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">            <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">".hg directory"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">directory</span> <span class="op">/</span> <span class="str">"pyproject.toml"</span><span class="op">)</span><span class="op">.</span><span class="nam">is_file</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">            <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">"pyproject.toml"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="nam">common_base</span> <span class="op">=</span> <span class="nam">max</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">        <span class="nam">set</span><span class="op">.</span><span class="nam">intersection</span><span class="op">(</span><span class="op">*</span><span class="op">(</span><span class="nam">set</span><span class="op">(</span><span class="nam">parents</span><span class="op">)</span> <span class="key">for</span> <span class="nam">parents</span> <span class="key">in</span> <span class="nam">src_parents</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">        <span class="nam">key</span><span class="op">=</span><span class="key">lambda</span> <span class="nam">path</span><span class="op">:</span> <span class="nam">path</span><span class="op">.</span><span class="nam">parts</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="key">for</span> <span class="nam">directory</span> <span class="key">in</span> <span class="op">(</span><span class="nam">common_base</span><span class="op">,</span> <span class="op">*</span><span class="nam">common_base</span><span class="op">.</span><span class="nam">parents</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">directory</span> <span class="op">/</span> <span class="str">"node_modules"</span><span class="op">)</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">            <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">"node_modules"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">"file system root"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">directory</span> <span class="op">/</span> <span class="str">".git"</span><span class="op">)</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">            <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">".git directory"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">directory</span> <span class="op">/</span> <span class="str">".hg"</span><span class="op">)</span><span class="op">.</span><span class="nam">is_dir</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">            <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">".hg directory"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">directory</span> <span class="op">/</span> <span class="str">"pyproject.toml"</span><span class="op">)</span><span class="op">.</span><span class="nam">is_file</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">            <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">"pyproject.toml"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">"file system root"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t"><span class="nam">__all__</span> <span class="op">=</span> <span class="op">[</span><span class="str">"chdir"</span><span class="op">,</span> <span class="str">"find_project_root"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a80ff4318293920f_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-17 14:04 +0200
+            created at 2023-07-17 18:17 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,75 +1,86 @@
 
-****** Coverage for src/su6_plugin_svelte_check/find_project_root.py: 100%
-******
+****** Coverage for src/su6_plugin_svelte_check/helpers.py: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 18 statements   18 run 0 missing 4 excluded *****
+***** 22 statements   22 run 0 missing 6 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-17 14:04 +0200
+at 2023-07-17 18:17 +0200
 
 
 1""" 
-2Modified from black.files. 
+2Re-usable helpers for this project. 
 3""" 
-4from functools import lru_cache 
-5from pathlib import Path 
-6from typing import Optional, Sequence, Tuple 
-7 
-8 
-9@lru_cache() 
-10def find_project_root(srcs: Sequence[str], stdin_filename: Optional[str] =
+4 
+5import contextlib 
+6from functools import lru_cache 
+7from pathlib import Path 
+8from typing import Optional, Sequence, Tuple 
+9 
+10try: 
+11 chdir = contextlib.chdir 
+12except AttributeError: # pragma: no cover 
+13 from contextlib_chdir import chdir # type: ignore 
+14 
+15 
+16@lru_cache() 
+17def find_project_root(srcs: Sequence[str], stdin_filename: Optional[str] =
 None) -> Tuple[Path, str]: 
-11 """ 
-12 Return a directory containing .git, .hg, or pyproject.toml. 
-13 
-14 That directory will be a common parent of all files and directories 
-15 passed in `srcs`. 
-16 
-17 If no directory in the tree contains a marker that would specify it's the 
-18 project root, the root of the file system is returned. 
-19 
-20 Returns a two-tuple with the first element as the project root path and 
-21 the second element as a string describing the method by which the 
-22 project root was discovered. 
-23 """ 
-24 if stdin_filename is not None: 
-25 srcs = tuple(stdin_filename if s == "-" else s for s in srcs) 
-26 if not srcs: 
-27 srcs = [str(Path.cwd().resolve())] 
-28 
-29 path_srcs = [Path(Path.cwd(), src).resolve() for src in srcs] 
+18 """ 
+19 Return a directory containing .git, .hg, or pyproject.toml. 
+20 
+21 That directory will be a common parent of all files and directories 
+22 passed in `srcs`. 
+23 
+24 If no directory in the tree contains a marker that would specify it's the 
+25 project root, the root of the file system is returned. 
+26 
+27 Returns a two-tuple with the first element as the project root path and 
+28 the second element as a string describing the method by which the 
+29 project root was discovered. 
 30 
-31 # A list of lists of parents for each 'src'. 'src' is included as a 
-32 # "parent" of itself if it is a directory 
-33 src_parents = [list(path.parents) + ([path] if path.is_dir() else []) for
-path in path_srcs] 
-34 
-35 common_base = max( 
-36 set.intersection(*(set(parents) for parents in src_parents)), 
-37 key=lambda path: path.parts, 
-38 ) 
+31 Modified from black.files. 
+32 """ 
+33 if stdin_filename is not None: 
+34 srcs = tuple(stdin_filename if s == "-" else s for s in srcs) 
+35 if not srcs: 
+36 srcs = [str(Path.cwd().resolve())] 
+37 
+38 path_srcs = [Path(Path.cwd(), src).resolve() for src in srcs] 
 39 
-40 for directory in (common_base, *common_base.parents): 
-41 if (directory / "node_modules").exists(): 
-42 return directory, "node_modules" 
+40 # A list of lists of parents for each 'src'. 'src' is included as a 
+41 # "parent" of itself if it is a directory 
+42 src_parents = [list(path.parents) + ([path] if path.is_dir() else []) for
+path in path_srcs] 
 43 
-44 if (directory / ".git").exists(): 
-45 return directory, ".git directory" 
-46 
-47 if (directory / ".hg").is_dir(): # pragma: no cover 
-48 return directory, ".hg directory" 
-49 
-50 if (directory / "pyproject.toml").is_file(): # pragma: no cover 
-51 return directory, "pyproject.toml" 
+44 common_base = max( 
+45 set.intersection(*(set(parents) for parents in src_parents)), 
+46 key=lambda path: path.parts, 
+47 ) 
+48 
+49 for directory in (common_base, *common_base.parents): 
+50 if (directory / "node_modules").exists(): 
+51 return directory, "node_modules" 
 52 
-53 return directory, "file system root" 
+53 if (directory / ".git").exists(): 
+54 return directory, ".git directory" 
+55 
+56 if (directory / ".hg").is_dir(): # pragma: no cover 
+57 return directory, ".hg directory" 
+58 
+59 if (directory / "pyproject.toml").is_file(): # pragma: no cover 
+60 return directory, "pyproject.toml" 
+61 
+62 return directory, "file system root" 
+63 
+64 
+65__all__ = ["chdir", "find_project_root"] 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-17 14:04 +0200
+at 2023-07-17 18:17 +0200
```

### Comparing `su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f_helpers_py.html` & `su6_plugin_svelte_check-0.5.0/htmlcov/d_a80ff4318293920f_cli_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/su6_plugin_svelte_check/helpers.py: 100%</title>
+    <title>Coverage for src/su6_plugin_svelte_check/cli.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/su6_plugin_svelte_check/helpers.py</b>:
+            <span class="text">Coverage for </span><b>src/su6_plugin_svelte_check/cli.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">24 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">24<span class="text"> run</span></button>
+            <span class="text">27 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">27<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
-            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">4<span class="text"> excluded</span></button>
+            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_a80ff4318293920f_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_a80ff4318293920f___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_a80ff4318293920f_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-17 17:28 +0200
+            created at 2023-07-17 18:23 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -77,86 +77,79 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Re-usable helpers for this project.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">This module contains an example of both methods of adding commands to su6.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">contextlib</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">functools</span> <span class="key">import</span> <span class="nam">lru_cache</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Optional</span><span class="op">,</span> <span class="nam">Sequence</span><span class="op">,</span> <span class="nam">Tuple</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">su6</span><span class="op">.</span><span class="nam">plugins</span> <span class="key">import</span> <span class="nam">PluginConfig</span><span class="op">,</span> <span class="nam">register</span><span class="op">,</span> <span class="nam">run_tool</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">chdir</span><span class="op">,</span> <span class="nam">find_project_root</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="nam">chdir</span> <span class="op">=</span> <span class="nam">contextlib</span><span class="op">.</span><span class="nam">chdir</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">except</span> <span class="nam">AttributeError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="key">from</span> <span class="nam">contextlib_chdir</span> <span class="key">import</span> <span class="nam">chdir</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="op">@</span><span class="nam">lru_cache</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">def</span> <span class="nam">find_project_root</span><span class="op">(</span><span class="nam">srcs</span><span class="op">:</span> <span class="nam">Sequence</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span> <span class="nam">stdin_filename</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Tuple</span><span class="op">[</span><span class="nam">Path</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="str">    Return a directory containing .git, .hg, or pyproject.toml.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="str">    That directory will be a common parent of all files and directories</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="str">    passed in `srcs`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="op">@</span><span class="nam">register</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">class</span> <span class="nam">SvelteCheckPluginConfig</span><span class="op">(</span><span class="nam">PluginConfig</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">    Config without state, loads [tool.su6.demo] from pyproject.toml into self.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="nam">target</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"."</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="nam">node_modules</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"./node_modules"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="nam">tsconfig</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"./tsconfig.json"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="str">    If no directory in the tree contains a marker that would specify it's the</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">    project root, the root of the file system is returned.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="nam">config</span> <span class="op">=</span> <span class="nam">SvelteCheckPluginConfig</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="str">    Returns a two-tuple with the first element as the project root path and</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="str">    the second element as a string describing the method by which the</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="str">    project root was discovered.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="str">    Modified from black.files.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="key">if</span> <span class="nam">stdin_filename</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">srcs</span> <span class="op">=</span> <span class="nam">tuple</span><span class="op">(</span><span class="nam">stdin_filename</span> <span class="key">if</span> <span class="nam">s</span> <span class="op">==</span> <span class="str">"-"</span> <span class="key">else</span> <span class="nam">s</span> <span class="key">for</span> <span class="nam">s</span> <span class="key">in</span> <span class="nam">srcs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">srcs</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="nam">srcs</span> <span class="op">=</span> <span class="op">[</span><span class="nam">str</span><span class="op">(</span><span class="nam">Path</span><span class="op">.</span><span class="nam">cwd</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">resolve</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="op">@</span><span class="nam">register</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="key">def</span> <span class="nam">install_svelte_check</span><span class="op">(</span><span class="nam">target_dir</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="str">    Install the svelte-check tool using npm.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="nam">config</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">target</span><span class="op">=</span><span class="nam">target_dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="key">with</span> <span class="nam">chdir</span><span class="op">(</span><span class="nam">config</span><span class="op">.</span><span class="nam">target</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="key">return</span> <span class="nam">run_tool</span><span class="op">(</span><span class="str">"npm"</span><span class="op">,</span> <span class="str">"install"</span><span class="op">,</span> <span class="str">"svelte-check"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="nam">path_srcs</span> <span class="op">=</span> <span class="op">[</span><span class="nam">Path</span><span class="op">(</span><span class="nam">Path</span><span class="op">.</span><span class="nam">cwd</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">src</span><span class="op">)</span><span class="op">.</span><span class="nam">resolve</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">src</span> <span class="key">in</span> <span class="nam">srcs</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="com"># A list of lists of parents for each 'src'. 'src' is included as a</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="com"># "parent" of itself if it is a directory</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="nam">src_parents</span> <span class="op">=</span> <span class="op">[</span><span class="nam">list</span><span class="op">(</span><span class="nam">path</span><span class="op">.</span><span class="nam">parents</span><span class="op">)</span> <span class="op">+</span> <span class="op">(</span><span class="op">[</span><span class="nam">path</span><span class="op">]</span> <span class="key">if</span> <span class="nam">path</span><span class="op">.</span><span class="nam">is_dir</span><span class="op">(</span><span class="op">)</span> <span class="key">else</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span> <span class="key">for</span> <span class="nam">path</span> <span class="key">in</span> <span class="nam">path_srcs</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="nam">common_base</span> <span class="op">=</span> <span class="nam">max</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">        <span class="nam">set</span><span class="op">.</span><span class="nam">intersection</span><span class="op">(</span><span class="op">*</span><span class="op">(</span><span class="nam">set</span><span class="op">(</span><span class="nam">parents</span><span class="op">)</span> <span class="key">for</span> <span class="nam">parents</span> <span class="key">in</span> <span class="nam">src_parents</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">        <span class="nam">key</span><span class="op">=</span><span class="key">lambda</span> <span class="nam">path</span><span class="op">:</span> <span class="nam">path</span><span class="op">.</span><span class="nam">parts</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="op">@</span><span class="nam">register</span><span class="op">(</span><span class="nam">add_to_all</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="key">def</span> <span class="nam">svelte_check</span><span class="op">(</span><span class="nam">target</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">tsconfig</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">node_modules</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="str">    Run the svelte-check tool.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="nam">config</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">,</span> <span class="nam">tsconfig</span><span class="op">=</span><span class="nam">tsconfig</span><span class="op">,</span> <span class="nam">target</span><span class="op">=</span><span class="nam">target</span><span class="op">,</span> <span class="nam">node_modules</span><span class="op">=</span><span class="nam">node_modules</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="com"># svelte-check --tsconfig ./tsconfig.json --threshold error</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="nam">root</span><span class="op">,</span> <span class="nam">_</span> <span class="op">=</span> <span class="nam">find_project_root</span><span class="op">(</span><span class="op">(</span><span class="nam">config</span><span class="op">.</span><span class="nam">node_modules</span><span class="op">,</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="nam">executable</span> <span class="op">=</span> <span class="nam">str</span><span class="op">(</span><span class="nam">root</span> <span class="op">/</span> <span class="str">"node_modules/svelte-check/bin/svelte-check"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="key">for</span> <span class="nam">directory</span> <span class="key">in</span> <span class="op">(</span><span class="nam">common_base</span><span class="op">,</span> <span class="op">*</span><span class="nam">common_base</span><span class="op">.</span><span class="nam">parents</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">directory</span> <span class="op">/</span> <span class="str">"node_modules"</span><span class="op">)</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">            <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">"node_modules"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">directory</span> <span class="op">/</span> <span class="str">".git"</span><span class="op">)</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">            <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">".git directory"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">directory</span> <span class="op">/</span> <span class="str">".hg"</span><span class="op">)</span><span class="op">.</span><span class="nam">is_dir</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">            <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">".hg directory"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="key">if</span> <span class="op">(</span><span class="nam">directory</span> <span class="op">/</span> <span class="str">"pyproject.toml"</span><span class="op">)</span><span class="op">.</span><span class="nam">is_file</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">            <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">"pyproject.toml"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="key">return</span> <span class="nam">directory</span><span class="op">,</span> <span class="str">"file system root"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t"><span class="nam">__all__</span> <span class="op">=</span> <span class="op">[</span><span class="str">"chdir"</span><span class="op">,</span> <span class="str">"find_project_root"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="nam">args</span> <span class="op">=</span> <span class="op">[</span><span class="str">"--workspace"</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">target</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="key">if</span> <span class="nam">config</span><span class="op">.</span><span class="nam">strict</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="str">"--fail-on-warnings"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="op">[</span><span class="str">"--threshold"</span><span class="op">,</span> <span class="str">"error"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">    <span class="key">if</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">config</span><span class="op">.</span><span class="nam">tsconfig</span><span class="op">)</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="op">[</span><span class="str">"--tsconfig"</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">tsconfig</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="key">return</span> <span class="nam">run_tool</span><span class="op">(</span><span class="nam">executable</span><span class="op">,</span> <span class="op">*</span><span class="nam">args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_a80ff4318293920f_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_a80ff4318293920f___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_a80ff4318293920f_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-17 17:28 +0200
+            created at 2023-07-17 18:23 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,86 +1,79 @@
 
-****** Coverage for src/su6_plugin_svelte_check/helpers.py: 100% ******
+****** Coverage for src/su6_plugin_svelte_check/cli.py: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 24 statements   24 run 0 missing 4 excluded *****
+***** 27 statements   27 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-17 17:28 +0200
+at 2023-07-17 18:23 +0200
 
 
 1""" 
-2Re-usable helpers for this project. 
+2This module contains an example of both methods of adding commands to su6. 
 3""" 
-4 
-5import contextlib 
-6from functools import lru_cache 
-7from pathlib import Path 
-8from typing import Optional, Sequence, Tuple 
+4from pathlib import Path 
+5 
+6from su6.plugins import PluginConfig, register, run_tool 
+7 
+8from .helpers import chdir, find_project_root 
 9 
-10try: 
-11 chdir = contextlib.chdir 
-12except AttributeError: 
-13 from contextlib_chdir import chdir # type: ignore 
-14 
-15 
-16@lru_cache() 
-17def find_project_root(srcs: Sequence[str], stdin_filename: Optional[str] =
-None) -> Tuple[Path, str]: 
-18 """ 
-19 Return a directory containing .git, .hg, or pyproject.toml. 
-20 
-21 That directory will be a common parent of all files and directories 
-22 passed in `srcs`. 
+10 
+11@register 
+12class SvelteCheckPluginConfig(PluginConfig): 
+13 """ 
+14 Config without state, loads [tool.su6.demo] from pyproject.toml into self. 
+15 """ 
+16 
+17 target: str = "." 
+18 node_modules: str = "./node_modules" 
+19 
+20 strict: bool = False 
+21 tsconfig: str = "./tsconfig.json" 
+22 
 23 
-24 If no directory in the tree contains a marker that would specify it's the 
-25 project root, the root of the file system is returned. 
+24config = SvelteCheckPluginConfig() 
+25 
 26 
-27 Returns a two-tuple with the first element as the project root path and 
-28 the second element as a string describing the method by which the 
-29 project root was discovered. 
-30 
-31 Modified from black.files. 
-32 """ 
-33 if stdin_filename is not None: 
-34 srcs = tuple(stdin_filename if s == "-" else s for s in srcs) 
-35 if not srcs: 
-36 srcs = [str(Path.cwd().resolve())] 
+27@register 
+28def install_svelte_check(target_dir: str = None) -> int: 
+29 """ 
+30 Install the svelte-check tool using npm. 
+31 """ 
+32 config.update(target=target_dir) 
+33 
+34 with chdir(config.target): 
+35 return run_tool("npm", "install", "svelte-check") 
+36 
 37 
-38 path_srcs = [Path(Path.cwd(), src).resolve() for src in srcs] 
-39 
-40 # A list of lists of parents for each 'src'. 'src' is included as a 
-41 # "parent" of itself if it is a directory 
-42 src_parents = [list(path.parents) + ([path] if path.is_dir() else []) for
-path in path_srcs] 
-43 
-44 common_base = max( 
-45 set.intersection(*(set(parents) for parents in src_parents)), 
-46 key=lambda path: path.parts, 
-47 ) 
+38@register(add_to_all=True) 
+39def svelte_check(target: str = None, strict: bool = None, tsconfig: str =
+None, node_modules: str = None) -> int: 
+40 """ 
+41 Run the svelte-check tool. 
+42 """ 
+43 config.update(strict=strict, tsconfig=tsconfig, target=target,
+node_modules=node_modules) 
+44 # svelte-check --tsconfig ./tsconfig.json --threshold error 
+45 
+46 root, _ = find_project_root((config.node_modules,)) 
+47 executable = str(root / "node_modules/svelte-check/bin/svelte-check") 
 48 
-49 for directory in (common_base, *common_base.parents): 
-50 if (directory / "node_modules").exists(): 
-51 return directory, "node_modules" 
-52 
-53 if (directory / ".git").exists(): 
-54 return directory, ".git directory" 
-55 
-56 if (directory / ".hg").is_dir(): # pragma: no cover 
-57 return directory, ".hg directory" 
-58 
-59 if (directory / "pyproject.toml").is_file(): # pragma: no cover 
-60 return directory, "pyproject.toml" 
-61 
-62 return directory, "file system root" 
-63 
-64 
-65__all__ = ["chdir", "find_project_root"] 
+49 args = ["--workspace", config.target] 
+50 if config.strict: 
+51 args.append("--fail-on-warnings") 
+52 else: 
+53 args.extend(["--threshold", "error"]) 
+54 
+55 if Path(config.tsconfig).exists(): 
+56 args.extend(["--tsconfig", config.tsconfig]) 
+57 
+58 return run_tool(executable, *args) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-17 17:28 +0200
+at 2023-07-17 18:23 +0200
```

### Comparing `su6_plugin_svelte_check-0.4.0/htmlcov/favicon_32.png` & `su6_plugin_svelte_check-0.5.0/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.4.0/htmlcov/index.html` & `su6_plugin_svelte_check-0.5.0/htmlcov/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-17 17:31 +0200
+            created at 2023-07-17 18:34 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -73,46 +73,46 @@
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_a80ff4318293920f_cli_py.html">src/su6_plugin_svelte_check/cli.py</a></td>
-                <td>26</td>
+                <td>27</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="26 26">100%</td>
+                <td class="right" data-ratio="27 27">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_a80ff4318293920f_helpers_py.html">src/su6_plugin_svelte_check/helpers.py</a></td>
-                <td>24</td>
+                <td>22</td>
                 <td>0</td>
-                <td>4</td>
-                <td class="right" data-ratio="24 24">100%</td>
+                <td>6</td>
+                <td class="right" data-ratio="22 22">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>51</td>
+                <td>50</td>
                 <td>0</td>
-                <td>4</td>
-                <td class="right" data-ratio="51 51">100%</td>
+                <td>6</td>
+                <td class="right" data-ratio="50 50">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-17 17:31 +0200
+            created at 2023-07-17 18:34 +0200
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_a80ff4318293920f_helpers_py.html"/>
         <a id="nextFileLink" class="nav" href="d_a80ff4318293920f___about___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -2,19 +2,19 @@
 ****** Coverage report: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-07-17 17:31 +0200
+coverage.py_v7.2.7, created at 2023-07-17 18:34 +0200
 
 Module                                   statements missing excluded coverage
 src/su6_plugin_svelte_check/__about__.py 1          0       0        100%
 src/su6_plugin_svelte_check/__init__.py  0          0       0        100%
-src/su6_plugin_svelte_check/cli.py       26         0       0        100%
-src/su6_plugin_svelte_check/helpers.py   24         0       4        100%
-Total                                    51         0       4        100%
+src/su6_plugin_svelte_check/cli.py       27         0       0        100%
+src/su6_plugin_svelte_check/helpers.py   22         0       6        100%
+Total                                    50         0       6        100%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-07-17 17:31 +0200
+coverage.py_v7.2.7, created at 2023-07-17 18:34 +0200
  ____
```

### Comparing `su6_plugin_svelte_check-0.4.0/htmlcov/keybd_closed.png` & `su6_plugin_svelte_check-0.5.0/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.4.0/htmlcov/keybd_open.png` & `su6_plugin_svelte_check-0.5.0/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.4.0/htmlcov/status.json` & `su6_plugin_svelte_check-0.5.0/htmlcov/status.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9934259259259259%*

 * *Differences: {"'files'": "{'d_a80ff4318293920f_cli_py': {'hash': '04dc6db6661f695785fe0e9f128799b9', 'index': "*

 * *            "{'nums': {insert: [(2, 27)], delete: [2]}}}, 'd_a80ff4318293920f_helpers_py': "*

 * *            "{'hash': '058000648d7c634847a6bafbfc2cf18a', 'index': {'nums': {insert: [(2, 22), (3, "*

 * *            '6)], delete: [3, 2]}}}}'}*

```diff
@@ -31,21 +31,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/su6_plugin_svelte_check/__init__.py"
             }
         },
         "d_a80ff4318293920f_cli_py": {
-            "hash": "45da77e06bcdd0a07714e422db7551cf",
+            "hash": "04dc6db6661f695785fe0e9f128799b9",
             "index": {
                 "html_filename": "d_a80ff4318293920f_cli_py.html",
                 "nums": [
                     0,
                     1,
-                    26,
+                    27,
                     0,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/su6_plugin_svelte_check/cli.py"
@@ -65,22 +65,22 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/su6_plugin_svelte_check/find_project_root.py"
             }
         },
         "d_a80ff4318293920f_helpers_py": {
-            "hash": "f973faa922c34b21dd0f94385e1521c5",
+            "hash": "058000648d7c634847a6bafbfc2cf18a",
             "index": {
                 "html_filename": "d_a80ff4318293920f_helpers_py.html",
                 "nums": [
                     0,
                     1,
-                    24,
-                    4,
+                    22,
+                    6,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/su6_plugin_svelte_check/helpers.py"
             }
```

### Comparing `su6_plugin_svelte_check-0.4.0/htmlcov/style.css` & `su6_plugin_svelte_check-0.5.0/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.4.0/pytest_examples/package-lock.json` & `su6_plugin_svelte_check-0.5.0/pytest_examples/package-lock.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.4.0/src/su6_plugin_svelte_check/cli.py` & `su6_plugin_svelte_check-0.5.0/src/su6_plugin_svelte_check/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,45 +10,47 @@
 
 @register
 class SvelteCheckPluginConfig(PluginConfig):
     """
     Config without state, loads [tool.su6.demo] from pyproject.toml into self.
     """
 
+    target: str = "."
+    node_modules: str = "./node_modules"
+
     strict: bool = False
     tsconfig: str = "./tsconfig.json"
 
 
 config = SvelteCheckPluginConfig()
 
 
 @register
 def install_svelte_check(target_dir: str = None) -> int:
     """
     Install the svelte-check tool using npm.
     """
-    target_dir = target_dir or "./"
+    config.update(target=target_dir)
 
-    with chdir(target_dir):
+    with chdir(config.target):
         return run_tool("npm", "install", "svelte-check")
 
 
 @register(add_to_all=True)
-def svelte_check(strict: bool = None, tsconfig: str = None, node_modules: str = None) -> int:
+def svelte_check(target: str = None, strict: bool = None, tsconfig: str = None, node_modules: str = None) -> int:
     """
     Run the svelte-check tool.
     """
-    config.update(strict=strict, tsconfig=tsconfig)
+    config.update(strict=strict, tsconfig=tsconfig, target=target, node_modules=node_modules)
     # svelte-check --tsconfig ./tsconfig.json --threshold error
 
-    node_modules = node_modules or "node_modules"
-    root, _ = find_project_root((node_modules,))
+    root, _ = find_project_root((config.node_modules,))
     executable = str(root / "node_modules/svelte-check/bin/svelte-check")
 
-    args = []
+    args = ["--workspace", config.target]
     if config.strict:
         args.append("--fail-on-warnings")
     else:
         args.extend(["--threshold", "error"])
 
     if Path(config.tsconfig).exists():
         args.extend(["--tsconfig", config.tsconfig])
```

### Comparing `su6_plugin_svelte_check-0.4.0/src/su6_plugin_svelte_check/helpers.py` & `su6_plugin_svelte_check-0.5.0/src/su6_plugin_svelte_check/helpers.py`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.4.0/tests/test_find_project_root.py` & `su6_plugin_svelte_check-0.5.0/tests/test_find_project_root.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 import contextlib
 from pathlib import Path
 
-from src.su6_plugin_svelte_check.helpers import find_project_root
-
-try:
-    chdir = contextlib.chdir
-except AttributeError:
-    from contextlib_chdir import chdir
+from src.su6_plugin_svelte_check.helpers import find_project_root, chdir
 
 
 def test_find_project_root_node_modules():
     with chdir("./pytest_examples/no_issues"):
         path, reason = find_project_root(tuple(), "")
         assert path.exists() and str(path.resolve()) == str(Path("../").resolve())
         assert reason == "node_modules"
```

### Comparing `su6_plugin_svelte_check-0.4.0/tests/test_plugin.py` & `su6_plugin_svelte_check-0.5.0/tests/test_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import contextlib
+import os
 import shutil
 from pathlib import Path
 
 from su6 import app
 from typer.testing import CliRunner
 from plumbum import local
 
@@ -38,32 +39,45 @@
     assert result.exit_code == 1
 
 
 def test_no_issues():
     with chdir("./pytest_examples"):
         prepare_env()
 
-        result = runner.invoke(app, ["svelte-check", "--tsconfig", "./tsconfig-no_issues.json"])
+        result = runner.invoke(app, ["svelte-check", "--target", "./no_issues"])
         print(result.stdout, result.stderr)
         assert result.exit_code == 0
 
 
 def test_issues():
     with chdir("./pytest_examples"):
         prepare_env()
 
-        result = runner.invoke(app, ["svelte-check", "--tsconfig", "./tsconfig-issues.json"])
+        result = runner.invoke(app, ["svelte-check", "--target", "./issues"])
         print(result.stdout, result.stderr)
         assert result.exit_code == 1
 
 
 def test_warnings():
     with chdir("./pytest_examples"):
         prepare_env()
 
-        result = runner.invoke(app, ["svelte-check", "--tsconfig", "./tsconfig-warnings.json"])
+        result = runner.invoke(app, ["svelte-check", "--target", "./warnings"])
         print(result.stdout, result.stderr)
         assert result.exit_code == 0
 
-        result = runner.invoke(app, ["svelte-check", "--tsconfig", "./tsconfig-warnings.json", "--strict"])
+        result = runner.invoke(app, ["svelte-check", "--target", "./warnings", "--strict"])
+        print(result.stdout, result.stderr)
+        assert result.exit_code == 1
+
+
+def test_custom_tsconfig():
+    with chdir("./pytest_examples"):
+        prepare_env()
+
+        result = runner.invoke(app, ["svelte-check", "--target", ".", "--tsconfig", "custom_tsconfig.json", "--no-strict"])
+        print(result.stdout, result.stderr)
+        assert result.exit_code == 0
+
+        result = runner.invoke(app, ["svelte-check", "--tsconfig", "custom_tsconfig.json", "--strict"])
         print(result.stdout, result.stderr)
         assert result.exit_code == 1
```

### Comparing `su6_plugin_svelte_check-0.4.0/LICENSE.txt` & `su6_plugin_svelte_check-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.4.0/pyproject.toml` & `su6_plugin_svelte_check-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,23 @@
 upload_to_repository = false
 upload_to_release = false
 build_command = "hatch build"
 
 [tool.su6]
 directory = "src"
 include = []
-exclude = ["svelte-check"] # ironic
+exclude = []
 stop-after-first-failure = true
 coverage = 100
 badge = true
 
+[tool.su6.svelte-check]
+target = "pytest_examples/no_issues"
+node_modules = "pytest_examples/node_modules"
+
 [tool.black]
 target-version = ["py311"]
 line-length = 120
 # 'extend-exclude' excludes files or directories in addition to the defaults
 extend-exclude = '''
 # A regex preceded with ^/ will apply only to files and directories
 # in the root of the project.
```

### Comparing `su6_plugin_svelte_check-0.4.0/PKG-INFO` & `su6_plugin_svelte_check-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: su6-plugin-svelte-check
-Version: 0.4.0
+Version: 0.5.0
 Summary: Svelte-check plugin for `su6`
 Project-URL: Documentation, https://github.com/robinvandernoord/su6-plugin-svelte-check#readme
 Project-URL: Issues, https://github.com/robinvandernoord/su6-plugin-svelte-check/issues
 Project-URL: Source, https://github.com/robinvandernoord/su6-plugin-svelte-check
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

