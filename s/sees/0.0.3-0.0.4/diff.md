# Comparing `tmp/sees-0.0.3.tar.gz` & `tmp/sees-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sees-0.0.3.tar", last modified: Sun Jul 16 22:38:49 2023, max compression
+gzip compressed data, was "sees-0.0.4.tar", last modified: Sun Jul 16 23:00:47 2023, max compression
```

## Comparing `sees-0.0.3.tar` & `sees-0.0.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.336706 sees-0.0.3/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     2494 2023-07-16 22:38:49.336706 sees-0.0.3/PKG-INFO
--rw-r--r--   0 claudio   (1001) claudio   (1001)     2025 2023-07-16 22:38:12.000000 sees-0.0.3/README.md
--rw-r--r--   0 claudio   (1001) claudio   (1001)      819 2023-07-16 22:37:18.000000 sees-0.0.3/pyproject.toml
--rw-r--r--   0 claudio   (1001) claudio   (1001)       38 2023-07-16 22:38:49.336706 sees-0.0.3/setup.cfg
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.326706 sees-0.0.3/src/
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.326706 sees-0.0.3/src/sees/
--rwxr-xr-x   0 claudio   (1001) claudio   (1001)    24801 2023-07-16 22:33:32.000000 sees-0.0.3/src/sees/__init__.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     8780 2023-07-16 22:07:15.000000 sees-0.0.3/src/sees/__main__.py
--rwxr-xr-x   0 claudio   (1001) claudio   (1001)    46057 2023-07-12 02:10:35.000000 sees-0.0.3/src/sees/_render.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.336706 sees-0.0.3/src/sees/canvas/
--rw-r--r--   0 claudio   (1001) claudio   (1001)      714 2023-07-16 22:32:53.000000 sees-0.0.3/src/sees/canvas/canvas.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     2620 2023-07-16 22:33:00.000000 sees-0.0.3/src/sees/canvas/gltflib.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1543 2023-07-16 22:33:08.000000 sees-0.0.3/src/sees/canvas/mpl.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     4894 2023-07-16 22:33:14.000000 sees-0.0.3/src/sees/canvas/ply.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1458 2023-07-16 22:33:22.000000 sees-0.0.3/src/sees/canvas/tri.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1376 2023-07-12 02:25:12.000000 sees-0.0.3/src/sees/config.py
--rwxr-xr-x   0 claudio   (1001) claudio   (1001)     5608 2023-07-16 22:18:49.000000 sees-0.0.3/src/sees/consolidate.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-07-16 06:07:59.000000 sees-0.0.3/src/sees/core.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-03-27 17:30:37.000000 sees-0.0.3/src/sees/section.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.336706 sees-0.0.3/src/sees/solid/
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.336706 sees-0.0.3/src/sees/solid/convert/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     3303 2022-12-07 20:44:36.000000 sees-0.0.3/src/sees/solid/convert/convert.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)      383 2022-12-07 20:44:36.000000 sees-0.0.3/src/sees/solid/convert/example.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1460 2023-03-28 16:46:02.000000 sees-0.0.3/src/sees/solid/ops.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)      265 2023-03-28 16:26:56.000000 sees-0.0.3/src/sees/solid/plt.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-03-27 17:30:37.000000 sees-0.0.3/src/sees/structure.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.336706 sees-0.0.3/src/sees/utilities/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     3098 2023-07-12 17:28:46.000000 sees-0.0.3/src/sees/utilities/alpha_shape.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)      202 2023-07-16 06:08:31.000000 sees-0.0.3/src/sees/views.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.336706 sees-0.0.3/src/sees.egg-info/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     2494 2023-07-16 22:38:49.000000 sees-0.0.3/src/sees.egg-info/PKG-INFO
--rw-r--r--   0 claudio   (1001) claudio   (1001)      651 2023-07-16 22:38:49.000000 sees-0.0.3/src/sees.egg-info/SOURCES.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)        1 2023-07-16 22:38:49.000000 sees-0.0.3/src/sees.egg-info/dependency_links.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)       44 2023-07-16 22:38:49.000000 sees-0.0.3/src/sees.egg-info/entry_points.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)       12 2023-07-16 22:38:49.000000 sees-0.0.3/src/sees.egg-info/top_level.txt
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.336706 sees-0.0.3/tests/
--rw-r--r--   0 claudio   (1001) claudio   (1001)      108 2022-06-20 06:36:53.000000 sees-0.0.3/tests/test.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 23:00:47.256706 sees-0.0.4/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2635 2023-07-16 23:00:47.256706 sees-0.0.4/PKG-INFO
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2168 2023-07-16 23:00:02.000000 sees-0.0.4/README.md
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      817 2023-07-16 22:59:18.000000 sees-0.0.4/pyproject.toml
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       38 2023-07-16 23:00:47.256706 sees-0.0.4/setup.cfg
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 23:00:47.246706 sees-0.0.4/src/
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 23:00:47.246706 sees-0.0.4/src/sees/
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)    24801 2023-07-16 22:33:32.000000 sees-0.0.4/src/sees/__init__.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     8780 2023-07-16 22:07:15.000000 sees-0.0.4/src/sees/__main__.py
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)    46057 2023-07-12 02:10:35.000000 sees-0.0.4/src/sees/_render.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 23:00:47.256706 sees-0.0.4/src/sees/canvas/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      714 2023-07-16 22:32:53.000000 sees-0.0.4/src/sees/canvas/canvas.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2620 2023-07-16 22:33:00.000000 sees-0.0.4/src/sees/canvas/gltflib.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1543 2023-07-16 22:33:08.000000 sees-0.0.4/src/sees/canvas/mpl.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     4894 2023-07-16 22:33:14.000000 sees-0.0.4/src/sees/canvas/ply.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1458 2023-07-16 22:33:22.000000 sees-0.0.4/src/sees/canvas/tri.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1376 2023-07-12 02:25:12.000000 sees-0.0.4/src/sees/config.py
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)     5608 2023-07-16 22:18:49.000000 sees-0.0.4/src/sees/consolidate.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-07-16 06:07:59.000000 sees-0.0.4/src/sees/core.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-03-27 17:30:37.000000 sees-0.0.4/src/sees/section.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 23:00:47.256706 sees-0.0.4/src/sees/solid/
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 23:00:47.256706 sees-0.0.4/src/sees/solid/convert/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3303 2022-12-07 20:44:36.000000 sees-0.0.4/src/sees/solid/convert/convert.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      383 2022-12-07 20:44:36.000000 sees-0.0.4/src/sees/solid/convert/example.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1460 2023-03-28 16:46:02.000000 sees-0.0.4/src/sees/solid/ops.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      265 2023-03-28 16:26:56.000000 sees-0.0.4/src/sees/solid/plt.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-03-27 17:30:37.000000 sees-0.0.4/src/sees/structure.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 23:00:47.256706 sees-0.0.4/src/sees/utilities/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3098 2023-07-12 17:28:46.000000 sees-0.0.4/src/sees/utilities/alpha_shape.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      202 2023-07-16 06:08:31.000000 sees-0.0.4/src/sees/views.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 23:00:47.246706 sees-0.0.4/src/sees.egg-info/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2635 2023-07-16 23:00:47.000000 sees-0.0.4/src/sees.egg-info/PKG-INFO
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      651 2023-07-16 23:00:47.000000 sees-0.0.4/src/sees.egg-info/SOURCES.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        1 2023-07-16 23:00:47.000000 sees-0.0.4/src/sees.egg-info/dependency_links.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       44 2023-07-16 23:00:47.000000 sees-0.0.4/src/sees.egg-info/entry_points.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       12 2023-07-16 23:00:47.000000 sees-0.0.4/src/sees.egg-info/top_level.txt
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 23:00:47.256706 sees-0.0.4/tests/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      108 2022-06-20 06:36:53.000000 sees-0.0.4/tests/test.py
```

### Comparing `sees-0.0.3/PKG-INFO` & `sees-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sees
-Version: 0.0.3
-Summary: A sensible OpenSees renderer
+Version: 0.0.4
+Summary: A modern OpenSees renderer
 Author-email: "Claudio M. Perez" <50180406+claudioperez@users.noreply.github.com>, Chrystal Chern <52893467+chrystalchern@users.noreply.github.com>
 Project-URL: repository, http://github.com/BRACE2/sees
 Project-URL: documentation, https://brace2.github.io/sees
 Keywords: seismic,post-processing,finite-element-analysis,earthquake-engineering
 Description-Content-Type: text/markdown
 
 # `sees`
@@ -17,25 +17,23 @@
 <img align="left" src="https://github.com/BRACE2/OpenSeesRT/blob/master/docs/figures/hockling.png?raw=true" width="350px" alt="SEES Logo">
 
 <!--
 https://github.com/claudioperez/sees/blob/master/docs/figures/hockling.png?raw=true
 -->
 
 
-**A sensible OpenSees renderer**
+**A modern OpenSees renderer**
 
 
 <br>
 
 <!-- 
 -------------------------------------------------------------------- 
 -->
 
-<br>
-
 <div style="align:center">
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/sees?logo=pypi&style=for-the-badge)](https://pypi.python.org/pypi/sees)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/sees?style=for-the-badge)](https://pypi.org/project/sees)
 
 <!--
 [![Latest conda-forge version](https://img.shields.io/conda/vn/conda-forge/sees?logo=conda-forge&style=for-the-badge)](https://anaconda.org/conda-forge/sees)
@@ -44,14 +42,16 @@
 
 </div>
 
 <!-- 
 -------------------------------------------------------------------- 
 -->
 
+`sees` is a finite element rendering library that leverages modern 
+web technologies to produce sharable, efficient, and beautiful renderings.
 
 
 <!-- Badge links -->
 
 [pypi-d-image]: https://img.shields.io/pypi/dm/sees.svg
 [license-badge]: https://img.shields.io/pypi/l/sees.svg
 [pypi-d-link]: https://pypi.org/project/sees
@@ -78,9 +78,9 @@
 
 -------------------------------------------------------------------- 
 
 <br>
 
 See also
 
-- [`opensees`](pypi.org/project/opensees)
+- [`opensees`](https://pypi.org/project/opensees)
```

### Comparing `sees-0.0.3/README.md` & `sees-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,25 +7,23 @@
 <img align="left" src="https://github.com/BRACE2/OpenSeesRT/blob/master/docs/figures/hockling.png?raw=true" width="350px" alt="SEES Logo">
 
 <!--
 https://github.com/claudioperez/sees/blob/master/docs/figures/hockling.png?raw=true
 -->
 
 
-**A sensible OpenSees renderer**
+**A modern OpenSees renderer**
 
 
 <br>
 
 <!-- 
 -------------------------------------------------------------------- 
 -->
 
-<br>
-
 <div style="align:center">
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/sees?logo=pypi&style=for-the-badge)](https://pypi.python.org/pypi/sees)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/sees?style=for-the-badge)](https://pypi.org/project/sees)
 
 <!--
 [![Latest conda-forge version](https://img.shields.io/conda/vn/conda-forge/sees?logo=conda-forge&style=for-the-badge)](https://anaconda.org/conda-forge/sees)
@@ -34,14 +32,16 @@
 
 </div>
 
 <!-- 
 -------------------------------------------------------------------- 
 -->
 
+`sees` is a finite element rendering library that leverages modern 
+web technologies to produce sharable, efficient, and beautiful renderings.
 
 
 <!-- Badge links -->
 
 [pypi-d-image]: https://img.shields.io/pypi/dm/sees.svg
 [license-badge]: https://img.shields.io/pypi/l/sees.svg
 [pypi-d-link]: https://pypi.org/project/sees
@@ -68,9 +68,9 @@
 
 -------------------------------------------------------------------- 
 
 <br>
 
 See also
 
-- [`opensees`](pypi.org/project/opensees)
+- [`opensees`](https://pypi.org/project/opensees)
```

### Comparing `sees-0.0.3/pyproject.toml` & `sees-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "sees"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   {name="Claudio M. Perez", email="50180406+claudioperez@users.noreply.github.com"},
   {name="Chrystal Chern",   email="52893467+chrystalchern@users.noreply.github.com"}
 ]
-description="A sensible OpenSees renderer"
+description="A modern OpenSees renderer"
 
 readme = "README.md"
 
 keywords = [
   "seismic",
   "post-processing",
   "finite-element-analysis",
```

### Comparing `sees-0.0.3/src/sees/__init__.py` & `sees-0.0.4/src/sees/__init__.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.3/src/sees/__main__.py` & `sees-0.0.4/src/sees/__main__.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.3/src/sees/_render.py` & `sees-0.0.4/src/sees/_render.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.3/src/sees/canvas/canvas.py` & `sees-0.0.4/src/sees/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.3/src/sees/canvas/gltflib.py` & `sees-0.0.4/src/sees/canvas/gltflib.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.3/src/sees/canvas/mpl.py` & `sees-0.0.4/src/sees/canvas/mpl.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.3/src/sees/canvas/ply.py` & `sees-0.0.4/src/sees/canvas/ply.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.3/src/sees/canvas/tri.py` & `sees-0.0.4/src/sees/canvas/tri.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.3/src/sees/config.py` & `sees-0.0.4/src/sees/config.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.3/src/sees/consolidate.py` & `sees-0.0.4/src/sees/consolidate.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.3/src/sees/solid/convert/convert.py` & `sees-0.0.4/src/sees/solid/convert/convert.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.3/src/sees/solid/ops.py` & `sees-0.0.4/src/sees/solid/ops.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.3/src/sees/utilities/alpha_shape.py` & `sees-0.0.4/src/sees/utilities/alpha_shape.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.3/src/sees.egg-info/PKG-INFO` & `sees-0.0.4/src/sees.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sees
-Version: 0.0.3
-Summary: A sensible OpenSees renderer
+Version: 0.0.4
+Summary: A modern OpenSees renderer
 Author-email: "Claudio M. Perez" <50180406+claudioperez@users.noreply.github.com>, Chrystal Chern <52893467+chrystalchern@users.noreply.github.com>
 Project-URL: repository, http://github.com/BRACE2/sees
 Project-URL: documentation, https://brace2.github.io/sees
 Keywords: seismic,post-processing,finite-element-analysis,earthquake-engineering
 Description-Content-Type: text/markdown
 
 # `sees`
@@ -17,25 +17,23 @@
 <img align="left" src="https://github.com/BRACE2/OpenSeesRT/blob/master/docs/figures/hockling.png?raw=true" width="350px" alt="SEES Logo">
 
 <!--
 https://github.com/claudioperez/sees/blob/master/docs/figures/hockling.png?raw=true
 -->
 
 
-**A sensible OpenSees renderer**
+**A modern OpenSees renderer**
 
 
 <br>
 
 <!-- 
 -------------------------------------------------------------------- 
 -->
 
-<br>
-
 <div style="align:center">
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/sees?logo=pypi&style=for-the-badge)](https://pypi.python.org/pypi/sees)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/sees?style=for-the-badge)](https://pypi.org/project/sees)
 
 <!--
 [![Latest conda-forge version](https://img.shields.io/conda/vn/conda-forge/sees?logo=conda-forge&style=for-the-badge)](https://anaconda.org/conda-forge/sees)
@@ -44,14 +42,16 @@
 
 </div>
 
 <!-- 
 -------------------------------------------------------------------- 
 -->
 
+`sees` is a finite element rendering library that leverages modern 
+web technologies to produce sharable, efficient, and beautiful renderings.
 
 
 <!-- Badge links -->
 
 [pypi-d-image]: https://img.shields.io/pypi/dm/sees.svg
 [license-badge]: https://img.shields.io/pypi/l/sees.svg
 [pypi-d-link]: https://pypi.org/project/sees
@@ -78,9 +78,9 @@
 
 -------------------------------------------------------------------- 
 
 <br>
 
 See also
 
-- [`opensees`](pypi.org/project/opensees)
+- [`opensees`](https://pypi.org/project/opensees)
```

### Comparing `sees-0.0.3/src/sees.egg-info/SOURCES.txt` & `sees-0.0.4/src/sees.egg-info/SOURCES.txt`

 * *Files identical despite different names*

