# Comparing `tmp/pyDeepP2SA-0.0.4.tar.gz` & `tmp/pyDeepP2SA-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDeepP2SA-0.0.4.tar", last modified: Mon Jul 17 17:17:25 2023, max compression
+gzip compressed data, was "pyDeepP2SA-0.0.5.tar", last modified: Mon Jul 17 17:25:19 2023, max compression
```

## Comparing `pyDeepP2SA-0.0.4.tar` & `pyDeepP2SA-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 brinthan   (501) staff       (20)        0 2023-07-17 17:17:25.408152 pyDeepP2SA-0.0.4/
--rw-r--r--   0 brinthan   (501) staff       (20)      324 2023-07-17 17:17:08.000000 pyDeepP2SA-0.0.4/CHANGELOG.txt
--rw-r--r--   0 brinthan   (501) staff       (20)     1057 2023-07-17 16:39:06.000000 pyDeepP2SA-0.0.4/LICENCE.txt
--rw-r--r--   0 brinthan   (501) staff       (20)       25 2023-07-17 16:39:06.000000 pyDeepP2SA-0.0.4/MANIFEST.in
--rw-r--r--   0 brinthan   (501) staff       (20)     9391 2023-07-17 17:17:25.408011 pyDeepP2SA-0.0.4/PKG-INFO
--rw-r--r--   0 brinthan   (501) staff       (20)     8413 2023-07-17 16:39:06.000000 pyDeepP2SA-0.0.4/README.md
--rw-r--r--   0 brinthan   (501) staff       (20)       38 2023-07-17 17:17:25.408190 pyDeepP2SA-0.0.4/setup.cfg
--rw-r--r--   0 brinthan   (501) staff       (20)     1042 2023-07-17 17:15:57.000000 pyDeepP2SA-0.0.4/setup.py
-drwxr-xr-x   0 brinthan   (501) staff       (20)        0 2023-07-17 17:17:25.407110 pyDeepP2SA-0.0.4/src/
-drwxr-xr-x   0 brinthan   (501) staff       (20)        0 2023-07-17 17:17:25.407852 pyDeepP2SA-0.0.4/src/pyDeepP2SA.egg-info/
--rw-r--r--   0 brinthan   (501) staff       (20)     9391 2023-07-17 17:17:25.000000 pyDeepP2SA-0.0.4/src/pyDeepP2SA.egg-info/PKG-INFO
--rw-r--r--   0 brinthan   (501) staff       (20)      263 2023-07-17 17:17:25.000000 pyDeepP2SA-0.0.4/src/pyDeepP2SA.egg-info/SOURCES.txt
--rw-r--r--   0 brinthan   (501) staff       (20)        1 2023-07-17 17:17:25.000000 pyDeepP2SA-0.0.4/src/pyDeepP2SA.egg-info/dependency_links.txt
--rw-r--r--   0 brinthan   (501) staff       (20)       77 2023-07-17 17:17:25.000000 pyDeepP2SA-0.0.4/src/pyDeepP2SA.egg-info/requires.txt
--rw-r--r--   0 brinthan   (501) staff       (20)       11 2023-07-17 17:17:25.000000 pyDeepP2SA-0.0.4/src/pyDeepP2SA.egg-info/top_level.txt
--rw-r--r--   0 brinthan   (501) staff       (20)    21295 2023-07-17 17:14:39.000000 pyDeepP2SA-0.0.4/src/pyDeepP2SA.py
+drwxr-xr-x   0 brinthan   (501) staff       (20)        0 2023-07-17 17:25:19.375367 pyDeepP2SA-0.0.5/
+-rw-r--r--   0 brinthan   (501) staff       (20)      324 2023-07-17 17:17:08.000000 pyDeepP2SA-0.0.5/CHANGELOG.txt
+-rw-r--r--   0 brinthan   (501) staff       (20)     1057 2023-07-17 16:39:06.000000 pyDeepP2SA-0.0.5/LICENCE.txt
+-rw-r--r--   0 brinthan   (501) staff       (20)       25 2023-07-17 16:39:06.000000 pyDeepP2SA-0.0.5/MANIFEST.in
+-rw-r--r--   0 brinthan   (501) staff       (20)     9391 2023-07-17 17:25:19.375196 pyDeepP2SA-0.0.5/PKG-INFO
+-rw-r--r--   0 brinthan   (501) staff       (20)     8413 2023-07-17 16:39:06.000000 pyDeepP2SA-0.0.5/README.md
+-rw-r--r--   0 brinthan   (501) staff       (20)       38 2023-07-17 17:25:19.375409 pyDeepP2SA-0.0.5/setup.cfg
+-rw-r--r--   0 brinthan   (501) staff       (20)     1042 2023-07-17 17:24:40.000000 pyDeepP2SA-0.0.5/setup.py
+drwxr-xr-x   0 brinthan   (501) staff       (20)        0 2023-07-17 17:25:19.374114 pyDeepP2SA-0.0.5/src/
+drwxr-xr-x   0 brinthan   (501) staff       (20)        0 2023-07-17 17:25:19.374746 pyDeepP2SA-0.0.5/src/pyDeepP2SA.egg-info/
+-rw-r--r--   0 brinthan   (501) staff       (20)     9391 2023-07-17 17:25:19.000000 pyDeepP2SA-0.0.5/src/pyDeepP2SA.egg-info/PKG-INFO
+-rw-r--r--   0 brinthan   (501) staff       (20)      263 2023-07-17 17:25:19.000000 pyDeepP2SA-0.0.5/src/pyDeepP2SA.egg-info/SOURCES.txt
+-rw-r--r--   0 brinthan   (501) staff       (20)        1 2023-07-17 17:25:19.000000 pyDeepP2SA-0.0.5/src/pyDeepP2SA.egg-info/dependency_links.txt
+-rw-r--r--   0 brinthan   (501) staff       (20)       77 2023-07-17 17:25:19.000000 pyDeepP2SA-0.0.5/src/pyDeepP2SA.egg-info/requires.txt
+-rw-r--r--   0 brinthan   (501) staff       (20)       11 2023-07-17 17:25:19.000000 pyDeepP2SA-0.0.5/src/pyDeepP2SA.egg-info/top_level.txt
+-rw-r--r--   0 brinthan   (501) staff       (20)    21296 2023-07-17 17:24:56.000000 pyDeepP2SA-0.0.5/src/pyDeepP2SA.py
```

### Comparing `pyDeepP2SA-0.0.4/LICENCE.txt` & `pyDeepP2SA-0.0.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pyDeepP2SA-0.0.4/PKG-INFO` & `pyDeepP2SA-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDeepP2SA
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package for particle size and shape analysis using deep learning
 Home-page: https://github.com/BrinthanK/pyDeepP2SA
 Author: Brinthan K
 Author-email: kanesalingambrinthan187@gmail.com
 License: MIT
 Keywords: Particle shape analyser,PSD,Deep learning,Image processing,Circularity
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyDeepP2SA-0.0.4/README.md` & `pyDeepP2SA-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyDeepP2SA-0.0.4/setup.py` & `pyDeepP2SA-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     'matplotlib',
     'pandas',
     'seaborn'
 ]
 
 setup(
     name='pyDeepP2SA',
-    version='0.0.4',
+    version='0.0.5',
     description='A python package for particle size and shape analysis using deep learning',
     py_modules=["pyDeepP2SA"],
     package_dir={'': 'src'},
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='https://github.com/BrinthanK/pyDeepP2SA',
     author='Brinthan K',
     author_email='kanesalingambrinthan187@gmail.com',
```

### Comparing `pyDeepP2SA-0.0.4/src/pyDeepP2SA.egg-info/PKG-INFO` & `pyDeepP2SA-0.0.5/src/pyDeepP2SA.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDeepP2SA
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package for particle size and shape analysis using deep learning
 Home-page: https://github.com/BrinthanK/pyDeepP2SA
 Author: Brinthan K
 Author-email: kanesalingambrinthan187@gmail.com
 License: MIT
 Keywords: Particle shape analyser,PSD,Deep learning,Image processing,Circularity
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyDeepP2SA-0.0.4/src/pyDeepP2SA.py` & `pyDeepP2SA-0.0.5/src/pyDeepP2SA.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,15 +431,15 @@
                     writer.writerow({
                         'Mask': i + 1, 'Area': area, 'Circularity': circularity, 'BBox': bbox,
                         'Predicted IOU': predicted_iou, 'Point Coords': point_coords,
                         'Stability Score': stability_score, 'Perimeter': perimeter,
                         'Diameter': diameter, 'Type': segment_type
                     })
 
-def plot_segment_bounding_boxes(csv_file, segment_types,image):
+def plot_segment_bounding_boxes(csv_file, segment_types, image):
     # Read the CSV file and extract the relevant data
     mask_details = []
     with open(csv_file, 'r') as file:
         reader = csv.DictReader(file)
         for row in reader:
             mask_details.append(row)
```

