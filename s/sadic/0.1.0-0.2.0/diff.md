# Comparing `tmp/sadic-0.1.0.tar.gz` & `tmp/sadic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sadic-0.1.0.tar", last modified: Thu May  4 11:11:20 2023, max compression
+gzip compressed data, was "sadic-0.2.0.tar", last modified: Mon Jul 17 15:20:36 2023, max compression
```

## Comparing `sadic-0.1.0.tar` & `sadic-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-05-04 11:11:20.398873 sadic-0.1.0/
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)     1073 2023-05-04 09:36:44.000000 sadic-0.1.0/LICENSE
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)     1039 2023-05-04 11:11:20.388873 sadic-0.1.0/PKG-INFO
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)       83 2022-12-22 13:05:48.000000 sadic-0.1.0/README.md
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)       80 2023-05-04 09:24:50.000000 sadic-0.1.0/pyproject.toml
-drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-05-04 11:11:20.348873 sadic-0.1.0/sadic/
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)      199 2023-05-04 11:09:38.000000 sadic-0.1.0/sadic/__init__.py
-drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-05-04 11:11:20.358873 sadic-0.1.0/sadic/algorithm/
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)        0 2023-05-04 08:58:14.000000 sadic-0.1.0/sadic/algorithm/__init__.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)     8289 2023-05-04 08:52:53.000000 sadic-0.1.0/sadic/algorithm/depth.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)     5791 2023-05-04 08:52:40.000000 sadic-0.1.0/sadic/algorithm/radius.py
-drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-05-04 11:11:20.358873 sadic-0.1.0/sadic/pdb/
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)       57 2023-05-04 10:57:49.000000 sadic-0.1.0/sadic/pdb/__init__.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)     5165 2023-02-17 16:33:15.000000 sadic-0.1.0/sadic/pdb/pdbentity.py
-drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-05-04 11:11:20.368873 sadic-0.1.0/sadic/quantizer/
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)      587 2023-05-04 10:58:17.000000 sadic-0.1.0/sadic/quantizer/__init__.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)     5635 2023-05-04 08:57:06.000000 sadic-0.1.0/sadic/quantizer/quantizer.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)      890 2023-05-04 11:05:37.000000 sadic-0.1.0/sadic/sadic.py
-drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-05-04 11:11:20.378873 sadic-0.1.0/sadic/solid/
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)      134 2023-05-04 10:56:30.000000 sadic-0.1.0/sadic/solid/__init__.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)     7888 2023-05-04 08:59:15.000000 sadic-0.1.0/sadic/solid/multisphere.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)      310 2023-02-02 17:06:25.000000 sadic-0.1.0/sadic/solid/solid.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)      974 2023-05-04 08:54:46.000000 sadic-0.1.0/sadic/solid/sphere.py
-drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-05-04 11:11:20.388873 sadic-0.1.0/sadic/utils/
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)       77 2023-05-04 10:56:48.000000 sadic-0.1.0/sadic/utils/__init__.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)       25 2023-04-17 10:08:29.000000 sadic-0.1.0/sadic/utils/config.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)     1246 2023-02-02 15:09:58.000000 sadic-0.1.0/sadic/utils/typing.py
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)      278 2023-05-04 08:57:25.000000 sadic-0.1.0/sadic/utils/utils.py
-drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-05-04 11:11:20.358873 sadic-0.1.0/sadic.egg-info/
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)     1039 2023-05-04 11:11:20.000000 sadic-0.1.0/sadic.egg-info/PKG-INFO
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)      582 2023-05-04 11:11:20.000000 sadic-0.1.0/sadic.egg-info/SOURCES.txt
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)        1 2023-05-04 11:11:20.000000 sadic-0.1.0/sadic.egg-info/dependency_links.txt
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)       42 2023-05-04 11:11:20.000000 sadic-0.1.0/sadic.egg-info/requires.txt
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)        6 2023-05-04 11:11:20.000000 sadic-0.1.0/sadic.egg-info/top_level.txt
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)       38 2023-05-04 11:11:20.398873 sadic-0.1.0/setup.cfg
--rw-r--r--   0 giacomo   (1000) giacomo   (1000)     1688 2023-05-04 10:35:48.000000 sadic-0.1.0/setup.py
+drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 15:20:36.640895 sadic-0.2.0/
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)     1073 2023-05-04 09:36:44.000000 sadic-0.2.0/LICENSE
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)      849 2023-07-17 15:20:36.640895 sadic-0.2.0/PKG-INFO
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)       83 2022-12-22 13:05:48.000000 sadic-0.2.0/README.md
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)       80 2023-05-04 09:24:50.000000 sadic-0.2.0/pyproject.toml
+drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 15:20:36.590894 sadic-0.2.0/sadic/
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)      235 2023-07-17 15:16:22.000000 sadic-0.2.0/sadic/__init__.py
+drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 15:20:36.600894 sadic-0.2.0/sadic/algorithm/
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)       40 2023-06-28 16:12:31.000000 sadic-0.2.0/sadic/algorithm/__init__.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)    17154 2023-07-04 16:27:17.000000 sadic-0.2.0/sadic/algorithm/depth.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)    13902 2023-06-28 15:16:01.000000 sadic-0.2.0/sadic/algorithm/radius.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)     6694 2023-07-17 13:58:00.000000 sadic-0.2.0/sadic/api.py
+drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 15:20:36.610895 sadic-0.2.0/sadic/pdb/
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)      205 2023-07-05 12:45:05.000000 sadic-0.2.0/sadic/pdb/__init__.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)    28554 2023-07-13 10:01:30.000000 sadic-0.2.0/sadic/pdb/pdbentity.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)    34069 2023-07-17 14:24:23.000000 sadic-0.2.0/sadic/pdb/result.py
+drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 15:20:36.610895 sadic-0.2.0/sadic/quantizer/
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)      435 2023-06-28 16:12:33.000000 sadic-0.2.0/sadic/quantizer/__init__.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)    14689 2023-07-05 10:39:23.000000 sadic-0.2.0/sadic/quantizer/quantizer.py
+drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 15:20:36.630895 sadic-0.2.0/sadic/solid/
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)      222 2023-06-28 16:13:18.000000 sadic-0.2.0/sadic/solid/__init__.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)    14080 2023-07-05 09:01:23.000000 sadic-0.2.0/sadic/solid/multisphere.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)     1103 2023-07-05 10:39:58.000000 sadic-0.2.0/sadic/solid/solid.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)     2955 2023-07-05 09:00:29.000000 sadic-0.2.0/sadic/solid/sphere.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)    23834 2023-07-05 08:59:26.000000 sadic-0.2.0/sadic/solid/voxel_solid.py
+drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 15:20:36.640895 sadic-0.2.0/sadic/utils/
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)       80 2023-07-05 10:31:34.000000 sadic-0.2.0/sadic/utils/__init__.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)       81 2023-06-28 22:41:32.000000 sadic-0.2.0/sadic/utils/config.py
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)      273 2023-07-05 10:38:14.000000 sadic-0.2.0/sadic/utils/repr.py
+drwxr-xr-x   0 giacomo   (1000) giacomo   (1000)        0 2023-07-17 15:20:36.600894 sadic-0.2.0/sadic.egg-info/
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)      849 2023-07-17 15:20:36.000000 sadic-0.2.0/sadic.egg-info/PKG-INFO
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)      604 2023-07-17 15:20:36.000000 sadic-0.2.0/sadic.egg-info/SOURCES.txt
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)        1 2023-07-17 15:20:36.000000 sadic-0.2.0/sadic.egg-info/dependency_links.txt
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)       48 2023-07-17 15:20:36.000000 sadic-0.2.0/sadic.egg-info/requires.txt
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)        6 2023-07-17 15:20:36.000000 sadic-0.2.0/sadic.egg-info/top_level.txt
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)       38 2023-07-17 15:20:36.640895 sadic-0.2.0/setup.cfg
+-rw-r--r--   0 giacomo   (1000) giacomo   (1000)     1672 2023-07-05 10:01:38.000000 sadic-0.2.0/setup.py
```

### Comparing `sadic-0.1.0/LICENSE` & `sadic-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sadic-0.1.0/PKG-INFO` & `sadic-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: sadic
-Version: 0.1.0
+Version: 0.2.0
 Summary: Reimplementation as a python package of the software for Simple Atom Depth Index Calculator (SADIC)
 Home-page: https://github.com/nunziati/sadic
 Author: Giacomo Nunziati
 Author-email: giacomo.nunziati.0@gmail.com
 License: GNU General Public License v3.0
 Keywords: protein atom depth
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Natural Language :: Italian
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 License-File: LICENSE
 
 # sadic-v2
 Reimplementation of the software for Simple Atom Depth Index Calculator
```

### Comparing `sadic-0.1.0/sadic.egg-info/PKG-INFO` & `sadic-0.2.0/sadic.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: sadic
-Version: 0.1.0
+Version: 0.2.0
 Summary: Reimplementation as a python package of the software for Simple Atom Depth Index Calculator (SADIC)
 Home-page: https://github.com/nunziati/sadic
 Author: Giacomo Nunziati
 Author-email: giacomo.nunziati.0@gmail.com
 License: GNU General Public License v3.0
 Keywords: protein atom depth
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Natural Language :: Italian
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 License-File: LICENSE
 
 # sadic-v2
 Reimplementation of the software for Simple Atom Depth Index Calculator
```

### Comparing `sadic-0.1.0/sadic.egg-info/SOURCES.txt` & `sadic-0.2.0/sadic.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 sadic/__init__.py
-sadic/sadic.py
+sadic/api.py
 sadic.egg-info/PKG-INFO
 sadic.egg-info/SOURCES.txt
 sadic.egg-info/dependency_links.txt
 sadic.egg-info/requires.txt
 sadic.egg-info/top_level.txt
 sadic/algorithm/__init__.py
 sadic/algorithm/depth.py
 sadic/algorithm/radius.py
 sadic/pdb/__init__.py
 sadic/pdb/pdbentity.py
+sadic/pdb/result.py
 sadic/quantizer/__init__.py
 sadic/quantizer/quantizer.py
 sadic/solid/__init__.py
 sadic/solid/multisphere.py
 sadic/solid/solid.py
 sadic/solid/sphere.py
+sadic/solid/voxel_solid.py
 sadic/utils/__init__.py
 sadic/utils/config.py
-sadic/utils/typing.py
-sadic/utils/utils.py
+sadic/utils/repr.py
```

### Comparing `sadic-0.1.0/setup.py` & `sadic-0.2.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,53 @@
-from setuptools import setup
+r"""setup.py"""
+
 import os
 
+from setuptools import setup
+
+
 def read(fname):
-    return open(os.path.join(os.path.dirname(__file__), fname)).read()
+    r"""Reads a file and returns its content as a string."""
+    return open(os.path.join(os.path.dirname(__file__), fname), encoding="utf-8").read()
+
 
 def get_version(rel_path):
+    r"""Gets the version of the package from the __init__ file."""
     for line in read(rel_path).splitlines():
-        if line.startswith('__version__'):
+        if line.startswith("__version__"):
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
-    else:
-        raise RuntimeError("Unable to find version string.")
-    
+
+    raise RuntimeError("Unable to find version string.")
+
+
 setup(
-    name='sadic',
-    version=get_version("sadic/__init__.py"),    
-    description='Reimplementation as a python package of the software for Simple Atom Depth Index Calculator (SADIC)',
-    url='https://github.com/nunziati/sadic',
-    author='Giacomo Nunziati',
-    author_email='giacomo.nunziati.0@gmail.com',
-    license='GNU General Public License v3.0',
-    keywords = "protein atom depth",
-    long_description=read('README.md'),
-    packages=['sadic', 'sadic.algorithm', 'sadic.quantizer', 'sadic.utils', 'sadic.solid', 'sadic.pdb'],
-    install_requires=[
-        'numpy',
-        'biopandas',
-        'biopython',
-        'tqdm',
-        'matplotlib'
+    name="sadic",
+    version=get_version("sadic/__init__.py"),
+    description="Reimplementation as a python package of the software for Simple Atom Depth Index "
+    "Calculator (SADIC)",
+    url="https://github.com/nunziati/sadic",
+    author="Giacomo Nunziati",
+    author_email="giacomo.nunziati.0@gmail.com",
+    license="GNU General Public License v3.0",
+    keywords="protein atom depth",
+    long_description=read("README.md"),
+    packages=[
+        "sadic",
+        "sadic.algorithm",
+        "sadic.quantizer",
+        "sadic.utils",
+        "sadic.solid",
+        "sadic.pdb",
     ],
-
+    install_requires=["numpy", "scipy", "biopandas", "biopython", "tqdm", "matplotlib"],
     classifiers=[
-        'Development Status :: 1 - Planning',
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Natural Language :: Italian',
-        'Operating System :: POSIX :: Linux',
-        'Operating System :: Microsoft :: Windows',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Topic :: Scientific/Engineering :: Bio-Informatics'
+        "Development Status :: 1 - Planning",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Operating System :: POSIX :: Linux",
+        "Operating System :: Microsoft :: Windows",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
-)
+)
```

