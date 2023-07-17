# Comparing `tmp/airvacuumvald-23.7.17.0.tar.gz` & `tmp/airvacuumvald-23.7.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airvacuumvald-23.7.17.0.tar", last modified: Mon Jul 17 18:05:18 2023, max compression
+gzip compressed data, was "airvacuumvald-23.7.17.1.tar", last modified: Mon Jul 17 18:27:52 2023, max compression
```

## Comparing `airvacuumvald-23.7.17.0.tar` & `airvacuumvald-23.7.17.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-17 18:05:18.185416 airvacuumvald-23.7.17.0/
--rw-rw-r--   0 j         (1000) j         (1000)      444 2023-07-17 18:05:18.185416 airvacuumvald-23.7.17.0/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)     3274 2023-07-17 17:31:50.000000 airvacuumvald-23.7.17.0/README.rst
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-17 18:05:18.185416 airvacuumvald-23.7.17.0/airvacuumvald/
--rw-rw-r--   0 j         (1000) j         (1000)       25 2023-07-17 17:31:50.000000 airvacuumvald-23.7.17.0/airvacuumvald/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)     2188 2023-07-17 17:31:50.000000 airvacuumvald-23.7.17.0/airvacuumvald/airvacuum.py
--rw-rw-r--   0 j         (1000) j         (1000)      577 2023-07-17 17:35:23.000000 airvacuumvald-23.7.17.0/airvacuumvald/tools.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-17 18:05:18.185416 airvacuumvald-23.7.17.0/airvacuumvald.egg-info/
--rw-rw-r--   0 j         (1000) j         (1000)      444 2023-07-17 18:05:18.000000 airvacuumvald-23.7.17.0/airvacuumvald.egg-info/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)      243 2023-07-17 18:05:18.000000 airvacuumvald-23.7.17.0/airvacuumvald.egg-info/SOURCES.txt
--rw-rw-r--   0 j         (1000) j         (1000)        1 2023-07-17 18:05:18.000000 airvacuumvald-23.7.17.0/airvacuumvald.egg-info/dependency_links.txt
--rw-rw-r--   0 j         (1000) j         (1000)       14 2023-07-17 18:05:18.000000 airvacuumvald-23.7.17.0/airvacuumvald.egg-info/top_level.txt
--rw-rw-r--   0 j         (1000) j         (1000)       38 2023-07-17 18:05:18.185416 airvacuumvald-23.7.17.0/setup.cfg
--rw-rw-r--   0 j         (1000) j         (1000)      713 2023-07-17 17:35:23.000000 airvacuumvald-23.7.17.0/setup.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-17 18:27:52.710010 airvacuumvald-23.7.17.1/
+-rw-rw-r--   0 j         (1000) j         (1000)      444 2023-07-17 18:27:52.710010 airvacuumvald-23.7.17.1/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)     3274 2023-07-17 17:31:50.000000 airvacuumvald-23.7.17.1/README.rst
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-17 18:27:52.710010 airvacuumvald-23.7.17.1/airvacuumvald/
+-rw-rw-r--   0 j         (1000) j         (1000)       46 2023-07-17 18:27:31.000000 airvacuumvald-23.7.17.1/airvacuumvald/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2188 2023-07-17 17:31:50.000000 airvacuumvald-23.7.17.1/airvacuumvald/airvacuum.py
+-rw-rw-r--   0 j         (1000) j         (1000)      577 2023-07-17 17:35:23.000000 airvacuumvald-23.7.17.1/airvacuumvald/tools.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-17 18:27:52.710010 airvacuumvald-23.7.17.1/airvacuumvald.egg-info/
+-rw-rw-r--   0 j         (1000) j         (1000)      444 2023-07-17 18:27:52.000000 airvacuumvald-23.7.17.1/airvacuumvald.egg-info/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)      243 2023-07-17 18:27:52.000000 airvacuumvald-23.7.17.1/airvacuumvald.egg-info/SOURCES.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        1 2023-07-17 18:27:52.000000 airvacuumvald-23.7.17.1/airvacuumvald.egg-info/dependency_links.txt
+-rw-rw-r--   0 j         (1000) j         (1000)       14 2023-07-17 18:27:52.000000 airvacuumvald-23.7.17.1/airvacuumvald.egg-info/top_level.txt
+-rw-rw-r--   0 j         (1000) j         (1000)       38 2023-07-17 18:27:52.710010 airvacuumvald-23.7.17.1/setup.cfg
+-rw-rw-r--   0 j         (1000) j         (1000)      712 2023-07-17 18:27:43.000000 airvacuumvald-23.7.17.1/setup.py
```

### Comparing `airvacuumvald-23.7.17.0/README.rst` & `airvacuumvald-23.7.17.1/README.rst`

 * *Files identical despite different names*

### Comparing `airvacuumvald-23.7.17.0/airvacuumvald/airvacuum.py` & `airvacuumvald-23.7.17.1/airvacuumvald/airvacuum.py`

 * *Files identical despite different names*

### Comparing `airvacuumvald-23.7.17.0/airvacuumvald/tools.py` & `airvacuumvald-23.7.17.1/airvacuumvald/tools.py`

 * *Files identical despite different names*

### Comparing `airvacuumvald-23.7.17.0/setup.py` & `airvacuumvald-23.7.17.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 from glob import glob
 
 setup(
     name="airvacuumvald",
     packages=["airvacuumvald"],
     include_package_data=True,
-    version='23.07.17.0',
+    version='23.7.17.1',
     license='GNU GPLv3',
     platforms='any',
     description='Python implementation of the air-to-vacuum and vacuum-to-air wavelength '
                 'conversion used by VALD (Vienna Atomic Line Database)',
     author='Julio Trevisan',
     author_email='juliotrevisan@gmail.com',
     url='https://github.com/trevisanj/airvacuumvald',
```

