# Comparing `tmp/jupyterlab_hide_cells-1.0.0.tar.gz` & `tmp/jupyterlab_hide_cells-1.0.1.tar.gz`

## Comparing `jupyterlab_hide_cells-1.0.0.tar` & `jupyterlab_hide_cells-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/.prettierignore
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/RELEASE.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/install.json
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/setup.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/tsconfig.json
--rw-r--r--   0        0        0   145945 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/yarn.lock
--rw-r--r--   0        0        0  2711422 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/documentation/JupyterLabHideCode.gif
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/jupyterlab-hide-cells/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/jupyterlab-hide-cells/_version.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/jupyterlab-hide-cells/labextension/package.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/jupyterlab-hide-cells/labextension/static/474.8c3eef16f64ac2348b91.js
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/jupyterlab-hide-cells/labextension/static/747.af787252e15b9daa2861.js
--rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/jupyterlab-hide-cells/labextension/static/remoteEntry.8a4ee27d91ac613d9545.js
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/jupyterlab-hide-cells/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/jupyterlab-hide-cells/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/src/config.ts
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/src/index.ts
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/style/index.js
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/LICENSE
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/README.md
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/.prettierignore
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/RELEASE.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/install.json
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/setup.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/tsconfig.json
+-rw-r--r--   0        0        0   145945 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/yarn.lock
+-rw-r--r--   0        0        0  2711422 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/documentation/JupyterLabHideCode.gif
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/jupyterlab-hide-cells/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/jupyterlab-hide-cells/_version.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/jupyterlab-hide-cells/labextension/package.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/jupyterlab-hide-cells/labextension/static/474.8c3eef16f64ac2348b91.js
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/jupyterlab-hide-cells/labextension/static/747.af787252e15b9daa2861.js
+-rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/jupyterlab-hide-cells/labextension/static/remoteEntry.6e1b57a88755dff1ddd7.js
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/jupyterlab-hide-cells/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/jupyterlab-hide-cells/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/src/config.ts
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/src/index.ts
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/style/index.js
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/README.md
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 jupyterlab_hide_cells-1.0.1/PKG-INFO
```

### Comparing `jupyterlab_hide_cells-1.0.0/RELEASE.md` & `jupyterlab_hide_cells-1.0.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_cells-1.0.0/package.json` & `jupyterlab_hide_cells-1.0.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'1.0.1'"}*

```diff
@@ -80,9 +80,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.0.1"
 }
```

### Comparing `jupyterlab_hide_cells-1.0.0/tsconfig.json` & `jupyterlab_hide_cells-1.0.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_cells-1.0.0/yarn.lock` & `jupyterlab_hide_cells-1.0.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_cells-1.0.0/documentation/JupyterLabHideCode.gif` & `jupyterlab_hide_cells-1.0.1/documentation/JupyterLabHideCode.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_cells-1.0.0/jupyterlab-hide-cells/labextension/package.json` & `jupyterlab_hide_cells-1.0.1/jupyterlab-hide-cells/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9755291005291005%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.6e1b57a88755dff1ddd7.js'}}",*

 * * "'version'": "'1.0.1'"}*

```diff
@@ -28,15 +28,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://git.rwth-aachen.de/learntech-lufgi9/public/jupyterlab-hide-cells",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.8a4ee27d91ac613d9545.js",
+            "load": "static/remoteEntry.6e1b57a88755dff1ddd7.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab-hide-cells/labextension"
     },
     "keywords": [
         "jupyter",
@@ -85,9 +85,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.0.1"
 }
```

### Comparing `jupyterlab_hide_cells-1.0.0/jupyterlab-hide-cells/labextension/static/474.8c3eef16f64ac2348b91.js` & `jupyterlab_hide_cells-1.0.1/jupyterlab-hide-cells/labextension/static/474.8c3eef16f64ac2348b91.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_cells-1.0.0/jupyterlab-hide-cells/labextension/static/747.af787252e15b9daa2861.js` & `jupyterlab_hide_cells-1.0.1/jupyterlab-hide-cells/labextension/static/747.af787252e15b9daa2861.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_cells-1.0.0/jupyterlab-hide-cells/labextension/static/remoteEntry.8a4ee27d91ac613d9545.js` & `jupyterlab_hide_cells-1.0.1/jupyterlab-hide-cells/labextension/static/remoteEntry.6e1b57a88755dff1ddd7.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         l = o[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : i > l.from)) && (o[r] = {
                         get: () => m.e(474).then((() => () => m(474))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab-hide-cells", "1.0.0"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("jupyterlab-hide-cells", "1.0.1"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_hide_cells-1.0.0/jupyterlab-hide-cells/labextension/static/third-party-licenses.json` & `jupyterlab_hide_cells-1.0.1/jupyterlab-hide-cells/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_cells-1.0.0/src/index.ts` & `jupyterlab_hide_cells-1.0.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_cells-1.0.0/.gitignore` & `jupyterlab_hide_cells-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_cells-1.0.0/LICENSE` & `jupyterlab_hide_cells-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_cells-1.0.0/README.md` & `jupyterlab_hide_cells-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_cells-1.0.0/pyproject.toml` & `jupyterlab_hide_cells-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 requires-python = ">=3.7"
 classifiers = [
     "Framework :: Jupyter",
     "Framework :: Jupyter :: JupyterLab",
     "Framework :: Jupyter :: JupyterLab :: 3",
     "Framework :: Jupyter :: JupyterLab :: Extensions",
     "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
-    "License :: OSI Approved :: BSD License",
+    "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
```

### Comparing `jupyterlab_hide_cells-1.0.0/PKG-INFO` & `jupyterlab_hide_cells-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-hide-cells
-Version: 1.0.0
+Version: 1.0.1
 Summary: jl-hide-cells
 Project-URL: Homepage, https://git.rwth-aachen.de/learntech-lufgi9/public/jupyterlab-hide-cells
 Project-URL: Bug Tracker, https://git.rwth-aachen.de/learntech-lufgi9/public/jupyterlab-hide-cells/issues
 Project-URL: Repository, https://git.rwth-aachen.de/learntech-lufgi9/public/jupyterlab-hide-cells.git
 Author-email: Annabell Brocker <a.brocker@cs.rwth-aachen.de>
 License: MIT License
         
@@ -29,15 +29,15 @@
         SOFTWARE.
 License-File: LICENSE
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

