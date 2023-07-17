# Comparing `tmp/foambryo-0.2.8.tar.gz` & `tmp/foambryo-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/foambryo/dist/.tmp-mlxx2h8t/foambryo-0.2.8.tar", last modified: Mon Jul 17 10:43:32 2023, max compression
+gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/foambryo/dist/.tmp-tly5_f6v/foambryo-0.2.9.tar", last modified: Mon Jul 17 10:47:15 2023, max compression
```

## Comparing `foambryo-0.2.8.tar` & `foambryo-0.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:43:32.461570 foambryo-0.2.8/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    11252 2023-07-17 10:43:32.461697 foambryo-0.2.8/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    10648 2023-07-11 09:38:23.000000 foambryo-0.2.8/README.md
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-06-23 13:21:07.000000 foambryo-0.2.8/pyproject.toml
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      891 2023-07-17 10:43:32.462391 foambryo-0.2.8/setup.cfg
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:43:32.450039 foambryo-0.2.8/src/
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:43:32.458400 foambryo-0.2.8/src/foambryo/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    26634 2023-07-11 12:03:17.000000 foambryo-0.2.8/src/foambryo/Force_viewer.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     4235 2023-06-23 13:21:07.000000 foambryo-0.2.8/src/foambryo/Inference_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     9713 2023-06-23 13:21:07.000000 foambryo-0.2.8/src/foambryo/Mesh_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    10634 2023-06-28 13:11:16.000000 foambryo-0.2.8/src/foambryo/Plotting_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     5836 2023-07-11 12:14:37.000000 foambryo-0.2.8/src/foambryo/Pressure_inference.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    28964 2023-06-23 13:21:07.000000 foambryo-0.2.8/src/foambryo/Tension_inference.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      223 2023-06-23 13:21:07.000000 foambryo-0.2.8/src/foambryo/__init__.py
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:43:32.461193 foambryo-0.2.8/src/foambryo.egg-info/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    11252 2023-07-17 10:43:32.000000 foambryo-0.2.8/src/foambryo.egg-info/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      438 2023-07-17 10:43:32.000000 foambryo-0.2.8/src/foambryo.egg-info/SOURCES.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-07-17 10:43:32.000000 foambryo-0.2.8/src/foambryo.egg-info/dependency_links.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      107 2023-07-17 10:43:32.000000 foambryo-0.2.8/src/foambryo.egg-info/requires.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        9 2023-07-17 10:43:32.000000 foambryo-0.2.8/src/foambryo.egg-info/top_level.txt
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:47:15.291154 foambryo-0.2.9/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    11201 2023-07-17 10:47:15.291274 foambryo-0.2.9/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10648 2023-07-11 09:38:23.000000 foambryo-0.2.9/README.md
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-06-23 13:21:07.000000 foambryo-0.2.9/pyproject.toml
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      851 2023-07-17 10:47:15.292110 foambryo-0.2.9/setup.cfg
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:47:15.280659 foambryo-0.2.9/src/
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:47:15.288269 foambryo-0.2.9/src/foambryo/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    26634 2023-07-11 12:03:17.000000 foambryo-0.2.9/src/foambryo/Force_viewer.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     4235 2023-06-23 13:21:07.000000 foambryo-0.2.9/src/foambryo/Inference_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     9713 2023-06-23 13:21:07.000000 foambryo-0.2.9/src/foambryo/Mesh_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10634 2023-06-28 13:11:16.000000 foambryo-0.2.9/src/foambryo/Plotting_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     5836 2023-07-11 12:14:37.000000 foambryo-0.2.9/src/foambryo/Pressure_inference.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    28964 2023-06-23 13:21:07.000000 foambryo-0.2.9/src/foambryo/Tension_inference.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      223 2023-06-23 13:21:07.000000 foambryo-0.2.9/src/foambryo/__init__.py
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:47:15.290804 foambryo-0.2.9/src/foambryo.egg-info/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    11201 2023-07-17 10:47:15.000000 foambryo-0.2.9/src/foambryo.egg-info/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      438 2023-07-17 10:47:15.000000 foambryo-0.2.9/src/foambryo.egg-info/SOURCES.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-07-17 10:47:15.000000 foambryo-0.2.9/src/foambryo.egg-info/dependency_links.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      107 2023-07-17 10:47:15.000000 foambryo-0.2.9/src/foambryo.egg-info/requires.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        9 2023-07-17 10:47:15.000000 foambryo-0.2.9/src/foambryo.egg-info/top_level.txt
```

### Comparing `foambryo-0.2.8/PKG-INFO` & `foambryo-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: foambryo
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tension inference for 3D cell assemblies
 Home-page: https://github.com/sacha-ichbiah/foambryo
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 License: CC BY-NC-SA 4.0
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ### foambryo
```

### Comparing `foambryo-0.2.8/README.md` & `foambryo-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.8/setup.cfg` & `foambryo-0.2.9/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [metadata]
 name = foambryo
-version = 0.2.8
+version = 0.2.9
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
-	License :: OSI Approved :: MIT License
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS
 	Intended Audience :: Science/Research
 license = CC BY-NC-SA 4.0
 
 [options]
 include_package_data = True
```

### Comparing `foambryo-0.2.8/src/foambryo/Force_viewer.py` & `foambryo-0.2.9/src/foambryo/Force_viewer.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.8/src/foambryo/Inference_utilities.py` & `foambryo-0.2.9/src/foambryo/Inference_utilities.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.8/src/foambryo/Mesh_utilities.py` & `foambryo-0.2.9/src/foambryo/Mesh_utilities.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.8/src/foambryo/Plotting_utilities.py` & `foambryo-0.2.9/src/foambryo/Plotting_utilities.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.8/src/foambryo/Pressure_inference.py` & `foambryo-0.2.9/src/foambryo/Pressure_inference.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.8/src/foambryo/Tension_inference.py` & `foambryo-0.2.9/src/foambryo/Tension_inference.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.8/src/foambryo.egg-info/PKG-INFO` & `foambryo-0.2.9/src/foambryo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: foambryo
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tension inference for 3D cell assemblies
 Home-page: https://github.com/sacha-ichbiah/foambryo
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 License: CC BY-NC-SA 4.0
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ### foambryo
```

