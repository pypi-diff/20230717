# Comparing `tmp/json-any-2023.6.tar.gz` & `tmp/json-any-2023.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-any-2023.6.tar", last modified: Thu Jul 13 17:07:40 2023, max compression
+gzip compressed data, was "json-any-2023.7.tar", last modified: Mon Jul 17 09:52:06 2023, max compression
```

## Comparing `json-any-2023.6.tar` & `json-any-2023.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 17:07:40.539948 json-any-2023.6/
--rw-r--r--   0 eric      (1000) users      (984)      109 2022-07-04 12:52:08.000000 json-any-2023.6/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-13 17:07:40.539948 json-any-2023.6/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json-any-2023.6/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     3458 2022-07-04 09:18:29.000000 json-any-2023.6/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 17:07:40.536614 json-any-2023.6/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 17:07:40.536614 json-any-2023.6/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1854 2022-07-05 06:50:56.000000 json-any-2023.6/documentation/wiki/description.asciidoc
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 17:07:40.536614 json-any-2023.6/json_any/
--rw-r--r--   0 eric      (1000) users      (984)     1749 2023-07-13 12:47:03.000000 json-any-2023.6/json_any/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 17:07:40.539948 json-any-2023.6/json_any/catalog/
--rw-r--r--   0 eric      (1000) users      (984)     2192 2023-07-10 12:59:03.000000 json-any-2023.6/json_any/catalog/module.py
--rw-r--r--   0 eric      (1000) users      (984)     4964 2023-07-13 14:00:49.000000 json-any-2023.6/json_any/catalog/type.py
--rw-r--r--   0 eric      (1000) users      (984)     1892 2023-07-13 12:46:11.000000 json-any-2023.6/json_any/constant.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 17:07:40.539948 json-any-2023.6/json_any/extension/
--rw-r--r--   0 eric      (1000) users      (984)     2417 2023-07-13 15:36:06.000000 json-any-2023.6/json_any/extension/module.py
--rw-r--r--   0 eric      (1000) users      (984)     8143 2023-07-13 13:13:57.000000 json-any-2023.6/json_any/extension/numpy.py
--rw-r--r--   0 eric      (1000) users      (984)     3671 2023-07-13 15:38:58.000000 json-any-2023.6/json_any/extension/type.py
--rw-r--r--   0 eric      (1000) users      (984)    11552 2023-07-13 14:17:27.000000 json-any-2023.6/json_any/json_to_object.py
--rw-r--r--   0 eric      (1000) users      (984)    12704 2023-07-13 15:16:14.000000 json-any-2023.6/json_any/object_to_json.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 17:07:40.539948 json-any-2023.6/json_any/task/
--rw-r--r--   0 eric      (1000) users      (984)     3300 2023-07-13 17:01:02.000000 json-any-2023.6/json_any/task/compression.py
--rw-r--r--   0 eric      (1000) users      (984)     5049 2023-07-13 16:38:45.000000 json-any-2023.6/json_any/task/storage.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-13 17:05:36.000000 json-any-2023.6/json_any/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 17:07:40.539948 json-any-2023.6/json_any.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-13 17:07:40.000000 json-any-2023.6/json_any.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      544 2023-07-13 17:07:40.000000 json-any-2023.6/json_any.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-13 17:07:40.000000 json-any-2023.6/json_any.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)        9 2023-07-13 17:07:40.000000 json-any-2023.6/json_any.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json-any-2023.6/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-13 17:07:40.539948 json-any-2023.6/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     5320 2023-07-13 15:24:10.000000 json-any-2023.6/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-17 09:52:06.954990 json-any-2023.7/
+-rw-r--r--   0 eric      (1000) users      (984)      109 2022-07-04 12:52:08.000000 json-any-2023.7/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-17 09:52:06.954990 json-any-2023.7/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json-any-2023.7/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)     3458 2022-07-04 09:18:29.000000 json-any-2023.7/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-17 09:52:06.948323 json-any-2023.7/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-17 09:52:06.951656 json-any-2023.7/documentation/wiki/
+-rw-r--r--   0 eric      (1000) users      (984)     1854 2022-07-05 06:50:56.000000 json-any-2023.7/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-17 09:52:06.951656 json-any-2023.7/json_any/
+-rw-r--r--   0 eric      (1000) users      (984)     1749 2023-07-13 12:47:03.000000 json-any-2023.7/json_any/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-17 09:52:06.951656 json-any-2023.7/json_any/catalog/
+-rw-r--r--   0 eric      (1000) users      (984)     2192 2023-07-10 12:59:03.000000 json-any-2023.7/json_any/catalog/module.py
+-rw-r--r--   0 eric      (1000) users      (984)     4964 2023-07-13 14:00:49.000000 json-any-2023.7/json_any/catalog/type.py
+-rw-r--r--   0 eric      (1000) users      (984)     1892 2023-07-13 12:46:11.000000 json-any-2023.7/json_any/constant.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-17 09:52:06.951656 json-any-2023.7/json_any/extension/
+-rw-r--r--   0 eric      (1000) users      (984)     2417 2023-07-13 15:36:06.000000 json-any-2023.7/json_any/extension/module.py
+-rw-r--r--   0 eric      (1000) users      (984)     8143 2023-07-13 13:13:57.000000 json-any-2023.7/json_any/extension/numpy.py
+-rw-r--r--   0 eric      (1000) users      (984)     3671 2023-07-13 15:38:58.000000 json-any-2023.7/json_any/extension/type.py
+-rw-r--r--   0 eric      (1000) users      (984)    11552 2023-07-13 14:17:27.000000 json-any-2023.7/json_any/json_to_object.py
+-rw-r--r--   0 eric      (1000) users      (984)    12704 2023-07-13 15:16:14.000000 json-any-2023.7/json_any/object_to_json.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-17 09:52:06.954990 json-any-2023.7/json_any/task/
+-rw-r--r--   0 eric      (1000) users      (984)     3348 2023-07-17 07:04:05.000000 json-any-2023.7/json_any/task/compression.py
+-rw-r--r--   0 eric      (1000) users      (984)     8258 2023-07-17 09:48:29.000000 json-any-2023.7/json_any/task/storage.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-17 09:49:52.000000 json-any-2023.7/json_any/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-17 09:52:06.951656 json-any-2023.7/json_any.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-17 09:52:06.000000 json-any-2023.7/json_any.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      544 2023-07-17 09:52:06.000000 json-any-2023.7/json_any.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-17 09:52:06.000000 json-any-2023.7/json_any.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)        9 2023-07-17 09:52:06.000000 json-any-2023.7/json_any.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json-any-2023.7/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-17 09:52:06.954990 json-any-2023.7/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     5320 2023-07-13 15:24:10.000000 json-any-2023.7/setup.py
```

### Comparing `json-any-2023.6/PKG-INFO` & `json-any-2023.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-any
-Version: 2023.6
+Version: 2023.7
 Summary: JSON and unJSON objects of any type
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/json-any/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/json-any//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/json-any/
```

### Comparing `json-any-2023.6/README-LICENCE-utf8.txt` & `json-any-2023.7/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `json-any-2023.6/README.rst` & `json-any-2023.7/README.rst`

 * *Files identical despite different names*

### Comparing `json-any-2023.6/documentation/wiki/description.asciidoc` & `json-any-2023.7/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `json-any-2023.6/json_any/__init__.py` & `json-any-2023.7/json_any/__init__.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.6/json_any/catalog/module.py` & `json-any-2023.7/json_any/catalog/module.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.6/json_any/catalog/type.py` & `json-any-2023.7/json_any/catalog/type.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.6/json_any/constant.py` & `json-any-2023.7/json_any/constant.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.6/json_any/extension/module.py` & `json-any-2023.7/json_any/extension/module.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.6/json_any/extension/numpy.py` & `json-any-2023.7/json_any/extension/numpy.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.6/json_any/extension/type.py` & `json-any-2023.7/json_any/extension/type.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.6/json_any/json_to_object.py` & `json-any-2023.7/json_any/json_to_object.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.6/json_any/object_to_json.py` & `json-any-2023.7/json_any/object_to_json.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.6/json_any/task/compression.py` & `json-any-2023.7/json_any/task/compression.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,16 @@
 ) -> bytes:
     """"""
     if isinstance(compressor, str):
         if compressor in STANDARD_COMPRESSOR_MODULES:
             Compressed, _ = ElementInModule(STANDARD_COMPRESSOR, compressor)
             if Compressed is None:
                 raise ImportError(
-                    f'{compressor}: Module not importable, or has no "{STANDARD_COMPRESSOR}" function.'
+                    f"{compressor}: Module not importable, "
+                    f'or has no "{STANDARD_COMPRESSOR}" function.'
                 )
         else:
             raise ValueError(f"{compressor}: Unhandled compression module.")
     else:
         Compressed = compressor
 
     return Compressed(jsoned.encode(), *args, **kwargs)
@@ -70,15 +71,16 @@
 ) -> str:
     """"""
     if isinstance(decompressor, str):
         if decompressor in STANDARD_COMPRESSOR_MODULES:
             Decompressed, _ = ElementInModule(STANDARD_DECOMPRESSOR, decompressor)
             if Decompressed is None:
                 raise ImportError(
-                    f'{decompressor}: Module not importable, or has no "{STANDARD_DECOMPRESSOR}" function.'
+                    f"{decompressor}: Module not importable, "
+                    f'or has no "{STANDARD_DECOMPRESSOR}" function.'
                 )
         else:
             raise ValueError(f"{decompressor}: Unhandled compression module.")
     else:
         Decompressed = decompressor
 
     decompressed = Decompressed(compressed, *args, **kwargs)
```

### Comparing `json-any-2023.6/json_any/version.py` & `json-any-2023.7/json_any/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2023.6"
+__version__ = "2023.7"
```

### Comparing `json-any-2023.6/json_any.egg-info/PKG-INFO` & `json-any-2023.7/json_any.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-any
-Version: 2023.6
+Version: 2023.7
 Summary: JSON and unJSON objects of any type
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/json-any/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/json-any//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/json-any/
```

### Comparing `json-any-2023.6/json_any.egg-info/SOURCES.txt` & `json-any-2023.7/json_any.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json-any-2023.6/setup.py` & `json-any-2023.7/setup.py`

 * *Files identical despite different names*

