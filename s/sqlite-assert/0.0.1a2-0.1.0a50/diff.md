# Comparing `tmp/sqlite_assert-0.0.1a2-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip` & `tmp/sqlite_assert-0.1.0a50-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7557 bytes, number of entries: 8
--rwxr-xr-x  2.0 unx    15784 b- defN 23-Jul-17 01:08 noop.cpython-311-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      307 b- defN 23-Jul-17 01:08 sqlite_assert/__init__.py
--rwxr-xr-x  2.0 unx    16568 b- defN 23-Jul-17 01:08 sqlite_assert/assert0.so
--rw-r--r--  2.0 unx       79 b- defN 23-Jul-17 01:08 sqlite_assert/version.py
--rw-r--r--  2.0 unx      511 b- defN 23-Jul-17 01:08 sqlite_assert-0.0.1a2.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-Jul-17 01:08 sqlite_assert-0.0.1a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-17 01:08 sqlite_assert-0.0.1a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      666 b- defN 23-Jul-17 01:08 sqlite_assert-0.0.1a2.dist-info/RECORD
-8 files, 34039 bytes uncompressed, 6389 bytes compressed:  81.2%
+Zip file size: 7569 bytes, number of entries: 8
+-rwxr-xr-x  2.0 unx    15784 b- defN 23-Jul-17 01:03 noop.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      307 b- defN 23-Jul-17 01:03 sqlite_assert/__init__.py
+-rwxr-xr-x  2.0 unx    16568 b- defN 23-Jul-17 01:03 sqlite_assert/assert0.so
+-rw-r--r--  2.0 unx       80 b- defN 23-Jul-17 01:03 sqlite_assert/version.py
+-rw-r--r--  2.0 unx      512 b- defN 23-Jul-17 01:03 sqlite_assert-0.1.0a50.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-Jul-17 01:03 sqlite_assert-0.1.0a50.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-17 01:03 sqlite_assert-0.1.0a50.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      670 b- defN 23-Jul-17 01:03 sqlite_assert-0.1.0a50.dist-info/RECORD
+8 files, 34045 bytes uncompressed, 6393 bytes compressed:  81.2%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_assert/assert0.so
 Comment: 
 
 Filename: sqlite_assert/version.py
 Comment: 
 
-Filename: sqlite_assert-0.0.1a2.dist-info/METADATA
+Filename: sqlite_assert-0.1.0a50.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_assert-0.0.1a2.dist-info/WHEEL
+Filename: sqlite_assert-0.1.0a50.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_assert-0.0.1a2.dist-info/top_level.txt
+Filename: sqlite_assert-0.1.0a50.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_assert-0.0.1a2.dist-info/RECORD
+Filename: sqlite_assert-0.1.0a50.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_assert/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.0.1-alpha.2"
+__version__ = "0.1.0-alpha.50"
 __version_info__ = tuple(__version__.split("."))
```

