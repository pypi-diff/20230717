# Comparing `tmp/doublecloud-0.7.0.tar.gz` & `tmp/doublecloud-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doublecloud-0.7.0.tar", last modified: Tue Jun 27 12:39:30 2023, max compression
+gzip compressed data, was "doublecloud-0.8.0.tar", last modified: Mon Jul 17 14:38:17 2023, max compression
```

## Comparing `doublecloud-0.7.0.tar` & `doublecloud-0.8.0.tar`

### file list

```diff
@@ -1,225 +1,225 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.215382 doublecloud-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 12:38:54.000000 doublecloud-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-27 12:39:30.215382 doublecloud-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-27 12:38:54.000000 doublecloud-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.175380 doublecloud-0.7.0/doublecloud/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_auth_fabric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_auth_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_backoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_operation_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_retry_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.179380 doublecloud-0.7.0/doublecloud/_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.179380 doublecloud-0.7.0/doublecloud/_wrappers/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_wrappers/clickhouse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.179380 doublecloud-0.7.0/doublecloud/_wrappers/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/_wrappers/kafka/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.179380 doublecloud-0.7.0/doublecloud/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.183380 doublecloud-0.7.0/doublecloud/clickhouse/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24545 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16265 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    27580 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/operation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/operation_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/version_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/version_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/version_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/version_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/version_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/clickhouse/v1/version_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.183380 doublecloud-0.7.0/doublecloud/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.191381 doublecloud-0.7.0/doublecloud/kafka/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/cluster_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/cluster_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/cluster_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/cluster_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20537 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/cluster_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/connector_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/connector_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/connector_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/connector_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/connector_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/connector_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/operation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/operation_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/topic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/topic_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/topic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/topic_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/topic_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/topic_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/user_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/user_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/user_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/version_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/version_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/version_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/version_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/version_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/kafka/v1/version_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.191381 doublecloud-0.7.0/doublecloud/network/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.191381 doublecloud-0.7.0/doublecloud/network/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_connection_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_connection_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_connection_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_connection_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_connection_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_connection_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/network_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/operation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/operation_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/network/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.191381 doublecloud-0.7.0/doublecloud/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.195381 doublecloud-0.7.0/doublecloud/transfer/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.199381 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.207381 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24164 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/kafka_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/kafka_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/kafka_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mongo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mongo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mongo_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mysql_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mysql_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mysql_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/parsers_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/parsers_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/parsers_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/postgres_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/postgres_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/postgres_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/serializers_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/serializers_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/serializers_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/operation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/operation_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/transfer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/transfer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/transfer_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/transfer_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/transfer_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19365 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/transfer/v1/transfer_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.207381 doublecloud-0.7.0/doublecloud/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/cluster_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/cluster_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/maintenance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/maintenance_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/maintenance_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/operation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/operation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/operation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/paging_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/paging_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/v1/paging_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.207381 doublecloud-0.7.0/doublecloud/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.215382 doublecloud-0.7.0/doublecloud/visualization/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/visualization/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/visualization/v1/workbook_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/visualization/v1/workbook_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/visualization/v1/workbook_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/visualization/v1/workbook_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/visualization/v1/workbook_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-06-27 12:38:54.000000 doublecloud-0.7.0/doublecloud/visualization/v1/workbook_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:39:30.179380 doublecloud-0.7.0/doublecloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-27 12:39:30.000000 doublecloud-0.7.0/doublecloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-06-27 12:39:30.000000 doublecloud-0.7.0/doublecloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:39:30.000000 doublecloud-0.7.0/doublecloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:39:30.000000 doublecloud-0.7.0/doublecloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-27 12:39:30.000000 doublecloud-0.7.0/doublecloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 12:39:30.000000 doublecloud-0.7.0/doublecloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-27 12:38:54.000000 doublecloud-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:39:30.215382 doublecloud-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-27 12:39:25.000000 doublecloud-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.756037 doublecloud-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 14:37:43.000000 doublecloud-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-17 14:38:17.756037 doublecloud-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-17 14:37:43.000000 doublecloud-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.728036 doublecloud-0.8.0/doublecloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/_auth_fabric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/_auth_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/_backoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/_consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/_operation_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/_retry_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.728036 doublecloud-0.8.0/doublecloud/_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/_wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.728036 doublecloud-0.8.0/doublecloud/_wrappers/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/_wrappers/clickhouse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.728036 doublecloud-0.8.0/doublecloud/_wrappers/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/_wrappers/kafka/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.728036 doublecloud-0.8.0/doublecloud/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.732036 doublecloud-0.8.0/doublecloud/clickhouse/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/backup_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/backup_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/backup_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/backup_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/backup_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/backup_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/cluster_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/cluster_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/cluster_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24545 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/cluster_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16265 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27580 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/operation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/operation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/version_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/version_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/version_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/version_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/version_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/clickhouse/v1/version_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.732036 doublecloud-0.8.0/doublecloud/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.736036 doublecloud-0.8.0/doublecloud/kafka/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/cluster_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/cluster_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/cluster_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20537 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/cluster_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/connector_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/connector_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/connector_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/connector_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/connector_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/connector_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/operation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/operation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/topic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/topic_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/topic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/topic_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/topic_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/topic_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/user_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/user_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/user_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/version_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/version_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/version_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/version_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/version_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/kafka/v1/version_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.736036 doublecloud-0.8.0/doublecloud/network/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.736036 doublecloud-0.8.0/doublecloud/network/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/network/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/network/v1/network_connection_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/network/v1/network_connection_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/network/v1/network_connection_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/network/v1/network_connection_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/network/v1/network_connection_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/network/v1/network_connection_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/network/v1/network_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/network/v1/network_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/network/v1/network_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/network/v1/network_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/network/v1/network_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/network/v1/network_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/network/v1/operation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/network/v1/operation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/network/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.736036 doublecloud-0.8.0/doublecloud/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.736036 doublecloud-0.8.0/doublecloud/transfer/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.740037 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.752037 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24164 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/kafka_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/kafka_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/kafka_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/mongo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/mongo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/mongo_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/mysql_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/mysql_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/mysql_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/parsers_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/parsers_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/parsers_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/postgres_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/postgres_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/postgres_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/serializers_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/serializers_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/serializers_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/endpoint_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/operation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/operation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/transfer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/transfer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/transfer_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/transfer_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/transfer_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19365 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/transfer/v1/transfer_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.756037 doublecloud-0.8.0/doublecloud/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/v1/cluster_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/v1/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/v1/maintenance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/v1/maintenance_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/v1/maintenance_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/v1/operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/v1/operation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/v1/operation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/v1/paging_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/v1/paging_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/v1/paging_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.756037 doublecloud-0.8.0/doublecloud/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.756037 doublecloud-0.8.0/doublecloud/visualization/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/visualization/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/visualization/v1/workbook_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/visualization/v1/workbook_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/visualization/v1/workbook_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/visualization/v1/workbook_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/visualization/v1/workbook_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-07-17 14:37:43.000000 doublecloud-0.8.0/doublecloud/visualization/v1/workbook_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:38:17.728036 doublecloud-0.8.0/doublecloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-17 14:38:17.000000 doublecloud-0.8.0/doublecloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-07-17 14:38:17.000000 doublecloud-0.8.0/doublecloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:38:17.000000 doublecloud-0.8.0/doublecloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:38:17.000000 doublecloud-0.8.0/doublecloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-17 14:38:17.000000 doublecloud-0.8.0/doublecloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 14:38:17.000000 doublecloud-0.8.0/doublecloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-17 14:37:43.000000 doublecloud-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:38:17.756037 doublecloud-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-17 14:38:13.000000 doublecloud-0.8.0/setup.py
```

### Comparing `doublecloud-0.7.0/LICENSE` & `doublecloud-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/PKG-INFO` & `doublecloud-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doublecloud
-Version: 0.7.0
+Version: 0.8.0
 Summary: The Double.Cloud official SDK
 Home-page: https://github.com/doublecloud/python-sdk
 Author: DoubleCloud GmbH
 Author-email: support@double.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doublecloud-0.7.0/README.md` & `doublecloud-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/_auth_fabric.py` & `doublecloud-0.8.0/doublecloud/_auth_fabric.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/_auth_plugin.py` & `doublecloud-0.8.0/doublecloud/_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/_backoff.py` & `doublecloud-0.8.0/doublecloud/_backoff.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/_channels.py` & `doublecloud-0.8.0/doublecloud/_channels.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/_operation_waiter.py` & `doublecloud-0.8.0/doublecloud/_operation_waiter.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/_retry_interceptor.py` & `doublecloud-0.8.0/doublecloud/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/_sdk.py` & `doublecloud-0.8.0/doublecloud/_sdk.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_pb2.py` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/backup_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_pb2.pyi` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/backup_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_service_pb2.py` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/backup_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_service_pb2.pyi` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/backup_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/backup_service_pb2_grpc.py` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/backup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_pb2.py` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_pb2.pyi` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_service_pb2.py` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/cluster_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_service_pb2.pyi` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/cluster_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/cluster_service_pb2_grpc.py` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/config_pb2.py` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/config_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/config_pb2.pyi` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/operation_service_pb2.py` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/operation_service_pb2.pyi` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/operation_service_pb2_grpc.py` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/version_pb2.py` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/version_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/version_pb2.pyi` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/version_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/version_service_pb2.py` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/version_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/version_service_pb2.pyi` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/version_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/clickhouse/v1/version_service_pb2_grpc.py` & `doublecloud-0.8.0/doublecloud/clickhouse/v1/version_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/cluster_pb2.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/cluster_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from doublecloud.v1 import cluster_pb2 as doublecloud_dot_v1_dot_cluster__pb2
 from doublecloud.v1 import maintenance_pb2 as doublecloud_dot_v1_dot_maintenance__pb2
 from doublecloud.kafka.v1 import config_pb2 as doublecloud_dot_kafka_dot_v1_dot_config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"doublecloud/kafka/v1/cluster.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1c\x64oublecloud/v1/cluster.proto\x1a doublecloud/v1/maintenance.proto\x1a!doublecloud/kafka/v1/config.proto\"\x8c\t\n\x07\x43luster\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x03 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x04 \x01(\tR\x08regionId\x12;\n\x0b\x63reate_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12\x12\n\x04name\x18\x06 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x07 \x01(\tR\x0b\x64\x65scription\x12\x35\n\x06status\x18\x08 \x01(\x0e\x32\x1d.doublecloud.v1.ClusterStatusR\x06status\x12\x18\n\x07version\x18\t \x01(\tR\x07version\x12\x44\n\tresources\x18\n \x01(\x0b\x32&.doublecloud.kafka.v1.ClusterResourcesR\tresources\x12M\n\x0f\x63onnection_info\x18\x0b \x01(\x0b\x32$.doublecloud.kafka.v1.ConnectionInfoR\x0e\x63onnectionInfo\x12.\n\x06\x61\x63\x63\x65ss\x18\x0c \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12>\n\nencryption\x18\r \x01(\x0b\x32\x1e.doublecloud.v1.DataEncryptionR\nencryption\x12\x1d\n\nnetwork_id\x18\x0e \x01(\tR\tnetworkId\x12\x63\n\x17private_connection_info\x18\x0f \x01(\x0b\x32+.doublecloud.kafka.v1.PrivateConnectionInfoR\x15privateConnectionInfo\x12P\n\x12maintenance_window\x18\x10 \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\x12Q\n\x11planned_operation\x18\x11 \x01(\x0b\x32$.doublecloud.v1.MaintenanceOperationR\x10plannedOperation\x12\x44\n\x0ckafka_config\x18\x12 \x01(\x0b\x32!.doublecloud.kafka.v1.KafkaConfigR\x0bkafkaConfig\x12|\n metrics_exporter_connection_info\x18\x13 \x01(\x0b\x32\x33.doublecloud.kafka.v1.MetricsExporterConnectionInfoR\x1dmetricsExporterConnectionInfo\x12`\n\x16schema_registry_config\x18\x14 \x01(\x0b\x32*.doublecloud.kafka.v1.SchemaRegistryConfigR\x14schemaRegistryConfig\"\xc4\x02\n\x10\x43lusterResources\x12\x42\n\x05kafka\x18\x01 \x01(\x0b\x32,.doublecloud.kafka.v1.ClusterResources.KafkaR\x05kafka\x1a\xeb\x01\n\x05Kafka\x12,\n\x12resource_preset_id\x18\x01 \x01(\tR\x10resourcePresetId\x12\x38\n\tdisk_size\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x08\x64iskSize\x12>\n\x0c\x62roker_count\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0b\x62rokerCount\x12:\n\nzone_count\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\tzoneCount\"m\n\x0e\x43onnectionInfo\x12+\n\x11\x63onnection_string\x18\x01 \x01(\tR\x10\x63onnectionString\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\"t\n\x15PrivateConnectionInfo\x12+\n\x11\x63onnection_string\x18\x01 \x01(\tR\x10\x63onnectionString\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\"O\n\x1dMetricsExporterConnectionInfo\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\"m\n\x04Host\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ncluster_id\x18\x02 \x01(\tR\tclusterId\x12\x32\n\x06status\x18\x03 \x01(\x0e\x32\x1a.doublecloud.v1.HostStatusR\x06statusB?Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafkab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"doublecloud/kafka/v1/cluster.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1c\x64oublecloud/v1/cluster.proto\x1a doublecloud/v1/maintenance.proto\x1a!doublecloud/kafka/v1/config.proto\"\xd9\t\n\x07\x43luster\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x03 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x04 \x01(\tR\x08regionId\x12;\n\x0b\x63reate_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12\x12\n\x04name\x18\x06 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x07 \x01(\tR\x0b\x64\x65scription\x12\x35\n\x06status\x18\x08 \x01(\x0e\x32\x1d.doublecloud.v1.ClusterStatusR\x06status\x12\x18\n\x07version\x18\t \x01(\tR\x07version\x12\x44\n\tresources\x18\n \x01(\x0b\x32&.doublecloud.kafka.v1.ClusterResourcesR\tresources\x12M\n\x0f\x63onnection_info\x18\x0b \x01(\x0b\x32$.doublecloud.kafka.v1.ConnectionInfoR\x0e\x63onnectionInfo\x12.\n\x06\x61\x63\x63\x65ss\x18\x0c \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12>\n\nencryption\x18\r \x01(\x0b\x32\x1e.doublecloud.v1.DataEncryptionR\nencryption\x12\x1d\n\nnetwork_id\x18\x0e \x01(\tR\tnetworkId\x12\x63\n\x17private_connection_info\x18\x0f \x01(\x0b\x32+.doublecloud.kafka.v1.PrivateConnectionInfoR\x15privateConnectionInfo\x12P\n\x12maintenance_window\x18\x10 \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\x12Q\n\x11planned_operation\x18\x11 \x01(\x0b\x32$.doublecloud.v1.MaintenanceOperationR\x10plannedOperation\x12\x44\n\x0ckafka_config\x18\x12 \x01(\x0b\x32!.doublecloud.kafka.v1.KafkaConfigR\x0bkafkaConfig\x12|\n metrics_exporter_connection_info\x18\x13 \x01(\x0b\x32\x33.doublecloud.kafka.v1.MetricsExporterConnectionInfoR\x1dmetricsExporterConnectionInfo\x12`\n\x16schema_registry_config\x18\x14 \x01(\x0b\x32*.doublecloud.kafka.v1.SchemaRegistryConfigR\x14schemaRegistryConfig\x12K\n\x0frest_api_config\x18\x15 \x01(\x0b\x32#.doublecloud.kafka.v1.RestAPIConfigR\rrestApiConfig\"\xc4\x02\n\x10\x43lusterResources\x12\x42\n\x05kafka\x18\x01 \x01(\x0b\x32,.doublecloud.kafka.v1.ClusterResources.KafkaR\x05kafka\x1a\xeb\x01\n\x05Kafka\x12,\n\x12resource_preset_id\x18\x01 \x01(\tR\x10resourcePresetId\x12\x38\n\tdisk_size\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x08\x64iskSize\x12>\n\x0c\x62roker_count\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0b\x62rokerCount\x12:\n\nzone_count\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\tzoneCount\"m\n\x0e\x43onnectionInfo\x12+\n\x11\x63onnection_string\x18\x01 \x01(\tR\x10\x63onnectionString\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\"t\n\x15PrivateConnectionInfo\x12+\n\x11\x63onnection_string\x18\x01 \x01(\tR\x10\x63onnectionString\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\"O\n\x1dMetricsExporterConnectionInfo\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\"m\n\x04Host\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ncluster_id\x18\x02 \x01(\tR\tclusterId\x12\x32\n\x06status\x18\x03 \x01(\x0e\x32\x1a.doublecloud.v1.HostStatusR\x06statusB?Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafkab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.kafka.v1.cluster_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafka'
   _globals['_CLUSTER']._serialized_start=225
-  _globals['_CLUSTER']._serialized_end=1389
-  _globals['_CLUSTERRESOURCES']._serialized_start=1392
-  _globals['_CLUSTERRESOURCES']._serialized_end=1716
-  _globals['_CLUSTERRESOURCES_KAFKA']._serialized_start=1481
-  _globals['_CLUSTERRESOURCES_KAFKA']._serialized_end=1716
-  _globals['_CONNECTIONINFO']._serialized_start=1718
-  _globals['_CONNECTIONINFO']._serialized_end=1827
-  _globals['_PRIVATECONNECTIONINFO']._serialized_start=1829
-  _globals['_PRIVATECONNECTIONINFO']._serialized_end=1945
-  _globals['_METRICSEXPORTERCONNECTIONINFO']._serialized_start=1947
-  _globals['_METRICSEXPORTERCONNECTIONINFO']._serialized_end=2026
-  _globals['_HOST']._serialized_start=2028
-  _globals['_HOST']._serialized_end=2137
+  _globals['_CLUSTER']._serialized_end=1466
+  _globals['_CLUSTERRESOURCES']._serialized_start=1469
+  _globals['_CLUSTERRESOURCES']._serialized_end=1793
+  _globals['_CLUSTERRESOURCES_KAFKA']._serialized_start=1558
+  _globals['_CLUSTERRESOURCES_KAFKA']._serialized_end=1793
+  _globals['_CONNECTIONINFO']._serialized_start=1795
+  _globals['_CONNECTIONINFO']._serialized_end=1904
+  _globals['_PRIVATECONNECTIONINFO']._serialized_start=1906
+  _globals['_PRIVATECONNECTIONINFO']._serialized_end=2022
+  _globals['_METRICSEXPORTERCONNECTIONINFO']._serialized_start=2024
+  _globals['_METRICSEXPORTERCONNECTIONINFO']._serialized_end=2103
+  _globals['_HOST']._serialized_start=2105
+  _globals['_HOST']._serialized_end=2214
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/cluster_pb2.pyi` & `doublecloud-0.8.0/doublecloud/kafka/v1/cluster_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Cluster(_message.Message):
-    __slots__ = ["id", "project_id", "cloud_type", "region_id", "create_time", "name", "description", "status", "version", "resources", "connection_info", "access", "encryption", "network_id", "private_connection_info", "maintenance_window", "planned_operation", "kafka_config", "metrics_exporter_connection_info", "schema_registry_config"]
+    __slots__ = ["id", "project_id", "cloud_type", "region_id", "create_time", "name", "description", "status", "version", "resources", "connection_info", "access", "encryption", "network_id", "private_connection_info", "maintenance_window", "planned_operation", "kafka_config", "metrics_exporter_connection_info", "schema_registry_config", "rest_api_config"]
     ID_FIELD_NUMBER: _ClassVar[int]
     PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     CLOUD_TYPE_FIELD_NUMBER: _ClassVar[int]
     REGION_ID_FIELD_NUMBER: _ClassVar[int]
     CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
@@ -27,14 +27,15 @@
     NETWORK_ID_FIELD_NUMBER: _ClassVar[int]
     PRIVATE_CONNECTION_INFO_FIELD_NUMBER: _ClassVar[int]
     MAINTENANCE_WINDOW_FIELD_NUMBER: _ClassVar[int]
     PLANNED_OPERATION_FIELD_NUMBER: _ClassVar[int]
     KAFKA_CONFIG_FIELD_NUMBER: _ClassVar[int]
     METRICS_EXPORTER_CONNECTION_INFO_FIELD_NUMBER: _ClassVar[int]
     SCHEMA_REGISTRY_CONFIG_FIELD_NUMBER: _ClassVar[int]
+    REST_API_CONFIG_FIELD_NUMBER: _ClassVar[int]
     id: str
     project_id: str
     cloud_type: str
     region_id: str
     create_time: _timestamp_pb2.Timestamp
     name: str
     description: str
@@ -47,15 +48,16 @@
     network_id: str
     private_connection_info: PrivateConnectionInfo
     maintenance_window: _maintenance_pb2.MaintenanceWindow
     planned_operation: _maintenance_pb2.MaintenanceOperation
     kafka_config: _config_pb2.KafkaConfig
     metrics_exporter_connection_info: MetricsExporterConnectionInfo
     schema_registry_config: _config_pb2.SchemaRegistryConfig
-    def __init__(self, id: _Optional[str] = ..., project_id: _Optional[str] = ..., cloud_type: _Optional[str] = ..., region_id: _Optional[str] = ..., create_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., status: _Optional[_Union[_cluster_pb2.ClusterStatus, str]] = ..., version: _Optional[str] = ..., resources: _Optional[_Union[ClusterResources, _Mapping]] = ..., connection_info: _Optional[_Union[ConnectionInfo, _Mapping]] = ..., access: _Optional[_Union[_cluster_pb2.Access, _Mapping]] = ..., encryption: _Optional[_Union[_cluster_pb2.DataEncryption, _Mapping]] = ..., network_id: _Optional[str] = ..., private_connection_info: _Optional[_Union[PrivateConnectionInfo, _Mapping]] = ..., maintenance_window: _Optional[_Union[_maintenance_pb2.MaintenanceWindow, _Mapping]] = ..., planned_operation: _Optional[_Union[_maintenance_pb2.MaintenanceOperation, _Mapping]] = ..., kafka_config: _Optional[_Union[_config_pb2.KafkaConfig, _Mapping]] = ..., metrics_exporter_connection_info: _Optional[_Union[MetricsExporterConnectionInfo, _Mapping]] = ..., schema_registry_config: _Optional[_Union[_config_pb2.SchemaRegistryConfig, _Mapping]] = ...) -> None: ...
+    rest_api_config: _config_pb2.RestAPIConfig
+    def __init__(self, id: _Optional[str] = ..., project_id: _Optional[str] = ..., cloud_type: _Optional[str] = ..., region_id: _Optional[str] = ..., create_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., status: _Optional[_Union[_cluster_pb2.ClusterStatus, str]] = ..., version: _Optional[str] = ..., resources: _Optional[_Union[ClusterResources, _Mapping]] = ..., connection_info: _Optional[_Union[ConnectionInfo, _Mapping]] = ..., access: _Optional[_Union[_cluster_pb2.Access, _Mapping]] = ..., encryption: _Optional[_Union[_cluster_pb2.DataEncryption, _Mapping]] = ..., network_id: _Optional[str] = ..., private_connection_info: _Optional[_Union[PrivateConnectionInfo, _Mapping]] = ..., maintenance_window: _Optional[_Union[_maintenance_pb2.MaintenanceWindow, _Mapping]] = ..., planned_operation: _Optional[_Union[_maintenance_pb2.MaintenanceOperation, _Mapping]] = ..., kafka_config: _Optional[_Union[_config_pb2.KafkaConfig, _Mapping]] = ..., metrics_exporter_connection_info: _Optional[_Union[MetricsExporterConnectionInfo, _Mapping]] = ..., schema_registry_config: _Optional[_Union[_config_pb2.SchemaRegistryConfig, _Mapping]] = ..., rest_api_config: _Optional[_Union[_config_pb2.RestAPIConfig, _Mapping]] = ...) -> None: ...
 
 class ClusterResources(_message.Message):
     __slots__ = ["kafka"]
     class Kafka(_message.Message):
         __slots__ = ["resource_preset_id", "disk_size", "broker_count", "zone_count"]
         RESOURCE_PRESET_ID_FIELD_NUMBER: _ClassVar[int]
         DISK_SIZE_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/cluster_service_pb2.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/cluster_service_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,49 +16,49 @@
 from doublecloud.v1 import maintenance_pb2 as doublecloud_dot_v1_dot_maintenance__pb2
 from doublecloud.v1 import operation_pb2 as doublecloud_dot_v1_dot_operation__pb2
 from doublecloud.v1 import paging_pb2 as doublecloud_dot_v1_dot_paging__pb2
 from doublecloud.kafka.v1 import cluster_pb2 as doublecloud_dot_kafka_dot_v1_dot_cluster__pb2
 from doublecloud.kafka.v1 import config_pb2 as doublecloud_dot_kafka_dot_v1_dot_config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*doublecloud/kafka/v1/cluster_service.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1c\x64oublecloud/v1/cluster.proto\x1a doublecloud/v1/maintenance.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\x1a\"doublecloud/kafka/v1/cluster.proto\x1a!doublecloud/kafka/v1/config.proto\"P\n\x11GetClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1c\n\tsensitive\x18\x02 \x01(\x08R\tsensitive\"\x9b\x01\n\x13ListClustersRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\x12\x35\n\x04view\x18\x03 \x01(\x0e\x32!.doublecloud.kafka.v1.ClusterViewR\x04view\"\x88\x01\n\x14ListClustersResponse\x12\x39\n\x08\x63lusters\x18\x01 \x03(\x0b\x32\x1d.doublecloud.kafka.v1.ClusterR\x08\x63lusters\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"\x90\x05\n\x14\x43reateClusterRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x02 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\x12\x18\n\x07version\x18\x06 \x01(\tR\x07version\x12\x44\n\tresources\x18\x07 \x01(\x0b\x32&.doublecloud.kafka.v1.ClusterResourcesR\tresources\x12.\n\x06\x61\x63\x63\x65ss\x18\x08 \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12>\n\nencryption\x18\t \x01(\x0b\x32\x1e.doublecloud.v1.DataEncryptionR\nencryption\x12\x1d\n\nnetwork_id\x18\n \x01(\tR\tnetworkId\x12P\n\x12maintenance_window\x18\x0b \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\x12\x44\n\x0ckafka_config\x18\x0c \x01(\x0b\x32!.doublecloud.kafka.v1.KafkaConfigR\x0bkafkaConfig\x12`\n\x16schema_registry_config\x18\r \x01(\x0b\x32*.doublecloud.kafka.v1.SchemaRegistryConfigR\x14schemaRegistryConfig\"\xf5\x03\n\x14UpdateClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x18\n\x07version\x18\x04 \x01(\tR\x07version\x12\x44\n\tresources\x18\x05 \x01(\x0b\x32&.doublecloud.kafka.v1.ClusterResourcesR\tresources\x12.\n\x06\x61\x63\x63\x65ss\x18\x06 \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12P\n\x12maintenance_window\x18\x07 \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\x12\x44\n\x0ckafka_config\x18\x08 \x01(\x0b\x32!.doublecloud.kafka.v1.KafkaConfigR\x0bkafkaConfig\x12`\n\x16schema_registry_config\x18\t \x01(\x0b\x32*.doublecloud.kafka.v1.SchemaRegistryConfigR\x14schemaRegistryConfig\"5\n\x14\x44\x65leteClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"?\n\x1eResetClusterCredentialsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"h\n\x17ListClusterHostsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x83\x01\n\x18ListClusterHostsResponse\x12\x30\n\x05hosts\x18\x01 \x03(\x0b\x32\x1a.doublecloud.kafka.v1.HostR\x05hosts\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"4\n\x13StartClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"3\n\x12StopClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"\xd0\x01\n\x1cRescheduleMaintenanceRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12G\n\x0freschedule_type\x18\x02 \x01(\x0e\x32\x1e.doublecloud.v1.RescheduleTypeR\x0erescheduleType\x12H\n\x12\x64\x65layed_until_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x64\x65layedUntilTime\"m\n\x1cListClusterOperationsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x91\x01\n\x1dListClusterOperationsResponse\x12\x39\n\noperations\x18\x01 \x03(\x0b\x32\x19.doublecloud.v1.OperationR\noperations\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage*V\n\x0b\x43lusterView\x12\x18\n\x14\x43LUSTER_VIEW_INVALID\x10\x00\x12\x16\n\x12\x43LUSTER_VIEW_BASIC\x10\x01\x12\x15\n\x11\x43LUSTER_VIEW_FULL\x10\x02\x32\x81\x08\n\x0e\x43lusterService\x12M\n\x03Get\x12\'.doublecloud.kafka.v1.GetClusterRequest\x1a\x1d.doublecloud.kafka.v1.Cluster\x12]\n\x04List\x12).doublecloud.kafka.v1.ListClustersRequest\x1a*.doublecloud.kafka.v1.ListClustersResponse\x12O\n\x06\x43reate\x12*.doublecloud.kafka.v1.CreateClusterRequest\x1a\x19.doublecloud.v1.Operation\x12O\n\x06Update\x12*.doublecloud.kafka.v1.UpdateClusterRequest\x1a\x19.doublecloud.v1.Operation\x12O\n\x06\x44\x65lete\x12*.doublecloud.kafka.v1.DeleteClusterRequest\x1a\x19.doublecloud.v1.Operation\x12\x63\n\x10ResetCredentials\x12\x34.doublecloud.kafka.v1.ResetClusterCredentialsRequest\x1a\x19.doublecloud.v1.Operation\x12j\n\tListHosts\x12-.doublecloud.kafka.v1.ListClusterHostsRequest\x1a..doublecloud.kafka.v1.ListClusterHostsResponse\x12M\n\x05Start\x12).doublecloud.kafka.v1.StartClusterRequest\x1a\x19.doublecloud.v1.Operation\x12K\n\x04Stop\x12(.doublecloud.kafka.v1.StopClusterRequest\x1a\x19.doublecloud.v1.Operation\x12\x66\n\x15RescheduleMaintenance\x12\x32.doublecloud.kafka.v1.RescheduleMaintenanceRequest\x1a\x19.doublecloud.v1.Operation\x12y\n\x0eListOperations\x12\x32.doublecloud.kafka.v1.ListClusterOperationsRequest\x1a\x33.doublecloud.kafka.v1.ListClusterOperationsResponseB?Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafkab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*doublecloud/kafka/v1/cluster_service.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1c\x64oublecloud/v1/cluster.proto\x1a doublecloud/v1/maintenance.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\x1a\"doublecloud/kafka/v1/cluster.proto\x1a!doublecloud/kafka/v1/config.proto\"P\n\x11GetClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1c\n\tsensitive\x18\x02 \x01(\x08R\tsensitive\"\x9b\x01\n\x13ListClustersRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\x12\x35\n\x04view\x18\x03 \x01(\x0e\x32!.doublecloud.kafka.v1.ClusterViewR\x04view\"\x88\x01\n\x14ListClustersResponse\x12\x39\n\x08\x63lusters\x18\x01 \x03(\x0b\x32\x1d.doublecloud.kafka.v1.ClusterR\x08\x63lusters\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"\xdd\x05\n\x14\x43reateClusterRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x02 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\x12\x18\n\x07version\x18\x06 \x01(\tR\x07version\x12\x44\n\tresources\x18\x07 \x01(\x0b\x32&.doublecloud.kafka.v1.ClusterResourcesR\tresources\x12.\n\x06\x61\x63\x63\x65ss\x18\x08 \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12>\n\nencryption\x18\t \x01(\x0b\x32\x1e.doublecloud.v1.DataEncryptionR\nencryption\x12\x1d\n\nnetwork_id\x18\n \x01(\tR\tnetworkId\x12P\n\x12maintenance_window\x18\x0b \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\x12\x44\n\x0ckafka_config\x18\x0c \x01(\x0b\x32!.doublecloud.kafka.v1.KafkaConfigR\x0bkafkaConfig\x12`\n\x16schema_registry_config\x18\r \x01(\x0b\x32*.doublecloud.kafka.v1.SchemaRegistryConfigR\x14schemaRegistryConfig\x12K\n\x0frest_api_config\x18\x0e \x01(\x0b\x32#.doublecloud.kafka.v1.RestAPIConfigR\rrestApiConfig\"\xc2\x04\n\x14UpdateClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x18\n\x07version\x18\x04 \x01(\tR\x07version\x12\x44\n\tresources\x18\x05 \x01(\x0b\x32&.doublecloud.kafka.v1.ClusterResourcesR\tresources\x12.\n\x06\x61\x63\x63\x65ss\x18\x06 \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12P\n\x12maintenance_window\x18\x07 \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\x12\x44\n\x0ckafka_config\x18\x08 \x01(\x0b\x32!.doublecloud.kafka.v1.KafkaConfigR\x0bkafkaConfig\x12`\n\x16schema_registry_config\x18\t \x01(\x0b\x32*.doublecloud.kafka.v1.SchemaRegistryConfigR\x14schemaRegistryConfig\x12K\n\x0frest_api_config\x18\n \x01(\x0b\x32#.doublecloud.kafka.v1.RestAPIConfigR\rrestApiConfig\"5\n\x14\x44\x65leteClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"?\n\x1eResetClusterCredentialsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"h\n\x17ListClusterHostsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x83\x01\n\x18ListClusterHostsResponse\x12\x30\n\x05hosts\x18\x01 \x03(\x0b\x32\x1a.doublecloud.kafka.v1.HostR\x05hosts\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"4\n\x13StartClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"3\n\x12StopClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"\xd0\x01\n\x1cRescheduleMaintenanceRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12G\n\x0freschedule_type\x18\x02 \x01(\x0e\x32\x1e.doublecloud.v1.RescheduleTypeR\x0erescheduleType\x12H\n\x12\x64\x65layed_until_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x64\x65layedUntilTime\"m\n\x1cListClusterOperationsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x91\x01\n\x1dListClusterOperationsResponse\x12\x39\n\noperations\x18\x01 \x03(\x0b\x32\x19.doublecloud.v1.OperationR\noperations\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage*V\n\x0b\x43lusterView\x12\x18\n\x14\x43LUSTER_VIEW_INVALID\x10\x00\x12\x16\n\x12\x43LUSTER_VIEW_BASIC\x10\x01\x12\x15\n\x11\x43LUSTER_VIEW_FULL\x10\x02\x32\x81\x08\n\x0e\x43lusterService\x12M\n\x03Get\x12\'.doublecloud.kafka.v1.GetClusterRequest\x1a\x1d.doublecloud.kafka.v1.Cluster\x12]\n\x04List\x12).doublecloud.kafka.v1.ListClustersRequest\x1a*.doublecloud.kafka.v1.ListClustersResponse\x12O\n\x06\x43reate\x12*.doublecloud.kafka.v1.CreateClusterRequest\x1a\x19.doublecloud.v1.Operation\x12O\n\x06Update\x12*.doublecloud.kafka.v1.UpdateClusterRequest\x1a\x19.doublecloud.v1.Operation\x12O\n\x06\x44\x65lete\x12*.doublecloud.kafka.v1.DeleteClusterRequest\x1a\x19.doublecloud.v1.Operation\x12\x63\n\x10ResetCredentials\x12\x34.doublecloud.kafka.v1.ResetClusterCredentialsRequest\x1a\x19.doublecloud.v1.Operation\x12j\n\tListHosts\x12-.doublecloud.kafka.v1.ListClusterHostsRequest\x1a..doublecloud.kafka.v1.ListClusterHostsResponse\x12M\n\x05Start\x12).doublecloud.kafka.v1.StartClusterRequest\x1a\x19.doublecloud.v1.Operation\x12K\n\x04Stop\x12(.doublecloud.kafka.v1.StopClusterRequest\x1a\x19.doublecloud.v1.Operation\x12\x66\n\x15RescheduleMaintenance\x12\x32.doublecloud.kafka.v1.RescheduleMaintenanceRequest\x1a\x19.doublecloud.v1.Operation\x12y\n\x0eListOperations\x12\x32.doublecloud.kafka.v1.ListClusterOperationsRequest\x1a\x33.doublecloud.kafka.v1.ListClusterOperationsResponseB?Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafkab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.kafka.v1.cluster_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafka'
-  _globals['_CLUSTERVIEW']._serialized_start=2776
-  _globals['_CLUSTERVIEW']._serialized_end=2862
+  _globals['_CLUSTERVIEW']._serialized_start=2930
+  _globals['_CLUSTERVIEW']._serialized_end=3016
   _globals['_GETCLUSTERREQUEST']._serialized_start=297
   _globals['_GETCLUSTERREQUEST']._serialized_end=377
   _globals['_LISTCLUSTERSREQUEST']._serialized_start=380
   _globals['_LISTCLUSTERSREQUEST']._serialized_end=535
   _globals['_LISTCLUSTERSRESPONSE']._serialized_start=538
   _globals['_LISTCLUSTERSRESPONSE']._serialized_end=674
   _globals['_CREATECLUSTERREQUEST']._serialized_start=677
-  _globals['_CREATECLUSTERREQUEST']._serialized_end=1333
-  _globals['_UPDATECLUSTERREQUEST']._serialized_start=1336
-  _globals['_UPDATECLUSTERREQUEST']._serialized_end=1837
-  _globals['_DELETECLUSTERREQUEST']._serialized_start=1839
-  _globals['_DELETECLUSTERREQUEST']._serialized_end=1892
-  _globals['_RESETCLUSTERCREDENTIALSREQUEST']._serialized_start=1894
-  _globals['_RESETCLUSTERCREDENTIALSREQUEST']._serialized_end=1957
-  _globals['_LISTCLUSTERHOSTSREQUEST']._serialized_start=1959
-  _globals['_LISTCLUSTERHOSTSREQUEST']._serialized_end=2063
-  _globals['_LISTCLUSTERHOSTSRESPONSE']._serialized_start=2066
-  _globals['_LISTCLUSTERHOSTSRESPONSE']._serialized_end=2197
-  _globals['_STARTCLUSTERREQUEST']._serialized_start=2199
-  _globals['_STARTCLUSTERREQUEST']._serialized_end=2251
-  _globals['_STOPCLUSTERREQUEST']._serialized_start=2253
-  _globals['_STOPCLUSTERREQUEST']._serialized_end=2304
-  _globals['_RESCHEDULEMAINTENANCEREQUEST']._serialized_start=2307
-  _globals['_RESCHEDULEMAINTENANCEREQUEST']._serialized_end=2515
-  _globals['_LISTCLUSTEROPERATIONSREQUEST']._serialized_start=2517
-  _globals['_LISTCLUSTEROPERATIONSREQUEST']._serialized_end=2626
-  _globals['_LISTCLUSTEROPERATIONSRESPONSE']._serialized_start=2629
-  _globals['_LISTCLUSTEROPERATIONSRESPONSE']._serialized_end=2774
-  _globals['_CLUSTERSERVICE']._serialized_start=2865
-  _globals['_CLUSTERSERVICE']._serialized_end=3890
+  _globals['_CREATECLUSTERREQUEST']._serialized_end=1410
+  _globals['_UPDATECLUSTERREQUEST']._serialized_start=1413
+  _globals['_UPDATECLUSTERREQUEST']._serialized_end=1991
+  _globals['_DELETECLUSTERREQUEST']._serialized_start=1993
+  _globals['_DELETECLUSTERREQUEST']._serialized_end=2046
+  _globals['_RESETCLUSTERCREDENTIALSREQUEST']._serialized_start=2048
+  _globals['_RESETCLUSTERCREDENTIALSREQUEST']._serialized_end=2111
+  _globals['_LISTCLUSTERHOSTSREQUEST']._serialized_start=2113
+  _globals['_LISTCLUSTERHOSTSREQUEST']._serialized_end=2217
+  _globals['_LISTCLUSTERHOSTSRESPONSE']._serialized_start=2220
+  _globals['_LISTCLUSTERHOSTSRESPONSE']._serialized_end=2351
+  _globals['_STARTCLUSTERREQUEST']._serialized_start=2353
+  _globals['_STARTCLUSTERREQUEST']._serialized_end=2405
+  _globals['_STOPCLUSTERREQUEST']._serialized_start=2407
+  _globals['_STOPCLUSTERREQUEST']._serialized_end=2458
+  _globals['_RESCHEDULEMAINTENANCEREQUEST']._serialized_start=2461
+  _globals['_RESCHEDULEMAINTENANCEREQUEST']._serialized_end=2669
+  _globals['_LISTCLUSTEROPERATIONSREQUEST']._serialized_start=2671
+  _globals['_LISTCLUSTEROPERATIONSREQUEST']._serialized_end=2780
+  _globals['_LISTCLUSTEROPERATIONSRESPONSE']._serialized_start=2783
+  _globals['_LISTCLUSTEROPERATIONSRESPONSE']._serialized_end=2928
+  _globals['_CLUSTERSERVICE']._serialized_start=3019
+  _globals['_CLUSTERSERVICE']._serialized_end=4044
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/cluster_service_pb2.pyi` & `doublecloud-0.8.0/doublecloud/kafka/v1/cluster_service_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -45,64 +45,68 @@
     CLUSTERS_FIELD_NUMBER: _ClassVar[int]
     NEXT_PAGE_FIELD_NUMBER: _ClassVar[int]
     clusters: _containers.RepeatedCompositeFieldContainer[_cluster_pb2_1.Cluster]
     next_page: _paging_pb2.NextPage
     def __init__(self, clusters: _Optional[_Iterable[_Union[_cluster_pb2_1.Cluster, _Mapping]]] = ..., next_page: _Optional[_Union[_paging_pb2.NextPage, _Mapping]] = ...) -> None: ...
 
 class CreateClusterRequest(_message.Message):
-    __slots__ = ["project_id", "cloud_type", "region_id", "name", "description", "version", "resources", "access", "encryption", "network_id", "maintenance_window", "kafka_config", "schema_registry_config"]
+    __slots__ = ["project_id", "cloud_type", "region_id", "name", "description", "version", "resources", "access", "encryption", "network_id", "maintenance_window", "kafka_config", "schema_registry_config", "rest_api_config"]
     PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     CLOUD_TYPE_FIELD_NUMBER: _ClassVar[int]
     REGION_ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     RESOURCES_FIELD_NUMBER: _ClassVar[int]
     ACCESS_FIELD_NUMBER: _ClassVar[int]
     ENCRYPTION_FIELD_NUMBER: _ClassVar[int]
     NETWORK_ID_FIELD_NUMBER: _ClassVar[int]
     MAINTENANCE_WINDOW_FIELD_NUMBER: _ClassVar[int]
     KAFKA_CONFIG_FIELD_NUMBER: _ClassVar[int]
     SCHEMA_REGISTRY_CONFIG_FIELD_NUMBER: _ClassVar[int]
+    REST_API_CONFIG_FIELD_NUMBER: _ClassVar[int]
     project_id: str
     cloud_type: str
     region_id: str
     name: str
     description: str
     version: str
     resources: _cluster_pb2_1.ClusterResources
     access: _cluster_pb2.Access
     encryption: _cluster_pb2.DataEncryption
     network_id: str
     maintenance_window: _maintenance_pb2.MaintenanceWindow
     kafka_config: _config_pb2.KafkaConfig
     schema_registry_config: _config_pb2.SchemaRegistryConfig
-    def __init__(self, project_id: _Optional[str] = ..., cloud_type: _Optional[str] = ..., region_id: _Optional[str] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., version: _Optional[str] = ..., resources: _Optional[_Union[_cluster_pb2_1.ClusterResources, _Mapping]] = ..., access: _Optional[_Union[_cluster_pb2.Access, _Mapping]] = ..., encryption: _Optional[_Union[_cluster_pb2.DataEncryption, _Mapping]] = ..., network_id: _Optional[str] = ..., maintenance_window: _Optional[_Union[_maintenance_pb2.MaintenanceWindow, _Mapping]] = ..., kafka_config: _Optional[_Union[_config_pb2.KafkaConfig, _Mapping]] = ..., schema_registry_config: _Optional[_Union[_config_pb2.SchemaRegistryConfig, _Mapping]] = ...) -> None: ...
+    rest_api_config: _config_pb2.RestAPIConfig
+    def __init__(self, project_id: _Optional[str] = ..., cloud_type: _Optional[str] = ..., region_id: _Optional[str] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., version: _Optional[str] = ..., resources: _Optional[_Union[_cluster_pb2_1.ClusterResources, _Mapping]] = ..., access: _Optional[_Union[_cluster_pb2.Access, _Mapping]] = ..., encryption: _Optional[_Union[_cluster_pb2.DataEncryption, _Mapping]] = ..., network_id: _Optional[str] = ..., maintenance_window: _Optional[_Union[_maintenance_pb2.MaintenanceWindow, _Mapping]] = ..., kafka_config: _Optional[_Union[_config_pb2.KafkaConfig, _Mapping]] = ..., schema_registry_config: _Optional[_Union[_config_pb2.SchemaRegistryConfig, _Mapping]] = ..., rest_api_config: _Optional[_Union[_config_pb2.RestAPIConfig, _Mapping]] = ...) -> None: ...
 
 class UpdateClusterRequest(_message.Message):
-    __slots__ = ["cluster_id", "name", "description", "version", "resources", "access", "maintenance_window", "kafka_config", "schema_registry_config"]
+    __slots__ = ["cluster_id", "name", "description", "version", "resources", "access", "maintenance_window", "kafka_config", "schema_registry_config", "rest_api_config"]
     CLUSTER_ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     RESOURCES_FIELD_NUMBER: _ClassVar[int]
     ACCESS_FIELD_NUMBER: _ClassVar[int]
     MAINTENANCE_WINDOW_FIELD_NUMBER: _ClassVar[int]
     KAFKA_CONFIG_FIELD_NUMBER: _ClassVar[int]
     SCHEMA_REGISTRY_CONFIG_FIELD_NUMBER: _ClassVar[int]
+    REST_API_CONFIG_FIELD_NUMBER: _ClassVar[int]
     cluster_id: str
     name: str
     description: str
     version: str
     resources: _cluster_pb2_1.ClusterResources
     access: _cluster_pb2.Access
     maintenance_window: _maintenance_pb2.MaintenanceWindow
     kafka_config: _config_pb2.KafkaConfig
     schema_registry_config: _config_pb2.SchemaRegistryConfig
-    def __init__(self, cluster_id: _Optional[str] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., version: _Optional[str] = ..., resources: _Optional[_Union[_cluster_pb2_1.ClusterResources, _Mapping]] = ..., access: _Optional[_Union[_cluster_pb2.Access, _Mapping]] = ..., maintenance_window: _Optional[_Union[_maintenance_pb2.MaintenanceWindow, _Mapping]] = ..., kafka_config: _Optional[_Union[_config_pb2.KafkaConfig, _Mapping]] = ..., schema_registry_config: _Optional[_Union[_config_pb2.SchemaRegistryConfig, _Mapping]] = ...) -> None: ...
+    rest_api_config: _config_pb2.RestAPIConfig
+    def __init__(self, cluster_id: _Optional[str] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., version: _Optional[str] = ..., resources: _Optional[_Union[_cluster_pb2_1.ClusterResources, _Mapping]] = ..., access: _Optional[_Union[_cluster_pb2.Access, _Mapping]] = ..., maintenance_window: _Optional[_Union[_maintenance_pb2.MaintenanceWindow, _Mapping]] = ..., kafka_config: _Optional[_Union[_config_pb2.KafkaConfig, _Mapping]] = ..., schema_registry_config: _Optional[_Union[_config_pb2.SchemaRegistryConfig, _Mapping]] = ..., rest_api_config: _Optional[_Union[_config_pb2.RestAPIConfig, _Mapping]] = ...) -> None: ...
 
 class DeleteClusterRequest(_message.Message):
     __slots__ = ["cluster_id"]
     CLUSTER_ID_FIELD_NUMBER: _ClassVar[int]
     cluster_id: str
     def __init__(self, cluster_id: _Optional[str] = ...) -> None: ...
```

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/cluster_service_pb2_grpc.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/config_pb2.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/config_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!doublecloud/kafka/v1/config.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1egoogle/protobuf/wrappers.proto\"\xaa\x01\n\x0bKafkaConfig\x12G\n\x11message_max_bytes\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0fmessageMaxBytes\x12R\n\x17replica_fetch_max_bytes\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x14replicaFetchMaxBytes\"0\n\x14SchemaRegistryConfig\x12\x18\n\x07\x65nabled\x18\x01 \x01(\x08R\x07\x65nabledB?Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafkab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!doublecloud/kafka/v1/config.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1egoogle/protobuf/wrappers.proto\"\xaa\x01\n\x0bKafkaConfig\x12G\n\x11message_max_bytes\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0fmessageMaxBytes\x12R\n\x17replica_fetch_max_bytes\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x14replicaFetchMaxBytes\"0\n\x14SchemaRegistryConfig\x12\x18\n\x07\x65nabled\x18\x01 \x01(\x08R\x07\x65nabled\")\n\rRestAPIConfig\x12\x18\n\x07\x65nabled\x18\x01 \x01(\x08R\x07\x65nabledB?Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafkab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.kafka.v1.config_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafka'
   _globals['_KAFKACONFIG']._serialized_start=92
   _globals['_KAFKACONFIG']._serialized_end=262
   _globals['_SCHEMAREGISTRYCONFIG']._serialized_start=264
   _globals['_SCHEMAREGISTRYCONFIG']._serialized_end=312
+  _globals['_RESTAPICONFIG']._serialized_start=314
+  _globals['_RESTAPICONFIG']._serialized_end=355
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/config_pb2.pyi` & `doublecloud-0.8.0/doublecloud/kafka/v1/config_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -14,7 +14,13 @@
     def __init__(self, message_max_bytes: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., replica_fetch_max_bytes: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ...) -> None: ...
 
 class SchemaRegistryConfig(_message.Message):
     __slots__ = ["enabled"]
     ENABLED_FIELD_NUMBER: _ClassVar[int]
     enabled: bool
     def __init__(self, enabled: bool = ...) -> None: ...
+
+class RestAPIConfig(_message.Message):
+    __slots__ = ["enabled"]
+    ENABLED_FIELD_NUMBER: _ClassVar[int]
+    enabled: bool
+    def __init__(self, enabled: bool = ...) -> None: ...
```

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/connector_pb2.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/connector_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/connector_pb2.pyi` & `doublecloud-0.8.0/doublecloud/kafka/v1/connector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/connector_service_pb2.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/connector_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/connector_service_pb2.pyi` & `doublecloud-0.8.0/doublecloud/kafka/v1/connector_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/connector_service_pb2_grpc.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/connector_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/operation_service_pb2.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/operation_service_pb2.pyi` & `doublecloud-0.8.0/doublecloud/kafka/v1/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/operation_service_pb2_grpc.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/topic_pb2.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/topic_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/topic_pb2.pyi` & `doublecloud-0.8.0/doublecloud/kafka/v1/topic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/topic_service_pb2.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/topic_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/topic_service_pb2.pyi` & `doublecloud-0.8.0/doublecloud/kafka/v1/topic_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/topic_service_pb2_grpc.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/topic_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/user_pb2.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/user_pb2.pyi` & `doublecloud-0.8.0/doublecloud/kafka/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/user_service_pb2.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/user_service_pb2.pyi` & `doublecloud-0.8.0/doublecloud/kafka/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/user_service_pb2_grpc.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/version_pb2.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/version_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/version_pb2.pyi` & `doublecloud-0.8.0/doublecloud/kafka/v1/version_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/version_service_pb2.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/version_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/version_service_pb2.pyi` & `doublecloud-0.8.0/doublecloud/kafka/v1/version_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/kafka/v1/version_service_pb2_grpc.py` & `doublecloud-0.8.0/doublecloud/kafka/v1/version_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/network/v1/network_connection_pb2.py` & `doublecloud-0.8.0/doublecloud/network/v1/network_connection_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/network/v1/network_connection_pb2.pyi` & `doublecloud-0.8.0/doublecloud/network/v1/network_connection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/network/v1/network_connection_service_pb2.py` & `doublecloud-0.8.0/doublecloud/network/v1/network_connection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/network/v1/network_connection_service_pb2.pyi` & `doublecloud-0.8.0/doublecloud/network/v1/network_connection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/network/v1/network_connection_service_pb2_grpc.py` & `doublecloud-0.8.0/doublecloud/network/v1/network_connection_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/network/v1/network_pb2.py` & `doublecloud-0.8.0/doublecloud/network/v1/network_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/network/v1/network_pb2.pyi` & `doublecloud-0.8.0/doublecloud/network/v1/network_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/network/v1/network_service_pb2.py` & `doublecloud-0.8.0/doublecloud/network/v1/network_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/network/v1/network_service_pb2.pyi` & `doublecloud-0.8.0/doublecloud/network/v1/network_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/network/v1/network_service_pb2_grpc.py` & `doublecloud-0.8.0/doublecloud/network/v1/network_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/network/v1/operation_service_pb2.py` & `doublecloud-0.8.0/doublecloud/network/v1/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/network/v1/operation_service_pb2.pyi` & `doublecloud-0.8.0/doublecloud/network/v1/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/network/v1/operation_service_pb2_grpc.py` & `doublecloud-0.8.0/doublecloud/network/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/common_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/common_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/common_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/kafka_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/kafka_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/kafka_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/kafka_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mongo_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/mongo_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mongo_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/mongo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mysql_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/mysql_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/mysql_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/mysql_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/parsers_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/parsers_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/parsers_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/parsers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/postgres_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/postgres_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/postgres_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/postgres_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/serializers_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/serializers_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint/serializers_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint/serializers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_service_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_service_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/endpoint_service_pb2_grpc.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/endpoint_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/operation_service_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/operation_service_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/operation_service_pb2_grpc.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/transfer_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/transfer_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/transfer_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/transfer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/transfer_service_pb2.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/transfer_service_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/transfer_service_pb2.pyi` & `doublecloud-0.8.0/doublecloud/transfer/v1/transfer_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/transfer/v1/transfer_service_pb2_grpc.py` & `doublecloud-0.8.0/doublecloud/transfer/v1/transfer_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/v1/cluster_pb2.py` & `doublecloud-0.8.0/doublecloud/v1/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/v1/cluster_pb2.pyi` & `doublecloud-0.8.0/doublecloud/v1/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/v1/maintenance_pb2.py` & `doublecloud-0.8.0/doublecloud/v1/maintenance_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/v1/maintenance_pb2.pyi` & `doublecloud-0.8.0/doublecloud/v1/maintenance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/v1/operation_pb2.py` & `doublecloud-0.8.0/doublecloud/v1/operation_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/v1/operation_pb2.pyi` & `doublecloud-0.8.0/doublecloud/v1/operation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/v1/paging_pb2.py` & `doublecloud-0.8.0/doublecloud/v1/paging_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/v1/paging_pb2.pyi` & `doublecloud-0.8.0/doublecloud/v1/paging_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/visualization/v1/workbook_pb2.py` & `doublecloud-0.8.0/doublecloud/visualization/v1/workbook_pb2.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/visualization/v1/workbook_pb2.pyi` & `doublecloud-0.8.0/doublecloud/visualization/v1/workbook_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud/visualization/v1/workbook_service_pb2.py` & `doublecloud-0.8.0/doublecloud/visualization/v1/workbook_service_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,43 +12,43 @@
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from doublecloud.v1 import operation_pb2 as doublecloud_dot_v1_dot_operation__pb2
 from doublecloud.visualization.v1 import workbook_pb2 as doublecloud_dot_visualization_dot_v1_dot_workbook__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3doublecloud/visualization/v1/workbook_service.proto\x12\x1c\x64oublecloud.visualization.v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a+doublecloud/visualization/v1/workbook.proto\"5\n\x12GetWorkbookRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\"Y\n\x13GetWorkbookResponse\x12\x42\n\x08workbook\x18\x01 \x01(\x0b\x32&.doublecloud.visualization.v1.WorkbookR\x08workbook\"]\n\x15\x43reateWorkbookRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12%\n\x0eworkbook_title\x18\x02 \x01(\tR\rworkbookTitle\"\xbd\x01\n\x15UpdateWorkbookRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\x42\n\x08workbook\x18\x02 \x01(\x0b\x32&.doublecloud.visualization.v1.WorkbookR\x08workbook\x12?\n\rforce_rewrite\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x0c\x66orceRewrite\"8\n\x15\x44\x65leteWorkbookRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\"h\n\x1cGetWorkbookConnectionRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\"i\n\x1dGetWorkbookConnectionResponse\x12H\n\nconnection\x18\x01 \x01(\x0b\x32(.doublecloud.visualization.v1.ConnectionR\nconnection\"\xf3\x01\n\x1f\x43reateWorkbookConnectionRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\x12H\n\nconnection\x18\x03 \x01(\x0b\x32(.doublecloud.visualization.v1.ConnectionR\nconnection\x12<\n\x06secret\x18\x04 \x01(\x0b\x32$.doublecloud.visualization.v1.SecretR\x06secret\"\xf3\x01\n\x1fUpdateWorkbookConnectionRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\x12H\n\nconnection\x18\x03 \x01(\x0b\x32(.doublecloud.visualization.v1.ConnectionR\nconnection\x12<\n\x06secret\x18\x04 \x01(\x0b\x32$.doublecloud.visualization.v1.SecretR\x06secret\"k\n\x1f\x44\x65leteWorkbookConnectionRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\"\xb6\x01\n\x1a\x41\x64viseDatasetFieldsRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\x12N\n\x0fpartial_dataset\x18\x03 \x01(\x0b\x32%.doublecloud.visualization.v1.DatasetR\x0epartialDataset\"^\n\x1b\x41\x64viseDatasetFieldsResponse\x12?\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32%.doublecloud.visualization.v1.DatasetR\x07\x64\x61taset2\xed\x07\n\x0fWorkbookService\x12j\n\x03Get\x12\x30.doublecloud.visualization.v1.GetWorkbookRequest\x1a\x31.doublecloud.visualization.v1.GetWorkbookResponse\x12X\n\x06\x43reate\x12\x33.doublecloud.visualization.v1.CreateWorkbookRequest\x1a\x19.doublecloud.v1.Operation\x12X\n\x06Update\x12\x33.doublecloud.visualization.v1.UpdateWorkbookRequest\x1a\x19.doublecloud.v1.Operation\x12X\n\x06\x44\x65lete\x12\x33.doublecloud.visualization.v1.DeleteWorkbookRequest\x1a\x19.doublecloud.v1.Operation\x12\x88\x01\n\rGetConnection\x12:.doublecloud.visualization.v1.GetWorkbookConnectionRequest\x1a;.doublecloud.visualization.v1.GetWorkbookConnectionResponse\x12l\n\x10\x43reateConnection\x12=.doublecloud.visualization.v1.CreateWorkbookConnectionRequest\x1a\x19.doublecloud.v1.Operation\x12l\n\x10UpdateConnection\x12=.doublecloud.visualization.v1.UpdateWorkbookConnectionRequest\x1a\x19.doublecloud.v1.Operation\x12l\n\x10\x44\x65leteConnection\x12=.doublecloud.visualization.v1.DeleteWorkbookConnectionRequest\x1a\x19.doublecloud.v1.Operation\x12\x8a\x01\n\x13\x41\x64viseDatasetFields\x12\x38.doublecloud.visualization.v1.AdviseDatasetFieldsRequest\x1a\x39.doublecloud.visualization.v1.AdviseDatasetFieldsResponseBOZMgithub.com/doublecloud/go-genproto/doublecloud/visualization/v1;visualizationb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3doublecloud/visualization/v1/workbook_service.proto\x12\x1c\x64oublecloud.visualization.v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a+doublecloud/visualization/v1/workbook.proto\"5\n\x12GetWorkbookRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\"\x9e\x01\n\x13GetWorkbookResponse\x12\x42\n\x08workbook\x18\x01 \x01(\x0b\x32&.doublecloud.visualization.v1.WorkbookR\x08workbook\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02id\x12\x14\n\x05title\x18\x03 \x01(\tR\x05title\x12\x1d\n\nproject_id\x18\x04 \x01(\tR\tprojectId\"]\n\x15\x43reateWorkbookRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12%\n\x0eworkbook_title\x18\x02 \x01(\tR\rworkbookTitle\"\xbd\x01\n\x15UpdateWorkbookRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\x42\n\x08workbook\x18\x02 \x01(\x0b\x32&.doublecloud.visualization.v1.WorkbookR\x08workbook\x12?\n\rforce_rewrite\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x0c\x66orceRewrite\"8\n\x15\x44\x65leteWorkbookRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\"h\n\x1cGetWorkbookConnectionRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\"i\n\x1dGetWorkbookConnectionResponse\x12H\n\nconnection\x18\x01 \x01(\x0b\x32(.doublecloud.visualization.v1.ConnectionR\nconnection\"\xf3\x01\n\x1f\x43reateWorkbookConnectionRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\x12H\n\nconnection\x18\x03 \x01(\x0b\x32(.doublecloud.visualization.v1.ConnectionR\nconnection\x12<\n\x06secret\x18\x04 \x01(\x0b\x32$.doublecloud.visualization.v1.SecretR\x06secret\"\xf3\x01\n\x1fUpdateWorkbookConnectionRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\x12H\n\nconnection\x18\x03 \x01(\x0b\x32(.doublecloud.visualization.v1.ConnectionR\nconnection\x12<\n\x06secret\x18\x04 \x01(\x0b\x32$.doublecloud.visualization.v1.SecretR\x06secret\"k\n\x1f\x44\x65leteWorkbookConnectionRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\"\xb6\x01\n\x1a\x41\x64viseDatasetFieldsRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\x12N\n\x0fpartial_dataset\x18\x03 \x01(\x0b\x32%.doublecloud.visualization.v1.DatasetR\x0epartialDataset\"^\n\x1b\x41\x64viseDatasetFieldsResponse\x12?\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32%.doublecloud.visualization.v1.DatasetR\x07\x64\x61taset2\xed\x07\n\x0fWorkbookService\x12j\n\x03Get\x12\x30.doublecloud.visualization.v1.GetWorkbookRequest\x1a\x31.doublecloud.visualization.v1.GetWorkbookResponse\x12X\n\x06\x43reate\x12\x33.doublecloud.visualization.v1.CreateWorkbookRequest\x1a\x19.doublecloud.v1.Operation\x12X\n\x06Update\x12\x33.doublecloud.visualization.v1.UpdateWorkbookRequest\x1a\x19.doublecloud.v1.Operation\x12X\n\x06\x44\x65lete\x12\x33.doublecloud.visualization.v1.DeleteWorkbookRequest\x1a\x19.doublecloud.v1.Operation\x12\x88\x01\n\rGetConnection\x12:.doublecloud.visualization.v1.GetWorkbookConnectionRequest\x1a;.doublecloud.visualization.v1.GetWorkbookConnectionResponse\x12l\n\x10\x43reateConnection\x12=.doublecloud.visualization.v1.CreateWorkbookConnectionRequest\x1a\x19.doublecloud.v1.Operation\x12l\n\x10UpdateConnection\x12=.doublecloud.visualization.v1.UpdateWorkbookConnectionRequest\x1a\x19.doublecloud.v1.Operation\x12l\n\x10\x44\x65leteConnection\x12=.doublecloud.visualization.v1.DeleteWorkbookConnectionRequest\x1a\x19.doublecloud.v1.Operation\x12\x8a\x01\n\x13\x41\x64viseDatasetFields\x12\x38.doublecloud.visualization.v1.AdviseDatasetFieldsRequest\x1a\x39.doublecloud.visualization.v1.AdviseDatasetFieldsResponseBOZMgithub.com/doublecloud/go-genproto/doublecloud/visualization/v1;visualizationb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.visualization.v1.workbook_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZMgithub.com/doublecloud/go-genproto/doublecloud/visualization/v1;visualization'
   _globals['_GETWORKBOOKREQUEST']._serialized_start=194
   _globals['_GETWORKBOOKREQUEST']._serialized_end=247
-  _globals['_GETWORKBOOKRESPONSE']._serialized_start=249
-  _globals['_GETWORKBOOKRESPONSE']._serialized_end=338
-  _globals['_CREATEWORKBOOKREQUEST']._serialized_start=340
-  _globals['_CREATEWORKBOOKREQUEST']._serialized_end=433
-  _globals['_UPDATEWORKBOOKREQUEST']._serialized_start=436
-  _globals['_UPDATEWORKBOOKREQUEST']._serialized_end=625
-  _globals['_DELETEWORKBOOKREQUEST']._serialized_start=627
-  _globals['_DELETEWORKBOOKREQUEST']._serialized_end=683
-  _globals['_GETWORKBOOKCONNECTIONREQUEST']._serialized_start=685
-  _globals['_GETWORKBOOKCONNECTIONREQUEST']._serialized_end=789
-  _globals['_GETWORKBOOKCONNECTIONRESPONSE']._serialized_start=791
-  _globals['_GETWORKBOOKCONNECTIONRESPONSE']._serialized_end=896
-  _globals['_CREATEWORKBOOKCONNECTIONREQUEST']._serialized_start=899
-  _globals['_CREATEWORKBOOKCONNECTIONREQUEST']._serialized_end=1142
-  _globals['_UPDATEWORKBOOKCONNECTIONREQUEST']._serialized_start=1145
-  _globals['_UPDATEWORKBOOKCONNECTIONREQUEST']._serialized_end=1388
-  _globals['_DELETEWORKBOOKCONNECTIONREQUEST']._serialized_start=1390
-  _globals['_DELETEWORKBOOKCONNECTIONREQUEST']._serialized_end=1497
-  _globals['_ADVISEDATASETFIELDSREQUEST']._serialized_start=1500
-  _globals['_ADVISEDATASETFIELDSREQUEST']._serialized_end=1682
-  _globals['_ADVISEDATASETFIELDSRESPONSE']._serialized_start=1684
-  _globals['_ADVISEDATASETFIELDSRESPONSE']._serialized_end=1778
-  _globals['_WORKBOOKSERVICE']._serialized_start=1781
-  _globals['_WORKBOOKSERVICE']._serialized_end=2786
+  _globals['_GETWORKBOOKRESPONSE']._serialized_start=250
+  _globals['_GETWORKBOOKRESPONSE']._serialized_end=408
+  _globals['_CREATEWORKBOOKREQUEST']._serialized_start=410
+  _globals['_CREATEWORKBOOKREQUEST']._serialized_end=503
+  _globals['_UPDATEWORKBOOKREQUEST']._serialized_start=506
+  _globals['_UPDATEWORKBOOKREQUEST']._serialized_end=695
+  _globals['_DELETEWORKBOOKREQUEST']._serialized_start=697
+  _globals['_DELETEWORKBOOKREQUEST']._serialized_end=753
+  _globals['_GETWORKBOOKCONNECTIONREQUEST']._serialized_start=755
+  _globals['_GETWORKBOOKCONNECTIONREQUEST']._serialized_end=859
+  _globals['_GETWORKBOOKCONNECTIONRESPONSE']._serialized_start=861
+  _globals['_GETWORKBOOKCONNECTIONRESPONSE']._serialized_end=966
+  _globals['_CREATEWORKBOOKCONNECTIONREQUEST']._serialized_start=969
+  _globals['_CREATEWORKBOOKCONNECTIONREQUEST']._serialized_end=1212
+  _globals['_UPDATEWORKBOOKCONNECTIONREQUEST']._serialized_start=1215
+  _globals['_UPDATEWORKBOOKCONNECTIONREQUEST']._serialized_end=1458
+  _globals['_DELETEWORKBOOKCONNECTIONREQUEST']._serialized_start=1460
+  _globals['_DELETEWORKBOOKCONNECTIONREQUEST']._serialized_end=1567
+  _globals['_ADVISEDATASETFIELDSREQUEST']._serialized_start=1570
+  _globals['_ADVISEDATASETFIELDSREQUEST']._serialized_end=1752
+  _globals['_ADVISEDATASETFIELDSRESPONSE']._serialized_start=1754
+  _globals['_ADVISEDATASETFIELDSRESPONSE']._serialized_end=1848
+  _globals['_WORKBOOKSERVICE']._serialized_start=1851
+  _globals['_WORKBOOKSERVICE']._serialized_end=2856
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.7.0/doublecloud/visualization/v1/workbook_service_pb2.pyi` & `doublecloud-0.8.0/doublecloud/visualization/v1/workbook_service_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,24 @@
 class GetWorkbookRequest(_message.Message):
     __slots__ = ["workbook_id"]
     WORKBOOK_ID_FIELD_NUMBER: _ClassVar[int]
     workbook_id: str
     def __init__(self, workbook_id: _Optional[str] = ...) -> None: ...
 
 class GetWorkbookResponse(_message.Message):
-    __slots__ = ["workbook"]
+    __slots__ = ["workbook", "id", "title", "project_id"]
     WORKBOOK_FIELD_NUMBER: _ClassVar[int]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    TITLE_FIELD_NUMBER: _ClassVar[int]
+    PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     workbook: _workbook_pb2.Workbook
-    def __init__(self, workbook: _Optional[_Union[_workbook_pb2.Workbook, _Mapping]] = ...) -> None: ...
+    id: str
+    title: str
+    project_id: str
+    def __init__(self, workbook: _Optional[_Union[_workbook_pb2.Workbook, _Mapping]] = ..., id: _Optional[str] = ..., title: _Optional[str] = ..., project_id: _Optional[str] = ...) -> None: ...
 
 class CreateWorkbookRequest(_message.Message):
     __slots__ = ["project_id", "workbook_title"]
     PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     WORKBOOK_TITLE_FIELD_NUMBER: _ClassVar[int]
     project_id: str
     workbook_title: str
```

### Comparing `doublecloud-0.7.0/doublecloud/visualization/v1/workbook_service_pb2_grpc.py` & `doublecloud-0.8.0/doublecloud/visualization/v1/workbook_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/doublecloud.egg-info/PKG-INFO` & `doublecloud-0.8.0/doublecloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doublecloud
-Version: 0.7.0
+Version: 0.8.0
 Summary: The Double.Cloud official SDK
 Home-page: https://github.com/doublecloud/python-sdk
 Author: DoubleCloud GmbH
 Author-email: support@double.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doublecloud-0.7.0/doublecloud.egg-info/SOURCES.txt` & `doublecloud-0.8.0/doublecloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/pyproject.toml` & `doublecloud-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doublecloud-0.7.0/setup.py` & `doublecloud-0.8.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 packages = find_packages(".", include=["doublecloud*"])
 
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 setup(
     name="doublecloud",
     version=__version__,
     description="The Double.Cloud official SDK",
     url="https://github.com/doublecloud/python-sdk",
     author="DoubleCloud GmbH",
```

