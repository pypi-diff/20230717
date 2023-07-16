# Comparing `tmp/mohaliyet_annconv-0.1.tar.gz` & `tmp/mohaliyet_annconv-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mohaliyet_annconv-0.1.tar", last modified: Sun Jul 16 22:44:13 2023, max compression
+gzip compressed data, was "mohaliyet_annconv-0.2.tar", last modified: Sun Jul 16 22:57:38 2023, max compression
```

## Comparing `mohaliyet_annconv-0.1.tar` & `mohaliyet_annconv-0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 22:44:13.932949 mohaliyet_annconv-0.1/
--rw-rw-rw-   0        0        0      246 2023-07-16 22:44:13.932949 mohaliyet_annconv-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-07-16 22:21:07.000000 mohaliyet_annconv-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 22:44:13.900940 mohaliyet_annconv-0.1/annotation_converter/
--rw-rw-rw-   0        0        0        0 2023-07-16 10:15:06.000000 mohaliyet_annconv-0.1/annotation_converter/__init__.py
--rw-rw-rw-   0        0        0     1912 2023-07-16 22:10:58.000000 mohaliyet_annconv-0.1/annotation_converter/main.py
--rw-rw-rw-   0        0        0     1732 2023-07-16 22:10:44.000000 mohaliyet_annconv-0.1/annotation_converter/parsers.py
--rw-rw-rw-   0        0        0     1020 2023-07-16 21:49:58.000000 mohaliyet_annconv-0.1/annotation_converter/writers.py
-drwxrwxrwx   0        0        0        0 2023-07-16 22:44:13.924958 mohaliyet_annconv-0.1/mohaliyet_annconv.egg-info/
--rw-rw-rw-   0        0        0      246 2023-07-16 22:44:13.000000 mohaliyet_annconv-0.1/mohaliyet_annconv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-07-16 22:44:13.000000 mohaliyet_annconv-0.1/mohaliyet_annconv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 22:44:13.000000 mohaliyet_annconv-0.1/mohaliyet_annconv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-07-16 22:44:13.000000 mohaliyet_annconv-0.1/mohaliyet_annconv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-07-16 22:44:13.000000 mohaliyet_annconv-0.1/mohaliyet_annconv.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-07-16 22:44:13.000000 mohaliyet_annconv-0.1/mohaliyet_annconv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 22:44:13.932949 mohaliyet_annconv-0.1/setup.cfg
--rw-rw-rw-   0        0        0      533 2023-07-16 22:42:59.000000 mohaliyet_annconv-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 22:44:13.932949 mohaliyet_annconv-0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-07-16 10:15:52.000000 mohaliyet_annconv-0.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 22:57:38.379702 mohaliyet_annconv-0.2/
+-rw-rw-rw-   0        0        0      246 2023-07-16 22:57:38.375695 mohaliyet_annconv-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-07-16 22:21:07.000000 mohaliyet_annconv-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 22:57:38.347657 mohaliyet_annconv-0.2/annotation_converter/
+-rw-rw-rw-   0        0        0        0 2023-07-16 10:15:06.000000 mohaliyet_annconv-0.2/annotation_converter/__init__.py
+-rw-rw-rw-   0        0        0     1912 2023-07-16 22:10:58.000000 mohaliyet_annconv-0.2/annotation_converter/main.py
+-rw-rw-rw-   0        0        0     1732 2023-07-16 22:10:44.000000 mohaliyet_annconv-0.2/annotation_converter/parsers.py
+-rw-rw-rw-   0        0        0     1020 2023-07-16 21:49:58.000000 mohaliyet_annconv-0.2/annotation_converter/writers.py
+drwxrwxrwx   0        0        0        0 2023-07-16 22:57:38.371684 mohaliyet_annconv-0.2/mohaliyet_annconv.egg-info/
+-rw-rw-rw-   0        0        0      246 2023-07-16 22:57:38.000000 mohaliyet_annconv-0.2/mohaliyet_annconv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-07-16 22:57:38.000000 mohaliyet_annconv-0.2/mohaliyet_annconv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 22:57:38.000000 mohaliyet_annconv-0.2/mohaliyet_annconv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-07-16 22:57:38.000000 mohaliyet_annconv-0.2/mohaliyet_annconv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 22:57:38.000000 mohaliyet_annconv-0.2/mohaliyet_annconv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-16 22:57:38.000000 mohaliyet_annconv-0.2/mohaliyet_annconv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 22:57:38.379702 mohaliyet_annconv-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      531 2023-07-16 22:56:31.000000 mohaliyet_annconv-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 22:57:38.375695 mohaliyet_annconv-0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-16 10:15:52.000000 mohaliyet_annconv-0.2/tests/__init__.py
```

### Comparing `mohaliyet_annconv-0.1/annotation_converter/main.py` & `mohaliyet_annconv-0.2/annotation_converter/main.py`

 * *Files identical despite different names*

### Comparing `mohaliyet_annconv-0.1/annotation_converter/parsers.py` & `mohaliyet_annconv-0.2/annotation_converter/parsers.py`

 * *Files identical despite different names*

### Comparing `mohaliyet_annconv-0.1/annotation_converter/writers.py` & `mohaliyet_annconv-0.2/annotation_converter/writers.py`

 * *Files identical despite different names*

### Comparing `mohaliyet_annconv-0.1/setup.py` & `mohaliyet_annconv-0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='mohaliyet_annconv',
-    version='0.1',
+    version='0.2',
     description='A utility for converting object detection annotations between different formats.',
     author='Mohammed Aliy',
     author_email='mohammed@mohaliy.et',
     url='https://www.mohaliy.et',
     packages=find_packages(),
     install_requires=['pillow'],
     entry_points={
         'console_scripts': [
-            'convert_annotations = annotation_converter.main:main',
+            'mohaliyet_annconv = annotation_converter.main:main',
         ],
     },
 )
```

