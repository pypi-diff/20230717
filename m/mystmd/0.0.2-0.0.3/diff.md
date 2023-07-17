# Comparing `tmp/mystmd-0.0.2.tar.gz` & `tmp/mystmd-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mystmd-0.0.2.tar", last modified: Mon Jul 17 19:13:12 2023, max compression
+gzip compressed data, was "mystmd-0.0.3.tar", last modified: Mon Jul 17 20:00:08 2023, max compression
```

## Comparing `mystmd-0.0.2.tar` & `mystmd-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 19:13:12.779007 mystmd-0.0.2/
--rw-r--r--   0 franklin   (501) staff       (20)     1088 2023-07-17 16:52:14.000000 mystmd-0.0.2/LICENSE
--rw-r--r--   0 franklin   (501) staff       (20)       55 2023-07-17 17:15:36.000000 mystmd-0.0.2/MANIFEST.in
--rw-r--r--   0 franklin   (501) staff       (20)      815 2023-07-17 19:13:12.779106 mystmd-0.0.2/PKG-INFO
--rw-r--r--   0 franklin   (501) staff       (20)       78 2023-07-04 19:42:57.000000 mystmd-0.0.2/README.md
-drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 19:13:12.766081 mystmd-0.0.2/dist/
--rwxr-xr-x   0 franklin   (501) staff       (20) 13079621 2023-07-15 00:22:54.000000 mystmd-0.0.2/dist/myst.cjs
-drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 19:13:12.778373 mystmd-0.0.2/mystmd.egg-info/
--rw-r--r--   0 franklin   (501) staff       (20)      815 2023-07-17 19:13:12.000000 mystmd-0.0.2/mystmd.egg-info/PKG-INFO
--rw-r--r--   0 franklin   (501) staff       (20)      255 2023-07-17 19:13:12.000000 mystmd-0.0.2/mystmd.egg-info/SOURCES.txt
--rw-r--r--   0 franklin   (501) staff       (20)        1 2023-07-17 19:13:12.000000 mystmd-0.0.2/mystmd.egg-info/dependency_links.txt
--rw-r--r--   0 franklin   (501) staff       (20)       45 2023-07-17 19:13:12.000000 mystmd-0.0.2/mystmd.egg-info/entry_points.txt
--rw-r--r--   0 franklin   (501) staff       (20)       10 2023-07-17 19:13:12.000000 mystmd-0.0.2/mystmd.egg-info/top_level.txt
-drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 19:13:12.778681 mystmd-0.0.2/mystmd_py/
--rw-r--r--   0 franklin   (501) staff       (20)        0 2023-07-17 16:26:51.000000 mystmd-0.0.2/mystmd_py/__init__.py
--rw-r--r--   0 franklin   (501) staff       (20)      829 2023-07-17 17:28:11.000000 mystmd-0.0.2/mystmd_py/main.py
--rw-r--r--   0 franklin   (501) staff       (20)      901 2023-07-17 19:13:12.779548 mystmd-0.0.2/setup.cfg
--rw-r--r--   0 franklin   (501) staff       (20)       37 2023-07-17 16:56:36.000000 mystmd-0.0.2/setup.py
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 20:00:08.615911 mystmd-0.0.3/
+-rw-r--r--   0 franklin   (501) staff       (20)     1088 2023-07-17 16:52:14.000000 mystmd-0.0.3/LICENSE
+-rw-r--r--   0 franklin   (501) staff       (20)       60 2023-07-17 19:59:06.000000 mystmd-0.0.3/MANIFEST.in
+-rw-r--r--   0 franklin   (501) staff       (20)      815 2023-07-17 20:00:08.616044 mystmd-0.0.3/PKG-INFO
+-rw-r--r--   0 franklin   (501) staff       (20)       78 2023-07-17 20:00:03.000000 mystmd-0.0.3/README.md
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 20:00:08.606014 mystmd-0.0.3/mystmd.egg-info/
+-rw-r--r--   0 franklin   (501) staff       (20)      815 2023-07-17 20:00:08.000000 mystmd-0.0.3/mystmd.egg-info/PKG-INFO
+-rw-r--r--   0 franklin   (501) staff       (20)      260 2023-07-17 20:00:08.000000 mystmd-0.0.3/mystmd.egg-info/SOURCES.txt
+-rw-r--r--   0 franklin   (501) staff       (20)        1 2023-07-17 20:00:08.000000 mystmd-0.0.3/mystmd.egg-info/dependency_links.txt
+-rw-r--r--   0 franklin   (501) staff       (20)       45 2023-07-17 20:00:08.000000 mystmd-0.0.3/mystmd.egg-info/entry_points.txt
+-rw-r--r--   0 franklin   (501) staff       (20)       10 2023-07-17 20:00:08.000000 mystmd-0.0.3/mystmd.egg-info/top_level.txt
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 20:00:08.606382 mystmd-0.0.3/mystmd_py/
+-rw-r--r--   0 franklin   (501) staff       (20)        0 2023-07-17 16:26:51.000000 mystmd-0.0.3/mystmd_py/__init__.py
+-rw-r--r--   0 franklin   (501) staff       (20)      813 2023-07-17 19:53:36.000000 mystmd-0.0.3/mystmd_py/main.py
+-rwxr-xr-x   0 franklin   (501) staff       (20) 13079621 2023-07-17 20:00:03.000000 mystmd-0.0.3/mystmd_py/myst.cjs
+-rw-r--r--   0 franklin   (501) staff       (20)      859 2023-07-17 20:00:08.616613 mystmd-0.0.3/setup.cfg
+-rw-r--r--   0 franklin   (501) staff       (20)       37 2023-07-17 16:56:36.000000 mystmd-0.0.3/setup.py
```

### Comparing `mystmd-0.0.2/LICENSE` & `mystmd-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mystmd-0.0.2/PKG-INFO` & `mystmd-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mystmd
-Version: 0.0.2
+Version: 0.0.3
 Summary: Command line tools for MyST Markdown
 Home-page: https://github.com/executablebooks/mystmd
 Author: Franklin Koch
 License: MIT
 Keywords: markdown,latex,writing-software,scientific-visualization,pdf-generation,science-research
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mystmd-0.0.2/dist/myst.cjs` & `mystmd-0.0.3/mystmd_py/myst.cjs`

 * *Files identical despite different names*

### Comparing `mystmd-0.0.2/mystmd.egg-info/PKG-INFO` & `mystmd-0.0.3/mystmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mystmd
-Version: 0.0.2
+Version: 0.0.3
 Summary: Command line tools for MyST Markdown
 Home-page: https://github.com/executablebooks/mystmd
 Author: Franklin Koch
 License: MIT
 Keywords: markdown,latex,writing-software,scientific-visualization,pdf-generation,science-research
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mystmd-0.0.2/mystmd_py/main.py` & `mystmd-0.0.3/mystmd_py/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 NODE_LOCATION = (
     shutil.which("node") or
     shutil.which("node.exe") or
     shutil.which("node.cmd")
 )
 PATH_TO_BIN_JS = str(
     (
-        pathlib.Path(__file__).parent.parent / 'dist' / 'myst.cjs'
+        pathlib.Path(__file__).parent / 'myst.cjs'
     ).resolve()
 )
 
 
 def main():
     if not NODE_LOCATION:
         sys.exit(
```

### Comparing `mystmd-0.0.2/setup.cfg` & `mystmd-0.0.3/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mystmd
-version = 0.0.2
+version = 0.0.3
 description = Command line tools for MyST Markdown
 author = Franklin Koch
 url = https://github.com/executablebooks/mystmd
 license = MIT
 license_file = LICENSE
 classifiers = 
 	Intended Audience :: Science/Research
@@ -19,17 +19,14 @@
 	Topic :: Scientific/Engineering
 keywords = markdown, latex, writing-software, scientific-visualization, pdf-generation, science-research
 
 [options]
 packages = find:
 python_requires = >=3.6
 
-[options.package_data]
-* = dist/myst.cjs
-
 [options.entry_points]
 console_scripts = 
 	myst = mystmd_py.main:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

