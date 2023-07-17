# Comparing `tmp/Bgolearn-2.1.1.tar.gz` & `tmp/Bgolearn-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bgolearn-2.1.1.tar", last modified: Fri Jun  9 00:10:45 2023, max compression
+gzip compressed data, was "Bgolearn-2.2.0.tar", last modified: Mon Jul 17 02:06:04 2023, max compression
```

## Comparing `Bgolearn-2.1.1.tar` & `Bgolearn-2.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-09 00:10:45.002756 Bgolearn-2.1.1/
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-09 00:10:45.001865 Bgolearn-2.1.1/Bgolearn/
--rwxr-xr-x   0 jacob      (501) staff       (20)    24205 2023-04-06 12:56:14.000000 Bgolearn-2.1.1/Bgolearn/BGO_eval.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     3932 2023-04-23 02:14:51.000000 Bgolearn-2.1.1/Bgolearn/BGOclf.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    18438 2022-10-13 07:31:41.000000 Bgolearn-2.1.1/Bgolearn/BGOmax.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    18412 2022-10-14 04:10:19.000000 Bgolearn-2.1.1/Bgolearn/BGOmin.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    21169 2023-06-09 00:10:03.000000 Bgolearn-2.1.1/Bgolearn/BGOsampling.py
--rwxr-xr-x   0 jacob      (501) staff       (20)      508 2023-06-09 00:06:27.000000 Bgolearn-2.1.1/Bgolearn/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-09 00:10:45.002462 Bgolearn-2.1.1/Bgolearn.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-06-09 00:10:44.000000 Bgolearn-2.1.1/Bgolearn.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      300 2023-06-09 00:10:44.000000 Bgolearn-2.1.1/Bgolearn.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-06-09 00:10:44.000000 Bgolearn-2.1.1/Bgolearn.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       43 2023-06-09 00:10:44.000000 Bgolearn-2.1.1/Bgolearn.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        9 2023-06-09 00:10:44.000000 Bgolearn-2.1.1/Bgolearn.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-06-09 00:10:45.002627 Bgolearn-2.1.1/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)     1917 2022-11-06 12:06:03.000000 Bgolearn-2.1.1/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-06-09 00:10:45.002798 Bgolearn-2.1.1/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1366 2023-06-09 00:10:21.000000 Bgolearn-2.1.1/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 02:06:04.810840 Bgolearn-2.2.0/
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 02:06:04.809801 Bgolearn-2.2.0/Bgolearn/
+-rwxr-xr-x   0 jacob      (501) staff       (20)    24205 2023-04-06 12:56:14.000000 Bgolearn-2.2.0/Bgolearn/BGO_eval.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     3932 2023-04-23 02:14:51.000000 Bgolearn-2.2.0/Bgolearn/BGOclf.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    18438 2022-10-13 07:31:41.000000 Bgolearn-2.2.0/Bgolearn/BGOmax.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    18412 2022-10-14 04:10:19.000000 Bgolearn-2.2.0/Bgolearn/BGOmin.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    21169 2023-06-17 08:28:15.000000 Bgolearn-2.2.0/Bgolearn/BGOsampling.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     1129 2023-07-17 01:55:17.000000 Bgolearn-2.2.0/Bgolearn/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 02:06:04.810543 Bgolearn-2.2.0/Bgolearn.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-07-17 02:06:04.000000 Bgolearn-2.2.0/Bgolearn.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      300 2023-07-17 02:06:04.000000 Bgolearn-2.2.0/Bgolearn.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-07-17 02:06:04.000000 Bgolearn-2.2.0/Bgolearn.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       43 2023-07-17 02:06:04.000000 Bgolearn-2.2.0/Bgolearn.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        9 2023-07-17 02:06:04.000000 Bgolearn-2.2.0/Bgolearn.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-07-17 02:06:04.810714 Bgolearn-2.2.0/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)     1917 2022-11-06 12:06:03.000000 Bgolearn-2.2.0/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-07-17 02:06:04.810881 Bgolearn-2.2.0/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1366 2023-07-17 02:05:54.000000 Bgolearn-2.2.0/setup.py
```

### Comparing `Bgolearn-2.1.1/Bgolearn/BGO_eval.py` & `Bgolearn-2.2.0/Bgolearn/BGO_eval.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.1.1/Bgolearn/BGOclf.py` & `Bgolearn-2.2.0/Bgolearn/BGOclf.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.1.1/Bgolearn/BGOmax.py` & `Bgolearn-2.2.0/Bgolearn/BGOmax.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.1.1/Bgolearn/BGOmin.py` & `Bgolearn-2.2.0/Bgolearn/BGOmin.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.1.1/Bgolearn/BGOsampling.py` & `Bgolearn-2.2.0/Bgolearn/BGOsampling.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.1.1/Bgolearn.egg-info/PKG-INFO` & `Bgolearn-2.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: Bgolearn
-Version: 2.1.1
-Summary: A Bayesian global optimization package for material design
-Home-page: https://github.com/Bin-Cao/Bgolearn
-Author: CaoBin
-Author-email: bcao@shu.edu.com
-Maintainer: CaoBin
-Maintainer-email: binjacobcao@gmail.com
-License: MIT License
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5
-
 
 [![](https://img.shields.io/badge/PyPI-caobin-blue)](https://pypi.org/project/Bgolearn/)
 # Python package - Bgolearn 
 
 
 
 ![Screen Shot 2022-07-11 at 9 13 28 AM](https://user-images.githubusercontent.com/86995074/178176016-8a79db81-fcfb-4af0-9b1c-aa4e6a113b5e.png)
```

### Comparing `Bgolearn-2.1.1/PKG-INFO` & `Bgolearn-2.2.0/Bgolearn.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bgolearn
-Version: 2.1.1
+Version: 2.2.0
 Summary: A Bayesian global optimization package for material design
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `Bgolearn-2.1.1/README.md` & `Bgolearn-2.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: Bgolearn
+Version: 2.2.0
+Summary: A Bayesian global optimization package for material design
+Home-page: https://github.com/Bin-Cao/Bgolearn
+Author: CaoBin
+Author-email: bcao@shu.edu.com
+Maintainer: CaoBin
+Maintainer-email: binjacobcao@gmail.com
+License: MIT License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.5
+
 
 [![](https://img.shields.io/badge/PyPI-caobin-blue)](https://pypi.org/project/Bgolearn/)
 # Python package - Bgolearn 
 
 
 
 ![Screen Shot 2022-07-11 at 9 13 28 AM](https://user-images.githubusercontent.com/86995074/178176016-8a79db81-fcfb-4af0-9b1c-aa4e6a113b5e.png)
```

### Comparing `Bgolearn-2.1.1/setup.py` & `Bgolearn-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='Bgolearn',  # 包名
-    version='2.1.1',  # 版本
+    version='2.2.0',  # 版本
     description="A Bayesian global optimization package for material design",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

