# Comparing `tmp/google-cloud-alloydb-0.2.1.tar.gz` & `tmp/google-cloud-alloydb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-alloydb-0.2.1.tar", last modified: Wed Jul  5 15:49:56 2023, max compression
+gzip compressed data, was "google-cloud-alloydb-0.3.0.tar", last modified: Mon Jul 17 13:51:10 2023, max compression
```

## Comparing `google-cloud-alloydb-0.2.1.tar` & `google-cloud-alloydb-0.3.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.877320 google-cloud-alloydb-0.2.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4362 2023-07-05 15:49:56.877320 google-cloud-alloydb-0.2.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3454 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.857317 google-cloud-alloydb-0.2.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.861318 google-cloud-alloydb-0.2.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.861318 google-cloud-alloydb-0.2.1/google/cloud/alloydb/
--rw-rw-r--   0 root         (0)     1003     4025 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.865318 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/
--rw-rw-r--   0 root         (0)     1003     3871 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    11355 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.865318 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.865318 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/
--rw-rw-r--   0 root         (0)     1003      761 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/__init__.py
--rw-rw-r--   0 root         (0)     1003   165410 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/async_client.py
--rw-rw-r--   0 root         (0)     1003   179610 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/client.py
--rw-rw-r--   0 root         (0)     1003    25613 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.865318 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    22170 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/base.py
--rw-rw-r--   0 root         (0)     1003    49405 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    50442 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   176653 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.865318 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/types/
--rw-rw-r--   0 root         (0)     1003     3607 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    62689 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/types/resources.py
--rw-rw-r--   0 root         (0)     1003    65977 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.865318 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/
--rw-rw-r--   0 root         (0)     1003     4138 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003    12199 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.865318 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.869319 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/
--rw-rw-r--   0 root         (0)     1003      761 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/__init__.py
--rw-rw-r--   0 root         (0)     1003   176279 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/async_client.py
--rw-rw-r--   0 root         (0)     1003   190294 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/client.py
--rw-rw-r--   0 root         (0)     1003    25818 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.869319 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    24539 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/base.py
--rw-rw-r--   0 root         (0)     1003    52275 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    53370 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   187729 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.869319 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/types/
--rw-rw-r--   0 root         (0)     1003     3869 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    67262 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/types/resources.py
--rw-rw-r--   0 root         (0)     1003    71128 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.869319 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/
--rw-rw-r--   0 root         (0)     1003     4137 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003    12197 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.869319 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.873319 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/
--rw-rw-r--   0 root         (0)     1003      761 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/__init__.py
--rw-rw-r--   0 root         (0)     1003   176103 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/async_client.py
--rw-rw-r--   0 root         (0)     1003   190118 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/client.py
--rw-rw-r--   0 root         (0)     1003    25777 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.873319 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    24537 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/base.py
--rw-rw-r--   0 root         (0)     1003    52243 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    53338 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   187531 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.873319 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     3869 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    67217 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/types/resources.py
--rw-rw-r--   0 root         (0)     1003    71098 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.873319 google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/
--rw-r--r--   0 root         (0)     1003     4362 2023-07-05 15:49:56.000000 google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3705 2023-07-05 15:49:56.000000 google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:49:56.000000 google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:49:56.000000 google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:49:56.000000 google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:49:56.000000 google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:49:56.000000 google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:49:56.877320 google-cloud-alloydb-0.2.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2973 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.873319 google-cloud-alloydb-0.2.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.877320 google-cloud-alloydb-0.2.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.877320 google-cloud-alloydb-0.2.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.877320 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   712763 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1/test_alloy_db_admin.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.877320 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1alpha/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003   754444 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1alpha/test_alloy_db_admin.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:56.877320 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   754409 2023-07-05 15:46:58.000000 google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1beta/test_alloy_db_admin.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.224226 google-cloud-alloydb-0.3.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4362 2023-07-17 13:51:10.224226 google-cloud-alloydb-0.3.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3454 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.200224 google-cloud-alloydb-0.3.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.200224 google-cloud-alloydb-0.3.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.204225 google-cloud-alloydb-0.3.0/google/cloud/alloydb/
+-rw-rw-r--   0 root         (0)     1003     4025 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.204225 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/
+-rw-rw-r--   0 root         (0)     1003     3871 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11355 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.204225 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.208225 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/
+-rw-rw-r--   0 root         (0)     1003      761 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/__init__.py
+-rw-rw-r--   0 root         (0)     1003   165410 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/async_client.py
+-rw-rw-r--   0 root         (0)     1003   179610 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/client.py
+-rw-rw-r--   0 root         (0)     1003    25613 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.208225 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22170 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    49405 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    50442 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   176653 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.208225 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3607 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    62706 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003    65977 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.208225 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/
+-rw-rw-r--   0 root         (0)     1003     4138 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12199 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.208225 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.212225 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/
+-rw-rw-r--   0 root         (0)     1003      761 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/__init__.py
+-rw-rw-r--   0 root         (0)     1003   176330 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/async_client.py
+-rw-rw-r--   0 root         (0)     1003   190345 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/client.py
+-rw-rw-r--   0 root         (0)     1003    25818 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.212225 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24539 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    52325 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    53420 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   187729 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.212225 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/types/
+-rw-rw-r--   0 root         (0)     1003     3869 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    69692 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/types/resources.py
+-rw-rw-r--   0 root         (0)     1003    71491 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.212225 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/
+-rw-rw-r--   0 root         (0)     1003     4137 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12197 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.212225 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.216225 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/
+-rw-rw-r--   0 root         (0)     1003      761 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/__init__.py
+-rw-rw-r--   0 root         (0)     1003   176104 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/async_client.py
+-rw-rw-r--   0 root         (0)     1003   190119 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/client.py
+-rw-rw-r--   0 root         (0)     1003    25777 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.216225 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24537 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    52243 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    53338 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   187531 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.216225 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     3869 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    67234 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/types/resources.py
+-rw-rw-r--   0 root         (0)     1003    71099 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.220226 google-cloud-alloydb-0.3.0/google_cloud_alloydb.egg-info/
+-rw-r--r--   0 root         (0)     1003     4362 2023-07-17 13:51:10.000000 google-cloud-alloydb-0.3.0/google_cloud_alloydb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3705 2023-07-17 13:51:10.000000 google-cloud-alloydb-0.3.0/google_cloud_alloydb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-17 13:51:10.000000 google-cloud-alloydb-0.3.0/google_cloud_alloydb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-17 13:51:10.000000 google-cloud-alloydb-0.3.0/google_cloud_alloydb.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-17 13:51:10.000000 google-cloud-alloydb-0.3.0/google_cloud_alloydb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-17 13:51:10.000000 google-cloud-alloydb-0.3.0/google_cloud_alloydb.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-17 13:51:10.000000 google-cloud-alloydb-0.3.0/google_cloud_alloydb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-17 13:51:10.224226 google-cloud-alloydb-0.3.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2973 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.220226 google-cloud-alloydb-0.3.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.220226 google-cloud-alloydb-0.3.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.220226 google-cloud-alloydb-0.3.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.220226 google-cloud-alloydb-0.3.0/tests/unit/gapic/alloydb_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/tests/unit/gapic/alloydb_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   712763 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/tests/unit/gapic/alloydb_v1/test_alloy_db_admin.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.220226 google-cloud-alloydb-0.3.0/tests/unit/gapic/alloydb_v1alpha/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/tests/unit/gapic/alloydb_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003   756044 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/tests/unit/gapic/alloydb_v1alpha/test_alloy_db_admin.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:10.220226 google-cloud-alloydb-0.3.0/tests/unit/gapic/alloydb_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/tests/unit/gapic/alloydb_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   754409 2023-07-17 13:48:20.000000 google-cloud-alloydb-0.3.0/tests/unit/gapic/alloydb_v1beta/test_alloy_db_admin.py
```

### Comparing `google-cloud-alloydb-0.2.1/LICENSE` & `google-cloud-alloydb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.1/MANIFEST.in` & `google-cloud-alloydb-0.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.1/PKG-INFO` & `google-cloud-alloydb-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-alloydb
-Version: 0.2.1
+Version: 0.3.0
 Summary: Google Cloud Alloydb API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-alloydb-0.2.1/README.rst` & `google-cloud-alloydb-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb/__init__.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb/gapic_version.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.2.1"  # {x-release-please-version}
+__version__ = "0.3.0"  # {x-release-please-version}
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/__init__.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/gapic_metadata.json` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/gapic_version.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.2.1"  # {x-release-please-version}
+__version__ = "0.3.0"  # {x-release-please-version}
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/__init__.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/__init__.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/async_client.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/client.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/pagers.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/__init__.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/base.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/grpc.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/grpc_asyncio.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/services/alloy_db_admin/transports/rest.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/services/alloy_db_admin/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/types/__init__.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/types/resources.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/types/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -137,15 +137,16 @@
 class MigrationSource(proto.Message):
     r"""Subset of the source instance configuration that is available
     when reading the cluster resource.
 
     Attributes:
         host_port (str):
             Output only. The host and port of the
-            on-premises instance in host:port format
+            on-premises instance in host:port
+            format
         reference_id (str):
             Output only. Place holder for the external
             source identifier(e.g DMS job name) that created
             the cluster.
         source_type (google.cloud.alloydb_v1.types.MigrationSource.MigrationSourceType):
             Output only. Type of migration source.
     """
@@ -689,21 +690,21 @@
             (https://google.aip.dev/154)
         annotations (MutableMapping[str, str]):
             Annotations to allow client tools to store
             small amount of arbitrary data. This is distinct
             from labels. https://google.aip.dev/128
         reconciling (bool):
             Output only. Reconciling
-            (https://google.aip.dev/128#reconciliation). Set
-            to true if the current state of Cluster does not
-            match the user's intended state, and the service
-            is actively updating the resource to reconcile
-            them. This can happen due to user-triggered
-            updates or system actions like failover or
-            maintenance.
+            (https://google.aip.dev/128#reconciliation).
+            Set to true if the current state of Cluster does
+            not match the user's intended state, and the
+            service is actively updating the resource to
+            reconcile them. This can happen due to
+            user-triggered updates or system actions like
+            failover or maintenance.
         initial_user (google.cloud.alloydb_v1.types.UserPassword):
             Input only. Initial user to setup during cluster creation.
             Required. If used in ``RestoreCluster`` this is ignored.
         automated_backup_policy (google.cloud.alloydb_v1.types.AutomatedBackupPolicy):
             The automated backup policy for this cluster.
             If no policy is provided then the default policy
             will be used. If backups are supported for the
@@ -1051,18 +1052,18 @@
             Read pool specific config.
         ip_address (str):
             Output only. The IP address for the Instance.
             This is the connection endpoint for an end-user
             application.
         reconciling (bool):
             Output only. Reconciling
-            (https://google.aip.dev/128#reconciliation). Set
-            to true if the current state of Instance does
-            not match the user's intended state, and the
-            service is actively updating the resource to
+            (https://google.aip.dev/128#reconciliation).
+            Set to true if the current state of Instance
+            does not match the user's intended state, and
+            the service is actively updating the resource to
             reconcile them. This can happen due to
             user-triggered updates or system actions like
             failover or maintenance.
         etag (str):
             For Resource freshness validation
             (https://google.aip.dev/154)
         annotations (MutableMapping[str, str]):
@@ -1138,18 +1139,19 @@
         INSTANCE_TYPE_UNSPECIFIED = 0
         PRIMARY = 1
         READ_POOL = 2
         SECONDARY = 3
 
     class AvailabilityType(proto.Enum):
         r"""The Availability type of an instance. Potential values:
+
         - ZONAL: The instance serves data from only one zone. Outages in
-        that     zone affect instance availability.
+          that     zone affect instance availability.
         - REGIONAL: The instance can serve data from more than one zone
-        in a     region (it is highly available).
+          in a     region (it is highly available).
 
         Values:
             AVAILABILITY_TYPE_UNSPECIFIED (0):
                 This is an unknown Availability type.
             ZONAL (1):
                 Zonal available instance.
             REGIONAL (2):
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1/types/service.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1/types/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/__init__.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/gapic_metadata.json` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/gapic_version.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.2.1"  # {x-release-please-version}
+__version__ = "0.3.0"  # {x-release-please-version}
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/__init__.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/__init__.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/async_client.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -3287,19 +3287,20 @@
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> service.GenerateClientCertificateResponse:
         r"""Generate a client certificate signed by a Cluster CA.
-        The sole purpose of this endpoint is to support the Auth
-        Proxy client and the endpoint's behavior is subject to
-        change without notice, so do not rely on its behavior
-        remaining constant. Future changes will not break the
-        Auth Proxy client.
+        The sole purpose of this endpoint is to support AlloyDB
+        connectors and the Auth Proxy client. The endpoint's
+        behavior is subject to change without notice, so do not
+        rely on its behavior remaining constant. Future changes
+        will not break AlloyDB connectors or the Auth Proxy
+        client.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -3440,14 +3441,15 @@
         Args:
             request (Optional[Union[google.cloud.alloydb_v1alpha.types.GetConnectionInfoRequest, dict]]):
                 The request object. Request message for
                 GetConnectionInfo.
             parent (:class:`str`):
                 Required. The name of the parent
                 resource. The required format is:
+
                 projects/{project}/locations/{location}/clusters/{cluster}/instances/{instance}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/client.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -3600,19 +3600,20 @@
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> service.GenerateClientCertificateResponse:
         r"""Generate a client certificate signed by a Cluster CA.
-        The sole purpose of this endpoint is to support the Auth
-        Proxy client and the endpoint's behavior is subject to
-        change without notice, so do not rely on its behavior
-        remaining constant. Future changes will not break the
-        Auth Proxy client.
+        The sole purpose of this endpoint is to support AlloyDB
+        connectors and the Auth Proxy client. The endpoint's
+        behavior is subject to change without notice, so do not
+        rely on its behavior remaining constant. Future changes
+        will not break AlloyDB connectors or the Auth Proxy
+        client.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -3746,14 +3747,15 @@
         Args:
             request (Union[google.cloud.alloydb_v1alpha.types.GetConnectionInfoRequest, dict]):
                 The request object. Request message for
                 GetConnectionInfo.
             parent (str):
                 Required. The name of the parent
                 resource. The required format is:
+
                 projects/{project}/locations/{location}/clusters/{cluster}/instances/{instance}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/pagers.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/__init__.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/base.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/grpc.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -906,19 +906,20 @@
     ) -> Callable[
         [service.GenerateClientCertificateRequest],
         service.GenerateClientCertificateResponse,
     ]:
         r"""Return a callable for the generate client certificate method over gRPC.
 
         Generate a client certificate signed by a Cluster CA.
-        The sole purpose of this endpoint is to support the Auth
-        Proxy client and the endpoint's behavior is subject to
-        change without notice, so do not rely on its behavior
-        remaining constant. Future changes will not break the
-        Auth Proxy client.
+        The sole purpose of this endpoint is to support AlloyDB
+        connectors and the Auth Proxy client. The endpoint's
+        behavior is subject to change without notice, so do not
+        rely on its behavior remaining constant. Future changes
+        will not break AlloyDB connectors or the Auth Proxy
+        client.
 
         Returns:
             Callable[[~.GenerateClientCertificateRequest],
                     ~.GenerateClientCertificateResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/grpc_asyncio.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -929,19 +929,20 @@
     ) -> Callable[
         [service.GenerateClientCertificateRequest],
         Awaitable[service.GenerateClientCertificateResponse],
     ]:
         r"""Return a callable for the generate client certificate method over gRPC.
 
         Generate a client certificate signed by a Cluster CA.
-        The sole purpose of this endpoint is to support the Auth
-        Proxy client and the endpoint's behavior is subject to
-        change without notice, so do not rely on its behavior
-        remaining constant. Future changes will not break the
-        Auth Proxy client.
+        The sole purpose of this endpoint is to support AlloyDB
+        connectors and the Auth Proxy client. The endpoint's
+        behavior is subject to change without notice, so do not
+        rely on its behavior remaining constant. Future changes
+        will not break AlloyDB connectors or the Auth Proxy
+        client.
 
         Returns:
             Callable[[~.GenerateClientCertificateRequest],
                     Awaitable[~.GenerateClientCertificateResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/rest.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/services/alloy_db_admin/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/types/__init__.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/types/resources.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/types/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -138,15 +138,16 @@
 class MigrationSource(proto.Message):
     r"""Subset of the source instance configuration that is available
     when reading the cluster resource.
 
     Attributes:
         host_port (str):
             Output only. The host and port of the
-            on-premises instance in host:port format
+            on-premises instance in host:port
+            format
         reference_id (str):
             Output only. Place holder for the external
             source identifier(e.g DMS job name) that created
             the cluster.
         source_type (google.cloud.alloydb_v1alpha.types.MigrationSource.MigrationSourceType):
             Output only. Type of migration source.
     """
@@ -488,18 +489,19 @@
 
     Attributes:
         enabled (bool):
             Whether ContinuousBackup is enabled.
 
             This field is a member of `oneof`_ ``_enabled``.
         recovery_window_days (int):
-            The number of days backups and logs will be
-            retained, which determines the window of time
-            that data is recoverable for. If not set, it
-            defaults to 14 days.
+            The number of days that are eligible to
+            restore from using PITR. To support the entire
+            recovery window, backups and logs are retained
+            for one day more than the recovery window. If
+            not set, defaults to 14 days.
         encryption_config (google.cloud.alloydb_v1alpha.types.EncryptionConfig):
             The encryption config can be specified to
             encrypt the backups with a customer-managed
             encryption key (CMEK). When this field is not
             specified, the backup will then use default
             encryption scheme to protect the user data.
     """
@@ -669,18 +671,19 @@
         cluster_type (google.cloud.alloydb_v1alpha.types.Cluster.ClusterType):
             Output only. The type of the cluster. This is an output-only
             field and it's populated at the Cluster creation time or the
             Cluster promotion time. The cluster type is determined by
             which RPC was used to create the cluster (i.e.
             ``CreateCluster`` vs. ``CreateSecondaryCluster``
         database_version (google.cloud.alloydb_v1alpha.types.DatabaseVersion):
-            Output only. The database engine major
-            version. This is an output-only field and it's
-            populated at the Cluster creation time. This
-            field cannot be changed after cluster creation.
+            Optional. The database engine major version.
+            This is an optional field and it is populated at
+            the Cluster creation time. If a database version
+            is not supplied at cluster creation time, then a
+            default database version will be used.
         network_config (google.cloud.alloydb_v1alpha.types.Cluster.NetworkConfig):
 
         network (str):
             Required. The resource link for the VPC network in which
             cluster resources are created and from which they are
             accessible via Private IP. The network must belong to the
             same project as the cluster. It is specified in the form:
@@ -692,21 +695,21 @@
             (https://google.aip.dev/154)
         annotations (MutableMapping[str, str]):
             Annotations to allow client tools to store
             small amount of arbitrary data. This is distinct
             from labels. https://google.aip.dev/128
         reconciling (bool):
             Output only. Reconciling
-            (https://google.aip.dev/128#reconciliation). Set
-            to true if the current state of Cluster does not
-            match the user's intended state, and the service
-            is actively updating the resource to reconcile
-            them. This can happen due to user-triggered
-            updates or system actions like failover or
-            maintenance.
+            (https://google.aip.dev/128#reconciliation).
+            Set to true if the current state of Cluster does
+            not match the user's intended state, and the
+            service is actively updating the resource to
+            reconcile them. This can happen due to
+            user-triggered updates or system actions like
+            failover or maintenance.
         initial_user (google.cloud.alloydb_v1alpha.types.UserPassword):
             Input only. Initial user to setup during cluster creation.
             Required. If used in ``RestoreCluster`` this is ignored.
         automated_backup_policy (google.cloud.alloydb_v1alpha.types.AutomatedBackupPolicy):
             The automated backup policy for this cluster.
             If no policy is provided then the default policy
             will be used. If backups are supported for the
@@ -736,14 +739,16 @@
             this cluster.
         secondary_config (google.cloud.alloydb_v1alpha.types.Cluster.SecondaryConfig):
             Cross Region replication config specific to
             SECONDARY cluster.
         primary_config (google.cloud.alloydb_v1alpha.types.Cluster.PrimaryConfig):
             Output only. Cross Region replication config
             specific to PRIMARY cluster.
+        satisfies_pzs (bool):
+            Reserved for future use.
     """
 
     class State(proto.Enum):
         r"""Cluster State
 
         Values:
             STATE_UNSPECIFIED (0):
@@ -995,14 +1000,18 @@
         message=SecondaryConfig,
     )
     primary_config: PrimaryConfig = proto.Field(
         proto.MESSAGE,
         number=23,
         message=PrimaryConfig,
     )
+    satisfies_pzs: bool = proto.Field(
+        proto.BOOL,
+        number=30,
+    )
 
 
 class Instance(proto.Message):
     r"""An Instance is a computing unit that an end customer can
     connect to. It's the main unit of computing resources in
     AlloyDB.
 
@@ -1091,18 +1100,18 @@
             Read pool specific config.
         ip_address (str):
             Output only. The IP address for the Instance.
             This is the connection endpoint for an end-user
             application.
         reconciling (bool):
             Output only. Reconciling
-            (https://google.aip.dev/128#reconciliation). Set
-            to true if the current state of Instance does
-            not match the user's intended state, and the
-            service is actively updating the resource to
+            (https://google.aip.dev/128#reconciliation).
+            Set to true if the current state of Instance
+            does not match the user's intended state, and
+            the service is actively updating the resource to
             reconcile them. This can happen due to
             user-triggered updates or system actions like
             failover or maintenance.
         etag (str):
             For Resource freshness validation
             (https://google.aip.dev/154)
         annotations (MutableMapping[str, str]):
@@ -1112,14 +1121,16 @@
         update_policy (google.cloud.alloydb_v1alpha.types.Instance.UpdatePolicy):
             Update policy that will be applied during
             instance update. This field is not persisted
             when you update the instance. To use a
             non-default update policy, you must
             specify explicitly specify the value in each
             update request.
+        satisfies_pzs (bool):
+            Reserved for future use.
     """
 
     class State(proto.Enum):
         r"""Instance State
 
         Values:
             STATE_UNSPECIFIED (0):
@@ -1185,18 +1196,19 @@
         INSTANCE_TYPE_UNSPECIFIED = 0
         PRIMARY = 1
         READ_POOL = 2
         SECONDARY = 3
 
     class AvailabilityType(proto.Enum):
         r"""The Availability type of an instance. Potential values:
+
         - ZONAL: The instance serves data from only one zone. Outages in
-        that     zone affect instance availability.
+          that     zone affect instance availability.
         - REGIONAL: The instance can serve data from more than one zone
-        in a     region (it is highly available).
+          in a     region (it is highly available).
 
         Values:
             AVAILABILITY_TYPE_UNSPECIFIED (0):
                 This is an unknown Availability type.
             ZONAL (1):
                 Zonal available instance.
             REGIONAL (2):
@@ -1453,14 +1465,18 @@
         number=18,
     )
     update_policy: UpdatePolicy = proto.Field(
         proto.MESSAGE,
         number=22,
         message=UpdatePolicy,
     )
+    satisfies_pzs: bool = proto.Field(
+        proto.BOOL,
+        number=24,
+    )
 
 
 class ConnectionInfo(proto.Message):
     r"""ConnectionInfo singleton resource.
     https://google.aip.dev/156
 
     Attributes:
@@ -1573,14 +1589,22 @@
         size_bytes (int):
             Output only. The size of the backup in bytes.
         expiry_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The time at which after the backup is eligible
             to be garbage collected. It is the duration specified by the
             backup's retention policy, added to the backup's
             create_time.
+        expiry_quantity (google.cloud.alloydb_v1alpha.types.Backup.QuantityBasedExpiry):
+            Output only. The QuantityBasedExpiry of the
+            backup, specified by the backup's retention
+            policy. Once the expiry quantity is over
+            retention, the backup is eligible to be garbage
+            collected.
+        satisfies_pzs (bool):
+            Reserved for future use.
     """
 
     class State(proto.Enum):
         r"""Backup State
 
         Values:
             STATE_UNSPECIFIED (0):
@@ -1619,14 +1643,49 @@
                 policy.
         """
         TYPE_UNSPECIFIED = 0
         ON_DEMAND = 1
         AUTOMATED = 2
         CONTINUOUS = 3
 
+    class QuantityBasedExpiry(proto.Message):
+        r"""A backup's position in a quantity-based retention queue, of backups
+        with the same source cluster and type, with length, retention,
+        specified by the backup's retention policy. Once the position is
+        greater than the retention, the backup is eligible to be garbage
+        collected.
+
+        Example: 5 backups from the same source cluster and type with a
+        quantity-based retention of 3 and denoted by backup_id (position,
+        retention).
+
+        Safe: backup_5 (1, 3), backup_4, (2, 3), backup_3 (3, 3). Awaiting
+        garbage collection: backup_2 (4, 3), backup_1 (5, 3)
+
+        Attributes:
+            retention_count (int):
+                Output only. The backup's position among its
+                backups with the same source cluster and type,
+                by descending chronological order create
+                time(i.e. newest first).
+            total_retention_count (int):
+                Output only. The length of the quantity-based
+                queue, specified by the backup's retention
+                policy.
+        """
+
+        retention_count: int = proto.Field(
+            proto.INT32,
+            number=1,
+        )
+        total_retention_count: int = proto.Field(
+            proto.INT32,
+            number=2,
+        )
+
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     display_name: str = proto.Field(
         proto.STRING,
         number=2,
@@ -1705,14 +1764,23 @@
         number=17,
     )
     expiry_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=19,
         message=timestamp_pb2.Timestamp,
     )
+    expiry_quantity: QuantityBasedExpiry = proto.Field(
+        proto.MESSAGE,
+        number=20,
+        message=QuantityBasedExpiry,
+    )
+    satisfies_pzs: bool = proto.Field(
+        proto.BOOL,
+        number=21,
+    )
 
 
 class SupportedDatabaseFlag(proto.Message):
     r"""SupportedDatabaseFlag gives general information about a database
     flag, like type and allowed values. This is a static value that is
     defined on the server side, and it cannot be modified by callers. To
     set the Database flags on a particular Instance, a caller should
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1alpha/types/service.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1alpha/types/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1656,14 +1656,19 @@
             requested duration. The duration can be from 1
             hour to 24 hours. The endpoint may or may not
             honor the hint. If the hint is left unspecified
             or is not honored, then the endpoint will pick
             an appropriate default duration.
         public_key (str):
             Optional. The public key from the client.
+        use_metadata_exchange (bool):
+            Optional. An optional hint to the endpoint to
+            generate a client ceritificate that can be used
+            by AlloyDB connectors to exchange additional
+            metadata with the server after TLS handshake.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
     request_id: str = proto.Field(
@@ -1679,14 +1684,18 @@
         number=4,
         message=duration_pb2.Duration,
     )
     public_key: str = proto.Field(
         proto.STRING,
         number=5,
     )
+    use_metadata_exchange: bool = proto.Field(
+        proto.BOOL,
+        number=6,
+    )
 
 
 class GenerateClientCertificateResponse(proto.Message):
     r"""Message returned by a GenerateClientCertificate operation.
 
     Attributes:
         pem_certificate (str):
@@ -1719,14 +1728,15 @@
 class GetConnectionInfoRequest(proto.Message):
     r"""Request message for GetConnectionInfo.
 
     Attributes:
         parent (str):
             Required. The name of the parent resource.
             The required format is:
+
             projects/{project}/locations/{location}/clusters/{cluster}/instances/{instance}
         request_id (str):
             Optional. An optional request ID to identify
             requests. Specify a unique request ID so that if
             you must retry your request, the server will
             know to ignore the request if it has already
             been completed. The server will guarantee that
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/__init__.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/gapic_metadata.json` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/gapic_version.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.2.1"  # {x-release-please-version}
+__version__ = "0.3.0"  # {x-release-please-version}
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/__init__.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/__init__.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/async_client.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -3440,14 +3440,15 @@
         Args:
             request (Optional[Union[google.cloud.alloydb_v1beta.types.GetConnectionInfoRequest, dict]]):
                 The request object. Request message for
                 GetConnectionInfo.
             parent (:class:`str`):
                 Required. The name of the parent
                 resource. The required format is:
+
                 projects/{project}/locations/{location}/clusters/{cluster}/instances/{instance}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/client.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -3746,14 +3746,15 @@
         Args:
             request (Union[google.cloud.alloydb_v1beta.types.GetConnectionInfoRequest, dict]):
                 The request object. Request message for
                 GetConnectionInfo.
             parent (str):
                 Required. The name of the parent
                 resource. The required format is:
+
                 projects/{project}/locations/{location}/clusters/{cluster}/instances/{instance}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/pagers.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/__init__.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/base.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/grpc.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/grpc_asyncio.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/rest.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/services/alloy_db_admin/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/types/__init__.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/types/resources.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/types/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -138,15 +138,16 @@
 class MigrationSource(proto.Message):
     r"""Subset of the source instance configuration that is available
     when reading the cluster resource.
 
     Attributes:
         host_port (str):
             Output only. The host and port of the
-            on-premises instance in host:port format
+            on-premises instance in host:port
+            format
         reference_id (str):
             Output only. Place holder for the external
             source identifier(e.g DMS job name) that created
             the cluster.
         source_type (google.cloud.alloydb_v1beta.types.MigrationSource.MigrationSourceType):
             Output only. Type of migration source.
     """
@@ -692,21 +693,21 @@
             (https://google.aip.dev/154)
         annotations (MutableMapping[str, str]):
             Annotations to allow client tools to store
             small amount of arbitrary data. This is distinct
             from labels. https://google.aip.dev/128
         reconciling (bool):
             Output only. Reconciling
-            (https://google.aip.dev/128#reconciliation). Set
-            to true if the current state of Cluster does not
-            match the user's intended state, and the service
-            is actively updating the resource to reconcile
-            them. This can happen due to user-triggered
-            updates or system actions like failover or
-            maintenance.
+            (https://google.aip.dev/128#reconciliation).
+            Set to true if the current state of Cluster does
+            not match the user's intended state, and the
+            service is actively updating the resource to
+            reconcile them. This can happen due to
+            user-triggered updates or system actions like
+            failover or maintenance.
         initial_user (google.cloud.alloydb_v1beta.types.UserPassword):
             Input only. Initial user to setup during cluster creation.
             Required. If used in ``RestoreCluster`` this is ignored.
         automated_backup_policy (google.cloud.alloydb_v1beta.types.AutomatedBackupPolicy):
             The automated backup policy for this cluster.
             If no policy is provided then the default policy
             will be used. If backups are supported for the
@@ -1091,18 +1092,18 @@
             Read pool specific config.
         ip_address (str):
             Output only. The IP address for the Instance.
             This is the connection endpoint for an end-user
             application.
         reconciling (bool):
             Output only. Reconciling
-            (https://google.aip.dev/128#reconciliation). Set
-            to true if the current state of Instance does
-            not match the user's intended state, and the
-            service is actively updating the resource to
+            (https://google.aip.dev/128#reconciliation).
+            Set to true if the current state of Instance
+            does not match the user's intended state, and
+            the service is actively updating the resource to
             reconcile them. This can happen due to
             user-triggered updates or system actions like
             failover or maintenance.
         etag (str):
             For Resource freshness validation
             (https://google.aip.dev/154)
         annotations (MutableMapping[str, str]):
@@ -1185,18 +1186,19 @@
         INSTANCE_TYPE_UNSPECIFIED = 0
         PRIMARY = 1
         READ_POOL = 2
         SECONDARY = 3
 
     class AvailabilityType(proto.Enum):
         r"""The Availability type of an instance. Potential values:
+
         - ZONAL: The instance serves data from only one zone. Outages in
-        that     zone affect instance availability.
+          that     zone affect instance availability.
         - REGIONAL: The instance can serve data from more than one zone
-        in a     region (it is highly available).
+          in a     region (it is highly available).
 
         Values:
             AVAILABILITY_TYPE_UNSPECIFIED (0):
                 This is an unknown Availability type.
             ZONAL (1):
                 Zonal available instance.
             REGIONAL (2):
```

### Comparing `google-cloud-alloydb-0.2.1/google/cloud/alloydb_v1beta/types/service.py` & `google-cloud-alloydb-0.3.0/google/cloud/alloydb_v1beta/types/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1719,14 +1719,15 @@
 class GetConnectionInfoRequest(proto.Message):
     r"""Request message for GetConnectionInfo.
 
     Attributes:
         parent (str):
             Required. The name of the parent resource.
             The required format is:
+
             projects/{project}/locations/{location}/clusters/{cluster}/instances/{instance}
         request_id (str):
             Optional. An optional request ID to identify
             requests. Specify a unique request ID so that if
             you must retry your request, the server will
             know to ignore the request if it has already
             been completed. The server will guarantee that
```

### Comparing `google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/PKG-INFO` & `google-cloud-alloydb-0.3.0/google_cloud_alloydb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-alloydb
-Version: 0.2.1
+Version: 0.3.0
 Summary: Google Cloud Alloydb API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-alloydb-0.2.1/google_cloud_alloydb.egg-info/SOURCES.txt` & `google-cloud-alloydb-0.3.0/google_cloud_alloydb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-0.2.1/setup.py` & `google-cloud-alloydb-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/tests/__init__.py` & `google-cloud-alloydb-0.3.0/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/tests/unit/__init__.py` & `google-cloud-alloydb-0.3.0/tests/unit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/tests/unit/gapic/__init__.py` & `google-cloud-alloydb-0.3.0/tests/unit/gapic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1/__init__.py` & `google-cloud-alloydb-0.3.0/tests/unit/gapic/alloydb_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1/test_alloy_db_admin.py` & `google-cloud-alloydb-0.3.0/tests/unit/gapic/alloydb_v1/test_alloy_db_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1alpha/__init__.py` & `google-cloud-alloydb-0.3.0/tests/unit/gapic/alloydb_v1alpha/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1alpha/test_alloy_db_admin.py` & `google-cloud-alloydb-0.3.0/tests/unit/gapic/alloydb_v1alpha/test_alloy_db_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1161,14 +1161,15 @@
             uid="uid_value",
             state=resources.Cluster.State.READY,
             cluster_type=resources.Cluster.ClusterType.PRIMARY,
             database_version=resources.DatabaseVersion.POSTGRES_13,
             network="network_value",
             etag="etag_value",
             reconciling=True,
+            satisfies_pzs=True,
         )
         response = client.get_cluster(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.GetClusterRequest()
@@ -1180,14 +1181,15 @@
     assert response.uid == "uid_value"
     assert response.state == resources.Cluster.State.READY
     assert response.cluster_type == resources.Cluster.ClusterType.PRIMARY
     assert response.database_version == resources.DatabaseVersion.POSTGRES_13
     assert response.network == "network_value"
     assert response.etag == "etag_value"
     assert response.reconciling is True
+    assert response.satisfies_pzs is True
 
 
 def test_get_cluster_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = AlloyDBAdminClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1225,14 +1227,15 @@
                 uid="uid_value",
                 state=resources.Cluster.State.READY,
                 cluster_type=resources.Cluster.ClusterType.PRIMARY,
                 database_version=resources.DatabaseVersion.POSTGRES_13,
                 network="network_value",
                 etag="etag_value",
                 reconciling=True,
+                satisfies_pzs=True,
             )
         )
         response = await client.get_cluster(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -1245,14 +1248,15 @@
     assert response.uid == "uid_value"
     assert response.state == resources.Cluster.State.READY
     assert response.cluster_type == resources.Cluster.ClusterType.PRIMARY
     assert response.database_version == resources.DatabaseVersion.POSTGRES_13
     assert response.network == "network_value"
     assert response.etag == "etag_value"
     assert response.reconciling is True
+    assert response.satisfies_pzs is True
 
 
 @pytest.mark.asyncio
 async def test_get_cluster_async_from_dict():
     await test_get_cluster_async(request_type=dict)
 
 
@@ -3222,14 +3226,15 @@
             state=resources.Instance.State.READY,
             instance_type=resources.Instance.InstanceType.PRIMARY,
             availability_type=resources.Instance.AvailabilityType.ZONAL,
             gce_zone="gce_zone_value",
             ip_address="ip_address_value",
             reconciling=True,
             etag="etag_value",
+            satisfies_pzs=True,
         )
         response = client.get_instance(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.GetInstanceRequest()
@@ -3242,14 +3247,15 @@
     assert response.state == resources.Instance.State.READY
     assert response.instance_type == resources.Instance.InstanceType.PRIMARY
     assert response.availability_type == resources.Instance.AvailabilityType.ZONAL
     assert response.gce_zone == "gce_zone_value"
     assert response.ip_address == "ip_address_value"
     assert response.reconciling is True
     assert response.etag == "etag_value"
+    assert response.satisfies_pzs is True
 
 
 def test_get_instance_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = AlloyDBAdminClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -3288,14 +3294,15 @@
                 state=resources.Instance.State.READY,
                 instance_type=resources.Instance.InstanceType.PRIMARY,
                 availability_type=resources.Instance.AvailabilityType.ZONAL,
                 gce_zone="gce_zone_value",
                 ip_address="ip_address_value",
                 reconciling=True,
                 etag="etag_value",
+                satisfies_pzs=True,
             )
         )
         response = await client.get_instance(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -3309,14 +3316,15 @@
     assert response.state == resources.Instance.State.READY
     assert response.instance_type == resources.Instance.InstanceType.PRIMARY
     assert response.availability_type == resources.Instance.AvailabilityType.ZONAL
     assert response.gce_zone == "gce_zone_value"
     assert response.ip_address == "ip_address_value"
     assert response.reconciling is True
     assert response.etag == "etag_value"
+    assert response.satisfies_pzs is True
 
 
 @pytest.mark.asyncio
 async def test_get_instance_async_from_dict():
     await test_get_instance_async(request_type=dict)
 
 
@@ -5737,14 +5745,15 @@
             type_=resources.Backup.Type.ON_DEMAND,
             description="description_value",
             cluster_uid="cluster_uid_value",
             cluster_name="cluster_name_value",
             reconciling=True,
             etag="etag_value",
             size_bytes=1089,
+            satisfies_pzs=True,
         )
         response = client.get_backup(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.GetBackupRequest()
@@ -5758,14 +5767,15 @@
     assert response.type_ == resources.Backup.Type.ON_DEMAND
     assert response.description == "description_value"
     assert response.cluster_uid == "cluster_uid_value"
     assert response.cluster_name == "cluster_name_value"
     assert response.reconciling is True
     assert response.etag == "etag_value"
     assert response.size_bytes == 1089
+    assert response.satisfies_pzs is True
 
 
 def test_get_backup_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = AlloyDBAdminClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -5805,14 +5815,15 @@
                 type_=resources.Backup.Type.ON_DEMAND,
                 description="description_value",
                 cluster_uid="cluster_uid_value",
                 cluster_name="cluster_name_value",
                 reconciling=True,
                 etag="etag_value",
                 size_bytes=1089,
+                satisfies_pzs=True,
             )
         )
         response = await client.get_backup(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -5827,14 +5838,15 @@
     assert response.type_ == resources.Backup.Type.ON_DEMAND
     assert response.description == "description_value"
     assert response.cluster_uid == "cluster_uid_value"
     assert response.cluster_name == "cluster_name_value"
     assert response.reconciling is True
     assert response.etag == "etag_value"
     assert response.size_bytes == 1089
+    assert response.satisfies_pzs is True
 
 
 @pytest.mark.asyncio
 async def test_get_backup_async_from_dict():
     await test_get_backup_async(request_type=dict)
 
 
@@ -9405,14 +9417,15 @@
             uid="uid_value",
             state=resources.Cluster.State.READY,
             cluster_type=resources.Cluster.ClusterType.PRIMARY,
             database_version=resources.DatabaseVersion.POSTGRES_13,
             network="network_value",
             etag="etag_value",
             reconciling=True,
+            satisfies_pzs=True,
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = resources.Cluster.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -9428,14 +9441,15 @@
     assert response.uid == "uid_value"
     assert response.state == resources.Cluster.State.READY
     assert response.cluster_type == resources.Cluster.ClusterType.PRIMARY
     assert response.database_version == resources.DatabaseVersion.POSTGRES_13
     assert response.network == "network_value"
     assert response.etag == "etag_value"
     assert response.reconciling is True
+    assert response.satisfies_pzs is True
 
 
 def test_get_cluster_rest_required_fields(request_type=service.GetClusterRequest):
     transport_class = transports.AlloyDBAdminRestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -9740,14 +9754,15 @@
         "secondary_config": {"primary_cluster_name": "primary_cluster_name_value"},
         "primary_config": {
             "secondary_cluster_names": [
                 "secondary_cluster_names_value1",
                 "secondary_cluster_names_value2",
             ]
         },
+        "satisfies_pzs": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -10017,14 +10032,15 @@
         "secondary_config": {"primary_cluster_name": "primary_cluster_name_value"},
         "primary_config": {
             "secondary_cluster_names": [
                 "secondary_cluster_names_value1",
                 "secondary_cluster_names_value2",
             ]
         },
+        "satisfies_pzs": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -10188,14 +10204,15 @@
         "secondary_config": {"primary_cluster_name": "primary_cluster_name_value"},
         "primary_config": {
             "secondary_cluster_names": [
                 "secondary_cluster_names_value1",
                 "secondary_cluster_names_value2",
             ]
         },
+        "satisfies_pzs": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -10445,14 +10462,15 @@
         "secondary_config": {"primary_cluster_name": "primary_cluster_name_value"},
         "primary_config": {
             "secondary_cluster_names": [
                 "secondary_cluster_names_value1",
                 "secondary_cluster_names_value2",
             ]
         },
+        "satisfies_pzs": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -11374,14 +11392,15 @@
         "secondary_config": {"primary_cluster_name": "primary_cluster_name_value"},
         "primary_config": {
             "secondary_cluster_names": [
                 "secondary_cluster_names_value1",
                 "secondary_cluster_names_value2",
             ]
         },
+        "satisfies_pzs": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -11655,14 +11674,15 @@
         "secondary_config": {"primary_cluster_name": "primary_cluster_name_value"},
         "primary_config": {
             "secondary_cluster_names": [
                 "secondary_cluster_names_value1",
                 "secondary_cluster_names_value2",
             ]
         },
+        "satisfies_pzs": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -12116,14 +12136,15 @@
             state=resources.Instance.State.READY,
             instance_type=resources.Instance.InstanceType.PRIMARY,
             availability_type=resources.Instance.AvailabilityType.ZONAL,
             gce_zone="gce_zone_value",
             ip_address="ip_address_value",
             reconciling=True,
             etag="etag_value",
+            satisfies_pzs=True,
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = resources.Instance.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -12140,14 +12161,15 @@
     assert response.state == resources.Instance.State.READY
     assert response.instance_type == resources.Instance.InstanceType.PRIMARY
     assert response.availability_type == resources.Instance.AvailabilityType.ZONAL
     assert response.gce_zone == "gce_zone_value"
     assert response.ip_address == "ip_address_value"
     assert response.reconciling is True
     assert response.etag == "etag_value"
+    assert response.satisfies_pzs is True
 
 
 def test_get_instance_rest_required_fields(request_type=service.GetInstanceRequest):
     transport_class = transports.AlloyDBAdminRestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -12419,14 +12441,15 @@
         },
         "read_pool_config": {"node_count": 1070},
         "ip_address": "ip_address_value",
         "reconciling": True,
         "etag": "etag_value",
         "annotations": {},
         "update_policy": {"mode": 1},
+        "satisfies_pzs": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -12661,14 +12684,15 @@
         },
         "read_pool_config": {"node_count": 1070},
         "ip_address": "ip_address_value",
         "reconciling": True,
         "etag": "etag_value",
         "annotations": {},
         "update_policy": {"mode": 1},
+        "satisfies_pzs": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -12791,14 +12815,15 @@
         },
         "read_pool_config": {"node_count": 1070},
         "ip_address": "ip_address_value",
         "reconciling": True,
         "etag": "etag_value",
         "annotations": {},
         "update_policy": {"mode": 1},
+        "satisfies_pzs": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -13035,14 +13060,15 @@
         },
         "read_pool_config": {"node_count": 1070},
         "ip_address": "ip_address_value",
         "reconciling": True,
         "etag": "etag_value",
         "annotations": {},
         "update_policy": {"mode": 1},
+        "satisfies_pzs": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -13170,14 +13196,15 @@
                     },
                     "read_pool_config": {"node_count": 1070},
                     "ip_address": "ip_address_value",
                     "reconciling": True,
                     "etag": "etag_value",
                     "annotations": {},
                     "update_policy": {"mode": 1},
+                    "satisfies_pzs": True,
                 },
                 "request_id": "request_id_value",
                 "validate_only": True,
             }
         ]
     }
     request = request_type(**request_init)
@@ -13398,14 +13425,15 @@
                     },
                     "read_pool_config": {"node_count": 1070},
                     "ip_address": "ip_address_value",
                     "reconciling": True,
                     "etag": "etag_value",
                     "annotations": {},
                     "update_policy": {"mode": 1},
+                    "satisfies_pzs": True,
                 },
                 "request_id": "request_id_value",
                 "validate_only": True,
             }
         ]
     }
     request = request_type(**request_init)
@@ -13476,14 +13504,15 @@
         },
         "read_pool_config": {"node_count": 1070},
         "ip_address": "ip_address_value",
         "reconciling": True,
         "etag": "etag_value",
         "annotations": {},
         "update_policy": {"mode": 1},
+        "satisfies_pzs": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -13700,14 +13729,15 @@
         },
         "read_pool_config": {"node_count": 1070},
         "ip_address": "ip_address_value",
         "reconciling": True,
         "etag": "etag_value",
         "annotations": {},
         "update_policy": {"mode": 1},
+        "satisfies_pzs": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -15252,14 +15282,15 @@
             type_=resources.Backup.Type.ON_DEMAND,
             description="description_value",
             cluster_uid="cluster_uid_value",
             cluster_name="cluster_name_value",
             reconciling=True,
             etag="etag_value",
             size_bytes=1089,
+            satisfies_pzs=True,
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = resources.Backup.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -15277,14 +15308,15 @@
     assert response.type_ == resources.Backup.Type.ON_DEMAND
     assert response.description == "description_value"
     assert response.cluster_uid == "cluster_uid_value"
     assert response.cluster_name == "cluster_name_value"
     assert response.reconciling is True
     assert response.etag == "etag_value"
     assert response.size_bytes == 1089
+    assert response.satisfies_pzs is True
 
 
 def test_get_backup_rest_required_fields(request_type=service.GetBackupRequest):
     transport_class = transports.AlloyDBAdminRestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -15540,14 +15572,16 @@
             "encryption_type": 1,
             "kms_key_versions": ["kms_key_versions_value1", "kms_key_versions_value2"],
         },
         "etag": "etag_value",
         "annotations": {},
         "size_bytes": 1089,
         "expiry_time": {},
+        "expiry_quantity": {"retention_count": 1632, "total_retention_count": 2275},
+        "satisfies_pzs": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -15770,14 +15804,16 @@
             "encryption_type": 1,
             "kms_key_versions": ["kms_key_versions_value1", "kms_key_versions_value2"],
         },
         "etag": "etag_value",
         "annotations": {},
         "size_bytes": 1089,
         "expiry_time": {},
+        "expiry_quantity": {"retention_count": 1632, "total_retention_count": 2275},
+        "satisfies_pzs": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -15890,14 +15926,16 @@
             "encryption_type": 1,
             "kms_key_versions": ["kms_key_versions_value1", "kms_key_versions_value2"],
         },
         "etag": "etag_value",
         "annotations": {},
         "size_bytes": 1089,
         "expiry_time": {},
+        "expiry_quantity": {"retention_count": 1632, "total_retention_count": 2275},
+        "satisfies_pzs": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -16100,14 +16138,16 @@
             "encryption_type": 1,
             "kms_key_versions": ["kms_key_versions_value1", "kms_key_versions_value2"],
         },
         "etag": "etag_value",
         "annotations": {},
         "size_bytes": 1089,
         "expiry_time": {},
+        "expiry_quantity": {"retention_count": 1632, "total_retention_count": 2275},
+        "satisfies_pzs": True,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
```

### Comparing `google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1beta/__init__.py` & `google-cloud-alloydb-0.3.0/tests/unit/gapic/alloydb_v1beta/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-alloydb-0.2.1/tests/unit/gapic/alloydb_v1beta/test_alloy_db_admin.py` & `google-cloud-alloydb-0.3.0/tests/unit/gapic/alloydb_v1beta/test_alloy_db_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

