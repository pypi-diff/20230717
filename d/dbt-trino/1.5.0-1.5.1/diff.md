# Comparing `tmp/dbt-trino-1.5.0.tar.gz` & `tmp/dbt-trino-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-trino-1.5.0.tar", last modified: Fri Apr 28 11:05:42 2023, max compression
+gzip compressed data, was "dbt-trino-1.5.1.tar", last modified: Mon Jul 17 19:17:02 2023, max compression
```

## Comparing `dbt-trino-1.5.0.tar` & `dbt-trino-1.5.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:05:42.488964 dbt-trino-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 11:05:10.000000 dbt-trino-1.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-04-28 11:05:42.488964 dbt-trino-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-28 11:05:10.000000 dbt-trino-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:05:42.484964 dbt-trino-1.5.0/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:05:42.484964 dbt-trino-1.5.0/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:05:42.484964 dbt-trino-1.5.0/dbt/adapters/trino/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-28 11:05:10.000000 dbt-trino-1.5.0/dbt/adapters/trino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 11:05:10.000000 dbt-trino-1.5.0/dbt/adapters/trino/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-04-28 11:05:10.000000 dbt-trino-1.5.0/dbt/adapters/trino/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/adapters/trino/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/adapters/trino/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/adapters/trino/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:05:42.484964 dbt-trino-1.5.0/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:05:42.484964 dbt-trino-1.5.0/dbt/include/trino/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:05:42.484964 dbt-trino-1.5.0/dbt/include/trino/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     9542 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:05:42.484964 dbt-trino-1.5.0/dbt/include/trino/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/materializations/materialized_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:05:42.484964 dbt-trino-1.5.0/dbt/include/trino/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:05:42.488964 dbt-trino-1.5.0/dbt/include/trino/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/dbt/include/trino/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:05:42.488964 dbt-trino-1.5.0/dbt_trino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-04-28 11:05:42.000000 dbt-trino-1.5.0/dbt_trino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-28 11:05:42.000000 dbt-trino-1.5.0/dbt_trino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:05:42.000000 dbt-trino-1.5.0/dbt_trino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:05:42.000000 dbt-trino-1.5.0/dbt_trino.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-28 11:05:42.000000 dbt-trino-1.5.0/dbt_trino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 11:05:42.000000 dbt-trino-1.5.0/dbt_trino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 11:05:42.488964 dbt-trino-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-28 11:05:11.000000 dbt-trino-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.616028 dbt-trino-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-17 19:17:02.616028 dbt-trino-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.608027 dbt-trino-1.5.1/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.608027 dbt-trino-1.5.1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.612027 dbt-trino-1.5.1/dbt/adapters/trino/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/adapters/trino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/adapters/trino/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/adapters/trino/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16345 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/adapters/trino/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/adapters/trino/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/adapters/trino/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.608027 dbt-trino-1.5.1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.612027 dbt-trino-1.5.1/dbt/include/trino/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.612027 dbt-trino-1.5.1/dbt/include/trino/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.612027 dbt-trino-1.5.1/dbt/include/trino/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/materializations/materialized_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.612027 dbt-trino-1.5.1/dbt/include/trino/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.612027 dbt-trino-1.5.1/dbt/include/trino/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.616028 dbt-trino-1.5.1/dbt_trino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-17 19:17:02.000000 dbt-trino-1.5.1/dbt_trino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-17 19:17:02.000000 dbt-trino-1.5.1/dbt_trino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:17:02.000000 dbt-trino-1.5.1/dbt_trino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:17:02.000000 dbt-trino-1.5.1/dbt_trino.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 19:17:02.000000 dbt-trino-1.5.1/dbt_trino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-17 19:17:02.000000 dbt-trino-1.5.1/dbt_trino.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 19:17:02.616028 dbt-trino-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/setup.py
```

### Comparing `dbt-trino-1.5.0/LICENSE.txt` & `dbt-trino-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.0/PKG-INFO` & `dbt-trino-1.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-trino
-Version: 1.5.0
+Version: 1.5.1
 Summary: The trino adapter plugin for dbt (data build tool)
 Home-page: https://github.com/starburstdata/dbt-trino
 Author: Starburst Data
 Author-email: info@starburstdata.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,28 +20,28 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # dbt-trino
 
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="assets/images/Starburst_Logo_White+Blue.svg" width="98%">
-  <source media="(prefers-color-scheme: light)" srcset="assets/images/Starburst_Logo_Black+Blue.svg" width="98%">
-  <img alt="Starburst" src="assets/images/Starburst_Logo_Black+Blue.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/Starburst_Logo_White%2BBlue.svg" width="98%">
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/Starburst_Logo_Black%2BBlue.svg" width="98%">
+  <img alt="Starburst" src="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/Starburst_Logo_Black%2BBlue.svg">
 </picture>
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="assets/images/dbt-signature_tm_light.svg" width="45%">
-  <source media="(prefers-color-scheme: light)" srcset="assets/images/dbt-signature_tm.svg" width="45%">
-  <img alt="dbt" src="assets/images/dbt-signature_tm.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/dbt-signature_tm_light.svg" width="45%">
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/dbt-signature_tm.svg" width="45%">
+  <img alt="dbt" src="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/dbt-signature_tm.svg">
 </picture>
 &nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="assets/images/trino-logo-dk-bg.svg" width="50%">
-  <source media="(prefers-color-scheme: light)" srcset="assets/images/trino-logo-w-bk.svg" width="50%">
-  <img alt="trino" src="assets/images/trino-logo-w-bk.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/trino-logo-dk-bg.svg" width="50%">
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/trino-logo-w-bk.svg" width="50%">
+  <img alt="trino" src="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/trino-logo-w-bk.svg">
 </picture>
 
 [![Build Status](https://github.com/starburstdata/dbt-trino/actions/workflows/ci.yml/badge.svg)](https://github.com/starburstdata/dbt-trino/actions/workflows/ci.yml?query=workflow%3A%22dbt-trino+tests%22+branch%3Amaster+event%3Apush) [![db-presto-trino Slack](https://img.shields.io/static/v1?logo=slack&logoColor=959DA5&label=Slack&labelColor=333a41&message=join%20conversation&color=3AC358)](https://getdbt.slack.com/channels/db-presto-trino)
 
 ## Introduction
 
 [dbt](https://docs.getdbt.com/docs/introduction) is a data transformation workflow tool that lets teams quickly and collaboratively deploy analytics code, following software engineering best practices like modularity, CI/CD, testing, and documentation. It enables anyone who knows SQL to build production-grade data pipelines.
@@ -56,15 +56,15 @@
 
 `dbt-trino` adapter uses [Trino](https://trino.io/) as a underlying query engine to perform query federation across disperse data sources. Trino connects to multiple and diverse data sources ([available connectors](https://trino.io/docs/current/connector.html)) via one dbt connection and process SQL queries at scale. Transformations defined in dbt are passed to Trino which handles these SQL transformation queries and translates them to queries specific to the systems it connects to create tables or views and manipulate data.
 
 This repository represents a fork of the [dbt-presto](https://github.com/dbt-labs/dbt-presto) with adaptations to make it work with Trino.
 
 ## Compatibility
 
-This dbt plugin has been tested against `Trino` version `414`, `Starburst Enterprise` version `413-e` and `Starburst Galaxy`.
+This dbt plugin has been tested against `Trino` version `422`, `Starburst Enterprise` version `420-e` and `Starburst Galaxy`.
 
 ## Setup & Configuration
 
 For information on installing and configuring your profile to authenticate to Trino or Starburst, please refer to [Starburst and Trino Setup](https://docs.getdbt.com/reference/warehouse-setups/trino-setup) in the dbt docs.
 
 ### Trino- and Starburst-specific configuration
```

### Comparing `dbt-trino-1.5.0/README.md` & `dbt-trino-1.5.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # dbt-trino
 
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="assets/images/Starburst_Logo_White+Blue.svg" width="98%">
-  <source media="(prefers-color-scheme: light)" srcset="assets/images/Starburst_Logo_Black+Blue.svg" width="98%">
-  <img alt="Starburst" src="assets/images/Starburst_Logo_Black+Blue.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/Starburst_Logo_White%2BBlue.svg" width="98%">
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/Starburst_Logo_Black%2BBlue.svg" width="98%">
+  <img alt="Starburst" src="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/Starburst_Logo_Black%2BBlue.svg">
 </picture>
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="assets/images/dbt-signature_tm_light.svg" width="45%">
-  <source media="(prefers-color-scheme: light)" srcset="assets/images/dbt-signature_tm.svg" width="45%">
-  <img alt="dbt" src="assets/images/dbt-signature_tm.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/dbt-signature_tm_light.svg" width="45%">
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/dbt-signature_tm.svg" width="45%">
+  <img alt="dbt" src="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/dbt-signature_tm.svg">
 </picture>
 &nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="assets/images/trino-logo-dk-bg.svg" width="50%">
-  <source media="(prefers-color-scheme: light)" srcset="assets/images/trino-logo-w-bk.svg" width="50%">
-  <img alt="trino" src="assets/images/trino-logo-w-bk.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/trino-logo-dk-bg.svg" width="50%">
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/trino-logo-w-bk.svg" width="50%">
+  <img alt="trino" src="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/trino-logo-w-bk.svg">
 </picture>
 
 [![Build Status](https://github.com/starburstdata/dbt-trino/actions/workflows/ci.yml/badge.svg)](https://github.com/starburstdata/dbt-trino/actions/workflows/ci.yml?query=workflow%3A%22dbt-trino+tests%22+branch%3Amaster+event%3Apush) [![db-presto-trino Slack](https://img.shields.io/static/v1?logo=slack&logoColor=959DA5&label=Slack&labelColor=333a41&message=join%20conversation&color=3AC358)](https://getdbt.slack.com/channels/db-presto-trino)
 
 ## Introduction
 
 [dbt](https://docs.getdbt.com/docs/introduction) is a data transformation workflow tool that lets teams quickly and collaboratively deploy analytics code, following software engineering best practices like modularity, CI/CD, testing, and documentation. It enables anyone who knows SQL to build production-grade data pipelines.
@@ -33,15 +33,15 @@
 
 `dbt-trino` adapter uses [Trino](https://trino.io/) as a underlying query engine to perform query federation across disperse data sources. Trino connects to multiple and diverse data sources ([available connectors](https://trino.io/docs/current/connector.html)) via one dbt connection and process SQL queries at scale. Transformations defined in dbt are passed to Trino which handles these SQL transformation queries and translates them to queries specific to the systems it connects to create tables or views and manipulate data.
 
 This repository represents a fork of the [dbt-presto](https://github.com/dbt-labs/dbt-presto) with adaptations to make it work with Trino.
 
 ## Compatibility
 
-This dbt plugin has been tested against `Trino` version `414`, `Starburst Enterprise` version `413-e` and `Starburst Galaxy`.
+This dbt plugin has been tested against `Trino` version `422`, `Starburst Enterprise` version `420-e` and `Starburst Galaxy`.
 
 ## Setup & Configuration
 
 For information on installing and configuring your profile to authenticate to Trino or Starburst, please refer to [Starburst and Trino Setup](https://docs.getdbt.com/reference/warehouse-setups/trino-setup) in the dbt docs.
 
 ### Trino- and Starburst-specific configuration
```

### Comparing `dbt-trino-1.5.0/dbt/adapters/trino/__init__.py` & `dbt-trino-1.5.1/dbt/adapters/trino/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.0/dbt/adapters/trino/column.py` & `dbt-trino-1.5.1/dbt/adapters/trino/column.py`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.0/dbt/adapters/trino/connections.py` & `dbt-trino-1.5.1/dbt/adapters/trino/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,14 +478,16 @@
             without_comments = re.sub(
                 re.compile("^.*(--.*)$", re.MULTILINE), "", individual_query
             ).strip()
 
             if without_comments == "":
                 continue
 
+            individual_query = self._add_query_comment(individual_query)
+
             parent = super(TrinoConnectionManager, self)
             connection, cursor = parent.add_query(
                 individual_query, auto_begin, bindings, abridge_sql_log
             )
 
         if cursor is None:
             conn = self.get_thread_connection()
```

### Comparing `dbt-trino-1.5.0/dbt/adapters/trino/impl.py` & `dbt-trino-1.5.1/dbt/adapters/trino/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.0/dbt/adapters/trino/relation.py` & `dbt-trino-1.5.1/dbt/adapters/trino/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.0/dbt/include/trino/macros/adapters.sql` & `dbt-trino-1.5.1/dbt/include/trino/macros/adapters.sql`

 * *Files 10% similar despite different names*

```diff
@@ -84,38 +84,45 @@
             {{ key }} = {{ value }}
             {%- if not loop.last -%}{{ ',\n  ' }}{%- endif -%}
           {%- endfor -%}
       )
   {%- endif -%}
 {%- endmacro -%}
 
+{% macro comment(comment) %}
+  {%- if comment is not none and comment|length > 0 -%}
+      comment '{{ comment | replace("'", "''") }}'
+  {%- endif -%}
+{%- endmacro -%}
 
 {% macro trino__create_table_as(temporary, relation, sql) -%}
   {%- set _properties = config.get('properties') -%}
 
   {%- set contract_config = config.get('contract') -%}
   {%- if contract_config.enforced -%}
 
   create table
     {{ relation }}
     {{ get_table_columns_and_constraints() }}
     {{ get_assert_columns_equivalent(sql) }}
     {%- set sql = get_select_subquery(sql) %}
+    {{ comment(model.get('description')) }}
     {{ properties(_properties) }}
   ;
 
   insert into {{ relation }}
     (
       {{ sql }}
     )
   ;
 
   {%- else %}
 
     create table {{ relation }}
+      {{ comment(model.get('description')) }}
       {{ properties(_properties) }}
     as (
       {{ sql }}
     );
 
    {%- endif %}
 {% endmacro %}
@@ -279,7 +286,24 @@
   {% set should_revoke = should_revoke(exists_as_view, full_refresh_mode=True) %}
   {% do apply_grants(target_relation, grant_config, should_revoke=True) %}
 
   {{ run_hooks(post_hooks) }}
 
   {{ return({'relations': [target_relation]}) }}
 {% endmacro %}
+
+{% macro trino__alter_column_type(relation, column_name, new_column_type) %}
+  {#
+    1. Create a new column (w/ temp name and correct type)
+    2. Copy data over to it
+    3. Drop the existing column
+    4. Rename the new column to existing column
+  #}
+  {%- set tmp_column = column_name + "__dbt_alter" -%}
+
+  {% call statement('alter_column_type') %}
+    alter table {{ relation }} add column {{ adapter.quote(tmp_column) }} {{ new_column_type }};
+    update {{ relation }} set {{ adapter.quote(tmp_column) }} = CAST({{ adapter.quote(column_name) }} AS {{ new_column_type }});
+    alter table {{ relation }} drop column {{ adapter.quote(column_name) }};
+    alter table {{ relation }} rename column {{ adapter.quote(tmp_column) }} to {{ adapter.quote(column_name) }}
+  {% endcall %}
+{% endmacro %}
```

### Comparing `dbt-trino-1.5.0/dbt/include/trino/macros/apply_grants.sql` & `dbt-trino-1.5.1/dbt/include/trino/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.0/dbt/include/trino/macros/catalog.sql` & `dbt-trino-1.5.1/dbt/include/trino/macros/catalog.sql`

 * *Files 10% similar despite different names*

```diff
@@ -54,15 +54,25 @@
                 schema_name = '{{ schema | lower }}'
             {% if not loop.last %}
             union all
             {% endif %}
             {%- endfor %}
         )
 
-        select *
+        select
+            table_database,
+            table_schema,
+            table_name,
+            table_type,
+            table_owner,
+            column_name,
+            column_index,
+            column_type,
+            column_comment,
+            table_comment
         from tables
         join columns using ("table_database", "table_schema", "table_name")
         join table_comment using ("table_database", "table_schema", "table_name")
         order by "column_index"
 
   {%- endcall -%}
```

### Comparing `dbt-trino-1.5.0/dbt/include/trino/macros/materializations/incremental.sql` & `dbt-trino-1.5.1/dbt/include/trino/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.0/dbt/include/trino/macros/materializations/materialized_view.sql` & `dbt-trino-1.5.1/dbt/include/trino/macros/materializations/materialized_view.sql`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,17 @@
 {%- endmaterialization %}
 
 
 {%- macro create_materialized_view_as(target_relation) -%}
   {%- set _properties = config.get('properties') -%}
   create or replace materialized view {{ target_relation }}
     {{ properties(_properties) }}
-  as (
+  as
   {{ sql }}
-  );
+  ;
 {%- endmacro -%}
 
 
 {%- macro refresh_materialized_view(target_relation) -%}
   {%- set sqlcode = "refresh materialized view " ~  target_relation %}
   {{ sqlcode }}
 {%- endmacro -%}
```

### Comparing `dbt-trino-1.5.0/dbt/include/trino/macros/materializations/seeds/helpers.sql` & `dbt-trino-1.5.1/dbt/include/trino/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.0/dbt/include/trino/macros/materializations/snapshot.sql` & `dbt-trino-1.5.1/dbt/include/trino/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.0/dbt/include/trino/macros/materializations/table.sql` & `dbt-trino-1.5.1/dbt/include/trino/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.0/dbt/include/trino/macros/utils/datediff.sql` & `dbt-trino-1.5.1/dbt/include/trino/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.0/dbt/include/trino/sample_profiles.yml` & `dbt-trino-1.5.1/dbt/include/trino/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.0/dbt_trino.egg-info/PKG-INFO` & `dbt-trino-1.5.1/dbt_trino.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-trino
-Version: 1.5.0
+Version: 1.5.1
 Summary: The trino adapter plugin for dbt (data build tool)
 Home-page: https://github.com/starburstdata/dbt-trino
 Author: Starburst Data
 Author-email: info@starburstdata.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,28 +20,28 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # dbt-trino
 
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="assets/images/Starburst_Logo_White+Blue.svg" width="98%">
-  <source media="(prefers-color-scheme: light)" srcset="assets/images/Starburst_Logo_Black+Blue.svg" width="98%">
-  <img alt="Starburst" src="assets/images/Starburst_Logo_Black+Blue.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/Starburst_Logo_White%2BBlue.svg" width="98%">
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/Starburst_Logo_Black%2BBlue.svg" width="98%">
+  <img alt="Starburst" src="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/Starburst_Logo_Black%2BBlue.svg">
 </picture>
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="assets/images/dbt-signature_tm_light.svg" width="45%">
-  <source media="(prefers-color-scheme: light)" srcset="assets/images/dbt-signature_tm.svg" width="45%">
-  <img alt="dbt" src="assets/images/dbt-signature_tm.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/dbt-signature_tm_light.svg" width="45%">
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/dbt-signature_tm.svg" width="45%">
+  <img alt="dbt" src="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/dbt-signature_tm.svg">
 </picture>
 &nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="assets/images/trino-logo-dk-bg.svg" width="50%">
-  <source media="(prefers-color-scheme: light)" srcset="assets/images/trino-logo-w-bk.svg" width="50%">
-  <img alt="trino" src="assets/images/trino-logo-w-bk.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/trino-logo-dk-bg.svg" width="50%">
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/trino-logo-w-bk.svg" width="50%">
+  <img alt="trino" src="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/trino-logo-w-bk.svg">
 </picture>
 
 [![Build Status](https://github.com/starburstdata/dbt-trino/actions/workflows/ci.yml/badge.svg)](https://github.com/starburstdata/dbt-trino/actions/workflows/ci.yml?query=workflow%3A%22dbt-trino+tests%22+branch%3Amaster+event%3Apush) [![db-presto-trino Slack](https://img.shields.io/static/v1?logo=slack&logoColor=959DA5&label=Slack&labelColor=333a41&message=join%20conversation&color=3AC358)](https://getdbt.slack.com/channels/db-presto-trino)
 
 ## Introduction
 
 [dbt](https://docs.getdbt.com/docs/introduction) is a data transformation workflow tool that lets teams quickly and collaboratively deploy analytics code, following software engineering best practices like modularity, CI/CD, testing, and documentation. It enables anyone who knows SQL to build production-grade data pipelines.
@@ -56,15 +56,15 @@
 
 `dbt-trino` adapter uses [Trino](https://trino.io/) as a underlying query engine to perform query federation across disperse data sources. Trino connects to multiple and diverse data sources ([available connectors](https://trino.io/docs/current/connector.html)) via one dbt connection and process SQL queries at scale. Transformations defined in dbt are passed to Trino which handles these SQL transformation queries and translates them to queries specific to the systems it connects to create tables or views and manipulate data.
 
 This repository represents a fork of the [dbt-presto](https://github.com/dbt-labs/dbt-presto) with adaptations to make it work with Trino.
 
 ## Compatibility
 
-This dbt plugin has been tested against `Trino` version `414`, `Starburst Enterprise` version `413-e` and `Starburst Galaxy`.
+This dbt plugin has been tested against `Trino` version `422`, `Starburst Enterprise` version `420-e` and `Starburst Galaxy`.
 
 ## Setup & Configuration
 
 For information on installing and configuring your profile to authenticate to Trino or Starburst, please refer to [Starburst and Trino Setup](https://docs.getdbt.com/reference/warehouse-setups/trino-setup) in the dbt docs.
 
 ### Trino- and Starburst-specific configuration
```

### Comparing `dbt-trino-1.5.0/dbt_trino.egg-info/SOURCES.txt` & `dbt-trino-1.5.1/dbt_trino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.0/setup.py` & `dbt-trino-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             "include/trino/macros/*.sql",
             "include/trino/macros/*/*.sql",
             "include/trino/macros/*/*/*.sql",
         ]
     },
     install_requires=[
         "dbt-core~={}".format(dbt_version),
-        "trino~=0.322",
+        "trino~=0.326",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
```

