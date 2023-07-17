# Comparing `tmp/birdroid.aws-secure-bucket-0.8.3.tar.gz` & `tmp/birdroid.aws-secure-bucket-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "birdroid.aws-secure-bucket-0.8.3.tar", last modified: Sun Jul 16 17:23:51 2023, max compression
+gzip compressed data, was "birdroid.aws-secure-bucket-0.8.4.tar", last modified: Mon Jul 17 17:24:56 2023, max compression
```

## Comparing `birdroid.aws-secure-bucket-0.8.3.tar` & `birdroid.aws-secure-bucket-0.8.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:23:51.460372 birdroid.aws-secure-bucket-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-16 17:23:39.000000 birdroid.aws-secure-bucket-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-16 17:23:39.000000 birdroid.aws-secure-bucket-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-16 17:23:51.460372 birdroid.aws-secure-bucket-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-16 17:23:39.000000 birdroid.aws-secure-bucket-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-16 17:23:39.000000 birdroid.aws-secure-bucket-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 17:23:51.460372 birdroid.aws-secure-bucket-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-16 17:23:39.000000 birdroid.aws-secure-bucket-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:23:51.456372 birdroid.aws-secure-bucket-0.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:23:51.456372 birdroid.aws-secure-bucket-0.8.3/src/birdroid/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:23:51.460372 birdroid.aws-secure-bucket-0.8.3/src/birdroid/aws_secure_bucket/
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-16 17:23:39.000000 birdroid.aws-secure-bucket-0.8.3/src/birdroid/aws_secure_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:23:51.460372 birdroid.aws-secure-bucket-0.8.3/src/birdroid/aws_secure_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-16 17:23:39.000000 birdroid.aws-secure-bucket-0.8.3/src/birdroid/aws_secure_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30742 2023-07-16 17:23:39.000000 birdroid.aws-secure-bucket-0.8.3/src/birdroid/aws_secure_bucket/_jsii/aws-secure-bucket@0.8.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:23:39.000000 birdroid.aws-secure-bucket-0.8.3/src/birdroid/aws_secure_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:23:51.456372 birdroid.aws-secure-bucket-0.8.3/src/birdroid.aws_secure_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-16 17:23:51.000000 birdroid.aws-secure-bucket-0.8.3/src/birdroid.aws_secure_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-16 17:23:51.000000 birdroid.aws-secure-bucket-0.8.3/src/birdroid.aws_secure_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:23:51.000000 birdroid.aws-secure-bucket-0.8.3/src/birdroid.aws_secure_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-16 17:23:51.000000 birdroid.aws-secure-bucket-0.8.3/src/birdroid.aws_secure_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 17:23:51.000000 birdroid.aws-secure-bucket-0.8.3/src/birdroid.aws_secure_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:24:56.841020 birdroid.aws-secure-bucket-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-17 17:24:40.000000 birdroid.aws-secure-bucket-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 17:24:40.000000 birdroid.aws-secure-bucket-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-17 17:24:56.841020 birdroid.aws-secure-bucket-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-17 17:24:40.000000 birdroid.aws-secure-bucket-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-17 17:24:40.000000 birdroid.aws-secure-bucket-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 17:24:56.841020 birdroid.aws-secure-bucket-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-17 17:24:40.000000 birdroid.aws-secure-bucket-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:24:56.837020 birdroid.aws-secure-bucket-0.8.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:24:56.837020 birdroid.aws-secure-bucket-0.8.4/src/birdroid/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:24:56.841020 birdroid.aws-secure-bucket-0.8.4/src/birdroid/aws_secure_bucket/
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-17 17:24:40.000000 birdroid.aws-secure-bucket-0.8.4/src/birdroid/aws_secure_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:24:56.841020 birdroid.aws-secure-bucket-0.8.4/src/birdroid/aws_secure_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-17 17:24:40.000000 birdroid.aws-secure-bucket-0.8.4/src/birdroid/aws_secure_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30741 2023-07-17 17:24:40.000000 birdroid.aws-secure-bucket-0.8.4/src/birdroid/aws_secure_bucket/_jsii/aws-secure-bucket@0.8.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:24:40.000000 birdroid.aws-secure-bucket-0.8.4/src/birdroid/aws_secure_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:24:56.841020 birdroid.aws-secure-bucket-0.8.4/src/birdroid.aws_secure_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-17 17:24:56.000000 birdroid.aws-secure-bucket-0.8.4/src/birdroid.aws_secure_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-17 17:24:56.000000 birdroid.aws-secure-bucket-0.8.4/src/birdroid.aws_secure_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:24:56.000000 birdroid.aws-secure-bucket-0.8.4/src/birdroid.aws_secure_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-17 17:24:56.000000 birdroid.aws-secure-bucket-0.8.4/src/birdroid.aws_secure_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 17:24:56.000000 birdroid.aws-secure-bucket-0.8.4/src/birdroid.aws_secure_bucket.egg-info/top_level.txt
```

### Comparing `birdroid.aws-secure-bucket-0.8.3/LICENSE` & `birdroid.aws-secure-bucket-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `birdroid.aws-secure-bucket-0.8.3/PKG-INFO` & `birdroid.aws-secure-bucket-0.8.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birdroid.aws-secure-bucket
-Version: 0.8.3
+Version: 0.8.4
 Summary: This is a Simple S3 Secure Bucket.
 Home-page: https://github.com/yicr/aws-secure-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `birdroid.aws-secure-bucket-0.8.3/README.md` & `birdroid.aws-secure-bucket-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `birdroid.aws-secure-bucket-0.8.3/setup.py` & `birdroid.aws-secure-bucket-0.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "birdroid.aws-secure-bucket",
-    "version": "0.8.3",
+    "version": "0.8.4",
     "description": "This is a Simple S3 Secure Bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-secure-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "birdroid.aws_secure_bucket",
         "birdroid.aws_secure_bucket._jsii"
     ],
     "package_data": {
         "birdroid.aws_secure_bucket._jsii": [
-            "aws-secure-bucket@0.8.3.jsii.tgz"
+            "aws-secure-bucket@0.8.4.jsii.tgz"
         ],
         "birdroid.aws_secure_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.61.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.84.0, <2.0.0",
+        "jsii>=1.85.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `birdroid.aws-secure-bucket-0.8.3/src/birdroid/aws_secure_bucket/__init__.py` & `birdroid.aws-secure-bucket-0.8.4/src/birdroid/aws_secure_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `birdroid.aws-secure-bucket-0.8.3/src/birdroid.aws_secure_bucket.egg-info/PKG-INFO` & `birdroid.aws-secure-bucket-0.8.4/src/birdroid.aws_secure_bucket.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birdroid.aws-secure-bucket
-Version: 0.8.3
+Version: 0.8.4
 Summary: This is a Simple S3 Secure Bucket.
 Home-page: https://github.com/yicr/aws-secure-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `birdroid.aws-secure-bucket-0.8.3/src/birdroid.aws_secure_bucket.egg-info/SOURCES.txt` & `birdroid.aws-secure-bucket-0.8.4/src/birdroid.aws_secure_bucket.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/birdroid.aws_secure_bucket.egg-info/SOURCES.txt
 src/birdroid.aws_secure_bucket.egg-info/dependency_links.txt
 src/birdroid.aws_secure_bucket.egg-info/requires.txt
 src/birdroid.aws_secure_bucket.egg-info/top_level.txt
 src/birdroid/aws_secure_bucket/__init__.py
 src/birdroid/aws_secure_bucket/py.typed
 src/birdroid/aws_secure_bucket/_jsii/__init__.py
-src/birdroid/aws_secure_bucket/_jsii/aws-secure-bucket@0.8.3.jsii.tgz
+src/birdroid/aws_secure_bucket/_jsii/aws-secure-bucket@0.8.4.jsii.tgz
```

