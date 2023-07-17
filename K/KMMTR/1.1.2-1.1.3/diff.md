# Comparing `tmp/KMMTR-1.1.2.tar.gz` & `tmp/KMMTR-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KMMTR-1.1.2.tar", last modified: Mon Jun  5 10:25:24 2023, max compression
+gzip compressed data, was "KMMTR-1.1.3.tar", last modified: Mon Jul 17 02:04:54 2023, max compression
```

## Comparing `KMMTR-1.1.2.tar` & `KMMTR-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-05 10:25:24.843181 KMMTR-1.1.2/
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-05 10:25:24.842284 KMMTR-1.1.2/KMMTR/
--rwxr-xr-x   0 jacob      (501) staff       (20)     6888 2023-06-05 08:58:37.000000 KMMTR-1.1.2/KMMTR/KMM.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     6782 2023-06-05 09:01:20.000000 KMMTR-1.1.2/KMMTR/KMMTR.py
--rwxr-xr-x   0 jacob      (501) staff       (20)      386 2023-04-19 10:18:26.000000 KMMTR-1.1.2/KMMTR/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-05 10:25:24.842876 KMMTR-1.1.2/KMMTR.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-06-05 10:25:24.000000 KMMTR-1.1.2/KMMTR.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      208 2023-06-05 10:25:24.000000 KMMTR-1.1.2/KMMTR.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-06-05 10:25:24.000000 KMMTR-1.1.2/KMMTR.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       33 2023-06-05 10:25:24.000000 KMMTR-1.1.2/KMMTR.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        6 2023-06-05 10:25:24.000000 KMMTR-1.1.2/KMMTR.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-06-05 10:25:24.843049 KMMTR-1.1.2/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      859 2023-04-20 09:04:07.000000 KMMTR-1.1.2/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-06-05 10:25:24.843220 KMMTR-1.1.2/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1381 2023-06-05 10:24:35.000000 KMMTR-1.1.2/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 02:04:54.734398 KMMTR-1.1.3/
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 02:04:54.733472 KMMTR-1.1.3/KMMTR/
+-rwxr-xr-x   0 jacob      (501) staff       (20)     6888 2023-06-05 08:58:37.000000 KMMTR-1.1.3/KMMTR/KMM.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     6782 2023-06-05 09:01:20.000000 KMMTR-1.1.3/KMMTR/KMMTR.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)      916 2023-07-17 01:58:30.000000 KMMTR-1.1.3/KMMTR/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 02:04:54.734108 KMMTR-1.1.3/KMMTR.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-07-17 02:04:54.000000 KMMTR-1.1.3/KMMTR.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      208 2023-07-17 02:04:54.000000 KMMTR-1.1.3/KMMTR.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-07-17 02:04:54.000000 KMMTR-1.1.3/KMMTR.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       33 2023-07-17 02:04:54.000000 KMMTR-1.1.3/KMMTR.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        6 2023-07-17 02:04:54.000000 KMMTR-1.1.3/KMMTR.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-07-17 02:04:54.734273 KMMTR-1.1.3/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      859 2023-04-20 09:04:07.000000 KMMTR-1.1.3/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-07-17 02:04:54.734438 KMMTR-1.1.3/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1381 2023-07-17 01:58:57.000000 KMMTR-1.1.3/setup.py
```

### Comparing `KMMTR-1.1.2/KMMTR/KMM.py` & `KMMTR-1.1.3/KMMTR/KMM.py`

 * *Files identical despite different names*

### Comparing `KMMTR-1.1.2/KMMTR/KMMTR.py` & `KMMTR-1.1.3/KMMTR/KMMTR.py`

 * *Files identical despite different names*

### Comparing `KMMTR-1.1.2/KMMTR.egg-info/PKG-INFO` & `KMMTR-1.1.3/KMMTR.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMMTR
-Version: 1.1.2
+Version: 1.1.3
 Summary: a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm
 Home-page: https://github.com/Bin-Cao/KMMTransferRegressor
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `KMMTR-1.1.2/PKG-INFO` & `KMMTR-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMMTR
-Version: 1.1.2
+Version: 1.1.3
 Summary: a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm
 Home-page: https://github.com/Bin-Cao/KMMTransferRegressor
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `KMMTR-1.1.2/README.md` & `KMMTR-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `KMMTR-1.1.2/setup.py` & `KMMTR-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='KMMTR',  # 包名
-    version='1.1.2',  # 版本
+    version='1.1.3',  # 版本
     description="a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

