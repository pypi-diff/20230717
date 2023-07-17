# Comparing `tmp/aws-secure-log-bucket-0.8.3.tar.gz` & `tmp/aws-secure-log-bucket-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-secure-log-bucket-0.8.3.tar", last modified: Sun Jul 16 18:16:00 2023, max compression
+gzip compressed data, was "aws-secure-log-bucket-0.8.4.tar", last modified: Mon Jul 17 18:17:48 2023, max compression
```

## Comparing `aws-secure-log-bucket-0.8.3.tar` & `aws-secure-log-bucket-0.8.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:16:00.091034 aws-secure-log-bucket-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-16 18:16:00.091034 aws-secure-log-bucket-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 18:16:00.091034 aws-secure-log-bucket-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:16:00.087033 aws-secure-log-bucket-0.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:16:00.091034 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket/
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:16:00.091034 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23402 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@0.8.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:16:00.091034 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-16 18:16:00.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-16 18:16:00.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 18:16:00.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-16 18:16:00.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-16 18:16:00.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:17:48.449271 aws-secure-log-bucket-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-17 18:17:34.000000 aws-secure-log-bucket-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 18:17:34.000000 aws-secure-log-bucket-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-17 18:17:48.449271 aws-secure-log-bucket-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-17 18:17:34.000000 aws-secure-log-bucket-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-17 18:17:34.000000 aws-secure-log-bucket-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 18:17:48.449271 aws-secure-log-bucket-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-17 18:17:34.000000 aws-secure-log-bucket-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:17:48.445271 aws-secure-log-bucket-0.8.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:17:48.449271 aws-secure-log-bucket-0.8.4/src/aws_secure_log_bucket/
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-17 18:17:34.000000 aws-secure-log-bucket-0.8.4/src/aws_secure_log_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:17:48.449271 aws-secure-log-bucket-0.8.4/src/aws_secure_log_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-17 18:17:34.000000 aws-secure-log-bucket-0.8.4/src/aws_secure_log_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23404 2023-07-17 18:17:34.000000 aws-secure-log-bucket-0.8.4/src/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@0.8.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 18:17:34.000000 aws-secure-log-bucket-0.8.4/src/aws_secure_log_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:17:48.449271 aws-secure-log-bucket-0.8.4/src/aws_secure_log_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-17 18:17:48.000000 aws-secure-log-bucket-0.8.4/src/aws_secure_log_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-17 18:17:48.000000 aws-secure-log-bucket-0.8.4/src/aws_secure_log_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 18:17:48.000000 aws-secure-log-bucket-0.8.4/src/aws_secure_log_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-17 18:17:48.000000 aws-secure-log-bucket-0.8.4/src/aws_secure_log_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 18:17:48.000000 aws-secure-log-bucket-0.8.4/src/aws_secure_log_bucket.egg-info/top_level.txt
```

### Comparing `aws-secure-log-bucket-0.8.3/LICENSE` & `aws-secure-log-bucket-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-secure-log-bucket-0.8.3/PKG-INFO` & `aws-secure-log-bucket-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-secure-log-bucket
-Version: 0.8.3
+Version: 0.8.4
 Summary: secure multiple transition phases in a single lifecycle policy bucket.
 Home-page: https://github.com/yicr/aws-secure-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-secure-log-bucket-0.8.3/README.md` & `aws-secure-log-bucket-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `aws-secure-log-bucket-0.8.3/setup.py` & `aws-secure-log-bucket-0.8.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-secure-log-bucket",
-    "version": "0.8.3",
+    "version": "0.8.4",
     "description": "secure multiple transition phases in a single lifecycle policy bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-secure-log-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,26 @@
     },
     "packages": [
         "aws_secure_log_bucket",
         "aws_secure_log_bucket._jsii"
     ],
     "package_data": {
         "aws_secure_log_bucket._jsii": [
-            "aws-secure-log-bucket@0.8.3.jsii.tgz"
+            "aws-secure-log-bucket@0.8.4.jsii.tgz"
         ],
         "aws_secure_log_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.61.0, <3.0.0",
         "aws-secure-bucket>=0.7.1, <0.8.0",
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

### Comparing `aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket/__init__.py` & `aws-secure-log-bucket-0.8.4/src/aws_secure_log_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket.egg-info/PKG-INFO` & `aws-secure-log-bucket-0.8.4/src/aws_secure_log_bucket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-secure-log-bucket
-Version: 0.8.3
+Version: 0.8.4
 Summary: secure multiple transition phases in a single lifecycle policy bucket.
 Home-page: https://github.com/yicr/aws-secure-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

