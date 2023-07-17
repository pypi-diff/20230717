# Comparing `tmp/mysqlbuilder-1.0.18.tar.gz` & `tmp/mysqlbuilder-1.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysqlbuilder-1.0.18.tar", last modified: Mon Jul 17 12:31:21 2023, max compression
+gzip compressed data, was "mysqlbuilder-1.0.19.tar", last modified: Mon Jul 17 12:43:22 2023, max compression
```

## Comparing `mysqlbuilder-1.0.18.tar` & `mysqlbuilder-1.0.19.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 12:31:21.340090 mysqlbuilder-1.0.18/
--rw-rw-rw-   0        0        0     1088 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.18/LICENSE
--rw-rw-rw-   0        0        0     5014 2023-07-17 12:31:21.339093 mysqlbuilder-1.0.18/PKG-INFO
--rw-rw-rw-   0        0        0     4682 2023-07-17 11:07:56.000000 mysqlbuilder-1.0.18/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 12:31:21.300197 mysqlbuilder-1.0.18/mysqlbuilder/
--rw-rw-rw-   0        0        0     7275 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.18/mysqlbuilder/Builder.py
--rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.18/mysqlbuilder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 12:31:21.332113 mysqlbuilder-1.0.18/mysqlbuilder.egg-info/
--rw-rw-rw-   0        0        0     5014 2023-07-17 12:31:21.000000 mysqlbuilder-1.0.18/mysqlbuilder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-17 12:31:21.000000 mysqlbuilder-1.0.18/mysqlbuilder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 12:31:21.000000 mysqlbuilder-1.0.18/mysqlbuilder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-17 12:31:21.000000 mysqlbuilder-1.0.18/mysqlbuilder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 12:31:21.341094 mysqlbuilder-1.0.18/setup.cfg
--rw-rw-rw-   0        0        0     1521 2023-07-17 12:31:15.000000 mysqlbuilder-1.0.18/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 12:31:21.337098 mysqlbuilder-1.0.18/tests/
--rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.18/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:43:22.229813 mysqlbuilder-1.0.19/
+-rw-rw-rw-   0        0        0     1088 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.19/LICENSE
+-rw-rw-rw-   0        0        0     5014 2023-07-17 12:43:22.228816 mysqlbuilder-1.0.19/PKG-INFO
+-rw-rw-rw-   0        0        0     4682 2023-07-17 11:07:56.000000 mysqlbuilder-1.0.19/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 12:43:22.171689 mysqlbuilder-1.0.19/mysqlbuilder/
+-rw-rw-rw-   0        0        0     7275 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.19/mysqlbuilder/Builder.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.19/mysqlbuilder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:43:22.219611 mysqlbuilder-1.0.19/mysqlbuilder.egg-info/
+-rw-rw-rw-   0        0        0     5014 2023-07-17 12:43:21.000000 mysqlbuilder-1.0.19/mysqlbuilder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-17 12:43:22.000000 mysqlbuilder-1.0.19/mysqlbuilder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 12:43:21.000000 mysqlbuilder-1.0.19/mysqlbuilder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-17 12:43:21.000000 mysqlbuilder-1.0.19/mysqlbuilder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 12:43:22.229813 mysqlbuilder-1.0.19/setup.cfg
+-rw-rw-rw-   0        0        0     1521 2023-07-17 12:43:18.000000 mysqlbuilder-1.0.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:43:22.225824 mysqlbuilder-1.0.19/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.19/tests/__init__.py
```

### Comparing `mysqlbuilder-1.0.18/LICENSE` & `mysqlbuilder-1.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlbuilder-1.0.18/PKG-INFO` & `mysqlbuilder-1.0.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlbuilder
-Version: 1.0.18
+Version: 1.0.19
 Summary: This is a simple mysql builder design to easiy query & get data from your database
 Home-page: https://github.com/Dip20/mysqlbuilder
 Author: Santu Sarkar
 Author-email: santusarkar2020@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mysqlbuilder-1.0.18/README.md` & `mysqlbuilder-1.0.19/README.md`

 * *Files identical despite different names*

### Comparing `mysqlbuilder-1.0.18/mysqlbuilder/Builder.py` & `mysqlbuilder-1.0.19/mysqlbuilder/Builder.py`

 * *Files identical despite different names*

### Comparing `mysqlbuilder-1.0.18/mysqlbuilder.egg-info/PKG-INFO` & `mysqlbuilder-1.0.19/mysqlbuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlbuilder
-Version: 1.0.18
+Version: 1.0.19
 Summary: This is a simple mysql builder design to easiy query & get data from your database
 Home-page: https://github.com/Dip20/mysqlbuilder
 Author: Santu Sarkar
 Author-email: santusarkar2020@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mysqlbuilder-1.0.18/setup.py` & `mysqlbuilder-1.0.19/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             file.write('MYSQL_DEFAULT_DATABASE = "your_database_name" \n MYSQL_USERNAME = "root" \n MYSQL_PASSWORD = ""')
     
         # os.mkdir('test_path')
                 
                 
 setup(
     name='mysqlbuilder',
-    version='1.0.18',
+    version='1.0.19',
     author='Santu Sarkar',
     author_email='santusarkar2020@gmail.com',
     description='This is a simple mysql builder design to easiy query & get data from your database',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Dip20/mysqlbuilder',
     packages=find_packages(),
```

