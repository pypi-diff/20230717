# Comparing `tmp/streamsbpy-1.0.7.tar.gz` & `tmp/streamsbpy-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamsbpy-1.0.7.tar", max compression
+gzip compressed data, was "streamsbpy-1.0.8.tar", max compression
```

## Comparing `streamsbpy-1.0.7.tar` & `streamsbpy-1.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-07-17 04:17:27.050923 streamsbpy-1.0.7/LICENSE
--rw-r--r--   0        0        0      455 2023-07-17 04:49:57.263502 streamsbpy-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      525 2023-07-17 04:17:30.910327 streamsbpy-1.0.7/README.md
--rw-r--r--   0        0        0        1 2023-07-17 04:18:50.945419 streamsbpy-1.0.7/streamsbpy/__init__.py
--rw-r--r--   0        0        0     5512 2023-07-17 04:18:46.902612 streamsbpy-1.0.7/streamsbpy/streamsbpy.py
--rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 streamsbpy-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-17 04:17:27.050923 streamsbpy-1.0.8/LICENSE
+-rw-r--r--   0        0        0      455 2023-07-17 05:03:39.706863 streamsbpy-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      525 2023-07-17 04:17:30.910327 streamsbpy-1.0.8/README.md
+-rw-r--r--   0        0        0       32 2023-07-17 05:02:37.423279 streamsbpy-1.0.8/streamsbpy/__init__.py
+-rw-r--r--   0        0        0     5512 2023-07-17 04:18:46.902612 streamsbpy-1.0.8/streamsbpy/streamsbpy.py
+-rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 streamsbpy-1.0.8/PKG-INFO
```

### Comparing `streamsbpy-1.0.7/LICENSE` & `streamsbpy-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `streamsbpy-1.0.7/README.md` & `streamsbpy-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `streamsbpy-1.0.7/streamsbpy/streamsbpy.py` & `streamsbpy-1.0.8/streamsbpy/streamsbpy.py`

 * *Files identical despite different names*

### Comparing `streamsbpy-1.0.7/PKG-INFO` & `streamsbpy-1.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamsbpy
-Version: 1.0.7
+Version: 1.0.8
 Summary: Interact Using StreamSb API
 Home-page: https://github.com/Code-xed
 License: GNU General Public License 3.0
 Author: Code-xed
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

