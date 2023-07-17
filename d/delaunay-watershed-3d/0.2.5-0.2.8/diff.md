# Comparing `tmp/delaunay_watershed_3d-0.2.5.tar.gz` & `tmp/delaunay_watershed_3d-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/delaunay-watershed/dist/.tmp-55fbnwhl/delaunay_watershed_3d-0.2.5.tar", last modified: Fri Jun 23 13:51:50 2023, max compression
+gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/delaunay-watershed/dist/.tmp-0wbaerlv/delaunay_watershed_3d-0.2.8.tar", last modified: Mon Jul 17 10:47:01 2023, max compression
```

## Comparing `delaunay_watershed_3d-0.2.5.tar` & `delaunay_watershed_3d-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 13:51:50.357334 delaunay_watershed_3d-0.2.5/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     7904 2023-06-23 13:51:50.357451 delaunay_watershed_3d-0.2.5/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     7218 2023-06-23 13:44:43.000000 delaunay_watershed_3d-0.2.5/README.md
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/pyproject.toml
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     1008 2023-06-23 13:51:50.358058 delaunay_watershed_3d-0.2.5/setup.cfg
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 13:51:50.339478 delaunay_watershed_3d-0.2.5/src/
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 13:51:50.344512 delaunay_watershed_3d-0.2.5/src/delaunay_watershed_3d.egg-info/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     7904 2023-06-23 13:51:50.000000 delaunay_watershed_3d-0.2.5/src/delaunay_watershed_3d.egg-info/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      531 2023-06-23 13:51:50.000000 delaunay_watershed_3d-0.2.5/src/delaunay_watershed_3d.egg-info/SOURCES.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-06-23 13:51:50.000000 delaunay_watershed_3d-0.2.5/src/delaunay_watershed_3d.egg-info/dependency_links.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      152 2023-06-23 13:51:50.000000 delaunay_watershed_3d-0.2.5/src/delaunay_watershed_3d.egg-info/requires.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        5 2023-06-23 13:51:50.000000 delaunay_watershed_3d-0.2.5/src/delaunay_watershed_3d.egg-info/top_level.txt
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 13:51:50.356707 delaunay_watershed_3d-0.2.5/src/dw3d/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    12255 2023-06-23 13:30:42.000000 delaunay_watershed_3d-0.2.5/src/dw3d/Curvature.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    21852 2023-06-23 13:29:29.000000 delaunay_watershed_3d-0.2.5/src/dw3d/Dcel.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6929 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/src/dw3d/Geometric_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    16784 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/src/dw3d/Geometry.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6334 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/src/dw3d/Graph_functions.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     2827 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/src/dw3d/Mask_reconstruction.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    10499 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/src/dw3d/Mesh_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     3506 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/src/dw3d/Networkx_functions.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       87 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/src/dw3d/__init__.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     5033 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/src/dw3d/functions.py
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:47:01.897778 delaunay_watershed_3d-0.2.8/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     7827 2023-07-17 10:47:01.897950 delaunay_watershed_3d-0.2.8/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     7218 2023-07-11 09:35:31.000000 delaunay_watershed_3d-0.2.8/README.md
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.8/pyproject.toml
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      954 2023-07-17 10:47:01.898752 delaunay_watershed_3d-0.2.8/setup.cfg
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:47:01.882136 delaunay_watershed_3d-0.2.8/src/
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:47:01.886395 delaunay_watershed_3d-0.2.8/src/delaunay_watershed_3d.egg-info/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     7827 2023-07-17 10:47:01.000000 delaunay_watershed_3d-0.2.8/src/delaunay_watershed_3d.egg-info/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      531 2023-07-17 10:47:01.000000 delaunay_watershed_3d-0.2.8/src/delaunay_watershed_3d.egg-info/SOURCES.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-07-17 10:47:01.000000 delaunay_watershed_3d-0.2.8/src/delaunay_watershed_3d.egg-info/dependency_links.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      152 2023-07-17 10:47:01.000000 delaunay_watershed_3d-0.2.8/src/delaunay_watershed_3d.egg-info/requires.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        5 2023-07-17 10:47:01.000000 delaunay_watershed_3d-0.2.8/src/delaunay_watershed_3d.egg-info/top_level.txt
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:47:01.897377 delaunay_watershed_3d-0.2.8/src/dw3d/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    12255 2023-06-23 13:30:42.000000 delaunay_watershed_3d-0.2.8/src/dw3d/Curvature.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    21852 2023-06-23 13:29:29.000000 delaunay_watershed_3d-0.2.8/src/dw3d/Dcel.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6929 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.8/src/dw3d/Geometric_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    16784 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.8/src/dw3d/Geometry.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6334 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.8/src/dw3d/Graph_functions.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     2827 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.8/src/dw3d/Mask_reconstruction.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10499 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.8/src/dw3d/Mesh_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     3506 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.8/src/dw3d/Networkx_functions.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       87 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.8/src/dw3d/__init__.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     5033 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.8/src/dw3d/functions.py
```

### Comparing `delaunay_watershed_3d-0.2.5/PKG-INFO` & `delaunay_watershed_3d-0.2.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: delaunay_watershed_3d
-Version: 0.2.5
+Version: 0.2.8
 Summary: Geometrical reconstruction of cell assemblies from instance segmentations
 Home-page: https://github.com/VirtualEmbryo/delaunay-watershed
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
+License: CC BY-NC-SA 4.0
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Delaunay-Watershed 3D
 
 <img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Figure_logo_white_arrow.png" alt="drawing" width="300"/>
```

### Comparing `delaunay_watershed_3d-0.2.5/README.md` & `delaunay_watershed_3d-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.5/setup.cfg` & `delaunay_watershed_3d-0.2.8/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [metadata]
 name = delaunay_watershed_3d
-version = 0.2.5
+version = 0.2.8
 author = Sacha Ichbiah
 author_email = sacha.ichbiah@college-de-france.fr
 description = Geometrical reconstruction of cell assemblies from instance segmentations
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/VirtualEmbryo/delaunay-watershed
 project_urls = 
 	Team website = https://www.turlierlab.com/
 classifiers = 
 	Programming Language :: Python :: 3
-	License :: OSI Approved :: MIT License
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS
-	License :: OSI Approved :: MIT License
 	Intended Audience :: Science/Research
+license = CC BY-NC-SA 4.0
 
 [options]
 include_package_data = True
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
```

### Comparing `delaunay_watershed_3d-0.2.5/src/delaunay_watershed_3d.egg-info/PKG-INFO` & `delaunay_watershed_3d-0.2.8/src/delaunay_watershed_3d.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: delaunay-watershed-3d
-Version: 0.2.5
+Version: 0.2.8
 Summary: Geometrical reconstruction of cell assemblies from instance segmentations
 Home-page: https://github.com/VirtualEmbryo/delaunay-watershed
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
+License: CC BY-NC-SA 4.0
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Delaunay-Watershed 3D
 
 <img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Figure_logo_white_arrow.png" alt="drawing" width="300"/>
```

### Comparing `delaunay_watershed_3d-0.2.5/src/delaunay_watershed_3d.egg-info/SOURCES.txt` & `delaunay_watershed_3d-0.2.8/src/delaunay_watershed_3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.5/src/dw3d/Curvature.py` & `delaunay_watershed_3d-0.2.8/src/dw3d/Curvature.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.5/src/dw3d/Dcel.py` & `delaunay_watershed_3d-0.2.8/src/dw3d/Dcel.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.5/src/dw3d/Geometric_utilities.py` & `delaunay_watershed_3d-0.2.8/src/dw3d/Geometric_utilities.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.5/src/dw3d/Geometry.py` & `delaunay_watershed_3d-0.2.8/src/dw3d/Geometry.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.5/src/dw3d/Graph_functions.py` & `delaunay_watershed_3d-0.2.8/src/dw3d/Graph_functions.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.5/src/dw3d/Mask_reconstruction.py` & `delaunay_watershed_3d-0.2.8/src/dw3d/Mask_reconstruction.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.5/src/dw3d/Mesh_utilities.py` & `delaunay_watershed_3d-0.2.8/src/dw3d/Mesh_utilities.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.5/src/dw3d/Networkx_functions.py` & `delaunay_watershed_3d-0.2.8/src/dw3d/Networkx_functions.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.5/src/dw3d/functions.py` & `delaunay_watershed_3d-0.2.8/src/dw3d/functions.py`

 * *Files identical despite different names*

