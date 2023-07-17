# Comparing `tmp/alibabacloud_rds20140815_py2-1.2.7.tar.gz` & `tmp/alibabacloud_rds20140815_py2-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_rds20140815_py2-1.2.7.tar", last modified: Sun Jul 16 15:09:46 2023, max compression
+gzip compressed data, was "dist/alibabacloud_rds20140815_py2-1.2.8.tar", last modified: Mon Jul 17 15:10:36 2023, max compression
```

## Comparing `alibabacloud_rds20140815_py2-1.2.7.tar` & `alibabacloud_rds20140815_py2-1.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/
--rw-r--r--   0 root         (0) root         (0)     2108 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2472 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/alibabacloud_rds20140815/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/alibabacloud_rds20140815/__init__.py
--rw-r--r--   0 root         (0) root         (0)   755057 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/alibabacloud_rds20140815/client.py
--rw-r--r--   0 root         (0) root         (0)  2570909 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/alibabacloud_rds20140815/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/alibabacloud_rds20140815_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2472 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/alibabacloud_rds20140815_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/alibabacloud_rds20140815_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/alibabacloud_rds20140815_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/alibabacloud_rds20140815_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/alibabacloud_rds20140815_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2903 2023-07-16 15:09:46.000000 alibabacloud_rds20140815_py2-1.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/alibabacloud_rds20140815/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/alibabacloud_rds20140815/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   755037 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/alibabacloud_rds20140815/client.py
+-rw-r--r--   0 root         (0) root         (0)  2570909 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/alibabacloud_rds20140815/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/alibabacloud_rds20140815_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/alibabacloud_rds20140815_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/alibabacloud_rds20140815_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/alibabacloud_rds20140815_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/alibabacloud_rds20140815_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/alibabacloud_rds20140815_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-07-17 15:10:36.000000 alibabacloud_rds20140815_py2-1.2.8/setup.py
```

### Comparing `alibabacloud_rds20140815_py2-1.2.7/ChangeLog.md` & `alibabacloud_rds20140815_py2-1.2.8/ChangeLog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-16 Version: 1.2.7
+- Add error code.
+
 2023-07-15 Version: 1.2.6
 - Add error code.
 
 2023-07-13 Version: 1.2.5
 - Support change instance config event for rds.
 - Add NodeId param for restart slave.
```

### Comparing `alibabacloud_rds20140815_py2-1.2.7/LICENSE` & `alibabacloud_rds20140815_py2-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.2.7/PKG-INFO` & `alibabacloud_rds20140815_py2-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_rds20140815_py2
-Version: 1.2.7
+Version: 1.2.8
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815_py2-1.2.7/README-CN.md` & `alibabacloud_rds20140815_py2-1.2.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.2.7/README.md` & `alibabacloud_rds20140815_py2-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.2.7/alibabacloud_rds20140815/client.py` & `alibabacloud_rds20140815_py2-1.2.8/alibabacloud_rds20140815/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11070,15 +11070,14 @@
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbinstance_connection_mode_with_options(request, runtime)
 
     def modify_dbinstance_connection_string_with_options(self, request, runtime):
         """
         ApsaraDB RDS provides the internal and public endpoints. ApsaraDB RDS also allows hybrid access by using both a virtual private cloud (VPC) endpoint and a classic network endpoint.
-        >
         *   You can change only the prefix of an endpoint.
         *   The read/write splitting endpoint cannot be changed.
         
 
         @param request: ModifyDBInstanceConnectionStringRequest
 
         @param runtime: runtime options for this request RuntimeOptions
@@ -11127,15 +11126,14 @@
             rds_20140815_models.ModifyDBInstanceConnectionStringResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_dbinstance_connection_string(self, request):
         """
         ApsaraDB RDS provides the internal and public endpoints. ApsaraDB RDS also allows hybrid access by using both a virtual private cloud (VPC) endpoint and a classic network endpoint.
-        >
         *   You can change only the prefix of an endpoint.
         *   The read/write splitting endpoint cannot be changed.
         
 
         @param request: ModifyDBInstanceConnectionStringRequest
 
         @return: ModifyDBInstanceConnectionStringResponse
```

### Comparing `alibabacloud_rds20140815_py2-1.2.7/alibabacloud_rds20140815/models.py` & `alibabacloud_rds20140815_py2-1.2.8/alibabacloud_rds20140815/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.2.7/alibabacloud_rds20140815_py2.egg-info/PKG-INFO` & `alibabacloud_rds20140815_py2-1.2.8/alibabacloud_rds20140815_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-rds20140815-py2
-Version: 1.2.7
+Version: 1.2.8
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815_py2-1.2.7/setup.py` & `alibabacloud_rds20140815_py2-1.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_rds20140815_py2.
 
-Created on 16/07/2023
+Created on 17/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_rds20140815"
 NAME = "alibabacloud_rds20140815_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud rds (20140815) SDK Library for Python2"
```

