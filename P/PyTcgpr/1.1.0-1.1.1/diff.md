# Comparing `tmp/PyTcgpr-1.1.0.tar.gz` & `tmp/PyTcgpr-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTcgpr-1.1.0.tar", last modified: Thu Jul  6 03:05:08 2023, max compression
+gzip compressed data, was "PyTcgpr-1.1.1.tar", last modified: Mon Jul 17 02:07:07 2023, max compression
```

## Comparing `PyTcgpr-1.1.0.tar` & `PyTcgpr-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-06 03:05:08.784296 PyTcgpr-1.1.0/
--rw-r--r--   0 jacob      (501) staff       (20)     1769 2023-07-06 03:05:08.784171 PyTcgpr-1.1.0/PKG-INFO
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-06 03:05:08.782702 PyTcgpr-1.1.0/PyTcgpr/
--rw-rw-rw-   0 jacob      (501) staff       (20)    12770 2023-07-06 03:03:53.000000 PyTcgpr-1.1.0/PyTcgpr/TCGPR.py
--rw-r--r--   0 jacob      (501) staff       (20)      482 2023-07-06 02:44:04.000000 PyTcgpr-1.1.0/PyTcgpr/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-06 03:05:08.783746 PyTcgpr-1.1.0/PyTcgpr/data/
--rw-rw-rw-   0 jacob      (501) staff       (20)    21513 2023-05-14 10:45:53.000000 PyTcgpr-1.1.0/PyTcgpr/data/DatasetPartition.py
--rw-rw-rw-   0 jacob      (501) staff       (20)    17365 2023-05-14 10:45:49.000000 PyTcgpr-1.1.0/PyTcgpr/data/OutliersIdentification.py
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-14 03:26:22.000000 PyTcgpr-1.1.0/PyTcgpr/data/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-06 03:05:08.784012 PyTcgpr-1.1.0/PyTcgpr/feature/
--rw-rw-rw-   0 jacob      (501) staff       (20)    23959 2023-05-14 10:45:49.000000 PyTcgpr-1.1.0/PyTcgpr/feature/FeaturesSelection.py
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-14 03:26:22.000000 PyTcgpr-1.1.0/PyTcgpr/feature/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-06 03:05:08.783324 PyTcgpr-1.1.0/PyTcgpr.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     1769 2023-07-06 03:05:08.000000 PyTcgpr-1.1.0/PyTcgpr.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      371 2023-07-06 03:05:08.000000 PyTcgpr-1.1.0/PyTcgpr.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-07-06 03:05:08.000000 PyTcgpr-1.1.0/PyTcgpr.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       21 2023-07-06 03:05:08.000000 PyTcgpr-1.1.0/PyTcgpr.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        8 2023-07-06 03:05:08.000000 PyTcgpr-1.1.0/PyTcgpr.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)     1142 2023-05-14 09:09:04.000000 PyTcgpr-1.1.0/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-07-06 03:05:08.784337 PyTcgpr-1.1.0/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1404 2023-07-06 03:04:47.000000 PyTcgpr-1.1.0/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 02:07:07.333443 PyTcgpr-1.1.1/
+-rw-r--r--   0 jacob      (501) staff       (20)     1769 2023-07-17 02:07:07.333312 PyTcgpr-1.1.1/PKG-INFO
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 02:07:07.331887 PyTcgpr-1.1.1/PyTcgpr/
+-rw-rw-rw-   0 jacob      (501) staff       (20)    12770 2023-07-06 03:03:53.000000 PyTcgpr-1.1.1/PyTcgpr/TCGPR.py
+-rw-r--r--   0 jacob      (501) staff       (20)     1154 2023-07-17 01:51:15.000000 PyTcgpr-1.1.1/PyTcgpr/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 02:07:07.332884 PyTcgpr-1.1.1/PyTcgpr/data/
+-rw-rw-rw-   0 jacob      (501) staff       (20)    21513 2023-05-14 10:45:53.000000 PyTcgpr-1.1.1/PyTcgpr/data/DatasetPartition.py
+-rw-rw-rw-   0 jacob      (501) staff       (20)    17365 2023-05-14 10:45:49.000000 PyTcgpr-1.1.1/PyTcgpr/data/OutliersIdentification.py
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-14 03:26:22.000000 PyTcgpr-1.1.1/PyTcgpr/data/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 02:07:07.333148 PyTcgpr-1.1.1/PyTcgpr/feature/
+-rw-rw-rw-   0 jacob      (501) staff       (20)    23959 2023-05-14 10:45:49.000000 PyTcgpr-1.1.1/PyTcgpr/feature/FeaturesSelection.py
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-14 03:26:22.000000 PyTcgpr-1.1.1/PyTcgpr/feature/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 02:07:07.332476 PyTcgpr-1.1.1/PyTcgpr.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     1769 2023-07-17 02:07:07.000000 PyTcgpr-1.1.1/PyTcgpr.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      371 2023-07-17 02:07:07.000000 PyTcgpr-1.1.1/PyTcgpr.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-07-17 02:07:07.000000 PyTcgpr-1.1.1/PyTcgpr.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       21 2023-07-17 02:07:07.000000 PyTcgpr-1.1.1/PyTcgpr.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        8 2023-07-17 02:07:07.000000 PyTcgpr-1.1.1/PyTcgpr.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)     1142 2023-05-14 09:09:04.000000 PyTcgpr-1.1.1/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-07-17 02:07:07.333482 PyTcgpr-1.1.1/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1404 2023-07-17 02:06:56.000000 PyTcgpr-1.1.1/setup.py
```

### Comparing `PyTcgpr-1.1.0/PKG-INFO` & `PyTcgpr-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTcgpr
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tree-Classifier for gaussian process model (TCGPR) is a data preprocessing algorithm based on the Gaussian correlation among data.
 Home-page: https://github.com/Bin-Cao/TCGPR
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: 17734910905@163.com
 License: MIT License
```

### Comparing `PyTcgpr-1.1.0/PyTcgpr/TCGPR.py` & `PyTcgpr-1.1.1/PyTcgpr/TCGPR.py`

 * *Files identical despite different names*

### Comparing `PyTcgpr-1.1.0/PyTcgpr/data/DatasetPartition.py` & `PyTcgpr-1.1.1/PyTcgpr/data/DatasetPartition.py`

 * *Files identical despite different names*

### Comparing `PyTcgpr-1.1.0/PyTcgpr/data/OutliersIdentification.py` & `PyTcgpr-1.1.1/PyTcgpr/data/OutliersIdentification.py`

 * *Files identical despite different names*

### Comparing `PyTcgpr-1.1.0/PyTcgpr/feature/FeaturesSelection.py` & `PyTcgpr-1.1.1/PyTcgpr/feature/FeaturesSelection.py`

 * *Files identical despite different names*

### Comparing `PyTcgpr-1.1.0/PyTcgpr.egg-info/PKG-INFO` & `PyTcgpr-1.1.1/PyTcgpr.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTcgpr
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tree-Classifier for gaussian process model (TCGPR) is a data preprocessing algorithm based on the Gaussian correlation among data.
 Home-page: https://github.com/Bin-Cao/TCGPR
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: 17734910905@163.com
 License: MIT License
```

### Comparing `PyTcgpr-1.1.0/README.md` & `PyTcgpr-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `PyTcgpr-1.1.0/setup.py` & `PyTcgpr-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='PyTcgpr',  # 包名
-    version='1.1.0',  # 版本
+    version='1.1.1',  # 版本
     description="Tree-Classifier for gaussian process model (TCGPR) is a data preprocessing algorithm based on the Gaussian correlation among data.",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='17734910905@163.com',  # 维护者邮件
```

