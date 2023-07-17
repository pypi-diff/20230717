# Comparing `tmp/streamsbpy-1.0.5.tar.gz` & `tmp/streamsbpy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamsbpy-1.0.5.tar", max compression
+gzip compressed data, was "streamsbpy-1.0.6.tar", max compression
```

## Comparing `streamsbpy-1.0.5.tar` & `streamsbpy-1.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-07-17 04:17:27.050923 streamsbpy-1.0.5/LICENSE
--rw-r--r--   0        0        0      456 2023-07-17 04:36:29.868344 streamsbpy-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      525 2023-07-17 04:17:30.910327 streamsbpy-1.0.5/README.md
--rw-r--r--   0        0        0        1 2023-07-17 04:18:50.945419 streamsbpy-1.0.5/streamsbpy/__init__.py
--rw-r--r--   0        0        0     5512 2023-07-17 04:18:46.902612 streamsbpy-1.0.5/streamsbpy/streamsbpy.py
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 streamsbpy-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-17 04:17:27.050923 streamsbpy-1.0.6/LICENSE
+-rw-r--r--   0        0        0      455 2023-07-17 04:44:35.485163 streamsbpy-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      525 2023-07-17 04:17:30.910327 streamsbpy-1.0.6/README.md
+-rw-r--r--   0        0        0        1 2023-07-17 04:18:50.945419 streamsbpy-1.0.6/streamsbpy/__init__.py
+-rw-r--r--   0        0        0     5512 2023-07-17 04:18:46.902612 streamsbpy-1.0.6/streamsbpy/streamsbpy.py
+-rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 streamsbpy-1.0.6/PKG-INFO
```

### Comparing `streamsbpy-1.0.5/LICENSE` & `streamsbpy-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `streamsbpy-1.0.5/README.md` & `streamsbpy-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `streamsbpy-1.0.5/streamsbpy/streamsbpy.py` & `streamsbpy-1.0.6/streamsbpy/streamsbpy.py`

 * *Files identical despite different names*

