# Comparing `tmp/foambryo-0.2.7.tar.gz` & `tmp/foambryo-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/foambryo/dist/.tmp-s1ec2pdq/foambryo-0.2.7.tar", last modified: Mon Jul 17 10:33:50 2023, max compression
+gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/foambryo/dist/.tmp-mlxx2h8t/foambryo-0.2.8.tar", last modified: Mon Jul 17 10:43:32 2023, max compression
```

## Comparing `foambryo-0.2.7.tar` & `foambryo-0.2.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:33:50.811644 foambryo-0.2.7/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    11278 2023-07-17 10:33:50.811828 foambryo-0.2.7/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    10648 2023-07-11 09:38:23.000000 foambryo-0.2.7/README.md
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-06-23 13:21:07.000000 foambryo-0.2.7/pyproject.toml
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      905 2023-07-17 10:33:50.812842 foambryo-0.2.7/setup.cfg
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:33:50.789502 foambryo-0.2.7/src/
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:33:50.805746 foambryo-0.2.7/src/foambryo/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    26634 2023-07-11 12:03:17.000000 foambryo-0.2.7/src/foambryo/Force_viewer.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     4235 2023-06-23 13:21:07.000000 foambryo-0.2.7/src/foambryo/Inference_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     9713 2023-06-23 13:21:07.000000 foambryo-0.2.7/src/foambryo/Mesh_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    10634 2023-06-28 13:11:16.000000 foambryo-0.2.7/src/foambryo/Plotting_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     5836 2023-07-11 12:14:37.000000 foambryo-0.2.7/src/foambryo/Pressure_inference.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    28964 2023-06-23 13:21:07.000000 foambryo-0.2.7/src/foambryo/Tension_inference.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      223 2023-06-23 13:21:07.000000 foambryo-0.2.7/src/foambryo/__init__.py
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:33:50.811132 foambryo-0.2.7/src/foambryo.egg-info/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    11278 2023-07-17 10:33:50.000000 foambryo-0.2.7/src/foambryo.egg-info/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      438 2023-07-17 10:33:50.000000 foambryo-0.2.7/src/foambryo.egg-info/SOURCES.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-07-17 10:33:50.000000 foambryo-0.2.7/src/foambryo.egg-info/dependency_links.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      107 2023-07-17 10:33:50.000000 foambryo-0.2.7/src/foambryo.egg-info/requires.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        9 2023-07-17 10:33:50.000000 foambryo-0.2.7/src/foambryo.egg-info/top_level.txt
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:43:32.461570 foambryo-0.2.8/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    11252 2023-07-17 10:43:32.461697 foambryo-0.2.8/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10648 2023-07-11 09:38:23.000000 foambryo-0.2.8/README.md
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-06-23 13:21:07.000000 foambryo-0.2.8/pyproject.toml
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      891 2023-07-17 10:43:32.462391 foambryo-0.2.8/setup.cfg
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:43:32.450039 foambryo-0.2.8/src/
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:43:32.458400 foambryo-0.2.8/src/foambryo/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    26634 2023-07-11 12:03:17.000000 foambryo-0.2.8/src/foambryo/Force_viewer.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     4235 2023-06-23 13:21:07.000000 foambryo-0.2.8/src/foambryo/Inference_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     9713 2023-06-23 13:21:07.000000 foambryo-0.2.8/src/foambryo/Mesh_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10634 2023-06-28 13:11:16.000000 foambryo-0.2.8/src/foambryo/Plotting_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     5836 2023-07-11 12:14:37.000000 foambryo-0.2.8/src/foambryo/Pressure_inference.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    28964 2023-06-23 13:21:07.000000 foambryo-0.2.8/src/foambryo/Tension_inference.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      223 2023-06-23 13:21:07.000000 foambryo-0.2.8/src/foambryo/__init__.py
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:43:32.461193 foambryo-0.2.8/src/foambryo.egg-info/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    11252 2023-07-17 10:43:32.000000 foambryo-0.2.8/src/foambryo.egg-info/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      438 2023-07-17 10:43:32.000000 foambryo-0.2.8/src/foambryo.egg-info/SOURCES.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-07-17 10:43:32.000000 foambryo-0.2.8/src/foambryo.egg-info/dependency_links.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      107 2023-07-17 10:43:32.000000 foambryo-0.2.8/src/foambryo.egg-info/requires.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        9 2023-07-17 10:43:32.000000 foambryo-0.2.8/src/foambryo.egg-info/top_level.txt
```

### Comparing `foambryo-0.2.7/PKG-INFO` & `foambryo-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: foambryo
-Version: 0.2.7
+Version: 0.2.8
 Summary: Tension inference for 3D cell assemblies
 Home-page: https://github.com/sacha-ichbiah/foambryo
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
+License: CC BY-NC-SA 4.0
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ### foambryo
 
 **foambryo** is a python package based on Polyscope designed to infer surface tensions, pressures and stresses from the geometry of epithelial-cell-clusters, namely early-embryos and structures encoutered in stem cell cultures, as organoids and embryoids.
```

### Comparing `foambryo-0.2.7/README.md` & `foambryo-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.7/setup.cfg` & `foambryo-0.2.8/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [metadata]
 name = foambryo
-version = 0.2.7
+version = 0.2.8
 author = Sacha Ichbiah
 author_email = sacha.ichbiah@college-de-france.fr
 description = Tension inference for 3D cell assemblies
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sacha-ichbiah/foambryo
 project_urls = 
 	Team website = https://www.turlierlab.com/
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS
-	License :: OSI Approved :: MIT License
 	Intended Audience :: Science/Research
+license = CC BY-NC-SA 4.0
 
 [options]
 include_package_data = True
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
```

### Comparing `foambryo-0.2.7/src/foambryo/Force_viewer.py` & `foambryo-0.2.8/src/foambryo/Force_viewer.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.7/src/foambryo/Inference_utilities.py` & `foambryo-0.2.8/src/foambryo/Inference_utilities.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.7/src/foambryo/Mesh_utilities.py` & `foambryo-0.2.8/src/foambryo/Mesh_utilities.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.7/src/foambryo/Plotting_utilities.py` & `foambryo-0.2.8/src/foambryo/Plotting_utilities.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.7/src/foambryo/Pressure_inference.py` & `foambryo-0.2.8/src/foambryo/Pressure_inference.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.7/src/foambryo/Tension_inference.py` & `foambryo-0.2.8/src/foambryo/Tension_inference.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.7/src/foambryo.egg-info/PKG-INFO` & `foambryo-0.2.8/src/foambryo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: foambryo
-Version: 0.2.7
+Version: 0.2.8
 Summary: Tension inference for 3D cell assemblies
 Home-page: https://github.com/sacha-ichbiah/foambryo
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
+License: CC BY-NC-SA 4.0
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ### foambryo
 
 **foambryo** is a python package based on Polyscope designed to infer surface tensions, pressures and stresses from the geometry of epithelial-cell-clusters, namely early-embryos and structures encoutered in stem cell cultures, as organoids and embryoids.
```

