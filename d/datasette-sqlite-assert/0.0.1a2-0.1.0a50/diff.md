# Comparing `tmp/datasette_sqlite_assert-0.0.1a2-py3-none-any.whl.zip` & `tmp/datasette_sqlite_assert-0.1.0a50-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2211 bytes, number of entries: 7
--rw-r--r--  2.0 unx      272 b- defN 23-Jul-17 01:08 datasette_sqlite_assert/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Jul-17 01:08 datasette_sqlite_assert/version.py
--rw-r--r--  2.0 unx      575 b- defN 23-Jul-17 01:08 datasette_sqlite_assert-0.0.1a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 01:08 datasette_sqlite_assert-0.0.1a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jul-17 01:08 datasette_sqlite_assert-0.0.1a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       24 b- defN 23-Jul-17 01:08 datasette_sqlite_assert-0.0.1a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      662 b- defN 23-Jul-17 01:08 datasette_sqlite_assert-0.0.1a2.dist-info/RECORD
-7 files, 1756 bytes uncompressed, 1003 bytes compressed:  42.9%
+Zip file size: 2223 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      272 b- defN 23-Jul-17 01:03 datasette_sqlite_assert/__init__.py
+-rw-r--r--  2.0 unx       80 b- defN 23-Jul-17 01:03 datasette_sqlite_assert/version.py
+-rw-r--r--  2.0 unx      576 b- defN 23-Jul-17 01:03 datasette_sqlite_assert-0.1.0a50.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 01:03 datasette_sqlite_assert-0.1.0a50.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-17 01:03 datasette_sqlite_assert-0.1.0a50.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       24 b- defN 23-Jul-17 01:03 datasette_sqlite_assert-0.1.0a50.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      667 b- defN 23-Jul-17 01:03 datasette_sqlite_assert-0.1.0a50.dist-info/RECORD
+7 files, 1763 bytes uncompressed, 1005 bytes compressed:  43.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_assert/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_assert/version.py
 Comment: 
 
-Filename: datasette_sqlite_assert-0.0.1a2.dist-info/METADATA
+Filename: datasette_sqlite_assert-0.1.0a50.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_assert-0.0.1a2.dist-info/WHEEL
+Filename: datasette_sqlite_assert-0.1.0a50.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_assert-0.0.1a2.dist-info/entry_points.txt
+Filename: datasette_sqlite_assert-0.1.0a50.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_assert-0.0.1a2.dist-info/top_level.txt
+Filename: datasette_sqlite_assert-0.1.0a50.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_assert-0.0.1a2.dist-info/RECORD
+Filename: datasette_sqlite_assert-0.1.0a50.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_assert/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.0.1-alpha.2"
+__version__ = "0.1.0-alpha.50"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_assert-0.0.1a2.dist-info/METADATA` & `datasette_sqlite_assert-0.1.0a50.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-assert
-Version: 0.0.1a2
+Version: 0.1.0a50
 Home-page: https://github.com/asg017/sqlite-assert
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-assert/issues
 Project-URL: CI, https://github.com/asg017/sqlite-assert/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-assert/releases
 Requires-Python: >=3.6
```

