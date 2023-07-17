# Comparing `tmp/model_monitoring-1.1.3.tar.gz` & `tmp/model_monitoring-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_monitoring-1.1.3.tar", last modified: Mon Jul 17 13:06:41 2023, max compression
+gzip compressed data, was "model_monitoring-1.1.4.tar", last modified: Mon Jul 17 14:19:57 2023, max compression
```

## Comparing `model_monitoring-1.1.3.tar` & `model_monitoring-1.1.4.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 13:06:41.797208 model_monitoring-1.1.3/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-07-17 10:54:05.000000 model_monitoring-1.1.3/LICENCE
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4747 2023-07-17 13:06:41.797208 model_monitoring-1.1.3/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4263 2023-07-17 10:54:05.000000 model_monitoring-1.1.3/README.md
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      725 2023-07-17 13:05:31.000000 model_monitoring-1.1.3/pyproject.toml
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-07-17 13:06:41.797208 model_monitoring-1.1.3/setup.cfg
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      935 2023-07-17 13:05:31.000000 model_monitoring-1.1.3/setup.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 13:06:41.737204 model_monitoring-1.1.3/src/
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 13:06:41.769206 model_monitoring-1.1.3/src/model_monitoring/
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 13:06:41.777207 model_monitoring-1.1.3/src/model_monitoring/XAI/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:54:05.000000 model_monitoring-1.1.3/src/model_monitoring/XAI/XAI.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    17043 2023-07-17 10:54:05.000000 model_monitoring-1.1.3/src/model_monitoring/XAI/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:50:14.000000 model_monitoring-1.1.3/src/model_monitoring/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2474 2023-07-17 10:50:14.000000 model_monitoring-1.1.3/src/model_monitoring/additional_metrics.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 13:06:41.777207 model_monitoring-1.1.3/src/model_monitoring/config/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 13:05:31.000000 model_monitoring-1.1.3/src/model_monitoring/config/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      554 2023-07-17 10:50:14.000000 model_monitoring-1.1.3/src/model_monitoring/config.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 13:06:41.781207 model_monitoring-1.1.3/src/model_monitoring/data_drift/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    11682 2023-07-17 10:50:14.000000 model_monitoring-1.1.3/src/model_monitoring/data_drift/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15980 2023-07-17 10:50:14.000000 model_monitoring-1.1.3/src/model_monitoring/data_drift/data_drift.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 13:06:41.785207 model_monitoring-1.1.3/src/model_monitoring/fairness_drift/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    17315 2023-07-17 10:50:14.000000 model_monitoring-1.1.3/src/model_monitoring/fairness_drift/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4917 2023-07-17 10:50:14.000000 model_monitoring-1.1.3/src/model_monitoring/fairness_drift/fairness_drift.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 13:06:41.785207 model_monitoring-1.1.3/src/model_monitoring/fairness_measures/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     7398 2023-07-17 10:50:14.000000 model_monitoring-1.1.3/src/model_monitoring/fairness_measures/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    23888 2023-07-17 10:50:14.000000 model_monitoring-1.1.3/src/model_monitoring/fairness_measures/fairness_measures.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 13:06:41.789207 model_monitoring-1.1.3/src/model_monitoring/model_performance/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10291 2023-07-17 10:50:14.000000 model_monitoring-1.1.3/src/model_monitoring/model_performance/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      801 2023-07-17 10:50:14.000000 model_monitoring-1.1.3/src/model_monitoring/model_performance/model_performance.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 13:06:41.793208 model_monitoring-1.1.3/src/model_monitoring/performance_measures/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     8616 2023-07-17 10:50:14.000000 model_monitoring-1.1.3/src/model_monitoring/performance_measures/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      380 2023-07-17 10:50:14.000000 model_monitoring-1.1.3/src/model_monitoring/performance_measures/performance_measures.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 13:06:41.797208 model_monitoring-1.1.3/src/model_monitoring/reference_metadata/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     5113 2023-07-17 10:50:14.000000 model_monitoring-1.1.3/src/model_monitoring/reference_metadata/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4489 2023-07-17 10:50:14.000000 model_monitoring-1.1.3/src/model_monitoring/reference_metadata/reference_metadata.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     5617 2023-07-17 10:50:14.000000 model_monitoring-1.1.3/src/model_monitoring/utils.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 13:06:41.773206 model_monitoring-1.1.3/src/model_monitoring.egg-info/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4747 2023-07-17 13:06:41.000000 model_monitoring-1.1.3/src/model_monitoring.egg-info/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1154 2023-07-17 13:06:41.000000 model_monitoring-1.1.3/src/model_monitoring.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-07-17 13:06:41.000000 model_monitoring-1.1.3/src/model_monitoring.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      112 2023-07-17 13:06:41.000000 model_monitoring-1.1.3/src/model_monitoring.egg-info/requires.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)       17 2023-07-17 13:06:41.000000 model_monitoring-1.1.3/src/model_monitoring.egg-info/top_level.txt
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 14:19:57.931522 model_monitoring-1.1.4/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-07-17 10:54:05.000000 model_monitoring-1.1.4/LICENCE
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       47 2023-07-17 14:19:28.000000 model_monitoring-1.1.4/MANIFEST.in
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4827 2023-07-17 14:19:57.931522 model_monitoring-1.1.4/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4349 2023-07-17 14:19:28.000000 model_monitoring-1.1.4/README.md
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      725 2023-07-17 14:19:28.000000 model_monitoring-1.1.4/pyproject.toml
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-07-17 14:19:57.931522 model_monitoring-1.1.4/setup.cfg
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1038 2023-07-17 14:19:28.000000 model_monitoring-1.1.4/setup.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 14:19:57.831515 model_monitoring-1.1.4/src/
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 14:19:57.883519 model_monitoring-1.1.4/src/model_monitoring/
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 14:19:57.887519 model_monitoring-1.1.4/src/model_monitoring/XAI/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:54:05.000000 model_monitoring-1.1.4/src/model_monitoring/XAI/XAI.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    17043 2023-07-17 10:54:05.000000 model_monitoring-1.1.4/src/model_monitoring/XAI/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2474 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/additional_metrics.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 14:19:57.915521 model_monitoring-1.1.4/src/model_monitoring/config/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      536 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/config/algorithm_settings.yml
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1499 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/config/drift_threshold.yml
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1263 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/config/fairness_drift_threshold.yml
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      554 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/config.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 14:19:57.919521 model_monitoring-1.1.4/src/model_monitoring/data_drift/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    11682 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/data_drift/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15980 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/data_drift/data_drift.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 14:19:57.919521 model_monitoring-1.1.4/src/model_monitoring/fairness_drift/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    17315 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/fairness_drift/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4917 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/fairness_drift/fairness_drift.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 14:19:57.923521 model_monitoring-1.1.4/src/model_monitoring/fairness_measures/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     7398 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/fairness_measures/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    23888 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/fairness_measures/fairness_measures.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 14:19:57.927522 model_monitoring-1.1.4/src/model_monitoring/model_performance/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10291 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/model_performance/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      801 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/model_performance/model_performance.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 14:19:57.927522 model_monitoring-1.1.4/src/model_monitoring/performance_measures/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     8616 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/performance_measures/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      380 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/performance_measures/performance_measures.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 14:19:57.931522 model_monitoring-1.1.4/src/model_monitoring/reference_metadata/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     5113 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/reference_metadata/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4489 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/reference_metadata/reference_metadata.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     5617 2023-07-17 10:50:14.000000 model_monitoring-1.1.4/src/model_monitoring/utils.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-07-17 14:19:57.883519 model_monitoring-1.1.4/src/model_monitoring.egg-info/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4827 2023-07-17 14:19:57.000000 model_monitoring-1.1.4/src/model_monitoring.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1282 2023-07-17 14:19:57.000000 model_monitoring-1.1.4/src/model_monitoring.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-07-17 14:19:57.000000 model_monitoring-1.1.4/src/model_monitoring.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      112 2023-07-17 14:19:57.000000 model_monitoring-1.1.4/src/model_monitoring.egg-info/requires.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       17 2023-07-17 14:19:57.000000 model_monitoring-1.1.4/src/model_monitoring.egg-info/top_level.txt
```

### Comparing `model_monitoring-1.1.3/LICENCE` & `model_monitoring-1.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.3/PKG-INFO` & `model_monitoring-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model_monitoring
-Version: 1.1.3
+Version: 1.1.4
 Summary: Model Monitoring
 Home-page: https://dev.azure.com/credem-data/DAT/_git/model_monitoring
 Author: DAT/Michelangelo Culiat
 Author-email: DAT - Michelangelo Culiat <mculiat@credem.it>
 Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/model_monitoring
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -46,14 +46,20 @@
 
 ## Struttura
 ```
 model_monitoring/
 |
 └─── .pre-commit-config.yaml
 |
+└─── pyproject.toml
+|
+└─── LICENCE
+|
+└─── MANIFEST.in
+|
 └─── README.md
 |
 └─── requirements.txt
 |
 └─── setup.py
 |
 └─── .gitignore
```

### Comparing `model_monitoring-1.1.3/README.md` & `model_monitoring-1.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 
 ## Struttura
 ```
 model_monitoring/
 |
 └─── .pre-commit-config.yaml
 |
+└─── pyproject.toml
+|
+└─── LICENCE
+|
+└─── MANIFEST.in
+|
 └─── README.md
 |
 └─── requirements.txt
 |
 └─── setup.py
 |
 └─── .gitignore
```

### Comparing `model_monitoring-1.1.3/pyproject.toml` & `model_monitoring-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model_monitoring"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="DAT - Michelangelo Culiat", email="mculiat@credem.it" },
 ]
 description = "Model Monitoring"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `model_monitoring-1.1.3/setup.py` & `model_monitoring-1.1.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name="model_monitoring",
-    version="1.1.3",
+    version="1.1.4",
     description="Package for Model Monitoring",
     author="DAT/Michelangelo Culiat",
     author_email="mculiat@credem.it",
     url="https://dev.azure.com/credem-data/DAT/_git/model_monitoring",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3 :: Only",
     ],
     packages=find_packages(where="src"),
+    package_data={
+        "model_monitoring": ["config/*.yml"],
+    },
+    include_package_data=True,
     package_dir={"": "src"},
     # Usato solo con 3.9 e 3.10
     python_requires=">=3.9, <4",
     install_requires=[
         "typed-ast==1.5.4",
         "numpy==1.22.4",
         "pandas==1.5.3",
```

### Comparing `model_monitoring-1.1.3/src/model_monitoring/XAI/__init__.py` & `model_monitoring-1.1.4/src/model_monitoring/XAI/__init__.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.3/src/model_monitoring/additional_metrics.py` & `model_monitoring-1.1.4/src/model_monitoring/additional_metrics.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.3/src/model_monitoring/config.py` & `model_monitoring-1.1.4/src/model_monitoring/config.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.3/src/model_monitoring/data_drift/__init__.py` & `model_monitoring-1.1.4/src/model_monitoring/data_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.3/src/model_monitoring/data_drift/data_drift.py` & `model_monitoring-1.1.4/src/model_monitoring/data_drift/data_drift.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.3/src/model_monitoring/fairness_drift/__init__.py` & `model_monitoring-1.1.4/src/model_monitoring/fairness_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.3/src/model_monitoring/fairness_drift/fairness_drift.py` & `model_monitoring-1.1.4/src/model_monitoring/fairness_drift/fairness_drift.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.3/src/model_monitoring/fairness_measures/__init__.py` & `model_monitoring-1.1.4/src/model_monitoring/fairness_measures/__init__.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.3/src/model_monitoring/fairness_measures/fairness_measures.py` & `model_monitoring-1.1.4/src/model_monitoring/fairness_measures/fairness_measures.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.3/src/model_monitoring/model_performance/__init__.py` & `model_monitoring-1.1.4/src/model_monitoring/model_performance/__init__.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.3/src/model_monitoring/model_performance/model_performance.py` & `model_monitoring-1.1.4/src/model_monitoring/model_performance/model_performance.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.3/src/model_monitoring/performance_measures/__init__.py` & `model_monitoring-1.1.4/src/model_monitoring/performance_measures/__init__.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.3/src/model_monitoring/reference_metadata/__init__.py` & `model_monitoring-1.1.4/src/model_monitoring/reference_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.3/src/model_monitoring/reference_metadata/reference_metadata.py` & `model_monitoring-1.1.4/src/model_monitoring/reference_metadata/reference_metadata.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.3/src/model_monitoring/utils.py` & `model_monitoring-1.1.4/src/model_monitoring/utils.py`

 * *Files identical despite different names*

### Comparing `model_monitoring-1.1.3/src/model_monitoring.egg-info/PKG-INFO` & `model_monitoring-1.1.4/src/model_monitoring.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-monitoring
-Version: 1.1.3
+Version: 1.1.4
 Summary: Model Monitoring
 Home-page: https://dev.azure.com/credem-data/DAT/_git/model_monitoring
 Author: DAT/Michelangelo Culiat
 Author-email: DAT - Michelangelo Culiat <mculiat@credem.it>
 Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/model_monitoring
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -46,14 +46,20 @@
 
 ## Struttura
 ```
 model_monitoring/
 |
 └─── .pre-commit-config.yaml
 |
+└─── pyproject.toml
+|
+└─── LICENCE
+|
+└─── MANIFEST.in
+|
 └─── README.md
 |
 └─── requirements.txt
 |
 └─── setup.py
 |
 └─── .gitignore
```

### Comparing `model_monitoring-1.1.3/src/model_monitoring.egg-info/SOURCES.txt` & `model_monitoring-1.1.4/src/model_monitoring.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 LICENCE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/model_monitoring/__init__.py
 src/model_monitoring/additional_metrics.py
 src/model_monitoring/config.py
 src/model_monitoring/utils.py
 src/model_monitoring.egg-info/PKG-INFO
 src/model_monitoring.egg-info/SOURCES.txt
 src/model_monitoring.egg-info/dependency_links.txt
 src/model_monitoring.egg-info/requires.txt
 src/model_monitoring.egg-info/top_level.txt
 src/model_monitoring/XAI/XAI.py
 src/model_monitoring/XAI/__init__.py
-src/model_monitoring/config/__init__.py
+src/model_monitoring/config/algorithm_settings.yml
+src/model_monitoring/config/drift_threshold.yml
+src/model_monitoring/config/fairness_drift_threshold.yml
 src/model_monitoring/data_drift/__init__.py
 src/model_monitoring/data_drift/data_drift.py
 src/model_monitoring/fairness_drift/__init__.py
 src/model_monitoring/fairness_drift/fairness_drift.py
 src/model_monitoring/fairness_measures/__init__.py
 src/model_monitoring/fairness_measures/fairness_measures.py
 src/model_monitoring/model_performance/__init__.py
```

