# Comparing `tmp/riptide_db_mysql-0.8.0-py3-none-any.whl.zip` & `tmp/riptide_db_mysql-0.8.0b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5018 bytes, number of entries: 8
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-17 10:41 riptide_db_mysql/__init__.py
--rw-r--r--  2.0 unx     4152 b- defN 23-Jul-17 10:41 riptide_db_mysql/mysql.py
--rw-r--r--  2.0 unx     1070 b- defN 23-Jul-17 10:42 riptide_db_mysql-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4166 b- defN 23-Jul-17 10:42 riptide_db_mysql-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 10:42 riptide_db_mysql-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       65 b- defN 23-Jul-17 10:42 riptide_db_mysql-0.8.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 23-Jul-17 10:42 riptide_db_mysql-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      699 b- defN 23-Jul-17 10:42 riptide_db_mysql-0.8.0.dist-info/RECORD
-8 files, 10261 bytes uncompressed, 3776 bytes compressed:  63.2%
+Zip file size: 5064 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 15:06 riptide_db_mysql/__init__.py
+-rw-r--r--  2.0 unx     4152 b- defN 23-May-24 15:06 riptide_db_mysql/mysql.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-May-24 15:07 riptide_db_mysql-0.8.0b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4235 b- defN 23-May-24 15:07 riptide_db_mysql-0.8.0b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-24 15:07 riptide_db_mysql-0.8.0b1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       65 b- defN 23-May-24 15:07 riptide_db_mysql-0.8.0b1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-May-24 15:07 riptide_db_mysql-0.8.0b1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      711 b- defN 23-May-24 15:07 riptide_db_mysql-0.8.0b1.dist-info/RECORD
+8 files, 10342 bytes uncompressed, 3798 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: riptide_db_mysql/__init__.py
 Comment: 
 
 Filename: riptide_db_mysql/mysql.py
 Comment: 
 
-Filename: riptide_db_mysql-0.8.0.dist-info/LICENSE
+Filename: riptide_db_mysql-0.8.0b1.dist-info/LICENSE
 Comment: 
 
-Filename: riptide_db_mysql-0.8.0.dist-info/METADATA
+Filename: riptide_db_mysql-0.8.0b1.dist-info/METADATA
 Comment: 
 
-Filename: riptide_db_mysql-0.8.0.dist-info/WHEEL
+Filename: riptide_db_mysql-0.8.0b1.dist-info/WHEEL
 Comment: 
 
-Filename: riptide_db_mysql-0.8.0.dist-info/entry_points.txt
+Filename: riptide_db_mysql-0.8.0b1.dist-info/entry_points.txt
 Comment: 
 
-Filename: riptide_db_mysql-0.8.0.dist-info/top_level.txt
+Filename: riptide_db_mysql-0.8.0b1.dist-info/top_level.txt
 Comment: 
 
-Filename: riptide_db_mysql-0.8.0.dist-info/RECORD
+Filename: riptide_db_mysql-0.8.0b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `riptide_db_mysql-0.8.0.dist-info/LICENSE` & `riptide_db_mysql-0.8.0b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `riptide_db_mysql-0.8.0.dist-info/METADATA` & `riptide_db_mysql-0.8.0b1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: riptide-db-mysql
-Version: 0.8.0
+Version: 0.8.0b1
 Summary: Tool to manage development environments for web applications using containers - MySQL Database Drvier
 Home-page: https://github.com/theCapypara/riptide-db-mysql/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: riptide-lib (<0.9,>=0.8.0)
+Requires-Dist: riptide-lib (<0.9,>=0.8.0b1)
 Requires-Dist: schema (>=0.7)
 
 |Riptide|
 =========
 
 .. |Riptide| image:: https://riptide-docs.readthedocs.io/en/latest/_images/logo.png
     :alt: Riptide
@@ -25,14 +25,15 @@
 .. class:: center
 
     ======================  ===================  ===================  ===================
     *Main packages:*        lib_                 proxy_               cli_
     *Container-Backends:*   engine_docker_
     *Database Drivers:*     **db_mysql**         db_mongo_
     *Plugins:*              php_xdebug_
+    *Kubernetes:*           k8s_client_          k8s_controller_
     *Related Projects:*     configcrunch_
     *More:*                 docs_                repo_                docker_images_
     ======================  ===================  ===================  ===================
 
 .. _lib:            https://github.com/theCapypara/riptide-lib
 .. _cli:            https://github.com/theCapypara/riptide-cli
 .. _proxy:          https://github.com/theCapypara/riptide-proxy
```

