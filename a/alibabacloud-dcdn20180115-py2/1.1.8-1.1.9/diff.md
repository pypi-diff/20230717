# Comparing `tmp/alibabacloud_dcdn20180115_py2-1.1.8.tar.gz` & `tmp/alibabacloud_dcdn20180115_py2-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dcdn20180115_py2-1.1.8.tar", last modified: Mon May 22 10:55:11 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dcdn20180115_py2-1.1.9.tar", last modified: Fri May 26 05:46:48 2023, max compression
```

## Comparing `alibabacloud_dcdn20180115_py2-1.1.8.tar` & `alibabacloud_dcdn20180115_py2-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:55:11.000000 alibabacloud_dcdn20180115_py2-1.1.8/
--rw-r--r--   0 root         (0) root         (0)     1897 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2478 2023-05-22 10:55:11.000000 alibabacloud_dcdn20180115_py2-1.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:55:11.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115/__init__.py
--rw-r--r--   0 root         (0) root         (0)   377676 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115/client.py
--rw-r--r--   0 root         (0) root         (0)  1271965 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:55:11.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2478 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      448 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-22 10:55:11.000000 alibabacloud_dcdn20180115_py2-1.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2908 2023-05-22 10:55:10.000000 alibabacloud_dcdn20180115_py2-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/
+-rw-r--r--   0 root         (0) root         (0)     1969 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/alibabacloud_dcdn20180115/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/alibabacloud_dcdn20180115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   377676 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/alibabacloud_dcdn20180115/client.py
+-rw-r--r--   0 root         (0) root         (0)  1271965 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/alibabacloud_dcdn20180115/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/alibabacloud_dcdn20180115_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/alibabacloud_dcdn20180115_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/alibabacloud_dcdn20180115_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/alibabacloud_dcdn20180115_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/alibabacloud_dcdn20180115_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/alibabacloud_dcdn20180115_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2908 2023-05-26 05:46:48.000000 alibabacloud_dcdn20180115_py2-1.1.9/setup.py
```

### Comparing `alibabacloud_dcdn20180115_py2-1.1.8/ChangeLog.md` & `alibabacloud_dcdn20180115_py2-1.1.9/ChangeLog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-05-22 Version: 1.1.8
+- Add DescribeDcdnFullDomainsBlockIPHistory.
+
 2023-05-19 Version: 1.1.7
 - Add DescribeDcdnDomainMd5Info.
 
 2023-04-25 Version: 1.1.6
 - Add CheckDcdnDomainExist.
 
 2023-03-24 Version: 1.1.5
```

### Comparing `alibabacloud_dcdn20180115_py2-1.1.8/LICENSE` & `alibabacloud_dcdn20180115_py2-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115_py2-1.1.8/PKG-INFO` & `alibabacloud_dcdn20180115_py2-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dcdn20180115_py2
-Version: 1.1.8
+Version: 1.1.9
 Summary: Alibaba Cloud dcdn (20180115) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dcdn20180115_py2-1.1.8/README-CN.md` & `alibabacloud_dcdn20180115_py2-1.1.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115_py2-1.1.8/README.md` & `alibabacloud_dcdn20180115_py2-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115/client.py` & `alibabacloud_dcdn20180115_py2-1.1.9/alibabacloud_dcdn20180115/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115/models.py` & `alibabacloud_dcdn20180115_py2-1.1.9/alibabacloud_dcdn20180115/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dcdn20180115_py2-1.1.8/alibabacloud_dcdn20180115_py2.egg-info/PKG-INFO` & `alibabacloud_dcdn20180115_py2-1.1.9/alibabacloud_dcdn20180115_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dcdn20180115-py2
-Version: 1.1.8
+Version: 1.1.9
 Summary: Alibaba Cloud dcdn (20180115) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dcdn20180115_py2-1.1.8/setup.py` & `alibabacloud_dcdn20180115_py2-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dcdn20180115_py2.
 
-Created on 22/05/2023
+Created on 26/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dcdn20180115"
 NAME = "alibabacloud_dcdn20180115_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud dcdn (20180115) SDK Library for Python2"
```

