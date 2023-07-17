# Comparing `tmp/gunfolds-0.7.tar.gz` & `tmp/gunfolds-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gunfolds-0.7.tar", last modified: Fri May 19 19:54:55 2023, max compression
+gzip compressed data, was "gunfolds-0.8.tar", last modified: Fri May 19 20:18:27 2023, max compression
```

## Comparing `gunfolds-0.7.tar` & `gunfolds-0.8.tar`

### file list

```diff
@@ -1,27 +1,55 @@
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:54:55.350335 gunfolds-0.7/
--rw-r--r--   0 gm         (501) staff       (20)    35121 2023-05-18 18:49:59.000000 gunfolds-0.7/LICENSE
--rw-r--r--   0 gm         (501) staff       (20)       50 2023-05-18 18:49:59.000000 gunfolds-0.7/MANIFEST.in
--rw-r--r--   0 gm         (501) staff       (20)      577 2023-05-19 19:54:55.350117 gunfolds-0.7/PKG-INFO
--rw-r--r--   0 gm         (501) staff       (20)      293 2023-05-18 18:49:59.000000 gunfolds-0.7/README.md
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:54:55.333399 gunfolds-0.7/gunfolds/
--rw-r--r--   0 gm         (501) staff       (20)       92 2023-05-19 19:54:10.000000 gunfolds-0.7/gunfolds/__init__.py
--rw-r--r--   0 gm         (501) staff       (20)    23098 2023-05-18 18:49:59.000000 gunfolds-0.7/gunfolds/conversions.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:54:55.347693 gunfolds-0.7/gunfolds/data/
--rw-r--r--   0 gm         (501) staff       (20)  5002273 2023-05-18 18:49:59.000000 gunfolds-0.7/gunfolds/data/allloops.zkl
--rw-r--r--   0 gm         (501) staff       (20)  1852335 2023-05-18 18:49:59.000000 gunfolds-0.7/gunfolds/data/circular_p.zkl
--rw-r--r--   0 gm         (501) staff       (20)     3987 2023-05-18 18:49:59.000000 gunfolds-0.7/gunfolds/data/colors.zkl
--rw-r--r--   0 gm         (501) staff       (20)     3691 2023-05-18 18:49:59.000000 gunfolds-0.7/gunfolds/data/testgraphs.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:54:55.349164 gunfolds-0.7/gunfolds/figures/
--rw-r--r--   0 gm         (501) staff       (20)     2976 2023-05-18 18:49:59.000000 gunfolds-0.7/gunfolds/figures/shipfig.tex
--rw-r--r--   0 gm         (501) staff       (20)     1412 2023-05-18 18:49:59.000000 gunfolds-0.7/gunfolds/figures/shippage.sty
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:54:55.334698 gunfolds-0.7/gunfolds.egg-info/
--rw-r--r--   0 gm         (501) staff       (20)      577 2023-05-19 19:54:55.000000 gunfolds-0.7/gunfolds.egg-info/PKG-INFO
--rw-r--r--   0 gm         (501) staff       (20)      456 2023-05-19 19:54:55.000000 gunfolds-0.7/gunfolds.egg-info/SOURCES.txt
--rw-r--r--   0 gm         (501) staff       (20)        1 2023-05-19 19:54:55.000000 gunfolds-0.7/gunfolds.egg-info/dependency_links.txt
--rw-r--r--   0 gm         (501) staff       (20)        1 2023-05-19 19:54:55.000000 gunfolds-0.7/gunfolds.egg-info/not-zip-safe
--rw-r--r--   0 gm         (501) staff       (20)       95 2023-05-19 19:54:55.000000 gunfolds-0.7/gunfolds.egg-info/requires.txt
--rw-r--r--   0 gm         (501) staff       (20)        9 2023-05-19 19:54:55.000000 gunfolds-0.7/gunfolds.egg-info/top_level.txt
--rw-r--r--   0 gm         (501) staff       (20)       38 2023-05-19 19:54:55.350421 gunfolds-0.7/setup.cfg
--rw-r--r--   0 gm         (501) staff       (20)     1239 2023-05-19 19:54:21.000000 gunfolds-0.7/setup.py
-drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 19:54:55.349456 gunfolds-0.7/tests/
--rw-r--r--   0 gm         (501) staff       (20)    20222 2023-05-18 18:49:59.000000 gunfolds-0.7/tests/tests.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 20:18:27.612903 gunfolds-0.8/
+-rw-r--r--   0 gm         (501) staff       (20)    35121 2023-05-18 18:49:59.000000 gunfolds-0.8/LICENSE
+-rw-r--r--   0 gm         (501) staff       (20)       50 2023-05-18 18:49:59.000000 gunfolds-0.8/MANIFEST.in
+-rw-r--r--   0 gm         (501) staff       (20)      577 2023-05-19 20:18:27.612684 gunfolds-0.8/PKG-INFO
+-rw-r--r--   0 gm         (501) staff       (20)      293 2023-05-18 18:49:59.000000 gunfolds-0.8/README.md
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 20:18:27.588531 gunfolds-0.8/gunfolds/
+-rw-r--r--   0 gm         (501) staff       (20)        0 2023-05-19 20:17:41.000000 gunfolds-0.8/gunfolds/__init__.py
+-rw-r--r--   0 gm         (501) staff       (20)    23098 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/conversions.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 20:18:27.602759 gunfolds-0.8/gunfolds/data/
+-rw-r--r--   0 gm         (501) staff       (20)  5002273 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/data/allloops.zkl
+-rw-r--r--   0 gm         (501) staff       (20)  1852335 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/data/circular_p.zkl
+-rw-r--r--   0 gm         (501) staff       (20)     3987 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/data/colors.zkl
+-rw-r--r--   0 gm         (501) staff       (20)     3691 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/data/testgraphs.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 20:18:27.604828 gunfolds-0.8/gunfolds/estimation/
+-rw-r--r--   0 gm         (501) staff       (20)        0 2023-05-19 19:17:53.000000 gunfolds-0.8/gunfolds/estimation/__init__.py
+-rw-r--r--   0 gm         (501) staff       (20)     2676 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/estimation/grangercausality.py
+-rw-r--r--   0 gm         (501) staff       (20)    25353 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/estimation/linear_model.py
+-rw-r--r--   0 gm         (501) staff       (20)     5904 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/estimation/pc.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 20:18:27.605480 gunfolds-0.8/gunfolds/figures/
+-rw-r--r--   0 gm         (501) staff       (20)     2976 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/figures/shipfig.tex
+-rw-r--r--   0 gm         (501) staff       (20)     1412 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/figures/shippage.sty
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 20:18:27.607284 gunfolds-0.8/gunfolds/solvers/
+-rw-r--r--   0 gm         (501) staff       (20)        0 2023-05-19 19:17:45.000000 gunfolds-0.8/gunfolds/solvers/__init__.py
+-rw-r--r--   0 gm         (501) staff       (20)     4156 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/solvers/clingo_msl.py
+-rw-r--r--   0 gm         (501) staff       (20)    14841 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/solvers/clingo_rasl.py
+-rw-r--r--   0 gm         (501) staff       (20)    43259 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/solvers/traversal.py
+-rw-r--r--   0 gm         (501) staff       (20)    18670 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/solvers/unknownrate.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 20:18:27.610552 gunfolds-0.8/gunfolds/utils/
+-rw-r--r--   0 gm         (501) staff       (20)      816 2023-05-19 19:17:34.000000 gunfolds-0.8/gunfolds/utils/__init__.py
+-rw-r--r--   0 gm         (501) staff       (20)    15415 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/utils/bfutils.py
+-rw-r--r--   0 gm         (501) staff       (20)     1130 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/utils/calc_procs.py
+-rw-r--r--   0 gm         (501) staff       (20)     3188 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/utils/clingo.py
+-rw-r--r--   0 gm         (501) staff       (20)     3684 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/utils/comparison.py
+-rw-r--r--   0 gm         (501) staff       (20)     4344 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/utils/ecj.py
+-rw-r--r--   0 gm         (501) staff       (20)    31572 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/utils/graphkit.py
+-rw-r--r--   0 gm         (501) staff       (20)     2332 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/utils/myTimeout.py
+-rw-r--r--   0 gm         (501) staff       (20)     3368 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/utils/neighborhoods.py
+-rw-r--r--   0 gm         (501) staff       (20)      864 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/utils/simpleloops.py
+-rw-r--r--   0 gm         (501) staff       (20)     1235 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/utils/zickle.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 20:18:27.611571 gunfolds-0.8/gunfolds/viz/
+-rw-r--r--   0 gm         (501) staff       (20)        0 2023-05-19 19:16:37.000000 gunfolds-0.8/gunfolds/viz/__init__.py
+-rw-r--r--   0 gm         (501) staff       (20)    20874 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/viz/dbn2latex.py
+-rw-r--r--   0 gm         (501) staff       (20)    10784 2023-05-18 18:49:59.000000 gunfolds-0.8/gunfolds/viz/gtool.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 20:18:27.590014 gunfolds-0.8/gunfolds.egg-info/
+-rw-r--r--   0 gm         (501) staff       (20)      577 2023-05-19 20:18:27.000000 gunfolds-0.8/gunfolds.egg-info/PKG-INFO
+-rw-r--r--   0 gm         (501) staff       (20)     1135 2023-05-19 20:18:27.000000 gunfolds-0.8/gunfolds.egg-info/SOURCES.txt
+-rw-r--r--   0 gm         (501) staff       (20)        1 2023-05-19 20:18:27.000000 gunfolds-0.8/gunfolds.egg-info/dependency_links.txt
+-rw-r--r--   0 gm         (501) staff       (20)        1 2023-05-19 19:54:55.000000 gunfolds-0.8/gunfolds.egg-info/not-zip-safe
+-rw-r--r--   0 gm         (501) staff       (20)       95 2023-05-19 20:18:27.000000 gunfolds-0.8/gunfolds.egg-info/requires.txt
+-rw-r--r--   0 gm         (501) staff       (20)       15 2023-05-19 20:18:27.000000 gunfolds-0.8/gunfolds.egg-info/top_level.txt
+-rw-r--r--   0 gm         (501) staff       (20)       38 2023-05-19 20:18:27.612986 gunfolds-0.8/setup.cfg
+-rw-r--r--   0 gm         (501) staff       (20)     1257 2023-05-19 20:17:52.000000 gunfolds-0.8/setup.py
+drwxr-xr-x   0 gm         (501) staff       (20)        0 2023-05-19 20:18:27.612246 gunfolds-0.8/tests/
+-rw-r--r--   0 gm         (501) staff       (20)        0 2023-05-18 18:49:59.000000 gunfolds-0.8/tests/__init__.py
+-rw-r--r--   0 gm         (501) staff       (20)    20222 2023-05-18 18:49:59.000000 gunfolds-0.8/tests/tests.py
```

### Comparing `gunfolds-0.7/LICENSE` & `gunfolds-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gunfolds-0.7/PKG-INFO` & `gunfolds-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gunfolds
-Version: 0.7
+Version: 0.8
 Summary: Tools to explore dynamic causal graphs in the case of undersampled data
 Author: Sergey Plis, Cynthia Freeman, Ian Beaver
 Author-email: splis@mrn.org
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gunfolds-0.7/gunfolds/conversions.py` & `gunfolds-0.8/gunfolds/conversions.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.7/gunfolds/data/allloops.zkl` & `gunfolds-0.8/gunfolds/data/allloops.zkl`

 * *Files identical despite different names*

### Comparing `gunfolds-0.7/gunfolds/data/circular_p.zkl` & `gunfolds-0.8/gunfolds/data/circular_p.zkl`

 * *Files identical despite different names*

### Comparing `gunfolds-0.7/gunfolds/data/colors.zkl` & `gunfolds-0.8/gunfolds/data/colors.zkl`

 * *Files identical despite different names*

### Comparing `gunfolds-0.7/gunfolds/data/testgraphs.py` & `gunfolds-0.8/gunfolds/data/testgraphs.py`

 * *Files identical despite different names*

### Comparing `gunfolds-0.7/gunfolds/figures/shipfig.tex` & `gunfolds-0.8/gunfolds/figures/shipfig.tex`

 * *Files identical despite different names*

### Comparing `gunfolds-0.7/gunfolds/figures/shippage.sty` & `gunfolds-0.8/gunfolds/figures/shippage.sty`

 * *Files identical despite different names*

### Comparing `gunfolds-0.7/gunfolds.egg-info/PKG-INFO` & `gunfolds-0.8/gunfolds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gunfolds
-Version: 0.7
+Version: 0.8
 Summary: Tools to explore dynamic causal graphs in the case of undersampled data
 Author: Sergey Plis, Cynthia Freeman, Ian Beaver
 Author-email: splis@mrn.org
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gunfolds-0.7/setup.py` & `gunfolds-0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup
+from setuptools import find_packages, setup
 
 with open('README.md') as description:
     description = description.read()
 
 exec(open('version.py').read()) # Acquire version constants.
 
 # Define some package entry points. These will be command-line scripts that get
@@ -17,19 +17,19 @@
 
 tests_require = install_requires
 
 setup(
     name='gunfolds',
     description='Tools to explore dynamic causal graphs in the case of undersampled data',
     long_description_content_type="text/markdown",
-    version=0.7,
+    version=0.8,
     author='Sergey Plis, Cynthia Freeman, Ian Beaver',
     author_email='splis@mrn.org',
     license='GPL',
     long_description=description,
     include_package_data=True, # Include files listed in MANIFEST.in
-    packages=['gunfolds'], # Sub-packages must be explicitly listed.
+    packages=find_packages(), # Sub-packages must be explicitly listed.
     #entry_points=epoints,
     install_requires=install_requires, # List of dependencies.
     test_suite='tests.tests',
     tests_require=tests_require,
     zip_safe=False) # Override annoying default behavior of easy_install.
```

### Comparing `gunfolds-0.7/tests/tests.py` & `gunfolds-0.8/tests/tests.py`

 * *Files identical despite different names*

