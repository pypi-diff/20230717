# Comparing `tmp/google-cloud-documentai-2.9.0.tar.gz` & `tmp/google-cloud-documentai-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-documentai-2.9.0.tar", last modified: Tue Jan 17 21:46:10 2023, max compression
+gzip compressed data, was "google-cloud-documentai-2.9.1.tar", last modified: Fri Jan 20 20:18:12 2023, max compression
```

## Comparing `google-cloud-documentai-2.9.0.tar` & `google-cloud-documentai-2.9.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.195739 google-cloud-documentai-2.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4686 2023-01-17 21:46:10.195739 google-cloud-documentai-2.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3761 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.171737 google-cloud-documentai-2.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.175737 google-cloud-documentai-2.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.179738 google-cloud-documentai-2.9.0/google/cloud/documentai/
--rw-rw-r--   0 root         (0)     1003     4783 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.179738 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/
--rw-rw-r--   0 root         (0)     1003     4407 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     5355 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.179738 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.179738 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/
--rw-rw-r--   0 root         (0)     1003      809 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   105477 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   118251 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/client.py
--rw-rw-r--   0 root         (0)     1003    16858 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.179738 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/transports/
--rw-rw-r--   0 root         (0)     1003     1291 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    17376 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    38867 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    39555 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.183738 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/
--rw-rw-r--   0 root         (0)     1003     4028 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2693 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/barcode.py
--rw-rw-r--   0 root         (0)     1003    64995 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/document.py
--rw-rw-r--   0 root         (0)     1003     6480 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/document_io.py
--rw-rw-r--   0 root         (0)     1003    30403 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/document_processor_service.py
--rw-rw-r--   0 root         (0)     1003     8495 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/document_schema.py
--rw-rw-r--   0 root         (0)     1003     2572 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003     2358 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/operation_metadata.py
--rw-rw-r--   0 root         (0)     1003     6963 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/processor.py
--rw-rw-r--   0 root         (0)     1003     3230 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/processor_type.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.183738 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/
--rw-rw-r--   0 root         (0)     1003     1966 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003     1133 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.183738 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.183738 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/document_understanding_service/
--rw-rw-r--   0 root         (0)     1003      825 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/document_understanding_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    19694 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/document_understanding_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    27406 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/document_understanding_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.183738 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/
--rw-rw-r--   0 root         (0)     1003     1327 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7607 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14009 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14324 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.187739 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/types/
--rw-rw-r--   0 root         (0)     1003     1603 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    40760 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/types/document.py
--rw-rw-r--   0 root         (0)     1003    18566 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/types/document_understanding.py
--rw-rw-r--   0 root         (0)     1003     2493 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/types/geometry.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.187739 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/
--rw-rw-r--   0 root         (0)     1003     5158 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/__init__.py
--rw-rw-r--   0 root         (0)     1003     6429 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.187739 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.187739 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/
--rw-rw-r--   0 root         (0)     1003      809 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   125985 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   140395 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/client.py
--rw-rw-r--   0 root         (0)     1003    22278 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.191739 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/transports/
--rw-rw-r--   0 root         (0)     1003     1291 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    19364 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    44082 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    44867 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.191739 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/
--rw-rw-r--   0 root         (0)     1003     4773 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2698 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/barcode.py
--rw-rw-r--   0 root         (0)     1003    65755 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/document.py
--rw-rw-r--   0 root         (0)     1003     6930 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/document_io.py
--rw-rw-r--   0 root         (0)     1003    46364 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/document_processor_service.py
--rw-rw-r--   0 root         (0)     1003     8525 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/document_schema.py
--rw-rw-r--   0 root         (0)     1003     9911 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/evaluation.py
--rw-rw-r--   0 root         (0)     1003     2587 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/geometry.py
--rw-rw-r--   0 root         (0)     1003     2368 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/operation_metadata.py
--rw-rw-r--   0 root         (0)     1003     6998 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/processor.py
--rw-rw-r--   0 root         (0)     1003     3240 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/processor_type.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.195739 google-cloud-documentai-2.9.0/google_cloud_documentai.egg-info/
--rw-r--r--   0 root         (0)     1003     4686 2023-01-17 21:46:10.000000 google-cloud-documentai-2.9.0/google_cloud_documentai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     4862 2023-01-17 21:46:10.000000 google-cloud-documentai-2.9.0/google_cloud_documentai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-17 21:46:10.000000 google-cloud-documentai-2.9.0/google_cloud_documentai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-17 21:46:10.000000 google-cloud-documentai-2.9.0/google_cloud_documentai.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-17 21:46:10.000000 google-cloud-documentai-2.9.0/google_cloud_documentai.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-01-17 21:46:10.000000 google-cloud-documentai-2.9.0/google_cloud_documentai.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-17 21:46:10.000000 google-cloud-documentai-2.9.0/google_cloud_documentai.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-17 21:46:10.199740 google-cloud-documentai-2.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2986 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.195739 google-cloud-documentai-2.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.195739 google-cloud-documentai-2.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.195739 google-cloud-documentai-2.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.195739 google-cloud-documentai-2.9.0/tests/unit/gapic/documentai_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/tests/unit/gapic/documentai_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   258437 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/tests/unit/gapic/documentai_v1/test_document_processor_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.195739 google-cloud-documentai-2.9.0/tests/unit/gapic/documentai_v1beta2/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/tests/unit/gapic/documentai_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003    69078 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/tests/unit/gapic/documentai_v1beta2/test_document_understanding_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-17 21:46:10.195739 google-cloud-documentai-2.9.0/tests/unit/gapic/documentai_v1beta3/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/tests/unit/gapic/documentai_v1beta3/__init__.py
--rw-rw-r--   0 root         (0)     1003   302616 2023-01-17 21:42:21.000000 google-cloud-documentai-2.9.0/tests/unit/gapic/documentai_v1beta3/test_document_processor_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.403174 google-cloud-documentai-2.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4686 2023-01-20 20:18:12.403174 google-cloud-documentai-2.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3761 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.379169 google-cloud-documentai-2.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.383170 google-cloud-documentai-2.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.383170 google-cloud-documentai-2.9.1/google/cloud/documentai/
+-rw-rw-r--   0 root         (0)     1003     4783 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.387171 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/
+-rw-rw-r--   0 root         (0)     1003     4407 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5355 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.387171 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.387171 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/
+-rw-rw-r--   0 root         (0)     1003      809 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   105477 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   118287 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16858 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.387171 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1291 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17376 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    38867 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    39555 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.391172 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/
+-rw-rw-r--   0 root         (0)     1003     4028 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2693 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/barcode.py
+-rw-rw-r--   0 root         (0)     1003    68687 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/document.py
+-rw-rw-r--   0 root         (0)     1003     6480 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/document_io.py
+-rw-rw-r--   0 root         (0)     1003    32547 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/document_processor_service.py
+-rw-rw-r--   0 root         (0)     1003     9185 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/document_schema.py
+-rw-rw-r--   0 root         (0)     1003     2572 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003     2786 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/operation_metadata.py
+-rw-rw-r--   0 root         (0)     1003     9345 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/processor.py
+-rw-rw-r--   0 root         (0)     1003     3230 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/processor_type.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.391172 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/
+-rw-rw-r--   0 root         (0)     1003     1966 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1133 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.391172 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.391172 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/document_understanding_service/
+-rw-rw-r--   0 root         (0)     1003      825 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/document_understanding_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19694 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/document_understanding_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27446 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/document_understanding_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.391172 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1327 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7607 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14009 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14324 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.391172 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/types/
+-rw-rw-r--   0 root         (0)     1003     1603 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    43594 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/types/document.py
+-rw-rw-r--   0 root         (0)     1003    19180 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/types/document_understanding.py
+-rw-rw-r--   0 root         (0)     1003     2493 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/types/geometry.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.395173 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/
+-rw-rw-r--   0 root         (0)     1003     5158 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6429 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.395173 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.395173 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/
+-rw-rw-r--   0 root         (0)     1003      809 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   125985 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   140431 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/client.py
+-rw-rw-r--   0 root         (0)     1003    22278 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.395173 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1291 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19364 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    44082 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    44867 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.399174 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/
+-rw-rw-r--   0 root         (0)     1003     4773 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2698 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/barcode.py
+-rw-rw-r--   0 root         (0)     1003    69482 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/document.py
+-rw-rw-r--   0 root         (0)     1003     6930 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/document_io.py
+-rw-rw-r--   0 root         (0)     1003    48936 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/document_processor_service.py
+-rw-rw-r--   0 root         (0)     1003     9215 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/document_schema.py
+-rw-rw-r--   0 root         (0)     1003    10735 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/evaluation.py
+-rw-rw-r--   0 root         (0)     1003     2587 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003     2796 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/operation_metadata.py
+-rw-rw-r--   0 root         (0)     1003     9380 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/processor.py
+-rw-rw-r--   0 root         (0)     1003     3240 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/processor_type.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.399174 google-cloud-documentai-2.9.1/google_cloud_documentai.egg-info/
+-rw-r--r--   0 root         (0)     1003     4686 2023-01-20 20:18:12.000000 google-cloud-documentai-2.9.1/google_cloud_documentai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     4862 2023-01-20 20:18:12.000000 google-cloud-documentai-2.9.1/google_cloud_documentai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-20 20:18:12.000000 google-cloud-documentai-2.9.1/google_cloud_documentai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-01-20 20:18:12.000000 google-cloud-documentai-2.9.1/google_cloud_documentai.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-20 20:18:12.000000 google-cloud-documentai-2.9.1/google_cloud_documentai.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-01-20 20:18:12.000000 google-cloud-documentai-2.9.1/google_cloud_documentai.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-01-20 20:18:12.000000 google-cloud-documentai-2.9.1/google_cloud_documentai.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-01-20 20:18:12.403174 google-cloud-documentai-2.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2986 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.399174 google-cloud-documentai-2.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.399174 google-cloud-documentai-2.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.399174 google-cloud-documentai-2.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.399174 google-cloud-documentai-2.9.1/tests/unit/gapic/documentai_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/tests/unit/gapic/documentai_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   258437 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/tests/unit/gapic/documentai_v1/test_document_processor_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.403174 google-cloud-documentai-2.9.1/tests/unit/gapic/documentai_v1beta2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/tests/unit/gapic/documentai_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    69078 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/tests/unit/gapic/documentai_v1beta2/test_document_understanding_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-20 20:18:12.403174 google-cloud-documentai-2.9.1/tests/unit/gapic/documentai_v1beta3/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/tests/unit/gapic/documentai_v1beta3/__init__.py
+-rw-rw-r--   0 root         (0)     1003   302616 2023-01-20 20:14:41.000000 google-cloud-documentai-2.9.1/tests/unit/gapic/documentai_v1beta3/test_document_processor_service.py
```

### Comparing `google-cloud-documentai-2.9.0/LICENSE` & `google-cloud-documentai-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/MANIFEST.in` & `google-cloud-documentai-2.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/PKG-INFO` & `google-cloud-documentai-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-documentai
-Version: 2.9.0
+Version: 2.9.1
 Summary: Google Cloud Documentai API client library
 Home-page: https://github.com/googleapis/python-documentai
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-documentai-2.9.0/README.rst` & `google-cloud-documentai-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai/__init__.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai/gapic_version.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/__init__.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/gapic_metadata.json` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/gapic_version.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/__init__.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/__init__.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/async_client.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/client.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2619,15 +2619,15 @@
             document_processor_service.ReviewDocumentResponse,
             metadata_type=document_processor_service.ReviewDocumentOperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "DocumentProcessorServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/pagers.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/transports/__init__.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/transports/base.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/transports/grpc.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/services/document_processor_service/transports/grpc_asyncio.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/services/document_processor_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/__init__.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/barcode.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/barcode.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/document.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/document.py`

 * *Files 3% similar despite different names*

```diff
@@ -392,15 +392,33 @@
                     [Layout][google.cloud.documentai.v1.Document.Page.Layout].
                 orientation (google.cloud.documentai_v1.types.Document.Page.Layout.Orientation):
                     Detected orientation for the
                     [Layout][google.cloud.documentai.v1.Document.Page.Layout].
             """
 
             class Orientation(proto.Enum):
-                r"""Detected human reading orientation."""
+                r"""Detected human reading orientation.
+
+                Values:
+                    ORIENTATION_UNSPECIFIED (0):
+                        Unspecified orientation.
+                    PAGE_UP (1):
+                        Orientation is aligned with page up.
+                    PAGE_RIGHT (2):
+                        Orientation is aligned with page right.
+                        Turn the head 90 degrees clockwise from upright
+                        to read.
+                    PAGE_DOWN (3):
+                        Orientation is aligned with page down.
+                        Turn the head 180 degrees from upright to read.
+                    PAGE_LEFT (4):
+                        Orientation is aligned with page left.
+                        Turn the head 90 degrees counterclockwise from
+                        upright to read.
+                """
                 ORIENTATION_UNSPECIFIED = 0
                 PAGE_UP = 1
                 PAGE_RIGHT = 2
                 PAGE_DOWN = 3
                 PAGE_LEFT = 4
 
             text_anchor: "Document.TextAnchor" = proto.Field(
@@ -547,15 +565,27 @@
 
                 Attributes:
                     type_ (google.cloud.documentai_v1.types.Document.Page.Token.DetectedBreak.Type):
                         Detected break type.
                 """
 
                 class Type(proto.Enum):
-                    r"""Enum to denote the type of break found."""
+                    r"""Enum to denote the type of break found.
+
+                    Values:
+                        TYPE_UNSPECIFIED (0):
+                            Unspecified break type.
+                        SPACE (1):
+                            A single whitespace.
+                        WIDE_SPACE (2):
+                            A wider whitespace.
+                        HYPHEN (3):
+                            A hyphen that indicates that a token has been
+                            split across lines.
+                    """
                     TYPE_UNSPECIFIED = 0
                     SPACE = 1
                     WIDE_SPACE = 2
                     HYPHEN = 3
 
                 type_: "Document.Page.Token.DetectedBreak.Type" = proto.Field(
                     proto.ENUM,
@@ -1340,15 +1370,48 @@
                     a layout element on the page.
                 confidence (float):
                     Optional. Confidence of detected page element, if
                     applicable. Range ``[0, 1]``.
             """
 
             class LayoutType(proto.Enum):
-                r"""The type of layout that is being referenced."""
+                r"""The type of layout that is being referenced.
+
+                Values:
+                    LAYOUT_TYPE_UNSPECIFIED (0):
+                        Layout Unspecified.
+                    BLOCK (1):
+                        References a
+                        [Page.blocks][google.cloud.documentai.v1.Document.Page.blocks]
+                        element.
+                    PARAGRAPH (2):
+                        References a
+                        [Page.paragraphs][google.cloud.documentai.v1.Document.Page.paragraphs]
+                        element.
+                    LINE (3):
+                        References a
+                        [Page.lines][google.cloud.documentai.v1.Document.Page.lines]
+                        element.
+                    TOKEN (4):
+                        References a
+                        [Page.tokens][google.cloud.documentai.v1.Document.Page.tokens]
+                        element.
+                    VISUAL_ELEMENT (5):
+                        References a
+                        [Page.visual_elements][google.cloud.documentai.v1.Document.Page.visual_elements]
+                        element.
+                    TABLE (6):
+                        Refrrences a
+                        [Page.tables][google.cloud.documentai.v1.Document.Page.tables]
+                        element.
+                    FORM_FIELD (7):
+                        References a
+                        [Page.form_fields][google.cloud.documentai.v1.Document.Page.form_fields]
+                        element.
+                """
                 LAYOUT_TYPE_UNSPECIFIED = 0
                 BLOCK = 1
                 PARAGRAPH = 2
                 LINE = 3
                 TOKEN = 4
                 VISUAL_ELEMENT = 5
                 TABLE = 6
@@ -1400,14 +1463,34 @@
             type_ (google.cloud.documentai_v1.types.Document.Provenance.OperationType):
                 The type of provenance operation.
         """
 
         class OperationType(proto.Enum):
             r"""If a processor or agent does an explicit operation on
             existing elements.
+
+            Values:
+                OPERATION_TYPE_UNSPECIFIED (0):
+                    Operation type unspecified. If no operation is specified a
+                    provenance entry is simply used to match against a
+                    ``parent``.
+                ADD (1):
+                    Add an element.
+                REMOVE (2):
+                    Remove an element identified by ``parent``.
+                REPLACE (3):
+                    Replace an element identified by ``parent``.
+                EVAL_REQUESTED (4):
+                    Request human review for the element identified by
+                    ``parent``.
+                EVAL_APPROVED (5):
+                    Element is reviewed and approved at human
+                    review, confidence will be set to 1.0.
+                EVAL_SKIPPED (6):
+                    Element is skipped in the validation process.
             """
             OPERATION_TYPE_UNSPECIFIED = 0
             ADD = 1
             REMOVE = 2
             REPLACE = 3
             EVAL_REQUESTED = 4
             EVAL_APPROVED = 5
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/document_io.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/document_io.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/document_processor_service.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/document_processor_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,35 @@
             document. This field is populated only when the [state] is
             [HUMAN_REVIEW_IN_PROGRESS]. It has the same response type
             and metadata as the long running operation returned by
             [ReviewDocument] method.
     """
 
     class State(proto.Enum):
-        r"""The final state of human review on a processed document."""
+        r"""The final state of human review on a processed document.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                Human review state is unspecified. Most
+                likely due to an internal error.
+            SKIPPED (1):
+                Human review is skipped for the document.
+                This can happen because human review is not
+                enabled on the processor or the processing
+                request has been set to skip this document.
+            VALIDATION_PASSED (2):
+                Human review validation is triggered and
+                passed, so no review is needed.
+            IN_PROGRESS (3):
+                Human review validation is triggered and the
+                document is under review.
+            ERROR (4):
+                Some error happened during triggering human review, see the
+                [state_message] for details.
+        """
         STATE_UNSPECIFIED = 0
         SKIPPED = 1
         VALIDATION_PASSED = 2
         IN_PROGRESS = 3
         ERROR = 4
 
     state: State = proto.Field(
@@ -268,15 +288,33 @@
             The last update time of the operation.
         individual_process_statuses (MutableSequence[google.cloud.documentai_v1.types.BatchProcessMetadata.IndividualProcessStatus]):
             The list of response details of each
             document.
     """
 
     class State(proto.Enum):
-        r"""Possible states of the batch processing operation."""
+        r"""Possible states of the batch processing operation.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The default value. This value is used if the
+                state is omitted.
+            WAITING (1):
+                Request operation is waiting for scheduling.
+            RUNNING (2):
+                Request is being processed.
+            SUCCEEDED (3):
+                The batch processing completed successfully.
+            CANCELLING (4):
+                The batch processing was being cancelled.
+            CANCELLED (5):
+                The batch processing was cancelled.
+            FAILED (6):
+                The batch processing has failed.
+        """
         STATE_UNSPECIFIED = 0
         WAITING = 1
         RUNNING = 2
         SUCCEEDED = 3
         CANCELLING = 4
         CANCELLED = 5
         FAILED = 6
@@ -914,15 +952,25 @@
         priority (google.cloud.documentai_v1.types.ReviewDocumentRequest.Priority):
             The priority of the human review task.
         document_schema (google.cloud.documentai_v1.types.DocumentSchema):
             The document schema of the human review task.
     """
 
     class Priority(proto.Enum):
-        r"""The priority level of the human review task."""
+        r"""The priority level of the human review task.
+
+        Values:
+            DEFAULT (0):
+                The default priority level.
+            URGENT (1):
+                The urgent priority level. The labeling
+                manager should allocate labeler resource to the
+                urgent task queue to respect this priority
+                level.
+        """
         DEFAULT = 0
         URGENT = 1
 
     inline_document: gcd_document.Document = proto.Field(
         proto.MESSAGE,
         number=4,
         oneof="source",
@@ -959,15 +1007,26 @@
             The state of the review operation.
         rejection_reason (str):
             The reason why the review is rejected by
             reviewer.
     """
 
     class State(proto.Enum):
-        r"""Possible states of the review operation."""
+        r"""Possible states of the review operation.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The default value. This value is used if the
+                state is omitted.
+            REJECTED (1):
+                The review operation is rejected by the
+                reviewer.
+            SUCCEEDED (2):
+                The review operation is succeeded.
+        """
         STATE_UNSPECIFIED = 0
         REJECTED = 1
         SUCCEEDED = 2
 
     gcs_destination: str = proto.Field(
         proto.STRING,
         number=1,
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/document_schema.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/document_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,14 +115,30 @@
                     document.
             """
 
             class OccurrenceType(proto.Enum):
                 r"""Types of occurrences of the entity type in the document.
                 Note: this represents the number of instances of an entity
                 types, not number of mentions of a given entity instance.
+
+                Values:
+                    OCCURRENCE_TYPE_UNSPECIFIED (0):
+                        Unspecified occurrence type.
+                    OPTIONAL_ONCE (1):
+                        There will be zero or one instance of this
+                        entity type.
+                    OPTIONAL_MULTIPLE (2):
+                        The entity type will appear zero or multiple
+                        times.
+                    REQUIRED_ONCE (3):
+                        The entity type will only appear exactly
+                        once.
+                    REQUIRED_MULTIPLE (4):
+                        The entity type will appear once or more
+                        times.
                 """
                 OCCURRENCE_TYPE_UNSPECIFIED = 0
                 OPTIONAL_ONCE = 1
                 OPTIONAL_MULTIPLE = 2
                 REQUIRED_ONCE = 3
                 REQUIRED_MULTIPLE = 4
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/geometry.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/operation_metadata.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/operation_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,30 @@
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             The creation time of the operation.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             The last update time of the operation.
     """
 
     class State(proto.Enum):
-        r"""State of the longrunning operation."""
+        r"""State of the longrunning operation.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                Unspecified state.
+            RUNNING (1):
+                Operation is still running.
+            CANCELLING (2):
+                Operation is being cancelled.
+            SUCCEEDED (3):
+                Operation succeeded.
+            FAILED (4):
+                Operation failed.
+            CANCELLED (5):
+                Operation is cancelled.
+        """
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         CANCELLING = 2
         SUCCEEDED = 3
         FAILED = 4
         CANCELLED = 5
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1/types/processor_type.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1/types/processor_type.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/__init__.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/gapic_metadata.json` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/gapic_version.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/__init__.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/document_understanding_service/__init__.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/document_understanding_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/document_understanding_service/async_client.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/document_understanding_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/document_understanding_service/client.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/document_understanding_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -642,15 +642,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "DocumentUnderstandingServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/__init__.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/base.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/grpc.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/grpc_asyncio.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/services/document_understanding_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/types/__init__.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/types/document.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/types/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -336,15 +336,33 @@
                     [Layout][google.cloud.documentai.v1beta2.Document.Page.Layout].
                 id (str):
                     Optional. This is the identifier used by referencing
                     [PageAnchor][google.cloud.documentai.v1beta2.Document.PageAnchor]s.
             """
 
             class Orientation(proto.Enum):
-                r"""Detected human reading orientation."""
+                r"""Detected human reading orientation.
+
+                Values:
+                    ORIENTATION_UNSPECIFIED (0):
+                        Unspecified orientation.
+                    PAGE_UP (1):
+                        Orientation is aligned with page up.
+                    PAGE_RIGHT (2):
+                        Orientation is aligned with page right.
+                        Turn the head 90 degrees clockwise from upright
+                        to read.
+                    PAGE_DOWN (3):
+                        Orientation is aligned with page down.
+                        Turn the head 180 degrees from upright to read.
+                    PAGE_LEFT (4):
+                        Orientation is aligned with page left.
+                        Turn the head 90 degrees counterclockwise from
+                        upright to read.
+                """
                 ORIENTATION_UNSPECIFIED = 0
                 PAGE_UP = 1
                 PAGE_RIGHT = 2
                 PAGE_DOWN = 3
                 PAGE_LEFT = 4
 
             text_anchor: "Document.TextAnchor" = proto.Field(
@@ -475,15 +493,27 @@
 
                 Attributes:
                     type_ (google.cloud.documentai_v1beta2.types.Document.Page.Token.DetectedBreak.Type):
                         Detected break type.
                 """
 
                 class Type(proto.Enum):
-                    r"""Enum to denote the type of break found."""
+                    r"""Enum to denote the type of break found.
+
+                    Values:
+                        TYPE_UNSPECIFIED (0):
+                            Unspecified break type.
+                        SPACE (1):
+                            A single whitespace.
+                        WIDE_SPACE (2):
+                            A wider whitespace.
+                        HYPHEN (3):
+                            A hyphen that indicates that a token has been
+                            split across lines.
+                    """
                     TYPE_UNSPECIFIED = 0
                     SPACE = 1
                     WIDE_SPACE = 2
                     HYPHEN = 3
 
                 type_: "Document.Page.Token.DetectedBreak.Type" = proto.Field(
                     proto.ENUM,
@@ -957,15 +987,48 @@
                     [Page.Layout.id][google.cloud.documentai.v1beta2.Document.Page.Layout.id]
                     on the page that this element references. If
                     [LayoutRef.type][] is specified this id must also be
                     specified.
             """
 
             class LayoutType(proto.Enum):
-                r"""The type of layout that is being referenced."""
+                r"""The type of layout that is being referenced.
+
+                Values:
+                    LAYOUT_TYPE_UNSPECIFIED (0):
+                        Layout Unspecified.
+                    BLOCK (1):
+                        References a
+                        [Page.blocks][google.cloud.documentai.v1beta2.Document.Page.blocks]
+                        element.
+                    PARAGRAPH (2):
+                        References a
+                        [Page.paragraphs][google.cloud.documentai.v1beta2.Document.Page.paragraphs]
+                        element.
+                    LINE (3):
+                        References a
+                        [Page.lines][google.cloud.documentai.v1beta2.Document.Page.lines]
+                        element.
+                    TOKEN (4):
+                        References a
+                        [Page.tokens][google.cloud.documentai.v1beta2.Document.Page.tokens]
+                        element.
+                    VISUAL_ELEMENT (5):
+                        References a
+                        [Page.visual_elements][google.cloud.documentai.v1beta2.Document.Page.visual_elements]
+                        element.
+                    TABLE (6):
+                        Refrrences a
+                        [Page.tables][google.cloud.documentai.v1beta2.Document.Page.tables]
+                        element.
+                    FORM_FIELD (7):
+                        References a
+                        [Page.form_fields][google.cloud.documentai.v1beta2.Document.Page.form_fields]
+                        element.
+                """
                 LAYOUT_TYPE_UNSPECIFIED = 0
                 BLOCK = 1
                 PARAGRAPH = 2
                 LINE = 3
                 TOKEN = 4
                 VISUAL_ELEMENT = 5
                 TABLE = 6
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/types/document_understanding.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/types/document_understanding.py`

 * *Files 1% similar despite different names*

```diff
@@ -536,15 +536,33 @@
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             The creation time of the operation.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             The last update time of the operation.
     """
 
     class State(proto.Enum):
-        r""""""
+        r"""
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The default value. This value is used if the
+                state is omitted.
+            ACCEPTED (1):
+                Request is received.
+            WAITING (2):
+                Request operation is waiting for scheduling.
+            RUNNING (3):
+                Request is being processed.
+            SUCCEEDED (4):
+                The batch processing completed successfully.
+            CANCELLED (5):
+                The batch processing was cancelled.
+            FAILED (6):
+                The batch processing has failed.
+        """
         STATE_UNSPECIFIED = 0
         ACCEPTED = 1
         WAITING = 2
         RUNNING = 3
         SUCCEEDED = 4
         CANCELLED = 5
         FAILED = 6
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta2/types/geometry.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta2/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/__init__.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/gapic_metadata.json` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/gapic_version.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/__init__.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/__init__.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/async_client.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/client.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3135,15 +3135,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "DocumentProcessorServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/pagers.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/transports/__init__.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/transports/base.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/transports/grpc.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/services/document_processor_service/transports/grpc_asyncio.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/services/document_processor_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/__init__.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/barcode.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/barcode.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/document.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -392,15 +392,33 @@
                     [Layout][google.cloud.documentai.v1beta3.Document.Page.Layout].
                 orientation (google.cloud.documentai_v1beta3.types.Document.Page.Layout.Orientation):
                     Detected orientation for the
                     [Layout][google.cloud.documentai.v1beta3.Document.Page.Layout].
             """
 
             class Orientation(proto.Enum):
-                r"""Detected human reading orientation."""
+                r"""Detected human reading orientation.
+
+                Values:
+                    ORIENTATION_UNSPECIFIED (0):
+                        Unspecified orientation.
+                    PAGE_UP (1):
+                        Orientation is aligned with page up.
+                    PAGE_RIGHT (2):
+                        Orientation is aligned with page right.
+                        Turn the head 90 degrees clockwise from upright
+                        to read.
+                    PAGE_DOWN (3):
+                        Orientation is aligned with page down.
+                        Turn the head 180 degrees from upright to read.
+                    PAGE_LEFT (4):
+                        Orientation is aligned with page left.
+                        Turn the head 90 degrees counterclockwise from
+                        upright to read.
+                """
                 ORIENTATION_UNSPECIFIED = 0
                 PAGE_UP = 1
                 PAGE_RIGHT = 2
                 PAGE_DOWN = 3
                 PAGE_LEFT = 4
 
             text_anchor: "Document.TextAnchor" = proto.Field(
@@ -550,15 +568,27 @@
 
                 Attributes:
                     type_ (google.cloud.documentai_v1beta3.types.Document.Page.Token.DetectedBreak.Type):
                         Detected break type.
                 """
 
                 class Type(proto.Enum):
-                    r"""Enum to denote the type of break found."""
+                    r"""Enum to denote the type of break found.
+
+                    Values:
+                        TYPE_UNSPECIFIED (0):
+                            Unspecified break type.
+                        SPACE (1):
+                            A single whitespace.
+                        WIDE_SPACE (2):
+                            A wider whitespace.
+                        HYPHEN (3):
+                            A hyphen that indicates that a token has been
+                            split across lines.
+                    """
                     TYPE_UNSPECIFIED = 0
                     SPACE = 1
                     WIDE_SPACE = 2
                     HYPHEN = 3
 
                 type_: "Document.Page.Token.DetectedBreak.Type" = proto.Field(
                     proto.ENUM,
@@ -1344,15 +1374,48 @@
                     a layout element on the page.
                 confidence (float):
                     Optional. Confidence of detected page element, if
                     applicable. Range ``[0, 1]``.
             """
 
             class LayoutType(proto.Enum):
-                r"""The type of layout that is being referenced."""
+                r"""The type of layout that is being referenced.
+
+                Values:
+                    LAYOUT_TYPE_UNSPECIFIED (0):
+                        Layout Unspecified.
+                    BLOCK (1):
+                        References a
+                        [Page.blocks][google.cloud.documentai.v1beta3.Document.Page.blocks]
+                        element.
+                    PARAGRAPH (2):
+                        References a
+                        [Page.paragraphs][google.cloud.documentai.v1beta3.Document.Page.paragraphs]
+                        element.
+                    LINE (3):
+                        References a
+                        [Page.lines][google.cloud.documentai.v1beta3.Document.Page.lines]
+                        element.
+                    TOKEN (4):
+                        References a
+                        [Page.tokens][google.cloud.documentai.v1beta3.Document.Page.tokens]
+                        element.
+                    VISUAL_ELEMENT (5):
+                        References a
+                        [Page.visual_elements][google.cloud.documentai.v1beta3.Document.Page.visual_elements]
+                        element.
+                    TABLE (6):
+                        Refrrences a
+                        [Page.tables][google.cloud.documentai.v1beta3.Document.Page.tables]
+                        element.
+                    FORM_FIELD (7):
+                        References a
+                        [Page.form_fields][google.cloud.documentai.v1beta3.Document.Page.form_fields]
+                        element.
+                """
                 LAYOUT_TYPE_UNSPECIFIED = 0
                 BLOCK = 1
                 PARAGRAPH = 2
                 LINE = 3
                 TOKEN = 4
                 VISUAL_ELEMENT = 5
                 TABLE = 6
@@ -1404,14 +1467,34 @@
             type_ (google.cloud.documentai_v1beta3.types.Document.Provenance.OperationType):
                 The type of provenance operation.
         """
 
         class OperationType(proto.Enum):
             r"""If a processor or agent does an explicit operation on
             existing elements.
+
+            Values:
+                OPERATION_TYPE_UNSPECIFIED (0):
+                    Operation type unspecified. If no operation is specified a
+                    provenance entry is simply used to match against a
+                    ``parent``.
+                ADD (1):
+                    Add an element.
+                REMOVE (2):
+                    Remove an element identified by ``parent``.
+                REPLACE (3):
+                    Replace an element identified by ``parent``.
+                EVAL_REQUESTED (4):
+                    Request human review for the element identified by
+                    ``parent``.
+                EVAL_APPROVED (5):
+                    Element is reviewed and approved at human
+                    review, confidence will be set to 1.0.
+                EVAL_SKIPPED (6):
+                    Element is skipped in the validation process.
             """
             OPERATION_TYPE_UNSPECIFIED = 0
             ADD = 1
             REMOVE = 2
             REPLACE = 3
             EVAL_REQUESTED = 4
             EVAL_APPROVED = 5
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/document_io.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/document_io.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/document_processor_service.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/document_processor_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,35 @@
             document. This field is populated only when the [state] is
             [HUMAN_REVIEW_IN_PROGRESS]. It has the same response type
             and metadata as the long running operation returned by
             [ReviewDocument] method.
     """
 
     class State(proto.Enum):
-        r"""The final state of human review on a processed document."""
+        r"""The final state of human review on a processed document.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                Human review state is unspecified. Most
+                likely due to an internal error.
+            SKIPPED (1):
+                Human review is skipped for the document.
+                This can happen because human review is not
+                enabled on the processor or the processing
+                request has been set to skip this document.
+            VALIDATION_PASSED (2):
+                Human review validation is triggered and
+                passed, so no review is needed.
+            IN_PROGRESS (3):
+                Human review validation is triggered and the
+                document is under review.
+            ERROR (4):
+                Some error happened during triggering human review, see the
+                [state_message] for details.
+        """
         STATE_UNSPECIFIED = 0
         SKIPPED = 1
         VALIDATION_PASSED = 2
         IN_PROGRESS = 3
         ERROR = 4
 
     state: State = proto.Field(
@@ -380,15 +400,33 @@
             The last update time of the operation.
         individual_process_statuses (MutableSequence[google.cloud.documentai_v1beta3.types.BatchProcessMetadata.IndividualProcessStatus]):
             The list of response details of each
             document.
     """
 
     class State(proto.Enum):
-        r"""Possible states of the batch processing operation."""
+        r"""Possible states of the batch processing operation.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The default value. This value is used if the
+                state is omitted.
+            WAITING (1):
+                Request operation is waiting for scheduling.
+            RUNNING (2):
+                Request is being processed.
+            SUCCEEDED (3):
+                The batch processing completed successfully.
+            CANCELLING (4):
+                The batch processing was being cancelled.
+            CANCELLED (5):
+                The batch processing was cancelled.
+            FAILED (6):
+                The batch processing has failed.
+        """
         STATE_UNSPECIFIED = 0
         WAITING = 1
         RUNNING = 2
         SUCCEEDED = 3
         CANCELLING = 4
         CANCELLED = 5
         FAILED = 6
@@ -1196,15 +1234,25 @@
         priority (google.cloud.documentai_v1beta3.types.ReviewDocumentRequest.Priority):
             The priority of the human review task.
         document_schema (google.cloud.documentai_v1beta3.types.DocumentSchema):
             The document schema of the human review task.
     """
 
     class Priority(proto.Enum):
-        r"""The priority level of the human review task."""
+        r"""The priority level of the human review task.
+
+        Values:
+            DEFAULT (0):
+                The default priority level.
+            URGENT (1):
+                The urgent priority level. The labeling
+                manager should allocate labeler resource to the
+                urgent task queue to respect this priority
+                level.
+        """
         DEFAULT = 0
         URGENT = 1
 
     inline_document: gcd_document.Document = proto.Field(
         proto.MESSAGE,
         number=4,
         oneof="source",
@@ -1246,15 +1294,26 @@
             The state of the review operation.
         rejection_reason (str):
             The reason why the review is rejected by
             reviewer.
     """
 
     class State(proto.Enum):
-        r"""Possible states of the review operation."""
+        r"""Possible states of the review operation.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The default value. This value is used if the
+                state is omitted.
+            REJECTED (1):
+                The review operation is rejected by the
+                reviewer.
+            SUCCEEDED (2):
+                The review operation is succeeded.
+        """
         STATE_UNSPECIFIED = 0
         REJECTED = 1
         SUCCEEDED = 2
 
     gcs_destination: str = proto.Field(
         proto.STRING,
         number=1,
@@ -1289,15 +1348,30 @@
             The basic metadata of the long running
             operation.
         question_id (str):
             The Crowd Compute question ID.
     """
 
     class State(proto.Enum):
-        r"""State of the longrunning operation."""
+        r"""State of the longrunning operation.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                Unspecified state.
+            RUNNING (1):
+                Operation is still running.
+            CANCELLING (2):
+                Operation is being cancelled.
+            SUCCEEDED (3):
+                Operation succeeded.
+            FAILED (4):
+                Operation failed.
+            CANCELLED (5):
+                Operation is cancelled.
+        """
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         CANCELLING = 2
         SUCCEEDED = 3
         FAILED = 4
         CANCELLED = 5
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/document_schema.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/document_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,14 +115,30 @@
                     document.
             """
 
             class OccurrenceType(proto.Enum):
                 r"""Types of occurrences of the entity type in the document.
                 Note: this represents the number of instances of an entity
                 types, not number of mentions of a given entity instance.
+
+                Values:
+                    OCCURRENCE_TYPE_UNSPECIFIED (0):
+                        Unspecified occurrence type.
+                    OPTIONAL_ONCE (1):
+                        There will be zero or one instance of this
+                        entity type.
+                    OPTIONAL_MULTIPLE (2):
+                        The entity type will appear zero or multiple
+                        times.
+                    REQUIRED_ONCE (3):
+                        The entity type will only appear exactly
+                        once.
+                    REQUIRED_MULTIPLE (4):
+                        The entity type will appear once or more
+                        times.
                 """
                 OCCURRENCE_TYPE_UNSPECIFIED = 0
                 OPTIONAL_ONCE = 1
                 OPTIONAL_MULTIPLE = 2
                 REQUIRED_ONCE = 3
                 REQUIRED_MULTIPLE = 4
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/evaluation.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/evaluation.py`

 * *Files 5% similar despite different names*

```diff
@@ -208,15 +208,31 @@
                 The ECE for the predicted entities with fuzzy
                 matching disabled, i.e., exact matching only.
             metrics_type (google.cloud.documentai_v1beta3.types.Evaluation.MultiConfidenceMetrics.MetricsType):
                 The metrics type for the label.
         """
 
         class MetricsType(proto.Enum):
-            r"""A type that determines how metrics should be interpreted."""
+            r"""A type that determines how metrics should be interpreted.
+
+            Values:
+                METRICS_TYPE_UNSPECIFIED (0):
+                    The metrics type is unspecified. By default,
+                    metrics without a particular specification are
+                    for leaf entity types (i.e., top-level entity
+                    types without child types, or child types which
+                    are not parent types themselves).
+                AGGREGATE (1):
+                    Indicates whether metrics for this particular
+                    label type represent an aggregate of metrics for
+                    other types instead of being based on actual
+                    TP/FP/FN values for the label type. Metrics for
+                    parent (i.e., non-leaf) entity types are an
+                    aggregate of metrics for their children.
+            """
             METRICS_TYPE_UNSPECIFIED = 0
             AGGREGATE = 1
 
         confidence_level_metrics: MutableSequence[
             "Evaluation.ConfidenceLevelMetrics"
         ] = proto.RepeatedField(
             proto.MESSAGE,
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/geometry.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/operation_metadata.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/operation_metadata.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,15 +40,30 @@
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             The creation time of the operation.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             The last update time of the operation.
     """
 
     class State(proto.Enum):
-        r"""State of the longrunning operation."""
+        r"""State of the longrunning operation.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                Unspecified state.
+            RUNNING (1):
+                Operation is still running.
+            CANCELLING (2):
+                Operation is being cancelled.
+            SUCCEEDED (3):
+                Operation succeeded.
+            FAILED (4):
+                Operation failed.
+            CANCELLED (5):
+                Operation is cancelled.
+        """
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         CANCELLING = 2
         SUCCEEDED = 3
         FAILED = 4
         CANCELLED = 5
```

### Comparing `google-cloud-documentai-2.9.0/google/cloud/documentai_v1beta3/types/processor_type.py` & `google-cloud-documentai-2.9.1/google/cloud/documentai_v1beta3/types/processor_type.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/google_cloud_documentai.egg-info/PKG-INFO` & `google-cloud-documentai-2.9.1/google_cloud_documentai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-documentai
-Version: 2.9.0
+Version: 2.9.1
 Summary: Google Cloud Documentai API client library
 Home-page: https://github.com/googleapis/python-documentai
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-documentai-2.9.0/google_cloud_documentai.egg-info/SOURCES.txt` & `google-cloud-documentai-2.9.1/google_cloud_documentai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/setup.py` & `google-cloud-documentai-2.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/tests/__init__.py` & `google-cloud-documentai-2.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/tests/unit/__init__.py` & `google-cloud-documentai-2.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/tests/unit/gapic/__init__.py` & `google-cloud-documentai-2.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/tests/unit/gapic/documentai_v1/__init__.py` & `google-cloud-documentai-2.9.1/tests/unit/gapic/documentai_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/tests/unit/gapic/documentai_v1/test_document_processor_service.py` & `google-cloud-documentai-2.9.1/tests/unit/gapic/documentai_v1/test_document_processor_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/tests/unit/gapic/documentai_v1beta2/__init__.py` & `google-cloud-documentai-2.9.1/tests/unit/gapic/documentai_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/tests/unit/gapic/documentai_v1beta2/test_document_understanding_service.py` & `google-cloud-documentai-2.9.1/tests/unit/gapic/documentai_v1beta2/test_document_understanding_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/tests/unit/gapic/documentai_v1beta3/__init__.py` & `google-cloud-documentai-2.9.1/tests/unit/gapic/documentai_v1beta3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-documentai-2.9.0/tests/unit/gapic/documentai_v1beta3/test_document_processor_service.py` & `google-cloud-documentai-2.9.1/tests/unit/gapic/documentai_v1beta3/test_document_processor_service.py`

 * *Files identical despite different names*

