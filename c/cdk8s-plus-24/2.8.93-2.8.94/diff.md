# Comparing `tmp/cdk8s-plus-24-2.8.93.tar.gz` & `tmp/cdk8s-plus-24-2.8.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-plus-24-2.8.93.tar", last modified: Sun Jul 16 02:45:44 2023, max compression
+gzip compressed data, was "cdk8s-plus-24-2.8.94.tar", last modified: Mon Jul 17 00:27:39 2023, max compression
```

## Comparing `cdk8s-plus-24-2.8.93.tar` & `cdk8s-plus-24-2.8.94.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:45:44.467352 cdk8s-plus-24-2.8.93/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-16 02:45:32.000000 cdk8s-plus-24-2.8.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-16 02:45:32.000000 cdk8s-plus-24-2.8.93/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-16 02:45:32.000000 cdk8s-plus-24-2.8.93/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-16 02:45:44.467352 cdk8s-plus-24-2.8.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-16 02:45:32.000000 cdk8s-plus-24-2.8.93/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-16 02:45:32.000000 cdk8s-plus-24-2.8.93/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 02:45:44.467352 cdk8s-plus-24-2.8.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-16 02:45:32.000000 cdk8s-plus-24-2.8.93/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:45:44.459352 cdk8s-plus-24-2.8.93/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:45:44.459352 cdk8s-plus-24-2.8.93/src/cdk8s_plus_24/
--rw-r--r--   0 runner    (1001) docker     (123)  1161790 2023-07-16 02:45:32.000000 cdk8s-plus-24-2.8.93/src/cdk8s_plus_24/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:45:44.459352 cdk8s-plus-24-2.8.93/src/cdk8s_plus_24/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-16 02:45:32.000000 cdk8s-plus-24-2.8.93/src/cdk8s_plus_24/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1279958 2023-07-16 02:45:32.000000 cdk8s-plus-24-2.8.93/src/cdk8s_plus_24/_jsii/cdk8s-plus-24@2.8.93.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:45:44.463352 cdk8s-plus-24-2.8.93/src/cdk8s_plus_24/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)  2878966 2023-07-16 02:45:32.000000 cdk8s-plus-24-2.8.93/src/cdk8s_plus_24/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 02:45:32.000000 cdk8s-plus-24-2.8.93/src/cdk8s_plus_24/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:45:44.459352 cdk8s-plus-24-2.8.93/src/cdk8s_plus_24.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-16 02:45:44.000000 cdk8s-plus-24-2.8.93/src/cdk8s_plus_24.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-16 02:45:44.000000 cdk8s-plus-24-2.8.93/src/cdk8s_plus_24.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 02:45:44.000000 cdk8s-plus-24-2.8.93/src/cdk8s_plus_24.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-16 02:45:44.000000 cdk8s-plus-24-2.8.93/src/cdk8s_plus_24.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 02:45:44.000000 cdk8s-plus-24-2.8.93/src/cdk8s_plus_24.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:27:39.155301 cdk8s-plus-24-2.8.94/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-17 00:27:24.000000 cdk8s-plus-24-2.8.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 00:27:24.000000 cdk8s-plus-24-2.8.94/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-17 00:27:24.000000 cdk8s-plus-24-2.8.94/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-17 00:27:39.155301 cdk8s-plus-24-2.8.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-17 00:27:24.000000 cdk8s-plus-24-2.8.94/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-17 00:27:24.000000 cdk8s-plus-24-2.8.94/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 00:27:39.155301 cdk8s-plus-24-2.8.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-17 00:27:24.000000 cdk8s-plus-24-2.8.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:27:39.143301 cdk8s-plus-24-2.8.94/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:27:39.147301 cdk8s-plus-24-2.8.94/src/cdk8s_plus_24/
+-rw-r--r--   0 runner    (1001) docker     (123)  1161790 2023-07-17 00:27:24.000000 cdk8s-plus-24-2.8.94/src/cdk8s_plus_24/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:27:39.147301 cdk8s-plus-24-2.8.94/src/cdk8s_plus_24/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-17 00:27:24.000000 cdk8s-plus-24-2.8.94/src/cdk8s_plus_24/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1279960 2023-07-17 00:27:24.000000 cdk8s-plus-24-2.8.94/src/cdk8s_plus_24/_jsii/cdk8s-plus-24@2.8.94.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:27:39.151301 cdk8s-plus-24-2.8.94/src/cdk8s_plus_24/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)  2878966 2023-07-17 00:27:24.000000 cdk8s-plus-24-2.8.94/src/cdk8s_plus_24/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 00:27:24.000000 cdk8s-plus-24-2.8.94/src/cdk8s_plus_24/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 00:27:39.147301 cdk8s-plus-24-2.8.94/src/cdk8s_plus_24.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-17 00:27:39.000000 cdk8s-plus-24-2.8.94/src/cdk8s_plus_24.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-17 00:27:39.000000 cdk8s-plus-24-2.8.94/src/cdk8s_plus_24.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 00:27:39.000000 cdk8s-plus-24-2.8.94/src/cdk8s_plus_24.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-17 00:27:39.000000 cdk8s-plus-24-2.8.94/src/cdk8s_plus_24.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 00:27:39.000000 cdk8s-plus-24-2.8.94/src/cdk8s_plus_24.egg-info/top_level.txt
```

### Comparing `cdk8s-plus-24-2.8.93/LICENSE` & `cdk8s-plus-24-2.8.94/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-24-2.8.93/PKG-INFO` & `cdk8s-plus-24-2.8.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-24
-Version: 2.8.93
+Version: 2.8.94
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-24 synthesizes Kubernetes manifests for Kubernetes 1.24.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-plus-24-2.8.93/README.md` & `cdk8s-plus-24-2.8.94/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-24-2.8.93/setup.py` & `cdk8s-plus-24-2.8.94/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-plus-24",
-    "version": "2.8.93",
+    "version": "2.8.94",
     "description": "cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-24 synthesizes Kubernetes manifests for Kubernetes 1.24.0",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-plus.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -23,15 +23,15 @@
     "packages": [
         "cdk8s_plus_24",
         "cdk8s_plus_24._jsii",
         "cdk8s_plus_24.k8s"
     ],
     "package_data": {
         "cdk8s_plus_24._jsii": [
-            "cdk8s-plus-24@2.8.93.jsii.tgz"
+            "cdk8s-plus-24@2.8.94.jsii.tgz"
         ],
         "cdk8s_plus_24": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk8s-plus-24-2.8.93/src/cdk8s_plus_24/__init__.py` & `cdk8s-plus-24-2.8.94/src/cdk8s_plus_24/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-24-2.8.93/src/cdk8s_plus_24/k8s/__init__.py` & `cdk8s-plus-24-2.8.94/src/cdk8s_plus_24/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-24-2.8.93/src/cdk8s_plus_24.egg-info/PKG-INFO` & `cdk8s-plus-24-2.8.94/src/cdk8s_plus_24.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-24
-Version: 2.8.93
+Version: 2.8.94
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-24 synthesizes Kubernetes manifests for Kubernetes 1.24.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

