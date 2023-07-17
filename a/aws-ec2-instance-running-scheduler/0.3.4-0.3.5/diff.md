# Comparing `tmp/aws-ec2-instance-running-scheduler-0.3.4.tar.gz` & `tmp/aws-ec2-instance-running-scheduler-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ec2-instance-running-scheduler-0.3.4.tar", last modified: Sun Jul 16 19:19:53 2023, max compression
+gzip compressed data, was "aws-ec2-instance-running-scheduler-0.3.5.tar", last modified: Mon Jul 17 19:20:30 2023, max compression
```

## Comparing `aws-ec2-instance-running-scheduler-0.3.4.tar` & `aws-ec2-instance-running-scheduler-0.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:19:53.323842 aws-ec2-instance-running-scheduler-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-16 19:19:42.000000 aws-ec2-instance-running-scheduler-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-16 19:19:42.000000 aws-ec2-instance-running-scheduler-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-16 19:19:53.323842 aws-ec2-instance-running-scheduler-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-16 19:19:42.000000 aws-ec2-instance-running-scheduler-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-16 19:19:42.000000 aws-ec2-instance-running-scheduler-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 19:19:53.323842 aws-ec2-instance-running-scheduler-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-16 19:19:42.000000 aws-ec2-instance-running-scheduler-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:19:53.323842 aws-ec2-instance-running-scheduler-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:19:53.323842 aws-ec2-instance-running-scheduler-0.3.4/src/aws_ec2_instance_running_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-07-16 19:19:42.000000 aws-ec2-instance-running-scheduler-0.3.4/src/aws_ec2_instance_running_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:19:53.323842 aws-ec2-instance-running-scheduler-0.3.4/src/aws_ec2_instance_running_scheduler/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-16 19:19:42.000000 aws-ec2-instance-running-scheduler-0.3.4/src/aws_ec2_instance_running_scheduler/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20606 2023-07-16 19:19:42.000000 aws-ec2-instance-running-scheduler-0.3.4/src/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.3.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 19:19:42.000000 aws-ec2-instance-running-scheduler-0.3.4/src/aws_ec2_instance_running_scheduler/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:19:53.323842 aws-ec2-instance-running-scheduler-0.3.4/src/aws_ec2_instance_running_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-16 19:19:53.000000 aws-ec2-instance-running-scheduler-0.3.4/src/aws_ec2_instance_running_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-16 19:19:53.000000 aws-ec2-instance-running-scheduler-0.3.4/src/aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 19:19:53.000000 aws-ec2-instance-running-scheduler-0.3.4/src/aws_ec2_instance_running_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-16 19:19:53.000000 aws-ec2-instance-running-scheduler-0.3.4/src/aws_ec2_instance_running_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-16 19:19:53.000000 aws-ec2-instance-running-scheduler-0.3.4/src/aws_ec2_instance_running_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:20:30.382882 aws-ec2-instance-running-scheduler-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-17 19:20:18.000000 aws-ec2-instance-running-scheduler-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 19:20:18.000000 aws-ec2-instance-running-scheduler-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-17 19:20:30.382882 aws-ec2-instance-running-scheduler-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-17 19:20:18.000000 aws-ec2-instance-running-scheduler-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-17 19:20:18.000000 aws-ec2-instance-running-scheduler-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 19:20:30.382882 aws-ec2-instance-running-scheduler-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-17 19:20:18.000000 aws-ec2-instance-running-scheduler-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:20:30.378882 aws-ec2-instance-running-scheduler-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:20:30.378882 aws-ec2-instance-running-scheduler-0.3.5/src/aws_ec2_instance_running_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-07-17 19:20:18.000000 aws-ec2-instance-running-scheduler-0.3.5/src/aws_ec2_instance_running_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:20:30.378882 aws-ec2-instance-running-scheduler-0.3.5/src/aws_ec2_instance_running_scheduler/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-17 19:20:18.000000 aws-ec2-instance-running-scheduler-0.3.5/src/aws_ec2_instance_running_scheduler/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20604 2023-07-17 19:20:18.000000 aws-ec2-instance-running-scheduler-0.3.5/src/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.3.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:20:18.000000 aws-ec2-instance-running-scheduler-0.3.5/src/aws_ec2_instance_running_scheduler/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:20:30.378882 aws-ec2-instance-running-scheduler-0.3.5/src/aws_ec2_instance_running_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-17 19:20:30.000000 aws-ec2-instance-running-scheduler-0.3.5/src/aws_ec2_instance_running_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-17 19:20:30.000000 aws-ec2-instance-running-scheduler-0.3.5/src/aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:20:30.000000 aws-ec2-instance-running-scheduler-0.3.5/src/aws_ec2_instance_running_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-17 19:20:30.000000 aws-ec2-instance-running-scheduler-0.3.5/src/aws_ec2_instance_running_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-17 19:20:30.000000 aws-ec2-instance-running-scheduler-0.3.5/src/aws_ec2_instance_running_scheduler.egg-info/top_level.txt
```

### Comparing `aws-ec2-instance-running-scheduler-0.3.4/LICENSE` & `aws-ec2-instance-running-scheduler-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-ec2-instance-running-scheduler-0.3.4/PKG-INFO` & `aws-ec2-instance-running-scheduler-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ec2-instance-running-scheduler
-Version: 0.3.4
+Version: 0.3.5
 Summary: AWS EC2 Instance Running Scheduler
 Home-page: https://github.com/yicr/aws-ec2-instance-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ec2-instance-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-ec2-instance-running-scheduler-0.3.4/README.md` & `aws-ec2-instance-running-scheduler-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `aws-ec2-instance-running-scheduler-0.3.4/setup.py` & `aws-ec2-instance-running-scheduler-0.3.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-ec2-instance-running-scheduler",
-    "version": "0.3.4",
+    "version": "0.3.5",
     "description": "AWS EC2 Instance Running Scheduler",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-ec2-instance-running-scheduler.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "aws_ec2_instance_running_scheduler",
         "aws_ec2_instance_running_scheduler._jsii"
     ],
     "package_data": {
         "aws_ec2_instance_running_scheduler._jsii": [
-            "aws-ec2-instance-running-scheduler@0.3.4.jsii.tgz"
+            "aws-ec2-instance-running-scheduler@0.3.5.jsii.tgz"
         ],
         "aws_ec2_instance_running_scheduler": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.62.0, <3.0.0",
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

### Comparing `aws-ec2-instance-running-scheduler-0.3.4/src/aws_ec2_instance_running_scheduler/__init__.py` & `aws-ec2-instance-running-scheduler-0.3.5/src/aws_ec2_instance_running_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-ec2-instance-running-scheduler-0.3.4/src/aws_ec2_instance_running_scheduler.egg-info/PKG-INFO` & `aws-ec2-instance-running-scheduler-0.3.5/src/aws_ec2_instance_running_scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ec2-instance-running-scheduler
-Version: 0.3.4
+Version: 0.3.5
 Summary: AWS EC2 Instance Running Scheduler
 Home-page: https://github.com/yicr/aws-ec2-instance-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ec2-instance-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-ec2-instance-running-scheduler-0.3.4/src/aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt` & `aws-ec2-instance-running-scheduler-0.3.5/src/aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_ec2_instance_running_scheduler/py.typed
 src/aws_ec2_instance_running_scheduler.egg-info/PKG-INFO
 src/aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt
 src/aws_ec2_instance_running_scheduler.egg-info/dependency_links.txt
 src/aws_ec2_instance_running_scheduler.egg-info/requires.txt
 src/aws_ec2_instance_running_scheduler.egg-info/top_level.txt
 src/aws_ec2_instance_running_scheduler/_jsii/__init__.py
-src/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.3.4.jsii.tgz
+src/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.3.5.jsii.tgz
```

