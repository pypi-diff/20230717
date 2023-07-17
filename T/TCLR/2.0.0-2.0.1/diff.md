# Comparing `tmp/TCLR-2.0.0.tar.gz` & `tmp/TCLR-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TCLR-2.0.0.tar", last modified: Thu May 25 08:43:54 2023, max compression
+gzip compressed data, was "TCLR-2.0.1.tar", last modified: Mon Jul 17 02:07:56 2023, max compression
```

## Comparing `TCLR-2.0.0.tar` & `TCLR-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-25 08:43:54.962953 TCLR-2.0.0/
--rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-25 08:43:54.962828 TCLR-2.0.0/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)     2570 2022-08-21 10:21:47.000000 TCLR-2.0.0/README.md
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-25 08:43:54.962075 TCLR-2.0.0/TCLR/
--rw-r-----   0 jacob      (501) staff       (20)    38792 2023-05-25 08:43:15.000000 TCLR-2.0.0/TCLR/TCLRalgorithm.py
--rw-r--r--   0 jacob      (501) staff       (20)      988 2023-05-25 08:16:57.000000 TCLR-2.0.0/TCLR/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-25 08:43:54.962659 TCLR-2.0.0/TCLR.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-25 08:43:54.000000 TCLR-2.0.0/TCLR.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      196 2023-05-25 08:43:54.000000 TCLR-2.0.0/TCLR.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-25 08:43:54.000000 TCLR-2.0.0/TCLR.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       30 2023-05-25 08:43:54.000000 TCLR-2.0.0/TCLR.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        5 2023-05-25 08:43:54.000000 TCLR-2.0.0/TCLR.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-25 08:43:54.962991 TCLR-2.0.0/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1440 2023-05-25 08:43:27.000000 TCLR-2.0.0/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 02:07:56.393867 TCLR-2.0.1/
+-rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-07-17 02:07:56.393736 TCLR-2.0.1/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)     2570 2022-08-21 10:21:47.000000 TCLR-2.0.1/README.md
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 02:07:56.392954 TCLR-2.0.1/TCLR/
+-rw-r-----   0 jacob      (501) staff       (20)    38792 2023-05-25 08:43:15.000000 TCLR-2.0.1/TCLR/TCLRalgorithm.py
+-rw-r--r--   0 jacob      (501) staff       (20)     1571 2023-07-17 01:56:20.000000 TCLR-2.0.1/TCLR/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 02:07:56.393568 TCLR-2.0.1/TCLR.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-07-17 02:07:56.000000 TCLR-2.0.1/TCLR.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      196 2023-07-17 02:07:56.000000 TCLR-2.0.1/TCLR.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-07-17 02:07:56.000000 TCLR-2.0.1/TCLR.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       30 2023-07-17 02:07:56.000000 TCLR-2.0.1/TCLR.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        5 2023-07-17 02:07:56.000000 TCLR-2.0.1/TCLR.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-07-17 02:07:56.393910 TCLR-2.0.1/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1440 2023-07-17 02:07:42.000000 TCLR-2.0.1/setup.py
```

### Comparing `TCLR-2.0.0/PKG-INFO` & `TCLR-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TCLR
-Version: 2.0.0
+Version: 2.0.1
 Summary: Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.
 Home-page: https://github.com/Bin-Cao/TCLRmodel
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `TCLR-2.0.0/README.md` & `TCLR-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `TCLR-2.0.0/TCLR/TCLRalgorithm.py` & `TCLR-2.0.1/TCLR/TCLRalgorithm.py`

 * *Files identical despite different names*

### Comparing `TCLR-2.0.0/TCLR.egg-info/PKG-INFO` & `TCLR-2.0.1/TCLR.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TCLR
-Version: 2.0.0
+Version: 2.0.1
 Summary: Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.
 Home-page: https://github.com/Bin-Cao/TCLRmodel
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `TCLR-2.0.0/setup.py` & `TCLR-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='TCLR',  # 包名
-    version='2.0.0',  # 版本
+    version='2.0.1',  # 版本
     description="Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

