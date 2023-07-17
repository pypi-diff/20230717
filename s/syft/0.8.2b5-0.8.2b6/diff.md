# Comparing `tmp/syft-0.8.2b5.tar.gz` & `tmp/syft-0.8.2b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.2b5.tar", last modified: Mon Jul 17 02:54:07 2023, max compression
+gzip compressed data, was "syft-0.8.2b6.tar", last modified: Mon Jul 17 15:39:19 2023, max compression
```

## Comparing `syft-0.8.2b5.tar` & `syft-0.8.2b6.tar`

### file list

```diff
@@ -1,213 +1,214 @@
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.227497 syft-0.8.2b5/
--rw-r--r--   0 om        (1001) users      (100)    11843 2023-07-17 02:52:43.000000 syft-0.8.2b5/LICENSE
--rw-r--r--   0 om        (1001) users      (100)       98 2023-07-17 02:52:43.000000 syft-0.8.2b5/MANIFEST.in
--rw-r--r--   0 om        (1001) users      (100)    16852 2023-07-17 02:54:07.227497 syft-0.8.2b5/PKG-INFO
--rw-r--r--   0 om        (1001) users      (100)    16170 2023-07-17 02:52:43.000000 syft-0.8.2b5/README.md
--rw-r--r--   0 om        (1001) users      (100)      272 2023-07-17 02:52:43.000000 syft-0.8.2b5/pyproject.toml
--rw-r--r--   0 om        (1001) users      (100)     3210 2023-07-17 02:54:07.227497 syft-0.8.2b5/setup.cfg
--rw-r--r--   0 om        (1001) users      (100)      107 2023-07-17 02:52:43.000000 syft-0.8.2b5/setup.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.211497 syft-0.8.2b5/src/
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.211497 syft-0.8.2b5/src/syft/
--rw-r--r--   0 om        (1001) users      (100)      580 2023-07-17 02:52:46.000000 syft-0.8.2b5/src/syft/VERSION
--rw-r--r--   0 om        (1001) users      (100)     5626 2023-07-17 02:52:46.000000 syft-0.8.2b5/src/syft/__init__.py
--rw-r--r--   0 om        (1001) users      (100)       93 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/__main__.py
--rw-r--r--   0 om        (1001) users      (100)      654 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/abstract_node.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.215497 syft-0.8.2b5/src/syft/capnp/
--rw-r--r--   0 om        (1001) users      (100)      270 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/capnp/__init__.py
--rw-r--r--   0 om        (1001) users      (100)       75 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/capnp/iterable.capnp
--rw-r--r--   0 om        (1001) users      (100)      102 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 om        (1001) users      (100)      186 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.215497 syft-0.8.2b5/src/syft/client/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    25732 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/api.py
--rw-r--r--   0 om        (1001) users      (100)    28112 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/client.py
--rw-r--r--   0 om        (1001) users      (100)      568 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/connection.py
--rw-r--r--   0 om        (1001) users      (100)      650 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/deploy.py
--rw-r--r--   0 om        (1001) users      (100)     8798 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/domain_client.py
--rw-r--r--   0 om        (1001) users      (100)     4434 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/enclave_client.py
--rw-r--r--   0 om        (1001) users      (100)     2372 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/gateway_client.py
--rw-r--r--   0 om        (1001) users      (100)    15257 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/registry.py
--rw-r--r--   0 om        (1001) users      (100)     2623 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/search.py
--rw-r--r--   0 om        (1001) users      (100)      549 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/user_settings.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.215497 syft-0.8.2b5/src/syft/external/
--rw-r--r--   0 om        (1001) users      (100)     1735 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/__init__.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.215497 syft-0.8.2b5/src/syft/external/oblv/
--rw-r--r--   0 om        (1001) users      (100)      860 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      284 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/auth.py
--rw-r--r--   0 om        (1001) users      (100)      212 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/constants.py
--rw-r--r--   0 om        (1001) users      (100)     4835 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/deployment.py
--rw-r--r--   0 om        (1001) users      (100)    12380 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 om        (1001) users      (100)     1800 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 om        (1001) users      (100)      489 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 om        (1001) users      (100)     2280 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 om        (1001) users      (100)     7462 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 om        (1001) users      (100)    13948 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 om        (1001) users      (100)     1146 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/gevent_patch.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.215497 syft-0.8.2b5/src/syft/img/
--rw-r--r--   0 om        (1001) users      (100)      297 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/img/base64.py
--rw-r--r--   0 om        (1001) users      (100)    25535 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/img/logo.png
--rw-r--r--   0 om        (1001) users      (100)    41764 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/img/small-grid-symbol-logo.png
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.215497 syft-0.8.2b5/src/syft/node/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     2631 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/credentials.py
--rw-r--r--   0 om        (1001) users      (100)      152 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/domain.py
--rw-r--r--   0 om        (1001) users      (100)      259 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/enclave.py
--rw-r--r--   0 om        (1001) users      (100)      728 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/gateway.py
--rw-r--r--   0 om        (1001) users      (100)    32225 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/node.py
--rw-r--r--   0 om        (1001) users      (100)     6960 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/routes.py
--rw-r--r--   0 om        (1001) users      (100)     2064 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/run.py
--rw-r--r--   0 om        (1001) users      (100)     6992 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/server.py
--rw-r--r--   0 om        (1001) users      (100)      127 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/worker.py
--rw-r--r--   0 om        (1001) users      (100)     1100 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/worker_settings.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.219498 syft-0.8.2b5/src/syft/serde/
--rw-r--r--   0 om        (1001) users      (100)      159 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     3597 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/array.py
--rw-r--r--   0 om        (1001) users      (100)     4099 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/arrow.py
--rw-r--r--   0 om        (1001) users      (100)      298 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/capnp.py
--rw-r--r--   0 om        (1001) users      (100)      722 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/deserialize.py
--rw-r--r--   0 om        (1001) users      (100)     1230 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/lib_permissions.py
--rw-r--r--   0 om        (1001) users      (100)    11663 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 om        (1001) users      (100)      875 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/mock.py
--rw-r--r--   0 om        (1001) users      (100)    11639 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/recursive.py
--rw-r--r--   0 om        (1001) users      (100)    10253 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 om        (1001) users      (100)     1822 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/serializable.py
--rw-r--r--   0 om        (1001) users      (100)      369 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/serialize.py
--rw-r--r--   0 om        (1001) users      (100)     4959 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/signature.py
--rw-r--r--   0 om        (1001) users      (100)     4885 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/third_party.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.219498 syft-0.8.2b5/src/syft/service/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/__init__.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.219498 syft-0.8.2b5/src/syft/service/action/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      703 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 om        (1001) users      (100)    16706 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/action_graph.py
--rw-r--r--   0 om        (1001) users      (100)     6874 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 om        (1001) users      (100)    48803 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/action_object.py
--rw-r--r--   0 om        (1001) users      (100)     2502 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/action_permissions.py
--rw-r--r--   0 om        (1001) users      (100)    26998 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/action_service.py
--rw-r--r--   0 om        (1001) users      (100)    10264 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/action_store.py
--rw-r--r--   0 om        (1001) users      (100)     1165 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/action_types.py
--rw-r--r--   0 om        (1001) users      (100)     3889 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/numpy.py
--rw-r--r--   0 om        (1001) users      (100)     2233 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/pandas.py
--rw-r--r--   0 om        (1001) users      (100)     2920 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/plan.py
--rw-r--r--   0 om        (1001) users      (100)     4951 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/verification.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.219498 syft-0.8.2b5/src/syft/service/code/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/code/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      236 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/code/code_parse.py
--rw-r--r--   0 om        (1001) users      (100)      102 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/code/unparse.py
--rw-r--r--   0 om        (1001) users      (100)    27413 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/code/user_code.py
--rw-r--r--   0 om        (1001) users      (100)     1756 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 om        (1001) users      (100)    10340 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/code/user_code_service.py
--rw-r--r--   0 om        (1001) users      (100)     1446 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 om        (1001) users      (100)     1782 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/context.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.219498 syft-0.8.2b5/src/syft/service/data_subject/
--rw-r--r--   0 om        (1001) users      (100)       69 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     4076 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 om        (1001) users      (100)      870 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 om        (1001) users      (100)     3215 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 om        (1001) users      (100)     5006 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/dataset/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/dataset/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    23590 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/dataset/dataset.py
--rw-r--r--   0 om        (1001) users      (100)     6382 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 om        (1001) users      (100)     1911 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/enclave/
--rw-r--r--   0 om        (1001) users      (100)     6038 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/enclave/enclave_service.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/metadata/
--rw-r--r--   0 om        (1001) users      (100)     1170 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/metadata/metadata_service.py
--rw-r--r--   0 om        (1001) users      (100)     3678 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/network/
--rw-r--r--   0 om        (1001) users      (100)    18148 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/network/network_service.py
--rw-r--r--   0 om        (1001) users      (100)     3100 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/network/node_peer.py
--rw-r--r--   0 om        (1001) users      (100)     4593 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/network/routes.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/notification/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/notification/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     7961 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/notification/notification_service.py
--rw-r--r--   0 om        (1001) users      (100)     4566 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/notification/notification_stash.py
--rw-r--r--   0 om        (1001) users      (100)     3259 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/notification/notifications.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/policy/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/policy/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    22437 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/policy/policy.py
--rw-r--r--   0 om        (1001) users      (100)     2081 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/policy/policy_service.py
--rw-r--r--   0 om        (1001) users      (100)     1077 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/project/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/project/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    48433 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/project/project.py
--rw-r--r--   0 om        (1001) users      (100)    15374 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/project/project_service.py
--rw-r--r--   0 om        (1001) users      (100)     1908 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/queue/
--rw-r--r--   0 om        (1001) users      (100)     2044 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/queue/base_queue.py
--rw-r--r--   0 om        (1001) users      (100)     3008 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/queue/queue.py
--rw-r--r--   0 om        (1001) users      (100)     4845 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 om        (1001) users      (100)     7929 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/request/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/request/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    27212 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/request/request.py
--rw-r--r--   0 om        (1001) users      (100)    10112 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/request/request_service.py
--rw-r--r--   0 om        (1001) users      (100)     1410 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/request/request_stash.py
--rw-r--r--   0 om        (1001) users      (100)     2850 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/response.py
--rw-r--r--   0 om        (1001) users      (100)    13653 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/service.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/settings/
--rw-r--r--   0 om        (1001) users      (100)      985 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/settings/settings.py
--rw-r--r--   0 om        (1001) users      (100)     3486 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/settings/settings_service.py
--rw-r--r--   0 om        (1001) users      (100)     1711 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/user/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/user/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      201 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/user/roles.py
--rw-r--r--   0 om        (1001) users      (100)     6115 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/user/user.py
--rw-r--r--   0 om        (1001) users      (100)     3427 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/user/user_roles.py
--rw-r--r--   0 om        (1001) users      (100)    16847 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/user/user_service.py
--rw-r--r--   0 om        (1001) users      (100)     4510 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/vpn/
--rw-r--r--   0 om        (1001) users      (100)     1809 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/vpn/headscale_client.py
--rw-r--r--   0 om        (1001) users      (100)     6789 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/vpn/tailscale_client.py
--rw-r--r--   0 om        (1001) users      (100)     5414 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/vpn/vpn.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.227497 syft-0.8.2b5/src/syft/store/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     3235 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/dict_document_store.py
--rw-r--r--   0 om        (1001) users      (100)    22993 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/document_store.py
--rw-r--r--   0 om        (1001) users      (100)    22010 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/kv_document_store.py
--rw-r--r--   0 om        (1001) users      (100)     4326 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/linked_obj.py
--rw-r--r--   0 om        (1001) users      (100)    11840 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/locks.py
--rw-r--r--   0 om        (1001) users      (100)     8768 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/mongo_client.py
--rw-r--r--   0 om        (1001) users      (100)      846 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/mongo_codecs.py
--rw-r--r--   0 om        (1001) users      (100)    13836 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/mongo_document_store.py
--rw-r--r--   0 om        (1001) users      (100)    13136 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.227497 syft-0.8.2b5/src/syft/types/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      136 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/base.py
--rw-r--r--   0 om        (1001) users      (100)     1091 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/datetime.py
--rw-r--r--   0 om        (1001) users      (100)     5167 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/grid_url.py
--rw-r--r--   0 om        (1001) users      (100)     4807 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/syft_metaclass.py
--rw-r--r--   0 om        (1001) users      (100)    25848 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/syft_object.py
--rw-r--r--   0 om        (1001) users      (100)     8113 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/transforms.py
--rw-r--r--   0 om        (1001) users      (100)     2098 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/twin_object.py
--rw-r--r--   0 om        (1001) users      (100)     8038 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/uid.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.227497 syft-0.8.2b5/src/syft/util/
--rw-r--r--   0 om        (1001) users      (100)       67 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      852 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/autoreload.py
--rw-r--r--   0 om        (1001) users      (100)      271 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/colors.py
--rw-r--r--   0 om        (1001) users      (100)       34 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/constants.py
--rw-r--r--   0 om        (1001) users      (100)     1514 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/decorators.py
--rw-r--r--   0 om        (1001) users      (100)      445 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/env.py
--rw-r--r--   0 om        (1001) users      (100)     1607 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/experimental_flags.py
--rw-r--r--   0 om        (1001) users      (100)     1327 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/filterwarnings.py
--rw-r--r--   0 om        (1001) users      (100)     2940 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/fonts.py
--rw-r--r--   0 om        (1001) users      (100)      153 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/jax_settings.py
--rw-r--r--   0 om        (1001) users      (100)     3779 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/logger.py
--rw-r--r--   0 om        (1001) users      (100)      752 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/markdown.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.227497 syft-0.8.2b5/src/syft/util/notebook_ui/
--rw-r--r--   0 om        (1001) users      (100)    27090 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/notebook_ui/notebook_addons.py
--rw-r--r--   0 om        (1001) users      (100)       42 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/options.py
--rw-r--r--   0 om        (1001) users      (100)     5297 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/schema.py
--rw-r--r--   0 om        (1001) users      (100)     2771 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/telemetry.py
--rw-r--r--   0 om        (1001) users      (100)     6728 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/trace_decorator.py
--rw-r--r--   0 om        (1001) users      (100)    22738 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/util.py
--rw-r--r--   0 om        (1001) users      (100)     3123 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/version_compare.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.215497 syft-0.8.2b5/src/syft.egg-info/
--rw-r--r--   0 om        (1001) users      (100)    16852 2023-07-17 02:54:07.000000 syft-0.8.2b5/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 om        (1001) users      (100)     5946 2023-07-17 02:54:07.000000 syft-0.8.2b5/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 om        (1001) users      (100)        1 2023-07-17 02:54:07.000000 syft-0.8.2b5/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 om        (1001) users      (100)       43 2023-07-17 02:54:07.000000 syft-0.8.2b5/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 om        (1001) users      (100)        1 2023-07-17 02:54:07.000000 syft-0.8.2b5/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 om        (1001) users      (100)     1555 2023-07-17 02:54:07.000000 syft-0.8.2b5/src/syft.egg-info/requires.txt
--rw-r--r--   0 om        (1001) users      (100)        5 2023-07-17 02:54:07.000000 syft-0.8.2b5/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.509721 syft-0.8.2b6/
+-rw-r--r--   0 om        (1001) users      (100)    11843 2023-07-17 15:37:23.000000 syft-0.8.2b6/LICENSE
+-rw-r--r--   0 om        (1001) users      (100)       98 2023-07-17 15:37:23.000000 syft-0.8.2b6/MANIFEST.in
+-rw-r--r--   0 om        (1001) users      (100)    16852 2023-07-17 15:39:19.509721 syft-0.8.2b6/PKG-INFO
+-rw-r--r--   0 om        (1001) users      (100)    16170 2023-07-17 15:37:23.000000 syft-0.8.2b6/README.md
+-rw-r--r--   0 om        (1001) users      (100)      272 2023-07-17 15:37:23.000000 syft-0.8.2b6/pyproject.toml
+-rw-r--r--   0 om        (1001) users      (100)     3210 2023-07-17 15:39:19.513721 syft-0.8.2b6/setup.cfg
+-rw-r--r--   0 om        (1001) users      (100)      107 2023-07-17 15:37:23.000000 syft-0.8.2b6/setup.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.493721 syft-0.8.2b6/src/
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.493721 syft-0.8.2b6/src/syft/
+-rw-r--r--   0 om        (1001) users      (100)      580 2023-07-17 15:37:26.000000 syft-0.8.2b6/src/syft/VERSION
+-rw-r--r--   0 om        (1001) users      (100)     5750 2023-07-17 15:37:26.000000 syft-0.8.2b6/src/syft/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)       93 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/__main__.py
+-rw-r--r--   0 om        (1001) users      (100)      790 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/abstract_node.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.497721 syft-0.8.2b6/src/syft/capnp/
+-rw-r--r--   0 om        (1001) users      (100)      270 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/capnp/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)       75 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 om        (1001) users      (100)      102 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 om        (1001) users      (100)      186 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.497721 syft-0.8.2b6/src/syft/client/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    26545 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/api.py
+-rw-r--r--   0 om        (1001) users      (100)    28762 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/client.py
+-rw-r--r--   0 om        (1001) users      (100)      568 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/connection.py
+-rw-r--r--   0 om        (1001) users      (100)      650 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/deploy.py
+-rw-r--r--   0 om        (1001) users      (100)     9211 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/domain_client.py
+-rw-r--r--   0 om        (1001) users      (100)     6924 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/enclave_client.py
+-rw-r--r--   0 om        (1001) users      (100)     6404 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/gateway_client.py
+-rw-r--r--   0 om        (1001) users      (100)    15257 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/registry.py
+-rw-r--r--   0 om        (1001) users      (100)     2623 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/search.py
+-rw-r--r--   0 om        (1001) users      (100)      549 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/client/user_settings.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.497721 syft-0.8.2b6/src/syft/external/
+-rw-r--r--   0 om        (1001) users      (100)     1735 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/__init__.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.497721 syft-0.8.2b6/src/syft/external/oblv/
+-rw-r--r--   0 om        (1001) users      (100)      860 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      284 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/auth.py
+-rw-r--r--   0 om        (1001) users      (100)      212 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/constants.py
+-rw-r--r--   0 om        (1001) users      (100)     4835 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 om        (1001) users      (100)    12380 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 om        (1001) users      (100)     1800 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 om        (1001) users      (100)      489 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 om        (1001) users      (100)     2280 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     7462 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 om        (1001) users      (100)    13948 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1146 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/gevent_patch.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.497721 syft-0.8.2b6/src/syft/img/
+-rw-r--r--   0 om        (1001) users      (100)      297 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/img/base64.py
+-rw-r--r--   0 om        (1001) users      (100)    25535 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/img/logo.png
+-rw-r--r--   0 om        (1001) users      (100)    41764 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/img/small-grid-symbol-logo.png
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.497721 syft-0.8.2b6/src/syft/node/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     2631 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/credentials.py
+-rw-r--r--   0 om        (1001) users      (100)      152 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/domain.py
+-rw-r--r--   0 om        (1001) users      (100)      259 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/enclave.py
+-rw-r--r--   0 om        (1001) users      (100)      819 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/gateway.py
+-rw-r--r--   0 om        (1001) users      (100)    33437 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/node.py
+-rw-r--r--   0 om        (1001) users      (100)     6960 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/routes.py
+-rw-r--r--   0 om        (1001) users      (100)     2064 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/run.py
+-rw-r--r--   0 om        (1001) users      (100)     7737 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/server.py
+-rw-r--r--   0 om        (1001) users      (100)      127 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/worker.py
+-rw-r--r--   0 om        (1001) users      (100)     1228 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/node/worker_settings.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.501721 syft-0.8.2b6/src/syft/serde/
+-rw-r--r--   0 om        (1001) users      (100)      159 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     3597 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/array.py
+-rw-r--r--   0 om        (1001) users      (100)     4099 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/arrow.py
+-rw-r--r--   0 om        (1001) users      (100)      298 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/capnp.py
+-rw-r--r--   0 om        (1001) users      (100)      722 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/deserialize.py
+-rw-r--r--   0 om        (1001) users      (100)     1230 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 om        (1001) users      (100)    11663 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 om        (1001) users      (100)      875 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/mock.py
+-rw-r--r--   0 om        (1001) users      (100)    11639 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/recursive.py
+-rw-r--r--   0 om        (1001) users      (100)    10253 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 om        (1001) users      (100)     1822 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/serializable.py
+-rw-r--r--   0 om        (1001) users      (100)      369 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/serialize.py
+-rw-r--r--   0 om        (1001) users      (100)     4959 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/signature.py
+-rw-r--r--   0 om        (1001) users      (100)     4885 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/serde/third_party.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.501721 syft-0.8.2b6/src/syft/service/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/__init__.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.501721 syft-0.8.2b6/src/syft/service/action/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      703 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 om        (1001) users      (100)    16706 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/action_graph.py
+-rw-r--r--   0 om        (1001) users      (100)     6874 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 om        (1001) users      (100)    48803 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/action_object.py
+-rw-r--r--   0 om        (1001) users      (100)     2502 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 om        (1001) users      (100)    27128 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/action_service.py
+-rw-r--r--   0 om        (1001) users      (100)    10264 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/action_store.py
+-rw-r--r--   0 om        (1001) users      (100)     1165 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/action_types.py
+-rw-r--r--   0 om        (1001) users      (100)     3889 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/numpy.py
+-rw-r--r--   0 om        (1001) users      (100)     2233 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/pandas.py
+-rw-r--r--   0 om        (1001) users      (100)     2920 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/plan.py
+-rw-r--r--   0 om        (1001) users      (100)     4951 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/action/verification.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.501721 syft-0.8.2b6/src/syft/service/code/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/code/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      236 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/code/code_parse.py
+-rw-r--r--   0 om        (1001) users      (100)      102 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/code/unparse.py
+-rw-r--r--   0 om        (1001) users      (100)    27413 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/code/user_code.py
+-rw-r--r--   0 om        (1001) users      (100)     1756 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 om        (1001) users      (100)    10340 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1446 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     1782 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/context.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.501721 syft-0.8.2b6/src/syft/service/data_subject/
+-rw-r--r--   0 om        (1001) users      (100)       69 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     4076 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 om        (1001) users      (100)      870 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 om        (1001) users      (100)     3215 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 om        (1001) users      (100)     5006 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/dataset/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    23590 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 om        (1001) users      (100)     6603 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1911 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/enclave/
+-rw-r--r--   0 om        (1001) users      (100)     6038 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/enclave/enclave_service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/metadata/
+-rw-r--r--   0 om        (1001) users      (100)     1170 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/metadata/metadata_service.py
+-rw-r--r--   0 om        (1001) users      (100)     3774 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/network/
+-rw-r--r--   0 om        (1001) users      (100)    18260 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/network/network_service.py
+-rw-r--r--   0 om        (1001) users      (100)     3100 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/network/node_peer.py
+-rw-r--r--   0 om        (1001) users      (100)     4657 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/network/routes.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/notification/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/notification/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     7961 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/notification/notification_service.py
+-rw-r--r--   0 om        (1001) users      (100)     4566 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/notification/notification_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     3259 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/notification/notifications.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/policy/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/policy/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    22437 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/policy/policy.py
+-rw-r--r--   0 om        (1001) users      (100)     2081 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1077 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/project/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/project/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    48433 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/project/project.py
+-rw-r--r--   0 om        (1001) users      (100)    15374 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/project/project_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1908 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/queue/
+-rw-r--r--   0 om        (1001) users      (100)     2044 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 om        (1001) users      (100)     3008 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/queue/queue.py
+-rw-r--r--   0 om        (1001) users      (100)     4845 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     7929 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/request/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/request/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    28165 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/request/request.py
+-rw-r--r--   0 om        (1001) users      (100)    10135 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/request/request_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1410 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/request/request_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     3100 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/response.py
+-rw-r--r--   0 om        (1001) users      (100)    13815 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/settings/
+-rw-r--r--   0 om        (1001) users      (100)     1109 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/settings/settings.py
+-rw-r--r--   0 om        (1001) users      (100)     3608 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1711 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/user/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/user/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      201 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/user/roles.py
+-rw-r--r--   0 om        (1001) users      (100)     6115 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/user/user.py
+-rw-r--r--   0 om        (1001) users      (100)     3427 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/user/user_roles.py
+-rw-r--r--   0 om        (1001) users      (100)    16878 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/user/user_service.py
+-rw-r--r--   0 om        (1001) users      (100)     4510 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.505721 syft-0.8.2b6/src/syft/service/vpn/
+-rw-r--r--   0 om        (1001) users      (100)     1809 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/vpn/headscale_client.py
+-rw-r--r--   0 om        (1001) users      (100)     6789 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/vpn/tailscale_client.py
+-rw-r--r--   0 om        (1001) users      (100)     5414 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/vpn/vpn.py
+-rw-r--r--   0 om        (1001) users      (100)     5171 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/service/warnings.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.509721 syft-0.8.2b6/src/syft/store/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     3235 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/dict_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    22993 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    22010 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/kv_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)     4326 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/linked_obj.py
+-rw-r--r--   0 om        (1001) users      (100)    11840 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/locks.py
+-rw-r--r--   0 om        (1001) users      (100)     8768 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/mongo_client.py
+-rw-r--r--   0 om        (1001) users      (100)      846 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 om        (1001) users      (100)    13836 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    13136 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.509721 syft-0.8.2b6/src/syft/types/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      136 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/base.py
+-rw-r--r--   0 om        (1001) users      (100)     1091 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/datetime.py
+-rw-r--r--   0 om        (1001) users      (100)     5167 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/grid_url.py
+-rw-r--r--   0 om        (1001) users      (100)     4807 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 om        (1001) users      (100)    25848 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/syft_object.py
+-rw-r--r--   0 om        (1001) users      (100)     8113 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/transforms.py
+-rw-r--r--   0 om        (1001) users      (100)     2098 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/twin_object.py
+-rw-r--r--   0 om        (1001) users      (100)     8038 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/types/uid.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.509721 syft-0.8.2b6/src/syft/util/
+-rw-r--r--   0 om        (1001) users      (100)       67 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      852 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/autoreload.py
+-rw-r--r--   0 om        (1001) users      (100)      271 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/colors.py
+-rw-r--r--   0 om        (1001) users      (100)       34 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/constants.py
+-rw-r--r--   0 om        (1001) users      (100)     1514 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/decorators.py
+-rw-r--r--   0 om        (1001) users      (100)      445 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/env.py
+-rw-r--r--   0 om        (1001) users      (100)     1607 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/experimental_flags.py
+-rw-r--r--   0 om        (1001) users      (100)     1327 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/filterwarnings.py
+-rw-r--r--   0 om        (1001) users      (100)     2940 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/fonts.py
+-rw-r--r--   0 om        (1001) users      (100)      153 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/jax_settings.py
+-rw-r--r--   0 om        (1001) users      (100)     3779 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/logger.py
+-rw-r--r--   0 om        (1001) users      (100)      752 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/markdown.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.509721 syft-0.8.2b6/src/syft/util/notebook_ui/
+-rw-r--r--   0 om        (1001) users      (100)    27090 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/notebook_ui/notebook_addons.py
+-rw-r--r--   0 om        (1001) users      (100)       42 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/options.py
+-rw-r--r--   0 om        (1001) users      (100)     5297 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/schema.py
+-rw-r--r--   0 om        (1001) users      (100)     2771 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/telemetry.py
+-rw-r--r--   0 om        (1001) users      (100)     6728 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/trace_decorator.py
+-rw-r--r--   0 om        (1001) users      (100)    23185 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/util.py
+-rw-r--r--   0 om        (1001) users      (100)     3123 2023-07-17 15:37:23.000000 syft-0.8.2b6/src/syft/util/version_compare.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 15:39:19.497721 syft-0.8.2b6/src/syft.egg-info/
+-rw-r--r--   0 om        (1001) users      (100)    16852 2023-07-17 15:39:19.000000 syft-0.8.2b6/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 om        (1001) users      (100)     5975 2023-07-17 15:39:19.000000 syft-0.8.2b6/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 om        (1001) users      (100)        1 2023-07-17 15:39:19.000000 syft-0.8.2b6/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 om        (1001) users      (100)       43 2023-07-17 15:39:19.000000 syft-0.8.2b6/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 om        (1001) users      (100)        1 2023-07-17 15:39:19.000000 syft-0.8.2b6/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 om        (1001) users      (100)     1555 2023-07-17 15:39:19.000000 syft-0.8.2b6/src/syft.egg-info/requires.txt
+-rw-r--r--   0 om        (1001) users      (100)        5 2023-07-17 15:39:19.000000 syft-0.8.2b6/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.2b5/LICENSE` & `syft-0.8.2b6/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/PKG-INFO` & `syft-0.8.2b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.2b5
+Version: 0.8.2b6
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.2b5 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.2b6 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: telemetry
```

### Comparing `syft-0.8.2b5/README.md` & `syft-0.8.2b6/README.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/setup.cfg` & `syft-0.8.2b6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.2-beta.5"
+version = attr: "0.8.2-beta.6"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
@@ -39,15 +39,15 @@
 	pycapnp==1.3.0
 	pydantic[email]==1.10.7
 	pymongo==4.3.3
 	pynacl==1.5.0
 	pyzmq>=23.2.1,<=25.1.0
 	redis==4.5.5
 	requests==2.31.0
-	RestrictedPython==6.0
+	RestrictedPython==6.1
 	result==0.10.0
 	tqdm==4.65.0
 	typeguard==2.13.3
 	typing_extensions==4.6.3
 	sherlock[redis,filelock]==0.4.1
 	uvicorn[standard]==0.22.0
 	fastapi==0.97.0
```

### Comparing `syft-0.8.2b5/src/syft/VERSION` & `syft-0.8.2b6/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.2-beta.5"
+__version__ = "0.8.2-beta.6"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.2b5/src/syft/__init__.py` & `syft-0.8.2b6/src/syft/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.2-beta.5"
+__version__ = "0.8.2-beta.6"
 
 # stdlib
 import pathlib
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
@@ -10,14 +10,16 @@
 # relative
 from . import gevent_patch  # noqa: F401
 from .abstract_node import NodeType  # noqa: F401
 from .client.client import connect  # noqa: F401
 from .client.client import login  # noqa: F401
 from .client.client import register  # noqa: F401
 from .client.deploy import Orchestra  # noqa: F401
+from .client.domain_client import DomainClient  # noqa: F401
+from .client.gateway_client import GatewayClient  # noqa: F401
 from .client.registry import DomainRegistry  # noqa: F401
 from .client.registry import EnclaveRegistry  # noqa: F401
 from .client.registry import NetworkRegistry  # noqa: F401
 from .client.search import Search  # noqa: F401
 from .client.search import SearchResults  # noqa: F401
 from .client.user_settings import UserSettings  # noqa: F401
 from .client.user_settings import settings  # noqa: F401
```

### Comparing `syft-0.8.2b5/src/syft/abstract_node.py` & `syft-0.8.2b6/src/syft/abstract_node.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,21 @@
     GATEWAY = "gateway"
 
     def __str__(self) -> str:
         # Use values when transforming NodeType to str
         return self.value
 
 
+@serializable()
+class NodeSideType(str, Enum):
+    LOW_SIDE = "low"
+    HIGH_SIDE = "high"
+
+
 class AbstractNode:
     id: Optional[UID]
     name: Optional[str]
     node_type: Optional[NodeType]
+    node_side_type: Optional[NodeSideType]
 
     def get_service(self, path_or_func: Union[str, Callable]) -> Callable:
         raise NotImplementedError
```

### Comparing `syft-0.8.2b5/src/syft/client/api.py` & `syft-0.8.2b6/src/syft/client/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 from ..service.context import AuthedServiceContext
 from ..service.context import ChangeContext
 from ..service.response import SyftAttributeError
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
 from ..service.service import UserLibConfigRegistry
 from ..service.service import UserServiceConfigRegistry
+from ..service.warnings import APIEndpointWarning
+from ..service.warnings import WarningContext
 from ..types.syft_object import SYFT_OBJECT_VERSION_1
 from ..types.syft_object import SyftBaseObject
 from ..types.syft_object import SyftObject
 from ..types.uid import LineageID
 from ..types.uid import UID
 from ..util.autoreload import autoreload_enabled
 from ..util.telemetry import instrument
@@ -85,23 +87,28 @@
         for key, api in reversed(cls.__api_registry__.items()):
             if key[0] == node_uid:
                 return api
         return None
 
 
 @serializable()
-class APIEndpoint(SyftBaseObject):
+class APIEndpoint(SyftObject):
+    __canonical_name__ = "APIEndpoint"
+    __version__ = SYFT_OBJECT_VERSION_1
+
+    id: UID
     service_path: str
     module_path: str
     name: str
     description: str
     doc_string: Optional[str]
     signature: Signature
     has_self: bool = False
     pre_kwargs: Optional[Dict[str, Any]]
+    warning: Optional[APIEndpointWarning]
 
 
 @serializable()
 class LibEndpoint(SyftBaseObject):
     # TODO: bad name, change
     service_path: str
     module_path: str
@@ -194,14 +201,15 @@
 
 def generate_remote_function(
     node_uid: UID,
     signature: Signature,
     path: str,
     make_call: Callable,
     pre_kwargs: Dict[str, Any],
+    warning: Optional[APIEndpointWarning],
 ):
     if "blocking" in signature.parameters:
         raise Exception(
             f"Signature {signature} can't have 'blocking' kwarg because its reserved"
         )
 
     def wrapper(*args, **kwargs):
@@ -222,14 +230,18 @@
         api_call = SyftAPICall(
             node_uid=node_uid,
             path=path,
             args=_valid_args,
             kwargs=_valid_kwargs,
             blocking=blocking,
         )
+
+        allowed = warning.show() if warning else True
+        if not allowed:
+            return
         result = make_call(api_call=api_call)
         return result
 
     wrapper.__ipython_inspector_signature_override__ = signature
     return wrapper
 
 
@@ -396,28 +408,36 @@
         # find user role by verify_key
         # TODO: we should probably not allow empty verify keys but instead make user always register
         role = node.get_role_for_credentials(user_verify_key)
         _user_service_config_registry = UserServiceConfigRegistry.from_role(role)
         _user_lib_config_registry = UserLibConfigRegistry.from_user(user_verify_key)
         endpoints: Dict[str, APIEndpoint] = {}
         lib_endpoints: Dict[str, LibEndpoint] = {}
+        warning_context = WarningContext(
+            node=node, role=role, credentials=user_verify_key
+        )
 
         for (
             path,
             service_config,
         ) in _user_service_config_registry.get_registered_configs().items():
             if not service_config.is_from_lib:
+                service_warning = service_config.warning
+                if service_warning:
+                    service_warning = service_warning.message_from(warning_context)
+                    service_warning.enabled = node.enable_warnings
                 endpoint = APIEndpoint(
                     service_path=path,
                     module_path=path,
                     name=service_config.public_name,
                     description="",
                     doc_string=service_config.doc_string,
                     signature=service_config.signature,
                     has_self=False,
+                    warning=service_warning,
                 )
                 endpoints[path] = endpoint
 
         for (
             path,
             lib_config,
         ) in _user_lib_config_registry.get_registered_configs().items():
@@ -516,14 +536,15 @@
                 if isinstance(v, APIEndpoint):
                     endpoint_function = generate_remote_function(
                         self.node_uid,
                         signature,
                         v.service_path,
                         self.make_call,
                         pre_kwargs=v.pre_kwargs,
+                        warning=v.warning,
                     )
                 elif isinstance(v, LibEndpoint):
                     endpoint_function = generate_remote_lib_function(
                         self,
                         self.node_uid,
                         signature,
                         v.service_path,
```

### Comparing `syft-0.8.2b5/src/syft/client/client.py` & `syft-0.8.2b6/src/syft/client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from typing_extensions import Self
 
 # relative
 from .. import __version__
 from ..abstract_node import AbstractNode
+from ..abstract_node import NodeSideType
 from ..abstract_node import NodeType
 from ..node.credentials import SyftSigningKey
 from ..node.credentials import SyftVerifyKey
 from ..node.credentials import UserLoginCredentials
 from ..serde.deserialize import _deserialize
 from ..serde.serializable import serializable
 from ..serde.serialize import _serialize
@@ -45,14 +46,15 @@
 from ..service.user.user_roles import ServiceRole
 from ..service.user.user_service import UserService
 from ..types.grid_url import GridURL
 from ..types.syft_object import SYFT_OBJECT_VERSION_1
 from ..types.uid import UID
 from ..util.logger import debug
 from ..util.telemetry import instrument
+from ..util.util import prompt_warning_message
 from ..util.util import thread_ident
 from ..util.util import verify_tls
 from .api import APIModule
 from .api import APIRegistry
 from .api import SignedSyftAPICall
 from .api import SyftAPI
 from .api import SyftAPICall
@@ -394,17 +396,14 @@
     def __repr__(self) -> str:
         return f"{type(self).__name__}"
 
     def __str__(self) -> str:
         return f"{type(self).__name__}"
 
     def get_client_type(self) -> Type[SyftClient]:
-        # TODO: Rasswanth, should remove passing in credentials
-        # when metadata are proxy forwarded in the grid routes
-        # in the gateway fixes PR
         # relative
         from .domain_client import DomainClient
         from .enclave_client import EnclaveClient
         from .gateway_client import GatewayClient
 
         metadata = self.get_node_metadata(credentials=SyftSigningKey.generate())
         if metadata.node_type == NodeType.DOMAIN.value:
@@ -584,15 +583,18 @@
             self.__user_role = user_private_key.role
         if signing_key is not None:
             self.credentials = signing_key
             self.__logged_in_user = email
             # TODO: How to get the role of the user?
             # self.__user_role =
             self._fetch_api(self.credentials)
-            print(f"Logged into {self.name} as <{email}>")
+            print(
+                f"Logged into <{self.name}: {self.metadata.node_side_type.capitalize()} side "
+                f"{self.metadata.node_type.capitalize()}> as <{email}>"
+            )
             if cache:
                 SyftClientSessionCache.add_client(
                     email=email,
                     password=password,
                     connection=self.connection,
                     syft_client=self,
                 )
@@ -639,14 +641,26 @@
                 password_verify=password,
                 institution=institution,
                 website=website,
                 created_by=self.credentials,
             )
         except Exception as e:
             return SyftError(message=str(e))
+
+        if self.metadata.node_side_type == NodeSideType.HIGH_SIDE.value:
+            message = (
+                "You're registering a user to a high side "
+                f"{self.metadata.node_type}, which could "
+                "host datasets with private information."
+            )
+            if self.metadata.show_warnings and not prompt_warning_message(
+                message=message
+            ):
+                return
+
         response = self.connection.register(new_user=new_user)
         if isinstance(response, tuple):
             response = response[0]
         return response
 
     def __getattr__(self, name):
         if (
@@ -764,15 +778,18 @@
 
     login_credentials = None
     if email and password:
         login_credentials = UserLoginCredentials(email=email, password=password)
 
     if login_credentials is None:
         if verbose:
-            print(f"Logged into {_client.name} as GUEST")
+            print(
+                f"Logged into <{_client.name}: {_client.metadata.node_side_type.capitalize()}-"
+                f"side {_client.metadata.node_type.capitalize()}> as GUEST"
+            )
         return _client.guest()
 
     if cache and login_credentials:
         _client_cache = SyftClientSessionCache.get_client(
             login_credentials.email,
             login_credentials.password,
             connection=connection,
```

### Comparing `syft-0.8.2b5/src/syft/client/connection.py` & `syft-0.8.2b6/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/client/deploy.py` & `syft-0.8.2b6/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/client/domain_client.py` & `syft-0.8.2b6/src/syft/client/domain_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import TYPE_CHECKING
 from typing import Union
 
 # third party
 from tqdm import tqdm
 
 # relative
+from ..abstract_node import NodeSideType
 from ..img.base64 import base64read
 from ..serde.serializable import serializable
 from ..service.dataset.dataset import Contributor
 from ..service.dataset.dataset import CreateAsset
 from ..service.dataset.dataset import CreateDataset
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
@@ -209,14 +210,29 @@
         <ul style='padding-left: 1em;'>
             {commands}
         </ul>
         """
 
         small_grid_symbol_logo = base64read("small-grid-symbol-logo.png")
 
+        url = getattr(self.connection, "url", None)
+        node_details = f"<strong>URL:</strong> {url}<br />" if url else ""
+        node_details += (
+            f"<strong>Node Type:</strong> {self.metadata.node_type.capitalize()}<br />"
+        )
+        node_side_type = (
+            "Low Side"
+            if self.metadata.node_side_type == NodeSideType.LOW_SIDE.value
+            else "High Side"
+        )
+        node_details += f"<strong>Node Side Type:</strong> {node_side_type}<br />"
+        node_details += (
+            f"<strong>Syft Version:</strong> {self.metadata.syft_version}<br />"
+        )
+
         return f"""
         <style>
             {fonts_css}
 
             .syft-container {{
                 padding: 5px;
                 font-family: 'Open Sans';
@@ -238,18 +254,15 @@
             }}
         </style>
         <div class="syft-client syft-container">
             <img src="{small_grid_symbol_logo}" alt="Logo"
             style="width:48px;height:48px;padding:3px;">
             <h2>Welcome to {self.name}</h2>
             <div class="syft-space">
-                <!-- <strong>Institution:</strong> TODO<br /> -->
-                <!-- <strong>Owner:</strong> TODO<br /> -->
-                <strong>URL:</strong> {getattr(self.connection, 'url', '')}<br />
-                <!-- <strong>PyGrid Admin:</strong> TODO<br /> -->
+                {node_details}
             </div>
             <div class='syft-alert-info syft-space'>
                 &#9432;&nbsp;
                 This domain is run by the library PySyft to learn more about how it works visit
                 <a href="https://github.com/OpenMined/PySyft">github.com/OpenMined/PySyft</a>.
             </div>
             <h4>Commands to Get Started</h4>
```

### Comparing `syft-0.8.2b5/src/syft/client/gateway_client.py` & `syft-0.8.2b6/src/syft/service/network/node_peer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,91 @@
 # stdlib
-from typing import Any
 from typing import List
 from typing import Optional
-from typing import Union
 
 # third party
 from typing_extensions import Self
 
 # relative
-from ..abstract_node import NodeType
-from ..node.credentials import SyftSigningKey
-from ..serde.serializable import serializable
-from ..service.network.node_peer import NodePeer
-from ..service.response import SyftError
-from ..service.response import SyftException
-from .client import SyftClient
+from ...abstract_node import NodeType
+from ...client.client import SyftClient
+from ...node.credentials import SyftSigningKey
+from ...node.credentials import SyftVerifyKey
+from ...serde.serializable import serializable
+from ...service.response import SyftError
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import SyftObject
+from ...types.uid import UID
+from ..context import NodeServiceContext
+from ..metadata.node_metadata import NodeMetadata
+from .routes import NodeRoute
+from .routes import NodeRouteType
+from .routes import connection_to_route
+from .routes import route_to_connection
 
 
 @serializable()
-class GatewayClient(SyftClient):
-    # TODO: add widget repr for gateway client
+class NodePeer(SyftObject):
+    # version
+    __canonical_name__ = "NodePeer"
+    __version__ = SYFT_OBJECT_VERSION_1
+
+    __attr_searchable__ = ["name", "node_type"]
+    __attr_unique__ = ["verify_key"]
+    __repr_attrs__ = ["name", "node_type", "admin_email"]
+
+    id: Optional[UID]
+    name: str
+    verify_key: SyftVerifyKey
+    is_vpn: bool = False
+    vpn_auth_key: Optional[str] = None
+    node_routes: List[NodeRouteType] = []
+    node_type: NodeType
+    admin_email: str
+
+    def update_routes(self, new_routes: List[NodeRoute]) -> None:
+        add_routes = []
+        existing_routes = set(self.node_routes)
+        for new_route in new_routes:
+            if new_route not in existing_routes:
+                add_routes.append(new_route)
+        self.node_routes += add_routes
+
+    @staticmethod
+    def from_client(client: SyftClient) -> Self:
+        if not client.metadata:
+            raise Exception("Client has have metadata first")
+
+        peer = client.metadata.to(NodeMetadata).to(NodePeer)
+        route = connection_to_route(client.connection)
+        peer.node_routes.append(route)
+        return peer
+
+    def client_with_context(self, context: NodeServiceContext) -> SyftClient:
+        if len(self.node_routes) < 1:
+            raise Exception(f"No routes to peer: {self}")
+        route = self.node_routes[0]
+        connection = route_to_connection(route=route)
+
+        client_type = connection.get_client_type()
+        if isinstance(client_type, SyftError):
+            return client_type
+        return client_type(connection=connection, credentials=context.node.signing_key)
+
+    def client_with_key(self, credentials: SyftSigningKey) -> SyftClient:
+        if len(self.node_routes) < 1:
+            raise Exception(f"No routes to peer: {self}")
+        route = self.node_routes[0]
+        connection = route_to_connection(route=route)
+        client_type = connection.get_client_type()
+        if isinstance(client_type, SyftError):
+            return client_type
 
-    def proxy_to(self, peer: Any) -> Self:
-        # relative
-        from .domain_client import DomainClient
-        from .enclave_client import EnclaveClient
-
-        connection = self.connection.with_proxy(peer.id)
-        metadata = connection.get_node_metadata(credentials=SyftSigningKey.generate())
-        if metadata.node_type == NodeType.DOMAIN.value:
-            client_type = DomainClient
-        elif metadata.node_type == NodeType.ENCLAVE.value:
-            client_type = EnclaveClient
-        else:
-            raise SyftException(
-                f"Unknown node type {metadata.node_type} to create proxy client"
-            )
-
-        client = client_type(
-            connection=connection,
-            credentials=self.credentials,
-        )
-        return client
-
-    def proxy_client_for(
-        self,
-        name: str,
-        email: Optional[str] = None,
-        password: Optional[str] = None,
-        **kwargs,
-    ):
-        peer = None
-        if self.api.has_service("network"):
-            peer = self.api.services.network.get_peer_by_name(name=name)
-        if peer is None:
-            return SyftError(message=f"No domain with name {name}")
-        res = self.proxy_to(peer)
-        if email and password:
-            res.login(email=email, password=password, **kwargs)
-        return res
+        return client_type(connection=connection, credentials=credentials)
 
     @property
-    def domains(self) -> Optional[Union[List[NodePeer], SyftError]]:
-        if not self.api.has_service("network"):
-            return None
-        return self.api.services.network.get_peers_by_type(node_type=NodeType.DOMAIN)
+    def guest_client(self) -> SyftClient:
+        guest_key = SyftSigningKey.generate()
+        return self.client_with_key(credentials=guest_key)
 
-    @property
-    def enclaves(self) -> Optional[Union[List[NodePeer], SyftError]]:
-        if not self.api.has_service("network"):
-            return None
-        return self.api.services.network.get_peers_by_type(node_type=NodeType.ENCLAVE)
+    def proxy_from(self, client: SyftClient) -> SyftClient:
+        return client.proxy_to(self)
```

### Comparing `syft-0.8.2b5/src/syft/client/registry.py` & `syft-0.8.2b6/src/syft/client/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/client/search.py` & `syft-0.8.2b6/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/client/user_settings.py` & `syft-0.8.2b6/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/external/__init__.py` & `syft-0.8.2b6/src/syft/external/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/external/oblv/__init__.py` & `syft-0.8.2b6/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/external/oblv/deployment.py` & `syft-0.8.2b6/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/external/oblv/deployment_client.py` & `syft-0.8.2b6/src/syft/external/oblv/deployment_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/external/oblv/exceptions.py` & `syft-0.8.2b6/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.2b6/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.2b6/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/external/oblv/oblv_service.py` & `syft-0.8.2b6/src/syft/external/oblv/oblv_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/gevent_patch.py` & `syft-0.8.2b6/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/img/logo.png` & `syft-0.8.2b6/src/syft/img/logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/img/small-grid-symbol-logo.png` & `syft-0.8.2b6/src/syft/img/small-grid-symbol-logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/node/credentials.py` & `syft-0.8.2b6/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/node/gateway.py` & `syft-0.8.2b6/src/syft/node/gateway.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 
 
 @serializable()
 class Gateway(Node):
     def post_init(self) -> None:
         self.node_type = NodeType.GATEWAY
         super().post_init()
-        self.connect_to_vpn_self()
+        try:
+            self.connect_to_vpn_self()
+        except Exception as e:
+            print("Error connecting to VPN: ", e)
 
     def connect_to_vpn_self(self) -> None:
         network_service = self.get_service(NetworkService)
         context = AuthedServiceContext(
             node=self, credentials=self.signing_key.verify_key
         )
-        result = network_service.connect_self(context=context)
-        print("Message: ", result.message)
+        network_service.connect_self(context=context)
+        # print("Message: ", result.message)
```

### Comparing `syft-0.8.2b5/src/syft/node/node.py` & `syft-0.8.2b6/src/syft/node/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from result import Err
 from result import Result
 from typing_extensions import Self
 
 # relative
 from .. import __version__
 from ..abstract_node import AbstractNode
+from ..abstract_node import NodeSideType
 from ..abstract_node import NodeType
 from ..client.api import SignedSyftAPICall
 from ..client.api import SyftAPI
 from ..client.api import SyftAPICall
 from ..client.api import SyftAPIData
 from ..client.api import debox_signed_syftapicall_response
 from ..external import OBLV
@@ -108,14 +109,15 @@
     return _deserialize(obj_bytes, from_bytes=True)
 
 
 NODE_PRIVATE_KEY = "NODE_PRIVATE_KEY"
 NODE_UID = "NODE_UID"
 NODE_TYPE = "NODE_TYPE"
 NODE_NAME = "NODE_NAME"
+NODE_SIDE_TYPE = "NODE_SIDE_TYPE"
 
 DEFAULT_ROOT_EMAIL = "DEFAULT_ROOT_EMAIL"
 DEFAULT_ROOT_PASSWORD = "DEFAULT_ROOT_PASSWORD"  # nosec
 
 
 def get_env(key: str, default: Optional[Any] = None) -> Optional[str]:
     return os.environ.get(key, default)
@@ -129,14 +131,18 @@
     return get_env(NODE_TYPE, "domain")
 
 
 def get_node_name() -> Optional[str]:
     return get_env(NODE_NAME, None)
 
 
+def get_node_side_type() -> str:
+    return get_env(NODE_SIDE_TYPE, "high")
+
+
 def get_node_uid_env() -> Optional[str]:
     return get_env(NODE_UID)
 
 
 def get_default_root_email() -> Optional[str]:
     return get_env(DEFAULT_ROOT_EMAIL, "info@openmined.org")
 
@@ -145,14 +151,18 @@
     return get_env(DEFAULT_ROOT_PASSWORD, "changethis")  # nosec
 
 
 def get_dev_mode() -> bool:
     return str_to_bool(get_env("DEV_MODE", "False"))
 
 
+def get_enable_warnings() -> bool:
+    return str_to_bool(get_env("ENABLE_WARNINGS", "False"))
+
+
 def get_venv_packages() -> str:
     res = subprocess.getoutput(
         "pip list --format=freeze",
     )
     return res
 
 
@@ -184,14 +194,16 @@
         root_password: str = default_root_password,
         processes: int = 0,
         is_subprocess: bool = False,
         node_type: Union[str, NodeType] = NodeType.DOMAIN,
         local_db: bool = False,
         sqlite_path: Optional[str] = None,
         queue_config: QueueConfig = ZMQQueueConfig,
+        node_side_type: Union[str, NodeSideType] = NodeSideType.HIGH_SIDE,
+        enable_warnings: bool = False,
     ):
         # 🟡 TODO 22: change our ENV variable format and default init args to make this
         # less horrible or add some convenience functions
         if node_uid_env is not None:
             self.id = UID.from_string(node_uid_env)
         else:
             if id is None:
@@ -245,14 +257,16 @@
         if OBLV:
             # relative
             from ..external.oblv.oblv_service import OblvService
 
             services += [OblvService]
             create_oblv_key_pair(worker=self)
 
+        self.enable_warnings = enable_warnings
+
         self.services = services
         self._construct_services()
 
         create_admin_new(  # nosec B106
             name="Jane Doe",
             email=root_email,
             password=root_password,
@@ -260,14 +274,18 @@
         )
 
         self.client_cache = {}
         if isinstance(node_type, str):
             node_type = NodeType(node_type)
         self.node_type = node_type
 
+        if isinstance(node_side_type, str):
+            node_side_type = NodeSideType(node_side_type)
+        self.node_side_type = node_side_type
+
         self.post_init()
         self.create_initial_settings(admin_email=root_email)
         if not (self.is_subprocess or self.processes == 0):
             self.init_queue_manager(queue_config=queue_config)
 
         NodeRegistry.set_node_for(self.id, self)
 
@@ -291,14 +309,16 @@
         *,  # Trasterisk
         name: str,
         processes: int = 0,
         reset: bool = False,
         local_db: bool = False,
         sqlite_path: Optional[str] = None,
         node_type: Union[str, NodeType] = NodeType.DOMAIN,
+        node_side_type: Union[str, NodeSideType] = NodeSideType.HIGH_SIDE,
+        enable_warnings: bool = False,
     ) -> Self:
         name_hash = hashlib.sha256(name.encode("utf8")).digest()
         name_hash_uuid = name_hash[0:16]
         name_hash_uuid = bytearray(name_hash_uuid)
         name_hash_uuid[6] = (
             name_hash_uuid[6] & 0x0F
         ) | 0x40  # Set version to 4 (uuid4)
@@ -335,14 +355,16 @@
             name=name,
             id=uid,
             signing_key=key,
             processes=processes,
             local_db=local_db,
             sqlite_path=sqlite_path,
             node_type=node_type,
+            node_side_type=node_side_type,
+            enable_warnings=enable_warnings,
         )
 
     def is_root(self, credentials: SyftVerifyKey) -> bool:
         return credentials == self.verify_key
 
     @property
     def root_client(self):
@@ -361,15 +383,18 @@
 
     def get_guest_client(self, verbose: bool = True):
         # relative
         from ..client.client import PythonConnection
 
         connection = PythonConnection(node=self)
         if verbose:
-            print(f"Logged into {self.name} as GUEST")
+            print(
+                f"Logged into <{self.name}: {self.node_side_type.value.capitalize()} "
+                f"side {self.node_type.value.capitalize()} > as GUEST"
+            )
 
         client_type = connection.get_client_type()
         if isinstance(client_type, SyftError):
             return client_type
 
         return client_type(connection=connection, credentials=SyftSigningKey.generate())
 
@@ -518,26 +543,28 @@
         name = ""
         deployed_on = ""
         organization = ""
         on_board = False
         description = ""
         signup_enabled = False
         admin_email = ""
+        show_warnings = self.enable_warnings
 
         settings_stash = SettingsStash(store=self.document_store)
         settings = settings_stash.get_all(self.signing_key.verify_key)
         if settings.is_ok() and len(settings.ok()) > 0:
             settings_data = settings.ok()[0]
             name = settings_data.name
             deployed_on = settings_data.deployed_on
             organization = settings_data.organization
             on_board = settings_data.on_board
             description = settings_data.description
             signup_enabled = settings_data.signup_enabled
             admin_email = settings_data.admin_email
+            show_warnings = settings_data.show_warnings
 
         return NodeMetadata(
             name=name,
             id=self.id,
             verify_key=self.verify_key,
             highest_object_version=HIGHEST_SYFT_OBJECT_VERSION,
             lowest_object_version=LOWEST_SYFT_OBJECT_VERSION,
@@ -545,14 +572,16 @@
             deployed_on=deployed_on,
             description=description,
             organization=organization,
             on_board=on_board,
             node_type=self.node_type.value,
             signup_enabled=signup_enabled,
             admin_email=admin_email,
+            node_side_type=self.node_side_type.value,
+            show_warnings=show_warnings,
         )
 
     @property
     def icon(self) -> str:
         return "🦾"
 
     @property
@@ -738,14 +767,16 @@
                 if self.node_type == NodeType.ENCLAVE:
                     flags.CAN_REGISTER = True
                 new_settings = NodeSettings(
                     name=self.name,
                     deployed_on=datetime.now().date().strftime("%m/%d/%Y"),
                     signup_enabled=flags.CAN_REGISTER,
                     admin_email=admin_email,
+                    node_side_type=self.node_side_type.value,
+                    show_warnings=self.enable_warnings,
                 )
                 result = settings_stash.set(
                     credentials=self.signing_key.verify_key, settings=new_settings
                 )
                 if result.is_ok():
                     return result.ok()
                 return None
```

### Comparing `syft-0.8.2b5/src/syft/node/routes.py` & `syft-0.8.2b6/src/syft/node/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/node/run.py` & `syft-0.8.2b6/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/node/server.py` & `syft-0.8.2b6/src/syft/node/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from fastapi import APIRouter
 from fastapi import FastAPI
 import requests
 from starlette.middleware.cors import CORSMiddleware
 import uvicorn
 
 # relative
+from ..abstract_node import NodeSideType
 from ..client.client import API_PATH
 from ..util.constants import DEFAULT_TIMEOUT
 from ..util.util import os_name
 from .domain import Domain
 from .enclave import Enclave
 from .gateway import Gateway
 from .node import NodeType
@@ -62,18 +63,31 @@
     NodeType.DOMAIN: Domain,
     NodeType.GATEWAY: Gateway,
     NodeType.ENCLAVE: Enclave,
 }
 
 
 def run_uvicorn(
-    name: str, node_type: Enum, host: str, port: int, reset: bool, dev_mode: bool
+    name: str,
+    node_type: Enum,
+    host: str,
+    port: int,
+    reset: bool,
+    dev_mode: bool,
+    node_side_type: str,
+    enable_warnings: bool,
 ):
     async def _run_uvicorn(
-        name: str, node_type: Enum, host: str, port: int, reset: bool, dev_mode: bool
+        name: str,
+        node_type: Enum,
+        host: str,
+        port: int,
+        reset: bool,
+        dev_mode: bool,
+        node_side_type: Enum,
     ):
         if node_type not in worker_classes:
             raise NotImplementedError(f"node_type: {node_type} is not supported")
         worker_class = worker_classes[node_type]
         if dev_mode:
             print(
                 f"\nWARNING: private key is based on node name: {name} in dev_mode. "
@@ -82,21 +96,25 @@
 
             worker = worker_class.named(
                 name=name,
                 processes=0,
                 reset=reset,
                 local_db=True,
                 node_type=node_type,
+                node_side_type=node_side_type,
+                enable_warnings=enable_warnings,
             )
         else:
             worker = worker_class(
                 name=name,
                 processes=0,
                 local_db=True,
                 node_type=node_type,
+                node_side_type=node_side_type,
+                enable_warnings=enable_warnings,
             )
         router = make_routes(worker=worker)
         app = make_app(worker.name, router=router)
 
         if reset:
             try:
                 python_pids = find_python_processes_on_port(port)
@@ -118,29 +136,51 @@
         server = uvicorn.Server(config)
 
         await server.serve()
         asyncio.get_running_loop().stop()
 
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
-    loop.run_until_complete(_run_uvicorn(name, node_type, host, port, reset, dev_mode))
+    loop.run_until_complete(
+        _run_uvicorn(
+            name,
+            node_type,
+            host,
+            port,
+            reset,
+            dev_mode,
+            node_side_type,
+        )
+    )
     loop.close()
 
 
 def serve_node(
     name: str,
     node_type: NodeType = NodeType.DOMAIN,
+    node_side_type: NodeSideType = NodeSideType.HIGH_SIDE,
     host: str = "0.0.0.0",  # nosec
     port: int = 8080,
     reset: bool = False,
     dev_mode: bool = False,
     tail: bool = False,
+    enable_warnings: bool = False,
 ) -> Tuple[Callable, Callable]:
     server_process = multiprocessing.Process(
-        target=run_uvicorn, args=(name, node_type, host, port, reset, dev_mode)
+        target=run_uvicorn,
+        args=(
+            name,
+            node_type,
+            host,
+            port,
+            reset,
+            dev_mode,
+            node_side_type,
+            enable_warnings,
+        ),
     )
 
     def stop():
         print(f"Stopping {name}")
         server_process.terminate()
         server_process.join()
```

### Comparing `syft-0.8.2b5/src/syft/node/worker_settings.py` & `syft-0.8.2b6/src/syft/node/worker_settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 # third party
 from typing_extensions import Self
 
 # relative
 from ..abstract_node import AbstractNode
+from ..abstract_node import NodeSideType
 from ..abstract_node import NodeType
 from ..node.credentials import SyftSigningKey
 from ..serde.serializable import serializable
 from ..store.document_store import StoreConfig
 from ..types.syft_object import SYFT_OBJECT_VERSION_1
 from ..types.syft_object import SyftObject
 from ..types.uid import UID
@@ -19,21 +20,23 @@
 class WorkerSettings(SyftObject):
     __canonical_name__ = "WorkerSettings"
     __version__ = SYFT_OBJECT_VERSION_1
 
     id: UID
     name: str
     node_type: NodeType
+    node_side_type: NodeSideType
     signing_key: SyftSigningKey
     document_store_config: StoreConfig
     action_store_config: StoreConfig
 
     @staticmethod
     def from_node(node: AbstractNode) -> Self:
         return WorkerSettings(
             id=node.id,
             name=node.name,
             node_type=node.node_type,
             signing_key=node.signing_key,
             document_store_config=node.document_store_config,
             action_store_config=node.action_store_config,
+            node_side_type=node.node_side_type.value,
         )
```

### Comparing `syft-0.8.2b5/src/syft/serde/array.py` & `syft-0.8.2b6/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/serde/arrow.py` & `syft-0.8.2b6/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/serde/deserialize.py` & `syft-0.8.2b6/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/serde/lib_permissions.py` & `syft-0.8.2b6/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/serde/lib_service_registry.py` & `syft-0.8.2b6/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/serde/mock.py` & `syft-0.8.2b6/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/serde/recursive.py` & `syft-0.8.2b6/src/syft/serde/recursive.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/serde/recursive_primitives.py` & `syft-0.8.2b6/src/syft/serde/recursive_primitives.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/serde/serializable.py` & `syft-0.8.2b6/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/serde/signature.py` & `syft-0.8.2b6/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/serde/third_party.py` & `syft-0.8.2b6/src/syft/serde/third_party.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/action/action_data_empty.py` & `syft-0.8.2b6/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/action/action_graph.py` & `syft-0.8.2b6/src/syft/service/action/action_graph.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/action/action_graph_service.py` & `syft-0.8.2b6/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/action/action_object.py` & `syft-0.8.2b6/src/syft/service/action/action_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/action/action_permissions.py` & `syft-0.8.2b6/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/action/action_service.py` & `syft-0.8.2b6/src/syft/service/action/action_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import UserLibConfigRegistry
 from ..service import service_method
 from ..user.user_roles import GUEST_ROLE_LEVEL
+from ..warnings import HighSideCRUDWarning
 from .action_object import Action
 from .action_object import ActionObject
 from .action_object import ActionObjectPointer
 from .action_object import ActionType
 from .action_object import AnyActionObject
 from .action_object import TwinMode
 from .action_permissions import ActionObjectREAD
@@ -51,15 +52,20 @@
             data = np.array(data)
         np_obj = NumpyArrayObject(
             syft_action_data=data, dtype=data.dtype, shape=data.shape
         )
         np_pointer = self.set(context, np_obj)
         return np_pointer
 
-    @service_method(path="action.set", name="set", roles=GUEST_ROLE_LEVEL)
+    @service_method(
+        path="action.set",
+        name="set",
+        roles=GUEST_ROLE_LEVEL,
+        warning=HighSideCRUDWarning(confirmation=True),
+    )
     def set(
         self,
         context: AuthedServiceContext,
         action_object: Union[ActionObject, TwinObject],
     ) -> Result[ActionObject, str]:
         """Save an object to the action store"""
         # 🟡 TODO 9: Create some kind of type checking / protocol for SyftSerializable
```

### Comparing `syft-0.8.2b5/src/syft/service/action/action_store.py` & `syft-0.8.2b6/src/syft/service/action/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/action/action_types.py` & `syft-0.8.2b6/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/action/numpy.py` & `syft-0.8.2b6/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/action/pandas.py` & `syft-0.8.2b6/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/action/plan.py` & `syft-0.8.2b6/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/action/verification.py` & `syft-0.8.2b6/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/code/user_code.py` & `syft-0.8.2b6/src/syft/service/code/user_code.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/code/user_code_parse.py` & `syft-0.8.2b6/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/code/user_code_service.py` & `syft-0.8.2b6/src/syft/service/code/user_code_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/code/user_code_stash.py` & `syft-0.8.2b6/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/context.py` & `syft-0.8.2b6/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/data_subject/data_subject.py` & `syft-0.8.2b6/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.2b6/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.2b6/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.2b6/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/dataset/dataset.py` & `syft-0.8.2b6/src/syft/service/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/dataset/dataset_service.py` & `syft-0.8.2b6/src/syft/service/dataset/dataset_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
 from ..user.user_roles import DATA_OWNER_ROLE_LEVEL
 from ..user.user_roles import DATA_SCIENTIST_ROLE_LEVEL
 from ..user.user_roles import GUEST_ROLE_LEVEL
+from ..warnings import CRUDReminder
+from ..warnings import HighSideCRUDWarning
 from .dataset import Asset
 from .dataset import CreateDataset
 from .dataset import Dataset
 from .dataset import DatasetPageView
 from .dataset_stash import DatasetStash
 
 
@@ -55,15 +57,20 @@
         if result.is_err():
             return SyftError(message=str(result.err()))
         return SyftSuccess(
             message=f"Dataset uploaded to '{context.node.name}'. "
             f"To see the datasets uploaded by a client on this node, use command `[your_client].datasets`"
         )
 
-    @service_method(path="dataset.get_all", name="get_all", roles=GUEST_ROLE_LEVEL)
+    @service_method(
+        path="dataset.get_all",
+        name="get_all",
+        roles=GUEST_ROLE_LEVEL,
+        warning=CRUDReminder(),
+    )
     def get_all(
         self,
         context: AuthedServiceContext,
         page_size: Optional[int] = 0,
         page_index: Optional[int] = 0,
     ) -> Union[DatasetPageView, List[Dataset], SyftError]:
         """Get a Dataset"""
@@ -159,15 +166,19 @@
                     if asset.action_id == uid:
                         assets.append(asset)
             return assets
         elif isinstance(datasets, SyftError):
             return datasets
         return []
 
-    @service_method(path="dataset.delete_by_id", name="dataset_delete_by_id")
+    @service_method(
+        path="dataset.delete_by_id",
+        name="dataset_delete_by_id",
+        warning=HighSideCRUDWarning(confirmation=True),
+    )
     def delete_dataset(self, context: AuthedServiceContext, uid: UID):
         result = self.stash.delete_by_uid(context.credentials, uid)
         if result.is_ok():
             return result.ok()
         else:
             return SyftError(message=result.err())
```

### Comparing `syft-0.8.2b5/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.2b6/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/enclave/enclave_service.py` & `syft-0.8.2b6/src/syft/service/enclave/enclave_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/metadata/metadata_service.py` & `syft-0.8.2b6/src/syft/service/metadata/metadata_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/metadata/node_metadata.py` & `syft-0.8.2b6/src/syft/service/metadata/node_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,14 +73,16 @@
     node_type: NodeType = NodeType.DOMAIN
     deployed_on: str = "Date"
     organization: str = "OpenMined"
     on_board: bool = False
     description: str = "Text"
     signup_enabled: bool
     admin_email: str
+    node_side_type: str
+    show_warnings: bool
 
     def check_version(self, client_version: str) -> bool:
         return check_version(
             client_version=client_version,
             server_version=self.syft_version,
             server_name=self.name,
         )
@@ -98,14 +100,16 @@
     node_type: str = NodeType.DOMAIN.value
     deployed_on: str = "Date"
     organization: str = "OpenMined"
     on_board: bool = False
     description: str = "My cool domain"
     signup_enabled: bool
     admin_email: str
+    node_side_type: str
+    show_warnings: bool
 
     def check_version(self, client_version: str) -> bool:
         return check_version(
             client_version=client_version,
             server_version=self.syft_version,
             server_name=self.name,
         )
```

### Comparing `syft-0.8.2b5/src/syft/service/network/network_service.py` & `syft-0.8.2b6/src/syft/service/network/network_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,21 +40,23 @@
 from ..user.user_roles import GUEST_ROLE_LEVEL
 from ..vpn.headscale_client import HeadscaleAuthToken
 from ..vpn.headscale_client import HeadscaleClient
 from ..vpn.tailscale_client import TailscaleClient
 from ..vpn.tailscale_client import TailscaleState
 from ..vpn.tailscale_client import TailscaleStatus
 from ..vpn.tailscale_client import get_vpn_client
+from ..warnings import CRUDWarning
 from .node_peer import NodePeer
 from .routes import HTTPNodeRoute
 from .routes import NodeRoute
 from .routes import PythonNodeRoute
 
 VerifyKeyPartitionKey = PartitionKey(key="verify_key", type_=SyftVerifyKey)
 NodeTypePartitionKey = PartitionKey(key="node_type", type_=NodeType)
+OrderByNamePartitionKey = PartitionKey(key="name", type_=str)
 
 
 @instrument
 @serializable()
 class NetworkStash(BaseUIDStoreStash):
     object_type = NodePeer
     settings: PartitionSettings = PartitionSettings(
@@ -100,15 +102,17 @@
         qks = QueryKeys(qks=[VerifyKeyPartitionKey.with_obj(verify_key)])
         return self.query_one(credentials, qks)
 
     def get_by_node_type(
         self, credentials: SyftVerifyKey, node_type: NodeType
     ) -> Result[List[NodePeer], SyftError]:
         qks = QueryKeys(qks=[NodeTypePartitionKey.with_obj(node_type)])
-        return self.query_all(credentials=credentials, qks=qks)
+        return self.query_all(
+            credentials=credentials, qks=qks, order_by=OrderByNamePartitionKey
+        )
 
 
 @instrument
 @serializable()
 class NetworkService(AbstractService):
     store: DocumentStore
     stash: NetworkStash
@@ -119,14 +123,15 @@
 
     # TODO: Check with MADHAVA, can we even allow guest user to introduce routes to
     # domain nodes?
     @service_method(
         path="network.exchange_credentials_with",
         name="exchange_credentials_with",
         roles=GUEST_ROLE_LEVEL,
+        warning=CRUDWarning(confirmation=True),
     )
     def exchange_credentials_with(
         self,
         context: AuthedServiceContext,
         self_node_route: NodeRoute,
         remote_node_route: NodeRoute,
         remote_node_verify_key: SyftVerifyKey,
@@ -278,15 +283,18 @@
     @service_method(
         path="network.get_all_peers", name="get_all_peers", roles=GUEST_ROLE_LEVEL
     )
     def get_all_peers(
         self, context: AuthedServiceContext
     ) -> Union[List[NodePeer], SyftError]:
         """Get all Peers"""
-        result = self.stash.get_all(credentials=context.node.verify_key)
+        result = self.stash.get_all(
+            credentials=context.node.verify_key,
+            order_by=OrderByNamePartitionKey,
+        )
         if result.is_ok():
             peers = result.ok()
             return peers
         return SyftError(message=result.err())
 
     @service_method(
         path="network.get_peer_by_name", name="get_peer_by_name", roles=GUEST_ROLE_LEVEL
@@ -341,19 +349,14 @@
         result = self.stash.get_by_uid(
             credentials=context.node.verify_key, uid=remote_peer.id
         )
 
         if result.is_err():
             return SyftError(message=f"{result.err()}")
 
-        if result.ok() is not None:
-            return SyftError(
-                message=f"Already connected to VPN Peer: {remote_peer.name}"
-            )
-
         # tell the remote peer our details
         if not context.node:
             return SyftError(message=f"{type(context)} has no node")
 
         # switch to the nodes signing key
         client = remote_peer.client_with_context(context=context)
```

### Comparing `syft-0.8.2b5/src/syft/service/network/routes.py` & `syft-0.8.2b6/src/syft/service/network/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         # relative
         from ...node.worker import Worker
 
         node = Worker(
             id=self.worker_settings.id,
             name=self.worker_settings.name,
             node_type=self.worker_settings.node_type,
+            node_side_type=self.worker_settings.node_side_type,
             signing_key=self.worker_settings.signing_key,
             document_store_config=self.worker_settings.document_store_config,
             action_store_config=self.worker_settings.action_store_config,
             processes=1,
         )
         return node
```

### Comparing `syft-0.8.2b5/src/syft/service/notification/notification_service.py` & `syft-0.8.2b6/src/syft/service/notification/notification_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/notification/notification_stash.py` & `syft-0.8.2b6/src/syft/service/notification/notification_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/notification/notifications.py` & `syft-0.8.2b6/src/syft/service/notification/notifications.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/policy/policy.py` & `syft-0.8.2b6/src/syft/service/policy/policy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/policy/policy_service.py` & `syft-0.8.2b6/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.2b6/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/project/project.py` & `syft-0.8.2b6/src/syft/service/project/project.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/project/project_service.py` & `syft-0.8.2b6/src/syft/service/project/project_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/project/project_stash.py` & `syft-0.8.2b6/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/queue/base_queue.py` & `syft-0.8.2b6/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/queue/queue.py` & `syft-0.8.2b6/src/syft/service/queue/queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/queue/queue_stash.py` & `syft-0.8.2b6/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/queue/zmq_queue.py` & `syft-0.8.2b6/src/syft/service/queue/zmq_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/request/request.py` & `syft-0.8.2b6/src/syft/service/request/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # third party
 from result import Err
 from result import Ok
 from result import Result
 from typing_extensions import Self
 
 # relative
+from ...abstract_node import NodeSideType
 from ...client.api import APIRegistry
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...serde.serialize import _serialize
 from ...store.linked_obj import LinkedObject
 from ...types.datetime import DateTime
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
@@ -31,14 +32,15 @@
 from ...types.transforms import transform
 from ...types.uid import LineageID
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import SURFACE
 from ...util.markdown import markdown_as_class_with_fields
 from ...util.notebook_ui.notebook_addons import REQUEST_ICON
+from ...util.util import prompt_warning_message
 from ..action.action_object import ActionObject
 from ..action.action_service import ActionService
 from ..action.action_store import ActionObjectPermission
 from ..action.action_store import ActionPermission
 from ..code.user_code import UserCode
 from ..code.user_code import UserCodeStatus
 from ..context import AuthedServiceContext
@@ -267,14 +269,33 @@
         return request_status
 
     def approve(self):
         api = APIRegistry.api_for(
             self.node_uid,
             self.syft_client_verify_key,
         )
+        # TODO: Refactor so that object can also be passed to generate warnings
+        metadata = api.connection.get_node_metadata(api.signing_key)
+        code = self.code
+        message, is_enclave = None, False
+
+        if code and not isinstance(code, SyftError):
+            is_enclave = getattr(code, "enclave_metadata", None) is not None
+
+        if is_enclave:
+            message = "On approval, the result will be released to the enclave."
+        elif metadata.node_side_type == NodeSideType.HIGH_SIDE.value:
+            message = (
+                "You're approving a request on "
+                f"{metadata.node_side_type} side {metadata.node_type} "
+                "which may host datasets with private information."
+            )
+        if message and metadata.show_warnings:
+            prompt_warning_message(message=message, confirm=True)
+
         print(f"Request approved for domain {api.node_name}")
         return api.services.request.apply(self.id)
 
     def deny(self, reason: str):
         """Denies the particular request.
 
         Args:
```

### Comparing `syft-0.8.2b5/src/syft/service/request/request_service.py` & `syft-0.8.2b6/src/syft/service/request/request_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,18 @@
                 requests[i : i + page_size] for i in range(0, len(requests), page_size)
             ]
             # Return the proper slice using chunk_index
             requests = requests[page_index]
 
         return requests
 
-    @service_method(path="request.apply", name="apply")
+    @service_method(
+        path="request.apply",
+        name="apply",
+    )
     def apply(
         self, context: AuthedServiceContext, uid: UID
     ) -> Union[SyftSuccess, SyftError]:
         request = self.stash.get_by_uid(context.credentials, uid)
         if request.is_ok():
             request = request.ok()
             result = request.apply(context=context)
```

### Comparing `syft-0.8.2b5/src/syft/service/request/request_stash.py` & `syft-0.8.2b6/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/response.py` & `syft-0.8.2b6/src/syft/service/response.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,15 +17,19 @@
 
     def __eq__(self, other) -> bool:
         if isinstance(other, SyftResponseMessage):
             return self.message == other.message and self._bool == other._bool
         return self._bool == other
 
     def __repr__(self) -> str:
-        return f"{type(self)}: {self.message}"
+        _class_name_ = type(self).__name__
+        return f"{_class_name_}: {self.message}"
+
+    def __str__(self) -> str:
+        return self.__repr__()
 
     @property
     def _repr_html_class_(self) -> str:
         return "alert-info"
 
     def _repr_html_(self) -> str:
         return (
@@ -54,14 +58,21 @@
 class SyftNotReady(SyftResponseMessage):
     @property
     def _repr_html_class_(self) -> str:
         return "alert-info"
 
 
 @serializable()
+class SyftWarning(SyftResponseMessage):
+    @property
+    def _repr_html_class_(self) -> str:
+        return "alert-warning"
+
+
+@serializable()
 class SyftException(Exception):
     traceback: bool = False
     traceback_limit: int = 10
 
     @property
     def _repr_html_class_(self) -> str:
         return "alert-danger"
```

### Comparing `syft-0.8.2b5/src/syft/service/service.py` & `syft-0.8.2b6/src/syft/service/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from ..types.syft_object import attach_attribute_to_syft_object
 from ..types.uid import UID
 from .context import AuthedServiceContext
 from .context import ChangeContext
 from .response import SyftError
 from .user.user_roles import DATA_OWNER_ROLE_LEVEL
 from .user.user_roles import ServiceRole
+from .warnings import APIEndpointWarning
 
 TYPE_TO_SERVICE = {}
 SERVICE_TO_TYPES = defaultdict(set)
 
 
 class AbstractService:
     node: AbstractNode
@@ -74,14 +75,15 @@
     public_path: str
     private_path: str
     public_name: str
     method_name: str
     doc_string: Optional[str]
     signature: Optional[Signature]
     is_from_lib: bool = False
+    warning: Optional[APIEndpointWarning]
 
 
 @serializable()
 class ServiceConfig(BaseConfig):
     permissions: List
     roles: List[ServiceRole]
 
@@ -305,14 +307,15 @@
 
 
 def service_method(
     name: Optional[str] = None,
     path: Optional[str] = None,
     roles: Optional[List[ServiceRole]] = None,
     autosplat: Optional[List[str]] = None,
+    warning: Optional[APIEndpointWarning] = None,
 ):
     if roles is None or len(roles) == 0:
         # TODO: this is dangerous, we probably want to be more conservative
         roles = DATA_OWNER_ROLE_LEVEL
 
     def wrapper(func):
         func_name = func.__name__
@@ -351,14 +354,15 @@
             private_path=_path,
             public_name=("public_" + func_name) if name is None else name,
             method_name=func_name,
             doc_string=func.__doc__,
             signature=signature,
             roles=roles,
             permissions=["Guest"],
+            warning=warning,
         )
         ServiceConfigRegistry.register(config)
 
         _decorator.__name__ = func.__name__
         _decorator.__qualname__ = func.__qualname__
         return _decorator
```

### Comparing `syft-0.8.2b5/src/syft/service/settings/settings.py` & `syft-0.8.2b6/src/syft/service/settings/settings.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # stdlib
 
 # relative
+from ...abstract_node import NodeSideType
 from ...serde.serializable import serializable
 from ...types.syft_object import PartialSyftObject
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
 from ...types.uid import UID
 
 
@@ -37,7 +38,9 @@
     name: str = "Node"
     deployed_on: str
     organization: str = "OpenMined"
     on_board: bool = True
     description: str = "Text"
     signup_enabled: bool
     admin_email: str
+    node_side_type: NodeSideType = NodeSideType.HIGH_SIDE
+    show_warnings: bool
```

### Comparing `syft-0.8.2b5/src/syft/service/settings/settings_service.py` & `syft-0.8.2b6/src/syft/service/settings/settings_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from ...util.experimental_flags import flags
 from ..context import AuthedServiceContext
 from ..context import UnauthedServiceContext
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import service_method
+from ..warnings import HighSideCRUDWarning
 from .settings import NodeSettings
 from .settings import NodeSettingsUpdate
 from .settings_stash import SettingsStash
 
 
 @serializable()
 class SettingsService(AbstractService):
@@ -75,15 +76,19 @@
                 else:
                     return SyftError(message=update_result.err())
             else:
                 return SyftError(message="No settings found")
         else:
             return SyftError(message=result.err())
 
-    @service_method(path="settings.allow_guest_signup", name="allow_guest_signup")
+    @service_method(
+        path="settings.allow_guest_signup",
+        name="allow_guest_signup",
+        warning=HighSideCRUDWarning(confirmation=True),
+    )
     def allow_guest_signup(
         self, context: AuthedServiceContext, enable: bool
     ) -> Union[SyftSuccess, SyftError]:
         """Enable/Disable Registration for Data Scientist or Guest Users."""
         flags.CAN_REGISTER = enable
         method = context.node.get_service_method(SettingsService.update)
         settings = NodeSettingsUpdate(signup_enabled=enable)
```

### Comparing `syft-0.8.2b5/src/syft/service/settings/settings_stash.py` & `syft-0.8.2b6/src/syft/service/settings/settings_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/user/user.py` & `syft-0.8.2b6/src/syft/service/user/user.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/user/user_roles.py` & `syft-0.8.2b6/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/user/user_service.py` & `syft-0.8.2b6/src/syft/service/user/user_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,19 @@
             user = result.ok()
             if user is None:
                 return SyftError(message=f"No user exists for given: {uid}")
             return user.to(UserView)
 
         return SyftError(message=str(result.err()))
 
-    @service_method(path="user.get_all", name="get_all", roles=DATA_OWNER_ROLE_LEVEL)
+    @service_method(
+        path="user.get_all",
+        name="get_all",
+        roles=DATA_OWNER_ROLE_LEVEL,
+    )
     def get_all(
         self,
         context: AuthedServiceContext,
         page_size: Optional[int] = 0,
         page_index: Optional[int] = 0,
     ) -> Union[Optional[UserViewPage], Optional[UserView], SyftError]:
         result = self.stash.get_all(context.credentials)
```

### Comparing `syft-0.8.2b5/src/syft/service/user/user_stash.py` & `syft-0.8.2b6/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/vpn/headscale_client.py` & `syft-0.8.2b6/src/syft/service/vpn/headscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/vpn/tailscale_client.py` & `syft-0.8.2b6/src/syft/service/vpn/tailscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/service/vpn/vpn.py` & `syft-0.8.2b6/src/syft/service/vpn/vpn.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/store/dict_document_store.py` & `syft-0.8.2b6/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/store/document_store.py` & `syft-0.8.2b6/src/syft/store/document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/store/kv_document_store.py` & `syft-0.8.2b6/src/syft/store/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/store/linked_obj.py` & `syft-0.8.2b6/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/store/locks.py` & `syft-0.8.2b6/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/store/mongo_client.py` & `syft-0.8.2b6/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/store/mongo_codecs.py` & `syft-0.8.2b6/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/store/mongo_document_store.py` & `syft-0.8.2b6/src/syft/store/mongo_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/store/sqlite_document_store.py` & `syft-0.8.2b6/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/types/datetime.py` & `syft-0.8.2b6/src/syft/types/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/types/grid_url.py` & `syft-0.8.2b6/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/types/syft_metaclass.py` & `syft-0.8.2b6/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/types/syft_object.py` & `syft-0.8.2b6/src/syft/types/syft_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/types/transforms.py` & `syft-0.8.2b6/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/types/twin_object.py` & `syft-0.8.2b6/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/types/uid.py` & `syft-0.8.2b6/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/util/autoreload.py` & `syft-0.8.2b6/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/util/decorators.py` & `syft-0.8.2b6/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/util/experimental_flags.py` & `syft-0.8.2b6/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/util/filterwarnings.py` & `syft-0.8.2b6/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/util/fonts.py` & `syft-0.8.2b6/src/syft/util/fonts.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/util/logger.py` & `syft-0.8.2b6/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/util/markdown.py` & `syft-0.8.2b6/src/syft/util/markdown.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/util/notebook_ui/notebook_addons.py` & `syft-0.8.2b6/src/syft/util/notebook_ui/notebook_addons.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/util/schema.py` & `syft-0.8.2b6/src/syft/util/schema.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/util/telemetry.py` & `syft-0.8.2b6/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/util/trace_decorator.py` & `syft-0.8.2b6/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft/util/util.py` & `syft-0.8.2b6/src/syft/util/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,20 @@
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Type
 from typing import Union
 
 # third party
+from IPython.display import display
 from forbiddenfruit import curse
 from nacl.signing import SigningKey
 from nacl.signing import VerifyKey
 import requests
+from rich.prompt import Confirm
 
 # relative
 from .logger import critical
 from .logger import debug
 from .logger import error
 from .logger import traceback_and_raise
 
@@ -439,14 +441,30 @@
         log = f"Cannot find {type(obj)} {fqn} in lib_ast. {e}"
         critical(log)
         raise Exception(log)
 
     return ref.pointer_type  # type: ignore
 
 
+def prompt_warning_message(message: str, confirm: bool = False) -> bool:
+    # relative
+    from ..service.response import SyftWarning
+
+    warning = SyftWarning(message=message)
+    display(warning)
+
+    if confirm:
+        allowed = Confirm.ask("Would you like to proceed?")
+        if not allowed:
+            display("Aborted !!")
+            return False
+
+    return True
+
+
 left_name = [
     "admiring",
     "adoring",
     "affectionate",
     "agitated",
     "amazing",
     "angry",
```

### Comparing `syft-0.8.2b5/src/syft/util/version_compare.py` & `syft-0.8.2b6/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b5/src/syft.egg-info/PKG-INFO` & `syft-0.8.2b6/src/syft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.2b5
+Version: 0.8.2b6
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.2b5 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.2b6 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: telemetry
```

### Comparing `syft-0.8.2b5/src/syft.egg-info/SOURCES.txt` & `syft-0.8.2b6/src/syft.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 src/syft/serde/serialize.py
 src/syft/serde/signature.py
 src/syft/serde/third_party.py
 src/syft/service/__init__.py
 src/syft/service/context.py
 src/syft/service/response.py
 src/syft/service/service.py
+src/syft/service/warnings.py
 src/syft/service/action/__init__.py
 src/syft/service/action/action_data_empty.py
 src/syft/service/action/action_graph.py
 src/syft/service/action/action_graph_service.py
 src/syft/service/action/action_object.py
 src/syft/service/action/action_permissions.py
 src/syft/service/action/action_service.py
```

### Comparing `syft-0.8.2b5/src/syft.egg-info/requires.txt` & `syft-0.8.2b6/src/syft.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 pycapnp==1.3.0
 pydantic[email]==1.10.7
 pymongo==4.3.3
 pynacl==1.5.0
 pyzmq<=25.1.0,>=23.2.1
 redis==4.5.5
 requests==2.31.0
-RestrictedPython==6.0
+RestrictedPython==6.1
 result==0.10.0
 tqdm==4.65.0
 typeguard==2.13.3
 typing_extensions==4.6.3
 sherlock[filelock,redis]==0.4.1
 uvicorn[standard]==0.22.0
 fastapi==0.97.0
```

