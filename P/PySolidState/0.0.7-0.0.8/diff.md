# Comparing `tmp/PySolidState-0.0.7.tar.gz` & `tmp/PySolidState-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySolidState-0.0.7.tar", last modified: Sun Jul 16 01:48:25 2023, max compression
+gzip compressed data, was "PySolidState-0.0.8.tar", last modified: Mon Jul 17 14:01:05 2023, max compression
```

## Comparing `PySolidState-0.0.7.tar` & `PySolidState-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 01:48:25.887492 PySolidState-0.0.7/
--rw-rw-rw-   0        0        0     1122 2023-07-16 01:48:25.886490 PySolidState-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-16 01:48:25.846495 PySolidState-0.0.7/PySolidState/
--rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.7/PySolidState/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 01:48:25.883493 PySolidState-0.0.7/PySolidState/crystal_structure/
--rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.7/PySolidState/crystal_structure/__init__.py
--rw-rw-rw-   0        0        0      786 2023-07-08 17:20:16.000000 PySolidState-0.0.7/PySolidState/crystal_structure/atom.py
--rw-rw-rw-   0        0        0     7666 2023-07-16 00:27:04.000000 PySolidState-0.0.7/PySolidState/crystal_structure/base.py
--rw-rw-rw-   0        0        0     7067 2023-07-16 00:26:51.000000 PySolidState-0.0.7/PySolidState/crystal_structure/crystalStructure.py
--rw-rw-rw-   0        0        0    16610 2023-07-16 01:44:51.000000 PySolidState-0.0.7/PySolidState/crystal_structure/lattice.py
--rw-rw-rw-   0        0        0     3431 2023-07-08 17:20:16.000000 PySolidState-0.0.7/PySolidState/crystal_structure/lattices.json
-drwxrwxrwx   0        0        0        0 2023-07-16 01:48:25.867492 PySolidState-0.0.7/PySolidState.egg-info/
--rw-rw-rw-   0        0        0     1122 2023-07-16 01:48:25.000000 PySolidState-0.0.7/PySolidState.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-07-16 01:48:25.000000 PySolidState-0.0.7/PySolidState.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 01:48:25.000000 PySolidState-0.0.7/PySolidState.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-16 01:48:25.000000 PySolidState-0.0.7/PySolidState.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-16 01:48:25.000000 PySolidState-0.0.7/PySolidState.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      416 2023-07-16 01:06:43.000000 PySolidState-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 01:48:25.888493 PySolidState-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1307 2023-07-16 01:48:20.000000 PySolidState-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:01:05.665491 PySolidState-0.0.8/
+-rw-rw-rw-   0        0        0     1122 2023-07-17 14:01:05.663490 PySolidState-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-17 14:01:05.628490 PySolidState-0.0.8/PySolidState/
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.8/PySolidState/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:01:05.661487 PySolidState-0.0.8/PySolidState/crystal_structure/
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.8/PySolidState/crystal_structure/__init__.py
+-rw-rw-rw-   0        0        0      786 2023-07-08 17:20:16.000000 PySolidState-0.0.8/PySolidState/crystal_structure/atom.py
+-rw-rw-rw-   0        0        0     7666 2023-07-16 00:27:04.000000 PySolidState-0.0.8/PySolidState/crystal_structure/base.py
+-rw-rw-rw-   0        0        0     7067 2023-07-16 00:26:51.000000 PySolidState-0.0.8/PySolidState/crystal_structure/crystalStructure.py
+-rw-rw-rw-   0        0        0    16788 2023-07-17 13:58:51.000000 PySolidState-0.0.8/PySolidState/crystal_structure/lattice.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:01:05.645491 PySolidState-0.0.8/PySolidState.egg-info/
+-rw-rw-rw-   0        0        0     1122 2023-07-17 14:01:05.000000 PySolidState-0.0.8/PySolidState.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2023-07-17 14:01:05.000000 PySolidState-0.0.8/PySolidState.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 14:01:05.000000 PySolidState-0.0.8/PySolidState.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-17 14:01:05.000000 PySolidState-0.0.8/PySolidState.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-17 14:01:05.000000 PySolidState-0.0.8/PySolidState.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      416 2023-07-16 01:06:43.000000 PySolidState-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 14:01:05.666495 PySolidState-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1307 2023-07-17 14:00:19.000000 PySolidState-0.0.8/setup.py
```

### Comparing `PySolidState-0.0.7/PKG-INFO` & `PySolidState-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.0.7
+Version: 0.0.8
 Summary: PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.
 Home-page: https://github.com/miguelta281/PySolidState
 Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe
 Author-email: makesens19@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PySolidState-0.0.7/PySolidState/crystal_structure/atom.py` & `PySolidState-0.0.8/PySolidState/crystal_structure/atom.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.0.7/PySolidState/crystal_structure/base.py` & `PySolidState-0.0.8/PySolidState/crystal_structure/base.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.0.7/PySolidState/crystal_structure/crystalStructure.py` & `PySolidState-0.0.8/PySolidState/crystal_structure/crystalStructure.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.0.7/PySolidState/crystal_structure/lattice.py` & `PySolidState-0.0.8/PySolidState/crystal_structure/lattice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from mpl_toolkits.mplot3d import Axes3D
 import json
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
+import pkg_resources
 
 
 class Lattice:
     def __init__(self, system: str = None, structure_type: str = None, magnitude: tuple = None, angles: tuple = None, dimension: str = '2D'):
 
         """
         Constructor of the Lattice class that represents a crystalline lattice in a three-dimensional system.
@@ -25,15 +26,18 @@
         
         self.dimension = dimension
         self.__system = system
         self.__structure_type = structure_type
 
         # Verificar si se van a utilizar sistemas predefinidos
         if system is not None:
-            with open('./PySolidState/crystal_structure\\lattices.json', "r") as file:
+            file_path = pkg_resources.resource_filename('PySolidState', 'crystal_structure/lattices.json')
+
+            # Leer el archivo
+            with open(file_path) as file:
                 lattices = json.load(file)
             
             self.magnitude = lattices[self.dimension][self.__system]['magnitude']
             self.angles = lattices[self.dimension][self.__system]['angles']
             if dimension == '2D':
                 self.__angles_radian = tuple(np.math.radians(degree) for degree in (90,90,lattices[self.dimension][self.__system]['angles'][2]))
             else:
@@ -250,16 +254,18 @@
         # Create the meshgrid of points
         v1, v2, v3 = np.meshgrid(v1_range, v2_range, v3_range)
 
         # Combine the points into a single array
         points_v = np.vstack([v1.ravel(), v2.ravel(), v3.ravel()]).T
 
 
-        # Load lattices.json
-        with open('./PySolidState/crystal_structure\\lattices.json', "r") as file:
+        file_path = pkg_resources.resource_filename('PySolidState', 'crystal_structure/lattices.json')
+
+        # Leer el archivo
+        with open(file_path) as file:
             lattices = json.load(file)
 
         if (self.__structure_type is not None):
             if (self.__structure_type in lattices[self.dimension][self.__system]['structure_type']):
                 if self.__structure_type == 'centered':
                     v1_centered, v2_centered, v3_centered = np.meshgrid(v1_range + 0.5, v2_range + 0.5, v3_range)
                     points_centered = np.vstack([v1_centered.ravel(), v2_centered.ravel(), v3_centered.ravel()]).T
@@ -322,8 +328,8 @@
              self.magnitude[2] * np.sqrt(
                 1 - np.cos(self.__angles_radian[0]) ** 2 - np.cos(self.__angles_radian[1]) ** 2 - np.cos(
                     self.__angles_radian[2]) ** 2 + 2 * np.cos(self.__angles_radian[0]) * np.cos(
                     self.__angles_radian[1]) * np.cos(self.__angles_radian[2])) / np.sin(self.__angles_radian[2])]])
 
         points_x = np.dot(points_v, T)
         return points_x
-    
+
```

### Comparing `PySolidState-0.0.7/PySolidState.egg-info/PKG-INFO` & `PySolidState-0.0.8/PySolidState.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.0.7
+Version: 0.0.8
 Summary: PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.
 Home-page: https://github.com/miguelta281/PySolidState
 Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe
 Author-email: makesens19@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PySolidState-0.0.7/setup.py` & `PySolidState-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="PySolidState",
-    version="0.0.7",
+    version="0.0.8",
     description="PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelta281/PySolidState",
     author="Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe",
     author_email="makesens19@gmail.com",
     license="GNU General Public License v3.0",
```

