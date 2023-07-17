# Comparing `tmp/strmprivacy-api-definitions-3.4.0.tar.gz` & `tmp/strmprivacy-api-definitions-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strmprivacy-api-definitions-3.4.0.tar", last modified: Tue Jul 11 07:56:12 2023, max compression
+gzip compressed data, was "strmprivacy-api-definitions-3.5.0.tar", last modified: Mon Jul 17 07:35:51 2023, max compression
```

## Comparing `strmprivacy-api-definitions-3.4.0.tar` & `strmprivacy-api-definitions-3.5.0.tar`

### file list

```diff
@@ -1,227 +1,227 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.884743 strmprivacy-api-definitions-3.4.0/
--rw-r--r--   0 root         (0) root         (0)      629 2023-07-11 07:56:12.884743 strmprivacy-api-definitions-3.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 07:56:12.884743 strmprivacy-api-definitions-3.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1443 2023-07-11 07:55:54.000000 strmprivacy-api-definitions-3.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.852741 strmprivacy-api-definitions-3.4.0/strmprivacy/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.852741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.852741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/account/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/account/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.853741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/account/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/account/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12198 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/account/v1/account_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16789 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.853741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.855741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2356 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2300 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3129 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2369 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3261 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3267 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.855741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/audit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/audit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.855741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/audit/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/audit/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3518 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/audit/v1/audit_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5030 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/audit/v1/audit_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.856741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_exporters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_exporters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.856741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_exporters/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_exporters/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5338 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9468 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.856741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_jobs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_jobs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.857741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_jobs/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_jobs/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7665 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10858 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.857741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.858741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/cli/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/cli/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3799 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/cli/v1/cli_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2753 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.858741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/comments/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/comments/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.859741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/comments/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/comments/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3987 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/comments/v1/comments_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6740 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/comments/v1/comments_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.859741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/credentials/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/credentials/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.859741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/credentials/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/credentials/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5049 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/credentials/v1/credentials_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8979 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.860741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/customer_entity_versions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/customer_entity_versions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.860741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/customer_entity_versions/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/customer_entity_versions/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7497 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10288 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.860741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_connectors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_connectors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.861741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_connectors/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_connectors/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5978 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9468 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.861741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_contracts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_contracts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.862742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_contracts/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_contracts/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22863 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28488 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.862742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_subjects/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_subjects/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.863741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_subjects/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_subjects/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9499 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9865 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.863741 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.864742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    82161 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1/entities_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1/entities_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.864742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1alpha/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1alpha/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12632 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.865742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/event_contracts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/event_contracts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.865742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/event_contracts/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/event_contracts/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15658 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    20098 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.866742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/handles/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/handles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.866742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/handles/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/handles/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2239 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/handles/v1/handles_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3057 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/handles/v1/handles_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.866742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.868742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7909 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/entities_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/entities_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6253 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/installations_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9499 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/installations_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6958 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/installed_components_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10345 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/installed_components_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.868742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_clusters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_clusters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.869742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_clusters/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_clusters/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6199 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9342 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.869742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_exporters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_exporters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.870742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_exporters/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_exporters/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5362 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9468 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.870742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_users/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_users/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.870742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_users/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_users/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5369 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8964 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.871742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/key_streams/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/key_streams/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.871742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/key_streams/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/key_streams/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3713 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/key_streams/v1/key_streams_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4941 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.871742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/monitoring/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.872742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/monitoring/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/monitoring/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6738 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/monitoring/v1/monitoring_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7722 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/monitoring/v1/monitoring_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.872742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/notifications/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/notifications/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.873742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/notifications/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/notifications/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10605 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/notifications/v1/notifications_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13648 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/notifications/v1/notifications_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.873742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/onboarding/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/onboarding/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.873742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/onboarding/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/onboarding/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2789 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3161 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.874742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/organizations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/organizations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.874742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/organizations/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/organizations/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5842 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/organizations/v1/organizations_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9075 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/organizations/v1/organizations_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.874742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/paging/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/paging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.875742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/paging/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/paging/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1340 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/paging/v1/paging_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/paging/v1/paging_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.875742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/policies/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/policies/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.876742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/policies/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/policies/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5782 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/policies/v1/policies_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10449 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/policies/v1/policies_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.876742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/project_plans/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/project_plans/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.877742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/project_plans/v1alpha/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/project_plans/v1alpha/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4521 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7409 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.877742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/projects/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/projects/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.877742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/projects/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/projects/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7458 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/projects/v1/projects_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14509 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/projects/v1/projects_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.878743 strmprivacy-api-definitions-3.4.0/strmprivacy/api/purpose_mapping/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/purpose_mapping/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.878743 strmprivacy-api-definitions-3.4.0/strmprivacy/api/purpose_mapping/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/purpose_mapping/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4483 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7407 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.878743 strmprivacy-api-definitions-3.4.0/strmprivacy/api/schemas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/schemas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.879742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/schemas/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/schemas/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13192 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/schemas/v1/schemas_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    17973 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.879742 strmprivacy-api-definitions-3.4.0/strmprivacy/api/sinks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/sinks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.880743 strmprivacy-api-definitions-3.4.0/strmprivacy/api/sinks/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/sinks/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5254 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/sinks/v1/sinks_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8223 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.881743 strmprivacy-api-definitions-3.4.0/strmprivacy/api/streams/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/streams/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.881743 strmprivacy-api-definitions-3.4.0/strmprivacy/api/streams/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/streams/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5689 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/streams/v1/streams_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10437 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.881743 strmprivacy-api-definitions-3.4.0/strmprivacy/api/usage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/usage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.882743 strmprivacy-api-definitions-3.4.0/strmprivacy/api/usage/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 07:56:11.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/usage/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4644 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/usage/v1/usage_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4831 2023-07-10 08:01:34.000000 strmprivacy-api-definitions-3.4.0/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:56:12.883743 strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/
--rw-r--r--   0 root         (0) root         (0)      629 2023-07-11 07:56:12.000000 strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7436 2023-07-11 07:56:12.000000 strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 07:56:12.000000 strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 07:56:12.000000 strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-11 07:56:12.000000 strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-11 07:56:12.000000 strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.496999 strmprivacy-api-definitions-3.5.0/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-07-17 07:35:51.496999 strmprivacy-api-definitions-3.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 07:35:51.496999 strmprivacy-api-definitions-3.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-07-17 07:35:28.000000 strmprivacy-api-definitions-3.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.462997 strmprivacy-api-definitions-3.5.0/strmprivacy/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.463997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.463997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/account/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/account/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.464997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/account/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/account/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12198 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/account/v1/account_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16789 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.464997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.466997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3261 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.466997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/audit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/audit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.467997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/audit/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/audit/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/audit/v1/audit_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5030 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/audit/v1/audit_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.467997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/batch_exporters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/batch_exporters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.468997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/batch_exporters/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/batch_exporters/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.468997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/batch_jobs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/batch_jobs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.469997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/batch_jobs/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/batch_jobs/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7665 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10858 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.470997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.470997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/cli/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/cli/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3799 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/cli/v1/cli_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2753 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.470997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/comments/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/comments/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.471997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/comments/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/comments/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3987 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/comments/v1/comments_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6740 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/comments/v1/comments_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.471997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/credentials/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/credentials/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.472997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/credentials/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/credentials/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5049 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/credentials/v1/credentials_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8979 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.472997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/customer_entity_versions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/customer_entity_versions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.473997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/customer_entity_versions/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/customer_entity_versions/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7497 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10288 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.473997 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_connectors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_connectors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.474998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_connectors/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_connectors/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5978 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.474998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_contracts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_contracts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.475998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_contracts/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_contracts/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22634 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28488 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.475998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_subjects/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_subjects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.476998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_subjects/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_subjects/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9499 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9865 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.476998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/entities/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/entities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.477998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/entities/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/entities/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    82471 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/entities/v1/entities_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/entities/v1/entities_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.478998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/entities/v1alpha/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/entities/v1alpha/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12632 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.478998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/event_contracts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/event_contracts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.478998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/event_contracts/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/event_contracts/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15658 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    20098 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.479998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/handles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/handles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.479998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/handles/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/handles/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/handles/v1/handles_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/handles/v1/handles_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.480998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/installations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/installations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.481998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/installations/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/installations/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7909 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/installations/v1/entities_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/installations/v1/entities_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6253 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/installations/v1/installations_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9499 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/installations/v1/installations_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6958 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/installations/v1/installed_components_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10345 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/installations/v1/installed_components_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.481998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_clusters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_clusters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.482998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_clusters/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_clusters/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6199 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9342 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.482998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_exporters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_exporters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.483998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_exporters/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_exporters/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5362 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.483998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_users/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_users/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.484998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_users/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_users/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5369 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8964 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.484998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/key_streams/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/key_streams/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.484998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/key_streams/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/key_streams/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3713 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/key_streams/v1/key_streams_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.485998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/monitoring/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.485998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/monitoring/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/monitoring/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6738 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/monitoring/v1/monitoring_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7722 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/monitoring/v1/monitoring_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.485998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/notifications/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/notifications/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.486998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/notifications/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/notifications/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11948 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/notifications/v1/notifications_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15621 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/notifications/v1/notifications_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.486998 strmprivacy-api-definitions-3.5.0/strmprivacy/api/onboarding/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/onboarding/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.487999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/onboarding/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/onboarding/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3161 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.488999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/organizations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/organizations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.488999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/organizations/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/organizations/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5842 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/organizations/v1/organizations_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9075 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/organizations/v1/organizations_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.488999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/paging/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/paging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.489999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/paging/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/paging/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/paging/v1/paging_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/paging/v1/paging_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.489999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/policies/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.489999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/policies/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/policies/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5782 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/policies/v1/policies_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10449 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/policies/v1/policies_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.489999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/project_plans/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/project_plans/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.490999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/project_plans/v1alpha/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/project_plans/v1alpha/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4521 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7409 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.490999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/projects/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/projects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.490999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/projects/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/projects/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7458 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/projects/v1/projects_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14509 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/projects/v1/projects_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.490999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/purpose_mapping/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/purpose_mapping/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.491999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/purpose_mapping/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/purpose_mapping/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4483 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7407 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.491999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/schemas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/schemas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.491999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/schemas/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/schemas/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13192 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/schemas/v1/schemas_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    17973 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.491999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/sinks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/sinks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.492999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/sinks/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/sinks/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5254 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/sinks/v1/sinks_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8223 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.492999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/streams/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/streams/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.493999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/streams/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/streams/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5689 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/streams/v1/streams_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10437 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.493999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/usage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/usage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.494999 strmprivacy-api-definitions-3.5.0/strmprivacy/api/usage/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 07:35:50.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/usage/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4644 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/usage/v1/usage_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4831 2023-07-17 07:34:53.000000 strmprivacy-api-definitions-3.5.0/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 07:35:51.495999 strmprivacy-api-definitions-3.5.0/strmprivacy_api_definitions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-07-17 07:35:51.000000 strmprivacy-api-definitions-3.5.0/strmprivacy_api_definitions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7436 2023-07-17 07:35:51.000000 strmprivacy-api-definitions-3.5.0/strmprivacy_api_definitions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 07:35:51.000000 strmprivacy-api-definitions-3.5.0/strmprivacy_api_definitions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 07:35:51.000000 strmprivacy-api-definitions-3.5.0/strmprivacy_api_definitions.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-17 07:35:51.000000 strmprivacy-api-definitions-3.5.0/strmprivacy_api_definitions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-17 07:35:51.000000 strmprivacy-api-definitions-3.5.0/strmprivacy_api_definitions.egg-info/top_level.txt
```

### Comparing `strmprivacy-api-definitions-3.4.0/PKG-INFO` & `strmprivacy-api-definitions-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strmprivacy-api-definitions
-Version: 3.4.0
+Version: 3.5.0
 Summary: STRM Privacy API definitions
 Home-page: UNKNOWN
 Author: Stream Machine B.V.
 Author-email: apis@strmprivacy.io
 License: UNKNOWN
 Keywords: strmprivacy api definitions
 Platform: UNKNOWN
```

### Comparing `strmprivacy-api-definitions-3.4.0/setup.py` & `strmprivacy-api-definitions-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/account/v1/account_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/account/v1/account_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/audit/v1/audit_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/audit/v1/audit_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/audit/v1/audit_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/audit/v1/audit_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/cli/v1/cli_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/cli/v1/cli_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/comments/v1/comments_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/comments/v1/comments_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/comments/v1/comments_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/comments/v1/comments_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/credentials/v1/credentials_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/credentials/v1/credentials_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from strmprivacy.api.entities.v1 import entities_v1_pb2 as strmprivacy_dot_api_dot_entities_dot_v1_dot_entities__v1__pb2
 from validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n9strmprivacy/api/data_contracts/v1/data_contracts_v1.proto\x12!strmprivacy.api.data_contracts.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a google/protobuf/field_mask.proto\x1a-strmprivacy/api/entities/v1/entities_v1.proto\x1a\x17validate/validate.proto\"\x84\x03\n\x18ListDataContractsRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x16\n\x06\x66ilter\x18\x02 \x01(\tR\x06\x66ilter\x12\x16\n\x06handle\x18\x03 \x01(\tR\x06handle\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12W\n\x0epublic_private\x18\x05 \x01(\x0e\x32\x30.strmprivacy.api.entities.v1.FilterPublicPrivateR\rpublicPrivate\x12:\n\x06labels\x18\x07 \x03(\x0b\x32\".strmprivacy.api.entities.v1.LabelR\x06labels\x12\x18\n\x07\x64omains\x18\x08 \x03(\tR\x07\x64omains\x12\x1e\n\nindustries\x18\t \x03(\tR\nindustries\x12\'\n\nproject_id\x18\n \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\x9b\x03\n\x19ListDataContractsResponse\x12T\n\x0e\x64\x61ta_contracts\x18\x01 \x03(\x0b\x32).strmprivacy.api.entities.v1.DataContractB\x02\x18\x01R\rdataContracts\x12\x95\x01\n\x1c\x64\x61ta_contracts_and_checksums\x18\x02 \x03(\x0b\x32T.strmprivacy.api.data_contracts.v1.ListDataContractsResponse.DataContractAndChecksumR\x19\x64\x61taContractsAndChecksums\x1a\x8f\x01\n\x17\x44\x61taContractAndChecksum\x12S\n\rdata_contract\x18\x01 \x01(\x0b\x32).strmprivacy.api.entities.v1.DataContractB\x03\xe0\x41\x02R\x0c\x64\x61taContract\x12\x1f\n\x08\x63hecksum\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x08\x63hecksum\"\x96\x01\n\x16GetDataContractRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12>\n\x03ref\x18\x02 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefR\x03ref\x12\x0e\n\x02id\x18\x03 \x01(\tR\x02id\"\x8f\x01\n\x17GetDataContractResponse\x12S\n\rdata_contract\x18\x01 \x01(\x0b\x32).strmprivacy.api.entities.v1.DataContractB\x03\xe0\x41\x02R\x0c\x64\x61taContract\x12\x1f\n\x08\x63hecksum\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x08\x63hecksum\"\xcc\x01\n\x19\x43reateDataContractRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12X\n\rdata_contract\x18\x02 \x01(\x0b\x32).strmprivacy.api.entities.v1.DataContractB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0c\x64\x61taContract\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\x92\x01\n\x1a\x43reateDataContractResponse\x12S\n\rdata_contract\x18\x01 \x01(\x0b\x32).strmprivacy.api.entities.v1.DataContractB\x03\xe0\x41\x02R\x0c\x64\x61taContract\x12\x1f\n\x08\x63hecksum\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x08\x63hecksum\"\xfc\x03\n\x19UpdateDataContractRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12X\n\rdata_contract\x18\x02 \x01(\x0b\x32).strmprivacy.api.entities.v1.DataContractB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0c\x64\x61taContract\x12#\n\x08\x63hecksum\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08\x63hecksum\x12\x45\n\x0bupdate_mask\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\nupdateMask\x12~\n\x13\x63onsole_wizard_step\x18\x05 \x01(\x0e\x32N.strmprivacy.api.data_contracts.v1.UpdateDataContractRequest.ConsoleWizardStepR\x11\x63onsoleWizardStep\"k\n\x11\x43onsoleWizardStep\x12#\n\x1f\x43ONSOLE_WIZARD_STEP_UNSPECIFIED\x10\x00\x12\n\n\x06SCHEMA\x10\x01\x12\x12\n\x0e\x45VENT_CONTRACT\x10\x02\x12\x11\n\rDATA_CONTRACT\x10\x03\"\x92\x01\n\x1aUpdateDataContractResponse\x12S\n\rdata_contract\x18\x01 \x01(\x0b\x32).strmprivacy.api.entities.v1.DataContractB\x03\xe0\x41\x02R\x0c\x64\x61taContract\x12\x1f\n\x08\x63hecksum\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x08\x63hecksum\"\xa4\x02\n\x19ReviewDataContractRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02id\x12X\n\x11\x64\x61ta_contract_ref\x18\x03 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefR\x0f\x64\x61taContractRef\x12\x46\n\x19\x61pprover_external_user_id\x18\x04 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x16\x61pproverExternalUserId\x12\'\n\x0fnotify_reviewer\x18\x05 \x01(\x08R\x0enotifyReviewer\"\x1c\n\x1aReviewDataContractResponse\"\xad\x01\n\x1a\x41pproveDataContractRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12X\n\x11\x64\x61ta_contract_ref\x18\x02 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefR\x0f\x64\x61taContractRef\x12%\n\x0enotify_creator\x18\x03 \x01(\x08R\rnotifyCreator\"\x1d\n\x1b\x41pproveDataContractResponse\"\xb5\x01\n\x1b\x41\x63tivateDataContractRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02id\x12X\n\x11\x64\x61ta_contract_ref\x18\x03 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefR\x0f\x64\x61taContractRef\"\x1e\n\x1c\x41\x63tivateDataContractResponse\"\xdc\x01\n\x19\x44\x65leteDataContractRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02id\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\x12X\n\x11\x64\x61ta_contract_ref\x18\x04 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefR\x0f\x64\x61taContractRef\"\x1c\n\x1a\x44\x65leteDataContractResponse\"\xb4\x01\n\x1a\x41rchiveDataContractRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02id\x12X\n\x11\x64\x61ta_contract_ref\x18\x03 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefR\x0f\x64\x61taContractRef\"\x1d\n\x1b\x41rchiveDataContractResponse\"\xb2\x01\n(ValidateDataContractsMaskedFieldsRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12X\n\rmasked_fields\x18\x02 \x01(\x0b\x32).strmprivacy.api.entities.v1.MaskedFieldsB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0cmaskedFields\"\x92\x04\n)ValidateDataContractsMaskedFieldsResponse\x12j\n\x06\x65rrors\x18\x01 \x03(\x0b\x32R.strmprivacy.api.data_contracts.v1.ValidateDataContractsMaskedFieldsResponse.ErrorR\x06\x65rrors\x1a\xf8\x02\n\x05\x45rror\x12\x13\n\x02id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x02id\x12]\n\x11\x64\x61ta_contract_ref\x18\x02 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefB\x03\xe0\x41\x02R\x0f\x64\x61taContractRef\x12\x18\n\x07message\x18\x03 \x01(\tR\x07message\x12u\n\x06\x65rrors\x18\x04 \x03(\x0b\x32].strmprivacy.api.data_contracts.v1.ValidateDataContractsMaskedFieldsResponse.Error.FieldErrorR\x06\x65rrors\x1aj\n\nFieldError\x12#\n\rfield_pattern\x18\x01 \x01(\tR\x0c\x66ieldPattern\x12\x1d\n\nfield_type\x18\x02 \x01(\tR\tfieldType\x12\x18\n\x07message\x18\x03 \x01(\tR\x07message\"\xfd\x01\n GetDataContractSchemaCodeRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02id\x12\x41\n\x08language\x18\x03 \x01(\tB%\xfa\x42\"r R\x04javaR\ntypescriptR\x06pythonR\x04rustR\x08language\x12X\n\x11\x64\x61ta_contract_ref\x18\x04 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefR\x0f\x64\x61taContractRef\"\x7f\n!GetDataContractSchemaCodeResponse\x12\x1f\n\x08\x66ilename\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x08\x66ilename\x12 \n\tdata_size\x18\x02 \x01(\x03\x42\x03\xe0\x41\x02R\x08\x64\x61taSize\x12\x17\n\x04\x64\x61ta\x18\x03 \x01(\x0c\x42\x03\xe0\x41\x02R\x04\x64\x61ta\"\x9a\x01\n&GetDataContractSchemaDefinitionRequest\x12!\n\x0c\x63onfluent_id\x18\x01 \x01(\x05R\x0b\x63onfluentId\x12M\n\x0b\x63luster_ref\x18\x02 \x01(\x0b\x32,.strmprivacy.api.entities.v1.KafkaClusterRefR\nclusterRef\"N\n\'GetDataContractSchemaDefinitionResponse\x12#\n\ndefinition\x18\x01 \x01(\tB\x03\xe0\x41\x02R\ndefinition\"\x9b\x01\n\x19SimpleSchemaDryRunRequest\x12~\n\x18simple_schema_definition\x18\x01 \x01(\x0b\x32:.strmprivacy.api.entities.v1.Schema.SimpleSchemaDefinitionB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x16simpleSchemaDefinition\"\x97\x01\n\x1aSimpleSchemaDryRunResponse\x12y\n\x18simple_schema_definition\x18\x01 \x01(\x0b\x32:.strmprivacy.api.entities.v1.Schema.SimpleSchemaDefinitionB\x03\xe0\x41\x02R\x16simpleSchemaDefinition2\x83\x10\n\x14\x44\x61taContractsService\x12\x8e\x01\n\x11ListDataContracts\x12;.strmprivacy.api.data_contracts.v1.ListDataContractsRequest\x1a<.strmprivacy.api.data_contracts.v1.ListDataContractsResponse\x12\x88\x01\n\x0fGetDataContract\x12\x39.strmprivacy.api.data_contracts.v1.GetDataContractRequest\x1a:.strmprivacy.api.data_contracts.v1.GetDataContractResponse\x12\x91\x01\n\x12\x43reateDataContract\x12<.strmprivacy.api.data_contracts.v1.CreateDataContractRequest\x1a=.strmprivacy.api.data_contracts.v1.CreateDataContractResponse\x12\x91\x01\n\x12UpdateDataContract\x12<.strmprivacy.api.data_contracts.v1.UpdateDataContractRequest\x1a=.strmprivacy.api.data_contracts.v1.UpdateDataContractResponse\x12\x91\x01\n\x12ReviewDataContract\x12<.strmprivacy.api.data_contracts.v1.ReviewDataContractRequest\x1a=.strmprivacy.api.data_contracts.v1.ReviewDataContractResponse\x12\x97\x01\n\x14\x41\x63tivateDataContract\x12>.strmprivacy.api.data_contracts.v1.ActivateDataContractRequest\x1a?.strmprivacy.api.data_contracts.v1.ActivateDataContractResponse\x12\x91\x01\n\x12\x44\x65leteDataContract\x12<.strmprivacy.api.data_contracts.v1.DeleteDataContractRequest\x1a=.strmprivacy.api.data_contracts.v1.DeleteDataContractResponse\x12\x94\x01\n\x13\x41rchiveDataContract\x12=.strmprivacy.api.data_contracts.v1.ArchiveDataContractRequest\x1a>.strmprivacy.api.data_contracts.v1.ArchiveDataContractResponse\x12\x94\x01\n\x13\x41pproveDataContract\x12=.strmprivacy.api.data_contracts.v1.ApproveDataContractRequest\x1a>.strmprivacy.api.data_contracts.v1.ApproveDataContractResponse\x12\xa6\x01\n\x19GetDataContractSchemaCode\x12\x43.strmprivacy.api.data_contracts.v1.GetDataContractSchemaCodeRequest\x1a\x44.strmprivacy.api.data_contracts.v1.GetDataContractSchemaCodeResponse\x12\xb8\x01\n\x1fGetDataContractSchemaDefinition\x12I.strmprivacy.api.data_contracts.v1.GetDataContractSchemaDefinitionRequest\x1aJ.strmprivacy.api.data_contracts.v1.GetDataContractSchemaDefinitionResponse\x12\xbe\x01\n!ValidateDataContractsMaskedFields\x12K.strmprivacy.api.data_contracts.v1.ValidateDataContractsMaskedFieldsRequest\x1aL.strmprivacy.api.data_contracts.v1.ValidateDataContractsMaskedFieldsResponse\x12\x91\x01\n\x12SimpleSchemaDryRun\x12<.strmprivacy.api.data_contracts.v1.SimpleSchemaDryRunRequest\x1a=.strmprivacy.api.data_contracts.v1.SimpleSchemaDryRunResponseB{\n$io.strmprivacy.api.data_contracts.v1P\x01ZQgithub.com/strmprivacy/api-definitions-go/v2/api/data_contracts/v1;data_contractsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n9strmprivacy/api/data_contracts/v1/data_contracts_v1.proto\x12!strmprivacy.api.data_contracts.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a google/protobuf/field_mask.proto\x1a-strmprivacy/api/entities/v1/entities_v1.proto\x1a\x17validate/validate.proto\"\x84\x03\n\x18ListDataContractsRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x16\n\x06\x66ilter\x18\x02 \x01(\tR\x06\x66ilter\x12\x16\n\x06handle\x18\x03 \x01(\tR\x06handle\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12W\n\x0epublic_private\x18\x05 \x01(\x0e\x32\x30.strmprivacy.api.entities.v1.FilterPublicPrivateR\rpublicPrivate\x12:\n\x06labels\x18\x07 \x03(\x0b\x32\".strmprivacy.api.entities.v1.LabelR\x06labels\x12\x18\n\x07\x64omains\x18\x08 \x03(\tR\x07\x64omains\x12\x1e\n\nindustries\x18\t \x03(\tR\nindustries\x12\'\n\nproject_id\x18\n \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\x9b\x03\n\x19ListDataContractsResponse\x12T\n\x0e\x64\x61ta_contracts\x18\x01 \x03(\x0b\x32).strmprivacy.api.entities.v1.DataContractB\x02\x18\x01R\rdataContracts\x12\x95\x01\n\x1c\x64\x61ta_contracts_and_checksums\x18\x02 \x03(\x0b\x32T.strmprivacy.api.data_contracts.v1.ListDataContractsResponse.DataContractAndChecksumR\x19\x64\x61taContractsAndChecksums\x1a\x8f\x01\n\x17\x44\x61taContractAndChecksum\x12S\n\rdata_contract\x18\x01 \x01(\x0b\x32).strmprivacy.api.entities.v1.DataContractB\x03\xe0\x41\x02R\x0c\x64\x61taContract\x12\x1f\n\x08\x63hecksum\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x08\x63hecksum\"\x96\x01\n\x16GetDataContractRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12>\n\x03ref\x18\x02 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefR\x03ref\x12\x0e\n\x02id\x18\x03 \x01(\tR\x02id\"\x8f\x01\n\x17GetDataContractResponse\x12S\n\rdata_contract\x18\x01 \x01(\x0b\x32).strmprivacy.api.entities.v1.DataContractB\x03\xe0\x41\x02R\x0c\x64\x61taContract\x12\x1f\n\x08\x63hecksum\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x08\x63hecksum\"\xcc\x01\n\x19\x43reateDataContractRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12X\n\rdata_contract\x18\x02 \x01(\x0b\x32).strmprivacy.api.entities.v1.DataContractB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0c\x64\x61taContract\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\x92\x01\n\x1a\x43reateDataContractResponse\x12S\n\rdata_contract\x18\x01 \x01(\x0b\x32).strmprivacy.api.entities.v1.DataContractB\x03\xe0\x41\x02R\x0c\x64\x61taContract\x12\x1f\n\x08\x63hecksum\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x08\x63hecksum\"\xf2\x03\n\x19UpdateDataContractRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12X\n\rdata_contract\x18\x02 \x01(\x0b\x32).strmprivacy.api.entities.v1.DataContractB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0c\x64\x61taContract\x12#\n\x08\x63hecksum\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08\x63hecksum\x12;\n\x0bupdate_mask\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskR\nupdateMask\x12~\n\x13\x63onsole_wizard_step\x18\x05 \x01(\x0e\x32N.strmprivacy.api.data_contracts.v1.UpdateDataContractRequest.ConsoleWizardStepR\x11\x63onsoleWizardStep\"k\n\x11\x43onsoleWizardStep\x12#\n\x1f\x43ONSOLE_WIZARD_STEP_UNSPECIFIED\x10\x00\x12\n\n\x06SCHEMA\x10\x01\x12\x12\n\x0e\x45VENT_CONTRACT\x10\x02\x12\x11\n\rDATA_CONTRACT\x10\x03\"\x92\x01\n\x1aUpdateDataContractResponse\x12S\n\rdata_contract\x18\x01 \x01(\x0b\x32).strmprivacy.api.entities.v1.DataContractB\x03\xe0\x41\x02R\x0c\x64\x61taContract\x12\x1f\n\x08\x63hecksum\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x08\x63hecksum\"\xa4\x02\n\x19ReviewDataContractRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02id\x12X\n\x11\x64\x61ta_contract_ref\x18\x03 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefR\x0f\x64\x61taContractRef\x12\x46\n\x19\x61pprover_external_user_id\x18\x04 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x16\x61pproverExternalUserId\x12\'\n\x0fnotify_reviewer\x18\x05 \x01(\x08R\x0enotifyReviewer\"\x1c\n\x1aReviewDataContractResponse\"\xad\x01\n\x1a\x41pproveDataContractRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12X\n\x11\x64\x61ta_contract_ref\x18\x02 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefR\x0f\x64\x61taContractRef\x12%\n\x0enotify_creator\x18\x03 \x01(\x08R\rnotifyCreator\"\x1d\n\x1b\x41pproveDataContractResponse\"\xb5\x01\n\x1b\x41\x63tivateDataContractRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02id\x12X\n\x11\x64\x61ta_contract_ref\x18\x03 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefR\x0f\x64\x61taContractRef\"\x1e\n\x1c\x41\x63tivateDataContractResponse\"\xdc\x01\n\x19\x44\x65leteDataContractRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02id\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\x12X\n\x11\x64\x61ta_contract_ref\x18\x04 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefR\x0f\x64\x61taContractRef\"\x1c\n\x1a\x44\x65leteDataContractResponse\"\xb4\x01\n\x1a\x41rchiveDataContractRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02id\x12X\n\x11\x64\x61ta_contract_ref\x18\x03 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefR\x0f\x64\x61taContractRef\"\x1d\n\x1b\x41rchiveDataContractResponse\"\xb2\x01\n(ValidateDataContractsMaskedFieldsRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12X\n\rmasked_fields\x18\x02 \x01(\x0b\x32).strmprivacy.api.entities.v1.MaskedFieldsB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0cmaskedFields\"\x92\x04\n)ValidateDataContractsMaskedFieldsResponse\x12j\n\x06\x65rrors\x18\x01 \x03(\x0b\x32R.strmprivacy.api.data_contracts.v1.ValidateDataContractsMaskedFieldsResponse.ErrorR\x06\x65rrors\x1a\xf8\x02\n\x05\x45rror\x12\x13\n\x02id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x02id\x12]\n\x11\x64\x61ta_contract_ref\x18\x02 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefB\x03\xe0\x41\x02R\x0f\x64\x61taContractRef\x12\x18\n\x07message\x18\x03 \x01(\tR\x07message\x12u\n\x06\x65rrors\x18\x04 \x03(\x0b\x32].strmprivacy.api.data_contracts.v1.ValidateDataContractsMaskedFieldsResponse.Error.FieldErrorR\x06\x65rrors\x1aj\n\nFieldError\x12#\n\rfield_pattern\x18\x01 \x01(\tR\x0c\x66ieldPattern\x12\x1d\n\nfield_type\x18\x02 \x01(\tR\tfieldType\x12\x18\n\x07message\x18\x03 \x01(\tR\x07message\"\xfd\x01\n GetDataContractSchemaCodeRequest\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02id\x12\x41\n\x08language\x18\x03 \x01(\tB%\xfa\x42\"r R\x04javaR\ntypescriptR\x06pythonR\x04rustR\x08language\x12X\n\x11\x64\x61ta_contract_ref\x18\x04 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefR\x0f\x64\x61taContractRef\"\x7f\n!GetDataContractSchemaCodeResponse\x12\x1f\n\x08\x66ilename\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x08\x66ilename\x12 \n\tdata_size\x18\x02 \x01(\x03\x42\x03\xe0\x41\x02R\x08\x64\x61taSize\x12\x17\n\x04\x64\x61ta\x18\x03 \x01(\x0c\x42\x03\xe0\x41\x02R\x04\x64\x61ta\"\x9a\x01\n&GetDataContractSchemaDefinitionRequest\x12!\n\x0c\x63onfluent_id\x18\x01 \x01(\x05R\x0b\x63onfluentId\x12M\n\x0b\x63luster_ref\x18\x02 \x01(\x0b\x32,.strmprivacy.api.entities.v1.KafkaClusterRefR\nclusterRef\"N\n\'GetDataContractSchemaDefinitionResponse\x12#\n\ndefinition\x18\x01 \x01(\tB\x03\xe0\x41\x02R\ndefinition\"\x9b\x01\n\x19SimpleSchemaDryRunRequest\x12~\n\x18simple_schema_definition\x18\x01 \x01(\x0b\x32:.strmprivacy.api.entities.v1.Schema.SimpleSchemaDefinitionB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x16simpleSchemaDefinition\"\x97\x01\n\x1aSimpleSchemaDryRunResponse\x12y\n\x18simple_schema_definition\x18\x01 \x01(\x0b\x32:.strmprivacy.api.entities.v1.Schema.SimpleSchemaDefinitionB\x03\xe0\x41\x02R\x16simpleSchemaDefinition2\x83\x10\n\x14\x44\x61taContractsService\x12\x8e\x01\n\x11ListDataContracts\x12;.strmprivacy.api.data_contracts.v1.ListDataContractsRequest\x1a<.strmprivacy.api.data_contracts.v1.ListDataContractsResponse\x12\x88\x01\n\x0fGetDataContract\x12\x39.strmprivacy.api.data_contracts.v1.GetDataContractRequest\x1a:.strmprivacy.api.data_contracts.v1.GetDataContractResponse\x12\x91\x01\n\x12\x43reateDataContract\x12<.strmprivacy.api.data_contracts.v1.CreateDataContractRequest\x1a=.strmprivacy.api.data_contracts.v1.CreateDataContractResponse\x12\x91\x01\n\x12UpdateDataContract\x12<.strmprivacy.api.data_contracts.v1.UpdateDataContractRequest\x1a=.strmprivacy.api.data_contracts.v1.UpdateDataContractResponse\x12\x91\x01\n\x12ReviewDataContract\x12<.strmprivacy.api.data_contracts.v1.ReviewDataContractRequest\x1a=.strmprivacy.api.data_contracts.v1.ReviewDataContractResponse\x12\x97\x01\n\x14\x41\x63tivateDataContract\x12>.strmprivacy.api.data_contracts.v1.ActivateDataContractRequest\x1a?.strmprivacy.api.data_contracts.v1.ActivateDataContractResponse\x12\x91\x01\n\x12\x44\x65leteDataContract\x12<.strmprivacy.api.data_contracts.v1.DeleteDataContractRequest\x1a=.strmprivacy.api.data_contracts.v1.DeleteDataContractResponse\x12\x94\x01\n\x13\x41rchiveDataContract\x12=.strmprivacy.api.data_contracts.v1.ArchiveDataContractRequest\x1a>.strmprivacy.api.data_contracts.v1.ArchiveDataContractResponse\x12\x94\x01\n\x13\x41pproveDataContract\x12=.strmprivacy.api.data_contracts.v1.ApproveDataContractRequest\x1a>.strmprivacy.api.data_contracts.v1.ApproveDataContractResponse\x12\xa6\x01\n\x19GetDataContractSchemaCode\x12\x43.strmprivacy.api.data_contracts.v1.GetDataContractSchemaCodeRequest\x1a\x44.strmprivacy.api.data_contracts.v1.GetDataContractSchemaCodeResponse\x12\xb8\x01\n\x1fGetDataContractSchemaDefinition\x12I.strmprivacy.api.data_contracts.v1.GetDataContractSchemaDefinitionRequest\x1aJ.strmprivacy.api.data_contracts.v1.GetDataContractSchemaDefinitionResponse\x12\xbe\x01\n!ValidateDataContractsMaskedFields\x12K.strmprivacy.api.data_contracts.v1.ValidateDataContractsMaskedFieldsRequest\x1aL.strmprivacy.api.data_contracts.v1.ValidateDataContractsMaskedFieldsResponse\x12\x91\x01\n\x12SimpleSchemaDryRun\x12<.strmprivacy.api.data_contracts.v1.SimpleSchemaDryRunRequest\x1a=.strmprivacy.api.data_contracts.v1.SimpleSchemaDryRunResponseB{\n$io.strmprivacy.api.data_contracts.v1P\x01ZQgithub.com/strmprivacy/api-definitions-go/v2/api/data_contracts/v1;data_contractsb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'strmprivacy.api.data_contracts.v1.data_contracts_v1_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n$io.strmprivacy.api.data_contracts.v1P\001ZQgithub.com/strmprivacy/api-definitions-go/v2/api/data_contracts/v1;data_contracts'
@@ -53,16 +53,14 @@
   _CREATEDATACONTRACTRESPONSE.fields_by_name['checksum']._serialized_options = b'\340A\002'
   _UPDATEDATACONTRACTREQUEST.fields_by_name['billing_id']._options = None
   _UPDATEDATACONTRACTREQUEST.fields_by_name['billing_id']._serialized_options = b'\030\001\372B\010r\006\230\001\000\320\001\001'
   _UPDATEDATACONTRACTREQUEST.fields_by_name['data_contract']._options = None
   _UPDATEDATACONTRACTREQUEST.fields_by_name['data_contract']._serialized_options = b'\372B\005\212\001\002\020\001'
   _UPDATEDATACONTRACTREQUEST.fields_by_name['checksum']._options = None
   _UPDATEDATACONTRACTREQUEST.fields_by_name['checksum']._serialized_options = b'\372B\004r\002\020\001'
-  _UPDATEDATACONTRACTREQUEST.fields_by_name['update_mask']._options = None
-  _UPDATEDATACONTRACTREQUEST.fields_by_name['update_mask']._serialized_options = b'\372B\005\212\001\002\020\001'
   _UPDATEDATACONTRACTRESPONSE.fields_by_name['data_contract']._options = None
   _UPDATEDATACONTRACTRESPONSE.fields_by_name['data_contract']._serialized_options = b'\340A\002'
   _UPDATEDATACONTRACTRESPONSE.fields_by_name['checksum']._options = None
   _UPDATEDATACONTRACTRESPONSE.fields_by_name['checksum']._serialized_options = b'\340A\002'
   _REVIEWDATACONTRACTREQUEST.fields_by_name['billing_id']._options = None
   _REVIEWDATACONTRACTREQUEST.fields_by_name['billing_id']._serialized_options = b'\030\001\372B\010r\006\230\001\000\320\001\001'
   _REVIEWDATACONTRACTREQUEST.fields_by_name['approver_external_user_id']._options = None
@@ -110,55 +108,55 @@
   _GETDATACONTRACTRESPONSE._serialized_start=1194
   _GETDATACONTRACTRESPONSE._serialized_end=1337
   _CREATEDATACONTRACTREQUEST._serialized_start=1340
   _CREATEDATACONTRACTREQUEST._serialized_end=1544
   _CREATEDATACONTRACTRESPONSE._serialized_start=1547
   _CREATEDATACONTRACTRESPONSE._serialized_end=1693
   _UPDATEDATACONTRACTREQUEST._serialized_start=1696
-  _UPDATEDATACONTRACTREQUEST._serialized_end=2204
-  _UPDATEDATACONTRACTREQUEST_CONSOLEWIZARDSTEP._serialized_start=2097
-  _UPDATEDATACONTRACTREQUEST_CONSOLEWIZARDSTEP._serialized_end=2204
-  _UPDATEDATACONTRACTRESPONSE._serialized_start=2207
-  _UPDATEDATACONTRACTRESPONSE._serialized_end=2353
-  _REVIEWDATACONTRACTREQUEST._serialized_start=2356
-  _REVIEWDATACONTRACTREQUEST._serialized_end=2648
-  _REVIEWDATACONTRACTRESPONSE._serialized_start=2650
-  _REVIEWDATACONTRACTRESPONSE._serialized_end=2678
-  _APPROVEDATACONTRACTREQUEST._serialized_start=2681
-  _APPROVEDATACONTRACTREQUEST._serialized_end=2854
-  _APPROVEDATACONTRACTRESPONSE._serialized_start=2856
-  _APPROVEDATACONTRACTRESPONSE._serialized_end=2885
-  _ACTIVATEDATACONTRACTREQUEST._serialized_start=2888
-  _ACTIVATEDATACONTRACTREQUEST._serialized_end=3069
-  _ACTIVATEDATACONTRACTRESPONSE._serialized_start=3071
-  _ACTIVATEDATACONTRACTRESPONSE._serialized_end=3101
-  _DELETEDATACONTRACTREQUEST._serialized_start=3104
-  _DELETEDATACONTRACTREQUEST._serialized_end=3324
-  _DELETEDATACONTRACTRESPONSE._serialized_start=3326
-  _DELETEDATACONTRACTRESPONSE._serialized_end=3354
-  _ARCHIVEDATACONTRACTREQUEST._serialized_start=3357
-  _ARCHIVEDATACONTRACTREQUEST._serialized_end=3537
-  _ARCHIVEDATACONTRACTRESPONSE._serialized_start=3539
-  _ARCHIVEDATACONTRACTRESPONSE._serialized_end=3568
-  _VALIDATEDATACONTRACTSMASKEDFIELDSREQUEST._serialized_start=3571
-  _VALIDATEDATACONTRACTSMASKEDFIELDSREQUEST._serialized_end=3749
-  _VALIDATEDATACONTRACTSMASKEDFIELDSRESPONSE._serialized_start=3752
-  _VALIDATEDATACONTRACTSMASKEDFIELDSRESPONSE._serialized_end=4282
-  _VALIDATEDATACONTRACTSMASKEDFIELDSRESPONSE_ERROR._serialized_start=3906
-  _VALIDATEDATACONTRACTSMASKEDFIELDSRESPONSE_ERROR._serialized_end=4282
-  _VALIDATEDATACONTRACTSMASKEDFIELDSRESPONSE_ERROR_FIELDERROR._serialized_start=4176
-  _VALIDATEDATACONTRACTSMASKEDFIELDSRESPONSE_ERROR_FIELDERROR._serialized_end=4282
-  _GETDATACONTRACTSCHEMACODEREQUEST._serialized_start=4285
-  _GETDATACONTRACTSCHEMACODEREQUEST._serialized_end=4538
-  _GETDATACONTRACTSCHEMACODERESPONSE._serialized_start=4540
-  _GETDATACONTRACTSCHEMACODERESPONSE._serialized_end=4667
-  _GETDATACONTRACTSCHEMADEFINITIONREQUEST._serialized_start=4670
-  _GETDATACONTRACTSCHEMADEFINITIONREQUEST._serialized_end=4824
-  _GETDATACONTRACTSCHEMADEFINITIONRESPONSE._serialized_start=4826
-  _GETDATACONTRACTSCHEMADEFINITIONRESPONSE._serialized_end=4904
-  _SIMPLESCHEMADRYRUNREQUEST._serialized_start=4907
-  _SIMPLESCHEMADRYRUNREQUEST._serialized_end=5062
-  _SIMPLESCHEMADRYRUNRESPONSE._serialized_start=5065
-  _SIMPLESCHEMADRYRUNRESPONSE._serialized_end=5216
-  _DATACONTRACTSSERVICE._serialized_start=5219
-  _DATACONTRACTSSERVICE._serialized_end=7270
+  _UPDATEDATACONTRACTREQUEST._serialized_end=2194
+  _UPDATEDATACONTRACTREQUEST_CONSOLEWIZARDSTEP._serialized_start=2087
+  _UPDATEDATACONTRACTREQUEST_CONSOLEWIZARDSTEP._serialized_end=2194
+  _UPDATEDATACONTRACTRESPONSE._serialized_start=2197
+  _UPDATEDATACONTRACTRESPONSE._serialized_end=2343
+  _REVIEWDATACONTRACTREQUEST._serialized_start=2346
+  _REVIEWDATACONTRACTREQUEST._serialized_end=2638
+  _REVIEWDATACONTRACTRESPONSE._serialized_start=2640
+  _REVIEWDATACONTRACTRESPONSE._serialized_end=2668
+  _APPROVEDATACONTRACTREQUEST._serialized_start=2671
+  _APPROVEDATACONTRACTREQUEST._serialized_end=2844
+  _APPROVEDATACONTRACTRESPONSE._serialized_start=2846
+  _APPROVEDATACONTRACTRESPONSE._serialized_end=2875
+  _ACTIVATEDATACONTRACTREQUEST._serialized_start=2878
+  _ACTIVATEDATACONTRACTREQUEST._serialized_end=3059
+  _ACTIVATEDATACONTRACTRESPONSE._serialized_start=3061
+  _ACTIVATEDATACONTRACTRESPONSE._serialized_end=3091
+  _DELETEDATACONTRACTREQUEST._serialized_start=3094
+  _DELETEDATACONTRACTREQUEST._serialized_end=3314
+  _DELETEDATACONTRACTRESPONSE._serialized_start=3316
+  _DELETEDATACONTRACTRESPONSE._serialized_end=3344
+  _ARCHIVEDATACONTRACTREQUEST._serialized_start=3347
+  _ARCHIVEDATACONTRACTREQUEST._serialized_end=3527
+  _ARCHIVEDATACONTRACTRESPONSE._serialized_start=3529
+  _ARCHIVEDATACONTRACTRESPONSE._serialized_end=3558
+  _VALIDATEDATACONTRACTSMASKEDFIELDSREQUEST._serialized_start=3561
+  _VALIDATEDATACONTRACTSMASKEDFIELDSREQUEST._serialized_end=3739
+  _VALIDATEDATACONTRACTSMASKEDFIELDSRESPONSE._serialized_start=3742
+  _VALIDATEDATACONTRACTSMASKEDFIELDSRESPONSE._serialized_end=4272
+  _VALIDATEDATACONTRACTSMASKEDFIELDSRESPONSE_ERROR._serialized_start=3896
+  _VALIDATEDATACONTRACTSMASKEDFIELDSRESPONSE_ERROR._serialized_end=4272
+  _VALIDATEDATACONTRACTSMASKEDFIELDSRESPONSE_ERROR_FIELDERROR._serialized_start=4166
+  _VALIDATEDATACONTRACTSMASKEDFIELDSRESPONSE_ERROR_FIELDERROR._serialized_end=4272
+  _GETDATACONTRACTSCHEMACODEREQUEST._serialized_start=4275
+  _GETDATACONTRACTSCHEMACODEREQUEST._serialized_end=4528
+  _GETDATACONTRACTSCHEMACODERESPONSE._serialized_start=4530
+  _GETDATACONTRACTSCHEMACODERESPONSE._serialized_end=4657
+  _GETDATACONTRACTSCHEMADEFINITIONREQUEST._serialized_start=4660
+  _GETDATACONTRACTSCHEMADEFINITIONREQUEST._serialized_end=4814
+  _GETDATACONTRACTSCHEMADEFINITIONRESPONSE._serialized_start=4816
+  _GETDATACONTRACTSCHEMADEFINITIONRESPONSE._serialized_end=4894
+  _SIMPLESCHEMADRYRUNREQUEST._serialized_start=4897
+  _SIMPLESCHEMADRYRUNREQUEST._serialized_end=5052
+  _SIMPLESCHEMADRYRUNRESPONSE._serialized_start=5055
+  _SIMPLESCHEMADRYRUNRESPONSE._serialized_end=5206
+  _DATACONTRACTSSERVICE._serialized_start=5209
+  _DATACONTRACTSSERVICE._serialized_end=7260
 # @@protoc_insertion_point(module_scope)
```

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1/entities_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/entities/v1/entities_v1_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.type import datetime_pb2 as google_dot_type_dot_datetime__pb2
 from validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-strmprivacy/api/entities/v1/entities_v1.proto\x12\x1bstrmprivacy.api.entities.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1agoogle/type/datetime.proto\x1a\x17validate/validate.proto\"\xab\x05\n\x06Stream\x12\x45\n\x03ref\x18\x01 \x01(\x0b\x32&.strmprivacy.api.entities.v1.StreamRefB\x0b\xe0\x41\x02\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12-\n\x0b\x64\x65scription\x18\x02 \x01(\tB\x0b\xfa\x42\x08r\x06\x18\xe8\x07\xd0\x01\x01R\x0b\x64\x65scription\x12/\n\x0e\x63onsent_levels\x18\x03 \x03(\x05\x42\x08\xfa\x42\x05\x92\x01\x02\x10\x32R\rconsentLevels\x12[\n\x12\x63onsent_level_type\x18\x04 \x01(\x0e\x32-.strmprivacy.api.entities.v1.ConsentLevelTypeR\x10\x63onsentLevelType\x12\x1d\n\x07\x65nabled\x18\x05 \x01(\x08\x42\x03\xe0\x41\x03R\x07\x65nabled\x12@\n\x06limits\x18\x06 \x01(\x0b\x32#.strmprivacy.api.entities.v1.LimitsB\x03\xe0\x41\x03R\x06limits\x12#\n\rlinked_stream\x18\x07 \x01(\tR\x0clinkedStream\x12$\n\x04tags\x18\x08 \x03(\tB\x10\xfa\x42\r\x92\x01\n\x10\x14\x18\x01\"\x04r\x02\x18\x64R\x04tags\x12O\n\x0b\x63redentials\x18\t \x03(\x0b\x32(.strmprivacy.api.entities.v1.CredentialsB\x03\xe0\x41\x03R\x0b\x63redentials\x12N\n\rmasked_fields\x18\n \x01(\x0b\x32).strmprivacy.api.entities.v1.MaskedFieldsR\x0cmaskedFields\x12&\n\x0bkafka_topic\x18\x0b \x01(\tB\x05\x18\x01\xe0\x41\x03R\nkafkaTopic\x12(\n\tpolicy_id\x18\x0c \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x08policyId\"\xaa\x01\n\x0e\x45xtendedStream\x12@\n\x06stream\x18\x01 \x01(\x0b\x32#.strmprivacy.api.entities.v1.StreamB\x03\xe0\x41\x03R\x06stream\x12\x19\n\x05topic\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x05topic\x12\x17\n\x04uuid\x18\x03 \x01(\tB\x03\xe0\x41\x03R\x04uuid\x12\"\n\nkey_stream\x18\x04 \x01(\x08\x42\x03\xe0\x41\x03R\tkeyStream\"\xc2\x01\n\x13\x45xtendedStreamGroup\x12U\n\rsource_stream\x18\x01 \x01(\x0b\x32+.strmprivacy.api.entities.v1.ExtendedStreamB\x03\xe0\x41\x03R\x0csourceStream\x12T\n\x0f\x64\x65rived_streams\x18\x02 \x03(\x0b\x32+.strmprivacy.api.entities.v1.ExtendedStreamR\x0e\x64\x65rivedStreams\"\x91\x03\n\x0cMaskedFields\x12\x1b\n\thash_type\x18\x01 \x01(\tR\x08hashType\x12\x37\n\x04seed\x18\x02 \x01(\tB#\xfa\x42 r\x1e\x18\xe8\x07\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04seed\x12\x63\n\x0e\x66ield_patterns\x18\x03 \x03(\x0b\x32<.strmprivacy.api.entities.v1.MaskedFields.FieldPatternsEntryR\rfieldPatterns\x1aw\n\x12\x46ieldPatternsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12K\n\x05value\x18\x02 \x01(\x0b\x32\x35.strmprivacy.api.entities.v1.MaskedFields.PatternListR\x05value:\x02\x38\x01\x1aM\n\x0bPatternList\x12>\n\x0e\x66ield_patterns\x18\x01 \x03(\tB\x17\xfa\x42\x14\x92\x01\x11\x18\x01\"\rr\x0b\xba\x01\x08strmMetaR\rfieldPatterns\"R\n\x06Limits\x12\"\n\nevent_rate\x18\x01 \x01(\x03\x42\x03\xe0\x41\x03R\teventRate\x12$\n\x0b\x65vent_count\x18\x02 \x01(\x03\x42\x03\xe0\x41\x03R\neventCount\"\x92\x01\n\tKeyStream\x12@\n\x03ref\x18\x01 \x01(\x0b\x32).strmprivacy.api.entities.v1.KeyStreamRefB\x03\xe0\x41\x03R\x03ref\x12\x1d\n\x06status\x18\x02 \x01(\tB\x05\x18\x01\xe0\x41\x03R\x06status\x12$\n\x0bkafka_topic\x18\x03 \x01(\tB\x03\xe0\x41\x03R\nkafkaTopic\"\x9c\x01\n\tStreamRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x38\n\x04name\x18\x02 \x01(\tB$\xfa\x42!r\x1f\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04name\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\x9f\x01\n\x0cKeyStreamRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x38\n\x04name\x18\x02 \x01(\tB$\xfa\x42!r\x1f\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04name\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\xa1\x01\n\x0b\x43redentials\x12\"\n\nbilling_id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\tbillingId\x12 \n\tclient_id\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x08\x63lientId\x12(\n\rclient_secret\x18\x03 \x01(\tB\x03\xe0\x41\x03R\x0c\x63lientSecret\x12\"\n\nproject_id\x18\x04 \x01(\tB\x03\xe0\x41\x03R\tprojectId\"\xdf\x01\n\x04Sink\x12;\n\x03ref\x18\x01 \x01(\x0b\x32$.strmprivacy.api.entities.v1.SinkRefB\x03\xe0\x41\x02R\x03ref\x12G\n\tsink_type\x18\x02 \x01(\x0e\x32%.strmprivacy.api.entities.v1.SinkTypeB\x03\xe0\x41\x02R\x08sinkType\x12\x43\n\x06\x62ucket\x18\x04 \x01(\x0b\x32).strmprivacy.api.entities.v1.BucketConfigH\x00R\x06\x62ucket:\x02\x18\x01\x42\x08\n\x06\x63onfig\"J\n\x07SinkRef\x12\"\n\nbilling_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\tbillingId\x12\x17\n\x04name\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x04name:\x02\x18\x01\"\x83\x01\n\x0c\x42ucketConfig\x12$\n\x0b\x62ucket_name\x18\x04 \x01(\tB\x03\xe0\x41\x02R\nbucketName\x12%\n\x0b\x63redentials\x18\x05 \x01(\tB\x03\xe0\x41\x02R\x0b\x63redentials\x12&\n\x0f\x61ssume_role_arn\x18\x06 \x01(\tR\rassumeRoleArn\"\x9f\x05\n\rDataConnector\x12I\n\x03ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.DataConnectorRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12O\n\ts3_bucket\x18\x02 \x01(\x0b\x32\x30.strmprivacy.api.entities.v1.AwsS3BucketLocationH\x00R\x08s3Bucket\x12~\n\x1bgoogle_cloud_storage_bucket\x18\x03 \x01(\x0b\x32=.strmprivacy.api.entities.v1.GoogleCloudStorageBucketLocationH\x00R\x18googleCloudStorageBucket\x12\x81\x01\n\x1c\x61zure_blob_storage_container\x18\x04 \x01(\x0b\x32>.strmprivacy.api.entities.v1.AzureBlobStorageContainerLocationH\x00R\x19\x61zureBlobStorageContainer\x12P\n\rjdbc_location\x18\x07 \x01(\x0b\x32).strmprivacy.api.entities.v1.JdbcLocationH\x00R\x0cjdbcLocation\x12\x1f\n\x04uuid\x18\x05 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x04uuid\x12j\n\x12\x64\x65pendent_entities\x18\x06 \x01(\x0b\x32;.strmprivacy.api.entities.v1.DataConnectorDependentEntitiesR\x11\x64\x65pendentEntitiesB\x0f\n\x08location\x12\x03\xf8\x42\x01\"\xa0\x01\n\x10\x44\x61taConnectorRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x35\n\x04name\x18\x02 \x01(\tB!\xfa\x42\x1er\x1c\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$R\x04name\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\xb3\x02\n\x1e\x44\x61taConnectorDependentEntities\x12S\n\x0f\x62\x61tch_exporters\x18\x01 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchExporterR\x0e\x62\x61tchExporters\x12\x44\n\nbatch_jobs\x18\x02 \x03(\x0b\x32%.strmprivacy.api.entities.v1.BatchJobR\tbatchJobs\x12v\n\x1cmicro_aggregation_batch_jobs\x18\x03 \x03(\x0b\x32\x35.strmprivacy.api.entities.v1.MicroAggregationBatchJobR\x19microAggregationBatchJobs\"\x9e\x01\n\x13\x41wsS3BucketLocation\x12(\n\x0b\x62ucket_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\nbucketName\x12)\n\x0b\x63redentials\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x63redentials\x12\x32\n\x0f\x61ssume_role_arn\x18\x03 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\xd0\x01\x01R\rassumeRoleArn\"w\n GoogleCloudStorageBucketLocation\x12(\n\x0b\x62ucket_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\nbucketName\x12)\n\x0b\x63redentials\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x63redentials\"\x8a\x02\n!AzureBlobStorageContainerLocation\x12\x37\n\x13storage_account_uri\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x11storageAccountUri\x12.\n\x0e\x63ontainer_name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\rcontainerName\x12|\n\x18\x63lient_secret_credential\x18\x03 \x01(\x0b\x32\x38.strmprivacy.api.entities.v1.AzureClientSecretCredentialB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x16\x63lientSecretCredential\"\x97\x01\n\x1b\x41zureClientSecretCredential\x12$\n\ttenant_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08tenantId\x12$\n\tclient_id\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08\x63lientId\x12,\n\rclient_secret\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0c\x63lientSecret\"\xad\x01\n\x0cJdbcLocation\x12\"\n\x08jdbc_uri\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x07jdbcUri\x12)\n\x0bprivate_key\x18\x02 \x01(\tB\x08\xfa\x42\x05r\x03\xd0\x01\x01R\nprivateKey\x12N\n\rdatabase_type\x18\x03 \x01(\x0e\x32).strmprivacy.api.entities.v1.DatabaseTypeR\x0c\x64\x61tabaseType\"\xa3\x01\n\x08\x44\x61taType\x12:\n\x03\x63sv\x18\x01 \x01(\x0b\x32&.strmprivacy.api.entities.v1.CsvConfigH\x00R\x03\x63sv\x12I\n\x08\x64\x61tabase\x18\x02 \x01(\x0b\x32+.strmprivacy.api.entities.v1.DatabaseConfigH\x00R\x08\x64\x61tabaseB\x10\n\tdata_type\x12\x03\xf8\x42\x01\"%\n\tCsvConfig\x12\x18\n\x07\x63harset\x18\x01 \x01(\tR\x07\x63harset\"\x8a\x05\n\rBatchExporter\x12I\n\x03ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.BatchExporterRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12G\n\nstream_ref\x18\x02 \x01(\x0b\x32&.strmprivacy.api.entities.v1.StreamRefH\x00R\tstreamRef\x12Q\n\x0ekey_stream_ref\x18\x03 \x01(\x0b\x32).strmprivacy.api.entities.v1.KeyStreamRefH\x00R\x0ckeyStreamRef\x12I\n\x08interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB\x12\xe0\x41\x02\xfa\x42\x0c\xaa\x01\t\"\x03\x08\x90\x1c\x32\x02\x08\x1eR\x08interval\x12*\n\tsink_name\x18\x05 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\x08sinkName\x12[\n\x0bpath_prefix\x18\x06 \x01(\tB:\xfa\x42\x37r5\x18\x84\x07\x32\t^.+[^\\/]$Z\x01.Z\x02..\xba\x01\x1a.well-known/acme-challenge\xd0\x01\x01R\npathPrefix\x12\x36\n\x17include_existing_events\x18\x07 \x01(\x08R\x15includeExistingEvents\x12\x65\n\x12\x64\x61ta_connector_ref\x18\x08 \x01(\x0b\x32-.strmprivacy.api.entities.v1.DataConnectorRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x10\x64\x61taConnectorRefB\x1f\n\x18stream_or_key_stream_ref\x12\x03\xf8\x42\x01\"\x98\x01\n\x15\x45xtendedBatchExporter\x12\x17\n\x04uuid\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x04uuid\x12\x19\n\x05topic\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x05topic\x12K\n\x08\x65xporter\x18\x03 \x01(\x0b\x32*.strmprivacy.api.entities.v1.BatchExporterB\x03\xe0\x41\x03R\x08\x65xporter\"\xa3\x01\n\x10\x42\x61tchExporterRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x38\n\x04name\x18\x02 \x01(\tB$\xfa\x42!r\x1f\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04name\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\xfa\x01\n\x0cKafkaCluster\x12\x43\n\x03ref\x18\x01 \x01(\x0b\x32,.strmprivacy.api.entities.v1.KafkaClusterRefB\x03\xe0\x41\x02R\x03ref\x12\x30\n\x11\x62ootstrap_servers\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x10\x62ootstrapServers\x12V\n\x0e\x61uth_mechanism\x18\x03 \x01(\x0e\x32*.strmprivacy.api.entities.v1.AuthMechanismB\x03\xe0\x41\x02R\rauthMechanism\x12\x1b\n\ttoken_uri\x18\x04 \x01(\tR\x08tokenUri\"\x93\x01\n\x0fKafkaClusterRef\x12\x1d\n\nbilling_id\x18\x01 \x01(\tR\tbillingId\x12\x35\n\x04name\x18\x02 \x01(\tB!\xfa\x42\x1er\x1c\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$R\x04name\x12*\n\nproject_id\x18\x03 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\tprojectId\"\xb3\x02\n\rKafkaExporter\x12I\n\x03ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.KafkaExporterRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12O\n\nstream_ref\x18\x02 \x01(\x0b\x32&.strmprivacy.api.entities.v1.StreamRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tstreamRef\x12H\n\x06target\x18\x03 \x01(\x0b\x32\x30.strmprivacy.api.entities.v1.KafkaExporterTargetR\x06target\x12<\n\x05users\x18\x04 \x03(\x0b\x32&.strmprivacy.api.entities.v1.KafkaUserR\x05users\"v\n\x10KafkaExporterRef\x12\x1d\n\nbilling_id\x18\x01 \x01(\tR\tbillingId\x12\x17\n\x04name\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x04name\x12*\n\nproject_id\x18\x03 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\tprojectId\"\x87\x02\n\x13KafkaExporterTarget\x12W\n\x0b\x63luster_ref\x18\x01 \x01(\x0b\x32,.strmprivacy.api.entities.v1.KafkaClusterRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\nclusterRef\x12\x34\n\x05topic\x18\x02 \x01(\tB\x1e\xfa\x42\x1br\x19\x18\xf9\x01\x32\x11^[a-zA-Z0-9._-]+$\xd0\x01\x01R\x05topic\x12(\n\tclient_id\x18\x03 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x08\x63lientId\x12\x37\n\rclient_secret\x18\x04 \x01(\tB\x12\xfa\x42\x0fr\r2\x08^[ -~]+$\xd0\x01\x01R\x0c\x63lientSecret\"\xc2\x02\n\tKafkaUser\x12\x45\n\x03ref\x18\x01 \x01(\x0b\x32).strmprivacy.api.entities.v1.KafkaUserRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12\x33\n\x13kafka_exporter_name\x18\x03 \x01(\tB\x03\xe0\x41\x03R\x11kafkaExporterName\x12\x19\n\x05topic\x18\x04 \x01(\tB\x03\xe0\x41\x03R\x05topic\x12 \n\tclient_id\x18\x05 \x01(\tB\x03\xe0\x41\x03R\x08\x63lientId\x12(\n\rclient_secret\x18\x06 \x01(\tB\x03\xe0\x41\x03R\x0c\x63lientSecret\x12R\n\x0b\x63luster_ref\x18\x07 \x01(\x0b\x32,.strmprivacy.api.entities.v1.KafkaClusterRefB\x03\xe0\x41\x03R\nclusterRef\"n\n\x0cKafkaUserRef\x12!\n\nbilling_id\x18\x01 \x01(\tB\x02\x18\x01R\tbillingId\x12\x17\n\x04name\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x04name\x12\"\n\nproject_id\x18\x03 \x01(\tB\x03\xe0\x41\x03R\tprojectId\"6\n\rConsentLevels\x12%\n\x0e\x63onsent_levels\x18\x01 \x03(\x05R\rconsentLevels\"\x9d\x01\n\x13\x43onsentLevelMapping\x12O\n\x03ref\x18\x01 \x01(\x0b\x32\x33.strmprivacy.api.entities.v1.ConsentLevelMappingRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12\x35\n\x04name\x18\x02 \x01(\tB!\xfa\x42\x1er\x1c\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$R\x04name\"\x8d\x01\n\x16\x43onsentLevelMappingRef\x12+\n\nbilling_id\x18\x01 \x01(\tB\x0c\x18\x01\xfa\x42\x07r\x05\x18\x00\xd0\x01\x01R\tbillingId\x12\x1d\n\x05level\x18\x02 \x01(\x05\x42\x07\xfa\x42\x04\x1a\x02(\x00R\x05level\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\x86\x03\n\x06Policy\x12\x18\n\x02id\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\x02id\x12\x38\n\x04name\x18\x02 \x01(\tB$\xfa\x42!r\x1f\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04name\x12*\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\x18\xe8\x07R\x0b\x64\x65scription\x12-\n\rlegal_grounds\x18\x04 \x01(\tB\x08\xfa\x42\x05r\x03\x18\xe8\x07R\x0clegalGrounds\x12\x30\n\x0eretention_days\x18\x05 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04(\x01@\x01R\rretentionDays\x12\x44\n\x05state\x18\x06 \x01(\x0e\x32).strmprivacy.api.entities.v1.Policy.StateB\x03\xe0\x41\x03R\x05state\"U\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x0f\n\x0bSTATE_DRAFT\x10\x01\x12\x10\n\x0cSTATE_ACTIVE\x10\x02\x12\x12\n\x0eSTATE_ARCHIVED\x10\x03\"\xb6\x01\n\x12WindowedEventCount\x12>\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\tstartTime\x12:\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\x07\x65ndTime\x12$\n\x0b\x65vent_count\x18\x03 \x01(\x03\x42\x03\xe0\x41\x03R\neventCount\"\xaf\x01\n\tSchemaRef\x12\x1b\n\x06handle\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x06handle\x12\x17\n\x04name\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x04name\x12\x1d\n\x07version\x18\x03 \x01(\tB\x03\xe0\x41\x02R\x07version\x12M\n\x0bschema_type\x18\x04 \x01(\x0e\x32\'.strmprivacy.api.entities.v1.SchemaTypeB\x03\xe0\x41\x03R\nschemaType\"\xe9\x06\n\x06Schema\x12\x42\n\x03ref\x18\x01 \x01(\x0b\x32&.strmprivacy.api.entities.v1.SchemaRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12\x44\n\x05state\x18\x02 \x01(\x0e\x32).strmprivacy.api.entities.v1.Schema.StateB\x03\xe0\x41\x03R\x05state\x12\x1b\n\tis_public\x18\x03 \x01(\x08R\x08isPublic\x12\x1e\n\ndefinition\x18\x04 \x01(\tR\ndefinition\x12%\n\x0b\x66ingerprint\x18\x05 \x01(\tB\x03\xe0\x41\x03R\x0b\x66ingerprint\x12G\n\x08metadata\x18\x06 \x01(\x0b\x32+.strmprivacy.api.entities.v1.SchemaMetadataR\x08metadata\x12_\n\rsimple_schema\x18\x07 \x01(\x0b\x32:.strmprivacy.api.entities.v1.Schema.SimpleSchemaDefinitionR\x0csimpleSchema\x12\x13\n\x02id\x18\x08 \x01(\tB\x03\xe0\x41\x03R\x02id\x1a\xbf\x02\n\x16SimpleSchemaDefinition\x12$\n\x04name\x18\x01 \x01(\tB\x10\xfa\x42\rr\x0b\x32\t^[^\\pC]+$R\x04name\x12]\n\tnamespace\x18\x02 \x01(\tB?\xfa\x42<r:25^([a-zA-Z_][a-zA-Z0-9_]*)(\\.[a-zA-Z_][a-zA-Z0-9_]*)*$\xd0\x01\x01R\tnamespace\x12\x1a\n\x03\x64oc\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\x18\x88\'R\x03\x64oc\x12\x43\n\x05nodes\x18\x04 \x03(\x0b\x32-.strmprivacy.api.entities.v1.SimpleSchemaNodeR\x05nodes\x12?\n\tavro_name\x18\x05 \x01(\tB\"\xfa\x42\x1fr\x1d\x32\x18^[a-zA-Z_][a-zA-Z0-9_]*$\xd0\x01\x01R\x08\x61vroName\"p\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\t\n\x05\x44RAFT\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x0c\n\x08\x41RCHIVED\x10\x03\x12\r\n\tIN_REVIEW\x10\x04\x12\x0e\n\nINCOMPLETE\x10\x05\x12\x0c\n\x08\x41PPROVED\x10\x06\"\xe3\x02\n\x10SimpleSchemaNode\x12O\n\x04type\x18\x01 \x01(\x0e\x32\x31.strmprivacy.api.entities.v1.SimpleSchemaNodeTypeB\x08\xfa\x42\x05\x82\x01\x02 \x00R\x04type\x12$\n\x04name\x18\x02 \x01(\tB\x10\xfa\x42\rr\x0b\x32\t^[^\\pC]+$R\x04name\x12?\n\tavro_name\x18\x07 \x01(\tB\"\xfa\x42\x1fr\x1d\x32\x18^[a-zA-Z_][a-zA-Z0-9_]*$\xd0\x01\x01R\x08\x61vroName\x12\x1a\n\x08repeated\x18\x03 \x01(\x08R\x08repeated\x12\x1a\n\x08required\x18\x04 \x01(\x08R\x08required\x12\x43\n\x05nodes\x18\x05 \x03(\x0b\x32-.strmprivacy.api.entities.v1.SimpleSchemaNodeR\x05nodes\x12\x1a\n\x03\x64oc\x18\x06 \x01(\tB\x08\xfa\x42\x05r\x03\x18\x88\'R\x03\x64oc\"\xd5\x02\n\x0eSchemaMetadata\x12-\n\x05title\x18\x01 \x01(\tB\x17\xfa\x42\x14r\x12\x10\x04\x18\x64\x32\t^[^\\pC]+$\xd0\x01\x01R\x05title\x12*\n\x0b\x64\x65scription\x18\x02 \x01(\tB\x08\xfa\x42\x05r\x03\x18\x88\'R\x0b\x64\x65scription\x12@\n\x0b\x63reate_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\ncreateTime\x12\x30\n\x08icon_uri\x18\x04 \x01(\tB\x15\xfa\x42\x12r\x10:\x08https://\xd0\x01\x01\x88\x01\x01R\x07iconUri\x12:\n\x06labels\x18\x05 \x03(\x0b\x32\".strmprivacy.api.entities.v1.LabelR\x06labels\x12\x18\n\x07\x64omains\x18\x06 \x03(\tR\x07\x64omains\x12\x1e\n\nindustries\x18\x07 \x03(\tR\nindustries\"\x9a\x01\n\x10\x45ventContractRef\x12\x1f\n\x06handle\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x04R\x06handle\x12\x33\n\x04name\x18\x02 \x01(\tB\x1f\xfa\x42\x1cr\x1a\x10\x04\x18\x64\x32\x14^[\\pL\\pN\\pS\\pM\\pP]+$R\x04name\x12\x30\n\x07version\x18\x03 \x01(\tB\x16\xfa\x42\x13r\x11\x32\x0f^\\d+\\.\\d+\\.\\d+$R\x07version\"\x82\x06\n\rEventContract\x12\x44\n\x03ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.EventContractRefB\x03\xe0\x41\x02R\x03ref\x12K\n\x05state\x18\x02 \x01(\x0e\x32\x30.strmprivacy.api.entities.v1.EventContract.StateB\x03\xe0\x41\x03R\x05state\x12J\n\nschema_ref\x18\x03 \x01(\x0b\x32&.strmprivacy.api.entities.v1.SchemaRefB\x03\xe0\x41\x02R\tschemaRef\x12\x1b\n\tis_public\x18\x04 \x01(\x08R\x08isPublic\x12 \n\tkey_field\x18\x05 \x01(\tB\x03\xe0\x41\x02R\x08keyField\x12X\n\npii_fields\x18\x06 \x03(\x0b\x32\x39.strmprivacy.api.entities.v1.EventContract.PiiFieldsEntryR\tpiiFields\x12I\n\x0bvalidations\x18\x07 \x03(\x0b\x32\'.strmprivacy.api.entities.v1.ValidationR\x0bvalidations\x12N\n\x08metadata\x18\x08 \x01(\x0b\x32\x32.strmprivacy.api.entities.v1.EventContractMetadataR\x08metadata\x12\x0e\n\x02id\x18\t \x01(\tR\x02id\x12,\n\x12\x64\x61ta_subject_field\x18\n \x01(\tR\x10\x64\x61taSubjectField\x1a<\n\x0ePiiFieldsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x05R\x05value:\x02\x38\x01\"b\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\t\n\x05\x44RAFT\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x0c\n\x08\x41RCHIVED\x10\x03\x12\r\n\tIN_REVIEW\x10\x04\x12\x0e\n\nINCOMPLETE\x10\x05\"\xc0\x02\n\x15\x45ventContractMetadata\x12\x19\n\x05title\x18\x01 \x01(\tB\x03\xe0\x41\x01R\x05title\x12%\n\x0b\x64\x65scription\x18\x02 \x01(\tB\x03\xe0\x41\x01R\x0b\x64\x65scription\x12@\n\x0b\x63reate_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\ncreateTime\x12\x1e\n\x08icon_uri\x18\x04 \x01(\tB\x03\xe0\x41\x01R\x07iconUri\x12?\n\x06labels\x18\x05 \x03(\x0b\x32\".strmprivacy.api.entities.v1.LabelB\x03\xe0\x41\x01R\x06labels\x12\x1d\n\x07\x64omains\x18\x06 \x03(\tB\x03\xe0\x41\x01R\x07\x64omains\x12#\n\nindustries\x18\x07 \x03(\tB\x03\xe0\x41\x01R\nindustries\"8\n\x05Label\x12\x19\n\x03key\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"l\n\nValidation\x12\x1d\n\x05\x66ield\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x05\x66ield\x12 \n\x04type\x18\x02 \x01(\tB\x0c\xfa\x42\tr\x07R\x05regexR\x04type\x12\x1d\n\x05value\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x05value\"\xfe\x02\n\nStreamTree\x12@\n\x06stream\x18\x01 \x01(\x0b\x32#.strmprivacy.api.entities.v1.StreamB\x03\xe0\x41\x02R\x06stream\x12\x45\n\nkey_stream\x18\x02 \x01(\x0b\x32&.strmprivacy.api.entities.v1.KeyStreamR\tkeyStream\x12=\n\x07\x64\x65rived\x18\x03 \x03(\x0b\x32#.strmprivacy.api.entities.v1.StreamR\x07\x64\x65rived\x12S\n\x0f\x62\x61tch_exporters\x18\x04 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchExporterR\x0e\x62\x61tchExporters\x12S\n\x0fkafka_exporters\x18\x05 \x03(\x0b\x32*.strmprivacy.api.entities.v1.KafkaExporterR\x0ekafkaExporters\"\x9f\x01\n\x08SinkTree\x12:\n\x04sink\x18\x01 \x01(\x0b\x32!.strmprivacy.api.entities.v1.SinkB\x03\xe0\x41\x02R\x04sink\x12S\n\x0f\x62\x61tch_exporters\x18\x02 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchExporterR\x0e\x62\x61tchExporters:\x02\x18\x01\"\xc8\x06\n\x08\x42\x61tchJob\x12\x44\n\x03ref\x18\x01 \x01(\x0b\x32(.strmprivacy.api.entities.v1.BatchJobRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12G\n\x06states\x18\x02 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchJobStateB\x03\xe0\x41\x03R\x06states\x12\\\n\x0bsource_data\x18\x03 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\nsourceData\x12N\n\x07\x63onsent\x18\x04 \x01(\x0b\x32*.strmprivacy.api.entities.v1.ConsentConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x07\x63onsent\x12W\n\nencryption\x18\x05 \x01(\x0b\x32-.strmprivacy.api.entities.v1.EncryptionConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\nencryption\x12\x65\n\x12\x65vent_contract_ref\x18\x06 \x01(\x0b\x32-.strmprivacy.api.entities.v1.EventContractRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x10\x65ventContractRef\x12[\n\x0e\x65ncrypted_data\x18\x07 \x01(\x0b\x32*.strmprivacy.api.entities.v1.EncryptedDataB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\rencryptedData\x12k\n\x14\x65ncryption_keys_data\x18\x08 \x01(\x0b\x32/.strmprivacy.api.entities.v1.EncryptionKeysDataB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x12\x65ncryptionKeysData\x12K\n\x0c\x64\x65rived_data\x18\t \x03(\x0b\x32(.strmprivacy.api.entities.v1.DerivedDataR\x0b\x64\x65rivedData\x12(\n\tpolicy_id\x18\n \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x08policyId\"\xf0\x01\n\x0f\x42\x61tchJobWrapper\x12Y\n\x14\x65ncryption_batch_job\x18\x01 \x01(\x0b\x32%.strmprivacy.api.entities.v1.BatchJobH\x00R\x12\x65ncryptionBatchJob\x12v\n\x1bmicro_aggregation_batch_job\x18\x02 \x01(\x0b\x32\x35.strmprivacy.api.entities.v1.MicroAggregationBatchJobH\x00R\x18microAggregationBatchJobB\n\n\x03job\x12\x03\xf8\x42\x01\"\x9a\x01\n\x10\x45xtendedBatchJob\x12\x46\n\tbatch_job\x18\x01 \x01(\x0b\x32%.strmprivacy.api.entities.v1.BatchJobB\x02\x18\x01R\x08\x62\x61tchJob\x12>\n\x03job\x18\x02 \x01(\x0b\x32,.strmprivacy.api.entities.v1.BatchJobWrapperR\x03job\"y\n\x0b\x42\x61tchJobRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x13\n\x02id\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x02id\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\xb9\x01\n\rBatchJobState\x12>\n\nstate_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\tstateTime\x12I\n\x05state\x18\x02 \x01(\x0e\x32..strmprivacy.api.entities.v1.BatchJobStateTypeB\x03\xe0\x41\x03R\x05state\x12\x1d\n\x07message\x18\x03 \x01(\tB\x03\xe0\x41\x01R\x07message\"\xda\x02\n\x14\x44\x61taConnectorAndType\x12\x65\n\x12\x64\x61ta_connector_ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.DataConnectorRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x10\x64\x61taConnectorRef\x12[\n\x0bpath_prefix\x18\x02 \x01(\tB:\xfa\x42\x37r5\x18\x84\x07\x32\t^.+[^\\/]$Z\x01.Z\x02..\xba\x01\x1a.well-known/acme-challenge\xd0\x01\x01R\npathPrefix\x12\x30\n\tfile_name\x18\x03 \x01(\tB\x13\xfa\x42\x10r\x0e\x32\t^[^\\pC]+$\xd0\x01\x01R\x08\x66ileName\x12L\n\tdata_type\x18\x04 \x01(\x0b\x32%.strmprivacy.api.entities.v1.DataTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x08\x64\x61taType\"}\n\x0e\x44\x61tabaseConfig\x12\"\n\x06schema\x18\x01 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\xd0\x01\x01R\x06schema\x12\x1d\n\x05table\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x05table\x12(\n\x07\x63olumns\x18\x03 \x03(\tB\x0e\xfa\x42\x0b\x92\x01\x08\"\x04r\x02\x10\x01(\x01R\x07\x63olumns\"\xbb\x01\n\rConsentConfig\x12\x39\n\x16\x64\x65\x66\x61ult_consent_levels\x18\x01 \x03(\x05\x42\x03\xe0\x41\x01R\x14\x64\x65\x66\x61ultConsentLevels\x12o\n\x17\x63onsent_level_extractor\x18\x02 \x01(\x0b\x32\x32.strmprivacy.api.entities.v1.ConsentLevelExtractorB\x03\xe0\x41\x01R\x15\x63onsentLevelExtractor\"\x89\x02\n\x15\x43onsentLevelExtractor\x12\x14\n\x05\x66ield\x18\x01 \x01(\tR\x05\x66ield\x12l\n\x0e\x66ield_patterns\x18\x02 \x03(\x0b\x32\x45.strmprivacy.api.entities.v1.ConsentLevelExtractor.FieldPatternsEntryR\rfieldPatterns\x1al\n\x12\x46ieldPatternsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12@\n\x05value\x18\x02 \x01(\x0b\x32*.strmprivacy.api.entities.v1.ConsentLevelsR\x05value:\x02\x38\x01\"\xa2\x01\n\x10\x45ncryptionConfig\x12\x61\n\x10timestamp_config\x18\x01 \x01(\x0b\x32,.strmprivacy.api.entities.v1.TimestampConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0ftimestampConfig\x12+\n\x12\x62\x61tch_job_group_id\x18\x02 \x01(\tR\x0f\x62\x61tchJobGroupId\"\xa1\x01\n\x0fTimestampConfig\x12*\n\x05\x66ield\x18\x01 \x01(\tB\x14\xfa\x42\x11r\x0f\x10\x04\x18\x32\x32\t^[^\\pC]+$R\x05\x66ield\x12\x1f\n\x06\x66ormat\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x06\x66ormat\x12\x41\n\x11\x64\x65\x66\x61ult_time_zone\x18\x03 \x01(\x0b\x32\x15.google.type.TimeZoneR\x0f\x64\x65\x66\x61ultTimeZone\"d\n\rEncryptedData\x12S\n\x06target\x18\x01 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x06target\"i\n\x12\x45ncryptionKeysData\x12S\n\x06target\x18\x01 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x06target\"\xb1\x02\n\x0b\x44\x65rivedData\x12N\n\x06target\x18\x01 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x03\xe0\x41\x02R\x06target\x12%\n\x0e\x63onsent_levels\x18\x02 \x03(\x05R\rconsentLevels\x12[\n\x12\x63onsent_level_type\x18\x03 \x01(\x0e\x32-.strmprivacy.api.entities.v1.ConsentLevelTypeR\x10\x63onsentLevelType\x12N\n\rmasked_fields\x18\x04 \x01(\x0b\x32).strmprivacy.api.entities.v1.MaskedFieldsR\x0cmaskedFields\"\xb7\x04\n\x18MicroAggregationBatchJob\x12\x44\n\x03ref\x18\x01 \x01(\x0b\x32(.strmprivacy.api.entities.v1.BatchJobRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12G\n\x06states\x18\x02 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchJobStateB\x03\xe0\x41\x03R\x06states\x12\\\n\x0bsource_data\x18\x03 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\nsourceData\x12\\\n\x0btarget_data\x18\x04 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\ntargetData\x12\x62\n\x11\x64\x61ta_contract_ref\x18\x05 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0f\x64\x61taContractRef\x12l\n\x12\x61ggregation_config\x18\x06 \x01(\x0b\x32\x33.strmprivacy.api.entities.v1.MicroAggregationConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x11\x61ggregationConfig\"\x80\x01\n\x16MicroAggregationConfig\x12\x37\n\x13minimum_k_anonymity\x18\x01 \x01(\x05\x42\x07\xfa\x42\x04\x1a\x02(\x02R\x11minimumKAnonymity\x12-\n\x12\x61ggregation_fields\x18\x02 \x03(\tR\x11\x61ggregationFields\"\x92\x01\n\x0f\x44\x61taContractRef\x12\"\n\x06handle\x18\x01 \x01(\tB\n\xe0\x41\x02\xfa\x42\x04r\x02\x10\x04R\x06handle\x12&\n\x04name\x18\x02 \x01(\tB\x12\xfa\x42\x0fr\r\x10\x04\x18\x64\x32\x07^[^/]+$R\x04name\x12\x33\n\x07version\x18\x03 \x01(\tB\x19\xe0\x41\x02\xfa\x42\x13r\x11\x32\x0f^\\d+\\.\\d+\\.\\d+$R\x07version\"\x94\x07\n\x0c\x44\x61taContract\x12\x13\n\x02id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x02id\x12H\n\x03ref\x18\x02 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12J\n\x05state\x18\x03 \x01(\x0e\x32/.strmprivacy.api.entities.v1.DataContract.StateB\x03\xe0\x41\x03R\x05state\x12\x1b\n\tis_public\x18\x04 \x01(\x08R\x08isPublic\x12$\n\tkey_field\x18\x05 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08keyField\x12[\n\npii_fields\x18\x06 \x03(\x0b\x32\x38.strmprivacy.api.entities.v1.DataContract.PiiFieldsEntryB\x02\x18\x01R\tpiiFields\x12I\n\x0bvalidations\x18\x07 \x03(\x0b\x32\'.strmprivacy.api.entities.v1.ValidationR\x0bvalidations\x12M\n\x08metadata\x18\x08 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataContractMetadataR\x08metadata\x12\x45\n\x06schema\x18\t \x01(\x0b\x32#.strmprivacy.api.entities.v1.SchemaB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x06schema\x12,\n\x12\x64\x61ta_subject_field\x18\n \x01(\tR\x10\x64\x61taSubjectField\x12\'\n\nproject_id\x18\x0b \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\x12Q\n\x0e\x66ield_metadata\x18\x0c \x03(\x0b\x32*.strmprivacy.api.entities.v1.FieldMetadataR\rfieldMetadata\x1a<\n\x0ePiiFieldsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x05R\x05value:\x02\x38\x01\"p\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\t\n\x05\x44RAFT\x10\x01\x12\r\n\tIN_REVIEW\x10\x02\x12\n\n\x06\x41\x43TIVE\x10\x03\x12\x0c\n\x08\x41RCHIVED\x10\x04\x12\x0e\n\nINCOMPLETE\x10\x05\x12\x0c\n\x08\x41PPROVED\x10\x06\"\xe1\x06\n\rFieldMetadata\x12\x1d\n\nfield_name\x18\x01 \x01(\tR\tfieldName\x12o\n\x14personal_data_config\x18\x02 \x01(\x0b\x32=.strmprivacy.api.entities.v1.FieldMetadata.PersonalDataConfigR\x12personalDataConfig\x12\x64\n\x15statistical_data_type\x18\x03 \x01(\x0e\x32\x30.strmprivacy.api.entities.v1.StatisticalDataTypeR\x13statisticalDataType\x12%\n\x0eordinal_values\x18\x04 \x03(\tR\rordinalValues\x12o\n\x14null_handling_config\x18\x05 \x01(\x0b\x32=.strmprivacy.api.entities.v1.FieldMetadata.NullHandlingConfigR\x12nullHandlingConfig\x1a\xc0\x01\n\x12PersonalDataConfig\x12\x1a\n\x06is_pii\x18\x01 \x01(\x08\x42\x03\xe0\x41\x02R\x05isPii\x12#\n\x0bis_quasi_id\x18\x02 \x01(\x08\x42\x03\xe0\x41\x02R\tisQuasiId\x12#\n\rpurpose_level\x18\x03 \x01(\x05R\x0cpurposeLevel\x12\x44\n\x1fgdpr_special_personal_data_type\x18\x04 \x01(\tR\x1bgdprSpecialPersonalDataType\x1a\xfe\x01\n\x12NullHandlingConfig\x12g\n\x04type\x18\x01 \x01(\x0e\x32N.strmprivacy.api.entities.v1.FieldMetadata.NullHandlingConfig.NullHandlingTypeB\x03\xe0\x41\x02R\x04type\x12#\n\rdefault_value\x18\x02 \x01(\tR\x0c\x64\x65\x66\x61ultValue\"Z\n\x10NullHandlingType\x12\"\n\x1eNULL_HANDLING_TYPE_UNSPECIFIED\x10\x00\x12\x0f\n\x0b\x44ROP_RECORD\x10\x01\x12\x11\n\rDEFAULT_VALUE\x10\x02\"\x9f\x02\n\x14\x44\x61taContractMetadata\x12-\n\x05title\x18\x01 \x01(\tB\x17\xfa\x42\x14r\x12\x10\x04\x18\x64\x32\t^[^\\pC]+$\xd0\x01\x01R\x05title\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12@\n\x0b\x63reate_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\ncreateTime\x12:\n\x06labels\x18\x05 \x03(\x0b\x32\".strmprivacy.api.entities.v1.LabelR\x06labels\x12\x18\n\x07\x64omains\x18\x06 \x03(\tR\x07\x64omains\x12\x1e\n\nindustries\x18\x07 \x03(\tR\nindustries\"\xbd\x02\n\x07Project\x12\x13\n\x02id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x02id\x12\x35\n\x04name\x18\x02 \x01(\tB!\xfa\x42\x1er\x1c\x10\x02\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$R\x04name\x12*\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\x18\x88\'R\x0b\x64\x65scription\x12,\n\x0forganization_id\x18\x04 \x01(\tB\x03\xe0\x41\x03R\x0eorganizationId\x12\x45\n\x05state\x18\x05 \x01(\x0e\x32*.strmprivacy.api.entities.v1.Project.StateB\x03\xe0\x41\x03R\x05state\"E\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x0f\n\x0bOPERATIONAL\x10\x01\x12\x14\n\x10PENDING_DELETION\x10\x02\"\xbe\x02\n\x04User\x12 \n\x05\x65mail\x18\x01 \x01(\tB\n\xfa\x42\x07r\x05\xd0\x01\x01`\x01R\x05\x65mail\x12\x1d\n\nfirst_name\x18\x02 \x01(\tR\tfirstName\x12\x1b\n\tlast_name\x18\x03 \x01(\tR\x08lastName\x12\x44\n\nuser_roles\x18\x04 \x03(\x0e\x32%.strmprivacy.api.entities.v1.UserRoleR\tuserRoles\x12\x35\n\x10\x65xternal_user_id\x18\x05 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0e\x65xternalUserId\x12\x34\n\x0forganization_id\x18\x06 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0eorganizationId\x12%\n\x0e\x66unction_title\x18\x07 \x01(\tR\rfunctionTitle\"\x82\x01\n\x0ePurposeMapping\x12\x1d\n\x05level\x18\x01 \x01(\x05\x42\x07\xfa\x42\x04\x1a\x02(\x00R\x05level\x12#\n\x07purpose\x18\x02 \x01(\tB\t\xfa\x42\x06r\x04\x10\x02\x18\x64R\x07purpose\x12,\n\x0b\x64\x65scription\x18\x03 \x01(\tB\n\xfa\x42\x07r\x05\x10\x02\xd0\x01\x01R\x0b\x64\x65scription\"\xaf\x01\n\nGenericRef\x12J\n\x04type\x18\x01 \x01(\x0e\x32\x36.strmprivacy.api.entities.v1.GenericRef.GenericRefTypeR\x04type\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02id\"E\n\x0eGenericRefType\x12 \n\x1cGENERIC_REF_TYPE_UNSPECIFIED\x10\x00\x12\x11\n\rDATA_CONTRACT\x10\x01\"\xac\x02\n\x07\x43omment\x12\x1b\n\x02id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x02id\x12\x45\n\x0b\x63reate_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x00R\ncreateTime\x12P\n\nentity_ref\x18\x03 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\x12$\n\x07\x63ontent\x18\x04 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xe8\x07R\x07\x63ontent\x12\x45\n\x07\x63reator\x18\x05 \x01(\x0b\x32!.strmprivacy.api.entities.v1.UserB\x08\xfa\x42\x05\x8a\x01\x02\x10\x00R\x07\x63reator\"\xfd\x02\n\x0f\x41uditTrailEntry\x12\x1b\n\x02id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x02id\x12\x45\n\x0b\x63reate_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x00R\ncreateTime\x12P\n\nentity_ref\x18\x03 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\x12$\n\x07\x63ontent\x18\x04 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xe8\x07R\x07\x63ontent\x12\x41\n\x05\x61\x63tor\x18\x05 \x01(\x0b\x32!.strmprivacy.api.entities.v1.UserB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x05\x61\x63tor\x12*\n\nproject_id\x18\x06 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\tprojectId\x12\x1f\n\x0b\x65ntity_name\x18\x07 \x01(\tR\nentityName*]\n\x08UserRole\x12\x19\n\x15USER_ROLE_UNSPECIFIED\x10\x00\x12\t\n\x05\x41\x44MIN\x10\x01\x12\x11\n\rPROJECT_ADMIN\x10\x02\x12\x0c\n\x08\x41PPROVER\x10\x03\x12\n\n\x06MEMBER\x10\x04*\x8d\x01\n\x11\x42\x61tchJobStateType\x12$\n BATCH_JOB_STATE_TYPE_UNSPECIFIED\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\x0b\n\x07STARTED\x10\x02\x12\x12\n\x0e\x45RROR_STARTING\x10\x03\x12\x0b\n\x07RUNNING\x10\x04\x12\x0c\n\x08\x46INISHED\x10\x05\x12\t\n\x05\x45RROR\x10\x06*T\n\x10\x43onsentLevelType\x12\"\n\x1e\x43ONSENT_LEVEL_TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nCUMULATIVE\x10\x01\x12\x0c\n\x08GRANULAR\x10\x02*=\n\x08SinkType\x12\x19\n\x15SINK_TYPE_UNSPECIFIED\x10\x00\x12\x06\n\x02S3\x10\x01\x12\n\n\x06GCLOUD\x10\x02\x1a\x02\x18\x01*M\n\rAuthMechanism\x12\x1e\n\x1a\x41UTH_MECHANISM_UNSPECIFIED\x10\x00\x12\x0e\n\nSASL_PLAIN\x10\x01\x12\x0c\n\x08SASL_SSL\x10\x02*C\n\nSchemaType\x12\x1b\n\x17SCHEMA_TYPE_UNSPECIFIED\x10\x00\x12\x08\n\x04\x41VRO\x10\x01\x12\x0e\n\nJSONSCHEMA\x10\x02*\x84\x01\n\x14SimpleSchemaNodeType\x12\'\n#SIMPLE_SCHEMA_NODE_TYPE_UNSPECIFIED\x10\x00\x12\n\n\x06STRING\x10\x01\x12\x0b\n\x07\x42OOLEAN\x10\x02\x12\t\n\x05\x46LOAT\x10\x03\x12\x0b\n\x07INTEGER\x10\x04\x12\x08\n\x04LONG\x10\x05\x12\x08\n\x04NODE\x10\n*_\n\x13\x46ilterPublicPrivate\x12%\n!FILTER_PUBLIC_PRIVATE_UNSPECIFIED\x10\x00\x12\x0f\n\x0bONLY_PUBLIC\x10\x01\x12\x10\n\x0cONLY_PRIVATE\x10\x02*e\n\x13StatisticalDataType\x12%\n!STATISTICAL_DATA_TYPE_UNSPECIFIED\x10\x00\x12\x0b\n\x07NOMINAL\x10\x01\x12\x0b\n\x07ORDINAL\x10\x02\x12\r\n\tNUMERICAL\x10\x03*\x92\x01\n\x10SubscriptionPlan\x12!\n\x1dSUBSCRIPTION_PLAN_UNSPECIFIED\x10\x00\x12\x08\n\x04\x46REE\x10\x01\x12\x0c\n\x08\x42USINESS\x10\x02\x12\x0f\n\x0bSELF_HOSTED\x10\x03\x12\x18\n\x14\x41WS_MARKETPLACE_PAYG\x10\x04\x12\x18\n\x14\x41WS_MARKETPLACE_BYOL\x10\x05*c\n\x0c\x44\x61tabaseType\x12\x1d\n\x19\x44\x41TABASE_TYPE_UNSPECIFIED\x10\x00\x12\x0c\n\x08POSTGRES\x10\x01\x12\t\n\x05MYSQL\x10\x02\x12\x0c\n\x08\x42IGQUERY\x10\x03\x12\r\n\tSNOWFLAKE\x10\x04\x42i\n\x1eio.strmprivacy.api.entities.v1P\x01ZEgithub.com/strmprivacy/api-definitions-go/v2/api/entities/v1;entitiesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-strmprivacy/api/entities/v1/entities_v1.proto\x12\x1bstrmprivacy.api.entities.v1\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1agoogle/type/datetime.proto\x1a\x17validate/validate.proto\"\xab\x05\n\x06Stream\x12\x45\n\x03ref\x18\x01 \x01(\x0b\x32&.strmprivacy.api.entities.v1.StreamRefB\x0b\xe0\x41\x02\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12-\n\x0b\x64\x65scription\x18\x02 \x01(\tB\x0b\xfa\x42\x08r\x06\x18\xe8\x07\xd0\x01\x01R\x0b\x64\x65scription\x12/\n\x0e\x63onsent_levels\x18\x03 \x03(\x05\x42\x08\xfa\x42\x05\x92\x01\x02\x10\x32R\rconsentLevels\x12[\n\x12\x63onsent_level_type\x18\x04 \x01(\x0e\x32-.strmprivacy.api.entities.v1.ConsentLevelTypeR\x10\x63onsentLevelType\x12\x1d\n\x07\x65nabled\x18\x05 \x01(\x08\x42\x03\xe0\x41\x03R\x07\x65nabled\x12@\n\x06limits\x18\x06 \x01(\x0b\x32#.strmprivacy.api.entities.v1.LimitsB\x03\xe0\x41\x03R\x06limits\x12#\n\rlinked_stream\x18\x07 \x01(\tR\x0clinkedStream\x12$\n\x04tags\x18\x08 \x03(\tB\x10\xfa\x42\r\x92\x01\n\x10\x14\x18\x01\"\x04r\x02\x18\x64R\x04tags\x12O\n\x0b\x63redentials\x18\t \x03(\x0b\x32(.strmprivacy.api.entities.v1.CredentialsB\x03\xe0\x41\x03R\x0b\x63redentials\x12N\n\rmasked_fields\x18\n \x01(\x0b\x32).strmprivacy.api.entities.v1.MaskedFieldsR\x0cmaskedFields\x12&\n\x0bkafka_topic\x18\x0b \x01(\tB\x05\x18\x01\xe0\x41\x03R\nkafkaTopic\x12(\n\tpolicy_id\x18\x0c \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x08policyId\"\xaa\x01\n\x0e\x45xtendedStream\x12@\n\x06stream\x18\x01 \x01(\x0b\x32#.strmprivacy.api.entities.v1.StreamB\x03\xe0\x41\x03R\x06stream\x12\x19\n\x05topic\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x05topic\x12\x17\n\x04uuid\x18\x03 \x01(\tB\x03\xe0\x41\x03R\x04uuid\x12\"\n\nkey_stream\x18\x04 \x01(\x08\x42\x03\xe0\x41\x03R\tkeyStream\"\xc2\x01\n\x13\x45xtendedStreamGroup\x12U\n\rsource_stream\x18\x01 \x01(\x0b\x32+.strmprivacy.api.entities.v1.ExtendedStreamB\x03\xe0\x41\x03R\x0csourceStream\x12T\n\x0f\x64\x65rived_streams\x18\x02 \x03(\x0b\x32+.strmprivacy.api.entities.v1.ExtendedStreamR\x0e\x64\x65rivedStreams\"\x91\x03\n\x0cMaskedFields\x12\x1b\n\thash_type\x18\x01 \x01(\tR\x08hashType\x12\x37\n\x04seed\x18\x02 \x01(\tB#\xfa\x42 r\x1e\x18\xe8\x07\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04seed\x12\x63\n\x0e\x66ield_patterns\x18\x03 \x03(\x0b\x32<.strmprivacy.api.entities.v1.MaskedFields.FieldPatternsEntryR\rfieldPatterns\x1aw\n\x12\x46ieldPatternsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12K\n\x05value\x18\x02 \x01(\x0b\x32\x35.strmprivacy.api.entities.v1.MaskedFields.PatternListR\x05value:\x02\x38\x01\x1aM\n\x0bPatternList\x12>\n\x0e\x66ield_patterns\x18\x01 \x03(\tB\x17\xfa\x42\x14\x92\x01\x11\x18\x01\"\rr\x0b\xba\x01\x08strmMetaR\rfieldPatterns\"R\n\x06Limits\x12\"\n\nevent_rate\x18\x01 \x01(\x03\x42\x03\xe0\x41\x03R\teventRate\x12$\n\x0b\x65vent_count\x18\x02 \x01(\x03\x42\x03\xe0\x41\x03R\neventCount\"\x92\x01\n\tKeyStream\x12@\n\x03ref\x18\x01 \x01(\x0b\x32).strmprivacy.api.entities.v1.KeyStreamRefB\x03\xe0\x41\x03R\x03ref\x12\x1d\n\x06status\x18\x02 \x01(\tB\x05\x18\x01\xe0\x41\x03R\x06status\x12$\n\x0bkafka_topic\x18\x03 \x01(\tB\x03\xe0\x41\x03R\nkafkaTopic\"\x9c\x01\n\tStreamRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x38\n\x04name\x18\x02 \x01(\tB$\xfa\x42!r\x1f\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04name\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\x9f\x01\n\x0cKeyStreamRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x38\n\x04name\x18\x02 \x01(\tB$\xfa\x42!r\x1f\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04name\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\xa1\x01\n\x0b\x43redentials\x12\"\n\nbilling_id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\tbillingId\x12 \n\tclient_id\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x08\x63lientId\x12(\n\rclient_secret\x18\x03 \x01(\tB\x03\xe0\x41\x03R\x0c\x63lientSecret\x12\"\n\nproject_id\x18\x04 \x01(\tB\x03\xe0\x41\x03R\tprojectId\"\xdf\x01\n\x04Sink\x12;\n\x03ref\x18\x01 \x01(\x0b\x32$.strmprivacy.api.entities.v1.SinkRefB\x03\xe0\x41\x02R\x03ref\x12G\n\tsink_type\x18\x02 \x01(\x0e\x32%.strmprivacy.api.entities.v1.SinkTypeB\x03\xe0\x41\x02R\x08sinkType\x12\x43\n\x06\x62ucket\x18\x04 \x01(\x0b\x32).strmprivacy.api.entities.v1.BucketConfigH\x00R\x06\x62ucket:\x02\x18\x01\x42\x08\n\x06\x63onfig\"J\n\x07SinkRef\x12\"\n\nbilling_id\x18\x01 \x01(\tB\x03\xe0\x41\x02R\tbillingId\x12\x17\n\x04name\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x04name:\x02\x18\x01\"\x83\x01\n\x0c\x42ucketConfig\x12$\n\x0b\x62ucket_name\x18\x04 \x01(\tB\x03\xe0\x41\x02R\nbucketName\x12%\n\x0b\x63redentials\x18\x05 \x01(\tB\x03\xe0\x41\x02R\x0b\x63redentials\x12&\n\x0f\x61ssume_role_arn\x18\x06 \x01(\tR\rassumeRoleArn\"\x9f\x05\n\rDataConnector\x12I\n\x03ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.DataConnectorRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12O\n\ts3_bucket\x18\x02 \x01(\x0b\x32\x30.strmprivacy.api.entities.v1.AwsS3BucketLocationH\x00R\x08s3Bucket\x12~\n\x1bgoogle_cloud_storage_bucket\x18\x03 \x01(\x0b\x32=.strmprivacy.api.entities.v1.GoogleCloudStorageBucketLocationH\x00R\x18googleCloudStorageBucket\x12\x81\x01\n\x1c\x61zure_blob_storage_container\x18\x04 \x01(\x0b\x32>.strmprivacy.api.entities.v1.AzureBlobStorageContainerLocationH\x00R\x19\x61zureBlobStorageContainer\x12P\n\rjdbc_location\x18\x07 \x01(\x0b\x32).strmprivacy.api.entities.v1.JdbcLocationH\x00R\x0cjdbcLocation\x12\x1f\n\x04uuid\x18\x05 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x04uuid\x12j\n\x12\x64\x65pendent_entities\x18\x06 \x01(\x0b\x32;.strmprivacy.api.entities.v1.DataConnectorDependentEntitiesR\x11\x64\x65pendentEntitiesB\x0f\n\x08location\x12\x03\xf8\x42\x01\"\xa0\x01\n\x10\x44\x61taConnectorRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x35\n\x04name\x18\x02 \x01(\tB!\xfa\x42\x1er\x1c\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$R\x04name\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\xb3\x02\n\x1e\x44\x61taConnectorDependentEntities\x12S\n\x0f\x62\x61tch_exporters\x18\x01 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchExporterR\x0e\x62\x61tchExporters\x12\x44\n\nbatch_jobs\x18\x02 \x03(\x0b\x32%.strmprivacy.api.entities.v1.BatchJobR\tbatchJobs\x12v\n\x1cmicro_aggregation_batch_jobs\x18\x03 \x03(\x0b\x32\x35.strmprivacy.api.entities.v1.MicroAggregationBatchJobR\x19microAggregationBatchJobs\"\x9e\x01\n\x13\x41wsS3BucketLocation\x12(\n\x0b\x62ucket_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\nbucketName\x12)\n\x0b\x63redentials\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x63redentials\x12\x32\n\x0f\x61ssume_role_arn\x18\x03 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\xd0\x01\x01R\rassumeRoleArn\"w\n GoogleCloudStorageBucketLocation\x12(\n\x0b\x62ucket_name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\nbucketName\x12)\n\x0b\x63redentials\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x63redentials\"\x8a\x02\n!AzureBlobStorageContainerLocation\x12\x37\n\x13storage_account_uri\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x11storageAccountUri\x12.\n\x0e\x63ontainer_name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\rcontainerName\x12|\n\x18\x63lient_secret_credential\x18\x03 \x01(\x0b\x32\x38.strmprivacy.api.entities.v1.AzureClientSecretCredentialB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x16\x63lientSecretCredential\"\x97\x01\n\x1b\x41zureClientSecretCredential\x12$\n\ttenant_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08tenantId\x12$\n\tclient_id\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08\x63lientId\x12,\n\rclient_secret\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0c\x63lientSecret\"\xad\x01\n\x0cJdbcLocation\x12\"\n\x08jdbc_uri\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x07jdbcUri\x12)\n\x0bprivate_key\x18\x02 \x01(\tB\x08\xfa\x42\x05r\x03\xd0\x01\x01R\nprivateKey\x12N\n\rdatabase_type\x18\x03 \x01(\x0e\x32).strmprivacy.api.entities.v1.DatabaseTypeR\x0c\x64\x61tabaseType\"\xa3\x01\n\x08\x44\x61taType\x12:\n\x03\x63sv\x18\x01 \x01(\x0b\x32&.strmprivacy.api.entities.v1.CsvConfigH\x00R\x03\x63sv\x12I\n\x08\x64\x61tabase\x18\x02 \x01(\x0b\x32+.strmprivacy.api.entities.v1.DatabaseConfigH\x00R\x08\x64\x61tabaseB\x10\n\tdata_type\x12\x03\xf8\x42\x01\"%\n\tCsvConfig\x12\x18\n\x07\x63harset\x18\x01 \x01(\tR\x07\x63harset\"\x8a\x05\n\rBatchExporter\x12I\n\x03ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.BatchExporterRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12G\n\nstream_ref\x18\x02 \x01(\x0b\x32&.strmprivacy.api.entities.v1.StreamRefH\x00R\tstreamRef\x12Q\n\x0ekey_stream_ref\x18\x03 \x01(\x0b\x32).strmprivacy.api.entities.v1.KeyStreamRefH\x00R\x0ckeyStreamRef\x12I\n\x08interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB\x12\xe0\x41\x02\xfa\x42\x0c\xaa\x01\t\"\x03\x08\x90\x1c\x32\x02\x08\x1eR\x08interval\x12*\n\tsink_name\x18\x05 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\x08sinkName\x12[\n\x0bpath_prefix\x18\x06 \x01(\tB:\xfa\x42\x37r5\x18\x84\x07\x32\t^.+[^\\/]$Z\x01.Z\x02..\xba\x01\x1a.well-known/acme-challenge\xd0\x01\x01R\npathPrefix\x12\x36\n\x17include_existing_events\x18\x07 \x01(\x08R\x15includeExistingEvents\x12\x65\n\x12\x64\x61ta_connector_ref\x18\x08 \x01(\x0b\x32-.strmprivacy.api.entities.v1.DataConnectorRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x10\x64\x61taConnectorRefB\x1f\n\x18stream_or_key_stream_ref\x12\x03\xf8\x42\x01\"\x98\x01\n\x15\x45xtendedBatchExporter\x12\x17\n\x04uuid\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x04uuid\x12\x19\n\x05topic\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x05topic\x12K\n\x08\x65xporter\x18\x03 \x01(\x0b\x32*.strmprivacy.api.entities.v1.BatchExporterB\x03\xe0\x41\x03R\x08\x65xporter\"\xa3\x01\n\x10\x42\x61tchExporterRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x38\n\x04name\x18\x02 \x01(\tB$\xfa\x42!r\x1f\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04name\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\xfa\x01\n\x0cKafkaCluster\x12\x43\n\x03ref\x18\x01 \x01(\x0b\x32,.strmprivacy.api.entities.v1.KafkaClusterRefB\x03\xe0\x41\x02R\x03ref\x12\x30\n\x11\x62ootstrap_servers\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x10\x62ootstrapServers\x12V\n\x0e\x61uth_mechanism\x18\x03 \x01(\x0e\x32*.strmprivacy.api.entities.v1.AuthMechanismB\x03\xe0\x41\x02R\rauthMechanism\x12\x1b\n\ttoken_uri\x18\x04 \x01(\tR\x08tokenUri\"\x93\x01\n\x0fKafkaClusterRef\x12\x1d\n\nbilling_id\x18\x01 \x01(\tR\tbillingId\x12\x35\n\x04name\x18\x02 \x01(\tB!\xfa\x42\x1er\x1c\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$R\x04name\x12*\n\nproject_id\x18\x03 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\tprojectId\"\xb3\x02\n\rKafkaExporter\x12I\n\x03ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.KafkaExporterRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12O\n\nstream_ref\x18\x02 \x01(\x0b\x32&.strmprivacy.api.entities.v1.StreamRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tstreamRef\x12H\n\x06target\x18\x03 \x01(\x0b\x32\x30.strmprivacy.api.entities.v1.KafkaExporterTargetR\x06target\x12<\n\x05users\x18\x04 \x03(\x0b\x32&.strmprivacy.api.entities.v1.KafkaUserR\x05users\"v\n\x10KafkaExporterRef\x12\x1d\n\nbilling_id\x18\x01 \x01(\tR\tbillingId\x12\x17\n\x04name\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x04name\x12*\n\nproject_id\x18\x03 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\tprojectId\"\x87\x02\n\x13KafkaExporterTarget\x12W\n\x0b\x63luster_ref\x18\x01 \x01(\x0b\x32,.strmprivacy.api.entities.v1.KafkaClusterRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\nclusterRef\x12\x34\n\x05topic\x18\x02 \x01(\tB\x1e\xfa\x42\x1br\x19\x18\xf9\x01\x32\x11^[a-zA-Z0-9._-]+$\xd0\x01\x01R\x05topic\x12(\n\tclient_id\x18\x03 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x08\x63lientId\x12\x37\n\rclient_secret\x18\x04 \x01(\tB\x12\xfa\x42\x0fr\r2\x08^[ -~]+$\xd0\x01\x01R\x0c\x63lientSecret\"\xc2\x02\n\tKafkaUser\x12\x45\n\x03ref\x18\x01 \x01(\x0b\x32).strmprivacy.api.entities.v1.KafkaUserRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12\x33\n\x13kafka_exporter_name\x18\x03 \x01(\tB\x03\xe0\x41\x03R\x11kafkaExporterName\x12\x19\n\x05topic\x18\x04 \x01(\tB\x03\xe0\x41\x03R\x05topic\x12 \n\tclient_id\x18\x05 \x01(\tB\x03\xe0\x41\x03R\x08\x63lientId\x12(\n\rclient_secret\x18\x06 \x01(\tB\x03\xe0\x41\x03R\x0c\x63lientSecret\x12R\n\x0b\x63luster_ref\x18\x07 \x01(\x0b\x32,.strmprivacy.api.entities.v1.KafkaClusterRefB\x03\xe0\x41\x03R\nclusterRef\"n\n\x0cKafkaUserRef\x12!\n\nbilling_id\x18\x01 \x01(\tB\x02\x18\x01R\tbillingId\x12\x17\n\x04name\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x04name\x12\"\n\nproject_id\x18\x03 \x01(\tB\x03\xe0\x41\x03R\tprojectId\"6\n\rConsentLevels\x12%\n\x0e\x63onsent_levels\x18\x01 \x03(\x05R\rconsentLevels\"\x9d\x01\n\x13\x43onsentLevelMapping\x12O\n\x03ref\x18\x01 \x01(\x0b\x32\x33.strmprivacy.api.entities.v1.ConsentLevelMappingRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12\x35\n\x04name\x18\x02 \x01(\tB!\xfa\x42\x1er\x1c\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$R\x04name\"\x8d\x01\n\x16\x43onsentLevelMappingRef\x12+\n\nbilling_id\x18\x01 \x01(\tB\x0c\x18\x01\xfa\x42\x07r\x05\x18\x00\xd0\x01\x01R\tbillingId\x12\x1d\n\x05level\x18\x02 \x01(\x05\x42\x07\xfa\x42\x04\x1a\x02(\x00R\x05level\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\x86\x03\n\x06Policy\x12\x18\n\x02id\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\x02id\x12\x38\n\x04name\x18\x02 \x01(\tB$\xfa\x42!r\x1f\x10\x04\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$\xd0\x01\x01R\x04name\x12*\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\x18\xe8\x07R\x0b\x64\x65scription\x12-\n\rlegal_grounds\x18\x04 \x01(\tB\x08\xfa\x42\x05r\x03\x18\xe8\x07R\x0clegalGrounds\x12\x30\n\x0eretention_days\x18\x05 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04(\x01@\x01R\rretentionDays\x12\x44\n\x05state\x18\x06 \x01(\x0e\x32).strmprivacy.api.entities.v1.Policy.StateB\x03\xe0\x41\x03R\x05state\"U\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x0f\n\x0bSTATE_DRAFT\x10\x01\x12\x10\n\x0cSTATE_ACTIVE\x10\x02\x12\x12\n\x0eSTATE_ARCHIVED\x10\x03\"\xb6\x01\n\x12WindowedEventCount\x12>\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\tstartTime\x12:\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\x07\x65ndTime\x12$\n\x0b\x65vent_count\x18\x03 \x01(\x03\x42\x03\xe0\x41\x03R\neventCount\"\xaf\x01\n\tSchemaRef\x12\x1b\n\x06handle\x18\x01 \x01(\tB\x03\xe0\x41\x02R\x06handle\x12\x17\n\x04name\x18\x02 \x01(\tB\x03\xe0\x41\x02R\x04name\x12\x1d\n\x07version\x18\x03 \x01(\tB\x03\xe0\x41\x02R\x07version\x12M\n\x0bschema_type\x18\x04 \x01(\x0e\x32\'.strmprivacy.api.entities.v1.SchemaTypeB\x03\xe0\x41\x03R\nschemaType\"\xe9\x06\n\x06Schema\x12\x42\n\x03ref\x18\x01 \x01(\x0b\x32&.strmprivacy.api.entities.v1.SchemaRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12\x44\n\x05state\x18\x02 \x01(\x0e\x32).strmprivacy.api.entities.v1.Schema.StateB\x03\xe0\x41\x03R\x05state\x12\x1b\n\tis_public\x18\x03 \x01(\x08R\x08isPublic\x12\x1e\n\ndefinition\x18\x04 \x01(\tR\ndefinition\x12%\n\x0b\x66ingerprint\x18\x05 \x01(\tB\x03\xe0\x41\x03R\x0b\x66ingerprint\x12G\n\x08metadata\x18\x06 \x01(\x0b\x32+.strmprivacy.api.entities.v1.SchemaMetadataR\x08metadata\x12_\n\rsimple_schema\x18\x07 \x01(\x0b\x32:.strmprivacy.api.entities.v1.Schema.SimpleSchemaDefinitionR\x0csimpleSchema\x12\x13\n\x02id\x18\x08 \x01(\tB\x03\xe0\x41\x03R\x02id\x1a\xbf\x02\n\x16SimpleSchemaDefinition\x12$\n\x04name\x18\x01 \x01(\tB\x10\xfa\x42\rr\x0b\x32\t^[^\\pC]+$R\x04name\x12]\n\tnamespace\x18\x02 \x01(\tB?\xfa\x42<r:25^([a-zA-Z_][a-zA-Z0-9_]*)(\\.[a-zA-Z_][a-zA-Z0-9_]*)*$\xd0\x01\x01R\tnamespace\x12\x1a\n\x03\x64oc\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\x18\x88\'R\x03\x64oc\x12\x43\n\x05nodes\x18\x04 \x03(\x0b\x32-.strmprivacy.api.entities.v1.SimpleSchemaNodeR\x05nodes\x12?\n\tavro_name\x18\x05 \x01(\tB\"\xfa\x42\x1fr\x1d\x32\x18^[a-zA-Z_][a-zA-Z0-9_]*$\xd0\x01\x01R\x08\x61vroName\"p\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\t\n\x05\x44RAFT\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x0c\n\x08\x41RCHIVED\x10\x03\x12\r\n\tIN_REVIEW\x10\x04\x12\x0e\n\nINCOMPLETE\x10\x05\x12\x0c\n\x08\x41PPROVED\x10\x06\"\xe3\x02\n\x10SimpleSchemaNode\x12O\n\x04type\x18\x01 \x01(\x0e\x32\x31.strmprivacy.api.entities.v1.SimpleSchemaNodeTypeB\x08\xfa\x42\x05\x82\x01\x02 \x00R\x04type\x12$\n\x04name\x18\x02 \x01(\tB\x10\xfa\x42\rr\x0b\x32\t^[^\\pC]+$R\x04name\x12?\n\tavro_name\x18\x07 \x01(\tB\"\xfa\x42\x1fr\x1d\x32\x18^[a-zA-Z_][a-zA-Z0-9_]*$\xd0\x01\x01R\x08\x61vroName\x12\x1a\n\x08repeated\x18\x03 \x01(\x08R\x08repeated\x12\x1a\n\x08required\x18\x04 \x01(\x08R\x08required\x12\x43\n\x05nodes\x18\x05 \x03(\x0b\x32-.strmprivacy.api.entities.v1.SimpleSchemaNodeR\x05nodes\x12\x1a\n\x03\x64oc\x18\x06 \x01(\tB\x08\xfa\x42\x05r\x03\x18\x88\'R\x03\x64oc\"\xd5\x02\n\x0eSchemaMetadata\x12-\n\x05title\x18\x01 \x01(\tB\x17\xfa\x42\x14r\x12\x10\x04\x18\x64\x32\t^[^\\pC]+$\xd0\x01\x01R\x05title\x12*\n\x0b\x64\x65scription\x18\x02 \x01(\tB\x08\xfa\x42\x05r\x03\x18\x88\'R\x0b\x64\x65scription\x12@\n\x0b\x63reate_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\ncreateTime\x12\x30\n\x08icon_uri\x18\x04 \x01(\tB\x15\xfa\x42\x12r\x10:\x08https://\xd0\x01\x01\x88\x01\x01R\x07iconUri\x12:\n\x06labels\x18\x05 \x03(\x0b\x32\".strmprivacy.api.entities.v1.LabelR\x06labels\x12\x18\n\x07\x64omains\x18\x06 \x03(\tR\x07\x64omains\x12\x1e\n\nindustries\x18\x07 \x03(\tR\nindustries\"\x9a\x01\n\x10\x45ventContractRef\x12\x1f\n\x06handle\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x04R\x06handle\x12\x33\n\x04name\x18\x02 \x01(\tB\x1f\xfa\x42\x1cr\x1a\x10\x04\x18\x64\x32\x14^[\\pL\\pN\\pS\\pM\\pP]+$R\x04name\x12\x30\n\x07version\x18\x03 \x01(\tB\x16\xfa\x42\x13r\x11\x32\x0f^\\d+\\.\\d+\\.\\d+$R\x07version\"\x82\x06\n\rEventContract\x12\x44\n\x03ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.EventContractRefB\x03\xe0\x41\x02R\x03ref\x12K\n\x05state\x18\x02 \x01(\x0e\x32\x30.strmprivacy.api.entities.v1.EventContract.StateB\x03\xe0\x41\x03R\x05state\x12J\n\nschema_ref\x18\x03 \x01(\x0b\x32&.strmprivacy.api.entities.v1.SchemaRefB\x03\xe0\x41\x02R\tschemaRef\x12\x1b\n\tis_public\x18\x04 \x01(\x08R\x08isPublic\x12 \n\tkey_field\x18\x05 \x01(\tB\x03\xe0\x41\x02R\x08keyField\x12X\n\npii_fields\x18\x06 \x03(\x0b\x32\x39.strmprivacy.api.entities.v1.EventContract.PiiFieldsEntryR\tpiiFields\x12I\n\x0bvalidations\x18\x07 \x03(\x0b\x32\'.strmprivacy.api.entities.v1.ValidationR\x0bvalidations\x12N\n\x08metadata\x18\x08 \x01(\x0b\x32\x32.strmprivacy.api.entities.v1.EventContractMetadataR\x08metadata\x12\x0e\n\x02id\x18\t \x01(\tR\x02id\x12,\n\x12\x64\x61ta_subject_field\x18\n \x01(\tR\x10\x64\x61taSubjectField\x1a<\n\x0ePiiFieldsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x05R\x05value:\x02\x38\x01\"b\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\t\n\x05\x44RAFT\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x0c\n\x08\x41RCHIVED\x10\x03\x12\r\n\tIN_REVIEW\x10\x04\x12\x0e\n\nINCOMPLETE\x10\x05\"\xc0\x02\n\x15\x45ventContractMetadata\x12\x19\n\x05title\x18\x01 \x01(\tB\x03\xe0\x41\x01R\x05title\x12%\n\x0b\x64\x65scription\x18\x02 \x01(\tB\x03\xe0\x41\x01R\x0b\x64\x65scription\x12@\n\x0b\x63reate_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\ncreateTime\x12\x1e\n\x08icon_uri\x18\x04 \x01(\tB\x03\xe0\x41\x01R\x07iconUri\x12?\n\x06labels\x18\x05 \x03(\x0b\x32\".strmprivacy.api.entities.v1.LabelB\x03\xe0\x41\x01R\x06labels\x12\x1d\n\x07\x64omains\x18\x06 \x03(\tB\x03\xe0\x41\x01R\x07\x64omains\x12#\n\nindustries\x18\x07 \x03(\tB\x03\xe0\x41\x01R\nindustries\"8\n\x05Label\x12\x19\n\x03key\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"l\n\nValidation\x12\x1d\n\x05\x66ield\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x05\x66ield\x12 \n\x04type\x18\x02 \x01(\tB\x0c\xfa\x42\tr\x07R\x05regexR\x04type\x12\x1d\n\x05value\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x05value\"\xfe\x02\n\nStreamTree\x12@\n\x06stream\x18\x01 \x01(\x0b\x32#.strmprivacy.api.entities.v1.StreamB\x03\xe0\x41\x02R\x06stream\x12\x45\n\nkey_stream\x18\x02 \x01(\x0b\x32&.strmprivacy.api.entities.v1.KeyStreamR\tkeyStream\x12=\n\x07\x64\x65rived\x18\x03 \x03(\x0b\x32#.strmprivacy.api.entities.v1.StreamR\x07\x64\x65rived\x12S\n\x0f\x62\x61tch_exporters\x18\x04 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchExporterR\x0e\x62\x61tchExporters\x12S\n\x0fkafka_exporters\x18\x05 \x03(\x0b\x32*.strmprivacy.api.entities.v1.KafkaExporterR\x0ekafkaExporters\"\x9f\x01\n\x08SinkTree\x12:\n\x04sink\x18\x01 \x01(\x0b\x32!.strmprivacy.api.entities.v1.SinkB\x03\xe0\x41\x02R\x04sink\x12S\n\x0f\x62\x61tch_exporters\x18\x02 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchExporterR\x0e\x62\x61tchExporters:\x02\x18\x01\"\xc8\x06\n\x08\x42\x61tchJob\x12\x44\n\x03ref\x18\x01 \x01(\x0b\x32(.strmprivacy.api.entities.v1.BatchJobRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12G\n\x06states\x18\x02 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchJobStateB\x03\xe0\x41\x03R\x06states\x12\\\n\x0bsource_data\x18\x03 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\nsourceData\x12N\n\x07\x63onsent\x18\x04 \x01(\x0b\x32*.strmprivacy.api.entities.v1.ConsentConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x07\x63onsent\x12W\n\nencryption\x18\x05 \x01(\x0b\x32-.strmprivacy.api.entities.v1.EncryptionConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\nencryption\x12\x65\n\x12\x65vent_contract_ref\x18\x06 \x01(\x0b\x32-.strmprivacy.api.entities.v1.EventContractRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x10\x65ventContractRef\x12[\n\x0e\x65ncrypted_data\x18\x07 \x01(\x0b\x32*.strmprivacy.api.entities.v1.EncryptedDataB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\rencryptedData\x12k\n\x14\x65ncryption_keys_data\x18\x08 \x01(\x0b\x32/.strmprivacy.api.entities.v1.EncryptionKeysDataB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x12\x65ncryptionKeysData\x12K\n\x0c\x64\x65rived_data\x18\t \x03(\x0b\x32(.strmprivacy.api.entities.v1.DerivedDataR\x0b\x64\x65rivedData\x12(\n\tpolicy_id\x18\n \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x08policyId\"\xf0\x01\n\x0f\x42\x61tchJobWrapper\x12Y\n\x14\x65ncryption_batch_job\x18\x01 \x01(\x0b\x32%.strmprivacy.api.entities.v1.BatchJobH\x00R\x12\x65ncryptionBatchJob\x12v\n\x1bmicro_aggregation_batch_job\x18\x02 \x01(\x0b\x32\x35.strmprivacy.api.entities.v1.MicroAggregationBatchJobH\x00R\x18microAggregationBatchJobB\n\n\x03job\x12\x03\xf8\x42\x01\"\x9a\x01\n\x10\x45xtendedBatchJob\x12\x46\n\tbatch_job\x18\x01 \x01(\x0b\x32%.strmprivacy.api.entities.v1.BatchJobB\x02\x18\x01R\x08\x62\x61tchJob\x12>\n\x03job\x18\x02 \x01(\x0b\x32,.strmprivacy.api.entities.v1.BatchJobWrapperR\x03job\"y\n\x0b\x42\x61tchJobRef\x12,\n\nbilling_id\x18\x01 \x01(\tB\r\x18\x01\xfa\x42\x08r\x06\x98\x01\x00\xd0\x01\x01R\tbillingId\x12\x13\n\x02id\x18\x02 \x01(\tB\x03\xe0\x41\x03R\x02id\x12\'\n\nproject_id\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\"\xb9\x01\n\rBatchJobState\x12>\n\nstate_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\tstateTime\x12I\n\x05state\x18\x02 \x01(\x0e\x32..strmprivacy.api.entities.v1.BatchJobStateTypeB\x03\xe0\x41\x03R\x05state\x12\x1d\n\x07message\x18\x03 \x01(\tB\x03\xe0\x41\x01R\x07message\"\xda\x02\n\x14\x44\x61taConnectorAndType\x12\x65\n\x12\x64\x61ta_connector_ref\x18\x01 \x01(\x0b\x32-.strmprivacy.api.entities.v1.DataConnectorRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x10\x64\x61taConnectorRef\x12[\n\x0bpath_prefix\x18\x02 \x01(\tB:\xfa\x42\x37r5\x18\x84\x07\x32\t^.+[^\\/]$Z\x01.Z\x02..\xba\x01\x1a.well-known/acme-challenge\xd0\x01\x01R\npathPrefix\x12\x30\n\tfile_name\x18\x03 \x01(\tB\x13\xfa\x42\x10r\x0e\x32\t^[^\\pC]+$\xd0\x01\x01R\x08\x66ileName\x12L\n\tdata_type\x18\x04 \x01(\x0b\x32%.strmprivacy.api.entities.v1.DataTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x08\x64\x61taType\"}\n\x0e\x44\x61tabaseConfig\x12\"\n\x06schema\x18\x01 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\xd0\x01\x01R\x06schema\x12\x1d\n\x05table\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x05table\x12(\n\x07\x63olumns\x18\x03 \x03(\tB\x0e\xfa\x42\x0b\x92\x01\x08\"\x04r\x02\x10\x01(\x01R\x07\x63olumns\"\xbb\x01\n\rConsentConfig\x12\x39\n\x16\x64\x65\x66\x61ult_consent_levels\x18\x01 \x03(\x05\x42\x03\xe0\x41\x01R\x14\x64\x65\x66\x61ultConsentLevels\x12o\n\x17\x63onsent_level_extractor\x18\x02 \x01(\x0b\x32\x32.strmprivacy.api.entities.v1.ConsentLevelExtractorB\x03\xe0\x41\x01R\x15\x63onsentLevelExtractor\"\x89\x02\n\x15\x43onsentLevelExtractor\x12\x14\n\x05\x66ield\x18\x01 \x01(\tR\x05\x66ield\x12l\n\x0e\x66ield_patterns\x18\x02 \x03(\x0b\x32\x45.strmprivacy.api.entities.v1.ConsentLevelExtractor.FieldPatternsEntryR\rfieldPatterns\x1al\n\x12\x46ieldPatternsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12@\n\x05value\x18\x02 \x01(\x0b\x32*.strmprivacy.api.entities.v1.ConsentLevelsR\x05value:\x02\x38\x01\"\xa2\x01\n\x10\x45ncryptionConfig\x12\x61\n\x10timestamp_config\x18\x01 \x01(\x0b\x32,.strmprivacy.api.entities.v1.TimestampConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0ftimestampConfig\x12+\n\x12\x62\x61tch_job_group_id\x18\x02 \x01(\tR\x0f\x62\x61tchJobGroupId\"\xa1\x01\n\x0fTimestampConfig\x12*\n\x05\x66ield\x18\x01 \x01(\tB\x14\xfa\x42\x11r\x0f\x10\x04\x18\x32\x32\t^[^\\pC]+$R\x05\x66ield\x12\x1f\n\x06\x66ormat\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x06\x66ormat\x12\x41\n\x11\x64\x65\x66\x61ult_time_zone\x18\x03 \x01(\x0b\x32\x15.google.type.TimeZoneR\x0f\x64\x65\x66\x61ultTimeZone\"d\n\rEncryptedData\x12S\n\x06target\x18\x01 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x06target\"i\n\x12\x45ncryptionKeysData\x12S\n\x06target\x18\x01 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x06target\"\xb1\x02\n\x0b\x44\x65rivedData\x12N\n\x06target\x18\x01 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x03\xe0\x41\x02R\x06target\x12%\n\x0e\x63onsent_levels\x18\x02 \x03(\x05R\rconsentLevels\x12[\n\x12\x63onsent_level_type\x18\x03 \x01(\x0e\x32-.strmprivacy.api.entities.v1.ConsentLevelTypeR\x10\x63onsentLevelType\x12N\n\rmasked_fields\x18\x04 \x01(\x0b\x32).strmprivacy.api.entities.v1.MaskedFieldsR\x0cmaskedFields\"\xb7\x04\n\x18MicroAggregationBatchJob\x12\x44\n\x03ref\x18\x01 \x01(\x0b\x32(.strmprivacy.api.entities.v1.BatchJobRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12G\n\x06states\x18\x02 \x03(\x0b\x32*.strmprivacy.api.entities.v1.BatchJobStateB\x03\xe0\x41\x03R\x06states\x12\\\n\x0bsource_data\x18\x03 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\nsourceData\x12\\\n\x0btarget_data\x18\x04 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataConnectorAndTypeB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\ntargetData\x12\x62\n\x11\x64\x61ta_contract_ref\x18\x05 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0f\x64\x61taContractRef\x12l\n\x12\x61ggregation_config\x18\x06 \x01(\x0b\x32\x33.strmprivacy.api.entities.v1.MicroAggregationConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x11\x61ggregationConfig\"\x80\x01\n\x16MicroAggregationConfig\x12\x37\n\x13minimum_k_anonymity\x18\x01 \x01(\x05\x42\x07\xfa\x42\x04\x1a\x02(\x02R\x11minimumKAnonymity\x12-\n\x12\x61ggregation_fields\x18\x02 \x03(\tR\x11\x61ggregationFields\"\x92\x01\n\x0f\x44\x61taContractRef\x12\"\n\x06handle\x18\x01 \x01(\tB\n\xe0\x41\x02\xfa\x42\x04r\x02\x10\x04R\x06handle\x12&\n\x04name\x18\x02 \x01(\tB\x12\xfa\x42\x0fr\r\x10\x04\x18\x64\x32\x07^[^/]+$R\x04name\x12\x33\n\x07version\x18\x03 \x01(\tB\x19\xe0\x41\x02\xfa\x42\x13r\x11\x32\x0f^\\d+\\.\\d+\\.\\d+$R\x07version\"\x94\x07\n\x0c\x44\x61taContract\x12\x13\n\x02id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x02id\x12H\n\x03ref\x18\x02 \x01(\x0b\x32,.strmprivacy.api.entities.v1.DataContractRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x03ref\x12J\n\x05state\x18\x03 \x01(\x0e\x32/.strmprivacy.api.entities.v1.DataContract.StateB\x03\xe0\x41\x03R\x05state\x12\x1b\n\tis_public\x18\x04 \x01(\x08R\x08isPublic\x12$\n\tkey_field\x18\x05 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08keyField\x12[\n\npii_fields\x18\x06 \x03(\x0b\x32\x38.strmprivacy.api.entities.v1.DataContract.PiiFieldsEntryB\x02\x18\x01R\tpiiFields\x12I\n\x0bvalidations\x18\x07 \x03(\x0b\x32\'.strmprivacy.api.entities.v1.ValidationR\x0bvalidations\x12M\n\x08metadata\x18\x08 \x01(\x0b\x32\x31.strmprivacy.api.entities.v1.DataContractMetadataR\x08metadata\x12\x45\n\x06schema\x18\t \x01(\x0b\x32#.strmprivacy.api.entities.v1.SchemaB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x06schema\x12,\n\x12\x64\x61ta_subject_field\x18\n \x01(\tR\x10\x64\x61taSubjectField\x12\'\n\nproject_id\x18\x0b \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\tprojectId\x12Q\n\x0e\x66ield_metadata\x18\x0c \x03(\x0b\x32*.strmprivacy.api.entities.v1.FieldMetadataR\rfieldMetadata\x1a<\n\x0ePiiFieldsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x05R\x05value:\x02\x38\x01\"p\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\t\n\x05\x44RAFT\x10\x01\x12\r\n\tIN_REVIEW\x10\x02\x12\n\n\x06\x41\x43TIVE\x10\x03\x12\x0c\n\x08\x41RCHIVED\x10\x04\x12\x0e\n\nINCOMPLETE\x10\x05\x12\x0c\n\x08\x41PPROVED\x10\x06\"\xe1\x06\n\rFieldMetadata\x12\x1d\n\nfield_name\x18\x01 \x01(\tR\tfieldName\x12o\n\x14personal_data_config\x18\x02 \x01(\x0b\x32=.strmprivacy.api.entities.v1.FieldMetadata.PersonalDataConfigR\x12personalDataConfig\x12\x64\n\x15statistical_data_type\x18\x03 \x01(\x0e\x32\x30.strmprivacy.api.entities.v1.StatisticalDataTypeR\x13statisticalDataType\x12%\n\x0eordinal_values\x18\x04 \x03(\tR\rordinalValues\x12o\n\x14null_handling_config\x18\x05 \x01(\x0b\x32=.strmprivacy.api.entities.v1.FieldMetadata.NullHandlingConfigR\x12nullHandlingConfig\x1a\xc0\x01\n\x12PersonalDataConfig\x12\x1a\n\x06is_pii\x18\x01 \x01(\x08\x42\x03\xe0\x41\x02R\x05isPii\x12#\n\x0bis_quasi_id\x18\x02 \x01(\x08\x42\x03\xe0\x41\x02R\tisQuasiId\x12#\n\rpurpose_level\x18\x03 \x01(\x05R\x0cpurposeLevel\x12\x44\n\x1fgdpr_special_personal_data_type\x18\x04 \x01(\tR\x1bgdprSpecialPersonalDataType\x1a\xfe\x01\n\x12NullHandlingConfig\x12g\n\x04type\x18\x01 \x01(\x0e\x32N.strmprivacy.api.entities.v1.FieldMetadata.NullHandlingConfig.NullHandlingTypeB\x03\xe0\x41\x02R\x04type\x12#\n\rdefault_value\x18\x02 \x01(\tR\x0c\x64\x65\x66\x61ultValue\"Z\n\x10NullHandlingType\x12\"\n\x1eNULL_HANDLING_TYPE_UNSPECIFIED\x10\x00\x12\x0f\n\x0b\x44ROP_RECORD\x10\x01\x12\x11\n\rDEFAULT_VALUE\x10\x02\"\x9f\x02\n\x14\x44\x61taContractMetadata\x12-\n\x05title\x18\x01 \x01(\tB\x17\xfa\x42\x14r\x12\x10\x04\x18\x64\x32\t^[^\\pC]+$\xd0\x01\x01R\x05title\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12@\n\x0b\x63reate_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x03\xe0\x41\x03R\ncreateTime\x12:\n\x06labels\x18\x05 \x03(\x0b\x32\".strmprivacy.api.entities.v1.LabelR\x06labels\x12\x18\n\x07\x64omains\x18\x06 \x03(\tR\x07\x64omains\x12\x1e\n\nindustries\x18\x07 \x03(\tR\nindustries\"\xbd\x02\n\x07Project\x12\x13\n\x02id\x18\x01 \x01(\tB\x03\xe0\x41\x03R\x02id\x12\x35\n\x04name\x18\x02 \x01(\tB!\xfa\x42\x1er\x1c\x10\x02\x18\x64\x32\x16^[\\pL\\pN\\pS\\pM\\pP\\s]+$R\x04name\x12*\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x08\xfa\x42\x05r\x03\x18\x88\'R\x0b\x64\x65scription\x12,\n\x0forganization_id\x18\x04 \x01(\tB\x03\xe0\x41\x03R\x0eorganizationId\x12\x45\n\x05state\x18\x05 \x01(\x0e\x32*.strmprivacy.api.entities.v1.Project.StateB\x03\xe0\x41\x03R\x05state\"E\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x0f\n\x0bOPERATIONAL\x10\x01\x12\x14\n\x10PENDING_DELETION\x10\x02\"\xbe\x02\n\x04User\x12 \n\x05\x65mail\x18\x01 \x01(\tB\n\xfa\x42\x07r\x05\xd0\x01\x01`\x01R\x05\x65mail\x12\x1d\n\nfirst_name\x18\x02 \x01(\tR\tfirstName\x12\x1b\n\tlast_name\x18\x03 \x01(\tR\x08lastName\x12\x44\n\nuser_roles\x18\x04 \x03(\x0e\x32%.strmprivacy.api.entities.v1.UserRoleR\tuserRoles\x12\x35\n\x10\x65xternal_user_id\x18\x05 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0e\x65xternalUserId\x12\x34\n\x0forganization_id\x18\x06 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0eorganizationId\x12%\n\x0e\x66unction_title\x18\x07 \x01(\tR\rfunctionTitle\"\x82\x01\n\x0ePurposeMapping\x12\x1d\n\x05level\x18\x01 \x01(\x05\x42\x07\xfa\x42\x04\x1a\x02(\x00R\x05level\x12#\n\x07purpose\x18\x02 \x01(\tB\t\xfa\x42\x06r\x04\x10\x02\x18\x64R\x07purpose\x12,\n\x0b\x64\x65scription\x18\x03 \x01(\tB\n\xfa\x42\x07r\x05\x10\x02\xd0\x01\x01R\x0b\x64\x65scription\"\xaf\x01\n\nGenericRef\x12J\n\x04type\x18\x01 \x01(\x0e\x32\x36.strmprivacy.api.entities.v1.GenericRef.GenericRefTypeR\x04type\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02id\"E\n\x0eGenericRefType\x12 \n\x1cGENERIC_REF_TYPE_UNSPECIFIED\x10\x00\x12\x11\n\rDATA_CONTRACT\x10\x01\"\xf9\x02\n\x07\x43omment\x12\x1b\n\x02id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x02id\x12\x45\n\x0b\x63reate_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x00R\ncreateTime\x12P\n\nentity_ref\x18\x03 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\x12$\n\x07\x63ontent\x18\x04 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xe8\x07R\x07\x63ontent\x12\x45\n\x07\x63reator\x18\x05 \x01(\x0b\x32!.strmprivacy.api.entities.v1.UserB\x08\xfa\x42\x05\x8a\x01\x02\x10\x00R\x07\x63reator\x12*\n\nproject_id\x18\x06 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\tprojectId\x12\x1f\n\x0b\x65ntity_name\x18\x07 \x01(\tR\nentityName\"\xfd\x02\n\x0f\x41uditTrailEntry\x12\x1b\n\x02id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x02id\x12\x45\n\x0b\x63reate_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x00R\ncreateTime\x12P\n\nentity_ref\x18\x03 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\x12$\n\x07\x63ontent\x18\x04 \x01(\tB\n\xfa\x42\x07r\x05\x10\x01\x18\xe8\x07R\x07\x63ontent\x12\x41\n\x05\x61\x63tor\x18\x05 \x01(\x0b\x32!.strmprivacy.api.entities.v1.UserB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x05\x61\x63tor\x12*\n\nproject_id\x18\x06 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\tprojectId\x12\x1f\n\x0b\x65ntity_name\x18\x07 \x01(\tR\nentityName*]\n\x08UserRole\x12\x19\n\x15USER_ROLE_UNSPECIFIED\x10\x00\x12\t\n\x05\x41\x44MIN\x10\x01\x12\x11\n\rPROJECT_ADMIN\x10\x02\x12\x0c\n\x08\x41PPROVER\x10\x03\x12\n\n\x06MEMBER\x10\x04*\x8d\x01\n\x11\x42\x61tchJobStateType\x12$\n BATCH_JOB_STATE_TYPE_UNSPECIFIED\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\x0b\n\x07STARTED\x10\x02\x12\x12\n\x0e\x45RROR_STARTING\x10\x03\x12\x0b\n\x07RUNNING\x10\x04\x12\x0c\n\x08\x46INISHED\x10\x05\x12\t\n\x05\x45RROR\x10\x06*T\n\x10\x43onsentLevelType\x12\"\n\x1e\x43ONSENT_LEVEL_TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nCUMULATIVE\x10\x01\x12\x0c\n\x08GRANULAR\x10\x02*=\n\x08SinkType\x12\x19\n\x15SINK_TYPE_UNSPECIFIED\x10\x00\x12\x06\n\x02S3\x10\x01\x12\n\n\x06GCLOUD\x10\x02\x1a\x02\x18\x01*M\n\rAuthMechanism\x12\x1e\n\x1a\x41UTH_MECHANISM_UNSPECIFIED\x10\x00\x12\x0e\n\nSASL_PLAIN\x10\x01\x12\x0c\n\x08SASL_SSL\x10\x02*C\n\nSchemaType\x12\x1b\n\x17SCHEMA_TYPE_UNSPECIFIED\x10\x00\x12\x08\n\x04\x41VRO\x10\x01\x12\x0e\n\nJSONSCHEMA\x10\x02*\x84\x01\n\x14SimpleSchemaNodeType\x12\'\n#SIMPLE_SCHEMA_NODE_TYPE_UNSPECIFIED\x10\x00\x12\n\n\x06STRING\x10\x01\x12\x0b\n\x07\x42OOLEAN\x10\x02\x12\t\n\x05\x46LOAT\x10\x03\x12\x0b\n\x07INTEGER\x10\x04\x12\x08\n\x04LONG\x10\x05\x12\x08\n\x04NODE\x10\n*_\n\x13\x46ilterPublicPrivate\x12%\n!FILTER_PUBLIC_PRIVATE_UNSPECIFIED\x10\x00\x12\x0f\n\x0bONLY_PUBLIC\x10\x01\x12\x10\n\x0cONLY_PRIVATE\x10\x02*e\n\x13StatisticalDataType\x12%\n!STATISTICAL_DATA_TYPE_UNSPECIFIED\x10\x00\x12\x0b\n\x07NOMINAL\x10\x01\x12\x0b\n\x07ORDINAL\x10\x02\x12\r\n\tNUMERICAL\x10\x03*\x92\x01\n\x10SubscriptionPlan\x12!\n\x1dSUBSCRIPTION_PLAN_UNSPECIFIED\x10\x00\x12\x08\n\x04\x46REE\x10\x01\x12\x0c\n\x08\x42USINESS\x10\x02\x12\x0f\n\x0bSELF_HOSTED\x10\x03\x12\x18\n\x14\x41WS_MARKETPLACE_PAYG\x10\x04\x12\x18\n\x14\x41WS_MARKETPLACE_BYOL\x10\x05*c\n\x0c\x44\x61tabaseType\x12\x1d\n\x19\x44\x41TABASE_TYPE_UNSPECIFIED\x10\x00\x12\x0c\n\x08POSTGRES\x10\x01\x12\t\n\x05MYSQL\x10\x02\x12\x0c\n\x08\x42IGQUERY\x10\x03\x12\r\n\tSNOWFLAKE\x10\x04\x42i\n\x1eio.strmprivacy.api.entities.v1P\x01ZEgithub.com/strmprivacy/api-definitions-go/v2/api/entities/v1;entitiesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'strmprivacy.api.entities.v1.entities_v1_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036io.strmprivacy.api.entities.v1P\001ZEgithub.com/strmprivacy/api-definitions-go/v2/api/entities/v1;entities'
@@ -468,48 +468,50 @@
   _COMMENT.fields_by_name['create_time']._serialized_options = b'\372B\005\262\001\002\010\000'
   _COMMENT.fields_by_name['entity_ref']._options = None
   _COMMENT.fields_by_name['entity_ref']._serialized_options = b'\372B\005\212\001\002\020\001'
   _COMMENT.fields_by_name['content']._options = None
   _COMMENT.fields_by_name['content']._serialized_options = b'\372B\007r\005\020\001\030\350\007'
   _COMMENT.fields_by_name['creator']._options = None
   _COMMENT.fields_by_name['creator']._serialized_options = b'\372B\005\212\001\002\020\000'
+  _COMMENT.fields_by_name['project_id']._options = None
+  _COMMENT.fields_by_name['project_id']._serialized_options = b'\372B\010r\006\320\001\001\260\001\001'
   _AUDITTRAILENTRY.fields_by_name['id']._options = None
   _AUDITTRAILENTRY.fields_by_name['id']._serialized_options = b'\372B\010r\006\320\001\001\260\001\001'
   _AUDITTRAILENTRY.fields_by_name['create_time']._options = None
   _AUDITTRAILENTRY.fields_by_name['create_time']._serialized_options = b'\372B\005\262\001\002\010\000'
   _AUDITTRAILENTRY.fields_by_name['entity_ref']._options = None
   _AUDITTRAILENTRY.fields_by_name['entity_ref']._serialized_options = b'\372B\005\212\001\002\020\001'
   _AUDITTRAILENTRY.fields_by_name['content']._options = None
   _AUDITTRAILENTRY.fields_by_name['content']._serialized_options = b'\372B\007r\005\020\001\030\350\007'
   _AUDITTRAILENTRY.fields_by_name['actor']._options = None
   _AUDITTRAILENTRY.fields_by_name['actor']._serialized_options = b'\372B\005\212\001\002\020\001'
   _AUDITTRAILENTRY.fields_by_name['project_id']._options = None
   _AUDITTRAILENTRY.fields_by_name['project_id']._serialized_options = b'\372B\010r\006\320\001\001\260\001\001'
-  _USERROLE._serialized_start=20148
-  _USERROLE._serialized_end=20241
-  _BATCHJOBSTATETYPE._serialized_start=20244
-  _BATCHJOBSTATETYPE._serialized_end=20385
-  _CONSENTLEVELTYPE._serialized_start=20387
-  _CONSENTLEVELTYPE._serialized_end=20471
-  _SINKTYPE._serialized_start=20473
-  _SINKTYPE._serialized_end=20534
-  _AUTHMECHANISM._serialized_start=20536
-  _AUTHMECHANISM._serialized_end=20613
-  _SCHEMATYPE._serialized_start=20615
-  _SCHEMATYPE._serialized_end=20682
-  _SIMPLESCHEMANODETYPE._serialized_start=20685
-  _SIMPLESCHEMANODETYPE._serialized_end=20817
-  _FILTERPUBLICPRIVATE._serialized_start=20819
-  _FILTERPUBLICPRIVATE._serialized_end=20914
-  _STATISTICALDATATYPE._serialized_start=20916
-  _STATISTICALDATATYPE._serialized_end=21017
-  _SUBSCRIPTIONPLAN._serialized_start=21020
-  _SUBSCRIPTIONPLAN._serialized_end=21166
-  _DATABASETYPE._serialized_start=21168
-  _DATABASETYPE._serialized_end=21267
+  _USERROLE._serialized_start=20225
+  _USERROLE._serialized_end=20318
+  _BATCHJOBSTATETYPE._serialized_start=20321
+  _BATCHJOBSTATETYPE._serialized_end=20462
+  _CONSENTLEVELTYPE._serialized_start=20464
+  _CONSENTLEVELTYPE._serialized_end=20548
+  _SINKTYPE._serialized_start=20550
+  _SINKTYPE._serialized_end=20611
+  _AUTHMECHANISM._serialized_start=20613
+  _AUTHMECHANISM._serialized_end=20690
+  _SCHEMATYPE._serialized_start=20692
+  _SCHEMATYPE._serialized_end=20759
+  _SIMPLESCHEMANODETYPE._serialized_start=20762
+  _SIMPLESCHEMANODETYPE._serialized_end=20894
+  _FILTERPUBLICPRIVATE._serialized_start=20896
+  _FILTERPUBLICPRIVATE._serialized_end=20991
+  _STATISTICALDATATYPE._serialized_start=20993
+  _STATISTICALDATATYPE._serialized_end=21094
+  _SUBSCRIPTIONPLAN._serialized_start=21097
+  _SUBSCRIPTIONPLAN._serialized_end=21243
+  _DATABASETYPE._serialized_start=21245
+  _DATABASETYPE._serialized_end=21344
   _STREAM._serialized_start=230
   _STREAM._serialized_end=913
   _EXTENDEDSTREAM._serialized_start=916
   _EXTENDEDSTREAM._serialized_end=1086
   _EXTENDEDSTREAMGROUP._serialized_start=1089
   _EXTENDEDSTREAMGROUP._serialized_end=1283
   _MASKEDFIELDS._serialized_start=1286
@@ -677,11 +679,11 @@
   _PURPOSEMAPPING._serialized_start=19151
   _PURPOSEMAPPING._serialized_end=19281
   _GENERICREF._serialized_start=19284
   _GENERICREF._serialized_end=19459
   _GENERICREF_GENERICREFTYPE._serialized_start=19390
   _GENERICREF_GENERICREFTYPE._serialized_end=19459
   _COMMENT._serialized_start=19462
-  _COMMENT._serialized_end=19762
-  _AUDITTRAILENTRY._serialized_start=19765
-  _AUDITTRAILENTRY._serialized_end=20146
+  _COMMENT._serialized_end=19839
+  _AUDITTRAILENTRY._serialized_start=19842
+  _AUDITTRAILENTRY._serialized_end=20223
 # @@protoc_insertion_point(module_scope)
```

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/handles/v1/handles_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/handles/v1/handles_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/handles/v1/handles_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/handles/v1/handles_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/entities_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/installations/v1/entities_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/installations_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/installations/v1/installations_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/installations_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/installations/v1/installations_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/installed_components_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/installations/v1/installed_components_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/installations/v1/installed_components_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/installations/v1/installed_components_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/key_streams/v1/key_streams_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/key_streams/v1/key_streams_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/monitoring/v1/monitoring_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/monitoring/v1/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/monitoring/v1/monitoring_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/monitoring/v1/monitoring_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/notifications/v1/notifications_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/notifications/v1/notifications_v1_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,26 +12,30 @@
 
 
 from strmprivacy.api.entities.v1 import entities_v1_pb2 as strmprivacy_dot_api_dot_entities_dot_v1_dot_entities__v1__pb2
 from validate import validate_pb2 as validate_dot_validate__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7strmprivacy/api/notifications/v1/notifications_v1.proto\x12 strmprivacy.api.notifications.v1\x1a-strmprivacy/api/entities/v1/entities_v1.proto\x1a\x17validate/validate.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x1d\n\x1bReceiveNotificationsRequest\"v\n\x1cReceiveNotificationsResponse\x12V\n\x0cnotification\x18\x01 \x01(\x0b\x32\x32.strmprivacy.api.notifications.v1.UserNotificationR\x0cnotification\"\xca\x01\n\x18NotifySubscribersRequest\x12P\n\nentity_ref\x18\x01 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\x12\\\n\x0cnotification\x18\x02 \x01(\x0b\x32..strmprivacy.api.notifications.v1.NotificationB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0cnotification\"\x1b\n\x19NotifySubscribersResponse\"\x83\x02\n\x0cNotification\x12\x45\n\x0b\x63reate_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x00R\ncreateTime\x12@\n\x07\x63omment\x18\x02 \x01(\x0b\x32$.strmprivacy.api.entities.v1.CommentH\x00R\x07\x63omment\x12Z\n\x11\x61udit_trail_entry\x18\x03 \x01(\x0b\x32,.strmprivacy.api.entities.v1.AuditTrailEntryH\x00R\x0f\x61uditTrailEntryB\x0e\n\x0cnotification\"\xa4\x02\n\x10UserNotification\x12\x1b\n\x02id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x02id\x12\\\n\x0cnotification\x18\x02 \x01(\x0b\x32..strmprivacy.api.notifications.v1.NotificationB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0cnotification\x12\x1f\n\x06reason\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x06reason\x12(\n\x10\x65xternal_user_id\x18\x04 \x01(\tR\x0e\x65xternalUserId\x12J\n\x0email_sent_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x00R\x0cmailSentTime\"\xa8\x01\n\x1dSubscribeNotificationsRequest\x12\x35\n\x10\x65xternal_user_id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0e\x65xternalUserId\x12P\n\nentity_ref\x18\x02 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\" \n\x1eSubscribeNotificationsResponse\"\xaa\x01\n\x1fUnSubscribeNotificationsRequest\x12\x35\n\x10\x65xternal_user_id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0e\x65xternalUserId\x12P\n\nentity_ref\x18\x02 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\"\"\n UnSubscribeNotificationsResponse\"Q\n\x18ListSubscriptionsRequest\x12\x35\n\x10\x65xternal_user_id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0e\x65xternalUserId\"q\n\x19ListSubscriptionsResponse\x12T\n\rsubscriptions\x18\x01 \x03(\x0b\x32..strmprivacy.api.notifications.v1.SubscriptionR\rsubscriptions\"\x97\x01\n\x0cSubscription\x12\x35\n\x10\x65xternal_user_id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0e\x65xternalUserId\x12P\n\nentity_ref\x18\x02 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\"\xdf\x01\n\x18ListNotificationsRequest\x12\x35\n\x10\x65xternal_user_id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0e\x65xternalUserId\x12P\n\nentity_ref\x18\x02 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\x12\x1b\n\tpage_size\x18\x03 \x01(\x05R\x08pageSize\x12\x1d\n\npage_token\x18\x04 \x01(\tR\tpageToken\"\x9d\x01\n\x19ListNotificationsResponse\x12X\n\rnotifications\x18\x01 \x03(\x0b\x32\x32.strmprivacy.api.notifications.v1.UserNotificationR\rnotifications\x12&\n\x0fnext_page_token\x18\x02 \x01(\tR\rnextPageToken2\x9f\x07\n\x14NotificationsService\x12\x9b\x01\n\x16SubscribeNotifications\x12?.strmprivacy.api.notifications.v1.SubscribeNotificationsRequest\x1a@.strmprivacy.api.notifications.v1.SubscribeNotificationsResponse\x12\xa1\x01\n\x18UnSubscribeNotifications\x12\x41.strmprivacy.api.notifications.v1.UnSubscribeNotificationsRequest\x1a\x42.strmprivacy.api.notifications.v1.UnSubscribeNotificationsResponse\x12\x8c\x01\n\x11ListSubscriptions\x12:.strmprivacy.api.notifications.v1.ListSubscriptionsRequest\x1a;.strmprivacy.api.notifications.v1.ListSubscriptionsResponse\x12\x8c\x01\n\x11NotifySubscribers\x12:.strmprivacy.api.notifications.v1.NotifySubscribersRequest\x1a;.strmprivacy.api.notifications.v1.NotifySubscribersResponse\x12\x97\x01\n\x14ReceiveNotifications\x12=.strmprivacy.api.notifications.v1.ReceiveNotificationsRequest\x1a>.strmprivacy.api.notifications.v1.ReceiveNotificationsResponse0\x01\x12\x8c\x01\n\x11ListNotifications\x12:.strmprivacy.api.notifications.v1.ListNotificationsRequest\x1a;.strmprivacy.api.notifications.v1.ListNotificationsResponseBx\n#io.strmprivacy.api.notifications.v1P\x01ZOgithub.com/strmprivacy/api-definitions-go/v2/api/notifications/v1;notificationsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7strmprivacy/api/notifications/v1/notifications_v1.proto\x12 strmprivacy.api.notifications.v1\x1a-strmprivacy/api/entities/v1/entities_v1.proto\x1a\x17validate/validate.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x1d\n\x1bReceiveNotificationsRequest\"v\n\x1cReceiveNotificationsResponse\x12V\n\x0cnotification\x18\x01 \x01(\x0b\x32\x32.strmprivacy.api.notifications.v1.UserNotificationR\x0cnotification\"\xca\x01\n\x18NotifySubscribersRequest\x12P\n\nentity_ref\x18\x01 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\x12\\\n\x0cnotification\x18\x02 \x01(\x0b\x32..strmprivacy.api.notifications.v1.NotificationB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0cnotification\"\x1b\n\x19NotifySubscribersResponse\"\xad\x01\n\x12NotifyUsersRequest\x12\x39\n\x11\x65xternal_user_ids\x18\x01 \x03(\tB\r\xfa\x42\n\x92\x01\x07\"\x05r\x03\xb0\x01\x01R\x0f\x65xternalUserIds\x12\\\n\x0cnotification\x18\x02 \x01(\x0b\x32..strmprivacy.api.notifications.v1.NotificationB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0cnotification\"\x15\n\x13NotifyUsersResponse\"\x83\x02\n\x0cNotification\x12\x45\n\x0b\x63reate_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x00R\ncreateTime\x12@\n\x07\x63omment\x18\x02 \x01(\x0b\x32$.strmprivacy.api.entities.v1.CommentH\x00R\x07\x63omment\x12Z\n\x11\x61udit_trail_entry\x18\x03 \x01(\x0b\x32,.strmprivacy.api.entities.v1.AuditTrailEntryH\x00R\x0f\x61uditTrailEntryB\x0e\n\x0cnotification\"\xa4\x02\n\x10UserNotification\x12\x1b\n\x02id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x02id\x12\\\n\x0cnotification\x18\x02 \x01(\x0b\x32..strmprivacy.api.notifications.v1.NotificationB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x0cnotification\x12\x1f\n\x06reason\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x06reason\x12(\n\x10\x65xternal_user_id\x18\x04 \x01(\tR\x0e\x65xternalUserId\x12J\n\x0email_sent_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x00R\x0cmailSentTime\"\xa8\x01\n\x1dSubscribeNotificationsRequest\x12\x35\n\x10\x65xternal_user_id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0e\x65xternalUserId\x12P\n\nentity_ref\x18\x02 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\" \n\x1eSubscribeNotificationsResponse\"\xaa\x01\n\x1fUnSubscribeNotificationsRequest\x12\x35\n\x10\x65xternal_user_id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0e\x65xternalUserId\x12P\n\nentity_ref\x18\x02 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\"\"\n UnSubscribeNotificationsResponse\"Q\n\x18ListSubscriptionsRequest\x12\x35\n\x10\x65xternal_user_id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0e\x65xternalUserId\"q\n\x19ListSubscriptionsResponse\x12T\n\rsubscriptions\x18\x01 \x03(\x0b\x32..strmprivacy.api.notifications.v1.SubscriptionR\rsubscriptions\"\x97\x01\n\x0cSubscription\x12\x35\n\x10\x65xternal_user_id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0e\x65xternalUserId\x12P\n\nentity_ref\x18\x02 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\tentityRef\"\xa6\x02\n\x18ListNotificationsRequest\x12\x35\n\x10\x65xternal_user_id\x18\x01 \x01(\tB\x0b\xfa\x42\x08r\x06\xd0\x01\x01\xb0\x01\x01R\x0e\x65xternalUserId\x12P\n\nentity_ref\x18\x02 \x01(\x0b\x32\'.strmprivacy.api.entities.v1.GenericRefB\x08\xfa\x42\x05\x8a\x01\x02\x10\x00R\tentityRef\x12\x1b\n\tpage_size\x18\x03 \x01(\x05R\x08pageSize\x12\x1d\n\npage_token\x18\x04 \x01(\tR\tpageToken\x12\x45\n\x0boffset_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x00R\noffsetTime\"\x9d\x01\n\x19ListNotificationsResponse\x12X\n\rnotifications\x18\x01 \x03(\x0b\x32\x32.strmprivacy.api.notifications.v1.UserNotificationR\rnotifications\x12&\n\x0fnext_page_token\x18\x02 \x01(\tR\rnextPageToken2\x9b\x08\n\x14NotificationsService\x12\x9b\x01\n\x16SubscribeNotifications\x12?.strmprivacy.api.notifications.v1.SubscribeNotificationsRequest\x1a@.strmprivacy.api.notifications.v1.SubscribeNotificationsResponse\x12\xa1\x01\n\x18UnSubscribeNotifications\x12\x41.strmprivacy.api.notifications.v1.UnSubscribeNotificationsRequest\x1a\x42.strmprivacy.api.notifications.v1.UnSubscribeNotificationsResponse\x12\x8c\x01\n\x11ListSubscriptions\x12:.strmprivacy.api.notifications.v1.ListSubscriptionsRequest\x1a;.strmprivacy.api.notifications.v1.ListSubscriptionsResponse\x12\x8c\x01\n\x11NotifySubscribers\x12:.strmprivacy.api.notifications.v1.NotifySubscribersRequest\x1a;.strmprivacy.api.notifications.v1.NotifySubscribersResponse\x12z\n\x0bNotifyUsers\x12\x34.strmprivacy.api.notifications.v1.NotifyUsersRequest\x1a\x35.strmprivacy.api.notifications.v1.NotifyUsersResponse\x12\x97\x01\n\x14ReceiveNotifications\x12=.strmprivacy.api.notifications.v1.ReceiveNotificationsRequest\x1a>.strmprivacy.api.notifications.v1.ReceiveNotificationsResponse0\x01\x12\x8c\x01\n\x11ListNotifications\x12:.strmprivacy.api.notifications.v1.ListNotificationsRequest\x1a;.strmprivacy.api.notifications.v1.ListNotificationsResponseBx\n#io.strmprivacy.api.notifications.v1P\x01ZOgithub.com/strmprivacy/api-definitions-go/v2/api/notifications/v1;notificationsb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'strmprivacy.api.notifications.v1.notifications_v1_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n#io.strmprivacy.api.notifications.v1P\001ZOgithub.com/strmprivacy/api-definitions-go/v2/api/notifications/v1;notifications'
   _NOTIFYSUBSCRIBERSREQUEST.fields_by_name['entity_ref']._options = None
   _NOTIFYSUBSCRIBERSREQUEST.fields_by_name['entity_ref']._serialized_options = b'\372B\005\212\001\002\020\001'
   _NOTIFYSUBSCRIBERSREQUEST.fields_by_name['notification']._options = None
   _NOTIFYSUBSCRIBERSREQUEST.fields_by_name['notification']._serialized_options = b'\372B\005\212\001\002\020\001'
+  _NOTIFYUSERSREQUEST.fields_by_name['external_user_ids']._options = None
+  _NOTIFYUSERSREQUEST.fields_by_name['external_user_ids']._serialized_options = b'\372B\n\222\001\007\"\005r\003\260\001\001'
+  _NOTIFYUSERSREQUEST.fields_by_name['notification']._options = None
+  _NOTIFYUSERSREQUEST.fields_by_name['notification']._serialized_options = b'\372B\005\212\001\002\020\001'
   _NOTIFICATION.fields_by_name['create_time']._options = None
   _NOTIFICATION.fields_by_name['create_time']._serialized_options = b'\372B\005\262\001\002\010\000'
   _USERNOTIFICATION.fields_by_name['id']._options = None
   _USERNOTIFICATION.fields_by_name['id']._serialized_options = b'\372B\010r\006\320\001\001\260\001\001'
   _USERNOTIFICATION.fields_by_name['notification']._options = None
   _USERNOTIFICATION.fields_by_name['notification']._serialized_options = b'\372B\005\212\001\002\020\001'
   _USERNOTIFICATION.fields_by_name['reason']._options = None
@@ -51,41 +55,47 @@
   _SUBSCRIPTION.fields_by_name['external_user_id']._options = None
   _SUBSCRIPTION.fields_by_name['external_user_id']._serialized_options = b'\372B\010r\006\320\001\001\260\001\001'
   _SUBSCRIPTION.fields_by_name['entity_ref']._options = None
   _SUBSCRIPTION.fields_by_name['entity_ref']._serialized_options = b'\372B\005\212\001\002\020\001'
   _LISTNOTIFICATIONSREQUEST.fields_by_name['external_user_id']._options = None
   _LISTNOTIFICATIONSREQUEST.fields_by_name['external_user_id']._serialized_options = b'\372B\010r\006\320\001\001\260\001\001'
   _LISTNOTIFICATIONSREQUEST.fields_by_name['entity_ref']._options = None
-  _LISTNOTIFICATIONSREQUEST.fields_by_name['entity_ref']._serialized_options = b'\372B\005\212\001\002\020\001'
+  _LISTNOTIFICATIONSREQUEST.fields_by_name['entity_ref']._serialized_options = b'\372B\005\212\001\002\020\000'
+  _LISTNOTIFICATIONSREQUEST.fields_by_name['offset_time']._options = None
+  _LISTNOTIFICATIONSREQUEST.fields_by_name['offset_time']._serialized_options = b'\372B\005\262\001\002\010\000'
   _RECEIVENOTIFICATIONSREQUEST._serialized_start=198
   _RECEIVENOTIFICATIONSREQUEST._serialized_end=227
   _RECEIVENOTIFICATIONSRESPONSE._serialized_start=229
   _RECEIVENOTIFICATIONSRESPONSE._serialized_end=347
   _NOTIFYSUBSCRIBERSREQUEST._serialized_start=350
   _NOTIFYSUBSCRIBERSREQUEST._serialized_end=552
   _NOTIFYSUBSCRIBERSRESPONSE._serialized_start=554
   _NOTIFYSUBSCRIBERSRESPONSE._serialized_end=581
-  _NOTIFICATION._serialized_start=584
-  _NOTIFICATION._serialized_end=843
-  _USERNOTIFICATION._serialized_start=846
-  _USERNOTIFICATION._serialized_end=1138
-  _SUBSCRIBENOTIFICATIONSREQUEST._serialized_start=1141
-  _SUBSCRIBENOTIFICATIONSREQUEST._serialized_end=1309
-  _SUBSCRIBENOTIFICATIONSRESPONSE._serialized_start=1311
-  _SUBSCRIBENOTIFICATIONSRESPONSE._serialized_end=1343
-  _UNSUBSCRIBENOTIFICATIONSREQUEST._serialized_start=1346
-  _UNSUBSCRIBENOTIFICATIONSREQUEST._serialized_end=1516
-  _UNSUBSCRIBENOTIFICATIONSRESPONSE._serialized_start=1518
-  _UNSUBSCRIBENOTIFICATIONSRESPONSE._serialized_end=1552
-  _LISTSUBSCRIPTIONSREQUEST._serialized_start=1554
-  _LISTSUBSCRIPTIONSREQUEST._serialized_end=1635
-  _LISTSUBSCRIPTIONSRESPONSE._serialized_start=1637
-  _LISTSUBSCRIPTIONSRESPONSE._serialized_end=1750
-  _SUBSCRIPTION._serialized_start=1753
-  _SUBSCRIPTION._serialized_end=1904
-  _LISTNOTIFICATIONSREQUEST._serialized_start=1907
-  _LISTNOTIFICATIONSREQUEST._serialized_end=2130
-  _LISTNOTIFICATIONSRESPONSE._serialized_start=2133
-  _LISTNOTIFICATIONSRESPONSE._serialized_end=2290
-  _NOTIFICATIONSSERVICE._serialized_start=2293
-  _NOTIFICATIONSSERVICE._serialized_end=3220
+  _NOTIFYUSERSREQUEST._serialized_start=584
+  _NOTIFYUSERSREQUEST._serialized_end=757
+  _NOTIFYUSERSRESPONSE._serialized_start=759
+  _NOTIFYUSERSRESPONSE._serialized_end=780
+  _NOTIFICATION._serialized_start=783
+  _NOTIFICATION._serialized_end=1042
+  _USERNOTIFICATION._serialized_start=1045
+  _USERNOTIFICATION._serialized_end=1337
+  _SUBSCRIBENOTIFICATIONSREQUEST._serialized_start=1340
+  _SUBSCRIBENOTIFICATIONSREQUEST._serialized_end=1508
+  _SUBSCRIBENOTIFICATIONSRESPONSE._serialized_start=1510
+  _SUBSCRIBENOTIFICATIONSRESPONSE._serialized_end=1542
+  _UNSUBSCRIBENOTIFICATIONSREQUEST._serialized_start=1545
+  _UNSUBSCRIBENOTIFICATIONSREQUEST._serialized_end=1715
+  _UNSUBSCRIBENOTIFICATIONSRESPONSE._serialized_start=1717
+  _UNSUBSCRIBENOTIFICATIONSRESPONSE._serialized_end=1751
+  _LISTSUBSCRIPTIONSREQUEST._serialized_start=1753
+  _LISTSUBSCRIPTIONSREQUEST._serialized_end=1834
+  _LISTSUBSCRIPTIONSRESPONSE._serialized_start=1836
+  _LISTSUBSCRIPTIONSRESPONSE._serialized_end=1949
+  _SUBSCRIPTION._serialized_start=1952
+  _SUBSCRIPTION._serialized_end=2103
+  _LISTNOTIFICATIONSREQUEST._serialized_start=2106
+  _LISTNOTIFICATIONSREQUEST._serialized_end=2400
+  _LISTNOTIFICATIONSRESPONSE._serialized_start=2403
+  _LISTNOTIFICATIONSRESPONSE._serialized_end=2560
+  _NOTIFICATIONSSERVICE._serialized_start=2563
+  _NOTIFICATIONSSERVICE._serialized_end=3614
 # @@protoc_insertion_point(module_scope)
```

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/notifications/v1/notifications_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/notifications/v1/notifications_v1_pb2_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,19 @@
                 response_deserializer=strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.ListSubscriptionsResponse.FromString,
                 )
         self.NotifySubscribers = channel.unary_unary(
                 '/strmprivacy.api.notifications.v1.NotificationsService/NotifySubscribers',
                 request_serializer=strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.NotifySubscribersRequest.SerializeToString,
                 response_deserializer=strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.NotifySubscribersResponse.FromString,
                 )
+        self.NotifyUsers = channel.unary_unary(
+                '/strmprivacy.api.notifications.v1.NotificationsService/NotifyUsers',
+                request_serializer=strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.NotifyUsersRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.NotifyUsersResponse.FromString,
+                )
         self.ReceiveNotifications = channel.unary_stream(
                 '/strmprivacy.api.notifications.v1.NotificationsService/ReceiveNotifications',
                 request_serializer=strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.ReceiveNotificationsRequest.SerializeToString,
                 response_deserializer=strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.ReceiveNotificationsResponse.FromString,
                 )
         self.ListNotifications = channel.unary_unary(
                 '/strmprivacy.api.notifications.v1.NotificationsService/ListNotifications',
@@ -73,14 +78,21 @@
     def NotifySubscribers(self, request, context):
         """Called by systems (schema-registry for instance) that want to notify subscribed users about something.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def NotifyUsers(self, request, context):
+        """Notify specific users directly, regardless of their subscriptions.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def ReceiveNotifications(self, request, context):
         """Called by the user's browser to receive notifications.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -110,14 +122,19 @@
                     response_serializer=strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.ListSubscriptionsResponse.SerializeToString,
             ),
             'NotifySubscribers': grpc.unary_unary_rpc_method_handler(
                     servicer.NotifySubscribers,
                     request_deserializer=strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.NotifySubscribersRequest.FromString,
                     response_serializer=strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.NotifySubscribersResponse.SerializeToString,
             ),
+            'NotifyUsers': grpc.unary_unary_rpc_method_handler(
+                    servicer.NotifyUsers,
+                    request_deserializer=strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.NotifyUsersRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.NotifyUsersResponse.SerializeToString,
+            ),
             'ReceiveNotifications': grpc.unary_stream_rpc_method_handler(
                     servicer.ReceiveNotifications,
                     request_deserializer=strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.ReceiveNotificationsRequest.FromString,
                     response_serializer=strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.ReceiveNotificationsResponse.SerializeToString,
             ),
             'ListNotifications': grpc.unary_unary_rpc_method_handler(
                     servicer.ListNotifications,
@@ -199,14 +216,31 @@
         return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.notifications.v1.NotificationsService/NotifySubscribers',
             strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.NotifySubscribersRequest.SerializeToString,
             strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.NotifySubscribersResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def NotifyUsers(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.notifications.v1.NotificationsService/NotifyUsers',
+            strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.NotifyUsersRequest.SerializeToString,
+            strmprivacy_dot_api_dot_notifications_dot_v1_dot_notifications__v1__pb2.NotifyUsersResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def ReceiveNotifications(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/organizations/v1/organizations_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/organizations/v1/organizations_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/organizations/v1/organizations_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/organizations/v1/organizations_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/paging/v1/paging_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/paging/v1/paging_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/policies/v1/policies_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/policies/v1/policies_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/policies/v1/policies_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/policies/v1/policies_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/projects/v1/projects_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/projects/v1/projects_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/projects/v1/projects_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/projects/v1/projects_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/schemas/v1/schemas_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/schemas/v1/schemas_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/sinks/v1/sinks_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/sinks/v1/sinks_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/streams/v1/streams_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/streams/v1/streams_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/usage/v1/usage_v1_pb2.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/usage/v1/usage_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.5.0/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/PKG-INFO` & `strmprivacy-api-definitions-3.5.0/strmprivacy_api_definitions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strmprivacy-api-definitions
-Version: 3.4.0
+Version: 3.5.0
 Summary: STRM Privacy API definitions
 Home-page: UNKNOWN
 Author: Stream Machine B.V.
 Author-email: apis@strmprivacy.io
 License: UNKNOWN
 Keywords: strmprivacy api definitions
 Platform: UNKNOWN
```

### Comparing `strmprivacy-api-definitions-3.4.0/strmprivacy_api_definitions.egg-info/SOURCES.txt` & `strmprivacy-api-definitions-3.5.0/strmprivacy_api_definitions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

