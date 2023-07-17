# Comparing `tmp/google-cloud-kms-inventory-0.1.1.tar.gz` & `tmp/google-cloud-kms-inventory-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-kms-inventory-0.1.1.tar", last modified: Wed Jul  5 15:53:38 2023, max compression
+gzip compressed data, was "google-cloud-kms-inventory-0.2.0.tar", last modified: Mon Jul 17 13:51:21 2023, max compression
```

## Comparing `google-cloud-kms-inventory-0.1.1.tar` & `google-cloud-kms-inventory-0.2.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.065025 google-cloud-kms-inventory-0.1.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4523 2023-07-05 15:53:38.065025 google-cloud-kms-inventory-0.1.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3603 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.053025 google-cloud-kms-inventory-0.1.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.053025 google-cloud-kms-inventory-0.1.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.057025 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory/
--rw-rw-r--   0 root         (0)     1003     1961 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       87 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.057025 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/
--rw-rw-r--   0 root         (0)     1003     1642 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2377 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       87 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.057025 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.057025 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    14956 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    24901 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/client.py
--rw-rw-r--   0 root         (0)     1003     6018 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.057025 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/
--rw-rw-r--   0 root         (0)     1003     1478 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6136 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12095 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12305 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12523 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.057025 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/
--rw-rw-r--   0 root         (0)     1003      785 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    20331 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    30846 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/client.py
--rw-rw-r--   0 root         (0)     1003     6306 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.061025 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/
--rw-rw-r--   0 root         (0)     1003     1464 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6773 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13849 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14080 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    18871 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.061025 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/types/
--rw-rw-r--   0 root         (0)     1003     1143 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2810 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/types/key_dashboard_service.py
--rw-rw-r--   0 root         (0)     1003     9093 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/types/key_tracking_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.061025 google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/
--rw-r--r--   0 root         (0)     1003     4523 2023-07-05 15:53:38.000000 google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2555 2023-07-05 15:53:38.000000 google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:38.000000 google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:53:38.000000 google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:53:38.000000 google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      291 2023-07-05 15:53:38.000000 google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:53:38.000000 google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:53:38.065025 google-cloud-kms-inventory-0.1.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2931 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.061025 google-cloud-kms-inventory-0.1.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.061025 google-cloud-kms-inventory-0.1.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.061025 google-cloud-kms-inventory-0.1.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:53:38.061025 google-cloud-kms-inventory-0.1.1/tests/unit/gapic/kms_inventory_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/tests/unit/gapic/kms_inventory_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    83570 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/tests/unit/gapic/kms_inventory_v1/test_key_dashboard_service.py
--rw-rw-r--   0 root         (0)     1003   107492 2023-07-05 15:46:59.000000 google-cloud-kms-inventory-0.1.1/tests/unit/gapic/kms_inventory_v1/test_key_tracking_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:21.401055 google-cloud-kms-inventory-0.2.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4523 2023-07-17 13:51:21.401055 google-cloud-kms-inventory-0.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3603 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:21.389053 google-cloud-kms-inventory-0.2.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:21.389053 google-cloud-kms-inventory-0.2.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:21.393054 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory/
+-rw-rw-r--   0 root         (0)     1003     1961 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       87 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:21.393054 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/
+-rw-rw-r--   0 root         (0)     1003     1642 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2377 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       87 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:21.393054 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:21.393054 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14956 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    24901 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6018 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:21.393054 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1478 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6136 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12095 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12305 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12523 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:21.397054 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/
+-rw-rw-r--   0 root         (0)     1003      785 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20331 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    30846 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6306 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:21.397054 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1464 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6773 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13849 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14080 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    18871 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:21.397054 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1143 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2810 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/types/key_dashboard_service.py
+-rw-rw-r--   0 root         (0)     1003    10153 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/types/key_tracking_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:21.397054 google-cloud-kms-inventory-0.2.0/google_cloud_kms_inventory.egg-info/
+-rw-r--r--   0 root         (0)     1003     4523 2023-07-17 13:51:21.000000 google-cloud-kms-inventory-0.2.0/google_cloud_kms_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2555 2023-07-17 13:51:21.000000 google-cloud-kms-inventory-0.2.0/google_cloud_kms_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-17 13:51:21.000000 google-cloud-kms-inventory-0.2.0/google_cloud_kms_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-17 13:51:21.000000 google-cloud-kms-inventory-0.2.0/google_cloud_kms_inventory.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-17 13:51:21.000000 google-cloud-kms-inventory-0.2.0/google_cloud_kms_inventory.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      291 2023-07-17 13:51:21.000000 google-cloud-kms-inventory-0.2.0/google_cloud_kms_inventory.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-17 13:51:21.000000 google-cloud-kms-inventory-0.2.0/google_cloud_kms_inventory.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-17 13:51:21.401055 google-cloud-kms-inventory-0.2.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2931 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:21.397054 google-cloud-kms-inventory-0.2.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:21.401055 google-cloud-kms-inventory-0.2.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:21.401055 google-cloud-kms-inventory-0.2.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-17 13:51:21.401055 google-cloud-kms-inventory-0.2.0/tests/unit/gapic/kms_inventory_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/tests/unit/gapic/kms_inventory_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    83769 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/tests/unit/gapic/kms_inventory_v1/test_key_dashboard_service.py
+-rw-rw-r--   0 root         (0)     1003   107555 2023-07-17 13:48:21.000000 google-cloud-kms-inventory-0.2.0/tests/unit/gapic/kms_inventory_v1/test_key_tracking_service.py
```

### Comparing `google-cloud-kms-inventory-0.1.1/LICENSE` & `google-cloud-kms-inventory-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.1/MANIFEST.in` & `google-cloud-kms-inventory-0.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.1/PKG-INFO` & `google-cloud-kms-inventory-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-kms-inventory
-Version: 0.1.1
+Version: 0.2.0
 Summary: Google Cloud Kms Inventory API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-kms-inventory-0.1.1/README.rst` & `google-cloud-kms-inventory-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory/__init__.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory/__init__.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory/gapic_version.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
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
-__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/__init__.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/__init__.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/gapic_metadata.json` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/gapic_version.py` & `google-cloud-kms-inventory-0.2.0/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
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
-__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/__init__.py` & `google-cloud-kms-inventory-0.2.0/tests/unit/__init__.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/__init__.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/__init__.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/async_client.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/async_client.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/client.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/client.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/pagers.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/pagers.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/__init__.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/__init__.py`

 * *Files 2% similar despite different names*

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/base.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/base.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/grpc.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/grpc.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/grpc_asyncio.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/rest.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_dashboard_service/transports/rest.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/__init__.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/__init__.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/async_client.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/async_client.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/client.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/client.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/pagers.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/pagers.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/__init__.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/__init__.py`

 * *Files 2% similar despite different names*

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/base.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/base.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/grpc.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/grpc.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/grpc_asyncio.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/rest.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/services/key_tracking_service/transports/rest.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/types/__init__.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/types/__init__.py`

 * *Files 8% similar despite different names*

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/types/key_dashboard_service.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/types/key_dashboard_service.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/google/cloud/kms_inventory_v1/types/key_tracking_service.py` & `google-cloud-kms-inventory-0.2.0/google/cloud/kms_inventory_v1/types/key_tracking_service.py`

 * *Files 9% similar despite different names*

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
@@ -52,14 +52,15 @@
     r"""Aggregate information about the resources protected by a
     Cloud KMS key in the same Cloud organization as the key.
 
     Attributes:
         name (str):
             The full name of the
             ProtectedResourcesSummary resource. Example:
+
             projects/test-project/locations/us/keyRings/test-keyring/cryptoKeys/test-key/protectedResourcesSummary
         resource_count (int):
             The total number of protected resources in
             the same Cloud organization as the key.
         project_count (int):
             The number of distinct Cloud projects in the
             same Cloud organization as the key that have
@@ -125,14 +126,33 @@
             A page token, received from a previous
             [KeyTrackingService.SearchProtectedResources][google.cloud.kms.inventory.v1.KeyTrackingService.SearchProtectedResources]
             call. Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to
             [KeyTrackingService.SearchProtectedResources][google.cloud.kms.inventory.v1.KeyTrackingService.SearchProtectedResources]
             must match the call that provided the page token.
+        resource_types (MutableSequence[str]):
+            Optional. A list of resource types that this request
+            searches for. If empty, it will search all the `trackable
+            resource
+            types <https://cloud.google.com/kms/docs/view-key-usage#tracked-resource-types>`__.
+
+            Regular expressions are also supported. For example:
+
+            -  ``compute.googleapis.com.*`` snapshots resources whose
+               type starts with ``compute.googleapis.com``.
+            -  ``.*Image`` snapshots resources whose type ends with
+               ``Image``.
+            -  ``.*Image.*`` snapshots resources whose type contains
+               ``Image``.
+
+            See `RE2 <https://github.com/google/re2/wiki/Syntax>`__ for
+            all supported regular expression syntax. If the regular
+            expression does not match any supported resource type, an
+            INVALID_ARGUMENT error will be returned.
     """
 
     scope: str = proto.Field(
         proto.STRING,
         number=2,
     )
     crypto_key: str = proto.Field(
@@ -143,14 +163,18 @@
         proto.INT32,
         number=3,
     )
     page_token: str = proto.Field(
         proto.STRING,
         number=4,
     )
+    resource_types: MutableSequence[str] = proto.RepeatedField(
+        proto.STRING,
+        number=5,
+    )
 
 
 class SearchProtectedResourcesResponse(proto.Message):
     r"""Response message for
     [KeyTrackingService.SearchProtectedResources][google.cloud.kms.inventory.v1.KeyTrackingService.SearchProtectedResources].
 
     Attributes:
```

### Comparing `google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/PKG-INFO` & `google-cloud-kms-inventory-0.2.0/google_cloud_kms_inventory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-kms-inventory
-Version: 0.1.1
+Version: 0.2.0
 Summary: Google Cloud Kms Inventory API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-kms-inventory-0.1.1/google_cloud_kms_inventory.egg-info/SOURCES.txt` & `google-cloud-kms-inventory-0.2.0/google_cloud_kms_inventory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-inventory-0.1.1/setup.py` & `google-cloud-kms-inventory-0.2.0/setup.py`

 * *Files 2% similar despite different names*

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

### Comparing `google-cloud-kms-inventory-0.1.1/tests/__init__.py` & `google-cloud-kms-inventory-0.2.0/tests/unit/gapic/__init__.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/tests/unit/__init__.py` & `google-cloud-kms-inventory-0.2.0/tests/unit/gapic/kms_inventory_v1/__init__.py`

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

### Comparing `google-cloud-kms-inventory-0.1.1/tests/unit/gapic/kms_inventory_v1/test_key_dashboard_service.py` & `google-cloud-kms-inventory-0.2.0/tests/unit/gapic/kms_inventory_v1/test_key_dashboard_service.py`

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
@@ -1158,17 +1158,19 @@
                     resources.CryptoKey(),
                     resources.CryptoKey(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_crypto_keys(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-kms-inventory-0.1.1/tests/unit/gapic/kms_inventory_v1/test_key_tracking_service.py` & `google-cloud-kms-inventory-0.2.0/tests/unit/gapic/kms_inventory_v1/test_key_tracking_service.py`

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
@@ -1816,14 +1816,15 @@
     ).search_protected_resources._get_unset_required_fields(jsonified_request)
     # Check that path parameters and body parameters are not mixing in.
     assert not set(unset_fields) - set(
         (
             "crypto_key",
             "page_size",
             "page_token",
+            "resource_types",
         )
     )
     jsonified_request.update(unset_fields)
 
     # verify required fields with non-default values are left alone
     assert "scope" in jsonified_request
     assert jsonified_request["scope"] == "scope_value"
@@ -1886,14 +1887,15 @@
     unset_fields = transport.search_protected_resources._get_unset_required_fields({})
     assert set(unset_fields) == (
         set(
             (
                 "cryptoKey",
                 "pageSize",
                 "pageToken",
+                "resourceTypes",
             )
         )
         & set(
             (
                 "scope",
                 "cryptoKey",
             )
```

