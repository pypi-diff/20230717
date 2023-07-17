# Comparing `tmp/airflow_mcd-0.1.5.tar.gz` & `tmp/airflow_mcd-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airflow_mcd-0.1.5.tar", last modified: Tue Jul 11 18:02:10 2023, max compression
+gzip compressed data, was "dist/airflow_mcd-0.1.6.tar", last modified: Mon Jul 17 16:35:49 2023, max compression
```

## Comparing `airflow_mcd-0.1.5.tar` & `airflow_mcd-0.1.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:02:10.851585 airflow_mcd-0.1.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:02:10.851585 airflow_mcd-0.1.5/.circleci/
--rw-r--r--   0 root         (0) root         (0)      168 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/.circleci/README
--rw-r--r--   0 root         (0) root         (0)     3102 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/.circleci/config.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:02:10.851585 airflow_mcd-0.1.5/.circleci/trufflehog_config/
--rw-r--r--   0 root         (0) root         (0)      377 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/.circleci/trufflehog_config/allowlist.json
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     1818 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/.gitignore
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1129 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/Makefile
--rw-r--r--   0 root         (0) root         (0)     7468 2023-07-11 18:02:10.851585 airflow_mcd-0.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/README-dev.md
--rw-r--r--   0 root         (0) root         (0)     6655 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:02:10.851585 airflow_mcd-0.1.5/airflow_mcd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/airflow_mcd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:02:10.851585 airflow_mcd-0.1.5/airflow_mcd/callbacks/
--rw-r--r--   0 root         (0) root         (0)     6967 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/airflow_mcd/callbacks/client.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/airflow_mcd/callbacks/mcd_callbacks.py
--rw-r--r--   0 root         (0) root         (0)     5412 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/airflow_mcd/callbacks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:02:10.851585 airflow_mcd-0.1.5/airflow_mcd/hooks/
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/airflow_mcd/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2784 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/airflow_mcd/hooks/session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:02:10.851585 airflow_mcd-0.1.5/airflow_mcd/operators/
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/airflow_mcd/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/airflow_mcd/operators/base_operator.py
--rw-r--r--   0 root         (0) root         (0)     3895 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/airflow_mcd/operators/circuit_breaker_operators.py
--rw-r--r--   0 root         (0) root         (0)    15263 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/airflow_mcd/operators/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:02:10.851585 airflow_mcd-0.1.5/airflow_mcd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7468 2023-07-11 18:02:10.000000 airflow_mcd-0.1.5/airflow_mcd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1137 2023-07-11 18:02:10.000000 airflow_mcd-0.1.5/airflow_mcd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 18:02:10.000000 airflow_mcd-0.1.5/airflow_mcd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-11 18:02:10.000000 airflow_mcd-0.1.5/airflow_mcd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-11 18:02:10.000000 airflow_mcd-0.1.5/airflow_mcd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:02:10.851585 airflow_mcd-0.1.5/examples/
--rw-r--r--   0 root         (0) root         (0)     2050 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/examples/sample_circuit_dag.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/requirements-ci.txt
--rw-r--r--   0 root         (0) root         (0)      177 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-11 18:02:10.851585 airflow_mcd-0.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1483 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:02:10.851585 airflow_mcd-0.1.5/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:02:10.851585 airflow_mcd-0.1.5/tests/callbacks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/tests/callbacks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12924 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/tests/callbacks/test_callbacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:02:10.851585 airflow_mcd-0.1.5/tests/hooks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/tests/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3780 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/tests/hooks/test_session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:02:10.851585 airflow_mcd-0.1.5/tests/operators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/tests/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      719 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/tests/operators/test_base_op.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/tests/operators/test_circuit_breaker_op.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/tests/operators/test_dbt_cli_config.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/tests/operators/test_dbt_default_config_provider.py
--rw-r--r--   0 root         (0) root         (0)    21136 2023-07-11 18:01:11.000000 airflow_mcd-0.1.5/tests/operators/test_dbt_operator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.253916 airflow_mcd-0.1.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/.circleci/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/.circleci/README
+-rw-r--r--   0 root         (0) root         (0)     3102 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/.circleci/config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/.circleci/trufflehog_config/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/.circleci/trufflehog_config/allowlist.json
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/Makefile
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-07-17 16:35:49.253916 airflow_mcd-0.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/README-dev.md
+-rw-r--r--   0 root         (0) root         (0)     6655 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/airflow_mcd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/airflow_mcd/callbacks/
+-rw-r--r--   0 root         (0) root         (0)     6967 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/callbacks/client.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/callbacks/mcd_callbacks.py
+-rw-r--r--   0 root         (0) root         (0)     5412 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/callbacks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/airflow_mcd/hooks/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2784 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/hooks/session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/airflow_mcd/operators/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/operators/base_operator.py
+-rw-r--r--   0 root         (0) root         (0)     3895 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/operators/circuit_breaker_operators.py
+-rw-r--r--   0 root         (0) root         (0)    15407 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/airflow_mcd/operators/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/airflow_mcd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-07-17 16:35:49.000000 airflow_mcd-0.1.6/airflow_mcd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-07-17 16:35:49.000000 airflow_mcd-0.1.6/airflow_mcd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 16:35:49.000000 airflow_mcd-0.1.6/airflow_mcd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-17 16:35:49.000000 airflow_mcd-0.1.6/airflow_mcd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-17 16:35:49.000000 airflow_mcd-0.1.6/airflow_mcd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/examples/
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/examples/sample_circuit_dag.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/requirements-ci.txt
+-rw-r--r--   0 root         (0) root         (0)      177 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-17 16:35:49.253916 airflow_mcd-0.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.249916 airflow_mcd-0.1.6/tests/callbacks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/callbacks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12924 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/callbacks/test_callbacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.253916 airflow_mcd-0.1.6/tests/hooks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/hooks/test_session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:35:49.253916 airflow_mcd-0.1.6/tests/operators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/operators/test_base_op.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/operators/test_circuit_breaker_op.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/operators/test_dbt_cli_config.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/operators/test_dbt_default_config_provider.py
+-rw-r--r--   0 root         (0) root         (0)    21136 2023-07-17 16:34:47.000000 airflow_mcd-0.1.6/tests/operators/test_dbt_operator.py
```

### Comparing `airflow_mcd-0.1.5/.circleci/config.yml` & `airflow_mcd-0.1.6/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/.gitignore` & `airflow_mcd-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/LICENSE` & `airflow_mcd-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/Makefile` & `airflow_mcd-0.1.6/Makefile`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/PKG-INFO` & `airflow_mcd-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow_mcd
-Version: 0.1.5
+Version: 0.1.6
 Summary: Monte Carlo's Apache Airflow Provider
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `airflow_mcd-0.1.5/README-dev.md` & `airflow_mcd-0.1.6/README-dev.md`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/README.md` & `airflow_mcd-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/airflow_mcd/callbacks/client.py` & `airflow_mcd-0.1.6/airflow_mcd/callbacks/client.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/airflow_mcd/callbacks/mcd_callbacks.py` & `airflow_mcd-0.1.6/airflow_mcd/callbacks/mcd_callbacks.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/airflow_mcd/callbacks/utils.py` & `airflow_mcd-0.1.6/airflow_mcd/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/airflow_mcd/hooks/session_hook.py` & `airflow_mcd-0.1.6/airflow_mcd/hooks/session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/airflow_mcd/operators/base_operator.py` & `airflow_mcd-0.1.6/airflow_mcd/operators/base_operator.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/airflow_mcd/operators/circuit_breaker_operators.py` & `airflow_mcd-0.1.6/airflow_mcd/operators/circuit_breaker_operators.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/airflow_mcd/operators/dbt.py` & `airflow_mcd-0.1.6/airflow_mcd/operators/dbt.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,14 +355,19 @@
 
 
 class DbtRunOperator(DbtOperator):
     def __init__(self, **kwargs):
         super(DbtRunOperator, self).__init__(command="run", **kwargs)
 
 
+class DbtSeedOperator(DbtOperator):
+    def __init__(self, **kwargs):
+        super(DbtSeedOperator, self).__init__(command="seed", **kwargs)
+
+
 class DbtSnapshotOperator(DbtOperator):
     def __init__(self, **kwargs):
         super(DbtSnapshotOperator, self).__init__(command="snapshot", **kwargs)
 
 
 class DbtTestOperator(DbtOperator):
     def __init__(self, **kwargs):
```

### Comparing `airflow_mcd-0.1.5/airflow_mcd.egg-info/PKG-INFO` & `airflow_mcd-0.1.6/airflow_mcd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-mcd
-Version: 0.1.5
+Version: 0.1.6
 Summary: Monte Carlo's Apache Airflow Provider
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `airflow_mcd-0.1.5/airflow_mcd.egg-info/SOURCES.txt` & `airflow_mcd-0.1.6/airflow_mcd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/examples/sample_circuit_dag.py` & `airflow_mcd-0.1.6/examples/sample_circuit_dag.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/setup.py` & `airflow_mcd-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/tests/callbacks/test_callbacks.py` & `airflow_mcd-0.1.6/tests/callbacks/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/tests/hooks/test_session_hook.py` & `airflow_mcd-0.1.6/tests/hooks/test_session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/tests/operators/test_base_op.py` & `airflow_mcd-0.1.6/tests/operators/test_base_op.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/tests/operators/test_circuit_breaker_op.py` & `airflow_mcd-0.1.6/tests/operators/test_circuit_breaker_op.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/tests/operators/test_dbt_cli_config.py` & `airflow_mcd-0.1.6/tests/operators/test_dbt_cli_config.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/tests/operators/test_dbt_default_config_provider.py` & `airflow_mcd-0.1.6/tests/operators/test_dbt_default_config_provider.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.5/tests/operators/test_dbt_operator.py` & `airflow_mcd-0.1.6/tests/operators/test_dbt_operator.py`

 * *Files identical despite different names*

