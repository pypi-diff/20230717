# Comparing `tmp/cdk-image-pipeline-0.3.7.tar.gz` & `tmp/cdk-image-pipeline-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-image-pipeline-0.3.7.tar", last modified: Fri Jul  7 15:10:34 2023, max compression
+gzip compressed data, was "cdk-image-pipeline-0.3.8.tar", last modified: Mon Jul 17 16:11:44 2023, max compression
```

## Comparing `cdk-image-pipeline-0.3.7.tar` & `cdk-image-pipeline-0.3.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:10:34.852561 cdk-image-pipeline-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-07 15:10:21.000000 cdk-image-pipeline-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-07 15:10:21.000000 cdk-image-pipeline-0.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-07-07 15:10:34.852561 cdk-image-pipeline-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-07-07 15:10:21.000000 cdk-image-pipeline-0.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-07 15:10:21.000000 cdk-image-pipeline-0.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:10:34.852561 cdk-image-pipeline-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-07 15:10:21.000000 cdk-image-pipeline-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:10:34.848561 cdk-image-pipeline-0.3.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:10:34.852561 cdk-image-pipeline-0.3.7/src/cdk_image_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)    39572 2023-07-07 15:10:21.000000 cdk-image-pipeline-0.3.7/src/cdk_image_pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:10:34.852561 cdk-image-pipeline-0.3.7/src/cdk_image_pipeline/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-07 15:10:21.000000 cdk-image-pipeline-0.3.7/src/cdk_image_pipeline/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31708 2023-07-07 15:10:21.000000 cdk-image-pipeline-0.3.7/src/cdk_image_pipeline/_jsii/cdk-image-pipeline@0.3.7.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:10:21.000000 cdk-image-pipeline-0.3.7/src/cdk_image_pipeline/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:10:34.852561 cdk-image-pipeline-0.3.7/src/cdk_image_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-07-07 15:10:34.000000 cdk-image-pipeline-0.3.7/src/cdk_image_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-07 15:10:34.000000 cdk-image-pipeline-0.3.7/src/cdk_image_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:10:34.000000 cdk-image-pipeline-0.3.7/src/cdk_image_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-07 15:10:34.000000 cdk-image-pipeline-0.3.7/src/cdk_image_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-07 15:10:34.000000 cdk-image-pipeline-0.3.7/src/cdk_image_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:11:44.303015 cdk-image-pipeline-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-17 16:11:32.000000 cdk-image-pipeline-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 16:11:32.000000 cdk-image-pipeline-0.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-07-17 16:11:44.303015 cdk-image-pipeline-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-07-17 16:11:32.000000 cdk-image-pipeline-0.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-17 16:11:32.000000 cdk-image-pipeline-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 16:11:44.303015 cdk-image-pipeline-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-17 16:11:32.000000 cdk-image-pipeline-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:11:44.299015 cdk-image-pipeline-0.3.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:11:44.299015 cdk-image-pipeline-0.3.8/src/cdk_image_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)    39572 2023-07-17 16:11:32.000000 cdk-image-pipeline-0.3.8/src/cdk_image_pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:11:44.299015 cdk-image-pipeline-0.3.8/src/cdk_image_pipeline/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-17 16:11:32.000000 cdk-image-pipeline-0.3.8/src/cdk_image_pipeline/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31711 2023-07-17 16:11:32.000000 cdk-image-pipeline-0.3.8/src/cdk_image_pipeline/_jsii/cdk-image-pipeline@0.3.8.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:11:32.000000 cdk-image-pipeline-0.3.8/src/cdk_image_pipeline/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:11:44.299015 cdk-image-pipeline-0.3.8/src/cdk_image_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-07-17 16:11:44.000000 cdk-image-pipeline-0.3.8/src/cdk_image_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-17 16:11:44.000000 cdk-image-pipeline-0.3.8/src/cdk_image_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:11:44.000000 cdk-image-pipeline-0.3.8/src/cdk_image_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-17 16:11:44.000000 cdk-image-pipeline-0.3.8/src/cdk_image_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-17 16:11:44.000000 cdk-image-pipeline-0.3.8/src/cdk_image_pipeline.egg-info/top_level.txt
```

### Comparing `cdk-image-pipeline-0.3.7/LICENSE` & `cdk-image-pipeline-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-image-pipeline-0.3.7/PKG-INFO` & `cdk-image-pipeline-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-image-pipeline
-Version: 0.3.7
+Version: 0.3.8
 Summary: Quickly deploy a complete EC2 Image Builder Image Pipeline using CDK
 Home-page: https://github.com/aws-samples/cdk-image-pipeline.git
 Author: Cameron Magee<magcamer@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws-samples/cdk-image-pipeline.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-image-pipeline-0.3.7/README.md` & `cdk-image-pipeline-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `cdk-image-pipeline-0.3.7/setup.py` & `cdk-image-pipeline-0.3.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-image-pipeline",
-    "version": "0.3.7",
+    "version": "0.3.8",
     "description": "Quickly deploy a complete EC2 Image Builder Image Pipeline using CDK",
     "license": "Apache-2.0",
     "url": "https://github.com/aws-samples/cdk-image-pipeline.git",
     "long_description_content_type": "text/markdown",
     "author": "Cameron Magee<magcamer@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_image_pipeline",
         "cdk_image_pipeline._jsii"
     ],
     "package_data": {
         "cdk_image_pipeline._jsii": [
-            "cdk-image-pipeline@0.3.7.jsii.tgz"
+            "cdk-image-pipeline@0.3.8.jsii.tgz"
         ],
         "cdk_image_pipeline": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-image-pipeline-0.3.7/src/cdk_image_pipeline/__init__.py` & `cdk-image-pipeline-0.3.8/src/cdk_image_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-image-pipeline-0.3.7/src/cdk_image_pipeline.egg-info/PKG-INFO` & `cdk-image-pipeline-0.3.8/src/cdk_image_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-image-pipeline
-Version: 0.3.7
+Version: 0.3.8
 Summary: Quickly deploy a complete EC2 Image Builder Image Pipeline using CDK
 Home-page: https://github.com/aws-samples/cdk-image-pipeline.git
 Author: Cameron Magee<magcamer@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws-samples/cdk-image-pipeline.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

