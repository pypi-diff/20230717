# Comparing `tmp/qrlew_datasets-0.2.1.tar.gz` & `tmp/qrlew_datasets-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrlew_datasets-0.2.1.tar", max compression
+gzip compressed data, was "qrlew_datasets-0.2.2.tar", max compression
```

## Comparing `qrlew_datasets-0.2.1.tar` & `qrlew_datasets-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-07-16 21:50:26.623518 qrlew_datasets-0.2.1/LICENSE
--rw-r--r--   0        0        0      287 2023-07-16 21:50:26.623518 qrlew_datasets-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-07-16 21:50:26.623518 qrlew_datasets-0.2.1/datasets/__init__.py
--rw-r--r--   0        0        0      449 2023-07-16 21:50:26.623518 qrlew_datasets-0.2.1/datasets/build.py
--rw-r--r--   0        0        0     2994 2023-07-16 21:50:26.623518 qrlew_datasets-0.2.1/datasets/database.py
--rw-r--r--   0        0        0       99 2023-07-16 21:50:26.623518 qrlew_datasets-0.2.1/datasets/databases/__init__.py
--rw-r--r--   0        0        0     3148 2023-07-16 21:50:26.623518 qrlew_datasets-0.2.1/datasets/databases/mariadb.py
--rw-r--r--   0        0        0     3365 2023-07-16 21:50:26.623518 qrlew_datasets-0.2.1/datasets/databases/postgresql.py
--rw-r--r--   0        0        0      212 2023-07-16 21:50:26.623518 qrlew_datasets-0.2.1/datasets/network.py
--rw-r--r--   0        0        0      179 2023-07-16 21:50:26.623518 qrlew_datasets-0.2.1/datasets/sources/__init__.py
--rw-r--r--   0        0        0      204 2023-07-16 21:50:26.623518 qrlew_datasets-0.2.1/datasets/sources/financial/__init__.py
--rw-r--r--   0        0        0      133 2023-07-16 21:50:27.199520 qrlew_datasets-0.2.1/datasets/sources/financial/financial.sql
--rw-r--r--   0        0        0      131 2023-07-16 21:50:27.199520 qrlew_datasets-0.2.1/datasets/sources/hepatitis/Hepatitis_std.sql
--rw-r--r--   0        0        0      208 2023-07-16 21:50:27.199520 qrlew_datasets-0.2.1/datasets/sources/hepatitis/__init__.py
--rw-r--r--   0        0        0      198 2023-07-16 21:50:27.199520 qrlew_datasets-0.2.1/datasets/sources/imdb/__init__.py
--rw-r--r--   0        0        0      134 2023-07-16 21:50:27.199520 qrlew_datasets-0.2.1/datasets/sources/imdb/imdb_ijs.sql
--rw-r--r--   0        0        0      744 2023-07-16 21:50:27.199520 qrlew_datasets-0.2.1/datasets/sources/loader.py
--rw-r--r--   0        0        0      551 2023-07-16 21:50:27.199520 qrlew_datasets-0.2.1/datasets/sources/relational_dataset_repository.py
--rw-r--r--   0        0        0      501 2023-07-16 21:50:27.199520 qrlew_datasets-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 qrlew_datasets-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-17 06:36:47.770057 qrlew_datasets-0.2.2/LICENSE
+-rw-r--r--   0        0        0      287 2023-07-17 06:36:47.770057 qrlew_datasets-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-17 06:36:47.770057 qrlew_datasets-0.2.2/datasets/__init__.py
+-rw-r--r--   0        0        0      449 2023-07-17 06:36:47.770057 qrlew_datasets-0.2.2/datasets/build.py
+-rw-r--r--   0        0        0     2994 2023-07-17 06:36:47.770057 qrlew_datasets-0.2.2/datasets/database.py
+-rw-r--r--   0        0        0       99 2023-07-17 06:36:47.770057 qrlew_datasets-0.2.2/datasets/databases/__init__.py
+-rw-r--r--   0        0        0     3148 2023-07-17 06:36:47.770057 qrlew_datasets-0.2.2/datasets/databases/mariadb.py
+-rw-r--r--   0        0        0     3365 2023-07-17 06:36:47.770057 qrlew_datasets-0.2.2/datasets/databases/postgresql.py
+-rw-r--r--   0        0        0      212 2023-07-17 06:36:47.770057 qrlew_datasets-0.2.2/datasets/network.py
+-rw-r--r--   0        0        0      179 2023-07-17 06:36:47.770057 qrlew_datasets-0.2.2/datasets/sources/__init__.py
+-rw-r--r--   0        0        0      204 2023-07-17 06:36:47.770057 qrlew_datasets-0.2.2/datasets/sources/financial/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-17 06:36:49.414046 qrlew_datasets-0.2.2/datasets/sources/financial/financial.sql
+-rw-r--r--   0        0        0      131 2023-07-17 06:36:49.414046 qrlew_datasets-0.2.2/datasets/sources/hepatitis/Hepatitis_std.sql
+-rw-r--r--   0        0        0      208 2023-07-17 06:36:49.418046 qrlew_datasets-0.2.2/datasets/sources/hepatitis/__init__.py
+-rw-r--r--   0        0        0      198 2023-07-17 06:36:49.418046 qrlew_datasets-0.2.2/datasets/sources/imdb/__init__.py
+-rw-r--r--   0        0        0      134 2023-07-17 06:36:49.418046 qrlew_datasets-0.2.2/datasets/sources/imdb/imdb_ijs.sql
+-rw-r--r--   0        0        0      744 2023-07-17 06:36:49.418046 qrlew_datasets-0.2.2/datasets/sources/loader.py
+-rw-r--r--   0        0        0      551 2023-07-17 06:36:49.418046 qrlew_datasets-0.2.2/datasets/sources/relational_dataset_repository.py
+-rw-r--r--   0        0        0      501 2023-07-17 06:36:49.418046 qrlew_datasets-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 qrlew_datasets-0.2.2/PKG-INFO
```

### Comparing `qrlew_datasets-0.2.1/LICENSE` & `qrlew_datasets-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qrlew_datasets-0.2.1/datasets/database.py` & `qrlew_datasets-0.2.2/datasets/database.py`

 * *Files identical despite different names*

### Comparing `qrlew_datasets-0.2.1/datasets/databases/mariadb.py` & `qrlew_datasets-0.2.2/datasets/databases/mariadb.py`

 * *Files identical despite different names*

### Comparing `qrlew_datasets-0.2.1/datasets/databases/postgresql.py` & `qrlew_datasets-0.2.2/datasets/databases/postgresql.py`

 * *Files identical despite different names*

### Comparing `qrlew_datasets-0.2.1/datasets/sources/loader.py` & `qrlew_datasets-0.2.2/datasets/sources/loader.py`

 * *Files identical despite different names*

### Comparing `qrlew_datasets-0.2.1/datasets/sources/relational_dataset_repository.py` & `qrlew_datasets-0.2.2/datasets/sources/relational_dataset_repository.py`

 * *Files identical despite different names*

### Comparing `qrlew_datasets-0.2.1/PKG-INFO` & `qrlew_datasets-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrlew-datasets
-Version: 0.2.1
+Version: 0.2.2
 Summary: Sample SQL datasets
 License: Apache 2.0
 Author: Nicolas Grislain
 Author-email: ng@sarus.tech
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

