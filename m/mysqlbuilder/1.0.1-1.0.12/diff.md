# Comparing `tmp/mysqlbuilder-1.0.1.tar.gz` & `tmp/mysqlbuilder-1.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysqlbuilder-1.0.1.tar", last modified: Mon Jul 17 11:20:48 2023, max compression
+gzip compressed data, was "mysqlbuilder-1.0.12.tar", last modified: Mon Jul 17 11:44:02 2023, max compression
```

## Comparing `mysqlbuilder-1.0.1.tar` & `mysqlbuilder-1.0.12.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 11:20:48.158045 mysqlbuilder-1.0.1/
--rw-rw-rw-   0        0        0     1088 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     5013 2023-07-17 11:20:48.153572 mysqlbuilder-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4682 2023-07-17 11:07:56.000000 mysqlbuilder-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 11:20:48.062600 mysqlbuilder-1.0.1/mysqlbuilder/
--rw-rw-rw-   0        0        0     7275 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.1/mysqlbuilder/Builder.py
--rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.1/mysqlbuilder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 11:20:48.146064 mysqlbuilder-1.0.1/mysqlbuilder.egg-info/
--rw-rw-rw-   0        0        0     5013 2023-07-17 11:20:47.000000 mysqlbuilder-1.0.1/mysqlbuilder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-17 11:20:47.000000 mysqlbuilder-1.0.1/mysqlbuilder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 11:20:47.000000 mysqlbuilder-1.0.1/mysqlbuilder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-17 11:20:47.000000 mysqlbuilder-1.0.1/mysqlbuilder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 11:20:48.159035 mysqlbuilder-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      638 2023-07-17 11:20:05.000000 mysqlbuilder-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 11:20:48.148952 mysqlbuilder-1.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:44:02.079505 mysqlbuilder-1.0.12/
+-rw-rw-rw-   0        0        0     1088 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.12/LICENSE
+-rw-rw-rw-   0        0        0     5014 2023-07-17 11:44:02.077510 mysqlbuilder-1.0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     4682 2023-07-17 11:07:56.000000 mysqlbuilder-1.0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 11:44:02.029639 mysqlbuilder-1.0.12/mysqlbuilder/
+-rw-rw-rw-   0        0        0     7275 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.12/mysqlbuilder/Builder.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.12/mysqlbuilder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:44:02.072522 mysqlbuilder-1.0.12/mysqlbuilder.egg-info/
+-rw-rw-rw-   0        0        0     5014 2023-07-17 11:44:01.000000 mysqlbuilder-1.0.12/mysqlbuilder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-17 11:44:01.000000 mysqlbuilder-1.0.12/mysqlbuilder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 11:44:01.000000 mysqlbuilder-1.0.12/mysqlbuilder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-17 11:44:01.000000 mysqlbuilder-1.0.12/mysqlbuilder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 11:44:02.080501 mysqlbuilder-1.0.12/setup.cfg
+-rw-rw-rw-   0        0        0      770 2023-07-17 11:43:12.000000 mysqlbuilder-1.0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:44:02.075515 mysqlbuilder-1.0.12/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.12/tests/__init__.py
```

### Comparing `mysqlbuilder-1.0.1/LICENSE` & `mysqlbuilder-1.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlbuilder-1.0.1/PKG-INFO` & `mysqlbuilder-1.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlbuilder
-Version: 1.0.1
+Version: 1.0.12
 Summary: This is a simple mysql builder design to easiy query & get data from your database
 Home-page: https://github.com/Dip20/mysqlbuilder
 Author: Santu Sarkar
 Author-email: santusarkar2020@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mysqlbuilder-1.0.1/README.md` & `mysqlbuilder-1.0.12/README.md`

 * *Files identical despite different names*

### Comparing `mysqlbuilder-1.0.1/mysqlbuilder/Builder.py` & `mysqlbuilder-1.0.12/mysqlbuilder/Builder.py`

 * *Files identical despite different names*

### Comparing `mysqlbuilder-1.0.1/mysqlbuilder.egg-info/PKG-INFO` & `mysqlbuilder-1.0.12/mysqlbuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlbuilder
-Version: 1.0.1
+Version: 1.0.12
 Summary: This is a simple mysql builder design to easiy query & get data from your database
 Home-page: https://github.com/Dip20/mysqlbuilder
 Author: Santu Sarkar
 Author-email: santusarkar2020@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mysqlbuilder-1.0.1/setup.py` & `mysqlbuilder-1.0.12/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
     
+file_path = ".mysqlbuilder.conf"
+
+with open(file_path, 'r', encoding='utf-8') as f:
+    create_config = f.read()
+    
+
+    
 setup(
     name='mysqlbuilder',
-    version='1.0.1',
+    version='1.0.12',
     author='Santu Sarkar',
     author_email='santusarkar2020@gmail.com',
     description='This is a simple mysql builder design to easiy query & get data from your database',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Dip20/mysqlbuilder',
     packages=find_packages(),
```

