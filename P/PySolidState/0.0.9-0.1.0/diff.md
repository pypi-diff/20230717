# Comparing `tmp/PySolidState-0.0.9.tar.gz` & `tmp/PySolidState-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySolidState-0.0.9.tar", last modified: Mon Jul 17 14:13:17 2023, max compression
+gzip compressed data, was "PySolidState-0.1.0.tar", last modified: Mon Jul 17 14:20:34 2023, max compression
```

## Comparing `PySolidState-0.0.9.tar` & `PySolidState-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 14:13:17.013962 PySolidState-0.0.9/
--rw-rw-rw-   0        0        0     1122 2023-07-17 14:13:17.011961 PySolidState-0.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-17 14:13:16.858235 PySolidState-0.0.9/PySolidState/
--rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.9/PySolidState/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 14:13:17.008957 PySolidState-0.0.9/PySolidState/crystal_structure/
--rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.0.9/PySolidState/crystal_structure/__init__.py
--rw-rw-rw-   0        0        0      786 2023-07-08 17:20:16.000000 PySolidState-0.0.9/PySolidState/crystal_structure/atom.py
--rw-rw-rw-   0        0        0     7666 2023-07-16 00:27:04.000000 PySolidState-0.0.9/PySolidState/crystal_structure/base.py
--rw-rw-rw-   0        0        0     7067 2023-07-16 00:26:51.000000 PySolidState-0.0.9/PySolidState/crystal_structure/crystalStructure.py
--rw-rw-rw-   0        0        0    16788 2023-07-17 13:58:51.000000 PySolidState-0.0.9/PySolidState/crystal_structure/lattice.py
-drwxrwxrwx   0        0        0        0 2023-07-17 14:13:16.993579 PySolidState-0.0.9/PySolidState.egg-info/
--rw-rw-rw-   0        0        0     1122 2023-07-17 14:13:16.000000 PySolidState-0.0.9/PySolidState.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      436 2023-07-17 14:13:16.000000 PySolidState-0.0.9/PySolidState.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 14:13:16.000000 PySolidState-0.0.9/PySolidState.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-17 14:13:16.000000 PySolidState-0.0.9/PySolidState.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-17 14:13:16.000000 PySolidState-0.0.9/PySolidState.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      416 2023-07-16 01:06:43.000000 PySolidState-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 14:13:17.013962 PySolidState-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1205 2023-07-17 14:13:08.000000 PySolidState-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:20:34.966346 PySolidState-0.1.0/
+-rw-rw-rw-   0        0        0     1122 2023-07-17 14:20:34.965360 PySolidState-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-17 14:20:34.914348 PySolidState-0.1.0/PySolidState/
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.1.0/PySolidState/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 14:20:34.961349 PySolidState-0.1.0/PySolidState/crystal_structure/
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.1.0/PySolidState/crystal_structure/__init__.py
+-rw-rw-rw-   0        0        0      786 2023-07-08 17:20:16.000000 PySolidState-0.1.0/PySolidState/crystal_structure/atom.py
+-rw-rw-rw-   0        0        0     7666 2023-07-16 00:27:04.000000 PySolidState-0.1.0/PySolidState/crystal_structure/base.py
+-rw-rw-rw-   0        0        0     7067 2023-07-16 00:26:51.000000 PySolidState-0.1.0/PySolidState/crystal_structure/crystalStructure.py
+-rw-rw-rw-   0        0        0    16788 2023-07-17 13:58:51.000000 PySolidState-0.1.0/PySolidState/crystal_structure/lattice.py
+-rw-rw-rw-   0        0        0     3431 2023-07-08 17:20:16.000000 PySolidState-0.1.0/PySolidState/crystal_structure/lattices.json
+drwxrwxrwx   0        0        0        0 2023-07-17 14:20:34.942349 PySolidState-0.1.0/PySolidState.egg-info/
+-rw-rw-rw-   0        0        0     1122 2023-07-17 14:20:34.000000 PySolidState-0.1.0/PySolidState.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2023-07-17 14:20:34.000000 PySolidState-0.1.0/PySolidState.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 14:20:34.000000 PySolidState-0.1.0/PySolidState.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-17 14:20:34.000000 PySolidState-0.1.0/PySolidState.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-17 14:20:34.000000 PySolidState-0.1.0/PySolidState.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      416 2023-07-16 01:06:43.000000 PySolidState-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 14:20:34.967347 PySolidState-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1371 2023-07-17 14:20:25.000000 PySolidState-0.1.0/setup.py
```

### Comparing `PySolidState-0.0.9/PKG-INFO` & `PySolidState-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.0.9
+Version: 0.1.0
 Summary: PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.
 Home-page: https://github.com/miguelta281/PySolidState
 Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe
 Author-email: makesens19@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PySolidState-0.0.9/PySolidState/crystal_structure/atom.py` & `PySolidState-0.1.0/PySolidState/crystal_structure/atom.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.0.9/PySolidState/crystal_structure/base.py` & `PySolidState-0.1.0/PySolidState/crystal_structure/base.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.0.9/PySolidState/crystal_structure/crystalStructure.py` & `PySolidState-0.1.0/PySolidState/crystal_structure/crystalStructure.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.0.9/PySolidState/crystal_structure/lattice.py` & `PySolidState-0.1.0/PySolidState/crystal_structure/lattice.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.0.9/PySolidState.egg-info/PKG-INFO` & `PySolidState-0.1.0/PySolidState.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySolidState
-Version: 0.0.9
+Version: 0.1.0
 Summary: PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.
 Home-page: https://github.com/miguelta281/PySolidState
 Author: Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe
 Author-email: makesens19@gmail.com
 License: GNU General Public License v3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PySolidState-0.0.9/setup.py` & `PySolidState-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,23 +6,28 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="PySolidState",
-    version="0.0.9",
+    version="0.1.0",
     description="PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelta281/PySolidState",
     author="Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe",
     author_email="makesens19@gmail.com",
     license="GNU General Public License v3.0",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
     ],
+    package_data={
+    'PySolidState': ['crystal_structure/lattices.json'],
+    },
     packages=["PySolidState", "PySolidState.crystal_structure"],
     include_package_data=True,
+    data_files=[('data', ['PySolidState/crystal_structure/lattices.json'])],
+
     install_requires=["numpy", "matplotlib","mayavi"]
 )
```

