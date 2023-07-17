# Comparing `tmp/airvacuumvald-0.17.12.11.0.tar.gz` & `tmp/airvacuumvald-23.7.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airvacuumvald-0.17.12.11.0.tar", last modified: Mon Dec 11 14:29:25 2017, max compression
+gzip compressed data, was "airvacuumvald-23.7.17.0.tar", last modified: Mon Jul 17 18:05:18 2023, max compression
```

## Comparing `airvacuumvald-0.17.12.11.0.tar` & `airvacuumvald-23.7.17.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2017-12-11 14:29:25.000000 airvacuumvald-0.17.12.11.0/
--rw-r--r--   0 j         (1000) j         (1000)      447 2017-12-11 14:29:25.000000 airvacuumvald-0.17.12.11.0/PKG-INFO
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2017-12-11 14:29:25.000000 airvacuumvald-0.17.12.11.0/airvacuumvald.egg-info/
--rw-r--r--   0 j         (1000) j         (1000)       14 2017-12-11 14:29:24.000000 airvacuumvald-0.17.12.11.0/airvacuumvald.egg-info/top_level.txt
--rw-r--r--   0 j         (1000) j         (1000)      447 2017-12-11 14:29:24.000000 airvacuumvald-0.17.12.11.0/airvacuumvald.egg-info/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)      220 2017-12-11 14:29:24.000000 airvacuumvald-0.17.12.11.0/airvacuumvald.egg-info/SOURCES.txt
--rw-r--r--   0 j         (1000) j         (1000)        1 2017-12-11 14:29:24.000000 airvacuumvald-0.17.12.11.0/airvacuumvald.egg-info/dependency_links.txt
--rw-r--r--   0 j         (1000) j         (1000)      715 2017-12-11 14:29:00.000000 airvacuumvald-0.17.12.11.0/setup.py
--rw-r--r--   0 j         (1000) j         (1000)     3274 2017-12-11 14:19:31.000000 airvacuumvald-0.17.12.11.0/README.rst
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2017-12-11 14:29:25.000000 airvacuumvald-0.17.12.11.0/airvacuumvald/
--rw-r--r--   0 j         (1000) j         (1000)     2188 2017-12-11 13:56:50.000000 airvacuumvald-0.17.12.11.0/airvacuumvald/airvacuum.py
--rw-r--r--   0 j         (1000) j         (1000)       25 2017-12-11 13:54:26.000000 airvacuumvald-0.17.12.11.0/airvacuumvald/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)       59 2017-12-11 14:29:25.000000 airvacuumvald-0.17.12.11.0/setup.cfg
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-17 18:05:18.185416 airvacuumvald-23.7.17.0/
+-rw-rw-r--   0 j         (1000) j         (1000)      444 2023-07-17 18:05:18.185416 airvacuumvald-23.7.17.0/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)     3274 2023-07-17 17:31:50.000000 airvacuumvald-23.7.17.0/README.rst
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-17 18:05:18.185416 airvacuumvald-23.7.17.0/airvacuumvald/
+-rw-rw-r--   0 j         (1000) j         (1000)       25 2023-07-17 17:31:50.000000 airvacuumvald-23.7.17.0/airvacuumvald/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2188 2023-07-17 17:31:50.000000 airvacuumvald-23.7.17.0/airvacuumvald/airvacuum.py
+-rw-rw-r--   0 j         (1000) j         (1000)      577 2023-07-17 17:35:23.000000 airvacuumvald-23.7.17.0/airvacuumvald/tools.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-17 18:05:18.185416 airvacuumvald-23.7.17.0/airvacuumvald.egg-info/
+-rw-rw-r--   0 j         (1000) j         (1000)      444 2023-07-17 18:05:18.000000 airvacuumvald-23.7.17.0/airvacuumvald.egg-info/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)      243 2023-07-17 18:05:18.000000 airvacuumvald-23.7.17.0/airvacuumvald.egg-info/SOURCES.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        1 2023-07-17 18:05:18.000000 airvacuumvald-23.7.17.0/airvacuumvald.egg-info/dependency_links.txt
+-rw-rw-r--   0 j         (1000) j         (1000)       14 2023-07-17 18:05:18.000000 airvacuumvald-23.7.17.0/airvacuumvald.egg-info/top_level.txt
+-rw-rw-r--   0 j         (1000) j         (1000)       38 2023-07-17 18:05:18.185416 airvacuumvald-23.7.17.0/setup.cfg
+-rw-rw-r--   0 j         (1000) j         (1000)      713 2023-07-17 17:35:23.000000 airvacuumvald-23.7.17.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `airvacuumvald-0.17.12.11.0/setup.py` & `airvacuumvald-23.7.17.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 from glob import glob
 
 setup(
     name="airvacuumvald",
     packages=["airvacuumvald"],
     include_package_data=True,
-    version='0.17.12.11.0',
+    version='23.07.17.0',
     license='GNU GPLv3',
     platforms='any',
     description='Python implementation of the air-to-vacuum and vacuum-to-air wavelength '
                 'conversion used by VALD (Vienna Atomic Line Database)',
     author='Julio Trevisan',
     author_email='juliotrevisan@gmail.com',
     url='https://github.com/trevisanj/airvacuumvald',
```

### Comparing `airvacuumvald-0.17.12.11.0/README.rst` & `airvacuumvald-23.7.17.0/README.rst`

 * *Files identical despite different names*

### Comparing `airvacuumvald-0.17.12.11.0/airvacuumvald/airvacuum.py` & `airvacuumvald-23.7.17.0/airvacuumvald/airvacuum.py`

 * *Files identical despite different names*

