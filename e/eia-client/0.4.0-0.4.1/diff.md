# Comparing `tmp/eia_client-0.4.0.tar.gz` & `tmp/eia_client-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eia_client-0.4.0.tar", last modified: Wed Jul 12 17:29:57 2023, max compression
+gzip compressed data, was "eia_client-0.4.1.tar", last modified: Mon Jul 17 20:50:45 2023, max compression
```

## Comparing `eia_client-0.4.0.tar` & `eia_client-0.4.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-12 17:29:57.495782 eia_client-0.4.0/
--rw-r--r--   0 te         (501) staff       (20)    11357 2023-02-04 20:51:40.000000 eia_client-0.4.0/LICENSE
--rw-r--r--   0 te         (501) staff       (20)       44 2023-07-12 17:21:42.000000 eia_client-0.4.0/MANIFEST.in
--rw-r--r--   0 te         (501) staff       (20)     2332 2023-07-12 17:29:57.496159 eia_client-0.4.0/PKG-INFO
--rw-r--r--   0 te         (501) staff       (20)     1725 2023-02-14 20:04:30.000000 eia_client-0.4.0/README.md
--rw-r--r--   0 te         (501) staff       (20)      103 2023-02-10 01:33:54.000000 eia_client-0.4.0/README.rst
-drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-12 17:29:57.478025 eia_client-0.4.0/docs/
-drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-12 17:29:57.482954 eia_client-0.4.0/docs/source/
--rw-r--r--   0 te         (501) staff       (20)     1279 2023-02-10 01:33:54.000000 eia_client-0.4.0/docs/source/conf.py
-drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-12 17:29:57.483747 eia_client-0.4.0/examples/
--rw-r--r--   0 te         (501) staff       (20)      398 2023-02-14 20:04:30.000000 eia_client-0.4.0/examples/example_elec_retail_sales.py
--rw-r--r--   0 te         (501) staff       (20)      334 2023-07-12 17:05:45.000000 eia_client-0.4.0/examples/example_total_energy.py
--rw-r--r--   0 te         (501) staff       (20)       96 2023-02-10 01:33:54.000000 eia_client-0.4.0/pyproject.toml
--rw-r--r--   0 te         (501) staff       (20)      948 2023-07-12 17:29:57.498134 eia_client-0.4.0/setup.cfg
-drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-12 17:29:57.478743 eia_client-0.4.0/src/
-drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-12 17:29:57.487354 eia_client-0.4.0/src/eia_client/
--rw-r--r--   0 te         (501) staff       (20)      194 2023-07-12 17:21:42.000000 eia_client-0.4.0/src/eia_client/__init__.py
--rw-r--r--   0 te         (501) staff       (20)     3054 2023-07-12 17:06:55.000000 eia_client-0.4.0/src/eia_client/api_key.py
--rw-r--r--   0 te         (501) staff       (20)     3110 2023-02-14 20:04:30.000000 eia_client-0.4.0/src/eia_client/cli.py
--rw-r--r--   0 te         (501) staff       (20)      828 2023-07-12 17:21:42.000000 eia_client-0.4.0/src/eia_client/client.py
-drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-12 17:29:57.493967 eia_client-0.4.0/src/eia_client/endpoint/
--rw-r--r--   0 te         (501) staff       (20)      174 2023-07-12 17:21:42.000000 eia_client-0.4.0/src/eia_client/endpoint/__init__.py
--rw-r--r--   0 te         (501) staff       (20)     3547 2023-07-12 17:21:42.000000 eia_client-0.4.0/src/eia_client/endpoint/builder.py
--rw-r--r--   0 te         (501) staff       (20)     2412 2023-07-12 17:21:42.000000 eia_client-0.4.0/src/eia_client/endpoint/electricity_retail_sales.py
--rw-r--r--   0 te         (501) staff       (20)     1644 2023-07-12 17:21:42.000000 eia_client-0.4.0/src/eia_client/endpoint/total_energy.py
--rw-r--r--   0 te         (501) staff       (20)      828 2023-07-12 17:08:09.000000 eia_client-0.4.0/src/eia_client/parse.py
--rw-r--r--   0 te         (501) staff       (20)      356 2023-07-12 17:21:42.000000 eia_client-0.4.0/src/eia_client/utils.py
-drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-12 17:29:57.490643 eia_client-0.4.0/src/eia_client.egg-info/
--rw-r--r--   0 te         (501) staff       (20)     2332 2023-07-12 17:29:57.000000 eia_client-0.4.0/src/eia_client.egg-info/PKG-INFO
--rw-r--r--   0 te         (501) staff       (20)      713 2023-07-12 17:29:57.000000 eia_client-0.4.0/src/eia_client.egg-info/SOURCES.txt
--rw-r--r--   0 te         (501) staff       (20)        1 2023-07-12 17:29:57.000000 eia_client-0.4.0/src/eia_client.egg-info/dependency_links.txt
--rw-r--r--   0 te         (501) staff       (20)      161 2023-07-12 17:29:57.000000 eia_client-0.4.0/src/eia_client.egg-info/requires.txt
--rw-r--r--   0 te         (501) staff       (20)       11 2023-07-12 17:29:57.000000 eia_client-0.4.0/src/eia_client.egg-info/top_level.txt
-drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-12 17:29:57.495201 eia_client-0.4.0/tests/
--rw-r--r--   0 te         (501) staff       (20)     1461 2023-02-14 20:04:30.000000 eia_client-0.4.0/tests/test_api_endpoint_builder.py
--rw-r--r--   0 te         (501) staff       (20)     1846 2023-02-14 20:04:30.000000 eia_client-0.4.0/tests/test_api_key.py
+drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-17 20:50:45.489923 eia_client-0.4.1/
+-rw-r--r--   0 te         (501) staff       (20)    11357 2023-02-04 20:51:40.000000 eia_client-0.4.1/LICENSE
+-rw-r--r--   0 te         (501) staff       (20)       44 2023-07-12 17:21:42.000000 eia_client-0.4.1/MANIFEST.in
+-rw-r--r--   0 te         (501) staff       (20)     2332 2023-07-17 20:50:45.490109 eia_client-0.4.1/PKG-INFO
+-rw-r--r--   0 te         (501) staff       (20)     1725 2023-02-14 20:04:30.000000 eia_client-0.4.1/README.md
+-rw-r--r--   0 te         (501) staff       (20)      103 2023-02-10 01:33:54.000000 eia_client-0.4.1/README.rst
+drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-17 20:50:45.473489 eia_client-0.4.1/docs/
+drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-17 20:50:45.477859 eia_client-0.4.1/docs/source/
+-rw-r--r--   0 te         (501) staff       (20)     1279 2023-02-10 01:33:54.000000 eia_client-0.4.1/docs/source/conf.py
+drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-17 20:50:45.479981 eia_client-0.4.1/examples/
+-rw-r--r--   0 te         (501) staff       (20)      398 2023-02-14 20:04:30.000000 eia_client-0.4.1/examples/example_elec_retail_sales.py
+-rw-r--r--   0 te         (501) staff       (20)      334 2023-07-12 17:05:45.000000 eia_client-0.4.1/examples/example_total_energy.py
+-rw-r--r--   0 te         (501) staff       (20)       96 2023-02-10 01:33:54.000000 eia_client-0.4.1/pyproject.toml
+-rw-r--r--   0 te         (501) staff       (20)      948 2023-07-17 20:50:45.491175 eia_client-0.4.1/setup.cfg
+drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-17 20:50:45.474191 eia_client-0.4.1/src/
+drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-17 20:50:45.482486 eia_client-0.4.1/src/eia_client/
+-rw-r--r--   0 te         (501) staff       (20)      194 2023-07-17 20:48:29.000000 eia_client-0.4.1/src/eia_client/__init__.py
+-rw-r--r--   0 te         (501) staff       (20)     3054 2023-07-12 17:06:55.000000 eia_client-0.4.1/src/eia_client/api_key.py
+-rw-r--r--   0 te         (501) staff       (20)     4231 2023-07-17 20:46:19.000000 eia_client-0.4.1/src/eia_client/cli.py
+-rw-r--r--   0 te         (501) staff       (20)      828 2023-07-12 17:21:42.000000 eia_client-0.4.1/src/eia_client/client.py
+drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-17 20:50:45.487742 eia_client-0.4.1/src/eia_client/endpoint/
+-rw-r--r--   0 te         (501) staff       (20)      174 2023-07-12 17:21:42.000000 eia_client-0.4.1/src/eia_client/endpoint/__init__.py
+-rw-r--r--   0 te         (501) staff       (20)     3547 2023-07-12 17:21:42.000000 eia_client-0.4.1/src/eia_client/endpoint/builder.py
+-rw-r--r--   0 te         (501) staff       (20)     2412 2023-07-12 17:21:42.000000 eia_client-0.4.1/src/eia_client/endpoint/electricity_retail_sales.py
+-rw-r--r--   0 te         (501) staff       (20)     1644 2023-07-12 17:21:42.000000 eia_client-0.4.1/src/eia_client/endpoint/total_energy.py
+-rw-r--r--   0 te         (501) staff       (20)      828 2023-07-12 17:08:09.000000 eia_client-0.4.1/src/eia_client/parse.py
+-rw-r--r--   0 te         (501) staff       (20)      356 2023-07-12 17:21:42.000000 eia_client-0.4.1/src/eia_client/utils.py
+drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-17 20:50:45.485118 eia_client-0.4.1/src/eia_client.egg-info/
+-rw-r--r--   0 te         (501) staff       (20)     2332 2023-07-17 20:50:45.000000 eia_client-0.4.1/src/eia_client.egg-info/PKG-INFO
+-rw-r--r--   0 te         (501) staff       (20)      713 2023-07-17 20:50:45.000000 eia_client-0.4.1/src/eia_client.egg-info/SOURCES.txt
+-rw-r--r--   0 te         (501) staff       (20)        1 2023-07-17 20:50:45.000000 eia_client-0.4.1/src/eia_client.egg-info/dependency_links.txt
+-rw-r--r--   0 te         (501) staff       (20)      161 2023-07-17 20:50:45.000000 eia_client-0.4.1/src/eia_client.egg-info/requires.txt
+-rw-r--r--   0 te         (501) staff       (20)       11 2023-07-17 20:50:45.000000 eia_client-0.4.1/src/eia_client.egg-info/top_level.txt
+drwxr-xr-x   0 te         (501) staff       (20)        0 2023-07-17 20:50:45.489198 eia_client-0.4.1/tests/
+-rw-r--r--   0 te         (501) staff       (20)     1461 2023-02-14 20:04:30.000000 eia_client-0.4.1/tests/test_api_endpoint_builder.py
+-rw-r--r--   0 te         (501) staff       (20)     1846 2023-02-14 20:04:30.000000 eia_client-0.4.1/tests/test_api_key.py
```

### Comparing `eia_client-0.4.0/LICENSE` & `eia_client-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eia_client-0.4.0/PKG-INFO` & `eia_client-0.4.1/src/eia_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eia_client
-Version: 0.4.0
+Name: eia-client
+Version: 0.4.1
 Summary: EIA Open Data API Python Client
 Home-page: https://github.com/tayeva/eia-client-python
 Author: tayeva
 Author-email: 124453543+tayeva@users.noreply.github.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eia_client-0.4.0/README.md` & `eia_client-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `eia_client-0.4.0/docs/source/conf.py` & `eia_client-0.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `eia_client-0.4.0/setup.cfg` & `eia_client-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `eia_client-0.4.0/src/eia_client/api_key.py` & `eia_client-0.4.1/src/eia_client/api_key.py`

 * *Files identical despite different names*

### Comparing `eia_client-0.4.0/src/eia_client/client.py` & `eia_client-0.4.1/src/eia_client/client.py`

 * *Files identical despite different names*

### Comparing `eia_client-0.4.0/src/eia_client/endpoint/builder.py` & `eia_client-0.4.1/src/eia_client/endpoint/builder.py`

 * *Files identical despite different names*

### Comparing `eia_client-0.4.0/src/eia_client/endpoint/electricity_retail_sales.py` & `eia_client-0.4.1/src/eia_client/endpoint/electricity_retail_sales.py`

 * *Files identical despite different names*

### Comparing `eia_client-0.4.0/src/eia_client/endpoint/total_energy.py` & `eia_client-0.4.1/src/eia_client/endpoint/total_energy.py`

 * *Files identical despite different names*

### Comparing `eia_client-0.4.0/src/eia_client/parse.py` & `eia_client-0.4.1/src/eia_client/parse.py`

 * *Files identical despite different names*

### Comparing `eia_client-0.4.0/src/eia_client.egg-info/PKG-INFO` & `eia_client-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eia-client
-Version: 0.4.0
+Name: eia_client
+Version: 0.4.1
 Summary: EIA Open Data API Python Client
 Home-page: https://github.com/tayeva/eia-client-python
 Author: tayeva
 Author-email: 124453543+tayeva@users.noreply.github.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eia_client-0.4.0/src/eia_client.egg-info/SOURCES.txt` & `eia_client-0.4.1/src/eia_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eia_client-0.4.0/tests/test_api_endpoint_builder.py` & `eia_client-0.4.1/tests/test_api_endpoint_builder.py`

 * *Files identical despite different names*

### Comparing `eia_client-0.4.0/tests/test_api_key.py` & `eia_client-0.4.1/tests/test_api_key.py`

 * *Files identical despite different names*

