# Comparing `tmp/tagmaps-0.22.2.tar.gz` & `tmp/tagmaps-0.22.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagmaps-0.22.2.tar", last modified: Tue May 16 06:26:17 2023, max compression
+gzip compressed data, was "tagmaps-0.22.3.tar", last modified: Mon Jul 17 11:24:34 2023, max compression
```

## Comparing `tagmaps-0.22.2.tar` & `tagmaps-0.22.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 06:26:17.341355 tagmaps-0.22.2/
--rw-r--r--   0 alex      (1000) alex      (1000)     8506 2023-05-16 06:25:42.000000 tagmaps-0.22.2/CHANGELOG.md
--rwxrwxrwx   0 alex      (1000) alex      (1000)    34940 2019-01-29 10:06:07.000000 tagmaps-0.22.2/LICENSE.md
--rw-rw-rw-   0 alex      (1000) alex      (1000)      164 2023-05-10 08:39:17.000000 tagmaps-0.22.2/MANIFEST.in
--rw-r--r--   0 alex      (1000) alex      (1000)    12279 2023-05-16 06:26:17.320066 tagmaps-0.22.2/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)    12128 2023-05-16 06:25:37.000000 tagmaps-0.22.2/README.md
--rw-r--r--   0 alex      (1000) alex      (1000)     2195 2023-05-16 06:25:37.000000 tagmaps-0.22.2/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-05-16 06:26:17.341740 tagmaps-0.22.2/setup.cfg
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 06:26:16.848250 tagmaps-0.22.2/src/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 06:26:16.988852 tagmaps-0.22.2/src/tagmaps/
--rw-rw-r--   0 alex      (1000) alex      (1000)      620 2021-02-18 12:42:56.000000 tagmaps-0.22.2/src/tagmaps/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5914 2022-07-27 08:37:55.000000 tagmaps-0.22.2/src/tagmaps/__main__.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 06:26:17.243393 tagmaps-0.22.2/src/tagmaps/classes/
--rw-rw-rw-   0 alex      (1000) alex      (1000)       33 2020-05-12 11:15:53.000000 tagmaps-0.22.2/src/tagmaps/classes/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    17469 2023-05-10 07:50:24.000000 tagmaps-0.22.2/src/tagmaps/classes/alpha_shapes.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    41054 2022-01-18 09:22:06.000000 tagmaps-0.22.2/src/tagmaps/classes/cluster.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    17232 2022-07-27 08:37:55.000000 tagmaps-0.22.2/src/tagmaps/classes/compile_output.py
--rw-r--r--   0 alex      (1000) alex      (1000)    23633 2022-11-28 06:40:14.000000 tagmaps-0.22.2/src/tagmaps/classes/interface.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)    17745 2021-02-18 09:36:00.000000 tagmaps-0.22.2/src/tagmaps/classes/load_data.py
--rw-r--r--   0 alex      (1000) alex      (1000)    10479 2023-05-10 07:55:05.000000 tagmaps-0.22.2/src/tagmaps/classes/plotting.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    32505 2021-02-18 12:42:56.000000 tagmaps-0.22.2/src/tagmaps/classes/prepare_data.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)     9578 2020-08-25 07:19:19.000000 tagmaps-0.22.2/src/tagmaps/classes/shared_structure.py
--rw-r--r--   0 alex      (1000) alex      (1000)    21911 2022-11-28 06:40:14.000000 tagmaps-0.22.2/src/tagmaps/classes/utils.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)       75 2019-02-25 08:56:16.000000 tagmaps-0.22.2/src/tagmaps/classes/write_output.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 06:26:17.276984 tagmaps-0.22.2/src/tagmaps/config/
--rw-rw-rw-   0 alex      (1000) alex      (1000)       39 2020-05-12 11:15:53.000000 tagmaps-0.22.2/src/tagmaps/config/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    26041 2022-07-27 08:37:55.000000 tagmaps-0.22.2/src/tagmaps/config/config.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)    31972 2017-12-21 09:44:59.000000 tagmaps-0.22.2/src/tagmaps/matplotlibrc
--rw-rw-r--   0 alex      (1000) alex      (1000)    19100 2022-07-27 08:37:55.000000 tagmaps-0.22.2/src/tagmaps/tagmaps_.py
--rw-r--r--   0 alex      (1000) alex      (1000)       46 2023-05-16 06:25:42.000000 tagmaps-0.22.2/src/tagmaps/version.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 06:26:17.019317 tagmaps-0.22.2/src/tagmaps.egg-info/
--rwxrwxrwx   0 alex      (1000) alex      (1000)    12279 2023-05-16 06:26:16.000000 tagmaps-0.22.2/src/tagmaps.egg-info/PKG-INFO
--rwxrwxrwx   0 alex      (1000) alex      (1000)      885 2023-05-16 06:26:16.000000 tagmaps-0.22.2/src/tagmaps.egg-info/SOURCES.txt
--rwxrwxrwx   0 alex      (1000) alex      (1000)        1 2023-05-16 06:26:16.000000 tagmaps-0.22.2/src/tagmaps.egg-info/dependency_links.txt
--rwxrwxrwx   0 alex      (1000) alex      (1000)       50 2023-05-16 06:26:16.000000 tagmaps-0.22.2/src/tagmaps.egg-info/entry_points.txt
--rwxrwxrwx   0 alex      (1000) alex      (1000)      110 2023-05-16 06:26:16.000000 tagmaps-0.22.2/src/tagmaps.egg-info/requires.txt
--rwxrwxrwx   0 alex      (1000) alex      (1000)        8 2023-05-16 06:26:16.000000 tagmaps-0.22.2/src/tagmaps.egg-info/top_level.txt
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-16 06:26:17.316745 tagmaps-0.22.2/tests/
--rw-r--r--   0 alex      (1000) alex      (1000)      627 2023-05-16 06:25:37.000000 tagmaps-0.22.2/tests/test_all.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)     3271 2019-02-22 14:26:36.000000 tagmaps-0.22.2/tests/test_emoji.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)      934 2019-01-29 10:06:07.000000 tagmaps-0.22.2/tests/test_post.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 11:24:34.908782 tagmaps-0.22.3/
+-rw-r--r--   0 alex      (1000) alex      (1000)     8701 2023-07-17 11:23:47.000000 tagmaps-0.22.3/CHANGELOG.md
+-rwxrwxrwx   0 alex      (1000) alex      (1000)    34940 2019-01-29 10:06:07.000000 tagmaps-0.22.3/LICENSE.md
+-rw-r--r--   0 alex      (1000) alex      (1000)      164 2023-05-16 10:04:37.000000 tagmaps-0.22.3/MANIFEST.in
+-rw-r--r--   0 alex      (1000) alex      (1000)    12288 2023-07-17 11:24:34.898678 tagmaps-0.22.3/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)    12137 2023-05-16 10:05:32.000000 tagmaps-0.22.3/README.md
+-rw-r--r--   0 alex      (1000) alex      (1000)     2195 2023-05-16 10:04:38.000000 tagmaps-0.22.3/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-07-17 11:24:34.908782 tagmaps-0.22.3/setup.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 11:24:34.491994 tagmaps-0.22.3/src/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 11:24:34.652163 tagmaps-0.22.3/src/tagmaps/
+-rw-r--r--   0 alex      (1000) alex      (1000)      620 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5914 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/__main__.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 11:24:34.825741 tagmaps-0.22.3/src/tagmaps/classes/
+-rw-r--r--   0 alex      (1000) alex      (1000)       33 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    17470 2023-07-17 11:20:03.000000 tagmaps-0.22.3/src/tagmaps/classes/alpha_shapes.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    41054 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/cluster.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    17232 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/compile_output.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    23633 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/interface.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    17745 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/load_data.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    10479 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/plotting.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    32505 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/prepare_data.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     9578 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/shared_structure.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    21911 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/utils.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       75 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/classes/write_output.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 11:24:34.844908 tagmaps-0.22.3/src/tagmaps/config/
+-rw-r--r--   0 alex      (1000) alex      (1000)       39 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/config/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    26041 2023-05-16 10:04:38.000000 tagmaps-0.22.3/src/tagmaps/config/config.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    31972 2023-05-16 10:04:39.000000 tagmaps-0.22.3/src/tagmaps/matplotlibrc
+-rw-r--r--   0 alex      (1000) alex      (1000)    19100 2023-05-16 10:04:39.000000 tagmaps-0.22.3/src/tagmaps/tagmaps_.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       46 2023-07-17 11:23:47.000000 tagmaps-0.22.3/src/tagmaps/version.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 11:24:34.679425 tagmaps-0.22.3/src/tagmaps.egg-info/
+-rwxrwxrwx   0 alex      (1000) alex      (1000)    12288 2023-07-17 11:24:34.000000 tagmaps-0.22.3/src/tagmaps.egg-info/PKG-INFO
+-rwxrwxrwx   0 alex      (1000) alex      (1000)      885 2023-07-17 11:24:34.000000 tagmaps-0.22.3/src/tagmaps.egg-info/SOURCES.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)        1 2023-07-17 11:24:34.000000 tagmaps-0.22.3/src/tagmaps.egg-info/dependency_links.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)       50 2023-07-17 11:24:34.000000 tagmaps-0.22.3/src/tagmaps.egg-info/entry_points.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)      110 2023-07-17 11:24:34.000000 tagmaps-0.22.3/src/tagmaps.egg-info/requires.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)        8 2023-07-17 11:24:34.000000 tagmaps-0.22.3/src/tagmaps.egg-info/top_level.txt
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 11:24:34.886654 tagmaps-0.22.3/tests/
+-rw-r--r--   0 alex      (1000) alex      (1000)      627 2023-05-16 10:04:39.000000 tagmaps-0.22.3/tests/test_all.py
+-rwxrwxrwx   0 alex      (1000) alex      (1000)     3271 2019-02-22 14:26:36.000000 tagmaps-0.22.3/tests/test_emoji.py
+-rwxrwxrwx   0 alex      (1000) alex      (1000)      934 2019-01-29 10:06:07.000000 tagmaps-0.22.3/tests/test_post.py
```

### Comparing `tagmaps-0.22.2/CHANGELOG.md` & `tagmaps-0.22.3/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.22.3 (2023-07-17)
+### Fix
+* Tri.vertices - Delaunay object has no attribute vertices ([`621b267`](https://github.com/Sieboldianus/TagMaps/commit/621b2673e34cec61c35c625a512b73b9937d6497))
+
 ## v0.22.2 (2023-05-16)
 
 
 ## v0.22.1 (2023-05-16)
 ### Documentation
 * Restructure Developers section ([`ae93e68`](https://github.com/Sieboldianus/TagMaps/commit/ae93e686040d23e75117fcd1053ede7502da4bdb))
 * Add high-level update to changelog ([`6a1bc1f`](https://github.com/Sieboldianus/TagMaps/commit/6a1bc1f9db9355ff6ba1efd99cac9a1b510945d1))
```

### Comparing `tagmaps-0.22.2/LICENSE.md` & `tagmaps-0.22.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/PKG-INFO` & `tagmaps-0.22.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagmaps
-Version: 0.22.2
+Version: 0.22.3
 Summary: Tag Clustering for Tag Maps
 Author-email: Alexander Dunkel <alexander.dunkel@tu-dresden.de>
 License: GNU GPLv3 or any higher
 Project-URL: Homepage, https://github.com/Sieboldianus/TagMaps
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -134,15 +134,15 @@
 ## Changelog & Download
 
 This is a high-level summary of version progress. See [CHANGELOG.md](CHANGELOG.md) for a full list of changes.
 
 2022-05-10: **TagMaps v0.22.0**
 
 - the project has finally migrated to a `pyproject.toml`-only based packaging system, as described in the [declarative config (pyproject.toml)](https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html)
-- structure now follows the [src-layout](https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#src-layout).
+- the code structure now follows the [src-layout](https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#src-layout).
 - fiona was pinned to `1.8.22` in conda until [#213](https://github.com/conda-forge/fiona-feedstock/issues/213) (Windows installations only) is solved
 
 2022-07-27: **TagMaps v0.21.0**
 
 - Add export to Mapnik ([`9db0d0d`](https://github.com/Sieboldianus/TagMaps/commit/9db0d0dc0a266f9eef7c3aac5bf663337c096f80)), enable with `--mapnik_export`
 - See a [jupyter lab notebook](https://ad.vgiscience.org/tagmaps-mapnik-jupyter/01_mapnik-tagmaps.html) that illustrates visualization of tag map data in [Mapnik](https://mapnik.org/)
```

### Comparing `tagmaps-0.22.2/README.md` & `tagmaps-0.22.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 ## Changelog & Download
 
 This is a high-level summary of version progress. See [CHANGELOG.md](CHANGELOG.md) for a full list of changes.
 
 2022-05-10: **TagMaps v0.22.0**
 
 - the project has finally migrated to a `pyproject.toml`-only based packaging system, as described in the [declarative config (pyproject.toml)](https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html)
-- structure now follows the [src-layout](https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#src-layout).
+- the code structure now follows the [src-layout](https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#src-layout).
 - fiona was pinned to `1.8.22` in conda until [#213](https://github.com/conda-forge/fiona-feedstock/issues/213) (Windows installations only) is solved
 
 2022-07-27: **TagMaps v0.21.0**
 
 - Add export to Mapnik ([`9db0d0d`](https://github.com/Sieboldianus/TagMaps/commit/9db0d0dc0a266f9eef7c3aac5bf663337c096f80)), enable with `--mapnik_export`
 - See a [jupyter lab notebook](https://ad.vgiscience.org/tagmaps-mapnik-jupyter/01_mapnik-tagmaps.html) that illustrates visualization of tag map data in [Mapnik](https://mapnik.org/)
```

### Comparing `tagmaps-0.22.2/pyproject.toml` & `tagmaps-0.22.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/src/tagmaps/__init__.py` & `tagmaps-0.22.3/src/tagmaps/__init__.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/src/tagmaps/__main__.py` & `tagmaps-0.22.3/src/tagmaps/__main__.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/src/tagmaps/classes/alpha_shapes.py` & `tagmaps-0.22.3/src/tagmaps/classes/alpha_shapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,15 +406,15 @@
         # It should be used for Delaunay triangulations
         # instead of using joggled input ('QJ').
         edges = set()
         edge_points = []
         # loop over triangles:
         # vert_ia, ib, ic = indices of corner points of the
         # triangle
-        for vert_ia, vert_ib, vert_ic in tri.vertices:
+        for vert_ia, vert_ib, vert_ic in tri.simplices:
             pa_v = coords[vert_ia]
             pb_v = coords[vert_ib]
             pc_v = coords[vert_ic]
             # Lengths of sides of triangle
             a_val = math.sqrt((pa_v[0] - pb_v[0]) ** 2 + (pa_v[1] - pb_v[1]) ** 2)
             b_val = math.sqrt((pb_v[0] - pc_v[0]) ** 2 + (pb_v[1] - pc_v[1]) ** 2)
             c_val = math.sqrt((pc_v[0] - pa_v[0]) ** 2 + (pc_v[1] - pa_v[1]) ** 2)
```

### Comparing `tagmaps-0.22.2/src/tagmaps/classes/cluster.py` & `tagmaps-0.22.3/src/tagmaps/classes/cluster.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/src/tagmaps/classes/compile_output.py` & `tagmaps-0.22.3/src/tagmaps/classes/compile_output.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/src/tagmaps/classes/interface.py` & `tagmaps-0.22.3/src/tagmaps/classes/interface.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/src/tagmaps/classes/load_data.py` & `tagmaps-0.22.3/src/tagmaps/classes/load_data.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/src/tagmaps/classes/plotting.py` & `tagmaps-0.22.3/src/tagmaps/classes/plotting.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/src/tagmaps/classes/prepare_data.py` & `tagmaps-0.22.3/src/tagmaps/classes/prepare_data.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/src/tagmaps/classes/shared_structure.py` & `tagmaps-0.22.3/src/tagmaps/classes/shared_structure.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/src/tagmaps/classes/utils.py` & `tagmaps-0.22.3/src/tagmaps/classes/utils.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/src/tagmaps/config/config.py` & `tagmaps-0.22.3/src/tagmaps/config/config.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/src/tagmaps/matplotlibrc` & `tagmaps-0.22.3/src/tagmaps/matplotlibrc`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/src/tagmaps/tagmaps_.py` & `tagmaps-0.22.3/src/tagmaps/tagmaps_.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/src/tagmaps.egg-info/PKG-INFO` & `tagmaps-0.22.3/src/tagmaps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagmaps
-Version: 0.22.2
+Version: 0.22.3
 Summary: Tag Clustering for Tag Maps
 Author-email: Alexander Dunkel <alexander.dunkel@tu-dresden.de>
 License: GNU GPLv3 or any higher
 Project-URL: Homepage, https://github.com/Sieboldianus/TagMaps
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -134,15 +134,15 @@
 ## Changelog & Download
 
 This is a high-level summary of version progress. See [CHANGELOG.md](CHANGELOG.md) for a full list of changes.
 
 2022-05-10: **TagMaps v0.22.0**
 
 - the project has finally migrated to a `pyproject.toml`-only based packaging system, as described in the [declarative config (pyproject.toml)](https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html)
-- structure now follows the [src-layout](https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#src-layout).
+- the code structure now follows the [src-layout](https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#src-layout).
 - fiona was pinned to `1.8.22` in conda until [#213](https://github.com/conda-forge/fiona-feedstock/issues/213) (Windows installations only) is solved
 
 2022-07-27: **TagMaps v0.21.0**
 
 - Add export to Mapnik ([`9db0d0d`](https://github.com/Sieboldianus/TagMaps/commit/9db0d0dc0a266f9eef7c3aac5bf663337c096f80)), enable with `--mapnik_export`
 - See a [jupyter lab notebook](https://ad.vgiscience.org/tagmaps-mapnik-jupyter/01_mapnik-tagmaps.html) that illustrates visualization of tag map data in [Mapnik](https://mapnik.org/)
```

### Comparing `tagmaps-0.22.2/src/tagmaps.egg-info/SOURCES.txt` & `tagmaps-0.22.3/src/tagmaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/tests/test_all.py` & `tagmaps-0.22.3/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/tests/test_emoji.py` & `tagmaps-0.22.3/tests/test_emoji.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.2/tests/test_post.py` & `tagmaps-0.22.3/tests/test_post.py`

 * *Files identical despite different names*

