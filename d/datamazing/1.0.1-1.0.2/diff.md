# Comparing `tmp/datamazing-1.0.1.tar.gz` & `tmp/datamazing-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamazing-1.0.1.tar", max compression
+gzip compressed data, was "datamazing-1.0.2.tar", max compression
```

## Comparing `datamazing-1.0.1.tar` & `datamazing-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       21 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/__init__.py
--rw-r--r--   0        0        0      277 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/_conform.py
--rw-r--r--   0        0        0      295 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/pandas/__init__.py
--rw-r--r--   0        0        0      267 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/pandas/datacollection/__init__.py
--rw-r--r--   0        0        0      126 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/pandas/testing/__init__.py
--rw-r--r--   0        0        0      766 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/pandas/testing/assertions.py
--rw-r--r--   0        0        0     3818 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/pandas/testing/data.py
--rw-r--r--   0        0        0        0 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/pandas/transformations/__init__.py
--rw-r--r--   0        0        0      649 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/pandas/transformations/basic.py
--rw-r--r--   0        0        0     3353 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/pandas/transformations/grouping.py
--rw-r--r--   0        0        0      868 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/pandas/transformations/resampling.py
--rw-r--r--   0        0        0      660 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/pandas/types.py
--rw-r--r--   0        0        0      184 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/pyspark/__init__.py
--rw-r--r--   0        0        0       92 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/pyspark/testing/__init__.py
--rw-r--r--   0        0        0      295 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/pyspark/testing/assertions.py
--rw-r--r--   0        0        0     2064 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/pyspark/testing/data.py
--rw-r--r--   0        0        0        0 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/pyspark/transformations/__init__.py
--rw-r--r--   0        0        0     1938 2023-07-14 12:01:06.707895 datamazing-1.0.1/datamazing/pyspark/transformations/grouping.py
--rw-r--r--   0        0        0      708 2023-07-14 12:01:06.711895 datamazing-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 datamazing-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       21 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/__init__.py
+-rw-r--r--   0        0        0      277 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/_conform.py
+-rw-r--r--   0        0        0      295 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/__init__.py
+-rw-r--r--   0        0        0      267 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/datacollection/__init__.py
+-rw-r--r--   0        0        0      126 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/testing/__init__.py
+-rw-r--r--   0        0        0      766 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/testing/assertions.py
+-rw-r--r--   0        0        0     3818 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/testing/data.py
+-rw-r--r--   0        0        0        0 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/transformations/__init__.py
+-rw-r--r--   0        0        0      649 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/transformations/basic.py
+-rw-r--r--   0        0        0     3353 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/transformations/grouping.py
+-rw-r--r--   0        0        0      868 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/transformations/resampling.py
+-rw-r--r--   0        0        0      660 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/types.py
+-rw-r--r--   0        0        0      184 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pyspark/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pyspark/testing/__init__.py
+-rw-r--r--   0        0        0      295 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pyspark/testing/assertions.py
+-rw-r--r--   0        0        0     2064 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pyspark/testing/data.py
+-rw-r--r--   0        0        0        0 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pyspark/transformations/__init__.py
+-rw-r--r--   0        0        0     3008 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pyspark/transformations/grouping.py
+-rw-r--r--   0        0        0      708 2023-07-17 11:54:32.142460 datamazing-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 datamazing-1.0.2/PKG-INFO
```

### Comparing `datamazing-1.0.1/datamazing/pandas/testing/assertions.py` & `datamazing-1.0.2/datamazing/pandas/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `datamazing-1.0.1/datamazing/pandas/testing/data.py` & `datamazing-1.0.2/datamazing/pandas/testing/data.py`

 * *Files identical despite different names*

### Comparing `datamazing-1.0.1/datamazing/pandas/transformations/basic.py` & `datamazing-1.0.2/datamazing/pandas/transformations/basic.py`

 * *Files identical despite different names*

### Comparing `datamazing-1.0.1/datamazing/pandas/transformations/grouping.py` & `datamazing-1.0.2/datamazing/pandas/transformations/grouping.py`

 * *Files identical despite different names*

### Comparing `datamazing-1.0.1/datamazing/pandas/transformations/resampling.py` & `datamazing-1.0.2/datamazing/pandas/transformations/resampling.py`

 * *Files identical despite different names*

### Comparing `datamazing-1.0.1/datamazing/pandas/types.py` & `datamazing-1.0.2/datamazing/pandas/types.py`

 * *Files identical despite different names*

### Comparing `datamazing-1.0.1/datamazing/pyspark/testing/data.py` & `datamazing-1.0.2/datamazing/pyspark/testing/data.py`

 * *Files identical despite different names*

### Comparing `datamazing-1.0.1/pyproject.toml` & `datamazing-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datamazing"
-version = "1.0.1"
+version = "1.0.2"
 description = "Package for working with pandas Dataset, but wit specialized functions used for Energinet"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "datamazing" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `datamazing-1.0.1/PKG-INFO` & `datamazing-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamazing
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package for working with pandas Dataset, but wit specialized functions used for Energinet
 Author: Mikkel Ladekarl Folmersen Nygaard
 Author-email: mny@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

