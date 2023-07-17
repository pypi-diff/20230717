# Comparing `tmp/datamaker-sdk-0.2.tar.gz` & `tmp/datamaker-sdk-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamaker-sdk-0.2.tar", last modified: Mon Jun 19 01:23:42 2023, max compression
+gzip compressed data, was "datamaker-sdk-0.3.tar", last modified: Mon Jul 17 00:32:49 2023, max compression
```

## Comparing `datamaker-sdk-0.2.tar` & `datamaker-sdk-0.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.689411 datamaker-sdk-0.2/
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.685410 datamaker-sdk-0.2/.github/
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.685410 datamaker-sdk-0.2/.github/workflows/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1131 2023-06-19 01:23:35.000000 datamaker-sdk-0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      221 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/.gitignore
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1101 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/LICENSE
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      870 2023-06-19 01:23:42.689411 datamaker-sdk-0.2/PKG-INFO
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/README.md
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.685410 datamaker-sdk-0.2/datamaker/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/__init__.py
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.685410 datamaker-sdk-0.2/datamaker/client/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     3526 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/client/__init__.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      405 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/client/exceptions.py
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.689411 datamaker-sdk-0.2/datamaker/client/mixins/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/client/mixins/__init__.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1021 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/client/mixins/annotation.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     3922 2023-06-19 01:07:34.000000 datamaker-sdk-0.2/datamaker/client/mixins/dataset.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      337 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/client/mixins/integration.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      904 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/client/mixins/ml.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      420 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/client/utils.py
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.689411 datamaker-sdk-0.2/datamaker/plugins/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1049 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/plugins/__init__.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1676 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/plugins/exports.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/plugins/imports.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     6894 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/plugins/neural_networks.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      455 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/plugins/preprocessors.py
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.689411 datamaker-sdk-0.2/datamaker/utils/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/utils/__init__.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1940 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/utils/file.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1401 2023-06-15 04:08:47.000000 datamaker-sdk-0.2/datamaker/utils/logger.py
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-06-19 01:23:42.689411 datamaker-sdk-0.2/datamaker_sdk.egg-info/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      870 2023-06-19 01:23:42.000000 datamaker-sdk-0.2/datamaker_sdk.egg-info/PKG-INFO
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      798 2023-06-19 01:23:42.000000 datamaker-sdk-0.2/datamaker_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)        1 2023-06-19 01:23:42.000000 datamaker-sdk-0.2/datamaker_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      106 2023-06-19 01:23:42.000000 datamaker-sdk-0.2/datamaker_sdk.egg-info/requires.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)       10 2023-06-19 01:23:42.000000 datamaker-sdk-0.2/datamaker_sdk.egg-info/top_level.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      162 2023-06-19 01:23:35.000000 datamaker-sdk-0.2/pyproject.toml
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1004 2023-06-19 01:23:42.689411 datamaker-sdk-0.2/setup.cfg
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-17 00:32:49.547648 datamaker-sdk-0.3/
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-17 00:32:49.543647 datamaker-sdk-0.3/.github/
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-17 00:32:49.547648 datamaker-sdk-0.3/.github/workflows/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1131 2023-06-19 01:23:35.000000 datamaker-sdk-0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      221 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/.gitignore
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1101 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/LICENSE
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      870 2023-07-17 00:32:49.547648 datamaker-sdk-0.3/PKG-INFO
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/README.md
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-17 00:32:49.547648 datamaker-sdk-0.3/datamaker/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/datamaker/__init__.py
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-17 00:32:49.547648 datamaker-sdk-0.3/datamaker/client/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     3597 2023-07-17 00:32:41.000000 datamaker-sdk-0.3/datamaker/client/__init__.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      405 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/datamaker/client/exceptions.py
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-17 00:32:49.547648 datamaker-sdk-0.3/datamaker/client/mixins/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/datamaker/client/mixins/__init__.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1021 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/datamaker/client/mixins/annotation.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     3922 2023-06-19 01:07:34.000000 datamaker-sdk-0.3/datamaker/client/mixins/dataset.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      242 2023-07-17 00:32:41.000000 datamaker-sdk-0.3/datamaker/client/mixins/hitl.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      337 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/datamaker/client/mixins/integration.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      904 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/datamaker/client/mixins/ml.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      420 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/datamaker/client/utils.py
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-17 00:32:49.547648 datamaker-sdk-0.3/datamaker/plugins/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1049 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/datamaker/plugins/__init__.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1676 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/datamaker/plugins/exports.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/datamaker/plugins/imports.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     6894 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/datamaker/plugins/neural_networks.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      455 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/datamaker/plugins/preprocessors.py
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-17 00:32:49.547648 datamaker-sdk-0.3/datamaker/utils/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)        0 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/datamaker/utils/__init__.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1940 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/datamaker/utils/file.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1401 2023-06-15 04:08:47.000000 datamaker-sdk-0.3/datamaker/utils/logger.py
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-17 00:32:49.547648 datamaker-sdk-0.3/datamaker_sdk.egg-info/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      870 2023-07-17 00:32:49.000000 datamaker-sdk-0.3/datamaker_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      830 2023-07-17 00:32:49.000000 datamaker-sdk-0.3/datamaker_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)        1 2023-07-17 00:32:49.000000 datamaker-sdk-0.3/datamaker_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      106 2023-07-17 00:32:49.000000 datamaker-sdk-0.3/datamaker_sdk.egg-info/requires.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)       10 2023-07-17 00:32:49.000000 datamaker-sdk-0.3/datamaker_sdk.egg-info/top_level.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      162 2023-06-19 01:23:35.000000 datamaker-sdk-0.3/pyproject.toml
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1004 2023-07-17 00:32:49.551648 datamaker-sdk-0.3/setup.cfg
```

### Comparing `datamaker-sdk-0.2/.github/workflows/python-publish.yml` & `datamaker-sdk-0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.2/LICENSE` & `datamaker-sdk-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.2/PKG-INFO` & `datamaker-sdk-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaker-sdk
-Version: 0.2
+Version: 0.3
 Summary: datamaker sdk
 Home-page: https://www.datamaker.io
 Author: datamaker
 Author-email: developer@datamaker.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamaker-sdk-0.2/datamaker/client/__init__.py` & `datamaker-sdk-0.3/datamaker/client/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 from django.utils.translation import gettext as _
 
 from ..utils.file import files_url_to_path_from_objs
 
 from .exceptions import ClientError
 from .mixins.annotation import AnnotationClientMixin
 from .mixins.dataset import DatasetClientMixin
+from .mixins.hitl import HITLClientMixin
 from .mixins.integration import IntegrationClientMixin
 from .mixins.ml import MLClientMixin
 
 
 class Client(AnnotationClientMixin,
              DatasetClientMixin,
+             HITLClientMixin,
              IntegrationClientMixin,
              MLClientMixin):
     base_url = None
     token = None
     workspace_code = None
 
     def __init__(self, base_url, token, workspace_code=None):
```

### Comparing `datamaker-sdk-0.2/datamaker/client/mixins/annotation.py` & `datamaker-sdk-0.3/datamaker/client/mixins/annotation.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.2/datamaker/client/mixins/dataset.py` & `datamaker-sdk-0.3/datamaker/client/mixins/dataset.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.2/datamaker/client/mixins/ml.py` & `datamaker-sdk-0.3/datamaker/client/mixins/ml.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.2/datamaker/plugins/__init__.py` & `datamaker-sdk-0.3/datamaker/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.2/datamaker/plugins/exports.py` & `datamaker-sdk-0.3/datamaker/plugins/exports.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.2/datamaker/plugins/neural_networks.py` & `datamaker-sdk-0.3/datamaker/plugins/neural_networks.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.2/datamaker/utils/file.py` & `datamaker-sdk-0.3/datamaker/utils/file.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.2/datamaker/utils/logger.py` & `datamaker-sdk-0.3/datamaker/utils/logger.py`

 * *Files identical despite different names*

### Comparing `datamaker-sdk-0.2/datamaker_sdk.egg-info/PKG-INFO` & `datamaker-sdk-0.3/datamaker_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaker-sdk
-Version: 0.2
+Version: 0.3
 Summary: datamaker sdk
 Home-page: https://www.datamaker.io
 Author: datamaker
 Author-email: developer@datamaker.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamaker-sdk-0.2/datamaker_sdk.egg-info/SOURCES.txt` & `datamaker-sdk-0.3/datamaker_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 datamaker/__init__.py
 datamaker/client/__init__.py
 datamaker/client/exceptions.py
 datamaker/client/utils.py
 datamaker/client/mixins/__init__.py
 datamaker/client/mixins/annotation.py
 datamaker/client/mixins/dataset.py
+datamaker/client/mixins/hitl.py
 datamaker/client/mixins/integration.py
 datamaker/client/mixins/ml.py
 datamaker/plugins/__init__.py
 datamaker/plugins/exports.py
 datamaker/plugins/imports.py
 datamaker/plugins/neural_networks.py
 datamaker/plugins/preprocessors.py
```

### Comparing `datamaker-sdk-0.2/setup.cfg` & `datamaker-sdk-0.3/setup.cfg`

 * *Files identical despite different names*

