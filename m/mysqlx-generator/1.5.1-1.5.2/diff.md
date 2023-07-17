# Comparing `tmp/mysqlx-generator-1.5.1.tar.gz` & `tmp/mysqlx-generator-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-generator-1.5.1.tar", last modified: Thu Jul 13 06:10:12 2023, max compression
+gzip compressed data, was "dist\mysqlx-generator-1.5.2.tar", last modified: Mon Jul 17 15:00:17 2023, max compression
```

## Comparing `mysqlx-generator-1.5.1.tar` & `mysqlx-generator-1.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-generator-1.5.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/mysqlx_generator/
--rw-rw-rw-   0        0        0     1653 2023-07-11 02:11:20.000000 mysqlx-generator-1.5.1/mysqlx_generator/generator.tpl
--rw-rw-rw-   0        0        0     5830 2023-07-11 01:46:17.000000 mysqlx-generator-1.5.1/mysqlx_generator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/mysqlx_generator.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/mysqlx_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-13 05:58:51.000000 mysqlx-generator-1.5.1/mysqlx_generator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2848 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/mysqlx_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/mysqlx_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0      325 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/mysqlx_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/mysqlx_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2848 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     2354 2023-07-13 06:07:01.000000 mysqlx-generator-1.5.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1127 2023-07-13 06:10:05.000000 mysqlx-generator-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/
+drwxrwxrwx   0        0        0        0 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/mysqlx/
+-rw-rw-rw-   0        0        0     5830 2023-07-11 01:46:17.000000 mysqlx-generator-1.5.2/mysqlx/generator.py
+-rw-rw-rw-   0        0        0     1653 2023-07-11 02:11:20.000000 mysqlx-generator-1.5.2/mysqlx/generator.tpl
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-generator-1.5.2/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/mysqlx_generator.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/mysqlx_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/mysqlx_generator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2825 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/mysqlx_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/mysqlx_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      317 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/mysqlx_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/mysqlx_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2825 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2354 2023-07-13 06:07:01.000000 mysqlx-generator-1.5.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-17 15:00:17.000000 mysqlx-generator-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1117 2023-07-17 15:00:10.000000 mysqlx-generator-1.5.2/setup.py
```

### Comparing `mysqlx-generator-1.5.1/mysqlx_generator/generator.tpl` & `mysqlx-generator-1.5.2/mysqlx/generator.tpl`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.5.1/mysqlx_generator/__init__.py` & `mysqlx-generator-1.5.2/mysqlx/generator.py`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.5.1/mysqlx_generator.egg-info/PKG-INFO` & `mysqlx-generator-1.5.2/mysqlx_generator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.5.1
+Version: 1.5.2
 Summary: mysqlx-generator is a model code generator from db tables for MySqlx.
 Home-page: https://gitee.com/summry/mysqlx/blob/master/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 Install
 '''''''
 
 .. code:: shell
 
    pip install mysqlx-generator
```

### Comparing `mysqlx-generator-1.5.1/PKG-INFO` & `mysqlx-generator-1.5.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.5.1
+Version: 1.5.2
 Summary: mysqlx-generator is a model code generator from db tables for MySqlx.
 Home-page: https://gitee.com/summry/mysqlx/blob/master/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 Install
 '''''''
 
 .. code:: shell
 
    pip install mysqlx-generator
```

### Comparing `mysqlx-generator-1.5.1/README.rst` & `mysqlx-generator-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.5.1/setup.py` & `mysqlx-generator-1.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,22 @@
     with open(os.path.join(here, rel_path), 'r', encoding='UTF-8') as fp:
         return fp.read()
 
 long_description = read("README.rst")
 
 setup(
     name='mysqlx-generator',
-    packages=['mysqlx_generator'],
+    packages=['mysqlx'],
     description="mysqlx-generator is a model code generator from db tables for MySqlx.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'mysqlx>=1.3.9',
     ],
-    version='1.5.1',
+    version='1.5.2',
     url='https://gitee.com/summry/mysqlx/blob/master/generator.md',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['MySQL', 'mysqlx', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

