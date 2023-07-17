# Comparing `tmp/dkist-processing-test-1.4.1rc1.tar.gz` & `tmp/dkist-processing-test-1.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-test-1.4.1rc1.tar", last modified: Tue Jul 11 18:24:46 2023, max compression
+gzip compressed data, was "dkist-processing-test-1.4.2rc1.tar", last modified: Mon Jul 17 18:26:58 2023, max compression
```

## Comparing `dkist-processing-test-1.4.1rc1.tar` & `dkist-processing-test-1.4.2rc1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 18:24:46.728165 dkist-processing-test-1.4.1rc1/
--rw-rw-rw-   0 root         (0) root         (0)     2417 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1980 2023-07-11 18:24:46.728165 dkist-processing-test-1.4.1rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2358 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 18:24:46.728165 dkist-processing-test-1.4.1rc1/dkist_processing_test/
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 18:24:46.728165 dkist-processing-test-1.4.1rc1/dkist_processing_test/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/models/parameters.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 18:24:46.728165 dkist-processing-test-1.4.1rc1/dkist_processing_test/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1371 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/tasks/exercise_numba.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/tasks/fail.py
--rw-rw-rw-   0 root         (0) root         (0)     3472 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/tasks/fake_science.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/tasks/movie.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/tasks/noop.py
--rw-rw-rw-   0 root         (0) root         (0)     2293 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/tasks/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1140 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2048 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 18:24:46.728165 dkist-processing-test-1.4.1rc1/dkist_processing_test/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2411 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    16665 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/tests/test_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 18:24:46.728165 dkist-processing-test-1.4.1rc1/dkist_processing_test/workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5072 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/workflows/common_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2093 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/workflows/end_to_end.py
--rw-rw-rw-   0 root         (0) root         (0)      362 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/workflows/exercise_numba.py
--rw-rw-rw-   0 root         (0) root         (0)      331 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/workflows/fail.py
--rw-rw-rw-   0 root         (0) root         (0)      676 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/workflows/noop.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test/workflows/trial_end_to_end.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 18:24:46.728165 dkist-processing-test-1.4.1rc1/dkist_processing_test.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1980 2023-07-11 18:24:46.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1369 2023-07-11 18:24:46.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-11 18:24:46.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-07-11 18:24:46.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-11 18:24:46.000000 dkist-processing-test-1.4.1rc1/dkist_processing_test.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-11 18:24:46.728165 dkist-processing-test-1.4.1rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-11 18:24:40.000000 dkist-processing-test-1.4.1rc1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:26:58.926018 dkist-processing-test-1.4.2rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     2417 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1980 2023-07-17 18:26:58.926018 dkist-processing-test-1.4.2rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2358 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:26:58.922018 dkist-processing-test-1.4.2rc1/dkist_processing_test/
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:26:58.922018 dkist-processing-test-1.4.2rc1/dkist_processing_test/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/models/parameters.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:26:58.926018 dkist-processing-test-1.4.2rc1/dkist_processing_test/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/tasks/exercise_numba.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/tasks/fail.py
+-rw-rw-rw-   0 root         (0) root         (0)     3472 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/tasks/fake_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/tasks/movie.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/tasks/noop.py
+-rw-rw-rw-   0 root         (0) root         (0)     2293 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/tasks/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:26:58.926018 dkist-processing-test-1.4.2rc1/dkist_processing_test/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2411 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    16665 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/tests/test_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:26:58.926018 dkist-processing-test-1.4.2rc1/dkist_processing_test/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5072 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/workflows/common_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/workflows/end_to_end.py
+-rw-rw-rw-   0 root         (0) root         (0)      362 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/workflows/exercise_numba.py
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/workflows/fail.py
+-rw-rw-rw-   0 root         (0) root         (0)      676 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/workflows/noop.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test/workflows/trial_end_to_end.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:26:58.922018 dkist-processing-test-1.4.2rc1/dkist_processing_test.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1980 2023-07-17 18:26:58.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2023-07-17 18:26:58.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-17 18:26:58.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-17 18:26:58.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-17 18:26:58.000000 dkist-processing-test-1.4.2rc1/dkist_processing_test.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-07-17 18:26:58.926018 dkist-processing-test-1.4.2rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-17 18:26:52.000000 dkist-processing-test-1.4.2rc1/setup.py
```

### Comparing `dkist-processing-test-1.4.1rc1/.gitignore` & `dkist-processing-test-1.4.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/.pre-commit-config.yaml` & `dkist-processing-test-1.4.2rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/PKG-INFO` & `dkist-processing-test-1.4.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-test
-Version: 1.4.1rc1
+Version: 1.4.2rc1
 Summary: Example Instrument code that is used by the DKIST Science Data Processing pipelines to test processing infrastructure.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-test/src/main/
 Author: NSO / AURA
 Author-email: dkistdc@nso.edu
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-processing-test-1.4.1rc1/README.rst` & `dkist-processing-test-1.4.2rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/bitbucket-pipelines.yml` & `dkist-processing-test-1.4.2rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/dkist_processing_test/models/parameters.py` & `dkist-processing-test-1.4.2rc1/dkist_processing_test/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/dkist_processing_test/tasks/exercise_numba.py` & `dkist-processing-test-1.4.2rc1/dkist_processing_test/tasks/exercise_numba.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/dkist_processing_test/tasks/fake_science.py` & `dkist-processing-test-1.4.2rc1/dkist_processing_test/tasks/fake_science.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/dkist_processing_test/tasks/movie.py` & `dkist-processing-test-1.4.2rc1/dkist_processing_test/tasks/movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/dkist_processing_test/tasks/parse.py` & `dkist-processing-test-1.4.2rc1/dkist_processing_test/tasks/parse.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/dkist_processing_test/tasks/trial_output_data.py` & `dkist-processing-test-1.4.2rc1/dkist_processing_test/tasks/trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/dkist_processing_test/tasks/write_l1.py` & `dkist-processing-test-1.4.2rc1/dkist_processing_test/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/dkist_processing_test/tests/conftest.py` & `dkist-processing-test-1.4.2rc1/dkist_processing_test/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/dkist_processing_test/tests/test_parameters.py` & `dkist-processing-test-1.4.2rc1/dkist_processing_test/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/dkist_processing_test/tests/test_tasks.py` & `dkist-processing-test-1.4.2rc1/dkist_processing_test/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/dkist_processing_test/workflows/common_tasks.py` & `dkist-processing-test-1.4.2rc1/dkist_processing_test/workflows/common_tasks.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/dkist_processing_test/workflows/end_to_end.py` & `dkist-processing-test-1.4.2rc1/dkist_processing_test/workflows/end_to_end.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/dkist_processing_test/workflows/noop.py` & `dkist-processing-test-1.4.2rc1/dkist_processing_test/workflows/noop.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/dkist_processing_test/workflows/trial_end_to_end.py` & `dkist-processing-test-1.4.2rc1/dkist_processing_test/workflows/trial_end_to_end.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/dkist_processing_test.egg-info/PKG-INFO` & `dkist-processing-test-1.4.2rc1/dkist_processing_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-test
-Version: 1.4.1rc1
+Version: 1.4.2rc1
 Summary: Example Instrument code that is used by the DKIST Science Data Processing pipelines to test processing infrastructure.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-test/src/main/
 Author: NSO / AURA
 Author-email: dkistdc@nso.edu
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-processing-test-1.4.1rc1/dkist_processing_test.egg-info/SOURCES.txt` & `dkist-processing-test-1.4.2rc1/dkist_processing_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.4.1rc1/setup.cfg` & `dkist-processing-test-1.4.2rc1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 [options]
 python_requires = >=3.11
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	dkist-processing-common == 4.0.1rc1
-	dkist-header-validator == 3.0.5
+	dkist-processing-common == 4.0.2rc1
+	dkist-header-validator == 4.0.0rc2
 	dkist-fits-specifications == 3.6.0
 	numba == 0.57.1
 	astropy == 5.3.0
 	numpy == 1.24.3
 	dkist-spectral-lines == 2.0.0
 
 [options.extras_require]
```

