# Comparing `tmp/lavlab-python-utils-1.2.1.tar.gz` & `tmp/lavlab-python-utils-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavlab-python-utils-1.2.1.tar", last modified: Mon Jul 17 11:08:51 2023, max compression
+gzip compressed data, was "lavlab-python-utils-1.2.2.tar", last modified: Mon Jul 17 11:15:35 2023, max compression
```

## Comparing `lavlab-python-utils-1.2.1.tar` & `lavlab-python-utils-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:08:51.862035 lavlab-python-utils-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-17 11:08:51.862035 lavlab-python-utils-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-17 11:08:37.000000 lavlab-python-utils-1.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-17 11:08:37.000000 lavlab-python-utils-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 11:08:51.862035 lavlab-python-utils-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:08:51.858035 lavlab-python-utils-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:08:51.858035 lavlab-python-utils-1.2.1/src/lavlab/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-17 11:08:37.000000 lavlab-python-utils-1.2.1/src/lavlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-17 11:08:37.000000 lavlab-python-utils-1.2.1/src/lavlab/omero_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    30918 2023-07-17 11:08:37.000000 lavlab-python-utils-1.2.1/src/lavlab/omero_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10553 2023-07-17 11:08:37.000000 lavlab-python-utils-1.2.1/src/lavlab/python_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:08:51.862035 lavlab-python-utils-1.2.1/src/lavlab_python_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-17 11:08:51.000000 lavlab-python-utils-1.2.1/src/lavlab_python_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-17 11:08:51.000000 lavlab-python-utils-1.2.1/src/lavlab_python_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:08:51.000000 lavlab-python-utils-1.2.1/src/lavlab_python_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 11:08:51.000000 lavlab-python-utils-1.2.1/src/lavlab_python_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 11:08:51.000000 lavlab-python-utils-1.2.1/src/lavlab_python_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:08:51.862035 lavlab-python-utils-1.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-17 11:08:37.000000 lavlab-python-utils-1.2.1/test/test_omero_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-17 11:08:37.000000 lavlab-python-utils-1.2.1/test/test_python_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:15:35.872019 lavlab-python-utils-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-17 11:15:35.872019 lavlab-python-utils-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-17 11:15:24.000000 lavlab-python-utils-1.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-17 11:15:24.000000 lavlab-python-utils-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 11:15:35.872019 lavlab-python-utils-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:15:35.872019 lavlab-python-utils-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:15:35.872019 lavlab-python-utils-1.2.2/src/lavlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-17 11:15:24.000000 lavlab-python-utils-1.2.2/src/lavlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-17 11:15:24.000000 lavlab-python-utils-1.2.2/src/lavlab/omero_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30918 2023-07-17 11:15:24.000000 lavlab-python-utils-1.2.2/src/lavlab/omero_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10553 2023-07-17 11:15:24.000000 lavlab-python-utils-1.2.2/src/lavlab/python_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:15:35.872019 lavlab-python-utils-1.2.2/src/lavlab_python_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-17 11:15:35.000000 lavlab-python-utils-1.2.2/src/lavlab_python_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-17 11:15:35.000000 lavlab-python-utils-1.2.2/src/lavlab_python_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:15:35.000000 lavlab-python-utils-1.2.2/src/lavlab_python_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 11:15:35.000000 lavlab-python-utils-1.2.2/src/lavlab_python_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 11:15:35.000000 lavlab-python-utils-1.2.2/src/lavlab_python_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:15:35.872019 lavlab-python-utils-1.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-17 11:15:24.000000 lavlab-python-utils-1.2.2/test/test_omero_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-17 11:15:24.000000 lavlab-python-utils-1.2.2/test/test_python_utils.py
```

### Comparing `lavlab-python-utils-1.2.1/PKG-INFO` & `lavlab-python-utils-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavlab-python-utils
-Version: 1.2.1
+Version: 1.2.2
 Summary: LaViolette Lab utility package
 Author-email: Michael Barrett <mjbarrett@mcw.edu>
 Project-URL: Homepage, https://github.com/laviolette-lab/lavlab-python-utils
 Project-URL: Bug Tracker, https://github.com/laviolette-lab/lavlab-python-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lavlab-python-utils-1.2.1/src/lavlab/omero_asyncio.py` & `lavlab-python-utils-1.2.2/src/lavlab/omero_asyncio.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.2.1/src/lavlab/omero_util.py` & `lavlab-python-utils-1.2.2/src/lavlab/omero_util.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.2.1/src/lavlab/python_util.py` & `lavlab-python-utils-1.2.2/src/lavlab/python_util.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.2.1/src/lavlab_python_utils.egg-info/PKG-INFO` & `lavlab-python-utils-1.2.2/src/lavlab_python_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavlab-python-utils
-Version: 1.2.1
+Version: 1.2.2
 Summary: LaViolette Lab utility package
 Author-email: Michael Barrett <mjbarrett@mcw.edu>
 Project-URL: Homepage, https://github.com/laviolette-lab/lavlab-python-utils
 Project-URL: Bug Tracker, https://github.com/laviolette-lab/lavlab-python-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lavlab-python-utils-1.2.1/test/test_omero_util.py` & `lavlab-python-utils-1.2.2/test/test_omero_util.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.2.1/test/test_python_utils.py` & `lavlab-python-utils-1.2.2/test/test_python_utils.py`

 * *Files identical despite different names*

