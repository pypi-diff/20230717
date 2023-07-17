# Comparing `tmp/woodwork-0.9.0.tar.gz` & `tmp/woodwork-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/woodwork-0.9.0.tar", last modified: Thu Nov 11 20:17:13 2021, max compression
+gzip compressed data, was "dist/woodwork-0.9.1.tar", last modified: Fri Nov 19 19:35:57 2021, max compression
```

## Comparing `woodwork-0.9.0.tar` & `woodwork-0.9.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 20:17:13.000000 woodwork-0.9.0/
--rw-r--r--   0 root         (0) root         (0)     1512 2021-11-11 20:17:09.000000 woodwork-0.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      108 2021-11-11 20:17:09.000000 woodwork-0.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5892 2021-11-11 20:17:13.000000 woodwork-0.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5087 2021-11-11 20:17:09.000000 woodwork-0.9.0/README.md
--rw-r--r--   0 root         (0) root         (0)       27 2021-11-11 20:17:09.000000 woodwork-0.9.0/dask-requirements.txt
--rw-r--r--   0 root         (0) root         (0)      300 2021-11-11 20:17:09.000000 woodwork-0.9.0/dev-requirements.txt
--rw-r--r--   0 root         (0) root         (0)       36 2021-11-11 20:17:09.000000 woodwork-0.9.0/koalas-requirements.txt
--rw-r--r--   0 root         (0) root         (0)       33 2021-11-11 20:17:09.000000 woodwork-0.9.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      530 2021-11-11 20:17:13.000000 woodwork-0.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1598 2021-11-11 20:17:09.000000 woodwork-0.9.0/setup.py
--rw-r--r--   0 root         (0) root         (0)      142 2021-11-11 20:17:09.000000 woodwork-0.9.0/test-requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork/
--rw-r--r--   0 root         (0) root         (0)      761 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/__main__.py
--rw-r--r--   0 root         (0) root         (0)     7364 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/accessor_utils.py
--rw-r--r--   0 root         (0) root         (0)    19635 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/column_accessor.py
--rw-r--r--   0 root         (0) root         (0)     8351 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/column_schema.py
--rw-r--r--   0 root         (0) root         (0)     2496 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork/demo/
--rw-r--r--   0 root         (0) root         (0)       34 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/demo/__init__.py
--rw-r--r--   0 root         (0) root         (0)       47 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/demo/api.py
--rw-r--r--   0 root         (0) root         (0)     2501 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/demo/retail.py
--rw-r--r--   0 root         (0) root         (0)     8259 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/deserialize.py
--rw-r--r--   0 root         (0) root         (0)     2617 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2091 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/indexers.py
--rw-r--r--   0 root         (0) root         (0)    15971 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/logical_types.py
--rw-r--r--   0 root         (0) root         (0)     7033 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/pandas_backport.py
--rw-r--r--   0 root         (0) root         (0)     1926 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/s3_utils.py
--rw-r--r--   0 root         (0) root         (0)     8882 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/serialize.py
--rw-r--r--   0 root         (0) root         (0)    26132 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/statistics_utils.py
--rw-r--r--   0 root         (0) root         (0)    56902 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/table_accessor.py
--rw-r--r--   0 root         (0) root         (0)    32991 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/table_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork/tests/accessor/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/accessor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33523 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/accessor/test_column_accessor.py
--rw-r--r--   0 root         (0) root         (0)    10542 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/accessor/test_indexers.py
--rw-r--r--   0 root         (0) root         (0)    33224 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/accessor/test_serialization.py
--rw-r--r--   0 root         (0) root         (0)    44155 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/accessor/test_statistics.py
--rw-r--r--   0 root         (0) root         (0)   106216 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/accessor/test_table_accessor.py
--rw-r--r--   0 root         (0) root         (0)    25700 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork/tests/demo_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/demo_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1729 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/demo_tests/test_retail.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork/tests/logical_types/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/logical_types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6432 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/logical_types/test_logical_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork/tests/schema/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16405 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/schema/test_column_schema.py
--rw-r--r--   0 root         (0) root         (0)    44644 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/schema/test_table_schema.py
--rw-r--r--   0 root         (0) root         (0)    23358 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/schema/test_table_schema_init.py
--rw-r--r--   0 root         (0) root         (0)     2435 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)     3965 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/test_pandas_backport.py
--rw-r--r--   0 root         (0) root         (0)       89 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork/tests/testing_utils/
--rw-r--r--   0 root         (0) root         (0)      178 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/testing_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2919 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/testing_utils/table_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork/tests/type_system/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/type_system/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8503 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/type_system/conftest.py
--rw-r--r--   0 root         (0) root         (0)     2133 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/type_system/test_custom_types.py
--rw-r--r--   0 root         (0) root         (0)     6993 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/type_system/test_ltype_inference.py
--rw-r--r--   0 root         (0) root         (0)    13471 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/type_system/test_type_system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork/tests/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10951 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/utils/test_accessor_utils.py
--rw-r--r--   0 root         (0) root         (0)    16170 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/utils/test_concat.py
--rw-r--r--   0 root         (0) root         (0)     8434 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/utils/test_read_file.py
--rw-r--r--   0 root         (0) root         (0)    16961 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/tests/utils/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork/type_sys/
--rw-r--r--   0 root         (0) root         (0)       37 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/type_sys/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3399 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/type_sys/inference_functions.py
--rw-r--r--   0 root         (0) root         (0)    14600 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/type_sys/type_system.py
--rw-r--r--   0 root         (0) root         (0)     6618 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/type_sys/utils.py
--rw-r--r--   0 root         (0) root         (0)      401 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/typing.py
--rw-r--r--   0 root         (0) root         (0)    19808 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2021-11-11 20:17:09.000000 woodwork-0.9.0/woodwork/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5892 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2246 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      285 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2021-11-11 20:17:13.000000 woodwork-0.9.0/woodwork.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-19 19:35:57.000000 woodwork-0.9.1/
+-rw-r--r--   0 root         (0) root         (0)     1512 2021-11-19 19:35:53.000000 woodwork-0.9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      108 2021-11-19 19:35:53.000000 woodwork-0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5892 2021-11-19 19:35:57.000000 woodwork-0.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5087 2021-11-19 19:35:53.000000 woodwork-0.9.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       27 2021-11-19 19:35:53.000000 woodwork-0.9.1/dask-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      300 2021-11-19 19:35:53.000000 woodwork-0.9.1/dev-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2021-11-19 19:35:53.000000 woodwork-0.9.1/koalas-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2021-11-19 19:35:53.000000 woodwork-0.9.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      530 2021-11-19 19:35:57.000000 woodwork-0.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1598 2021-11-19 19:35:53.000000 woodwork-0.9.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)      143 2021-11-19 19:35:53.000000 woodwork-0.9.1/test-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-19 19:35:57.000000 woodwork-0.9.1/woodwork/
+-rw-r--r--   0 root         (0) root         (0)      761 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     7364 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/accessor_utils.py
+-rw-r--r--   0 root         (0) root         (0)    19635 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/column_accessor.py
+-rw-r--r--   0 root         (0) root         (0)     8351 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/column_schema.py
+-rw-r--r--   0 root         (0) root         (0)     2496 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-19 19:35:57.000000 woodwork-0.9.1/woodwork/demo/
+-rw-r--r--   0 root         (0) root         (0)       34 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/demo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       47 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/demo/api.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/demo/retail.py
+-rw-r--r--   0 root         (0) root         (0)     8259 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/deserialize.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/indexers.py
+-rw-r--r--   0 root         (0) root         (0)    15971 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/logical_types.py
+-rw-r--r--   0 root         (0) root         (0)     7033 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/pandas_backport.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/s3_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8882 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/serialize.py
+-rw-r--r--   0 root         (0) root         (0)    26164 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/statistics_utils.py
+-rw-r--r--   0 root         (0) root         (0)    56902 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/table_accessor.py
+-rw-r--r--   0 root         (0) root         (0)    32991 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/table_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-19 19:35:57.000000 woodwork-0.9.1/woodwork/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-19 19:35:57.000000 woodwork-0.9.1/woodwork/tests/accessor/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/accessor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33523 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/accessor/test_column_accessor.py
+-rw-r--r--   0 root         (0) root         (0)    10542 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/accessor/test_indexers.py
+-rw-r--r--   0 root         (0) root         (0)    33224 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/accessor/test_serialization.py
+-rw-r--r--   0 root         (0) root         (0)    44608 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/accessor/test_statistics.py
+-rw-r--r--   0 root         (0) root         (0)   106216 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/accessor/test_table_accessor.py
+-rw-r--r--   0 root         (0) root         (0)    25700 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-19 19:35:57.000000 woodwork-0.9.1/woodwork/tests/demo_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/demo_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/demo_tests/test_retail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-19 19:35:57.000000 woodwork-0.9.1/woodwork/tests/logical_types/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/logical_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6432 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/logical_types/test_logical_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-19 19:35:57.000000 woodwork-0.9.1/woodwork/tests/schema/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16405 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/schema/test_column_schema.py
+-rw-r--r--   0 root         (0) root         (0)    44644 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/schema/test_table_schema.py
+-rw-r--r--   0 root         (0) root         (0)    23358 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/schema/test_table_schema_init.py
+-rw-r--r--   0 root         (0) root         (0)     2435 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     3965 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/test_pandas_backport.py
+-rw-r--r--   0 root         (0) root         (0)       89 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-19 19:35:57.000000 woodwork-0.9.1/woodwork/tests/testing_utils/
+-rw-r--r--   0 root         (0) root         (0)      178 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/testing_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2919 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/testing_utils/table_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-19 19:35:57.000000 woodwork-0.9.1/woodwork/tests/type_system/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/type_system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8503 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/type_system/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/type_system/test_custom_types.py
+-rw-r--r--   0 root         (0) root         (0)     6993 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/type_system/test_ltype_inference.py
+-rw-r--r--   0 root         (0) root         (0)    13471 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/type_system/test_type_system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-19 19:35:57.000000 woodwork-0.9.1/woodwork/tests/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10951 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/utils/test_accessor_utils.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/utils/test_concat.py
+-rw-r--r--   0 root         (0) root         (0)     8434 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/utils/test_read_file.py
+-rw-r--r--   0 root         (0) root         (0)    16961 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/tests/utils/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-19 19:35:57.000000 woodwork-0.9.1/woodwork/type_sys/
+-rw-r--r--   0 root         (0) root         (0)       37 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/type_sys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/type_sys/inference_functions.py
+-rw-r--r--   0 root         (0) root         (0)    14600 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/type_sys/type_system.py
+-rw-r--r--   0 root         (0) root         (0)     6618 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/type_sys/utils.py
+-rw-r--r--   0 root         (0) root         (0)      401 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/typing.py
+-rw-r--r--   0 root         (0) root         (0)    19808 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2021-11-19 19:35:53.000000 woodwork-0.9.1/woodwork/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-19 19:35:57.000000 woodwork-0.9.1/woodwork.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5892 2021-11-19 19:35:56.000000 woodwork-0.9.1/woodwork.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2246 2021-11-19 19:35:56.000000 woodwork-0.9.1/woodwork.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-19 19:35:56.000000 woodwork-0.9.1/woodwork.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2021-11-19 19:35:56.000000 woodwork-0.9.1/woodwork.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      285 2021-11-19 19:35:56.000000 woodwork-0.9.1/woodwork.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2021-11-19 19:35:56.000000 woodwork-0.9.1/woodwork.egg-info/top_level.txt
```

### Comparing `woodwork-0.9.0/LICENSE` & `woodwork-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/PKG-INFO` & `woodwork-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woodwork
-Version: 0.9.0
+Version: 0.9.1
 Summary: a two-dimensional data object with labeled axes and typing information
 Home-page: https://github.com/alteryx/woodwork/
 Author: Alteryx, Inc.
 Author-email: support@featurelabs.com
 License: BSD 3-clause
 Keywords: data science machine learning typing
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: woodwork Version: 0.9.0 Summary: a two-dimensional
+Metadata-Version: 2.1 Name: woodwork Version: 0.9.1 Summary: a two-dimensional
 data object with labeled axes and typing information Home-page: https://
 github.com/alteryx/woodwork/ Author: Alteryx, Inc. Author-email:
 support@featurelabs.com License: BSD 3-clause Keywords: data science machine
 learning typing Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `woodwork-0.9.0/README.md` & `woodwork-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/setup.cfg` & `woodwork-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/setup.py` & `woodwork-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 extras_require['complete'] = sorted(set(sum(extras_require.values(), [])))
 
 setup(
     name='woodwork',
     author='Alteryx, Inc.',
     author_email='support@featurelabs.com',
     license='BSD 3-clause',
-    version='0.9.0',
+    version='0.9.1',
     description='a two-dimensional data object with labeled axes and typing information',
     url='https://github.com/alteryx/woodwork/',
     classifiers=[
          'Development Status :: 3 - Alpha',
          'Intended Audience :: Developers',
          'Programming Language :: Python :: 3',
          'Programming Language :: Python :: 3.7',
```

### Comparing `woodwork-0.9.0/woodwork/__init__.py` & `woodwork-0.9.1/woodwork/__init__.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/accessor_utils.py` & `woodwork-0.9.1/woodwork/accessor_utils.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/column_accessor.py` & `woodwork-0.9.1/woodwork/column_accessor.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/column_schema.py` & `woodwork-0.9.1/woodwork/column_schema.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/config.py` & `woodwork-0.9.1/woodwork/config.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/demo/retail.py` & `woodwork-0.9.1/woodwork/demo/retail.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/deserialize.py` & `woodwork-0.9.1/woodwork/deserialize.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/exceptions.py` & `woodwork-0.9.1/woodwork/exceptions.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/indexers.py` & `woodwork-0.9.1/woodwork/indexers.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/logical_types.py` & `woodwork-0.9.1/woodwork/logical_types.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/pandas_backport.py` & `woodwork-0.9.1/woodwork/pandas_backport.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/s3_utils.py` & `woodwork-0.9.1/woodwork/s3_utils.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/serialize.py` & `woodwork-0.9.1/woodwork/serialize.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/statistics_utils.py` & `woodwork-0.9.1/woodwork/statistics_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,16 +276,17 @@
     valid_types = get_valid_mi_types()
     valid_columns = [
         col_name
         for col_name, col in dataframe.ww.columns.items()
         if type(col.logical_type) in valid_types
     ]
 
-    if not include_index and dataframe.ww.index is not None:
-        valid_columns.remove(dataframe.ww.index)
+    index = dataframe.ww.index
+    if not include_index and index is not None and index in valid_columns:
+        valid_columns.remove(index)
 
     data = dataframe.loc[:, valid_columns]
     if _is_dask_dataframe(data):
         data = data.compute()
     if _is_koalas_dataframe(dataframe):
         data = data.to_pandas()
```

### Comparing `woodwork-0.9.0/woodwork/table_accessor.py` & `woodwork-0.9.1/woodwork/table_accessor.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/table_schema.py` & `woodwork-0.9.1/woodwork/table_schema.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/accessor/test_column_accessor.py` & `woodwork-0.9.1/woodwork/tests/accessor/test_column_accessor.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/accessor/test_indexers.py` & `woodwork-0.9.1/woodwork/tests/accessor/test_indexers.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/accessor/test_serialization.py` & `woodwork-0.9.1/woodwork/tests/accessor/test_serialization.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/accessor/test_statistics.py` & `woodwork-0.9.1/woodwork/tests/accessor/test_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,14 +291,31 @@
     mi = sample_df.ww.get_valid_mi_columns(include_index=False)
     assert "id" not in mi
 
     mi = sample_df.ww.get_valid_mi_columns(include_index=True)
     assert "id" in mi
 
 
+def test_mutual_info_with_string_index():
+    df = pd.DataFrame(
+        {
+            "id": ["a", "b", "c"],
+            "col1": [1, 2, 3],
+            "col2": [10, 20, 30],
+        }
+    )
+    df.ww.init(index="id", logical_types={"id": "unknown"})
+    mi = df.ww.mutual_information()
+
+    cols_used = set(np.unique(mi[["column_1", "column_2"]].values))
+    assert "id" not in cols_used
+    assert "col1" in cols_used
+    assert "col2" in cols_used
+
+
 def test_get_describe_dict(describe_df):
     describe_df.ww.init(index="index_col")
 
     stats_dict = _get_describe_dict(describe_df)
     stats_dict_to_df = pd.DataFrame(stats_dict)
     for extra in ["histogram", "top_values", "recent_values"]:
         assert extra not in stats_dict_to_df.index
```

### Comparing `woodwork-0.9.0/woodwork/tests/accessor/test_table_accessor.py` & `woodwork-0.9.1/woodwork/tests/accessor/test_table_accessor.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/conftest.py` & `woodwork-0.9.1/woodwork/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/demo_tests/test_retail.py` & `woodwork-0.9.1/woodwork/tests/demo_tests/test_retail.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/logical_types/test_logical_types.py` & `woodwork-0.9.1/woodwork/tests/logical_types/test_logical_types.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/schema/test_column_schema.py` & `woodwork-0.9.1/woodwork/tests/schema/test_column_schema.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/schema/test_table_schema.py` & `woodwork-0.9.1/woodwork/tests/schema/test_table_schema.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/schema/test_table_schema_init.py` & `woodwork-0.9.1/woodwork/tests/schema/test_table_schema_init.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/test_config.py` & `woodwork-0.9.1/woodwork/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/test_pandas_backport.py` & `woodwork-0.9.1/woodwork/tests/test_pandas_backport.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/testing_utils/table_utils.py` & `woodwork-0.9.1/woodwork/tests/testing_utils/table_utils.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/type_system/conftest.py` & `woodwork-0.9.1/woodwork/tests/type_system/conftest.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/type_system/test_custom_types.py` & `woodwork-0.9.1/woodwork/tests/type_system/test_custom_types.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/type_system/test_ltype_inference.py` & `woodwork-0.9.1/woodwork/tests/type_system/test_ltype_inference.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/type_system/test_type_system.py` & `woodwork-0.9.1/woodwork/tests/type_system/test_type_system.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/utils/test_accessor_utils.py` & `woodwork-0.9.1/woodwork/tests/utils/test_accessor_utils.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/utils/test_concat.py` & `woodwork-0.9.1/woodwork/tests/utils/test_concat.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/utils/test_read_file.py` & `woodwork-0.9.1/woodwork/tests/utils/test_read_file.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/tests/utils/test_utils.py` & `woodwork-0.9.1/woodwork/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/type_sys/inference_functions.py` & `woodwork-0.9.1/woodwork/type_sys/inference_functions.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/type_sys/type_system.py` & `woodwork-0.9.1/woodwork/type_sys/type_system.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/type_sys/utils.py` & `woodwork-0.9.1/woodwork/type_sys/utils.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork/utils.py` & `woodwork-0.9.1/woodwork/utils.py`

 * *Files identical despite different names*

### Comparing `woodwork-0.9.0/woodwork.egg-info/PKG-INFO` & `woodwork-0.9.1/woodwork.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woodwork
-Version: 0.9.0
+Version: 0.9.1
 Summary: a two-dimensional data object with labeled axes and typing information
 Home-page: https://github.com/alteryx/woodwork/
 Author: Alteryx, Inc.
 Author-email: support@featurelabs.com
 License: BSD 3-clause
 Keywords: data science machine learning typing
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: woodwork Version: 0.9.0 Summary: a two-dimensional
+Metadata-Version: 2.1 Name: woodwork Version: 0.9.1 Summary: a two-dimensional
 data object with labeled axes and typing information Home-page: https://
 github.com/alteryx/woodwork/ Author: Alteryx, Inc. Author-email:
 support@featurelabs.com License: BSD 3-clause Keywords: data science machine
 learning typing Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `woodwork-0.9.0/woodwork.egg-info/SOURCES.txt` & `woodwork-0.9.1/woodwork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

