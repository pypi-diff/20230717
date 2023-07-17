# Comparing `tmp/ghga_connector-0.3.7.tar.gz` & `tmp/ghga_connector-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_connector-0.3.7.tar", last modified: Thu Jul 13 11:04:21 2023, max compression
+gzip compressed data, was "ghga_connector-0.3.8.tar", last modified: Mon Jul 17 14:17:11 2023, max compression
```

## Comparing `ghga_connector-0.3.7.tar` & `ghga_connector-0.3.8.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.022512 ghga_connector-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-07-13 11:04:21.022512 ghga_connector-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.014511 ghga_connector-0.3.7/ghga_connector/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.014511 ghga_connector-0.3.7/ghga_connector/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.014511 ghga_connector-0.3.7/ghga_connector/core/api_calls/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/api_calls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/api_calls/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/api_calls/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/api_calls/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/api_calls/well_knowns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/api_calls/work_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/batch_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/file_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/http_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/ghga_connector/core/message_display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.014511 ghga_connector-0.3.7/ghga_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-07-13 11:04:20.000000 ghga_connector-0.3.7/ghga_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-13 11:04:21.000000 ghga_connector-0.3.7/ghga_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:04:20.000000 ghga_connector-0.3.7/ghga_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-13 11:04:20.000000 ghga_connector-0.3.7/ghga_connector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:04:20.000000 ghga_connector-0.3.7/ghga_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-13 11:04:20.000000 ghga_connector-0.3.7/ghga_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 11:04:20.000000 ghga_connector-0.3.7/ghga_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.018512 ghga_connector-0.3.7/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/scripts/get_package_name.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18568 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/scripts/license_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.018512 ghga_connector-0.3.7/scripts/script_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/scripts/script_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/scripts/script_utils/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4972 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/scripts/update_config_docs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6729 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/scripts/update_readme.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8499 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/scripts/update_template_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-13 11:04:21.022512 ghga_connector-0.3.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.010511 ghga_connector-0.3.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.018512 ghga_connector-0.3.7/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/fixtures/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/fixtures/endpoints_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.018512 ghga_connector-0.3.7/tests/fixtures/mock_api/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/fixtures/mock_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14443 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/fixtures/mock_api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/fixtures/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/fixtures/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/fixtures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.018512 ghga_connector-0.3.7/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.018512 ghga_connector-0.3.7/tests/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/integration/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/integration/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16502 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/integration/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/integration/test_file_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.018512 ghga_connector-0.3.7/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:21.022512 ghga_connector-0.3.7/tests/unit/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/unit/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/unit/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/unit/test_api_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/unit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 11:04:03.000000 ghga_connector-0.3.7/tests/unit/test_file_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.611518 ghga_connector-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-07-17 14:17:11.611518 ghga_connector-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.603518 ghga_connector-0.3.8/ghga_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.603518 ghga_connector-0.3.8/ghga_connector/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.607518 ghga_connector-0.3.8/ghga_connector/core/api_calls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/api_calls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/api_calls/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/api_calls/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/api_calls/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/api_calls/well_knowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/api_calls/work_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/batch_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/http_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/message_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.603518 ghga_connector-0.3.8/ghga_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-07-17 14:17:11.000000 ghga_connector-0.3.8/ghga_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-17 14:17:11.000000 ghga_connector-0.3.8/ghga_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:17:11.000000 ghga_connector-0.3.8/ghga_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-17 14:17:11.000000 ghga_connector-0.3.8/ghga_connector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:17:11.000000 ghga_connector-0.3.8/ghga_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 14:17:11.000000 ghga_connector-0.3.8/ghga_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 14:17:11.000000 ghga_connector-0.3.8/ghga_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.607518 ghga_connector-0.3.8/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/scripts/get_package_name.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18568 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/scripts/license_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.607518 ghga_connector-0.3.8/scripts/script_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/scripts/script_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/scripts/script_utils/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4972 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/scripts/update_config_docs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6729 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/scripts/update_readme.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8499 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/scripts/update_template_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-17 14:17:11.615518 ghga_connector-0.3.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.599518 ghga_connector-0.3.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.611518 ghga_connector-0.3.8/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/fixtures/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/fixtures/endpoints_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.611518 ghga_connector-0.3.8/tests/fixtures/mock_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/fixtures/mock_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/fixtures/mock_api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/fixtures/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/fixtures/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/fixtures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.611518 ghga_connector-0.3.8/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.611518 ghga_connector-0.3.8/tests/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/integration/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/integration/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16425 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/integration/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/integration/test_file_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.611518 ghga_connector-0.3.8/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.611518 ghga_connector-0.3.8/tests/unit/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/unit/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/unit/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/unit/test_api_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/unit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/unit/test_file_operations.py
```

### Comparing `ghga_connector-0.3.7/LICENSE` & `ghga_connector-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/PKG-INFO` & `ghga_connector-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_connector
-Version: 0.3.7
+Version: 0.3.8
 Summary: GHGA Connector - A CLI client application for interacting with the GHGA system.
 Home-page: https://github.com/ghga-de/ghga-connector
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -41,29 +41,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-connector):
 ```bash
-docker pull ghga/ghga-connector:0.3.7
+docker pull ghga/ghga-connector:0.3.8
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-connector:0.3.7 .
+docker build -t ghga/ghga-connector:0.3.8 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-connector:0.3.7 --help
+docker run -p 8080:8080 ghga/ghga-connector:0.3.8 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
 
@@ -77,15 +77,15 @@
 The service requires the following configuration parameters:
 - **`max_retries`** *(integer)*: Number of times to retry failed API calls. Default: `5`.
 
 - **`max_wait_time`** *(integer)*: Maximal time in seconds to wait before quitting without a download. Default: `3600`.
 
 - **`part_size`** *(integer)*: The part size to use for download. Default: `16777216`.
 
-- **`wkvs_api_url`** *(string)*: URL to the root of the WKVS API. Should start with https://.
+- **`wkvs_api_url`** *(string)*: URL to the root of the WKVS API. Should start with https://. Default: `https://data.ghga.de/.well-known`.
 
 
 ### Usage:
 
 A template YAML for configurating the service can be found at
 [`./example-config.yaml`](./example-config.yaml).
 Please adapt it, rename it to `.ghga_connector.yaml`, and place it into one of the following locations:
```

### Comparing `ghga_connector-0.3.7/README.md` & `ghga_connector-0.3.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,29 +24,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-connector):
 ```bash
-docker pull ghga/ghga-connector:0.3.7
+docker pull ghga/ghga-connector:0.3.8
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-connector:0.3.7 .
+docker build -t ghga/ghga-connector:0.3.8 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-connector:0.3.7 --help
+docker run -p 8080:8080 ghga/ghga-connector:0.3.8 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
 
@@ -60,15 +60,15 @@
 The service requires the following configuration parameters:
 - **`max_retries`** *(integer)*: Number of times to retry failed API calls. Default: `5`.
 
 - **`max_wait_time`** *(integer)*: Maximal time in seconds to wait before quitting without a download. Default: `3600`.
 
 - **`part_size`** *(integer)*: The part size to use for download. Default: `16777216`.
 
-- **`wkvs_api_url`** *(string)*: URL to the root of the WKVS API. Should start with https://.
+- **`wkvs_api_url`** *(string)*: URL to the root of the WKVS API. Should start with https://. Default: `https://data.ghga.de/.well-known`.
 
 
 ### Usage:
 
 A template YAML for configurating the service can be found at
 [`./example-config.yaml`](./example-config.yaml).
 Please adapt it, rename it to `.ghga_connector.yaml`, and place it into one of the following locations:
```

### Comparing `ghga_connector-0.3.7/ghga_connector/__init__.py` & `ghga_connector-0.3.8/ghga_connector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 CLI - Client to perform up- and download operations to and from a local ghga instance
 """
 
-__version__ = "0.3.7"
+__version__ = "0.3.8"
```

### Comparing `ghga_connector-0.3.7/ghga_connector/__main__.py` & `ghga_connector-0.3.8/ghga_connector/__main__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/ghga_connector/cli.py` & `ghga_connector-0.3.8/ghga_connector/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -59,20 +59,20 @@
 cli = typer.Typer(no_args_is_help=True)
 
 
 def upload(  # noqa C901
     *,
     file_id: str = typer.Option(..., help="The id of the file to upload"),
     file_path: Path = typer.Option(..., help="The path to the file to upload"),
-    submitter_pubkey_path: Path = typer.Argument(
+    my_public_key_path: Path = typer.Option(
         "./key.pub",
         help="The path to a public key from the key pair that was announced in the "
         + "metadata. Defaults to key.pub in the current folder.",
     ),
-    submitter_private_key_path: Path = typer.Argument(
+    my_private_key_path: Path = typer.Option(
         "./key.sec",
         help="The path to a private key from the key pair that will be used to encrypt the "
         + "crypt4gh envelope. Defaults to key.sec in the current folder.",
     ),
     debug: bool = typer.Option(
         False, help="Set this option in order to view traceback for errors."
     ),
@@ -91,35 +91,35 @@
 
     core.upload(
         api_url=ucs_api_url,
         file_id=file_id,
         file_path=file_path,
         message_display=CLIMessageDisplay(),
         server_pubkey=server_pubkey,
-        submitter_pubkey_path=submitter_pubkey_path,
-        submitter_private_key_path=submitter_private_key_path,
+        my_public_key_path=my_public_key_path,
+        my_private_key_path=my_private_key_path,
     )
 
 
 if strtobool(os.getenv("UPLOAD_ENABLED") or "false"):
-    cli.command()(upload)
+    cli.command(no_args_is_help=True)(upload)
 
 
-@cli.command()
+@cli.command(no_args_is_help=True)
 def download(  # pylint: disable=too-many-arguments,too-many-locals
     *,
     output_dir: Path = typer.Option(
         ..., help="The directory to put the downloaded files into."
     ),
-    submitter_pubkey_path: Path = typer.Argument(
+    my_public_key_path: Path = typer.Option(
         "./key.pub",
-        help="The path to a public key from the key pair that was announced in the "
-        + "metadata. Defaults to key.pub in the current folder.",
+        help="The path to a public key from the key pair that was announced when the "
+        + "download token was created. Defaults to key.pub in the current folder.",
     ),
-    submitter_private_key_path: Path = typer.Argument(
+    my_private_key_path: Path = typer.Option(
         "./key.sec",
         help="The path to a private key from the key pair that will be used to decrypt "
         + "the work package access token and work order token. Defaults to key.sec in "
         + "the current folder.",
     ),
     debug: bool = typer.Option(
         False, help="Set this option in order to view traceback for errors."
@@ -130,45 +130,45 @@
     """
     if not debug:
         sys.excepthook = lambda x, y, z: None
 
     core.HttpxClientState.configure(CONFIG.max_retries)
     message_display = CLIMessageDisplay()
 
-    if not submitter_pubkey_path.is_file():
-        message_display.failure(f"The file '{submitter_pubkey_path}' does not exist.")
+    if not my_public_key_path.is_file():
+        message_display.failure(f"The file '{my_public_key_path}' does not exist.")
         raise core.exceptions.PubKeyFileDoesNotExistError(
-            pubkey_path=submitter_pubkey_path
+            pubkey_path=my_public_key_path
         )
 
     if not output_dir.is_dir():
         message_display.failure(f"The directory '{output_dir}' does not exist.")
         raise core.exceptions.DirectoryDoesNotExistError(output_dir=output_dir)
 
-    submitter_public_key = crypt4gh.keys.get_public_key(filepath=submitter_pubkey_path)
-    submitter_private_key = crypt4gh.keys.get_private_key(
-        filepath=submitter_private_key_path, callback=None
+    my_public_key = crypt4gh.keys.get_public_key(filepath=my_public_key_path)
+    my_private_key = crypt4gh.keys.get_private_key(
+        filepath=my_private_key_path, callback=None
     )
 
     # get work package access token and id from user input, will be used in later PR
     work_package_id, work_package_token = core.main.get_wps_token(
         max_tries=3, message_display=message_display
     )
-    decrypted_token = crypt.decrypt(data=work_package_token, key=submitter_private_key)
+    decrypted_token = crypt.decrypt(data=work_package_token, key=my_private_key)
 
     wkvs_caller = core.WKVSCaller(CONFIG.wkvs_api_url)
     wps_api_url = wkvs_caller.get_wps_api_url()
     dcs_api_url = wkvs_caller.get_dcs_api_url()
 
     work_package_accessor = core.WorkPackageAccessor(
         access_token=decrypted_token,
         api_url=wps_api_url,
         dcs_api_url=dcs_api_url,
         package_id=work_package_id,
-        submitter_private_key=submitter_private_key,
+        my_private_key=my_private_key,
     )
     file_ids_with_extension = work_package_accessor.get_package_files()
 
     io_handler = core.CliIoHandler()
     staging_parameters = core.StagingParameters(
         api_url=dcs_api_url,
         file_ids_with_extension=file_ids_with_extension,
@@ -189,21 +189,21 @@
                 api_url=dcs_api_url,
                 file_id=file_id,
                 file_extension=file_ids_with_extension[file_id],
                 output_dir=output_dir,
                 max_wait_time=CONFIG.max_wait_time,
                 part_size=CONFIG.part_size,
                 message_display=message_display,
-                submitter_public_key=submitter_public_key,
+                my_public_key=my_public_key,
                 work_package_accessor=work_package_accessor,
             )
         file_stager.update_staged_files()
 
 
-@cli.command()
+@cli.command(no_args_is_help=True)
 def decrypt(  # noqa: C901 # pylint: disable=too-many-branches
     *,
     input_dir: Path = typer.Option(
         ...,
         help="Path to the directory containing files that should be decrypted using a "
         + "common decryption key.",
     ),
```

### Comparing `ghga_connector-0.3.7/ghga_connector/config.py` & `ghga_connector-0.3.8/ghga_connector/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,9 +33,10 @@
         MAX_WAIT_TIME,
         description="Maximal time in seconds to wait before quitting without a download.",
     )
     part_size: int = Field(
         DEFAULT_PART_SIZE, description="The part size to use for download."
     )
     wkvs_api_url: str = Field(
-        ..., description="URL to the root of the WKVS API. Should start with https://"
+        "https://data.ghga.de/.well-known",
+        description="URL to the root of the WKVS API. Should start with https://",
     )
```

### Comparing `ghga_connector-0.3.7/ghga_connector/core/__init__.py` & `ghga_connector-0.3.8/ghga_connector/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/ghga_connector/core/api_calls/__init__.py` & `ghga_connector-0.3.8/ghga_connector/core/api_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/ghga_connector/core/api_calls/download.py` & `ghga_connector-0.3.8/ghga_connector/core/api_calls/download.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/ghga_connector/core/api_calls/upload.py` & `ghga_connector-0.3.8/ghga_connector/core/api_calls/upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     """
 
     # build url and headers
     url = f"{api_url}/uploads"
     headers = {"Accept": "application/json", "Content-Type": "application/json"}
     public_key = base64.b64encode(crypt4gh.keys.get_public_key(pubkey_path)).decode()
 
-    post_data = {"file_id": file_id, "submitter_public_key": public_key}
+    post_data = {"file_id": file_id, "my_public_key": public_key}
     serialized_data = json.dumps(post_data)
 
     # Make function call to get upload url
     try:
         with httpx_client() as client:
             response = client.post(
                 url=url, headers=headers, content=serialized_data, timeout=TIMEOUT
```

### Comparing `ghga_connector-0.3.7/ghga_connector/core/api_calls/utils.py` & `ghga_connector-0.3.8/ghga_connector/core/api_calls/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/ghga_connector/core/api_calls/well_knowns.py` & `ghga_connector-0.3.8/ghga_connector/core/api_calls/well_knowns.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/ghga_connector/core/api_calls/work_package.py` & `ghga_connector-0.3.8/ghga_connector/core/api_calls/work_package.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class WorkPackageAccessor:
     """Wrapper for WPS associated API call parameters"""
 
     access_token: str
     api_url: str
     dcs_api_url: str
     package_id: str
-    submitter_private_key: str
+    my_private_key: str
 
     def get_package_files(self) -> dict[str, str]:
         """
         Call WPS endpoint and retrieve work package information.
         """
 
         url = f"{self.api_url}/work-packages/{self.package_id}"
@@ -83,14 +83,16 @@
         if status_code != 201:
             if status_code == 403:
                 raise exceptions.NoWorkPackageAccessError(
                     work_package_id=self.package_id
                 )
             raise exceptions.InvalidWPSResponseError(url=url, response_code=status_code)
 
-        encrypted_token = response.content
-        return _decrypt(data=encrypted_token, key=self.submitter_private_key)
+        encrypted_token = response.json()
+        if not encrypted_token or not isinstance(encrypted_token, str):
+            raise exceptions.InvalidWPSResponseError(url=url, response_code=status_code)
+        return _decrypt(data=encrypted_token, key=self.my_private_key)
 
 
 def _decrypt(*, data: str, key: str):
     """Factored out decryption so this can be mocked."""
     return decrypt(data=data, key=key)
```

### Comparing `ghga_connector-0.3.7/ghga_connector/core/batch_processing.py` & `ghga_connector-0.3.8/ghga_connector/core/batch_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,15 @@
                 + f" seconds for {len(self.staging_state.unstaged_files)} unstaged file(s)."
             )
             sleep(self.staging_parameters.retry_after)
 
     def _handle_unknown(self, unknown_ids: list[str]):
         """Process user interaction for unknown file IDs"""
         message = (
-            f"No download exists for the following file IDs: {' ,'.join(unknown_ids)}"
+            f"No download exists for the following file IDs: {', '.join(unknown_ids)}"
         )
         self.message_display.failure(message)
 
         unknown_ids_present = (
             "Some of the provided file IDs cannot be downloaded."
             + "\nDo you want to proceed ?\n[Yes][No]\n"
         )
```

### Comparing `ghga_connector-0.3.7/ghga_connector/core/client.py` & `ghga_connector-0.3.8/ghga_connector/core/client.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/ghga_connector/core/constants.py` & `ghga_connector-0.3.8/ghga_connector/core/constants.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/ghga_connector/core/exceptions.py` & `ghga_connector-0.3.8/ghga_connector/core/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     """Thrown, when the specified public key file does not exist."""
 
     def __init__(self, *, pubkey_path: Path):
         message = f"The public key file {pubkey_path} does not exist."
         super().__init__(message)
 
 
-class PubkeyMismatchError(RuntimeError):
+class PubKeyMismatchError(RuntimeError):
     """
     Thrown when the user public key announced in the submission metadata retrieved from
     the work package service does not match the user public key provided to the connector
     """
 
     def __init__(self):
         message = (
@@ -301,15 +301,15 @@
         )
         super().__init__(message)
 
 
 class InvalidWPSResponseError(RuntimeError):
     """
     Thrown when communication with the Work Package Service returns an unexpected response.
-    This should be used instead of BadResponseError when handling WPS results to differntiate
+    This should be used instead of BadResponseError when handling WPS results to differentiate.
     """
 
     def __init__(self, *, url: str, response_code: int):
         self.response_code = response_code
         message = (
             f"The request to the WPS at {url} failed with an unexpected response code "
             + f"of {response_code}."
```

### Comparing `ghga_connector-0.3.7/ghga_connector/core/file_operations.py` & `ghga_connector-0.3.8/ghga_connector/core/file_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,24 +38,24 @@
 
 class Crypt4GHEncryptor:
     """Convenience class to deal with Crypt4GH encryption"""
 
     def __init__(
         self,
         server_pubkey: str,
-        submitter_private_key_path: Path,
+        my_private_key_path: Path,
     ) -> None:
         self.server_public = base64.b64decode(server_pubkey)
-        self.submitter_private = crypt4gh.keys.get_private_key(
-            submitter_private_key_path, callback=None
+        self.my_private_key = crypt4gh.keys.get_private_key(
+            my_private_key_path, callback=None
         )
 
     def encrypt_file(self, *, file_path: Path) -> Path:
         """Encrypt provided file using Crypt4GH lib"""
-        keys = [(0, self.submitter_private, self.server_public)]
+        keys = [(0, self.my_private_key, self.server_public)]
         with file_path.open("rb") as infile:
             # NamedTemporaryFile cannot be opened a second time on Windows, manually
             # deal with setup + teardown instead
             raw_fd, outfile_path = mkstemp()
             with open(raw_fd, "wb") as outfile:
                 crypt4gh.lib.encrypt(keys=keys, infile=infile, outfile=outfile)
             return Path(outfile_path)
```

### Comparing `ghga_connector-0.3.7/ghga_connector/core/http_translation.py` & `ghga_connector-0.3.8/ghga_connector/core/http_translation.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/ghga_connector/core/main.py` & `ghga_connector-0.3.8/ghga_connector/core/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,31 +48,29 @@
 def upload(  # noqa C901, pylint: disable=too-many-statements,too-many-branches
     *,
     api_url: str,
     file_id: str,
     file_path: Path,
     message_display: AbstractMessageDisplay,
     server_pubkey: str,
-    submitter_pubkey_path: Path,
-    submitter_private_key_path: Path,
+    my_public_key_path: Path,
+    my_private_key_path: Path,
 ) -> None:
     """
     Core command to upload a file. Can be called by CLI, GUI, etc.
     """
 
-    if not submitter_pubkey_path.is_file():
-        message_display.failure(f"The file {submitter_pubkey_path} does not exist.")
-        raise exceptions.PubKeyFileDoesNotExistError(pubkey_path=submitter_pubkey_path)
+    if not my_public_key_path.is_file():
+        message_display.failure(f"The file {my_public_key_path} does not exist.")
+        raise exceptions.PubKeyFileDoesNotExistError(pubkey_path=my_public_key_path)
 
-    if not submitter_private_key_path.is_file():
-        message_display.failure(
-            f"The file {submitter_private_key_path} does not exist."
-        )
+    if not my_private_key_path.is_file():
+        message_display.failure(f"The file {my_private_key_path} does not exist.")
         raise exceptions.PrivateKeyFileDoesNotExistError(
-            private_key_path=submitter_private_key_path
+            private_key_path=my_private_key_path
         )
 
     if not file_path.is_file():
         message_display.failure(f"The file {file_path} does not exist.")
         raise exceptions.FileDoesNotExistError(file_path=file_path)
 
     if is_file_encrypted(file_path):
@@ -85,15 +83,15 @@
 
     if not check_url(api_url):
         message_display.failure(f"The url {api_url} is not currently reachable.")
         raise exceptions.ApiNotReachableError(api_url=api_url)
 
     try:
         upload_id, part_size = start_multipart_upload(
-            api_url=api_url, file_id=file_id, pubkey_path=submitter_pubkey_path
+            api_url=api_url, file_id=file_id, pubkey_path=my_public_key_path
         )
     except exceptions.NoUploadPossibleError as error:
         message_display.failure(
             f"This user can't start a multipart upload for the file_id '{file_id}'"
         )
         raise error
     except exceptions.UploadNotRegisteredError as error:
@@ -119,15 +117,15 @@
         raise error
     except exceptions.RequestFailedError as error:
         message_display.failure("The request to start a multipart upload has failed.")
         raise error
 
     encryptor = Crypt4GHEncryptor(
         server_pubkey=server_pubkey,
-        submitter_private_key_path=submitter_private_key_path,
+        my_private_key_path=my_private_key_path,
     )
 
     encrypted_file_path = encryptor.encrypt_file(file_path=file_path)
 
     try:
         upload_file_parts(
             api_url=api_url,
@@ -181,15 +179,15 @@
 def download(  # pylint: disable=too-many-arguments, too-many-locals # noqa: C901, R0914
     *,
     api_url: str,
     output_dir: Path,
     part_size: int,
     message_display: AbstractMessageDisplay,
     max_wait_time: int,
-    submitter_public_key: bytes,
+    my_public_key: bytes,
     work_package_accessor: WorkPackageAccessor,
     file_id: str,
     file_extension: str = "",
 ) -> None:
     """
     Core command to download a file. Can be called by CLI, GUI, etc.
     """
@@ -222,15 +220,15 @@
         work_package_accessor=work_package_accessor,
     )
 
     # get file header envelope
     try:
         envelope = get_file_header_envelope(
             file_id=file_id,
-            public_key=submitter_public_key,
+            public_key=my_public_key,
             work_package_accessor=work_package_accessor,
         )
     except (
         exceptions.FileNotRegisteredError,
         exceptions.EnvelopeNotFoundError,
         exceptions.ExternalApiError,
     ) as error:
@@ -329,21 +327,26 @@
     """
     Expect the work package id and access token as a colon separated string
     The user will have to input this manually to avoid it becomming part of the
     command line history.
     """
     for _ in range(max_tries):
         work_package_string = input(
-            "Paste the complete work package string you got from the UI: "
+            "Please paste the complete download token "
+            + "that you copied from the GHGA data portal: "
         )
         work_package_parts = work_package_string.split(":")
-        if len(work_package_parts) != 2:
+        if not (
+            len(work_package_parts) == 2
+            and 20 <= len(work_package_parts[0]) < 40
+            and 80 <= len(work_package_parts[1]) < 120
+        ):
             message_display.display(
-                "Invalid input. Please enter the work package string you got from the "
-                + "UI unaltered."
+                "Invalid input. Please enter the download token "
+                + "you got from the GHGA data portal unaltered."
             )
             continue
         return work_package_parts
     message_display.failure(
         f"Tried {max_tries} times to parse the work package string and failed."
     )
     raise exceptions.InvalidWorkPackageToken(tries=max_tries)
```

### Comparing `ghga_connector-0.3.7/ghga_connector/core/message_display.py` & `ghga_connector-0.3.8/ghga_connector/core/message_display.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/ghga_connector.egg-info/PKG-INFO` & `ghga_connector-0.3.8/ghga_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga-connector
-Version: 0.3.7
+Version: 0.3.8
 Summary: GHGA Connector - A CLI client application for interacting with the GHGA system.
 Home-page: https://github.com/ghga-de/ghga-connector
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -41,29 +41,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-connector):
 ```bash
-docker pull ghga/ghga-connector:0.3.7
+docker pull ghga/ghga-connector:0.3.8
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-connector:0.3.7 .
+docker build -t ghga/ghga-connector:0.3.8 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-connector:0.3.7 --help
+docker run -p 8080:8080 ghga/ghga-connector:0.3.8 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
 
@@ -77,15 +77,15 @@
 The service requires the following configuration parameters:
 - **`max_retries`** *(integer)*: Number of times to retry failed API calls. Default: `5`.
 
 - **`max_wait_time`** *(integer)*: Maximal time in seconds to wait before quitting without a download. Default: `3600`.
 
 - **`part_size`** *(integer)*: The part size to use for download. Default: `16777216`.
 
-- **`wkvs_api_url`** *(string)*: URL to the root of the WKVS API. Should start with https://.
+- **`wkvs_api_url`** *(string)*: URL to the root of the WKVS API. Should start with https://. Default: `https://data.ghga.de/.well-known`.
 
 
 ### Usage:
 
 A template YAML for configurating the service can be found at
 [`./example-config.yaml`](./example-config.yaml).
 Please adapt it, rename it to `.ghga_connector.yaml`, and place it into one of the following locations:
```

### Comparing `ghga_connector-0.3.7/ghga_connector.egg-info/SOURCES.txt` & `ghga_connector-0.3.8/ghga_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/scripts/__init__.py` & `ghga_connector-0.3.8/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/scripts/get_package_name.py` & `ghga_connector-0.3.8/scripts/get_package_name.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/scripts/license_checker.py` & `ghga_connector-0.3.8/scripts/license_checker.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/scripts/script_utils/__init__.py` & `ghga_connector-0.3.8/scripts/script_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/scripts/script_utils/cli.py` & `ghga_connector-0.3.8/scripts/script_utils/cli.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/scripts/update_config_docs.py` & `ghga_connector-0.3.8/scripts/update_config_docs.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/scripts/update_readme.py` & `ghga_connector-0.3.8/scripts/update_readme.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/scripts/update_template_files.py` & `ghga_connector-0.3.8/scripts/update_template_files.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/setup.cfg` & `ghga_connector-0.3.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/setup.py` & `ghga_connector-0.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/tests/fixtures/__init__.py` & `ghga_connector-0.3.8/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/tests/fixtures/config.py` & `ghga_connector-0.3.8/tests/fixtures/config.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/tests/fixtures/endpoints_handler.py` & `ghga_connector-0.3.8/tests/fixtures/endpoints_handler.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/tests/fixtures/mock_api/__init__.py` & `ghga_connector-0.3.8/tests/fixtures/mock_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/tests/fixtures/mock_api/app.py` & `ghga_connector-0.3.8/tests/fixtures/mock_api/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,40 +437,37 @@
 
 @EndpointsHandler.post("/work-packages/{package_id}/files/{file_id}/work-order-tokens")
 def create_work_order_token(package_id: str, file_id: str):
     """Mock Work Order Token endpoint"""
 
     # has to be at least 48 chars long
     return httpx.Response(
-        status_code=201, content=base64.b64encode(b"1234567890" * 5).decode()
+        status_code=201,
+        json=base64.b64encode(b"1234567890" * 5).decode(),
     )
 
 
 @EndpointsHandler.get("/values/{value_name}")
 def mock_wkvs(value_name: str):
     """Mock the WKVS /values/value_name endpoint"""
     values: dict[str, str] = {
         "crypt4gh_public_key": "qx5g31H7rdsq7sgkew9ElkLIXvBje4RxDVcAHcJD8XY=",
         "wps_api_url": "http://127.0.0.1/wps",
         "dcs_api_url": "http://127.0.0.1/download",
         "ucs_api_url": "http://127.0.0.1/upload",
     }
 
-    if value_name in values:
-        return httpx.Response(
-            status_code=200,
-            json={value_name: values[value_name]},
-        )
-    else:
+    if value_name not in values:
         raise HttpyException(
             status_code=404,
             exception_id="valueNotConfigured",
             description=f"The value {value_name} is not configured.",
             data={"value_name": value_name},
         )
+    return httpx.Response(status_code=200, json={value_name: values[value_name]})
 
 
 def handle_request(request: httpx.Request):
     """
     This is used as the callback function for the httpx_mock fixture in test_cli.py.
     """
     url = str(request.url)
```

### Comparing `ghga_connector-0.3.7/tests/fixtures/s3.py` & `ghga_connector-0.3.8/tests/fixtures/s3.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/tests/fixtures/state.py` & `ghga_connector-0.3.8/tests/fixtures/state.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/tests/fixtures/utils.py` & `ghga_connector-0.3.8/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/tests/integration/__init__.py` & `ghga_connector-0.3.8/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/tests/integration/fixtures/__init__.py` & `ghga_connector-0.3.8/tests/integration/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/tests/integration/fixtures/utils.py` & `ghga_connector-0.3.8/tests/integration/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/tests/integration/test_cli.py` & `ghga_connector-0.3.8/tests/integration/test_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,16 +133,16 @@
             download_api=api_url,
             part_size=part_size,
             wps_api_url=api_url,
         ),
     ):
         download(
             output_dir=tmp_path,
-            submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
-            submitter_private_key_path=Path(PRIVATE_KEY_FILE),
+            my_public_key_path=Path(PUBLIC_KEY_FILE),
+            my_private_key_path=Path(PRIVATE_KEY_FILE),
         )
 
     with open(tmp_path / f"{big_object.object_id}.c4gh", "rb") as file:
         observed_content = file.read()
 
     assert observed_content == big_file_content
 
@@ -245,38 +245,38 @@
                 ):
                     with pytest.raises(
                         exceptions.UnauthorizedAPICallError,
                         match="This is not the token you're looking for.",
                     ):
                         download(
                             output_dir=output_dir,
-                            submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
-                            submitter_private_key_path=Path(PRIVATE_KEY_FILE),
+                            my_public_key_path=Path(PUBLIC_KEY_FILE),
+                            my_private_key_path=Path(PRIVATE_KEY_FILE),
                         )
                 with patch(
                     "ghga_connector.core.api_calls.work_package._decrypt",
                     lambda data, key: "file_id_mismatch",
                 ):
                     with pytest.raises(
                         exceptions.UnauthorizedAPICallError,
                         match="Endpoint file ID did not match file ID announced in work order token.",
                     ):
                         download(
                             output_dir=output_dir,
-                            submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
-                            submitter_private_key_path=Path(PRIVATE_KEY_FILE),
+                            my_public_key_path=Path(PUBLIC_KEY_FILE),
+                            my_private_key_path=Path(PRIVATE_KEY_FILE),
                         )
             else:
                 with pytest.raises(  # type: ignore
                     expected_exception
                 ) if expected_exception else nullcontext():
                     download(
                         output_dir=output_dir,
-                        submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
-                        submitter_private_key_path=Path(PRIVATE_KEY_FILE),
+                        my_public_key_path=Path(PUBLIC_KEY_FILE),
+                        my_private_key_path=Path(PRIVATE_KEY_FILE),
                     )
 
         # BadResponseCode is no longer propagated and file at path does not exist
         if file_name == "file_not_downloadable":
             return
 
         tmp_file = tmp_path / "file_with_envelope"
@@ -321,15 +321,15 @@
 
     if file_name == "encrypted_file":
         # encrypt test file on the fly
         server_pubkey = base64.b64encode(
             crypt4gh.keys.get_public_key(PUBLIC_KEY_FILE)
         ).decode("utf-8")
         encryptor = Crypt4GHEncryptor(
-            server_pubkey=server_pubkey, submitter_private_key_path=PRIVATE_KEY_FILE
+            server_pubkey=server_pubkey, my_private_key_path=PRIVATE_KEY_FILE
         )
         encrypted_path = encryptor.encrypt_file(file_path=uploadable_file.file_path)
 
     # initiate upload
     upload_id = await s3_fixture.storage.init_multipart_upload(
         bucket_id=uploadable_file.grouping_label,
         object_id=uploadable_file.file_id,
@@ -355,23 +355,23 @@
         with pytest.raises(  # type: ignore
             expected_exception
         ) if expected_exception else nullcontext():
             if file_name == "encrypted_file":
                 upload(
                     file_id=uploadable_file.file_id,
                     file_path=Path(encrypted_path).resolve(),
-                    submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
-                    submitter_private_key_path=Path(PRIVATE_KEY_FILE),
+                    my_public_key_path=Path(PUBLIC_KEY_FILE),
+                    my_private_key_path=Path(PRIVATE_KEY_FILE),
                 )
             else:
                 upload(
                     file_id=uploadable_file.file_id,
                     file_path=uploadable_file.file_path.resolve(),
-                    submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
-                    submitter_private_key_path=Path(PRIVATE_KEY_FILE),
+                    my_public_key_path=Path(PUBLIC_KEY_FILE),
+                    my_private_key_path=Path(PRIVATE_KEY_FILE),
                 )
 
             await s3_fixture.storage.complete_multipart_upload(
                 upload_id=upload_id,
                 bucket_id=uploadable_file.grouping_label,
                 object_id=uploadable_file.file_id,
             )
@@ -451,16 +451,16 @@
         with patch(
             "ghga_connector.cli.CONFIG",
             get_test_config(),
         ):
             upload(
                 file_id=file_id,
                 file_path=Path(file.name),
-                submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
-                submitter_private_key_path=Path(PRIVATE_KEY_FILE),
+                my_public_key_path=Path(PUBLIC_KEY_FILE),
+                my_private_key_path=Path(PRIVATE_KEY_FILE),
             )
 
     # confirm upload
     await s3_fixture.storage.complete_multipart_upload(
         upload_id=upload_id,
         bucket_id=bucket_id,
         object_id=file_id,
```

### Comparing `ghga_connector-0.3.7/tests/integration/test_file_operations.py` & `ghga_connector-0.3.8/tests/integration/test_file_operations.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/tests/unit/__init__.py` & `ghga_connector-0.3.8/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/tests/unit/fixtures/__init__.py` & `ghga_connector-0.3.8/tests/unit/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/tests/unit/fixtures/utils.py` & `ghga_connector-0.3.8/tests/unit/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/tests/unit/test_api_calls.py` & `ghga_connector-0.3.8/tests/unit/test_api_calls.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,42 +157,42 @@
 
     wp_id, wp_token = mock_wps_token(1, None)
     work_package_accessor = WorkPackageAccessor(
         access_token=wp_token,
         api_url="http://127.0.0.1",
         dcs_api_url="",
         package_id=wp_id,
-        submitter_private_key="",
+        my_private_key="",
     )
     response = work_package_accessor.get_package_files()
     assert response == files
 
     httpx_mock.add_response(json={"files": files}, status_code=403)
 
     with pytest.raises(NoWorkPackageAccessError):
         wp_id, wp_token = mock_wps_token(1, None)
         work_package_accessor = WorkPackageAccessor(
             access_token=wp_token,
             api_url="http://127.0.0.1",
             dcs_api_url="",
             package_id=wp_id,
-            submitter_private_key="",
+            my_private_key="",
         )
         response = work_package_accessor.get_package_files()
 
     httpx_mock.add_response(json={"files": files}, status_code=500)
 
     with pytest.raises(InvalidWPSResponseError):
         wp_id, wp_token = mock_wps_token(1, None)
         work_package_accessor = WorkPackageAccessor(
             access_token=wp_token,
             api_url="http://127.0.0.1",
             dcs_api_url="",
             package_id=wp_id,
-            submitter_private_key="",
+            my_private_key="",
         )
         response = work_package_accessor.get_package_files()
 
 
 @pytest.mark.asyncio
 async def test_wkvs_calls(httpx_mock: HTTPXMock):
     """Test handling of responses for WKVS api calls"""
```

### Comparing `ghga_connector-0.3.7/tests/unit/test_core.py` & `ghga_connector-0.3.8/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.7/tests/unit/test_file_operations.py` & `ghga_connector-0.3.8/tests/unit/test_file_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         with NamedTemporaryFile() as out_file:
             # fill source file with random data
             in_file.write(os.urandom(file_size))
             in_file.seek(0)
 
             # produce encrypted file
             encryptor = Crypt4GHEncryptor(
-                server_pubkey=pubkey, submitter_private_key_path=private_key_path
+                server_pubkey=pubkey, my_private_key_path=private_key_path
             )
             encrypted_file_loc = encryptor.encrypt_file(file_path=Path(in_file.name))
 
             assert is_file_encrypted(encrypted_file_loc)
             decryptor = Crypt4GHDecryptor(decryption_key_path=private_key_path)
             decryptor.decrypt_file(
                 input_path=encrypted_file_loc,
```

