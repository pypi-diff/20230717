# Comparing `tmp/mango-framework-0.5.0.tar.gz` & `tmp/mango-framework-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-framework-0.5.0.tar", last modified: Mon Jul 17 12:00:33 2023, max compression
+gzip compressed data, was "mango-framework-0.5.1.tar", last modified: Mon Jul 17 12:11:46 2023, max compression
```

## Comparing `mango-framework-0.5.0.tar` & `mango-framework-0.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:00:33.899848 mango-framework-0.5.0/
--rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.5.0/LICENSE
--rw-r--r--   0 mohammed   (501) staff       (20)     1903 2023-07-17 12:00:33.899612 mango-framework-0.5.0/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)     1210 2023-07-17 11:58:46.000000 mango-framework-0.5.0/README.md
--rw-r--r--   0 mohammed   (501) staff       (20)     5747 2023-07-17 05:04:24.000000 mango-framework-0.5.0/mango.py
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:00:33.899411 mango-framework-0.5.0/mango_framework.egg-info/
--rw-r--r--   0 mohammed   (501) staff       (20)     1903 2023-07-17 12:00:33.000000 mango-framework-0.5.0/mango_framework.egg-info/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-17 12:00:33.000000 mango-framework-0.5.0/mango_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:00:33.000000 mango-framework-0.5.0/mango_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:00:33.000000 mango-framework-0.5.0/mango_framework.egg-info/top_level.txt
--rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-17 12:00:33.899902 mango-framework-0.5.0/setup.cfg
--rw-r--r--   0 mohammed   (501) staff       (20)      882 2023-07-17 12:00:30.000000 mango-framework-0.5.0/setup.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:11:46.175012 mango-framework-0.5.1/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.5.1/LICENSE
+-rw-r--r--   0 mohammed   (501) staff       (20)     1890 2023-07-17 12:11:46.174902 mango-framework-0.5.1/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)     1210 2023-07-17 11:58:46.000000 mango-framework-0.5.1/README.md
+-rw-r--r--   0 mohammed   (501) staff       (20)     5747 2023-07-17 05:04:24.000000 mango-framework-0.5.1/mango.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 12:11:46.174740 mango-framework-0.5.1/mango_framework.egg-info/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1890 2023-07-17 12:11:46.000000 mango-framework-0.5.1/mango_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-17 12:11:46.000000 mango-framework-0.5.1/mango_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:11:46.000000 mango-framework-0.5.1/mango_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 12:11:46.000000 mango-framework-0.5.1/mango_framework.egg-info/top_level.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-17 12:11:46.175058 mango-framework-0.5.1/setup.cfg
+-rw-r--r--   0 mohammed   (501) staff       (20)      869 2023-07-17 12:11:42.000000 mango-framework-0.5.1/setup.py
```

### Comparing `mango-framework-0.5.0/LICENSE` & `mango-framework-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mango-framework-0.5.0/PKG-INFO` & `mango-framework-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.5.0
+Version: 0.5.1
 Summary: A lightweight and highly customizable Python framework for building web applications
-Home-page: https://github.com/yourusername/mango-framework
+Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `mango-framework-0.5.0/README.md` & `mango-framework-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mango-framework-0.5.0/mango.py` & `mango-framework-0.5.1/mango.py`

 * *Files identical despite different names*

### Comparing `mango-framework-0.5.0/mango_framework.egg-info/PKG-INFO` & `mango-framework-0.5.1/mango_framework.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.5.0
+Version: 0.5.1
 Summary: A lightweight and highly customizable Python framework for building web applications
-Home-page: https://github.com/yourusername/mango-framework
+Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `mango-framework-0.5.0/setup.py` & `mango-framework-0.5.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='mango-framework',
-    version='0.5.0',
+    version='0.5.1',
     author='Mohammed',
     author_email='fdlnaal@gmail.com',
     description='A lightweight and highly customizable Python framework for building web applications',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/yourusername/mango-framework',
+    url='https://github.com/momo-AUX1/mango',
     packages=['.'],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

