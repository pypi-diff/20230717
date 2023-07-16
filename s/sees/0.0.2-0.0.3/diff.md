# Comparing `tmp/sees-0.0.2.tar.gz` & `tmp/sees-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sees-0.0.2.tar", last modified: Wed Jul 12 22:53:21 2023, max compression
+gzip compressed data, was "sees-0.0.3.tar", last modified: Sun Jul 16 22:38:49 2023, max compression
```

## Comparing `sees-0.0.2.tar` & `sees-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.055062 sees-0.0.2/
--rw-r--r--   0 claudio   (1001) claudio   (1001)      390 2023-07-12 22:53:21.055062 sees-0.0.2/PKG-INFO
--rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-07-12 02:36:52.000000 sees-0.0.2/README.md
--rw-r--r--   0 claudio   (1001) claudio   (1001)      726 2023-07-12 22:52:34.000000 sees-0.0.2/pyproject.toml
--rw-r--r--   0 claudio   (1001) claudio   (1001)       38 2023-07-12 22:53:21.055062 sees-0.0.2/setup.cfg
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.045062 sees-0.0.2/src/
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.055062 sees-0.0.2/src/sees/
--rwxr-xr-x   0 claudio   (1001) claudio   (1001)    25650 2023-07-12 19:58:25.000000 sees-0.0.2/src/sees/__init__.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     8200 2023-07-12 20:46:07.000000 sees-0.0.2/src/sees/__main__.py
--rwxr-xr-x   0 claudio   (1001) claudio   (1001)    46057 2023-07-12 02:10:35.000000 sees-0.0.2/src/sees/_render.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.055062 sees-0.0.2/src/sees/canvas/
--rw-r--r--   0 claudio   (1001) claudio   (1001)      698 2023-07-12 02:42:52.000000 sees-0.0.2/src/sees/canvas/canvas.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     2604 2023-07-12 03:36:02.000000 sees-0.0.2/src/sees/canvas/gltflib.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1501 2023-07-12 02:42:06.000000 sees-0.0.2/src/sees/canvas/mpl.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     4878 2023-07-12 22:52:20.000000 sees-0.0.2/src/sees/canvas/ply.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1442 2023-07-12 04:22:07.000000 sees-0.0.2/src/sees/canvas/tri.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1376 2023-07-12 02:25:12.000000 sees-0.0.2/src/sees/config.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-03-27 17:30:37.000000 sees-0.0.2/src/sees/section.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.055062 sees-0.0.2/src/sees/solid/
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.055062 sees-0.0.2/src/sees/solid/convert/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     3303 2022-12-07 20:44:36.000000 sees-0.0.2/src/sees/solid/convert/convert.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)      383 2022-12-07 20:44:36.000000 sees-0.0.2/src/sees/solid/convert/example.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1460 2023-03-28 16:46:02.000000 sees-0.0.2/src/sees/solid/ops.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)      265 2023-03-28 16:26:56.000000 sees-0.0.2/src/sees/solid/plt.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-03-27 17:30:37.000000 sees-0.0.2/src/sees/structure.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.055062 sees-0.0.2/src/sees/utilities/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     3098 2023-07-12 17:28:46.000000 sees-0.0.2/src/sees/utilities/alpha_shape.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.055062 sees-0.0.2/src/sees.egg-info/
--rw-r--r--   0 claudio   (1001) claudio   (1001)      390 2023-07-12 22:53:20.000000 sees-0.0.2/src/sees.egg-info/PKG-INFO
--rw-r--r--   0 claudio   (1001) claudio   (1001)      592 2023-07-12 22:53:21.000000 sees-0.0.2/src/sees.egg-info/SOURCES.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)        1 2023-07-12 22:53:20.000000 sees-0.0.2/src/sees.egg-info/dependency_links.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)       44 2023-07-12 22:53:20.000000 sees-0.0.2/src/sees.egg-info/entry_points.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)        5 2023-07-12 22:53:20.000000 sees-0.0.2/src/sees.egg-info/top_level.txt
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.055062 sees-0.0.2/tests/
--rw-r--r--   0 claudio   (1001) claudio   (1001)      108 2022-06-20 06:36:53.000000 sees-0.0.2/tests/test.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.336706 sees-0.0.3/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2494 2023-07-16 22:38:49.336706 sees-0.0.3/PKG-INFO
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2025 2023-07-16 22:38:12.000000 sees-0.0.3/README.md
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      819 2023-07-16 22:37:18.000000 sees-0.0.3/pyproject.toml
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       38 2023-07-16 22:38:49.336706 sees-0.0.3/setup.cfg
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.326706 sees-0.0.3/src/
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.326706 sees-0.0.3/src/sees/
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)    24801 2023-07-16 22:33:32.000000 sees-0.0.3/src/sees/__init__.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     8780 2023-07-16 22:07:15.000000 sees-0.0.3/src/sees/__main__.py
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)    46057 2023-07-12 02:10:35.000000 sees-0.0.3/src/sees/_render.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.336706 sees-0.0.3/src/sees/canvas/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      714 2023-07-16 22:32:53.000000 sees-0.0.3/src/sees/canvas/canvas.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2620 2023-07-16 22:33:00.000000 sees-0.0.3/src/sees/canvas/gltflib.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1543 2023-07-16 22:33:08.000000 sees-0.0.3/src/sees/canvas/mpl.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     4894 2023-07-16 22:33:14.000000 sees-0.0.3/src/sees/canvas/ply.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1458 2023-07-16 22:33:22.000000 sees-0.0.3/src/sees/canvas/tri.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1376 2023-07-12 02:25:12.000000 sees-0.0.3/src/sees/config.py
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)     5608 2023-07-16 22:18:49.000000 sees-0.0.3/src/sees/consolidate.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-07-16 06:07:59.000000 sees-0.0.3/src/sees/core.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-03-27 17:30:37.000000 sees-0.0.3/src/sees/section.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.336706 sees-0.0.3/src/sees/solid/
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.336706 sees-0.0.3/src/sees/solid/convert/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3303 2022-12-07 20:44:36.000000 sees-0.0.3/src/sees/solid/convert/convert.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      383 2022-12-07 20:44:36.000000 sees-0.0.3/src/sees/solid/convert/example.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1460 2023-03-28 16:46:02.000000 sees-0.0.3/src/sees/solid/ops.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      265 2023-03-28 16:26:56.000000 sees-0.0.3/src/sees/solid/plt.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-03-27 17:30:37.000000 sees-0.0.3/src/sees/structure.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.336706 sees-0.0.3/src/sees/utilities/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3098 2023-07-12 17:28:46.000000 sees-0.0.3/src/sees/utilities/alpha_shape.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      202 2023-07-16 06:08:31.000000 sees-0.0.3/src/sees/views.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.336706 sees-0.0.3/src/sees.egg-info/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2494 2023-07-16 22:38:49.000000 sees-0.0.3/src/sees.egg-info/PKG-INFO
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      651 2023-07-16 22:38:49.000000 sees-0.0.3/src/sees.egg-info/SOURCES.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        1 2023-07-16 22:38:49.000000 sees-0.0.3/src/sees.egg-info/dependency_links.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       44 2023-07-16 22:38:49.000000 sees-0.0.3/src/sees.egg-info/entry_points.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       12 2023-07-16 22:38:49.000000 sees-0.0.3/src/sees.egg-info/top_level.txt
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:38:49.336706 sees-0.0.3/tests/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      108 2022-06-20 06:36:53.000000 sees-0.0.3/tests/test.py
```

### Comparing `sees-0.0.2/pyproject.toml` & `sees-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 [project]
 name = "sees"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   {name="Claudio M. Perez", email="50180406+claudioperez@users.noreply.github.com"},
   {name="Chrystal Chern",   email="52893467+chrystalchern@users.noreply.github.com"}
 ]
+description="A sensible OpenSees renderer"
 
 readme = "README.md"
 
 keywords = [
   "seismic",
+  "post-processing",
+  "finite-element-analysis",
   "earthquake-engineering",
 ] 
 
 [options]
 #packages = find
 install_requires = [
   "sdof",
```

### Comparing `sees-0.0.2/src/sees/__init__.py` & `sees-0.0.3/src/sees/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,9 @@
 #!/bin/env python
-
-# # Synopsis
 #
-# >`render.py [<options>] <model-file>`
-#
-# >**Chrystal Chern**, and **Claudio Perez**
-# 
-#
-# This script plots the geometry of a structural
-# model given a SAM JSON file.
-#
-#
-# ## Matlab
-# In order to install the Matlab bindings, open Matlab in a
-# directory containing the files `render.py` and `render.m`,
-# and run the following command in the Matlab interpreter:
-#
-#     render --install
-#
-# Once this process is complete, the command `render` can be
-# called from Matlab, just as described below for the command
-# line.
-#
-# # Usage
-# This script can be used either as a module, or as a command
-# line utility. When invoked from the command line on
-# **Windows**, {NAME} should be `python -m render`. For example:
-#
-#     python -m render model.json --axes 2 --view elev
-#
-# The script may be invoked with the following options:
-
 # The remainder of this script is broken into the following sections:
 #
 # - Data shaping / Misc.
 # - Kinematics
 # - Plotting
 # - Command line processing
 #
```

### Comparing `sees-0.0.2/src/sees/_render.py` & `sees-0.0.3/src/sees/_render.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.2/src/sees/canvas/canvas.py` & `sees-0.0.3/src/sees/canvas/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Claudio Perez
 import numpy as np
 class Canvas:
     def build(self): ...
     def show(self): ...
     def write(self, filename=None): ...
     def plot_nodes(self, coords, label = None, props=None, data=None): ...
```

### Comparing `sees-0.0.2/src/sees/canvas/gltflib.py` & `sees-0.0.3/src/sees/canvas/gltflib.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Claudio Perez
 import numpy as np
 import pygltflib
 from .canvas import Canvas
 
 class GltfLibCanvas(Canvas):
     def __init__(self, config=None):
         self.config = config
```

### Comparing `sees-0.0.2/src/sees/canvas/mpl.py` & `sees-0.0.3/src/sees/canvas/mpl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from .canvas import Canvas
+# Claudio Perez
 import numpy as np
+from .canvas import Canvas
+from ..views import VIEWS
 
 class MatplotlibCanvas(Canvas):
     def __init__(self, ax=None):
         if ax is None:
             import matplotlib.pyplot as plt
             self.plt = plt
             _, ax = plt.subplots(1, 1, subplot_kw={"projection": "3d"})
```

### Comparing `sees-0.0.2/src/sees/canvas/ply.py` & `sees-0.0.3/src/sees/canvas/ply.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Claudio Perez
 from .canvas import Canvas
 import numpy as np
 
 class PlotlyCanvas(Canvas):
     def __init__(self, config=None):
         self.data = []
         self.config = config
```

### Comparing `sees-0.0.2/src/sees/canvas/tri.py` & `sees-0.0.3/src/sees/canvas/tri.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Claudio Perez
 from .canvas import Canvas
 import trimesh
 import numpy as np
 
 class TrimeshCanvas(Canvas):
     def __init__(self, config=None):
         self.scene = trimesh.Scene()
```

### Comparing `sees-0.0.2/src/sees/config.py` & `sees-0.0.3/src/sees/config.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.2/src/sees/solid/convert/convert.py` & `sees-0.0.3/src/sees/solid/convert/convert.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.2/src/sees/solid/ops.py` & `sees-0.0.3/src/sees/solid/ops.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.2/src/sees/utilities/alpha_shape.py` & `sees-0.0.3/src/sees/utilities/alpha_shape.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.2/src/sees.egg-info/SOURCES.txt` & `sees-0.0.3/src/sees.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 README.md
 pyproject.toml
 src/sees/__init__.py
 src/sees/__main__.py
 src/sees/_render.py
 src/sees/config.py
+src/sees/consolidate.py
+src/sees/core.py
 src/sees/section.py
 src/sees/structure.py
+src/sees/views.py
 src/sees.egg-info/PKG-INFO
 src/sees.egg-info/SOURCES.txt
 src/sees.egg-info/dependency_links.txt
 src/sees.egg-info/entry_points.txt
 src/sees.egg-info/top_level.txt
 src/sees/canvas/canvas.py
 src/sees/canvas/gltflib.py
```

