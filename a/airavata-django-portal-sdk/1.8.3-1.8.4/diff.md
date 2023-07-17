# Comparing `tmp/airavata-django-portal-sdk-1.8.3.tar.gz` & `tmp/airavata-django-portal-sdk-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airavata-django-portal-sdk-1.8.3.tar", last modified: Fri Apr 28 20:30:52 2023, max compression
+gzip compressed data, was "airavata-django-portal-sdk-1.8.4.tar", last modified: Mon Jul 17 15:17:52 2023, max compression
```

## Comparing `airavata-django-portal-sdk-1.8.3.tar` & `airavata-django-portal-sdk-1.8.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:52.638175 airavata-django-portal-sdk-1.8.3/
--rw-r--r--   0 machrist (661619347) 1014028542    11356 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/LICENSE
--rw-r--r--   0 machrist (661619347) 1014028542     3307 2023-04-28 20:30:52.638276 airavata-django-portal-sdk-1.8.3/PKG-INFO
--rw-r--r--   0 machrist (661619347) 1014028542     2463 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/README.md
-drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:52.631788 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/
--rw-r--r--   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/__init__.py
--rw-r--r--   0 machrist (661619347) 1014028542      124 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/apps.py
--rw-r--r--   0 machrist (661619347) 1014028542       74 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/decorators.py
-drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:52.633382 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/experiment_util/
--rw-r--r--   0 machrist (661619347) 1014028542      119 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/experiment_util/__init__.py
--rw-r--r--   0 machrist (661619347) 1014028542     8661 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/experiment_util/api.py
--rw-r--r--   0 machrist (661619347) 1014028542     4798 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/experiment_util/intermediate_output.py
-drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:52.634260 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/migrations/
--rw-r--r--   0 machrist (661619347) 1014028542      687 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/migrations/0001_initial.py
--rw-r--r--   0 machrist (661619347) 1014028542     1020 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/migrations/0002_userfiles_file_resource_id.py
--rw-r--r--   0 machrist (661619347) 1014028542     1914 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/migrations/0003_auto_20220225_1510.py
--rw-r--r--   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/migrations/__init__.py
--rw-r--r--   0 machrist (661619347) 1014028542      731 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/models.py
--rw-r--r--   0 machrist (661619347) 1014028542     1783 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/queue_settings_calculators.py
--rw-r--r--   0 machrist (661619347) 1014028542     1480 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/remoteapi.py
--rw-r--r--   0 machrist (661619347) 1014028542      993 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/serializers.py
-drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:52.635383 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/
--rw-r--r--   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/__init__.py
--rw-r--r--   0 machrist (661619347) 1014028542     3848 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/test_queue_settings_calculator.py
--rw-r--r--   0 machrist (661619347) 1014028542      439 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/test_settings.py
--rw-r--r--   0 machrist (661619347) 1014028542    15900 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/test_user_storage.py
--rw-r--r--   0 machrist (661619347) 1014028542      345 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/test_util.py
--rw-r--r--   0 machrist (661619347) 1014028542     5512 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/test_views.py
--rw-r--r--   0 machrist (661619347) 1014028542     1027 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/urls.py
-drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:52.635918 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/
--rw-r--r--   0 machrist (661619347) 1014028542     1126 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/__init__.py
--rw-r--r--   0 machrist (661619347) 1014028542    42739 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/api.py
-drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:52.637965 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/
--rw-r--r--   0 machrist (661619347) 1014028542    15554 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/CredCommon_pb2.py
--rw-r--r--   0 machrist (661619347) 1014028542      159 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/CredCommon_pb2_grpc.py
--rw-r--r--   0 machrist (661619347) 1014028542    61784 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/MFTApi_pb2.py
--rw-r--r--   0 machrist (661619347) 1014028542    14361 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/MFTApi_pb2_grpc.py
--rw-r--r--   0 machrist (661619347) 1014028542      330 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/__init__.py
--rw-r--r--   0 machrist (661619347) 1014028542     2779 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/base.py
--rw-r--r--   0 machrist (661619347) 1014028542    13793 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/django_filesystem_provider.py
--rw-r--r--   0 machrist (661619347) 1014028542    12378 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/mft_provider.py
--rw-r--r--   0 machrist (661619347) 1014028542      343 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/util.py
--rw-r--r--   0 machrist (661619347) 1014028542     8926 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/views.py
-drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:52.632870 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk.egg-info/
--rw-r--r--   0 machrist (661619347) 1014028542     3307 2023-04-28 20:30:52.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk.egg-info/PKG-INFO
--rw-r--r--   0 machrist (661619347) 1014028542     2035 2023-04-28 20:30:52.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 machrist (661619347) 1014028542        1 2023-04-28 20:30:52.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 machrist (661619347) 1014028542       77 2023-04-28 20:30:52.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk.egg-info/requires.txt
--rw-r--r--   0 machrist (661619347) 1014028542       27 2023-04-28 20:30:52.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk.egg-info/top_level.txt
--rw-r--r--   0 machrist (661619347) 1014028542      222 2023-04-28 20:30:52.638581 airavata-django-portal-sdk-1.8.3/setup.cfg
--rw-r--r--   0 machrist (661619347) 1014028542     1356 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/setup.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-07-17 15:17:52.133234 airavata-django-portal-sdk-1.8.4/
+-rw-r--r--   0 machrist (661619347) 1014028542    11356 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/LICENSE
+-rw-r--r--   0 machrist (661619347) 1014028542     3307 2023-07-17 15:17:52.133308 airavata-django-portal-sdk-1.8.4/PKG-INFO
+-rw-r--r--   0 machrist (661619347) 1014028542     2463 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/README.md
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-07-17 15:17:52.127845 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/
+-rw-r--r--   0 machrist (661619347) 1014028542        0 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/__init__.py
+-rw-r--r--   0 machrist (661619347) 1014028542      124 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/apps.py
+-rw-r--r--   0 machrist (661619347) 1014028542       74 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/decorators.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-07-17 15:17:52.129068 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/experiment_util/
+-rw-r--r--   0 machrist (661619347) 1014028542      119 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/experiment_util/__init__.py
+-rw-r--r--   0 machrist (661619347) 1014028542     8661 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/experiment_util/api.py
+-rw-r--r--   0 machrist (661619347) 1014028542     4798 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/experiment_util/intermediate_output.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-07-17 15:17:52.129806 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/migrations/
+-rw-r--r--   0 machrist (661619347) 1014028542      687 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/migrations/0001_initial.py
+-rw-r--r--   0 machrist (661619347) 1014028542     1020 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/migrations/0002_userfiles_file_resource_id.py
+-rw-r--r--   0 machrist (661619347) 1014028542     1914 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/migrations/0003_auto_20220225_1510.py
+-rw-r--r--   0 machrist (661619347) 1014028542        0 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/migrations/__init__.py
+-rw-r--r--   0 machrist (661619347) 1014028542      731 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/models.py
+-rw-r--r--   0 machrist (661619347) 1014028542     1783 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/queue_settings_calculators.py
+-rw-r--r--   0 machrist (661619347) 1014028542     1480 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/remoteapi.py
+-rw-r--r--   0 machrist (661619347) 1014028542      993 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/serializers.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-07-17 15:17:52.130725 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/tests/
+-rw-r--r--   0 machrist (661619347) 1014028542        0 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/tests/__init__.py
+-rw-r--r--   0 machrist (661619347) 1014028542     3848 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/tests/test_queue_settings_calculator.py
+-rw-r--r--   0 machrist (661619347) 1014028542      439 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/tests/test_settings.py
+-rw-r--r--   0 machrist (661619347) 1014028542    17668 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/tests/test_user_storage.py
+-rw-r--r--   0 machrist (661619347) 1014028542      345 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/tests/test_util.py
+-rw-r--r--   0 machrist (661619347) 1014028542     5512 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/tests/test_views.py
+-rw-r--r--   0 machrist (661619347) 1014028542     1027 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/urls.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-07-17 15:17:52.131092 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/
+-rw-r--r--   0 machrist (661619347) 1014028542     1126 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/__init__.py
+-rw-r--r--   0 machrist (661619347) 1014028542    42744 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/api.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-07-17 15:17:52.133039 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/backends/
+-rw-r--r--   0 machrist (661619347) 1014028542    15554 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/backends/CredCommon_pb2.py
+-rw-r--r--   0 machrist (661619347) 1014028542      159 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/backends/CredCommon_pb2_grpc.py
+-rw-r--r--   0 machrist (661619347) 1014028542    61784 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/backends/MFTApi_pb2.py
+-rw-r--r--   0 machrist (661619347) 1014028542    14361 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/backends/MFTApi_pb2_grpc.py
+-rw-r--r--   0 machrist (661619347) 1014028542      330 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/backends/__init__.py
+-rw-r--r--   0 machrist (661619347) 1014028542     2779 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/backends/base.py
+-rw-r--r--   0 machrist (661619347) 1014028542    13793 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/backends/django_filesystem_provider.py
+-rw-r--r--   0 machrist (661619347) 1014028542    12378 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/backends/mft_provider.py
+-rw-r--r--   0 machrist (661619347) 1014028542      343 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/util.py
+-rw-r--r--   0 machrist (661619347) 1014028542     8926 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/views.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-07-17 15:17:52.128559 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk.egg-info/
+-rw-r--r--   0 machrist (661619347) 1014028542     3307 2023-07-17 15:17:52.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 machrist (661619347) 1014028542     2035 2023-07-17 15:17:52.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 machrist (661619347) 1014028542        1 2023-07-17 15:17:52.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 machrist (661619347) 1014028542       77 2023-07-17 15:17:52.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk.egg-info/requires.txt
+-rw-r--r--   0 machrist (661619347) 1014028542       27 2023-07-17 15:17:52.000000 airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk.egg-info/top_level.txt
+-rw-r--r--   0 machrist (661619347) 1014028542      222 2023-07-17 15:17:52.133595 airavata-django-portal-sdk-1.8.4/setup.cfg
+-rw-r--r--   0 machrist (661619347) 1014028542     1356 2023-07-17 15:17:04.000000 airavata-django-portal-sdk-1.8.4/setup.py
```

### Comparing `airavata-django-portal-sdk-1.8.3/LICENSE` & `airavata-django-portal-sdk-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/PKG-INFO` & `airavata-django-portal-sdk-1.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airavata-django-portal-sdk
-Version: 1.8.3
+Version: 1.8.4
 Summary: The Airavata Django Portal SDK is a library that makes it easier to develop Airavata Django Portal customizations.
 Home-page: https://github.com/apache/airavata-django-portal-sdk
 Author: Apache Software Foundation
 Author-email: dev@airavata.apache.org
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `airavata-django-portal-sdk-1.8.3/README.md` & `airavata-django-portal-sdk-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/experiment_util/api.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/experiment_util/api.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/experiment_util/intermediate_output.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/experiment_util/intermediate_output.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/migrations/0001_initial.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/migrations/0002_userfiles_file_resource_id.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/migrations/0002_userfiles_file_resource_id.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/migrations/0003_auto_20220225_1510.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/migrations/0003_auto_20220225_1510.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/models.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/models.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/queue_settings_calculators.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/queue_settings_calculators.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/remoteapi.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/remoteapi.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/serializers.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/serializers.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/test_queue_settings_calculator.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/tests/test_queue_settings_calculator.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/test_user_storage.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/tests/test_user_storage.py`

 * *Files 9% similar despite different names*

```diff
@@ -325,7 +325,40 @@
             # and the data product is for new_storage_resource_id
             self.assertEqual(default_storage_resource_id, settings.USER_STORAGES['default']['STORAGE_RESOURCE_ID'])
             self.assertEqual(non_default_storage_resource_id, data_product.replicaLocations[0].storageResourceId)
             self.assertNotEqual(default_storage_resource_id, non_default_storage_resource_id)
 
             exists = user_storage.exists(self.request, data_product)
             self.assertTrue(exists)
+
+
+class SaveInputFileTests(BaseTestCase):
+    def test_save_input_file_duplicated_name(self):
+        "Test saving two input files with the same name"
+        with tempfile.TemporaryDirectory() as tmpdirname, \
+                self.settings(GATEWAY_DATA_STORE_DIR=tmpdirname,
+                              GATEWAY_DATA_STORE_HOSTNAME="gateway.com"):
+            file = io.StringIO("Foo file")
+            file.name = "foo.txt"
+            user_storage.save_input_file(self.request, file)
+            file.seek(0)
+            # Save it again
+            user_storage.save_input_file(self.request, file)
+
+            self.assertEqual(2, self.request.airavata_client.registerDataProduct.call_count)
+
+            args1, _ = self.request.airavata_client.registerDataProduct.call_args_list[0]
+            dp1 = args1[1]
+            args2, _ = self.request.airavata_client.registerDataProduct.call_args_list[1]
+            dp2 = args2[1]
+
+            # Both files should have the same productName, even though the second
+            # was renamed on the filesystem to avoid collision
+            self.assertEqual("foo.txt", dp1.productName)
+            self.assertEqual("foo.txt", dp2.productName)
+            self.assertEqual(1, len(dp1.replicaLocations))
+            self.assertEqual(1, len(dp2.replicaLocations))
+            # First file should be saved to the fs with the original name
+            self.assertEqual("foo.txt", os.path.basename(dp1.replicaLocations[0].filePath))
+            self.assertNotEqual(dp1.replicaLocations[0].filePath, dp2.replicaLocations[0].filePath)
+            # Check that the saved location was renamed to not conflict with the first upload
+            self.assertTrue(os.path.basename(dp2.replicaLocations[0].filePath).startswith("foo_"))
```

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/test_views.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/urls.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/urls.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/__init__.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/api.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         return data_product
     else:
         backend = get_user_storage_provider(request, storage_resource_id=storage_resource_id)
         file_name = name if name is not None else os.path.basename(file.name)
         storage_resource_id, resource_path = backend.save(
             TMP_INPUT_FILE_UPLOAD_DIR, file, name=file_name)
         data_product = _save_data_product(
-            request, resource_path, storage_resource_id, name=name, content_type=content_type, backend=backend
+            request, resource_path, storage_resource_id, name=file_name, content_type=content_type, backend=backend
         )
         return data_product
 
 
 def _copy_input_file(request, data_product=None, data_product_uri=None, storage_resource_id=None):
     if data_product is None:
         data_product = _get_data_product(request, data_product_uri)
```

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/CredCommon_pb2.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/backends/CredCommon_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/MFTApi_pb2.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/backends/MFTApi_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/MFTApi_pb2_grpc.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/backends/MFTApi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/base.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/backends/base.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/django_filesystem_provider.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/backends/django_filesystem_provider.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/mft_provider.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/user_storage/backends/mft_provider.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/views.py` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk/views.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk.egg-info/PKG-INFO` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airavata-django-portal-sdk
-Version: 1.8.3
+Version: 1.8.4
 Summary: The Airavata Django Portal SDK is a library that makes it easier to develop Airavata Django Portal customizations.
 Home-page: https://github.com/apache/airavata-django-portal-sdk
 Author: Apache Software Foundation
 Author-email: dev@airavata.apache.org
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk.egg-info/SOURCES.txt` & `airavata-django-portal-sdk-1.8.4/airavata_django_portal_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.3/setup.py` & `airavata-django-portal-sdk-1.8.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 setup(
     name="airavata-django-portal-sdk",
-    version="1.8.3",
+    version="1.8.4",
     url="https://github.com/apache/airavata-django-portal-sdk",
     author="Apache Software Foundation",
     author_email="dev@airavata.apache.org",
     description=(
         "The Airavata Django Portal SDK is a library that makes "
         "it easier to develop Airavata Django Portal customizations."
     ),
```

