# Comparing `tmp/trubrics-1.4.2.tar.gz` & `tmp/trubrics-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trubrics-1.4.2.tar", last modified: Wed Jul  5 09:01:17 2023, max compression
+gzip compressed data, was "trubrics-1.4.3.tar", last modified: Mon Jul 17 11:10:39 2023, max compression
```

## Comparing `trubrics-1.4.2.tar` & `trubrics-1.4.3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.962143 trubrics-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-05 09:01:06.000000 trubrics-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-05 09:01:17.962143 trubrics-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-05 09:01:06.000000 trubrics-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.954143 trubrics-1.4.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:06.000000 trubrics-1.4.2/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.954143 trubrics-1.4.2/examples/feedback/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:06.000000 trubrics-1.4.2/examples/feedback/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.954143 trubrics-1.4.2/examples/feedback/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:06.000000 trubrics-1.4.2/examples/feedback/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-05 09:01:06.000000 trubrics-1.4.2/examples/feedback/streamlit/llm_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-05 09:01:06.000000 trubrics-1.4.2/examples/feedback/streamlit/titanic_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-05 09:01:06.000000 trubrics-1.4.2/examples/feedback/streamlit/trubrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-05 09:01:06.000000 trubrics-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-05 09:01:06.000000 trubrics-1.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-05 09:01:17.962143 trubrics-1.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.954143 trubrics-1.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-05 09:01:06.000000 trubrics-1.4.2/tests/test_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.954143 trubrics-1.4.2/trubrics/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.954143 trubrics-1.4.2/trubrics/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/example/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/example/my_first_trubric.json
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/example/titanic.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/example/titanic_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/example/titanic_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/example/trubric_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/feedback/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/feedback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/feedback/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/feedback/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/feedback/save_to_trubrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/integrations/dash/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/dash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/dash/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/integrations/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/gradio/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/integrations/mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/mlflow/trubrics_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/integrations/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/streamlit/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/integrations/streamlit/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/trubrics_platform/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/trubrics_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/trubrics_platform/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/trubrics_platform/firestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/trubrics_platform/trubrics_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/utils/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/validations/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/validations/dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.958143 trubrics-1.4.2/trubrics/validations/model/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/validations/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/validations/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/validations/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-05 09:01:06.000000 trubrics-1.4.2/trubrics/validations/validation_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:01:17.954143 trubrics-1.4.2/trubrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-05 09:01:17.000000 trubrics-1.4.2/trubrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-05 09:01:17.000000 trubrics-1.4.2/trubrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:01:17.000000 trubrics-1.4.2/trubrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 09:01:17.000000 trubrics-1.4.2/trubrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-05 09:01:17.000000 trubrics-1.4.2/trubrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 09:01:17.000000 trubrics-1.4.2/trubrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.143630 trubrics-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-17 11:10:24.000000 trubrics-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-17 11:10:39.143630 trubrics-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-17 11:10:24.000000 trubrics-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:24.000000 trubrics-1.4.3/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/examples/feedback/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:24.000000 trubrics-1.4.3/examples/feedback/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/examples/feedback/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:24.000000 trubrics-1.4.3/examples/feedback/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-17 11:10:24.000000 trubrics-1.4.3/examples/feedback/streamlit/llm_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-17 11:10:24.000000 trubrics-1.4.3/examples/feedback/streamlit/titanic_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-17 11:10:24.000000 trubrics-1.4.3/examples/feedback/streamlit/trubrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-17 11:10:24.000000 trubrics-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 11:10:24.000000 trubrics-1.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-17 11:10:39.143630 trubrics-1.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-17 11:10:24.000000 trubrics-1.4.3/tests/test_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/trubrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/trubrics/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/trubrics/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/example/my_first_trubric.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/example/titanic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/example/titanic_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/example/titanic_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/example/trubric_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/trubrics/feedback/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/feedback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/feedback/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/feedback/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/feedback/save_to_trubrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/trubrics/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/trubrics/integrations/dash/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/dash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/dash/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/trubrics/integrations/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/gradio/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.143630 trubrics-1.4.3/trubrics/integrations/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/mlflow/trubrics_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.143630 trubrics-1.4.3/trubrics/integrations/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/streamlit/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/streamlit/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.143630 trubrics-1.4.3/trubrics/trubrics_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/trubrics_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/trubrics_platform/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/trubrics_platform/firestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/trubrics_platform/trubrics_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.143630 trubrics-1.4.3/trubrics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/utils/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.143630 trubrics-1.4.3/trubrics/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/validations/dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.143630 trubrics-1.4.3/trubrics/validations/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/validations/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/validations/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/validations/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/validations/validation_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/trubrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-17 11:10:39.000000 trubrics-1.4.3/trubrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-17 11:10:39.000000 trubrics-1.4.3/trubrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:10:39.000000 trubrics-1.4.3/trubrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-17 11:10:39.000000 trubrics-1.4.3/trubrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-17 11:10:39.000000 trubrics-1.4.3/trubrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 11:10:39.000000 trubrics-1.4.3/trubrics.egg-info/top_level.txt
```

### Comparing `trubrics-1.4.2/LICENSE` & `trubrics-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/README.md` & `trubrics-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/examples/feedback/streamlit/llm_app.py` & `trubrics-1.4.3/examples/feedback/streamlit/llm_app.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/examples/feedback/streamlit/titanic_app.py` & `trubrics-1.4.3/examples/feedback/streamlit/titanic_app.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/examples/feedback/streamlit/trubrics_utils.py` & `trubrics-1.4.3/examples/feedback/streamlit/trubrics_utils.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/setup.cfg` & `trubrics-1.4.3/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trubrics
-version = 1.4.2
+version = 1.4.3
 description = The first user insights platform for AI models.
 long_description = Full documentation available at https://trubrics.github.io/trubrics-sdk/.
 
 [options]
 packages = find:
 install_requires = file: requirements.txt
 
@@ -28,12 +28,13 @@
 profile = black
 
 [options.extras_require]
 streamlit = streamlit>=1.20.0
 dash = dash>=2.6.2; dash-bootstrap-components>=1.2.1
 gradio = gradio>=3.8.1
 mlflow = mlflow>=2.0.0
+validations = GitPython>=3.1.31; numpy>=1.21.6; pandas>=1.3.5; scikit-learn>=1.0.0,<1.1.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `trubrics-1.4.2/tests/test_context.py` & `trubrics-1.4.3/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/cli/main.py` & `trubrics-1.4.3/trubrics/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from pathlib import Path
 
 import typer
 from rich import print as rprint
 
-from trubrics.cli.run import validate_trubric_run_context
-from trubrics.trubrics_platform.trubrics_config import TrubricsDefaults
-
 app = typer.Typer(pretty_exceptions_show_locals=False)
 
 
 def version_callback(value: bool):
     if value:
         import trubrics
 
@@ -37,14 +34,17 @@
 
     Args:
         save_ui: whether to save validations to the UI with in app user authentication
         run_context_path: path to the trubrics run context
         trubric_output_file_path: path to save your output trubric file
         raise_on_failure: raise an exception on failure of trubric
     """
+    from trubrics.cli.run import validate_trubric_run_context
+    from trubrics.trubrics_platform.trubrics_config import TrubricsDefaults
+
     trubric_run_path = None
     if run_context_path != "example":
         trubric_run_path = Path(run_context_path).absolute()
         if not trubric_run_path.exists():
             rprint(f"[red]Path '{trubric_run_path}' not found.[red]")
             raise typer.Abort()
         rc = validate_trubric_run_context(str(trubric_run_path)).RUN_CONTEXT
```

### Comparing `trubrics-1.4.2/trubrics/cli/run.py` & `trubrics-1.4.3/trubrics/cli/run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/context.py` & `trubrics-1.4.3/trubrics/context.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/example/my_first_trubric.json` & `trubrics-1.4.3/trubrics/example/my_first_trubric.json`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/example/titanic.py` & `trubrics-1.4.3/trubrics/example/titanic.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/example/titanic_data.csv` & `trubrics-1.4.3/trubrics/example/titanic_data.csv`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/example/trubric_run.py` & `trubrics-1.4.3/trubrics/example/trubric_run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/exceptions.py` & `trubrics-1.4.3/trubrics/exceptions.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/feedback/config.py` & `trubrics-1.4.3/trubrics/feedback/config.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/feedback/dataclass.py` & `trubrics-1.4.3/trubrics/feedback/dataclass.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/feedback/save_to_trubrics.py` & `trubrics-1.4.3/trubrics/feedback/save_to_trubrics.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/integrations/dash/collect.py` & `trubrics-1.4.3/trubrics/integrations/dash/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/integrations/gradio/collect.py` & `trubrics-1.4.3/trubrics/integrations/gradio/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/integrations/mlflow/trubrics_validator.py` & `trubrics-1.4.3/trubrics/integrations/mlflow/trubrics_validator.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/integrations/streamlit/collect.py` & `trubrics-1.4.3/trubrics/integrations/streamlit/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/integrations/streamlit/experiment.py` & `trubrics-1.4.3/trubrics/integrations/streamlit/experiment.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/trubrics_platform/auth.py` & `trubrics-1.4.3/trubrics/trubrics_platform/auth.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/trubrics_platform/firestore.py` & `trubrics-1.4.3/trubrics/trubrics_platform/firestore.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/trubrics_platform/trubrics_config.py` & `trubrics-1.4.3/trubrics/trubrics_platform/trubrics_config.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/validations/dataclass.py` & `trubrics-1.4.3/trubrics/validations/dataclass.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/validations/model/base.py` & `trubrics-1.4.3/trubrics/validations/model/base.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/validations/run.py` & `trubrics-1.4.3/trubrics/validations/run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics/validations/validation_output.py` & `trubrics-1.4.3/trubrics/validations/validation_output.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.2/trubrics.egg-info/SOURCES.txt` & `trubrics-1.4.3/trubrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

