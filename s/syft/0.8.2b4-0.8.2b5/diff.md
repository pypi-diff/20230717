# Comparing `tmp/syft-0.8.2b4.tar.gz` & `tmp/syft-0.8.2b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.2b4.tar", last modified: Fri Jul 14 05:28:24 2023, max compression
+gzip compressed data, was "syft-0.8.2b5.tar", last modified: Mon Jul 17 02:54:07 2023, max compression
```

## Comparing `syft-0.8.2b4.tar` & `syft-0.8.2b5.tar`

### file list

```diff
@@ -1,211 +1,213 @@
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.845855 syft-0.8.2b4/
--rw-r--r--   0 om        (1001) users      (100)    11843 2023-07-14 05:26:20.000000 syft-0.8.2b4/LICENSE
--rw-r--r--   0 om        (1001) users      (100)       98 2023-07-14 05:26:20.000000 syft-0.8.2b4/MANIFEST.in
--rw-r--r--   0 om        (1001) users      (100)    16852 2023-07-14 05:28:24.845855 syft-0.8.2b4/PKG-INFO
--rw-r--r--   0 om        (1001) users      (100)    16170 2023-07-14 05:26:20.000000 syft-0.8.2b4/README.md
--rw-r--r--   0 om        (1001) users      (100)      272 2023-07-14 05:26:20.000000 syft-0.8.2b4/pyproject.toml
--rw-r--r--   0 om        (1001) users      (100)     3210 2023-07-14 05:28:24.845855 syft-0.8.2b4/setup.cfg
--rw-r--r--   0 om        (1001) users      (100)      107 2023-07-14 05:26:20.000000 syft-0.8.2b4/setup.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.829855 syft-0.8.2b4/src/
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.829855 syft-0.8.2b4/src/syft/
--rw-r--r--   0 om        (1001) users      (100)      580 2023-07-14 05:26:27.000000 syft-0.8.2b4/src/syft/VERSION
--rw-r--r--   0 om        (1001) users      (100)     5626 2023-07-14 05:26:27.000000 syft-0.8.2b4/src/syft/__init__.py
--rw-r--r--   0 om        (1001) users      (100)       93 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/__main__.py
--rw-r--r--   0 om        (1001) users      (100)      654 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/abstract_node.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.833855 syft-0.8.2b4/src/syft/capnp/
--rw-r--r--   0 om        (1001) users      (100)      270 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/capnp/__init__.py
--rw-r--r--   0 om        (1001) users      (100)       75 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/capnp/iterable.capnp
--rw-r--r--   0 om        (1001) users      (100)      102 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 om        (1001) users      (100)      186 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.833855 syft-0.8.2b4/src/syft/client/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    25732 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/api.py
--rw-r--r--   0 om        (1001) users      (100)    28029 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/client.py
--rw-r--r--   0 om        (1001) users      (100)      568 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/connection.py
--rw-r--r--   0 om        (1001) users      (100)      650 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/deploy.py
--rw-r--r--   0 om        (1001) users      (100)     8798 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/domain_client.py
--rw-r--r--   0 om        (1001) users      (100)     4434 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/enclave_client.py
--rw-r--r--   0 om        (1001) users      (100)     2372 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/gateway_client.py
--rw-r--r--   0 om        (1001) users      (100)    15257 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/registry.py
--rw-r--r--   0 om        (1001) users      (100)     2623 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/search.py
--rw-r--r--   0 om        (1001) users      (100)      549 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/client/user_settings.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.833855 syft-0.8.2b4/src/syft/external/
--rw-r--r--   0 om        (1001) users      (100)     1735 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/__init__.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.833855 syft-0.8.2b4/src/syft/external/oblv/
--rw-r--r--   0 om        (1001) users      (100)      860 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      284 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/auth.py
--rw-r--r--   0 om        (1001) users      (100)      212 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/constants.py
--rw-r--r--   0 om        (1001) users      (100)     4835 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/deployment.py
--rw-r--r--   0 om        (1001) users      (100)    12380 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 om        (1001) users      (100)     1800 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 om        (1001) users      (100)      489 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 om        (1001) users      (100)     2280 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 om        (1001) users      (100)     7462 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 om        (1001) users      (100)    13948 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 om        (1001) users      (100)     1146 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/gevent_patch.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.833855 syft-0.8.2b4/src/syft/img/
--rw-r--r--   0 om        (1001) users      (100)      297 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/img/base64.py
--rw-r--r--   0 om        (1001) users      (100)    25535 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/img/logo.png
--rw-r--r--   0 om        (1001) users      (100)    41764 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/img/small-grid-symbol-logo.png
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.837855 syft-0.8.2b4/src/syft/node/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     2631 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/credentials.py
--rw-r--r--   0 om        (1001) users      (100)      152 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/domain.py
--rw-r--r--   0 om        (1001) users      (100)      259 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/enclave.py
--rw-r--r--   0 om        (1001) users      (100)      728 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/gateway.py
--rw-r--r--   0 om        (1001) users      (100)    31684 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/node.py
--rw-r--r--   0 om        (1001) users      (100)     6960 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/routes.py
--rw-r--r--   0 om        (1001) users      (100)     2064 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/run.py
--rw-r--r--   0 om        (1001) users      (100)     6992 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/server.py
--rw-r--r--   0 om        (1001) users      (100)      127 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/worker.py
--rw-r--r--   0 om        (1001) users      (100)     1100 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/node/worker_settings.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.837855 syft-0.8.2b4/src/syft/serde/
--rw-r--r--   0 om        (1001) users      (100)      159 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     3597 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/array.py
--rw-r--r--   0 om        (1001) users      (100)     4099 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/arrow.py
--rw-r--r--   0 om        (1001) users      (100)      298 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/capnp.py
--rw-r--r--   0 om        (1001) users      (100)      722 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/deserialize.py
--rw-r--r--   0 om        (1001) users      (100)     1230 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/lib_permissions.py
--rw-r--r--   0 om        (1001) users      (100)    11663 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 om        (1001) users      (100)      875 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/mock.py
--rw-r--r--   0 om        (1001) users      (100)    11639 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/recursive.py
--rw-r--r--   0 om        (1001) users      (100)    10253 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 om        (1001) users      (100)     1822 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/serializable.py
--rw-r--r--   0 om        (1001) users      (100)      369 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/serialize.py
--rw-r--r--   0 om        (1001) users      (100)     4959 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/signature.py
--rw-r--r--   0 om        (1001) users      (100)     4885 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/serde/third_party.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.837855 syft-0.8.2b4/src/syft/service/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/__init__.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.837855 syft-0.8.2b4/src/syft/service/action/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      703 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 om        (1001) users      (100)    16706 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/action_graph.py
--rw-r--r--   0 om        (1001) users      (100)     6874 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 om        (1001) users      (100)    48803 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/action_object.py
--rw-r--r--   0 om        (1001) users      (100)     2502 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/action_permissions.py
--rw-r--r--   0 om        (1001) users      (100)    26998 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/action_service.py
--rw-r--r--   0 om        (1001) users      (100)    10264 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/action_store.py
--rw-r--r--   0 om        (1001) users      (100)     1165 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/action_types.py
--rw-r--r--   0 om        (1001) users      (100)     3889 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/numpy.py
--rw-r--r--   0 om        (1001) users      (100)     2233 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/pandas.py
--rw-r--r--   0 om        (1001) users      (100)     2920 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/plan.py
--rw-r--r--   0 om        (1001) users      (100)     4951 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/action/verification.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.837855 syft-0.8.2b4/src/syft/service/code/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/code/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      236 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/code/code_parse.py
--rw-r--r--   0 om        (1001) users      (100)      102 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/code/unparse.py
--rw-r--r--   0 om        (1001) users      (100)    27413 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/code/user_code.py
--rw-r--r--   0 om        (1001) users      (100)     1756 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 om        (1001) users      (100)    10340 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/code/user_code_service.py
--rw-r--r--   0 om        (1001) users      (100)     1446 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 om        (1001) users      (100)     1782 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/context.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.837855 syft-0.8.2b4/src/syft/service/data_subject/
--rw-r--r--   0 om        (1001) users      (100)       69 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     4076 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 om        (1001) users      (100)      870 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 om        (1001) users      (100)     3215 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 om        (1001) users      (100)     5006 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/dataset/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/dataset/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    23590 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/dataset/dataset.py
--rw-r--r--   0 om        (1001) users      (100)     6382 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 om        (1001) users      (100)     1911 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/enclave/
--rw-r--r--   0 om        (1001) users      (100)     6038 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/enclave/enclave_service.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/metadata/
--rw-r--r--   0 om        (1001) users      (100)     3605 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/network/
--rw-r--r--   0 om        (1001) users      (100)    18133 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/network/network_service.py
--rw-r--r--   0 om        (1001) users      (100)     3064 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/network/node_peer.py
--rw-r--r--   0 om        (1001) users      (100)     4593 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/network/routes.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/notification/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/notification/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     7961 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/notification/notification_service.py
--rw-r--r--   0 om        (1001) users      (100)     4566 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/notification/notification_stash.py
--rw-r--r--   0 om        (1001) users      (100)     3259 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/notification/notifications.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/policy/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/policy/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    22437 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/policy/policy.py
--rw-r--r--   0 om        (1001) users      (100)     2081 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/policy/policy_service.py
--rw-r--r--   0 om        (1001) users      (100)     1077 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/project/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/project/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    48433 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/project/project.py
--rw-r--r--   0 om        (1001) users      (100)    15374 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/project/project_service.py
--rw-r--r--   0 om        (1001) users      (100)     1908 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/queue/
--rw-r--r--   0 om        (1001) users      (100)     2044 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/queue/base_queue.py
--rw-r--r--   0 om        (1001) users      (100)     3008 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/queue/queue.py
--rw-r--r--   0 om        (1001) users      (100)     4845 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 om        (1001) users      (100)     7929 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/request/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/request/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    26923 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/request/request.py
--rw-r--r--   0 om        (1001) users      (100)    10112 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/request/request_service.py
--rw-r--r--   0 om        (1001) users      (100)     1410 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/request/request_stash.py
--rw-r--r--   0 om        (1001) users      (100)     2850 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/response.py
--rw-r--r--   0 om        (1001) users      (100)    13653 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/service.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/settings/
--rw-r--r--   0 om        (1001) users      (100)      881 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/settings/settings.py
--rw-r--r--   0 om        (1001) users      (100)     3486 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/settings/settings_service.py
--rw-r--r--   0 om        (1001) users      (100)     1711 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/user/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/user/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      201 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/user/roles.py
--rw-r--r--   0 om        (1001) users      (100)     6115 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/user/user.py
--rw-r--r--   0 om        (1001) users      (100)     3427 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/user/user_roles.py
--rw-r--r--   0 om        (1001) users      (100)    15957 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/user/user_service.py
--rw-r--r--   0 om        (1001) users      (100)     4363 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.841855 syft-0.8.2b4/src/syft/service/vpn/
--rw-r--r--   0 om        (1001) users      (100)     1809 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/vpn/headscale_client.py
--rw-r--r--   0 om        (1001) users      (100)     6789 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/vpn/tailscale_client.py
--rw-r--r--   0 om        (1001) users      (100)     5414 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/service/vpn/vpn.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.845855 syft-0.8.2b4/src/syft/store/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     3235 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/dict_document_store.py
--rw-r--r--   0 om        (1001) users      (100)    22993 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/document_store.py
--rw-r--r--   0 om        (1001) users      (100)    22010 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/kv_document_store.py
--rw-r--r--   0 om        (1001) users      (100)     4326 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/linked_obj.py
--rw-r--r--   0 om        (1001) users      (100)    11840 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/locks.py
--rw-r--r--   0 om        (1001) users      (100)     8768 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/mongo_client.py
--rw-r--r--   0 om        (1001) users      (100)      846 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/mongo_codecs.py
--rw-r--r--   0 om        (1001) users      (100)    13836 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/mongo_document_store.py
--rw-r--r--   0 om        (1001) users      (100)    13136 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.845855 syft-0.8.2b4/src/syft/types/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      136 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/base.py
--rw-r--r--   0 om        (1001) users      (100)     1091 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/datetime.py
--rw-r--r--   0 om        (1001) users      (100)     5167 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/grid_url.py
--rw-r--r--   0 om        (1001) users      (100)     4807 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/syft_metaclass.py
--rw-r--r--   0 om        (1001) users      (100)    25848 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/syft_object.py
--rw-r--r--   0 om        (1001) users      (100)     8113 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/transforms.py
--rw-r--r--   0 om        (1001) users      (100)     2098 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/twin_object.py
--rw-r--r--   0 om        (1001) users      (100)     8038 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/types/uid.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.845855 syft-0.8.2b4/src/syft/util/
--rw-r--r--   0 om        (1001) users      (100)       67 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      852 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/autoreload.py
--rw-r--r--   0 om        (1001) users      (100)      271 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/colors.py
--rw-r--r--   0 om        (1001) users      (100)       34 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/constants.py
--rw-r--r--   0 om        (1001) users      (100)     1514 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/decorators.py
--rw-r--r--   0 om        (1001) users      (100)     1607 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/experimental_flags.py
--rw-r--r--   0 om        (1001) users      (100)     1327 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/filterwarnings.py
--rw-r--r--   0 om        (1001) users      (100)     2940 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/fonts.py
--rw-r--r--   0 om        (1001) users      (100)      153 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/jax_settings.py
--rw-r--r--   0 om        (1001) users      (100)     3779 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/logger.py
--rw-r--r--   0 om        (1001) users      (100)      752 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/markdown.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.845855 syft-0.8.2b4/src/syft/util/notebook_ui/
--rw-r--r--   0 om        (1001) users      (100)    27090 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/notebook_ui/notebook_addons.py
--rw-r--r--   0 om        (1001) users      (100)       42 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/options.py
--rw-r--r--   0 om        (1001) users      (100)     5297 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/schema.py
--rw-r--r--   0 om        (1001) users      (100)     2771 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/telemetry.py
--rw-r--r--   0 om        (1001) users      (100)     6728 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/trace_decorator.py
--rw-r--r--   0 om        (1001) users      (100)    22738 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/util.py
--rw-r--r--   0 om        (1001) users      (100)     3123 2023-07-14 05:26:20.000000 syft-0.8.2b4/src/syft/util/version_compare.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-14 05:28:24.833855 syft-0.8.2b4/src/syft.egg-info/
--rw-r--r--   0 om        (1001) users      (100)    16852 2023-07-14 05:28:24.000000 syft-0.8.2b4/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 om        (1001) users      (100)     5879 2023-07-14 05:28:24.000000 syft-0.8.2b4/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 om        (1001) users      (100)        1 2023-07-14 05:28:24.000000 syft-0.8.2b4/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 om        (1001) users      (100)       43 2023-07-14 05:28:24.000000 syft-0.8.2b4/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 om        (1001) users      (100)        1 2023-07-14 05:28:24.000000 syft-0.8.2b4/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 om        (1001) users      (100)     1555 2023-07-14 05:28:24.000000 syft-0.8.2b4/src/syft.egg-info/requires.txt
--rw-r--r--   0 om        (1001) users      (100)        5 2023-07-14 05:28:24.000000 syft-0.8.2b4/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.227497 syft-0.8.2b5/
+-rw-r--r--   0 om        (1001) users      (100)    11843 2023-07-17 02:52:43.000000 syft-0.8.2b5/LICENSE
+-rw-r--r--   0 om        (1001) users      (100)       98 2023-07-17 02:52:43.000000 syft-0.8.2b5/MANIFEST.in
+-rw-r--r--   0 om        (1001) users      (100)    16852 2023-07-17 02:54:07.227497 syft-0.8.2b5/PKG-INFO
+-rw-r--r--   0 om        (1001) users      (100)    16170 2023-07-17 02:52:43.000000 syft-0.8.2b5/README.md
+-rw-r--r--   0 om        (1001) users      (100)      272 2023-07-17 02:52:43.000000 syft-0.8.2b5/pyproject.toml
+-rw-r--r--   0 om        (1001) users      (100)     3210 2023-07-17 02:54:07.227497 syft-0.8.2b5/setup.cfg
+-rw-r--r--   0 om        (1001) users      (100)      107 2023-07-17 02:52:43.000000 syft-0.8.2b5/setup.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.211497 syft-0.8.2b5/src/
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.211497 syft-0.8.2b5/src/syft/
+-rw-r--r--   0 om        (1001) users      (100)      580 2023-07-17 02:52:46.000000 syft-0.8.2b5/src/syft/VERSION
+-rw-r--r--   0 om        (1001) users      (100)     5626 2023-07-17 02:52:46.000000 syft-0.8.2b5/src/syft/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)       93 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/__main__.py
+-rw-r--r--   0 om        (1001) users      (100)      654 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/abstract_node.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.215497 syft-0.8.2b5/src/syft/capnp/
+-rw-r--r--   0 om        (1001) users      (100)      270 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/capnp/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)       75 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 om        (1001) users      (100)      102 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 om        (1001) users      (100)      186 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.215497 syft-0.8.2b5/src/syft/client/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    25732 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/api.py
+-rw-r--r--   0 om        (1001) users      (100)    28112 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/client.py
+-rw-r--r--   0 om        (1001) users      (100)      568 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/connection.py
+-rw-r--r--   0 om        (1001) users      (100)      650 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/deploy.py
+-rw-r--r--   0 om        (1001) users      (100)     8798 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/domain_client.py
+-rw-r--r--   0 om        (1001) users      (100)     4434 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/enclave_client.py
+-rw-r--r--   0 om        (1001) users      (100)     2372 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/gateway_client.py
+-rw-r--r--   0 om        (1001) users      (100)    15257 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/registry.py
+-rw-r--r--   0 om        (1001) users      (100)     2623 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/search.py
+-rw-r--r--   0 om        (1001) users      (100)      549 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/client/user_settings.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.215497 syft-0.8.2b5/src/syft/external/
+-rw-r--r--   0 om        (1001) users      (100)     1735 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/__init__.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.215497 syft-0.8.2b5/src/syft/external/oblv/
+-rw-r--r--   0 om        (1001) users      (100)      860 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      284 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/auth.py
+-rw-r--r--   0 om        (1001) users      (100)      212 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/constants.py
+-rw-r--r--   0 om        (1001) users      (100)     4835 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 om        (1001) users      (100)    12380 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 om        (1001) users      (100)     1800 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 om        (1001) users      (100)      489 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 om        (1001) users      (100)     2280 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     7462 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 om        (1001) users      (100)    13948 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1146 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/gevent_patch.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.215497 syft-0.8.2b5/src/syft/img/
+-rw-r--r--   0 om        (1001) users      (100)      297 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/img/base64.py
+-rw-r--r--   0 om        (1001) users      (100)    25535 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/img/logo.png
+-rw-r--r--   0 om        (1001) users      (100)    41764 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/img/small-grid-symbol-logo.png
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.215497 syft-0.8.2b5/src/syft/node/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     2631 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/credentials.py
+-rw-r--r--   0 om        (1001) users      (100)      152 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/domain.py
+-rw-r--r--   0 om        (1001) users      (100)      259 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/enclave.py
+-rw-r--r--   0 om        (1001) users      (100)      728 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/gateway.py
+-rw-r--r--   0 om        (1001) users      (100)    32225 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/node.py
+-rw-r--r--   0 om        (1001) users      (100)     6960 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/routes.py
+-rw-r--r--   0 om        (1001) users      (100)     2064 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/run.py
+-rw-r--r--   0 om        (1001) users      (100)     6992 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/server.py
+-rw-r--r--   0 om        (1001) users      (100)      127 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/worker.py
+-rw-r--r--   0 om        (1001) users      (100)     1100 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/node/worker_settings.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.219498 syft-0.8.2b5/src/syft/serde/
+-rw-r--r--   0 om        (1001) users      (100)      159 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     3597 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/array.py
+-rw-r--r--   0 om        (1001) users      (100)     4099 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/arrow.py
+-rw-r--r--   0 om        (1001) users      (100)      298 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/capnp.py
+-rw-r--r--   0 om        (1001) users      (100)      722 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/deserialize.py
+-rw-r--r--   0 om        (1001) users      (100)     1230 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 om        (1001) users      (100)    11663 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 om        (1001) users      (100)      875 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/mock.py
+-rw-r--r--   0 om        (1001) users      (100)    11639 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/recursive.py
+-rw-r--r--   0 om        (1001) users      (100)    10253 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 om        (1001) users      (100)     1822 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/serializable.py
+-rw-r--r--   0 om        (1001) users      (100)      369 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/serialize.py
+-rw-r--r--   0 om        (1001) users      (100)     4959 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/signature.py
+-rw-r--r--   0 om        (1001) users      (100)     4885 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/serde/third_party.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.219498 syft-0.8.2b5/src/syft/service/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/__init__.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.219498 syft-0.8.2b5/src/syft/service/action/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      703 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 om        (1001) users      (100)    16706 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/action_graph.py
+-rw-r--r--   0 om        (1001) users      (100)     6874 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 om        (1001) users      (100)    48803 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/action_object.py
+-rw-r--r--   0 om        (1001) users      (100)     2502 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 om        (1001) users      (100)    26998 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/action_service.py
+-rw-r--r--   0 om        (1001) users      (100)    10264 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/action_store.py
+-rw-r--r--   0 om        (1001) users      (100)     1165 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/action_types.py
+-rw-r--r--   0 om        (1001) users      (100)     3889 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/numpy.py
+-rw-r--r--   0 om        (1001) users      (100)     2233 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/pandas.py
+-rw-r--r--   0 om        (1001) users      (100)     2920 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/plan.py
+-rw-r--r--   0 om        (1001) users      (100)     4951 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/action/verification.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.219498 syft-0.8.2b5/src/syft/service/code/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/code/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      236 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/code/code_parse.py
+-rw-r--r--   0 om        (1001) users      (100)      102 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/code/unparse.py
+-rw-r--r--   0 om        (1001) users      (100)    27413 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/code/user_code.py
+-rw-r--r--   0 om        (1001) users      (100)     1756 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 om        (1001) users      (100)    10340 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1446 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     1782 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/context.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.219498 syft-0.8.2b5/src/syft/service/data_subject/
+-rw-r--r--   0 om        (1001) users      (100)       69 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     4076 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 om        (1001) users      (100)      870 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 om        (1001) users      (100)     3215 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 om        (1001) users      (100)     5006 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/dataset/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    23590 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 om        (1001) users      (100)     6382 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1911 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/enclave/
+-rw-r--r--   0 om        (1001) users      (100)     6038 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/enclave/enclave_service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/metadata/
+-rw-r--r--   0 om        (1001) users      (100)     1170 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/metadata/metadata_service.py
+-rw-r--r--   0 om        (1001) users      (100)     3678 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/network/
+-rw-r--r--   0 om        (1001) users      (100)    18148 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/network/network_service.py
+-rw-r--r--   0 om        (1001) users      (100)     3100 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/network/node_peer.py
+-rw-r--r--   0 om        (1001) users      (100)     4593 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/network/routes.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/notification/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/notification/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     7961 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/notification/notification_service.py
+-rw-r--r--   0 om        (1001) users      (100)     4566 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/notification/notification_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     3259 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/notification/notifications.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/policy/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/policy/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    22437 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/policy/policy.py
+-rw-r--r--   0 om        (1001) users      (100)     2081 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1077 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/project/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/project/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    48433 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/project/project.py
+-rw-r--r--   0 om        (1001) users      (100)    15374 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/project/project_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1908 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/queue/
+-rw-r--r--   0 om        (1001) users      (100)     2044 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 om        (1001) users      (100)     3008 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/queue/queue.py
+-rw-r--r--   0 om        (1001) users      (100)     4845 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     7929 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/request/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/request/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    27212 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/request/request.py
+-rw-r--r--   0 om        (1001) users      (100)    10112 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/request/request_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1410 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/request/request_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     2850 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/response.py
+-rw-r--r--   0 om        (1001) users      (100)    13653 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/settings/
+-rw-r--r--   0 om        (1001) users      (100)      985 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/settings/settings.py
+-rw-r--r--   0 om        (1001) users      (100)     3486 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1711 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/user/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/user/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      201 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/user/roles.py
+-rw-r--r--   0 om        (1001) users      (100)     6115 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/user/user.py
+-rw-r--r--   0 om        (1001) users      (100)     3427 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/user/user_roles.py
+-rw-r--r--   0 om        (1001) users      (100)    16847 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/user/user_service.py
+-rw-r--r--   0 om        (1001) users      (100)     4510 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.223497 syft-0.8.2b5/src/syft/service/vpn/
+-rw-r--r--   0 om        (1001) users      (100)     1809 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/vpn/headscale_client.py
+-rw-r--r--   0 om        (1001) users      (100)     6789 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/vpn/tailscale_client.py
+-rw-r--r--   0 om        (1001) users      (100)     5414 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/service/vpn/vpn.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.227497 syft-0.8.2b5/src/syft/store/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     3235 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/dict_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    22993 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    22010 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/kv_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)     4326 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/linked_obj.py
+-rw-r--r--   0 om        (1001) users      (100)    11840 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/locks.py
+-rw-r--r--   0 om        (1001) users      (100)     8768 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/mongo_client.py
+-rw-r--r--   0 om        (1001) users      (100)      846 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 om        (1001) users      (100)    13836 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    13136 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.227497 syft-0.8.2b5/src/syft/types/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      136 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/base.py
+-rw-r--r--   0 om        (1001) users      (100)     1091 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/datetime.py
+-rw-r--r--   0 om        (1001) users      (100)     5167 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/grid_url.py
+-rw-r--r--   0 om        (1001) users      (100)     4807 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 om        (1001) users      (100)    25848 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/syft_object.py
+-rw-r--r--   0 om        (1001) users      (100)     8113 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/transforms.py
+-rw-r--r--   0 om        (1001) users      (100)     2098 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/twin_object.py
+-rw-r--r--   0 om        (1001) users      (100)     8038 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/types/uid.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.227497 syft-0.8.2b5/src/syft/util/
+-rw-r--r--   0 om        (1001) users      (100)       67 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      852 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/autoreload.py
+-rw-r--r--   0 om        (1001) users      (100)      271 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/colors.py
+-rw-r--r--   0 om        (1001) users      (100)       34 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/constants.py
+-rw-r--r--   0 om        (1001) users      (100)     1514 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/decorators.py
+-rw-r--r--   0 om        (1001) users      (100)      445 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/env.py
+-rw-r--r--   0 om        (1001) users      (100)     1607 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/experimental_flags.py
+-rw-r--r--   0 om        (1001) users      (100)     1327 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/filterwarnings.py
+-rw-r--r--   0 om        (1001) users      (100)     2940 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/fonts.py
+-rw-r--r--   0 om        (1001) users      (100)      153 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/jax_settings.py
+-rw-r--r--   0 om        (1001) users      (100)     3779 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/logger.py
+-rw-r--r--   0 om        (1001) users      (100)      752 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/markdown.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.227497 syft-0.8.2b5/src/syft/util/notebook_ui/
+-rw-r--r--   0 om        (1001) users      (100)    27090 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/notebook_ui/notebook_addons.py
+-rw-r--r--   0 om        (1001) users      (100)       42 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/options.py
+-rw-r--r--   0 om        (1001) users      (100)     5297 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/schema.py
+-rw-r--r--   0 om        (1001) users      (100)     2771 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/telemetry.py
+-rw-r--r--   0 om        (1001) users      (100)     6728 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/trace_decorator.py
+-rw-r--r--   0 om        (1001) users      (100)    22738 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/util.py
+-rw-r--r--   0 om        (1001) users      (100)     3123 2023-07-17 02:52:43.000000 syft-0.8.2b5/src/syft/util/version_compare.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-17 02:54:07.215497 syft-0.8.2b5/src/syft.egg-info/
+-rw-r--r--   0 om        (1001) users      (100)    16852 2023-07-17 02:54:07.000000 syft-0.8.2b5/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 om        (1001) users      (100)     5946 2023-07-17 02:54:07.000000 syft-0.8.2b5/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 om        (1001) users      (100)        1 2023-07-17 02:54:07.000000 syft-0.8.2b5/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 om        (1001) users      (100)       43 2023-07-17 02:54:07.000000 syft-0.8.2b5/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 om        (1001) users      (100)        1 2023-07-17 02:54:07.000000 syft-0.8.2b5/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 om        (1001) users      (100)     1555 2023-07-17 02:54:07.000000 syft-0.8.2b5/src/syft.egg-info/requires.txt
+-rw-r--r--   0 om        (1001) users      (100)        5 2023-07-17 02:54:07.000000 syft-0.8.2b5/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.2b4/LICENSE` & `syft-0.8.2b5/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/PKG-INFO` & `syft-0.8.2b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.2b4
+Version: 0.8.2b5
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
-Metadata-Version: 2.1 Name: syft Version: 0.8.2b4 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.2b5 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: telemetry
```

### Comparing `syft-0.8.2b4/README.md` & `syft-0.8.2b5/README.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/setup.cfg` & `syft-0.8.2b5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.2-beta.4"
+version = attr: "0.8.2-beta.5"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
```

### Comparing `syft-0.8.2b4/src/syft/VERSION` & `syft-0.8.2b5/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.2-beta.4"
+__version__ = "0.8.2-beta.5"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.2b4/src/syft/__init__.py` & `syft-0.8.2b5/src/syft/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.2-beta.4"
+__version__ = "0.8.2-beta.5"
 
 # stdlib
 import pathlib
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
```

### Comparing `syft-0.8.2b4/src/syft/abstract_node.py` & `syft-0.8.2b5/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/client/api.py` & `syft-0.8.2b5/src/syft/client/api.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/client/client.py` & `syft-0.8.2b5/src/syft/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,14 +436,17 @@
         self.connection = connection
         self.metadata = metadata
         self.credentials: Optional[SyftSigningKey] = credentials
         self._api = api
 
         self.post_init()
 
+    def get_env(self) -> str:
+        return self.api.services.metadata.get_env()
+
     def post_init(self) -> None:
         if self.metadata is None:
             self._fetch_node_metadata(self.credentials)
 
     def create_project(
         self, name: str, description: str, user_email_address: str
     ) -> Any:
```

### Comparing `syft-0.8.2b4/src/syft/client/connection.py` & `syft-0.8.2b5/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/client/deploy.py` & `syft-0.8.2b5/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/client/domain_client.py` & `syft-0.8.2b5/src/syft/client/domain_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/client/enclave_client.py` & `syft-0.8.2b5/src/syft/client/enclave_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/client/gateway_client.py` & `syft-0.8.2b5/src/syft/client/gateway_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/client/registry.py` & `syft-0.8.2b5/src/syft/client/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/client/search.py` & `syft-0.8.2b5/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/client/user_settings.py` & `syft-0.8.2b5/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/external/__init__.py` & `syft-0.8.2b5/src/syft/external/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/external/oblv/__init__.py` & `syft-0.8.2b5/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/external/oblv/deployment.py` & `syft-0.8.2b5/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/external/oblv/deployment_client.py` & `syft-0.8.2b5/src/syft/external/oblv/deployment_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/external/oblv/exceptions.py` & `syft-0.8.2b5/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.2b5/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.2b5/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/external/oblv/oblv_service.py` & `syft-0.8.2b5/src/syft/external/oblv/oblv_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/gevent_patch.py` & `syft-0.8.2b5/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/img/logo.png` & `syft-0.8.2b5/src/syft/img/logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/img/small-grid-symbol-logo.png` & `syft-0.8.2b5/src/syft/img/small-grid-symbol-logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/node/credentials.py` & `syft-0.8.2b5/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/node/gateway.py` & `syft-0.8.2b5/src/syft/node/gateway.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/node/node.py` & `syft-0.8.2b5/src/syft/node/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import binascii
 import contextlib
 from datetime import datetime
 from functools import partial
 import hashlib
 from multiprocessing import current_process
 import os
+import subprocess  # nosec
 import traceback
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
@@ -48,14 +49,15 @@
 from ..service.context import NodeServiceContext
 from ..service.context import UnauthedServiceContext
 from ..service.context import UserLoginCredentials
 from ..service.data_subject.data_subject_member_service import DataSubjectMemberService
 from ..service.data_subject.data_subject_service import DataSubjectService
 from ..service.dataset.dataset_service import DatasetService
 from ..service.enclave.enclave_service import EnclaveService
+from ..service.metadata.metadata_service import MetadataService
 from ..service.metadata.node_metadata import NodeMetadata
 from ..service.network.network_service import NetworkService
 from ..service.notification.notification_service import NotificationService
 from ..service.policy.policy_service import PolicyService
 from ..service.project.project_service import ProjectService
 from ..service.queue.queue import APICallMessageHandler
 from ..service.queue.queue import QueueManager
@@ -143,27 +145,35 @@
     return get_env(DEFAULT_ROOT_PASSWORD, "changethis")  # nosec
 
 
 def get_dev_mode() -> bool:
     return str_to_bool(get_env("DEV_MODE", "False"))
 
 
+def get_venv_packages() -> str:
+    res = subprocess.getoutput(
+        "pip list --format=freeze",
+    )
+    return res
+
+
 dev_mode = get_dev_mode()
 
 signing_key_env = get_private_key_env()
 node_uid_env = get_node_uid_env()
 
 default_root_email = get_default_root_email()
 default_root_password = get_default_root_password()
 
 
 @instrument
 class Node(AbstractNode):
     signing_key: Optional[SyftSigningKey]
     required_signed_calls: bool = True
+    packages: str
 
     def __init__(
         self,
         *,  # Trasterisk
         name: Optional[str] = None,
         id: Optional[UID] = None,
         services: Optional[List[Type[AbstractService]]] = None,
@@ -183,14 +193,15 @@
         # less horrible or add some convenience functions
         if node_uid_env is not None:
             self.id = UID.from_string(node_uid_env)
         else:
             if id is None:
                 id = UID()
             self.id = id
+        self.packages = get_venv_packages()
 
         self.signing_key = None
         if signing_key_env is not None:
             self.signing_key = SyftSigningKey.from_string(signing_key_env)
         else:
             if isinstance(signing_key, SigningKey):
                 signing_key = SyftSigningKey(signing_key=signing_key)
@@ -213,14 +224,15 @@
                 DataSubjectService,
                 NetworkService,
                 PolicyService,
                 NotificationService,
                 DataSubjectMemberService,
                 ProjectService,
                 EnclaveService,
+                MetadataService,
             ]
             if services is None
             else services
         )
 
         self.service_config = ServiceConfigRegistry.get_registered_configs()
         self.local_db = local_db
@@ -249,15 +261,15 @@
 
         self.client_cache = {}
         if isinstance(node_type, str):
             node_type = NodeType(node_type)
         self.node_type = node_type
 
         self.post_init()
-        self.create_initial_settings()
+        self.create_initial_settings(admin_email=root_email)
         if not (self.is_subprocess or self.processes == 0):
             self.init_queue_manager(queue_config=queue_config)
 
         NodeRegistry.set_node_for(self.id, self)
 
     def init_queue_manager(self, queue_config: QueueConfig):
         MessageHandlers = [APICallMessageHandler]
@@ -458,14 +470,15 @@
                 DataSubjectService,
                 NetworkService,
                 PolicyService,
                 NotificationService,
                 DataSubjectMemberService,
                 ProjectService,
                 EnclaveService,
+                MetadataService,
             ]
 
             if OBLV:
                 # relative
                 from ..external.oblv.oblv_service import OblvService
 
                 store_services += [OblvService]
@@ -504,39 +517,42 @@
     def metadata(self) -> NodeMetadata:
         name = ""
         deployed_on = ""
         organization = ""
         on_board = False
         description = ""
         signup_enabled = False
+        admin_email = ""
 
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
+            admin_email = settings_data.admin_email
 
         return NodeMetadata(
             name=name,
             id=self.id,
             verify_key=self.verify_key,
             highest_object_version=HIGHEST_SYFT_OBJECT_VERSION,
             lowest_object_version=LOWEST_SYFT_OBJECT_VERSION,
             syft_version=__version__,
             deployed_on=deployed_on,
             description=description,
             organization=organization,
             on_board=on_board,
             node_type=self.node_type.value,
             signup_enabled=signup_enabled,
+            admin_email=admin_email,
         )
 
     @property
     def icon(self) -> str:
         return "🦾"
 
     @property
@@ -703,15 +719,15 @@
         return partial(method, context=context)
 
     def get_unauthed_context(
         self, login_credentials: UserLoginCredentials
     ) -> NodeServiceContext:
         return UnauthedServiceContext(node=self, login_credentials=login_credentials)
 
-    def create_initial_settings(self) -> Optional[NodeSettings]:
+    def create_initial_settings(self, admin_email: str) -> Optional[NodeSettings]:
         if self.name is None:
             self.name = random_name()
         try:
             settings_stash = SettingsStash(store=self.document_store)
             settings_exists = settings_stash.get_all(self.signing_key.verify_key).ok()
             if settings_exists:
                 self.name = settings_exists[0].name
@@ -721,14 +737,15 @@
                 # as enclaves do not have superusers
                 if self.node_type == NodeType.ENCLAVE:
                     flags.CAN_REGISTER = True
                 new_settings = NodeSettings(
                     name=self.name,
                     deployed_on=datetime.now().date().strftime("%m/%d/%Y"),
                     signup_enabled=flags.CAN_REGISTER,
+                    admin_email=admin_email,
                 )
                 result = settings_stash.set(
                     credentials=self.signing_key.verify_key, settings=new_settings
                 )
                 if result.is_ok():
                     return result.ok()
                 return None
```

### Comparing `syft-0.8.2b4/src/syft/node/routes.py` & `syft-0.8.2b5/src/syft/node/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/node/run.py` & `syft-0.8.2b5/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/node/server.py` & `syft-0.8.2b5/src/syft/node/server.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/node/worker_settings.py` & `syft-0.8.2b5/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/serde/array.py` & `syft-0.8.2b5/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/serde/arrow.py` & `syft-0.8.2b5/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/serde/deserialize.py` & `syft-0.8.2b5/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/serde/lib_permissions.py` & `syft-0.8.2b5/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/serde/lib_service_registry.py` & `syft-0.8.2b5/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/serde/mock.py` & `syft-0.8.2b5/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/serde/recursive.py` & `syft-0.8.2b5/src/syft/serde/recursive.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/serde/recursive_primitives.py` & `syft-0.8.2b5/src/syft/serde/recursive_primitives.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/serde/serializable.py` & `syft-0.8.2b5/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/serde/signature.py` & `syft-0.8.2b5/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/serde/third_party.py` & `syft-0.8.2b5/src/syft/serde/third_party.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/action/action_data_empty.py` & `syft-0.8.2b5/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/action/action_graph.py` & `syft-0.8.2b5/src/syft/service/action/action_graph.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/action/action_graph_service.py` & `syft-0.8.2b5/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/action/action_object.py` & `syft-0.8.2b5/src/syft/service/action/action_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/action/action_permissions.py` & `syft-0.8.2b5/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/action/action_service.py` & `syft-0.8.2b5/src/syft/service/action/action_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/action/action_store.py` & `syft-0.8.2b5/src/syft/service/action/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/action/action_types.py` & `syft-0.8.2b5/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/action/numpy.py` & `syft-0.8.2b5/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/action/pandas.py` & `syft-0.8.2b5/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/action/plan.py` & `syft-0.8.2b5/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/action/verification.py` & `syft-0.8.2b5/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/code/user_code.py` & `syft-0.8.2b5/src/syft/service/code/user_code.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/code/user_code_parse.py` & `syft-0.8.2b5/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/code/user_code_service.py` & `syft-0.8.2b5/src/syft/service/code/user_code_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/code/user_code_stash.py` & `syft-0.8.2b5/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/context.py` & `syft-0.8.2b5/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/data_subject/data_subject.py` & `syft-0.8.2b5/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.2b5/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.2b5/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.2b5/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/dataset/dataset.py` & `syft-0.8.2b5/src/syft/service/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/dataset/dataset_service.py` & `syft-0.8.2b5/src/syft/service/dataset/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.2b5/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/enclave/enclave_service.py` & `syft-0.8.2b5/src/syft/service/enclave/enclave_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/metadata/node_metadata.py` & `syft-0.8.2b5/src/syft/service/metadata/node_metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     description: Optional[str]
     on_board: Optional[bool]
     id: Optional[UID]
     verify_key: Optional[SyftVerifyKey]
     highest_object_version: Optional[int]
     lowest_object_version: Optional[int]
     syft_version: Optional[str]
+    admin_email: Optional[str]
 
 
 @serializable()
 class NodeMetadata(SyftObject):
     __canonical_name__ = "NodeMetadata"
     __version__ = SYFT_OBJECT_VERSION_1
 
@@ -71,14 +72,15 @@
     syft_version: str
     node_type: NodeType = NodeType.DOMAIN
     deployed_on: str = "Date"
     organization: str = "OpenMined"
     on_board: bool = False
     description: str = "Text"
     signup_enabled: bool
+    admin_email: str
 
     def check_version(self, client_version: str) -> bool:
         return check_version(
             client_version=client_version,
             server_version=self.syft_version,
             server_name=self.name,
         )
@@ -95,14 +97,15 @@
     syft_version: str
     node_type: str = NodeType.DOMAIN.value
     deployed_on: str = "Date"
     organization: str = "OpenMined"
     on_board: bool = False
     description: str = "My cool domain"
     signup_enabled: bool
+    admin_email: str
 
     def check_version(self, client_version: str) -> bool:
         return check_version(
             client_version=client_version,
             server_version=self.syft_version,
             server_name=self.name,
         )
```

### Comparing `syft-0.8.2b4/src/syft/service/network/network_service.py` & `syft-0.8.2b5/src/syft/service/network/network_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,9 +526,9 @@
     ).as_container_host()
     return HTTPConnection(url=url, proxy_target_uid=obj.proxy_target_uid)
 
 
 @transform(NodeMetadata, NodePeer)
 def metadata_to_peer() -> List[Callable]:
     return [
-        keep(["id", "name", "verify_key", "node_type"]),
+        keep(["id", "name", "verify_key", "node_type", "admin_email"]),
     ]
```

### Comparing `syft-0.8.2b4/src/syft/service/network/node_peer.py` & `syft-0.8.2b5/src/syft/service/network/node_peer.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,24 @@
 class NodePeer(SyftObject):
     # version
     __canonical_name__ = "NodePeer"
     __version__ = SYFT_OBJECT_VERSION_1
 
     __attr_searchable__ = ["name", "node_type"]
     __attr_unique__ = ["verify_key"]
-    __repr_attrs__ = ["name", "node_type"]
+    __repr_attrs__ = ["name", "node_type", "admin_email"]
 
     id: Optional[UID]
     name: str
     verify_key: SyftVerifyKey
     is_vpn: bool = False
     vpn_auth_key: Optional[str] = None
     node_routes: List[NodeRouteType] = []
     node_type: NodeType
+    admin_email: str
 
     def update_routes(self, new_routes: List[NodeRoute]) -> None:
         add_routes = []
         existing_routes = set(self.node_routes)
         for new_route in new_routes:
             if new_route not in existing_routes:
                 add_routes.append(new_route)
```

### Comparing `syft-0.8.2b4/src/syft/service/network/routes.py` & `syft-0.8.2b5/src/syft/service/network/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/notification/notification_service.py` & `syft-0.8.2b5/src/syft/service/notification/notification_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/notification/notification_stash.py` & `syft-0.8.2b5/src/syft/service/notification/notification_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/notification/notifications.py` & `syft-0.8.2b5/src/syft/service/notification/notifications.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/policy/policy.py` & `syft-0.8.2b5/src/syft/service/policy/policy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/policy/policy_service.py` & `syft-0.8.2b5/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.2b5/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/project/project.py` & `syft-0.8.2b5/src/syft/service/project/project.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/project/project_service.py` & `syft-0.8.2b5/src/syft/service/project/project_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/project/project_stash.py` & `syft-0.8.2b5/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/queue/base_queue.py` & `syft-0.8.2b5/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/queue/queue.py` & `syft-0.8.2b5/src/syft/service/queue/queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/queue/queue_stash.py` & `syft-0.8.2b5/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/queue/zmq_queue.py` & `syft-0.8.2b5/src/syft/service/queue/zmq_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/request/request.py` & `syft-0.8.2b5/src/syft/service/request/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,27 +185,30 @@
             str_change = f"{str_change}. "
             str_changes.append(str_change)
         str_changes = "\n".join(str_changes)
         api = APIRegistry.api_for(
             self.node_uid,
             self.syft_client_verify_key,
         )
-
+        metadata = api.services.metadata.get_metadata()
+        admin_email = metadata.admin_email
+        node_name = api.node_name.capitalize() if api.node_name is not None else ""
         return f"""
             <style>
             .syft-request {{color: {SURFACE[options.color_theme]};}}
             </style>
             <div class='syft-request'>
                 <h3>Request</h3>
                 <p><strong>Id: </strong>{self.id}</p>
                 <p><strong>Request time: </strong>{self.request_time}</p>
                 {updated_at_line}
                 <p><strong>Changes: </strong> {str_changes}</p>
                 <p><strong>Status: </strong>{self.status}</p>
-                <p><strong>Sent to Domain </strong>{api.node_name}</p>
+                <p><strong>Requested on: </strong> {node_name} of type <strong> \
+                    {metadata.node_type.value.capitalize()}</strong> owned by {admin_email}</p>
             </div>
             """
 
     def _coll_repr_(self):
         if self.status == RequestStatus.APPROVED:
             badge_color = "badge-green"
         elif self.status == RequestStatus.PENDING:
```

### Comparing `syft-0.8.2b4/src/syft/service/request/request_service.py` & `syft-0.8.2b5/src/syft/service/request/request_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/request/request_stash.py` & `syft-0.8.2b5/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/response.py` & `syft-0.8.2b5/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/service.py` & `syft-0.8.2b5/src/syft/service/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/settings/settings.py` & `syft-0.8.2b5/src/syft/service/settings/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,21 +15,29 @@
 
     id: UID
     name: str
     organization: str
     description: str
     on_board: bool
     signup_enabled: bool
+    admin_email: str
 
 
 @serializable()
 class NodeSettings(SyftObject):
     __canonical_name__ = "NodeSettings"
     __version__ = SYFT_OBJECT_VERSION_1
-    __repr_attrs__ = ["name", "organization", "deployed_on", "signup_enabled"]
+    __repr_attrs__ = [
+        "name",
+        "organization",
+        "deployed_on",
+        "signup_enabled",
+        "admin_email",
+    ]
 
     name: str = "Node"
     deployed_on: str
     organization: str = "OpenMined"
     on_board: bool = True
     description: str = "Text"
     signup_enabled: bool
+    admin_email: str
```

### Comparing `syft-0.8.2b4/src/syft/service/settings/settings_service.py` & `syft-0.8.2b5/src/syft/service/settings/settings_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/settings/settings_stash.py` & `syft-0.8.2b5/src/syft/service/settings/settings_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/user/user.py` & `syft-0.8.2b5/src/syft/service/user/user.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/user/user_roles.py` & `syft-0.8.2b5/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/user/user_service.py` & `syft-0.8.2b5/src/syft/service/user/user_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from ..context import UnauthedServiceContext
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
+from ..settings.settings_stash import SettingsStash
 from .user import User
 from .user import UserCreate
 from .user import UserPrivateKey
 from .user import UserSearch
 from .user import UserUpdate
 from .user import UserView
 from .user import UserViewPage
@@ -171,14 +172,23 @@
             ]
             # Return the proper slice using page_index
             results = results[page_index]
             results = UserViewPage(users=results, total=total)
 
         return results
 
+    # @service_method(path="user.get_admin", name="get_admin", roles=GUEST_ROLE_LEVEL)
+    # def get_admin(self, context: AuthedServiceContext) -> UserView:
+    #     result = self.stash.admin_user()
+    #     if result.is_ok():
+    #         user = result.ok()
+    #         if user:
+    #             return user
+    #     return SyftError(message=str(result.err()))
+
     @service_method(
         path="user.get_current_user", name="get_current_user", roles=GUEST_ROLE_LEVEL
     )
     def get_current_user(self, context: AuthedServiceContext) -> UserView:
         result = self.stash.get_by_verify_key(
             credentials=context.credentials, verify_key=context.credentials
         )
@@ -266,14 +276,23 @@
         if result.is_err():
             error_msg = (
                 f"Failed to update user with UID: {uid}. Error: {str(result.err())}"
             )
             return SyftError(message=error_msg)
 
         user = result.ok()
+        if user.role == ServiceRole.ADMIN:
+            settings_stash = SettingsStash(store=self.store)
+            settings = settings_stash.get_all(context.credentials)
+            if settings.is_ok() and len(settings.ok()) > 0:
+                settings_data = settings.ok()[0]
+                settings_data.admin_email = user.email
+                settings_stash.update(
+                    credentials=context.credentials, settings=settings_data
+                )
 
         return user.to(UserView)
 
     def get_target_object(self, credentials: SyftVerifyKey, uid: UID):
         user_result = self.stash.get_by_uid(credentials=credentials, uid=uid)
         if user_result.is_err():
             return SyftError(message=str(user_result.err()))
```

### Comparing `syft-0.8.2b4/src/syft/service/user/user_stash.py` & `syft-0.8.2b5/src/syft/service/user/user_stash.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,14 +55,19 @@
         return super().set(
             credentials=credentials, obj=res.ok(), add_permissions=add_permissions
         )
 
     def admin_verify_key(self):
         return Ok(self.partition.root_verify_key)
 
+    def admin_user(self):
+        return self.get_by_role(
+            credentials=self.admin_verify_key().ok(), role=ServiceRole.ADMIN
+        )
+
     def get_by_uid(
         self, credentials: SyftVerifyKey, uid: UID
     ) -> Result[Optional[User], str]:
         qks = QueryKeys(qks=[UIDPartitionKey.with_obj(uid)])
         return self.query_one(credentials=credentials, qks=qks)
 
     def get_by_email(
```

### Comparing `syft-0.8.2b4/src/syft/service/vpn/headscale_client.py` & `syft-0.8.2b5/src/syft/service/vpn/headscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/vpn/tailscale_client.py` & `syft-0.8.2b5/src/syft/service/vpn/tailscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/service/vpn/vpn.py` & `syft-0.8.2b5/src/syft/service/vpn/vpn.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/store/dict_document_store.py` & `syft-0.8.2b5/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/store/document_store.py` & `syft-0.8.2b5/src/syft/store/document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/store/kv_document_store.py` & `syft-0.8.2b5/src/syft/store/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/store/linked_obj.py` & `syft-0.8.2b5/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/store/locks.py` & `syft-0.8.2b5/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/store/mongo_client.py` & `syft-0.8.2b5/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/store/mongo_codecs.py` & `syft-0.8.2b5/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/store/mongo_document_store.py` & `syft-0.8.2b5/src/syft/store/mongo_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/store/sqlite_document_store.py` & `syft-0.8.2b5/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/types/datetime.py` & `syft-0.8.2b5/src/syft/types/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/types/grid_url.py` & `syft-0.8.2b5/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/types/syft_metaclass.py` & `syft-0.8.2b5/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/types/syft_object.py` & `syft-0.8.2b5/src/syft/types/syft_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/types/transforms.py` & `syft-0.8.2b5/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/types/twin_object.py` & `syft-0.8.2b5/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/types/uid.py` & `syft-0.8.2b5/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/util/autoreload.py` & `syft-0.8.2b5/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/util/decorators.py` & `syft-0.8.2b5/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/util/experimental_flags.py` & `syft-0.8.2b5/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/util/filterwarnings.py` & `syft-0.8.2b5/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/util/fonts.py` & `syft-0.8.2b5/src/syft/util/fonts.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/util/logger.py` & `syft-0.8.2b5/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/util/markdown.py` & `syft-0.8.2b5/src/syft/util/markdown.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/util/notebook_ui/notebook_addons.py` & `syft-0.8.2b5/src/syft/util/notebook_ui/notebook_addons.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/util/schema.py` & `syft-0.8.2b5/src/syft/util/schema.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/util/telemetry.py` & `syft-0.8.2b5/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/util/trace_decorator.py` & `syft-0.8.2b5/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/util/util.py` & `syft-0.8.2b5/src/syft/util/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft/util/version_compare.py` & `syft-0.8.2b5/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b4/src/syft.egg-info/PKG-INFO` & `syft-0.8.2b5/src/syft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.2b4
+Version: 0.8.2b5
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
-Metadata-Version: 2.1 Name: syft Version: 0.8.2b4 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.2b5 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: telemetry
```

### Comparing `syft-0.8.2b4/src/syft.egg-info/SOURCES.txt` & `syft-0.8.2b5/src/syft.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 src/syft/service/data_subject/data_subject_member_service.py
 src/syft/service/data_subject/data_subject_service.py
 src/syft/service/dataset/__init__.py
 src/syft/service/dataset/dataset.py
 src/syft/service/dataset/dataset_service.py
 src/syft/service/dataset/dataset_stash.py
 src/syft/service/enclave/enclave_service.py
+src/syft/service/metadata/metadata_service.py
 src/syft/service/metadata/node_metadata.py
 src/syft/service/network/network_service.py
 src/syft/service/network/node_peer.py
 src/syft/service/network/routes.py
 src/syft/service/notification/__init__.py
 src/syft/service/notification/notification_service.py
 src/syft/service/notification/notification_stash.py
@@ -160,14 +161,15 @@
 src/syft/types/twin_object.py
 src/syft/types/uid.py
 src/syft/util/__init__.py
 src/syft/util/autoreload.py
 src/syft/util/colors.py
 src/syft/util/constants.py
 src/syft/util/decorators.py
+src/syft/util/env.py
 src/syft/util/experimental_flags.py
 src/syft/util/filterwarnings.py
 src/syft/util/fonts.py
 src/syft/util/jax_settings.py
 src/syft/util/logger.py
 src/syft/util/markdown.py
 src/syft/util/options.py
```

### Comparing `syft-0.8.2b4/src/syft.egg-info/requires.txt` & `syft-0.8.2b5/src/syft.egg-info/requires.txt`

 * *Files identical despite different names*

