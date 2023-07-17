# Comparing `tmp/randog-0.5.0.tar.gz` & `tmp/randog-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randog-0.5.0.tar", last modified: Sun Jun 11 03:47:07 2023, max compression
+gzip compressed data, was "randog-0.6.0.tar", last modified: Mon Jul 17 07:03:47 2023, max compression
```

## Comparing `randog-0.5.0.tar` & `randog-0.6.0.tar`

### file list

```diff
@@ -1,44 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:47:07.572332 randog-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-11 03:46:54.000000 randog-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-11 03:47:07.572332 randog-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-11 03:46:54.000000 randog-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:47:07.564332 randog-0.5.0/randog/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-11 03:46:54.000000 randog-0.5.0/randog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-11 03:46:54.000000 randog-0.5.0/randog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-11 03:46:54.000000 randog-0.5.0/randog/_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:47:07.568332 randog-0.5.0/randog/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 03:46:54.000000 randog-0.5.0/randog/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-11 03:46:54.000000 randog-0.5.0/randog/_utils/nullsafe.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-11 03:46:54.000000 randog-0.5.0/randog/_utils/type.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-11 03:46:54.000000 randog-0.5.0/randog/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:47:07.572332 randog-0.5.0/randog/factory/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_by_callable.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_by_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_decimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_float.py
--rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_from_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_from_pyfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_increment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_int.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_timedelta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-11 03:46:54.000000 randog-0.5.0/randog/factory/_union.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:47:07.572332 randog-0.5.0/randog/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-06-11 03:46:54.000000 randog-0.5.0/randog/sqlalchemy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:47:07.568332 randog-0.5.0/randog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-11 03:47:07.000000 randog-0.5.0/randog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-11 03:47:07.000000 randog-0.5.0/randog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 03:47:07.000000 randog-0.5.0/randog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 03:47:07.000000 randog-0.5.0/randog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 03:47:07.572332 randog-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-11 03:46:54.000000 randog-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:47.608795 randog-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-17 07:03:36.000000 randog-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-17 07:03:47.608795 randog-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-17 07:03:36.000000 randog-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:47.604795 randog-0.6.0/randog/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-17 07:03:36.000000 randog-0.6.0/randog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-17 07:03:36.000000 randog-0.6.0/randog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:47.604795 randog-0.6.0/randog/_main/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_main_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:47.604795 randog-0.6.0/randog/_main/_subcmd_def/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_byfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_timedelta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:47.604795 randog-0.6.0/randog/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_utils/nullsafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_utils/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-17 07:03:36.000000 randog-0.6.0/randog/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:47.608795 randog-0.6.0/randog/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_by_callable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_by_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_from_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_from_pyfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_increment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_timedelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_union.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:47.608795 randog-0.6.0/randog/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-17 07:03:36.000000 randog-0.6.0/randog/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-07-17 07:03:36.000000 randog-0.6.0/randog/sqlalchemy/_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-17 07:03:36.000000 randog-0.6.0/randog/sqlalchemy/_custom_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-07-17 07:03:36.000000 randog-0.6.0/randog/timedelta_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:47.604795 randog-0.6.0/randog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-17 07:03:47.000000 randog-0.6.0/randog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-17 07:03:47.000000 randog-0.6.0/randog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 07:03:47.000000 randog-0.6.0/randog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 07:03:47.000000 randog-0.6.0/randog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 07:03:47.608795 randog-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-17 07:03:36.000000 randog-0.6.0/setup.py
```

### Comparing `randog-0.5.0/LICENSE` & `randog-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `randog-0.5.0/PKG-INFO` & `randog-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: randog
-Version: 0.5.0
+Version: 0.6.0
 Summary: Generate data randomly
 Home-page: UNKNOWN
 Author: k-izumi
 Author-email: k.izumi.ysk@gmail.com
 Maintainer: k-izumi
 Maintainer-email: k.izumi.ysk@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/unaguna/random-obj-generator/issues
 Project-URL: Documentation, https://unaguna.github.io/random-obj-generator/
 Project-URL: Source Code, https://github.com/unaguna/random-obj-generator
-Description: **randog 0.5.0 — Randomly object generator**
+Description: **randog 0.6.0 — Randomly object generator**
         
         **randog** is a package which helps to generate data randomly.
         
         ## Install
         
         You can install from PyPI.
```

### Comparing `randog-0.5.0/README.md` & `randog-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-**randog 0.5.0 — Randomly object generator**
+**randog 0.6.0 — Randomly object generator**
 
 **randog** is a package which helps to generate data randomly.
 
 ## Install
 
 You can install from PyPI.
```

### Comparing `randog-0.5.0/randog/_examples.py` & `randog-0.6.0/randog/_examples.py`

 * *Files identical despite different names*

### Comparing `randog-0.5.0/randog/factory/__init__.py` & `randog-0.6.0/randog/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `randog-0.5.0/randog/factory/_base.py` & `randog-0.6.0/randog/factory/_base.py`

 * *Files identical despite different names*

### Comparing `randog-0.5.0/randog/factory/_bool.py` & `randog-0.6.0/randog/factory/_bool.py`

 * *Files identical despite different names*

### Comparing `randog-0.5.0/randog/factory/_by_callable.py` & `randog-0.6.0/randog/factory/_by_callable.py`

 * *Files identical despite different names*

### Comparing `randog-0.5.0/randog/factory/_by_iterator.py` & `randog-0.6.0/randog/factory/_by_iterator.py`

 * *Files identical despite different names*

### Comparing `randog-0.5.0/randog/factory/_choice.py` & `randog-0.6.0/randog/factory/_choice.py`

 * *Files identical despite different names*

### Comparing `randog-0.5.0/randog/factory/_date.py` & `randog-0.6.0/randog/factory/_date.py`

 * *Files identical despite different names*

### Comparing `randog-0.5.0/randog/factory/_datetime.py` & `randog-0.6.0/randog/factory/_datetime.py`

 * *Files identical despite different names*

### Comparing `randog-0.5.0/randog/factory/_decimal.py` & `randog-0.6.0/randog/factory/_decimal.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,11 +100,11 @@
         )
         self._decimal_len = dforc(lambda x: Decimal(1).scaleb(-x), decimal_len)
 
     def next(self) -> Decimal:
         pre_value = self._factory.next()
         value = Decimal(pre_value)
 
-        if self._decimal_len is not None:
+        if self._decimal_len is not None and value.is_finite():
             value = value.quantize(self._decimal_len)
 
         return value
```

### Comparing `randog-0.5.0/randog/factory/_dict.py` & `randog-0.6.0/randog/factory/_dict.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass
 from random import Random
 import typing as t
 
 from ._base import Factory
 from .._utils.nullsafe import dfor
+from ..exceptions import FactoryConstructionError
 
 
 _item_tuple = t.Tuple[Factory, float]
 
 
 @dataclass
 class DictItem:
@@ -40,42 +41,56 @@
         elif len(args) == 1 and isinstance(args[0], tuple):
             self.prop_exists = args[0][1]
             self.factory = args[0][0]
         elif len(args) == 2:
             self.factory = args[0]
             self.prop_exists = args[1]
         else:
-            raise ValueError()
+            raise DictItemValueError()
+
+
+class DictItemValueError(ValueError):
+    pass
 
 
 def randdict(
     items_dict: t.Optional[
         t.Mapping[t.Hashable, t.Union[Factory, _item_tuple, DictItem]]
     ] = None,
     *,
     rnd: t.Optional[Random] = None,
     **items: t.Union[Factory, _item_tuple, DictItem],
-) -> Factory[int]:
+) -> Factory[dict]:
     """Return a factory generating random dict.
 
     Parameters
     ----------
     items : Mapping
         the factories of each key. If `items_dict` is specified, `items` will be ignored.
     items_dict: Mapping
         the factories of each key. Use when keyword arguments cannot be specified.
     rnd : Random, optional
         random number generator to be used
     """
     if items_dict is not None:
         items = items_dict
 
-    items_normalized = {
-        k: v if isinstance(v, DictItem) else DictItem(v) for k, v in items.items()
-    }
+    items_normalized = {}
+    non_factory_item_keys = []
+    for key, value in items.items():
+        try:
+            items_normalized[key] = (
+                value if isinstance(value, DictItem) else DictItem(value)
+            )
+        except DictItemValueError:
+            non_factory_item_keys.append(str(key))
+    if len(non_factory_item_keys) > 0:
+        raise FactoryConstructionError(
+            f"randdict received non-factory object for item: {', '.join(non_factory_item_keys)}"
+        )
 
     return DictRandomFactory(items_normalized, rnd=rnd)
 
 
 class DictRandomFactory(Factory[dict]):
     """factory generating random dict"""
```

### Comparing `randog-0.5.0/randog/factory/_float.py` & `randog-0.6.0/randog/factory/_float.py`

 * *Files identical despite different names*

### Comparing `randog-0.5.0/randog/factory/_from_example.py` & `randog-0.6.0/randog/factory/_from_example.py`

 * *Files identical despite different names*

### Comparing `randog-0.5.0/randog/factory/_from_pyfile.py` & `randog-0.6.0/randog/factory/_from_pyfile.py`

 * *Files identical despite different names*

### Comparing `randog-0.5.0/randog/factory/_increment.py` & `randog-0.6.0/randog/factory/_increment.py`

 * *Files identical despite different names*

### Comparing `randog-0.5.0/randog/factory/_int.py` & `randog-0.6.0/randog/factory/_int.py`

 * *Files identical despite different names*

### Comparing `randog-0.5.0/randog/factory/_list.py` & `randog-0.6.0/randog/factory/_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,14 +78,24 @@
             When the specified generating conditions are inconsistent.
         """
         self._random = dfor(rnd, Random())
         self._length = dfor(length, len(items))
         self._factories = items
         self._type = type
 
+        non_factory_item_indexes = [
+            str(i)
+            for i, factory in enumerate(self._factories)
+            if not isinstance(factory, Factory)
+        ]
+        if len(non_factory_item_indexes) > 0:
+            raise FactoryConstructionError(
+                f"randlist received non-factory object for item: index {', '.join(non_factory_item_indexes)}"
+            )
+
         if isinstance(self._length, Factory) and len(self._factories) == 0:
             raise FactoryConstructionError(
                 "the factory of element must be given to randlist() if length is at random"
             )
         if (
             not isinstance(self._length, Factory)
             and self._length > 0
```

### Comparing `randog-0.5.0/randog/factory/_str.py` & `randog-0.6.0/randog/factory/_str.py`

 * *Files identical despite different names*

### Comparing `randog-0.5.0/randog/factory/_timedelta.py` & `randog-0.6.0/randog/factory/_timedelta.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,21 @@
             random number generator to be used
 
         Raises
         ------
         FactoryConstructionError
             When the specified generating conditions are inconsistent.
         """
-        if unit is not None and unit < dt.timedelta(0):
-            unit = -unit
+        if unit is not None:
+            if unit == dt.timedelta(0):
+                raise FactoryConstructionError(
+                    "the unit for randtimedelta must not be zero"
+                )
+            if unit < dt.timedelta(0):
+                unit = -unit
 
         self._random = dfor(rnd, Random())
         self._min, self._max, self._unit = self._normalize(minimum, maximum, unit)
 
         if self._min > self._max:
             raise FactoryConstructionError("empty range for randtimedelta")
```

### Comparing `randog-0.5.0/randog/factory/_union.py` & `randog-0.6.0/randog/factory/_union.py`

 * *Files identical despite different names*

### Comparing `randog-0.5.0/randog.egg-info/PKG-INFO` & `randog-0.6.0/randog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: randog
-Version: 0.5.0
+Version: 0.6.0
 Summary: Generate data randomly
 Home-page: UNKNOWN
 Author: k-izumi
 Author-email: k.izumi.ysk@gmail.com
 Maintainer: k-izumi
 Maintainer-email: k.izumi.ysk@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/unaguna/random-obj-generator/issues
 Project-URL: Documentation, https://unaguna.github.io/random-obj-generator/
 Project-URL: Source Code, https://github.com/unaguna/random-obj-generator
-Description: **randog 0.5.0 — Randomly object generator**
+Description: **randog 0.6.0 — Randomly object generator**
         
         **randog** is a package which helps to generate data randomly.
         
         ## Install
         
         You can install from PyPI.
```

### Comparing `randog-0.5.0/setup.py` & `randog-0.6.0/setup.py`

 * *Files identical despite different names*

