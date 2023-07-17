# Comparing `tmp/fabric-orchestrator-client-1.5.1.tar.gz` & `tmp/fabric-orchestrator-client-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-orchestrator-client-1.5.1.tar", last modified: Sat Jun 17 10:06:11 2023, max compression
+gzip compressed data, was "fabric-orchestrator-client-1.5.2.tar", last modified: Mon Jul 17 20:55:45 2023, max compression
```

## Comparing `fabric-orchestrator-client-1.5.1.tar` & `fabric-orchestrator-client-1.5.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0      793 2023-05-11 17:37:01.210207 fabric-orchestrator-client-1.5.1/.gitignore
--rw-r--r--   0        0        0     1030 2023-05-11 17:37:01.210355 fabric-orchestrator-client-1.5.1/.swagger-codegen-ignore
--rw-r--r--   0        0        0        7 2023-06-10 11:27:02.431890 fabric-orchestrator-client-1.5.1/.swagger-codegen/VERSION
--rw-r--r--   0        0        0      349 2023-05-11 17:37:01.210626 fabric-orchestrator-client-1.5.1/.travis.yml
--rw-r--r--   0        0        0      770 2023-05-11 17:37:01.210729 fabric-orchestrator-client-1.5.1/CODEGEN.md
--rw-r--r--   0        0        0     1071 2023-05-11 17:37:01.210862 fabric-orchestrator-client-1.5.1/LICENSE
--rw-r--r--   0        0        0       59 2023-05-11 17:37:01.210963 fabric-orchestrator-client-1.5.1/MANIFEST.in
--rw-r--r--   0        0        0     9867 2023-06-12 16:30:43.340015 fabric-orchestrator-client-1.5.1/README.md
--rw-r--r--   0        0        0      340 2023-06-10 11:27:02.433089 fabric-orchestrator-client-1.5.1/docs/Poa.md
--rw-r--r--   0        0        0      557 2023-06-12 16:30:43.340871 fabric-orchestrator-client-1.5.1/docs/PoaData.md
--rw-r--r--   0        0        0      376 2023-06-10 11:27:02.434037 fabric-orchestrator-client-1.5.1/docs/PoaPost.md
--rw-r--r--   0        0        0      430 2023-06-10 11:27:02.434323 fabric-orchestrator-client-1.5.1/docs/PoaPostData.md
--rw-r--r--   0        0        0      369 2023-06-10 11:27:02.434841 fabric-orchestrator-client-1.5.1/docs/PoaPostDataVcpuCpuMap.md
--rw-r--r--   0        0        0     6404 2023-06-12 16:30:43.341529 fabric-orchestrator-client-1.5.1/docs/PoasApi.md
--rw-r--r--   0        0        0     4263 2023-05-11 17:37:01.211350 fabric-orchestrator-client-1.5.1/docs/ResourcesApi.md
--rw-r--r--   0        0        0    20667 2023-06-12 16:30:43.341882 fabric-orchestrator-client-1.5.1/docs/SlicesApi.md
--rw-r--r--   0        0        0     4102 2023-06-12 16:30:43.342523 fabric-orchestrator-client-1.5.1/docs/SliversApi.md
--rw-r--r--   0        0        0      335 2023-05-11 17:37:01.211789 fabric-orchestrator-client-1.5.1/docs/Success.md
--rw-r--r--   0        0        0      352 2023-05-11 17:37:01.211912 fabric-orchestrator-client-1.5.1/docs/Version.md
--rw-r--r--   0        0        0       22 2023-06-17 09:55:40.714963 fabric-orchestrator-client-1.5.1/fabric_cf/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 17:37:01.212158 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/__init__.py
--rw-r--r--   0        0        0    21840 2023-06-12 16:30:43.343170 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/orchestrator_proxy.py
--rw-r--r--   0        0        0     3557 2023-06-12 16:30:43.344093 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/__init__.py
--rw-r--r--   0        0        0      468 2023-06-12 16:30:43.344852 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/__init__.py
--rw-r--r--   0        0        0    13515 2023-06-12 16:30:43.345710 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/poas_api.py
--rw-r--r--   0        0        0     9597 2023-05-11 17:37:01.213024 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/resources_api.py
--rw-r--r--   0        0        0    44360 2023-06-12 17:06:53.843598 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/slices_api.py
--rw-r--r--   0        0        0     9260 2023-06-12 16:30:43.347087 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
--rw-r--r--   0        0        0     3748 2023-05-11 17:37:01.213724 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/version_api.py
--rw-r--r--   0        0        0    25128 2023-05-11 17:37:01.213944 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api_client.py
--rw-r--r--   0        0        0     8240 2023-05-11 17:37:01.214372 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/configuration.py
--rw-r--r--   0        0        0     2978 2023-06-10 11:27:02.438784 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/__init__.py
--rw-r--r--   0        0        0     3427 2023-06-10 11:27:02.439359 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/poa.py
--rw-r--r--   0        0        0     6654 2023-06-12 16:30:43.348013 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/poa_data.py
--rw-r--r--   0        0        0     4034 2023-06-10 11:27:02.440677 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/poa_post.py
--rw-r--r--   0        0        0     3878 2023-06-10 11:27:02.441305 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py
--rw-r--r--   0        0        0     3648 2023-06-10 11:27:02.441612 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py
--rw-r--r--   0        0        0     3055 2023-05-11 17:37:01.214908 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/resource.py
--rw-r--r--   0        0        0     3420 2023-05-11 17:37:01.215233 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/resources.py
--rw-r--r--   0        0        0     8496 2023-05-11 17:37:01.215453 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slice.py
--rw-r--r--   0        0        0     3444 2023-06-12 16:30:43.348954 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slice_details.py
--rw-r--r--   0        0        0     3412 2023-05-11 17:37:01.215680 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slices.py
--rw-r--r--   0        0        0     3951 2023-06-10 11:27:02.442381 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slices_post.py
--rw-r--r--   0        0        0    10905 2023-06-10 11:27:02.443007 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/sliver.py
--rw-r--r--   0        0        0     3422 2023-05-11 17:37:01.216181 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slivers.py
--rw-r--r--   0        0        0     4999 2023-05-11 17:37:01.216373 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
--rw-r--r--   0        0        0     3832 2023-05-11 17:37:01.216668 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
--rw-r--r--   0        0        0     6211 2023-05-11 17:37:01.216937 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
--rw-r--r--   0        0        0     4253 2023-05-11 17:37:01.217164 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
--rw-r--r--   0        0        0     3163 2023-05-11 17:37:01.217341 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
--rw-r--r--   0        0        0     5771 2023-05-11 17:37:01.217534 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
--rw-r--r--   0        0        0     5063 2023-05-11 17:37:01.217713 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
--rw-r--r--   0        0        0     3870 2023-05-11 17:37:01.217919 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
--rw-r--r--   0        0        0     4994 2023-05-11 17:37:01.218148 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
--rw-r--r--   0        0        0     3831 2023-05-11 17:37:01.218431 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
--rw-r--r--   0        0        0     4971 2023-05-11 17:37:01.218623 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
--rw-r--r--   0        0        0     3819 2023-05-11 17:37:01.218944 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
--rw-r--r--   0        0        0     5224 2023-05-11 17:37:01.219262 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
--rw-r--r--   0        0        0     3963 2023-05-11 17:37:01.219487 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
--rw-r--r--   0        0        0     3413 2023-05-11 17:37:01.219669 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/version.py
--rw-r--r--   0        0        0     3882 2023-05-11 17:37:01.219920 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/version_data.py
--rw-r--r--   0        0        0    12988 2023-05-11 17:37:01.220174 fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/rest.py
--rw-r--r--   0        0        0     1663 2023-05-11 17:37:01.220383 fabric-orchestrator-client-1.5.1/git_push.sh
--rw-r--r--   0        0        0     1024 2023-06-17 09:55:40.699613 fabric-orchestrator-client-1.5.1/pyproject.toml
--rw-r--r--   0        0        0       16 2023-06-10 11:27:02.444133 fabric-orchestrator-client-1.5.1/test/__init__.py
--rw-r--r--   0        0        0      809 2023-06-10 11:27:02.444942 fabric-orchestrator-client-1.5.1/test/test_poa.py
--rw-r--r--   0        0        0      843 2023-06-10 11:27:02.445598 fabric-orchestrator-client-1.5.1/test/test_poa_data.py
--rw-r--r--   0        0        0      843 2023-06-10 11:27:02.446320 fabric-orchestrator-client-1.5.1/test/test_poa_post.py
--rw-r--r--   0        0        0      877 2023-06-10 11:27:02.447271 fabric-orchestrator-client-1.5.1/test/test_poa_post_data.py
--rw-r--r--   0        0        0      963 2023-06-10 11:27:02.448091 fabric-orchestrator-client-1.5.1/test/test_poa_post_data_vcpu_cpu_map.py
--rw-r--r--   0        0        0     1157 2023-06-12 16:30:43.349539 fabric-orchestrator-client-1.5.1/test/test_poas_api.py
--rw-r--r--   0        0        0      896 2023-05-11 17:37:01.221224 fabric-orchestrator-client-1.5.1/test/test_resource.py
--rw-r--r--   0        0        0      950 2023-05-11 17:37:01.221397 fabric-orchestrator-client-1.5.1/test/test_resources.py
--rw-r--r--   0        0        0     1206 2023-05-11 17:37:01.221693 fabric-orchestrator-client-1.5.1/test/test_resources_api.py
--rw-r--r--   0        0        0      872 2023-05-11 17:37:01.221929 fabric-orchestrator-client-1.5.1/test/test_slice.py
--rw-r--r--   0        0        0      930 2023-05-11 17:37:01.222101 fabric-orchestrator-client-1.5.1/test/test_slice_details.py
--rw-r--r--   0        0        0      880 2023-05-11 17:37:01.222270 fabric-orchestrator-client-1.5.1/test/test_slices.py
--rw-r--r--   0        0        0     2165 2023-06-12 16:30:43.349919 fabric-orchestrator-client-1.5.1/test/test_slices_api.py
--rw-r--r--   0        0        0      867 2023-06-10 11:27:02.448859 fabric-orchestrator-client-1.5.1/test/test_slices_post.py
--rw-r--r--   0        0        0      880 2023-05-11 17:37:01.222608 fabric-orchestrator-client-1.5.1/test/test_sliver.py
--rw-r--r--   0        0        0      888 2023-05-11 17:37:01.222785 fabric-orchestrator-client-1.5.1/test/test_slivers.py
--rw-r--r--   0        0        0      974 2023-06-12 16:30:43.350780 fabric-orchestrator-client-1.5.1/test/test_slivers_api.py
--rw-r--r--   0        0        0      998 2023-05-11 17:37:01.223296 fabric-orchestrator-client-1.5.1/test/test_status200_ok_no_content.py
--rw-r--r--   0        0        0     1032 2023-05-11 17:37:01.223607 fabric-orchestrator-client-1.5.1/test/test_status200_ok_no_content_data.py
--rw-r--r--   0        0        0      996 2023-05-11 17:37:01.223847 fabric-orchestrator-client-1.5.1/test/test_status200_ok_paginated.py
--rw-r--r--   0        0        0      972 2023-05-11 17:37:01.224081 fabric-orchestrator-client-1.5.1/test/test_status200_ok_single.py
--rw-r--r--   0        0        0      988 2023-05-11 17:37:01.224292 fabric-orchestrator-client-1.5.1/test/test_status400_bad_request.py
--rw-r--r--   0        0        0     1038 2023-05-11 17:37:01.224535 fabric-orchestrator-client-1.5.1/test/test_status400_bad_request_errors.py
--rw-r--r--   0        0        0     1002 2023-05-11 17:37:01.224771 fabric-orchestrator-client-1.5.1/test/test_status401_unauthorized.py
--rw-r--r--   0        0        0     1052 2023-05-11 17:37:01.225030 fabric-orchestrator-client-1.5.1/test/test_status401_unauthorized_errors.py
--rw-r--r--   0        0        0      978 2023-05-11 17:37:01.225269 fabric-orchestrator-client-1.5.1/test/test_status403_forbidden.py
--rw-r--r--   0        0        0     1028 2023-05-11 17:37:01.225554 fabric-orchestrator-client-1.5.1/test/test_status403_forbidden_errors.py
--rw-r--r--   0        0        0      972 2023-05-11 17:37:01.225840 fabric-orchestrator-client-1.5.1/test/test_status404_not_found.py
--rw-r--r--   0        0        0     1022 2023-05-11 17:37:01.226137 fabric-orchestrator-client-1.5.1/test/test_status404_not_found_errors.py
--rw-r--r--   0        0        0     1062 2023-05-11 17:37:01.226327 fabric-orchestrator-client-1.5.1/test/test_status500_internal_server_error.py
--rw-r--r--   0        0        0     1112 2023-05-11 17:37:01.226547 fabric-orchestrator-client-1.5.1/test/test_status500_internal_server_error_errors.py
--rw-r--r--   0        0        0      888 2023-05-11 17:37:01.226964 fabric-orchestrator-client-1.5.1/test/test_version.py
--rw-r--r--   0        0        0      814 2023-05-11 17:37:01.227150 fabric-orchestrator-client-1.5.1/test/test_version_api.py
--rw-r--r--   0        0        0      922 2023-05-11 17:37:01.227332 fabric-orchestrator-client-1.5.1/test/test_version_data.py
--rw-r--r--   0        0        0      143 2023-05-11 17:37:01.227515 fabric-orchestrator-client-1.5.1/tox.ini
--rw-r--r--   0        0        0    10816 1970-01-01 00:00:00.000000 fabric-orchestrator-client-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0      793 2023-05-11 17:37:01.210207 fabric-orchestrator-client-1.5.2/.gitignore
+-rw-r--r--   0        0        0     1030 2023-05-11 17:37:01.210355 fabric-orchestrator-client-1.5.2/.swagger-codegen-ignore
+-rw-r--r--   0        0        0        7 2023-07-17 20:49:48.768205 fabric-orchestrator-client-1.5.2/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0      349 2023-05-11 17:37:01.210626 fabric-orchestrator-client-1.5.2/.travis.yml
+-rw-r--r--   0        0        0      770 2023-05-11 17:37:01.210729 fabric-orchestrator-client-1.5.2/CODEGEN.md
+-rw-r--r--   0        0        0     1071 2023-05-11 17:37:01.210862 fabric-orchestrator-client-1.5.2/LICENSE
+-rw-r--r--   0        0        0       59 2023-05-11 17:37:01.210963 fabric-orchestrator-client-1.5.2/MANIFEST.in
+-rw-r--r--   0        0        0     9867 2023-07-17 20:49:48.770096 fabric-orchestrator-client-1.5.2/README.md
+-rw-r--r--   0        0        0      340 2023-07-17 20:49:48.770872 fabric-orchestrator-client-1.5.2/docs/Poa.md
+-rw-r--r--   0        0        0      557 2023-07-17 20:49:48.771474 fabric-orchestrator-client-1.5.2/docs/PoaData.md
+-rw-r--r--   0        0        0      376 2023-07-17 20:49:48.772151 fabric-orchestrator-client-1.5.2/docs/PoaPost.md
+-rw-r--r--   0        0        0      430 2023-07-17 20:49:48.772876 fabric-orchestrator-client-1.5.2/docs/PoaPostData.md
+-rw-r--r--   0        0        0      369 2023-07-17 20:49:48.773303 fabric-orchestrator-client-1.5.2/docs/PoaPostDataVcpuCpuMap.md
+-rw-r--r--   0        0        0     6404 2023-07-17 20:49:48.774052 fabric-orchestrator-client-1.5.2/docs/PoasApi.md
+-rw-r--r--   0        0        0     4263 2023-05-11 17:37:01.211350 fabric-orchestrator-client-1.5.2/docs/ResourcesApi.md
+-rw-r--r--   0        0        0    20667 2023-07-17 20:49:48.775232 fabric-orchestrator-client-1.5.2/docs/SlicesApi.md
+-rw-r--r--   0        0        0     4102 2023-07-17 20:49:48.776060 fabric-orchestrator-client-1.5.2/docs/SliversApi.md
+-rw-r--r--   0        0        0      335 2023-05-11 17:37:01.211789 fabric-orchestrator-client-1.5.2/docs/Success.md
+-rw-r--r--   0        0        0      352 2023-05-11 17:37:01.211912 fabric-orchestrator-client-1.5.2/docs/Version.md
+-rw-r--r--   0        0        0       22 2023-07-17 20:55:28.031580 fabric-orchestrator-client-1.5.2/fabric_cf/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 17:37:01.212158 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/__init__.py
+-rw-r--r--   0        0        0    21840 2023-07-17 20:49:48.777773 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/orchestrator_proxy.py
+-rw-r--r--   0        0        0     3557 2023-07-17 20:49:48.778938 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/__init__.py
+-rw-r--r--   0        0        0      468 2023-07-17 20:49:48.779817 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/__init__.py
+-rw-r--r--   0        0        0    13515 2023-07-17 20:49:48.780918 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/poas_api.py
+-rw-r--r--   0        0        0     9597 2023-05-11 17:37:01.213024 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/resources_api.py
+-rw-r--r--   0        0        0    43978 2023-07-17 20:52:06.850318 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/slices_api.py
+-rw-r--r--   0        0        0     9260 2023-07-17 20:49:48.782141 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
+-rw-r--r--   0        0        0     3748 2023-05-11 17:37:01.213724 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/version_api.py
+-rw-r--r--   0        0        0    25272 2023-07-17 20:47:34.398882 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api_client.py
+-rw-r--r--   0        0        0     8240 2023-05-11 17:37:01.214372 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/configuration.py
+-rw-r--r--   0        0        0     2978 2023-07-17 20:49:48.782449 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/__init__.py
+-rw-r--r--   0        0        0     3427 2023-07-17 20:49:48.783245 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa.py
+-rw-r--r--   0        0        0     6654 2023-07-17 20:49:48.784161 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa_data.py
+-rw-r--r--   0        0        0     4034 2023-07-17 20:49:48.785395 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa_post.py
+-rw-r--r--   0        0        0     3878 2023-07-17 20:49:48.786219 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py
+-rw-r--r--   0        0        0     3648 2023-07-17 20:49:48.786798 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py
+-rw-r--r--   0        0        0     3055 2023-05-11 17:37:01.214908 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/resource.py
+-rw-r--r--   0        0        0     3420 2023-05-11 17:37:01.215233 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/resources.py
+-rw-r--r--   0        0        0     8496 2023-05-11 17:37:01.215453 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slice.py
+-rw-r--r--   0        0        0     3444 2023-07-17 20:49:48.787456 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slice_details.py
+-rw-r--r--   0        0        0     3412 2023-05-11 17:37:01.215680 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slices.py
+-rw-r--r--   0        0        0     3951 2023-07-17 20:49:48.788286 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slices_post.py
+-rw-r--r--   0        0        0    10905 2023-07-17 20:49:48.789193 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/sliver.py
+-rw-r--r--   0        0        0     3422 2023-05-11 17:37:01.216181 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slivers.py
+-rw-r--r--   0        0        0     4999 2023-05-11 17:37:01.216373 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     3832 2023-05-11 17:37:01.216668 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     6211 2023-05-11 17:37:01.216937 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
+-rw-r--r--   0        0        0     4253 2023-05-11 17:37:01.217164 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
+-rw-r--r--   0        0        0     3163 2023-05-11 17:37:01.217341 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
+-rw-r--r--   0        0        0     5771 2023-05-11 17:37:01.217534 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     5063 2023-05-11 17:37:01.217713 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     3870 2023-05-11 17:37:01.217919 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     4994 2023-05-11 17:37:01.218148 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
+-rw-r--r--   0        0        0     3831 2023-05-11 17:37:01.218431 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     4971 2023-05-11 17:37:01.218623 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
+-rw-r--r--   0        0        0     3819 2023-05-11 17:37:01.218944 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     5224 2023-05-11 17:37:01.219262 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     3963 2023-05-11 17:37:01.219487 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     3413 2023-05-11 17:37:01.219669 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/version.py
+-rw-r--r--   0        0        0     3882 2023-05-11 17:37:01.219920 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/version_data.py
+-rw-r--r--   0        0        0    12988 2023-05-11 17:37:01.220174 fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/rest.py
+-rw-r--r--   0        0        0     1663 2023-05-11 17:37:01.220383 fabric-orchestrator-client-1.5.2/git_push.sh
+-rw-r--r--   0        0        0     1024 2023-07-17 20:54:47.871007 fabric-orchestrator-client-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-07-17 20:49:48.791020 fabric-orchestrator-client-1.5.2/test/__init__.py
+-rw-r--r--   0        0        0      809 2023-07-17 20:49:48.791882 fabric-orchestrator-client-1.5.2/test/test_poa.py
+-rw-r--r--   0        0        0      843 2023-07-17 20:49:48.792642 fabric-orchestrator-client-1.5.2/test/test_poa_data.py
+-rw-r--r--   0        0        0      843 2023-07-17 20:49:48.793127 fabric-orchestrator-client-1.5.2/test/test_poa_post.py
+-rw-r--r--   0        0        0      877 2023-07-17 20:49:48.793692 fabric-orchestrator-client-1.5.2/test/test_poa_post_data.py
+-rw-r--r--   0        0        0      963 2023-07-17 20:49:48.794485 fabric-orchestrator-client-1.5.2/test/test_poa_post_data_vcpu_cpu_map.py
+-rw-r--r--   0        0        0     1157 2023-07-17 20:49:48.795260 fabric-orchestrator-client-1.5.2/test/test_poas_api.py
+-rw-r--r--   0        0        0      896 2023-05-11 17:37:01.221224 fabric-orchestrator-client-1.5.2/test/test_resource.py
+-rw-r--r--   0        0        0      950 2023-05-11 17:37:01.221397 fabric-orchestrator-client-1.5.2/test/test_resources.py
+-rw-r--r--   0        0        0     1206 2023-05-11 17:37:01.221693 fabric-orchestrator-client-1.5.2/test/test_resources_api.py
+-rw-r--r--   0        0        0      872 2023-05-11 17:37:01.221929 fabric-orchestrator-client-1.5.2/test/test_slice.py
+-rw-r--r--   0        0        0      930 2023-05-11 17:37:01.222101 fabric-orchestrator-client-1.5.2/test/test_slice_details.py
+-rw-r--r--   0        0        0      880 2023-05-11 17:37:01.222270 fabric-orchestrator-client-1.5.2/test/test_slices.py
+-rw-r--r--   0        0        0     2165 2023-07-17 20:49:48.796346 fabric-orchestrator-client-1.5.2/test/test_slices_api.py
+-rw-r--r--   0        0        0      867 2023-07-17 20:49:48.797642 fabric-orchestrator-client-1.5.2/test/test_slices_post.py
+-rw-r--r--   0        0        0      880 2023-05-11 17:37:01.222608 fabric-orchestrator-client-1.5.2/test/test_sliver.py
+-rw-r--r--   0        0        0      888 2023-05-11 17:37:01.222785 fabric-orchestrator-client-1.5.2/test/test_slivers.py
+-rw-r--r--   0        0        0      974 2023-07-17 20:49:48.798816 fabric-orchestrator-client-1.5.2/test/test_slivers_api.py
+-rw-r--r--   0        0        0      998 2023-05-11 17:37:01.223296 fabric-orchestrator-client-1.5.2/test/test_status200_ok_no_content.py
+-rw-r--r--   0        0        0     1032 2023-05-11 17:37:01.223607 fabric-orchestrator-client-1.5.2/test/test_status200_ok_no_content_data.py
+-rw-r--r--   0        0        0      996 2023-05-11 17:37:01.223847 fabric-orchestrator-client-1.5.2/test/test_status200_ok_paginated.py
+-rw-r--r--   0        0        0      972 2023-05-11 17:37:01.224081 fabric-orchestrator-client-1.5.2/test/test_status200_ok_single.py
+-rw-r--r--   0        0        0      988 2023-05-11 17:37:01.224292 fabric-orchestrator-client-1.5.2/test/test_status400_bad_request.py
+-rw-r--r--   0        0        0     1038 2023-05-11 17:37:01.224535 fabric-orchestrator-client-1.5.2/test/test_status400_bad_request_errors.py
+-rw-r--r--   0        0        0     1002 2023-05-11 17:37:01.224771 fabric-orchestrator-client-1.5.2/test/test_status401_unauthorized.py
+-rw-r--r--   0        0        0     1052 2023-05-11 17:37:01.225030 fabric-orchestrator-client-1.5.2/test/test_status401_unauthorized_errors.py
+-rw-r--r--   0        0        0      978 2023-05-11 17:37:01.225269 fabric-orchestrator-client-1.5.2/test/test_status403_forbidden.py
+-rw-r--r--   0        0        0     1028 2023-05-11 17:37:01.225554 fabric-orchestrator-client-1.5.2/test/test_status403_forbidden_errors.py
+-rw-r--r--   0        0        0      972 2023-05-11 17:37:01.225840 fabric-orchestrator-client-1.5.2/test/test_status404_not_found.py
+-rw-r--r--   0        0        0     1022 2023-05-11 17:37:01.226137 fabric-orchestrator-client-1.5.2/test/test_status404_not_found_errors.py
+-rw-r--r--   0        0        0     1062 2023-05-11 17:37:01.226327 fabric-orchestrator-client-1.5.2/test/test_status500_internal_server_error.py
+-rw-r--r--   0        0        0     1112 2023-05-11 17:37:01.226547 fabric-orchestrator-client-1.5.2/test/test_status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0      888 2023-05-11 17:37:01.226964 fabric-orchestrator-client-1.5.2/test/test_version.py
+-rw-r--r--   0        0        0      814 2023-05-11 17:37:01.227150 fabric-orchestrator-client-1.5.2/test/test_version_api.py
+-rw-r--r--   0        0        0      922 2023-05-11 17:37:01.227332 fabric-orchestrator-client-1.5.2/test/test_version_data.py
+-rw-r--r--   0        0        0      143 2023-05-11 17:37:01.227515 fabric-orchestrator-client-1.5.2/tox.ini
+-rw-r--r--   0        0        0    10816 1970-01-01 00:00:00.000000 fabric-orchestrator-client-1.5.2/PKG-INFO
```

### Comparing `fabric-orchestrator-client-1.5.1/.gitignore` & `fabric-orchestrator-client-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/.swagger-codegen-ignore` & `fabric-orchestrator-client-1.5.2/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/CODEGEN.md` & `fabric-orchestrator-client-1.5.2/CODEGEN.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/LICENSE` & `fabric-orchestrator-client-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/README.md` & `fabric-orchestrator-client-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/docs/PoaData.md` & `fabric-orchestrator-client-1.5.2/docs/PoaData.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/docs/PoasApi.md` & `fabric-orchestrator-client-1.5.2/docs/PoasApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/docs/ResourcesApi.md` & `fabric-orchestrator-client-1.5.2/docs/ResourcesApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/docs/SlicesApi.md` & `fabric-orchestrator-client-1.5.2/docs/SlicesApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/docs/SliversApi.md` & `fabric-orchestrator-client-1.5.2/docs/SliversApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/orchestrator_proxy.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/orchestrator_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/__init__.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/poas_api.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/poas_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/resources_api.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/slices_api.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/slices_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,59 +25,59 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def slices_create_post(self, body, name, ssh_key, **kwargs):  # noqa: E501
+    def slices_create_post(self, body, name, **kwargs):  # noqa: E501
         """Create slice  # noqa: E501
 
         Request to create slice as described in the request. Request would be a graph ML describing the requested resources. Resources may be requested to be created now or in future. On success, one or more slivers are allocated, containing resources satisfying the request, and assigned to the given slice. This API returns list and description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke get slice API to get the latest state of the requested resources.    # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.slices_create_post(body, name, ssh_key, async_req=True)
+        >>> thread = api.slices_create_post(body, name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str body: (required)
+        :param SlicesPost body: Create new Slice (required)
         :param str name: Slice Name (required)
         :param str ssh_key: User SSH Key (required)
         :param str lease_end_time: Lease End Time for the Slice
         :return: Slivers
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.slices_create_post_with_http_info(body, name, ssh_key, **kwargs)  # noqa: E501
+            return self.slices_create_post_with_http_info(body, name, **kwargs)  # noqa: E501
         else:
-            (data) = self.slices_create_post_with_http_info(body, name, ssh_key, **kwargs)  # noqa: E501
+            (data) = self.slices_create_post_with_http_info(body, name, **kwargs)  # noqa: E501
             return data
 
-    def slices_create_post_with_http_info(self, body, name, ssh_key, **kwargs):  # noqa: E501
+    def slices_create_post_with_http_info(self, body, name, **kwargs):  # noqa: E501
         """Create slice  # noqa: E501
 
         Request to create slice as described in the request. Request would be a graph ML describing the requested resources. Resources may be requested to be created now or in future. On success, one or more slivers are allocated, containing resources satisfying the request, and assigned to the given slice. This API returns list and description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke get slice API to get the latest state of the requested resources.    # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.slices_create_post_with_http_info(body, name, ssh_key, async_req=True)
+        >>> thread = api.slices_create_post_with_http_info(body, name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str body: (required)
+        :param SlicesPost body: Create new Slice (required)
         :param str name: Slice Name (required)
         :param str ssh_key: User SSH Key (required)
         :param str lease_end_time: Lease End Time for the Slice
         :return: Slivers
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body', 'name', 'ssh_key', 'lease_end_time']  # noqa: E501
+        all_params = ['body', 'name', 'lease_end_time']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -92,28 +92,22 @@
         if ('body' not in params or
                 params['body'] is None):
             raise ValueError("Missing the required parameter `body` when calling `slices_create_post`")  # noqa: E501
         # verify the required parameter 'name' is set
         if ('name' not in params or
                 params['name'] is None):
             raise ValueError("Missing the required parameter `name` when calling `slices_create_post`")  # noqa: E501
-        # verify the required parameter 'ssh_key' is set
-        if ('ssh_key' not in params or
-                params['ssh_key'] is None):
-            raise ValueError("Missing the required parameter `ssh_key` when calling `slices_create_post`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'name' in params:
             query_params.append(('name', params['name']))  # noqa: E501
-        if 'ssh_key' in params:
-            query_params.append(('ssh_key', params['ssh_key']))  # noqa: E501
         if 'lease_end_time' in params:
             query_params.append(('lease_end_time', params['lease_end_time']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -123,15 +117,15 @@
             body_params = params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['text/plain'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['bearerAuth']  # noqa: E501
 
         return self.api_client.call_api(
             '/slices/create', 'POST',
             path_params,
```

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api/version_api.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/api_client.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     Contact: kthare10@unc.edu
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 from __future__ import absolute_import
 
 import datetime
 import json
+import logging
 import mimetypes
 from multiprocessing.pool import ThreadPool
 import os
 import re
 import tempfile
 
 # python 2 and python 3 compatibility library
@@ -71,16 +72,19 @@
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
         self.user_agent = 'Swagger-Codegen/1.0.0/python'
 
     def __del__(self):
-        self.pool.close()
-        self.pool.join()
+        try:
+            self.pool.close()
+            self.pool.join()
+        except Exception as e:
+            logging.getLogger().error(f"Ignoring connexion pool error: {e}")
 
     @property
     def user_agent(self):
         """User agent for this API client"""
         return self.default_headers['User-Agent']
 
     @user_agent.setter
```

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/configuration.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/__init__.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/poa.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/poa_data.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/poa_post.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/resource.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/resources.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slice.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slice_details.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slices.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slices_post.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slices_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/sliver.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/slivers.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/version.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/models/version_data.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/fabric_cf/orchestrator/swagger_client/rest.py` & `fabric-orchestrator-client-1.5.2/fabric_cf/orchestrator/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/git_push.sh` & `fabric-orchestrator-client-1.5.2/git_push.sh`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/pyproject.toml` & `fabric-orchestrator-client-1.5.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 requires-python = '>=3.9'
 dependencies = [
     "certifi >= 14.05.14",
     "six >= 1.10",
     "python_dateutil >= 2.5.3",
     "requests>=2.28.1",
-    "fabric-fim==1.5.2",
+    "fabric-fim==1.5.3",
     ]
 
 [project.optional-dependencies]
 test = ["coverage>=4.0.3",
         "nose>=1.3.7",
         "pluggy>=0.3.1",
         "py>=1.4.31",
```

### Comparing `fabric-orchestrator-client-1.5.1/test/test_poa.py` & `fabric-orchestrator-client-1.5.2/test/test_poa.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_poa_data.py` & `fabric-orchestrator-client-1.5.2/test/test_poa_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_poa_post.py` & `fabric-orchestrator-client-1.5.2/test/test_poa_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_poa_post_data.py` & `fabric-orchestrator-client-1.5.2/test/test_poa_post_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_poa_post_data_vcpu_cpu_map.py` & `fabric-orchestrator-client-1.5.2/test/test_poa_post_data_vcpu_cpu_map.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_poas_api.py` & `fabric-orchestrator-client-1.5.2/test/test_poas_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_resource.py` & `fabric-orchestrator-client-1.5.2/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_resources.py` & `fabric-orchestrator-client-1.5.2/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_resources_api.py` & `fabric-orchestrator-client-1.5.2/test/test_resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_slice.py` & `fabric-orchestrator-client-1.5.2/test/test_slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_slice_details.py` & `fabric-orchestrator-client-1.5.2/test/test_slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_slices.py` & `fabric-orchestrator-client-1.5.2/test/test_slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_slices_api.py` & `fabric-orchestrator-client-1.5.2/test/test_slices_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_slices_post.py` & `fabric-orchestrator-client-1.5.2/test/test_slices_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_sliver.py` & `fabric-orchestrator-client-1.5.2/test/test_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_slivers.py` & `fabric-orchestrator-client-1.5.2/test/test_slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_slivers_api.py` & `fabric-orchestrator-client-1.5.2/test/test_slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_status200_ok_no_content.py` & `fabric-orchestrator-client-1.5.2/test/test_status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.5.2/test/test_status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_status200_ok_paginated.py` & `fabric-orchestrator-client-1.5.2/test/test_status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_status200_ok_single.py` & `fabric-orchestrator-client-1.5.2/test/test_status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_status400_bad_request.py` & `fabric-orchestrator-client-1.5.2/test/test_status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_status400_bad_request_errors.py` & `fabric-orchestrator-client-1.5.2/test/test_status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_status401_unauthorized.py` & `fabric-orchestrator-client-1.5.2/test/test_status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.5.2/test/test_status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_status403_forbidden.py` & `fabric-orchestrator-client-1.5.2/test/test_status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_status403_forbidden_errors.py` & `fabric-orchestrator-client-1.5.2/test/test_status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_status404_not_found.py` & `fabric-orchestrator-client-1.5.2/test/test_status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_status404_not_found_errors.py` & `fabric-orchestrator-client-1.5.2/test/test_status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_status500_internal_server_error.py` & `fabric-orchestrator-client-1.5.2/test/test_status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.5.2/test/test_status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_version.py` & `fabric-orchestrator-client-1.5.2/test/test_version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_version_api.py` & `fabric-orchestrator-client-1.5.2/test/test_version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/test/test_version_data.py` & `fabric-orchestrator-client-1.5.2/test/test_version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.5.1/PKG-INFO` & `fabric-orchestrator-client-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: fabric-orchestrator-client
-Version: 1.5.1
+Version: 1.5.2
 Summary: Fabric Orchestrator API
 Keywords: Swagger,Fabric Orchestrator API
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: certifi >= 14.05.14
 Requires-Dist: six >= 1.10
 Requires-Dist: python_dateutil >= 2.5.3
 Requires-Dist: requests>=2.28.1
-Requires-Dist: fabric-fim==1.5.2
+Requires-Dist: fabric-fim==1.5.3
 Requires-Dist: coverage>=4.0.3 ; extra == "test"
 Requires-Dist: nose>=1.3.7 ; extra == "test"
 Requires-Dist: pluggy>=0.3.1 ; extra == "test"
 Requires-Dist: py>=1.4.31 ; extra == "test"
 Requires-Dist: randomize>=0.13 ; extra == "test"
 Project-URL: Home, https://fabric-testbed.net/
 Project-URL: Sources, https://github.com/fabric-testbed/OrchestratorClient
```

