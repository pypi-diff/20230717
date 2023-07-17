# Comparing `tmp/mysqlbuilder-1.0.12.tar.gz` & `tmp/mysqlbuilder-1.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysqlbuilder-1.0.12.tar", last modified: Mon Jul 17 11:44:02 2023, max compression
+gzip compressed data, was "mysqlbuilder-1.0.13.tar", last modified: Mon Jul 17 11:49:33 2023, max compression
```

## Comparing `mysqlbuilder-1.0.12.tar` & `mysqlbuilder-1.0.13.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 11:44:02.079505 mysqlbuilder-1.0.12/
--rw-rw-rw-   0        0        0     1088 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.12/LICENSE
--rw-rw-rw-   0        0        0     5014 2023-07-17 11:44:02.077510 mysqlbuilder-1.0.12/PKG-INFO
--rw-rw-rw-   0        0        0     4682 2023-07-17 11:07:56.000000 mysqlbuilder-1.0.12/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 11:44:02.029639 mysqlbuilder-1.0.12/mysqlbuilder/
--rw-rw-rw-   0        0        0     7275 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.12/mysqlbuilder/Builder.py
--rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.12/mysqlbuilder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 11:44:02.072522 mysqlbuilder-1.0.12/mysqlbuilder.egg-info/
--rw-rw-rw-   0        0        0     5014 2023-07-17 11:44:01.000000 mysqlbuilder-1.0.12/mysqlbuilder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-17 11:44:01.000000 mysqlbuilder-1.0.12/mysqlbuilder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 11:44:01.000000 mysqlbuilder-1.0.12/mysqlbuilder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-17 11:44:01.000000 mysqlbuilder-1.0.12/mysqlbuilder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 11:44:02.080501 mysqlbuilder-1.0.12/setup.cfg
--rw-rw-rw-   0        0        0      770 2023-07-17 11:43:12.000000 mysqlbuilder-1.0.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 11:44:02.075515 mysqlbuilder-1.0.12/tests/
--rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.12/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:49:33.319467 mysqlbuilder-1.0.13/
+-rw-rw-rw-   0        0        0     1088 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.13/LICENSE
+-rw-rw-rw-   0        0        0     5014 2023-07-17 11:49:33.318472 mysqlbuilder-1.0.13/PKG-INFO
+-rw-rw-rw-   0        0        0     4682 2023-07-17 11:07:56.000000 mysqlbuilder-1.0.13/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 11:49:33.271596 mysqlbuilder-1.0.13/mysqlbuilder/
+-rw-rw-rw-   0        0        0     7275 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.13/mysqlbuilder/Builder.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.13/mysqlbuilder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:49:33.310490 mysqlbuilder-1.0.13/mysqlbuilder.egg-info/
+-rw-rw-rw-   0        0        0     5014 2023-07-17 11:49:33.000000 mysqlbuilder-1.0.13/mysqlbuilder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-17 11:49:33.000000 mysqlbuilder-1.0.13/mysqlbuilder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 11:49:33.000000 mysqlbuilder-1.0.13/mysqlbuilder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-17 11:49:33.000000 mysqlbuilder-1.0.13/mysqlbuilder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 11:49:33.321470 mysqlbuilder-1.0.13/setup.cfg
+-rw-rw-rw-   0        0        0      821 2023-07-17 11:49:20.000000 mysqlbuilder-1.0.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:49:33.316475 mysqlbuilder-1.0.13/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-17 03:53:20.000000 mysqlbuilder-1.0.13/tests/__init__.py
```

### Comparing `mysqlbuilder-1.0.12/LICENSE` & `mysqlbuilder-1.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlbuilder-1.0.12/PKG-INFO` & `mysqlbuilder-1.0.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlbuilder
-Version: 1.0.12
+Version: 1.0.13
 Summary: This is a simple mysql builder design to easiy query & get data from your database
 Home-page: https://github.com/Dip20/mysqlbuilder
 Author: Santu Sarkar
 Author-email: santusarkar2020@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mysqlbuilder-1.0.12/README.md` & `mysqlbuilder-1.0.13/README.md`

 * *Files identical despite different names*

### Comparing `mysqlbuilder-1.0.12/mysqlbuilder/Builder.py` & `mysqlbuilder-1.0.13/mysqlbuilder/Builder.py`

 * *Files identical despite different names*

### Comparing `mysqlbuilder-1.0.12/mysqlbuilder.egg-info/PKG-INFO` & `mysqlbuilder-1.0.13/mysqlbuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlbuilder
-Version: 1.0.12
+Version: 1.0.13
 Summary: This is a simple mysql builder design to easiy query & get data from your database
 Home-page: https://github.com/Dip20/mysqlbuilder
 Author: Santu Sarkar
 Author-email: santusarkar2020@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

