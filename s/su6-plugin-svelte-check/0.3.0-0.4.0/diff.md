# Comparing `tmp/su6_plugin_svelte_check-0.3.0.tar.gz` & `tmp/su6_plugin_svelte_check-0.4.0.tar.gz`

## Comparing `su6_plugin_svelte_check-0.3.0.tar` & `su6_plugin_svelte_check-0.4.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/coverage.svg
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/.github/workflows/su6.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/d_a80ff4318293920f___about___py.html
--rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/d_a80ff4318293920f___init___py.html
--rw-r--r--   0        0        0    15560 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/d_a80ff4318293920f_cli_py.html
--rw-r--r--   0        0        0    19618 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/d_a80ff4318293920f_find_project_root_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/htmlcov/style.css
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/.gitignore
--rw-r--r--   0        0        0    32309 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/package-lock.json
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/package.json
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/tsconfig-issues.json
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/tsconfig-no_issues.json
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/tsconfig-warnings.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/issues/index.svelte
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/no_issues/index.svelte
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pytest_examples/warnings/index.svelte
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/src/su6_plugin_svelte_check/__about__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/src/su6_plugin_svelte_check/__init__.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/src/su6_plugin_svelte_check/cli.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/src/su6_plugin_svelte_check/find_project_root.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/tests/test_about.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/tests/test_find_project_root.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/tests/test_plugin.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/README.md
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/coverage.svg
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/.github/workflows/su6.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f___about___py.html
+-rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f___init___py.html
+-rw-r--r--   0        0        0    18443 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f_cli_py.html
+-rw-r--r--   0        0        0    19618 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f_find_project_root_py.html
+-rw-r--r--   0        0        0    21967 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f_helpers_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/htmlcov/style.css
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/.gitignore
+-rw-r--r--   0        0        0    32309 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/package-lock.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/package.json
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/tsconfig-issues.json
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/tsconfig-no_issues.json
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/tsconfig-warnings.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/issues/index.svelte
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/no_issues/index.svelte
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pytest_examples/warnings/index.svelte
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/src/su6_plugin_svelte_check/__about__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/src/su6_plugin_svelte_check/__init__.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/src/su6_plugin_svelte_check/cli.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/src/su6_plugin_svelte_check/helpers.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/tests/test_about.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/tests/test_find_project_root.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/tests/test_plugin.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/README.md
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 su6_plugin_svelte_check-0.4.0/PKG-INFO
```

### Comparing `su6_plugin_svelte_check-0.3.0/CHANGELOG.md` & `su6_plugin_svelte_check-0.4.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.4.0 (2023-07-17)
+### Feature
+* Add install-svelte-check command ([`84630d2`](https://github.com/robinvandernoord/su6-plugin-svelte-check/commit/84630d254fd1946d5789f50a427d29024f41b227))
+
 ## v0.3.0 (2023-07-17)
 ### Feature
 * Allow specifying a custom --node-modules directory which should have `svelte-check` ([`db1dc42`](https://github.com/robinvandernoord/su6-plugin-svelte-check/commit/db1dc42720e7f94020249b6859097b3cb541cda0))
 
 ## v0.2.2 (2023-07-17)
 ### Fix
 * Don't include node modules in git!! ([`360325c`](https://github.com/robinvandernoord/su6-plugin-svelte-check/commit/360325c02ed99fb34519941061e9b78679601d61))
```

### Comparing `su6_plugin_svelte_check-0.3.0/coverage.svg` & `su6_plugin_svelte_check-0.4.0/coverage.svg`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.3.0/htmlcov/coverage_html.js` & `su6_plugin_svelte_check-0.4.0/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.3.0/htmlcov/d_a80ff4318293920f___about___py.html` & `su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f___about___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a80ff4318293920f___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-17 14:04 +0200
+            created at 2023-07-17 17:31 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -83,23 +83,23 @@
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">This file contains the module version.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># SPDX-FileCopyrightText: 2023-present Robin van der Noord &lt;robinvandernoord@gmail.com></span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.1.0"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.4.0"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a80ff4318293920f___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-17 14:04 +0200
+            created at 2023-07-17 17:31 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,22 +7,22 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 1 statements   1 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-17 14:04 +0200
+at 2023-07-17 17:31 +0200
 
 
 1""" 
 2This file contains the module version. 
 3""" 
 4 
 5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
 <robinvandernoord@gmail.com> 
 6# 
 7# SPDX-License-Identifier: MIT 
-8__version__ = "0.1.0" 
+8__version__ = "0.4.0" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-17 14:04 +0200
+at 2023-07-17 17:31 +0200
```

### Comparing `su6_plugin_svelte_check-0.3.0/htmlcov/d_a80ff4318293920f___init___py.html` & `su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f___init___py.html`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.3.0/htmlcov/d_a80ff4318293920f_cli_py.html` & `su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f_cli_py.html`

 * *Files 8% similar despite different names*

```diff
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">20 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">20<span class="text"> run</span></button>
+            <span class="text">26 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">26<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a80ff4318293920f___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_a80ff4318293920f_find_project_root_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_a80ff4318293920f_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-17 14:04 +0200
+            created at 2023-07-17 17:28 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -83,15 +83,15 @@
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">This module contains an example of both methods of adding commands to su6.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">su6</span><span class="op">.</span><span class="nam">plugins</span> <span class="key">import</span> <span class="nam">PluginConfig</span><span class="op">,</span> <span class="nam">register</span><span class="op">,</span> <span class="nam">run_tool</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">find_project_root</span> <span class="key">import</span> <span class="nam">find_project_root</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">chdir</span><span class="op">,</span> <span class="nam">find_project_root</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="op">@</span><span class="nam">register</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">class</span> <span class="nam">SvelteCheckPluginConfig</span><span class="op">(</span><span class="nam">PluginConfig</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">    Config without state, loads [tool.su6.demo] from pyproject.toml into self.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
@@ -99,44 +99,55 @@
     <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="nam">tsconfig</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"./tsconfig.json"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="nam">config</span> <span class="op">=</span> <span class="nam">SvelteCheckPluginConfig</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="op">@</span><span class="nam">register</span><span class="op">(</span><span class="nam">add_to_all</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="key">def</span> <span class="nam">svelte_check</span><span class="op">(</span><span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">tsconfig</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="op">@</span><span class="nam">register</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="key">def</span> <span class="nam">install_svelte_check</span><span class="op">(</span><span class="nam">target_dir</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="str">    Register a top-level command.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="str">    @register works without ()</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="nam">config</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">,</span> <span class="nam">tsconfig</span><span class="op">=</span><span class="nam">tsconfig</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="com"># svelte-check --tsconfig ./tsconfig.json --threshold error</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="nam">root</span><span class="op">,</span> <span class="nam">_</span> <span class="op">=</span> <span class="nam">find_project_root</span><span class="op">(</span><span class="op">(</span><span class="str">"node_modules"</span><span class="op">,</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="nam">executable</span> <span class="op">=</span> <span class="nam">str</span><span class="op">(</span><span class="nam">root</span> <span class="op">/</span> <span class="str">"node_modules/svelte-check/bin/svelte-check"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="nam">args</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">if</span> <span class="nam">config</span><span class="op">.</span><span class="nam">strict</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="str">"--fail-on-warnings"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="op">[</span><span class="str">"--threshold"</span><span class="op">,</span> <span class="str">"error"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="key">if</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">config</span><span class="op">.</span><span class="nam">tsconfig</span><span class="op">)</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="op">[</span><span class="str">"--tsconfig"</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">tsconfig</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="key">return</span> <span class="nam">run_tool</span><span class="op">(</span><span class="nam">executable</span><span class="op">,</span> <span class="op">*</span><span class="nam">args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="str">    Install the svelte-check tool using npm.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="nam">target_dir</span> <span class="op">=</span> <span class="nam">target_dir</span> <span class="key">or</span> <span class="str">"./"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="key">with</span> <span class="nam">chdir</span><span class="op">(</span><span class="nam">target_dir</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="key">return</span> <span class="nam">run_tool</span><span class="op">(</span><span class="str">"npm"</span><span class="op">,</span> <span class="str">"install"</span><span class="op">,</span> <span class="str">"svelte-check"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t"><span class="op">@</span><span class="nam">register</span><span class="op">(</span><span class="nam">add_to_all</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t"><span class="key">def</span> <span class="nam">svelte_check</span><span class="op">(</span><span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">tsconfig</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">node_modules</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="str">    Run the svelte-check tool.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="nam">config</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">,</span> <span class="nam">tsconfig</span><span class="op">=</span><span class="nam">tsconfig</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="com"># svelte-check --tsconfig ./tsconfig.json --threshold error</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="nam">node_modules</span> <span class="op">=</span> <span class="nam">node_modules</span> <span class="key">or</span> <span class="str">"node_modules"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="nam">root</span><span class="op">,</span> <span class="nam">_</span> <span class="op">=</span> <span class="nam">find_project_root</span><span class="op">(</span><span class="op">(</span><span class="nam">node_modules</span><span class="op">,</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="nam">executable</span> <span class="op">=</span> <span class="nam">str</span><span class="op">(</span><span class="nam">root</span> <span class="op">/</span> <span class="str">"node_modules/svelte-check/bin/svelte-check"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="nam">args</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="key">if</span> <span class="nam">config</span><span class="op">.</span><span class="nam">strict</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="str">"--fail-on-warnings"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="op">[</span><span class="str">"--threshold"</span><span class="op">,</span> <span class="str">"error"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="key">if</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">config</span><span class="op">.</span><span class="nam">tsconfig</span><span class="op">)</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="op">[</span><span class="str">"--tsconfig"</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">tsconfig</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="key">return</span> <span class="nam">run_tool</span><span class="op">(</span><span class="nam">executable</span><span class="op">,</span> <span class="op">*</span><span class="nam">args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a80ff4318293920f___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_a80ff4318293920f_find_project_root_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_a80ff4318293920f_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-17 14:04 +0200
+            created at 2023-07-17 17:28 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,27 +5,27 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 20 statements   20 run 0 missing 0 excluded *****
+***** 26 statements   26 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-17 14:04 +0200
+at 2023-07-17 17:28 +0200
 
 
 1""" 
 2This module contains an example of both methods of adding commands to su6. 
 3""" 
 4from pathlib import Path 
 5 
 6from su6.plugins import PluginConfig, register, run_tool 
 7 
-8from .find_project_root import find_project_root 
+8from .helpers import chdir, find_project_root 
 9 
 10 
 11@register 
 12class SvelteCheckPluginConfig(PluginConfig): 
 13 """ 
 14 Config without state, loads [tool.su6.demo] from pyproject.toml into self. 
 15 """ 
@@ -33,32 +33,44 @@
 17 strict: bool = False 
 18 tsconfig: str = "./tsconfig.json" 
 19 
 20 
 21config = SvelteCheckPluginConfig() 
 22 
 23 
-24@register(add_to_all=True) 
-25def svelte_check(strict: bool = None, tsconfig: str = None) -> int: 
+24@register 
+25def install_svelte_check(target_dir: str = None) -> int: 
 26 """ 
-27 Register a top-level command. 
-28 
-29 @register works without () 
-30 """ 
-31 config.update(strict=strict, tsconfig=tsconfig) 
-32 # svelte-check --tsconfig ./tsconfig.json --threshold error 
-33 root, _ = find_project_root(("node_modules",)) 
-34 executable = str(root / "node_modules/svelte-check/bin/svelte-check") 
-35 
-36 args = [] 
-37 if config.strict: 
-38 args.append("--fail-on-warnings") 
-39 else: 
-40 args.extend(["--threshold", "error"]) 
-41 
-42 if Path(config.tsconfig).exists(): 
-43 args.extend(["--tsconfig", config.tsconfig]) 
-44 
-45 return run_tool(executable, *args) 
+27 Install the svelte-check tool using npm. 
+28 """ 
+29 target_dir = target_dir or "./" 
+30 
+31 with chdir(target_dir): 
+32 return run_tool("npm", "install", "svelte-check") 
+33 
+34 
+35@register(add_to_all=True) 
+36def svelte_check(strict: bool = None, tsconfig: str = None, node_modules: str
+= None) -> int: 
+37 """ 
+38 Run the svelte-check tool. 
+39 """ 
+40 config.update(strict=strict, tsconfig=tsconfig) 
+41 # svelte-check --tsconfig ./tsconfig.json --threshold error 
+42 
+43 node_modules = node_modules or "node_modules" 
+44 root, _ = find_project_root((node_modules,)) 
+45 executable = str(root / "node_modules/svelte-check/bin/svelte-check") 
+46 
+47 args = [] 
+48 if config.strict: 
+49 args.append("--fail-on-warnings") 
+50 else: 
+51 args.extend(["--threshold", "error"]) 
+52 
+53 if Path(config.tsconfig).exists(): 
+54 args.extend(["--tsconfig", config.tsconfig]) 
+55 
+56 return run_tool(executable, *args) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-07-17 14:04 +0200
+at 2023-07-17 17:28 +0200
```

### Comparing `su6_plugin_svelte_check-0.3.0/htmlcov/d_a80ff4318293920f_find_project_root_py.html` & `su6_plugin_svelte_check-0.4.0/htmlcov/d_a80ff4318293920f_find_project_root_py.html`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.3.0/htmlcov/favicon_32.png` & `su6_plugin_svelte_check-0.4.0/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.3.0/htmlcov/index.html` & `su6_plugin_svelte_check-0.4.0/htmlcov/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-07-17 14:04 +0200
+            created at 2023-07-17 17:31 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -73,50 +73,50 @@
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_a80ff4318293920f_cli_py.html">src/su6_plugin_svelte_check/cli.py</a></td>
-                <td>20</td>
+                <td>26</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="20 20">100%</td>
+                <td class="right" data-ratio="26 26">100%</td>
             </tr>
             <tr class="file">
-                <td class="name left"><a href="d_a80ff4318293920f_find_project_root_py.html">src/su6_plugin_svelte_check/find_project_root.py</a></td>
-                <td>18</td>
+                <td class="name left"><a href="d_a80ff4318293920f_helpers_py.html">src/su6_plugin_svelte_check/helpers.py</a></td>
+                <td>24</td>
                 <td>0</td>
                 <td>4</td>
-                <td class="right" data-ratio="18 18">100%</td>
+                <td class="right" data-ratio="24 24">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>39</td>
+                <td>51</td>
                 <td>0</td>
                 <td>4</td>
-                <td class="right" data-ratio="39 39">100%</td>
+                <td class="right" data-ratio="51 51">100%</td>
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
-            created at 2023-07-17 14:04 +0200
+            created at 2023-07-17 17:31 +0200
         </p>
     </div>
     <aside class="hidden">
-        <a id="prevFileLink" class="nav" href="d_a80ff4318293920f_find_project_root_py.html"/>
+        <a id="prevFileLink" class="nav" href="d_a80ff4318293920f_helpers_py.html"/>
         <a id="nextFileLink" class="nav" href="d_a80ff4318293920f___about___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
         <button type="button" class="button_show_hide_help" data-shortcut="?"/>
     </aside>
 </footer>
 </body>
```

#### html2text {}

```diff
@@ -2,20 +2,19 @@
 ****** Coverage report: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-07-17 14:04 +0200
+coverage.py_v7.2.7, created at 2023-07-17 17:31 +0200
 
 Module                                   statements missing excluded coverage
 src/su6_plugin_svelte_check/__about__.py 1          0       0        100%
 src/su6_plugin_svelte_check/__init__.py  0          0       0        100%
-src/su6_plugin_svelte_check/cli.py       20         0       0        100%
-src/su6_plugin_svelte_check/             18         0       4        100%
-find_project_root.py
-Total                                    39         0       4        100%
+src/su6_plugin_svelte_check/cli.py       26         0       0        100%
+src/su6_plugin_svelte_check/helpers.py   24         0       4        100%
+Total                                    51         0       4        100%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-07-17 14:04 +0200
+coverage.py_v7.2.7, created at 2023-07-17 17:31 +0200
  ____
```

### Comparing `su6_plugin_svelte_check-0.3.0/htmlcov/keybd_closed.png` & `su6_plugin_svelte_check-0.4.0/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.3.0/htmlcov/keybd_open.png` & `su6_plugin_svelte_check-0.4.0/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.3.0/htmlcov/status.json` & `su6_plugin_svelte_check-0.4.0/htmlcov/status.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9686342592592593%*

 * *Differences: {"'files'": "{'d_a80ff4318293920f___about___py': {'hash': '1e16d0a5be4c6d956997203e73b239ce'}, "*

 * *            "'d_a80ff4318293920f_cli_py': {'hash': '45da77e06bcdd0a07714e422db7551cf', 'index': "*

 * *            "{'nums': {insert: [(2, 26)], delete: [2]}}}, 'd_a80ff4318293920f_helpers_py': "*

 * *            "OrderedDict([('hash', 'f973faa922c34b21dd0f94385e1521c5'), ('index', "*

 * *            "OrderedDict([('nums', [0, 1, 24, 4, 0, 0, 0, 0]), ('html_filename', "*

 * *            "'d_a80ff4318293920f_helpers_py.html'), ('rel […]*

```diff
@@ -1,11 +1,11 @@
 {
     "files": {
         "d_a80ff4318293920f___about___py": {
-            "hash": "5488b5f3b6de41d6f8f0220908652475",
+            "hash": "1e16d0a5be4c6d956997203e73b239ce",
             "index": {
                 "html_filename": "d_a80ff4318293920f___about___py.html",
                 "nums": [
                     0,
                     1,
                     1,
                     0,
@@ -31,21 +31,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/su6_plugin_svelte_check/__init__.py"
             }
         },
         "d_a80ff4318293920f_cli_py": {
-            "hash": "452b384877a0b5e480b840f5b4a905b9",
+            "hash": "45da77e06bcdd0a07714e422db7551cf",
             "index": {
                 "html_filename": "d_a80ff4318293920f_cli_py.html",
                 "nums": [
                     0,
                     1,
-                    20,
+                    26,
                     0,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/su6_plugin_svelte_check/cli.py"
@@ -63,13 +63,30 @@
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/su6_plugin_svelte_check/find_project_root.py"
             }
+        },
+        "d_a80ff4318293920f_helpers_py": {
+            "hash": "f973faa922c34b21dd0f94385e1521c5",
+            "index": {
+                "html_filename": "d_a80ff4318293920f_helpers_py.html",
+                "nums": [
+                    0,
+                    1,
+                    24,
+                    4,
+                    0,
+                    0,
+                    0,
+                    0
+                ],
+                "relative_filename": "src/su6_plugin_svelte_check/helpers.py"
+            }
         }
     },
     "format": 2,
     "globals": "09cc4020e70e256a5926957b03a43d6c",
     "version": "7.2.7"
 }
```

### Comparing `su6_plugin_svelte_check-0.3.0/htmlcov/style.css` & `su6_plugin_svelte_check-0.4.0/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.3.0/pytest_examples/package-lock.json` & `su6_plugin_svelte_check-0.4.0/pytest_examples/package-lock.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.3.0/pytest_examples/tsconfig-issues.json` & `su6_plugin_svelte_check-0.4.0/pytest_examples/tsconfig-issues.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.3.0/pytest_examples/tsconfig-no_issues.json` & `su6_plugin_svelte_check-0.4.0/pytest_examples/tsconfig-no_issues.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.3.0/pytest_examples/tsconfig-warnings.json` & `su6_plugin_svelte_check-0.4.0/pytest_examples/tsconfig-warnings.json`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.3.0/src/su6_plugin_svelte_check/cli.py` & `su6_plugin_svelte_check-0.4.0/src/su6_plugin_svelte_check/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This module contains an example of both methods of adding commands to su6.
 """
 from pathlib import Path
 
 from su6.plugins import PluginConfig, register, run_tool
 
-from .find_project_root import find_project_root
+from .helpers import chdir, find_project_root
 
 
 @register
 class SvelteCheckPluginConfig(PluginConfig):
     """
     Config without state, loads [tool.su6.demo] from pyproject.toml into self.
     """
@@ -17,20 +17,29 @@
     strict: bool = False
     tsconfig: str = "./tsconfig.json"
 
 
 config = SvelteCheckPluginConfig()
 
 
+@register
+def install_svelte_check(target_dir: str = None) -> int:
+    """
+    Install the svelte-check tool using npm.
+    """
+    target_dir = target_dir or "./"
+
+    with chdir(target_dir):
+        return run_tool("npm", "install", "svelte-check")
+
+
 @register(add_to_all=True)
 def svelte_check(strict: bool = None, tsconfig: str = None, node_modules: str = None) -> int:
     """
-    Register a top-level command.
-
-    @register works without ()
+    Run the svelte-check tool.
     """
     config.update(strict=strict, tsconfig=tsconfig)
     # svelte-check --tsconfig ./tsconfig.json --threshold error
 
     node_modules = node_modules or "node_modules"
     root, _ = find_project_root((node_modules,))
     executable = str(root / "node_modules/svelte-check/bin/svelte-check")
```

### Comparing `su6_plugin_svelte_check-0.3.0/src/su6_plugin_svelte_check/find_project_root.py` & `su6_plugin_svelte_check-0.4.0/src/su6_plugin_svelte_check/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 """
-Modified from black.files.
+Re-usable helpers for this project.
 """
+
+import contextlib
 from functools import lru_cache
 from pathlib import Path
 from typing import Optional, Sequence, Tuple
 
+try:
+    chdir = contextlib.chdir
+except AttributeError:  # pragma: no cover
+    from contextlib_chdir import chdir  # type: ignore
+
 
 @lru_cache()
 def find_project_root(srcs: Sequence[str], stdin_filename: Optional[str] = None) -> Tuple[Path, str]:
     """
     Return a directory containing .git, .hg, or pyproject.toml.
 
     That directory will be a common parent of all files and directories
@@ -16,14 +23,16 @@
 
     If no directory in the tree contains a marker that would specify it's the
     project root, the root of the file system is returned.
 
     Returns a two-tuple with the first element as the project root path and
     the second element as a string describing the method by which the
     project root was discovered.
+
+    Modified from black.files.
     """
     if stdin_filename is not None:
         srcs = tuple(stdin_filename if s == "-" else s for s in srcs)
     if not srcs:
         srcs = [str(Path.cwd().resolve())]
 
     path_srcs = [Path(Path.cwd(), src).resolve() for src in srcs]
@@ -47,7 +56,10 @@
         if (directory / ".hg").is_dir():  # pragma: no cover
             return directory, ".hg directory"
 
         if (directory / "pyproject.toml").is_file():  # pragma: no cover
             return directory, "pyproject.toml"
 
     return directory, "file system root"
+
+
+__all__ = ["chdir", "find_project_root"]
```

### Comparing `su6_plugin_svelte_check-0.3.0/tests/test_find_project_root.py` & `su6_plugin_svelte_check-0.4.0/tests/test_find_project_root.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import contextlib
 from pathlib import Path
 
-from src.su6_plugin_svelte_check.find_project_root import find_project_root
+from src.su6_plugin_svelte_check.helpers import find_project_root
 
 try:
     chdir = contextlib.chdir
 except AttributeError:
     from contextlib_chdir import chdir
```

### Comparing `su6_plugin_svelte_check-0.3.0/LICENSE.txt` & `su6_plugin_svelte_check-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.3.0/pyproject.toml` & `su6_plugin_svelte_check-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `su6_plugin_svelte_check-0.3.0/PKG-INFO` & `su6_plugin_svelte_check-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: su6-plugin-svelte-check
-Version: 0.3.0
+Version: 0.4.0
 Summary: Svelte-check plugin for `su6`
 Project-URL: Documentation, https://github.com/robinvandernoord/su6-plugin-svelte-check#readme
 Project-URL: Issues, https://github.com/robinvandernoord/su6-plugin-svelte-check/issues
 Project-URL: Source, https://github.com/robinvandernoord/su6-plugin-svelte-check
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

