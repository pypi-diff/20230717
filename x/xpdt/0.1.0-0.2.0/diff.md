# Comparing `tmp/xpdt-0.1.0.tar.gz` & `tmp/xpdt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpdt-0.1.0.tar", last modified: Sat Jul 15 02:03:13 2023, max compression
+gzip compressed data, was "xpdt-0.2.0.tar", last modified: Mon Jul 17 01:51:02 2023, max compression
```

## Comparing `xpdt-0.1.0.tar` & `xpdt-0.2.0.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-15 02:03:13.487199 xpdt-0.1.0/
--rw-r-----   0 scara     (1000) scara     (1000)    35147 2021-05-22 04:38:57.000000 xpdt-0.1.0/LICENSE.txt
--rw-r-----   0 scara     (1000) scara     (1000)       90 2021-05-22 04:38:57.000000 xpdt-0.1.0/MANIFEST.in
--rw-r-----   0 scara     (1000) scara     (1000)     4166 2023-07-15 02:03:13.487199 xpdt-0.1.0/PKG-INFO
--rw-r-----   0 scara     (1000) scara     (1000)     3178 2023-07-09 09:54:10.000000 xpdt-0.1.0/README.md
-drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-15 02:03:13.482199 xpdt-0.1.0/examples/
--rw-r-----   0 scara     (1000) scara     (1000)      291 2023-07-09 09:54:10.000000 xpdt-0.1.0/examples/example1.xpdt
--rw-r-----   0 scara     (1000) scara     (1000)       79 2023-07-15 02:03:13.487199 xpdt-0.1.0/setup.cfg
--rwxr-x---   0 scara     (1000) scara     (1000)     1600 2023-07-09 09:54:10.000000 xpdt-0.1.0/setup.py
-drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-15 02:03:13.484199 xpdt-0.1.0/test/
--rw-r-----   0 scara     (1000) scara     (1000)     2024 2023-07-09 09:54:10.000000 xpdt-0.1.0/test/test_decode.py
--rw-r-----   0 scara     (1000) scara     (1000)     1167 2023-07-09 09:54:10.000000 xpdt-0.1.0/test/test_enums.py
--rw-r-----   0 scara     (1000) scara     (1000)     1273 2023-07-09 09:54:10.000000 xpdt-0.1.0/test/test_nested.py
--rw-r-----   0 scara     (1000) scara     (1000)     2266 2023-07-09 09:54:10.000000 xpdt-0.1.0/test/test_parser.py
--rw-r-----   0 scara     (1000) scara     (1000)     1597 2023-07-09 09:54:10.000000 xpdt-0.1.0/test/test_roundtrip.py
--rw-r-----   0 scara     (1000) scara     (1000)     2007 2023-07-09 09:54:10.000000 xpdt-0.1.0/test/test_stringy.py
-drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-15 02:03:13.486199 xpdt-0.1.0/xpdt/
--rw-r-----   0 scara     (1000) scara     (1000)      801 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/__init__.py
--rw-r-----   0 scara     (1000) scara     (1000)     3720 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/__main__.py
--rw-r-----   0 scara     (1000) scara     (1000)      282 2023-07-15 02:01:41.000000 xpdt-0.1.0/xpdt/__version__.py
--rw-r-----   0 scara     (1000) scara     (1000)     1477 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/basetypes.py
--rw-r-----   0 scara     (1000) scara     (1000)     1799 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/buftypes.py
--rw-r-----   0 scara     (1000) scara     (1000)      505 2021-05-22 04:38:57.000000 xpdt-0.1.0/xpdt/c.py
--rw-r-----   0 scara     (1000) scara     (1000)      587 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/decl.py
--rw-r-----   0 scara     (1000) scara     (1000)      222 2021-05-26 05:19:37.000000 xpdt-0.1.0/xpdt/dupes.py
--rw-r-----   0 scara     (1000) scara     (1000)     1107 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/integraltype.py
--rw-r-----   0 scara     (1000) scara     (1000)      799 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/intstack.py
--rw-r-----   0 scara     (1000) scara     (1000)     1586 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/jinja.py
--rw-r-----   0 scara     (1000) scara     (1000)     1506 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/lex.py
--rw-r-----   0 scara     (1000) scara     (1000)     2091 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/load.py
--rw-r-----   0 scara     (1000) scara     (1000)      726 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/member.py
--rw-r-----   0 scara     (1000) scara     (1000)     4768 2023-07-09 10:14:27.000000 xpdt-0.1.0/xpdt/namespace.py
--rw-r-----   0 scara     (1000) scara     (1000)     5165 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/parse.py
--rw-r-----   0 scara     (1000) scara     (1000)        0 2021-05-22 04:38:57.000000 xpdt-0.1.0/xpdt/py.typed
--rw-r-----   0 scara     (1000) scara     (1000)     5013 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/registry.py
--rw-r-----   0 scara     (1000) scara     (1000)     2583 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/shiftreduce.py
--rw-r-----   0 scara     (1000) scara     (1000)     7269 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/struct.py
--rw-r-----   0 scara     (1000) scara     (1000)     3078 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/symbology.py
-drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-15 02:03:13.487199 xpdt-0.1.0/xpdt/templates/
--rw-r-----   0 scara     (1000) scara     (1000)        0 2021-05-22 04:38:57.000000 xpdt-0.1.0/xpdt/templates/__init__.py
--rw-r-----   0 scara     (1000) scara     (1000)      664 2023-07-09 10:21:23.000000 xpdt-0.1.0/xpdt/templates/api.c
--rw-r-----   0 scara     (1000) scara     (1000)      385 2023-07-09 09:56:13.000000 xpdt-0.1.0/xpdt/templates/apihdr.c
--rw-r-----   0 scara     (1000) scara     (1000)     2151 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/templates/fixed.pyt
--rw-r-----   0 scara     (1000) scara     (1000)    12735 2023-07-09 10:16:00.000000 xpdt-0.1.0/xpdt/templates/macros.c
--rw-r-----   0 scara     (1000) scara     (1000)     4088 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/templates/vbuf.pyt
--rw-r-----   0 scara     (1000) scara     (1000)     1765 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/templates/xpdt.c
--rw-r-----   0 scara     (1000) scara     (1000)     7750 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/templates/xpdt.pyt
--rw-r-----   0 scara     (1000) scara     (1000)     2434 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/type.py
--rw-r-----   0 scara     (1000) scara     (1000)      150 2021-05-22 04:38:57.000000 xpdt-0.1.0/xpdt/typedef.py
--rw-r-----   0 scara     (1000) scara     (1000)      511 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/uuidtype.py
-drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-15 02:03:13.486199 xpdt-0.1.0/xpdt.egg-info/
--rw-r-----   0 scara     (1000) scara     (1000)     4166 2023-07-15 02:03:13.000000 xpdt-0.1.0/xpdt.egg-info/PKG-INFO
--rw-r-----   0 scara     (1000) scara     (1000)      939 2023-07-15 02:03:13.000000 xpdt-0.1.0/xpdt.egg-info/SOURCES.txt
--rw-r-----   0 scara     (1000) scara     (1000)        1 2023-07-15 02:03:13.000000 xpdt-0.1.0/xpdt.egg-info/dependency_links.txt
--rw-r-----   0 scara     (1000) scara     (1000)       44 2023-07-15 02:03:13.000000 xpdt-0.1.0/xpdt.egg-info/entry_points.txt
--rw-r-----   0 scara     (1000) scara     (1000)       12 2023-07-15 02:03:13.000000 xpdt-0.1.0/xpdt.egg-info/requires.txt
--rw-r-----   0 scara     (1000) scara     (1000)        5 2023-07-15 02:03:13.000000 xpdt-0.1.0/xpdt.egg-info/top_level.txt
+drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-17 01:51:02.871278 xpdt-0.2.0/
+-rw-r-----   0 scara     (1000) scara     (1000)    35147 2021-05-22 04:38:57.000000 xpdt-0.2.0/LICENSE.txt
+-rw-r-----   0 scara     (1000) scara     (1000)       90 2021-05-22 04:38:57.000000 xpdt-0.2.0/MANIFEST.in
+-rw-r-----   0 scara     (1000) scara     (1000)     4166 2023-07-17 01:51:02.871278 xpdt-0.2.0/PKG-INFO
+-rw-r-----   0 scara     (1000) scara     (1000)     3178 2023-07-09 09:54:10.000000 xpdt-0.2.0/README.md
+drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-17 01:51:02.866278 xpdt-0.2.0/examples/
+-rw-r-----   0 scara     (1000) scara     (1000)      291 2023-07-09 09:54:10.000000 xpdt-0.2.0/examples/example1.xpdt
+-rw-r-----   0 scara     (1000) scara     (1000)       79 2023-07-17 01:51:02.871278 xpdt-0.2.0/setup.cfg
+-rwxr-x---   0 scara     (1000) scara     (1000)     1600 2023-07-09 09:54:10.000000 xpdt-0.2.0/setup.py
+drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-17 01:51:02.867278 xpdt-0.2.0/test/
+-rw-r-----   0 scara     (1000) scara     (1000)     2024 2023-07-09 09:54:10.000000 xpdt-0.2.0/test/test_decode.py
+-rw-r-----   0 scara     (1000) scara     (1000)     1167 2023-07-09 09:54:10.000000 xpdt-0.2.0/test/test_enums.py
+-rw-r-----   0 scara     (1000) scara     (1000)     1273 2023-07-09 09:54:10.000000 xpdt-0.2.0/test/test_nested.py
+-rw-r-----   0 scara     (1000) scara     (1000)     2266 2023-07-09 09:54:10.000000 xpdt-0.2.0/test/test_parser.py
+-rw-r-----   0 scara     (1000) scara     (1000)     1597 2023-07-09 09:54:10.000000 xpdt-0.2.0/test/test_roundtrip.py
+-rw-r-----   0 scara     (1000) scara     (1000)     2007 2023-07-09 09:54:10.000000 xpdt-0.2.0/test/test_stringy.py
+drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-17 01:51:02.870278 xpdt-0.2.0/xpdt/
+-rw-r-----   0 scara     (1000) scara     (1000)      801 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/__init__.py
+-rw-r-----   0 scara     (1000) scara     (1000)     4123 2023-07-17 01:50:07.000000 xpdt-0.2.0/xpdt/__main__.py
+-rw-r-----   0 scara     (1000) scara     (1000)      282 2023-07-17 01:50:28.000000 xpdt-0.2.0/xpdt/__version__.py
+-rw-r-----   0 scara     (1000) scara     (1000)     1477 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/basetypes.py
+-rw-r-----   0 scara     (1000) scara     (1000)     1799 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/buftypes.py
+-rw-r-----   0 scara     (1000) scara     (1000)      505 2021-05-22 04:38:57.000000 xpdt-0.2.0/xpdt/c.py
+-rw-r-----   0 scara     (1000) scara     (1000)      587 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/decl.py
+-rw-r-----   0 scara     (1000) scara     (1000)      222 2021-05-26 05:19:37.000000 xpdt-0.2.0/xpdt/dupes.py
+-rw-r-----   0 scara     (1000) scara     (1000)     1107 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/integraltype.py
+-rw-r-----   0 scara     (1000) scara     (1000)      799 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/intstack.py
+-rw-r-----   0 scara     (1000) scara     (1000)     1586 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/jinja.py
+-rw-r-----   0 scara     (1000) scara     (1000)     1506 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/lex.py
+-rw-r-----   0 scara     (1000) scara     (1000)     2091 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/load.py
+-rw-r-----   0 scara     (1000) scara     (1000)      726 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/member.py
+-rw-r-----   0 scara     (1000) scara     (1000)     4768 2023-07-09 10:14:27.000000 xpdt-0.2.0/xpdt/namespace.py
+-rw-r-----   0 scara     (1000) scara     (1000)     5165 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/parse.py
+-rw-r-----   0 scara     (1000) scara     (1000)        0 2021-05-22 04:38:57.000000 xpdt-0.2.0/xpdt/py.typed
+-rw-r-----   0 scara     (1000) scara     (1000)     5013 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/registry.py
+-rw-r-----   0 scara     (1000) scara     (1000)     2583 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/shiftreduce.py
+-rw-r-----   0 scara     (1000) scara     (1000)     7269 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/struct.py
+-rw-r-----   0 scara     (1000) scara     (1000)     3078 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/symbology.py
+drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-17 01:51:02.871278 xpdt-0.2.0/xpdt/templates/
+-rw-r-----   0 scara     (1000) scara     (1000)        0 2021-05-22 04:38:57.000000 xpdt-0.2.0/xpdt/templates/__init__.py
+drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-17 01:51:02.871278 xpdt-0.2.0/xpdt/templates/__pycache__/
+-rw-r-----   0 scara     (1000) scara     (1000)      156 2023-07-15 02:16:14.000000 xpdt-0.2.0/xpdt/templates/__pycache__/__init__.cpython-311.pyc
+-rw-r-----   0 scara     (1000) scara     (1000)      664 2023-07-09 10:21:23.000000 xpdt-0.2.0/xpdt/templates/api.c
+-rw-r-----   0 scara     (1000) scara     (1000)      385 2023-07-09 09:56:13.000000 xpdt-0.2.0/xpdt/templates/apihdr.c
+-rw-r-----   0 scara     (1000) scara     (1000)     2151 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/templates/fixed.pyt
+-rw-r-----   0 scara     (1000) scara     (1000)    12735 2023-07-09 10:16:00.000000 xpdt-0.2.0/xpdt/templates/macros.c
+-rw-r-----   0 scara     (1000) scara     (1000)     4088 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/templates/vbuf.pyt
+-rw-r-----   0 scara     (1000) scara     (1000)     1765 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/templates/xpdt.c
+-rw-r-----   0 scara     (1000) scara     (1000)     7750 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/templates/xpdt.pyt
+-rw-r-----   0 scara     (1000) scara     (1000)     2434 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/type.py
+-rw-r-----   0 scara     (1000) scara     (1000)      150 2021-05-22 04:38:57.000000 xpdt-0.2.0/xpdt/typedef.py
+-rw-r-----   0 scara     (1000) scara     (1000)      511 2023-07-09 09:54:10.000000 xpdt-0.2.0/xpdt/uuidtype.py
+drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-17 01:51:02.870278 xpdt-0.2.0/xpdt.egg-info/
+-rw-r-----   0 scara     (1000) scara     (1000)     4166 2023-07-17 01:51:02.000000 xpdt-0.2.0/xpdt.egg-info/PKG-INFO
+-rw-r-----   0 scara     (1000) scara     (1000)      991 2023-07-17 01:51:02.000000 xpdt-0.2.0/xpdt.egg-info/SOURCES.txt
+-rw-r-----   0 scara     (1000) scara     (1000)        1 2023-07-17 01:51:02.000000 xpdt-0.2.0/xpdt.egg-info/dependency_links.txt
+-rw-r-----   0 scara     (1000) scara     (1000)       44 2023-07-17 01:51:02.000000 xpdt-0.2.0/xpdt.egg-info/entry_points.txt
+-rw-r-----   0 scara     (1000) scara     (1000)       12 2023-07-17 01:51:02.000000 xpdt-0.2.0/xpdt.egg-info/requires.txt
+-rw-r-----   0 scara     (1000) scara     (1000)        5 2023-07-17 01:51:02.000000 xpdt-0.2.0/xpdt.egg-info/top_level.txt
```

### Comparing `xpdt-0.1.0/LICENSE.txt` & `xpdt-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/PKG-INFO` & `xpdt-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpdt
-Version: 0.1.0
+Version: 0.2.0
 Summary: eXPeditious Data Transfer
 Home-page: https://github.com/giannitedesco/xpdt
 Author: Gianni Tedesco
 Author-email: gianni@scaramanga.co.uk
 License: GPLv3
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `xpdt-0.1.0/README.md` & `xpdt-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/setup.py` & `xpdt-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/test/test_decode.py` & `xpdt-0.2.0/test/test_decode.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/test/test_enums.py` & `xpdt-0.2.0/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/test/test_nested.py` & `xpdt-0.2.0/test/test_nested.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/test/test_parser.py` & `xpdt-0.2.0/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/test/test_roundtrip.py` & `xpdt-0.2.0/test/test_roundtrip.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/test/test_stringy.py` & `xpdt-0.2.0/test/test_stringy.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/__init__.py` & `xpdt-0.2.0/xpdt/__init__.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/__main__.py` & `xpdt-0.2.0/xpdt/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,47 +11,55 @@
 _stdio_handler.setFormatter(_fmt)
 _log = logging.getLogger(__package__)
 _log.addHandler(_stdio_handler)
 
 
 class BackendDef:
     suffix: ClassVar[str]
+    incl: ClassVar[bool] = False
 
     __slots__ = (
         '_p',
         '_ns',
         '_inc_prefix',
     )
 
     _p: Path
     _ns: NameSpace
     _inc_prefix: Optional[str]
 
     def _name(self, base: Path, name: str) -> Path:
         return base / (name + self.suffix)
 
-    def __init__(self, ns: NameSpace, base: Path,
+    def __init__(self,
+                 ns: NameSpace,
+                 base: Path,
+                 inc_base: Optional[Path],
                  inc_prefix: Optional[str] = None) -> None:
         self._ns = ns
         name = ns.name
         assert name is not None
-        self._p = self._name(base, name)
+        if self.incl and inc_base is not None:
+            self._p = self._name(inc_base, name)
+        else:
+            self._p = self._name(base, name)
         self._inc_prefix = inc_prefix
 
     def _gen(self, f: TextIO) -> None:
         raise NotImplementedError
 
     def gen(self) -> None:
         _log.info('Writing code: %s', self._p)
         with self._p.open('w') as f:
             return self._gen(f)
 
 
 class OutputC(BackendDef):
     suffix = '_impl.h'
+    incl = True
     __slots__ = ()
 
     def _gen(self, f: TextIO) -> None:
         self._ns.gen_c(f)
 
 
 class OutputCAPI(BackendDef):
@@ -60,14 +68,15 @@
 
     def _gen(self, f: TextIO) -> None:
         self._ns.gen_c_api_entries(f, self._inc_prefix)
 
 
 class OutputCHdr(BackendDef):
     suffix = '_api.h'
+    incl = True
     __slots__ = ()
 
     def _gen(self, f: TextIO) -> None:
         self._ns.gen_c_api_hdr(f)
 
 
 class OutputPy(BackendDef):
@@ -106,14 +115,17 @@
                       default='c',
                       type=str,
                       help='Output language: %s' % ', '.join(backends.keys()))
     opts.add_argument('--out', '-o',
                       default=Path(),
                       type=Path,
                       help='Output dir')
+    opts.add_argument('--inc-dir', '-i',
+                      type=Path,
+                      help='Output dir to write includes')
     opts.add_argument('-I',
                       dest='inc_prefix',
                       help='Include path (for C headers)')
     opts.add_argument('file',
                       type=Path,
                       nargs='+',
                       help='xpdt schema files')
@@ -137,13 +149,13 @@
         file_generators = backends[args.language]
     except KeyError:
         print(f'Unknown language: "{args.language}"')
         raise SystemExit(1)
 
     args.out.mkdir(exist_ok=True)
     for cls in file_generators:
-        backend = cls(ns, args.out, args.inc_prefix)
+        backend = cls(ns, args.out, args.inc_dir, args.inc_prefix)
         backend.gen()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `xpdt-0.1.0/xpdt/basetypes.py` & `xpdt-0.2.0/xpdt/basetypes.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/buftypes.py` & `xpdt-0.2.0/xpdt/buftypes.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/decl.py` & `xpdt-0.2.0/xpdt/decl.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/integraltype.py` & `xpdt-0.2.0/xpdt/integraltype.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/intstack.py` & `xpdt-0.2.0/xpdt/intstack.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/jinja.py` & `xpdt-0.2.0/xpdt/jinja.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/lex.py` & `xpdt-0.2.0/xpdt/lex.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/load.py` & `xpdt-0.2.0/xpdt/load.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/member.py` & `xpdt-0.2.0/xpdt/member.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/namespace.py` & `xpdt-0.2.0/xpdt/namespace.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/parse.py` & `xpdt-0.2.0/xpdt/parse.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/registry.py` & `xpdt-0.2.0/xpdt/registry.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/shiftreduce.py` & `xpdt-0.2.0/xpdt/shiftreduce.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/struct.py` & `xpdt-0.2.0/xpdt/struct.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/symbology.py` & `xpdt-0.2.0/xpdt/symbology.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/templates/api.c` & `xpdt-0.2.0/xpdt/templates/api.c`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/templates/fixed.pyt` & `xpdt-0.2.0/xpdt/templates/fixed.pyt`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/templates/macros.c` & `xpdt-0.2.0/xpdt/templates/macros.c`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/templates/vbuf.pyt` & `xpdt-0.2.0/xpdt/templates/vbuf.pyt`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/templates/xpdt.c` & `xpdt-0.2.0/xpdt/templates/xpdt.c`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/templates/xpdt.pyt` & `xpdt-0.2.0/xpdt/templates/xpdt.pyt`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt/type.py` & `xpdt-0.2.0/xpdt/type.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.1.0/xpdt.egg-info/PKG-INFO` & `xpdt-0.2.0/xpdt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpdt
-Version: 0.1.0
+Version: 0.2.0
 Summary: eXPeditious Data Transfer
 Home-page: https://github.com/giannitedesco/xpdt
 Author: Gianni Tedesco
 Author-email: gianni@scaramanga.co.uk
 License: GPLv3
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `xpdt-0.1.0/xpdt.egg-info/SOURCES.txt` & `xpdt-0.2.0/xpdt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -43,8 +43,9 @@
 xpdt/templates/__init__.py
 xpdt/templates/api.c
 xpdt/templates/apihdr.c
 xpdt/templates/fixed.pyt
 xpdt/templates/macros.c
 xpdt/templates/vbuf.pyt
 xpdt/templates/xpdt.c
-xpdt/templates/xpdt.pyt
+xpdt/templates/xpdt.pyt
+xpdt/templates/__pycache__/__init__.cpython-311.pyc
```

