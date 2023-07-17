# Comparing `tmp/mysqlbuilder-1.0.0.tar.gz` & `tmp/mysqlbuilder-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysqlbuilder-1.0.0.tar", last modified: Mon Jul 17 07:45:24 2023, max compression
+gzip compressed data, was "mysqlbuilder-1.0.1.tar", last modified: Mon Jul 17 11:20:48 2023, max compression
```

## Comparing `mysqlbuilder-1.0.0.tar` & `mysqlbuilder-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 07:45:24.662541 mysqlbuilder-1.0.0/
--rw-rw-rw-   0        0        0     1088 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      365 2023-07-17 07:45:24.661543 mysqlbuilder-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-07-17 03:54:39.000000 mysqlbuilder-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 07:45:24.616673 mysqlbuilder-1.0.0/mysqlbuilder/
--rw-rw-rw-   0        0        0     7275 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.0/mysqlbuilder/Builder.py
--rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.0/mysqlbuilder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:45:24.656555 mysqlbuilder-1.0.0/mysqlbuilder.egg-info/
--rw-rw-rw-   0        0        0      365 2023-07-17 07:45:24.000000 mysqlbuilder-1.0.0/mysqlbuilder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-17 07:45:24.000000 mysqlbuilder-1.0.0/mysqlbuilder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 07:45:24.000000 mysqlbuilder-1.0.0/mysqlbuilder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-17 07:45:24.000000 mysqlbuilder-1.0.0/mysqlbuilder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 07:45:24.662541 mysqlbuilder-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      564 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:45:24.659555 mysqlbuilder-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:20:48.158045 mysqlbuilder-1.0.1/
+-rw-rw-rw-   0        0        0     1088 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     5013 2023-07-17 11:20:48.153572 mysqlbuilder-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4682 2023-07-17 11:07:56.000000 mysqlbuilder-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 11:20:48.062600 mysqlbuilder-1.0.1/mysqlbuilder/
+-rw-rw-rw-   0        0        0     7275 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.1/mysqlbuilder/Builder.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.1/mysqlbuilder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:20:48.146064 mysqlbuilder-1.0.1/mysqlbuilder.egg-info/
+-rw-rw-rw-   0        0        0     5013 2023-07-17 11:20:47.000000 mysqlbuilder-1.0.1/mysqlbuilder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-17 11:20:47.000000 mysqlbuilder-1.0.1/mysqlbuilder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 11:20:47.000000 mysqlbuilder-1.0.1/mysqlbuilder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-17 11:20:47.000000 mysqlbuilder-1.0.1/mysqlbuilder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 11:20:48.159035 mysqlbuilder-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      638 2023-07-17 11:20:05.000000 mysqlbuilder-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:20:48.148952 mysqlbuilder-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.1/tests/__init__.py
```

### Comparing `mysqlbuilder-1.0.0/LICENSE` & `mysqlbuilder-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlbuilder-1.0.0/mysqlbuilder/Builder.py` & `mysqlbuilder-1.0.1/mysqlbuilder/Builder.py`

 * *Files identical despite different names*

### Comparing `mysqlbuilder-1.0.0/setup.py` & `mysqlbuilder-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from setuptools import setup, find_packages
 
+with open('README.md', 'r', encoding='utf-8') as f:
+    long_description = f.read()
+    
 setup(
     name='mysqlbuilder',
-    version='1.0.0',
+    version='1.0.1',
     author='Santu Sarkar',
     author_email='santusarkar2020@gmail.com',
     description='This is a simple mysql builder design to easiy query & get data from your database',
-    long_description='Long description of your package',
+    long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Dip20/mysqlbuilder',
     packages=find_packages(),
     install_requires=[
          # Add any dependencies required by your package
     ]
 )
```

