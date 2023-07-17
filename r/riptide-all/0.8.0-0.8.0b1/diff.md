# Comparing `tmp/riptide_all-0.8.0-py3-none-any.whl.zip` & `tmp/riptide_all-0.8.0b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3017 bytes, number of entries: 5
--rw-r--r--  2.0 unx     1070 b- defN 23-Jul-17 10:48 riptide_all-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4151 b- defN 23-Jul-17 10:48 riptide_all-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 10:48 riptide_all-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-17 10:48 riptide_all-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      405 b- defN 23-Jul-17 10:48 riptide_all-0.8.0.dist-info/RECORD
-5 files, 5719 bytes uncompressed, 2257 bytes compressed:  60.5%
+Zip file size: 3058 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     1070 b- defN 23-May-24 15:13 riptide_all-0.8.0b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4230 b- defN 23-May-24 15:13 riptide_all-0.8.0b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-24 15:13 riptide_all-0.8.0b1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-24 15:13 riptide_all-0.8.0b1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      415 b- defN 23-May-24 15:13 riptide_all-0.8.0b1.dist-info/RECORD
+5 files, 5808 bytes uncompressed, 2278 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: riptide_all-0.8.0.dist-info/LICENSE
+Filename: riptide_all-0.8.0b1.dist-info/LICENSE
 Comment: 
 
-Filename: riptide_all-0.8.0.dist-info/METADATA
+Filename: riptide_all-0.8.0b1.dist-info/METADATA
 Comment: 
 
-Filename: riptide_all-0.8.0.dist-info/WHEEL
+Filename: riptide_all-0.8.0b1.dist-info/WHEEL
 Comment: 
 
-Filename: riptide_all-0.8.0.dist-info/top_level.txt
+Filename: riptide_all-0.8.0b1.dist-info/top_level.txt
 Comment: 
 
-Filename: riptide_all-0.8.0.dist-info/RECORD
+Filename: riptide_all-0.8.0b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `riptide_all-0.8.0.dist-info/LICENSE` & `riptide_all-0.8.0b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `riptide_all-0.8.0.dist-info/METADATA` & `riptide_all-0.8.0b1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 Metadata-Version: 2.1
 Name: riptide-all
-Version: 0.8.0
+Version: 0.8.0b1
 Summary: Tool to manage development environments for web applications using containers - Meta Package
 Home-page: https://github.com/Parakoopa/riptide-all/
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
-Requires-Dist: riptide-cli (<0.9,>=0.8.0)
-Requires-Dist: riptide-proxy (<0.9,>=0.8.0)
-Requires-Dist: riptide-engine-docker (<0.9,>=0.8.0)
-Requires-Dist: riptide-db-mysql (<0.9,>=0.8.0)
-Requires-Dist: riptide-plugin-php-xdebug (<0.9,>=0.8.0)
+Requires-Dist: riptide-lib (<0.9,>=0.8.0b1)
+Requires-Dist: riptide-cli (<0.9,>=0.8.0b1)
+Requires-Dist: riptide-proxy (<0.9,>=0.8.0b1)
+Requires-Dist: riptide-engine-docker (<0.9,>=0.8.0b1)
+Requires-Dist: riptide-db-mysql (<0.9,>=0.8.0b1)
+Requires-Dist: riptide-plugin-php-xdebug (<0.9,>=0.8.0b1)
 
 |Riptide|
 =========
 
 .. |Riptide| image:: https://riptide-docs.readthedocs.io/en/latest/_images/logo.png
     :alt: Riptide
 
 .. class:: center
 
     ======================  ===================  ===================  ===================
     *Main packages:*        lib_                 proxy_               cli_
     *Container-Backends:*   engine_docker_
     *Database Drivers:*     db_mysql_            db_mongo_
     *Plugins:*              php_xdebug_
+    *Kubernetes:*           k8s_client_          k8s_controller_
     *Related Projects:*     configcrunch_
     *More:*                 docs_                repo_                docker_images_
     ======================  ===================  ===================  ===================
 
 .. _lib:            https://github.com/Parakoopa/riptide-lib
 .. _cli:            https://github.com/Parakoopa/riptide-cli
 .. _proxy:          https://github.com/Parakoopa/riptide-proxy
```

