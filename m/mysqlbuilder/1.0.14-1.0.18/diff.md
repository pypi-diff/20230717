# Comparing `tmp/mysqlbuilder-1.0.14.tar.gz` & `tmp/mysqlbuilder-1.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysqlbuilder-1.0.14.tar", last modified: Mon Jul 17 11:57:07 2023, max compression
+gzip compressed data, was "mysqlbuilder-1.0.18.tar", last modified: Mon Jul 17 12:31:21 2023, max compression
```

## Comparing `mysqlbuilder-1.0.14.tar` & `mysqlbuilder-1.0.18.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 11:57:07.799787 mysqlbuilder-1.0.14/
--rw-rw-rw-   0        0        0     1088 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.14/LICENSE
--rw-rw-rw-   0        0        0     5014 2023-07-17 11:57:07.797797 mysqlbuilder-1.0.14/PKG-INFO
--rw-rw-rw-   0        0        0     4682 2023-07-17 11:07:56.000000 mysqlbuilder-1.0.14/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 11:57:07.764880 mysqlbuilder-1.0.14/mysqlbuilder/
--rw-rw-rw-   0        0        0     7275 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.14/mysqlbuilder/Builder.py
--rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.14/mysqlbuilder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 11:57:07.792805 mysqlbuilder-1.0.14/mysqlbuilder.egg-info/
--rw-rw-rw-   0        0        0     5014 2023-07-17 11:57:07.000000 mysqlbuilder-1.0.14/mysqlbuilder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-17 11:57:07.000000 mysqlbuilder-1.0.14/mysqlbuilder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 11:57:07.000000 mysqlbuilder-1.0.14/mysqlbuilder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-17 11:57:07.000000 mysqlbuilder-1.0.14/mysqlbuilder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 11:57:07.800784 mysqlbuilder-1.0.14/setup.cfg
--rw-rw-rw-   0        0        0     1499 2023-07-17 11:57:00.000000 mysqlbuilder-1.0.14/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 11:57:07.794800 mysqlbuilder-1.0.14/tests/
--rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.14/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:31:21.340090 mysqlbuilder-1.0.18/
+-rw-rw-rw-   0        0        0     1088 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.18/LICENSE
+-rw-rw-rw-   0        0        0     5014 2023-07-17 12:31:21.339093 mysqlbuilder-1.0.18/PKG-INFO
+-rw-rw-rw-   0        0        0     4682 2023-07-17 11:07:56.000000 mysqlbuilder-1.0.18/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 12:31:21.300197 mysqlbuilder-1.0.18/mysqlbuilder/
+-rw-rw-rw-   0        0        0     7275 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.18/mysqlbuilder/Builder.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.18/mysqlbuilder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:31:21.332113 mysqlbuilder-1.0.18/mysqlbuilder.egg-info/
+-rw-rw-rw-   0        0        0     5014 2023-07-17 12:31:21.000000 mysqlbuilder-1.0.18/mysqlbuilder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-17 12:31:21.000000 mysqlbuilder-1.0.18/mysqlbuilder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 12:31:21.000000 mysqlbuilder-1.0.18/mysqlbuilder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-17 12:31:21.000000 mysqlbuilder-1.0.18/mysqlbuilder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 12:31:21.341094 mysqlbuilder-1.0.18/setup.cfg
+-rw-rw-rw-   0        0        0     1521 2023-07-17 12:31:15.000000 mysqlbuilder-1.0.18/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:31:21.337098 mysqlbuilder-1.0.18/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.18/tests/__init__.py
```

### Comparing `mysqlbuilder-1.0.14/LICENSE` & `mysqlbuilder-1.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlbuilder-1.0.14/PKG-INFO` & `mysqlbuilder-1.0.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlbuilder
-Version: 1.0.14
+Version: 1.0.18
 Summary: This is a simple mysql builder design to easiy query & get data from your database
 Home-page: https://github.com/Dip20/mysqlbuilder
 Author: Santu Sarkar
 Author-email: santusarkar2020@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mysqlbuilder-1.0.14/README.md` & `mysqlbuilder-1.0.18/README.md`

 * *Files identical despite different names*

### Comparing `mysqlbuilder-1.0.14/mysqlbuilder/Builder.py` & `mysqlbuilder-1.0.18/mysqlbuilder/Builder.py`

 * *Files identical despite different names*

### Comparing `mysqlbuilder-1.0.14/mysqlbuilder.egg-info/PKG-INFO` & `mysqlbuilder-1.0.18/mysqlbuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlbuilder
-Version: 1.0.14
+Version: 1.0.18
 Summary: This is a simple mysql builder design to easiy query & get data from your database
 Home-page: https://github.com/Dip20/mysqlbuilder
 Author: Santu Sarkar
 Author-email: santusarkar2020@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mysqlbuilder-1.0.14/setup.py` & `mysqlbuilder-1.0.18/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,23 +15,24 @@
         install.run(self)
 
     
         # Get the project's root directory
         project_root = os.path.abspath(os.path.dirname(os.path.dirname(__file__)))
 
         # Create the file in the project's root directory
-        file_path = os.path.join(project_root, '.mysqlbuilder.conf')
+        file_path = os.path.join(project_root, '.mysqlbuilder.confg')
         with open(file_path, 'w') as file:
             file.write('MYSQL_DEFAULT_DATABASE = "your_database_name" \n MYSQL_USERNAME = "root" \n MYSQL_PASSWORD = ""')
-                
+    
+        # os.mkdir('test_path')
                 
                 
 setup(
     name='mysqlbuilder',
-    version='1.0.14',
+    version='1.0.18',
     author='Santu Sarkar',
     author_email='santusarkar2020@gmail.com',
     description='This is a simple mysql builder design to easiy query & get data from your database',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Dip20/mysqlbuilder',
     packages=find_packages(),
```

