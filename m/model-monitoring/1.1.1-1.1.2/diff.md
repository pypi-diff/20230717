# Comparing `tmp/model_monitoring-1.1.1.tar.gz` & `tmp/model_monitoring-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_monitoring-1.1.1.tar", last modified: Mon Jul 17 10:56:59 2023, max compression
+gzip compressed data, was "model_monitoring-1.1.2.tar", last modified: Mon Jul 17 11:13:17 2023, max compression
```

## Comparing `model_monitoring-1.1.1.tar` & `model_monitoring-1.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:56:59.976993 model_monitoring-1.1.1/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-07-17 10:54:05.000000 model_monitoring-1.1.1/LICENCE
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4747 2023-07-17 10:56:59.976993 model_monitoring-1.1.1/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4263 2023-07-17 10:54:05.000000 model_monitoring-1.1.1/README.md
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      725 2023-07-17 10:54:05.000000 model_monitoring-1.1.1/pyproject.toml
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-07-17 10:56:59.976993 model_monitoring-1.1.1/setup.cfg
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      935 2023-07-17 10:54:05.000000 model_monitoring-1.1.1/setup.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:56:59.948990 model_monitoring-1.1.1/src/
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:56:59.960991 model_monitoring-1.1.1/src/model_monitoring/
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:56:59.968992 model_monitoring-1.1.1/src/model_monitoring/XAI/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:54:05.000000 model_monitoring-1.1.1/src/model_monitoring/XAI/XAI.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    17043 2023-07-17 10:54:05.000000 model_monitoring-1.1.1/src/model_monitoring/XAI/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:50:14.000000 model_monitoring-1.1.1/src/model_monitoring/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2474 2023-07-17 10:50:14.000000 model_monitoring-1.1.1/src/model_monitoring/additional_metrics.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      554 2023-07-17 10:50:14.000000 model_monitoring-1.1.1/src/model_monitoring/config.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:56:59.968992 model_monitoring-1.1.1/src/model_monitoring/data_drift/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    11682 2023-07-17 10:50:14.000000 model_monitoring-1.1.1/src/model_monitoring/data_drift/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15980 2023-07-17 10:50:14.000000 model_monitoring-1.1.1/src/model_monitoring/data_drift/data_drift.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:56:59.968992 model_monitoring-1.1.1/src/model_monitoring/fairness_drift/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    17315 2023-07-17 10:50:14.000000 model_monitoring-1.1.1/src/model_monitoring/fairness_drift/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4917 2023-07-17 10:50:14.000000 model_monitoring-1.1.1/src/model_monitoring/fairness_drift/fairness_drift.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:56:59.972993 model_monitoring-1.1.1/src/model_monitoring/fairness_measures/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     7398 2023-07-17 10:50:14.000000 model_monitoring-1.1.1/src/model_monitoring/fairness_measures/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    23888 2023-07-17 10:50:14.000000 model_monitoring-1.1.1/src/model_monitoring/fairness_measures/fairness_measures.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:56:59.972993 model_monitoring-1.1.1/src/model_monitoring/model_performance/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10291 2023-07-17 10:50:14.000000 model_monitoring-1.1.1/src/model_monitoring/model_performance/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      801 2023-07-17 10:50:14.000000 model_monitoring-1.1.1/src/model_monitoring/model_performance/model_performance.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:56:59.976993 model_monitoring-1.1.1/src/model_monitoring/performance_measures/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     8616 2023-07-17 10:50:14.000000 model_monitoring-1.1.1/src/model_monitoring/performance_measures/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      380 2023-07-17 10:50:14.000000 model_monitoring-1.1.1/src/model_monitoring/performance_measures/performance_measures.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:56:59.976993 model_monitoring-1.1.1/src/model_monitoring/reference_metadata/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     5113 2023-07-17 10:50:14.000000 model_monitoring-1.1.1/src/model_monitoring/reference_metadata/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4489 2023-07-17 10:50:14.000000 model_monitoring-1.1.1/src/model_monitoring/reference_metadata/reference_metadata.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     5617 2023-07-17 10:50:14.000000 model_monitoring-1.1.1/src/model_monitoring/utils.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:56:59.964992 model_monitoring-1.1.1/src/model_monitoring.egg-info/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4747 2023-07-17 10:56:59.000000 model_monitoring-1.1.1/src/model_monitoring.egg-info/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1114 2023-07-17 10:56:59.000000 model_monitoring-1.1.1/src/model_monitoring.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-07-17 10:56:59.000000 model_monitoring-1.1.1/src/model_monitoring.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      112 2023-07-17 10:56:59.000000 model_monitoring-1.1.1/src/model_monitoring.egg-info/requires.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)       17 2023-07-17 10:56:59.000000 model_monitoring-1.1.1/src/model_monitoring.egg-info/top_level.txt
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 11:13:17.722701 model_monitoring-1.1.2/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-07-17 10:54:05.000000 model_monitoring-1.1.2/LICENCE
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4747 2023-07-17 11:13:17.722701 model_monitoring-1.1.2/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4263 2023-07-17 10:54:05.000000 model_monitoring-1.1.2/README.md
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      725 2023-07-17 11:12:30.000000 model_monitoring-1.1.2/pyproject.toml
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-07-17 11:13:17.722701 model_monitoring-1.1.2/setup.cfg
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      935 2023-07-17 11:12:30.000000 model_monitoring-1.1.2/setup.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 11:13:17.666696 model_monitoring-1.1.2/src/
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 11:13:17.698699 model_monitoring-1.1.2/src/model_monitoring/
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 11:13:17.706699 model_monitoring-1.1.2/src/model_monitoring/XAI/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:54:05.000000 model_monitoring-1.1.2/src/model_monitoring/XAI/XAI.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    17043 2023-07-17 10:54:05.000000 model_monitoring-1.1.2/src/model_monitoring/XAI/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:50:14.000000 model_monitoring-1.1.2/src/model_monitoring/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2474 2023-07-17 10:50:14.000000 model_monitoring-1.1.2/src/model_monitoring/additional_metrics.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      554 2023-07-17 10:50:14.000000 model_monitoring-1.1.2/src/model_monitoring/config.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 11:13:17.706699 model_monitoring-1.1.2/src/model_monitoring/data_drift/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    11682 2023-07-17 10:50:14.000000 model_monitoring-1.1.2/src/model_monitoring/data_drift/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15980 2023-07-17 10:50:14.000000 model_monitoring-1.1.2/src/model_monitoring/data_drift/data_drift.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 11:13:17.710700 model_monitoring-1.1.2/src/model_monitoring/fairness_drift/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    17315 2023-07-17 10:50:14.000000 model_monitoring-1.1.2/src/model_monitoring/fairness_drift/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4917 2023-07-17 10:50:14.000000 model_monitoring-1.1.2/src/model_monitoring/fairness_drift/fairness_drift.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 11:13:17.714700 model_monitoring-1.1.2/src/model_monitoring/fairness_measures/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     7398 2023-07-17 10:50:14.000000 model_monitoring-1.1.2/src/model_monitoring/fairness_measures/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    23888 2023-07-17 10:50:14.000000 model_monitoring-1.1.2/src/model_monitoring/fairness_measures/fairness_measures.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 11:13:17.718701 model_monitoring-1.1.2/src/model_monitoring/model_performance/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10291 2023-07-17 10:50:14.000000 model_monitoring-1.1.2/src/model_monitoring/model_performance/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      801 2023-07-17 10:50:14.000000 model_monitoring-1.1.2/src/model_monitoring/model_performance/model_performance.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 11:13:17.718701 model_monitoring-1.1.2/src/model_monitoring/performance_measures/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     8616 2023-07-17 10:50:14.000000 model_monitoring-1.1.2/src/model_monitoring/performance_measures/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      380 2023-07-17 10:50:14.000000 model_monitoring-1.1.2/src/model_monitoring/performance_measures/performance_measures.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 11:13:17.722701 model_monitoring-1.1.2/src/model_monitoring/reference_metadata/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     5113 2023-07-17 10:50:14.000000 model_monitoring-1.1.2/src/model_monitoring/reference_metadata/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4489 2023-07-17 10:50:14.000000 model_monitoring-1.1.2/src/model_monitoring/reference_metadata/reference_metadata.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     5617 2023-07-17 10:50:14.000000 model_monitoring-1.1.2/src/model_monitoring/utils.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 11:13:17.706699 model_monitoring-1.1.2/src/model_monitoring.egg-info/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4747 2023-07-17 11:13:17.000000 model_monitoring-1.1.2/src/model_monitoring.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1114 2023-07-17 11:13:17.000000 model_monitoring-1.1.2/src/model_monitoring.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-07-17 11:13:17.000000 model_monitoring-1.1.2/src/model_monitoring.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      112 2023-07-17 11:13:17.000000 model_monitoring-1.1.2/src/model_monitoring.egg-info/requires.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       17 2023-07-17 11:13:17.000000 model_monitoring-1.1.2/src/model_monitoring.egg-info/top_level.txt
```

### Comparing `model_monitoring-1.1.1/LICENCE` & `model_monitoring-1.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.1/PKG-INFO` & `model_monitoring-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model_monitoring
-Version: 1.1.1
+Version: 1.1.2
 Summary: Model Monitoring
 Home-page: https://dev.azure.com/credem-data/DAT/_git/model_monitoring
 Author: DAT/Michelangelo Culiat
 Author-email: DAT - Michelangelo Culiat <mculiat@credem.it>
 Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/model_monitoring
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `model_monitoring-1.1.1/README.md` & `model_monitoring-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.1/pyproject.toml` & `model_monitoring-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model_monitoring"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="DAT - Michelangelo Culiat", email="mculiat@credem.it" },
 ]
 description = "Model Monitoring"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `model_monitoring-1.1.1/setup.py` & `model_monitoring-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="model_monitoring",
-    version="1.1.1",
+    version="1.1.2",
     description="Package for Model Monitoring",
     author="DAT/Michelangelo Culiat",
     author_email="mculiat@credem.it",
     url="https://dev.azure.com/credem-data/DAT/_git/model_monitoring",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
```

### Comparing `model_monitoring-1.1.1/src/model_monitoring/XAI/__init__.py` & `model_monitoring-1.1.2/src/model_monitoring/XAI/__init__.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.1/src/model_monitoring/additional_metrics.py` & `model_monitoring-1.1.2/src/model_monitoring/additional_metrics.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.1/src/model_monitoring/config.py` & `model_monitoring-1.1.2/src/model_monitoring/config.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.1/src/model_monitoring/data_drift/__init__.py` & `model_monitoring-1.1.2/src/model_monitoring/data_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.1/src/model_monitoring/data_drift/data_drift.py` & `model_monitoring-1.1.2/src/model_monitoring/data_drift/data_drift.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.1/src/model_monitoring/fairness_drift/__init__.py` & `model_monitoring-1.1.2/src/model_monitoring/fairness_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.1/src/model_monitoring/fairness_drift/fairness_drift.py` & `model_monitoring-1.1.2/src/model_monitoring/fairness_drift/fairness_drift.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.1/src/model_monitoring/fairness_measures/__init__.py` & `model_monitoring-1.1.2/src/model_monitoring/fairness_measures/__init__.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.1/src/model_monitoring/fairness_measures/fairness_measures.py` & `model_monitoring-1.1.2/src/model_monitoring/fairness_measures/fairness_measures.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.1/src/model_monitoring/model_performance/__init__.py` & `model_monitoring-1.1.2/src/model_monitoring/model_performance/__init__.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.1/src/model_monitoring/model_performance/model_performance.py` & `model_monitoring-1.1.2/src/model_monitoring/model_performance/model_performance.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.1/src/model_monitoring/performance_measures/__init__.py` & `model_monitoring-1.1.2/src/model_monitoring/performance_measures/__init__.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.1/src/model_monitoring/reference_metadata/__init__.py` & `model_monitoring-1.1.2/src/model_monitoring/reference_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.1/src/model_monitoring/reference_metadata/reference_metadata.py` & `model_monitoring-1.1.2/src/model_monitoring/reference_metadata/reference_metadata.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.1/src/model_monitoring/utils.py` & `model_monitoring-1.1.2/src/model_monitoring/utils.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.1/src/model_monitoring.egg-info/PKG-INFO` & `model_monitoring-1.1.2/src/model_monitoring.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-monitoring
-Version: 1.1.1
+Version: 1.1.2
 Summary: Model Monitoring
 Home-page: https://dev.azure.com/credem-data/DAT/_git/model_monitoring
 Author: DAT/Michelangelo Culiat
 Author-email: DAT - Michelangelo Culiat <mculiat@credem.it>
 Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/model_monitoring
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `model_monitoring-1.1.1/src/model_monitoring.egg-info/SOURCES.txt` & `model_monitoring-1.1.2/src/model_monitoring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

