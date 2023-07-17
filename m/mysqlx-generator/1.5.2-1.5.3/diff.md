# Comparing `tmp/mysqlx-generator-1.5.2.tar.gz` & `tmp/mysqlx-generator-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-generator-1.5.2.tar", last modified: Mon Jul 17 15:00:17 2023, max compression
+gzip compressed data, was "dist\mysqlx-generator-1.5.3.tar", last modified: Mon Jul 17 15:11:01 2023, max compression
```

## Comparing `mysqlx-generator-1.5.2.tar` & `mysqlx-generator-1.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/
-drwxrwxrwx   0        0        0        0 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/mysqlx/
--rw-rw-rw-   0        0        0     5830 2023-07-11 01:46:17.000000 mysqlx-generator-1.5.2/mysqlx/generator.py
--rw-rw-rw-   0        0        0     1653 2023-07-11 02:11:20.000000 mysqlx-generator-1.5.2/mysqlx/generator.tpl
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-generator-1.5.2/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/mysqlx_generator.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/mysqlx_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/mysqlx_generator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2825 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/mysqlx_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/mysqlx_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0      317 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/mysqlx_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/mysqlx_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2825 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     2354 2023-07-13 06:07:01.000000 mysqlx-generator-1.5.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1117 2023-07-17 15:00:10.000000 mysqlx-generator-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/
+drwxrwxrwx   0        0        0        0 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/mysqlx/
+-rw-rw-rw-   0        0        0     5830 2023-07-11 01:46:17.000000 mysqlx-generator-1.5.3/mysqlx/generator.py
+-rw-rw-rw-   0        0        0     1653 2023-07-11 02:11:20.000000 mysqlx-generator-1.5.3/mysqlx/generator.tpl
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-generator-1.5.3/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/mysqlx_generator.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/mysqlx_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/mysqlx_generator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2825 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/mysqlx_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/mysqlx_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      317 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/mysqlx_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/mysqlx_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2825 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2354 2023-07-17 15:10:48.000000 mysqlx-generator-1.5.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1117 2023-07-17 15:10:55.000000 mysqlx-generator-1.5.3/setup.py
```

### Comparing `mysqlx-generator-1.5.2/mysqlx/generator.py` & `mysqlx-generator-1.5.3/mysqlx/generator.py`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.5.2/mysqlx/generator.tpl` & `mysqlx-generator-1.5.3/mysqlx/generator.tpl`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.5.2/mysqlx_generator.egg-info/PKG-INFO` & `mysqlx-generator-1.5.3/mysqlx_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.5.2
+Version: 1.5.3
 Summary: mysqlx-generator is a model code generator from db tables for MySqlx.
 Home-page: https://gitee.com/summry/mysqlx/blob/master/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
@@ -19,15 +19,15 @@
    pip install mysqlx-generator
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from mysqlx_generator import Generator
+   from mysqlx.generator import Generator
 
 
    if __name__ == '__main__':
        coder = Generator(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test')
        # you can generate a model class for one table
        coder.generate_with_tables(tables='user', path='models.py')
        # you can generate model classes for tables
```

### Comparing `mysqlx-generator-1.5.2/PKG-INFO` & `mysqlx-generator-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.5.2
+Version: 1.5.3
 Summary: mysqlx-generator is a model code generator from db tables for MySqlx.
 Home-page: https://gitee.com/summry/mysqlx/blob/master/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
@@ -19,15 +19,15 @@
    pip install mysqlx-generator
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from mysqlx_generator import Generator
+   from mysqlx.generator import Generator
 
 
    if __name__ == '__main__':
        coder = Generator(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test')
        # you can generate a model class for one table
        coder.generate_with_tables(tables='user', path='models.py')
        # you can generate model classes for tables
```

### Comparing `mysqlx-generator-1.5.2/README.rst` & `mysqlx-generator-1.5.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
    pip install mysqlx-generator
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from mysqlx_generator import Generator
+   from mysqlx.generator import Generator
 
 
    if __name__ == '__main__':
        coder = Generator(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test')
        # you can generate a model class for one table
        coder.generate_with_tables(tables='user', path='models.py')
        # you can generate model classes for tables
```

### Comparing `mysqlx-generator-1.5.2/setup.py` & `mysqlx-generator-1.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     packages=['mysqlx'],
     description="mysqlx-generator is a model code generator from db tables for MySqlx.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'mysqlx>=1.3.9',
     ],
-    version='1.5.2',
+    version='1.5.3',
     url='https://gitee.com/summry/mysqlx/blob/master/generator.md',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['MySQL', 'mysqlx', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

