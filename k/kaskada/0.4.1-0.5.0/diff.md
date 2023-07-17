# Comparing `tmp/kaskada-0.4.1.tar.gz` & `tmp/kaskada-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaskada-0.4.1.tar", max compression
+gzip compressed data, was "kaskada-0.5.0.tar", max compression
```

## Comparing `kaskada-0.4.1.tar` & `kaskada-0.5.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1646 2023-05-01 19:22:44.891724 kaskada-0.4.1/README.md
--rw-r--r--   0        0        0     3917 2023-06-20 17:23:20.820629 kaskada-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     7656 2023-06-06 17:35:42.987556 kaskada-0.4.1/src/fenlmagic/__init__.py
--rw-r--r--   0        0        0      401 2023-04-05 20:07:05.230947 kaskada-0.4.1/src/fenlmagic/utils.py
--rw-r--r--   0        0        0       33 2023-05-01 19:22:44.892917 kaskada-0.4.1/src/kaskada/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 15:20:54.673916 kaskada-0.4.1/src/kaskada/api/__init__.py
--rw-r--r--   0        0        0      569 2023-05-23 16:27:30.619980 kaskada-0.4.1/src/kaskada/api/api_utils.py
--rw-r--r--   0        0        0        0 2023-05-23 16:27:30.620032 kaskada-0.4.1/src/kaskada/api/local_session/__init__.py
--rw-r--r--   0        0        0     3573 2023-05-23 16:27:30.620441 kaskada-0.4.1/src/kaskada/api/local_session/local_service.py
--rw-r--r--   0        0        0     3312 2023-05-24 15:28:38.424727 kaskada-0.4.1/src/kaskada/api/local_session/local_session_keep_alive.py
--rw-r--r--   0        0        0     6381 2023-04-05 20:07:05.231172 kaskada-0.4.1/src/kaskada/api/release.py
--rw-r--r--   0        0        0     1108 2023-06-06 17:35:42.987905 kaskada-0.4.1/src/kaskada/api/remote_session/__init__.py
--rw-r--r--   0        0        0    11294 2023-06-15 16:50:30.249227 kaskada-0.4.1/src/kaskada/api/session.py
--rw-r--r--   0        0        0    11972 2023-06-06 17:35:42.988531 kaskada-0.4.1/src/kaskada/client.py
--rw-r--r--   0        0        0     1500 2023-04-05 20:07:05.231408 kaskada-0.4.1/src/kaskada/formatters.css
--rw-r--r--   0        0        0      984 2023-04-05 20:07:05.231471 kaskada-0.4.1/src/kaskada/formatters.js
--rw-r--r--   0        0        0    26206 2023-04-05 20:07:05.231594 kaskada-0.4.1/src/kaskada/formatters.py
--rw-r--r--   0        0        0     7337 2023-05-01 19:22:49.940266 kaskada-0.4.1/src/kaskada/formatters_helpers.py
--rw-r--r--   0        0        0    10325 2023-05-30 23:13:08.825837 kaskada-0.4.1/src/kaskada/formatters_shared.py
--rw-r--r--   0        0        0        0 2023-05-23 16:27:30.621359 kaskada-0.4.1/src/kaskada/health/__init__.py
--rw-r--r--   0        0        0     1886 2023-05-23 16:27:30.621683 kaskada-0.4.1/src/kaskada/health/health_check_client.py
--rw-r--r--   0        0        0     4522 2023-05-23 16:27:30.621896 kaskada-0.4.1/src/kaskada/health/health_check_servicer.py
--rw-r--r--   0        0        0     2326 2023-05-23 16:27:30.622083 kaskada-0.4.1/src/kaskada/health/health_check_watcher.py
--rw-r--r--   0        0        0     7626 2023-06-16 14:06:27.521454 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/common_pb2.py
--rw-r--r--   0        0        0      159 2023-06-16 14:06:27.526292 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
--rw-r--r--   0        0        0    13155 2023-06-16 14:06:27.520709 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
--rw-r--r--   0        0        0    12538 2023-06-16 14:06:27.530338 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
--rw-r--r--   0        0        0     4489 2023-06-16 14:06:27.527963 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
--rw-r--r--   0        0        0     2938 2023-06-16 14:06:27.529640 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
--rw-r--r--   0        0        0     4191 2023-06-16 14:06:27.522431 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/destinations_pb2.py
--rw-r--r--   0        0        0      159 2023-06-16 14:06:27.526364 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
--rw-r--r--   0        0        0     2718 2023-06-16 14:06:27.530593 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
--rw-r--r--   0        0        0      159 2023-06-16 14:06:27.531560 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
--rw-r--r--   0        0        0     3976 2023-06-16 14:06:27.532320 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/file_service_pb2.py
--rw-r--r--   0        0        0     5054 2023-06-16 14:06:27.533962 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
--rw-r--r--   0        0        0     1710 2023-05-15 22:34:43.474188 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/health_pb2.py
--rw-r--r--   0        0        0      159 2023-05-15 22:34:43.474353 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/health_pb2_grpc.py
--rw-r--r--   0        0        0    10837 2023-06-16 14:06:27.534314 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
--rw-r--r--   0        0        0     9283 2023-06-16 14:06:27.536488 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
--rw-r--r--   0        0        0     1897 2023-06-16 14:06:27.536464 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/options_pb2.py
--rw-r--r--   0        0        0      159 2023-06-16 14:06:27.538548 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
--rw-r--r--   0        0        0    13180 2023-06-16 14:06:27.541085 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/plan_pb2.py
--rw-r--r--   0        0        0      159 2023-06-16 14:06:27.540976 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
--rw-r--r--   0        0        0     3398 2023-06-16 14:06:27.541884 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
--rw-r--r--   0        0        0     4894 2023-06-16 14:06:27.542461 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
--rw-r--r--   0        0        0     2805 2023-06-16 14:06:27.543469 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/pulsar_pb2.py
--rw-r--r--   0        0        0      159 2023-06-16 14:06:27.543684 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/pulsar_pb2_grpc.py
--rw-r--r--   0        0        0    11773 2023-06-16 14:06:27.544769 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/query_service_pb2.py
--rw-r--r--   0        0        0     6542 2023-06-16 14:06:27.545476 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     4018 2023-06-16 14:06:27.545999 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/schema_pb2.py
--rw-r--r--   0        0        0      159 2023-06-16 14:06:27.544085 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-06-16 14:06:27.546778 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/sources_pb2.py
--rw-r--r--   0        0        0      159 2023-06-16 14:06:27.547035 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/sources_pb2_grpc.py
--rw-r--r--   0        0        0     2729 2023-06-16 14:06:27.548973 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/spec_pb2.py
--rw-r--r--   0        0        0      159 2023-06-16 14:06:27.549601 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
--rw-r--r--   0        0        0    11249 2023-06-16 14:06:27.552866 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/table_service_pb2.py
--rw-r--r--   0        0        0    10053 2023-06-16 14:06:27.553614 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
--rw-r--r--   0        0        0     5157 2023-06-16 14:06:27.554368 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
--rw-r--r--   0        0        0      159 2023-06-16 14:06:27.554353 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
--rw-r--r--   0        0        0     8140 2023-06-16 14:06:27.555880 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/view_service_pb2.py
--rw-r--r--   0        0        0     8153 2023-06-16 14:06:27.556002 kaskada-0.4.1/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
--rw-r--r--   0        0        0    16491 2023-06-16 14:06:27.555867 kaskada-0.4.1/src/kaskada/kaskada/v2alpha/query_service_pb2.py
--rw-r--r--   0        0        0     8377 2023-06-16 14:06:27.556311 kaskada-0.4.1/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     8622 2023-05-01 19:22:49.940570 kaskada-0.4.1/src/kaskada/materialization.py
--rw-r--r--   0        0        0     9272 2023-05-01 19:22:49.940719 kaskada-0.4.1/src/kaskada/query.py
--rw-r--r--   0        0        0     2564 2023-04-05 20:07:05.232035 kaskada-0.4.1/src/kaskada/slice_filters.py
--rw-r--r--   0        0        0    10286 2023-06-06 17:35:42.988703 kaskada-0.4.1/src/kaskada/table.py
--rw-r--r--   0        0        0     7131 2023-05-08 21:01:05.018302 kaskada-0.4.1/src/kaskada/utils.py
--rw-r--r--   0        0        0     4543 2023-05-01 19:22:49.941272 kaskada-0.4.1/src/kaskada/view.py
--rw-r--r--   0        0        0    29800 2023-04-05 20:07:05.233220 kaskada-0.4.1/vendor/validate/validate.proto
--rw-r--r--   0        0        0    13089 2023-04-05 20:07:05.233314 kaskada-0.4.1/vendor/validate/validate_pb2.py
--rw-r--r--   0        0        0    22952 2023-04-05 20:07:05.233416 kaskada-0.4.1/vendor/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-05 20:07:05.233487 kaskada-0.4.1/vendor/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 kaskada-0.4.1/setup.py
--rw-r--r--   0        0        0     2742 1970-01-01 00:00:00.000000 kaskada-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1646 2023-07-17 18:54:47.236325 kaskada-0.5.0/README.md
+-rw-r--r--   0        0        0     3917 2023-07-17 18:54:47.236325 kaskada-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7632 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/fenlmagic/__init__.py
+-rw-r--r--   0        0        0      401 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/fenlmagic/utils.py
+-rw-r--r--   0        0        0       33 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/api/__init__.py
+-rw-r--r--   0        0        0      569 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/api/api_utils.py
+-rw-r--r--   0        0        0        0 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/api/local_session/__init__.py
+-rw-r--r--   0        0        0     3573 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/api/local_session/local_service.py
+-rw-r--r--   0        0        0     3312 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/api/local_session/local_session_keep_alive.py
+-rw-r--r--   0        0        0     6381 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/api/release.py
+-rw-r--r--   0        0        0     1108 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/api/remote_session/__init__.py
+-rw-r--r--   0        0        0    12106 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/api/session.py
+-rw-r--r--   0        0        0    11972 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/client.py
+-rw-r--r--   0        0        0     1500 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/formatters.css
+-rw-r--r--   0        0        0      984 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/formatters.js
+-rw-r--r--   0        0        0    26206 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/formatters.py
+-rw-r--r--   0        0        0     7337 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/formatters_helpers.py
+-rw-r--r--   0        0        0    10325 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/formatters_shared.py
+-rw-r--r--   0        0        0        0 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/health/__init__.py
+-rw-r--r--   0        0        0     1886 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/health/health_check_client.py
+-rw-r--r--   0        0        0     4522 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/health/health_check_servicer.py
+-rw-r--r--   0        0        0     2326 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/health/health_check_watcher.py
+-rw-r--r--   0        0        0     7352 2023-07-17 18:54:48.012318 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/common_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-17 18:54:48.012318 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
+-rw-r--r--   0        0        0    13155 2023-07-17 18:54:48.044319 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
+-rw-r--r--   0        0        0    12538 2023-07-17 18:54:48.044319 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4489 2023-07-17 18:54:48.072320 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
+-rw-r--r--   0        0        0     2938 2023-07-17 18:54:48.068320 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4191 2023-07-17 18:54:48.092320 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/destinations_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-17 18:54:48.120321 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
+-rw-r--r--   0        0        0     2718 2023-07-17 18:54:48.124321 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-17 18:54:48.148322 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
+-rw-r--r--   0        0        0     4491 2023-07-17 18:54:48.152322 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/file_service_pb2.py
+-rw-r--r--   0        0        0     5054 2023-07-17 18:54:48.180323 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2222 2023-07-17 18:54:48.184323 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/kafka_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-17 18:54:48.204323 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/kafka_pb2_grpc.py
+-rw-r--r--   0        0        0    10837 2023-07-17 18:54:48.228324 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
+-rw-r--r--   0        0        0     9283 2023-07-17 18:54:48.232324 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1897 2023-07-17 18:54:48.256325 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/options_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-17 18:54:48.468330 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
+-rw-r--r--   0        0        0    13180 2023-07-17 18:54:48.284325 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/plan_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-17 18:54:48.320326 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
+-rw-r--r--   0        0        0     3398 2023-07-17 18:54:48.352327 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
+-rw-r--r--   0        0        0     4894 2023-07-17 18:54:48.392328 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2805 2023-07-17 18:54:48.420329 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/pulsar_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-17 18:54:48.456330 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/pulsar_pb2_grpc.py
+-rw-r--r--   0        0        0    11773 2023-07-17 18:54:48.484331 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     6542 2023-07-17 18:54:48.496331 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4384 2023-07-17 18:54:48.512332 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/schema_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-17 18:54:48.528332 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
+-rw-r--r--   0        0        0     2827 2023-07-17 18:54:48.540332 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/sources_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-17 18:54:48.552333 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/sources_pb2_grpc.py
+-rw-r--r--   0        0        0     2729 2023-07-17 18:54:48.568333 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/spec_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-17 18:54:48.588334 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
+-rw-r--r--   0        0        0    11323 2023-07-17 18:54:48.592334 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/table_service_pb2.py
+-rw-r--r--   0        0        0    10053 2023-07-17 18:54:48.612334 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5157 2023-07-17 18:54:48.624335 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-17 18:54:48.632335 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
+-rw-r--r--   0        0        0     8140 2023-07-17 18:54:48.648336 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/view_service_pb2.py
+-rw-r--r--   0        0        0     8153 2023-07-17 18:54:48.668336 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
+-rw-r--r--   0        0        0    16491 2023-07-17 18:54:48.680336 kaskada-0.5.0/src/kaskada/kaskada/v2alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     8377 2023-07-17 18:54:48.708337 kaskada-0.5.0/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8622 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/materialization.py
+-rw-r--r--   0        0        0     9272 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/query.py
+-rw-r--r--   0        0        0     2564 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/slice_filters.py
+-rw-r--r--   0        0        0    10286 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/table.py
+-rw-r--r--   0        0        0     7131 2023-07-17 18:54:47.240324 kaskada-0.5.0/src/kaskada/utils.py
+-rw-r--r--   0        0        0     4543 2023-07-17 18:54:47.240324 kaskada-0.5.0/src/kaskada/view.py
+-rw-r--r--   0        0        0    29800 2023-07-17 18:54:47.240324 kaskada-0.5.0/vendor/validate/validate.proto
+-rw-r--r--   0        0        0    13089 2023-07-17 18:54:47.240324 kaskada-0.5.0/vendor/validate/validate_pb2.py
+-rw-r--r--   0        0        0    22952 2023-07-17 18:54:47.240324 kaskada-0.5.0/vendor/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-17 18:54:47.240324 kaskada-0.5.0/vendor/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 kaskada-0.5.0/setup.py
+-rw-r--r--   0        0        0     2742 1970-01-01 00:00:00.000000 kaskada-0.5.0/PKG-INFO
```

### Comparing `kaskada-0.4.1/README.md` & `kaskada-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/pyproject.toml` & `kaskada-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kaskada"
-version = "0.4.1"
+version = "0.5.0"
 description = "A client library for the Kaskada time travel machine learning service"
 authors = ["Kaskada <maintainers@kaskada.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "kaskada", from = "src" },
     { include = "validate", from = "vendor" },
```

### Comparing `kaskada-0.4.1/src/fenlmagic/__init__.py` & `kaskada-0.5.0/src/fenlmagic/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -141,38 +141,34 @@
                 changed_since_time=clean_arg(args.changed_since_time),
                 final_result_time=clean_arg(args.final_time),
                 limits=query_pb.Query.Limits(**limits),
                 response_as=response_as,
                 client=self.client,
             )
             query_result = QueryResult(expression, resp)
-
             if not dry_run and render_dataframe:
-                # TODO: figure out how to support reading from multiple parquet paths
-                if (
-                    len(
-                        query_result.query_response.destination.object_store.output_paths.paths
-                    )
-                    > 0
-                ):
-                    if response_as == query.ResponseType.FILE_TYPE_PARQUET:
-                        df = pandas.read_parquet(
-                            query_result.query_response.destination.object_store.output_paths.paths[
-                                0
-                            ],
-                            engine="pyarrow",
-                        )
-                        query_result.set_dataframe(df)
-                    elif response_as == query.ResponseType.FILE_TYPE_CSV:
-                        df = pandas.read_csv(
-                            query_result.query_response.destination.object_store.output_paths.paths[
-                                0
-                            ],
-                        )
-                        query_result.set_dataframe(df)
+                output_paths = (
+                    query_result.query_response.destination.object_store.output_paths.paths
+                )
+                if len(output_paths) > 0:
+                    dataframes = []
+                    for parquet_output_path in output_paths:
+                        if response_as == query.ResponseType.FILE_TYPE_PARQUET:
+                            df = pandas.read_parquet(
+                                parquet_output_path, engine="pyarrow"
+                            )
+                            dataframes.append(df)
+                        elif response_as == query.ResponseType.FILE_TYPE_CSV:
+                            df = pandas.read_csv(parquet_output_path, engine="pyarrow")
+                            dataframes.append(df)
+                        else:
+                            raise NotImplementedError(
+                                f"unknown response type: {response_as}", response_as
+                            )
+                    query_result.set_dataframe(pandas.concat(dataframes))
 
             if var is not None:
                 IPython.get_ipython().push({var: query_result})
 
             return query_result
         except Exception as e:
             raise UsageError(e)
```

### Comparing `kaskada-0.4.1/src/kaskada/api/api_utils.py` & `kaskada-0.5.0/src/kaskada/api/api_utils.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/api/local_session/local_service.py` & `kaskada-0.5.0/src/kaskada/api/local_session/local_service.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/api/local_session/local_session_keep_alive.py` & `kaskada-0.5.0/src/kaskada/api/local_session/local_session_keep_alive.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/api/release.py` & `kaskada-0.5.0/src/kaskada/api/release.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/api/remote_session/__init__.py` & `kaskada-0.5.0/src/kaskada/api/remote_session/__init__.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/api/session.py` & `kaskada-0.5.0/src/kaskada/api/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 import os
-import time
 from abc import ABC
 from datetime import datetime
 from pathlib import Path
-from typing import Any, Dict, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
 import kaskada.client
 from kaskada.api import release
 from kaskada.api.local_session.local_service import KaskadaLocalService
 from kaskada.api.local_session.local_session_keep_alive import LocalSessionKeepAlive
 
 logger = logging.getLogger(__name__)
@@ -189,14 +188,35 @@
         return self
 
     def database_path(self, path: str):
         self.manager_configs["-db-path"] = path
         self.in_memory(False)
         return self
 
+    def with_manager_args(self, configs: List[Tuple[str, Any]]):
+        """Configure the Manager to run with a list of arguments. The arguments must be prefixed with a "-" and boolean values are represented as "1" or "0".
+
+        For example:
+        ```
+        from kaskada.api.session import LocalBuilder
+            session = LocalBuilder().with_manager_configs([
+                ("-object-store-type", "local"),
+                ("-object-store-path", "/Users/kevin.nguyen/Github/kaskada/examples3"),
+                ("-db-in-memory", "1"),
+                ("-rest-port", 12345)
+            ]).build()
+        ```
+
+        Args:
+            configs (List[Tuple[str, Any]]): Manager arguments
+        """
+        for config in configs:
+            self.manager_configs[config[0]] = config[1]
+        return self
+
     def manager_rest_port(self, port: int):
         self.manager_configs["-rest-port"] = port
         return self
 
     def manager_grpc_port(self, port: int):
         self.manager_configs["-grpc-port"] = port
         return self
```

### Comparing `kaskada-0.4.1/src/kaskada/client.py` & `kaskada-0.5.0/src/kaskada/client.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/formatters.css` & `kaskada-0.5.0/src/kaskada/formatters.css`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/formatters.js` & `kaskada-0.5.0/src/kaskada/formatters.js`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/formatters.py` & `kaskada-0.5.0/src/kaskada/formatters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/formatters_helpers.py` & `kaskada-0.5.0/src/kaskada/formatters_helpers.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/formatters_shared.py` & `kaskada-0.5.0/src/kaskada/formatters_shared.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/health/health_check_client.py` & `kaskada-0.5.0/src/kaskada/health/health_check_client.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/health/health_check_servicer.py` & `kaskada-0.5.0/src/kaskada/health/health_check_servicer.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/health/health_check_watcher.py` & `kaskada-0.5.0/src/kaskada/health/health_check_watcher.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/common_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/common_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,56 +10,55 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from kaskada.kaskada.v1alpha import fenl_diagnostics_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_fenl__diagnostics__pb2
-from kaskada.kaskada.v1alpha import pulsar_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_pulsar__pb2
 from kaskada.kaskada.v1alpha import schema_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_schema__pb2
 from kaskada.kaskada.v1alpha import sources_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_sources__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$kaskada/kaskada/v1alpha/common.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a.kaskada/kaskada/v1alpha/fenl_diagnostics.proto\x1a$kaskada/kaskada/v1alpha/pulsar.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\x1a%kaskada/kaskada/v1alpha/sources.proto\"\xd5\x01\n\nSourceData\x12#\n\x0cparquet_path\x18\x01 \x01(\tH\x00R\x0bparquetPath\x12\x1b\n\x08\x63sv_path\x18\x02 \x01(\tH\x00R\x07\x63svPath\x12\x1b\n\x08\x63sv_data\x18\x03 \x01(\tH\x00R\x07\x63svData\x12^\n\x13pulsar_subscription\x18\x04 \x01(\x0b\x32+.kaskada.kaskada.v1alpha.PulsarSubscriptionH\x00R\x12pulsarSubscriptionB\x08\n\x06source\"]\n\tFileInput\x12>\n\tfile_type\x18\x01 \x01(\x0e\x32!.kaskada.kaskada.v1alpha.FileTypeR\x08\x66ileType\x12\x10\n\x03uri\x18\x02 \x01(\tR\x03uri\"c\n\x0b\x46ileResults\x12>\n\tfile_type\x18\x01 \x01(\x0e\x32!.kaskada.kaskada.v1alpha.FileTypeR\x08\x66ileType\x12\x14\n\x05paths\x18\x02 \x03(\tR\x05paths\"\xae\x02\n\x0bTableConfig\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x12\n\x04uuid\x18\x06 \x01(\tR\x04uuid\x12(\n\x10time_column_name\x18\x02 \x01(\tR\x0etimeColumnName\x12L\n\x13subsort_column_name\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x11subsortColumnName\x12*\n\x11group_column_name\x18\x04 \x01(\tR\x0fgroupColumnName\x12\x1a\n\x08grouping\x18\x05 \x01(\tR\x08grouping\x12\x37\n\x06source\x18\x07 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SourceR\x06source\"g\n\rTableMetadata\x12\x37\n\x06schema\x18\x01 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SchemaR\x06schema\x12\x1d\n\nfile_count\x18\x02 \x01(\x03R\tfileCount\"\xe6\x01\n\x0cPreparedFile\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12@\n\x0emin_event_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cminEventTime\x12@\n\x0emax_event_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cmaxEventTime\x12\x19\n\x08num_rows\x18\x04 \x01(\x03R\x07numRows\x12#\n\rmetadata_path\x18\x05 \x01(\tR\x0cmetadataPath\"\xb5\x02\n\tSlicePlan\x12\x1d\n\ntable_name\x18\x01 \x01(\tR\ttableName\x12K\n\x07percent\x18\x02 \x01(\x0b\x32/.kaskada.kaskada.v1alpha.SlicePlan.PercentSliceH\x00R\x07percent\x12U\n\x0b\x65ntity_keys\x18\x03 \x01(\x0b\x32\x32.kaskada.kaskada.v1alpha.SlicePlan.EntityKeysSliceH\x00R\nentityKeys\x1a(\n\x0cPercentSlice\x12\x18\n\x07percent\x18\x01 \x01(\x01R\x07percent\x1a\x32\n\x0f\x45ntityKeysSlice\x12\x1f\n\x0b\x65ntity_keys\x18\x01 \x03(\tR\nentityKeysB\x07\n\x05slice\",\n\x04Uuid\x12\x12\n\x04high\x18\x01 \x01(\x04R\x04high\x12\x10\n\x03low\x18\x02 \x01(\x04R\x03low\"\x9f\x02\n\x0cSliceRequest\x12N\n\x07percent\x18\x01 \x01(\x0b\x32\x32.kaskada.kaskada.v1alpha.SliceRequest.PercentSliceH\x00R\x07percent\x12X\n\x0b\x65ntity_keys\x18\x02 \x01(\x0b\x32\x35.kaskada.kaskada.v1alpha.SliceRequest.EntityKeysSliceH\x00R\nentityKeys\x1a(\n\x0cPercentSlice\x12\x18\n\x07percent\x18\x01 \x01(\x01R\x07percent\x1a\x32\n\x0f\x45ntityKeysSlice\x12\x1f\n\x0b\x65ntity_keys\x18\x02 \x03(\tR\nentityKeysB\x07\n\x05slice\"\xc4\x01\n\x08\x41nalysis\x12#\n\rmissing_names\x18\x01 \x03(\tR\x0cmissingNames\x12S\n\x10\x66\x65nl_diagnostics\x18\x02 \x01(\x0b\x32(.kaskada.kaskada.v1alpha.FenlDiagnosticsR\x0f\x66\x65nlDiagnostics\x12\x1f\n\x0b\x63\x61n_execute\x18\x03 \x01(\x08R\ncanExecute\x12\x1d\n\nfree_names\x18\x04 \x03(\tR\tfreeNames\"/\n\x0eRequestDetails\x12\x1d\n\nrequest_id\x18\x01 \x01(\tR\trequestId*O\n\x08\x46ileType\x12\x19\n\x15\x46ILE_TYPE_UNSPECIFIED\x10\x00\x12\x15\n\x11\x46ILE_TYPE_PARQUET\x10\x01\x12\x11\n\rFILE_TYPE_CSV\x10\x02*\x9b\x01\n\x11PerEntityBehavior\x12#\n\x1fPER_ENTITY_BEHAVIOR_UNSPECIFIED\x10\x00\x12\x1b\n\x17PER_ENTITY_BEHAVIOR_ALL\x10\x01\x12\x1d\n\x19PER_ENTITY_BEHAVIOR_FINAL\x10\x02\x12%\n!PER_ENTITY_BEHAVIOR_FINAL_AT_TIME\x10\x03\x42\xfb\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\x0b\x43ommonProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$kaskada/kaskada/v1alpha/common.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a.kaskada/kaskada/v1alpha/fenl_diagnostics.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\x1a%kaskada/kaskada/v1alpha/sources.proto\"u\n\nSourceData\x12#\n\x0cparquet_path\x18\x01 \x01(\tH\x00R\x0bparquetPath\x12\x1b\n\x08\x63sv_path\x18\x02 \x01(\tH\x00R\x07\x63svPath\x12\x1b\n\x08\x63sv_data\x18\x03 \x01(\tH\x00R\x07\x63svDataB\x08\n\x06source\"]\n\tFileInput\x12>\n\tfile_type\x18\x01 \x01(\x0e\x32!.kaskada.kaskada.v1alpha.FileTypeR\x08\x66ileType\x12\x10\n\x03uri\x18\x02 \x01(\tR\x03uri\"c\n\x0b\x46ileResults\x12>\n\tfile_type\x18\x01 \x01(\x0e\x32!.kaskada.kaskada.v1alpha.FileTypeR\x08\x66ileType\x12\x14\n\x05paths\x18\x02 \x03(\tR\x05paths\"\xae\x02\n\x0bTableConfig\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x12\n\x04uuid\x18\x06 \x01(\tR\x04uuid\x12(\n\x10time_column_name\x18\x02 \x01(\tR\x0etimeColumnName\x12L\n\x13subsort_column_name\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x11subsortColumnName\x12*\n\x11group_column_name\x18\x04 \x01(\tR\x0fgroupColumnName\x12\x1a\n\x08grouping\x18\x05 \x01(\tR\x08grouping\x12\x37\n\x06source\x18\x07 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SourceR\x06source\"g\n\rTableMetadata\x12\x37\n\x06schema\x18\x01 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SchemaR\x06schema\x12\x1d\n\nfile_count\x18\x02 \x01(\x03R\tfileCount\"\xe6\x01\n\x0cPreparedFile\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12@\n\x0emin_event_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cminEventTime\x12@\n\x0emax_event_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cmaxEventTime\x12\x19\n\x08num_rows\x18\x04 \x01(\x03R\x07numRows\x12#\n\rmetadata_path\x18\x05 \x01(\tR\x0cmetadataPath\"\xb5\x02\n\tSlicePlan\x12\x1d\n\ntable_name\x18\x01 \x01(\tR\ttableName\x12K\n\x07percent\x18\x02 \x01(\x0b\x32/.kaskada.kaskada.v1alpha.SlicePlan.PercentSliceH\x00R\x07percent\x12U\n\x0b\x65ntity_keys\x18\x03 \x01(\x0b\x32\x32.kaskada.kaskada.v1alpha.SlicePlan.EntityKeysSliceH\x00R\nentityKeys\x1a(\n\x0cPercentSlice\x12\x18\n\x07percent\x18\x01 \x01(\x01R\x07percent\x1a\x32\n\x0f\x45ntityKeysSlice\x12\x1f\n\x0b\x65ntity_keys\x18\x01 \x03(\tR\nentityKeysB\x07\n\x05slice\",\n\x04Uuid\x12\x12\n\x04high\x18\x01 \x01(\x04R\x04high\x12\x10\n\x03low\x18\x02 \x01(\x04R\x03low\"\x9f\x02\n\x0cSliceRequest\x12N\n\x07percent\x18\x01 \x01(\x0b\x32\x32.kaskada.kaskada.v1alpha.SliceRequest.PercentSliceH\x00R\x07percent\x12X\n\x0b\x65ntity_keys\x18\x02 \x01(\x0b\x32\x35.kaskada.kaskada.v1alpha.SliceRequest.EntityKeysSliceH\x00R\nentityKeys\x1a(\n\x0cPercentSlice\x12\x18\n\x07percent\x18\x01 \x01(\x01R\x07percent\x1a\x32\n\x0f\x45ntityKeysSlice\x12\x1f\n\x0b\x65ntity_keys\x18\x02 \x03(\tR\nentityKeysB\x07\n\x05slice\"\xc4\x01\n\x08\x41nalysis\x12#\n\rmissing_names\x18\x01 \x03(\tR\x0cmissingNames\x12S\n\x10\x66\x65nl_diagnostics\x18\x02 \x01(\x0b\x32(.kaskada.kaskada.v1alpha.FenlDiagnosticsR\x0f\x66\x65nlDiagnostics\x12\x1f\n\x0b\x63\x61n_execute\x18\x03 \x01(\x08R\ncanExecute\x12\x1d\n\nfree_names\x18\x04 \x03(\tR\tfreeNames\"/\n\x0eRequestDetails\x12\x1d\n\nrequest_id\x18\x01 \x01(\tR\trequestId*O\n\x08\x46ileType\x12\x19\n\x15\x46ILE_TYPE_UNSPECIFIED\x10\x00\x12\x15\n\x11\x46ILE_TYPE_PARQUET\x10\x01\x12\x11\n\rFILE_TYPE_CSV\x10\x02*\x9b\x01\n\x11PerEntityBehavior\x12#\n\x1fPER_ENTITY_BEHAVIOR_UNSPECIFIED\x10\x00\x12\x1b\n\x17PER_ENTITY_BEHAVIOR_ALL\x10\x01\x12\x1d\n\x19PER_ENTITY_BEHAVIOR_FINAL\x10\x02\x12%\n!PER_ENTITY_BEHAVIOR_FINAL_AT_TIME\x10\x03\x42\xfb\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\x0b\x43ommonProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\013CommonProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
-  _globals['_FILETYPE']._serialized_start=2244
-  _globals['_FILETYPE']._serialized_end=2323
-  _globals['_PERENTITYBEHAVIOR']._serialized_start=2326
-  _globals['_PERENTITYBEHAVIOR']._serialized_end=2481
-  _globals['_SOURCEDATA']._serialized_start=294
-  _globals['_SOURCEDATA']._serialized_end=507
-  _globals['_FILEINPUT']._serialized_start=509
-  _globals['_FILEINPUT']._serialized_end=602
-  _globals['_FILERESULTS']._serialized_start=604
-  _globals['_FILERESULTS']._serialized_end=703
-  _globals['_TABLECONFIG']._serialized_start=706
-  _globals['_TABLECONFIG']._serialized_end=1008
-  _globals['_TABLEMETADATA']._serialized_start=1010
-  _globals['_TABLEMETADATA']._serialized_end=1113
-  _globals['_PREPAREDFILE']._serialized_start=1116
-  _globals['_PREPAREDFILE']._serialized_end=1346
-  _globals['_SLICEPLAN']._serialized_start=1349
-  _globals['_SLICEPLAN']._serialized_end=1658
-  _globals['_SLICEPLAN_PERCENTSLICE']._serialized_start=1557
-  _globals['_SLICEPLAN_PERCENTSLICE']._serialized_end=1597
-  _globals['_SLICEPLAN_ENTITYKEYSSLICE']._serialized_start=1599
-  _globals['_SLICEPLAN_ENTITYKEYSSLICE']._serialized_end=1649
-  _globals['_UUID']._serialized_start=1660
-  _globals['_UUID']._serialized_end=1704
-  _globals['_SLICEREQUEST']._serialized_start=1707
-  _globals['_SLICEREQUEST']._serialized_end=1994
-  _globals['_SLICEREQUEST_PERCENTSLICE']._serialized_start=1557
-  _globals['_SLICEREQUEST_PERCENTSLICE']._serialized_end=1597
-  _globals['_SLICEREQUEST_ENTITYKEYSSLICE']._serialized_start=1935
-  _globals['_SLICEREQUEST_ENTITYKEYSSLICE']._serialized_end=1985
-  _globals['_ANALYSIS']._serialized_start=1997
-  _globals['_ANALYSIS']._serialized_end=2193
-  _globals['_REQUESTDETAILS']._serialized_start=2195
-  _globals['_REQUESTDETAILS']._serialized_end=2242
+  _globals['_FILETYPE']._serialized_start=2109
+  _globals['_FILETYPE']._serialized_end=2188
+  _globals['_PERENTITYBEHAVIOR']._serialized_start=2191
+  _globals['_PERENTITYBEHAVIOR']._serialized_end=2346
+  _globals['_SOURCEDATA']._serialized_start=255
+  _globals['_SOURCEDATA']._serialized_end=372
+  _globals['_FILEINPUT']._serialized_start=374
+  _globals['_FILEINPUT']._serialized_end=467
+  _globals['_FILERESULTS']._serialized_start=469
+  _globals['_FILERESULTS']._serialized_end=568
+  _globals['_TABLECONFIG']._serialized_start=571
+  _globals['_TABLECONFIG']._serialized_end=873
+  _globals['_TABLEMETADATA']._serialized_start=875
+  _globals['_TABLEMETADATA']._serialized_end=978
+  _globals['_PREPAREDFILE']._serialized_start=981
+  _globals['_PREPAREDFILE']._serialized_end=1211
+  _globals['_SLICEPLAN']._serialized_start=1214
+  _globals['_SLICEPLAN']._serialized_end=1523
+  _globals['_SLICEPLAN_PERCENTSLICE']._serialized_start=1422
+  _globals['_SLICEPLAN_PERCENTSLICE']._serialized_end=1462
+  _globals['_SLICEPLAN_ENTITYKEYSSLICE']._serialized_start=1464
+  _globals['_SLICEPLAN_ENTITYKEYSSLICE']._serialized_end=1514
+  _globals['_UUID']._serialized_start=1525
+  _globals['_UUID']._serialized_end=1569
+  _globals['_SLICEREQUEST']._serialized_start=1572
+  _globals['_SLICEREQUEST']._serialized_end=1859
+  _globals['_SLICEREQUEST_PERCENTSLICE']._serialized_start=1422
+  _globals['_SLICEREQUEST_PERCENTSLICE']._serialized_end=1462
+  _globals['_SLICEREQUEST_ENTITYKEYSSLICE']._serialized_start=1800
+  _globals['_SLICEREQUEST_ENTITYKEYSSLICE']._serialized_end=1850
+  _globals['_ANALYSIS']._serialized_start=1862
+  _globals['_ANALYSIS']._serialized_end=2058
+  _globals['_REQUESTDETAILS']._serialized_start=2060
+  _globals['_REQUESTDETAILS']._serialized_end=2107
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/compute_service_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/compute_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/destinations_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/destinations_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/file_service_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/file_service_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from kaskada.kaskada.v1alpha import common_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_common__pb2
+from kaskada.kaskada.v1alpha import kafka_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_kafka__pb2
+from kaskada.kaskada.v1alpha import pulsar_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_pulsar__pb2
 from kaskada.kaskada.v1alpha import schema_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_schema__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*kaskada/kaskada/v1alpha/file_service.proto\x12\x17kaskada.kaskada.v1alpha\x1a$kaskada/kaskada/v1alpha/common.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\"I\n\x0eSourceMetadata\x12\x37\n\x06schema\x18\x01 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SchemaR\x06schema\"Z\n\x12GetMetadataRequest\x12\x44\n\x0bsource_data\x18\x01 \x01(\x0b\x32#.kaskada.kaskada.v1alpha.SourceDataR\nsourceData\"g\n\x13GetMetadataResponse\x12P\n\x0fsource_metadata\x18\x01 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.SourceMetadataR\x0esourceMetadata\"\xbe\x01\n\x14MergeMetadataRequest\x12M\n\x0etable_metadata\x18\x01 \x01(\x0b\x32&.kaskada.kaskada.v1alpha.TableMetadataR\rtableMetadata\x12W\n\x13new_source_metadata\x18\x02 \x03(\x0b\x32\'.kaskada.kaskada.v1alpha.SourceMetadataR\x11newSourceMetadata\"\x98\x02\n\x15MergeMetadataResponse\x12Z\n\x15merged_table_metadata\x18\x01 \x01(\x0b\x32&.kaskada.kaskada.v1alpha.TableMetadataR\x13mergedTableMetadata\x12n\n\x12new_source_results\x18\x02 \x03(\x0b\x32@.kaskada.kaskada.v1alpha.MergeMetadataResponse.SourceMergeResultR\x10newSourceResults\x1a\x33\n\x11SourceMergeResult\x12\x1e\n\ncompatible\x18\x01 \x01(\x08R\ncompatible2\xe7\x01\n\x0b\x46ileService\x12h\n\x0bGetMetadata\x12+.kaskada.kaskada.v1alpha.GetMetadataRequest\x1a,.kaskada.kaskada.v1alpha.GetMetadataResponse\x12n\n\rMergeMetadata\x12-.kaskada.kaskada.v1alpha.MergeMetadataRequest\x1a..kaskada.kaskada.v1alpha.MergeMetadataResponseB\x80\x02\n\x1b\x63om.kaskada.kaskada.v1alphaB\x10\x46ileServiceProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*kaskada/kaskada/v1alpha/file_service.proto\x12\x17kaskada.kaskada.v1alpha\x1a$kaskada/kaskada/v1alpha/common.proto\x1a#kaskada/kaskada/v1alpha/kafka.proto\x1a$kaskada/kaskada/v1alpha/pulsar.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\"I\n\x0eSourceMetadata\x12\x37\n\x06schema\x18\x01 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SchemaR\x06schema\"\xff\x01\n\x12GetMetadataRequest\x12\x46\n\x0bsource_data\x18\x01 \x01(\x0b\x32#.kaskada.kaskada.v1alpha.SourceDataH\x00R\nsourceData\x12L\n\rpulsar_config\x18\x02 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.PulsarConfigH\x00R\x0cpulsarConfig\x12I\n\x0ckafka_config\x18\x03 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.KafkaConfigH\x00R\x0bkafkaConfigB\x08\n\x06source\"g\n\x13GetMetadataResponse\x12P\n\x0fsource_metadata\x18\x01 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.SourceMetadataR\x0esourceMetadata\"\xbe\x01\n\x14MergeMetadataRequest\x12M\n\x0etable_metadata\x18\x01 \x01(\x0b\x32&.kaskada.kaskada.v1alpha.TableMetadataR\rtableMetadata\x12W\n\x13new_source_metadata\x18\x02 \x03(\x0b\x32\'.kaskada.kaskada.v1alpha.SourceMetadataR\x11newSourceMetadata\"\x98\x02\n\x15MergeMetadataResponse\x12Z\n\x15merged_table_metadata\x18\x01 \x01(\x0b\x32&.kaskada.kaskada.v1alpha.TableMetadataR\x13mergedTableMetadata\x12n\n\x12new_source_results\x18\x02 \x03(\x0b\x32@.kaskada.kaskada.v1alpha.MergeMetadataResponse.SourceMergeResultR\x10newSourceResults\x1a\x33\n\x11SourceMergeResult\x12\x1e\n\ncompatible\x18\x01 \x01(\x08R\ncompatible2\xe7\x01\n\x0b\x46ileService\x12h\n\x0bGetMetadata\x12+.kaskada.kaskada.v1alpha.GetMetadataRequest\x1a,.kaskada.kaskada.v1alpha.GetMetadataResponse\x12n\n\rMergeMetadata\x12-.kaskada.kaskada.v1alpha.MergeMetadataRequest\x1a..kaskada.kaskada.v1alpha.MergeMetadataResponseB\x80\x02\n\x1b\x63om.kaskada.kaskada.v1alphaB\x10\x46ileServiceProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.file_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\020FileServiceProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
-  _globals['_SOURCEMETADATA']._serialized_start=147
-  _globals['_SOURCEMETADATA']._serialized_end=220
-  _globals['_GETMETADATAREQUEST']._serialized_start=222
-  _globals['_GETMETADATAREQUEST']._serialized_end=312
-  _globals['_GETMETADATARESPONSE']._serialized_start=314
-  _globals['_GETMETADATARESPONSE']._serialized_end=417
-  _globals['_MERGEMETADATAREQUEST']._serialized_start=420
-  _globals['_MERGEMETADATAREQUEST']._serialized_end=610
-  _globals['_MERGEMETADATARESPONSE']._serialized_start=613
-  _globals['_MERGEMETADATARESPONSE']._serialized_end=893
-  _globals['_MERGEMETADATARESPONSE_SOURCEMERGERESULT']._serialized_start=842
-  _globals['_MERGEMETADATARESPONSE_SOURCEMERGERESULT']._serialized_end=893
-  _globals['_FILESERVICE']._serialized_start=896
-  _globals['_FILESERVICE']._serialized_end=1127
+  _globals['_SOURCEMETADATA']._serialized_start=222
+  _globals['_SOURCEMETADATA']._serialized_end=295
+  _globals['_GETMETADATAREQUEST']._serialized_start=298
+  _globals['_GETMETADATAREQUEST']._serialized_end=553
+  _globals['_GETMETADATARESPONSE']._serialized_start=555
+  _globals['_GETMETADATARESPONSE']._serialized_end=658
+  _globals['_MERGEMETADATAREQUEST']._serialized_start=661
+  _globals['_MERGEMETADATAREQUEST']._serialized_end=851
+  _globals['_MERGEMETADATARESPONSE']._serialized_start=854
+  _globals['_MERGEMETADATARESPONSE']._serialized_end=1134
+  _globals['_MERGEMETADATARESPONSE_SOURCEMERGERESULT']._serialized_start=1083
+  _globals['_MERGEMETADATARESPONSE_SOURCEMERGERESULT']._serialized_end=1134
+  _globals['_FILESERVICE']._serialized_start=1137
+  _globals['_FILESERVICE']._serialized_end=1368
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/health_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/options_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: kaskada/kaskada/v1alpha/health.proto
+# source: kaskada/kaskada/v1alpha/options.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from grpc.health.v1 import health_pb2 as grpc_dot_health_dot_v1_dot_health__pb2
+from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$kaskada/kaskada/v1alpha/health.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1bgrpc/health/v1/health.protoB\xfb\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\x0bHealthProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%kaskada/kaskada/v1alpha/options.proto\x12\x17kaskada.kaskada.v1alpha\x1a google/protobuf/descriptor.proto:=\n\tsensitive\x12\x1d.google.protobuf.FieldOptions\x18\xd0\x86\x03 \x01(\x08R\tsensitiveB\xfc\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\x0cOptionsProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.health_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.options_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
+  google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(sensitive)
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\013HealthProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
+  DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\014OptionsProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/options_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/spec_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: kaskada/kaskada/v1alpha/options.proto
+# source: kaskada/kaskada/v1alpha/spec.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
+from kaskada.kaskada.v1alpha import materialization_service_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_materialization__service__pb2
+from kaskada.kaskada.v1alpha import query_service_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2
+from kaskada.kaskada.v1alpha import table_service_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_table__service__pb2
+from kaskada.kaskada.v1alpha import view_service_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_view__service__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%kaskada/kaskada/v1alpha/options.proto\x12\x17kaskada.kaskada.v1alpha\x1a google/protobuf/descriptor.proto:=\n\tsensitive\x12\x1d.google.protobuf.FieldOptions\x18\xd0\x86\x03 \x01(\x08R\tsensitiveB\xfc\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\x0cOptionsProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"kaskada/kaskada/v1alpha/spec.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x35kaskada/kaskada/v1alpha/materialization_service.proto\x1a+kaskada/kaskada/v1alpha/query_service.proto\x1a+kaskada/kaskada/v1alpha/table_service.proto\x1a*kaskada/kaskada/v1alpha/view_service.proto\"\x83\x02\n\x04Spec\x12\x36\n\x06tables\x18\x01 \x03(\x0b\x32\x1e.kaskada.kaskada.v1alpha.TableR\x06tables\x12\x33\n\x05views\x18\x02 \x03(\x0b\x32\x1d.kaskada.kaskada.v1alpha.ViewR\x05views\x12\x38\n\x07queries\x18\x03 \x03(\x0b\x32\x1e.kaskada.kaskada.v1alpha.QueryR\x07queries\x12T\n\x10materializations\x18\x04 \x03(\x0b\x32(.kaskada.kaskada.v1alpha.MaterializationR\x10materializationsB\xf9\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\tSpecProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.options_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.spec_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(sensitive)
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\014OptionsProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
+  DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\tSpecProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
+  _globals['_SPEC']._serialized_start=253
+  _globals['_SPEC']._serialized_end=512
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/plan_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/plan_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/pulsar_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/pulsar_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/query_service_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/schema_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/schema_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$kaskada/kaskada/v1alpha/schema.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1bgoogle/protobuf/empty.proto\"\xd0\x08\n\x08\x44\x61taType\x12O\n\tprimitive\x18\x01 \x01(\x0e\x32/.kaskada.kaskada.v1alpha.DataType.PrimitiveTypeH\x00R\tprimitive\x12\x39\n\x06struct\x18\x02 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SchemaH\x00R\x06struct\x12\x30\n\x06window\x18\x03 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00R\x06window\x12\x37\n\x04list\x18\x04 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeH\x00R\x04list\"\xc4\x06\n\rPrimitiveType\x12\x1e\n\x1aPRIMITIVE_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13PRIMITIVE_TYPE_NULL\x10\x01\x12\x17\n\x13PRIMITIVE_TYPE_BOOL\x10\x02\x12\x15\n\x11PRIMITIVE_TYPE_I8\x10\x03\x12\x16\n\x12PRIMITIVE_TYPE_I16\x10\x04\x12\x16\n\x12PRIMITIVE_TYPE_I32\x10\x05\x12\x16\n\x12PRIMITIVE_TYPE_I64\x10\x06\x12\x15\n\x11PRIMITIVE_TYPE_U8\x10\x07\x12\x16\n\x12PRIMITIVE_TYPE_U16\x10\x08\x12\x16\n\x12PRIMITIVE_TYPE_U32\x10\t\x12\x16\n\x12PRIMITIVE_TYPE_U64\x10\n\x12\x16\n\x12PRIMITIVE_TYPE_F16\x10\x0b\x12\x16\n\x12PRIMITIVE_TYPE_F32\x10\x0c\x12\x16\n\x12PRIMITIVE_TYPE_F64\x10\r\x12\x19\n\x15PRIMITIVE_TYPE_STRING\x10\x0e\x12$\n PRIMITIVE_TYPE_INTERVAL_DAY_TIME\x10\x0f\x12&\n\"PRIMITIVE_TYPE_INTERVAL_YEAR_MONTH\x10\x10\x12\"\n\x1ePRIMITIVE_TYPE_DURATION_SECOND\x10\x11\x12\'\n#PRIMITIVE_TYPE_DURATION_MILLISECOND\x10\x12\x12\'\n#PRIMITIVE_TYPE_DURATION_MICROSECOND\x10\x13\x12&\n\"PRIMITIVE_TYPE_DURATION_NANOSECOND\x10\x14\x12#\n\x1fPRIMITIVE_TYPE_TIMESTAMP_SECOND\x10\x15\x12(\n$PRIMITIVE_TYPE_TIMESTAMP_MILLISECOND\x10\x16\x12(\n$PRIMITIVE_TYPE_TIMESTAMP_MICROSECOND\x10\x17\x12\'\n#PRIMITIVE_TYPE_TIMESTAMP_NANOSECOND\x10\x18\x12\x17\n\x13PRIMITIVE_TYPE_JSON\x10\x19\x12\x19\n\x15PRIMITIVE_TYPE_DATE32\x10\x1a\x42\x06\n\x04kind\"\xa4\x01\n\x06Schema\x12=\n\x06\x66ields\x18\x01 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.Schema.FieldR\x06\x66ields\x1a[\n\x05\x46ield\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\tdata_type\x18\x02 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\x08\x64\x61taTypeB\xfb\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\x0bSchemaProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$kaskada/kaskada/v1alpha/schema.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1bgoogle/protobuf/empty.proto\"\x80\n\n\x08\x44\x61taType\x12O\n\tprimitive\x18\x01 \x01(\x0e\x32/.kaskada.kaskada.v1alpha.DataType.PrimitiveTypeH\x00R\tprimitive\x12\x39\n\x06struct\x18\x02 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SchemaH\x00R\x06struct\x12\x30\n\x06window\x18\x03 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00R\x06window\x12\x37\n\x04list\x18\x04 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeH\x00R\x04list\x12\x39\n\x03map\x18\x05 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.DataType.MapH\x00R\x03map\x1as\n\x03Map\x12\x33\n\x03key\x18\x01 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\x03key\x12\x37\n\x05value\x18\x02 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\x05value\"\xc4\x06\n\rPrimitiveType\x12\x1e\n\x1aPRIMITIVE_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13PRIMITIVE_TYPE_NULL\x10\x01\x12\x17\n\x13PRIMITIVE_TYPE_BOOL\x10\x02\x12\x15\n\x11PRIMITIVE_TYPE_I8\x10\x03\x12\x16\n\x12PRIMITIVE_TYPE_I16\x10\x04\x12\x16\n\x12PRIMITIVE_TYPE_I32\x10\x05\x12\x16\n\x12PRIMITIVE_TYPE_I64\x10\x06\x12\x15\n\x11PRIMITIVE_TYPE_U8\x10\x07\x12\x16\n\x12PRIMITIVE_TYPE_U16\x10\x08\x12\x16\n\x12PRIMITIVE_TYPE_U32\x10\t\x12\x16\n\x12PRIMITIVE_TYPE_U64\x10\n\x12\x16\n\x12PRIMITIVE_TYPE_F16\x10\x0b\x12\x16\n\x12PRIMITIVE_TYPE_F32\x10\x0c\x12\x16\n\x12PRIMITIVE_TYPE_F64\x10\r\x12\x19\n\x15PRIMITIVE_TYPE_STRING\x10\x0e\x12$\n PRIMITIVE_TYPE_INTERVAL_DAY_TIME\x10\x0f\x12&\n\"PRIMITIVE_TYPE_INTERVAL_YEAR_MONTH\x10\x10\x12\"\n\x1ePRIMITIVE_TYPE_DURATION_SECOND\x10\x11\x12\'\n#PRIMITIVE_TYPE_DURATION_MILLISECOND\x10\x12\x12\'\n#PRIMITIVE_TYPE_DURATION_MICROSECOND\x10\x13\x12&\n\"PRIMITIVE_TYPE_DURATION_NANOSECOND\x10\x14\x12#\n\x1fPRIMITIVE_TYPE_TIMESTAMP_SECOND\x10\x15\x12(\n$PRIMITIVE_TYPE_TIMESTAMP_MILLISECOND\x10\x16\x12(\n$PRIMITIVE_TYPE_TIMESTAMP_MICROSECOND\x10\x17\x12\'\n#PRIMITIVE_TYPE_TIMESTAMP_NANOSECOND\x10\x18\x12\x17\n\x13PRIMITIVE_TYPE_JSON\x10\x19\x12\x19\n\x15PRIMITIVE_TYPE_DATE32\x10\x1a\x42\x06\n\x04kind\"\xa4\x01\n\x06Schema\x12=\n\x06\x66ields\x18\x01 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.Schema.FieldR\x06\x66ields\x1a[\n\x05\x46ield\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\tdata_type\x18\x02 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\x08\x64\x61taTypeB\xfb\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\x0bSchemaProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.schema_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\013SchemaProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
   _globals['_DATATYPE']._serialized_start=95
-  _globals['_DATATYPE']._serialized_end=1199
-  _globals['_DATATYPE_PRIMITIVETYPE']._serialized_start=355
-  _globals['_DATATYPE_PRIMITIVETYPE']._serialized_end=1191
-  _globals['_SCHEMA']._serialized_start=1202
-  _globals['_SCHEMA']._serialized_end=1366
-  _globals['_SCHEMA_FIELD']._serialized_start=1275
-  _globals['_SCHEMA_FIELD']._serialized_end=1366
+  _globals['_DATATYPE']._serialized_end=1375
+  _globals['_DATATYPE_MAP']._serialized_start=413
+  _globals['_DATATYPE_MAP']._serialized_end=528
+  _globals['_DATATYPE_PRIMITIVETYPE']._serialized_start=531
+  _globals['_DATATYPE_PRIMITIVETYPE']._serialized_end=1367
+  _globals['_SCHEMA']._serialized_start=1378
+  _globals['_SCHEMA']._serialized_end=1542
+  _globals['_SCHEMA_FIELD']._serialized_start=1451
+  _globals['_SCHEMA_FIELD']._serialized_end=1542
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/sources_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/sources_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,26 +7,29 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from kaskada.kaskada.v1alpha import kafka_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_kafka__pb2
 from kaskada.kaskada.v1alpha import pulsar_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_pulsar__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%kaskada/kaskada/v1alpha/sources.proto\x12\x17kaskada.kaskada.v1alpha\x1a$kaskada/kaskada/v1alpha/pulsar.proto\"\x97\x01\n\x06Source\x12\x42\n\x07kaskada\x18\x01 \x01(\x0b\x32&.kaskada.kaskada.v1alpha.KaskadaSourceH\x00R\x07kaskada\x12?\n\x06pulsar\x18\x02 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.PulsarSourceH\x00R\x06pulsarB\x08\n\x06source\"\x0f\n\rKaskadaSource\"M\n\x0cPulsarSource\x12=\n\x06\x63onfig\x18\x01 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.PulsarConfigR\x06\x63onfigB\xfc\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\x0cSourcesProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%kaskada/kaskada/v1alpha/sources.proto\x12\x17kaskada.kaskada.v1alpha\x1a#kaskada/kaskada/v1alpha/kafka.proto\x1a$kaskada/kaskada/v1alpha/pulsar.proto\"\xd5\x01\n\x06Source\x12\x42\n\x07kaskada\x18\x01 \x01(\x0b\x32&.kaskada.kaskada.v1alpha.KaskadaSourceH\x00R\x07kaskada\x12?\n\x06pulsar\x18\x02 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.PulsarSourceH\x00R\x06pulsar\x12<\n\x05kafka\x18\x03 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.KafkaSourceH\x00R\x05kafkaB\x08\n\x06source\"\x0f\n\rKaskadaSource\"M\n\x0cPulsarSource\x12=\n\x06\x63onfig\x18\x01 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.PulsarConfigR\x06\x63onfig\"K\n\x0bKafkaSource\x12<\n\x06\x63onfig\x18\x01 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.KafkaConfigR\x06\x63onfigB\xfc\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\x0cSourcesProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.sources_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\014SourcesProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
-  _globals['_SOURCE']._serialized_start=105
-  _globals['_SOURCE']._serialized_end=256
-  _globals['_KASKADASOURCE']._serialized_start=258
-  _globals['_KASKADASOURCE']._serialized_end=273
-  _globals['_PULSARSOURCE']._serialized_start=275
-  _globals['_PULSARSOURCE']._serialized_end=352
+  _globals['_SOURCE']._serialized_start=142
+  _globals['_SOURCE']._serialized_end=355
+  _globals['_KASKADASOURCE']._serialized_start=357
+  _globals['_KASKADASOURCE']._serialized_end=372
+  _globals['_PULSARSOURCE']._serialized_start=374
+  _globals['_PULSARSOURCE']._serialized_end=451
+  _globals['_KAFKASOURCE']._serialized_start=453
+  _globals['_KAFKASOURCE']._serialized_end=528
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/table_service_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/table_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from kaskada.kaskada.v1alpha import common_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_common__pb2
 from kaskada.kaskada.v1alpha import schema_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_schema__pb2
 from kaskada.kaskada.v1alpha import sources_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_sources__pb2
 from validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+kaskada/kaskada/v1alpha/table_service.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a$kaskada/kaskada/v1alpha/common.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\x1a%kaskada/kaskada/v1alpha/sources.proto\x1a\x17validate/validate.proto\"\xf6\x04\n\x05Table\x12\x1e\n\x08table_id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x07tableId\x12&\n\ntable_name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\ttableName\x12\x31\n\x10time_column_name\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0etimeColumnName\x12<\n\x16\x65ntity_key_column_name\x18\x04 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x13\x65ntityKeyColumnName\x12U\n\x13subsort_column_name\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValueB\x07\xfa\x42\x04r\x02\x10\x01R\x11subsortColumnName\x12\x1f\n\x0bgrouping_id\x18\x06 \x01(\tR\ngroupingId\x12@\n\x0b\x63reate_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\ncreateTime\x12@\n\x0bupdate_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\nupdateTime\x12\x1d\n\x07version\x18\t \x01(\x03\x42\x03\xe0\x41\x03R\x07version\x12<\n\x06schema\x18\n \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SchemaB\x03\xe0\x41\x03R\x06schema\x12\"\n\nfile_count\x18\x0b \x01(\x03\x42\x03\xe0\x41\x03R\tfileCount\x12\x37\n\x06source\x18\x0c \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SourceR\x06source\"s\n\x11ListTablesRequest\x12\x16\n\x06search\x18\x01 \x01(\tR\x06search\x12\'\n\tpage_size\x18\x02 \x01(\x05\x42\n\xfa\x42\x07\x1a\x05\x18\xe8\x07(\x00R\x08pageSize\x12\x1d\n\npage_token\x18\x03 \x01(\tR\tpageToken\"\xc6\x01\n\x12ListTablesResponse\x12\x36\n\x06tables\x18\x01 \x03(\x0b\x32\x1e.kaskada.kaskada.v1alpha.TableR\x06tables\x12&\n\x0fnext_page_token\x18\x02 \x01(\tR\rnextPageToken\x12P\n\x0frequest_details\x18\x03 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.RequestDetailsR\x0erequestDetails\"9\n\x0fGetTableRequest\x12&\n\ntable_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\ttableName\"\x9a\x01\n\x10GetTableResponse\x12\x34\n\x05table\x18\x01 \x01(\x0b\x32\x1e.kaskada.kaskada.v1alpha.TableR\x05table\x12P\n\x0frequest_details\x18\x02 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.RequestDetailsR\x0erequestDetails\"T\n\x12\x43reateTableRequest\x12>\n\x05table\x18\x01 \x01(\x0b\x32\x1e.kaskada.kaskada.v1alpha.TableB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x05table\"\x9d\x01\n\x13\x43reateTableResponse\x12\x34\n\x05table\x18\x01 \x01(\x0b\x32\x1e.kaskada.kaskada.v1alpha.TableR\x05table\x12P\n\x0frequest_details\x18\x02 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.RequestDetailsR\x0erequestDetails\"R\n\x12\x44\x65leteTableRequest\x12&\n\ntable_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\ttableName\x12\x14\n\x05\x66orce\x18\x02 \x01(\x08R\x05\x66orce\"\x8b\x01\n\x13\x44\x65leteTableResponse\x12\"\n\rdata_token_id\x18\x01 \x01(\tR\x0b\x64\x61taTokenId\x12P\n\x0frequest_details\x18\x02 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.RequestDetailsR\x0erequestDetails\"\x92\x01\n\x0fLoadDataRequest\x12&\n\ntable_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\ttableName\x12\x43\n\nfile_input\x18\x02 \x01(\x0b\x32\".kaskada.kaskada.v1alpha.FileInputH\x00R\tfileInputB\x12\n\x0bsource_data\x12\x03\xf8\x42\x01\"\x88\x01\n\x10LoadDataResponse\x12\"\n\rdata_token_id\x18\x01 \x01(\tR\x0b\x64\x61taTokenId\x12P\n\x0frequest_details\x18\x02 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.RequestDetailsR\x0erequestDetails2\xbe\x05\n\x0cTableService\x12~\n\nListTables\x12*.kaskada.kaskada.v1alpha.ListTablesRequest\x1a+.kaskada.kaskada.v1alpha.ListTablesResponse\"\x17\x82\xd3\xe4\x93\x02\x11\x12\x0f/v1alpha/tables\x12\x87\x01\n\x08GetTable\x12(.kaskada.kaskada.v1alpha.GetTableRequest\x1a).kaskada.kaskada.v1alpha.GetTableResponse\"&\x82\xd3\xe4\x93\x02 \x12\x1e/v1alpha/tables/{table_name=*}\x12\x88\x01\n\x0b\x43reateTable\x12+.kaskada.kaskada.v1alpha.CreateTableRequest\x1a,.kaskada.kaskada.v1alpha.CreateTableResponse\"\x1e\x82\xd3\xe4\x93\x02\x18:\x05table\"\x0f/v1alpha/tables\x12\x90\x01\n\x0b\x44\x65leteTable\x12+.kaskada.kaskada.v1alpha.DeleteTableRequest\x1a,.kaskada.kaskada.v1alpha.DeleteTableResponse\"&\x82\xd3\xe4\x93\x02 *\x1e/v1alpha/tables/{table_name=*}\x12\x85\x01\n\x08LoadData\x12(.kaskada.kaskada.v1alpha.LoadDataRequest\x1a).kaskada.kaskada.v1alpha.LoadDataResponse\"$\x82\xd3\xe4\x93\x02\x1e:\x01*\"\x19/v1alpha/tables/load_dataB\x81\x02\n\x1b\x63om.kaskada.kaskada.v1alphaB\x11TableServiceProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+kaskada/kaskada/v1alpha/table_service.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a$kaskada/kaskada/v1alpha/common.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\x1a%kaskada/kaskada/v1alpha/sources.proto\x1a\x17validate/validate.proto\"\xf6\x04\n\x05Table\x12\x1e\n\x08table_id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x07tableId\x12&\n\ntable_name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\ttableName\x12\x31\n\x10time_column_name\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0etimeColumnName\x12<\n\x16\x65ntity_key_column_name\x18\x04 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x13\x65ntityKeyColumnName\x12U\n\x13subsort_column_name\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValueB\x07\xfa\x42\x04r\x02\x10\x01R\x11subsortColumnName\x12\x1f\n\x0bgrouping_id\x18\x06 \x01(\tR\ngroupingId\x12@\n\x0b\x63reate_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\ncreateTime\x12@\n\x0bupdate_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\nupdateTime\x12\x1d\n\x07version\x18\t \x01(\x03\x42\x03\xe0\x41\x03R\x07version\x12<\n\x06schema\x18\n \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SchemaB\x03\xe0\x41\x03R\x06schema\x12\"\n\nfile_count\x18\x0b \x01(\x03\x42\x03\xe0\x41\x03R\tfileCount\x12\x37\n\x06source\x18\x0c \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SourceR\x06source\"s\n\x11ListTablesRequest\x12\x16\n\x06search\x18\x01 \x01(\tR\x06search\x12\'\n\tpage_size\x18\x02 \x01(\x05\x42\n\xfa\x42\x07\x1a\x05\x18\xe8\x07(\x00R\x08pageSize\x12\x1d\n\npage_token\x18\x03 \x01(\tR\tpageToken\"\xc6\x01\n\x12ListTablesResponse\x12\x36\n\x06tables\x18\x01 \x03(\x0b\x32\x1e.kaskada.kaskada.v1alpha.TableR\x06tables\x12&\n\x0fnext_page_token\x18\x02 \x01(\tR\rnextPageToken\x12P\n\x0frequest_details\x18\x03 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.RequestDetailsR\x0erequestDetails\"9\n\x0fGetTableRequest\x12&\n\ntable_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\ttableName\"\x9a\x01\n\x10GetTableResponse\x12\x34\n\x05table\x18\x01 \x01(\x0b\x32\x1e.kaskada.kaskada.v1alpha.TableR\x05table\x12P\n\x0frequest_details\x18\x02 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.RequestDetailsR\x0erequestDetails\"T\n\x12\x43reateTableRequest\x12>\n\x05table\x18\x01 \x01(\x0b\x32\x1e.kaskada.kaskada.v1alpha.TableB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x05table\"\x9d\x01\n\x13\x43reateTableResponse\x12\x34\n\x05table\x18\x01 \x01(\x0b\x32\x1e.kaskada.kaskada.v1alpha.TableR\x05table\x12P\n\x0frequest_details\x18\x02 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.RequestDetailsR\x0erequestDetails\"R\n\x12\x44\x65leteTableRequest\x12&\n\ntable_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\ttableName\x12\x14\n\x05\x66orce\x18\x02 \x01(\x08R\x05\x66orce\"\x8b\x01\n\x13\x44\x65leteTableResponse\x12\"\n\rdata_token_id\x18\x01 \x01(\tR\x0b\x64\x61taTokenId\x12P\n\x0frequest_details\x18\x02 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.RequestDetailsR\x0erequestDetails\"\xc0\x01\n\x0fLoadDataRequest\x12&\n\ntable_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\ttableName\x12\x43\n\nfile_input\x18\x02 \x01(\x0b\x32\".kaskada.kaskada.v1alpha.FileInputH\x00R\tfileInput\x12,\n\x12\x63opy_to_filesystem\x18\x03 \x01(\x08R\x10\x63opyToFilesystemB\x12\n\x0bsource_data\x12\x03\xf8\x42\x01\"\x88\x01\n\x10LoadDataResponse\x12\"\n\rdata_token_id\x18\x01 \x01(\tR\x0b\x64\x61taTokenId\x12P\n\x0frequest_details\x18\x02 \x01(\x0b\x32\'.kaskada.kaskada.v1alpha.RequestDetailsR\x0erequestDetails2\xbe\x05\n\x0cTableService\x12~\n\nListTables\x12*.kaskada.kaskada.v1alpha.ListTablesRequest\x1a+.kaskada.kaskada.v1alpha.ListTablesResponse\"\x17\x82\xd3\xe4\x93\x02\x11\x12\x0f/v1alpha/tables\x12\x87\x01\n\x08GetTable\x12(.kaskada.kaskada.v1alpha.GetTableRequest\x1a).kaskada.kaskada.v1alpha.GetTableResponse\"&\x82\xd3\xe4\x93\x02 \x12\x1e/v1alpha/tables/{table_name=*}\x12\x88\x01\n\x0b\x43reateTable\x12+.kaskada.kaskada.v1alpha.CreateTableRequest\x1a,.kaskada.kaskada.v1alpha.CreateTableResponse\"\x1e\x82\xd3\xe4\x93\x02\x18:\x05table\"\x0f/v1alpha/tables\x12\x90\x01\n\x0b\x44\x65leteTable\x12+.kaskada.kaskada.v1alpha.DeleteTableRequest\x1a,.kaskada.kaskada.v1alpha.DeleteTableResponse\"&\x82\xd3\xe4\x93\x02 *\x1e/v1alpha/tables/{table_name=*}\x12\x85\x01\n\x08LoadData\x12(.kaskada.kaskada.v1alpha.LoadDataRequest\x1a).kaskada.kaskada.v1alpha.LoadDataResponse\"$\x82\xd3\xe4\x93\x02\x1e:\x01*\"\x19/v1alpha/tables/load_dataB\x81\x02\n\x1b\x63om.kaskada.kaskada.v1alphaB\x11TableServiceProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.table_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -87,13 +87,13 @@
   _globals['_CREATETABLERESPONSE']._serialized_start=1594
   _globals['_CREATETABLERESPONSE']._serialized_end=1751
   _globals['_DELETETABLEREQUEST']._serialized_start=1753
   _globals['_DELETETABLEREQUEST']._serialized_end=1835
   _globals['_DELETETABLERESPONSE']._serialized_start=1838
   _globals['_DELETETABLERESPONSE']._serialized_end=1977
   _globals['_LOADDATAREQUEST']._serialized_start=1980
-  _globals['_LOADDATAREQUEST']._serialized_end=2126
-  _globals['_LOADDATARESPONSE']._serialized_start=2129
-  _globals['_LOADDATARESPONSE']._serialized_end=2265
-  _globals['_TABLESERVICE']._serialized_start=2268
-  _globals['_TABLESERVICE']._serialized_end=2970
+  _globals['_LOADDATAREQUEST']._serialized_end=2172
+  _globals['_LOADDATARESPONSE']._serialized_start=2175
+  _globals['_LOADDATARESPONSE']._serialized_end=2311
+  _globals['_TABLESERVICE']._serialized_start=2314
+  _globals['_TABLESERVICE']._serialized_end=3016
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/test_cases_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/test_cases_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/view_service_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/view_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py` & `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v2alpha/query_service_pb2.py` & `kaskada-0.5.0/src/kaskada/kaskada/v2alpha/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py` & `kaskada-0.5.0/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/materialization.py` & `kaskada-0.5.0/src/kaskada/materialization.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/query.py` & `kaskada-0.5.0/src/kaskada/query.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/slice_filters.py` & `kaskada-0.5.0/src/kaskada/slice_filters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/table.py` & `kaskada-0.5.0/src/kaskada/table.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/utils.py` & `kaskada-0.5.0/src/kaskada/utils.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/src/kaskada/view.py` & `kaskada-0.5.0/src/kaskada/view.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/vendor/validate/validate.proto` & `kaskada-0.5.0/vendor/validate/validate.proto`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/vendor/validate/validate_pb2.py` & `kaskada-0.5.0/vendor/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/vendor/validate/validate_pb2.pyi` & `kaskada-0.5.0/vendor/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `kaskada-0.4.1/setup.py` & `kaskada-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  'pyarrow>=10.0.1,<11.0.0',
  'pygithub>=1.57,<2.0',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'kaskada',
-    'version': '0.4.1',
+    'version': '0.5.0',
     'description': 'A client library for the Kaskada time travel machine learning service',
     'long_description': '# Kaskada SDK\n\n## Developer Instructions\nThe package uses Poetry to develop and build.\n\n1. Install Pyenv [Pyenv Documentation](https://github.com/pyenv/pyenv)\n1. Install Python 3.9.16: `$ pyenv install 3.9.16`\n1. Install Poetry [Poetry Documentation](https://python-poetry.org/docs/)\n1. Install dependences: `$ poetry install`\n\n### Run tasks\nThe package uses [`poethepoet`](https://github.com/nat-n/poethepoet) for running tasks\n\n#### Test Task\nTo run tests: `$ poetry run poe test` \n\n#### Check Style Task\nTo check the style: `$ poetry run poe style`\n\n#### Format Task\nTo auto-format (isort + black): `$ poetry run poe format`\n\n#### Check Static Type Task\nTo perform static type analysis (mypy): `$ poetry run poe types`\n\n#### Lint Task\nTo run the linter (pylint): `$ poetry run poe lint`\n\n#### Generate documentation \nWe use Sphinx and rely on autogeneration extensions within Sphinx to read docstrings and \ngenerate an HTML formatted version of the codes documentation. \n\n* `poetry run poe docs` : generates and builds the docs \n* `poetry run poe docs-generate` : generates the docs (.rst files)\n* `poetry run poe docs-build` : builds the HTML rendered version of the generated docs (from .rst to .html)\n\nThe generated HTML is located inside `docs/build`. Load `docs/build/index.html` in your browser to see the HTML rendered output. \n\n## Using the Client from Jupyter\n\n#### Install Jupyter\nTo install Jupyter: `$ pip install notebook`\n\n#### Build the Client\nTo build the client: `$ poetry build`\n\n#### Install the Client\nTo install the client: `$ pip install dist/*.whl`\n\n#### Open a Jupyter Notebook\nTo open a notebook: `$ jupyter notebook`\n',
     'author': 'Kaskada',
     'author_email': 'maintainers@kaskada.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kaskada-0.4.1/PKG-INFO` & `kaskada-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaskada
-Version: 0.4.1
+Version: 0.5.0
 Summary: A client library for the Kaskada time travel machine learning service
 License: Apache-2.0
 Author: Kaskada
 Author-email: maintainers@kaskada.io
 Requires-Python: >=3.8.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

