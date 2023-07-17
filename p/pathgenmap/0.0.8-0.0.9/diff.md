# Comparing `tmp/pathgenmap-0.0.8.tar.gz` & `tmp/pathgenmap-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathgenmap-0.0.8.tar", last modified: Fri Jul 14 00:06:22 2023, max compression
+gzip compressed data, was "pathgenmap-0.0.9.tar", last modified: Fri Jul 14 00:10:14 2023, max compression
```

## Comparing `pathgenmap-0.0.8.tar` & `pathgenmap-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-14 00:06:22.580023 pathgenmap-0.0.8/
--rw-r--r--   0 marcossousa   (501) staff       (20)     1083 2023-07-13 00:05:25.000000 pathgenmap-0.0.8/LICENSE
--rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-14 00:06:22.579383 pathgenmap-0.0.8/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      740 2023-07-13 21:56:31.000000 pathgenmap-0.0.8/README.md
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-14 00:06:22.574100 pathgenmap-0.0.8/pathgenmap/
--rw-r--r--   0 marcossousa   (501) staff       (20)     1307 2023-07-13 00:07:52.000000 pathgenmap-0.0.8/pathgenmap/EggAnnot.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     3011 2023-07-13 13:17:10.000000 pathgenmap-0.0.8/pathgenmap/Integration.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     1889 2023-07-13 11:28:07.000000 pathgenmap-0.0.8/pathgenmap/PathAnalys.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     1140 2023-07-14 00:06:16.000000 pathgenmap-0.0.8/pathgenmap/PathGenMap.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     1205 2023-07-13 11:46:42.000000 pathgenmap-0.0.8/pathgenmap/SpeciesAbundance.py
--rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-07-13 00:03:39.000000 pathgenmap-0.0.8/pathgenmap/__init__.py
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-14 00:06:22.578335 pathgenmap-0.0.8/pathgenmap.egg-info/
--rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-14 00:06:22.000000 pathgenmap-0.0.8/pathgenmap.egg-info/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      385 2023-07-14 00:06:22.000000 pathgenmap-0.0.8/pathgenmap.egg-info/SOURCES.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-07-14 00:06:22.000000 pathgenmap-0.0.8/pathgenmap.egg-info/dependency_links.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       59 2023-07-14 00:06:22.000000 pathgenmap-0.0.8/pathgenmap.egg-info/entry_points.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       27 2023-07-14 00:06:22.000000 pathgenmap-0.0.8/pathgenmap.egg-info/requires.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       11 2023-07-14 00:06:22.000000 pathgenmap-0.0.8/pathgenmap.egg-info/top_level.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-07-14 00:06:22.580284 pathgenmap-0.0.8/setup.cfg
--rw-r--r--   0 marcossousa   (501) staff       (20)      655 2023-07-14 00:06:16.000000 pathgenmap-0.0.8/setup.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-14 00:10:14.500530 pathgenmap-0.0.9/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1083 2023-07-13 00:05:25.000000 pathgenmap-0.0.9/LICENSE
+-rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-14 00:10:14.499904 pathgenmap-0.0.9/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      740 2023-07-13 21:56:31.000000 pathgenmap-0.0.9/README.md
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-14 00:10:14.493083 pathgenmap-0.0.9/pathgenmap/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1307 2023-07-13 00:07:52.000000 pathgenmap-0.0.9/pathgenmap/EggAnnot.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     3014 2023-07-14 00:10:06.000000 pathgenmap-0.0.9/pathgenmap/Integration.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1889 2023-07-13 11:28:07.000000 pathgenmap-0.0.9/pathgenmap/PathAnalys.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1140 2023-07-14 00:06:16.000000 pathgenmap-0.0.9/pathgenmap/PathGenMap.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1205 2023-07-13 11:46:42.000000 pathgenmap-0.0.9/pathgenmap/SpeciesAbundance.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-07-13 00:03:39.000000 pathgenmap-0.0.9/pathgenmap/__init__.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-14 00:10:14.498015 pathgenmap-0.0.9/pathgenmap.egg-info/
+-rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-14 00:10:14.000000 pathgenmap-0.0.9/pathgenmap.egg-info/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      385 2023-07-14 00:10:14.000000 pathgenmap-0.0.9/pathgenmap.egg-info/SOURCES.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-07-14 00:10:14.000000 pathgenmap-0.0.9/pathgenmap.egg-info/dependency_links.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       59 2023-07-14 00:10:14.000000 pathgenmap-0.0.9/pathgenmap.egg-info/entry_points.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       27 2023-07-14 00:10:14.000000 pathgenmap-0.0.9/pathgenmap.egg-info/requires.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       11 2023-07-14 00:10:14.000000 pathgenmap-0.0.9/pathgenmap.egg-info/top_level.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-07-14 00:10:14.500755 pathgenmap-0.0.9/setup.cfg
+-rw-r--r--   0 marcossousa   (501) staff       (20)      655 2023-07-14 00:10:06.000000 pathgenmap-0.0.9/setup.py
```

### Comparing `pathgenmap-0.0.8/LICENSE` & `pathgenmap-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.8/README.md` & `pathgenmap-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.8/pathgenmap/EggAnnot.py` & `pathgenmap-0.0.9/pathgenmap/EggAnnot.py`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.8/pathgenmap/Integration.py` & `pathgenmap-0.0.9/pathgenmap/Integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
-from PathAnalys import PathwaysList
-from EggAnnot import EggNOG
-from SpeciesAbundance import SpeciesAbundance
+from .PathAnalys import PathwaysList
+from .EggAnnot import EggNOG
+from .SpeciesAbundance import SpeciesAbundance
 from tqdm import tqdm
 
 
 class Manager:
     def __init__(self):
         self.abundance = None
         self.eggnog = None
```

### Comparing `pathgenmap-0.0.8/pathgenmap/PathAnalys.py` & `pathgenmap-0.0.9/pathgenmap/PathAnalys.py`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.8/pathgenmap/PathGenMap.py` & `pathgenmap-0.0.9/pathgenmap/PathGenMap.py`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.8/pathgenmap/SpeciesAbundance.py` & `pathgenmap-0.0.9/pathgenmap/SpeciesAbundance.py`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.8/setup.py` & `pathgenmap-0.0.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pathgenmap",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(),
     install_requires=["pandas>=1.1.0", "tqdm>=4.48.0"],
     author="Marcos Paulo Alves de Sousa",
     author_email="msousa@museu-goeldi.br",
     description="PathGenMap is a comprehensive Python application designed to integrate pathway, annotation, and species abundance data.",
     license="MIT",
     keywords="pathway annotation species abundance",
```

