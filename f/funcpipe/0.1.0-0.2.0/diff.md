# Comparing `tmp/funcpipe-0.1.0.tar.gz` & `tmp/funcpipe-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcpipe-0.1.0.tar", max compression
+gzip compressed data, was "funcpipe-0.2.0.tar", max compression
```

## Comparing `funcpipe-0.1.0.tar` & `funcpipe-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-06-23 01:49:48.183047 funcpipe-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-06-23 01:39:02.443200 funcpipe-0.1.0/README.md
--rw-r--r--   0        0        0      455 2023-06-23 01:39:34.523193 funcpipe-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      849 2023-06-23 01:47:16.393082 funcpipe-0.1.0/src/funcpipe/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 02:02:17.352870 funcpipe-0.1.0/src/funcpipe/py.typed
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 funcpipe-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-17 14:07:59.170576 funcpipe-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-17 14:07:59.170576 funcpipe-0.2.0/README.md
+-rw-r--r--   0        0        0      455 2023-07-17 14:09:49.640603 funcpipe-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1326 2023-07-17 14:08:25.020584 funcpipe-0.2.0/src/funcpipe/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 14:07:59.170576 funcpipe-0.2.0/src/funcpipe/py.typed
+-rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 funcpipe-0.2.0/PKG-INFO
```

### Comparing `funcpipe-0.1.0/LICENSE` & `funcpipe-0.2.0/LICENSE`

 * *Files identical despite different names*

