# Comparing `tmp/mystmd-0.0.3.tar.gz` & `tmp/mystmd-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mystmd-0.0.3.tar", last modified: Mon Jul 17 20:00:08 2023, max compression
+gzip compressed data, was "mystmd-0.0.4.tar", last modified: Mon Jul 17 20:23:00 2023, max compression
```

## Comparing `mystmd-0.0.3.tar` & `mystmd-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 20:00:08.615911 mystmd-0.0.3/
--rw-r--r--   0 franklin   (501) staff       (20)     1088 2023-07-17 16:52:14.000000 mystmd-0.0.3/LICENSE
--rw-r--r--   0 franklin   (501) staff       (20)       60 2023-07-17 19:59:06.000000 mystmd-0.0.3/MANIFEST.in
--rw-r--r--   0 franklin   (501) staff       (20)      815 2023-07-17 20:00:08.616044 mystmd-0.0.3/PKG-INFO
--rw-r--r--   0 franklin   (501) staff       (20)       78 2023-07-17 20:00:03.000000 mystmd-0.0.3/README.md
-drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 20:00:08.606014 mystmd-0.0.3/mystmd.egg-info/
--rw-r--r--   0 franklin   (501) staff       (20)      815 2023-07-17 20:00:08.000000 mystmd-0.0.3/mystmd.egg-info/PKG-INFO
--rw-r--r--   0 franklin   (501) staff       (20)      260 2023-07-17 20:00:08.000000 mystmd-0.0.3/mystmd.egg-info/SOURCES.txt
--rw-r--r--   0 franklin   (501) staff       (20)        1 2023-07-17 20:00:08.000000 mystmd-0.0.3/mystmd.egg-info/dependency_links.txt
--rw-r--r--   0 franklin   (501) staff       (20)       45 2023-07-17 20:00:08.000000 mystmd-0.0.3/mystmd.egg-info/entry_points.txt
--rw-r--r--   0 franklin   (501) staff       (20)       10 2023-07-17 20:00:08.000000 mystmd-0.0.3/mystmd.egg-info/top_level.txt
-drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 20:00:08.606382 mystmd-0.0.3/mystmd_py/
--rw-r--r--   0 franklin   (501) staff       (20)        0 2023-07-17 16:26:51.000000 mystmd-0.0.3/mystmd_py/__init__.py
--rw-r--r--   0 franklin   (501) staff       (20)      813 2023-07-17 19:53:36.000000 mystmd-0.0.3/mystmd_py/main.py
--rwxr-xr-x   0 franklin   (501) staff       (20) 13079621 2023-07-17 20:00:03.000000 mystmd-0.0.3/mystmd_py/myst.cjs
--rw-r--r--   0 franklin   (501) staff       (20)      859 2023-07-17 20:00:08.616613 mystmd-0.0.3/setup.cfg
--rw-r--r--   0 franklin   (501) staff       (20)       37 2023-07-17 16:56:36.000000 mystmd-0.0.3/setup.py
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 20:23:00.766412 mystmd-0.0.4/
+-rw-r--r--   0 franklin   (501) staff       (20)     1088 2023-07-17 16:52:14.000000 mystmd-0.0.4/LICENSE
+-rw-r--r--   0 franklin   (501) staff       (20)       60 2023-07-17 19:59:06.000000 mystmd-0.0.4/MANIFEST.in
+-rw-r--r--   0 franklin   (501) staff       (20)      815 2023-07-17 20:23:00.766532 mystmd-0.0.4/PKG-INFO
+-rw-r--r--   0 franklin   (501) staff       (20)       78 2023-07-17 20:22:56.000000 mystmd-0.0.4/README.md
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 20:23:00.757045 mystmd-0.0.4/mystmd.egg-info/
+-rw-r--r--   0 franklin   (501) staff       (20)      815 2023-07-17 20:23:00.000000 mystmd-0.0.4/mystmd.egg-info/PKG-INFO
+-rw-r--r--   0 franklin   (501) staff       (20)      260 2023-07-17 20:23:00.000000 mystmd-0.0.4/mystmd.egg-info/SOURCES.txt
+-rw-r--r--   0 franklin   (501) staff       (20)        1 2023-07-17 20:23:00.000000 mystmd-0.0.4/mystmd.egg-info/dependency_links.txt
+-rw-r--r--   0 franklin   (501) staff       (20)       45 2023-07-17 20:23:00.000000 mystmd-0.0.4/mystmd.egg-info/entry_points.txt
+-rw-r--r--   0 franklin   (501) staff       (20)       10 2023-07-17 20:23:00.000000 mystmd-0.0.4/mystmd.egg-info/top_level.txt
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 20:23:00.757536 mystmd-0.0.4/mystmd_py/
+-rw-r--r--   0 franklin   (501) staff       (20)        0 2023-07-17 16:26:51.000000 mystmd-0.0.4/mystmd_py/__init__.py
+-rw-r--r--   0 franklin   (501) staff       (20)      813 2023-07-17 19:53:36.000000 mystmd-0.0.4/mystmd_py/main.py
+-rwxr-xr-x   0 franklin   (501) staff       (20) 13079621 2023-07-17 20:22:56.000000 mystmd-0.0.4/mystmd_py/myst.cjs
+-rw-r--r--   0 franklin   (501) staff       (20)      914 2023-07-17 20:23:00.766976 mystmd-0.0.4/setup.cfg
+-rw-r--r--   0 franklin   (501) staff       (20)       37 2023-07-17 16:56:36.000000 mystmd-0.0.4/setup.py
```

### Comparing `mystmd-0.0.3/LICENSE` & `mystmd-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mystmd-0.0.3/PKG-INFO` & `mystmd-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mystmd
-Version: 0.0.3
+Version: 0.0.4
 Summary: Command line tools for MyST Markdown
 Home-page: https://github.com/executablebooks/mystmd
 Author: Franklin Koch
 License: MIT
 Keywords: markdown,latex,writing-software,scientific-visualization,pdf-generation,science-research
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mystmd-0.0.3/mystmd.egg-info/PKG-INFO` & `mystmd-0.0.4/mystmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mystmd
-Version: 0.0.3
+Version: 0.0.4
 Summary: Command line tools for MyST Markdown
 Home-page: https://github.com/executablebooks/mystmd
 Author: Franklin Koch
 License: MIT
 Keywords: markdown,latex,writing-software,scientific-visualization,pdf-generation,science-research
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mystmd-0.0.3/mystmd_py/main.py` & `mystmd-0.0.4/mystmd_py/main.py`

 * *Files identical despite different names*

### Comparing `mystmd-0.0.3/mystmd_py/myst.cjs` & `mystmd-0.0.4/mystmd_py/myst.cjs`

 * *Files identical despite different names*

