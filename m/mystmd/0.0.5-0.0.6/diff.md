# Comparing `tmp/mystmd-0.0.5.tar.gz` & `tmp/mystmd-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mystmd-0.0.5.tar", last modified: Mon Jul 17 20:25:54 2023, max compression
+gzip compressed data, was "mystmd-0.0.6.tar", last modified: Mon Jul 17 20:27:41 2023, max compression
```

## Comparing `mystmd-0.0.5.tar` & `mystmd-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 20:25:54.459558 mystmd-0.0.5/
--rw-r--r--   0 franklin   (501) staff       (20)     1088 2023-07-17 16:52:14.000000 mystmd-0.0.5/LICENSE
--rw-r--r--   0 franklin   (501) staff       (20)       60 2023-07-17 19:59:06.000000 mystmd-0.0.5/MANIFEST.in
--rw-r--r--   0 franklin   (501) staff       (20)      815 2023-07-17 20:25:54.459695 mystmd-0.0.5/PKG-INFO
--rw-r--r--   0 franklin   (501) staff       (20)       78 2023-07-17 20:25:49.000000 mystmd-0.0.5/README.md
-drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 20:25:54.449440 mystmd-0.0.5/mystmd.egg-info/
--rw-r--r--   0 franklin   (501) staff       (20)      815 2023-07-17 20:25:54.000000 mystmd-0.0.5/mystmd.egg-info/PKG-INFO
--rw-r--r--   0 franklin   (501) staff       (20)      260 2023-07-17 20:25:54.000000 mystmd-0.0.5/mystmd.egg-info/SOURCES.txt
--rw-r--r--   0 franklin   (501) staff       (20)        1 2023-07-17 20:25:54.000000 mystmd-0.0.5/mystmd.egg-info/dependency_links.txt
--rw-r--r--   0 franklin   (501) staff       (20)       45 2023-07-17 20:25:54.000000 mystmd-0.0.5/mystmd.egg-info/entry_points.txt
--rw-r--r--   0 franklin   (501) staff       (20)       10 2023-07-17 20:25:54.000000 mystmd-0.0.5/mystmd.egg-info/top_level.txt
-drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 20:25:54.450109 mystmd-0.0.5/mystmd_py/
--rw-r--r--   0 franklin   (501) staff       (20)        0 2023-07-17 16:26:51.000000 mystmd-0.0.5/mystmd_py/__init__.py
--rw-r--r--   0 franklin   (501) staff       (20)      813 2023-07-17 19:53:36.000000 mystmd-0.0.5/mystmd_py/main.py
--rwxr-xr-x   0 franklin   (501) staff       (20) 13079621 2023-07-17 20:25:49.000000 mystmd-0.0.5/mystmd_py/myst.cjs
--rw-r--r--   0 franklin   (501) staff       (20)      887 2023-07-17 20:25:54.460260 mystmd-0.0.5/setup.cfg
--rw-r--r--   0 franklin   (501) staff       (20)       37 2023-07-17 16:56:36.000000 mystmd-0.0.5/setup.py
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 20:27:41.529462 mystmd-0.0.6/
+-rw-r--r--   0 franklin   (501) staff       (20)     1088 2023-07-17 16:52:14.000000 mystmd-0.0.6/LICENSE
+-rw-r--r--   0 franklin   (501) staff       (20)       60 2023-07-17 19:59:06.000000 mystmd-0.0.6/MANIFEST.in
+-rw-r--r--   0 franklin   (501) staff       (20)      815 2023-07-17 20:27:41.529590 mystmd-0.0.6/PKG-INFO
+-rw-r--r--   0 franklin   (501) staff       (20)       78 2023-07-17 20:27:36.000000 mystmd-0.0.6/README.md
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 20:27:41.518537 mystmd-0.0.6/mystmd.egg-info/
+-rw-r--r--   0 franklin   (501) staff       (20)      815 2023-07-17 20:27:41.000000 mystmd-0.0.6/mystmd.egg-info/PKG-INFO
+-rw-r--r--   0 franklin   (501) staff       (20)      260 2023-07-17 20:27:41.000000 mystmd-0.0.6/mystmd.egg-info/SOURCES.txt
+-rw-r--r--   0 franklin   (501) staff       (20)        1 2023-07-17 20:27:41.000000 mystmd-0.0.6/mystmd.egg-info/dependency_links.txt
+-rw-r--r--   0 franklin   (501) staff       (20)       45 2023-07-17 20:27:41.000000 mystmd-0.0.6/mystmd.egg-info/entry_points.txt
+-rw-r--r--   0 franklin   (501) staff       (20)       10 2023-07-17 20:27:41.000000 mystmd-0.0.6/mystmd.egg-info/top_level.txt
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 20:27:41.519164 mystmd-0.0.6/mystmd_py/
+-rw-r--r--   0 franklin   (501) staff       (20)        0 2023-07-17 16:26:51.000000 mystmd-0.0.6/mystmd_py/__init__.py
+-rw-r--r--   0 franklin   (501) staff       (20)      802 2023-07-17 20:27:07.000000 mystmd-0.0.6/mystmd_py/main.py
+-rwxr-xr-x   0 franklin   (501) staff       (20) 13079621 2023-07-17 20:27:36.000000 mystmd-0.0.6/mystmd_py/myst.cjs
+-rw-r--r--   0 franklin   (501) staff       (20)      887 2023-07-17 20:27:41.530079 mystmd-0.0.6/setup.cfg
+-rw-r--r--   0 franklin   (501) staff       (20)       37 2023-07-17 16:56:36.000000 mystmd-0.0.6/setup.py
```

### Comparing `mystmd-0.0.5/LICENSE` & `mystmd-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mystmd-0.0.5/PKG-INFO` & `mystmd-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mystmd
-Version: 0.0.5
+Version: 0.0.6
 Summary: Command line tools for MyST Markdown
 Home-page: https://github.com/executablebooks/mystmd
 Author: Franklin Koch
 License: MIT
 Keywords: markdown,latex,writing-software,scientific-visualization,pdf-generation,science-research
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mystmd-0.0.5/mystmd.egg-info/PKG-INFO` & `mystmd-0.0.6/mystmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mystmd
-Version: 0.0.5
+Version: 0.0.6
 Summary: Command line tools for MyST Markdown
 Home-page: https://github.com/executablebooks/mystmd
 Author: Franklin Koch
 License: MIT
 Keywords: markdown,latex,writing-software,scientific-visualization,pdf-generation,science-research
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mystmd-0.0.5/mystmd_py/main.py` & `mystmd-0.0.6/mystmd_py/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         sys.exit(
             'You must install node to run myst\n\n'
             'We recommend installing the latest LTS release, using your preferred package manager\n'
             'or following instructions here: https://nodejs.org/en/download'
         )
     node = str(pathlib.Path(NODE_LOCATION).resolve())
     p = subprocess.Popen(
-        [node, PATH_TO_BIN_JS, '--stdio', *sys.argv[1:]],
+        [node, PATH_TO_BIN_JS, *sys.argv[1:]],
         stdin=sys.stdin, stdout=sys.stdout
     )
     sys.exit(p.wait())
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `mystmd-0.0.5/mystmd_py/myst.cjs` & `mystmd-0.0.6/mystmd_py/myst.cjs`

 * *Files identical despite different names*

### Comparing `mystmd-0.0.5/setup.cfg` & `mystmd-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mystmd
-version = 0.0.5
+version = 0.0.6
 description = Command line tools for MyST Markdown
 author = Franklin Koch
 url = https://github.com/executablebooks/mystmd
 license = MIT
 license_file = LICENSE
 classifiers = 
 	Intended Audience :: Science/Research
```

