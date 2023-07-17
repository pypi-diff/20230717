# Comparing `tmp/skypilot-nightly-1.0.0.dev20230715.tar.gz` & `tmp/skypilot-nightly-1.0.0.dev20230716.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot-nightly-1.0.0.dev20230715.tar", last modified: Sat Jul 15 10:40:53 2023, max compression
+gzip compressed data, was "skypilot-nightly-1.0.0.dev20230716.tar", last modified: Sun Jul 16 10:40:58 2023, max compression
```

## Comparing `skypilot-nightly-1.0.0.dev20230715.tar` & `skypilot-nightly-1.0.0.dev20230716.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.067319 skypilot-nightly-1.0.0.dev20230715/
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-15 10:40:53.067319 skypilot-nightly-1.0.0.dev20230715/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 10:40:53.067319 skypilot-nightly-1.0.0.dev20230715/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-15 10:40:45.000000 skypilot-nightly-1.0.0.dev20230715/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.047319 skypilot-nightly-1.0.0.dev20230715/sky/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-15 10:40:45.000000 skypilot-nightly-1.0.0.dev20230715/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.047319 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.047319 skypilot-nightly-1.0.0.dev20230715/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)   112833 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   200283 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.047319 skypilot-nightly-1.0.0.dev20230715/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/onprem_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.047319 skypilot-nightly-1.0.0.dev20230715/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (123)   167453 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.051319 skypilot-nightly-1.0.0.dev20230715/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41057 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    25706 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    42681 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19980 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    14724 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.051319 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    23188 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.051319 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    18969 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.051319 skypilot-nightly-1.0.0.dev20230715/sky/data/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    89247 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.051319 skypilot-nightly-1.0.0.dev20230715/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.055318 skypilot-nightly-1.0.0.dev20230715/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/provision/aws/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.055318 skypilot-nightly-1.0.0.dev20230715/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.055318 skypilot-nightly-1.0.0.dev20230715/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-15 10:40:45.000000 skypilot-nightly-1.0.0.dev20230715/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.055318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/log_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.043318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.055318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.055318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.055318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.055318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/lambda_cloud/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/scp/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/scp/scp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/job_head.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skypilot_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/spot/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/spot_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/spot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.063319 skypilot-nightly-1.0.0.dev20230715/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/gcp-tpu-create.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/gcp-tpu-delete.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/spot-controller.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.063319 skypilot-nightly-1.0.0.dev20230715/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.063319 skypilot-nightly-1.0.0.dev20230715/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.063319 skypilot-nightly-1.0.0.dev20230715/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/env_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/tpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.067319 skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-15 10:40:53.000000 skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-15 10:40:53.000000 skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 10:40:53.000000 skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-15 10:40:53.000000 skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-15 10:40:53.000000 skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-15 10:40:53.000000 skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.067319 skypilot-nightly-1.0.0.dev20230715/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_onprem.py
--rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_pycryptodome_version.py
--rw-r--r--   0 runner    (1001) docker     (123)   123678 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_wheels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.280852 skypilot-nightly-1.0.0.dev20230716/
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-16 10:40:58.280852 skypilot-nightly-1.0.0.dev20230716/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 10:40:58.280852 skypilot-nightly-1.0.0.dev20230716/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-16 10:40:49.000000 skypilot-nightly-1.0.0.dev20230716/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.252852 skypilot-nightly-1.0.0.dev20230716/sky/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-16 10:40:49.000000 skypilot-nightly-1.0.0.dev20230716/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.252852 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.256852 skypilot-nightly-1.0.0.dev20230716/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112970 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   200283 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.256852 skypilot-nightly-1.0.0.dev20230716/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/onprem_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.256852 skypilot-nightly-1.0.0.dev20230716/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167453 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.256852 skypilot-nightly-1.0.0.dev20230716/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41057 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25706 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42681 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19980 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14724 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.260852 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23188 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.260852 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18969 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.260852 skypilot-nightly-1.0.0.dev20230716/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89247 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.260852 skypilot-nightly-1.0.0.dev20230716/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.260852 skypilot-nightly-1.0.0.dev20230716/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/provision/aws/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.260852 skypilot-nightly-1.0.0.dev20230716/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.260852 skypilot-nightly-1.0.0.dev20230716/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-16 10:40:49.000000 skypilot-nightly-1.0.0.dev20230716/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.264852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/log_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.244852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.264852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.264852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.264852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.264852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.268852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.268852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/lambda_cloud/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.268852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.268852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/scp/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/scp/scp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.268852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/job_head.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skypilot_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.272852 skypilot-nightly-1.0.0.dev20230716/sky/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.272852 skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.272852 skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.272852 skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/spot_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/spot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.272852 skypilot-nightly-1.0.0.dev20230716/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/gcp-tpu-create.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/gcp-tpu-delete.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/spot-controller.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.272852 skypilot-nightly-1.0.0.dev20230716/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.276852 skypilot-nightly-1.0.0.dev20230716/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.276852 skypilot-nightly-1.0.0.dev20230716/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/env_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/tpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.276852 skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-16 10:40:58.000000 skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-16 10:40:58.000000 skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 10:40:58.000000 skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-16 10:40:58.000000 skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-16 10:40:58.000000 skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-16 10:40:58.000000 skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.280852 skypilot-nightly-1.0.0.dev20230716/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_onprem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_pycryptodome_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124066 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_wheels.py
```

### Comparing `skypilot-nightly-1.0.0.dev20230715/LICENSE` & `skypilot-nightly-1.0.0.dev20230716/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230716/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230716/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230715
+Version: 1.0.0.dev20230716
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230715
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230716
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230715/README.md` & `skypilot-nightly-1.0.0.dev20230716/README.md`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/pyproject.toml` & `skypilot-nightly-1.0.0.dev20230716/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/setup.py` & `skypilot-nightly-1.0.0.dev20230716/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/__init__.py` & `skypilot-nightly-1.0.0.dev20230716/sky/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The SkyPilot package."""
 import os
 
 # Replaced with the current commit when building the wheels.
-__commit__ = 'e924e44a4a2a0bf8dae2953f3cf3c05e4bdb5f76'
-__version__ = '1.0.0-dev20230715'
+__commit__ = '95fdb5b21a87bb3a592bc7178cb508f183daa84e'
+__version__ = '1.0.0-dev20230716'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 # Keep this order to avoid cyclic imports
 from sky import backends
 from sky import benchmark
 from sky import clouds
 from sky.clouds.service_catalog import list_accelerators
```

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/adaptors/aws.py` & `skypilot-nightly-1.0.0.dev20230716/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/adaptors/azure.py` & `skypilot-nightly-1.0.0.dev20230716/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/adaptors/cloudflare.py` & `skypilot-nightly-1.0.0.dev20230716/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/adaptors/docker.py` & `skypilot-nightly-1.0.0.dev20230716/sky/adaptors/docker.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/adaptors/gcp.py` & `skypilot-nightly-1.0.0.dev20230716/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/adaptors/ibm.py` & `skypilot-nightly-1.0.0.dev20230716/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/adaptors/oci.py` & `skypilot-nightly-1.0.0.dev20230716/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/authentication.py` & `skypilot-nightly-1.0.0.dev20230716/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/backends/backend.py` & `skypilot-nightly-1.0.0.dev20230716/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/backends/backend_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/backends/backend_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -934,14 +934,18 @@
                 # Azure only:
                 'azure_subscription_id': azure_subscription_id,
                 'resource_group': f'{cluster_name}-{region_name}',
 
                 # GCP only:
                 'gcp_project_id': gcp_project_id,
 
+                # Conda setup
+                'conda_installation_commands':
+                    constants.CONDA_INSTALLATION_COMMANDS,
+
                 # Port of Ray (GCS server).
                 # Ray's default port 6379 is conflicted with Redis.
                 'ray_port': constants.SKY_REMOTE_RAY_PORT,
                 'ray_dashboard_port': constants.SKY_REMOTE_RAY_DASHBOARD_PORT,
                 'ray_temp_dir': constants.SKY_REMOTE_RAY_TEMPDIR,
                 'dump_port_command': dump_port_command,
                 # Ray version.
```

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/backends/cloud_vm_ray_backend.py` & `skypilot-nightly-1.0.0.dev20230716/sky/backends/cloud_vm_ray_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/backends/docker_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/backends/local_docker_backend.py` & `skypilot-nightly-1.0.0.dev20230716/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot-nightly-1.0.0.dev20230716/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/backends/onprem_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/backends/onprem_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/backends/wheel_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/benchmark/benchmark_state.py` & `skypilot-nightly-1.0.0.dev20230716/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/benchmark/benchmark_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/check.py` & `skypilot-nightly-1.0.0.dev20230716/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/cli.py` & `skypilot-nightly-1.0.0.dev20230716/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/cloud_stores.py` & `skypilot-nightly-1.0.0.dev20230716/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/__init__.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/aws.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/azure.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/cloud.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/gcp.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/ibm.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/local.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/local.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/oci.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/scp.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/__init__.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/aws_catalog.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/azure_catalog.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/common.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/config.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/oci_catalog.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/scp_catalog.py` & `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/core.py` & `skypilot-nightly-1.0.0.dev20230716/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/dag.py` & `skypilot-nightly-1.0.0.dev20230716/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/data/data_transfer.py` & `skypilot-nightly-1.0.0.dev20230716/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/data/data_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/data/mounting_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/data/storage.py` & `skypilot-nightly-1.0.0.dev20230716/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/data/storage_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/exceptions.py` & `skypilot-nightly-1.0.0.dev20230716/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/execution.py` & `skypilot-nightly-1.0.0.dev20230716/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/global_user_state.py` & `skypilot-nightly-1.0.0.dev20230716/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/optimizer.py` & `skypilot-nightly-1.0.0.dev20230716/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/provision/__init__.py` & `skypilot-nightly-1.0.0.dev20230716/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/provision/aws/instance.py` & `skypilot-nightly-1.0.0.dev20230716/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/provision/gcp/instance.py` & `skypilot-nightly-1.0.0.dev20230716/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/provision/gcp/instance_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/resources.py` & `skypilot-nightly-1.0.0.dev20230716/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/setup_files/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230716/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/setup_files/setup.py` & `skypilot-nightly-1.0.0.dev20230716/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/sky_logging.py` & `skypilot-nightly-1.0.0.dev20230716/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/LICENSE` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/attempt_skylet.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/autostop_lib.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/configs.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/constants.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/constants.py`

 * *Files 17% similar despite different names*

```diff
@@ -42,7 +42,18 @@
 SKYLET_VERSION = '2'
 SKYLET_VERSION_FILE = '~/.sky/skylet_version'
 
 # `sky spot dashboard`-related
 #
 # Port on the remote spot controller that the dashboard is running on.
 SPOT_DASHBOARD_REMOTE_PORT = 5000
+
+# Install conda on the remote cluster if it is not already installed.
+# We do not install the latest conda with python 3.11 because ray has not
+# officially supported it yet.
+# https://github.com/ray-project/ray/issues/31606
+CONDA_INSTALLATION_COMMANDS = (
+    '(which conda > /dev/null 2>&1 && conda init > /dev/null) || '
+    '(wget -nc https://repo.anaconda.com/miniconda/Miniconda3-py39_23.5.2-0-Linux-x86_64.sh -O Miniconda3-Linux-x86_64.sh && '  # pylint: disable=line-too-long
+    'bash Miniconda3-Linux-x86_64.sh -b && '
+    'eval "$(~/miniconda3/bin/conda shell.bash hook)" && conda init && '
+    'conda config --set auto_activate_base true);')
```

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/events.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/job_lib.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/log_lib.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/config.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/node_provider.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/azure-config-template.json` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/config.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/node_provider.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/config.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/constants.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/node.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/node.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/ibm/node_provider.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/ibm/utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/lambda_cloud/lambda_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/lambda_cloud/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/config.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/node_provider.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/query_helper.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/scp/config.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/scp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/scp/scp_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/scp/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/__init__.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/worker.py.patch` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/skylet.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skylet/subprocess_daemon.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/skypilot_config.py` & `skypilot-nightly-1.0.0.dev20230716/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/spot/__init__.py` & `skypilot-nightly-1.0.0.dev20230716/sky/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/spot/constants.py` & `skypilot-nightly-1.0.0.dev20230716/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/spot/controller.py` & `skypilot-nightly-1.0.0.dev20230716/sky/spot/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/dashboard.py` & `skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/static/favicon.ico` & `skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/templates/index.html` & `skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/spot/recovery_strategy.py` & `skypilot-nightly-1.0.0.dev20230716/sky/spot/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/spot/spot_state.py` & `skypilot-nightly-1.0.0.dev20230716/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/spot/spot_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/spot/spot_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/status_lib.py` & `skypilot-nightly-1.0.0.dev20230716/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/task.py` & `skypilot-nightly-1.0.0.dev20230716/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/templates/aws-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230716/sky/templates/aws-ray.yml.j2`

 * *Files 5% similar despite different names*

```diff
@@ -186,15 +186,15 @@
   # Line 'sudo grep ..': set the number of threads per process to unlimited to avoid ray job submit stucking issue when the number of running ray jobs increase.
   # Line 'mkdir -p ..': disable host key check
   # Line 'python3 -c ..': patch the buggy ray files and enable `-o allow_other` option for `goofys`
   - mkdir -p ~/.ssh; touch ~/.ssh/config;
     pip3 --version > /dev/null 2>&1 || (curl -sSL https://bootstrap.pypa.io/get-pip.py -o get-pip.py && python3 get-pip.py && echo "PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc);
     (type -a python | grep -q python3) || echo 'alias python=python3' >> ~/.bashrc;
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
-    (which conda > /dev/null 2>&1 && conda init > /dev/null) || (wget -nc https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh && bash Miniconda3-latest-Linux-x86_64.sh -b && eval "$(~/miniconda3/bin/conda shell.bash hook)" && conda init && conda config --set auto_activate_base true);
+    {{ conda_installation_commands }}
     source ~/.bashrc;
     (pip3 list | grep "ray " | grep {{ray_version}} 2>&1 > /dev/null || pip3 install --exists-action w -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app;
     (pip3 list | grep "skypilot " && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[aws]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
     sudo bash -c 'rm -rf /etc/security/limits.d; echo "* soft nofile 1048576" >> /etc/security/limits.conf; echo "* hard nofile 1048576" >> /etc/security/limits.conf';
     sudo grep -e '^DefaultTasksMax' /etc/systemd/system.conf || (sudo bash -c 'echo "DefaultTasksMax=infinity" >> /etc/systemd/system.conf'); sudo systemctl set-property user-$(id -u $(whoami)).slice TasksMax=infinity; sudo systemctl daemon-reload;
     mkdir -p ~/.ssh; (grep -Pzo -q "Host \*\n  StrictHostKeyChecking no" ~/.ssh/config) || printf "Host *\n  StrictHostKeyChecking no\n" >> ~/.ssh/config;
     python3 -c "from sky.skylet.ray_patches import patch; patch()" || exit 1;
```

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/templates/azure-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230716/sky/templates/azure-ray.yml.j2`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     sudo pkill -9 dpkg;
     sudo pkill -9 apt-get;
     sudo dpkg --configure --force-overwrite -a;
     mkdir -p ~/.ssh; touch ~/.ssh/config;
     pip3 --version > /dev/null 2>&1 || (curl -sSL https://bootstrap.pypa.io/get-pip.py -o get-pip.py && python3 get-pip.py && echo "PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc);
     (type -a python | grep -q python3) || echo 'alias python=python3' >> ~/.bashrc;
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
-    which conda > /dev/null 2>&1 || (wget -nc https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh && bash Miniconda3-latest-Linux-x86_64.sh -b && eval "$(/home/azureuser/miniconda3/bin/conda shell.bash hook)" && conda init && conda config --set auto_activate_base true);
+    {{ conda_installation_commands }}
     source ~/.bashrc;
     (pip3 list | grep "ray " | grep {{ray_version}} 2>&1 > /dev/null || pip3 install --exists-action w -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app && touch ~/.sudo_as_admin_successful;
     (pip3 list | grep "skypilot " && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[azure]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
     sudo bash -c 'rm -rf /etc/security/limits.d; echo "* soft nofile 1048576" >> /etc/security/limits.conf; echo "* hard nofile 1048576" >> /etc/security/limits.conf';
     sudo grep -e '^DefaultTasksMax' /etc/systemd/system.conf || (sudo bash -c 'echo "DefaultTasksMax=infinity" >> /etc/systemd/system.conf'); sudo systemctl set-property user-$(id -u $(whoami)).slice TasksMax=infinity; sudo systemctl daemon-reload;
     mkdir -p ~/.ssh; (grep -Pzo -q "Host \*\n  StrictHostKeyChecking no" ~/.ssh/config) || printf "Host *\n  StrictHostKeyChecking no\n" >> ~/.ssh/config;
     python3 -c "from sky.skylet.ray_patches import patch; patch()" || exit 1;
```

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/templates/gcp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230716/sky/templates/gcp-ray.yml.j2`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     sudo pkill -9 dpkg;
     sudo pkill -9 apt-get;
     sudo dpkg --configure --force-overwrite -a;
     mkdir -p ~/.ssh; touch ~/.ssh/config;
     pip3 --version > /dev/null 2>&1 || (curl -sSL https://bootstrap.pypa.io/get-pip.py -o get-pip.py && python3 get-pip.py && echo "PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc);
     (type -a python | grep -q python3) || echo 'alias python=python3' >> ~/.bashrc;
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
-    which conda > /dev/null 2>&1 || (wget -nc https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh && bash Miniconda3-latest-Linux-x86_64.sh -b && eval "$(/home/gcpuser/miniconda3/bin/conda shell.bash hook)" && conda init && conda config --set auto_activate_base true);
+    {{ conda_installation_commands }}
     source ~/.bashrc;
   {%- if tpu_vm %}
     test -f /home/gcpuser/miniconda3/etc/profile.d/conda.sh && source /home/gcpuser/miniconda3/etc/profile.d/conda.sh && conda activate base || true;
     pip3 install --upgrade google-api-python-client;
   {%- endif %}
     (pip3 list | grep "ray " | grep {{ray_version}} 2>&1 > /dev/null || pip3 install --exists-action w -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app;
     (pip3 list | grep "skypilot " && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[gcp]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
```

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/templates/ibm-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230716/sky/templates/ibm-ray.yml.j2`

 * *Files 8% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     sudo pkill -9 apt-get;
     sudo pkill -9 dpkg;
     sudo dpkg --configure -a;
     mkdir -p ~/.ssh; touch ~/.ssh/config;
     pip3 --version > /dev/null 2>&1 || (curl -sSL https://bootstrap.pypa.io/get-pip.py -o get-pip.py && python3 get-pip.py && echo "PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc);
     (type -a python | grep -q python3) || echo 'alias python=python3' >> ~/.bashrc;
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
-    (which conda > /dev/null 2>&1 && conda init > /dev/null && conda config --set auto_activate_base false) || (wget -nc https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh && bash Miniconda3-latest-Linux-x86_64.sh -b && eval "$(~/miniconda3/bin/conda shell.bash hook)" && conda init && conda config --set auto_activate_base true);
+    {{ conda_installation_commands }}
     source ~/.bashrc;
     (pip3 list | grep ray | grep {{ray_version}} 2>&1 > /dev/null || pip3 install -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app;
     (pip3 list | grep skypilot && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[ibm]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
     sudo bash -c 'rm -rf /etc/security/limits.d; echo "* soft nofile 1048576" >> /etc/security/limits.conf; echo "* hard nofile 1048576" >> /etc/security/limits.conf';
     sudo grep -e '^DefaultTasksMax' /etc/systemd/system.conf || (sudo bash -c 'echo "DefaultTasksMax=infinity" >> /etc/systemd/system.conf'); sudo systemctl set-property user-$(id -u $(whoami)).slice TasksMax=infinity; sudo systemctl daemon-reload;
     mkdir -p ~/.ssh; (grep -Pzo -q "Host \*\n  StrictHostKeyChecking no" ~/.ssh/config) || printf "Host *\n  StrictHostKeyChecking no\n" >> ~/.ssh/config;
     python3 -c "from sky.skylet.ray_patches import patch; patch()" || exit 1;
```

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/templates/lambda-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230716/sky/templates/lambda-ray.yml.j2`

 * *Files 3% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     sudo pkill -9 apt-get;
     sudo pkill -9 dpkg;
     sudo dpkg --configure -a;
     mkdir -p ~/.ssh; touch ~/.ssh/config;
     rm ~/.local/bin/pip ~/.local/bin/pip3 ~/.local/bin/pip3.8 ~/.local/bin/pip3.10;
     (type -a python | grep -q python3) || echo 'alias python=python3' >> ~/.bashrc;
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
-    which conda > /dev/null 2>&1 || (wget -nc https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh && bash Miniconda3-latest-Linux-x86_64.sh -b && eval "$(~/miniconda3/bin/conda shell.bash hook)" && conda init && conda config --set auto_activate_base true);
+    {{ conda_installation_commands }}
     source ~/.bashrc;
     (pip3 list | grep "ray " | grep {{ray_version}} 2>&1 > /dev/null || pip3 install --exists-action w -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app && touch ~/.sudo_as_admin_successful;
     (pip3 list | grep "skypilot " && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[lambda]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
     sudo bash -c 'rm -rf /etc/security/limits.d; echo "* soft nofile 1048576" >> /etc/security/limits.conf; echo "* hard nofile 1048576" >> /etc/security/limits.conf';
     sudo grep -e '^DefaultTasksMax' /etc/systemd/system.conf || (sudo bash -c 'echo "DefaultTasksMax=infinity" >> /etc/systemd/system.conf'); sudo systemctl set-property user-$(id -u $(whoami)).slice TasksMax=infinity; sudo systemctl daemon-reload;
     mkdir -p ~/.ssh; (grep -Pzo -q "Host \*\n  StrictHostKeyChecking no" ~/.ssh/config) || printf "Host *\n  StrictHostKeyChecking no\n" >> ~/.ssh/config;
     python3 -c "from sky.skylet.ray_patches import patch; patch()" || exit 1;
```

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/templates/local-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230716/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/templates/oci-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230716/sky/templates/oci-ray.yml.j2`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     sudo pkill -9 dpkg;
     sudo dpkg --configure -a;
     ([ `sudo lshw -class display | grep "NVIDIA Corporation" | wc -l` -gt 0 ]) && (sudo which nvidia-smi > /dev/null || ( sudo apt-get install nvidia-driver-530-open -y && sudo apt-get install nvidia-driver-525-server -y ) || true);
     mkdir -p ~/.ssh; touch ~/.ssh/config;
     pip3 --version > /dev/null 2>&1 || (curl -sSL https://bootstrap.pypa.io/get-pip.py -o get-pip.py && python3 get-pip.py && echo "PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc);
     (type -a python | grep -q python3) || echo 'alias python=python3' >> ~/.bashrc;
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
-    which conda > /dev/null 2>&1 || (wget -nc https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh && bash Miniconda3-latest-Linux-x86_64.sh -b && eval "$(~/miniconda3/bin/conda shell.bash hook)" && conda init && conda config --set auto_activate_base true);
+    {{ conda_installation_commands }}
     source ~/.bashrc;
     pip3 install oci;
     (pip3 list | grep ray | grep {{ray_version}} 2>&1 > /dev/null || pip3 install -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app && touch ~/.sudo_as_admin_successful;
     (pip3 list | grep skypilot && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
     sudo bash -c 'rm -rf /etc/security/limits.d; echo "* soft nofile 1048576" >> /etc/security/limits.conf; echo "* hard nofile 1048576" >> /etc/security/limits.conf';
     sudo grep -e '^DefaultTasksMax' /etc/systemd/system.conf || (sudo bash -c 'echo "DefaultTasksMax=infinity" >> /etc/systemd/system.conf'); sudo systemctl set-property user-$(id -u $(whoami)).slice TasksMax=infinity; sudo systemctl daemon-reload;
     mkdir -p ~/.ssh; (grep -Pzo -q "Host \*\n  StrictHostKeyChecking no" ~/.ssh/config) || printf "Host *\n  StrictHostKeyChecking no\n" >> ~/.ssh/config;
```

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/templates/scp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230716/sky/templates/scp-ray.yml.j2`

 * *Files 10% similar despite different names*

```diff
@@ -70,15 +70,15 @@
   # Line 'sudo grep ..': set the number of threads per process to unlimited to avoid ray job submit stucking issue when the number of running ray jobs increase.
   # Line 'mkdir -p ..': disable host key check
   # Line 'python3 -c ..': patch the buggy ray files and enable `-o allow_other` option for `goofys`
   - mkdir -p ~/.ssh; touch ~/.ssh/config;
     pip3 --version > /dev/null 2>&1 || (curl -sSL https://bootstrap.pypa.io/get-pip.py -o get-pip.py && python3 get-pip.py && echo "PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc);
     (type -a python | grep -q python3) || echo 'alias python=python3' >> ~/.bashrc;
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
-    (which conda > /dev/null 2>&1 && conda init > /dev/null) || (wget -nc https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh && bash Miniconda3-latest-Linux-x86_64.sh -b && eval "$(~/miniconda3/bin/conda shell.bash hook)" && conda init && conda config --set auto_activate_base true);
+    {{ conda_installation_commands }}
     source ~/.bashrc;
     (pip3 list | grep "ray " | grep {{ray_version}} 2>&1 > /dev/null || pip3 install --exists-action w -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app;
     (pip3 list | grep "skypilot " && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[scp]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
     sudo bash -c 'rm -rf /etc/security/limits.d; echo "* soft nofile 1048576" >> /etc/security/limits.conf; echo "* hard nofile 1048576" >> /etc/security/limits.conf';
     sudo grep -e '^DefaultTasksMax' /etc/systemd/system.conf || (sudo bash -c 'echo "DefaultTasksMax=infinity" >> /etc/systemd/system.conf'); sudo systemctl set-property user-$(id -u $(whoami)).slice TasksMax=infinity; sudo systemctl daemon-reload;
     mkdir -p ~/.ssh; (grep -Pzo -q "Host \*\n  StrictHostKeyChecking no" ~/.ssh/config) || printf "Host *\n  StrictHostKeyChecking no\n" >> ~/.ssh/config;
     python3 -c "from sky.skylet.ray_patches import patch; patch()" || exit 1;
```

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/templates/spot-controller.yaml.j2` & `skypilot-nightly-1.0.0.dev20230716/sky/templates/spot-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/usage/constants.py` & `skypilot-nightly-1.0.0.dev20230716/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/usage/usage_lib.py` & `skypilot-nightly-1.0.0.dev20230716/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/utils/accelerator_registry.py` & `skypilot-nightly-1.0.0.dev20230716/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/utils/cli_utils/status_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/utils/command_runner.py` & `skypilot-nightly-1.0.0.dev20230716/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/utils/common_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/utils/dag_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/utils/db_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/utils/env_options.py` & `skypilot-nightly-1.0.0.dev20230716/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/utils/log_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/utils/schemas.py` & `skypilot-nightly-1.0.0.dev20230716/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/utils/subprocess_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/utils/timeline.py` & `skypilot-nightly-1.0.0.dev20230716/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/utils/tpu_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/utils/tpu_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/utils/ux_utils.py` & `skypilot-nightly-1.0.0.dev20230716/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/sky/utils/validator.py` & `skypilot-nightly-1.0.0.dev20230716/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230715
+Version: 1.0.0.dev20230716
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230715
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230716
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/requires.txt` & `skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/tests/test_cli.py` & `skypilot-nightly-1.0.0.dev20230716/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/tests/test_config.py` & `skypilot-nightly-1.0.0.dev20230716/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/tests/test_jobs.py` & `skypilot-nightly-1.0.0.dev20230716/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/tests/test_list_accelerators.py` & `skypilot-nightly-1.0.0.dev20230716/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/tests/test_onprem.py` & `skypilot-nightly-1.0.0.dev20230716/tests/test_onprem.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/tests/test_optimizer_dryruns.py` & `skypilot-nightly-1.0.0.dev20230716/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/tests/test_optimizer_random_dag.py` & `skypilot-nightly-1.0.0.dev20230716/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/tests/test_smoke.py` & `skypilot-nightly-1.0.0.dev20230716/tests/test_smoke.py`

 * *Files 1% similar despite different names*

```diff
@@ -3187,4544 +3187,4569 @@
 0000c720: 2023 2049 424d 2063 6c6f 7564 2063 7572   # IBM cloud cur
 0000c730: 7265 6e74 6c79 2064 6f65 736e 2774 2070  rently doesn't p
 0000c740: 726f 7669 6465 2070 7562 6c69 6320 696d  rovide public im
 0000c750: 6167 6520 7769 7468 2043 5544 410a 4070  age with CUDA.@p
 0000c760: 7974 6573 742e 6d61 726b 2e6e 6f5f 7363  ytest.mark.no_sc
 0000c770: 7020 2023 2053 4350 2064 6f65 7320 6e6f  p  # SCP does no
 0000c780: 7420 7375 7070 6f72 7420 6e75 6d5f 6e6f  t support num_no
-0000c790: 6465 7320 3e20 3120 7965 740a 6465 6620  des > 1 yet.def 
-0000c7a0: 7465 7374 5f64 6973 7472 6962 7574 6564  test_distributed
-0000c7b0: 5f74 6628 6765 6e65 7269 635f 636c 6f75  _tf(generic_clou
-0000c7c0: 643a 2073 7472 293a 0a20 2020 206e 616d  d: str):.    nam
-0000c7d0: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
-0000c7e0: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
-0000c7f0: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
-0000c800: 2027 7265 736e 6574 5f64 6973 7472 6962   'resnet_distrib
-0000c810: 7574 6564 5f74 665f 6170 7027 2c0a 2020  uted_tf_app',.  
-0000c820: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-0000c830: 2020 2020 2320 4e4f 5445 3a20 7275 6e6e      # NOTE: runn
-0000c840: 696e 6720 6974 2074 7769 6365 2077 696c  ing it twice wil
-0000c850: 6c20 6861 6e67 2028 736f 6d65 7469 6d65  l hang (sometime
-0000c860: 733f 2920 2d20 616e 2061 7070 2d6c 6576  s?) - an app-lev
-0000c870: 656c 2062 7567 2e0a 2020 2020 2020 2020  el bug..        
-0000c880: 2020 2020 6627 7079 7468 6f6e 2065 7861      f'python exa
-0000c890: 6d70 6c65 732f 7265 736e 6574 5f64 6973  mples/resnet_dis
-0000c8a0: 7472 6962 7574 6564 5f74 665f 6170 702e  tributed_tf_app.
-0000c8b0: 7079 207b 6e61 6d65 7d20 7b67 656e 6572  py {name} {gener
-0000c8c0: 6963 5f63 6c6f 7564 7d27 2c0a 2020 2020  ic_cloud}',.    
-0000c8d0: 2020 2020 2020 2020 6627 736b 7920 6c6f          f'sky lo
-0000c8e0: 6773 207b 6e61 6d65 7d20 3120 2d2d 7374  gs {name} 1 --st
-0000c8f0: 6174 7573 272c 2020 2320 456e 7375 7265  atus',  # Ensure
-0000c900: 2074 6865 206a 6f62 2073 7563 6365 6564   the job succeed
-0000c910: 6564 2e0a 2020 2020 2020 2020 5d2c 0a20  ed..        ],. 
-0000c920: 2020 2020 2020 2066 2773 6b79 2064 6f77         f'sky dow
-0000c930: 6e20 2d79 207b 6e61 6d65 7d27 2c0a 2020  n -y {name}',.  
-0000c940: 2020 2020 2020 7469 6d65 6f75 743d 3235        timeout=25
-0000c950: 202a 2036 302c 2020 2320 3235 206d 696e   * 60,  # 25 min
-0000c960: 7320 2869 7420 7461 6b65 7320 6172 6f75  s (it takes arou
-0000c970: 6e64 207e 3139 206d 696e 7329 0a20 2020  nd ~19 mins).   
-0000c980: 2029 0a20 2020 2072 756e 5f6f 6e65 5f74   ).    run_one_t
-0000c990: 6573 7428 7465 7374 290a 0a0a 2320 2d2d  est(test)...# --
-0000c9a0: 2d2d 2d2d 2d2d 2d2d 2054 6573 7469 6e67  -------- Testing
-0000c9b0: 2047 4350 2073 7461 7274 2061 6e64 2073   GCP start and s
-0000c9c0: 746f 7020 696e 7374 616e 6365 7320 2d2d  top instances --
-0000c9d0: 2d2d 2d2d 2d2d 2d2d 0a40 7079 7465 7374  --------.@pytest
-0000c9e0: 2e6d 6172 6b2e 6763 700a 6465 6620 7465  .mark.gcp.def te
-0000c9f0: 7374 5f67 6370 5f73 7461 7274 5f73 746f  st_gcp_start_sto
-0000ca00: 7028 293a 0a20 2020 206e 616d 6520 3d20  p():.    name = 
-0000ca10: 5f67 6574 5f63 6c75 7374 6572 5f6e 616d  _get_cluster_nam
-0000ca20: 6528 290a 2020 2020 7465 7374 203d 2054  e().    test = T
-0000ca30: 6573 7428 0a20 2020 2020 2020 2027 6763  est(.        'gc
-0000ca40: 702d 7374 6172 742d 7374 6f70 272c 0a20  p-start-stop',. 
-0000ca50: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-0000ca60: 2020 2020 2066 2773 6b79 206c 6175 6e63       f'sky launc
-0000ca70: 6820 2d79 202d 6320 7b6e 616d 657d 2065  h -y -c {name} e
-0000ca80: 7861 6d70 6c65 732f 6763 705f 7374 6172  xamples/gcp_star
-0000ca90: 745f 7374 6f70 2e79 616d 6c27 2c0a 2020  t_stop.yaml',.  
-0000caa0: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
-0000cab0: 6c6f 6773 207b 6e61 6d65 7d20 3120 2d2d  logs {name} 1 --
-0000cac0: 7374 6174 7573 272c 2020 2320 456e 7375  status',  # Ensu
-0000cad0: 7265 2074 6865 206a 6f62 2073 7563 6365  re the job succe
-0000cae0: 6564 6564 2e0a 2020 2020 2020 2020 2020  eded..          
-0000caf0: 2020 6627 736b 7920 6578 6563 207b 6e61    f'sky exec {na
-0000cb00: 6d65 7d20 6578 616d 706c 6573 2f67 6370  me} examples/gcp
-0000cb10: 5f73 7461 7274 5f73 746f 702e 7961 6d6c  _start_stop.yaml
-0000cb20: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-0000cb30: 2773 6b79 206c 6f67 7320 7b6e 616d 657d  'sky logs {name}
-0000cb40: 2032 202d 2d73 7461 7475 7327 2c20 2023   2 --status',  #
-0000cb50: 2045 6e73 7572 6520 7468 6520 6a6f 6220   Ensure the job 
-0000cb60: 7375 6363 6565 6465 642e 0a20 2020 2020  succeeded..     
-0000cb70: 2020 2020 2020 2066 2773 6b79 2065 7865         f'sky exe
-0000cb80: 6320 7b6e 616d 657d 2022 7072 6c69 6d69  c {name} "prlimi
-0000cb90: 7420 2d6e 202d 2d70 6964 3d5c 2428 7067  t -n --pid=\$(pg
-0000cba0: 7265 7020 2d66 205c 2772 6179 6c65 742f  rep -f \'raylet/
-0000cbb0: 7261 796c 6574 202d 2d72 6179 6c65 745f  raylet --raylet_
-0000cbc0: 736f 636b 6574 5f6e 616d 655c 2729 207c  socket_name\') |
-0000cbd0: 2067 7265 7020 5c27 225c 2731 3034 3835   grep \'"\'10485
-0000cbe0: 3736 2031 3034 3835 3736 5c27 225c 2722  76 1048576\'"\'"
-0000cbf0: 272c 2020 2320 456e 7375 7265 2074 6865  ',  # Ensure the
-0000cc00: 2072 6179 6c65 7420 7072 6f63 6573 7320   raylet process 
-0000cc10: 6861 7320 7468 6520 636f 7272 6563 7420  has the correct 
-0000cc20: 6669 6c65 2064 6573 6372 6970 746f 7220  file descriptor 
-0000cc30: 6c69 6d69 742e 0a20 2020 2020 2020 2020  limit..         
-0000cc40: 2020 2066 2773 6b79 206c 6f67 7320 7b6e     f'sky logs {n
-0000cc50: 616d 657d 2033 202d 2d73 7461 7475 7327  ame} 3 --status'
-0000cc60: 2c20 2023 2045 6e73 7572 6520 7468 6520  ,  # Ensure the 
-0000cc70: 6a6f 6220 7375 6363 6565 6465 642e 0a20  job succeeded.. 
-0000cc80: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-0000cc90: 2073 746f 7020 2d79 207b 6e61 6d65 7d27   stop -y {name}'
-0000cca0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-0000ccb0: 736c 6565 7020 3230 272c 0a20 2020 2020  sleep 20',.     
-0000ccc0: 2020 2020 2020 2066 2773 6b79 2073 7461         f'sky sta
-0000ccd0: 7274 202d 7920 7b6e 616d 657d 202d 6920  rt -y {name} -i 
-0000cce0: 3127 2c0a 2020 2020 2020 2020 2020 2020  1',.            
-0000ccf0: 6627 736b 7920 6578 6563 207b 6e61 6d65  f'sky exec {name
-0000cd00: 7d20 6578 616d 706c 6573 2f67 6370 5f73  } examples/gcp_s
-0000cd10: 7461 7274 5f73 746f 702e 7961 6d6c 272c  tart_stop.yaml',
-0000cd20: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-0000cd30: 6b79 206c 6f67 7320 7b6e 616d 657d 2034  ky logs {name} 4
-0000cd40: 202d 2d73 7461 7475 7327 2c20 2023 2045   --status',  # E
-0000cd50: 6e73 7572 6520 7468 6520 6a6f 6220 7375  nsure the job su
-0000cd60: 6363 6565 6465 642e 0a20 2020 2020 2020  cceeded..       
-0000cd70: 2020 2020 2027 736c 6565 7020 3138 3027       'sleep 180'
-0000cd80: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-0000cd90: 736b 7920 7374 6174 7573 202d 7220 7b6e  sky status -r {n
-0000cda0: 616d 657d 207c 2067 7265 7020 2249 4e49  ame} | grep "INI
-0000cdb0: 545c 7c53 544f 5050 4544 2227 2c0a 2020  T\|STOPPED"',.  
-0000cdc0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-0000cdd0: 2066 2773 6b79 2064 6f77 6e20 2d79 207b   f'sky down -y {
-0000cde0: 6e61 6d65 7d27 2c0a 2020 2020 290a 2020  name}',.    ).  
-0000cdf0: 2020 7275 6e5f 6f6e 655f 7465 7374 2874    run_one_test(t
-0000ce00: 6573 7429 0a0a 0a23 202d 2d2d 2d2d 2d2d  est)...# -------
-0000ce10: 2d2d 2d20 5465 7374 696e 6720 417a 7572  --- Testing Azur
-0000ce20: 6520 7374 6172 7420 616e 6420 7374 6f70  e start and stop
-0000ce30: 2069 6e73 7461 6e63 6573 202d 2d2d 2d2d   instances -----
-0000ce40: 2d2d 2d2d 2d0a 4070 7974 6573 742e 6d61  -----.@pytest.ma
-0000ce50: 726b 2e61 7a75 7265 0a64 6566 2074 6573  rk.azure.def tes
-0000ce60: 745f 617a 7572 655f 7374 6172 745f 7374  t_azure_start_st
-0000ce70: 6f70 2829 3a0a 2020 2020 6e61 6d65 203d  op():.    name =
-0000ce80: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
-0000ce90: 6d65 2829 0a20 2020 2074 6573 7420 3d20  me().    test = 
-0000cea0: 5465 7374 280a 2020 2020 2020 2020 2761  Test(.        'a
-0000ceb0: 7a75 7265 2d73 7461 7274 2d73 746f 7027  zure-start-stop'
-0000cec0: 2c0a 2020 2020 2020 2020 5b0a 2020 2020  ,.        [.    
-0000ced0: 2020 2020 2020 2020 6627 736b 7920 6c61          f'sky la
-0000cee0: 756e 6368 202d 7920 2d63 207b 6e61 6d65  unch -y -c {name
-0000cef0: 7d20 6578 616d 706c 6573 2f61 7a75 7265  } examples/azure
-0000cf00: 5f73 7461 7274 5f73 746f 702e 7961 6d6c  _start_stop.yaml
-0000cf10: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-0000cf20: 2773 6b79 2065 7865 6320 7b6e 616d 657d  'sky exec {name}
-0000cf30: 2065 7861 6d70 6c65 732f 617a 7572 655f   examples/azure_
-0000cf40: 7374 6172 745f 7374 6f70 2e79 616d 6c27  start_stop.yaml'
-0000cf50: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-0000cf60: 736b 7920 6c6f 6773 207b 6e61 6d65 7d20  sky logs {name} 
-0000cf70: 3120 2d2d 7374 6174 7573 272c 2020 2320  1 --status',  # 
-0000cf80: 456e 7375 7265 2074 6865 206a 6f62 2073  Ensure the job s
-0000cf90: 7563 6365 6564 6564 2e0a 2020 2020 2020  ucceeded..      
-0000cfa0: 2020 2020 2020 6627 736b 7920 6578 6563        f'sky exec
-0000cfb0: 207b 6e61 6d65 7d20 2270 726c 696d 6974   {name} "prlimit
-0000cfc0: 202d 6e20 2d2d 7069 643d 5c24 2870 6772   -n --pid=\$(pgr
-0000cfd0: 6570 202d 6620 5c27 7261 796c 6574 2f72  ep -f \'raylet/r
-0000cfe0: 6179 6c65 7420 2d2d 7261 796c 6574 5f73  aylet --raylet_s
-0000cff0: 6f63 6b65 745f 6e61 6d65 5c27 2920 7c20  ocket_name\') | 
-0000d000: 6772 6570 205c 2722 5c27 3130 3438 3537  grep \'"\'104857
-0000d010: 3620 3130 3438 3537 365c 2722 5c27 2227  6 1048576\'"\'"'
-0000d020: 2c20 2023 2045 6e73 7572 6520 7468 6520  ,  # Ensure the 
-0000d030: 7261 796c 6574 2070 726f 6365 7373 2068  raylet process h
-0000d040: 6173 2074 6865 2063 6f72 7265 6374 2066  as the correct f
-0000d050: 696c 6520 6465 7363 7269 7074 6f72 206c  ile descriptor l
-0000d060: 696d 6974 2e0a 2020 2020 2020 2020 2020  imit..          
-0000d070: 2020 6627 736b 7920 6c6f 6773 207b 6e61    f'sky logs {na
-0000d080: 6d65 7d20 3220 2d2d 7374 6174 7573 272c  me} 2 --status',
-0000d090: 2020 2320 456e 7375 7265 2074 6865 206a    # Ensure the j
-0000d0a0: 6f62 2073 7563 6365 6564 6564 2e0a 2020  ob succeeded..  
-0000d0b0: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
-0000d0c0: 7374 6f70 202d 7920 7b6e 616d 657d 272c  stop -y {name}',
-0000d0d0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-0000d0e0: 6b79 2073 7461 7274 202d 7920 7b6e 616d  ky start -y {nam
-0000d0f0: 657d 202d 6920 3127 2c0a 2020 2020 2020  e} -i 1',.      
-0000d100: 2020 2020 2020 6627 736b 7920 6578 6563        f'sky exec
-0000d110: 207b 6e61 6d65 7d20 6578 616d 706c 6573   {name} examples
-0000d120: 2f61 7a75 7265 5f73 7461 7274 5f73 746f  /azure_start_sto
-0000d130: 702e 7961 6d6c 272c 0a20 2020 2020 2020  p.yaml',.       
-0000d140: 2020 2020 2066 2773 6b79 206c 6f67 7320       f'sky logs 
-0000d150: 7b6e 616d 657d 2033 202d 2d73 7461 7475  {name} 3 --statu
-0000d160: 7327 2c20 2023 2045 6e73 7572 6520 7468  s',  # Ensure th
-0000d170: 6520 6a6f 6220 7375 6363 6565 6465 642e  e job succeeded.
-0000d180: 0a20 2020 2020 2020 2020 2020 2027 736c  .            'sl
-0000d190: 6565 7020 3230 3027 2c0a 2020 2020 2020  eep 200',.      
-0000d1a0: 2020 2020 2020 6627 733d 2428 736b 7920        f's=$(sky 
-0000d1b0: 7374 6174 7573 202d 7220 7b6e 616d 657d  status -r {name}
-0000d1c0: 2920 2626 2065 6368 6f20 2473 2026 2620  ) && echo $s && 
-0000d1d0: 6563 686f 2024 7320 7c20 6772 6570 2022  echo $s | grep "
-0000d1e0: 494e 4954 5c7c 5354 4f50 5045 4422 270a  INIT\|STOPPED"'.
-0000d1f0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-0000d200: 2020 2066 2773 6b79 2064 6f77 6e20 2d79     f'sky down -y
-0000d210: 207b 6e61 6d65 7d27 2c0a 2020 2020 2020   {name}',.      
-0000d220: 2020 7469 6d65 6f75 743d 3330 202a 2036    timeout=30 * 6
-0000d230: 302c 2020 2320 3330 206d 696e 730a 2020  0,  # 30 mins.  
-0000d240: 2020 290a 2020 2020 7275 6e5f 6f6e 655f    ).    run_one_
-0000d250: 7465 7374 2874 6573 7429 0a0a 0a23 202d  test(test)...# -
-0000d260: 2d2d 2d2d 2d2d 2d2d 2d20 5465 7374 696e  --------- Testin
-0000d270: 6720 4175 746f 7374 6f70 7069 6e67 202d  g Autostopping -
-0000d280: 2d2d 2d2d 2d2d 2d2d 2d0a 4070 7974 6573  ---------.@pytes
-0000d290: 742e 6d61 726b 2e6e 6f5f 6c61 6d62 6461  t.mark.no_lambda
-0000d2a0: 5f63 6c6f 7564 2020 2320 4c61 6d62 6461  _cloud  # Lambda
-0000d2b0: 2043 6c6f 7564 2064 6f65 7320 6e6f 7420   Cloud does not 
-0000d2c0: 7375 7070 6f72 7420 7374 6f70 7069 6e67  support stopping
-0000d2d0: 2069 6e73 7461 6e63 6573 0a40 7079 7465   instances.@pyte
-0000d2e0: 7374 2e6d 6172 6b2e 6e6f 5f69 626d 2020  st.mark.no_ibm  
-0000d2f0: 2320 4649 5828 4942 4d29 2073 706f 7261  # FIX(IBM) spora
-0000d300: 6469 6361 6c6c 7920 6661 696c 732c 2061  dically fails, a
-0000d310: 7320 7265 7374 6172 7465 6420 776f 726b  s restarted work
-0000d320: 6572 7320 7374 6179 2075 6e69 6e69 7469  ers stay uniniti
-0000d330: 616c 697a 6564 2069 6e64 6566 696e 6974  alized indefinit
-0000d340: 656c 790a 4070 7974 6573 742e 6d61 726b  ely.@pytest.mark
-0000d350: 2e6e 6f5f 7363 7020 2023 2053 4350 2064  .no_scp  # SCP d
-0000d360: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
-0000d370: 6e75 6d5f 6e6f 6465 7320 3e20 3120 7965  num_nodes > 1 ye
-0000d380: 740a 6465 6620 7465 7374 5f61 7574 6f73  t.def test_autos
-0000d390: 746f 7028 6765 6e65 7269 635f 636c 6f75  top(generic_clou
-0000d3a0: 643a 2073 7472 293a 0a20 2020 206e 616d  d: str):.    nam
-0000d3b0: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
-0000d3c0: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
-0000d3d0: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
-0000d3e0: 2027 6175 746f 7374 6f70 272c 0a20 2020   'autostop',.   
-0000d3f0: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
-0000d400: 2020 2066 2773 6b79 206c 6175 6e63 6820     f'sky launch 
-0000d410: 2d79 202d 6420 2d63 207b 6e61 6d65 7d20  -y -d -c {name} 
-0000d420: 2d2d 6e75 6d2d 6e6f 6465 7320 3220 2d2d  --num-nodes 2 --
-0000d430: 636c 6f75 6420 7b67 656e 6572 6963 5f63  cloud {generic_c
-0000d440: 6c6f 7564 7d20 7465 7374 732f 7465 7374  loud} tests/test
-0000d450: 5f79 616d 6c73 2f6d 696e 696d 616c 2e79  _yamls/minimal.y
-0000d460: 616d 6c27 2c0a 2020 2020 2020 2020 2020  aml',.          
-0000d470: 2020 6627 736b 7920 6175 746f 7374 6f70    f'sky autostop
-0000d480: 202d 7920 7b6e 616d 657d 202d 6920 3127   -y {name} -i 1'
-0000d490: 2c0a 0a20 2020 2020 2020 2020 2020 2023  ,..            #
-0000d4a0: 2045 6e73 7572 6520 6175 746f 7374 6f70   Ensure autostop
-0000d4b0: 2069 7320 7365 742e 0a20 2020 2020 2020   is set..       
-0000d4c0: 2020 2020 2066 2773 6b79 2073 7461 7475       f'sky statu
-0000d4d0: 7320 7c20 6772 6570 207b 6e61 6d65 7d20  s | grep {name} 
-0000d4e0: 7c20 6772 6570 2022 316d 2227 2c0a 0a20  | grep "1m"',.. 
-0000d4f0: 2020 2020 2020 2020 2020 2023 2045 6e73             # Ens
-0000d500: 7572 6520 7468 6520 636c 7573 7465 7220  ure the cluster 
-0000d510: 6973 206e 6f74 2073 746f 7070 6564 2065  is not stopped e
-0000d520: 6172 6c79 2e0a 2020 2020 2020 2020 2020  arly..          
-0000d530: 2020 2773 6c65 6570 2034 3527 2c0a 2020    'sleep 45',.  
-0000d540: 2020 2020 2020 2020 2020 6627 733d 2428            f's=$(
-0000d550: 736b 7920 7374 6174 7573 207b 6e61 6d65  sky status {name
-0000d560: 7d20 2d2d 7265 6672 6573 6829 3b20 6563  } --refresh); ec
-0000d570: 686f 2022 2473 223b 2065 6368 6f3b 2065  ho "$s"; echo; e
-0000d580: 6368 6f3b 2065 6368 6f20 2224 7322 2020  cho; echo "$s"  
-0000d590: 7c20 6772 6570 207b 6e61 6d65 7d20 7c20  | grep {name} | 
-0000d5a0: 6772 6570 2055 5027 2c0a 0a20 2020 2020  grep UP',..     
-0000d5b0: 2020 2020 2020 2023 2045 6e73 7572 6520         # Ensure 
-0000d5c0: 7468 6520 636c 7573 7465 7220 6973 2053  the cluster is S
-0000d5d0: 544f 5050 4544 2e0a 2020 2020 2020 2020  TOPPED..        
-0000d5e0: 2020 2020 2773 6c65 6570 2032 3530 272c      'sleep 250',
-0000d5f0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-0000d600: 3d24 2873 6b79 2073 7461 7475 7320 7b6e  =$(sky status {n
-0000d610: 616d 657d 202d 2d72 6566 7265 7368 293b  ame} --refresh);
-0000d620: 2065 6368 6f20 2224 7322 3b20 6563 686f   echo "$s"; echo
-0000d630: 3b20 6563 686f 3b20 6563 686f 2022 2473  ; echo; echo "$s
-0000d640: 2220 207c 2067 7265 7020 7b6e 616d 657d  "  | grep {name}
-0000d650: 207c 2067 7265 7020 5354 4f50 5045 4427   | grep STOPPED'
-0000d660: 2c0a 0a20 2020 2020 2020 2020 2020 2023  ,..            #
-0000d670: 2045 6e73 7572 6520 7468 6520 636c 7573   Ensure the clus
-0000d680: 7465 7220 6973 2055 5020 616e 6420 7468  ter is UP and th
-0000d690: 6520 6175 746f 7374 6f70 2073 6574 7469  e autostop setti
-0000d6a0: 6e67 2069 7320 7265 7365 7420 2827 2d27  ng is reset ('-'
-0000d6b0: 292e 0a20 2020 2020 2020 2020 2020 2066  )..            f
-0000d6c0: 2773 6b79 2073 7461 7274 202d 7920 7b6e  'sky start -y {n
-0000d6d0: 616d 657d 272c 0a20 2020 2020 2020 2020  ame}',.         
-0000d6e0: 2020 2066 2773 6b79 2073 7461 7475 7320     f'sky status 
-0000d6f0: 7c20 6772 6570 207b 6e61 6d65 7d20 7c20  | grep {name} | 
-0000d700: 6772 6570 202d 4520 2255 505c 732b 2d22  grep -E "UP\s+-"
-0000d710: 272c 0a0a 2020 2020 2020 2020 2020 2020  ',..            
-0000d720: 2320 456e 7375 7265 2074 6865 206a 6f62  # Ensure the job
-0000d730: 2073 7563 6365 6564 6564 2e0a 2020 2020   succeeded..    
-0000d740: 2020 2020 2020 2020 6627 736b 7920 6578          f'sky ex
-0000d750: 6563 207b 6e61 6d65 7d20 7465 7374 732f  ec {name} tests/
-0000d760: 7465 7374 5f79 616d 6c73 2f6d 696e 696d  test_yamls/minim
-0000d770: 616c 2e79 616d 6c27 2c0a 2020 2020 2020  al.yaml',.      
-0000d780: 2020 2020 2020 6627 736b 7920 6c6f 6773        f'sky logs
-0000d790: 207b 6e61 6d65 7d20 3220 2d2d 7374 6174   {name} 2 --stat
-0000d7a0: 7573 272c 0a0a 2020 2020 2020 2020 2020  us',..          
-0000d7b0: 2020 2320 5465 7374 2072 6573 7461 7274    # Test restart
-0000d7c0: 696e 6720 7468 6520 6964 6c65 6e65 7373  ing the idleness
-0000d7d0: 2074 696d 6572 2076 6961 2063 616e 6365   timer via cance
-0000d7e0: 6c20 2b20 7265 7365 743a 0a20 2020 2020  l + reset:.     
-0000d7f0: 2020 2020 2020 2066 2773 6b79 2061 7574         f'sky aut
-0000d800: 6f73 746f 7020 2d79 207b 6e61 6d65 7d20  ostop -y {name} 
-0000d810: 2d69 2031 272c 2020 2320 4964 6c65 6e65  -i 1',  # Idlene
-0000d820: 7373 2073 7461 7274 7320 636f 756e 7469  ss starts counti
-0000d830: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
-0000d840: 2773 6c65 6570 2034 3527 2c20 2023 2041  'sleep 45',  # A
-0000d850: 6c6d 6f73 7420 7265 6163 6865 6420 7468  lmost reached th
-0000d860: 6520 7468 7265 7368 6f6c 642e 0a20 2020  e threshold..   
-0000d870: 2020 2020 2020 2020 2066 2773 6b79 2061           f'sky a
-0000d880: 7574 6f73 746f 7020 2d79 207b 6e61 6d65  utostop -y {name
-0000d890: 7d20 2d2d 6361 6e63 656c 272c 0a20 2020  } --cancel',.   
-0000d8a0: 2020 2020 2020 2020 2066 2773 6b79 2061           f'sky a
-0000d8b0: 7574 6f73 746f 7020 2d79 207b 6e61 6d65  utostop -y {name
-0000d8c0: 7d20 2d69 2031 272c 2020 2320 5368 6f75  } -i 1',  # Shou
-0000d8d0: 6c64 2072 6573 7461 7274 2074 6865 2074  ld restart the t
-0000d8e0: 696d 6572 2e0a 2020 2020 2020 2020 2020  imer..          
-0000d8f0: 2020 2773 6c65 6570 2034 3527 2c0a 2020    'sleep 45',.  
-0000d900: 2020 2020 2020 2020 2020 6627 733d 2428            f's=$(
-0000d910: 736b 7920 7374 6174 7573 207b 6e61 6d65  sky status {name
-0000d920: 7d20 2d2d 7265 6672 6573 6829 3b20 6563  } --refresh); ec
-0000d930: 686f 2022 2473 223b 2065 6368 6f3b 2065  ho "$s"; echo; e
-0000d940: 6368 6f3b 2065 6368 6f20 2224 7322 207c  cho; echo "$s" |
-0000d950: 2067 7265 7020 7b6e 616d 657d 207c 2067   grep {name} | g
-0000d960: 7265 7020 5550 272c 0a20 2020 2020 2020  rep UP',.       
-0000d970: 2020 2020 2027 736c 6565 7020 3235 3027       'sleep 250'
-0000d980: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-0000d990: 733d 2428 736b 7920 7374 6174 7573 207b  s=$(sky status {
-0000d9a0: 6e61 6d65 7d20 2d2d 7265 6672 6573 6829  name} --refresh)
-0000d9b0: 3b20 6563 686f 2022 2473 223b 2065 6368  ; echo "$s"; ech
-0000d9c0: 6f3b 2065 6368 6f3b 2065 6368 6f20 2224  o; echo; echo "$
-0000d9d0: 7322 2020 7c20 6772 6570 207b 6e61 6d65  s"  | grep {name
-0000d9e0: 7d20 7c20 6772 6570 2053 544f 5050 4544  } | grep STOPPED
-0000d9f0: 272c 0a0a 2020 2020 2020 2020 2020 2020  ',..            
-0000da00: 2320 5465 7374 2072 6573 7461 7274 696e  # Test restartin
-0000da10: 6720 7468 6520 6964 6c65 6e65 7373 2074  g the idleness t
-0000da20: 696d 6572 2076 6961 2065 7865 633a 0a20  imer via exec:. 
-0000da30: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-0000da40: 2073 7461 7274 202d 7920 7b6e 616d 657d   start -y {name}
-0000da50: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-0000da60: 2773 6b79 2073 7461 7475 7320 7c20 6772  'sky status | gr
-0000da70: 6570 207b 6e61 6d65 7d20 7c20 6772 6570  ep {name} | grep
-0000da80: 202d 4520 2255 505c 732b 2d22 272c 0a20   -E "UP\s+-"',. 
-0000da90: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-0000daa0: 2061 7574 6f73 746f 7020 2d79 207b 6e61   autostop -y {na
-0000dab0: 6d65 7d20 2d69 2031 272c 2020 2320 4964  me} -i 1',  # Id
-0000dac0: 6c65 6e65 7373 2073 7461 7274 7320 636f  leness starts co
-0000dad0: 756e 7469 6e67 2e0a 2020 2020 2020 2020  unting..        
-0000dae0: 2020 2020 2773 6c65 6570 2034 3527 2c20      'sleep 45', 
-0000daf0: 2023 2041 6c6d 6f73 7420 7265 6163 6865   # Almost reache
-0000db00: 6420 7468 6520 7468 7265 7368 6f6c 642e  d the threshold.
-0000db10: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-0000db20: 6b79 2065 7865 6320 7b6e 616d 657d 2065  ky exec {name} e
-0000db30: 6368 6f20 6869 272c 2020 2320 5368 6f75  cho hi',  # Shou
-0000db40: 6c64 2072 6573 7461 7274 2074 6865 2074  ld restart the t
-0000db50: 696d 6572 2e0a 2020 2020 2020 2020 2020  imer..          
-0000db60: 2020 2773 6c65 6570 2034 3527 2c0a 2020    'sleep 45',.  
-0000db70: 2020 2020 2020 2020 2020 6627 733d 2428            f's=$(
-0000db80: 736b 7920 7374 6174 7573 207b 6e61 6d65  sky status {name
-0000db90: 7d20 2d2d 7265 6672 6573 6829 3b20 6563  } --refresh); ec
-0000dba0: 686f 2022 2473 223b 2065 6368 6f3b 2065  ho "$s"; echo; e
-0000dbb0: 6368 6f3b 2065 6368 6f20 2224 7322 2020  cho; echo "$s"  
-0000dbc0: 7c20 6772 6570 207b 6e61 6d65 7d20 7c20  | grep {name} | 
-0000dbd0: 6772 6570 2055 5027 2c0a 2020 2020 2020  grep UP',.      
-0000dbe0: 2020 2020 2020 2773 6c65 6570 2032 3530        'sleep 250
-0000dbf0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-0000dc00: 2773 3d24 2873 6b79 2073 7461 7475 7320  's=$(sky status 
-0000dc10: 7b6e 616d 657d 202d 2d72 6566 7265 7368  {name} --refresh
-0000dc20: 293b 2065 6368 6f20 2224 7322 3b20 6563  ); echo "$s"; ec
-0000dc30: 686f 3b20 6563 686f 3b20 6563 686f 2022  ho; echo; echo "
-0000dc40: 2473 2220 207c 2067 7265 7020 7b6e 616d  $s"  | grep {nam
-0000dc50: 657d 207c 2067 7265 7020 5354 4f50 5045  e} | grep STOPPE
-0000dc60: 4427 2c0a 2020 2020 2020 2020 5d2c 0a20  D',.        ],. 
-0000dc70: 2020 2020 2020 2066 2773 6b79 2064 6f77         f'sky dow
-0000dc80: 6e20 2d79 207b 6e61 6d65 7d27 2c0a 2020  n -y {name}',.  
-0000dc90: 2020 2020 2020 7469 6d65 6f75 743d 3230        timeout=20
-0000dca0: 202a 2036 302c 0a20 2020 2029 0a20 2020   * 60,.    ).   
-0000dcb0: 2072 756e 5f6f 6e65 5f74 6573 7428 7465   run_one_test(te
-0000dcc0: 7374 290a 0a0a 2320 2d2d 2d2d 2d2d 2d2d  st)...# --------
-0000dcd0: 2d2d 2054 6573 7469 6e67 2041 7574 6f64  -- Testing Autod
-0000dce0: 6f77 6e69 6e67 202d 2d2d 2d2d 2d2d 2d2d  owning ---------
-0000dcf0: 2d0a 4070 7974 6573 742e 6d61 726b 2e6e  -.@pytest.mark.n
-0000dd00: 6f5f 7363 7020 2023 2053 4350 2064 6f65  o_scp  # SCP doe
-0000dd10: 7320 6e6f 7420 7375 7070 6f72 7420 6e75  s not support nu
-0000dd20: 6d5f 6e6f 6465 7320 3e20 3120 7965 742e  m_nodes > 1 yet.
-0000dd30: 2052 756e 2074 6573 745f 7363 705f 6175   Run test_scp_au
-0000dd40: 746f 646f 776e 2069 6e73 7465 6164 2e0a  todown instead..
-0000dd50: 6465 6620 7465 7374 5f61 7574 6f64 6f77  def test_autodow
-0000dd60: 6e28 6765 6e65 7269 635f 636c 6f75 643a  n(generic_cloud:
-0000dd70: 2073 7472 293a 0a20 2020 206e 616d 6520   str):.    name 
-0000dd80: 3d20 5f67 6574 5f63 6c75 7374 6572 5f6e  = _get_cluster_n
-0000dd90: 616d 6528 290a 2020 2020 7465 7374 203d  ame().    test =
-0000dda0: 2054 6573 7428 0a20 2020 2020 2020 2027   Test(.        '
-0000ddb0: 6175 746f 646f 776e 272c 0a20 2020 2020  autodown',.     
-0000ddc0: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-0000ddd0: 2066 2773 6b79 206c 6175 6e63 6820 2d79   f'sky launch -y
-0000dde0: 202d 6420 2d63 207b 6e61 6d65 7d20 2d2d   -d -c {name} --
-0000ddf0: 6e75 6d2d 6e6f 6465 7320 3220 2d2d 636c  num-nodes 2 --cl
-0000de00: 6f75 6420 7b67 656e 6572 6963 5f63 6c6f  oud {generic_clo
-0000de10: 7564 7d20 7465 7374 732f 7465 7374 5f79  ud} tests/test_y
-0000de20: 616d 6c73 2f6d 696e 696d 616c 2e79 616d  amls/minimal.yam
-0000de30: 6c27 2c0a 2020 2020 2020 2020 2020 2020  l',.            
-0000de40: 6627 736b 7920 6175 746f 7374 6f70 202d  f'sky autostop -
-0000de50: 7920 7b6e 616d 657d 202d 2d64 6f77 6e20  y {name} --down 
-0000de60: 2d69 2031 272c 0a20 2020 2020 2020 2020  -i 1',.         
-0000de70: 2020 2023 2045 6e73 7572 6520 6175 746f     # Ensure auto
-0000de80: 7374 6f70 2069 7320 7365 742e 0a20 2020  stop is set..   
-0000de90: 2020 2020 2020 2020 2066 2773 6b79 2073           f'sky s
-0000dea0: 7461 7475 7320 7c20 6772 6570 207b 6e61  tatus | grep {na
-0000deb0: 6d65 7d20 7c20 6772 6570 2022 316d 2028  me} | grep "1m (
-0000dec0: 646f 776e 2922 272c 0a20 2020 2020 2020  down)"',.       
-0000ded0: 2020 2020 2023 2045 6e73 7572 6520 7468       # Ensure th
-0000dee0: 6520 636c 7573 7465 7220 6973 206e 6f74  e cluster is not
-0000def0: 2074 6572 6d69 6e61 7465 6420 6561 726c   terminated earl
-0000df00: 792e 0a20 2020 2020 2020 2020 2020 2027  y..            '
-0000df10: 736c 6565 7020 3435 272c 0a20 2020 2020  sleep 45',.     
-0000df20: 2020 2020 2020 2066 2773 3d24 2873 6b79         f's=$(sky
-0000df30: 2073 7461 7475 7320 7b6e 616d 657d 202d   status {name} -
-0000df40: 2d72 6566 7265 7368 293b 2065 6368 6f20  -refresh); echo 
-0000df50: 2224 7322 3b20 6563 686f 3b20 6563 686f  "$s"; echo; echo
-0000df60: 3b20 6563 686f 2022 2473 2220 207c 2067  ; echo "$s"  | g
-0000df70: 7265 7020 7b6e 616d 657d 207c 2067 7265  rep {name} | gre
-0000df80: 7020 5550 272c 0a20 2020 2020 2020 2020  p UP',.         
-0000df90: 2020 2023 2045 6e73 7572 6520 7468 6520     # Ensure the 
-0000dfa0: 636c 7573 7465 7220 6973 2074 6572 6d69  cluster is termi
-0000dfb0: 6e61 7465 642e 0a20 2020 2020 2020 2020  nated..         
-0000dfc0: 2020 2027 736c 6565 7020 3230 3027 2c0a     'sleep 200',.
-0000dfd0: 2020 2020 2020 2020 2020 2020 6627 733d              f's=
-0000dfe0: 2428 534b 5950 494c 4f54 5f44 4542 5547  $(SKYPILOT_DEBUG
-0000dff0: 3d30 2073 6b79 2073 7461 7475 7320 7b6e  =0 sky status {n
-0000e000: 616d 657d 202d 2d72 6566 7265 7368 2920  ame} --refresh) 
-0000e010: 2626 2065 6368 6f20 2224 7322 2026 2620  && echo "$s" && 
-0000e020: 7b7b 2065 6368 6f20 2224 7322 207c 2067  {{ echo "$s" | g
-0000e030: 7265 7020 7b6e 616d 657d 207c 2067 7265  rep {name} | gre
-0000e040: 7020 2241 7574 6f64 6f77 6e65 6420 636c  p "Autodowned cl
-0000e050: 7573 7465 725c 7c74 6572 6d69 6e61 7465  uster\|terminate
-0000e060: 6420 6f6e 2074 6865 2063 6c6f 7564 223b  d on the cloud";
-0000e070: 207d 7d20 7c7c 207b 7b20 6563 686f 2022   }} || {{ echo "
-0000e080: 2473 2220 7c20 6772 6570 207b 6e61 6d65  $s" | grep {name
-0000e090: 7d20 2626 2065 7869 7420 3120 7c7c 2065  } && exit 1 || e
-0000e0a0: 7869 7420 303b 207d 7d27 2c0a 2020 2020  xit 0; }}',.    
-0000e0b0: 2020 2020 2020 2020 6627 736b 7920 6c61          f'sky la
-0000e0c0: 756e 6368 202d 7920 2d64 202d 6320 7b6e  unch -y -d -c {n
-0000e0d0: 616d 657d 202d 2d63 6c6f 7564 207b 6765  ame} --cloud {ge
-0000e0e0: 6e65 7269 635f 636c 6f75 647d 202d 2d6e  neric_cloud} --n
-0000e0f0: 756d 2d6e 6f64 6573 2032 202d 2d64 6f77  um-nodes 2 --dow
-0000e100: 6e20 7465 7374 732f 7465 7374 5f79 616d  n tests/test_yam
-0000e110: 6c73 2f6d 696e 696d 616c 2e79 616d 6c27  ls/minimal.yaml'
-0000e120: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-0000e130: 736b 7920 7374 6174 7573 207c 2067 7265  sky status | gre
-0000e140: 7020 7b6e 616d 657d 207c 2067 7265 7020  p {name} | grep 
-0000e150: 5550 272c 2020 2320 456e 7375 7265 2074  UP',  # Ensure t
-0000e160: 6865 2063 6c75 7374 6572 2069 7320 5550  he cluster is UP
-0000e170: 2e0a 2020 2020 2020 2020 2020 2020 6627  ..            f'
-0000e180: 736b 7920 6578 6563 207b 6e61 6d65 7d20  sky exec {name} 
-0000e190: 2d2d 636c 6f75 6420 7b67 656e 6572 6963  --cloud {generic
-0000e1a0: 5f63 6c6f 7564 7d20 7465 7374 732f 7465  _cloud} tests/te
-0000e1b0: 7374 5f79 616d 6c73 2f6d 696e 696d 616c  st_yamls/minimal
-0000e1c0: 2e79 616d 6c27 2c0a 2020 2020 2020 2020  .yaml',.        
-0000e1d0: 2020 2020 6627 736b 7920 7374 6174 7573      f'sky status
-0000e1e0: 207c 2067 7265 7020 7b6e 616d 657d 207c   | grep {name} |
-0000e1f0: 2067 7265 7020 2231 6d20 2864 6f77 6e29   grep "1m (down)
-0000e200: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-0000e210: 2773 6c65 6570 2032 3430 272c 0a20 2020  'sleep 240',.   
-0000e220: 2020 2020 2020 2020 2023 2045 6e73 7572           # Ensur
-0000e230: 6520 7468 6520 636c 7573 7465 7220 6973  e the cluster is
-0000e240: 2074 6572 6d69 6e61 7465 642e 0a20 2020   terminated..   
-0000e250: 2020 2020 2020 2020 2066 2773 3d24 2853           f's=$(S
-0000e260: 4b59 5049 4c4f 545f 4445 4255 473d 3020  KYPILOT_DEBUG=0 
-0000e270: 736b 7920 7374 6174 7573 207b 6e61 6d65  sky status {name
-0000e280: 7d20 2d2d 7265 6672 6573 6829 2026 2620  } --refresh) && 
-0000e290: 6563 686f 2022 2473 2220 2626 207b 7b20  echo "$s" && {{ 
-0000e2a0: 6563 686f 2022 2473 2220 7c20 6772 6570  echo "$s" | grep
-0000e2b0: 207b 6e61 6d65 7d20 7c20 6772 6570 2022   {name} | grep "
-0000e2c0: 4175 746f 646f 776e 6564 2063 6c75 7374  Autodowned clust
-0000e2d0: 6572 5c7c 7465 726d 696e 6174 6564 206f  er\|terminated o
-0000e2e0: 6e20 7468 6520 636c 6f75 6422 3b20 7d7d  n the cloud"; }}
-0000e2f0: 207c 7c20 7b7b 2065 6368 6f20 2224 7322   || {{ echo "$s"
-0000e300: 207c 2067 7265 7020 7b6e 616d 657d 2026   | grep {name} &
-0000e310: 2620 6578 6974 2031 207c 7c20 6578 6974  & exit 1 || exit
-0000e320: 2030 3b20 7d7d 272c 0a20 2020 2020 2020   0; }}',.       
-0000e330: 2020 2020 2066 2773 6b79 206c 6175 6e63       f'sky launc
-0000e340: 6820 2d79 202d 6420 2d63 207b 6e61 6d65  h -y -d -c {name
-0000e350: 7d20 2d2d 636c 6f75 6420 7b67 656e 6572  } --cloud {gener
-0000e360: 6963 5f63 6c6f 7564 7d20 2d2d 6e75 6d2d  ic_cloud} --num-
-0000e370: 6e6f 6465 7320 3220 2d2d 646f 776e 2074  nodes 2 --down t
-0000e380: 6573 7473 2f74 6573 745f 7961 6d6c 732f  ests/test_yamls/
-0000e390: 6d69 6e69 6d61 6c2e 7961 6d6c 272c 0a20  minimal.yaml',. 
-0000e3a0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-0000e3b0: 2061 7574 6f73 746f 7020 2d79 207b 6e61   autostop -y {na
-0000e3c0: 6d65 7d20 2d2d 6361 6e63 656c 272c 0a20  me} --cancel',. 
-0000e3d0: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
-0000e3e0: 7020 3234 3027 2c0a 2020 2020 2020 2020  p 240',.        
-0000e3f0: 2020 2020 2320 456e 7375 7265 2074 6865      # Ensure the
-0000e400: 2063 6c75 7374 6572 2069 7320 7374 696c   cluster is stil
-0000e410: 6c20 5550 2e0a 2020 2020 2020 2020 2020  l UP..          
-0000e420: 2020 6627 733d 2428 534b 5950 494c 4f54    f's=$(SKYPILOT
-0000e430: 5f44 4542 5547 3d30 2073 6b79 2073 7461  _DEBUG=0 sky sta
-0000e440: 7475 7320 7b6e 616d 657d 202d 2d72 6566  tus {name} --ref
-0000e450: 7265 7368 2920 2626 2065 6368 6f20 2224  resh) && echo "$
-0000e460: 7322 2026 2620 6563 686f 2022 2473 2220  s" && echo "$s" 
-0000e470: 7c20 6772 6570 207b 6e61 6d65 7d20 7c20  | grep {name} | 
-0000e480: 6772 6570 2055 5027 2c0a 2020 2020 2020  grep UP',.      
-0000e490: 2020 5d2c 0a20 2020 2020 2020 2066 2773    ],.        f's
-0000e4a0: 6b79 2064 6f77 6e20 2d79 207b 6e61 6d65  ky down -y {name
-0000e4b0: 7d27 2c0a 2020 2020 2020 2020 7469 6d65  }',.        time
-0000e4c0: 6f75 743d 3230 202a 2036 302c 0a20 2020  out=20 * 60,.   
-0000e4d0: 2029 0a20 2020 2072 756e 5f6f 6e65 5f74   ).    run_one_t
-0000e4e0: 6573 7428 7465 7374 290a 0a0a 4070 7974  est(test)...@pyt
-0000e4f0: 6573 742e 6d61 726b 2e73 6370 0a64 6566  est.mark.scp.def
-0000e500: 2074 6573 745f 7363 705f 6175 746f 646f   test_scp_autodo
-0000e510: 776e 2829 3a0a 2020 2020 6e61 6d65 203d  wn():.    name =
-0000e520: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
-0000e530: 6d65 2829 0a20 2020 2074 6573 7420 3d20  me().    test = 
-0000e540: 5465 7374 280a 2020 2020 2020 2020 2753  Test(.        'S
-0000e550: 4350 5f61 7574 6f64 6f77 6e27 2c0a 2020  CP_autodown',.  
-0000e560: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-0000e570: 2020 2020 6627 736b 7920 6c61 756e 6368      f'sky launch
-0000e580: 202d 7920 2d64 202d 6320 7b6e 616d 657d   -y -d -c {name}
-0000e590: 207b 5343 505f 5459 5045 7d20 7465 7374   {SCP_TYPE} test
-0000e5a0: 732f 7465 7374 5f79 616d 6c73 2f6d 696e  s/test_yamls/min
-0000e5b0: 696d 616c 2e79 616d 6c27 2c0a 2020 2020  imal.yaml',.    
-0000e5c0: 2020 2020 2020 2020 6627 736b 7920 6175          f'sky au
-0000e5d0: 746f 7374 6f70 202d 7920 7b6e 616d 657d  tostop -y {name}
-0000e5e0: 202d 2d64 6f77 6e20 2d69 2031 272c 0a20   --down -i 1',. 
-0000e5f0: 2020 2020 2020 2020 2020 2023 2045 6e73             # Ens
-0000e600: 7572 6520 6175 746f 7374 6f70 2069 7320  ure autostop is 
-0000e610: 7365 742e 0a20 2020 2020 2020 2020 2020  set..           
-0000e620: 2066 2773 6b79 2073 7461 7475 7320 7c20   f'sky status | 
-0000e630: 6772 6570 207b 6e61 6d65 7d20 7c20 6772  grep {name} | gr
-0000e640: 6570 2022 316d 2028 646f 776e 2922 272c  ep "1m (down)"',
-0000e650: 0a20 2020 2020 2020 2020 2020 2023 2045  .            # E
-0000e660: 6e73 7572 6520 7468 6520 636c 7573 7465  nsure the cluste
-0000e670: 7220 6973 206e 6f74 2074 6572 6d69 6e61  r is not termina
-0000e680: 7465 6420 6561 726c 792e 0a20 2020 2020  ted early..     
-0000e690: 2020 2020 2020 2027 736c 6565 7020 3435         'sleep 45
-0000e6a0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-0000e6b0: 2773 6b79 2073 7461 7475 7320 2d2d 7265  'sky status --re
-0000e6c0: 6672 6573 6820 7c20 6772 6570 207b 6e61  fresh | grep {na
-0000e6d0: 6d65 7d20 7c20 6772 6570 2055 5027 2c0a  me} | grep UP',.
-0000e6e0: 2020 2020 2020 2020 2020 2020 2320 456e              # En
-0000e6f0: 7375 7265 2074 6865 2063 6c75 7374 6572  sure the cluster
-0000e700: 2069 7320 7465 726d 696e 6174 6564 2e0a   is terminated..
-0000e710: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
-0000e720: 6570 2032 3030 272c 0a20 2020 2020 2020  ep 200',.       
-0000e730: 2020 2020 2066 2773 3d24 2853 4b59 5049       f's=$(SKYPI
-0000e740: 4c4f 545f 4445 4255 473d 3020 736b 7920  LOT_DEBUG=0 sky 
-0000e750: 7374 6174 7573 202d 2d72 6566 7265 7368  status --refresh
-0000e760: 2920 2626 2070 7269 6e74 6620 2224 7322  ) && printf "$s"
-0000e770: 2026 2620 7b7b 2065 6368 6f20 2224 7322   && {{ echo "$s"
-0000e780: 207c 2067 7265 7020 7b6e 616d 657d 207c   | grep {name} |
-0000e790: 2067 7265 7020 2241 7574 6f64 6f77 6e65   grep "Autodowne
-0000e7a0: 6420 636c 7573 7465 725c 7c74 6572 6d69  d cluster\|termi
-0000e7b0: 6e61 7465 6420 6f6e 2074 6865 2063 6c6f  nated on the clo
-0000e7c0: 7564 223b 207d 7d20 7c7c 207b 7b20 6563  ud"; }} || {{ ec
-0000e7d0: 686f 2022 2473 2220 7c20 6772 6570 207b  ho "$s" | grep {
-0000e7e0: 6e61 6d65 7d20 2626 2065 7869 7420 3120  name} && exit 1 
-0000e7f0: 7c7c 2065 7869 7420 303b 207d 7d27 2c0a  || exit 0; }}',.
-0000e800: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-0000e810: 7920 6c61 756e 6368 202d 7920 2d64 202d  y launch -y -d -
-0000e820: 6320 7b6e 616d 657d 207b 5343 505f 5459  c {name} {SCP_TY
-0000e830: 5045 7d20 2d2d 646f 776e 2074 6573 7473  PE} --down tests
-0000e840: 2f74 6573 745f 7961 6d6c 732f 6d69 6e69  /test_yamls/mini
-0000e850: 6d61 6c2e 7961 6d6c 272c 0a20 2020 2020  mal.yaml',.     
-0000e860: 2020 2020 2020 2066 2773 6b79 2073 7461         f'sky sta
-0000e870: 7475 7320 7c20 6772 6570 207b 6e61 6d65  tus | grep {name
-0000e880: 7d20 7c20 6772 6570 2055 5027 2c20 2023  } | grep UP',  #
-0000e890: 2045 6e73 7572 6520 7468 6520 636c 7573   Ensure the clus
-0000e8a0: 7465 7220 6973 2055 502e 0a20 2020 2020  ter is UP..     
-0000e8b0: 2020 2020 2020 2066 2773 6b79 2065 7865         f'sky exe
-0000e8c0: 6320 7b6e 616d 657d 207b 5343 505f 5459  c {name} {SCP_TY
-0000e8d0: 5045 7d20 7465 7374 732f 7465 7374 5f79  PE} tests/test_y
-0000e8e0: 616d 6c73 2f6d 696e 696d 616c 2e79 616d  amls/minimal.yam
-0000e8f0: 6c27 2c0a 2020 2020 2020 2020 2020 2020  l',.            
-0000e900: 6627 736b 7920 7374 6174 7573 207c 2067  f'sky status | g
-0000e910: 7265 7020 7b6e 616d 657d 207c 2067 7265  rep {name} | gre
-0000e920: 7020 2231 6d20 2864 6f77 6e29 2227 2c0a  p "1m (down)"',.
-0000e930: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
-0000e940: 6570 2032 3030 272c 0a20 2020 2020 2020  ep 200',.       
-0000e950: 2020 2020 2023 2045 6e73 7572 6520 7468       # Ensure th
-0000e960: 6520 636c 7573 7465 7220 6973 2074 6572  e cluster is ter
-0000e970: 6d69 6e61 7465 642e 0a20 2020 2020 2020  minated..       
-0000e980: 2020 2020 2066 2773 3d24 2853 4b59 5049       f's=$(SKYPI
-0000e990: 4c4f 545f 4445 4255 473d 3020 736b 7920  LOT_DEBUG=0 sky 
-0000e9a0: 7374 6174 7573 202d 2d72 6566 7265 7368  status --refresh
-0000e9b0: 2920 2626 2070 7269 6e74 6620 2224 7322  ) && printf "$s"
-0000e9c0: 2026 2620 7b7b 2065 6368 6f20 2224 7322   && {{ echo "$s"
-0000e9d0: 207c 2067 7265 7020 7b6e 616d 657d 207c   | grep {name} |
-0000e9e0: 2067 7265 7020 2241 7574 6f64 6f77 6e65   grep "Autodowne
-0000e9f0: 6420 636c 7573 7465 725c 7c74 6572 6d69  d cluster\|termi
-0000ea00: 6e61 7465 6420 6f6e 2074 6865 2063 6c6f  nated on the clo
-0000ea10: 7564 223b 207d 7d20 7c7c 207b 7b20 6563  ud"; }} || {{ ec
-0000ea20: 686f 2022 2473 2220 7c20 6772 6570 207b  ho "$s" | grep {
-0000ea30: 6e61 6d65 7d20 2626 2065 7869 7420 3120  name} && exit 1 
-0000ea40: 7c7c 2065 7869 7420 303b 207d 7d27 2c0a  || exit 0; }}',.
-0000ea50: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-0000ea60: 7920 6c61 756e 6368 202d 7920 2d64 202d  y launch -y -d -
-0000ea70: 6320 7b6e 616d 657d 207b 5343 505f 5459  c {name} {SCP_TY
-0000ea80: 5045 7d20 2d2d 646f 776e 2074 6573 7473  PE} --down tests
-0000ea90: 2f74 6573 745f 7961 6d6c 732f 6d69 6e69  /test_yamls/mini
-0000eaa0: 6d61 6c2e 7961 6d6c 272c 0a20 2020 2020  mal.yaml',.     
-0000eab0: 2020 2020 2020 2066 2773 6b79 2061 7574         f'sky aut
-0000eac0: 6f73 746f 7020 2d79 207b 6e61 6d65 7d20  ostop -y {name} 
-0000ead0: 2d2d 6361 6e63 656c 272c 0a20 2020 2020  --cancel',.     
-0000eae0: 2020 2020 2020 2027 736c 6565 7020 3230         'sleep 20
-0000eaf0: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
-0000eb00: 2320 456e 7375 7265 2074 6865 2063 6c75  # Ensure the clu
-0000eb10: 7374 6572 2069 7320 7374 696c 6c20 5550  ster is still UP
-0000eb20: 2e0a 2020 2020 2020 2020 2020 2020 6627  ..            f'
-0000eb30: 733d 2428 534b 5950 494c 4f54 5f44 4542  s=$(SKYPILOT_DEB
-0000eb40: 5547 3d30 2073 6b79 2073 7461 7475 7320  UG=0 sky status 
-0000eb50: 2d2d 7265 6672 6573 6829 2026 2620 7072  --refresh) && pr
-0000eb60: 696e 7466 2022 2473 2220 2626 2065 6368  intf "$s" && ech
-0000eb70: 6f20 2224 7322 207c 2067 7265 7020 7b6e  o "$s" | grep {n
-0000eb80: 616d 657d 207c 2067 7265 7020 5550 272c  ame} | grep UP',
-0000eb90: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
-0000eba0: 2020 2020 6627 736b 7920 646f 776e 202d      f'sky down -
-0000ebb0: 7920 7b6e 616d 657d 272c 0a20 2020 2020  y {name}',.     
-0000ebc0: 2020 2074 696d 656f 7574 3d32 3520 2a20     timeout=25 * 
-0000ebd0: 3630 2c0a 2020 2020 290a 2020 2020 7275  60,.    ).    ru
-0000ebe0: 6e5f 6f6e 655f 7465 7374 2874 6573 7429  n_one_test(test)
-0000ebf0: 0a0a 0a64 6566 205f 6765 745f 6361 6e63  ...def _get_canc
-0000ec00: 656c 5f74 6173 6b5f 7769 7468 5f63 6c6f  el_task_with_clo
-0000ec10: 7564 286e 616d 652c 2063 6c6f 7564 2c20  ud(name, cloud, 
-0000ec20: 7469 6d65 6f75 743d 3135 202a 2036 3029  timeout=15 * 60)
-0000ec30: 3a0a 2020 2020 7465 7374 203d 2054 6573  :.    test = Tes
-0000ec40: 7428 0a20 2020 2020 2020 2066 277b 636c  t(.        f'{cl
-0000ec50: 6f75 647d 2d63 616e 6365 6c2d 7461 736b  oud}-cancel-task
-0000ec60: 272c 0a20 2020 2020 2020 205b 0a20 2020  ',.        [.   
-0000ec70: 2020 2020 2020 2020 2066 2773 6b79 206c           f'sky l
-0000ec80: 6175 6e63 6820 2d63 207b 6e61 6d65 7d20  aunch -c {name} 
-0000ec90: 6578 616d 706c 6573 2f72 6573 6e65 745f  examples/resnet_
-0000eca0: 6170 702e 7961 6d6c 202d 2d63 6c6f 7564  app.yaml --cloud
-0000ecb0: 207b 636c 6f75 647d 202d 7920 2d64 272c   {cloud} -y -d',
-0000ecc0: 0a20 2020 2020 2020 2020 2020 2023 2057  .            # W
-0000ecd0: 6169 7420 7468 6520 4750 5520 7072 6f63  ait the GPU proc
-0000ece0: 6573 7320 746f 2073 7461 7274 2e0a 2020  ess to start..  
-0000ecf0: 2020 2020 2020 2020 2020 2773 6c65 6570            'sleep
-0000ed00: 2036 3027 2c0a 2020 2020 2020 2020 2020   60',.          
-0000ed10: 2020 6627 736b 7920 6578 6563 207b 6e61    f'sky exec {na
-0000ed20: 6d65 7d20 226e 7669 6469 612d 736d 6920  me} "nvidia-smi 
-0000ed30: 7c20 6772 6570 2070 7974 686f 6e22 272c  | grep python"',
-0000ed40: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-0000ed50: 6b79 206c 6f67 7320 7b6e 616d 657d 2032  ky logs {name} 2
-0000ed60: 202d 2d73 7461 7475 7327 2c20 2023 2045   --status',  # E
-0000ed70: 6e73 7572 6520 7468 6520 6a6f 6220 7375  nsure the job su
-0000ed80: 6363 6565 6465 642e 0a20 2020 2020 2020  cceeded..       
-0000ed90: 2020 2020 2066 2773 6b79 2063 616e 6365       f'sky cance
-0000eda0: 6c20 2d79 207b 6e61 6d65 7d20 3127 2c0a  l -y {name} 1',.
-0000edb0: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
-0000edc0: 6570 2036 3027 2c0a 2020 2020 2020 2020  ep 60',.        
-0000edd0: 2020 2020 2320 6368 6563 6b20 6966 2074      # check if t
-0000ede0: 6865 2070 7974 686f 6e20 6a6f 6220 6973  he python job is
-0000edf0: 2067 6f6e 652e 0a20 2020 2020 2020 2020   gone..         
-0000ee00: 2020 2066 2773 6b79 2065 7865 6320 7b6e     f'sky exec {n
-0000ee10: 616d 657d 2022 2120 6e76 6964 6961 2d73  ame} "! nvidia-s
-0000ee20: 6d69 207c 2067 7265 7020 7079 7468 6f6e  mi | grep python
-0000ee30: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-0000ee40: 6627 736b 7920 6c6f 6773 207b 6e61 6d65  f'sky logs {name
-0000ee50: 7d20 3320 2d2d 7374 6174 7573 272c 2020  } 3 --status',  
-0000ee60: 2320 456e 7375 7265 2074 6865 206a 6f62  # Ensure the job
-0000ee70: 2073 7563 6365 6564 6564 2e0a 2020 2020   succeeded..    
-0000ee80: 2020 2020 5d2c 0a20 2020 2020 2020 2066      ],.        f
-0000ee90: 2773 6b79 2064 6f77 6e20 2d79 207b 6e61  'sky down -y {na
-0000eea0: 6d65 7d27 2c0a 2020 2020 2020 2020 7469  me}',.        ti
-0000eeb0: 6d65 6f75 743d 7469 6d65 6f75 742c 0a20  meout=timeout,. 
-0000eec0: 2020 2029 0a20 2020 2072 6574 7572 6e20     ).    return 
-0000eed0: 7465 7374 0a0a 0a23 202d 2d2d 2d2d 2d2d  test...# -------
-0000eee0: 2d2d 2d20 5465 7374 696e 6720 6073 6b79  --- Testing `sky
-0000eef0: 2063 616e 6365 6c60 202d 2d2d 2d2d 2d2d   cancel` -------
-0000ef00: 2d2d 2d0a 4070 7974 6573 742e 6d61 726b  ---.@pytest.mark
-0000ef10: 2e61 7773 0a64 6566 2074 6573 745f 6361  .aws.def test_ca
-0000ef20: 6e63 656c 5f61 7773 2829 3a0a 2020 2020  ncel_aws():.    
-0000ef30: 6e61 6d65 203d 205f 6765 745f 636c 7573  name = _get_clus
-0000ef40: 7465 725f 6e61 6d65 2829 0a20 2020 2074  ter_name().    t
-0000ef50: 6573 7420 3d20 5f67 6574 5f63 616e 6365  est = _get_cance
-0000ef60: 6c5f 7461 736b 5f77 6974 685f 636c 6f75  l_task_with_clou
-0000ef70: 6428 6e61 6d65 2c20 2761 7773 2729 0a20  d(name, 'aws'). 
-0000ef80: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
-0000ef90: 7465 7374 290a 0a0a 4070 7974 6573 742e  test)...@pytest.
-0000efa0: 6d61 726b 2e67 6370 0a64 6566 2074 6573  mark.gcp.def tes
-0000efb0: 745f 6361 6e63 656c 5f67 6370 2829 3a0a  t_cancel_gcp():.
-0000efc0: 2020 2020 6e61 6d65 203d 205f 6765 745f      name = _get_
-0000efd0: 636c 7573 7465 725f 6e61 6d65 2829 0a20  cluster_name(). 
-0000efe0: 2020 2074 6573 7420 3d20 5f67 6574 5f63     test = _get_c
-0000eff0: 616e 6365 6c5f 7461 736b 5f77 6974 685f  ancel_task_with_
-0000f000: 636c 6f75 6428 6e61 6d65 2c20 2767 6370  cloud(name, 'gcp
-0000f010: 2729 0a20 2020 2072 756e 5f6f 6e65 5f74  ').    run_one_t
-0000f020: 6573 7428 7465 7374 290a 0a0a 4070 7974  est(test)...@pyt
-0000f030: 6573 742e 6d61 726b 2e61 7a75 7265 0a64  est.mark.azure.d
-0000f040: 6566 2074 6573 745f 6361 6e63 656c 5f61  ef test_cancel_a
-0000f050: 7a75 7265 2829 3a0a 2020 2020 6e61 6d65  zure():.    name
-0000f060: 203d 205f 6765 745f 636c 7573 7465 725f   = _get_cluster_
-0000f070: 6e61 6d65 2829 0a20 2020 2074 6573 7420  name().    test 
-0000f080: 3d20 5f67 6574 5f63 616e 6365 6c5f 7461  = _get_cancel_ta
-0000f090: 736b 5f77 6974 685f 636c 6f75 6428 6e61  sk_with_cloud(na
-0000f0a0: 6d65 2c20 2761 7a75 7265 272c 2074 696d  me, 'azure', tim
-0000f0b0: 656f 7574 3d33 3020 2a20 3630 290a 2020  eout=30 * 60).  
-0000f0c0: 2020 7275 6e5f 6f6e 655f 7465 7374 2874    run_one_test(t
-0000f0d0: 6573 7429 0a0a 0a40 7079 7465 7374 2e6d  est)...@pytest.m
-0000f0e0: 6172 6b2e 6e6f 5f6c 616d 6264 615f 636c  ark.no_lambda_cl
-0000f0f0: 6f75 6420 2023 204c 616d 6264 6120 436c  oud  # Lambda Cl
-0000f100: 6f75 6420 646f 6573 206e 6f74 2068 6176  oud does not hav
-0000f110: 6520 5631 3030 2067 7075 730a 4070 7974  e V100 gpus.@pyt
-0000f120: 6573 742e 6d61 726b 2e6e 6f5f 6962 6d20  est.mark.no_ibm 
-0000f130: 2023 2049 424d 2063 6c6f 7564 2063 7572   # IBM cloud cur
-0000f140: 7265 6e74 6c79 2064 6f65 736e 2774 2070  rently doesn't p
-0000f150: 726f 7669 6465 2070 7562 6c69 6320 696d  rovide public im
-0000f160: 6167 6520 7769 7468 2043 5544 410a 4070  age with CUDA.@p
-0000f170: 7974 6573 742e 6d61 726b 2e6e 6f5f 7363  ytest.mark.no_sc
-0000f180: 7020 2023 2053 4350 2064 6f65 7320 6e6f  p  # SCP does no
-0000f190: 7420 7375 7070 6f72 7420 6e75 6d5f 6e6f  t support num_no
-0000f1a0: 6465 7320 3e20 3120 7965 740a 6465 6620  des > 1 yet.def 
-0000f1b0: 7465 7374 5f63 616e 6365 6c5f 7079 746f  test_cancel_pyto
-0000f1c0: 7263 6828 6765 6e65 7269 635f 636c 6f75  rch(generic_clou
-0000f1d0: 643a 2073 7472 293a 0a20 2020 206e 616d  d: str):.    nam
-0000f1e0: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
-0000f1f0: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
-0000f200: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
-0000f210: 2027 6361 6e63 656c 2d70 7974 6f72 6368   'cancel-pytorch
-0000f220: 272c 0a20 2020 2020 2020 205b 0a20 2020  ',.        [.   
-0000f230: 2020 2020 2020 2020 2066 2773 6b79 206c           f'sky l
-0000f240: 6175 6e63 6820 2d63 207b 6e61 6d65 7d20  aunch -c {name} 
-0000f250: 2d2d 636c 6f75 6420 7b67 656e 6572 6963  --cloud {generic
-0000f260: 5f63 6c6f 7564 7d20 6578 616d 706c 6573  _cloud} examples
-0000f270: 2f72 6573 6e65 745f 6469 7374 7269 6275  /resnet_distribu
-0000f280: 7465 645f 746f 7263 682e 7961 6d6c 202d  ted_torch.yaml -
-0000f290: 7920 2d64 272c 0a20 2020 2020 2020 2020  y -d',.         
-0000f2a0: 2020 2023 2057 6169 7420 7468 6520 4750     # Wait the GP
-0000f2b0: 5520 7072 6f63 6573 7320 746f 2073 7461  U process to sta
-0000f2c0: 7274 2e0a 2020 2020 2020 2020 2020 2020  rt..            
-0000f2d0: 2773 6c65 6570 2039 3027 2c0a 2020 2020  'sleep 90',.    
-0000f2e0: 2020 2020 2020 2020 6627 736b 7920 6578          f'sky ex
-0000f2f0: 6563 207b 6e61 6d65 7d20 226e 7669 6469  ec {name} "nvidi
-0000f300: 612d 736d 6920 7c20 6772 6570 2070 7974  a-smi | grep pyt
-0000f310: 686f 6e22 272c 0a20 2020 2020 2020 2020  hon"',.         
-0000f320: 2020 2066 2773 6b79 206c 6f67 7320 7b6e     f'sky logs {n
-0000f330: 616d 657d 2032 202d 2d73 7461 7475 7327  ame} 2 --status'
-0000f340: 2c20 2023 2045 6e73 7572 6520 7468 6520  ,  # Ensure the 
-0000f350: 6a6f 6220 7375 6363 6565 6465 642e 0a20  job succeeded.. 
-0000f360: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-0000f370: 2063 616e 6365 6c20 2d79 207b 6e61 6d65   cancel -y {name
-0000f380: 7d20 3127 2c0a 2020 2020 2020 2020 2020  } 1',.          
-0000f390: 2020 2773 6c65 6570 2036 3027 2c0a 2020    'sleep 60',.  
-0000f3a0: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
-0000f3b0: 6578 6563 207b 6e61 6d65 7d20 2228 6e76  exec {name} "(nv
-0000f3c0: 6964 6961 2d73 6d69 207c 2067 7265 7020  idia-smi | grep 
-0000f3d0: 5c27 4e6f 2072 756e 6e69 6e67 2070 726f  \'No running pro
-0000f3e0: 6365 7373 5c27 2920 7c7c 2027 0a20 2020  cess\') || '.   
-0000f3f0: 2020 2020 2020 2020 2023 2045 6e73 7572           # Ensur
-0000f400: 6520 586f 7267 2069 7320 7468 6520 6f6e  e Xorg is the on
-0000f410: 6c79 2070 726f 6365 7373 2072 756e 6e69  ly process runni
-0000f420: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
-0000f430: 275b 205c 2428 6e76 6964 6961 2d73 6d69  '[ \$(nvidia-smi
-0000f440: 207c 2067 7265 7020 2d41 2031 3020 5072   | grep -A 10 Pr
-0000f450: 6f63 6573 7365 7320 7c20 6772 6570 202d  ocesses | grep -
-0000f460: 4120 3130 203d 3d3d 207c 2067 7265 7020  A 10 === | grep 
-0000f470: 2d76 2058 6f72 6729 202d 6571 2032 205d  -v Xorg) -eq 2 ]
-0000f480: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-0000f490: 6627 736b 7920 6c6f 6773 207b 6e61 6d65  f'sky logs {name
-0000f4a0: 7d20 3320 2d2d 7374 6174 7573 272c 2020  } 3 --status',  
-0000f4b0: 2320 456e 7375 7265 2074 6865 206a 6f62  # Ensure the job
-0000f4c0: 2073 7563 6365 6564 6564 2e0a 2020 2020   succeeded..    
-0000f4d0: 2020 2020 5d2c 0a20 2020 2020 2020 2066      ],.        f
-0000f4e0: 2773 6b79 2064 6f77 6e20 2d79 207b 6e61  'sky down -y {na
-0000f4f0: 6d65 7d27 2c0a 2020 2020 2020 2020 7469  me}',.        ti
-0000f500: 6d65 6f75 743d 3230 202a 2036 302c 0a20  meout=20 * 60,. 
-0000f510: 2020 2029 0a20 2020 2072 756e 5f6f 6e65     ).    run_one
-0000f520: 5f74 6573 7428 7465 7374 290a 0a0a 2320  _test(test)...# 
-0000f530: 6361 6e27 7420 7573 6520 605f 6765 745f  can't use `_get_
-0000f540: 6361 6e63 656c 5f74 6173 6b5f 7769 7468  cancel_task_with
-0000f550: 5f63 6c6f 7564 2829 602c 2061 7320 636f  _cloud()`, as co
-0000f560: 6d6d 616e 6420 606e 7669 6469 612d 736d  mmand `nvidia-sm
-0000f570: 6960 0a23 2072 6571 7569 7265 7320 6120  i`.# requires a 
-0000f580: 4355 4441 2070 7562 6c69 6320 696d 6167  CUDA public imag
-0000f590: 652c 2077 6869 6368 2049 424d 2064 6f65  e, which IBM doe
-0000f5a0: 736e 2774 206f 6666 6572 0a40 7079 7465  sn't offer.@pyte
-0000f5b0: 7374 2e6d 6172 6b2e 6962 6d0a 6465 6620  st.mark.ibm.def 
-0000f5c0: 7465 7374 5f63 616e 6365 6c5f 6962 6d28  test_cancel_ibm(
-0000f5d0: 293a 0a20 2020 206e 616d 6520 3d20 5f67  ):.    name = _g
-0000f5e0: 6574 5f63 6c75 7374 6572 5f6e 616d 6528  et_cluster_name(
-0000f5f0: 290a 2020 2020 7465 7374 203d 2054 6573  ).    test = Tes
-0000f600: 7428 0a20 2020 2020 2020 2027 6962 6d2d  t(.        'ibm-
-0000f610: 6361 6e63 656c 2d74 6173 6b27 2c0a 2020  cancel-task',.  
-0000f620: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-0000f630: 2020 2020 6627 736b 7920 6c61 756e 6368      f'sky launch
-0000f640: 202d 7920 2d63 207b 6e61 6d65 7d20 2d2d   -y -c {name} --
-0000f650: 636c 6f75 6420 6962 6d20 6578 616d 706c  cloud ibm exampl
-0000f660: 6573 2f6d 696e 696d 616c 2e79 616d 6c27  es/minimal.yaml'
-0000f670: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-0000f680: 736b 7920 6578 6563 207b 6e61 6d65 7d20  sky exec {name} 
-0000f690: 2d6e 207b 6e61 6d65 7d2d 3120 2d64 2020  -n {name}-1 -d  
-0000f6a0: 2277 6869 6c65 2074 7275 653b 2064 6f20  "while true; do 
-0000f6b0: 6563 686f 205c 2748 656c 6c6f 2053 6b79  echo \'Hello Sky
-0000f6c0: 5069 6c6f 745c 273b 2073 6c65 6570 2032  Pilot\'; sleep 2
-0000f6d0: 3b20 646f 6e65 2227 2c0a 2020 2020 2020  ; done"',.      
-0000f6e0: 2020 2020 2020 2773 6c65 6570 2032 3027        'sleep 20'
-0000f6f0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-0000f700: 736b 7920 7175 6575 6520 7b6e 616d 657d  sky queue {name}
-0000f710: 207c 2067 7265 7020 7b6e 616d 657d 2d31   | grep {name}-1
-0000f720: 207c 2067 7265 7020 5255 4e4e 494e 4727   | grep RUNNING'
-0000f730: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-0000f740: 736b 7920 6361 6e63 656c 202d 7920 7b6e  sky cancel -y {n
-0000f750: 616d 657d 2032 272c 0a20 2020 2020 2020  ame} 2',.       
-0000f760: 2020 2020 2066 2773 6c65 6570 2035 272c       f'sleep 5',
-0000f770: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-0000f780: 6b79 2071 7565 7565 207b 6e61 6d65 7d20  ky queue {name} 
-0000f790: 7c20 6772 6570 207b 6e61 6d65 7d2d 3120  | grep {name}-1 
-0000f7a0: 7c20 6772 6570 2043 414e 4345 4c4c 4544  | grep CANCELLED
-0000f7b0: 272c 0a20 2020 2020 2020 205d 2c0a 2020  ',.        ],.  
-0000f7c0: 2020 2020 2020 6627 736b 7920 646f 776e        f'sky down
-0000f7d0: 202d 7920 7b6e 616d 657d 272c 0a20 2020   -y {name}',.   
-0000f7e0: 2029 0a20 2020 2072 756e 5f6f 6e65 5f74   ).    run_one_t
-0000f7f0: 6573 7428 7465 7374 290a 0a0a 2320 2d2d  est(test)...# --
-0000f800: 2d2d 2d2d 2d2d 2d2d 2054 6573 7469 6e67  -------- Testing
-0000f810: 2075 7365 2d73 706f 7420 6f70 7469 6f6e   use-spot option
-0000f820: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 4070 7974   ----------.@pyt
-0000f830: 6573 742e 6d61 726b 2e6e 6f5f 6c61 6d62  est.mark.no_lamb
-0000f840: 6461 5f63 6c6f 7564 2020 2320 4c61 6d62  da_cloud  # Lamb
-0000f850: 6461 2043 6c6f 7564 2064 6f65 7320 6e6f  da Cloud does no
-0000f860: 7420 7375 7070 6f72 7420 7370 6f74 2069  t support spot i
-0000f870: 6e73 7461 6e63 6573 0a40 7079 7465 7374  nstances.@pytest
-0000f880: 2e6d 6172 6b2e 6e6f 5f69 626d 2020 2320  .mark.no_ibm  # 
-0000f890: 4942 4d20 436c 6f75 6420 646f 6573 206e  IBM Cloud does n
-0000f8a0: 6f74 2073 7570 706f 7274 2073 706f 7420  ot support spot 
-0000f8b0: 696e 7374 616e 6365 730a 4070 7974 6573  instances.@pytes
-0000f8c0: 742e 6d61 726b 2e6e 6f5f 7363 7020 2023  t.mark.no_scp  #
-0000f8d0: 2053 4350 2064 6f65 7320 6e6f 7420 7375   SCP does not su
-0000f8e0: 7070 6f72 7420 7370 6f74 2069 6e73 7461  pport spot insta
-0000f8f0: 6e63 6573 0a64 6566 2074 6573 745f 7573  nces.def test_us
-0000f900: 655f 7370 6f74 2867 656e 6572 6963 5f63  e_spot(generic_c
-0000f910: 6c6f 7564 3a20 7374 7229 3a0a 2020 2020  loud: str):.    
-0000f920: 2222 2254 6573 7420 7573 652d 7370 6f74  """Test use-spot
-0000f930: 2061 6e64 2073 6b79 2065 7865 632e 2222   and sky exec.""
-0000f940: 220a 2020 2020 6e61 6d65 203d 205f 6765  ".    name = _ge
-0000f950: 745f 636c 7573 7465 725f 6e61 6d65 2829  t_cluster_name()
-0000f960: 0a20 2020 2074 6573 7420 3d20 5465 7374  .    test = Test
-0000f970: 280a 2020 2020 2020 2020 2775 7365 2d73  (.        'use-s
-0000f980: 706f 7427 2c0a 2020 2020 2020 2020 5b0a  pot',.        [.
-0000f990: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-0000f9a0: 7920 6c61 756e 6368 202d 6320 7b6e 616d  y launch -c {nam
-0000f9b0: 657d 202d 2d63 6c6f 7564 207b 6765 6e65  e} --cloud {gene
-0000f9c0: 7269 635f 636c 6f75 647d 2074 6573 7473  ric_cloud} tests
-0000f9d0: 2f74 6573 745f 7961 6d6c 732f 6d69 6e69  /test_yamls/mini
-0000f9e0: 6d61 6c2e 7961 6d6c 202d 2d75 7365 2d73  mal.yaml --use-s
-0000f9f0: 706f 7420 2d79 272c 0a20 2020 2020 2020  pot -y',.       
-0000fa00: 2020 2020 2066 2773 6b79 206c 6f67 7320       f'sky logs 
-0000fa10: 7b6e 616d 657d 2031 202d 2d73 7461 7475  {name} 1 --statu
-0000fa20: 7327 2c0a 2020 2020 2020 2020 2020 2020  s',.            
-0000fa30: 6627 736b 7920 6578 6563 207b 6e61 6d65  f'sky exec {name
-0000fa40: 7d20 6563 686f 2068 6927 2c0a 2020 2020  } echo hi',.    
-0000fa50: 2020 2020 2020 2020 6627 736b 7920 6c6f          f'sky lo
-0000fa60: 6773 207b 6e61 6d65 7d20 3220 2d2d 7374  gs {name} 2 --st
-0000fa70: 6174 7573 272c 0a20 2020 2020 2020 205d  atus',.        ]
-0000fa80: 2c0a 2020 2020 2020 2020 6627 736b 7920  ,.        f'sky 
-0000fa90: 646f 776e 202d 7920 7b6e 616d 657d 272c  down -y {name}',
-0000faa0: 0a20 2020 2029 0a20 2020 2072 756e 5f6f  .    ).    run_o
-0000fab0: 6e65 5f74 6573 7428 7465 7374 290a 0a0a  ne_test(test)...
-0000fac0: 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2054 6573  # ---------- Tes
-0000fad0: 7469 6e67 206d 616e 6167 6564 2073 706f  ting managed spo
-0000fae0: 7420 2d2d 2d2d 2d2d 2d2d 2d2d 0a40 7079  t ----------.@py
-0000faf0: 7465 7374 2e6d 6172 6b2e 6e6f 5f6c 616d  test.mark.no_lam
-0000fb00: 6264 615f 636c 6f75 6420 2023 204c 616d  bda_cloud  # Lam
-0000fb10: 6264 6120 436c 6f75 6420 646f 6573 206e  bda Cloud does n
-0000fb20: 6f74 2073 7570 706f 7274 2073 706f 7420  ot support spot 
-0000fb30: 696e 7374 616e 6365 730a 4070 7974 6573  instances.@pytes
-0000fb40: 742e 6d61 726b 2e6e 6f5f 6962 6d20 2023  t.mark.no_ibm  #
-0000fb50: 2049 424d 2043 6c6f 7564 2064 6f65 7320   IBM Cloud does 
-0000fb60: 6e6f 7420 7375 7070 6f72 7420 7370 6f74  not support spot
-0000fb70: 2069 6e73 7461 6e63 6573 0a40 7079 7465   instances.@pyte
-0000fb80: 7374 2e6d 6172 6b2e 6e6f 5f73 6370 2020  st.mark.no_scp  
-0000fb90: 2320 5343 5020 646f 6573 206e 6f74 2073  # SCP does not s
-0000fba0: 7570 706f 7274 2073 706f 7420 696e 7374  upport spot inst
-0000fbb0: 616e 6365 730a 4070 7974 6573 742e 6d61  ances.@pytest.ma
-0000fbc0: 726b 2e6d 616e 6167 6564 5f73 706f 740a  rk.managed_spot.
-0000fbd0: 6465 6620 7465 7374 5f73 706f 7428 6765  def test_spot(ge
-0000fbe0: 6e65 7269 635f 636c 6f75 643a 2073 7472  neric_cloud: str
-0000fbf0: 293a 0a20 2020 2022 2222 5465 7374 2074  ):.    """Test t
-0000fc00: 6865 2073 706f 7420 7961 6d6c 2e22 2222  he spot yaml."""
-0000fc10: 0a20 2020 206e 616d 6520 3d20 5f67 6574  .    name = _get
-0000fc20: 5f63 6c75 7374 6572 5f6e 616d 6528 290a  _cluster_name().
-0000fc30: 2020 2020 7465 7374 203d 2054 6573 7428      test = Test(
-0000fc40: 0a20 2020 2020 2020 2027 6d61 6e61 6765  .        'manage
-0000fc50: 642d 7370 6f74 272c 0a20 2020 2020 2020  d-spot',.       
-0000fc60: 205b 0a20 2020 2020 2020 2020 2020 2066   [.            f
-0000fc70: 2773 6b79 2073 706f 7420 6c61 756e 6368  'sky spot launch
-0000fc80: 202d 6e20 7b6e 616d 657d 2d31 202d 2d63   -n {name}-1 --c
-0000fc90: 6c6f 7564 207b 6765 6e65 7269 635f 636c  loud {generic_cl
-0000fca0: 6f75 647d 2065 7861 6d70 6c65 732f 6d61  oud} examples/ma
-0000fcb0: 6e61 6765 645f 7370 6f74 2e79 616d 6c20  naged_spot.yaml 
-0000fcc0: 2d79 202d 6427 2c0a 2020 2020 2020 2020  -y -d',.        
-0000fcd0: 2020 2020 6627 736b 7920 7370 6f74 206c      f'sky spot l
-0000fce0: 6175 6e63 6820 2d6e 207b 6e61 6d65 7d2d  aunch -n {name}-
-0000fcf0: 3220 2d2d 636c 6f75 6420 7b67 656e 6572  2 --cloud {gener
-0000fd00: 6963 5f63 6c6f 7564 7d20 6578 616d 706c  ic_cloud} exampl
-0000fd10: 6573 2f6d 616e 6167 6564 5f73 706f 742e  es/managed_spot.
-0000fd20: 7961 6d6c 202d 7920 2d64 272c 0a20 2020  yaml -y -d',.   
-0000fd30: 2020 2020 2020 2020 2027 736c 6565 7020           'sleep 
-0000fd40: 3527 2c0a 2020 2020 2020 2020 2020 2020  5',.            
-0000fd50: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
-0000fd60: 4149 547d 7c20 6772 6570 207b 6e61 6d65  AIT}| grep {name
-0000fd70: 7d2d 3120 7c20 6865 6164 202d 6e31 207c  }-1 | head -n1 |
-0000fd80: 2067 7265 7020 2253 5441 5254 494e 475c   grep "STARTING\
-0000fd90: 7c52 554e 4e49 4e47 2227 2c0a 2020 2020  |RUNNING"',.    
-0000fda0: 2020 2020 2020 2020 6627 7b5f 5350 4f54          f'{_SPOT
-0000fdb0: 5f51 5545 5545 5f57 4149 547d 7c20 6772  _QUEUE_WAIT}| gr
-0000fdc0: 6570 207b 6e61 6d65 7d2d 3220 7c20 6865  ep {name}-2 | he
-0000fdd0: 6164 202d 6e31 207c 2067 7265 7020 2253  ad -n1 | grep "S
-0000fde0: 5441 5254 494e 475c 7c52 554e 4e49 4e47  TARTING\|RUNNING
-0000fdf0: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-0000fe00: 5f53 504f 545f 4341 4e43 454c 5f57 4149  _SPOT_CANCEL_WAI
-0000fe10: 542e 666f 726d 6174 286a 6f62 5f6e 616d  T.format(job_nam
-0000fe20: 653d 6627 7b6e 616d 657d 2d31 2729 2c0a  e=f'{name}-1'),.
-0000fe30: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
-0000fe40: 6570 2035 272c 0a20 2020 2020 2020 2020  ep 5',.         
-0000fe50: 2020 2066 277b 5f53 504f 545f 5155 4555     f'{_SPOT_QUEU
-0000fe60: 455f 5741 4954 7d7c 2067 7265 7020 7b6e  E_WAIT}| grep {n
-0000fe70: 616d 657d 2d31 207c 2068 6561 6420 2d6e  ame}-1 | head -n
-0000fe80: 3120 7c20 6772 6570 2022 4341 4e43 454c  1 | grep "CANCEL
-0000fe90: 4c49 4e47 5c7c 4341 4e43 454c 4c45 4422  LING\|CANCELLED"
-0000fea0: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
-0000feb0: 736c 6565 7020 3230 3027 2c0a 2020 2020  sleep 200',.    
-0000fec0: 2020 2020 2020 2020 6627 7b5f 5350 4f54          f'{_SPOT
-0000fed0: 5f51 5545 5545 5f57 4149 547d 7c20 6772  _QUEUE_WAIT}| gr
-0000fee0: 6570 207b 6e61 6d65 7d2d 3120 7c20 6865  ep {name}-1 | he
-0000fef0: 6164 202d 6e31 207c 2067 7265 7020 4341  ad -n1 | grep CA
-0000ff00: 4e43 454c 4c45 4427 2c0a 2020 2020 2020  NCELLED',.      
-0000ff10: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
-0000ff20: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
-0000ff30: 207b 6e61 6d65 7d2d 3220 7c20 6865 6164   {name}-2 | head
-0000ff40: 202d 6e31 207c 2067 7265 7020 2252 554e   -n1 | grep "RUN
-0000ff50: 4e49 4e47 5c7c 5355 4343 4545 4445 4422  NING\|SUCCEEDED"
-0000ff60: 272c 0a20 2020 2020 2020 205d 2c0a 2020  ',.        ],.  
-0000ff70: 2020 2020 2020 2320 544f 444f 287a 6877        # TODO(zhw
-0000ff80: 7529 3a20 4368 616e 6765 2074 6f20 5f53  u): Change to _S
-0000ff90: 504f 545f 4341 4e43 454c 5f57 4149 542e  POT_CANCEL_WAIT.
-0000ffa0: 666f 726d 6174 286a 6f62 5f6e 616d 653d  format(job_name=
-0000ffb0: 6627 7b6e 616d 657d 2d31 202d 6e20 7b6e  f'{name}-1 -n {n
-0000ffc0: 616d 657d 2d32 2729 2077 6865 6e0a 2020  ame}-2') when.  
-0000ffd0: 2020 2020 2020 2320 6361 6e63 656c 696e        # cancelin
-0000ffe0: 6720 6d75 6c74 6970 6c65 206a 6f62 206e  g multiple job n
-0000fff0: 616d 6573 2069 7320 7375 7070 6f72 7465  ames is supporte
-00010000: 642e 0a20 2020 2020 2020 2028 5f53 504f  d..        (_SPO
-00010010: 545f 4341 4e43 454c 5f57 4149 542e 666f  T_CANCEL_WAIT.fo
-00010020: 726d 6174 286a 6f62 5f6e 616d 653d 6627  rmat(job_name=f'
-00010030: 7b6e 616d 657d 2d31 2729 202b 2027 3b20  {name}-1') + '; 
-00010040: 2720 2b0a 2020 2020 2020 2020 205f 5350  ' +.         _SP
-00010050: 4f54 5f43 414e 4345 4c5f 5741 4954 2e66  OT_CANCEL_WAIT.f
-00010060: 6f72 6d61 7428 6a6f 625f 6e61 6d65 3d66  ormat(job_name=f
-00010070: 277b 6e61 6d65 7d2d 3227 2929 2c0a 2020  '{name}-2')),.  
-00010080: 2020 2020 2020 2320 496e 6372 6561 7365        # Increase
-00010090: 2074 696d 656f 7574 2073 696e 6365 2073   timeout since s
-000100a0: 6b79 2073 706f 7420 7175 6575 6520 2d72  ky spot queue -r
-000100b0: 2063 616e 2062 6520 626c 6f63 6b65 6420   can be blocked 
-000100c0: 6279 206f 7468 6572 2073 706f 7420 7465  by other spot te
-000100d0: 7374 732e 0a20 2020 2020 2020 2074 696d  sts..        tim
-000100e0: 656f 7574 3d32 3020 2a20 3630 2c0a 2020  eout=20 * 60,.  
-000100f0: 2020 290a 2020 2020 7275 6e5f 6f6e 655f    ).    run_one_
-00010100: 7465 7374 2874 6573 7429 0a0a 0a40 7079  test(test)...@py
-00010110: 7465 7374 2e6d 6172 6b2e 6e6f 5f6c 616d  test.mark.no_lam
-00010120: 6264 615f 636c 6f75 6420 2023 204c 616d  bda_cloud  # Lam
-00010130: 6264 6120 436c 6f75 6420 646f 6573 206e  bda Cloud does n
-00010140: 6f74 2073 7570 706f 7274 2073 706f 7420  ot support spot 
-00010150: 696e 7374 616e 6365 730a 4070 7974 6573  instances.@pytes
-00010160: 742e 6d61 726b 2e6e 6f5f 6962 6d20 2023  t.mark.no_ibm  #
-00010170: 2049 424d 2043 6c6f 7564 2064 6f65 7320   IBM Cloud does 
-00010180: 6e6f 7420 7375 7070 6f72 7420 7370 6f74  not support spot
-00010190: 2069 6e73 7461 6e63 6573 0a40 7079 7465   instances.@pyte
-000101a0: 7374 2e6d 6172 6b2e 6e6f 5f73 6370 2020  st.mark.no_scp  
-000101b0: 2320 5343 5020 646f 6573 206e 6f74 2073  # SCP does not s
-000101c0: 7570 706f 7274 2073 706f 7420 696e 7374  upport spot inst
-000101d0: 616e 6365 730a 4070 7974 6573 742e 6d61  ances.@pytest.ma
-000101e0: 726b 2e6d 616e 6167 6564 5f73 706f 740a  rk.managed_spot.
-000101f0: 6465 6620 7465 7374 5f73 706f 745f 7069  def test_spot_pi
-00010200: 7065 6c69 6e65 2867 656e 6572 6963 5f63  peline(generic_c
-00010210: 6c6f 7564 3a20 7374 7229 3a0a 2020 2020  loud: str):.    
-00010220: 2222 2254 6573 7420 6120 7370 6f74 c2a0  """Test a spot..
-00010230: 7069 7065 6c69 6e65 2e22 2222 0a20 2020  pipeline.""".   
-00010240: 206e 616d 6520 3d20 5f67 6574 5f63 6c75   name = _get_clu
-00010250: 7374 6572 5f6e 616d 6528 290a 2020 2020  ster_name().    
-00010260: 7465 7374 203d 2054 6573 7428 0a20 2020  test = Test(.   
-00010270: 2020 2020 2027 7370 6f74 2d70 6970 656c       'spot-pipel
-00010280: 696e 6527 2c0a 2020 2020 2020 2020 5b0a  ine',.        [.
-00010290: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-000102a0: 7920 7370 6f74 206c 6175 6e63 6820 2d6e  y spot launch -n
-000102b0: 207b 6e61 6d65 7d20 7465 7374 732f 7465   {name} tests/te
-000102c0: 7374 5f79 616d 6c73 2f70 6970 656c 696e  st_yamls/pipelin
-000102d0: 652e 7961 6d6c 202d 7920 2d64 272c 0a20  e.yaml -y -d',. 
-000102e0: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
-000102f0: 7020 3527 2c0a 2020 2020 2020 2020 2020  p 5',.          
-00010300: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
-00010310: 5f57 4149 547d 7c20 6772 6570 207b 6e61  _WAIT}| grep {na
-00010320: 6d65 7d20 7c20 6865 6164 202d 6e31 207c  me} | head -n1 |
-00010330: 2067 7265 7020 2253 5441 5254 494e 475c   grep "STARTING\
-00010340: 7c52 554e 4e49 4e47 2227 2c0a 2020 2020  |RUNNING"',.    
-00010350: 2020 2020 2020 2020 2320 6067 7265 7020          # `grep 
-00010360: 2d41 2034 207b 6e61 6d65 7d60 2066 696e  -A 4 {name}` fin
-00010370: 6473 2074 6865 206a 6f62 2077 6974 6820  ds the job with 
-00010380: 7b6e 616d 657d 2061 6e64 2074 6865 2034  {name} and the 4
-00010390: 206c 696e 6573 0a20 2020 2020 2020 2020   lines.         
-000103a0: 2020 2023 2061 6674 6572 2069 742c 2069     # after it, i
-000103b0: 2e65 2e20 7468 6520 3420 7461 736b 7320  .e. the 4 tasks 
-000103c0: 7769 7468 696e 2074 6865 206a 6f62 2e0a  within the job..
-000103d0: 2020 2020 2020 2020 2020 2020 2320 6073              # `s
-000103e0: 6564 202d 6e20 3270 6020 6765 7473 2074  ed -n 2p` gets t
-000103f0: 6865 2073 6563 6f6e 6420 6c69 6e65 206f  he second line o
-00010400: 6620 7468 6520 3420 6c69 6e65 732c 2069  f the 4 lines, i
-00010410: 2e65 2e20 7468 6520 6669 7273 740a 2020  .e. the first.  
-00010420: 2020 2020 2020 2020 2020 2320 7461 736b            # task
-00010430: 2077 6974 6869 6e20 7468 6520 6a6f 622e   within the job.
-00010440: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
-00010450: 5f53 504f 545f 5155 4555 455f 5741 4954  _SPOT_QUEUE_WAIT
-00010460: 7d7c 2067 7265 7020 2d41 2034 207b 6e61  }| grep -A 4 {na
-00010470: 6d65 7d7c 2073 6564 202d 6e20 3270 207c  me}| sed -n 2p |
-00010480: 2067 7265 7020 2253 5441 5254 494e 475c   grep "STARTING\
-00010490: 7c52 554e 4e49 4e47 2227 2c0a 2020 2020  |RUNNING"',.    
-000104a0: 2020 2020 2020 2020 6627 7b5f 5350 4f54          f'{_SPOT
-000104b0: 5f51 5545 5545 5f57 4149 547d 7c20 6772  _QUEUE_WAIT}| gr
-000104c0: 6570 202d 4120 3420 7b6e 616d 657d 7c20  ep -A 4 {name}| 
-000104d0: 7365 6420 2d6e 2033 7020 7c20 6772 6570  sed -n 3p | grep
-000104e0: 2022 5045 4e44 494e 4722 272c 0a20 2020   "PENDING"',.   
-000104f0: 2020 2020 2020 2020 205f 5350 4f54 5f43           _SPOT_C
-00010500: 414e 4345 4c5f 5741 4954 2e66 6f72 6d61  ANCEL_WAIT.forma
-00010510: 7428 6a6f 625f 6e61 6d65 3d66 277b 6e61  t(job_name=f'{na
-00010520: 6d65 7d27 292c 0a20 2020 2020 2020 2020  me}'),.         
-00010530: 2020 2027 736c 6565 7020 3527 2c0a 2020     'sleep 5',.  
-00010540: 2020 2020 2020 2020 2020 6627 7b5f 5350            f'{_SP
-00010550: 4f54 5f51 5545 5545 5f57 4149 547d 7c20  OT_QUEUE_WAIT}| 
-00010560: 6772 6570 202d 4120 3420 7b6e 616d 657d  grep -A 4 {name}
-00010570: 7c20 7365 6420 2d6e 2032 7020 7c20 6772  | sed -n 2p | gr
-00010580: 6570 2022 4341 4e43 454c 4c49 4e47 5c7c  ep "CANCELLING\|
-00010590: 4341 4e43 454c 4c45 4422 272c 0a20 2020  CANCELLED"',.   
-000105a0: 2020 2020 2020 2020 2066 277b 5f53 504f           f'{_SPO
-000105b0: 545f 5155 4555 455f 5741 4954 7d7c 2067  T_QUEUE_WAIT}| g
-000105c0: 7265 7020 2d41 2034 207b 6e61 6d65 7d7c  rep -A 4 {name}|
-000105d0: 2073 6564 202d 6e20 3370 207c 2067 7265   sed -n 3p | gre
-000105e0: 7020 2243 414e 4345 4c4c 494e 475c 7c43  p "CANCELLING\|C
-000105f0: 414e 4345 4c4c 4544 2227 2c0a 2020 2020  ANCELLED"',.    
-00010600: 2020 2020 2020 2020 6627 7b5f 5350 4f54          f'{_SPOT
-00010610: 5f51 5545 5545 5f57 4149 547d 7c20 6772  _QUEUE_WAIT}| gr
-00010620: 6570 202d 4120 3420 7b6e 616d 657d 7c20  ep -A 4 {name}| 
-00010630: 7365 6420 2d6e 2034 7020 7c20 6772 6570  sed -n 4p | grep
-00010640: 2022 4341 4e43 454c 4c49 4e47 5c7c 4341   "CANCELLING\|CA
-00010650: 4e43 454c 4c45 4422 272c 0a20 2020 2020  NCELLED"',.     
-00010660: 2020 2020 2020 2066 277b 5f53 504f 545f         f'{_SPOT_
-00010670: 5155 4555 455f 5741 4954 7d7c 2067 7265  QUEUE_WAIT}| gre
-00010680: 7020 2d41 2034 207b 6e61 6d65 7d7c 2073  p -A 4 {name}| s
-00010690: 6564 202d 6e20 3570 207c 2067 7265 7020  ed -n 5p | grep 
-000106a0: 2243 414e 4345 4c4c 494e 475c 7c43 414e  "CANCELLING\|CAN
-000106b0: 4345 4c4c 4544 2227 2c0a 2020 2020 2020  CELLED"',.      
-000106c0: 2020 2020 2020 2773 6c65 6570 2032 3030        'sleep 200
-000106d0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-000106e0: 277b 5f53 504f 545f 5155 4555 455f 5741  '{_SPOT_QUEUE_WA
-000106f0: 4954 7d7c 2067 7265 7020 2d41 2034 207b  IT}| grep -A 4 {
-00010700: 6e61 6d65 7d7c 2073 6564 202d 6e20 3270  name}| sed -n 2p
-00010710: 207c 2067 7265 7020 2243 414e 4345 4c4c   | grep "CANCELL
-00010720: 4544 2227 2c0a 2020 2020 2020 2020 2020  ED"',.          
-00010730: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
-00010740: 5f57 4149 547d 7c20 6772 6570 202d 4120  _WAIT}| grep -A 
-00010750: 3420 7b6e 616d 657d 7c20 7365 6420 2d6e  4 {name}| sed -n
-00010760: 2033 7020 7c20 6772 6570 2022 4341 4e43   3p | grep "CANC
-00010770: 454c 4c45 4422 272c 0a20 2020 2020 2020  ELLED"',.       
-00010780: 2020 2020 2066 277b 5f53 504f 545f 5155       f'{_SPOT_QU
-00010790: 4555 455f 5741 4954 7d7c 2067 7265 7020  EUE_WAIT}| grep 
-000107a0: 2d41 2034 207b 6e61 6d65 7d7c 2073 6564  -A 4 {name}| sed
-000107b0: 202d 6e20 3470 207c 2067 7265 7020 2243   -n 4p | grep "C
-000107c0: 414e 4345 4c4c 4544 2227 2c0a 2020 2020  ANCELLED"',.    
-000107d0: 2020 2020 2020 2020 6627 7b5f 5350 4f54          f'{_SPOT
-000107e0: 5f51 5545 5545 5f57 4149 547d 7c20 6772  _QUEUE_WAIT}| gr
-000107f0: 6570 202d 4120 3420 7b6e 616d 657d 7c20  ep -A 4 {name}| 
-00010800: 7365 6420 2d6e 2035 7020 7c20 6772 6570  sed -n 5p | grep
-00010810: 2022 4341 4e43 454c 4c45 4422 272c 0a20   "CANCELLED"',. 
-00010820: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-00010830: 2020 5f53 504f 545f 4341 4e43 454c 5f57    _SPOT_CANCEL_W
-00010840: 4149 542e 666f 726d 6174 286a 6f62 5f6e  AIT.format(job_n
-00010850: 616d 653d 6627 7b6e 616d 657d 2729 2c0a  ame=f'{name}'),.
-00010860: 2020 2020 2020 2020 2320 496e 6372 6561          # Increa
-00010870: 7365 2074 696d 656f 7574 2073 696e 6365  se timeout since
-00010880: 2073 6b79 2073 706f 7420 7175 6575 6520   sky spot queue 
-00010890: 2d72 2063 616e 2062 6520 626c 6f63 6b65  -r can be blocke
-000108a0: 6420 6279 206f 7468 6572 2073 706f 7420  d by other spot 
-000108b0: 7465 7374 732e 0a20 2020 2020 2020 2074  tests..        t
-000108c0: 696d 656f 7574 3d33 3020 2a20 3630 2c0a  imeout=30 * 60,.
-000108d0: 2020 2020 290a 2020 2020 7275 6e5f 6f6e      ).    run_on
-000108e0: 655f 7465 7374 2874 6573 7429 0a0a 0a40  e_test(test)...@
-000108f0: 7079 7465 7374 2e6d 6172 6b2e 6e6f 5f6c  pytest.mark.no_l
-00010900: 616d 6264 615f 636c 6f75 6420 2023 204c  ambda_cloud  # L
-00010910: 616d 6264 6120 436c 6f75 6420 646f 6573  ambda Cloud does
-00010920: 206e 6f74 2073 7570 706f 7274 2073 706f   not support spo
-00010930: 7420 696e 7374 616e 6365 730a 4070 7974  t instances.@pyt
-00010940: 6573 742e 6d61 726b 2e6e 6f5f 6962 6d20  est.mark.no_ibm 
-00010950: 2023 2049 424d 2043 6c6f 7564 2064 6f65   # IBM Cloud doe
-00010960: 7320 6e6f 7420 7375 7070 6f72 7420 7370  s not support sp
-00010970: 6f74 2069 6e73 7461 6e63 6573 0a40 7079  ot instances.@py
-00010980: 7465 7374 2e6d 6172 6b2e 6e6f 5f73 6370  test.mark.no_scp
-00010990: 2020 2320 5343 5020 646f 6573 206e 6f74    # SCP does not
-000109a0: 2073 7570 706f 7274 2073 706f 7420 696e   support spot in
-000109b0: 7374 616e 6365 730a 4070 7974 6573 742e  stances.@pytest.
-000109c0: 6d61 726b 2e6d 616e 6167 6564 5f73 706f  mark.managed_spo
-000109d0: 740a 6465 6620 7465 7374 5f73 706f 745f  t.def test_spot_
-000109e0: 6661 696c 6564 5f73 6574 7570 2867 656e  failed_setup(gen
-000109f0: 6572 6963 5f63 6c6f 7564 3a20 7374 7229  eric_cloud: str)
-00010a00: 3a0a 2020 2020 2222 2254 6573 7420 6d61  :.    """Test ma
-00010a10: 6e61 6765 6420 7370 6f74 206a 6f62 2077  naged spot job w
-00010a20: 6974 6820 6661 696c 6564 2073 6574 7570  ith failed setup
-00010a30: 2e22 2222 0a20 2020 206e 616d 6520 3d20  .""".    name = 
-00010a40: 5f67 6574 5f63 6c75 7374 6572 5f6e 616d  _get_cluster_nam
-00010a50: 6528 290a 2020 2020 7465 7374 203d 2054  e().    test = T
-00010a60: 6573 7428 0a20 2020 2020 2020 2027 7370  est(.        'sp
-00010a70: 6f74 5f66 6169 6c65 645f 7365 7475 7027  ot_failed_setup'
-00010a80: 2c0a 2020 2020 2020 2020 5b0a 2020 2020  ,.        [.    
-00010a90: 2020 2020 2020 2020 6627 736b 7920 7370          f'sky sp
-00010aa0: 6f74 206c 6175 6e63 6820 2d6e 207b 6e61  ot launch -n {na
-00010ab0: 6d65 7d20 2d2d 636c 6f75 6420 7b67 656e  me} --cloud {gen
-00010ac0: 6572 6963 5f63 6c6f 7564 7d20 2d79 202d  eric_cloud} -y -
-00010ad0: 6420 7465 7374 732f 7465 7374 5f79 616d  d tests/test_yam
-00010ae0: 6c73 2f66 6169 6c65 645f 7365 7475 702e  ls/failed_setup.
-00010af0: 7961 6d6c 272c 0a20 2020 2020 2020 2020  yaml',.         
-00010b00: 2020 2027 736c 6565 7020 3333 3027 2c0a     'sleep 330',.
-00010b10: 2020 2020 2020 2020 2020 2020 2320 4d61              # Ma
-00010b20: 6b65 2073 7572 6520 7468 6520 6a6f 6220  ke sure the job 
-00010b30: 6661 696c 6564 2071 7569 636b 6c79 2e0a  failed quickly..
-00010b40: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
-00010b50: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
-00010b60: 207c 2067 7265 7020 7b6e 616d 657d 207c   | grep {name} |
-00010b70: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
-00010b80: 2022 4641 494c 4544 5f53 4554 5550 2227   "FAILED_SETUP"'
-00010b90: 2c0a 2020 2020 2020 2020 5d2c 0a20 2020  ,.        ],.   
-00010ba0: 2020 2020 205f 5350 4f54 5f43 414e 4345       _SPOT_CANCE
-00010bb0: 4c5f 5741 4954 2e66 6f72 6d61 7428 6a6f  L_WAIT.format(jo
-00010bc0: 625f 6e61 6d65 3d6e 616d 6529 2c0a 2020  b_name=name),.  
-00010bd0: 2020 2020 2020 2320 496e 6372 6561 7365        # Increase
-00010be0: 2074 696d 656f 7574 2073 696e 6365 2073   timeout since s
-00010bf0: 6b79 2073 706f 7420 7175 6575 6520 2d72  ky spot queue -r
-00010c00: 2063 616e 2062 6520 626c 6f63 6b65 6420   can be blocked 
-00010c10: 6279 206f 7468 6572 2073 706f 7420 7465  by other spot te
-00010c20: 7374 732e 0a20 2020 2020 2020 2074 696d  sts..        tim
-00010c30: 656f 7574 3d32 3020 2a20 3630 2c0a 2020  eout=20 * 60,.  
-00010c40: 2020 290a 2020 2020 7275 6e5f 6f6e 655f    ).    run_one_
-00010c50: 7465 7374 2874 6573 7429 0a0a 0a40 7079  test(test)...@py
-00010c60: 7465 7374 2e6d 6172 6b2e 6e6f 5f6c 616d  test.mark.no_lam
-00010c70: 6264 615f 636c 6f75 6420 2023 204c 616d  bda_cloud  # Lam
-00010c80: 6264 6120 436c 6f75 6420 646f 6573 206e  bda Cloud does n
-00010c90: 6f74 2073 7570 706f 7274 2073 706f 7420  ot support spot 
-00010ca0: 696e 7374 616e 6365 730a 4070 7974 6573  instances.@pytes
-00010cb0: 742e 6d61 726b 2e6e 6f5f 6962 6d20 2023  t.mark.no_ibm  #
-00010cc0: 2049 424d 2043 6c6f 7564 2064 6f65 7320   IBM Cloud does 
-00010cd0: 6e6f 7420 7375 7070 6f72 7420 7370 6f74  not support spot
-00010ce0: 2069 6e73 7461 6e63 6573 0a40 7079 7465   instances.@pyte
-00010cf0: 7374 2e6d 6172 6b2e 6e6f 5f73 6370 2020  st.mark.no_scp  
-00010d00: 2320 5343 5020 646f 6573 206e 6f74 2073  # SCP does not s
-00010d10: 7570 706f 7274 2073 706f 7420 696e 7374  upport spot inst
-00010d20: 616e 6365 730a 4070 7974 6573 742e 6d61  ances.@pytest.ma
-00010d30: 726b 2e6d 616e 6167 6564 5f73 706f 740a  rk.managed_spot.
-00010d40: 6465 6620 7465 7374 5f73 706f 745f 7069  def test_spot_pi
-00010d50: 7065 6c69 6e65 5f66 6169 6c65 645f 7365  peline_failed_se
-00010d60: 7475 7028 6765 6e65 7269 635f 636c 6f75  tup(generic_clou
-00010d70: 643a 2073 7472 293a 0a20 2020 2022 2222  d: str):.    """
-00010d80: 5465 7374 206d 616e 6167 6564 2073 706f  Test managed spo
-00010d90: 7420 6a6f 6220 7769 7468 2066 6169 6c65  t job with faile
-00010da0: 6420 7365 7475 7020 666f 7220 6120 7069  d setup for a pi
-00010db0: 7065 6c69 6e65 2e22 2222 0a20 2020 206e  peline.""".    n
-00010dc0: 616d 6520 3d20 5f67 6574 5f63 6c75 7374  ame = _get_clust
-00010dd0: 6572 5f6e 616d 6528 290a 2020 2020 7465  er_name().    te
-00010de0: 7374 203d 2054 6573 7428 0a20 2020 2020  st = Test(.     
-00010df0: 2020 2027 7370 6f74 5f70 6970 656c 696e     'spot_pipelin
-00010e00: 655f 6661 696c 6564 5f73 6574 7570 272c  e_failed_setup',
-00010e10: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
-00010e20: 2020 2020 2020 2066 2773 6b79 2073 706f         f'sky spo
-00010e30: 7420 6c61 756e 6368 202d 6e20 7b6e 616d  t launch -n {nam
-00010e40: 657d 202d 7920 2d64 2074 6573 7473 2f74  e} -y -d tests/t
-00010e50: 6573 745f 7961 6d6c 732f 6661 696c 6564  est_yamls/failed
-00010e60: 5f73 6574 7570 5f70 6970 656c 696e 652e  _setup_pipeline.
-00010e70: 7961 6d6c 272c 0a20 2020 2020 2020 2020  yaml',.         
-00010e80: 2020 2027 736c 6565 7020 3830 3027 2c0a     'sleep 800',.
-00010e90: 2020 2020 2020 2020 2020 2020 2320 4d61              # Ma
-00010ea0: 6b65 2073 7572 6520 7468 6520 6a6f 6220  ke sure the job 
-00010eb0: 6661 696c 6564 2071 7569 636b 6c79 2e0a  failed quickly..
-00010ec0: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
-00010ed0: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
-00010ee0: 207c 2067 7265 7020 7b6e 616d 657d 207c   | grep {name} |
-00010ef0: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
-00010f00: 2022 4641 494c 4544 5f53 4554 5550 2227   "FAILED_SETUP"'
-00010f10: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
-00010f20: 5461 736b 2030 2073 686f 756c 6420 6265  Task 0 should be
-00010f30: 2053 5543 4345 4544 4544 2e0a 2020 2020   SUCCEEDED..    
-00010f40: 2020 2020 2020 2020 6627 7b5f 5350 4f54          f'{_SPOT
-00010f50: 5f51 5545 5545 5f57 4149 547d 207c 2067  _QUEUE_WAIT} | g
-00010f60: 7265 7020 2d41 2034 207b 6e61 6d65 7d7c  rep -A 4 {name}|
-00010f70: 2073 6564 202d 6e20 3270 207c 2067 7265   sed -n 2p | gre
-00010f80: 7020 2253 5543 4345 4544 4544 2227 2c0a  p "SUCCEEDED"',.
-00010f90: 2020 2020 2020 2020 2020 2020 2320 5461              # Ta
-00010fa0: 736b 2031 2073 686f 756c 6420 6265 2046  sk 1 should be F
-00010fb0: 4149 4c45 445f 5345 5455 502e 0a20 2020  AILED_SETUP..   
-00010fc0: 2020 2020 2020 2020 2066 277b 5f53 504f           f'{_SPO
-00010fd0: 545f 5155 4555 455f 5741 4954 7d20 7c20  T_QUEUE_WAIT} | 
-00010fe0: 6772 6570 202d 4120 3420 7b6e 616d 657d  grep -A 4 {name}
-00010ff0: 7c20 7365 6420 2d6e 2033 7020 7c20 6772  | sed -n 3p | gr
-00011000: 6570 2022 4641 494c 4544 5f53 4554 5550  ep "FAILED_SETUP
-00011010: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-00011020: 2320 5461 736b 2032 2073 686f 756c 6420  # Task 2 should 
-00011030: 6265 2043 414e 4345 4c4c 4544 2e0a 2020  be CANCELLED..  
-00011040: 2020 2020 2020 2020 2020 6627 7b5f 5350            f'{_SP
-00011050: 4f54 5f51 5545 5545 5f57 4149 547d 207c  OT_QUEUE_WAIT} |
-00011060: 2067 7265 7020 2d41 2034 207b 6e61 6d65   grep -A 4 {name
-00011070: 7d7c 2073 6564 202d 6e20 3470 207c 2067  }| sed -n 4p | g
-00011080: 7265 7020 2243 414e 4345 4c4c 4544 2227  rep "CANCELLED"'
-00011090: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
-000110a0: 5461 736b 2033 2073 686f 756c 6420 6265  Task 3 should be
-000110b0: 2043 414e 4345 4c4c 4544 2e0a 2020 2020   CANCELLED..    
-000110c0: 2020 2020 2020 2020 6627 7b5f 5350 4f54          f'{_SPOT
-000110d0: 5f51 5545 5545 5f57 4149 547d 207c 2067  _QUEUE_WAIT} | g
-000110e0: 7265 7020 2d41 2034 207b 6e61 6d65 7d7c  rep -A 4 {name}|
-000110f0: 2073 6564 202d 6e20 3570 207c 2067 7265   sed -n 5p | gre
-00011100: 7020 2243 414e 4345 4c4c 4544 2227 2c0a  p "CANCELLED"',.
-00011110: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00011120: 2020 205f 5350 4f54 5f43 414e 4345 4c5f     _SPOT_CANCEL_
-00011130: 5741 4954 2e66 6f72 6d61 7428 6a6f 625f  WAIT.format(job_
-00011140: 6e61 6d65 3d6e 616d 6529 2c0a 2020 2020  name=name),.    
-00011150: 2020 2020 2320 496e 6372 6561 7365 2074      # Increase t
-00011160: 696d 656f 7574 2073 696e 6365 2073 6b79  imeout since sky
-00011170: 2073 706f 7420 7175 6575 6520 2d72 2063   spot queue -r c
-00011180: 616e 2062 6520 626c 6f63 6b65 6420 6279  an be blocked by
-00011190: 206f 7468 6572 2073 706f 7420 7465 7374   other spot test
-000111a0: 732e 0a20 2020 2020 2020 2074 696d 656f  s..        timeo
-000111b0: 7574 3d33 3020 2a20 3630 2c0a 2020 2020  ut=30 * 60,.    
-000111c0: 290a 2020 2020 7275 6e5f 6f6e 655f 7465  ).    run_one_te
-000111d0: 7374 2874 6573 7429 0a0a 0a23 202d 2d2d  st(test)...# ---
-000111e0: 2d2d 2d2d 2d2d 2d20 5465 7374 696e 6720  ------- Testing 
-000111f0: 6d61 6e61 6765 6420 7370 6f74 2072 6563  managed spot rec
-00011200: 6f76 6572 7920 2d2d 2d2d 2d2d 2d2d 2d2d  overy ----------
-00011210: 0a0a 0a40 7079 7465 7374 2e6d 6172 6b2e  ...@pytest.mark.
-00011220: 6177 730a 4070 7974 6573 742e 6d61 726b  aws.@pytest.mark
-00011230: 2e6d 616e 6167 6564 5f73 706f 740a 6465  .managed_spot.de
-00011240: 6620 7465 7374 5f73 706f 745f 7265 636f  f test_spot_reco
-00011250: 7665 7279 5f61 7773 2861 7773 5f63 6f6e  very_aws(aws_con
-00011260: 6669 675f 7265 6769 6f6e 293a 0a20 2020  fig_region):.   
-00011270: 2022 2222 5465 7374 206d 616e 6167 6564   """Test managed
-00011280: 2073 706f 7420 7265 636f 7665 7279 2e22   spot recovery."
-00011290: 2222 0a20 2020 206e 616d 6520 3d20 5f67  "".    name = _g
-000112a0: 6574 5f63 6c75 7374 6572 5f6e 616d 6528  et_cluster_name(
-000112b0: 290a 2020 2020 7265 6769 6f6e 203d 2061  ).    region = a
-000112c0: 7773 5f63 6f6e 6669 675f 7265 6769 6f6e  ws_config_region
-000112d0: 0a20 2020 2074 6573 7420 3d20 5465 7374  .    test = Test
-000112e0: 280a 2020 2020 2020 2020 2773 706f 745f  (.        'spot_
-000112f0: 7265 636f 7665 7279 5f61 7773 272c 0a20  recovery_aws',. 
-00011300: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-00011310: 2020 2020 2066 2773 6b79 2073 706f 7420       f'sky spot 
-00011320: 6c61 756e 6368 202d 2d63 6c6f 7564 2061  launch --cloud a
-00011330: 7773 202d 2d72 6567 696f 6e20 7b72 6567  ws --region {reg
-00011340: 696f 6e7d 202d 6e20 7b6e 616d 657d 2022  ion} -n {name} "
-00011350: 6563 686f 2053 4b59 5049 4c4f 545f 5441  echo SKYPILOT_TA
-00011360: 534b 5f49 443a 205c 2453 4b59 5049 4c4f  SK_ID: \$SKYPILO
-00011370: 545f 5441 534b 5f49 443b 2073 6c65 6570  T_TASK_ID; sleep
-00011380: 2031 3830 3022 2020 2d79 202d 6427 2c0a   1800"  -y -d',.
-00011390: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
-000113a0: 6570 2033 3630 272c 0a20 2020 2020 2020  ep 360',.       
-000113b0: 2020 2020 2066 277b 5f53 504f 545f 5155       f'{_SPOT_QU
-000113c0: 4555 455f 5741 4954 7d7c 2067 7265 7020  EUE_WAIT}| grep 
-000113d0: 7b6e 616d 657d 207c 2068 6561 6420 2d6e  {name} | head -n
-000113e0: 3120 7c20 6772 6570 2022 5255 4e4e 494e  1 | grep "RUNNIN
-000113f0: 4722 272c 0a20 2020 2020 2020 2020 2020  G"',.           
-00011400: 2066 2752 554e 5f49 443d 2428 736b 7920   f'RUN_ID=$(sky 
-00011410: 7370 6f74 206c 6f67 7320 2d6e 207b 6e61  spot logs -n {na
-00011420: 6d65 7d20 2d2d 6e6f 2d66 6f6c 6c6f 7720  me} --no-follow 
-00011430: 7c20 6772 6570 2053 4b59 5049 4c4f 545f  | grep SKYPILOT_
-00011440: 5441 534b 5f49 4420 7c20 6375 7420 2d64  TASK_ID | cut -d
-00011450: 3a20 2d66 3229 3b20 6563 686f 2022 2452  : -f2); echo "$R
-00011460: 554e 5f49 4422 207c 2074 6565 202f 746d  UN_ID" | tee /tm
-00011470: 702f 7b6e 616d 657d 2d72 756e 2d69 6427  p/{name}-run-id'
-00011480: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
-00011490: 5465 726d 696e 6174 6520 7468 6520 636c  Terminate the cl
-000114a0: 7573 7465 7220 6d61 6e75 616c 6c79 2e0a  uster manually..
-000114b0: 2020 2020 2020 2020 2020 2020 2866 2761              (f'a
-000114c0: 7773 2065 6332 2074 6572 6d69 6e61 7465  ws ec2 terminate
-000114d0: 2d69 6e73 7461 6e63 6573 202d 2d72 6567  -instances --reg
-000114e0: 696f 6e20 7b72 6567 696f 6e7d 202d 2d69  ion {region} --i
-000114f0: 6e73 7461 6e63 652d 6964 7320 2428 270a  nstance-ids $('.
-00011500: 2020 2020 2020 2020 2020 2020 2066 2761               f'a
-00011510: 7773 2065 6332 2064 6573 6372 6962 652d  ws ec2 describe-
-00011520: 696e 7374 616e 6365 7320 2d2d 7265 6769  instances --regi
-00011530: 6f6e 207b 7265 6769 6f6e 7d20 270a 2020  on {region} '.  
-00011540: 2020 2020 2020 2020 2020 2066 272d 2d66             f'--f
-00011550: 696c 7465 7273 204e 616d 653d 7461 673a  ilters Name=tag:
-00011560: 7261 792d 636c 7573 7465 722d 6e61 6d65  ray-cluster-name
-00011570: 2c56 616c 7565 733d 7b6e 616d 657d 2a20  ,Values={name}* 
-00011580: 270a 2020 2020 2020 2020 2020 2020 2066  '.             f
-00011590: 272d 2d71 7565 7279 2052 6573 6572 7661  '--query Reserva
-000115a0: 7469 6f6e 735b 5d2e 496e 7374 616e 6365  tions[].Instance
-000115b0: 735b 5d2e 496e 7374 616e 6365 4964 2027  s[].InstanceId '
-000115c0: 0a20 2020 2020 2020 2020 2020 2020 272d  .             '-
-000115d0: 2d6f 7574 7075 7420 7465 7874 2927 292c  -output text)'),
-000115e0: 0a20 2020 2020 2020 2020 2020 2027 736c  .            'sl
-000115f0: 6565 7020 3130 3027 2c0a 2020 2020 2020  eep 100',.      
-00011600: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
-00011610: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
-00011620: 207b 6e61 6d65 7d20 7c20 6865 6164 202d   {name} | head -
-00011630: 6e31 207c 2067 7265 7020 2252 4543 4f56  n1 | grep "RECOV
-00011640: 4552 494e 4722 272c 0a20 2020 2020 2020  ERING"',.       
-00011650: 2020 2020 2027 736c 6565 7020 3230 3027       'sleep 200'
-00011660: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-00011670: 7b5f 5350 4f54 5f51 5545 5545 5f57 4149  {_SPOT_QUEUE_WAI
-00011680: 547d 7c20 6772 6570 207b 6e61 6d65 7d20  T}| grep {name} 
-00011690: 7c20 6865 6164 202d 6e31 207c 2067 7265  | head -n1 | gre
-000116a0: 7020 2252 554e 4e49 4e47 2227 2c0a 2020  p "RUNNING"',.  
-000116b0: 2020 2020 2020 2020 2020 6627 5255 4e5f            f'RUN_
-000116c0: 4944 3d24 2863 6174 202f 746d 702f 7b6e  ID=$(cat /tmp/{n
-000116d0: 616d 657d 2d72 756e 2d69 6429 3b20 6563  ame}-run-id); ec
-000116e0: 686f 2024 5255 4e5f 4944 3b20 736b 7920  ho $RUN_ID; sky 
-000116f0: 7370 6f74 206c 6f67 7320 2d6e 207b 6e61  spot logs -n {na
-00011700: 6d65 7d20 2d2d 6e6f 2d66 6f6c 6c6f 7720  me} --no-follow 
-00011710: 7c20 6772 6570 2053 4b59 5049 4c4f 545f  | grep SKYPILOT_
-00011720: 5441 534b 5f49 4420 7c20 6772 6570 2022  TASK_ID | grep "
-00011730: 2452 554e 5f49 4422 272c 0a20 2020 2020  $RUN_ID"',.     
-00011740: 2020 205d 2c0a 2020 2020 2020 2020 5f53     ],.        _S
-00011750: 504f 545f 4341 4e43 454c 5f57 4149 542e  POT_CANCEL_WAIT.
-00011760: 666f 726d 6174 286a 6f62 5f6e 616d 653d  format(job_name=
-00011770: 6e61 6d65 292c 0a20 2020 2020 2020 2074  name),.        t
-00011780: 696d 656f 7574 3d32 3520 2a20 3630 2c0a  imeout=25 * 60,.
-00011790: 2020 2020 290a 2020 2020 7275 6e5f 6f6e      ).    run_on
-000117a0: 655f 7465 7374 2874 6573 7429 0a0a 0a40  e_test(test)...@
-000117b0: 7079 7465 7374 2e6d 6172 6b2e 6763 700a  pytest.mark.gcp.
-000117c0: 4070 7974 6573 742e 6d61 726b 2e6d 616e  @pytest.mark.man
-000117d0: 6167 6564 5f73 706f 740a 6465 6620 7465  aged_spot.def te
-000117e0: 7374 5f73 706f 745f 7265 636f 7665 7279  st_spot_recovery
-000117f0: 5f67 6370 2829 3a0a 2020 2020 2222 2254  _gcp():.    """T
-00011800: 6573 7420 6d61 6e61 6765 6420 7370 6f74  est managed spot
-00011810: 2072 6563 6f76 6572 792e 2222 220a 2020   recovery.""".  
-00011820: 2020 6e61 6d65 203d 205f 6765 745f 636c    name = _get_cl
-00011830: 7573 7465 725f 6e61 6d65 2829 0a20 2020  uster_name().   
-00011840: 207a 6f6e 6520 3d20 2775 732d 6561 7374   zone = 'us-east
-00011850: 342d 6227 0a20 2020 2071 7565 7279 5f63  4-b'.    query_c
-00011860: 6d64 203d 2028 6627 6763 6c6f 7564 2063  md = (f'gcloud c
-00011870: 6f6d 7075 7465 2069 6e73 7461 6e63 6573  ompute instances
-00011880: 206c 6973 7420 2d2d 6669 6c74 6572 3d27   list --filter='
-00011890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000118a0: 2020 6627 2228 6c61 6265 6c73 2e72 6179    f'"(labels.ray
-000118b0: 2d63 6c75 7374 6572 2d6e 616d 653a 7b6e  -cluster-name:{n
-000118c0: 616d 657d 2922 2027 0a20 2020 2020 2020  ame})" '.       
-000118d0: 2020 2020 2020 2020 2020 6627 2d2d 7a6f            f'--zo
-000118e0: 6e65 733d 7b7a 6f6e 657d 202d 2d66 6f72  nes={zone} --for
-000118f0: 6d61 743d 2276 616c 7565 286e 616d 6529  mat="value(name)
-00011900: 2227 290a 2020 2020 7465 726d 696e 6174  "').    terminat
-00011910: 655f 636d 6420 3d20 2866 2767 636c 6f75  e_cmd = (f'gclou
-00011920: 6420 636f 6d70 7574 6520 696e 7374 616e  d compute instan
-00011930: 6365 7320 6465 6c65 7465 202d 2d7a 6f6e  ces delete --zon
-00011940: 653d 7b7a 6f6e 657d 270a 2020 2020 2020  e={zone}'.      
-00011950: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00011960: 2720 2d2d 7175 6965 7420 2428 7b71 7565  ' --quiet $({que
-00011970: 7279 5f63 6d64 7d29 2729 0a20 2020 2074  ry_cmd})').    t
-00011980: 6573 7420 3d20 5465 7374 280a 2020 2020  est = Test(.    
-00011990: 2020 2020 2773 706f 745f 7265 636f 7665      'spot_recove
-000119a0: 7279 5f67 6370 272c 0a20 2020 2020 2020  ry_gcp',.       
-000119b0: 205b 0a20 2020 2020 2020 2020 2020 2066   [.            f
-000119c0: 2773 6b79 2073 706f 7420 6c61 756e 6368  'sky spot launch
-000119d0: 202d 2d63 6c6f 7564 2067 6370 202d 2d7a   --cloud gcp --z
-000119e0: 6f6e 6520 7b7a 6f6e 657d 202d 6e20 7b6e  one {zone} -n {n
-000119f0: 616d 657d 2022 6563 686f 2053 4b59 5049  ame} "echo SKYPI
-00011a00: 4c4f 545f 5441 534b 5f49 443a 205c 2453  LOT_TASK_ID: \$S
-00011a10: 4b59 5049 4c4f 545f 5441 534b 5f49 443b  KYPILOT_TASK_ID;
-00011a20: 2073 6c65 6570 2031 3830 3022 2020 2d79   sleep 1800"  -y
-00011a30: 202d 6427 2c0a 2020 2020 2020 2020 2020   -d',.          
-00011a40: 2020 2773 6c65 6570 2033 3630 272c 0a20    'sleep 360',. 
-00011a50: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
-00011a60: 504f 545f 5155 4555 455f 5741 4954 7d7c  POT_QUEUE_WAIT}|
-00011a70: 2067 7265 7020 7b6e 616d 657d 207c 2068   grep {name} | h
-00011a80: 6561 6420 2d6e 3120 7c20 6772 6570 2022  ead -n1 | grep "
-00011a90: 5255 4e4e 494e 4722 272c 0a20 2020 2020  RUNNING"',.     
-00011aa0: 2020 2020 2020 2066 2752 554e 5f49 443d         f'RUN_ID=
-00011ab0: 2428 736b 7920 7370 6f74 206c 6f67 7320  $(sky spot logs 
-00011ac0: 2d6e 207b 6e61 6d65 7d20 2d2d 6e6f 2d66  -n {name} --no-f
-00011ad0: 6f6c 6c6f 7720 7c20 6772 6570 2053 4b59  ollow | grep SKY
-00011ae0: 5049 4c4f 545f 5441 534b 5f49 4420 7c20  PILOT_TASK_ID | 
-00011af0: 6375 7420 2d64 3a20 2d66 3229 3b20 6563  cut -d: -f2); ec
-00011b00: 686f 2022 2452 554e 5f49 4422 207c 2074  ho "$RUN_ID" | t
-00011b10: 6565 202f 746d 702f 7b6e 616d 657d 2d72  ee /tmp/{name}-r
-00011b20: 756e 2d69 6427 2c0a 2020 2020 2020 2020  un-id',.        
-00011b30: 2020 2020 2320 5465 726d 696e 6174 6520      # Terminate 
-00011b40: 7468 6520 636c 7573 7465 7220 6d61 6e75  the cluster manu
-00011b50: 616c 6c79 2e0a 2020 2020 2020 2020 2020  ally..          
-00011b60: 2020 7465 726d 696e 6174 655f 636d 642c    terminate_cmd,
-00011b70: 0a20 2020 2020 2020 2020 2020 2027 736c  .            'sl
-00011b80: 6565 7020 3130 3027 2c0a 2020 2020 2020  eep 100',.      
-00011b90: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
-00011ba0: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
-00011bb0: 207b 6e61 6d65 7d20 7c20 6865 6164 202d   {name} | head -
-00011bc0: 6e31 207c 2067 7265 7020 2252 4543 4f56  n1 | grep "RECOV
-00011bd0: 4552 494e 4722 272c 0a20 2020 2020 2020  ERING"',.       
-00011be0: 2020 2020 2027 736c 6565 7020 3230 3027       'sleep 200'
-00011bf0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-00011c00: 7b5f 5350 4f54 5f51 5545 5545 5f57 4149  {_SPOT_QUEUE_WAI
-00011c10: 547d 7c20 6772 6570 207b 6e61 6d65 7d20  T}| grep {name} 
-00011c20: 7c20 6865 6164 202d 6e31 207c 2067 7265  | head -n1 | gre
-00011c30: 7020 2252 554e 4e49 4e47 2227 2c0a 2020  p "RUNNING"',.  
-00011c40: 2020 2020 2020 2020 2020 6627 5255 4e5f            f'RUN_
-00011c50: 4944 3d24 2863 6174 202f 746d 702f 7b6e  ID=$(cat /tmp/{n
-00011c60: 616d 657d 2d72 756e 2d69 6429 3b20 6563  ame}-run-id); ec
-00011c70: 686f 2024 5255 4e5f 4944 3b20 736b 7920  ho $RUN_ID; sky 
-00011c80: 7370 6f74 206c 6f67 7320 2d6e 207b 6e61  spot logs -n {na
-00011c90: 6d65 7d20 2d2d 6e6f 2d66 6f6c 6c6f 7720  me} --no-follow 
-00011ca0: 7c20 6772 6570 2053 4b59 5049 4c4f 545f  | grep SKYPILOT_
-00011cb0: 5441 534b 5f49 443a 207c 2067 7265 7020  TASK_ID: | grep 
-00011cc0: 2224 5255 4e5f 4944 2227 2c0a 2020 2020  "$RUN_ID"',.    
-00011cd0: 2020 2020 5d2c 0a20 2020 2020 2020 205f      ],.        _
-00011ce0: 5350 4f54 5f43 414e 4345 4c5f 5741 4954  SPOT_CANCEL_WAIT
-00011cf0: 2e66 6f72 6d61 7428 6a6f 625f 6e61 6d65  .format(job_name
-00011d00: 3d6e 616d 6529 2c0a 2020 2020 2020 2020  =name),.        
-00011d10: 7469 6d65 6f75 743d 3235 202a 2036 302c  timeout=25 * 60,
-00011d20: 0a20 2020 2029 0a20 2020 2072 756e 5f6f  .    ).    run_o
-00011d30: 6e65 5f74 6573 7428 7465 7374 290a 0a0a  ne_test(test)...
-00011d40: 4070 7974 6573 742e 6d61 726b 2e61 7773  @pytest.mark.aws
-00011d50: 0a40 7079 7465 7374 2e6d 6172 6b2e 6d61  .@pytest.mark.ma
-00011d60: 6e61 6765 645f 7370 6f74 0a64 6566 2074  naged_spot.def t
-00011d70: 6573 745f 7370 6f74 5f70 6970 656c 696e  est_spot_pipelin
-00011d80: 655f 7265 636f 7665 7279 5f61 7773 2861  e_recovery_aws(a
-00011d90: 7773 5f63 6f6e 6669 675f 7265 6769 6f6e  ws_config_region
-00011da0: 293a 0a20 2020 2022 2222 5465 7374 206d  ):.    """Test m
-00011db0: 616e 6167 6564 2073 706f 7420 7265 636f  anaged spot reco
-00011dc0: 7665 7279 2066 6f72 2061 2070 6970 656c  very for a pipel
-00011dd0: 696e 652e 2222 220a 2020 2020 6e61 6d65  ine.""".    name
-00011de0: 203d 205f 6765 745f 636c 7573 7465 725f   = _get_cluster_
-00011df0: 6e61 6d65 2829 0a20 2020 2072 6567 696f  name().    regio
-00011e00: 6e20 3d20 6177 735f 636f 6e66 6967 5f72  n = aws_config_r
-00011e10: 6567 696f 6e0a 2020 2020 6966 2072 6567  egion.    if reg
-00011e20: 696f 6e20 213d 2027 7573 2d77 6573 742d  ion != 'us-west-
-00011e30: 3227 3a0a 2020 2020 2020 2020 7079 7465  2':.        pyte
-00011e40: 7374 2e73 6b69 7028 274f 6e6c 7920 7275  st.skip('Only ru
-00011e50: 6e20 7370 6f74 2070 6970 656c 696e 6520  n spot pipeline 
-00011e60: 7265 636f 7665 7279 2074 6573 7420 696e  recovery test in
-00011e70: 2075 732d 7765 7374 2d32 2729 0a20 2020   us-west-2').   
-00011e80: 2074 6573 7420 3d20 5465 7374 280a 2020   test = Test(.  
-00011e90: 2020 2020 2020 2773 706f 745f 7069 7065        'spot_pipe
-00011ea0: 6c69 6e65 5f72 6563 6f76 6572 795f 6177  line_recovery_aw
-00011eb0: 7327 2c0a 2020 2020 2020 2020 5b0a 2020  s',.        [.  
-00011ec0: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
-00011ed0: 7370 6f74 206c 6175 6e63 6820 2d6e 207b  spot launch -n {
-00011ee0: 6e61 6d65 7d20 7465 7374 732f 7465 7374  name} tests/test
-00011ef0: 5f79 616d 6c73 2f70 6970 656c 696e 655f  _yamls/pipeline_
-00011f00: 6177 732e 7961 6d6c 2020 2d79 202d 6427  aws.yaml  -y -d'
-00011f10: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
-00011f20: 6c65 6570 2034 3030 272c 0a20 2020 2020  leep 400',.     
-00011f30: 2020 2020 2020 2066 277b 5f53 504f 545f         f'{_SPOT_
-00011f40: 5155 4555 455f 5741 4954 7d7c 2067 7265  QUEUE_WAIT}| gre
-00011f50: 7020 7b6e 616d 657d 207c 2068 6561 6420  p {name} | head 
-00011f60: 2d6e 3120 7c20 6772 6570 2022 5255 4e4e  -n1 | grep "RUNN
-00011f70: 494e 4722 272c 0a20 2020 2020 2020 2020  ING"',.         
-00011f80: 2020 2066 2752 554e 5f49 443d 2428 736b     f'RUN_ID=$(sk
-00011f90: 7920 7370 6f74 206c 6f67 7320 2d6e 207b  y spot logs -n {
-00011fa0: 6e61 6d65 7d20 2d2d 6e6f 2d66 6f6c 6c6f  name} --no-follo
-00011fb0: 7720 7c20 6772 6570 2053 4b59 5049 4c4f  w | grep SKYPILO
-00011fc0: 545f 5441 534b 5f49 443a 207c 2063 7574  T_TASK_ID: | cut
-00011fd0: 202d 643a 202d 6632 293b 2065 6368 6f20   -d: -f2); echo 
-00011fe0: 2224 5255 4e5f 4944 2220 7c20 7465 6520  "$RUN_ID" | tee 
-00011ff0: 2f74 6d70 2f7b 6e61 6d65 7d2d 7275 6e2d  /tmp/{name}-run-
-00012000: 6964 272c 0a20 2020 2020 2020 2020 2020  id',.           
-00012010: 2066 2752 554e 5f49 4453 3d24 2873 6b79   f'RUN_IDS=$(sky
-00012020: 2073 706f 7420 6c6f 6773 202d 6e20 7b6e   spot logs -n {n
-00012030: 616d 657d 202d 2d6e 6f2d 666f 6c6c 6f77  ame} --no-follow
-00012040: 207c 2067 7265 7020 2d41 2034 2053 4b59   | grep -A 4 SKY
-00012050: 5049 4c4f 545f 5441 534b 5f49 4453 207c  PILOT_TASK_IDS |
-00012060: 2063 7574 202d 6422 2922 202d 6632 293b   cut -d")" -f2);
-00012070: 2065 6368 6f20 2224 5255 4e5f 4944 5322   echo "$RUN_IDS"
-00012080: 207c 2074 6565 202f 746d 702f 7b6e 616d   | tee /tmp/{nam
-00012090: 657d 2d72 756e 2d69 6473 272c 0a20 2020  e}-run-ids',.   
-000120a0: 2020 2020 2020 2020 2023 2054 6572 6d69           # Termi
-000120b0: 6e61 7465 2074 6865 2063 6c75 7374 6572  nate the cluster
-000120c0: 206d 616e 7561 6c6c 792e 0a20 2020 2020   manually..     
-000120d0: 2020 2020 2020 2023 2054 6865 2060 6361         # The `ca
-000120e0: 7420 2e2e 2e7c 2072 6576 6020 6973 2074  t ...| rev` is t
-000120f0: 6f20 7265 7472 6965 7665 2074 6865 206a  o retrieve the j
-00012100: 6f62 5f69 6420 6672 6f6d 2074 6865 0a20  ob_id from the. 
-00012110: 2020 2020 2020 2020 2020 2023 2053 4b59             # SKY
-00012120: 5049 4c4f 545f 5441 534b 5f49 442c 2077  PILOT_TASK_ID, w
-00012130: 6869 6368 2067 6574 7320 7468 6520 7365  hich gets the se
-00012140: 636f 6e64 2074 6f20 6c61 7374 2066 6965  cond to last fie
-00012150: 6c64 0a20 2020 2020 2020 2020 2020 2023  ld.            #
-00012160: 2073 6570 6172 6174 6564 2062 7920 602d   separated by `-
-00012170: 602e 0a20 2020 2020 2020 2020 2020 2028  `..            (
-00012180: 6627 5350 4f54 5f4a 4f42 5f49 443d 6063  f'SPOT_JOB_ID=`c
-00012190: 6174 202f 746d 702f 7b6e 616d 657d 2d72  at /tmp/{name}-r
-000121a0: 756e 2d69 6420 7c20 7265 7620 7c20 270a  un-id | rev | '.
-000121b0: 2020 2020 2020 2020 2020 2020 2027 6375               'cu
-000121c0: 7420 2d64 5c27 2d5c 2720 2d66 3220 7c20  t -d\'-\' -f2 | 
-000121d0: 7265 7660 3b27 0a20 2020 2020 2020 2020  rev`;'.         
-000121e0: 2020 2020 6627 6177 7320 6563 3220 7465      f'aws ec2 te
-000121f0: 726d 696e 6174 652d 696e 7374 616e 6365  rminate-instance
-00012200: 7320 2d2d 7265 6769 6f6e 207b 7265 6769  s --region {regi
-00012210: 6f6e 7d20 2d2d 696e 7374 616e 6365 2d69  on} --instance-i
-00012220: 6473 2024 2827 0a20 2020 2020 2020 2020  ds $('.         
-00012230: 2020 2020 6627 6177 7320 6563 3220 6465      f'aws ec2 de
-00012240: 7363 7269 6265 2d69 6e73 7461 6e63 6573  scribe-instances
-00012250: 202d 2d72 6567 696f 6e20 7b72 6567 696f   --region {regio
-00012260: 6e7d 2027 0a20 2020 2020 2020 2020 2020  n} '.           
-00012270: 2020 272d 2d66 696c 7465 7273 204e 616d    '--filters Nam
-00012280: 653d 7461 673a 7261 792d 636c 7573 7465  e=tag:ray-cluste
-00012290: 722d 6e61 6d65 2c56 616c 7565 733d 2a2d  r-name,Values=*-
-000122a0: 247b 5350 4f54 5f4a 4f42 5f49 447d 2027  ${SPOT_JOB_ID} '
-000122b0: 0a20 2020 2020 2020 2020 2020 2020 6627  .             f'
-000122c0: 2d2d 7175 6572 7920 5265 7365 7276 6174  --query Reservat
-000122d0: 696f 6e73 5b5d 2e49 6e73 7461 6e63 6573  ions[].Instances
-000122e0: 5b5d 2e49 6e73 7461 6e63 6549 6420 270a  [].InstanceId '.
-000122f0: 2020 2020 2020 2020 2020 2020 2027 2d2d               '--
-00012300: 6f75 7470 7574 2074 6578 7429 2729 2c0a  output text)'),.
-00012310: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
-00012320: 6570 2031 3030 272c 0a20 2020 2020 2020  ep 100',.       
-00012330: 2020 2020 2066 277b 5f53 504f 545f 5155       f'{_SPOT_QU
-00012340: 4555 455f 5741 4954 7d7c 2067 7265 7020  EUE_WAIT}| grep 
-00012350: 7b6e 616d 657d 207c 2068 6561 6420 2d6e  {name} | head -n
-00012360: 3120 7c20 6772 6570 2022 5245 434f 5645  1 | grep "RECOVE
-00012370: 5249 4e47 2227 2c0a 2020 2020 2020 2020  RING"',.        
-00012380: 2020 2020 2773 6c65 6570 2032 3030 272c      'sleep 200',
-00012390: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
-000123a0: 5f53 504f 545f 5155 4555 455f 5741 4954  _SPOT_QUEUE_WAIT
-000123b0: 7d7c 2067 7265 7020 7b6e 616d 657d 207c  }| grep {name} |
-000123c0: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
-000123d0: 2022 5255 4e4e 494e 4722 272c 0a20 2020   "RUNNING"',.   
-000123e0: 2020 2020 2020 2020 2066 2752 554e 5f49           f'RUN_I
-000123f0: 443d 2428 6361 7420 2f74 6d70 2f7b 6e61  D=$(cat /tmp/{na
-00012400: 6d65 7d2d 7275 6e2d 6964 293b 2065 6368  me}-run-id); ech
-00012410: 6f20 2452 554e 5f49 443b 2073 6b79 2073  o $RUN_ID; sky s
-00012420: 706f 7420 6c6f 6773 202d 6e20 7b6e 616d  pot logs -n {nam
-00012430: 657d 202d 2d6e 6f2d 666f 6c6c 6f77 207c  e} --no-follow |
-00012440: 2067 7265 7020 534b 5950 494c 4f54 5f54   grep SKYPILOT_T
-00012450: 4153 4b5f 4944 3a20 7c20 6772 6570 2022  ASK_ID: | grep "
-00012460: 2452 554e 5f49 4422 272c 0a20 2020 2020  $RUN_ID"',.     
-00012470: 2020 2020 2020 2066 2752 554e 5f49 4453         f'RUN_IDS
-00012480: 3d24 2873 6b79 2073 706f 7420 6c6f 6773  =$(sky spot logs
-00012490: 202d 6e20 7b6e 616d 657d 202d 2d6e 6f2d   -n {name} --no-
-000124a0: 666f 6c6c 6f77 207c 2067 7265 7020 2d41  follow | grep -A
-000124b0: 2034 2053 4b59 5049 4c4f 545f 5441 534b   4 SKYPILOT_TASK
-000124c0: 5f49 4453 207c 2063 7574 202d 6422 2922  _IDS | cut -d")"
-000124d0: 202d 6632 293b 2065 6368 6f20 2224 5255   -f2); echo "$RU
-000124e0: 4e5f 4944 5322 207c 2074 6565 202f 746d  N_IDS" | tee /tm
-000124f0: 702f 7b6e 616d 657d 2d72 756e 2d69 6473  p/{name}-run-ids
-00012500: 2d6e 6577 272c 0a20 2020 2020 2020 2020  -new',.         
-00012510: 2020 2066 2764 6966 6620 2f74 6d70 2f7b     f'diff /tmp/{
-00012520: 6e61 6d65 7d2d 7275 6e2d 6964 7320 2f74  name}-run-ids /t
-00012530: 6d70 2f7b 6e61 6d65 7d2d 7275 6e2d 6964  mp/{name}-run-id
-00012540: 732d 6e65 7727 2c0a 2020 2020 2020 2020  s-new',.        
-00012550: 2020 2020 6627 6361 7420 2f74 6d70 2f7b      f'cat /tmp/{
-00012560: 6e61 6d65 7d2d 7275 6e2d 6964 7320 7c20  name}-run-ids | 
-00012570: 7365 6420 2d6e 2032 7020 7c20 6772 6570  sed -n 2p | grep
-00012580: 2060 6361 7420 2f74 6d70 2f7b 6e61 6d65   `cat /tmp/{name
-00012590: 7d2d 7275 6e2d 6964 6027 2c0a 2020 2020  }-run-id`',.    
-000125a0: 2020 2020 5d2c 0a20 2020 2020 2020 205f      ],.        _
-000125b0: 5350 4f54 5f43 414e 4345 4c5f 5741 4954  SPOT_CANCEL_WAIT
-000125c0: 2e66 6f72 6d61 7428 6a6f 625f 6e61 6d65  .format(job_name
-000125d0: 3d6e 616d 6529 2c0a 2020 2020 2020 2020  =name),.        
-000125e0: 7469 6d65 6f75 743d 3235 202a 2036 302c  timeout=25 * 60,
-000125f0: 0a20 2020 2029 0a20 2020 2072 756e 5f6f  .    ).    run_o
-00012600: 6e65 5f74 6573 7428 7465 7374 290a 0a0a  ne_test(test)...
-00012610: 4070 7974 6573 742e 6d61 726b 2e67 6370  @pytest.mark.gcp
-00012620: 0a40 7079 7465 7374 2e6d 6172 6b2e 6d61  .@pytest.mark.ma
-00012630: 6e61 6765 645f 7370 6f74 0a64 6566 2074  naged_spot.def t
-00012640: 6573 745f 7370 6f74 5f70 6970 656c 696e  est_spot_pipelin
-00012650: 655f 7265 636f 7665 7279 5f67 6370 2829  e_recovery_gcp()
-00012660: 3a0a 2020 2020 2222 2254 6573 7420 6d61  :.    """Test ma
-00012670: 6e61 6765 6420 7370 6f74 2072 6563 6f76  naged spot recov
-00012680: 6572 7920 666f 7220 6120 7069 7065 6c69  ery for a pipeli
-00012690: 6e65 2e22 2222 0a20 2020 206e 616d 6520  ne.""".    name 
-000126a0: 3d20 5f67 6574 5f63 6c75 7374 6572 5f6e  = _get_cluster_n
-000126b0: 616d 6528 290a 2020 2020 7a6f 6e65 203d  ame().    zone =
-000126c0: 2027 7573 2d65 6173 7434 2d62 270a 2020   'us-east4-b'.  
-000126d0: 2020 7175 6572 795f 636d 6420 3d20 2827    query_cmd = ('
-000126e0: 6763 6c6f 7564 2063 6f6d 7075 7465 2069  gcloud compute i
-000126f0: 6e73 7461 6e63 6573 206c 6973 7420 2d2d  nstances list --
-00012700: 6669 6c74 6572 3d27 0a20 2020 2020 2020  filter='.       
-00012710: 2020 2020 2020 2020 2020 2722 286c 6162            '"(lab
-00012720: 656c 732e 7261 792d 636c 7573 7465 722d  els.ray-cluster-
-00012730: 6e61 6d65 3a2a 2d24 7b53 504f 545f 4a4f  name:*-${SPOT_JO
-00012740: 425f 4944 7d29 2220 270a 2020 2020 2020  B_ID})" '.      
-00012750: 2020 2020 2020 2020 2020 2066 272d 2d7a             f'--z
-00012760: 6f6e 6573 3d7b 7a6f 6e65 7d20 2d2d 666f  ones={zone} --fo
-00012770: 726d 6174 3d22 7661 6c75 6528 6e61 6d65  rmat="value(name
-00012780: 2922 2729 0a20 2020 2074 6572 6d69 6e61  )"').    termina
-00012790: 7465 5f63 6d64 203d 2028 6627 6763 6c6f  te_cmd = (f'gclo
-000127a0: 7564 2063 6f6d 7075 7465 2069 6e73 7461  ud compute insta
-000127b0: 6e63 6573 2064 656c 6574 6520 2d2d 7a6f  nces delete --zo
-000127c0: 6e65 3d7b 7a6f 6e65 7d27 0a20 2020 2020  ne={zone}'.     
-000127d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127e0: 6627 202d 2d71 7569 6574 2024 287b 7175  f' --quiet $({qu
-000127f0: 6572 795f 636d 647d 2927 290a 2020 2020  ery_cmd})').    
-00012800: 7465 7374 203d 2054 6573 7428 0a20 2020  test = Test(.   
-00012810: 2020 2020 2027 7370 6f74 5f70 6970 656c       'spot_pipel
-00012820: 696e 655f 7265 636f 7665 7279 5f67 6370  ine_recovery_gcp
-00012830: 272c 0a20 2020 2020 2020 205b 0a20 2020  ',.        [.   
-00012840: 2020 2020 2020 2020 2066 2773 6b79 2073           f'sky s
-00012850: 706f 7420 6c61 756e 6368 202d 6e20 7b6e  pot launch -n {n
-00012860: 616d 657d 2074 6573 7473 2f74 6573 745f  ame} tests/test_
-00012870: 7961 6d6c 732f 7069 7065 6c69 6e65 5f67  yamls/pipeline_g
-00012880: 6370 2e79 616d 6c20 202d 7920 2d64 272c  cp.yaml  -y -d',
-00012890: 0a20 2020 2020 2020 2020 2020 2027 736c  .            'sl
-000128a0: 6565 7020 3430 3027 2c0a 2020 2020 2020  eep 400',.      
-000128b0: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
-000128c0: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
-000128d0: 207b 6e61 6d65 7d20 7c20 6865 6164 202d   {name} | head -
-000128e0: 6e31 207c 2067 7265 7020 2252 554e 4e49  n1 | grep "RUNNI
-000128f0: 4e47 2227 2c0a 2020 2020 2020 2020 2020  NG"',.          
-00012900: 2020 6627 5255 4e5f 4944 3d24 2873 6b79    f'RUN_ID=$(sky
-00012910: 2073 706f 7420 6c6f 6773 202d 6e20 7b6e   spot logs -n {n
-00012920: 616d 657d 202d 2d6e 6f2d 666f 6c6c 6f77  ame} --no-follow
-00012930: 207c 2067 7265 7020 534b 5950 494c 4f54   | grep SKYPILOT
-00012940: 5f54 4153 4b5f 4944 3a20 7c20 6375 7420  _TASK_ID: | cut 
-00012950: 2d64 3a20 2d66 3229 3b20 6563 686f 2022  -d: -f2); echo "
-00012960: 2452 554e 5f49 4422 207c 2074 6565 202f  $RUN_ID" | tee /
-00012970: 746d 702f 7b6e 616d 657d 2d72 756e 2d69  tmp/{name}-run-i
-00012980: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
-00012990: 6627 5255 4e5f 4944 533d 2428 736b 7920  f'RUN_IDS=$(sky 
-000129a0: 7370 6f74 206c 6f67 7320 2d6e 207b 6e61  spot logs -n {na
-000129b0: 6d65 7d20 2d2d 6e6f 2d66 6f6c 6c6f 7720  me} --no-follow 
-000129c0: 7c20 6772 6570 202d 4120 3420 534b 5950  | grep -A 4 SKYP
-000129d0: 494c 4f54 5f54 4153 4b5f 4944 5320 7c20  ILOT_TASK_IDS | 
-000129e0: 6375 7420 2d64 2229 2220 2d66 3229 3b20  cut -d")" -f2); 
-000129f0: 6563 686f 2022 2452 554e 5f49 4453 2220  echo "$RUN_IDS" 
-00012a00: 7c20 7465 6520 2f74 6d70 2f7b 6e61 6d65  | tee /tmp/{name
-00012a10: 7d2d 7275 6e2d 6964 7327 2c0a 2020 2020  }-run-ids',.    
-00012a20: 2020 2020 2020 2020 2320 5465 726d 696e          # Termin
-00012a30: 6174 6520 7468 6520 636c 7573 7465 7220  ate the cluster 
-00012a40: 6d61 6e75 616c 6c79 2e0a 2020 2020 2020  manually..      
-00012a50: 2020 2020 2020 2320 5468 6520 6063 6174        # The `cat
-00012a60: 202e 2e2e 7c20 7265 7660 2069 7320 746f   ...| rev` is to
-00012a70: 2072 6574 7269 6576 6520 7468 6520 6a6f   retrieve the jo
-00012a80: 625f 6964 2066 726f 6d20 7468 650a 2020  b_id from the.  
-00012a90: 2020 2020 2020 2020 2020 2320 534b 5950            # SKYP
-00012aa0: 494c 4f54 5f54 4153 4b5f 4944 2c20 7768  ILOT_TASK_ID, wh
-00012ab0: 6963 6820 6765 7473 2074 6865 2073 6563  ich gets the sec
-00012ac0: 6f6e 6420 746f 206c 6173 7420 6669 656c  ond to last fiel
-00012ad0: 640a 2020 2020 2020 2020 2020 2020 2320  d.            # 
-00012ae0: 7365 7061 7261 7465 6420 6279 2060 2d60  separated by `-`
-00012af0: 2e0a 2020 2020 2020 2020 2020 2020 2866  ..            (f
-00012b00: 2753 504f 545f 4a4f 425f 4944 3d60 6361  'SPOT_JOB_ID=`ca
-00012b10: 7420 2f74 6d70 2f7b 6e61 6d65 7d2d 7275  t /tmp/{name}-ru
-00012b20: 6e2d 6964 207c 2072 6576 207c 2027 0a20  n-id | rev | '. 
-00012b30: 2020 2020 2020 2020 2020 2020 6627 6375              f'cu
-00012b40: 7420 2d64 5c27 2d5c 2720 2d66 3220 7c20  t -d\'-\' -f2 | 
-00012b50: 7265 7660 3b7b 7465 726d 696e 6174 655f  rev`;{terminate_
-00012b60: 636d 647d 2729 2c0a 2020 2020 2020 2020  cmd}'),.        
-00012b70: 2020 2020 2773 6c65 6570 2031 3030 272c      'sleep 100',
-00012b80: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
-00012b90: 5f53 504f 545f 5155 4555 455f 5741 4954  _SPOT_QUEUE_WAIT
-00012ba0: 7d7c 2067 7265 7020 7b6e 616d 657d 207c  }| grep {name} |
-00012bb0: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
-00012bc0: 2022 5245 434f 5645 5249 4e47 2227 2c0a   "RECOVERING"',.
-00012bd0: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
-00012be0: 6570 2032 3030 272c 0a20 2020 2020 2020  ep 200',.       
-00012bf0: 2020 2020 2066 277b 5f53 504f 545f 5155       f'{_SPOT_QU
-00012c00: 4555 455f 5741 4954 7d7c 2067 7265 7020  EUE_WAIT}| grep 
-00012c10: 7b6e 616d 657d 207c 2068 6561 6420 2d6e  {name} | head -n
-00012c20: 3120 7c20 6772 6570 2022 5255 4e4e 494e  1 | grep "RUNNIN
-00012c30: 4722 272c 0a20 2020 2020 2020 2020 2020  G"',.           
-00012c40: 2066 2752 554e 5f49 443d 2428 6361 7420   f'RUN_ID=$(cat 
-00012c50: 2f74 6d70 2f7b 6e61 6d65 7d2d 7275 6e2d  /tmp/{name}-run-
-00012c60: 6964 293b 2065 6368 6f20 2452 554e 5f49  id); echo $RUN_I
-00012c70: 443b 2073 6b79 2073 706f 7420 6c6f 6773  D; sky spot logs
-00012c80: 202d 6e20 7b6e 616d 657d 202d 2d6e 6f2d   -n {name} --no-
-00012c90: 666f 6c6c 6f77 207c 2067 7265 7020 534b  follow | grep SK
-00012ca0: 5950 494c 4f54 5f54 4153 4b5f 4944 3a20  YPILOT_TASK_ID: 
-00012cb0: 7c20 6772 6570 2022 2452 554e 5f49 4422  | grep "$RUN_ID"
-00012cc0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-00012cd0: 2752 554e 5f49 4453 3d24 2873 6b79 2073  'RUN_IDS=$(sky s
-00012ce0: 706f 7420 6c6f 6773 202d 6e20 7b6e 616d  pot logs -n {nam
-00012cf0: 657d 202d 2d6e 6f2d 666f 6c6c 6f77 207c  e} --no-follow |
-00012d00: 2067 7265 7020 2d41 2034 2053 4b59 5049   grep -A 4 SKYPI
-00012d10: 4c4f 545f 5441 534b 5f49 4453 207c 2063  LOT_TASK_IDS | c
-00012d20: 7574 202d 6422 2922 202d 6632 293b 2065  ut -d")" -f2); e
-00012d30: 6368 6f20 2224 5255 4e5f 4944 5322 207c  cho "$RUN_IDS" |
-00012d40: 2074 6565 202f 746d 702f 7b6e 616d 657d   tee /tmp/{name}
-00012d50: 2d72 756e 2d69 6473 2d6e 6577 272c 0a20  -run-ids-new',. 
-00012d60: 2020 2020 2020 2020 2020 2066 2764 6966             f'dif
-00012d70: 6620 2f74 6d70 2f7b 6e61 6d65 7d2d 7275  f /tmp/{name}-ru
-00012d80: 6e2d 6964 7320 2f74 6d70 2f7b 6e61 6d65  n-ids /tmp/{name
-00012d90: 7d2d 7275 6e2d 6964 732d 6e65 7727 2c0a  }-run-ids-new',.
-00012da0: 2020 2020 2020 2020 2020 2020 6627 6361              f'ca
-00012db0: 7420 2f74 6d70 2f7b 6e61 6d65 7d2d 7275  t /tmp/{name}-ru
-00012dc0: 6e2d 6964 7320 7c20 7365 6420 2d6e 2032  n-ids | sed -n 2
-00012dd0: 7020 7c20 6772 6570 2060 6361 7420 2f74  p | grep `cat /t
-00012de0: 6d70 2f7b 6e61 6d65 7d2d 7275 6e2d 6964  mp/{name}-run-id
-00012df0: 6027 2c0a 2020 2020 2020 2020 5d2c 0a20  `',.        ],. 
-00012e00: 2020 2020 2020 205f 5350 4f54 5f43 414e         _SPOT_CAN
-00012e10: 4345 4c5f 5741 4954 2e66 6f72 6d61 7428  CEL_WAIT.format(
-00012e20: 6a6f 625f 6e61 6d65 3d6e 616d 6529 2c0a  job_name=name),.
-00012e30: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
-00012e40: 3235 202a 2036 302c 0a20 2020 2029 0a20  25 * 60,.    ). 
-00012e50: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
-00012e60: 7465 7374 290a 0a0a 4070 7974 6573 742e  test)...@pytest.
-00012e70: 6d61 726b 2e6e 6f5f 6c61 6d62 6461 5f63  mark.no_lambda_c
-00012e80: 6c6f 7564 2020 2320 4c61 6d62 6461 2043  loud  # Lambda C
-00012e90: 6c6f 7564 2064 6f65 7320 6e6f 7420 7375  loud does not su
-00012ea0: 7070 6f72 7420 7370 6f74 2069 6e73 7461  pport spot insta
-00012eb0: 6e63 6573 0a40 7079 7465 7374 2e6d 6172  nces.@pytest.mar
-00012ec0: 6b2e 6e6f 5f69 626d 2020 2320 4942 4d20  k.no_ibm  # IBM 
-00012ed0: 436c 6f75 6420 646f 6573 206e 6f74 2073  Cloud does not s
-00012ee0: 7570 706f 7274 2073 706f 7420 696e 7374  upport spot inst
-00012ef0: 616e 6365 730a 4070 7974 6573 742e 6d61  ances.@pytest.ma
-00012f00: 726b 2e6e 6f5f 7363 7020 2023 2053 4350  rk.no_scp  # SCP
-00012f10: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
-00012f20: 7420 7370 6f74 2069 6e73 7461 6e63 6573  t spot instances
-00012f30: 0a40 7079 7465 7374 2e6d 6172 6b2e 6d61  .@pytest.mark.ma
-00012f40: 6e61 6765 645f 7370 6f74 0a64 6566 2074  naged_spot.def t
-00012f50: 6573 745f 7370 6f74 5f72 6563 6f76 6572  est_spot_recover
-00012f60: 795f 6465 6661 756c 745f 7265 736f 7572  y_default_resour
-00012f70: 6365 7328 6765 6e65 7269 635f 636c 6f75  ces(generic_clou
-00012f80: 643a 2073 7472 293a 0a20 2020 2022 2222  d: str):.    """
-00012f90: 5465 7374 206d 616e 6167 6564 2073 706f  Test managed spo
-00012fa0: 7420 7265 636f 7665 7279 2066 6f72 2064  t recovery for d
-00012fb0: 6566 6175 6c74 2072 6573 6f75 7263 6573  efault resources
-00012fc0: 2e22 2222 0a20 2020 206e 616d 6520 3d20  .""".    name = 
-00012fd0: 5f67 6574 5f63 6c75 7374 6572 5f6e 616d  _get_cluster_nam
-00012fe0: 6528 290a 2020 2020 7465 7374 203d 2054  e().    test = T
-00012ff0: 6573 7428 0a20 2020 2020 2020 2027 6d61  est(.        'ma
-00013000: 6e61 6765 642d 7370 6f74 2d72 6563 6f76  naged-spot-recov
-00013010: 6572 792d 6465 6661 756c 742d 7265 736f  ery-default-reso
-00013020: 7572 6365 7327 2c0a 2020 2020 2020 2020  urces',.        
-00013030: 5b0a 2020 2020 2020 2020 2020 2020 6627  [.            f'
-00013040: 736b 7920 7370 6f74 206c 6175 6e63 6820  sky spot launch 
-00013050: 2d6e 207b 6e61 6d65 7d20 2d2d 636c 6f75  -n {name} --clou
-00013060: 6420 7b67 656e 6572 6963 5f63 6c6f 7564  d {generic_cloud
-00013070: 7d20 2273 6c65 6570 2033 3020 2626 2073  } "sleep 30 && s
-00013080: 7564 6f20 7368 7574 646f 776e 206e 6f77  udo shutdown now
-00013090: 2026 2620 736c 6565 7020 3130 3030 2220   && sleep 1000" 
-000130a0: 2d79 202d 6427 2c0a 2020 2020 2020 2020  -y -d',.        
-000130b0: 2020 2020 2773 6c65 6570 2033 3630 272c      'sleep 360',
-000130c0: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
-000130d0: 5f53 504f 545f 5155 4555 455f 5741 4954  _SPOT_QUEUE_WAIT
-000130e0: 7d7c 2067 7265 7020 7b6e 616d 657d 207c  }| grep {name} |
-000130f0: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
-00013100: 2022 5255 4e4e 494e 475c 7c52 4543 4f56   "RUNNING\|RECOV
-00013110: 4552 494e 4722 272c 0a20 2020 2020 2020  ERING"',.       
-00013120: 205d 2c0a 2020 2020 2020 2020 5f53 504f   ],.        _SPO
-00013130: 545f 4341 4e43 454c 5f57 4149 542e 666f  T_CANCEL_WAIT.fo
-00013140: 726d 6174 286a 6f62 5f6e 616d 653d 6e61  rmat(job_name=na
-00013150: 6d65 292c 0a20 2020 2020 2020 2074 696d  me),.        tim
-00013160: 656f 7574 3d32 3520 2a20 3630 2c0a 2020  eout=25 * 60,.  
-00013170: 2020 290a 2020 2020 7275 6e5f 6f6e 655f    ).    run_one_
-00013180: 7465 7374 2874 6573 7429 0a0a 0a40 7079  test(test)...@py
-00013190: 7465 7374 2e6d 6172 6b2e 6177 730a 4070  test.mark.aws.@p
-000131a0: 7974 6573 742e 6d61 726b 2e6d 616e 6167  ytest.mark.manag
-000131b0: 6564 5f73 706f 740a 6465 6620 7465 7374  ed_spot.def test
-000131c0: 5f73 706f 745f 7265 636f 7665 7279 5f6d  _spot_recovery_m
-000131d0: 756c 7469 5f6e 6f64 655f 6177 7328 6177  ulti_node_aws(aw
-000131e0: 735f 636f 6e66 6967 5f72 6567 696f 6e29  s_config_region)
-000131f0: 3a0a 2020 2020 2222 2254 6573 7420 6d61  :.    """Test ma
-00013200: 6e61 6765 6420 7370 6f74 2072 6563 6f76  naged spot recov
-00013210: 6572 792e 2222 220a 2020 2020 6e61 6d65  ery.""".    name
-00013220: 203d 205f 6765 745f 636c 7573 7465 725f   = _get_cluster_
-00013230: 6e61 6d65 2829 0a20 2020 2072 6567 696f  name().    regio
-00013240: 6e20 3d20 6177 735f 636f 6e66 6967 5f72  n = aws_config_r
-00013250: 6567 696f 6e0a 2020 2020 7465 7374 203d  egion.    test =
-00013260: 2054 6573 7428 0a20 2020 2020 2020 2027   Test(.        '
-00013270: 7370 6f74 5f72 6563 6f76 6572 795f 6d75  spot_recovery_mu
-00013280: 6c74 695f 6e6f 6465 5f61 7773 272c 0a20  lti_node_aws',. 
-00013290: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-000132a0: 2020 2020 2066 2773 6b79 2073 706f 7420       f'sky spot 
-000132b0: 6c61 756e 6368 202d 2d63 6c6f 7564 2061  launch --cloud a
-000132c0: 7773 202d 2d72 6567 696f 6e20 7b72 6567  ws --region {reg
-000132d0: 696f 6e7d 202d 6e20 7b6e 616d 657d 202d  ion} -n {name} -
-000132e0: 2d6e 756d 2d6e 6f64 6573 2032 2022 6563  -num-nodes 2 "ec
-000132f0: 686f 2053 4b59 5049 4c4f 545f 5441 534b  ho SKYPILOT_TASK
-00013300: 5f49 443a 205c 2453 4b59 5049 4c4f 545f  _ID: \$SKYPILOT_
-00013310: 5441 534b 5f49 443b 2073 6c65 6570 2031  TASK_ID; sleep 1
-00013320: 3830 3022 2020 2d79 202d 6427 2c0a 2020  800"  -y -d',.  
-00013330: 2020 2020 2020 2020 2020 2773 6c65 6570            'sleep
-00013340: 2034 3530 272c 0a20 2020 2020 2020 2020   450',.         
-00013350: 2020 2066 277b 5f53 504f 545f 5155 4555     f'{_SPOT_QUEU
-00013360: 455f 5741 4954 7d7c 2067 7265 7020 7b6e  E_WAIT}| grep {n
-00013370: 616d 657d 207c 2068 6561 6420 2d6e 3120  ame} | head -n1 
-00013380: 7c20 6772 6570 2022 5255 4e4e 494e 4722  | grep "RUNNING"
-00013390: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-000133a0: 2752 554e 5f49 443d 2428 736b 7920 7370  'RUN_ID=$(sky sp
-000133b0: 6f74 206c 6f67 7320 2d6e 207b 6e61 6d65  ot logs -n {name
-000133c0: 7d20 2d2d 6e6f 2d66 6f6c 6c6f 7720 7c20  } --no-follow | 
-000133d0: 6772 6570 2053 4b59 5049 4c4f 545f 5441  grep SKYPILOT_TA
-000133e0: 534b 5f49 4420 7c20 6375 7420 2d64 3a20  SK_ID | cut -d: 
-000133f0: 2d66 3229 3b20 6563 686f 2022 2452 554e  -f2); echo "$RUN
-00013400: 5f49 4422 207c 2074 6565 202f 746d 702f  _ID" | tee /tmp/
-00013410: 7b6e 616d 657d 2d72 756e 2d69 6427 2c0a  {name}-run-id',.
-00013420: 2020 2020 2020 2020 2020 2020 2320 5465              # Te
-00013430: 726d 696e 6174 6520 7468 6520 776f 726b  rminate the work
-00013440: 6572 206d 616e 7561 6c6c 792e 0a20 2020  er manually..   
-00013450: 2020 2020 2020 2020 2028 6627 6177 7320           (f'aws 
-00013460: 6563 3220 7465 726d 696e 6174 652d 696e  ec2 terminate-in
-00013470: 7374 616e 6365 7320 2d2d 7265 6769 6f6e  stances --region
-00013480: 207b 7265 6769 6f6e 7d20 2d2d 696e 7374   {region} --inst
-00013490: 616e 6365 2d69 6473 2024 2827 0a20 2020  ance-ids $('.   
-000134a0: 2020 2020 2020 2020 2020 6627 6177 7320            f'aws 
-000134b0: 6563 3220 6465 7363 7269 6265 2d69 6e73  ec2 describe-ins
-000134c0: 7461 6e63 6573 202d 2d72 6567 696f 6e20  tances --region 
-000134d0: 7b72 6567 696f 6e7d 2027 0a20 2020 2020  {region} '.     
-000134e0: 2020 2020 2020 2020 6627 2d2d 6669 6c74          f'--filt
-000134f0: 6572 7320 4e61 6d65 3d74 6167 3a72 6179  ers Name=tag:ray
-00013500: 2d63 6c75 7374 6572 2d6e 616d 652c 5661  -cluster-name,Va
-00013510: 6c75 6573 3d7b 6e61 6d65 7d2a 2027 0a20  lues={name}* '. 
-00013520: 2020 2020 2020 2020 2020 2020 274e 616d              'Nam
-00013530: 653d 7461 673a 7261 792d 6e6f 6465 2d74  e=tag:ray-node-t
-00013540: 7970 652c 5661 6c75 6573 3d77 6f72 6b65  ype,Values=worke
-00013550: 7220 270a 2020 2020 2020 2020 2020 2020  r '.            
-00013560: 2066 272d 2d71 7565 7279 2052 6573 6572   f'--query Reser
-00013570: 7661 7469 6f6e 735b 5d2e 496e 7374 616e  vations[].Instan
-00013580: 6365 735b 5d2e 496e 7374 616e 6365 4964  ces[].InstanceId
-00013590: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-000135a0: 272d 2d6f 7574 7075 7420 7465 7874 2927  '--output text)'
-000135b0: 292c 0a20 2020 2020 2020 2020 2020 2027  ),.            '
-000135c0: 736c 6565 7020 3530 272c 0a20 2020 2020  sleep 50',.     
-000135d0: 2020 2020 2020 2066 277b 5f53 504f 545f         f'{_SPOT_
-000135e0: 5155 4555 455f 5741 4954 7d7c 2067 7265  QUEUE_WAIT}| gre
-000135f0: 7020 7b6e 616d 657d 207c 2068 6561 6420  p {name} | head 
-00013600: 2d6e 3120 7c20 6772 6570 2022 5245 434f  -n1 | grep "RECO
-00013610: 5645 5249 4e47 2227 2c0a 2020 2020 2020  VERING"',.      
-00013620: 2020 2020 2020 2773 6c65 6570 2035 3630        'sleep 560
-00013630: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-00013640: 277b 5f53 504f 545f 5155 4555 455f 5741  '{_SPOT_QUEUE_WA
-00013650: 4954 7d7c 2067 7265 7020 7b6e 616d 657d  IT}| grep {name}
-00013660: 207c 2068 6561 6420 2d6e 3120 7c20 6772   | head -n1 | gr
-00013670: 6570 2022 5255 4e4e 494e 4722 272c 0a20  ep "RUNNING"',. 
-00013680: 2020 2020 2020 2020 2020 2066 2752 554e             f'RUN
-00013690: 5f49 443d 2428 6361 7420 2f74 6d70 2f7b  _ID=$(cat /tmp/{
-000136a0: 6e61 6d65 7d2d 7275 6e2d 6964 293b 2065  name}-run-id); e
-000136b0: 6368 6f20 2452 554e 5f49 443b 2073 6b79  cho $RUN_ID; sky
-000136c0: 2073 706f 7420 6c6f 6773 202d 6e20 7b6e   spot logs -n {n
-000136d0: 616d 657d 202d 2d6e 6f2d 666f 6c6c 6f77  ame} --no-follow
-000136e0: 207c 2067 7265 7020 534b 5950 494c 4f54   | grep SKYPILOT
-000136f0: 5f54 4153 4b5f 4944 207c 2063 7574 202d  _TASK_ID | cut -
-00013700: 643a 202d 6632 207c 2067 7265 7020 2224  d: -f2 | grep "$
-00013710: 5255 4e5f 4944 2227 2c0a 2020 2020 2020  RUN_ID"',.      
-00013720: 2020 5d2c 0a20 2020 2020 2020 205f 5350    ],.        _SP
-00013730: 4f54 5f43 414e 4345 4c5f 5741 4954 2e66  OT_CANCEL_WAIT.f
-00013740: 6f72 6d61 7428 6a6f 625f 6e61 6d65 3d6e  ormat(job_name=n
-00013750: 616d 6529 2c0a 2020 2020 2020 2020 7469  ame),.        ti
-00013760: 6d65 6f75 743d 3330 202a 2036 302c 0a20  meout=30 * 60,. 
-00013770: 2020 2029 0a20 2020 2072 756e 5f6f 6e65     ).    run_one
-00013780: 5f74 6573 7428 7465 7374 290a 0a0a 4070  _test(test)...@p
-00013790: 7974 6573 742e 6d61 726b 2e67 6370 0a40  ytest.mark.gcp.@
-000137a0: 7079 7465 7374 2e6d 6172 6b2e 6d61 6e61  pytest.mark.mana
-000137b0: 6765 645f 7370 6f74 0a64 6566 2074 6573  ged_spot.def tes
-000137c0: 745f 7370 6f74 5f72 6563 6f76 6572 795f  t_spot_recovery_
-000137d0: 6d75 6c74 695f 6e6f 6465 5f67 6370 2829  multi_node_gcp()
-000137e0: 3a0a 2020 2020 2222 2254 6573 7420 6d61  :.    """Test ma
-000137f0: 6e61 6765 6420 7370 6f74 2072 6563 6f76  naged spot recov
-00013800: 6572 792e 2222 220a 2020 2020 6e61 6d65  ery.""".    name
-00013810: 203d 205f 6765 745f 636c 7573 7465 725f   = _get_cluster_
-00013820: 6e61 6d65 2829 0a20 2020 207a 6f6e 6520  name().    zone 
-00013830: 3d20 2775 732d 7765 7374 322d 6127 0a20  = 'us-west2-a'. 
-00013840: 2020 2023 2055 7365 2027 3a27 2074 6f20     # Use ':' to 
-00013850: 6d61 7463 6820 6173 2074 6865 2063 6c75  match as the clu
-00013860: 7374 6572 206e 616d 6520 7769 6c6c 2063  ster name will c
-00013870: 6f6e 7461 696e 2074 6865 2073 7566 6669  ontain the suffi
-00013880: 7820 7769 7468 206a 6f62 2069 640a 2020  x with job id.  
-00013890: 2020 7175 6572 795f 636d 6420 3d20 280a    query_cmd = (.
-000138a0: 2020 2020 2020 2020 6627 6763 6c6f 7564          f'gcloud
-000138b0: 2063 6f6d 7075 7465 2069 6e73 7461 6e63   compute instanc
-000138c0: 6573 206c 6973 7420 2d2d 6669 6c74 6572  es list --filter
-000138d0: 3d27 0a20 2020 2020 2020 2066 2722 286c  ='.        f'"(l
-000138e0: 6162 656c 732e 7261 792d 636c 7573 7465  abels.ray-cluste
-000138f0: 722d 6e61 6d65 3a7b 6e61 6d65 7d20 414e  r-name:{name} AN
-00013900: 4420 6c61 6265 6c73 2e72 6179 2d6e 6f64  D labels.ray-nod
-00013910: 652d 7479 7065 3d77 6f72 6b65 7229 2220  e-type=worker)" 
-00013920: 270a 2020 2020 2020 2020 6627 2d2d 7a6f  '.        f'--zo
-00013930: 6e65 733d 7b7a 6f6e 657d 202d 2d66 6f72  nes={zone} --for
-00013940: 6d61 743d 2276 616c 7565 286e 616d 6529  mat="value(name)
-00013950: 2227 290a 2020 2020 7465 726d 696e 6174  "').    terminat
-00013960: 655f 636d 6420 3d20 2866 2767 636c 6f75  e_cmd = (f'gclou
-00013970: 6420 636f 6d70 7574 6520 696e 7374 616e  d compute instan
-00013980: 6365 7320 6465 6c65 7465 202d 2d7a 6f6e  ces delete --zon
-00013990: 653d 7b7a 6f6e 657d 270a 2020 2020 2020  e={zone}'.      
-000139a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000139b0: 2720 2d2d 7175 6965 7420 2428 7b71 7565  ' --quiet $({que
-000139c0: 7279 5f63 6d64 7d29 2729 0a20 2020 2074  ry_cmd})').    t
-000139d0: 6573 7420 3d20 5465 7374 280a 2020 2020  est = Test(.    
-000139e0: 2020 2020 2773 706f 745f 7265 636f 7665      'spot_recove
-000139f0: 7279 5f6d 756c 7469 5f6e 6f64 655f 6763  ry_multi_node_gc
-00013a00: 7027 2c0a 2020 2020 2020 2020 5b0a 2020  p',.        [.  
-00013a10: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
-00013a20: 7370 6f74 206c 6175 6e63 6820 2d2d 636c  spot launch --cl
-00013a30: 6f75 6420 6763 7020 2d2d 7a6f 6e65 207b  oud gcp --zone {
-00013a40: 7a6f 6e65 7d20 2d6e 207b 6e61 6d65 7d20  zone} -n {name} 
-00013a50: 2d2d 6e75 6d2d 6e6f 6465 7320 3220 2265  --num-nodes 2 "e
-00013a60: 6368 6f20 534b 5950 494c 4f54 5f54 4153  cho SKYPILOT_TAS
-00013a70: 4b5f 4944 3a20 5c24 534b 5950 494c 4f54  K_ID: \$SKYPILOT
-00013a80: 5f54 4153 4b5f 4944 3b20 736c 6565 7020  _TASK_ID; sleep 
-00013a90: 3138 3030 2220 202d 7920 2d64 272c 0a20  1800"  -y -d',. 
-00013aa0: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
-00013ab0: 7020 3430 3027 2c0a 2020 2020 2020 2020  p 400',.        
-00013ac0: 2020 2020 6627 7b5f 5350 4f54 5f51 5545      f'{_SPOT_QUE
-00013ad0: 5545 5f57 4149 547d 7c20 6772 6570 207b  UE_WAIT}| grep {
-00013ae0: 6e61 6d65 7d20 7c20 6865 6164 202d 6e31  name} | head -n1
-00013af0: 207c 2067 7265 7020 2252 554e 4e49 4e47   | grep "RUNNING
-00013b00: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-00013b10: 6627 5255 4e5f 4944 3d24 2873 6b79 2073  f'RUN_ID=$(sky s
-00013b20: 706f 7420 6c6f 6773 202d 6e20 7b6e 616d  pot logs -n {nam
-00013b30: 657d 202d 2d6e 6f2d 666f 6c6c 6f77 207c  e} --no-follow |
-00013b40: 2067 7265 7020 534b 5950 494c 4f54 5f54   grep SKYPILOT_T
-00013b50: 4153 4b5f 4944 207c 2063 7574 202d 643a  ASK_ID | cut -d:
-00013b60: 202d 6632 293b 2065 6368 6f20 2224 5255   -f2); echo "$RU
-00013b70: 4e5f 4944 2220 7c20 7465 6520 2f74 6d70  N_ID" | tee /tmp
-00013b80: 2f7b 6e61 6d65 7d2d 7275 6e2d 6964 272c  /{name}-run-id',
-00013b90: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
-00013ba0: 6572 6d69 6e61 7465 2074 6865 2077 6f72  erminate the wor
-00013bb0: 6b65 7220 6d61 6e75 616c 6c79 2e0a 2020  ker manually..  
-00013bc0: 2020 2020 2020 2020 2020 7465 726d 696e            termin
-00013bd0: 6174 655f 636d 642c 0a20 2020 2020 2020  ate_cmd,.       
-00013be0: 2020 2020 2027 736c 6565 7020 3530 272c       'sleep 50',
-00013bf0: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
-00013c00: 5f53 504f 545f 5155 4555 455f 5741 4954  _SPOT_QUEUE_WAIT
-00013c10: 7d7c 2067 7265 7020 7b6e 616d 657d 207c  }| grep {name} |
-00013c20: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
-00013c30: 2022 5245 434f 5645 5249 4e47 2227 2c0a   "RECOVERING"',.
-00013c40: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
-00013c50: 6570 2034 3230 272c 0a20 2020 2020 2020  ep 420',.       
-00013c60: 2020 2020 2066 277b 5f53 504f 545f 5155       f'{_SPOT_QU
-00013c70: 4555 455f 5741 4954 7d7c 2067 7265 7020  EUE_WAIT}| grep 
-00013c80: 7b6e 616d 657d 207c 2068 6561 6420 2d6e  {name} | head -n
-00013c90: 3120 7c20 6772 6570 2022 5255 4e4e 494e  1 | grep "RUNNIN
-00013ca0: 4722 272c 0a20 2020 2020 2020 2020 2020  G"',.           
-00013cb0: 2066 2752 554e 5f49 443d 2428 6361 7420   f'RUN_ID=$(cat 
-00013cc0: 2f74 6d70 2f7b 6e61 6d65 7d2d 7275 6e2d  /tmp/{name}-run-
-00013cd0: 6964 293b 2065 6368 6f20 2452 554e 5f49  id); echo $RUN_I
-00013ce0: 443b 2073 6b79 2073 706f 7420 6c6f 6773  D; sky spot logs
-00013cf0: 202d 6e20 7b6e 616d 657d 202d 2d6e 6f2d   -n {name} --no-
-00013d00: 666f 6c6c 6f77 207c 2067 7265 7020 534b  follow | grep SK
-00013d10: 5950 494c 4f54 5f54 4153 4b5f 4944 207c  YPILOT_TASK_ID |
-00013d20: 2063 7574 202d 643a 202d 6632 207c 2067   cut -d: -f2 | g
-00013d30: 7265 7020 2224 5255 4e5f 4944 2227 2c0a  rep "$RUN_ID"',.
-00013d40: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00013d50: 2020 205f 5350 4f54 5f43 414e 4345 4c5f     _SPOT_CANCEL_
-00013d60: 5741 4954 2e66 6f72 6d61 7428 6a6f 625f  WAIT.format(job_
-00013d70: 6e61 6d65 3d6e 616d 6529 2c0a 2020 2020  name=name),.    
-00013d80: 2020 2020 7469 6d65 6f75 743d 3235 202a      timeout=25 *
-00013d90: 2036 302c 0a20 2020 2029 0a20 2020 2072   60,.    ).    r
-00013da0: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
-00013db0: 290a 0a0a 4070 7974 6573 742e 6d61 726b  )...@pytest.mark
-00013dc0: 2e61 7773 0a40 7079 7465 7374 2e6d 6172  .aws.@pytest.mar
-00013dd0: 6b2e 6d61 6e61 6765 645f 7370 6f74 0a64  k.managed_spot.d
-00013de0: 6566 2074 6573 745f 7370 6f74 5f63 616e  ef test_spot_can
-00013df0: 6365 6c6c 6174 696f 6e5f 6177 7328 6177  cellation_aws(aw
-00013e00: 735f 636f 6e66 6967 5f72 6567 696f 6e29  s_config_region)
-00013e10: 3a0a 2020 2020 6e61 6d65 203d 205f 6765  :.    name = _ge
-00013e20: 745f 636c 7573 7465 725f 6e61 6d65 2829  t_cluster_name()
-00013e30: 0a20 2020 2072 6567 696f 6e20 3d20 6177  .    region = aw
-00013e40: 735f 636f 6e66 6967 5f72 6567 696f 6e0a  s_config_region.
-00013e50: 2020 2020 7465 7374 203d 2054 6573 7428      test = Test(
-00013e60: 0a20 2020 2020 2020 2027 7370 6f74 5f63  .        'spot_c
-00013e70: 616e 6365 6c6c 6174 696f 6e5f 6177 7327  ancellation_aws'
-00013e80: 2c0a 2020 2020 2020 2020 5b0a 2020 2020  ,.        [.    
-00013e90: 2020 2020 2020 2020 2320 5465 7374 2063          # Test c
-00013ea0: 616e 6365 6c6c 6174 696f 6e20 6475 7269  ancellation duri
-00013eb0: 6e67 2073 706f 7420 636c 7573 7465 7220  ng spot cluster 
-00013ec0: 6265 696e 6720 6c61 756e 6368 6564 2e0a  being launched..
-00013ed0: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-00013ee0: 7920 7370 6f74 206c 6175 6e63 6820 2d2d  y spot launch --
-00013ef0: 636c 6f75 6420 6177 7320 2d2d 7265 6769  cloud aws --regi
-00013f00: 6f6e 207b 7265 6769 6f6e 7d20 2d6e 207b  on {region} -n {
-00013f10: 6e61 6d65 7d20 2273 6c65 6570 2031 3030  name} "sleep 100
-00013f20: 3022 2020 2d79 202d 6427 2c0a 2020 2020  0"  -y -d',.    
-00013f30: 2020 2020 2020 2020 2773 6c65 6570 2036          'sleep 6
-00013f40: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
-00013f50: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
-00013f60: 4149 547d 7c20 6772 6570 207b 6e61 6d65  AIT}| grep {name
-00013f70: 7d20 7c20 6865 6164 202d 6e31 207c 2067  } | head -n1 | g
-00013f80: 7265 7020 2253 5441 5254 494e 4722 272c  rep "STARTING"',
-00013f90: 0a20 2020 2020 2020 2020 2020 205f 5350  .            _SP
-00013fa0: 4f54 5f43 414e 4345 4c5f 5741 4954 2e66  OT_CANCEL_WAIT.f
-00013fb0: 6f72 6d61 7428 6a6f 625f 6e61 6d65 3d6e  ormat(job_name=n
-00013fc0: 616d 6529 2c0a 2020 2020 2020 2020 2020  ame),.          
-00013fd0: 2020 2773 6c65 6570 2035 272c 0a20 2020    'sleep 5',.   
-00013fe0: 2020 2020 2020 2020 2066 277b 5f53 504f           f'{_SPO
-00013ff0: 545f 5155 4555 455f 5741 4954 7d7c 2067  T_QUEUE_WAIT}| g
-00014000: 7265 7020 7b6e 616d 657d 207c 2068 6561  rep {name} | hea
-00014010: 6420 2d6e 3120 7c20 6772 6570 2022 4341  d -n1 | grep "CA
-00014020: 4e43 454c 4c49 4e47 5c7c 4341 4e43 454c  NCELLING\|CANCEL
-00014030: 4c45 4422 272c 0a20 2020 2020 2020 2020  LED"',.         
-00014040: 2020 2027 736c 6565 7020 3132 3027 2c0a     'sleep 120',.
-00014050: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
-00014060: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
-00014070: 7c20 6772 6570 207b 6e61 6d65 7d20 7c20  | grep {name} | 
-00014080: 6865 6164 202d 6e31 207c 2067 7265 7020  head -n1 | grep 
-00014090: 2243 414e 4345 4c4c 4544 2227 2c0a 2020  "CANCELLED"',.  
-000140a0: 2020 2020 2020 2020 2020 2866 2773 3d24            (f's=$
-000140b0: 2861 7773 2065 6332 2064 6573 6372 6962  (aws ec2 describ
-000140c0: 652d 696e 7374 616e 6365 7320 2d2d 7265  e-instances --re
-000140d0: 6769 6f6e 207b 7265 6769 6f6e 7d20 270a  gion {region} '.
-000140e0: 2020 2020 2020 2020 2020 2020 2066 272d               f'-
-000140f0: 2d66 696c 7465 7273 204e 616d 653d 7461  -filters Name=ta
-00014100: 673a 7261 792d 636c 7573 7465 722d 6e61  g:ray-cluster-na
-00014110: 6d65 2c56 616c 7565 733d 7b6e 616d 657d  me,Values={name}
-00014120: 2d2a 2027 0a20 2020 2020 2020 2020 2020  -* '.           
-00014130: 2020 6627 2d2d 7175 6572 7920 5265 7365    f'--query Rese
-00014140: 7276 6174 696f 6e73 5b5d 2e49 6e73 7461  rvations[].Insta
-00014150: 6e63 6573 5b5d 2e53 7461 7465 5b5d 2e4e  nces[].State[].N
-00014160: 616d 6520 270a 2020 2020 2020 2020 2020  ame '.          
-00014170: 2020 2027 2d2d 6f75 7470 7574 2074 6578     '--output tex
-00014180: 7429 2026 2620 6563 686f 2022 2473 2220  t) && echo "$s" 
-00014190: 2626 2065 6368 6f3b 205b 5b20 2d7a 2022  && echo; [[ -z "
-000141a0: 2473 2220 5d5d 207c 7c20 5b5b 2022 2473  $s" ]] || [[ "$s
-000141b0: 2220 3d20 2274 6572 6d69 6e61 7465 6422  " = "terminated"
-000141c0: 205d 5d20 7c7c 205b 5b20 2224 7322 203d   ]] || [[ "$s" =
-000141d0: 2022 7368 7574 7469 6e67 2d64 6f77 6e22   "shutting-down"
-000141e0: 205d 5d27 0a20 2020 2020 2020 2020 2020   ]]'.           
-000141f0: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00014200: 2320 5465 7374 2063 616e 6365 6c6c 696e  # Test cancellin
-00014210: 6720 7468 6520 7370 6f74 2063 6c75 7374  g the spot clust
-00014220: 6572 2064 7572 696e 6720 7370 6f74 206a  er during spot j
-00014230: 6f62 2062 6569 6e67 2073 6574 7570 2e0a  ob being setup..
-00014240: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-00014250: 7920 7370 6f74 206c 6175 6e63 6820 2d2d  y spot launch --
-00014260: 636c 6f75 6420 6177 7320 2d2d 7265 6769  cloud aws --regi
-00014270: 6f6e 207b 7265 6769 6f6e 7d20 2d6e 207b  on {region} -n {
-00014280: 6e61 6d65 7d2d 3220 7465 7374 732f 7465  name}-2 tests/te
-00014290: 7374 5f79 616d 6c73 2f74 6573 745f 6c6f  st_yamls/test_lo
-000142a0: 6e67 5f73 6574 7570 2e79 616d 6c20 202d  ng_setup.yaml  -
-000142b0: 7920 2d64 272c 0a20 2020 2020 2020 2020  y -d',.         
-000142c0: 2020 2027 736c 6565 7020 3330 3027 2c0a     'sleep 300',.
-000142d0: 2020 2020 2020 2020 2020 2020 5f53 504f              _SPO
-000142e0: 545f 4341 4e43 454c 5f57 4149 542e 666f  T_CANCEL_WAIT.fo
-000142f0: 726d 6174 286a 6f62 5f6e 616d 653d 6627  rmat(job_name=f'
-00014300: 7b6e 616d 657d 2d32 2729 2c0a 2020 2020  {name}-2'),.    
-00014310: 2020 2020 2020 2020 2773 6c65 6570 2035          'sleep 5
-00014320: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-00014330: 277b 5f53 504f 545f 5155 4555 455f 5741  '{_SPOT_QUEUE_WA
-00014340: 4954 7d7c 2067 7265 7020 7b6e 616d 657d  IT}| grep {name}
-00014350: 2d32 207c 2068 6561 6420 2d6e 3120 7c20  -2 | head -n1 | 
-00014360: 6772 6570 2022 4341 4e43 454c 4c49 4e47  grep "CANCELLING
-00014370: 5c7c 4341 4e43 454c 4c45 4422 272c 0a20  \|CANCELLED"',. 
-00014380: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
-00014390: 7020 3132 3027 2c0a 2020 2020 2020 2020  p 120',.        
-000143a0: 2020 2020 6627 7b5f 5350 4f54 5f51 5545      f'{_SPOT_QUE
-000143b0: 5545 5f57 4149 547d 7c20 6772 6570 207b  UE_WAIT}| grep {
-000143c0: 6e61 6d65 7d2d 3220 7c20 6865 6164 202d  name}-2 | head -
-000143d0: 6e31 207c 2067 7265 7020 2243 414e 4345  n1 | grep "CANCE
-000143e0: 4c4c 4544 2227 2c0a 2020 2020 2020 2020  LLED"',.        
-000143f0: 2020 2020 2866 2773 3d24 2861 7773 2065      (f's=$(aws e
-00014400: 6332 2064 6573 6372 6962 652d 696e 7374  c2 describe-inst
-00014410: 616e 6365 7320 2d2d 7265 6769 6f6e 207b  ances --region {
-00014420: 7265 6769 6f6e 7d20 270a 2020 2020 2020  region} '.      
-00014430: 2020 2020 2020 2066 272d 2d66 696c 7465         f'--filte
-00014440: 7273 204e 616d 653d 7461 673a 7261 792d  rs Name=tag:ray-
-00014450: 636c 7573 7465 722d 6e61 6d65 2c56 616c  cluster-name,Val
-00014460: 7565 733d 7b6e 616d 657d 2d32 2d2a 2027  ues={name}-2-* '
-00014470: 0a20 2020 2020 2020 2020 2020 2020 6627  .             f'
-00014480: 2d2d 7175 6572 7920 5265 7365 7276 6174  --query Reservat
-00014490: 696f 6e73 5b5d 2e49 6e73 7461 6e63 6573  ions[].Instances
-000144a0: 5b5d 2e53 7461 7465 5b5d 2e4e 616d 6520  [].State[].Name 
-000144b0: 270a 2020 2020 2020 2020 2020 2020 2027  '.             '
-000144c0: 2d2d 6f75 7470 7574 2074 6578 7429 2026  --output text) &
-000144d0: 2620 6563 686f 2022 2473 2220 2626 2065  & echo "$s" && e
-000144e0: 6368 6f3b 205b 5b20 2d7a 2022 2473 2220  cho; [[ -z "$s" 
-000144f0: 5d5d 207c 7c20 5b5b 2022 2473 2220 3d20  ]] || [[ "$s" = 
-00014500: 2274 6572 6d69 6e61 7465 6422 205d 5d20  "terminated" ]] 
-00014510: 7c7c 205b 5b20 2224 7322 203d 2022 7368  || [[ "$s" = "sh
-00014520: 7574 7469 6e67 2d64 6f77 6e22 205d 5d27  utting-down" ]]'
-00014530: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
-00014540: 2020 2020 2020 2020 2020 2020 2320 5465              # Te
-00014550: 7374 2063 616e 6365 6c6c 6174 696f 6e20  st cancellation 
-00014560: 6475 7269 6e67 2073 706f 7420 6a6f 6220  during spot job 
-00014570: 6973 2072 6563 6f76 6572 696e 672e 0a20  is recovering.. 
-00014580: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-00014590: 2073 706f 7420 6c61 756e 6368 202d 2d63   spot launch --c
-000145a0: 6c6f 7564 2061 7773 202d 2d72 6567 696f  loud aws --regio
-000145b0: 6e20 7b72 6567 696f 6e7d 202d 6e20 7b6e  n {region} -n {n
-000145c0: 616d 657d 2d33 2022 736c 6565 7020 3130  ame}-3 "sleep 10
-000145d0: 3030 2220 202d 7920 2d64 272c 0a20 2020  00"  -y -d',.   
-000145e0: 2020 2020 2020 2020 2027 736c 6565 7020           'sleep 
-000145f0: 3330 3027 2c0a 2020 2020 2020 2020 2020  300',.          
-00014600: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
-00014610: 5f57 4149 547d 7c20 6772 6570 207b 6e61  _WAIT}| grep {na
-00014620: 6d65 7d2d 3320 7c20 6865 6164 202d 6e31  me}-3 | head -n1
-00014630: 207c 2067 7265 7020 2252 554e 4e49 4e47   | grep "RUNNING
-00014640: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-00014650: 2320 5465 726d 696e 6174 6520 7468 6520  # Terminate the 
-00014660: 636c 7573 7465 7220 6d61 6e75 616c 6c79  cluster manually
-00014670: 2e0a 2020 2020 2020 2020 2020 2020 2866  ..            (f
-00014680: 2761 7773 2065 6332 2074 6572 6d69 6e61  'aws ec2 termina
-00014690: 7465 2d69 6e73 7461 6e63 6573 202d 2d72  te-instances --r
-000146a0: 6567 696f 6e20 7b72 6567 696f 6e7d 202d  egion {region} -
-000146b0: 2d69 6e73 7461 6e63 652d 6964 7320 2428  -instance-ids $(
-000146c0: 270a 2020 2020 2020 2020 2020 2020 2066  '.             f
-000146d0: 2761 7773 2065 6332 2064 6573 6372 6962  'aws ec2 describ
-000146e0: 652d 696e 7374 616e 6365 7320 2d2d 7265  e-instances --re
-000146f0: 6769 6f6e 207b 7265 6769 6f6e 7d20 270a  gion {region} '.
-00014700: 2020 2020 2020 2020 2020 2020 2066 272d               f'-
-00014710: 2d66 696c 7465 7273 204e 616d 653d 7461  -filters Name=ta
-00014720: 673a 7261 792d 636c 7573 7465 722d 6e61  g:ray-cluster-na
-00014730: 6d65 2c56 616c 7565 733d 7b6e 616d 657d  me,Values={name}
-00014740: 2d33 2d2a 2027 0a20 2020 2020 2020 2020  -3-* '.         
-00014750: 2020 2020 6627 2d2d 7175 6572 7920 5265      f'--query Re
-00014760: 7365 7276 6174 696f 6e73 5b5d 2e49 6e73  servations[].Ins
-00014770: 7461 6e63 6573 5b5d 2e49 6e73 7461 6e63  tances[].Instanc
-00014780: 6549 6420 270a 2020 2020 2020 2020 2020  eId '.          
-00014790: 2020 2027 2d2d 6f75 7470 7574 2074 6578     '--output tex
-000147a0: 7429 2729 2c0a 2020 2020 2020 2020 2020  t)'),.          
-000147b0: 2020 2773 6c65 6570 2031 3230 272c 0a20    'sleep 120',. 
-000147c0: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
-000147d0: 504f 545f 5155 4555 455f 5741 4954 7d7c  POT_QUEUE_WAIT}|
-000147e0: 2067 7265 7020 7b6e 616d 657d 2d33 207c   grep {name}-3 |
-000147f0: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
-00014800: 2022 5245 434f 5645 5249 4e47 2227 2c0a   "RECOVERING"',.
-00014810: 2020 2020 2020 2020 2020 2020 5f53 504f              _SPO
-00014820: 545f 4341 4e43 454c 5f57 4149 542e 666f  T_CANCEL_WAIT.fo
-00014830: 726d 6174 286a 6f62 5f6e 616d 653d 6627  rmat(job_name=f'
-00014840: 7b6e 616d 657d 2d33 2729 2c0a 2020 2020  {name}-3'),.    
-00014850: 2020 2020 2020 2020 2773 6c65 6570 2035          'sleep 5
-00014860: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-00014870: 277b 5f53 504f 545f 5155 4555 455f 5741  '{_SPOT_QUEUE_WA
-00014880: 4954 7d7c 2067 7265 7020 7b6e 616d 657d  IT}| grep {name}
-00014890: 2d33 207c 2068 6561 6420 2d6e 3120 7c20  -3 | head -n1 | 
-000148a0: 6772 6570 2022 4341 4e43 454c 4c49 4e47  grep "CANCELLING
-000148b0: 5c7c 4341 4e43 454c 4c45 4422 272c 0a20  \|CANCELLED"',. 
-000148c0: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
-000148d0: 7020 3132 3027 2c0a 2020 2020 2020 2020  p 120',.        
-000148e0: 2020 2020 6627 7b5f 5350 4f54 5f51 5545      f'{_SPOT_QUE
-000148f0: 5545 5f57 4149 547d 7c20 6772 6570 207b  UE_WAIT}| grep {
-00014900: 6e61 6d65 7d2d 3320 7c20 6865 6164 202d  name}-3 | head -
-00014910: 6e31 207c 2067 7265 7020 2243 414e 4345  n1 | grep "CANCE
-00014920: 4c4c 4544 2227 2c0a 2020 2020 2020 2020  LLED"',.        
-00014930: 2020 2020 2320 5468 6520 636c 7573 7465      # The cluste
-00014940: 7220 7368 6f75 6c64 2062 6520 7465 726d  r should be term
-00014950: 696e 6174 6564 2028 7368 7574 7469 6e67  inated (shutting
-00014960: 2d64 6f77 6e29 2061 6674 6572 2063 616e  -down) after can
-00014970: 6365 6c6c 6174 696f 6e2e 2057 6520 646f  cellation. We do
-00014980: 6e27 7420 7573 6520 7468 6520 603d 6020  n't use the `=` 
-00014990: 6f70 6572 6174 6f72 2068 6572 6520 6265  operator here be
-000149a0: 6361 7573 650a 2020 2020 2020 2020 2020  cause.          
-000149b0: 2020 2320 7468 6572 6520 6361 6e20 6265    # there can be
-000149c0: 206d 756c 7469 706c 6520 564d 2077 6974   multiple VM wit
-000149d0: 6820 7468 6520 7361 6d65 206e 616d 6520  h the same name 
-000149e0: 6475 6520 746f 2074 6865 2072 6563 6f76  due to the recov
-000149f0: 6572 792e 0a20 2020 2020 2020 2020 2020  ery..           
-00014a00: 2028 6627 733d 2428 6177 7320 6563 3220   (f's=$(aws ec2 
-00014a10: 6465 7363 7269 6265 2d69 6e73 7461 6e63  describe-instanc
-00014a20: 6573 202d 2d72 6567 696f 6e20 7b72 6567  es --region {reg
-00014a30: 696f 6e7d 2027 0a20 2020 2020 2020 2020  ion} '.         
-00014a40: 2020 2020 6627 2d2d 6669 6c74 6572 7320      f'--filters 
-00014a50: 4e61 6d65 3d74 6167 3a72 6179 2d63 6c75  Name=tag:ray-clu
-00014a60: 7374 6572 2d6e 616d 652c 5661 6c75 6573  ster-name,Values
-00014a70: 3d7b 6e61 6d65 7d2d 332d 2a20 270a 2020  ={name}-3-* '.  
-00014a80: 2020 2020 2020 2020 2020 2066 272d 2d71             f'--q
-00014a90: 7565 7279 2052 6573 6572 7661 7469 6f6e  uery Reservation
-00014aa0: 735b 5d2e 496e 7374 616e 6365 735b 5d2e  s[].Instances[].
-00014ab0: 5374 6174 655b 5d2e 4e61 6d65 2027 0a20  State[].Name '. 
-00014ac0: 2020 2020 2020 2020 2020 2020 272d 2d6f              '--o
-00014ad0: 7574 7075 7420 7465 7874 2920 2626 2065  utput text) && e
-00014ae0: 6368 6f20 2224 7322 2026 2620 6563 686f  cho "$s" && echo
-00014af0: 3b20 5b5b 202d 7a20 2224 7322 205d 5d20  ; [[ -z "$s" ]] 
-00014b00: 7c7c 2065 6368 6f20 2224 7322 207c 2067  || echo "$s" | g
-00014b10: 7265 7020 2d76 202d 4520 2270 656e 6469  rep -v -E "pendi
-00014b20: 6e67 7c72 756e 6e69 6e67 7c73 746f 7070  ng|running|stopp
-00014b30: 6564 7c73 746f 7070 696e 6722 270a 2020  ed|stopping"'.  
-00014b40: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-00014b50: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00014b60: 7469 6d65 6f75 743d 3235 202a 2036 3029  timeout=25 * 60)
-00014b70: 0a20 2020 2072 756e 5f6f 6e65 5f74 6573  .    run_one_tes
-00014b80: 7428 7465 7374 290a 0a0a 4070 7974 6573  t(test)...@pytes
-00014b90: 742e 6d61 726b 2e67 6370 0a40 7079 7465  t.mark.gcp.@pyte
-00014ba0: 7374 2e6d 6172 6b2e 6d61 6e61 6765 645f  st.mark.managed_
-00014bb0: 7370 6f74 0a64 6566 2074 6573 745f 7370  spot.def test_sp
-00014bc0: 6f74 5f63 616e 6365 6c6c 6174 696f 6e5f  ot_cancellation_
-00014bd0: 6763 7028 293a 0a20 2020 206e 616d 6520  gcp():.    name 
-00014be0: 3d20 5f67 6574 5f63 6c75 7374 6572 5f6e  = _get_cluster_n
-00014bf0: 616d 6528 290a 2020 2020 7a6f 6e65 203d  ame().    zone =
-00014c00: 2027 7573 2d77 6573 7433 2d62 270a 2020   'us-west3-b'.  
-00014c10: 2020 7175 6572 795f 7374 6174 655f 636d    query_state_cm
-00014c20: 6420 3d20 2827 6763 6c6f 7564 2063 6f6d  d = ('gcloud com
-00014c30: 7075 7465 2069 6e73 7461 6e63 6573 206c  pute instances l
-00014c40: 6973 7420 270a 2020 2020 2020 2020 2020  ist '.          
-00014c50: 2020 2020 2020 2020 2020 2020 2066 272d               f'-
-00014c60: 2d66 696c 7465 723d 2228 6c61 6265 6c73  -filter="(labels
-00014c70: 2e72 6179 2d63 6c75 7374 6572 2d6e 616d  .ray-cluster-nam
-00014c80: 653a 7b6e 616d 657d 2922 2027 0a20 2020  e:{name})" '.   
-00014c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ca0: 2020 2020 272d 2d66 6f72 6d61 743d 2276      '--format="v
-00014cb0: 616c 7565 2873 7461 7475 7329 2227 290a  alue(status)"').
-00014cc0: 2020 2020 7175 6572 795f 636d 6420 3d20      query_cmd = 
-00014cd0: 2866 2767 636c 6f75 6420 636f 6d70 7574  (f'gcloud comput
-00014ce0: 6520 696e 7374 616e 6365 7320 6c69 7374  e instances list
-00014cf0: 202d 2d66 696c 7465 723d 270a 2020 2020   --filter='.    
-00014d00: 2020 2020 2020 2020 2020 2020 2066 2722               f'"
-00014d10: 286c 6162 656c 732e 7261 792d 636c 7573  (labels.ray-clus
-00014d20: 7465 722d 6e61 6d65 3a7b 6e61 6d65 7d29  ter-name:{name})
-00014d30: 2220 270a 2020 2020 2020 2020 2020 2020  " '.            
-00014d40: 2020 2020 2066 272d 2d7a 6f6e 6573 3d7b       f'--zones={
-00014d50: 7a6f 6e65 7d20 2d2d 666f 726d 6174 3d22  zone} --format="
-00014d60: 7661 6c75 6528 6e61 6d65 2922 2729 0a20  value(name)"'). 
-00014d70: 2020 2074 6572 6d69 6e61 7465 5f63 6d64     terminate_cmd
-00014d80: 203d 2028 6627 6763 6c6f 7564 2063 6f6d   = (f'gcloud com
-00014d90: 7075 7465 2069 6e73 7461 6e63 6573 2064  pute instances d
-00014da0: 656c 6574 6520 2d2d 7a6f 6e65 3d7b 7a6f  elete --zone={zo
-00014db0: 6e65 7d27 0a20 2020 2020 2020 2020 2020  ne}'.           
-00014dc0: 2020 2020 2020 2020 2020 6627 202d 2d71            f' --q
-00014dd0: 7569 6574 2024 287b 7175 6572 795f 636d  uiet $({query_cm
-00014de0: 647d 2927 290a 2020 2020 7465 7374 203d  d})').    test =
-00014df0: 2054 6573 7428 0a20 2020 2020 2020 2027   Test(.        '
-00014e00: 7370 6f74 5f63 616e 6365 6c6c 6174 696f  spot_cancellatio
-00014e10: 6e5f 6763 7027 2c0a 2020 2020 2020 2020  n_gcp',.        
-00014e20: 5b0a 2020 2020 2020 2020 2020 2020 2320  [.            # 
-00014e30: 5465 7374 2063 616e 6365 6c6c 6174 696f  Test cancellatio
-00014e40: 6e20 6475 7269 6e67 2073 706f 7420 636c  n during spot cl
-00014e50: 7573 7465 7220 6265 696e 6720 6c61 756e  uster being laun
-00014e60: 6368 6564 2e0a 2020 2020 2020 2020 2020  ched..          
-00014e70: 2020 6627 736b 7920 7370 6f74 206c 6175    f'sky spot lau
-00014e80: 6e63 6820 2d2d 636c 6f75 6420 6763 7020  nch --cloud gcp 
-00014e90: 2d2d 7a6f 6e65 207b 7a6f 6e65 7d20 2d6e  --zone {zone} -n
-00014ea0: 207b 6e61 6d65 7d20 2273 6c65 6570 2031   {name} "sleep 1
-00014eb0: 3030 3022 2020 2d79 202d 6427 2c0a 2020  000"  -y -d',.  
-00014ec0: 2020 2020 2020 2020 2020 2773 6c65 6570            'sleep
-00014ed0: 2036 3027 2c0a 2020 2020 2020 2020 2020   60',.          
-00014ee0: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
-00014ef0: 5f57 4149 547d 7c20 6772 6570 207b 6e61  _WAIT}| grep {na
-00014f00: 6d65 7d20 7c20 6865 6164 202d 6e31 207c  me} | head -n1 |
-00014f10: 2067 7265 7020 2253 5441 5254 494e 4722   grep "STARTING"
-00014f20: 272c 0a20 2020 2020 2020 2020 2020 205f  ',.            _
-00014f30: 5350 4f54 5f43 414e 4345 4c5f 5741 4954  SPOT_CANCEL_WAIT
-00014f40: 2e66 6f72 6d61 7428 6a6f 625f 6e61 6d65  .format(job_name
-00014f50: 3d6e 616d 6529 2c0a 2020 2020 2020 2020  =name),.        
-00014f60: 2020 2020 2773 6c65 6570 2035 272c 0a20      'sleep 5',. 
-00014f70: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
-00014f80: 504f 545f 5155 4555 455f 5741 4954 7d7c  POT_QUEUE_WAIT}|
-00014f90: 2067 7265 7020 7b6e 616d 657d 207c 2068   grep {name} | h
-00014fa0: 6561 6420 2d6e 3120 7c20 6772 6570 2022  ead -n1 | grep "
-00014fb0: 4341 4e43 454c 4c49 4e47 5c7c 4341 4e43  CANCELLING\|CANC
-00014fc0: 454c 4c45 4422 272c 0a20 2020 2020 2020  ELLED"',.       
-00014fd0: 2020 2020 2027 736c 6565 7020 3132 3027       'sleep 120'
-00014fe0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-00014ff0: 7b5f 5350 4f54 5f51 5545 5545 5f57 4149  {_SPOT_QUEUE_WAI
-00015000: 547d 7c20 6772 6570 207b 6e61 6d65 7d20  T}| grep {name} 
-00015010: 7c20 6865 6164 202d 6e31 207c 2067 7265  | head -n1 | gre
-00015020: 7020 2243 414e 4345 4c4c 4544 2227 2c0a  p "CANCELLED"',.
-00015030: 2020 2020 2020 2020 2020 2020 2320 5465              # Te
-00015040: 7374 2063 616e 6365 6c6c 696e 6720 7468  st cancelling th
-00015050: 6520 7370 6f74 2063 6c75 7374 6572 2064  e spot cluster d
-00015060: 7572 696e 6720 7370 6f74 206a 6f62 2062  uring spot job b
-00015070: 6569 6e67 2073 6574 7570 2e0a 2020 2020  eing setup..    
-00015080: 2020 2020 2020 2020 6627 736b 7920 7370          f'sky sp
-00015090: 6f74 206c 6175 6e63 6820 2d2d 636c 6f75  ot launch --clou
-000150a0: 6420 6763 7020 2d2d 7a6f 6e65 207b 7a6f  d gcp --zone {zo
-000150b0: 6e65 7d20 2d6e 207b 6e61 6d65 7d2d 3220  ne} -n {name}-2 
-000150c0: 7465 7374 732f 7465 7374 5f79 616d 6c73  tests/test_yamls
-000150d0: 2f74 6573 745f 6c6f 6e67 5f73 6574 7570  /test_long_setup
-000150e0: 2e79 616d 6c20 202d 7920 2d64 272c 0a20  .yaml  -y -d',. 
-000150f0: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
-00015100: 7020 3330 3027 2c0a 2020 2020 2020 2020  p 300',.        
-00015110: 2020 2020 5f53 504f 545f 4341 4e43 454c      _SPOT_CANCEL
-00015120: 5f57 4149 542e 666f 726d 6174 286a 6f62  _WAIT.format(job
-00015130: 5f6e 616d 653d 6627 7b6e 616d 657d 2d32  _name=f'{name}-2
-00015140: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00015150: 2773 6c65 6570 2035 272c 0a20 2020 2020  'sleep 5',.     
-00015160: 2020 2020 2020 2066 277b 5f53 504f 545f         f'{_SPOT_
-00015170: 5155 4555 455f 5741 4954 7d7c 2067 7265  QUEUE_WAIT}| gre
-00015180: 7020 7b6e 616d 657d 2d32 207c 2068 6561  p {name}-2 | hea
-00015190: 6420 2d6e 3120 7c20 6772 6570 2022 4341  d -n1 | grep "CA
-000151a0: 4e43 454c 4c49 4e47 5c7c 4341 4e43 454c  NCELLING\|CANCEL
-000151b0: 4c45 4422 272c 0a20 2020 2020 2020 2020  LED"',.         
-000151c0: 2020 2027 736c 6565 7020 3132 3027 2c0a     'sleep 120',.
-000151d0: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
-000151e0: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
-000151f0: 7c20 6772 6570 207b 6e61 6d65 7d2d 3220  | grep {name}-2 
-00015200: 7c20 6865 6164 202d 6e31 207c 2067 7265  | head -n1 | gre
-00015210: 7020 2243 414e 4345 4c4c 4544 2227 2c0a  p "CANCELLED"',.
-00015220: 2020 2020 2020 2020 2020 2020 2320 5465              # Te
-00015230: 7374 2063 616e 6365 6c6c 6174 696f 6e20  st cancellation 
-00015240: 6475 7269 6e67 2073 706f 7420 6a6f 6220  during spot job 
-00015250: 6973 2072 6563 6f76 6572 696e 672e 0a20  is recovering.. 
-00015260: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-00015270: 2073 706f 7420 6c61 756e 6368 202d 2d63   spot launch --c
-00015280: 6c6f 7564 2067 6370 202d 2d7a 6f6e 6520  loud gcp --zone 
-00015290: 7b7a 6f6e 657d 202d 6e20 7b6e 616d 657d  {zone} -n {name}
-000152a0: 2d33 2022 736c 6565 7020 3130 3030 2220  -3 "sleep 1000" 
-000152b0: 202d 7920 2d64 272c 0a20 2020 2020 2020   -y -d',.       
-000152c0: 2020 2020 2027 736c 6565 7020 3330 3027       'sleep 300'
-000152d0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-000152e0: 7b5f 5350 4f54 5f51 5545 5545 5f57 4149  {_SPOT_QUEUE_WAI
-000152f0: 547d 7c20 6772 6570 207b 6e61 6d65 7d2d  T}| grep {name}-
-00015300: 3320 7c20 6865 6164 202d 6e31 207c 2067  3 | head -n1 | g
-00015310: 7265 7020 2252 554e 4e49 4e47 2227 2c0a  rep "RUNNING"',.
-00015320: 2020 2020 2020 2020 2020 2020 2320 5465              # Te
-00015330: 726d 696e 6174 6520 7468 6520 636c 7573  rminate the clus
-00015340: 7465 7220 6d61 6e75 616c 6c79 2e0a 2020  ter manually..  
-00015350: 2020 2020 2020 2020 2020 7465 726d 696e            termin
-00015360: 6174 655f 636d 642c 0a20 2020 2020 2020  ate_cmd,.       
-00015370: 2020 2020 2027 736c 6565 7020 3130 3027       'sleep 100'
-00015380: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-00015390: 7b5f 5350 4f54 5f51 5545 5545 5f57 4149  {_SPOT_QUEUE_WAI
-000153a0: 547d 7c20 6772 6570 207b 6e61 6d65 7d2d  T}| grep {name}-
-000153b0: 3320 7c20 6865 6164 202d 6e31 207c 2067  3 | head -n1 | g
-000153c0: 7265 7020 2252 4543 4f56 4552 494e 4722  rep "RECOVERING"
-000153d0: 272c 0a20 2020 2020 2020 2020 2020 205f  ',.            _
-000153e0: 5350 4f54 5f43 414e 4345 4c5f 5741 4954  SPOT_CANCEL_WAIT
-000153f0: 2e66 6f72 6d61 7428 6a6f 625f 6e61 6d65  .format(job_name
-00015400: 3d66 277b 6e61 6d65 7d2d 3327 292c 0a20  =f'{name}-3'),. 
-00015410: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
-00015420: 7020 3527 2c0a 2020 2020 2020 2020 2020  p 5',.          
-00015430: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
-00015440: 5f57 4149 547d 7c20 6772 6570 207b 6e61  _WAIT}| grep {na
-00015450: 6d65 7d2d 3320 7c20 6865 6164 202d 6e31  me}-3 | head -n1
-00015460: 207c 2067 7265 7020 2243 414e 4345 4c4c   | grep "CANCELL
-00015470: 494e 475c 7c43 414e 4345 4c4c 4544 2227  ING\|CANCELLED"'
-00015480: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
-00015490: 6c65 6570 2031 3230 272c 0a20 2020 2020  leep 120',.     
-000154a0: 2020 2020 2020 2066 277b 5f53 504f 545f         f'{_SPOT_
-000154b0: 5155 4555 455f 5741 4954 7d7c 2067 7265  QUEUE_WAIT}| gre
-000154c0: 7020 7b6e 616d 657d 2d33 207c 2068 6561  p {name}-3 | hea
-000154d0: 6420 2d6e 3120 7c20 6772 6570 2022 4341  d -n1 | grep "CA
-000154e0: 4e43 454c 4c45 4422 272c 0a20 2020 2020  NCELLED"',.     
-000154f0: 2020 2020 2020 2023 2054 6865 2063 6c75         # The clu
-00015500: 7374 6572 2073 686f 756c 6420 6265 2074  ster should be t
-00015510: 6572 6d69 6e61 7465 6420 2853 544f 5050  erminated (STOPP
-00015520: 494e 4729 2061 6674 6572 2063 616e 6365  ING) after cance
-00015530: 6c6c 6174 696f 6e2e 2057 6520 646f 6e27  llation. We don'
-00015540: 7420 7573 6520 7468 6520 603d 6020 6f70  t use the `=` op
-00015550: 6572 6174 6f72 2068 6572 6520 6265 6361  erator here beca
-00015560: 7573 650a 2020 2020 2020 2020 2020 2020  use.            
-00015570: 2320 7468 6572 6520 6361 6e20 6265 206d  # there can be m
-00015580: 756c 7469 706c 6520 564d 2077 6974 6820  ultiple VM with 
-00015590: 7468 6520 7361 6d65 206e 616d 6520 6475  the same name du
-000155a0: 6520 746f 2074 6865 2072 6563 6f76 6572  e to the recover
-000155b0: 792e 0a20 2020 2020 2020 2020 2020 2028  y..            (
-000155c0: 6627 733d 2428 7b71 7565 7279 5f73 7461  f's=$({query_sta
-000155d0: 7465 5f63 6d64 7d29 2026 2620 6563 686f  te_cmd}) && echo
-000155e0: 2022 2473 2220 2626 2065 6368 6f3b 205b   "$s" && echo; [
-000155f0: 5b20 2d7a 2022 2473 2220 5d5d 207c 7c20  [ -z "$s" ]] || 
-00015600: 6563 686f 2022 2473 2220 7c20 6772 6570  echo "$s" | grep
-00015610: 202d 7620 2d45 2022 5052 4f56 4953 494f   -v -E "PROVISIO
-00015620: 4e49 4e47 7c53 5441 4749 4e47 7c52 554e  NING|STAGING|RUN
-00015630: 4e49 4e47 7c52 4550 4149 5249 4e47 7c54  NING|REPAIRING|T
-00015640: 4552 4d49 4e41 5445 447c 5355 5350 454e  ERMINATED|SUSPEN
-00015650: 4449 4e47 7c53 5553 5045 4e44 4544 7c53  DING|SUSPENDED|S
-00015660: 5553 5045 4e44 4544 2227 0a20 2020 2020  USPENDED"'.     
-00015670: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-00015680: 2020 5d2c 0a20 2020 2020 2020 2074 696d    ],.        tim
-00015690: 656f 7574 3d32 3520 2a20 3630 290a 2020  eout=25 * 60).  
-000156a0: 2020 7275 6e5f 6f6e 655f 7465 7374 2874    run_one_test(t
-000156b0: 6573 7429 0a0a 0a23 202d 2d2d 2d2d 2d2d  est)...# -------
-000156c0: 2d2d 2d20 5465 7374 696e 6720 7374 6f72  --- Testing stor
-000156d0: 6167 6520 666f 7220 6d61 6e61 6765 6420  age for managed 
-000156e0: 7370 6f74 202d 2d2d 2d2d 2d2d 2d2d 2d0a  spot ----------.
-000156f0: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
-00015700: 6c61 6d62 6461 5f63 6c6f 7564 2020 2320  lambda_cloud  # 
-00015710: 4c61 6d62 6461 2043 6c6f 7564 2064 6f65  Lambda Cloud doe
-00015720: 7320 6e6f 7420 7375 7070 6f72 7420 7370  s not support sp
-00015730: 6f74 2069 6e73 7461 6e63 6573 0a40 7079  ot instances.@py
-00015740: 7465 7374 2e6d 6172 6b2e 6e6f 5f69 626d  test.mark.no_ibm
-00015750: 2020 2320 4942 4d20 436c 6f75 6420 646f    # IBM Cloud do
-00015760: 6573 206e 6f74 2073 7570 706f 7274 2073  es not support s
-00015770: 706f 7420 696e 7374 616e 6365 730a 4070  pot instances.@p
-00015780: 7974 6573 742e 6d61 726b 2e6e 6f5f 7363  ytest.mark.no_sc
-00015790: 7020 2023 2053 4350 2064 6f65 7320 6e6f  p  # SCP does no
-000157a0: 7420 7375 7070 6f72 7420 7370 6f74 2069  t support spot i
-000157b0: 6e73 7461 6e63 6573 0a40 7079 7465 7374  nstances.@pytest
-000157c0: 2e6d 6172 6b2e 6d61 6e61 6765 645f 7370  .mark.managed_sp
-000157d0: 6f74 0a64 6566 2074 6573 745f 7370 6f74  ot.def test_spot
-000157e0: 5f73 746f 7261 6765 2867 656e 6572 6963  _storage(generic
-000157f0: 5f63 6c6f 7564 3a20 7374 7229 3a0a 2020  _cloud: str):.  
-00015800: 2020 2222 2254 6573 7420 7374 6f72 6167    """Test storag
-00015810: 6520 7769 7468 206d 616e 6167 6564 2073  e with managed s
-00015820: 706f 7422 2222 0a20 2020 206e 616d 6520  pot""".    name 
-00015830: 3d20 5f67 6574 5f63 6c75 7374 6572 5f6e  = _get_cluster_n
-00015840: 616d 6528 290a 2020 2020 7961 6d6c 5f73  ame().    yaml_s
-00015850: 7472 203d 2070 6174 686c 6962 2e50 6174  tr = pathlib.Pat
-00015860: 6828 0a20 2020 2020 2020 2027 6578 616d  h(.        'exam
-00015870: 706c 6573 2f6d 616e 6167 6564 5f73 706f  ples/managed_spo
-00015880: 745f 7769 7468 5f73 746f 7261 6765 2e79  t_with_storage.y
-00015890: 616d 6c27 292e 7265 6164 5f74 6578 7428  aml').read_text(
-000158a0: 290a 2020 2020 7374 6f72 6167 655f 6e61  ).    storage_na
-000158b0: 6d65 203d 2066 2773 6b79 2d74 6573 742d  me = f'sky-test-
-000158c0: 7b69 6e74 2874 696d 652e 7469 6d65 2829  {int(time.time()
-000158d0: 297d 270a 2020 2020 7961 6d6c 5f73 7472  )}'.    yaml_str
-000158e0: 203d 2079 616d 6c5f 7374 722e 7265 706c   = yaml_str.repl
-000158f0: 6163 6528 2773 6b79 2d77 6f72 6b64 6972  ace('sky-workdir
-00015900: 2d7a 6877 7527 2c20 7374 6f72 6167 655f  -zhwu', storage_
-00015910: 6e61 6d65 290a 2020 2020 7769 7468 2074  name).    with t
-00015920: 656d 7066 696c 652e 4e61 6d65 6454 656d  empfile.NamedTem
-00015930: 706f 7261 7279 4669 6c65 2873 7566 6669  poraryFile(suffi
-00015940: 783d 272e 7961 6d6c 272c 206d 6f64 653d  x='.yaml', mode=
-00015950: 2777 2729 2061 7320 663a 0a20 2020 2020  'w') as f:.     
-00015960: 2020 2066 2e77 7269 7465 2879 616d 6c5f     f.write(yaml_
-00015970: 7374 7229 0a20 2020 2020 2020 2066 2e66  str).        f.f
-00015980: 6c75 7368 2829 0a20 2020 2020 2020 2066  lush().        f
-00015990: 696c 655f 7061 7468 203d 2066 2e6e 616d  ile_path = f.nam
-000159a0: 650a 2020 2020 2020 2020 7465 7374 203d  e.        test =
-000159b0: 2054 6573 7428 0a20 2020 2020 2020 2020   Test(.         
-000159c0: 2020 2027 7370 6f74 5f73 746f 7261 6765     'spot_storage
-000159d0: 272c 0a20 2020 2020 2020 2020 2020 205b  ',.            [
-000159e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000159f0: 202a 7374 6f72 6167 655f 7365 7475 705f   *storage_setup_
-00015a00: 636f 6d6d 616e 6473 2c0a 2020 2020 2020  commands,.      
-00015a10: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
-00015a20: 7370 6f74 206c 6175 6e63 6820 2d6e 207b  spot launch -n {
-00015a30: 6e61 6d65 7d20 2d2d 636c 6f75 6420 7b67  name} --cloud {g
-00015a40: 656e 6572 6963 5f63 6c6f 7564 7d20 7b66  eneric_cloud} {f
-00015a50: 696c 655f 7061 7468 7d20 2d79 272c 0a20  ile_path} -y',. 
-00015a60: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00015a70: 736c 6565 7020 3630 272c 2020 2320 5761  sleep 60',  # Wa
-00015a80: 6974 2074 6865 2073 706f 7420 7175 6575  it the spot queu
-00015a90: 6520 746f 2062 6520 7570 6461 7465 640a  e to be updated.
-00015aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ab0: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
-00015ac0: 4149 547d 7c20 6772 6570 207b 6e61 6d65  AIT}| grep {name
-00015ad0: 7d20 7c20 6772 6570 2053 5543 4345 4544  } | grep SUCCEED
-00015ae0: 4544 272c 0a20 2020 2020 2020 2020 2020  ED',.           
-00015af0: 2020 2020 2066 275b 2024 2861 7773 2073       f'[ $(aws s
-00015b00: 3361 7069 206c 6973 742d 6275 636b 6574  3api list-bucket
-00015b10: 7320 2d2d 7175 6572 7920 2242 7563 6b65  s --query "Bucke
-00015b20: 7473 5b3f 636f 6e74 6169 6e73 284e 616d  ts[?contains(Nam
-00015b30: 652c 205c 277b 7374 6f72 6167 655f 6e61  e, \'{storage_na
-00015b40: 6d65 7d5c 2729 5d2e 4e61 6d65 2220 2d2d  me}\')].Name" --
-00015b50: 6f75 7470 7574 2074 6578 7420 7c20 7763  output text | wc
-00015b60: 202d 6c29 202d 6571 2030 205d 270a 2020   -l) -eq 0 ]'.  
-00015b70: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
-00015b80: 2020 2020 2020 2020 205f 5350 4f54 5f43           _SPOT_C
-00015b90: 414e 4345 4c5f 5741 4954 2e66 6f72 6d61  ANCEL_WAIT.forma
-00015ba0: 7428 6a6f 625f 6e61 6d65 3d6e 616d 6529  t(job_name=name)
-00015bb0: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
-00015bc0: 496e 6372 6561 7365 2074 696d 656f 7574  Increase timeout
-00015bd0: 2073 696e 6365 2073 6b79 2073 706f 7420   since sky spot 
-00015be0: 7175 6575 6520 2d72 2063 616e 2062 6520  queue -r can be 
-00015bf0: 626c 6f63 6b65 6420 6279 206f 7468 6572  blocked by other
-00015c00: 2073 706f 7420 7465 7374 732e 0a20 2020   spot tests..   
-00015c10: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
-00015c20: 3d32 3020 2a20 3630 2c0a 2020 2020 2020  =20 * 60,.      
-00015c30: 2020 290a 2020 2020 2020 2020 7275 6e5f    ).        run_
-00015c40: 6f6e 655f 7465 7374 2874 6573 7429 0a0a  one_test(test)..
-00015c50: 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d20 5465  .# ---------- Te
-00015c60: 7374 696e 6720 7370 6f74 2054 5055 202d  sting spot TPU -
-00015c70: 2d2d 2d2d 2d2d 2d2d 2d0a 4070 7974 6573  ---------.@pytes
-00015c80: 742e 6d61 726b 2e67 6370 0a40 7079 7465  t.mark.gcp.@pyte
-00015c90: 7374 2e6d 6172 6b2e 6d61 6e61 6765 645f  st.mark.managed_
-00015ca0: 7370 6f74 0a64 6566 2074 6573 745f 7370  spot.def test_sp
-00015cb0: 6f74 5f74 7075 2829 3a0a 2020 2020 2222  ot_tpu():.    ""
-00015cc0: 2254 6573 7420 6d61 6e61 6765 6420 7370  "Test managed sp
-00015cd0: 6f74 206f 6e20 5450 552e 2222 220a 2020  ot on TPU.""".  
-00015ce0: 2020 6e61 6d65 203d 205f 6765 745f 636c    name = _get_cl
-00015cf0: 7573 7465 725f 6e61 6d65 2829 0a20 2020  uster_name().   
-00015d00: 2074 6573 7420 3d20 5465 7374 280a 2020   test = Test(.  
-00015d10: 2020 2020 2020 2774 6573 742d 7370 6f74        'test-spot
-00015d20: 2d74 7075 272c 0a20 2020 2020 2020 205b  -tpu',.        [
-00015d30: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-00015d40: 6b79 2073 706f 7420 6c61 756e 6368 202d  ky spot launch -
-00015d50: 6e20 7b6e 616d 657d 2065 7861 6d70 6c65  n {name} example
-00015d60: 732f 7470 752f 7470 7576 6d5f 6d6e 6973  s/tpu/tpuvm_mnis
-00015d70: 742e 7961 6d6c 202d 7920 2d64 272c 0a20  t.yaml -y -d',. 
-00015d80: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
-00015d90: 7020 3527 2c0a 2020 2020 2020 2020 2020  p 5',.          
-00015da0: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
-00015db0: 5f57 4149 547d 7c20 6772 6570 207b 6e61  _WAIT}| grep {na
-00015dc0: 6d65 7d20 7c20 6865 6164 202d 6e31 207c  me} | head -n1 |
-00015dd0: 2067 7265 7020 5354 4152 5449 4e47 272c   grep STARTING',
-00015de0: 0a20 2020 2020 2020 2020 2020 2027 736c  .            'sl
-00015df0: 6565 7020 3630 3027 2c20 2023 2054 5055  eep 600',  # TPU
-00015e00: 2074 616b 6573 2061 2077 6869 6c65 2074   takes a while t
-00015e10: 6f20 6c61 756e 6368 0a20 2020 2020 2020  o launch.       
-00015e20: 2020 2020 2066 277b 5f53 504f 545f 5155       f'{_SPOT_QU
-00015e30: 4555 455f 5741 4954 7d7c 2067 7265 7020  EUE_WAIT}| grep 
-00015e40: 7b6e 616d 657d 207c 2068 6561 6420 2d6e  {name} | head -n
-00015e50: 3120 7c20 6772 6570 2022 5255 4e4e 494e  1 | grep "RUNNIN
-00015e60: 475c 7c53 5543 4345 4544 4544 2227 2c0a  G\|SUCCEEDED"',.
-00015e70: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00015e80: 2020 205f 5350 4f54 5f43 414e 4345 4c5f     _SPOT_CANCEL_
-00015e90: 5741 4954 2e66 6f72 6d61 7428 6a6f 625f  WAIT.format(job_
-00015ea0: 6e61 6d65 3d6e 616d 6529 2c0a 2020 2020  name=name),.    
-00015eb0: 2020 2020 2320 496e 6372 6561 7365 2074      # Increase t
-00015ec0: 696d 656f 7574 2073 696e 6365 2073 6b79  imeout since sky
-00015ed0: 2073 706f 7420 7175 6575 6520 2d72 2063   spot queue -r c
-00015ee0: 616e 2062 6520 626c 6f63 6b65 6420 6279  an be blocked by
-00015ef0: 206f 7468 6572 2073 706f 7420 7465 7374   other spot test
-00015f00: 732e 0a20 2020 2020 2020 2074 696d 656f  s..        timeo
-00015f10: 7574 3d32 3020 2a20 3630 2c0a 2020 2020  ut=20 * 60,.    
-00015f20: 290a 2020 2020 7275 6e5f 6f6e 655f 7465  ).    run_one_te
-00015f30: 7374 2874 6573 7429 0a0a 0a23 202d 2d2d  st(test)...# ---
-00015f40: 2d2d 2d2d 2d2d 2d20 5465 7374 696e 6720  ------- Testing 
-00015f50: 656e 7620 666f 7220 7370 6f74 202d 2d2d  env for spot ---
-00015f60: 2d2d 2d2d 2d2d 2d0a 4070 7974 6573 742e  -------.@pytest.
-00015f70: 6d61 726b 2e6e 6f5f 6c61 6d62 6461 5f63  mark.no_lambda_c
-00015f80: 6c6f 7564 2020 2320 4c61 6d62 6461 2043  loud  # Lambda C
-00015f90: 6c6f 7564 2064 6f65 7320 6e6f 7420 7375  loud does not su
-00015fa0: 7070 6f72 7420 7370 6f74 2069 6e73 7461  pport spot insta
-00015fb0: 6e63 6573 0a40 7079 7465 7374 2e6d 6172  nces.@pytest.mar
-00015fc0: 6b2e 6e6f 5f69 626d 2020 2320 4942 4d20  k.no_ibm  # IBM 
-00015fd0: 436c 6f75 6420 646f 6573 206e 6f74 2073  Cloud does not s
-00015fe0: 7570 706f 7274 2073 706f 7420 696e 7374  upport spot inst
-00015ff0: 616e 6365 730a 4070 7974 6573 742e 6d61  ances.@pytest.ma
-00016000: 726b 2e6e 6f5f 7363 7020 2023 2053 4350  rk.no_scp  # SCP
-00016010: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
-00016020: 7420 7370 6f74 2069 6e73 7461 6e63 6573  t spot instances
-00016030: 0a40 7079 7465 7374 2e6d 6172 6b2e 6d61  .@pytest.mark.ma
-00016040: 6e61 6765 645f 7370 6f74 0a64 6566 2074  naged_spot.def t
-00016050: 6573 745f 7370 6f74 5f69 6e6c 696e 655f  est_spot_inline_
-00016060: 656e 7628 6765 6e65 7269 635f 636c 6f75  env(generic_clou
-00016070: 643a 2073 7472 293a 0a20 2020 2022 2222  d: str):.    """
-00016080: 5465 7374 2073 706f 7420 656e 7622 2222  Test spot env"""
-00016090: 0a20 2020 206e 616d 6520 3d20 5f67 6574  .    name = _get
-000160a0: 5f63 6c75 7374 6572 5f6e 616d 6528 290a  _cluster_name().
-000160b0: 2020 2020 7465 7374 203d 2054 6573 7428      test = Test(
-000160c0: 0a20 2020 2020 2020 2027 7465 7374 2d73  .        'test-s
-000160d0: 706f 742d 696e 6c69 6e65 2d65 6e76 272c  pot-inline-env',
-000160e0: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
-000160f0: 2020 2020 2020 2066 2773 6b79 2073 706f         f'sky spo
-00016100: 7420 6c61 756e 6368 202d 6e20 7b6e 616d  t launch -n {nam
-00016110: 657d 202d 7920 2d2d 636c 6f75 6420 7b67  e} -y --cloud {g
-00016120: 656e 6572 6963 5f63 6c6f 7564 7d20 2d2d  eneric_cloud} --
-00016130: 656e 7620 5445 5354 5f45 4e56 3d22 6865  env TEST_ENV="he
-00016140: 6c6c 6f20 776f 726c 6422 202d 2d20 2228  llo world" -- "(
-00016150: 5b5b 2021 202d 7a20 5c5c 225c 2454 4553  [[ ! -z \\"\$TES
-00016160: 545f 454e 565c 5c22 205d 5d20 2626 205b  T_ENV\\" ]] && [
-00016170: 5b20 2120 2d7a 205c 5c22 5c24 534b 5950  [ ! -z \\"\$SKYP
-00016180: 494c 4f54 5f4e 4f44 455f 4950 535c 5c22  ILOT_NODE_IPS\\"
-00016190: 205d 5d20 2626 205b 5b20 2120 2d7a 205c   ]] && [[ ! -z \
-000161a0: 5c22 5c24 534b 5950 494c 4f54 5f4e 4f44  \"\$SKYPILOT_NOD
-000161b0: 455f 5241 4e4b 5c5c 2220 5d5d 2920 7c7c  E_RANK\\" ]]) ||
-000161c0: 2065 7869 7420 3122 272c 0a20 2020 2020   exit 1"',.     
-000161d0: 2020 2020 2020 2027 736c 6565 7020 3230         'sleep 20
-000161e0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-000161f0: 277b 5f53 504f 545f 5155 4555 455f 5741  '{_SPOT_QUEUE_WA
-00016200: 4954 7d20 7c20 6772 6570 207b 6e61 6d65  IT} | grep {name
-00016210: 7d20 7c20 6772 6570 2053 5543 4345 4544  } | grep SUCCEED
-00016220: 4544 272c 0a20 2020 2020 2020 205d 2c0a  ED',.        ],.
-00016230: 2020 2020 2020 2020 5f53 504f 545f 4341          _SPOT_CA
-00016240: 4e43 454c 5f57 4149 542e 666f 726d 6174  NCEL_WAIT.format
-00016250: 286a 6f62 5f6e 616d 653d 6e61 6d65 292c  (job_name=name),
-00016260: 0a20 2020 2020 2020 2023 2049 6e63 7265  .        # Incre
-00016270: 6173 6520 7469 6d65 6f75 7420 7369 6e63  ase timeout sinc
-00016280: 6520 736b 7920 7370 6f74 2071 7565 7565  e sky spot queue
-00016290: 202d 7220 6361 6e20 6265 2062 6c6f 636b   -r can be block
-000162a0: 6564 2062 7920 6f74 6865 7220 7370 6f74  ed by other spot
-000162b0: 2074 6573 7473 2e0a 2020 2020 2020 2020   tests..        
-000162c0: 7469 6d65 6f75 743d 3230 202a 2036 302c  timeout=20 * 60,
-000162d0: 0a20 2020 2029 0a20 2020 2072 756e 5f6f  .    ).    run_o
-000162e0: 6e65 5f74 6573 7428 7465 7374 290a 0a0a  ne_test(test)...
-000162f0: 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2054 6573  # ---------- Tes
-00016300: 7469 6e67 2065 6e76 202d 2d2d 2d2d 2d2d  ting env -------
-00016310: 2d2d 2d0a 6465 6620 7465 7374 5f69 6e6c  ---.def test_inl
-00016320: 696e 655f 656e 7628 6765 6e65 7269 635f  ine_env(generic_
-00016330: 636c 6f75 643a 2073 7472 293a 0a20 2020  cloud: str):.   
-00016340: 2022 2222 5465 7374 2065 6e76 2222 220a   """Test env""".
-00016350: 2020 2020 6e61 6d65 203d 205f 6765 745f      name = _get_
-00016360: 636c 7573 7465 725f 6e61 6d65 2829 0a20  cluster_name(). 
-00016370: 2020 2074 6573 7420 3d20 5465 7374 280a     test = Test(.
-00016380: 2020 2020 2020 2020 2774 6573 742d 696e          'test-in
-00016390: 6c69 6e65 2d65 6e76 272c 0a20 2020 2020  line-env',.     
-000163a0: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-000163b0: 2066 2773 6b79 206c 6175 6e63 6820 2d63   f'sky launch -c
-000163c0: 207b 6e61 6d65 7d20 2d79 202d 2d63 6c6f   {name} -y --clo
-000163d0: 7564 207b 6765 6e65 7269 635f 636c 6f75  ud {generic_clou
-000163e0: 647d 202d 2d65 6e76 2054 4553 545f 454e  d} --env TEST_EN
-000163f0: 563d 2268 656c 6c6f 2077 6f72 6c64 2220  V="hello world" 
-00016400: 2d2d 2022 285b 5b20 2120 2d7a 205c 5c22  -- "([[ ! -z \\"
-00016410: 5c24 5445 5354 5f45 4e56 5c5c 2220 5d5d  \$TEST_ENV\\" ]]
-00016420: 2026 2620 5b5b 2021 202d 7a20 5c5c 225c   && [[ ! -z \\"\
-00016430: 2453 4b59 5049 4c4f 545f 4e4f 4445 5f49  $SKYPILOT_NODE_I
-00016440: 5053 5c5c 2220 5d5d 2026 2620 5b5b 2021  PS\\" ]] && [[ !
-00016450: 202d 7a20 5c5c 225c 2453 4b59 5049 4c4f   -z \\"\$SKYPILO
-00016460: 545f 4e4f 4445 5f52 414e 4b5c 5c22 205d  T_NODE_RANK\\" ]
-00016470: 5d29 207c 7c20 6578 6974 2031 2227 2c0a  ]) || exit 1"',.
-00016480: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-00016490: 7920 6c6f 6773 207b 6e61 6d65 7d20 3120  y logs {name} 1 
-000164a0: 2d2d 7374 6174 7573 272c 0a20 2020 2020  --status',.     
-000164b0: 2020 2020 2020 2066 2773 6b79 2065 7865         f'sky exe
-000164c0: 6320 7b6e 616d 657d 202d 2d65 6e76 2054  c {name} --env T
-000164d0: 4553 545f 454e 5632 3d22 7375 6363 6573  EST_ENV2="succes
-000164e0: 7322 2022 285b 5b20 2120 2d7a 205c 5c22  s" "([[ ! -z \\"
-000164f0: 5c24 5445 5354 5f45 4e56 325c 5c22 205d  \$TEST_ENV2\\" ]
-00016500: 5d20 2626 205b 5b20 2120 2d7a 205c 5c22  ] && [[ ! -z \\"
-00016510: 5c24 534b 5950 494c 4f54 5f4e 4f44 455f  \$SKYPILOT_NODE_
-00016520: 4950 535c 5c22 205d 5d20 2626 205b 5b20  IPS\\" ]] && [[ 
-00016530: 2120 2d7a 205c 5c22 5c24 534b 5950 494c  ! -z \\"\$SKYPIL
-00016540: 4f54 5f4e 4f44 455f 5241 4e4b 5c5c 2220  OT_NODE_RANK\\" 
-00016550: 5d5d 2920 7c7c 2065 7869 7420 3122 272c  ]]) || exit 1"',
-00016560: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-00016570: 6b79 206c 6f67 7320 7b6e 616d 657d 2032  ky logs {name} 2
-00016580: 202d 2d73 7461 7475 7327 2c0a 2020 2020   --status',.    
-00016590: 2020 2020 5d2c 0a20 2020 2020 2020 2066      ],.        f
-000165a0: 2773 6b79 2064 6f77 6e20 2d79 207b 6e61  'sky down -y {na
-000165b0: 6d65 7d27 2c0a 2020 2020 290a 2020 2020  me}',.    ).    
-000165c0: 7275 6e5f 6f6e 655f 7465 7374 2874 6573  run_one_test(tes
-000165d0: 7429 0a0a 0a23 202d 2d2d 2d2d 2d2d 2d2d  t)...# ---------
-000165e0: 2d20 5465 7374 696e 6720 6375 7374 6f6d  - Testing custom
-000165f0: 2069 6d61 6765 202d 2d2d 2d2d 2d2d 2d2d   image ---------
-00016600: 2d0a 4070 7974 6573 742e 6d61 726b 2e61  -.@pytest.mark.a
-00016610: 7773 0a64 6566 2074 6573 745f 6375 7374  ws.def test_cust
-00016620: 6f6d 5f69 6d61 6765 2829 3a0a 2020 2020  om_image():.    
-00016630: 2222 2254 6573 7420 6375 7374 6f6d 2069  """Test custom i
-00016640: 6d61 6765 2222 220a 2020 2020 6e61 6d65  mage""".    name
-00016650: 203d 205f 6765 745f 636c 7573 7465 725f   = _get_cluster_
-00016660: 6e61 6d65 2829 0a20 2020 2074 6573 7420  name().    test 
-00016670: 3d20 5465 7374 280a 2020 2020 2020 2020  = Test(.        
-00016680: 2774 6573 742d 6375 7374 6f6d 2d69 6d61  'test-custom-ima
-00016690: 6765 272c 0a20 2020 2020 2020 205b 0a20  ge',.        [. 
-000166a0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-000166b0: 206c 6175 6e63 6820 2d63 207b 6e61 6d65   launch -c {name
-000166c0: 7d20 2d2d 7265 7472 792d 756e 7469 6c2d  } --retry-until-
-000166d0: 7570 202d 7920 6578 616d 706c 6573 2f63  up -y examples/c
-000166e0: 7573 746f 6d5f 696d 6167 652e 7961 6d6c  ustom_image.yaml
-000166f0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-00016700: 2773 6b79 206c 6f67 7320 7b6e 616d 657d  'sky logs {name}
-00016710: 2031 202d 2d73 7461 7475 7327 2c0a 2020   1 --status',.  
-00016720: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-00016730: 2066 2773 6b79 2064 6f77 6e20 2d79 207b   f'sky down -y {
-00016740: 6e61 6d65 7d27 2c0a 2020 2020 2020 2020  name}',.        
-00016750: 7469 6d65 6f75 743d 3330 202a 2036 302c  timeout=30 * 60,
-00016760: 0a20 2020 2029 0a20 2020 2072 756e 5f6f  .    ).    run_o
-00016770: 6e65 5f74 6573 7428 7465 7374 290a 0a0a  ne_test(test)...
-00016780: 4070 7974 6573 742e 6d61 726b 2e73 6c6f  @pytest.mark.slo
-00016790: 770a 6465 6620 7465 7374 5f61 7a75 7265  w.def test_azure
-000167a0: 5f73 7461 7274 5f73 746f 705f 7477 6f5f  _start_stop_two_
-000167b0: 6e6f 6465 7328 293a 0a20 2020 206e 616d  nodes():.    nam
-000167c0: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
-000167d0: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
-000167e0: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
-000167f0: 2027 617a 7572 652d 7374 6172 742d 7374   'azure-start-st
-00016800: 6f70 2d74 776f 2d6e 6f64 6573 272c 0a20  op-two-nodes',. 
-00016810: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-00016820: 2020 2020 2066 2773 6b79 206c 6175 6e63       f'sky launc
-00016830: 6820 2d2d 6e75 6d2d 6e6f 6465 733d 3220  h --num-nodes=2 
-00016840: 2d79 202d 6320 7b6e 616d 657d 2065 7861  -y -c {name} exa
-00016850: 6d70 6c65 732f 617a 7572 655f 7374 6172  mples/azure_star
-00016860: 745f 7374 6f70 2e79 616d 6c27 2c0a 2020  t_stop.yaml',.  
-00016870: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
-00016880: 6578 6563 202d 2d6e 756d 2d6e 6f64 6573  exec --num-nodes
-00016890: 3d32 207b 6e61 6d65 7d20 6578 616d 706c  =2 {name} exampl
-000168a0: 6573 2f61 7a75 7265 5f73 7461 7274 5f73  es/azure_start_s
-000168b0: 746f 702e 7961 6d6c 272c 0a20 2020 2020  top.yaml',.     
-000168c0: 2020 2020 2020 2066 2773 6b79 206c 6f67         f'sky log
-000168d0: 7320 7b6e 616d 657d 2031 202d 2d73 7461  s {name} 1 --sta
-000168e0: 7475 7327 2c20 2023 2045 6e73 7572 6520  tus',  # Ensure 
-000168f0: 7468 6520 6a6f 6220 7375 6363 6565 6465  the job succeede
-00016900: 642e 0a20 2020 2020 2020 2020 2020 2066  d..            f
-00016910: 2773 6b79 2073 746f 7020 2d79 207b 6e61  'sky stop -y {na
-00016920: 6d65 7d27 2c0a 2020 2020 2020 2020 2020  me}',.          
-00016930: 2020 6627 736b 7920 7374 6172 7420 2d79    f'sky start -y
-00016940: 207b 6e61 6d65 7d27 2c0a 2020 2020 2020   {name}',.      
-00016950: 2020 2020 2020 6627 736b 7920 6578 6563        f'sky exec
-00016960: 202d 2d6e 756d 2d6e 6f64 6573 3d32 207b   --num-nodes=2 {
-00016970: 6e61 6d65 7d20 6578 616d 706c 6573 2f61  name} examples/a
-00016980: 7a75 7265 5f73 7461 7274 5f73 746f 702e  zure_start_stop.
-00016990: 7961 6d6c 272c 0a20 2020 2020 2020 2020  yaml',.         
-000169a0: 2020 2066 2773 6b79 206c 6f67 7320 7b6e     f'sky logs {n
-000169b0: 616d 657d 2032 202d 2d73 7461 7475 7327  ame} 2 --status'
-000169c0: 2c20 2023 2045 6e73 7572 6520 7468 6520  ,  # Ensure the 
-000169d0: 6a6f 6220 7375 6363 6565 6465 642e 0a20  job succeeded.. 
-000169e0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-000169f0: 2020 6627 736b 7920 646f 776e 202d 7920    f'sky down -y 
-00016a00: 7b6e 616d 657d 272c 0a20 2020 2020 2020  {name}',.       
-00016a10: 2074 696d 656f 7574 3d33 3020 2a20 3630   timeout=30 * 60
-00016a20: 2c20 2023 2033 3020 6d69 6e73 2020 2869  ,  # 30 mins  (i
-00016a30: 7420 7461 6b65 7320 6172 6f75 6e64 207e  t takes around ~
-00016a40: 3233 206d 696e 7329 0a20 2020 2029 0a20  23 mins).    ). 
-00016a50: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
-00016a60: 7465 7374 290a 0a0a 2320 2d2d 2d2d 2d2d  test)...# ------
-00016a70: 2d2d 2d2d 2054 6573 7469 6e67 2065 6e76  ---- Testing env
-00016a80: 2066 6f72 2064 6973 6b20 7469 6572 202d   for disk tier -
-00016a90: 2d2d 2d2d 2d2d 2d2d 2d0a 4070 7974 6573  ---------.@pytes
-00016aa0: 742e 6d61 726b 2e61 7773 0a64 6566 2074  t.mark.aws.def t
-00016ab0: 6573 745f 6177 735f 6469 736b 5f74 6965  est_aws_disk_tie
-00016ac0: 7228 293a 0a0a 2020 2020 6465 6620 5f67  r():..    def _g
-00016ad0: 6574 5f61 7773 5f71 7565 7279 5f63 6f6d  et_aws_query_com
-00016ae0: 6d61 6e64 2872 6567 696f 6e2c 2069 6e73  mand(region, ins
-00016af0: 7461 6e63 655f 6964 2c20 6669 656c 642c  tance_id, field,
-00016b00: 2065 7870 6563 7465 6429 3a0a 2020 2020   expected):.    
-00016b10: 2020 2020 7265 7475 726e 2028 6627 6177      return (f'aw
-00016b20: 7320 6563 3220 6465 7363 7269 6265 2d76  s ec2 describe-v
-00016b30: 6f6c 756d 6573 202d 2d72 6567 696f 6e20  olumes --region 
-00016b40: 7b72 6567 696f 6e7d 2027 0a20 2020 2020  {region} '.     
-00016b50: 2020 2020 2020 2020 2020 2066 272d 2d66             f'--f
-00016b60: 696c 7465 7273 204e 616d 653d 6174 7461  ilters Name=atta
-00016b70: 6368 6d65 6e74 2e69 6e73 7461 6e63 652d  chment.instance-
-00016b80: 6964 2c56 616c 7565 733d 7b69 6e73 7461  id,Values={insta
-00016b90: 6e63 655f 6964 7d20 270a 2020 2020 2020  nce_id} '.      
-00016ba0: 2020 2020 2020 2020 2020 6627 2d2d 7175            f'--qu
-00016bb0: 6572 7920 566f 6c75 6d65 735b 2a5d 2e7b  ery Volumes[*].{
-00016bc0: 6669 656c 647d 207c 2067 7265 7020 7b65  field} | grep {e
-00016bd0: 7870 6563 7465 647d 203b 2027 290a 0a20  xpected} ; ').. 
-00016be0: 2020 2066 6f72 2064 6973 6b5f 7469 6572     for disk_tier
-00016bf0: 2069 6e20 5b27 6c6f 7727 2c20 276d 6564   in ['low', 'med
-00016c00: 6975 6d27 2c20 2768 6967 6827 5d3a 0a20  ium', 'high']:. 
-00016c10: 2020 2020 2020 2073 7065 6373 203d 2041         specs = A
-00016c20: 5753 2e5f 6765 745f 6469 736b 5f73 7065  WS._get_disk_spe
-00016c30: 6373 2864 6973 6b5f 7469 6572 290a 2020  cs(disk_tier).  
-00016c40: 2020 2020 2020 6e61 6d65 203d 205f 6765        name = _ge
-00016c50: 745f 636c 7573 7465 725f 6e61 6d65 2829  t_cluster_name()
-00016c60: 202b 2027 2d27 202b 2064 6973 6b5f 7469   + '-' + disk_ti
-00016c70: 6572 0a20 2020 2020 2020 2072 6567 696f  er.        regio
-00016c80: 6e20 3d20 2775 732d 7765 7374 2d32 270a  n = 'us-west-2'.
-00016c90: 2020 2020 2020 2020 7465 7374 203d 2054          test = T
-00016ca0: 6573 7428 0a20 2020 2020 2020 2020 2020  est(.           
-00016cb0: 2027 6177 732d 6469 736b 2d74 6965 7227   'aws-disk-tier'
-00016cc0: 2c0a 2020 2020 2020 2020 2020 2020 5b0a  ,.            [.
-00016cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ce0: 6627 736b 7920 6c61 756e 6368 202d 7920  f'sky launch -y 
-00016cf0: 2d63 207b 6e61 6d65 7d20 2d2d 636c 6f75  -c {name} --clou
-00016d00: 6420 6177 7320 2d2d 7265 6769 6f6e 207b  d aws --region {
-00016d10: 7265 6769 6f6e 7d20 270a 2020 2020 2020  region} '.      
-00016d20: 2020 2020 2020 2020 2020 6627 2d2d 6469            f'--di
-00016d30: 736b 2d74 6965 7220 7b64 6973 6b5f 7469  sk-tier {disk_ti
-00016d40: 6572 7d20 6563 686f 2022 6865 6c6c 6f20  er} echo "hello 
-00016d50: 736b 7922 272c 0a20 2020 2020 2020 2020  sky"',.         
-00016d60: 2020 2020 2020 2066 2769 643d 6061 7773         f'id=`aws
-00016d70: 2065 6332 2064 6573 6372 6962 652d 696e   ec2 describe-in
-00016d80: 7374 616e 6365 7320 2d2d 7265 6769 6f6e  stances --region
-00016d90: 207b 7265 6769 6f6e 7d20 2d2d 6669 6c74   {region} --filt
-00016da0: 6572 7320 270a 2020 2020 2020 2020 2020  ers '.          
-00016db0: 2020 2020 2020 6627 4e61 6d65 3d74 6167        f'Name=tag
-00016dc0: 3a72 6179 2d63 6c75 7374 6572 2d6e 616d  :ray-cluster-nam
-00016dd0: 652c 5661 6c75 6573 3d7b 6e61 6d65 7d20  e,Values={name} 
-00016de0: 2d2d 7175 6572 7920 270a 2020 2020 2020  --query '.      
-00016df0: 2020 2020 2020 2020 2020 6627 5265 7365            f'Rese
-00016e00: 7276 6174 696f 6e73 5b5d 2e49 6e73 7461  rvations[].Insta
-00016e10: 6e63 6573 5b5d 2e49 6e73 7461 6e63 6549  nces[].InstanceI
-00016e20: 6420 2d2d 6f75 7470 7574 2074 6578 7460  d --output text`
-00016e30: 3b20 2720 2b0a 2020 2020 2020 2020 2020  ; ' +.          
-00016e40: 2020 2020 2020 5f67 6574 5f61 7773 5f71        _get_aws_q
-00016e50: 7565 7279 5f63 6f6d 6d61 6e64 2872 6567  uery_command(reg
-00016e60: 696f 6e2c 2027 2469 6427 2c20 2756 6f6c  ion, '$id', 'Vol
-00016e70: 756d 6554 7970 6527 2c0a 2020 2020 2020  umeType',.      
-00016e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ea0: 2073 7065 6373 5b27 6469 736b 5f74 6965   specs['disk_tie
-00016eb0: 7227 5d29 202b 0a20 2020 2020 2020 2020  r']) +.         
-00016ec0: 2020 2020 2020 2028 2727 2069 6620 6469         ('' if di
-00016ed0: 736b 5f74 6965 7220 3d3d 2027 6c6f 7727  sk_tier == 'low'
-00016ee0: 2065 6c73 650a 2020 2020 2020 2020 2020   else.          
-00016ef0: 2020 2020 2020 2028 5f67 6574 5f61 7773         (_get_aws
-00016f00: 5f71 7565 7279 5f63 6f6d 6d61 6e64 2872  _query_command(r
-00016f10: 6567 696f 6e2c 2027 2469 6427 2c20 2749  egion, '$id', 'I
-00016f20: 6f70 7327 2c0a 2020 2020 2020 2020 2020  ops',.          
-00016f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016f50: 7065 6373 5b27 6469 736b 5f69 6f70 7327  pecs['disk_iops'
-00016f60: 5d29 202b 0a20 2020 2020 2020 2020 2020  ]) +.           
-00016f70: 2020 2020 2020 205f 6765 745f 6177 735f         _get_aws_
-00016f80: 7175 6572 795f 636f 6d6d 616e 6428 7265  query_command(re
-00016f90: 6769 6f6e 2c20 2724 6964 272c 2027 5468  gion, '$id', 'Th
-00016fa0: 726f 7567 6870 7574 272c 0a20 2020 2020  roughput',.     
-00016fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fd0: 2020 2020 7370 6563 735b 2764 6973 6b5f      specs['disk_
-00016fe0: 7468 726f 7567 6870 7574 275d 2929 292c  throughput']))),
-00016ff0: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
-00017000: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-00017010: 7920 646f 776e 202d 7920 7b6e 616d 657d  y down -y {name}
-00017020: 272c 0a20 2020 2020 2020 2020 2020 2074  ',.            t
-00017030: 696d 656f 7574 3d31 3020 2a20 3630 2c20  imeout=10 * 60, 
-00017040: 2023 2031 3020 6d69 6e73 2020 2869 7420   # 10 mins  (it 
-00017050: 7461 6b65 7320 6172 6f75 6e64 207e 3620  takes around ~6 
-00017060: 6d69 6e73 290a 2020 2020 2020 2020 290a  mins).        ).
-00017070: 2020 2020 2020 2020 7275 6e5f 6f6e 655f          run_one_
-00017080: 7465 7374 2874 6573 7429 0a0a 0a40 7079  test(test)...@py
-00017090: 7465 7374 2e6d 6172 6b2e 6763 700a 6465  test.mark.gcp.de
-000170a0: 6620 7465 7374 5f67 6370 5f64 6973 6b5f  f test_gcp_disk_
-000170b0: 7469 6572 2829 3a0a 2020 2020 666f 7220  tier():.    for 
-000170c0: 6469 736b 5f74 6965 7220 696e 205b 276c  disk_tier in ['l
-000170d0: 6f77 272c 2027 6d65 6469 756d 272c 2027  ow', 'medium', '
-000170e0: 6869 6768 275d 3a0a 2020 2020 2020 2020  high']:.        
-000170f0: 7479 7065 203d 2047 4350 2e5f 6765 745f  type = GCP._get_
-00017100: 6469 736b 5f74 7970 6528 6469 736b 5f74  disk_type(disk_t
-00017110: 6965 7229 0a20 2020 2020 2020 206e 616d  ier).        nam
-00017120: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
-00017130: 5f6e 616d 6528 2920 2b20 272d 2720 2b20  _name() + '-' + 
-00017140: 6469 736b 5f74 6965 720a 2020 2020 2020  disk_tier.      
-00017150: 2020 7265 6769 6f6e 203d 2027 7573 2d77    region = 'us-w
-00017160: 6573 7432 270a 2020 2020 2020 2020 7465  est2'.        te
-00017170: 7374 203d 2054 6573 7428 0a20 2020 2020  st = Test(.     
-00017180: 2020 2020 2020 2027 6763 702d 6469 736b         'gcp-disk
-00017190: 2d74 6965 7227 2c0a 2020 2020 2020 2020  -tier',.        
-000171a0: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
-000171b0: 2020 2020 2020 6627 736b 7920 6c61 756e        f'sky laun
-000171c0: 6368 202d 7920 2d63 207b 6e61 6d65 7d20  ch -y -c {name} 
-000171d0: 2d2d 636c 6f75 6420 6763 7020 2d2d 7265  --cloud gcp --re
-000171e0: 6769 6f6e 207b 7265 6769 6f6e 7d20 270a  gion {region} '.
-000171f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017200: 6627 2d2d 6469 736b 2d74 6965 7220 7b64  f'--disk-tier {d
-00017210: 6973 6b5f 7469 6572 7d20 6563 686f 2022  isk_tier} echo "
-00017220: 6865 6c6c 6f20 736b 7922 272c 0a20 2020  hello sky"',.   
-00017230: 2020 2020 2020 2020 2020 2020 2066 276e               f'n
-00017240: 616d 653d 6067 636c 6f75 6420 636f 6d70  ame=`gcloud comp
-00017250: 7574 6520 696e 7374 616e 6365 7320 6c69  ute instances li
-00017260: 7374 202d 2d66 696c 7465 723d 270a 2020  st --filter='.  
-00017270: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-00017280: 226c 6162 656c 732e 7261 792d 636c 7573  "labels.ray-clus
-00017290: 7465 722d 6e61 6d65 3a7b 6e61 6d65 7d22  ter-name:{name}"
-000172a0: 202d 2d66 6f72 6d61 743d 2276 616c 7565   --format="value
-000172b0: 286e 616d 6529 2260 3b20 270a 2020 2020  (name)"`; '.    
-000172c0: 2020 2020 2020 2020 2020 2020 6627 6763              f'gc
-000172d0: 6c6f 7564 2063 6f6d 7075 7465 2064 6973  loud compute dis
-000172e0: 6b73 206c 6973 7420 2d2d 6669 6c74 6572  ks list --filter
-000172f0: 3d22 6e61 6d65 3d24 6e61 6d65 2220 270a  ="name=$name" '.
-00017300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017310: 6627 2d2d 666f 726d 6174 3d22 7661 6c75  f'--format="valu
-00017320: 6528 7479 7065 2922 207c 2067 7265 7020  e(type)" | grep 
-00017330: 7b74 7970 657d 2027 0a20 2020 2020 2020  {type} '.       
-00017340: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00017350: 2020 2020 6627 736b 7920 646f 776e 202d      f'sky down -
-00017360: 7920 7b6e 616d 657d 272c 0a20 2020 2020  y {name}',.     
-00017370: 2020 2020 2020 2074 696d 656f 7574 3d36         timeout=6
-00017380: 202a 2036 302c 2020 2320 3620 6d69 6e73   * 60,  # 6 mins
-00017390: 2020 2869 7420 7461 6b65 7320 6172 6f75    (it takes arou
-000173a0: 6e64 207e 3320 6d69 6e73 290a 2020 2020  nd ~3 mins).    
-000173b0: 2020 2020 290a 2020 2020 2020 2020 7275      ).        ru
-000173c0: 6e5f 6f6e 655f 7465 7374 2874 6573 7429  n_one_test(test)
-000173d0: 0a0a 0a40 7079 7465 7374 2e6d 6172 6b2e  ...@pytest.mark.
-000173e0: 617a 7572 650a 6465 6620 7465 7374 5f61  azure.def test_a
-000173f0: 7a75 7265 5f64 6973 6b5f 7469 6572 2829  zure_disk_tier()
-00017400: 3a0a 2020 2020 666f 7220 6469 736b 5f74  :.    for disk_t
-00017410: 6965 7220 696e 205b 276c 6f77 272c 2027  ier in ['low', '
-00017420: 6d65 6469 756d 275d 3a0a 2020 2020 2020  medium']:.      
-00017430: 2020 7479 7065 203d 2041 7a75 7265 2e5f    type = Azure._
-00017440: 6765 745f 6469 736b 5f74 7970 6528 6469  get_disk_type(di
-00017450: 736b 5f74 6965 7229 0a20 2020 2020 2020  sk_tier).       
-00017460: 206e 616d 6520 3d20 5f67 6574 5f63 6c75   name = _get_clu
-00017470: 7374 6572 5f6e 616d 6528 2920 2b20 272d  ster_name() + '-
-00017480: 2720 2b20 6469 736b 5f74 6965 720a 2020  ' + disk_tier.  
-00017490: 2020 2020 2020 7265 6769 6f6e 203d 2027        region = '
-000174a0: 7765 7374 7573 3227 0a20 2020 2020 2020  westus2'.       
-000174b0: 2074 6573 7420 3d20 5465 7374 280a 2020   test = Test(.  
-000174c0: 2020 2020 2020 2020 2020 2761 7a75 7265            'azure
-000174d0: 2d64 6973 6b2d 7469 6572 272c 0a20 2020  -disk-tier',.   
-000174e0: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
-000174f0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-00017500: 206c 6175 6e63 6820 2d79 202d 6320 7b6e   launch -y -c {n
-00017510: 616d 657d 202d 2d63 6c6f 7564 2061 7a75  ame} --cloud azu
-00017520: 7265 202d 2d72 6567 696f 6e20 7b72 6567  re --region {reg
-00017530: 696f 6e7d 2027 0a20 2020 2020 2020 2020  ion} '.         
-00017540: 2020 2020 2020 2066 272d 2d64 6973 6b2d         f'--disk-
-00017550: 7469 6572 207b 6469 736b 5f74 6965 727d  tier {disk_tier}
-00017560: 2065 6368 6f20 2268 656c 6c6f 2073 6b79   echo "hello sky
-00017570: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-00017580: 2020 2020 6627 617a 2072 6573 6f75 7263      f'az resourc
-00017590: 6520 6c69 7374 202d 2d74 6167 2072 6179  e list --tag ray
-000175a0: 2d63 6c75 7374 6572 2d6e 616d 653d 7b6e  -cluster-name={n
-000175b0: 616d 657d 202d 2d71 7565 7279 2027 0a20  ame} --query '. 
-000175c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000175d0: 2722 5b3f 7479 7065 3d3d 5c27 4d69 6372  '"[?type==\'Micr
-000175e0: 6f73 6f66 742e 436f 6d70 7574 652f 6469  osoft.Compute/di
-000175f0: 736b 735c 275d 2e73 6b75 2e6e 616d 6522  sks\'].sku.name"
-00017600: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-00017610: 2020 2066 272d 2d6f 7574 7075 7420 7473     f'--output ts
-00017620: 7620 7c20 6772 6570 207b 7479 7065 7d27  v | grep {type}'
-00017630: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
-00017640: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-00017650: 7920 646f 776e 202d 7920 7b6e 616d 657d  y down -y {name}
-00017660: 272c 0a20 2020 2020 2020 2020 2020 2074  ',.            t
-00017670: 696d 656f 7574 3d32 3020 2a20 3630 2c20  imeout=20 * 60, 
-00017680: 2023 2032 3020 6d69 6e73 2020 2869 7420   # 20 mins  (it 
-00017690: 7461 6b65 7320 6172 6f75 6e64 207e 3132  takes around ~12
-000176a0: 206d 696e 7329 0a20 2020 2020 2020 2029   mins).        )
-000176b0: 0a20 2020 2020 2020 2072 756e 5f6f 6e65  .        run_one
-000176c0: 5f74 6573 7428 7465 7374 290a 0a0a 2320  _test(test)...# 
-000176d0: 2d2d 2d2d 2d2d 2054 6573 7469 6e67 205a  ------ Testing Z
-000176e0: 6572 6f20 5175 6f74 6120 4661 696c 6f76  ero Quota Failov
-000176f0: 6572 202d 2d2d 2d2d 2d0a 4070 7974 6573  er ------.@pytes
-00017700: 742e 6d61 726b 2e61 7773 0a64 6566 2074  t.mark.aws.def t
-00017710: 6573 745f 6177 735f 7a65 726f 5f71 756f  est_aws_zero_quo
-00017720: 7461 5f66 6169 6c6f 7665 7228 293a 0a0a  ta_failover():..
-00017730: 2020 2020 6e61 6d65 203d 205f 6765 745f      name = _get_
-00017740: 636c 7573 7465 725f 6e61 6d65 2829 0a20  cluster_name(). 
-00017750: 2020 2072 6567 696f 6e20 3d20 6765 745f     region = get_
-00017760: 6177 735f 7265 6769 6f6e 5f66 6f72 5f71  aws_region_for_q
-00017770: 756f 7461 5f66 6169 6c6f 7665 7228 290a  uota_failover().
-00017780: 0a20 2020 2069 6620 6e6f 7420 7265 6769  .    if not regi
-00017790: 6f6e 3a0a 2020 2020 2020 2020 7265 7475  on:.        retu
-000177a0: 726e 0a0a 2020 2020 7465 7374 203d 2054  rn..    test = T
-000177b0: 6573 7428 0a20 2020 2020 2020 2027 6177  est(.        'aw
-000177c0: 732d 7a65 726f 2d71 756f 7461 2d66 6169  s-zero-quota-fai
-000177d0: 6c6f 7665 7227 2c0a 2020 2020 2020 2020  lover',.        
-000177e0: 5b0a 2020 2020 2020 2020 2020 2020 6627  [.            f'
-000177f0: 736b 7920 6c61 756e 6368 202d 7920 2d63  sky launch -y -c
-00017800: 207b 6e61 6d65 7d20 2d2d 636c 6f75 6420   {name} --cloud 
-00017810: 6177 7320 2d2d 7265 6769 6f6e 207b 7265  aws --region {re
-00017820: 6769 6f6e 7d20 2d2d 6770 7573 2056 3130  gion} --gpus V10
-00017830: 303a 3820 2d2d 7573 652d 7370 6f74 207c  0:8 --use-spot |
-00017840: 2067 7265 7020 2246 6f75 6e64 206e 6f20   grep "Found no 
-00017850: 7175 6f74 6122 272c 0a20 2020 2020 2020  quota"',.       
-00017860: 205d 2c0a 2020 2020 2020 2020 6627 736b   ],.        f'sk
-00017870: 7920 646f 776e 202d 7920 7b6e 616d 657d  y down -y {name}
-00017880: 272c 0a20 2020 2029 0a20 2020 2072 756e  ',.    ).    run
-00017890: 5f6f 6e65 5f74 6573 7428 7465 7374 290a  _one_test(test).
-000178a0: 0a0a 2320 2d2d 2d2d 2d2d 2d20 5465 7374  ..# ------- Test
-000178b0: 696e 6720 7573 6572 2072 6179 2063 6c75  ing user ray clu
-000178c0: 7374 6572 202d 2d2d 2d2d 2d2d 2d0a 6465  ster --------.de
-000178d0: 6620 7465 7374 5f75 7365 725f 7261 795f  f test_user_ray_
-000178e0: 636c 7573 7465 7228 293a 0a20 2020 206e  cluster():.    n
-000178f0: 616d 6520 3d20 5f67 6574 5f63 6c75 7374  ame = _get_clust
-00017900: 6572 5f6e 616d 6528 290a 2020 2020 7465  er_name().    te
-00017910: 7374 203d 2054 6573 7428 0a20 2020 2020  st = Test(.     
-00017920: 2020 2027 7573 6572 2d72 6179 2d63 6c75     'user-ray-clu
-00017930: 7374 6572 272c 0a20 2020 2020 2020 205b  ster',.        [
-00017940: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-00017950: 6b79 206c 6175 6e63 6820 2d79 202d 6320  ky launch -y -c 
-00017960: 7b6e 616d 657d 2022 7261 7920 7374 6172  {name} "ray star
-00017970: 7420 2d2d 6865 6164 2227 2c0a 2020 2020  t --head"',.    
-00017980: 2020 2020 2020 2020 6627 736b 7920 6578          f'sky ex
-00017990: 6563 207b 6e61 6d65 7d20 2265 6368 6f20  ec {name} "echo 
-000179a0: 6869 2227 2c0a 2020 2020 2020 2020 2020  hi"',.          
-000179b0: 2020 6627 736b 7920 6c6f 6773 207b 6e61    f'sky logs {na
-000179c0: 6d65 7d20 3120 2d2d 7374 6174 7573 272c  me} 1 --status',
-000179d0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-000179e0: 6b79 2073 7461 7475 7320 2d72 207c 2067  ky status -r | g
-000179f0: 7265 7020 7b6e 616d 657d 207c 2067 7265  rep {name} | gre
-00017a00: 7020 5550 272c 0a20 2020 2020 2020 2020  p UP',.         
-00017a10: 2020 2066 2773 6b79 2065 7865 6320 7b6e     f'sky exec {n
-00017a20: 616d 657d 2022 6563 686f 2062 7965 2227  ame} "echo bye"'
-00017a30: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-00017a40: 736b 7920 6c6f 6773 207b 6e61 6d65 7d20  sky logs {name} 
-00017a50: 3220 2d2d 7374 6174 7573 272c 0a20 2020  2 --status',.   
-00017a60: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00017a70: 6627 736b 7920 646f 776e 202d 7920 7b6e  f'sky down -y {n
-00017a80: 616d 657d 272c 0a20 2020 2029 0a20 2020  ame}',.    ).   
-00017a90: 2072 756e 5f6f 6e65 5f74 6573 7428 7465   run_one_test(te
-00017aa0: 7374 290a 0a0a 2320 2d2d 2d2d 2d2d 2d20  st)...# ------- 
-00017ab0: 5465 7374 696e 6720 7468 6520 636f 7265  Testing the core
-00017ac0: 2041 5049 202d 2d2d 2d2d 2d2d 2d0a 2320   API --------.# 
-00017ad0: 4d6f 7374 206f 6620 7468 6520 636f 7265  Most of the core
-00017ae0: 2041 5049 7320 6861 7665 2062 6565 6e20   APIs have been 
-00017af0: 7465 7374 6564 2069 6e20 7468 6520 434c  tested in the CL
-00017b00: 4920 7465 7374 732e 0a23 2054 6865 7365  I tests..# These
-00017b10: 2074 6573 7473 2061 7265 2066 6f72 2074   tests are for t
-00017b20: 6573 7469 6e67 2074 6865 2072 6574 7572  esting the retur
-00017b30: 6e20 7661 6c75 6520 6f66 2074 6865 2041  n value of the A
-00017b40: 5049 7320 6e6f 7420 6675 6c6c 7920 7573  PIs not fully us
-00017b50: 6564 2069 6e20 434c 492e 0a64 6566 2074  ed in CLI..def t
-00017b60: 6573 745f 636f 7265 5f61 7069 2829 3a0a  est_core_api():.
-00017b70: 2020 2020 6e61 6d65 203d 205f 6765 745f      name = _get_
-00017b80: 636c 7573 7465 725f 6e61 6d65 2829 0a20  cluster_name(). 
-00017b90: 2020 2073 6b79 2e6c 6175 6e63 680a 2020     sky.launch.  
-00017ba0: 2020 2320 544f 444f 287a 6877 7529 3a20    # TODO(zhwu): 
-00017bb0: 4164 6420 6120 7465 7374 2066 6f72 2063  Add a test for c
-00017bc0: 6f72 6520 6170 692e 0a0a 0a23 202d 2d2d  ore api....# ---
-00017bd0: 2d2d 2d2d 2d2d 2d20 5465 7374 696e 6720  ------- Testing 
-00017be0: 5374 6f72 6167 6520 2d2d 2d2d 2d2d 2d2d  Storage --------
-00017bf0: 2d2d 0a63 6c61 7373 2054 6573 7453 746f  --.class TestSto
-00017c00: 7261 6765 5769 7468 4372 6564 656e 7469  rageWithCredenti
-00017c10: 616c 733a 0a20 2020 2022 2222 5374 6f72  als:.    """Stor
-00017c20: 6167 6520 7465 7374 7320 7768 6963 6820  age tests which 
-00017c30: 7265 7175 6972 6520 6372 6564 656e 7469  require credenti
-00017c40: 616c 7320 616e 6420 6e65 7477 6f72 6b20  als and network 
-00017c50: 636f 6e6e 6563 7469 6f6e 2222 220a 0a20  connection""".. 
-00017c60: 2020 2041 5753 5f49 4e56 414c 4944 5f4e     AWS_INVALID_N
-00017c70: 414d 4553 203d 205b 0a20 2020 2020 2020  AMES = [.       
-00017c80: 2027 6162 272c 2020 2320 6c65 7373 2074   'ab',  # less t
-00017c90: 6861 6e20 3320 6368 6172 6163 7465 7273  han 3 characters
-00017ca0: 0a20 2020 2020 2020 2027 6162 6364 6566  .        'abcdef
-00017cb0: 6768 696a 6b6c 6d6e 6f70 7172 7374 7576  ghijklmnopqrstuv
-00017cc0: 7778 797a 6162 6364 6566 6768 696a 6b6c  wxyzabcdefghijkl
-00017cd0: 6d6e 6f70 7172 7374 7576 7778 797a 6162  mnopqrstuvwxyzab
-00017ce0: 6364 6566 6768 696a 6b6c 6d6e 6f70 7172  cdefghijklmnopqr
-00017cf0: 7374 7576 7778 797a 3127 2c0a 2020 2020  stuvwxyz1',.    
-00017d00: 2020 2020 2320 6d6f 7265 2074 6861 6e20      # more than 
-00017d10: 3633 2063 6861 7261 6374 6572 730a 2020  63 characters.  
-00017d20: 2020 2020 2020 2741 6263 6465 6627 2c20        'Abcdef', 
-00017d30: 2023 2063 6f6e 7461 696e 7320 616e 2075   # contains an u
-00017d40: 7070 6572 6361 7365 206c 6574 7465 720a  ppercase letter.
-00017d50: 2020 2020 2020 2020 2761 6263 2064 6566          'abc def
-00017d60: 272c 2020 2320 636f 6e74 6169 6e73 2061  ',  # contains a
-00017d70: 2073 7061 6365 0a20 2020 2020 2020 2027   space.        '
-00017d80: 6162 632e 2e64 6566 272c 2020 2320 7477  abc..def',  # tw
-00017d90: 6f20 6164 6a61 6365 6e74 2070 6572 696f  o adjacent perio
-00017da0: 6473 0a20 2020 2020 2020 2027 3139 322e  ds.        '192.
-00017db0: 3136 382e 352e 3427 2c20 2023 2066 6f72  168.5.4',  # for
-00017dc0: 6d61 7474 6564 2061 7320 616e 2049 5020  matted as an IP 
-00017dd0: 6164 6472 6573 730a 2020 2020 2020 2020  address.        
-00017de0: 2778 6e2d 2d62 7563 6b65 7427 2c20 2023  'xn--bucket',  #
-00017df0: 2073 7461 7274 7320 7769 7468 2027 786e   starts with 'xn
-00017e00: 2d2d 2720 7072 6566 6978 0a20 2020 2020  --' prefix.     
-00017e10: 2020 2027 6275 636b 6574 2d73 3361 6c69     'bucket-s3ali
-00017e20: 6173 272c 2020 2320 656e 6473 2077 6974  as',  # ends wit
-00017e30: 6820 272d 7333 616c 6961 7327 2073 7566  h '-s3alias' suf
-00017e40: 6669 780a 2020 2020 2020 2020 2762 7563  fix.        'buc
-00017e50: 6b65 742d 2d6f 6c2d 7333 272c 2020 2320  ket--ol-s3',  # 
-00017e60: 656e 6473 2077 6974 6820 272d 2d6f 6c2d  ends with '--ol-
-00017e70: 7333 2720 7375 6666 6978 0a20 2020 2020  s3' suffix.     
-00017e80: 2020 2027 2e61 6263 272c 2020 2320 7374     '.abc',  # st
-00017e90: 6172 7473 2077 6974 6820 6120 646f 740a  arts with a dot.
-00017ea0: 2020 2020 2020 2020 2761 6263 2e27 2c20          'abc.', 
-00017eb0: 2023 2065 6e64 7320 7769 7468 2061 2064   # ends with a d
-00017ec0: 6f74 0a20 2020 2020 2020 2027 2d61 6263  ot.        '-abc
-00017ed0: 272c 2020 2320 7374 6172 7473 2077 6974  ',  # starts wit
-00017ee0: 6820 6120 6879 7068 656e 0a20 2020 2020  h a hyphen.     
-00017ef0: 2020 2027 6162 632d 272c 2020 2320 656e     'abc-',  # en
-00017f00: 6473 2077 6974 6820 6120 6879 7068 656e  ds with a hyphen
-00017f10: 0a20 2020 205d 0a0a 2020 2020 4743 535f  .    ]..    GCS_
-00017f20: 494e 5641 4c49 445f 4e41 4d45 5320 3d20  INVALID_NAMES = 
-00017f30: 5b0a 2020 2020 2020 2020 2761 6227 2c20  [.        'ab', 
-00017f40: 2023 206c 6573 7320 7468 616e 2033 2063   # less than 3 c
-00017f50: 6861 7261 6374 6572 730a 2020 2020 2020  haracters.      
-00017f60: 2020 2761 6263 6465 6667 6869 6a6b 6c6d    'abcdefghijklm
-00017f70: 6e6f 7071 7273 7475 7677 7879 7a61 6263  nopqrstuvwxyzabc
-00017f80: 6465 6667 6869 6a6b 6c6d 6e6f 7071 7273  defghijklmnopqrs
-00017f90: 7475 7677 7879 7a61 6263 6465 6667 6869  tuvwxyzabcdefghi
-00017fa0: 6a6b 6c6d 6e6f 7071 7273 7475 7677 7879  jklmnopqrstuvwxy
-00017fb0: 7a31 272c 0a20 2020 2020 2020 2023 206d  z1',.        # m
-00017fc0: 6f72 6520 7468 616e 2036 3320 6368 6172  ore than 63 char
-00017fd0: 6163 7465 7273 2028 7769 7468 6f75 7420  acters (without 
-00017fe0: 646f 7473 290a 2020 2020 2020 2020 2741  dots).        'A
-00017ff0: 6263 6465 6627 2c20 2023 2063 6f6e 7461  bcdef',  # conta
-00018000: 696e 7320 616e 2075 7070 6572 6361 7365  ins an uppercase
-00018010: 206c 6574 7465 720a 2020 2020 2020 2020   letter.        
-00018020: 2761 6263 2064 6566 272c 2020 2320 636f  'abc def',  # co
-00018030: 6e74 6169 6e73 2061 2073 7061 6365 0a20  ntains a space. 
-00018040: 2020 2020 2020 2027 6162 632e 2e64 6566         'abc..def
-00018050: 272c 2020 2320 7477 6f20 6164 6a61 6365  ',  # two adjace
-00018060: 6e74 2070 6572 696f 6473 0a20 2020 2020  nt periods.     
-00018070: 2020 2027 6162 635f 2e64 6566 2e67 6869     'abc_.def.ghi
-00018080: 2e6a 6b6c 6d6e 6f70 7172 7374 7576 7778  .jklmnopqrstuvwx
-00018090: 797a 6162 6364 6566 6768 696a 6b6c 6d6e  yzabcdefghijklmn
-000180a0: 6f70 7172 7374 7576 7778 797a 6162 6364  opqrstuvwxyzabcd
-000180b0: 6566 6768 696a 6b6c 6d6e 6f70 7172 7374  efghijklmnopqrst
-000180c0: 7576 7778 797a 3127 0a20 2020 2020 2020  uvwxyz1'.       
-000180d0: 2023 204d 6f72 6520 7468 616e 2036 3320   # More than 63 
-000180e0: 6368 6172 6163 7465 7273 2062 6574 7765  characters betwe
-000180f0: 656e 2064 6f74 730a 2020 2020 2020 2020  en dots.        
-00018100: 2761 6263 5f2e 6465 662e 6768 692e 6a6b  'abc_.def.ghi.jk
-00018110: 6c6d 6e6f 7071 7273 7475 7677 7879 7a61  lmnopqrstuvwxyza
-00018120: 6263 6465 6667 6869 6a6b 6c6d 6e6f 7071  bcdefghijklmnopq
-00018130: 6667 6869 6a6b 6c6d 6e6f 7071 7273 7475  fghijklmnopqrstu
-00018140: 7677 2720 2a20 352c 0a20 2020 2020 2020  vw' * 5,.       
-00018150: 2023 206d 6f72 6520 7468 616e 2032 3232   # more than 222
-00018160: 2063 6861 7261 6374 6572 7320 2877 6974   characters (wit
-00018170: 6820 646f 7473 290a 2020 2020 2020 2020  h dots).        
-00018180: 2731 3932 2e31 3638 2e35 2e34 272c 2020  '192.168.5.4',  
-00018190: 2320 666f 726d 6174 7465 6420 6173 2061  # formatted as a
-000181a0: 6e20 4950 2061 6464 7265 7373 0a20 2020  n IP address.   
-000181b0: 2020 2020 2027 676f 6f67 6275 636b 6574       'googbucket
-000181c0: 272c 2020 2320 7374 6172 7473 2077 6974  ',  # starts wit
-000181d0: 6820 2767 6f6f 6727 2070 7265 6669 780a  h 'goog' prefix.
-000181e0: 2020 2020 2020 2020 2767 6f6f 676c 6562          'googleb
-000181f0: 7563 6b65 7427 2c20 2023 2063 6f6e 7461  ucket',  # conta
-00018200: 696e 7320 2767 6f6f 676c 6527 0a20 2020  ins 'google'.   
-00018210: 2020 2020 2027 6730 3067 6c65 6275 636b       'g00glebuck
-00018220: 6574 272c 2020 2320 7661 7269 616e 7420  et',  # variant 
-00018230: 6f66 2027 676f 6f67 6c65 270a 2020 2020  of 'google'.    
-00018240: 2020 2020 2767 6f30 676c 6562 7563 6b65      'go0glebucke
-00018250: 7427 2c20 2023 2076 6172 6961 6e74 206f  t',  # variant o
-00018260: 6620 2767 6f6f 676c 6527 0a20 2020 2020  f 'google'.     
-00018270: 2020 2027 6730 6f67 6c65 6275 636b 6574     'g0oglebucket
-00018280: 272c 2020 2320 7661 7269 616e 7420 6f66  ',  # variant of
-00018290: 2027 676f 6f67 6c65 270a 2020 2020 2020   'google'.      
-000182a0: 2020 272e 6162 6327 2c20 2023 2073 7461    '.abc',  # sta
-000182b0: 7274 7320 7769 7468 2061 2064 6f74 0a20  rts with a dot. 
-000182c0: 2020 2020 2020 2027 6162 632e 272c 2020         'abc.',  
-000182d0: 2320 656e 6473 2077 6974 6820 6120 646f  # ends with a do
-000182e0: 740a 2020 2020 2020 2020 275f 6162 6327  t.        '_abc'
-000182f0: 2c20 2023 2073 7461 7274 7320 7769 7468  ,  # starts with
-00018300: 2061 6e20 756e 6465 7273 636f 7265 0a20   an underscore. 
-00018310: 2020 2020 2020 2027 6162 635f 272c 2020         'abc_',  
-00018320: 2320 656e 6473 2077 6974 6820 616e 2075  # ends with an u
-00018330: 6e64 6572 7363 6f72 650a 2020 2020 5d0a  nderscore.    ].
-00018340: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-00018350: 6f64 0a20 2020 2064 6566 2063 6c69 5f64  od.    def cli_d
-00018360: 656c 6574 655f 636d 6428 7374 6f72 655f  elete_cmd(store_
-00018370: 7479 7065 2c20 6275 636b 6574 5f6e 616d  type, bucket_nam
-00018380: 6529 3a0a 2020 2020 2020 2020 6966 2073  e):.        if s
-00018390: 746f 7265 5f74 7970 6520 3d3d 2073 746f  tore_type == sto
-000183a0: 7261 6765 5f6c 6962 2e53 746f 7265 5479  rage_lib.StoreTy
-000183b0: 7065 2e53 333a 0a20 2020 2020 2020 2020  pe.S3:.         
-000183c0: 2020 2075 726c 203d 2066 2773 333a 2f2f     url = f's3://
-000183d0: 7b62 7563 6b65 745f 6e61 6d65 7d27 0a20  {bucket_name}'. 
-000183e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000183f0: 6e20 6627 6177 7320 7333 2072 6220 7b75  n f'aws s3 rb {u
-00018400: 726c 7d20 2d2d 666f 7263 6527 0a20 2020  rl} --force'.   
-00018410: 2020 2020 2069 6620 7374 6f72 655f 7479       if store_ty
-00018420: 7065 203d 3d20 7374 6f72 6167 655f 6c69  pe == storage_li
-00018430: 622e 5374 6f72 6554 7970 652e 4743 533a  b.StoreType.GCS:
-00018440: 0a20 2020 2020 2020 2020 2020 2075 726c  .            url
-00018450: 203d 2066 2767 733a 2f2f 7b62 7563 6b65   = f'gs://{bucke
-00018460: 745f 6e61 6d65 7d27 0a20 2020 2020 2020  t_name}'.       
-00018470: 2020 2020 2072 6574 7572 6e20 6627 6773       return f'gs
-00018480: 7574 696c 202d 6d20 726d 202d 7220 7b75  util -m rm -r {u
-00018490: 726c 7d27 0a20 2020 2020 2020 2069 6620  rl}'.        if 
-000184a0: 7374 6f72 655f 7479 7065 203d 3d20 7374  store_type == st
-000184b0: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
-000184c0: 7970 652e 5232 3a0a 2020 2020 2020 2020  ype.R2:.        
-000184d0: 2020 2020 656e 6470 6f69 6e74 5f75 726c      endpoint_url
-000184e0: 203d 2063 6c6f 7564 666c 6172 652e 6372   = cloudflare.cr
-000184f0: 6561 7465 5f65 6e64 706f 696e 7428 290a  eate_endpoint().
-00018500: 2020 2020 2020 2020 2020 2020 7572 6c20              url 
-00018510: 3d20 6627 7333 3a2f 2f7b 6275 636b 6574  = f's3://{bucket
-00018520: 5f6e 616d 657d 270a 2020 2020 2020 2020  _name}'.        
-00018530: 2020 2020 7265 7475 726e 2066 2741 5753      return f'AWS
-00018540: 5f53 4841 5245 445f 4352 4544 454e 5449  _SHARED_CREDENTI
-00018550: 414c 535f 4649 4c45 3d7b 636c 6f75 6466  ALS_FILE={cloudf
-00018560: 6c61 7265 2e52 325f 4352 4544 454e 5449  lare.R2_CREDENTI
-00018570: 414c 535f 5041 5448 7d20 6177 7320 7333  ALS_PATH} aws s3
-00018580: 2072 6220 7b75 726c 7d20 2d2d 666f 7263   rb {url} --forc
-00018590: 6520 2d2d 656e 6470 6f69 6e74 207b 656e  e --endpoint {en
-000185a0: 6470 6f69 6e74 5f75 726c 7d20 2d2d 7072  dpoint_url} --pr
-000185b0: 6f66 696c 653d 7232 270a 0a20 2020 2040  ofile=r2'..    @
-000185c0: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
-000185d0: 2064 6566 2063 6c69 5f6c 735f 636d 6428   def cli_ls_cmd(
-000185e0: 7374 6f72 655f 7479 7065 2c20 6275 636b  store_type, buck
-000185f0: 6574 5f6e 616d 652c 2073 7566 6669 783d  et_name, suffix=
-00018600: 2727 293a 0a20 2020 2020 2020 2069 6620  ''):.        if 
-00018610: 7374 6f72 655f 7479 7065 203d 3d20 7374  store_type == st
-00018620: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
-00018630: 7970 652e 5333 3a0a 2020 2020 2020 2020  ype.S3:.        
-00018640: 2020 2020 6966 2073 7566 6669 783a 0a20      if suffix:. 
-00018650: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00018660: 726c 203d 2066 2773 333a 2f2f 7b62 7563  rl = f's3://{buc
-00018670: 6b65 745f 6e61 6d65 7d2f 7b73 7566 6669  ket_name}/{suffi
-00018680: 787d 270a 2020 2020 2020 2020 2020 2020  x}'.            
-00018690: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000186a0: 2020 2020 2020 7572 6c20 3d20 6627 7333        url = f's3
-000186b0: 3a2f 2f7b 6275 636b 6574 5f6e 616d 657d  ://{bucket_name}
-000186c0: 270a 2020 2020 2020 2020 2020 2020 7265  '.            re
-000186d0: 7475 726e 2066 2761 7773 2073 3320 6c73  turn f'aws s3 ls
-000186e0: 207b 7572 6c7d 270a 2020 2020 2020 2020   {url}'.        
-000186f0: 6966 2073 746f 7265 5f74 7970 6520 3d3d  if store_type ==
-00018700: 2073 746f 7261 6765 5f6c 6962 2e53 746f   storage_lib.Sto
-00018710: 7265 5479 7065 2e47 4353 3a0a 2020 2020  reType.GCS:.    
-00018720: 2020 2020 2020 2020 6966 2073 7566 6669          if suffi
-00018730: 783a 0a20 2020 2020 2020 2020 2020 2020  x:.             
-00018740: 2020 2075 726c 203d 2066 2767 733a 2f2f     url = f'gs://
-00018750: 7b62 7563 6b65 745f 6e61 6d65 7d2f 7b73  {bucket_name}/{s
-00018760: 7566 6669 787d 270a 2020 2020 2020 2020  uffix}'.        
-00018770: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00018780: 2020 2020 2020 2020 2020 7572 6c20 3d20            url = 
-00018790: 6627 6773 3a2f 2f7b 6275 636b 6574 5f6e  f'gs://{bucket_n
-000187a0: 616d 657d 270a 2020 2020 2020 2020 2020  ame}'.          
-000187b0: 2020 7265 7475 726e 2066 2767 7375 7469    return f'gsuti
-000187c0: 6c20 6c73 207b 7572 6c7d 270a 2020 2020  l ls {url}'.    
-000187d0: 2020 2020 6966 2073 746f 7265 5f74 7970      if store_typ
-000187e0: 6520 3d3d 2073 746f 7261 6765 5f6c 6962  e == storage_lib
-000187f0: 2e53 746f 7265 5479 7065 2e52 323a 0a20  .StoreType.R2:. 
-00018800: 2020 2020 2020 2020 2020 2065 6e64 706f             endpo
-00018810: 696e 745f 7572 6c20 3d20 636c 6f75 6466  int_url = cloudf
-00018820: 6c61 7265 2e63 7265 6174 655f 656e 6470  lare.create_endp
-00018830: 6f69 6e74 2829 0a20 2020 2020 2020 2020  oint().         
-00018840: 2020 2069 6620 7375 6666 6978 3a0a 2020     if suffix:.  
-00018850: 2020 2020 2020 2020 2020 2020 2020 7572                ur
-00018860: 6c20 3d20 6627 7333 3a2f 2f7b 6275 636b  l = f's3://{buck
-00018870: 6574 5f6e 616d 657d 2f7b 7375 6666 6978  et_name}/{suffix
-00018880: 7d27 0a20 2020 2020 2020 2020 2020 2065  }'.            e
-00018890: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000188a0: 2020 2020 2075 726c 203d 2066 2773 333a       url = f's3:
-000188b0: 2f2f 7b62 7563 6b65 745f 6e61 6d65 7d27  //{bucket_name}'
-000188c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000188d0: 7572 6e20 6627 4157 535f 5348 4152 4544  urn f'AWS_SHARED
-000188e0: 5f43 5245 4445 4e54 4941 4c53 5f46 494c  _CREDENTIALS_FIL
-000188f0: 453d 7b63 6c6f 7564 666c 6172 652e 5232  E={cloudflare.R2
-00018900: 5f43 5245 4445 4e54 4941 4c53 5f50 4154  _CREDENTIALS_PAT
-00018910: 487d 2061 7773 2073 3320 6c73 207b 7572  H} aws s3 ls {ur
-00018920: 6c7d 202d 2d65 6e64 706f 696e 7420 7b65  l} --endpoint {e
-00018930: 6e64 706f 696e 745f 7572 6c7d 202d 2d70  ndpoint_url} --p
-00018940: 726f 6669 6c65 3d72 3227 0a0a 2020 2020  rofile=r2'..    
-00018950: 4070 7974 6573 742e 6669 7874 7572 650a  @pytest.fixture.
-00018960: 2020 2020 6465 6620 746d 705f 736f 7572      def tmp_sour
-00018970: 6365 2873 656c 662c 2074 6d70 5f70 6174  ce(self, tmp_pat
-00018980: 6829 3a0a 2020 2020 2020 2020 2320 4372  h):.        # Cr
-00018990: 6561 7465 7320 6120 7465 6d70 6f72 6172  eates a temporar
-000189a0: 7920 6469 7265 6374 6f72 7920 7769 7468  y directory with
-000189b0: 2061 2066 696c 6520 696e 2069 740a 2020   a file in it.  
-000189c0: 2020 2020 2020 746d 705f 6469 7220 3d20        tmp_dir = 
-000189d0: 746d 705f 7061 7468 202f 2027 746d 702d  tmp_path / 'tmp-
-000189e0: 736f 7572 6365 270a 2020 2020 2020 2020  source'.        
-000189f0: 746d 705f 6469 722e 6d6b 6469 7228 290a  tmp_dir.mkdir().
-00018a00: 2020 2020 2020 2020 746d 705f 6669 6c65          tmp_file
-00018a10: 203d 2074 6d70 5f64 6972 202f 2027 746d   = tmp_dir / 'tm
-00018a20: 702d 6669 6c65 270a 2020 2020 2020 2020  p-file'.        
-00018a30: 746d 705f 6669 6c65 2e77 7269 7465 5f74  tmp_file.write_t
-00018a40: 6578 7428 2774 6573 7427 290a 2020 2020  ext('test').    
-00018a50: 2020 2020 6369 7263 6c65 5f6c 696e 6b20      circle_link 
-00018a60: 3d20 746d 705f 6469 7220 2f20 2763 6972  = tmp_dir / 'cir
-00018a70: 636c 652d 6c69 6e6b 270a 2020 2020 2020  cle-link'.      
-00018a80: 2020 6369 7263 6c65 5f6c 696e 6b2e 7379    circle_link.sy
-00018a90: 6d6c 696e 6b5f 746f 2874 6d70 5f64 6972  mlink_to(tmp_dir
-00018aa0: 2c20 7461 7267 6574 5f69 735f 6469 7265  , target_is_dire
-00018ab0: 6374 6f72 793d 5472 7565 290a 2020 2020  ctory=True).    
-00018ac0: 2020 2020 7969 656c 6420 7374 7228 746d      yield str(tm
-00018ad0: 705f 6469 7229 0a0a 2020 2020 4070 7974  p_dir)..    @pyt
-00018ae0: 6573 742e 6669 7874 7572 650a 2020 2020  est.fixture.    
-00018af0: 6465 6620 746d 705f 6275 636b 6574 5f6e  def tmp_bucket_n
-00018b00: 616d 6528 7365 6c66 293a 0a20 2020 2020  ame(self):.     
-00018b10: 2020 2023 2043 7265 6174 6573 2061 2074     # Creates a t
-00018b20: 656d 706f 7261 7279 2062 7563 6b65 7420  emporary bucket 
-00018b30: 6e61 6d65 0a20 2020 2020 2020 2023 2074  name.        # t
-00018b40: 696d 652e 7469 6d65 2829 2072 6574 7572  ime.time() retur
-00018b50: 6e73 2076 6172 7969 6e67 2070 7265 6369  ns varying preci
-00018b60: 7369 6f6e 206f 6e20 6469 6666 6572 656e  sion on differen
-00018b70: 7420 7379 7374 656d 732c 2073 6f20 7765  t systems, so we
-00018b80: 0a20 2020 2020 2020 2023 2072 6570 6c61  .        # repla
-00018b90: 6365 2074 6865 2064 6563 696d 616c 2070  ce the decimal p
-00018ba0: 6f69 6e74 2061 6e64 2075 7365 2077 6861  oint and use wha
-00018bb0: 7465 7665 7220 7072 6563 6973 696f 6e20  tever precision 
-00018bc0: 7765 2063 616e 2067 6574 2e0a 2020 2020  we can get..    
-00018bd0: 2020 2020 7469 6d65 7374 616d 7020 3d20      timestamp = 
-00018be0: 7374 7228 7469 6d65 2e74 696d 6528 2929  str(time.time())
-00018bf0: 2e72 6570 6c61 6365 2827 2e27 2c20 2727  .replace('.', ''
-00018c00: 290a 2020 2020 2020 2020 7969 656c 6420  ).        yield 
-00018c10: 6627 736b 792d 7465 7374 2d7b 7469 6d65  f'sky-test-{time
-00018c20: 7374 616d 707d 270a 0a20 2020 2040 7374  stamp}'..    @st
-00018c30: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
-00018c40: 6566 2079 6965 6c64 5f73 746f 7261 6765  ef yield_storage
-00018c50: 5f6f 626a 6563 7428 0a20 2020 2020 2020  _object(.       
-00018c60: 2020 2020 206e 616d 653a 204f 7074 696f       name: Optio
-00018c70: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-00018c80: 0a20 2020 2020 2020 2020 2020 2073 6f75  .            sou
-00018c90: 7263 653a 204f 7074 696f 6e61 6c5b 7374  rce: Optional[st
-00018ca0: 6f72 6167 655f 6c69 622e 5061 7468 5d20  orage_lib.Path] 
-00018cb0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00018cc0: 2020 2020 7374 6f72 6573 3a20 4f70 7469      stores: Opti
-00018cd0: 6f6e 616c 5b44 6963 745b 7374 6f72 6167  onal[Dict[storag
-00018ce0: 655f 6c69 622e 5374 6f72 6554 7970 652c  e_lib.StoreType,
-00018cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d10: 2020 2073 746f 7261 6765 5f6c 6962 2e41     storage_lib.A
-00018d20: 6273 7472 6163 7453 746f 7265 5d5d 203d  bstractStore]] =
-00018d30: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00018d40: 2020 2070 6572 7369 7374 656e 743a 204f     persistent: O
-00018d50: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
-00018d60: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-00018d70: 2020 6d6f 6465 3a20 7374 6f72 6167 655f    mode: storage_
-00018d80: 6c69 622e 5374 6f72 6167 654d 6f64 6520  lib.StorageMode 
-00018d90: 3d20 7374 6f72 6167 655f 6c69 622e 5374  = storage_lib.St
-00018da0: 6f72 6167 654d 6f64 652e 4d4f 554e 5429  orageMode.MOUNT)
-00018db0: 3a0a 2020 2020 2020 2020 2320 4372 6561  :.        # Crea
-00018dc0: 7465 7320 6120 7465 6d70 6f72 6172 7920  tes a temporary 
-00018dd0: 7374 6f72 6167 6520 6f62 6a65 6374 2e20  storage object. 
-00018de0: 5374 6f72 6573 206d 7573 7420 6265 2061  Stores must be a
-00018df0: 6464 6564 2069 6e20 7468 6520 7465 7374  dded in the test
-00018e00: 2e0a 2020 2020 2020 2020 7374 6f72 6167  ..        storag
-00018e10: 655f 6f62 6a20 3d20 7374 6f72 6167 655f  e_obj = storage_
-00018e20: 6c69 622e 5374 6f72 6167 6528 6e61 6d65  lib.Storage(name
-00018e30: 3d6e 616d 652c 0a20 2020 2020 2020 2020  =name,.         
-00018e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e60: 2073 6f75 7263 653d 736f 7572 6365 2c0a   source=source,.
-00018e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c790: 6465 7320 3e20 3120 7965 740a 4070 7974  des > 1 yet.@pyt
+0000c7a0: 6573 742e 6d61 726b 2e73 6b69 7028 0a20  est.mark.skip(. 
+0000c7b0: 2020 2072 6561 736f 6e3d 0a20 2020 2027     reason=.    '
+0000c7c0: 5468 6520 7265 736e 6574 5f64 6973 7472  The resnet_distr
+0000c7d0: 6962 7574 6564 5f74 665f 6170 7020 6973  ibuted_tf_app is
+0000c7e0: 2066 6c61 6b79 2c20 6475 6520 746f 2069   flaky, due to i
+0000c7f0: 7420 6661 696c 696e 6720 746f 2064 6574  t failing to det
+0000c800: 6563 7420 4750 5573 2e27 290a 6465 6620  ect GPUs.').def 
+0000c810: 7465 7374 5f64 6973 7472 6962 7574 6564  test_distributed
+0000c820: 5f74 6628 6765 6e65 7269 635f 636c 6f75  _tf(generic_clou
+0000c830: 643a 2073 7472 293a 0a20 2020 206e 616d  d: str):.    nam
+0000c840: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
+0000c850: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
+0000c860: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
+0000c870: 2027 7265 736e 6574 5f64 6973 7472 6962   'resnet_distrib
+0000c880: 7574 6564 5f74 665f 6170 7027 2c0a 2020  uted_tf_app',.  
+0000c890: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+0000c8a0: 2020 2020 2320 4e4f 5445 3a20 7275 6e6e      # NOTE: runn
+0000c8b0: 696e 6720 6974 2074 7769 6365 2077 696c  ing it twice wil
+0000c8c0: 6c20 6861 6e67 2028 736f 6d65 7469 6d65  l hang (sometime
+0000c8d0: 733f 2920 2d20 616e 2061 7070 2d6c 6576  s?) - an app-lev
+0000c8e0: 656c 2062 7567 2e0a 2020 2020 2020 2020  el bug..        
+0000c8f0: 2020 2020 6627 7079 7468 6f6e 2065 7861      f'python exa
+0000c900: 6d70 6c65 732f 7265 736e 6574 5f64 6973  mples/resnet_dis
+0000c910: 7472 6962 7574 6564 5f74 665f 6170 702e  tributed_tf_app.
+0000c920: 7079 207b 6e61 6d65 7d20 7b67 656e 6572  py {name} {gener
+0000c930: 6963 5f63 6c6f 7564 7d27 2c0a 2020 2020  ic_cloud}',.    
+0000c940: 2020 2020 2020 2020 6627 736b 7920 6c6f          f'sky lo
+0000c950: 6773 207b 6e61 6d65 7d20 3120 2d2d 7374  gs {name} 1 --st
+0000c960: 6174 7573 272c 2020 2320 456e 7375 7265  atus',  # Ensure
+0000c970: 2074 6865 206a 6f62 2073 7563 6365 6564   the job succeed
+0000c980: 6564 2e0a 2020 2020 2020 2020 5d2c 0a20  ed..        ],. 
+0000c990: 2020 2020 2020 2066 2773 6b79 2064 6f77         f'sky dow
+0000c9a0: 6e20 2d79 207b 6e61 6d65 7d27 2c0a 2020  n -y {name}',.  
+0000c9b0: 2020 2020 2020 7469 6d65 6f75 743d 3235        timeout=25
+0000c9c0: 202a 2036 302c 2020 2320 3235 206d 696e   * 60,  # 25 min
+0000c9d0: 7320 2869 7420 7461 6b65 7320 6172 6f75  s (it takes arou
+0000c9e0: 6e64 207e 3139 206d 696e 7329 0a20 2020  nd ~19 mins).   
+0000c9f0: 2029 0a20 2020 2072 756e 5f6f 6e65 5f74   ).    run_one_t
+0000ca00: 6573 7428 7465 7374 290a 0a0a 2320 2d2d  est(test)...# --
+0000ca10: 2d2d 2d2d 2d2d 2d2d 2054 6573 7469 6e67  -------- Testing
+0000ca20: 2047 4350 2073 7461 7274 2061 6e64 2073   GCP start and s
+0000ca30: 746f 7020 696e 7374 616e 6365 7320 2d2d  top instances --
+0000ca40: 2d2d 2d2d 2d2d 2d2d 0a40 7079 7465 7374  --------.@pytest
+0000ca50: 2e6d 6172 6b2e 6763 700a 6465 6620 7465  .mark.gcp.def te
+0000ca60: 7374 5f67 6370 5f73 7461 7274 5f73 746f  st_gcp_start_sto
+0000ca70: 7028 293a 0a20 2020 206e 616d 6520 3d20  p():.    name = 
+0000ca80: 5f67 6574 5f63 6c75 7374 6572 5f6e 616d  _get_cluster_nam
+0000ca90: 6528 290a 2020 2020 7465 7374 203d 2054  e().    test = T
+0000caa0: 6573 7428 0a20 2020 2020 2020 2027 6763  est(.        'gc
+0000cab0: 702d 7374 6172 742d 7374 6f70 272c 0a20  p-start-stop',. 
+0000cac0: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+0000cad0: 2020 2020 2066 2773 6b79 206c 6175 6e63       f'sky launc
+0000cae0: 6820 2d79 202d 6320 7b6e 616d 657d 2065  h -y -c {name} e
+0000caf0: 7861 6d70 6c65 732f 6763 705f 7374 6172  xamples/gcp_star
+0000cb00: 745f 7374 6f70 2e79 616d 6c27 2c0a 2020  t_stop.yaml',.  
+0000cb10: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
+0000cb20: 6c6f 6773 207b 6e61 6d65 7d20 3120 2d2d  logs {name} 1 --
+0000cb30: 7374 6174 7573 272c 2020 2320 456e 7375  status',  # Ensu
+0000cb40: 7265 2074 6865 206a 6f62 2073 7563 6365  re the job succe
+0000cb50: 6564 6564 2e0a 2020 2020 2020 2020 2020  eded..          
+0000cb60: 2020 6627 736b 7920 6578 6563 207b 6e61    f'sky exec {na
+0000cb70: 6d65 7d20 6578 616d 706c 6573 2f67 6370  me} examples/gcp
+0000cb80: 5f73 7461 7274 5f73 746f 702e 7961 6d6c  _start_stop.yaml
+0000cb90: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+0000cba0: 2773 6b79 206c 6f67 7320 7b6e 616d 657d  'sky logs {name}
+0000cbb0: 2032 202d 2d73 7461 7475 7327 2c20 2023   2 --status',  #
+0000cbc0: 2045 6e73 7572 6520 7468 6520 6a6f 6220   Ensure the job 
+0000cbd0: 7375 6363 6565 6465 642e 0a20 2020 2020  succeeded..     
+0000cbe0: 2020 2020 2020 2066 2773 6b79 2065 7865         f'sky exe
+0000cbf0: 6320 7b6e 616d 657d 2022 7072 6c69 6d69  c {name} "prlimi
+0000cc00: 7420 2d6e 202d 2d70 6964 3d5c 2428 7067  t -n --pid=\$(pg
+0000cc10: 7265 7020 2d66 205c 2772 6179 6c65 742f  rep -f \'raylet/
+0000cc20: 7261 796c 6574 202d 2d72 6179 6c65 745f  raylet --raylet_
+0000cc30: 736f 636b 6574 5f6e 616d 655c 2729 207c  socket_name\') |
+0000cc40: 2067 7265 7020 5c27 225c 2731 3034 3835   grep \'"\'10485
+0000cc50: 3736 2031 3034 3835 3736 5c27 225c 2722  76 1048576\'"\'"
+0000cc60: 272c 2020 2320 456e 7375 7265 2074 6865  ',  # Ensure the
+0000cc70: 2072 6179 6c65 7420 7072 6f63 6573 7320   raylet process 
+0000cc80: 6861 7320 7468 6520 636f 7272 6563 7420  has the correct 
+0000cc90: 6669 6c65 2064 6573 6372 6970 746f 7220  file descriptor 
+0000cca0: 6c69 6d69 742e 0a20 2020 2020 2020 2020  limit..         
+0000ccb0: 2020 2066 2773 6b79 206c 6f67 7320 7b6e     f'sky logs {n
+0000ccc0: 616d 657d 2033 202d 2d73 7461 7475 7327  ame} 3 --status'
+0000ccd0: 2c20 2023 2045 6e73 7572 6520 7468 6520  ,  # Ensure the 
+0000cce0: 6a6f 6220 7375 6363 6565 6465 642e 0a20  job succeeded.. 
+0000ccf0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+0000cd00: 2073 746f 7020 2d79 207b 6e61 6d65 7d27   stop -y {name}'
+0000cd10: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+0000cd20: 736c 6565 7020 3230 272c 0a20 2020 2020  sleep 20',.     
+0000cd30: 2020 2020 2020 2066 2773 6b79 2073 7461         f'sky sta
+0000cd40: 7274 202d 7920 7b6e 616d 657d 202d 6920  rt -y {name} -i 
+0000cd50: 3127 2c0a 2020 2020 2020 2020 2020 2020  1',.            
+0000cd60: 6627 736b 7920 6578 6563 207b 6e61 6d65  f'sky exec {name
+0000cd70: 7d20 6578 616d 706c 6573 2f67 6370 5f73  } examples/gcp_s
+0000cd80: 7461 7274 5f73 746f 702e 7961 6d6c 272c  tart_stop.yaml',
+0000cd90: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+0000cda0: 6b79 206c 6f67 7320 7b6e 616d 657d 2034  ky logs {name} 4
+0000cdb0: 202d 2d73 7461 7475 7327 2c20 2023 2045   --status',  # E
+0000cdc0: 6e73 7572 6520 7468 6520 6a6f 6220 7375  nsure the job su
+0000cdd0: 6363 6565 6465 642e 0a20 2020 2020 2020  cceeded..       
+0000cde0: 2020 2020 2027 736c 6565 7020 3138 3027       'sleep 180'
+0000cdf0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+0000ce00: 736b 7920 7374 6174 7573 202d 7220 7b6e  sky status -r {n
+0000ce10: 616d 657d 207c 2067 7265 7020 2249 4e49  ame} | grep "INI
+0000ce20: 545c 7c53 544f 5050 4544 2227 2c0a 2020  T\|STOPPED"',.  
+0000ce30: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+0000ce40: 2066 2773 6b79 2064 6f77 6e20 2d79 207b   f'sky down -y {
+0000ce50: 6e61 6d65 7d27 2c0a 2020 2020 290a 2020  name}',.    ).  
+0000ce60: 2020 7275 6e5f 6f6e 655f 7465 7374 2874    run_one_test(t
+0000ce70: 6573 7429 0a0a 0a23 202d 2d2d 2d2d 2d2d  est)...# -------
+0000ce80: 2d2d 2d20 5465 7374 696e 6720 417a 7572  --- Testing Azur
+0000ce90: 6520 7374 6172 7420 616e 6420 7374 6f70  e start and stop
+0000cea0: 2069 6e73 7461 6e63 6573 202d 2d2d 2d2d   instances -----
+0000ceb0: 2d2d 2d2d 2d0a 4070 7974 6573 742e 6d61  -----.@pytest.ma
+0000cec0: 726b 2e61 7a75 7265 0a64 6566 2074 6573  rk.azure.def tes
+0000ced0: 745f 617a 7572 655f 7374 6172 745f 7374  t_azure_start_st
+0000cee0: 6f70 2829 3a0a 2020 2020 6e61 6d65 203d  op():.    name =
+0000cef0: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
+0000cf00: 6d65 2829 0a20 2020 2074 6573 7420 3d20  me().    test = 
+0000cf10: 5465 7374 280a 2020 2020 2020 2020 2761  Test(.        'a
+0000cf20: 7a75 7265 2d73 7461 7274 2d73 746f 7027  zure-start-stop'
+0000cf30: 2c0a 2020 2020 2020 2020 5b0a 2020 2020  ,.        [.    
+0000cf40: 2020 2020 2020 2020 6627 736b 7920 6c61          f'sky la
+0000cf50: 756e 6368 202d 7920 2d63 207b 6e61 6d65  unch -y -c {name
+0000cf60: 7d20 6578 616d 706c 6573 2f61 7a75 7265  } examples/azure
+0000cf70: 5f73 7461 7274 5f73 746f 702e 7961 6d6c  _start_stop.yaml
+0000cf80: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+0000cf90: 2773 6b79 2065 7865 6320 7b6e 616d 657d  'sky exec {name}
+0000cfa0: 2065 7861 6d70 6c65 732f 617a 7572 655f   examples/azure_
+0000cfb0: 7374 6172 745f 7374 6f70 2e79 616d 6c27  start_stop.yaml'
+0000cfc0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+0000cfd0: 736b 7920 6c6f 6773 207b 6e61 6d65 7d20  sky logs {name} 
+0000cfe0: 3120 2d2d 7374 6174 7573 272c 2020 2320  1 --status',  # 
+0000cff0: 456e 7375 7265 2074 6865 206a 6f62 2073  Ensure the job s
+0000d000: 7563 6365 6564 6564 2e0a 2020 2020 2020  ucceeded..      
+0000d010: 2020 2020 2020 6627 736b 7920 6578 6563        f'sky exec
+0000d020: 207b 6e61 6d65 7d20 2270 726c 696d 6974   {name} "prlimit
+0000d030: 202d 6e20 2d2d 7069 643d 5c24 2870 6772   -n --pid=\$(pgr
+0000d040: 6570 202d 6620 5c27 7261 796c 6574 2f72  ep -f \'raylet/r
+0000d050: 6179 6c65 7420 2d2d 7261 796c 6574 5f73  aylet --raylet_s
+0000d060: 6f63 6b65 745f 6e61 6d65 5c27 2920 7c20  ocket_name\') | 
+0000d070: 6772 6570 205c 2722 5c27 3130 3438 3537  grep \'"\'104857
+0000d080: 3620 3130 3438 3537 365c 2722 5c27 2227  6 1048576\'"\'"'
+0000d090: 2c20 2023 2045 6e73 7572 6520 7468 6520  ,  # Ensure the 
+0000d0a0: 7261 796c 6574 2070 726f 6365 7373 2068  raylet process h
+0000d0b0: 6173 2074 6865 2063 6f72 7265 6374 2066  as the correct f
+0000d0c0: 696c 6520 6465 7363 7269 7074 6f72 206c  ile descriptor l
+0000d0d0: 696d 6974 2e0a 2020 2020 2020 2020 2020  imit..          
+0000d0e0: 2020 6627 736b 7920 6c6f 6773 207b 6e61    f'sky logs {na
+0000d0f0: 6d65 7d20 3220 2d2d 7374 6174 7573 272c  me} 2 --status',
+0000d100: 2020 2320 456e 7375 7265 2074 6865 206a    # Ensure the j
+0000d110: 6f62 2073 7563 6365 6564 6564 2e0a 2020  ob succeeded..  
+0000d120: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
+0000d130: 7374 6f70 202d 7920 7b6e 616d 657d 272c  stop -y {name}',
+0000d140: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+0000d150: 6b79 2073 7461 7274 202d 7920 7b6e 616d  ky start -y {nam
+0000d160: 657d 202d 6920 3127 2c0a 2020 2020 2020  e} -i 1',.      
+0000d170: 2020 2020 2020 6627 736b 7920 6578 6563        f'sky exec
+0000d180: 207b 6e61 6d65 7d20 6578 616d 706c 6573   {name} examples
+0000d190: 2f61 7a75 7265 5f73 7461 7274 5f73 746f  /azure_start_sto
+0000d1a0: 702e 7961 6d6c 272c 0a20 2020 2020 2020  p.yaml',.       
+0000d1b0: 2020 2020 2066 2773 6b79 206c 6f67 7320       f'sky logs 
+0000d1c0: 7b6e 616d 657d 2033 202d 2d73 7461 7475  {name} 3 --statu
+0000d1d0: 7327 2c20 2023 2045 6e73 7572 6520 7468  s',  # Ensure th
+0000d1e0: 6520 6a6f 6220 7375 6363 6565 6465 642e  e job succeeded.
+0000d1f0: 0a20 2020 2020 2020 2020 2020 2027 736c  .            'sl
+0000d200: 6565 7020 3230 3027 2c0a 2020 2020 2020  eep 200',.      
+0000d210: 2020 2020 2020 6627 733d 2428 736b 7920        f's=$(sky 
+0000d220: 7374 6174 7573 202d 7220 7b6e 616d 657d  status -r {name}
+0000d230: 2920 2626 2065 6368 6f20 2473 2026 2620  ) && echo $s && 
+0000d240: 6563 686f 2024 7320 7c20 6772 6570 2022  echo $s | grep "
+0000d250: 494e 4954 5c7c 5354 4f50 5045 4422 270a  INIT\|STOPPED"'.
+0000d260: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+0000d270: 2020 2066 2773 6b79 2064 6f77 6e20 2d79     f'sky down -y
+0000d280: 207b 6e61 6d65 7d27 2c0a 2020 2020 2020   {name}',.      
+0000d290: 2020 7469 6d65 6f75 743d 3330 202a 2036    timeout=30 * 6
+0000d2a0: 302c 2020 2320 3330 206d 696e 730a 2020  0,  # 30 mins.  
+0000d2b0: 2020 290a 2020 2020 7275 6e5f 6f6e 655f    ).    run_one_
+0000d2c0: 7465 7374 2874 6573 7429 0a0a 0a23 202d  test(test)...# -
+0000d2d0: 2d2d 2d2d 2d2d 2d2d 2d20 5465 7374 696e  --------- Testin
+0000d2e0: 6720 4175 746f 7374 6f70 7069 6e67 202d  g Autostopping -
+0000d2f0: 2d2d 2d2d 2d2d 2d2d 2d0a 4070 7974 6573  ---------.@pytes
+0000d300: 742e 6d61 726b 2e6e 6f5f 6c61 6d62 6461  t.mark.no_lambda
+0000d310: 5f63 6c6f 7564 2020 2320 4c61 6d62 6461  _cloud  # Lambda
+0000d320: 2043 6c6f 7564 2064 6f65 7320 6e6f 7420   Cloud does not 
+0000d330: 7375 7070 6f72 7420 7374 6f70 7069 6e67  support stopping
+0000d340: 2069 6e73 7461 6e63 6573 0a40 7079 7465   instances.@pyte
+0000d350: 7374 2e6d 6172 6b2e 6e6f 5f69 626d 2020  st.mark.no_ibm  
+0000d360: 2320 4649 5828 4942 4d29 2073 706f 7261  # FIX(IBM) spora
+0000d370: 6469 6361 6c6c 7920 6661 696c 732c 2061  dically fails, a
+0000d380: 7320 7265 7374 6172 7465 6420 776f 726b  s restarted work
+0000d390: 6572 7320 7374 6179 2075 6e69 6e69 7469  ers stay uniniti
+0000d3a0: 616c 697a 6564 2069 6e64 6566 696e 6974  alized indefinit
+0000d3b0: 656c 790a 4070 7974 6573 742e 6d61 726b  ely.@pytest.mark
+0000d3c0: 2e6e 6f5f 7363 7020 2023 2053 4350 2064  .no_scp  # SCP d
+0000d3d0: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
+0000d3e0: 6e75 6d5f 6e6f 6465 7320 3e20 3120 7965  num_nodes > 1 ye
+0000d3f0: 740a 6465 6620 7465 7374 5f61 7574 6f73  t.def test_autos
+0000d400: 746f 7028 6765 6e65 7269 635f 636c 6f75  top(generic_clou
+0000d410: 643a 2073 7472 293a 0a20 2020 206e 616d  d: str):.    nam
+0000d420: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
+0000d430: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
+0000d440: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
+0000d450: 2027 6175 746f 7374 6f70 272c 0a20 2020   'autostop',.   
+0000d460: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+0000d470: 2020 2066 2773 6b79 206c 6175 6e63 6820     f'sky launch 
+0000d480: 2d79 202d 6420 2d63 207b 6e61 6d65 7d20  -y -d -c {name} 
+0000d490: 2d2d 6e75 6d2d 6e6f 6465 7320 3220 2d2d  --num-nodes 2 --
+0000d4a0: 636c 6f75 6420 7b67 656e 6572 6963 5f63  cloud {generic_c
+0000d4b0: 6c6f 7564 7d20 7465 7374 732f 7465 7374  loud} tests/test
+0000d4c0: 5f79 616d 6c73 2f6d 696e 696d 616c 2e79  _yamls/minimal.y
+0000d4d0: 616d 6c27 2c0a 2020 2020 2020 2020 2020  aml',.          
+0000d4e0: 2020 6627 736b 7920 6175 746f 7374 6f70    f'sky autostop
+0000d4f0: 202d 7920 7b6e 616d 657d 202d 6920 3127   -y {name} -i 1'
+0000d500: 2c0a 0a20 2020 2020 2020 2020 2020 2023  ,..            #
+0000d510: 2045 6e73 7572 6520 6175 746f 7374 6f70   Ensure autostop
+0000d520: 2069 7320 7365 742e 0a20 2020 2020 2020   is set..       
+0000d530: 2020 2020 2066 2773 6b79 2073 7461 7475       f'sky statu
+0000d540: 7320 7c20 6772 6570 207b 6e61 6d65 7d20  s | grep {name} 
+0000d550: 7c20 6772 6570 2022 316d 2227 2c0a 0a20  | grep "1m"',.. 
+0000d560: 2020 2020 2020 2020 2020 2023 2045 6e73             # Ens
+0000d570: 7572 6520 7468 6520 636c 7573 7465 7220  ure the cluster 
+0000d580: 6973 206e 6f74 2073 746f 7070 6564 2065  is not stopped e
+0000d590: 6172 6c79 2e0a 2020 2020 2020 2020 2020  arly..          
+0000d5a0: 2020 2773 6c65 6570 2034 3527 2c0a 2020    'sleep 45',.  
+0000d5b0: 2020 2020 2020 2020 2020 6627 733d 2428            f's=$(
+0000d5c0: 736b 7920 7374 6174 7573 207b 6e61 6d65  sky status {name
+0000d5d0: 7d20 2d2d 7265 6672 6573 6829 3b20 6563  } --refresh); ec
+0000d5e0: 686f 2022 2473 223b 2065 6368 6f3b 2065  ho "$s"; echo; e
+0000d5f0: 6368 6f3b 2065 6368 6f20 2224 7322 2020  cho; echo "$s"  
+0000d600: 7c20 6772 6570 207b 6e61 6d65 7d20 7c20  | grep {name} | 
+0000d610: 6772 6570 2055 5027 2c0a 0a20 2020 2020  grep UP',..     
+0000d620: 2020 2020 2020 2023 2045 6e73 7572 6520         # Ensure 
+0000d630: 7468 6520 636c 7573 7465 7220 6973 2053  the cluster is S
+0000d640: 544f 5050 4544 2e0a 2020 2020 2020 2020  TOPPED..        
+0000d650: 2020 2020 2773 6c65 6570 2032 3530 272c      'sleep 250',
+0000d660: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+0000d670: 3d24 2873 6b79 2073 7461 7475 7320 7b6e  =$(sky status {n
+0000d680: 616d 657d 202d 2d72 6566 7265 7368 293b  ame} --refresh);
+0000d690: 2065 6368 6f20 2224 7322 3b20 6563 686f   echo "$s"; echo
+0000d6a0: 3b20 6563 686f 3b20 6563 686f 2022 2473  ; echo; echo "$s
+0000d6b0: 2220 207c 2067 7265 7020 7b6e 616d 657d  "  | grep {name}
+0000d6c0: 207c 2067 7265 7020 5354 4f50 5045 4427   | grep STOPPED'
+0000d6d0: 2c0a 0a20 2020 2020 2020 2020 2020 2023  ,..            #
+0000d6e0: 2045 6e73 7572 6520 7468 6520 636c 7573   Ensure the clus
+0000d6f0: 7465 7220 6973 2055 5020 616e 6420 7468  ter is UP and th
+0000d700: 6520 6175 746f 7374 6f70 2073 6574 7469  e autostop setti
+0000d710: 6e67 2069 7320 7265 7365 7420 2827 2d27  ng is reset ('-'
+0000d720: 292e 0a20 2020 2020 2020 2020 2020 2066  )..            f
+0000d730: 2773 6b79 2073 7461 7274 202d 7920 7b6e  'sky start -y {n
+0000d740: 616d 657d 272c 0a20 2020 2020 2020 2020  ame}',.         
+0000d750: 2020 2066 2773 6b79 2073 7461 7475 7320     f'sky status 
+0000d760: 7c20 6772 6570 207b 6e61 6d65 7d20 7c20  | grep {name} | 
+0000d770: 6772 6570 202d 4520 2255 505c 732b 2d22  grep -E "UP\s+-"
+0000d780: 272c 0a0a 2020 2020 2020 2020 2020 2020  ',..            
+0000d790: 2320 456e 7375 7265 2074 6865 206a 6f62  # Ensure the job
+0000d7a0: 2073 7563 6365 6564 6564 2e0a 2020 2020   succeeded..    
+0000d7b0: 2020 2020 2020 2020 6627 736b 7920 6578          f'sky ex
+0000d7c0: 6563 207b 6e61 6d65 7d20 7465 7374 732f  ec {name} tests/
+0000d7d0: 7465 7374 5f79 616d 6c73 2f6d 696e 696d  test_yamls/minim
+0000d7e0: 616c 2e79 616d 6c27 2c0a 2020 2020 2020  al.yaml',.      
+0000d7f0: 2020 2020 2020 6627 736b 7920 6c6f 6773        f'sky logs
+0000d800: 207b 6e61 6d65 7d20 3220 2d2d 7374 6174   {name} 2 --stat
+0000d810: 7573 272c 0a0a 2020 2020 2020 2020 2020  us',..          
+0000d820: 2020 2320 5465 7374 2072 6573 7461 7274    # Test restart
+0000d830: 696e 6720 7468 6520 6964 6c65 6e65 7373  ing the idleness
+0000d840: 2074 696d 6572 2076 6961 2063 616e 6365   timer via cance
+0000d850: 6c20 2b20 7265 7365 743a 0a20 2020 2020  l + reset:.     
+0000d860: 2020 2020 2020 2066 2773 6b79 2061 7574         f'sky aut
+0000d870: 6f73 746f 7020 2d79 207b 6e61 6d65 7d20  ostop -y {name} 
+0000d880: 2d69 2031 272c 2020 2320 4964 6c65 6e65  -i 1',  # Idlene
+0000d890: 7373 2073 7461 7274 7320 636f 756e 7469  ss starts counti
+0000d8a0: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
+0000d8b0: 2773 6c65 6570 2034 3527 2c20 2023 2041  'sleep 45',  # A
+0000d8c0: 6c6d 6f73 7420 7265 6163 6865 6420 7468  lmost reached th
+0000d8d0: 6520 7468 7265 7368 6f6c 642e 0a20 2020  e threshold..   
+0000d8e0: 2020 2020 2020 2020 2066 2773 6b79 2061           f'sky a
+0000d8f0: 7574 6f73 746f 7020 2d79 207b 6e61 6d65  utostop -y {name
+0000d900: 7d20 2d2d 6361 6e63 656c 272c 0a20 2020  } --cancel',.   
+0000d910: 2020 2020 2020 2020 2066 2773 6b79 2061           f'sky a
+0000d920: 7574 6f73 746f 7020 2d79 207b 6e61 6d65  utostop -y {name
+0000d930: 7d20 2d69 2031 272c 2020 2320 5368 6f75  } -i 1',  # Shou
+0000d940: 6c64 2072 6573 7461 7274 2074 6865 2074  ld restart the t
+0000d950: 696d 6572 2e0a 2020 2020 2020 2020 2020  imer..          
+0000d960: 2020 2773 6c65 6570 2034 3527 2c0a 2020    'sleep 45',.  
+0000d970: 2020 2020 2020 2020 2020 6627 733d 2428            f's=$(
+0000d980: 736b 7920 7374 6174 7573 207b 6e61 6d65  sky status {name
+0000d990: 7d20 2d2d 7265 6672 6573 6829 3b20 6563  } --refresh); ec
+0000d9a0: 686f 2022 2473 223b 2065 6368 6f3b 2065  ho "$s"; echo; e
+0000d9b0: 6368 6f3b 2065 6368 6f20 2224 7322 207c  cho; echo "$s" |
+0000d9c0: 2067 7265 7020 7b6e 616d 657d 207c 2067   grep {name} | g
+0000d9d0: 7265 7020 5550 272c 0a20 2020 2020 2020  rep UP',.       
+0000d9e0: 2020 2020 2027 736c 6565 7020 3235 3027       'sleep 250'
+0000d9f0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+0000da00: 733d 2428 736b 7920 7374 6174 7573 207b  s=$(sky status {
+0000da10: 6e61 6d65 7d20 2d2d 7265 6672 6573 6829  name} --refresh)
+0000da20: 3b20 6563 686f 2022 2473 223b 2065 6368  ; echo "$s"; ech
+0000da30: 6f3b 2065 6368 6f3b 2065 6368 6f20 2224  o; echo; echo "$
+0000da40: 7322 2020 7c20 6772 6570 207b 6e61 6d65  s"  | grep {name
+0000da50: 7d20 7c20 6772 6570 2053 544f 5050 4544  } | grep STOPPED
+0000da60: 272c 0a0a 2020 2020 2020 2020 2020 2020  ',..            
+0000da70: 2320 5465 7374 2072 6573 7461 7274 696e  # Test restartin
+0000da80: 6720 7468 6520 6964 6c65 6e65 7373 2074  g the idleness t
+0000da90: 696d 6572 2076 6961 2065 7865 633a 0a20  imer via exec:. 
+0000daa0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+0000dab0: 2073 7461 7274 202d 7920 7b6e 616d 657d   start -y {name}
+0000dac0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+0000dad0: 2773 6b79 2073 7461 7475 7320 7c20 6772  'sky status | gr
+0000dae0: 6570 207b 6e61 6d65 7d20 7c20 6772 6570  ep {name} | grep
+0000daf0: 202d 4520 2255 505c 732b 2d22 272c 0a20   -E "UP\s+-"',. 
+0000db00: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+0000db10: 2061 7574 6f73 746f 7020 2d79 207b 6e61   autostop -y {na
+0000db20: 6d65 7d20 2d69 2031 272c 2020 2320 4964  me} -i 1',  # Id
+0000db30: 6c65 6e65 7373 2073 7461 7274 7320 636f  leness starts co
+0000db40: 756e 7469 6e67 2e0a 2020 2020 2020 2020  unting..        
+0000db50: 2020 2020 2773 6c65 6570 2034 3527 2c20      'sleep 45', 
+0000db60: 2023 2041 6c6d 6f73 7420 7265 6163 6865   # Almost reache
+0000db70: 6420 7468 6520 7468 7265 7368 6f6c 642e  d the threshold.
+0000db80: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+0000db90: 6b79 2065 7865 6320 7b6e 616d 657d 2065  ky exec {name} e
+0000dba0: 6368 6f20 6869 272c 2020 2320 5368 6f75  cho hi',  # Shou
+0000dbb0: 6c64 2072 6573 7461 7274 2074 6865 2074  ld restart the t
+0000dbc0: 696d 6572 2e0a 2020 2020 2020 2020 2020  imer..          
+0000dbd0: 2020 2773 6c65 6570 2034 3527 2c0a 2020    'sleep 45',.  
+0000dbe0: 2020 2020 2020 2020 2020 6627 733d 2428            f's=$(
+0000dbf0: 736b 7920 7374 6174 7573 207b 6e61 6d65  sky status {name
+0000dc00: 7d20 2d2d 7265 6672 6573 6829 3b20 6563  } --refresh); ec
+0000dc10: 686f 2022 2473 223b 2065 6368 6f3b 2065  ho "$s"; echo; e
+0000dc20: 6368 6f3b 2065 6368 6f20 2224 7322 2020  cho; echo "$s"  
+0000dc30: 7c20 6772 6570 207b 6e61 6d65 7d20 7c20  | grep {name} | 
+0000dc40: 6772 6570 2055 5027 2c0a 2020 2020 2020  grep UP',.      
+0000dc50: 2020 2020 2020 2773 6c65 6570 2032 3530        'sleep 250
+0000dc60: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+0000dc70: 2773 3d24 2873 6b79 2073 7461 7475 7320  's=$(sky status 
+0000dc80: 7b6e 616d 657d 202d 2d72 6566 7265 7368  {name} --refresh
+0000dc90: 293b 2065 6368 6f20 2224 7322 3b20 6563  ); echo "$s"; ec
+0000dca0: 686f 3b20 6563 686f 3b20 6563 686f 2022  ho; echo; echo "
+0000dcb0: 2473 2220 207c 2067 7265 7020 7b6e 616d  $s"  | grep {nam
+0000dcc0: 657d 207c 2067 7265 7020 5354 4f50 5045  e} | grep STOPPE
+0000dcd0: 4427 2c0a 2020 2020 2020 2020 5d2c 0a20  D',.        ],. 
+0000dce0: 2020 2020 2020 2066 2773 6b79 2064 6f77         f'sky dow
+0000dcf0: 6e20 2d79 207b 6e61 6d65 7d27 2c0a 2020  n -y {name}',.  
+0000dd00: 2020 2020 2020 7469 6d65 6f75 743d 3230        timeout=20
+0000dd10: 202a 2036 302c 0a20 2020 2029 0a20 2020   * 60,.    ).   
+0000dd20: 2072 756e 5f6f 6e65 5f74 6573 7428 7465   run_one_test(te
+0000dd30: 7374 290a 0a0a 2320 2d2d 2d2d 2d2d 2d2d  st)...# --------
+0000dd40: 2d2d 2054 6573 7469 6e67 2041 7574 6f64  -- Testing Autod
+0000dd50: 6f77 6e69 6e67 202d 2d2d 2d2d 2d2d 2d2d  owning ---------
+0000dd60: 2d0a 4070 7974 6573 742e 6d61 726b 2e6e  -.@pytest.mark.n
+0000dd70: 6f5f 7363 7020 2023 2053 4350 2064 6f65  o_scp  # SCP doe
+0000dd80: 7320 6e6f 7420 7375 7070 6f72 7420 6e75  s not support nu
+0000dd90: 6d5f 6e6f 6465 7320 3e20 3120 7965 742e  m_nodes > 1 yet.
+0000dda0: 2052 756e 2074 6573 745f 7363 705f 6175   Run test_scp_au
+0000ddb0: 746f 646f 776e 2069 6e73 7465 6164 2e0a  todown instead..
+0000ddc0: 6465 6620 7465 7374 5f61 7574 6f64 6f77  def test_autodow
+0000ddd0: 6e28 6765 6e65 7269 635f 636c 6f75 643a  n(generic_cloud:
+0000dde0: 2073 7472 293a 0a20 2020 206e 616d 6520   str):.    name 
+0000ddf0: 3d20 5f67 6574 5f63 6c75 7374 6572 5f6e  = _get_cluster_n
+0000de00: 616d 6528 290a 2020 2020 7465 7374 203d  ame().    test =
+0000de10: 2054 6573 7428 0a20 2020 2020 2020 2027   Test(.        '
+0000de20: 6175 746f 646f 776e 272c 0a20 2020 2020  autodown',.     
+0000de30: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+0000de40: 2066 2773 6b79 206c 6175 6e63 6820 2d79   f'sky launch -y
+0000de50: 202d 6420 2d63 207b 6e61 6d65 7d20 2d2d   -d -c {name} --
+0000de60: 6e75 6d2d 6e6f 6465 7320 3220 2d2d 636c  num-nodes 2 --cl
+0000de70: 6f75 6420 7b67 656e 6572 6963 5f63 6c6f  oud {generic_clo
+0000de80: 7564 7d20 7465 7374 732f 7465 7374 5f79  ud} tests/test_y
+0000de90: 616d 6c73 2f6d 696e 696d 616c 2e79 616d  amls/minimal.yam
+0000dea0: 6c27 2c0a 2020 2020 2020 2020 2020 2020  l',.            
+0000deb0: 6627 736b 7920 6175 746f 7374 6f70 202d  f'sky autostop -
+0000dec0: 7920 7b6e 616d 657d 202d 2d64 6f77 6e20  y {name} --down 
+0000ded0: 2d69 2031 272c 0a20 2020 2020 2020 2020  -i 1',.         
+0000dee0: 2020 2023 2045 6e73 7572 6520 6175 746f     # Ensure auto
+0000def0: 7374 6f70 2069 7320 7365 742e 0a20 2020  stop is set..   
+0000df00: 2020 2020 2020 2020 2066 2773 6b79 2073           f'sky s
+0000df10: 7461 7475 7320 7c20 6772 6570 207b 6e61  tatus | grep {na
+0000df20: 6d65 7d20 7c20 6772 6570 2022 316d 2028  me} | grep "1m (
+0000df30: 646f 776e 2922 272c 0a20 2020 2020 2020  down)"',.       
+0000df40: 2020 2020 2023 2045 6e73 7572 6520 7468       # Ensure th
+0000df50: 6520 636c 7573 7465 7220 6973 206e 6f74  e cluster is not
+0000df60: 2074 6572 6d69 6e61 7465 6420 6561 726c   terminated earl
+0000df70: 792e 0a20 2020 2020 2020 2020 2020 2027  y..            '
+0000df80: 736c 6565 7020 3435 272c 0a20 2020 2020  sleep 45',.     
+0000df90: 2020 2020 2020 2066 2773 3d24 2873 6b79         f's=$(sky
+0000dfa0: 2073 7461 7475 7320 7b6e 616d 657d 202d   status {name} -
+0000dfb0: 2d72 6566 7265 7368 293b 2065 6368 6f20  -refresh); echo 
+0000dfc0: 2224 7322 3b20 6563 686f 3b20 6563 686f  "$s"; echo; echo
+0000dfd0: 3b20 6563 686f 2022 2473 2220 207c 2067  ; echo "$s"  | g
+0000dfe0: 7265 7020 7b6e 616d 657d 207c 2067 7265  rep {name} | gre
+0000dff0: 7020 5550 272c 0a20 2020 2020 2020 2020  p UP',.         
+0000e000: 2020 2023 2045 6e73 7572 6520 7468 6520     # Ensure the 
+0000e010: 636c 7573 7465 7220 6973 2074 6572 6d69  cluster is termi
+0000e020: 6e61 7465 642e 0a20 2020 2020 2020 2020  nated..         
+0000e030: 2020 2027 736c 6565 7020 3230 3027 2c0a     'sleep 200',.
+0000e040: 2020 2020 2020 2020 2020 2020 6627 733d              f's=
+0000e050: 2428 534b 5950 494c 4f54 5f44 4542 5547  $(SKYPILOT_DEBUG
+0000e060: 3d30 2073 6b79 2073 7461 7475 7320 7b6e  =0 sky status {n
+0000e070: 616d 657d 202d 2d72 6566 7265 7368 2920  ame} --refresh) 
+0000e080: 2626 2065 6368 6f20 2224 7322 2026 2620  && echo "$s" && 
+0000e090: 7b7b 2065 6368 6f20 2224 7322 207c 2067  {{ echo "$s" | g
+0000e0a0: 7265 7020 7b6e 616d 657d 207c 2067 7265  rep {name} | gre
+0000e0b0: 7020 2241 7574 6f64 6f77 6e65 6420 636c  p "Autodowned cl
+0000e0c0: 7573 7465 725c 7c74 6572 6d69 6e61 7465  uster\|terminate
+0000e0d0: 6420 6f6e 2074 6865 2063 6c6f 7564 223b  d on the cloud";
+0000e0e0: 207d 7d20 7c7c 207b 7b20 6563 686f 2022   }} || {{ echo "
+0000e0f0: 2473 2220 7c20 6772 6570 207b 6e61 6d65  $s" | grep {name
+0000e100: 7d20 2626 2065 7869 7420 3120 7c7c 2065  } && exit 1 || e
+0000e110: 7869 7420 303b 207d 7d27 2c0a 2020 2020  xit 0; }}',.    
+0000e120: 2020 2020 2020 2020 6627 736b 7920 6c61          f'sky la
+0000e130: 756e 6368 202d 7920 2d64 202d 6320 7b6e  unch -y -d -c {n
+0000e140: 616d 657d 202d 2d63 6c6f 7564 207b 6765  ame} --cloud {ge
+0000e150: 6e65 7269 635f 636c 6f75 647d 202d 2d6e  neric_cloud} --n
+0000e160: 756d 2d6e 6f64 6573 2032 202d 2d64 6f77  um-nodes 2 --dow
+0000e170: 6e20 7465 7374 732f 7465 7374 5f79 616d  n tests/test_yam
+0000e180: 6c73 2f6d 696e 696d 616c 2e79 616d 6c27  ls/minimal.yaml'
+0000e190: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+0000e1a0: 736b 7920 7374 6174 7573 207c 2067 7265  sky status | gre
+0000e1b0: 7020 7b6e 616d 657d 207c 2067 7265 7020  p {name} | grep 
+0000e1c0: 5550 272c 2020 2320 456e 7375 7265 2074  UP',  # Ensure t
+0000e1d0: 6865 2063 6c75 7374 6572 2069 7320 5550  he cluster is UP
+0000e1e0: 2e0a 2020 2020 2020 2020 2020 2020 6627  ..            f'
+0000e1f0: 736b 7920 6578 6563 207b 6e61 6d65 7d20  sky exec {name} 
+0000e200: 2d2d 636c 6f75 6420 7b67 656e 6572 6963  --cloud {generic
+0000e210: 5f63 6c6f 7564 7d20 7465 7374 732f 7465  _cloud} tests/te
+0000e220: 7374 5f79 616d 6c73 2f6d 696e 696d 616c  st_yamls/minimal
+0000e230: 2e79 616d 6c27 2c0a 2020 2020 2020 2020  .yaml',.        
+0000e240: 2020 2020 6627 736b 7920 7374 6174 7573      f'sky status
+0000e250: 207c 2067 7265 7020 7b6e 616d 657d 207c   | grep {name} |
+0000e260: 2067 7265 7020 2231 6d20 2864 6f77 6e29   grep "1m (down)
+0000e270: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
+0000e280: 2773 6c65 6570 2032 3430 272c 0a20 2020  'sleep 240',.   
+0000e290: 2020 2020 2020 2020 2023 2045 6e73 7572           # Ensur
+0000e2a0: 6520 7468 6520 636c 7573 7465 7220 6973  e the cluster is
+0000e2b0: 2074 6572 6d69 6e61 7465 642e 0a20 2020   terminated..   
+0000e2c0: 2020 2020 2020 2020 2066 2773 3d24 2853           f's=$(S
+0000e2d0: 4b59 5049 4c4f 545f 4445 4255 473d 3020  KYPILOT_DEBUG=0 
+0000e2e0: 736b 7920 7374 6174 7573 207b 6e61 6d65  sky status {name
+0000e2f0: 7d20 2d2d 7265 6672 6573 6829 2026 2620  } --refresh) && 
+0000e300: 6563 686f 2022 2473 2220 2626 207b 7b20  echo "$s" && {{ 
+0000e310: 6563 686f 2022 2473 2220 7c20 6772 6570  echo "$s" | grep
+0000e320: 207b 6e61 6d65 7d20 7c20 6772 6570 2022   {name} | grep "
+0000e330: 4175 746f 646f 776e 6564 2063 6c75 7374  Autodowned clust
+0000e340: 6572 5c7c 7465 726d 696e 6174 6564 206f  er\|terminated o
+0000e350: 6e20 7468 6520 636c 6f75 6422 3b20 7d7d  n the cloud"; }}
+0000e360: 207c 7c20 7b7b 2065 6368 6f20 2224 7322   || {{ echo "$s"
+0000e370: 207c 2067 7265 7020 7b6e 616d 657d 2026   | grep {name} &
+0000e380: 2620 6578 6974 2031 207c 7c20 6578 6974  & exit 1 || exit
+0000e390: 2030 3b20 7d7d 272c 0a20 2020 2020 2020   0; }}',.       
+0000e3a0: 2020 2020 2066 2773 6b79 206c 6175 6e63       f'sky launc
+0000e3b0: 6820 2d79 202d 6420 2d63 207b 6e61 6d65  h -y -d -c {name
+0000e3c0: 7d20 2d2d 636c 6f75 6420 7b67 656e 6572  } --cloud {gener
+0000e3d0: 6963 5f63 6c6f 7564 7d20 2d2d 6e75 6d2d  ic_cloud} --num-
+0000e3e0: 6e6f 6465 7320 3220 2d2d 646f 776e 2074  nodes 2 --down t
+0000e3f0: 6573 7473 2f74 6573 745f 7961 6d6c 732f  ests/test_yamls/
+0000e400: 6d69 6e69 6d61 6c2e 7961 6d6c 272c 0a20  minimal.yaml',. 
+0000e410: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+0000e420: 2061 7574 6f73 746f 7020 2d79 207b 6e61   autostop -y {na
+0000e430: 6d65 7d20 2d2d 6361 6e63 656c 272c 0a20  me} --cancel',. 
+0000e440: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
+0000e450: 7020 3234 3027 2c0a 2020 2020 2020 2020  p 240',.        
+0000e460: 2020 2020 2320 456e 7375 7265 2074 6865      # Ensure the
+0000e470: 2063 6c75 7374 6572 2069 7320 7374 696c   cluster is stil
+0000e480: 6c20 5550 2e0a 2020 2020 2020 2020 2020  l UP..          
+0000e490: 2020 6627 733d 2428 534b 5950 494c 4f54    f's=$(SKYPILOT
+0000e4a0: 5f44 4542 5547 3d30 2073 6b79 2073 7461  _DEBUG=0 sky sta
+0000e4b0: 7475 7320 7b6e 616d 657d 202d 2d72 6566  tus {name} --ref
+0000e4c0: 7265 7368 2920 2626 2065 6368 6f20 2224  resh) && echo "$
+0000e4d0: 7322 2026 2620 6563 686f 2022 2473 2220  s" && echo "$s" 
+0000e4e0: 7c20 6772 6570 207b 6e61 6d65 7d20 7c20  | grep {name} | 
+0000e4f0: 6772 6570 2055 5027 2c0a 2020 2020 2020  grep UP',.      
+0000e500: 2020 5d2c 0a20 2020 2020 2020 2066 2773    ],.        f's
+0000e510: 6b79 2064 6f77 6e20 2d79 207b 6e61 6d65  ky down -y {name
+0000e520: 7d27 2c0a 2020 2020 2020 2020 7469 6d65  }',.        time
+0000e530: 6f75 743d 3230 202a 2036 302c 0a20 2020  out=20 * 60,.   
+0000e540: 2029 0a20 2020 2072 756e 5f6f 6e65 5f74   ).    run_one_t
+0000e550: 6573 7428 7465 7374 290a 0a0a 4070 7974  est(test)...@pyt
+0000e560: 6573 742e 6d61 726b 2e73 6370 0a64 6566  est.mark.scp.def
+0000e570: 2074 6573 745f 7363 705f 6175 746f 646f   test_scp_autodo
+0000e580: 776e 2829 3a0a 2020 2020 6e61 6d65 203d  wn():.    name =
+0000e590: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
+0000e5a0: 6d65 2829 0a20 2020 2074 6573 7420 3d20  me().    test = 
+0000e5b0: 5465 7374 280a 2020 2020 2020 2020 2753  Test(.        'S
+0000e5c0: 4350 5f61 7574 6f64 6f77 6e27 2c0a 2020  CP_autodown',.  
+0000e5d0: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+0000e5e0: 2020 2020 6627 736b 7920 6c61 756e 6368      f'sky launch
+0000e5f0: 202d 7920 2d64 202d 6320 7b6e 616d 657d   -y -d -c {name}
+0000e600: 207b 5343 505f 5459 5045 7d20 7465 7374   {SCP_TYPE} test
+0000e610: 732f 7465 7374 5f79 616d 6c73 2f6d 696e  s/test_yamls/min
+0000e620: 696d 616c 2e79 616d 6c27 2c0a 2020 2020  imal.yaml',.    
+0000e630: 2020 2020 2020 2020 6627 736b 7920 6175          f'sky au
+0000e640: 746f 7374 6f70 202d 7920 7b6e 616d 657d  tostop -y {name}
+0000e650: 202d 2d64 6f77 6e20 2d69 2031 272c 0a20   --down -i 1',. 
+0000e660: 2020 2020 2020 2020 2020 2023 2045 6e73             # Ens
+0000e670: 7572 6520 6175 746f 7374 6f70 2069 7320  ure autostop is 
+0000e680: 7365 742e 0a20 2020 2020 2020 2020 2020  set..           
+0000e690: 2066 2773 6b79 2073 7461 7475 7320 7c20   f'sky status | 
+0000e6a0: 6772 6570 207b 6e61 6d65 7d20 7c20 6772  grep {name} | gr
+0000e6b0: 6570 2022 316d 2028 646f 776e 2922 272c  ep "1m (down)"',
+0000e6c0: 0a20 2020 2020 2020 2020 2020 2023 2045  .            # E
+0000e6d0: 6e73 7572 6520 7468 6520 636c 7573 7465  nsure the cluste
+0000e6e0: 7220 6973 206e 6f74 2074 6572 6d69 6e61  r is not termina
+0000e6f0: 7465 6420 6561 726c 792e 0a20 2020 2020  ted early..     
+0000e700: 2020 2020 2020 2027 736c 6565 7020 3435         'sleep 45
+0000e710: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+0000e720: 2773 6b79 2073 7461 7475 7320 2d2d 7265  'sky status --re
+0000e730: 6672 6573 6820 7c20 6772 6570 207b 6e61  fresh | grep {na
+0000e740: 6d65 7d20 7c20 6772 6570 2055 5027 2c0a  me} | grep UP',.
+0000e750: 2020 2020 2020 2020 2020 2020 2320 456e              # En
+0000e760: 7375 7265 2074 6865 2063 6c75 7374 6572  sure the cluster
+0000e770: 2069 7320 7465 726d 696e 6174 6564 2e0a   is terminated..
+0000e780: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
+0000e790: 6570 2032 3030 272c 0a20 2020 2020 2020  ep 200',.       
+0000e7a0: 2020 2020 2066 2773 3d24 2853 4b59 5049       f's=$(SKYPI
+0000e7b0: 4c4f 545f 4445 4255 473d 3020 736b 7920  LOT_DEBUG=0 sky 
+0000e7c0: 7374 6174 7573 202d 2d72 6566 7265 7368  status --refresh
+0000e7d0: 2920 2626 2070 7269 6e74 6620 2224 7322  ) && printf "$s"
+0000e7e0: 2026 2620 7b7b 2065 6368 6f20 2224 7322   && {{ echo "$s"
+0000e7f0: 207c 2067 7265 7020 7b6e 616d 657d 207c   | grep {name} |
+0000e800: 2067 7265 7020 2241 7574 6f64 6f77 6e65   grep "Autodowne
+0000e810: 6420 636c 7573 7465 725c 7c74 6572 6d69  d cluster\|termi
+0000e820: 6e61 7465 6420 6f6e 2074 6865 2063 6c6f  nated on the clo
+0000e830: 7564 223b 207d 7d20 7c7c 207b 7b20 6563  ud"; }} || {{ ec
+0000e840: 686f 2022 2473 2220 7c20 6772 6570 207b  ho "$s" | grep {
+0000e850: 6e61 6d65 7d20 2626 2065 7869 7420 3120  name} && exit 1 
+0000e860: 7c7c 2065 7869 7420 303b 207d 7d27 2c0a  || exit 0; }}',.
+0000e870: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+0000e880: 7920 6c61 756e 6368 202d 7920 2d64 202d  y launch -y -d -
+0000e890: 6320 7b6e 616d 657d 207b 5343 505f 5459  c {name} {SCP_TY
+0000e8a0: 5045 7d20 2d2d 646f 776e 2074 6573 7473  PE} --down tests
+0000e8b0: 2f74 6573 745f 7961 6d6c 732f 6d69 6e69  /test_yamls/mini
+0000e8c0: 6d61 6c2e 7961 6d6c 272c 0a20 2020 2020  mal.yaml',.     
+0000e8d0: 2020 2020 2020 2066 2773 6b79 2073 7461         f'sky sta
+0000e8e0: 7475 7320 7c20 6772 6570 207b 6e61 6d65  tus | grep {name
+0000e8f0: 7d20 7c20 6772 6570 2055 5027 2c20 2023  } | grep UP',  #
+0000e900: 2045 6e73 7572 6520 7468 6520 636c 7573   Ensure the clus
+0000e910: 7465 7220 6973 2055 502e 0a20 2020 2020  ter is UP..     
+0000e920: 2020 2020 2020 2066 2773 6b79 2065 7865         f'sky exe
+0000e930: 6320 7b6e 616d 657d 207b 5343 505f 5459  c {name} {SCP_TY
+0000e940: 5045 7d20 7465 7374 732f 7465 7374 5f79  PE} tests/test_y
+0000e950: 616d 6c73 2f6d 696e 696d 616c 2e79 616d  amls/minimal.yam
+0000e960: 6c27 2c0a 2020 2020 2020 2020 2020 2020  l',.            
+0000e970: 6627 736b 7920 7374 6174 7573 207c 2067  f'sky status | g
+0000e980: 7265 7020 7b6e 616d 657d 207c 2067 7265  rep {name} | gre
+0000e990: 7020 2231 6d20 2864 6f77 6e29 2227 2c0a  p "1m (down)"',.
+0000e9a0: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
+0000e9b0: 6570 2032 3030 272c 0a20 2020 2020 2020  ep 200',.       
+0000e9c0: 2020 2020 2023 2045 6e73 7572 6520 7468       # Ensure th
+0000e9d0: 6520 636c 7573 7465 7220 6973 2074 6572  e cluster is ter
+0000e9e0: 6d69 6e61 7465 642e 0a20 2020 2020 2020  minated..       
+0000e9f0: 2020 2020 2066 2773 3d24 2853 4b59 5049       f's=$(SKYPI
+0000ea00: 4c4f 545f 4445 4255 473d 3020 736b 7920  LOT_DEBUG=0 sky 
+0000ea10: 7374 6174 7573 202d 2d72 6566 7265 7368  status --refresh
+0000ea20: 2920 2626 2070 7269 6e74 6620 2224 7322  ) && printf "$s"
+0000ea30: 2026 2620 7b7b 2065 6368 6f20 2224 7322   && {{ echo "$s"
+0000ea40: 207c 2067 7265 7020 7b6e 616d 657d 207c   | grep {name} |
+0000ea50: 2067 7265 7020 2241 7574 6f64 6f77 6e65   grep "Autodowne
+0000ea60: 6420 636c 7573 7465 725c 7c74 6572 6d69  d cluster\|termi
+0000ea70: 6e61 7465 6420 6f6e 2074 6865 2063 6c6f  nated on the clo
+0000ea80: 7564 223b 207d 7d20 7c7c 207b 7b20 6563  ud"; }} || {{ ec
+0000ea90: 686f 2022 2473 2220 7c20 6772 6570 207b  ho "$s" | grep {
+0000eaa0: 6e61 6d65 7d20 2626 2065 7869 7420 3120  name} && exit 1 
+0000eab0: 7c7c 2065 7869 7420 303b 207d 7d27 2c0a  || exit 0; }}',.
+0000eac0: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+0000ead0: 7920 6c61 756e 6368 202d 7920 2d64 202d  y launch -y -d -
+0000eae0: 6320 7b6e 616d 657d 207b 5343 505f 5459  c {name} {SCP_TY
+0000eaf0: 5045 7d20 2d2d 646f 776e 2074 6573 7473  PE} --down tests
+0000eb00: 2f74 6573 745f 7961 6d6c 732f 6d69 6e69  /test_yamls/mini
+0000eb10: 6d61 6c2e 7961 6d6c 272c 0a20 2020 2020  mal.yaml',.     
+0000eb20: 2020 2020 2020 2066 2773 6b79 2061 7574         f'sky aut
+0000eb30: 6f73 746f 7020 2d79 207b 6e61 6d65 7d20  ostop -y {name} 
+0000eb40: 2d2d 6361 6e63 656c 272c 0a20 2020 2020  --cancel',.     
+0000eb50: 2020 2020 2020 2027 736c 6565 7020 3230         'sleep 20
+0000eb60: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
+0000eb70: 2320 456e 7375 7265 2074 6865 2063 6c75  # Ensure the clu
+0000eb80: 7374 6572 2069 7320 7374 696c 6c20 5550  ster is still UP
+0000eb90: 2e0a 2020 2020 2020 2020 2020 2020 6627  ..            f'
+0000eba0: 733d 2428 534b 5950 494c 4f54 5f44 4542  s=$(SKYPILOT_DEB
+0000ebb0: 5547 3d30 2073 6b79 2073 7461 7475 7320  UG=0 sky status 
+0000ebc0: 2d2d 7265 6672 6573 6829 2026 2620 7072  --refresh) && pr
+0000ebd0: 696e 7466 2022 2473 2220 2626 2065 6368  intf "$s" && ech
+0000ebe0: 6f20 2224 7322 207c 2067 7265 7020 7b6e  o "$s" | grep {n
+0000ebf0: 616d 657d 207c 2067 7265 7020 5550 272c  ame} | grep UP',
+0000ec00: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
+0000ec10: 2020 2020 6627 736b 7920 646f 776e 202d      f'sky down -
+0000ec20: 7920 7b6e 616d 657d 272c 0a20 2020 2020  y {name}',.     
+0000ec30: 2020 2074 696d 656f 7574 3d32 3520 2a20     timeout=25 * 
+0000ec40: 3630 2c0a 2020 2020 290a 2020 2020 7275  60,.    ).    ru
+0000ec50: 6e5f 6f6e 655f 7465 7374 2874 6573 7429  n_one_test(test)
+0000ec60: 0a0a 0a64 6566 205f 6765 745f 6361 6e63  ...def _get_canc
+0000ec70: 656c 5f74 6173 6b5f 7769 7468 5f63 6c6f  el_task_with_clo
+0000ec80: 7564 286e 616d 652c 2063 6c6f 7564 2c20  ud(name, cloud, 
+0000ec90: 7469 6d65 6f75 743d 3135 202a 2036 3029  timeout=15 * 60)
+0000eca0: 3a0a 2020 2020 7465 7374 203d 2054 6573  :.    test = Tes
+0000ecb0: 7428 0a20 2020 2020 2020 2066 277b 636c  t(.        f'{cl
+0000ecc0: 6f75 647d 2d63 616e 6365 6c2d 7461 736b  oud}-cancel-task
+0000ecd0: 272c 0a20 2020 2020 2020 205b 0a20 2020  ',.        [.   
+0000ece0: 2020 2020 2020 2020 2066 2773 6b79 206c           f'sky l
+0000ecf0: 6175 6e63 6820 2d63 207b 6e61 6d65 7d20  aunch -c {name} 
+0000ed00: 6578 616d 706c 6573 2f72 6573 6e65 745f  examples/resnet_
+0000ed10: 6170 702e 7961 6d6c 202d 2d63 6c6f 7564  app.yaml --cloud
+0000ed20: 207b 636c 6f75 647d 202d 7920 2d64 272c   {cloud} -y -d',
+0000ed30: 0a20 2020 2020 2020 2020 2020 2023 2057  .            # W
+0000ed40: 6169 7420 7468 6520 4750 5520 7072 6f63  ait the GPU proc
+0000ed50: 6573 7320 746f 2073 7461 7274 2e0a 2020  ess to start..  
+0000ed60: 2020 2020 2020 2020 2020 2773 6c65 6570            'sleep
+0000ed70: 2036 3027 2c0a 2020 2020 2020 2020 2020   60',.          
+0000ed80: 2020 6627 736b 7920 6578 6563 207b 6e61    f'sky exec {na
+0000ed90: 6d65 7d20 226e 7669 6469 612d 736d 6920  me} "nvidia-smi 
+0000eda0: 7c20 6772 6570 2070 7974 686f 6e22 272c  | grep python"',
+0000edb0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+0000edc0: 6b79 206c 6f67 7320 7b6e 616d 657d 2032  ky logs {name} 2
+0000edd0: 202d 2d73 7461 7475 7327 2c20 2023 2045   --status',  # E
+0000ede0: 6e73 7572 6520 7468 6520 6a6f 6220 7375  nsure the job su
+0000edf0: 6363 6565 6465 642e 0a20 2020 2020 2020  cceeded..       
+0000ee00: 2020 2020 2066 2773 6b79 2063 616e 6365       f'sky cance
+0000ee10: 6c20 2d79 207b 6e61 6d65 7d20 3127 2c0a  l -y {name} 1',.
+0000ee20: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
+0000ee30: 6570 2036 3027 2c0a 2020 2020 2020 2020  ep 60',.        
+0000ee40: 2020 2020 2320 6368 6563 6b20 6966 2074      # check if t
+0000ee50: 6865 2070 7974 686f 6e20 6a6f 6220 6973  he python job is
+0000ee60: 2067 6f6e 652e 0a20 2020 2020 2020 2020   gone..         
+0000ee70: 2020 2066 2773 6b79 2065 7865 6320 7b6e     f'sky exec {n
+0000ee80: 616d 657d 2022 2120 6e76 6964 6961 2d73  ame} "! nvidia-s
+0000ee90: 6d69 207c 2067 7265 7020 7079 7468 6f6e  mi | grep python
+0000eea0: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
+0000eeb0: 6627 736b 7920 6c6f 6773 207b 6e61 6d65  f'sky logs {name
+0000eec0: 7d20 3320 2d2d 7374 6174 7573 272c 2020  } 3 --status',  
+0000eed0: 2320 456e 7375 7265 2074 6865 206a 6f62  # Ensure the job
+0000eee0: 2073 7563 6365 6564 6564 2e0a 2020 2020   succeeded..    
+0000eef0: 2020 2020 5d2c 0a20 2020 2020 2020 2066      ],.        f
+0000ef00: 2773 6b79 2064 6f77 6e20 2d79 207b 6e61  'sky down -y {na
+0000ef10: 6d65 7d27 2c0a 2020 2020 2020 2020 7469  me}',.        ti
+0000ef20: 6d65 6f75 743d 7469 6d65 6f75 742c 0a20  meout=timeout,. 
+0000ef30: 2020 2029 0a20 2020 2072 6574 7572 6e20     ).    return 
+0000ef40: 7465 7374 0a0a 0a23 202d 2d2d 2d2d 2d2d  test...# -------
+0000ef50: 2d2d 2d20 5465 7374 696e 6720 6073 6b79  --- Testing `sky
+0000ef60: 2063 616e 6365 6c60 202d 2d2d 2d2d 2d2d   cancel` -------
+0000ef70: 2d2d 2d0a 4070 7974 6573 742e 6d61 726b  ---.@pytest.mark
+0000ef80: 2e61 7773 0a40 7079 7465 7374 2e6d 6172  .aws.@pytest.mar
+0000ef90: 6b2e 736b 6970 280a 2020 2020 7265 6173  k.skip(.    reas
+0000efa0: 6f6e 3d27 5468 6520 7265 736e 6574 5f61  on='The resnet_a
+0000efb0: 7070 2069 7320 666c 616b 792c 2064 7565  pp is flaky, due
+0000efc0: 2074 6f20 5446 2066 6169 6c69 6e67 2074   to TF failing t
+0000efd0: 6f20 6465 7465 6374 2047 5055 732e 2729  o detect GPUs.')
+0000efe0: 0a64 6566 2074 6573 745f 6361 6e63 656c  .def test_cancel
+0000eff0: 5f61 7773 2829 3a0a 2020 2020 6e61 6d65  _aws():.    name
+0000f000: 203d 205f 6765 745f 636c 7573 7465 725f   = _get_cluster_
+0000f010: 6e61 6d65 2829 0a20 2020 2074 6573 7420  name().    test 
+0000f020: 3d20 5f67 6574 5f63 616e 6365 6c5f 7461  = _get_cancel_ta
+0000f030: 736b 5f77 6974 685f 636c 6f75 6428 6e61  sk_with_cloud(na
+0000f040: 6d65 2c20 2761 7773 2729 0a20 2020 2072  me, 'aws').    r
+0000f050: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
+0000f060: 290a 0a0a 4070 7974 6573 742e 6d61 726b  )...@pytest.mark
+0000f070: 2e67 6370 0a40 7079 7465 7374 2e6d 6172  .gcp.@pytest.mar
+0000f080: 6b2e 736b 6970 280a 2020 2020 7265 6173  k.skip(.    reas
+0000f090: 6f6e 3d27 5468 6520 7265 736e 6574 5f61  on='The resnet_a
+0000f0a0: 7070 2069 7320 666c 616b 792c 2064 7565  pp is flaky, due
+0000f0b0: 2074 6f20 5446 2066 6169 6c69 6e67 2074   to TF failing t
+0000f0c0: 6f20 6465 7465 6374 2047 5055 732e 2729  o detect GPUs.')
+0000f0d0: 0a64 6566 2074 6573 745f 6361 6e63 656c  .def test_cancel
+0000f0e0: 5f67 6370 2829 3a0a 2020 2020 6e61 6d65  _gcp():.    name
+0000f0f0: 203d 205f 6765 745f 636c 7573 7465 725f   = _get_cluster_
+0000f100: 6e61 6d65 2829 0a20 2020 2074 6573 7420  name().    test 
+0000f110: 3d20 5f67 6574 5f63 616e 6365 6c5f 7461  = _get_cancel_ta
+0000f120: 736b 5f77 6974 685f 636c 6f75 6428 6e61  sk_with_cloud(na
+0000f130: 6d65 2c20 2767 6370 2729 0a20 2020 2072  me, 'gcp').    r
+0000f140: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
+0000f150: 290a 0a0a 4070 7974 6573 742e 6d61 726b  )...@pytest.mark
+0000f160: 2e61 7a75 7265 0a40 7079 7465 7374 2e6d  .azure.@pytest.m
+0000f170: 6172 6b2e 736b 6970 280a 2020 2020 7265  ark.skip(.    re
+0000f180: 6173 6f6e 3d27 5468 6520 7265 736e 6574  ason='The resnet
+0000f190: 5f61 7070 2069 7320 666c 616b 792c 2064  _app is flaky, d
+0000f1a0: 7565 2074 6f20 5446 2066 6169 6c69 6e67  ue to TF failing
+0000f1b0: 2074 6f20 6465 7465 6374 2047 5055 732e   to detect GPUs.
+0000f1c0: 2729 0a64 6566 2074 6573 745f 6361 6e63  ').def test_canc
+0000f1d0: 656c 5f61 7a75 7265 2829 3a0a 2020 2020  el_azure():.    
+0000f1e0: 6e61 6d65 203d 205f 6765 745f 636c 7573  name = _get_clus
+0000f1f0: 7465 725f 6e61 6d65 2829 0a20 2020 2074  ter_name().    t
+0000f200: 6573 7420 3d20 5f67 6574 5f63 616e 6365  est = _get_cance
+0000f210: 6c5f 7461 736b 5f77 6974 685f 636c 6f75  l_task_with_clou
+0000f220: 6428 6e61 6d65 2c20 2761 7a75 7265 272c  d(name, 'azure',
+0000f230: 2074 696d 656f 7574 3d33 3020 2a20 3630   timeout=30 * 60
+0000f240: 290a 2020 2020 7275 6e5f 6f6e 655f 7465  ).    run_one_te
+0000f250: 7374 2874 6573 7429 0a0a 0a40 7079 7465  st(test)...@pyte
+0000f260: 7374 2e6d 6172 6b2e 6e6f 5f6c 616d 6264  st.mark.no_lambd
+0000f270: 615f 636c 6f75 6420 2023 204c 616d 6264  a_cloud  # Lambd
+0000f280: 6120 436c 6f75 6420 646f 6573 206e 6f74  a Cloud does not
+0000f290: 2068 6176 6520 5631 3030 2067 7075 730a   have V100 gpus.
+0000f2a0: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
+0000f2b0: 6962 6d20 2023 2049 424d 2063 6c6f 7564  ibm  # IBM cloud
+0000f2c0: 2063 7572 7265 6e74 6c79 2064 6f65 736e   currently doesn
+0000f2d0: 2774 2070 726f 7669 6465 2070 7562 6c69  't provide publi
+0000f2e0: 6320 696d 6167 6520 7769 7468 2043 5544  c image with CUD
+0000f2f0: 410a 4070 7974 6573 742e 6d61 726b 2e6e  A.@pytest.mark.n
+0000f300: 6f5f 7363 7020 2023 2053 4350 2064 6f65  o_scp  # SCP doe
+0000f310: 7320 6e6f 7420 7375 7070 6f72 7420 6e75  s not support nu
+0000f320: 6d5f 6e6f 6465 7320 3e20 3120 7965 740a  m_nodes > 1 yet.
+0000f330: 6465 6620 7465 7374 5f63 616e 6365 6c5f  def test_cancel_
+0000f340: 7079 746f 7263 6828 6765 6e65 7269 635f  pytorch(generic_
+0000f350: 636c 6f75 643a 2073 7472 293a 0a20 2020  cloud: str):.   
+0000f360: 206e 616d 6520 3d20 5f67 6574 5f63 6c75   name = _get_clu
+0000f370: 7374 6572 5f6e 616d 6528 290a 2020 2020  ster_name().    
+0000f380: 7465 7374 203d 2054 6573 7428 0a20 2020  test = Test(.   
+0000f390: 2020 2020 2027 6361 6e63 656c 2d70 7974       'cancel-pyt
+0000f3a0: 6f72 6368 272c 0a20 2020 2020 2020 205b  orch',.        [
+0000f3b0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+0000f3c0: 6b79 206c 6175 6e63 6820 2d63 207b 6e61  ky launch -c {na
+0000f3d0: 6d65 7d20 2d2d 636c 6f75 6420 7b67 656e  me} --cloud {gen
+0000f3e0: 6572 6963 5f63 6c6f 7564 7d20 6578 616d  eric_cloud} exam
+0000f3f0: 706c 6573 2f72 6573 6e65 745f 6469 7374  ples/resnet_dist
+0000f400: 7269 6275 7465 645f 746f 7263 682e 7961  ributed_torch.ya
+0000f410: 6d6c 202d 7920 2d64 272c 0a20 2020 2020  ml -y -d',.     
+0000f420: 2020 2020 2020 2023 2057 6169 7420 7468         # Wait th
+0000f430: 6520 4750 5520 7072 6f63 6573 7320 746f  e GPU process to
+0000f440: 2073 7461 7274 2e0a 2020 2020 2020 2020   start..        
+0000f450: 2020 2020 2773 6c65 6570 2039 3027 2c0a      'sleep 90',.
+0000f460: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+0000f470: 7920 6578 6563 207b 6e61 6d65 7d20 226e  y exec {name} "n
+0000f480: 7669 6469 612d 736d 6920 7c20 6772 6570  vidia-smi | grep
+0000f490: 2070 7974 686f 6e22 272c 0a20 2020 2020   python"',.     
+0000f4a0: 2020 2020 2020 2066 2773 6b79 206c 6f67         f'sky log
+0000f4b0: 7320 7b6e 616d 657d 2032 202d 2d73 7461  s {name} 2 --sta
+0000f4c0: 7475 7327 2c20 2023 2045 6e73 7572 6520  tus',  # Ensure 
+0000f4d0: 7468 6520 6a6f 6220 7375 6363 6565 6465  the job succeede
+0000f4e0: 642e 0a20 2020 2020 2020 2020 2020 2066  d..            f
+0000f4f0: 2773 6b79 2063 616e 6365 6c20 2d79 207b  'sky cancel -y {
+0000f500: 6e61 6d65 7d20 3127 2c0a 2020 2020 2020  name} 1',.      
+0000f510: 2020 2020 2020 2773 6c65 6570 2036 3027        'sleep 60'
+0000f520: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+0000f530: 736b 7920 6578 6563 207b 6e61 6d65 7d20  sky exec {name} 
+0000f540: 2228 6e76 6964 6961 2d73 6d69 207c 2067  "(nvidia-smi | g
+0000f550: 7265 7020 5c27 4e6f 2072 756e 6e69 6e67  rep \'No running
+0000f560: 2070 726f 6365 7373 5c27 2920 7c7c 2027   process\') || '
+0000f570: 0a20 2020 2020 2020 2020 2020 2023 2045  .            # E
+0000f580: 6e73 7572 6520 586f 7267 2069 7320 7468  nsure Xorg is th
+0000f590: 6520 6f6e 6c79 2070 726f 6365 7373 2072  e only process r
+0000f5a0: 756e 6e69 6e67 2e0a 2020 2020 2020 2020  unning..        
+0000f5b0: 2020 2020 275b 205c 2428 6e76 6964 6961      '[ \$(nvidia
+0000f5c0: 2d73 6d69 207c 2067 7265 7020 2d41 2031  -smi | grep -A 1
+0000f5d0: 3020 5072 6f63 6573 7365 7320 7c20 6772  0 Processes | gr
+0000f5e0: 6570 202d 4120 3130 203d 3d3d 207c 2067  ep -A 10 === | g
+0000f5f0: 7265 7020 2d76 2058 6f72 6729 202d 6571  rep -v Xorg) -eq
+0000f600: 2032 205d 2227 2c0a 2020 2020 2020 2020   2 ]"',.        
+0000f610: 2020 2020 6627 736b 7920 6c6f 6773 207b      f'sky logs {
+0000f620: 6e61 6d65 7d20 3320 2d2d 7374 6174 7573  name} 3 --status
+0000f630: 272c 2020 2320 456e 7375 7265 2074 6865  ',  # Ensure the
+0000f640: 206a 6f62 2073 7563 6365 6564 6564 2e0a   job succeeded..
+0000f650: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+0000f660: 2020 2066 2773 6b79 2064 6f77 6e20 2d79     f'sky down -y
+0000f670: 207b 6e61 6d65 7d27 2c0a 2020 2020 2020   {name}',.      
+0000f680: 2020 7469 6d65 6f75 743d 3230 202a 2036    timeout=20 * 6
+0000f690: 302c 0a20 2020 2029 0a20 2020 2072 756e  0,.    ).    run
+0000f6a0: 5f6f 6e65 5f74 6573 7428 7465 7374 290a  _one_test(test).
+0000f6b0: 0a0a 2320 6361 6e27 7420 7573 6520 605f  ..# can't use `_
+0000f6c0: 6765 745f 6361 6e63 656c 5f74 6173 6b5f  get_cancel_task_
+0000f6d0: 7769 7468 5f63 6c6f 7564 2829 602c 2061  with_cloud()`, a
+0000f6e0: 7320 636f 6d6d 616e 6420 606e 7669 6469  s command `nvidi
+0000f6f0: 612d 736d 6960 0a23 2072 6571 7569 7265  a-smi`.# require
+0000f700: 7320 6120 4355 4441 2070 7562 6c69 6320  s a CUDA public 
+0000f710: 696d 6167 652c 2077 6869 6368 2049 424d  image, which IBM
+0000f720: 2064 6f65 736e 2774 206f 6666 6572 0a40   doesn't offer.@
+0000f730: 7079 7465 7374 2e6d 6172 6b2e 6962 6d0a  pytest.mark.ibm.
+0000f740: 6465 6620 7465 7374 5f63 616e 6365 6c5f  def test_cancel_
+0000f750: 6962 6d28 293a 0a20 2020 206e 616d 6520  ibm():.    name 
+0000f760: 3d20 5f67 6574 5f63 6c75 7374 6572 5f6e  = _get_cluster_n
+0000f770: 616d 6528 290a 2020 2020 7465 7374 203d  ame().    test =
+0000f780: 2054 6573 7428 0a20 2020 2020 2020 2027   Test(.        '
+0000f790: 6962 6d2d 6361 6e63 656c 2d74 6173 6b27  ibm-cancel-task'
+0000f7a0: 2c0a 2020 2020 2020 2020 5b0a 2020 2020  ,.        [.    
+0000f7b0: 2020 2020 2020 2020 6627 736b 7920 6c61          f'sky la
+0000f7c0: 756e 6368 202d 7920 2d63 207b 6e61 6d65  unch -y -c {name
+0000f7d0: 7d20 2d2d 636c 6f75 6420 6962 6d20 6578  } --cloud ibm ex
+0000f7e0: 616d 706c 6573 2f6d 696e 696d 616c 2e79  amples/minimal.y
+0000f7f0: 616d 6c27 2c0a 2020 2020 2020 2020 2020  aml',.          
+0000f800: 2020 6627 736b 7920 6578 6563 207b 6e61    f'sky exec {na
+0000f810: 6d65 7d20 2d6e 207b 6e61 6d65 7d2d 3120  me} -n {name}-1 
+0000f820: 2d64 2020 2277 6869 6c65 2074 7275 653b  -d  "while true;
+0000f830: 2064 6f20 6563 686f 205c 2748 656c 6c6f   do echo \'Hello
+0000f840: 2053 6b79 5069 6c6f 745c 273b 2073 6c65   SkyPilot\'; sle
+0000f850: 6570 2032 3b20 646f 6e65 2227 2c0a 2020  ep 2; done"',.  
+0000f860: 2020 2020 2020 2020 2020 2773 6c65 6570            'sleep
+0000f870: 2032 3027 2c0a 2020 2020 2020 2020 2020   20',.          
+0000f880: 2020 6627 736b 7920 7175 6575 6520 7b6e    f'sky queue {n
+0000f890: 616d 657d 207c 2067 7265 7020 7b6e 616d  ame} | grep {nam
+0000f8a0: 657d 2d31 207c 2067 7265 7020 5255 4e4e  e}-1 | grep RUNN
+0000f8b0: 494e 4727 2c0a 2020 2020 2020 2020 2020  ING',.          
+0000f8c0: 2020 6627 736b 7920 6361 6e63 656c 202d    f'sky cancel -
+0000f8d0: 7920 7b6e 616d 657d 2032 272c 0a20 2020  y {name} 2',.   
+0000f8e0: 2020 2020 2020 2020 2066 2773 6c65 6570           f'sleep
+0000f8f0: 2035 272c 0a20 2020 2020 2020 2020 2020   5',.           
+0000f900: 2066 2773 6b79 2071 7565 7565 207b 6e61   f'sky queue {na
+0000f910: 6d65 7d20 7c20 6772 6570 207b 6e61 6d65  me} | grep {name
+0000f920: 7d2d 3120 7c20 6772 6570 2043 414e 4345  }-1 | grep CANCE
+0000f930: 4c4c 4544 272c 0a20 2020 2020 2020 205d  LLED',.        ]
+0000f940: 2c0a 2020 2020 2020 2020 6627 736b 7920  ,.        f'sky 
+0000f950: 646f 776e 202d 7920 7b6e 616d 657d 272c  down -y {name}',
+0000f960: 0a20 2020 2029 0a20 2020 2072 756e 5f6f  .    ).    run_o
+0000f970: 6e65 5f74 6573 7428 7465 7374 290a 0a0a  ne_test(test)...
+0000f980: 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2054 6573  # ---------- Tes
+0000f990: 7469 6e67 2075 7365 2d73 706f 7420 6f70  ting use-spot op
+0000f9a0: 7469 6f6e 202d 2d2d 2d2d 2d2d 2d2d 2d0a  tion ----------.
+0000f9b0: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
+0000f9c0: 6c61 6d62 6461 5f63 6c6f 7564 2020 2320  lambda_cloud  # 
+0000f9d0: 4c61 6d62 6461 2043 6c6f 7564 2064 6f65  Lambda Cloud doe
+0000f9e0: 7320 6e6f 7420 7375 7070 6f72 7420 7370  s not support sp
+0000f9f0: 6f74 2069 6e73 7461 6e63 6573 0a40 7079  ot instances.@py
+0000fa00: 7465 7374 2e6d 6172 6b2e 6e6f 5f69 626d  test.mark.no_ibm
+0000fa10: 2020 2320 4942 4d20 436c 6f75 6420 646f    # IBM Cloud do
+0000fa20: 6573 206e 6f74 2073 7570 706f 7274 2073  es not support s
+0000fa30: 706f 7420 696e 7374 616e 6365 730a 4070  pot instances.@p
+0000fa40: 7974 6573 742e 6d61 726b 2e6e 6f5f 7363  ytest.mark.no_sc
+0000fa50: 7020 2023 2053 4350 2064 6f65 7320 6e6f  p  # SCP does no
+0000fa60: 7420 7375 7070 6f72 7420 7370 6f74 2069  t support spot i
+0000fa70: 6e73 7461 6e63 6573 0a64 6566 2074 6573  nstances.def tes
+0000fa80: 745f 7573 655f 7370 6f74 2867 656e 6572  t_use_spot(gener
+0000fa90: 6963 5f63 6c6f 7564 3a20 7374 7229 3a0a  ic_cloud: str):.
+0000faa0: 2020 2020 2222 2254 6573 7420 7573 652d      """Test use-
+0000fab0: 7370 6f74 2061 6e64 2073 6b79 2065 7865  spot and sky exe
+0000fac0: 632e 2222 220a 2020 2020 6e61 6d65 203d  c.""".    name =
+0000fad0: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
+0000fae0: 6d65 2829 0a20 2020 2074 6573 7420 3d20  me().    test = 
+0000faf0: 5465 7374 280a 2020 2020 2020 2020 2775  Test(.        'u
+0000fb00: 7365 2d73 706f 7427 2c0a 2020 2020 2020  se-spot',.      
+0000fb10: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
+0000fb20: 6627 736b 7920 6c61 756e 6368 202d 6320  f'sky launch -c 
+0000fb30: 7b6e 616d 657d 202d 2d63 6c6f 7564 207b  {name} --cloud {
+0000fb40: 6765 6e65 7269 635f 636c 6f75 647d 2074  generic_cloud} t
+0000fb50: 6573 7473 2f74 6573 745f 7961 6d6c 732f  ests/test_yamls/
+0000fb60: 6d69 6e69 6d61 6c2e 7961 6d6c 202d 2d75  minimal.yaml --u
+0000fb70: 7365 2d73 706f 7420 2d79 272c 0a20 2020  se-spot -y',.   
+0000fb80: 2020 2020 2020 2020 2066 2773 6b79 206c           f'sky l
+0000fb90: 6f67 7320 7b6e 616d 657d 2031 202d 2d73  ogs {name} 1 --s
+0000fba0: 7461 7475 7327 2c0a 2020 2020 2020 2020  tatus',.        
+0000fbb0: 2020 2020 6627 736b 7920 6578 6563 207b      f'sky exec {
+0000fbc0: 6e61 6d65 7d20 6563 686f 2068 6927 2c0a  name} echo hi',.
+0000fbd0: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+0000fbe0: 7920 6c6f 6773 207b 6e61 6d65 7d20 3220  y logs {name} 2 
+0000fbf0: 2d2d 7374 6174 7573 272c 0a20 2020 2020  --status',.     
+0000fc00: 2020 205d 2c0a 2020 2020 2020 2020 6627     ],.        f'
+0000fc10: 736b 7920 646f 776e 202d 7920 7b6e 616d  sky down -y {nam
+0000fc20: 657d 272c 0a20 2020 2029 0a20 2020 2072  e}',.    ).    r
+0000fc30: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
+0000fc40: 290a 0a0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d  )...# ----------
+0000fc50: 2054 6573 7469 6e67 206d 616e 6167 6564   Testing managed
+0000fc60: 2073 706f 7420 2d2d 2d2d 2d2d 2d2d 2d2d   spot ----------
+0000fc70: 0a40 7079 7465 7374 2e6d 6172 6b2e 6e6f  .@pytest.mark.no
+0000fc80: 5f6c 616d 6264 615f 636c 6f75 6420 2023  _lambda_cloud  #
+0000fc90: 204c 616d 6264 6120 436c 6f75 6420 646f   Lambda Cloud do
+0000fca0: 6573 206e 6f74 2073 7570 706f 7274 2073  es not support s
+0000fcb0: 706f 7420 696e 7374 616e 6365 730a 4070  pot instances.@p
+0000fcc0: 7974 6573 742e 6d61 726b 2e6e 6f5f 6962  ytest.mark.no_ib
+0000fcd0: 6d20 2023 2049 424d 2043 6c6f 7564 2064  m  # IBM Cloud d
+0000fce0: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
+0000fcf0: 7370 6f74 2069 6e73 7461 6e63 6573 0a40  spot instances.@
+0000fd00: 7079 7465 7374 2e6d 6172 6b2e 6e6f 5f73  pytest.mark.no_s
+0000fd10: 6370 2020 2320 5343 5020 646f 6573 206e  cp  # SCP does n
+0000fd20: 6f74 2073 7570 706f 7274 2073 706f 7420  ot support spot 
+0000fd30: 696e 7374 616e 6365 730a 4070 7974 6573  instances.@pytes
+0000fd40: 742e 6d61 726b 2e6d 616e 6167 6564 5f73  t.mark.managed_s
+0000fd50: 706f 740a 6465 6620 7465 7374 5f73 706f  pot.def test_spo
+0000fd60: 7428 6765 6e65 7269 635f 636c 6f75 643a  t(generic_cloud:
+0000fd70: 2073 7472 293a 0a20 2020 2022 2222 5465   str):.    """Te
+0000fd80: 7374 2074 6865 2073 706f 7420 7961 6d6c  st the spot yaml
+0000fd90: 2e22 2222 0a20 2020 206e 616d 6520 3d20  .""".    name = 
+0000fda0: 5f67 6574 5f63 6c75 7374 6572 5f6e 616d  _get_cluster_nam
+0000fdb0: 6528 290a 2020 2020 7465 7374 203d 2054  e().    test = T
+0000fdc0: 6573 7428 0a20 2020 2020 2020 2027 6d61  est(.        'ma
+0000fdd0: 6e61 6765 642d 7370 6f74 272c 0a20 2020  naged-spot',.   
+0000fde0: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+0000fdf0: 2020 2066 2773 6b79 2073 706f 7420 6c61     f'sky spot la
+0000fe00: 756e 6368 202d 6e20 7b6e 616d 657d 2d31  unch -n {name}-1
+0000fe10: 202d 2d63 6c6f 7564 207b 6765 6e65 7269   --cloud {generi
+0000fe20: 635f 636c 6f75 647d 2065 7861 6d70 6c65  c_cloud} example
+0000fe30: 732f 6d61 6e61 6765 645f 7370 6f74 2e79  s/managed_spot.y
+0000fe40: 616d 6c20 2d79 202d 6427 2c0a 2020 2020  aml -y -d',.    
+0000fe50: 2020 2020 2020 2020 6627 736b 7920 7370          f'sky sp
+0000fe60: 6f74 206c 6175 6e63 6820 2d6e 207b 6e61  ot launch -n {na
+0000fe70: 6d65 7d2d 3220 2d2d 636c 6f75 6420 7b67  me}-2 --cloud {g
+0000fe80: 656e 6572 6963 5f63 6c6f 7564 7d20 6578  eneric_cloud} ex
+0000fe90: 616d 706c 6573 2f6d 616e 6167 6564 5f73  amples/managed_s
+0000fea0: 706f 742e 7961 6d6c 202d 7920 2d64 272c  pot.yaml -y -d',
+0000feb0: 0a20 2020 2020 2020 2020 2020 2027 736c  .            'sl
+0000fec0: 6565 7020 3527 2c0a 2020 2020 2020 2020  eep 5',.        
+0000fed0: 2020 2020 6627 7b5f 5350 4f54 5f51 5545      f'{_SPOT_QUE
+0000fee0: 5545 5f57 4149 547d 7c20 6772 6570 207b  UE_WAIT}| grep {
+0000fef0: 6e61 6d65 7d2d 3120 7c20 6865 6164 202d  name}-1 | head -
+0000ff00: 6e31 207c 2067 7265 7020 2253 5441 5254  n1 | grep "START
+0000ff10: 494e 475c 7c52 554e 4e49 4e47 2227 2c0a  ING\|RUNNING"',.
+0000ff20: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
+0000ff30: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
+0000ff40: 7c20 6772 6570 207b 6e61 6d65 7d2d 3220  | grep {name}-2 
+0000ff50: 7c20 6865 6164 202d 6e31 207c 2067 7265  | head -n1 | gre
+0000ff60: 7020 2253 5441 5254 494e 475c 7c52 554e  p "STARTING\|RUN
+0000ff70: 4e49 4e47 2227 2c0a 2020 2020 2020 2020  NING"',.        
+0000ff80: 2020 2020 5f53 504f 545f 4341 4e43 454c      _SPOT_CANCEL
+0000ff90: 5f57 4149 542e 666f 726d 6174 286a 6f62  _WAIT.format(job
+0000ffa0: 5f6e 616d 653d 6627 7b6e 616d 657d 2d31  _name=f'{name}-1
+0000ffb0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0000ffc0: 2773 6c65 6570 2035 272c 0a20 2020 2020  'sleep 5',.     
+0000ffd0: 2020 2020 2020 2066 277b 5f53 504f 545f         f'{_SPOT_
+0000ffe0: 5155 4555 455f 5741 4954 7d7c 2067 7265  QUEUE_WAIT}| gre
+0000fff0: 7020 7b6e 616d 657d 2d31 207c 2068 6561  p {name}-1 | hea
+00010000: 6420 2d6e 3120 7c20 6772 6570 2022 4341  d -n1 | grep "CA
+00010010: 4e43 454c 4c49 4e47 5c7c 4341 4e43 454c  NCELLING\|CANCEL
+00010020: 4c45 4422 272c 0a20 2020 2020 2020 2020  LED"',.         
+00010030: 2020 2027 736c 6565 7020 3230 3027 2c0a     'sleep 200',.
+00010040: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
+00010050: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
+00010060: 7c20 6772 6570 207b 6e61 6d65 7d2d 3120  | grep {name}-1 
+00010070: 7c20 6865 6164 202d 6e31 207c 2067 7265  | head -n1 | gre
+00010080: 7020 4341 4e43 454c 4c45 4427 2c0a 2020  p CANCELLED',.  
+00010090: 2020 2020 2020 2020 2020 6627 7b5f 5350            f'{_SP
+000100a0: 4f54 5f51 5545 5545 5f57 4149 547d 7c20  OT_QUEUE_WAIT}| 
+000100b0: 6772 6570 207b 6e61 6d65 7d2d 3220 7c20  grep {name}-2 | 
+000100c0: 6865 6164 202d 6e31 207c 2067 7265 7020  head -n1 | grep 
+000100d0: 2252 554e 4e49 4e47 5c7c 5355 4343 4545  "RUNNING\|SUCCEE
+000100e0: 4445 4422 272c 0a20 2020 2020 2020 205d  DED"',.        ]
+000100f0: 2c0a 2020 2020 2020 2020 2320 544f 444f  ,.        # TODO
+00010100: 287a 6877 7529 3a20 4368 616e 6765 2074  (zhwu): Change t
+00010110: 6f20 5f53 504f 545f 4341 4e43 454c 5f57  o _SPOT_CANCEL_W
+00010120: 4149 542e 666f 726d 6174 286a 6f62 5f6e  AIT.format(job_n
+00010130: 616d 653d 6627 7b6e 616d 657d 2d31 202d  ame=f'{name}-1 -
+00010140: 6e20 7b6e 616d 657d 2d32 2729 2077 6865  n {name}-2') whe
+00010150: 6e0a 2020 2020 2020 2020 2320 6361 6e63  n.        # canc
+00010160: 656c 696e 6720 6d75 6c74 6970 6c65 206a  eling multiple j
+00010170: 6f62 206e 616d 6573 2069 7320 7375 7070  ob names is supp
+00010180: 6f72 7465 642e 0a20 2020 2020 2020 2028  orted..        (
+00010190: 5f53 504f 545f 4341 4e43 454c 5f57 4149  _SPOT_CANCEL_WAI
+000101a0: 542e 666f 726d 6174 286a 6f62 5f6e 616d  T.format(job_nam
+000101b0: 653d 6627 7b6e 616d 657d 2d31 2729 202b  e=f'{name}-1') +
+000101c0: 2027 3b20 2720 2b0a 2020 2020 2020 2020   '; ' +.        
+000101d0: 205f 5350 4f54 5f43 414e 4345 4c5f 5741   _SPOT_CANCEL_WA
+000101e0: 4954 2e66 6f72 6d61 7428 6a6f 625f 6e61  IT.format(job_na
+000101f0: 6d65 3d66 277b 6e61 6d65 7d2d 3227 2929  me=f'{name}-2'))
+00010200: 2c0a 2020 2020 2020 2020 2320 496e 6372  ,.        # Incr
+00010210: 6561 7365 2074 696d 656f 7574 2073 696e  ease timeout sin
+00010220: 6365 2073 6b79 2073 706f 7420 7175 6575  ce sky spot queu
+00010230: 6520 2d72 2063 616e 2062 6520 626c 6f63  e -r can be bloc
+00010240: 6b65 6420 6279 206f 7468 6572 2073 706f  ked by other spo
+00010250: 7420 7465 7374 732e 0a20 2020 2020 2020  t tests..       
+00010260: 2074 696d 656f 7574 3d32 3020 2a20 3630   timeout=20 * 60
+00010270: 2c0a 2020 2020 290a 2020 2020 7275 6e5f  ,.    ).    run_
+00010280: 6f6e 655f 7465 7374 2874 6573 7429 0a0a  one_test(test)..
+00010290: 0a40 7079 7465 7374 2e6d 6172 6b2e 6e6f  .@pytest.mark.no
+000102a0: 5f6c 616d 6264 615f 636c 6f75 6420 2023  _lambda_cloud  #
+000102b0: 204c 616d 6264 6120 436c 6f75 6420 646f   Lambda Cloud do
+000102c0: 6573 206e 6f74 2073 7570 706f 7274 2073  es not support s
+000102d0: 706f 7420 696e 7374 616e 6365 730a 4070  pot instances.@p
+000102e0: 7974 6573 742e 6d61 726b 2e6e 6f5f 6962  ytest.mark.no_ib
+000102f0: 6d20 2023 2049 424d 2043 6c6f 7564 2064  m  # IBM Cloud d
+00010300: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
+00010310: 7370 6f74 2069 6e73 7461 6e63 6573 0a40  spot instances.@
+00010320: 7079 7465 7374 2e6d 6172 6b2e 6e6f 5f73  pytest.mark.no_s
+00010330: 6370 2020 2320 5343 5020 646f 6573 206e  cp  # SCP does n
+00010340: 6f74 2073 7570 706f 7274 2073 706f 7420  ot support spot 
+00010350: 696e 7374 616e 6365 730a 4070 7974 6573  instances.@pytes
+00010360: 742e 6d61 726b 2e6d 616e 6167 6564 5f73  t.mark.managed_s
+00010370: 706f 740a 6465 6620 7465 7374 5f73 706f  pot.def test_spo
+00010380: 745f 7069 7065 6c69 6e65 2867 656e 6572  t_pipeline(gener
+00010390: 6963 5f63 6c6f 7564 3a20 7374 7229 3a0a  ic_cloud: str):.
+000103a0: 2020 2020 2222 2254 6573 7420 6120 7370      """Test a sp
+000103b0: 6f74 c2a0 7069 7065 6c69 6e65 2e22 2222  ot..pipeline."""
+000103c0: 0a20 2020 206e 616d 6520 3d20 5f67 6574  .    name = _get
+000103d0: 5f63 6c75 7374 6572 5f6e 616d 6528 290a  _cluster_name().
+000103e0: 2020 2020 7465 7374 203d 2054 6573 7428      test = Test(
+000103f0: 0a20 2020 2020 2020 2027 7370 6f74 2d70  .        'spot-p
+00010400: 6970 656c 696e 6527 2c0a 2020 2020 2020  ipeline',.      
+00010410: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
+00010420: 6627 736b 7920 7370 6f74 206c 6175 6e63  f'sky spot launc
+00010430: 6820 2d6e 207b 6e61 6d65 7d20 7465 7374  h -n {name} test
+00010440: 732f 7465 7374 5f79 616d 6c73 2f70 6970  s/test_yamls/pip
+00010450: 656c 696e 652e 7961 6d6c 202d 7920 2d64  eline.yaml -y -d
+00010460: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
+00010470: 736c 6565 7020 3527 2c0a 2020 2020 2020  sleep 5',.      
+00010480: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
+00010490: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
+000104a0: 207b 6e61 6d65 7d20 7c20 6865 6164 202d   {name} | head -
+000104b0: 6e31 207c 2067 7265 7020 2253 5441 5254  n1 | grep "START
+000104c0: 494e 475c 7c52 554e 4e49 4e47 2227 2c0a  ING\|RUNNING"',.
+000104d0: 2020 2020 2020 2020 2020 2020 2320 6067              # `g
+000104e0: 7265 7020 2d41 2034 207b 6e61 6d65 7d60  rep -A 4 {name}`
+000104f0: 2066 696e 6473 2074 6865 206a 6f62 2077   finds the job w
+00010500: 6974 6820 7b6e 616d 657d 2061 6e64 2074  ith {name} and t
+00010510: 6865 2034 206c 696e 6573 0a20 2020 2020  he 4 lines.     
+00010520: 2020 2020 2020 2023 2061 6674 6572 2069         # after i
+00010530: 742c 2069 2e65 2e20 7468 6520 3420 7461  t, i.e. the 4 ta
+00010540: 736b 7320 7769 7468 696e 2074 6865 206a  sks within the j
+00010550: 6f62 2e0a 2020 2020 2020 2020 2020 2020  ob..            
+00010560: 2320 6073 6564 202d 6e20 3270 6020 6765  # `sed -n 2p` ge
+00010570: 7473 2074 6865 2073 6563 6f6e 6420 6c69  ts the second li
+00010580: 6e65 206f 6620 7468 6520 3420 6c69 6e65  ne of the 4 line
+00010590: 732c 2069 2e65 2e20 7468 6520 6669 7273  s, i.e. the firs
+000105a0: 740a 2020 2020 2020 2020 2020 2020 2320  t.            # 
+000105b0: 7461 736b 2077 6974 6869 6e20 7468 6520  task within the 
+000105c0: 6a6f 622e 0a20 2020 2020 2020 2020 2020  job..           
+000105d0: 2066 277b 5f53 504f 545f 5155 4555 455f   f'{_SPOT_QUEUE_
+000105e0: 5741 4954 7d7c 2067 7265 7020 2d41 2034  WAIT}| grep -A 4
+000105f0: 207b 6e61 6d65 7d7c 2073 6564 202d 6e20   {name}| sed -n 
+00010600: 3270 207c 2067 7265 7020 2253 5441 5254  2p | grep "START
+00010610: 494e 475c 7c52 554e 4e49 4e47 2227 2c0a  ING\|RUNNING"',.
+00010620: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
+00010630: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
+00010640: 7c20 6772 6570 202d 4120 3420 7b6e 616d  | grep -A 4 {nam
+00010650: 657d 7c20 7365 6420 2d6e 2033 7020 7c20  e}| sed -n 3p | 
+00010660: 6772 6570 2022 5045 4e44 494e 4722 272c  grep "PENDING"',
+00010670: 0a20 2020 2020 2020 2020 2020 205f 5350  .            _SP
+00010680: 4f54 5f43 414e 4345 4c5f 5741 4954 2e66  OT_CANCEL_WAIT.f
+00010690: 6f72 6d61 7428 6a6f 625f 6e61 6d65 3d66  ormat(job_name=f
+000106a0: 277b 6e61 6d65 7d27 292c 0a20 2020 2020  '{name}'),.     
+000106b0: 2020 2020 2020 2027 736c 6565 7020 3527         'sleep 5'
+000106c0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+000106d0: 7b5f 5350 4f54 5f51 5545 5545 5f57 4149  {_SPOT_QUEUE_WAI
+000106e0: 547d 7c20 6772 6570 202d 4120 3420 7b6e  T}| grep -A 4 {n
+000106f0: 616d 657d 7c20 7365 6420 2d6e 2032 7020  ame}| sed -n 2p 
+00010700: 7c20 6772 6570 2022 4341 4e43 454c 4c49  | grep "CANCELLI
+00010710: 4e47 5c7c 4341 4e43 454c 4c45 4422 272c  NG\|CANCELLED"',
+00010720: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
+00010730: 5f53 504f 545f 5155 4555 455f 5741 4954  _SPOT_QUEUE_WAIT
+00010740: 7d7c 2067 7265 7020 2d41 2034 207b 6e61  }| grep -A 4 {na
+00010750: 6d65 7d7c 2073 6564 202d 6e20 3370 207c  me}| sed -n 3p |
+00010760: 2067 7265 7020 2243 414e 4345 4c4c 494e   grep "CANCELLIN
+00010770: 475c 7c43 414e 4345 4c4c 4544 2227 2c0a  G\|CANCELLED"',.
+00010780: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
+00010790: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
+000107a0: 7c20 6772 6570 202d 4120 3420 7b6e 616d  | grep -A 4 {nam
+000107b0: 657d 7c20 7365 6420 2d6e 2034 7020 7c20  e}| sed -n 4p | 
+000107c0: 6772 6570 2022 4341 4e43 454c 4c49 4e47  grep "CANCELLING
+000107d0: 5c7c 4341 4e43 454c 4c45 4422 272c 0a20  \|CANCELLED"',. 
+000107e0: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
+000107f0: 504f 545f 5155 4555 455f 5741 4954 7d7c  POT_QUEUE_WAIT}|
+00010800: 2067 7265 7020 2d41 2034 207b 6e61 6d65   grep -A 4 {name
+00010810: 7d7c 2073 6564 202d 6e20 3570 207c 2067  }| sed -n 5p | g
+00010820: 7265 7020 2243 414e 4345 4c4c 494e 475c  rep "CANCELLING\
+00010830: 7c43 414e 4345 4c4c 4544 2227 2c0a 2020  |CANCELLED"',.  
+00010840: 2020 2020 2020 2020 2020 2773 6c65 6570            'sleep
+00010850: 2032 3030 272c 0a20 2020 2020 2020 2020   200',.         
+00010860: 2020 2066 277b 5f53 504f 545f 5155 4555     f'{_SPOT_QUEU
+00010870: 455f 5741 4954 7d7c 2067 7265 7020 2d41  E_WAIT}| grep -A
+00010880: 2034 207b 6e61 6d65 7d7c 2073 6564 202d   4 {name}| sed -
+00010890: 6e20 3270 207c 2067 7265 7020 2243 414e  n 2p | grep "CAN
+000108a0: 4345 4c4c 4544 2227 2c0a 2020 2020 2020  CELLED"',.      
+000108b0: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
+000108c0: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
+000108d0: 202d 4120 3420 7b6e 616d 657d 7c20 7365   -A 4 {name}| se
+000108e0: 6420 2d6e 2033 7020 7c20 6772 6570 2022  d -n 3p | grep "
+000108f0: 4341 4e43 454c 4c45 4422 272c 0a20 2020  CANCELLED"',.   
+00010900: 2020 2020 2020 2020 2066 277b 5f53 504f           f'{_SPO
+00010910: 545f 5155 4555 455f 5741 4954 7d7c 2067  T_QUEUE_WAIT}| g
+00010920: 7265 7020 2d41 2034 207b 6e61 6d65 7d7c  rep -A 4 {name}|
+00010930: 2073 6564 202d 6e20 3470 207c 2067 7265   sed -n 4p | gre
+00010940: 7020 2243 414e 4345 4c4c 4544 2227 2c0a  p "CANCELLED"',.
+00010950: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
+00010960: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
+00010970: 7c20 6772 6570 202d 4120 3420 7b6e 616d  | grep -A 4 {nam
+00010980: 657d 7c20 7365 6420 2d6e 2035 7020 7c20  e}| sed -n 5p | 
+00010990: 6772 6570 2022 4341 4e43 454c 4c45 4422  grep "CANCELLED"
+000109a0: 272c 0a20 2020 2020 2020 205d 2c0a 2020  ',.        ],.  
+000109b0: 2020 2020 2020 5f53 504f 545f 4341 4e43        _SPOT_CANC
+000109c0: 454c 5f57 4149 542e 666f 726d 6174 286a  EL_WAIT.format(j
+000109d0: 6f62 5f6e 616d 653d 6627 7b6e 616d 657d  ob_name=f'{name}
+000109e0: 2729 2c0a 2020 2020 2020 2020 2320 496e  '),.        # In
+000109f0: 6372 6561 7365 2074 696d 656f 7574 2073  crease timeout s
+00010a00: 696e 6365 2073 6b79 2073 706f 7420 7175  ince sky spot qu
+00010a10: 6575 6520 2d72 2063 616e 2062 6520 626c  eue -r can be bl
+00010a20: 6f63 6b65 6420 6279 206f 7468 6572 2073  ocked by other s
+00010a30: 706f 7420 7465 7374 732e 0a20 2020 2020  pot tests..     
+00010a40: 2020 2074 696d 656f 7574 3d33 3020 2a20     timeout=30 * 
+00010a50: 3630 2c0a 2020 2020 290a 2020 2020 7275  60,.    ).    ru
+00010a60: 6e5f 6f6e 655f 7465 7374 2874 6573 7429  n_one_test(test)
+00010a70: 0a0a 0a40 7079 7465 7374 2e6d 6172 6b2e  ...@pytest.mark.
+00010a80: 6e6f 5f6c 616d 6264 615f 636c 6f75 6420  no_lambda_cloud 
+00010a90: 2023 204c 616d 6264 6120 436c 6f75 6420   # Lambda Cloud 
+00010aa0: 646f 6573 206e 6f74 2073 7570 706f 7274  does not support
+00010ab0: 2073 706f 7420 696e 7374 616e 6365 730a   spot instances.
+00010ac0: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
+00010ad0: 6962 6d20 2023 2049 424d 2043 6c6f 7564  ibm  # IBM Cloud
+00010ae0: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
+00010af0: 7420 7370 6f74 2069 6e73 7461 6e63 6573  t spot instances
+00010b00: 0a40 7079 7465 7374 2e6d 6172 6b2e 6e6f  .@pytest.mark.no
+00010b10: 5f73 6370 2020 2320 5343 5020 646f 6573  _scp  # SCP does
+00010b20: 206e 6f74 2073 7570 706f 7274 2073 706f   not support spo
+00010b30: 7420 696e 7374 616e 6365 730a 4070 7974  t instances.@pyt
+00010b40: 6573 742e 6d61 726b 2e6d 616e 6167 6564  est.mark.managed
+00010b50: 5f73 706f 740a 6465 6620 7465 7374 5f73  _spot.def test_s
+00010b60: 706f 745f 6661 696c 6564 5f73 6574 7570  pot_failed_setup
+00010b70: 2867 656e 6572 6963 5f63 6c6f 7564 3a20  (generic_cloud: 
+00010b80: 7374 7229 3a0a 2020 2020 2222 2254 6573  str):.    """Tes
+00010b90: 7420 6d61 6e61 6765 6420 7370 6f74 206a  t managed spot j
+00010ba0: 6f62 2077 6974 6820 6661 696c 6564 2073  ob with failed s
+00010bb0: 6574 7570 2e22 2222 0a20 2020 206e 616d  etup.""".    nam
+00010bc0: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
+00010bd0: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
+00010be0: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
+00010bf0: 2027 7370 6f74 5f66 6169 6c65 645f 7365   'spot_failed_se
+00010c00: 7475 7027 2c0a 2020 2020 2020 2020 5b0a  tup',.        [.
+00010c10: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+00010c20: 7920 7370 6f74 206c 6175 6e63 6820 2d6e  y spot launch -n
+00010c30: 207b 6e61 6d65 7d20 2d2d 636c 6f75 6420   {name} --cloud 
+00010c40: 7b67 656e 6572 6963 5f63 6c6f 7564 7d20  {generic_cloud} 
+00010c50: 2d79 202d 6420 7465 7374 732f 7465 7374  -y -d tests/test
+00010c60: 5f79 616d 6c73 2f66 6169 6c65 645f 7365  _yamls/failed_se
+00010c70: 7475 702e 7961 6d6c 272c 0a20 2020 2020  tup.yaml',.     
+00010c80: 2020 2020 2020 2027 736c 6565 7020 3333         'sleep 33
+00010c90: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
+00010ca0: 2320 4d61 6b65 2073 7572 6520 7468 6520  # Make sure the 
+00010cb0: 6a6f 6220 6661 696c 6564 2071 7569 636b  job failed quick
+00010cc0: 6c79 2e0a 2020 2020 2020 2020 2020 2020  ly..            
+00010cd0: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
+00010ce0: 4149 547d 207c 2067 7265 7020 7b6e 616d  AIT} | grep {nam
+00010cf0: 657d 207c 2068 6561 6420 2d6e 3120 7c20  e} | head -n1 | 
+00010d00: 6772 6570 2022 4641 494c 4544 5f53 4554  grep "FAILED_SET
+00010d10: 5550 2227 2c0a 2020 2020 2020 2020 5d2c  UP"',.        ],
+00010d20: 0a20 2020 2020 2020 205f 5350 4f54 5f43  .        _SPOT_C
+00010d30: 414e 4345 4c5f 5741 4954 2e66 6f72 6d61  ANCEL_WAIT.forma
+00010d40: 7428 6a6f 625f 6e61 6d65 3d6e 616d 6529  t(job_name=name)
+00010d50: 2c0a 2020 2020 2020 2020 2320 496e 6372  ,.        # Incr
+00010d60: 6561 7365 2074 696d 656f 7574 2073 696e  ease timeout sin
+00010d70: 6365 2073 6b79 2073 706f 7420 7175 6575  ce sky spot queu
+00010d80: 6520 2d72 2063 616e 2062 6520 626c 6f63  e -r can be bloc
+00010d90: 6b65 6420 6279 206f 7468 6572 2073 706f  ked by other spo
+00010da0: 7420 7465 7374 732e 0a20 2020 2020 2020  t tests..       
+00010db0: 2074 696d 656f 7574 3d32 3020 2a20 3630   timeout=20 * 60
+00010dc0: 2c0a 2020 2020 290a 2020 2020 7275 6e5f  ,.    ).    run_
+00010dd0: 6f6e 655f 7465 7374 2874 6573 7429 0a0a  one_test(test)..
+00010de0: 0a40 7079 7465 7374 2e6d 6172 6b2e 6e6f  .@pytest.mark.no
+00010df0: 5f6c 616d 6264 615f 636c 6f75 6420 2023  _lambda_cloud  #
+00010e00: 204c 616d 6264 6120 436c 6f75 6420 646f   Lambda Cloud do
+00010e10: 6573 206e 6f74 2073 7570 706f 7274 2073  es not support s
+00010e20: 706f 7420 696e 7374 616e 6365 730a 4070  pot instances.@p
+00010e30: 7974 6573 742e 6d61 726b 2e6e 6f5f 6962  ytest.mark.no_ib
+00010e40: 6d20 2023 2049 424d 2043 6c6f 7564 2064  m  # IBM Cloud d
+00010e50: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
+00010e60: 7370 6f74 2069 6e73 7461 6e63 6573 0a40  spot instances.@
+00010e70: 7079 7465 7374 2e6d 6172 6b2e 6e6f 5f73  pytest.mark.no_s
+00010e80: 6370 2020 2320 5343 5020 646f 6573 206e  cp  # SCP does n
+00010e90: 6f74 2073 7570 706f 7274 2073 706f 7420  ot support spot 
+00010ea0: 696e 7374 616e 6365 730a 4070 7974 6573  instances.@pytes
+00010eb0: 742e 6d61 726b 2e6d 616e 6167 6564 5f73  t.mark.managed_s
+00010ec0: 706f 740a 6465 6620 7465 7374 5f73 706f  pot.def test_spo
+00010ed0: 745f 7069 7065 6c69 6e65 5f66 6169 6c65  t_pipeline_faile
+00010ee0: 645f 7365 7475 7028 6765 6e65 7269 635f  d_setup(generic_
+00010ef0: 636c 6f75 643a 2073 7472 293a 0a20 2020  cloud: str):.   
+00010f00: 2022 2222 5465 7374 206d 616e 6167 6564   """Test managed
+00010f10: 2073 706f 7420 6a6f 6220 7769 7468 2066   spot job with f
+00010f20: 6169 6c65 6420 7365 7475 7020 666f 7220  ailed setup for 
+00010f30: 6120 7069 7065 6c69 6e65 2e22 2222 0a20  a pipeline.""". 
+00010f40: 2020 206e 616d 6520 3d20 5f67 6574 5f63     name = _get_c
+00010f50: 6c75 7374 6572 5f6e 616d 6528 290a 2020  luster_name().  
+00010f60: 2020 7465 7374 203d 2054 6573 7428 0a20    test = Test(. 
+00010f70: 2020 2020 2020 2027 7370 6f74 5f70 6970         'spot_pip
+00010f80: 656c 696e 655f 6661 696c 6564 5f73 6574  eline_failed_set
+00010f90: 7570 272c 0a20 2020 2020 2020 205b 0a20  up',.        [. 
+00010fa0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+00010fb0: 2073 706f 7420 6c61 756e 6368 202d 6e20   spot launch -n 
+00010fc0: 7b6e 616d 657d 202d 7920 2d64 2074 6573  {name} -y -d tes
+00010fd0: 7473 2f74 6573 745f 7961 6d6c 732f 6661  ts/test_yamls/fa
+00010fe0: 696c 6564 5f73 6574 7570 5f70 6970 656c  iled_setup_pipel
+00010ff0: 696e 652e 7961 6d6c 272c 0a20 2020 2020  ine.yaml',.     
+00011000: 2020 2020 2020 2027 736c 6565 7020 3830         'sleep 80
+00011010: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
+00011020: 2320 4d61 6b65 2073 7572 6520 7468 6520  # Make sure the 
+00011030: 6a6f 6220 6661 696c 6564 2071 7569 636b  job failed quick
+00011040: 6c79 2e0a 2020 2020 2020 2020 2020 2020  ly..            
+00011050: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
+00011060: 4149 547d 207c 2067 7265 7020 7b6e 616d  AIT} | grep {nam
+00011070: 657d 207c 2068 6561 6420 2d6e 3120 7c20  e} | head -n1 | 
+00011080: 6772 6570 2022 4641 494c 4544 5f53 4554  grep "FAILED_SET
+00011090: 5550 2227 2c0a 2020 2020 2020 2020 2020  UP"',.          
+000110a0: 2020 2320 5461 736b 2030 2073 686f 756c    # Task 0 shoul
+000110b0: 6420 6265 2053 5543 4345 4544 4544 2e0a  d be SUCCEEDED..
+000110c0: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
+000110d0: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
+000110e0: 207c 2067 7265 7020 2d41 2034 207b 6e61   | grep -A 4 {na
+000110f0: 6d65 7d7c 2073 6564 202d 6e20 3270 207c  me}| sed -n 2p |
+00011100: 2067 7265 7020 2253 5543 4345 4544 4544   grep "SUCCEEDED
+00011110: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
+00011120: 2320 5461 736b 2031 2073 686f 756c 6420  # Task 1 should 
+00011130: 6265 2046 4149 4c45 445f 5345 5455 502e  be FAILED_SETUP.
+00011140: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
+00011150: 5f53 504f 545f 5155 4555 455f 5741 4954  _SPOT_QUEUE_WAIT
+00011160: 7d20 7c20 6772 6570 202d 4120 3420 7b6e  } | grep -A 4 {n
+00011170: 616d 657d 7c20 7365 6420 2d6e 2033 7020  ame}| sed -n 3p 
+00011180: 7c20 6772 6570 2022 4641 494c 4544 5f53  | grep "FAILED_S
+00011190: 4554 5550 2227 2c0a 2020 2020 2020 2020  ETUP"',.        
+000111a0: 2020 2020 2320 5461 736b 2032 2073 686f      # Task 2 sho
+000111b0: 756c 6420 6265 2043 414e 4345 4c4c 4544  uld be CANCELLED
+000111c0: 2e0a 2020 2020 2020 2020 2020 2020 6627  ..            f'
+000111d0: 7b5f 5350 4f54 5f51 5545 5545 5f57 4149  {_SPOT_QUEUE_WAI
+000111e0: 547d 207c 2067 7265 7020 2d41 2034 207b  T} | grep -A 4 {
+000111f0: 6e61 6d65 7d7c 2073 6564 202d 6e20 3470  name}| sed -n 4p
+00011200: 207c 2067 7265 7020 2243 414e 4345 4c4c   | grep "CANCELL
+00011210: 4544 2227 2c0a 2020 2020 2020 2020 2020  ED"',.          
+00011220: 2020 2320 5461 736b 2033 2073 686f 756c    # Task 3 shoul
+00011230: 6420 6265 2043 414e 4345 4c4c 4544 2e0a  d be CANCELLED..
+00011240: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
+00011250: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
+00011260: 207c 2067 7265 7020 2d41 2034 207b 6e61   | grep -A 4 {na
+00011270: 6d65 7d7c 2073 6564 202d 6e20 3570 207c  me}| sed -n 5p |
+00011280: 2067 7265 7020 2243 414e 4345 4c4c 4544   grep "CANCELLED
+00011290: 2227 2c0a 2020 2020 2020 2020 5d2c 0a20  "',.        ],. 
+000112a0: 2020 2020 2020 205f 5350 4f54 5f43 414e         _SPOT_CAN
+000112b0: 4345 4c5f 5741 4954 2e66 6f72 6d61 7428  CEL_WAIT.format(
+000112c0: 6a6f 625f 6e61 6d65 3d6e 616d 6529 2c0a  job_name=name),.
+000112d0: 2020 2020 2020 2020 2320 496e 6372 6561          # Increa
+000112e0: 7365 2074 696d 656f 7574 2073 696e 6365  se timeout since
+000112f0: 2073 6b79 2073 706f 7420 7175 6575 6520   sky spot queue 
+00011300: 2d72 2063 616e 2062 6520 626c 6f63 6b65  -r can be blocke
+00011310: 6420 6279 206f 7468 6572 2073 706f 7420  d by other spot 
+00011320: 7465 7374 732e 0a20 2020 2020 2020 2074  tests..        t
+00011330: 696d 656f 7574 3d33 3020 2a20 3630 2c0a  imeout=30 * 60,.
+00011340: 2020 2020 290a 2020 2020 7275 6e5f 6f6e      ).    run_on
+00011350: 655f 7465 7374 2874 6573 7429 0a0a 0a23  e_test(test)...#
+00011360: 202d 2d2d 2d2d 2d2d 2d2d 2d20 5465 7374   ---------- Test
+00011370: 696e 6720 6d61 6e61 6765 6420 7370 6f74  ing managed spot
+00011380: 2072 6563 6f76 6572 7920 2d2d 2d2d 2d2d   recovery ------
+00011390: 2d2d 2d2d 0a0a 0a40 7079 7465 7374 2e6d  ----...@pytest.m
+000113a0: 6172 6b2e 6177 730a 4070 7974 6573 742e  ark.aws.@pytest.
+000113b0: 6d61 726b 2e6d 616e 6167 6564 5f73 706f  mark.managed_spo
+000113c0: 740a 6465 6620 7465 7374 5f73 706f 745f  t.def test_spot_
+000113d0: 7265 636f 7665 7279 5f61 7773 2861 7773  recovery_aws(aws
+000113e0: 5f63 6f6e 6669 675f 7265 6769 6f6e 293a  _config_region):
+000113f0: 0a20 2020 2022 2222 5465 7374 206d 616e  .    """Test man
+00011400: 6167 6564 2073 706f 7420 7265 636f 7665  aged spot recove
+00011410: 7279 2e22 2222 0a20 2020 206e 616d 6520  ry.""".    name 
+00011420: 3d20 5f67 6574 5f63 6c75 7374 6572 5f6e  = _get_cluster_n
+00011430: 616d 6528 290a 2020 2020 7265 6769 6f6e  ame().    region
+00011440: 203d 2061 7773 5f63 6f6e 6669 675f 7265   = aws_config_re
+00011450: 6769 6f6e 0a20 2020 2074 6573 7420 3d20  gion.    test = 
+00011460: 5465 7374 280a 2020 2020 2020 2020 2773  Test(.        's
+00011470: 706f 745f 7265 636f 7665 7279 5f61 7773  pot_recovery_aws
+00011480: 272c 0a20 2020 2020 2020 205b 0a20 2020  ',.        [.   
+00011490: 2020 2020 2020 2020 2066 2773 6b79 2073           f'sky s
+000114a0: 706f 7420 6c61 756e 6368 202d 2d63 6c6f  pot launch --clo
+000114b0: 7564 2061 7773 202d 2d72 6567 696f 6e20  ud aws --region 
+000114c0: 7b72 6567 696f 6e7d 202d 6e20 7b6e 616d  {region} -n {nam
+000114d0: 657d 2022 6563 686f 2053 4b59 5049 4c4f  e} "echo SKYPILO
+000114e0: 545f 5441 534b 5f49 443a 205c 2453 4b59  T_TASK_ID: \$SKY
+000114f0: 5049 4c4f 545f 5441 534b 5f49 443b 2073  PILOT_TASK_ID; s
+00011500: 6c65 6570 2031 3830 3022 2020 2d79 202d  leep 1800"  -y -
+00011510: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
+00011520: 2773 6c65 6570 2033 3630 272c 0a20 2020  'sleep 360',.   
+00011530: 2020 2020 2020 2020 2066 277b 5f53 504f           f'{_SPO
+00011540: 545f 5155 4555 455f 5741 4954 7d7c 2067  T_QUEUE_WAIT}| g
+00011550: 7265 7020 7b6e 616d 657d 207c 2068 6561  rep {name} | hea
+00011560: 6420 2d6e 3120 7c20 6772 6570 2022 5255  d -n1 | grep "RU
+00011570: 4e4e 494e 4722 272c 0a20 2020 2020 2020  NNING"',.       
+00011580: 2020 2020 2066 2752 554e 5f49 443d 2428       f'RUN_ID=$(
+00011590: 736b 7920 7370 6f74 206c 6f67 7320 2d6e  sky spot logs -n
+000115a0: 207b 6e61 6d65 7d20 2d2d 6e6f 2d66 6f6c   {name} --no-fol
+000115b0: 6c6f 7720 7c20 6772 6570 2053 4b59 5049  low | grep SKYPI
+000115c0: 4c4f 545f 5441 534b 5f49 4420 7c20 6375  LOT_TASK_ID | cu
+000115d0: 7420 2d64 3a20 2d66 3229 3b20 6563 686f  t -d: -f2); echo
+000115e0: 2022 2452 554e 5f49 4422 207c 2074 6565   "$RUN_ID" | tee
+000115f0: 202f 746d 702f 7b6e 616d 657d 2d72 756e   /tmp/{name}-run
+00011600: 2d69 6427 2c0a 2020 2020 2020 2020 2020  -id',.          
+00011610: 2020 2320 5465 726d 696e 6174 6520 7468    # Terminate th
+00011620: 6520 636c 7573 7465 7220 6d61 6e75 616c  e cluster manual
+00011630: 6c79 2e0a 2020 2020 2020 2020 2020 2020  ly..            
+00011640: 2866 2761 7773 2065 6332 2074 6572 6d69  (f'aws ec2 termi
+00011650: 6e61 7465 2d69 6e73 7461 6e63 6573 202d  nate-instances -
+00011660: 2d72 6567 696f 6e20 7b72 6567 696f 6e7d  -region {region}
+00011670: 202d 2d69 6e73 7461 6e63 652d 6964 7320   --instance-ids 
+00011680: 2428 270a 2020 2020 2020 2020 2020 2020  $('.            
+00011690: 2066 2761 7773 2065 6332 2064 6573 6372   f'aws ec2 descr
+000116a0: 6962 652d 696e 7374 616e 6365 7320 2d2d  ibe-instances --
+000116b0: 7265 6769 6f6e 207b 7265 6769 6f6e 7d20  region {region} 
+000116c0: 270a 2020 2020 2020 2020 2020 2020 2066  '.             f
+000116d0: 272d 2d66 696c 7465 7273 204e 616d 653d  '--filters Name=
+000116e0: 7461 673a 7261 792d 636c 7573 7465 722d  tag:ray-cluster-
+000116f0: 6e61 6d65 2c56 616c 7565 733d 7b6e 616d  name,Values={nam
+00011700: 657d 2a20 270a 2020 2020 2020 2020 2020  e}* '.          
+00011710: 2020 2066 272d 2d71 7565 7279 2052 6573     f'--query Res
+00011720: 6572 7661 7469 6f6e 735b 5d2e 496e 7374  ervations[].Inst
+00011730: 616e 6365 735b 5d2e 496e 7374 616e 6365  ances[].Instance
+00011740: 4964 2027 0a20 2020 2020 2020 2020 2020  Id '.           
+00011750: 2020 272d 2d6f 7574 7075 7420 7465 7874    '--output text
+00011760: 2927 292c 0a20 2020 2020 2020 2020 2020  )'),.           
+00011770: 2027 736c 6565 7020 3130 3027 2c0a 2020   'sleep 100',.  
+00011780: 2020 2020 2020 2020 2020 6627 7b5f 5350            f'{_SP
+00011790: 4f54 5f51 5545 5545 5f57 4149 547d 7c20  OT_QUEUE_WAIT}| 
+000117a0: 6772 6570 207b 6e61 6d65 7d20 7c20 6865  grep {name} | he
+000117b0: 6164 202d 6e31 207c 2067 7265 7020 2252  ad -n1 | grep "R
+000117c0: 4543 4f56 4552 494e 4722 272c 0a20 2020  ECOVERING"',.   
+000117d0: 2020 2020 2020 2020 2027 736c 6565 7020           'sleep 
+000117e0: 3230 3027 2c0a 2020 2020 2020 2020 2020  200',.          
+000117f0: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
+00011800: 5f57 4149 547d 7c20 6772 6570 207b 6e61  _WAIT}| grep {na
+00011810: 6d65 7d20 7c20 6865 6164 202d 6e31 207c  me} | head -n1 |
+00011820: 2067 7265 7020 2252 554e 4e49 4e47 2227   grep "RUNNING"'
+00011830: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+00011840: 5255 4e5f 4944 3d24 2863 6174 202f 746d  RUN_ID=$(cat /tm
+00011850: 702f 7b6e 616d 657d 2d72 756e 2d69 6429  p/{name}-run-id)
+00011860: 3b20 6563 686f 2024 5255 4e5f 4944 3b20  ; echo $RUN_ID; 
+00011870: 736b 7920 7370 6f74 206c 6f67 7320 2d6e  sky spot logs -n
+00011880: 207b 6e61 6d65 7d20 2d2d 6e6f 2d66 6f6c   {name} --no-fol
+00011890: 6c6f 7720 7c20 6772 6570 2053 4b59 5049  low | grep SKYPI
+000118a0: 4c4f 545f 5441 534b 5f49 4420 7c20 6772  LOT_TASK_ID | gr
+000118b0: 6570 2022 2452 554e 5f49 4422 272c 0a20  ep "$RUN_ID"',. 
+000118c0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+000118d0: 2020 5f53 504f 545f 4341 4e43 454c 5f57    _SPOT_CANCEL_W
+000118e0: 4149 542e 666f 726d 6174 286a 6f62 5f6e  AIT.format(job_n
+000118f0: 616d 653d 6e61 6d65 292c 0a20 2020 2020  ame=name),.     
+00011900: 2020 2074 696d 656f 7574 3d32 3520 2a20     timeout=25 * 
+00011910: 3630 2c0a 2020 2020 290a 2020 2020 7275  60,.    ).    ru
+00011920: 6e5f 6f6e 655f 7465 7374 2874 6573 7429  n_one_test(test)
+00011930: 0a0a 0a40 7079 7465 7374 2e6d 6172 6b2e  ...@pytest.mark.
+00011940: 6763 700a 4070 7974 6573 742e 6d61 726b  gcp.@pytest.mark
+00011950: 2e6d 616e 6167 6564 5f73 706f 740a 6465  .managed_spot.de
+00011960: 6620 7465 7374 5f73 706f 745f 7265 636f  f test_spot_reco
+00011970: 7665 7279 5f67 6370 2829 3a0a 2020 2020  very_gcp():.    
+00011980: 2222 2254 6573 7420 6d61 6e61 6765 6420  """Test managed 
+00011990: 7370 6f74 2072 6563 6f76 6572 792e 2222  spot recovery.""
+000119a0: 220a 2020 2020 6e61 6d65 203d 205f 6765  ".    name = _ge
+000119b0: 745f 636c 7573 7465 725f 6e61 6d65 2829  t_cluster_name()
+000119c0: 0a20 2020 207a 6f6e 6520 3d20 2775 732d  .    zone = 'us-
+000119d0: 6561 7374 342d 6227 0a20 2020 2071 7565  east4-b'.    que
+000119e0: 7279 5f63 6d64 203d 2028 6627 6763 6c6f  ry_cmd = (f'gclo
+000119f0: 7564 2063 6f6d 7075 7465 2069 6e73 7461  ud compute insta
+00011a00: 6e63 6573 206c 6973 7420 2d2d 6669 6c74  nces list --filt
+00011a10: 6572 3d27 0a20 2020 2020 2020 2020 2020  er='.           
+00011a20: 2020 2020 2020 6627 2228 6c61 6265 6c73        f'"(labels
+00011a30: 2e72 6179 2d63 6c75 7374 6572 2d6e 616d  .ray-cluster-nam
+00011a40: 653a 7b6e 616d 657d 2922 2027 0a20 2020  e:{name})" '.   
+00011a50: 2020 2020 2020 2020 2020 2020 2020 6627                f'
+00011a60: 2d2d 7a6f 6e65 733d 7b7a 6f6e 657d 202d  --zones={zone} -
+00011a70: 2d66 6f72 6d61 743d 2276 616c 7565 286e  -format="value(n
+00011a80: 616d 6529 2227 290a 2020 2020 7465 726d  ame)"').    term
+00011a90: 696e 6174 655f 636d 6420 3d20 2866 2767  inate_cmd = (f'g
+00011aa0: 636c 6f75 6420 636f 6d70 7574 6520 696e  cloud compute in
+00011ab0: 7374 616e 6365 7320 6465 6c65 7465 202d  stances delete -
+00011ac0: 2d7a 6f6e 653d 7b7a 6f6e 657d 270a 2020  -zone={zone}'.  
+00011ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ae0: 2020 2066 2720 2d2d 7175 6965 7420 2428     f' --quiet $(
+00011af0: 7b71 7565 7279 5f63 6d64 7d29 2729 0a20  {query_cmd})'). 
+00011b00: 2020 2074 6573 7420 3d20 5465 7374 280a     test = Test(.
+00011b10: 2020 2020 2020 2020 2773 706f 745f 7265          'spot_re
+00011b20: 636f 7665 7279 5f67 6370 272c 0a20 2020  covery_gcp',.   
+00011b30: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+00011b40: 2020 2066 2773 6b79 2073 706f 7420 6c61     f'sky spot la
+00011b50: 756e 6368 202d 2d63 6c6f 7564 2067 6370  unch --cloud gcp
+00011b60: 202d 2d7a 6f6e 6520 7b7a 6f6e 657d 202d   --zone {zone} -
+00011b70: 6e20 7b6e 616d 657d 2022 6563 686f 2053  n {name} "echo S
+00011b80: 4b59 5049 4c4f 545f 5441 534b 5f49 443a  KYPILOT_TASK_ID:
+00011b90: 205c 2453 4b59 5049 4c4f 545f 5441 534b   \$SKYPILOT_TASK
+00011ba0: 5f49 443b 2073 6c65 6570 2031 3830 3022  _ID; sleep 1800"
+00011bb0: 2020 2d79 202d 6427 2c0a 2020 2020 2020    -y -d',.      
+00011bc0: 2020 2020 2020 2773 6c65 6570 2033 3630        'sleep 360
+00011bd0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+00011be0: 277b 5f53 504f 545f 5155 4555 455f 5741  '{_SPOT_QUEUE_WA
+00011bf0: 4954 7d7c 2067 7265 7020 7b6e 616d 657d  IT}| grep {name}
+00011c00: 207c 2068 6561 6420 2d6e 3120 7c20 6772   | head -n1 | gr
+00011c10: 6570 2022 5255 4e4e 494e 4722 272c 0a20  ep "RUNNING"',. 
+00011c20: 2020 2020 2020 2020 2020 2066 2752 554e             f'RUN
+00011c30: 5f49 443d 2428 736b 7920 7370 6f74 206c  _ID=$(sky spot l
+00011c40: 6f67 7320 2d6e 207b 6e61 6d65 7d20 2d2d  ogs -n {name} --
+00011c50: 6e6f 2d66 6f6c 6c6f 7720 7c20 6772 6570  no-follow | grep
+00011c60: 2053 4b59 5049 4c4f 545f 5441 534b 5f49   SKYPILOT_TASK_I
+00011c70: 4420 7c20 6375 7420 2d64 3a20 2d66 3229  D | cut -d: -f2)
+00011c80: 3b20 6563 686f 2022 2452 554e 5f49 4422  ; echo "$RUN_ID"
+00011c90: 207c 2074 6565 202f 746d 702f 7b6e 616d   | tee /tmp/{nam
+00011ca0: 657d 2d72 756e 2d69 6427 2c0a 2020 2020  e}-run-id',.    
+00011cb0: 2020 2020 2020 2020 2320 5465 726d 696e          # Termin
+00011cc0: 6174 6520 7468 6520 636c 7573 7465 7220  ate the cluster 
+00011cd0: 6d61 6e75 616c 6c79 2e0a 2020 2020 2020  manually..      
+00011ce0: 2020 2020 2020 7465 726d 696e 6174 655f        terminate_
+00011cf0: 636d 642c 0a20 2020 2020 2020 2020 2020  cmd,.           
+00011d00: 2027 736c 6565 7020 3130 3027 2c0a 2020   'sleep 100',.  
+00011d10: 2020 2020 2020 2020 2020 6627 7b5f 5350            f'{_SP
+00011d20: 4f54 5f51 5545 5545 5f57 4149 547d 7c20  OT_QUEUE_WAIT}| 
+00011d30: 6772 6570 207b 6e61 6d65 7d20 7c20 6865  grep {name} | he
+00011d40: 6164 202d 6e31 207c 2067 7265 7020 2252  ad -n1 | grep "R
+00011d50: 4543 4f56 4552 494e 4722 272c 0a20 2020  ECOVERING"',.   
+00011d60: 2020 2020 2020 2020 2027 736c 6565 7020           'sleep 
+00011d70: 3230 3027 2c0a 2020 2020 2020 2020 2020  200',.          
+00011d80: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
+00011d90: 5f57 4149 547d 7c20 6772 6570 207b 6e61  _WAIT}| grep {na
+00011da0: 6d65 7d20 7c20 6865 6164 202d 6e31 207c  me} | head -n1 |
+00011db0: 2067 7265 7020 2252 554e 4e49 4e47 2227   grep "RUNNING"'
+00011dc0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+00011dd0: 5255 4e5f 4944 3d24 2863 6174 202f 746d  RUN_ID=$(cat /tm
+00011de0: 702f 7b6e 616d 657d 2d72 756e 2d69 6429  p/{name}-run-id)
+00011df0: 3b20 6563 686f 2024 5255 4e5f 4944 3b20  ; echo $RUN_ID; 
+00011e00: 736b 7920 7370 6f74 206c 6f67 7320 2d6e  sky spot logs -n
+00011e10: 207b 6e61 6d65 7d20 2d2d 6e6f 2d66 6f6c   {name} --no-fol
+00011e20: 6c6f 7720 7c20 6772 6570 2053 4b59 5049  low | grep SKYPI
+00011e30: 4c4f 545f 5441 534b 5f49 443a 207c 2067  LOT_TASK_ID: | g
+00011e40: 7265 7020 2224 5255 4e5f 4944 2227 2c0a  rep "$RUN_ID"',.
+00011e50: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00011e60: 2020 205f 5350 4f54 5f43 414e 4345 4c5f     _SPOT_CANCEL_
+00011e70: 5741 4954 2e66 6f72 6d61 7428 6a6f 625f  WAIT.format(job_
+00011e80: 6e61 6d65 3d6e 616d 6529 2c0a 2020 2020  name=name),.    
+00011e90: 2020 2020 7469 6d65 6f75 743d 3235 202a      timeout=25 *
+00011ea0: 2036 302c 0a20 2020 2029 0a20 2020 2072   60,.    ).    r
+00011eb0: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
+00011ec0: 290a 0a0a 4070 7974 6573 742e 6d61 726b  )...@pytest.mark
+00011ed0: 2e61 7773 0a40 7079 7465 7374 2e6d 6172  .aws.@pytest.mar
+00011ee0: 6b2e 6d61 6e61 6765 645f 7370 6f74 0a64  k.managed_spot.d
+00011ef0: 6566 2074 6573 745f 7370 6f74 5f70 6970  ef test_spot_pip
+00011f00: 656c 696e 655f 7265 636f 7665 7279 5f61  eline_recovery_a
+00011f10: 7773 2861 7773 5f63 6f6e 6669 675f 7265  ws(aws_config_re
+00011f20: 6769 6f6e 293a 0a20 2020 2022 2222 5465  gion):.    """Te
+00011f30: 7374 206d 616e 6167 6564 2073 706f 7420  st managed spot 
+00011f40: 7265 636f 7665 7279 2066 6f72 2061 2070  recovery for a p
+00011f50: 6970 656c 696e 652e 2222 220a 2020 2020  ipeline.""".    
+00011f60: 6e61 6d65 203d 205f 6765 745f 636c 7573  name = _get_clus
+00011f70: 7465 725f 6e61 6d65 2829 0a20 2020 2072  ter_name().    r
+00011f80: 6567 696f 6e20 3d20 6177 735f 636f 6e66  egion = aws_conf
+00011f90: 6967 5f72 6567 696f 6e0a 2020 2020 6966  ig_region.    if
+00011fa0: 2072 6567 696f 6e20 213d 2027 7573 2d77   region != 'us-w
+00011fb0: 6573 742d 3227 3a0a 2020 2020 2020 2020  est-2':.        
+00011fc0: 7079 7465 7374 2e73 6b69 7028 274f 6e6c  pytest.skip('Onl
+00011fd0: 7920 7275 6e20 7370 6f74 2070 6970 656c  y run spot pipel
+00011fe0: 696e 6520 7265 636f 7665 7279 2074 6573  ine recovery tes
+00011ff0: 7420 696e 2075 732d 7765 7374 2d32 2729  t in us-west-2')
+00012000: 0a20 2020 2074 6573 7420 3d20 5465 7374  .    test = Test
+00012010: 280a 2020 2020 2020 2020 2773 706f 745f  (.        'spot_
+00012020: 7069 7065 6c69 6e65 5f72 6563 6f76 6572  pipeline_recover
+00012030: 795f 6177 7327 2c0a 2020 2020 2020 2020  y_aws',.        
+00012040: 5b0a 2020 2020 2020 2020 2020 2020 6627  [.            f'
+00012050: 736b 7920 7370 6f74 206c 6175 6e63 6820  sky spot launch 
+00012060: 2d6e 207b 6e61 6d65 7d20 7465 7374 732f  -n {name} tests/
+00012070: 7465 7374 5f79 616d 6c73 2f70 6970 656c  test_yamls/pipel
+00012080: 696e 655f 6177 732e 7961 6d6c 2020 2d79  ine_aws.yaml  -y
+00012090: 202d 6427 2c0a 2020 2020 2020 2020 2020   -d',.          
+000120a0: 2020 2773 6c65 6570 2034 3030 272c 0a20    'sleep 400',. 
+000120b0: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
+000120c0: 504f 545f 5155 4555 455f 5741 4954 7d7c  POT_QUEUE_WAIT}|
+000120d0: 2067 7265 7020 7b6e 616d 657d 207c 2068   grep {name} | h
+000120e0: 6561 6420 2d6e 3120 7c20 6772 6570 2022  ead -n1 | grep "
+000120f0: 5255 4e4e 494e 4722 272c 0a20 2020 2020  RUNNING"',.     
+00012100: 2020 2020 2020 2066 2752 554e 5f49 443d         f'RUN_ID=
+00012110: 2428 736b 7920 7370 6f74 206c 6f67 7320  $(sky spot logs 
+00012120: 2d6e 207b 6e61 6d65 7d20 2d2d 6e6f 2d66  -n {name} --no-f
+00012130: 6f6c 6c6f 7720 7c20 6772 6570 2053 4b59  ollow | grep SKY
+00012140: 5049 4c4f 545f 5441 534b 5f49 443a 207c  PILOT_TASK_ID: |
+00012150: 2063 7574 202d 643a 202d 6632 293b 2065   cut -d: -f2); e
+00012160: 6368 6f20 2224 5255 4e5f 4944 2220 7c20  cho "$RUN_ID" | 
+00012170: 7465 6520 2f74 6d70 2f7b 6e61 6d65 7d2d  tee /tmp/{name}-
+00012180: 7275 6e2d 6964 272c 0a20 2020 2020 2020  run-id',.       
+00012190: 2020 2020 2066 2752 554e 5f49 4453 3d24       f'RUN_IDS=$
+000121a0: 2873 6b79 2073 706f 7420 6c6f 6773 202d  (sky spot logs -
+000121b0: 6e20 7b6e 616d 657d 202d 2d6e 6f2d 666f  n {name} --no-fo
+000121c0: 6c6c 6f77 207c 2067 7265 7020 2d41 2034  llow | grep -A 4
+000121d0: 2053 4b59 5049 4c4f 545f 5441 534b 5f49   SKYPILOT_TASK_I
+000121e0: 4453 207c 2063 7574 202d 6422 2922 202d  DS | cut -d")" -
+000121f0: 6632 293b 2065 6368 6f20 2224 5255 4e5f  f2); echo "$RUN_
+00012200: 4944 5322 207c 2074 6565 202f 746d 702f  IDS" | tee /tmp/
+00012210: 7b6e 616d 657d 2d72 756e 2d69 6473 272c  {name}-run-ids',
+00012220: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
+00012230: 6572 6d69 6e61 7465 2074 6865 2063 6c75  erminate the clu
+00012240: 7374 6572 206d 616e 7561 6c6c 792e 0a20  ster manually.. 
+00012250: 2020 2020 2020 2020 2020 2023 2054 6865             # The
+00012260: 2060 6361 7420 2e2e 2e7c 2072 6576 6020   `cat ...| rev` 
+00012270: 6973 2074 6f20 7265 7472 6965 7665 2074  is to retrieve t
+00012280: 6865 206a 6f62 5f69 6420 6672 6f6d 2074  he job_id from t
+00012290: 6865 0a20 2020 2020 2020 2020 2020 2023  he.            #
+000122a0: 2053 4b59 5049 4c4f 545f 5441 534b 5f49   SKYPILOT_TASK_I
+000122b0: 442c 2077 6869 6368 2067 6574 7320 7468  D, which gets th
+000122c0: 6520 7365 636f 6e64 2074 6f20 6c61 7374  e second to last
+000122d0: 2066 6965 6c64 0a20 2020 2020 2020 2020   field.         
+000122e0: 2020 2023 2073 6570 6172 6174 6564 2062     # separated b
+000122f0: 7920 602d 602e 0a20 2020 2020 2020 2020  y `-`..         
+00012300: 2020 2028 6627 5350 4f54 5f4a 4f42 5f49     (f'SPOT_JOB_I
+00012310: 443d 6063 6174 202f 746d 702f 7b6e 616d  D=`cat /tmp/{nam
+00012320: 657d 2d72 756e 2d69 6420 7c20 7265 7620  e}-run-id | rev 
+00012330: 7c20 270a 2020 2020 2020 2020 2020 2020  | '.            
+00012340: 2027 6375 7420 2d64 5c27 2d5c 2720 2d66   'cut -d\'-\' -f
+00012350: 3220 7c20 7265 7660 3b27 0a20 2020 2020  2 | rev`;'.     
+00012360: 2020 2020 2020 2020 6627 6177 7320 6563          f'aws ec
+00012370: 3220 7465 726d 696e 6174 652d 696e 7374  2 terminate-inst
+00012380: 616e 6365 7320 2d2d 7265 6769 6f6e 207b  ances --region {
+00012390: 7265 6769 6f6e 7d20 2d2d 696e 7374 616e  region} --instan
+000123a0: 6365 2d69 6473 2024 2827 0a20 2020 2020  ce-ids $('.     
+000123b0: 2020 2020 2020 2020 6627 6177 7320 6563          f'aws ec
+000123c0: 3220 6465 7363 7269 6265 2d69 6e73 7461  2 describe-insta
+000123d0: 6e63 6573 202d 2d72 6567 696f 6e20 7b72  nces --region {r
+000123e0: 6567 696f 6e7d 2027 0a20 2020 2020 2020  egion} '.       
+000123f0: 2020 2020 2020 272d 2d66 696c 7465 7273        '--filters
+00012400: 204e 616d 653d 7461 673a 7261 792d 636c   Name=tag:ray-cl
+00012410: 7573 7465 722d 6e61 6d65 2c56 616c 7565  uster-name,Value
+00012420: 733d 2a2d 247b 5350 4f54 5f4a 4f42 5f49  s=*-${SPOT_JOB_I
+00012430: 447d 2027 0a20 2020 2020 2020 2020 2020  D} '.           
+00012440: 2020 6627 2d2d 7175 6572 7920 5265 7365    f'--query Rese
+00012450: 7276 6174 696f 6e73 5b5d 2e49 6e73 7461  rvations[].Insta
+00012460: 6e63 6573 5b5d 2e49 6e73 7461 6e63 6549  nces[].InstanceI
+00012470: 6420 270a 2020 2020 2020 2020 2020 2020  d '.            
+00012480: 2027 2d2d 6f75 7470 7574 2074 6578 7429   '--output text)
+00012490: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+000124a0: 2773 6c65 6570 2031 3030 272c 0a20 2020  'sleep 100',.   
+000124b0: 2020 2020 2020 2020 2066 277b 5f53 504f           f'{_SPO
+000124c0: 545f 5155 4555 455f 5741 4954 7d7c 2067  T_QUEUE_WAIT}| g
+000124d0: 7265 7020 7b6e 616d 657d 207c 2068 6561  rep {name} | hea
+000124e0: 6420 2d6e 3120 7c20 6772 6570 2022 5245  d -n1 | grep "RE
+000124f0: 434f 5645 5249 4e47 2227 2c0a 2020 2020  COVERING"',.    
+00012500: 2020 2020 2020 2020 2773 6c65 6570 2032          'sleep 2
+00012510: 3030 272c 0a20 2020 2020 2020 2020 2020  00',.           
+00012520: 2066 277b 5f53 504f 545f 5155 4555 455f   f'{_SPOT_QUEUE_
+00012530: 5741 4954 7d7c 2067 7265 7020 7b6e 616d  WAIT}| grep {nam
+00012540: 657d 207c 2068 6561 6420 2d6e 3120 7c20  e} | head -n1 | 
+00012550: 6772 6570 2022 5255 4e4e 494e 4722 272c  grep "RUNNING"',
+00012560: 0a20 2020 2020 2020 2020 2020 2066 2752  .            f'R
+00012570: 554e 5f49 443d 2428 6361 7420 2f74 6d70  UN_ID=$(cat /tmp
+00012580: 2f7b 6e61 6d65 7d2d 7275 6e2d 6964 293b  /{name}-run-id);
+00012590: 2065 6368 6f20 2452 554e 5f49 443b 2073   echo $RUN_ID; s
+000125a0: 6b79 2073 706f 7420 6c6f 6773 202d 6e20  ky spot logs -n 
+000125b0: 7b6e 616d 657d 202d 2d6e 6f2d 666f 6c6c  {name} --no-foll
+000125c0: 6f77 207c 2067 7265 7020 534b 5950 494c  ow | grep SKYPIL
+000125d0: 4f54 5f54 4153 4b5f 4944 3a20 7c20 6772  OT_TASK_ID: | gr
+000125e0: 6570 2022 2452 554e 5f49 4422 272c 0a20  ep "$RUN_ID"',. 
+000125f0: 2020 2020 2020 2020 2020 2066 2752 554e             f'RUN
+00012600: 5f49 4453 3d24 2873 6b79 2073 706f 7420  _IDS=$(sky spot 
+00012610: 6c6f 6773 202d 6e20 7b6e 616d 657d 202d  logs -n {name} -
+00012620: 2d6e 6f2d 666f 6c6c 6f77 207c 2067 7265  -no-follow | gre
+00012630: 7020 2d41 2034 2053 4b59 5049 4c4f 545f  p -A 4 SKYPILOT_
+00012640: 5441 534b 5f49 4453 207c 2063 7574 202d  TASK_IDS | cut -
+00012650: 6422 2922 202d 6632 293b 2065 6368 6f20  d")" -f2); echo 
+00012660: 2224 5255 4e5f 4944 5322 207c 2074 6565  "$RUN_IDS" | tee
+00012670: 202f 746d 702f 7b6e 616d 657d 2d72 756e   /tmp/{name}-run
+00012680: 2d69 6473 2d6e 6577 272c 0a20 2020 2020  -ids-new',.     
+00012690: 2020 2020 2020 2066 2764 6966 6620 2f74         f'diff /t
+000126a0: 6d70 2f7b 6e61 6d65 7d2d 7275 6e2d 6964  mp/{name}-run-id
+000126b0: 7320 2f74 6d70 2f7b 6e61 6d65 7d2d 7275  s /tmp/{name}-ru
+000126c0: 6e2d 6964 732d 6e65 7727 2c0a 2020 2020  n-ids-new',.    
+000126d0: 2020 2020 2020 2020 6627 6361 7420 2f74          f'cat /t
+000126e0: 6d70 2f7b 6e61 6d65 7d2d 7275 6e2d 6964  mp/{name}-run-id
+000126f0: 7320 7c20 7365 6420 2d6e 2032 7020 7c20  s | sed -n 2p | 
+00012700: 6772 6570 2060 6361 7420 2f74 6d70 2f7b  grep `cat /tmp/{
+00012710: 6e61 6d65 7d2d 7275 6e2d 6964 6027 2c0a  name}-run-id`',.
+00012720: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00012730: 2020 205f 5350 4f54 5f43 414e 4345 4c5f     _SPOT_CANCEL_
+00012740: 5741 4954 2e66 6f72 6d61 7428 6a6f 625f  WAIT.format(job_
+00012750: 6e61 6d65 3d6e 616d 6529 2c0a 2020 2020  name=name),.    
+00012760: 2020 2020 7469 6d65 6f75 743d 3235 202a      timeout=25 *
+00012770: 2036 302c 0a20 2020 2029 0a20 2020 2072   60,.    ).    r
+00012780: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
+00012790: 290a 0a0a 4070 7974 6573 742e 6d61 726b  )...@pytest.mark
+000127a0: 2e67 6370 0a40 7079 7465 7374 2e6d 6172  .gcp.@pytest.mar
+000127b0: 6b2e 6d61 6e61 6765 645f 7370 6f74 0a64  k.managed_spot.d
+000127c0: 6566 2074 6573 745f 7370 6f74 5f70 6970  ef test_spot_pip
+000127d0: 656c 696e 655f 7265 636f 7665 7279 5f67  eline_recovery_g
+000127e0: 6370 2829 3a0a 2020 2020 2222 2254 6573  cp():.    """Tes
+000127f0: 7420 6d61 6e61 6765 6420 7370 6f74 2072  t managed spot r
+00012800: 6563 6f76 6572 7920 666f 7220 6120 7069  ecovery for a pi
+00012810: 7065 6c69 6e65 2e22 2222 0a20 2020 206e  peline.""".    n
+00012820: 616d 6520 3d20 5f67 6574 5f63 6c75 7374  ame = _get_clust
+00012830: 6572 5f6e 616d 6528 290a 2020 2020 7a6f  er_name().    zo
+00012840: 6e65 203d 2027 7573 2d65 6173 7434 2d62  ne = 'us-east4-b
+00012850: 270a 2020 2020 7175 6572 795f 636d 6420  '.    query_cmd 
+00012860: 3d20 2827 6763 6c6f 7564 2063 6f6d 7075  = ('gcloud compu
+00012870: 7465 2069 6e73 7461 6e63 6573 206c 6973  te instances lis
+00012880: 7420 2d2d 6669 6c74 6572 3d27 0a20 2020  t --filter='.   
+00012890: 2020 2020 2020 2020 2020 2020 2020 2722                '"
+000128a0: 286c 6162 656c 732e 7261 792d 636c 7573  (labels.ray-clus
+000128b0: 7465 722d 6e61 6d65 3a2a 2d24 7b53 504f  ter-name:*-${SPO
+000128c0: 545f 4a4f 425f 4944 7d29 2220 270a 2020  T_JOB_ID})" '.  
+000128d0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000128e0: 272d 2d7a 6f6e 6573 3d7b 7a6f 6e65 7d20  '--zones={zone} 
+000128f0: 2d2d 666f 726d 6174 3d22 7661 6c75 6528  --format="value(
+00012900: 6e61 6d65 2922 2729 0a20 2020 2074 6572  name)"').    ter
+00012910: 6d69 6e61 7465 5f63 6d64 203d 2028 6627  minate_cmd = (f'
+00012920: 6763 6c6f 7564 2063 6f6d 7075 7465 2069  gcloud compute i
+00012930: 6e73 7461 6e63 6573 2064 656c 6574 6520  nstances delete 
+00012940: 2d2d 7a6f 6e65 3d7b 7a6f 6e65 7d27 0a20  --zone={zone}'. 
+00012950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012960: 2020 2020 6627 202d 2d71 7569 6574 2024      f' --quiet $
+00012970: 287b 7175 6572 795f 636d 647d 2927 290a  ({query_cmd})').
+00012980: 2020 2020 7465 7374 203d 2054 6573 7428      test = Test(
+00012990: 0a20 2020 2020 2020 2027 7370 6f74 5f70  .        'spot_p
+000129a0: 6970 656c 696e 655f 7265 636f 7665 7279  ipeline_recovery
+000129b0: 5f67 6370 272c 0a20 2020 2020 2020 205b  _gcp',.        [
+000129c0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+000129d0: 6b79 2073 706f 7420 6c61 756e 6368 202d  ky spot launch -
+000129e0: 6e20 7b6e 616d 657d 2074 6573 7473 2f74  n {name} tests/t
+000129f0: 6573 745f 7961 6d6c 732f 7069 7065 6c69  est_yamls/pipeli
+00012a00: 6e65 5f67 6370 2e79 616d 6c20 202d 7920  ne_gcp.yaml  -y 
+00012a10: 2d64 272c 0a20 2020 2020 2020 2020 2020  -d',.           
+00012a20: 2027 736c 6565 7020 3430 3027 2c0a 2020   'sleep 400',.  
+00012a30: 2020 2020 2020 2020 2020 6627 7b5f 5350            f'{_SP
+00012a40: 4f54 5f51 5545 5545 5f57 4149 547d 7c20  OT_QUEUE_WAIT}| 
+00012a50: 6772 6570 207b 6e61 6d65 7d20 7c20 6865  grep {name} | he
+00012a60: 6164 202d 6e31 207c 2067 7265 7020 2252  ad -n1 | grep "R
+00012a70: 554e 4e49 4e47 2227 2c0a 2020 2020 2020  UNNING"',.      
+00012a80: 2020 2020 2020 6627 5255 4e5f 4944 3d24        f'RUN_ID=$
+00012a90: 2873 6b79 2073 706f 7420 6c6f 6773 202d  (sky spot logs -
+00012aa0: 6e20 7b6e 616d 657d 202d 2d6e 6f2d 666f  n {name} --no-fo
+00012ab0: 6c6c 6f77 207c 2067 7265 7020 534b 5950  llow | grep SKYP
+00012ac0: 494c 4f54 5f54 4153 4b5f 4944 3a20 7c20  ILOT_TASK_ID: | 
+00012ad0: 6375 7420 2d64 3a20 2d66 3229 3b20 6563  cut -d: -f2); ec
+00012ae0: 686f 2022 2452 554e 5f49 4422 207c 2074  ho "$RUN_ID" | t
+00012af0: 6565 202f 746d 702f 7b6e 616d 657d 2d72  ee /tmp/{name}-r
+00012b00: 756e 2d69 6427 2c0a 2020 2020 2020 2020  un-id',.        
+00012b10: 2020 2020 6627 5255 4e5f 4944 533d 2428      f'RUN_IDS=$(
+00012b20: 736b 7920 7370 6f74 206c 6f67 7320 2d6e  sky spot logs -n
+00012b30: 207b 6e61 6d65 7d20 2d2d 6e6f 2d66 6f6c   {name} --no-fol
+00012b40: 6c6f 7720 7c20 6772 6570 202d 4120 3420  low | grep -A 4 
+00012b50: 534b 5950 494c 4f54 5f54 4153 4b5f 4944  SKYPILOT_TASK_ID
+00012b60: 5320 7c20 6375 7420 2d64 2229 2220 2d66  S | cut -d")" -f
+00012b70: 3229 3b20 6563 686f 2022 2452 554e 5f49  2); echo "$RUN_I
+00012b80: 4453 2220 7c20 7465 6520 2f74 6d70 2f7b  DS" | tee /tmp/{
+00012b90: 6e61 6d65 7d2d 7275 6e2d 6964 7327 2c0a  name}-run-ids',.
+00012ba0: 2020 2020 2020 2020 2020 2020 2320 5465              # Te
+00012bb0: 726d 696e 6174 6520 7468 6520 636c 7573  rminate the clus
+00012bc0: 7465 7220 6d61 6e75 616c 6c79 2e0a 2020  ter manually..  
+00012bd0: 2020 2020 2020 2020 2020 2320 5468 6520            # The 
+00012be0: 6063 6174 202e 2e2e 7c20 7265 7660 2069  `cat ...| rev` i
+00012bf0: 7320 746f 2072 6574 7269 6576 6520 7468  s to retrieve th
+00012c00: 6520 6a6f 625f 6964 2066 726f 6d20 7468  e job_id from th
+00012c10: 650a 2020 2020 2020 2020 2020 2020 2320  e.            # 
+00012c20: 534b 5950 494c 4f54 5f54 4153 4b5f 4944  SKYPILOT_TASK_ID
+00012c30: 2c20 7768 6963 6820 6765 7473 2074 6865  , which gets the
+00012c40: 2073 6563 6f6e 6420 746f 206c 6173 7420   second to last 
+00012c50: 6669 656c 640a 2020 2020 2020 2020 2020  field.          
+00012c60: 2020 2320 7365 7061 7261 7465 6420 6279    # separated by
+00012c70: 2060 2d60 2e0a 2020 2020 2020 2020 2020   `-`..          
+00012c80: 2020 2866 2753 504f 545f 4a4f 425f 4944    (f'SPOT_JOB_ID
+00012c90: 3d60 6361 7420 2f74 6d70 2f7b 6e61 6d65  =`cat /tmp/{name
+00012ca0: 7d2d 7275 6e2d 6964 207c 2072 6576 207c  }-run-id | rev |
+00012cb0: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+00012cc0: 6627 6375 7420 2d64 5c27 2d5c 2720 2d66  f'cut -d\'-\' -f
+00012cd0: 3220 7c20 7265 7660 3b7b 7465 726d 696e  2 | rev`;{termin
+00012ce0: 6174 655f 636d 647d 2729 2c0a 2020 2020  ate_cmd}'),.    
+00012cf0: 2020 2020 2020 2020 2773 6c65 6570 2031          'sleep 1
+00012d00: 3030 272c 0a20 2020 2020 2020 2020 2020  00',.           
+00012d10: 2066 277b 5f53 504f 545f 5155 4555 455f   f'{_SPOT_QUEUE_
+00012d20: 5741 4954 7d7c 2067 7265 7020 7b6e 616d  WAIT}| grep {nam
+00012d30: 657d 207c 2068 6561 6420 2d6e 3120 7c20  e} | head -n1 | 
+00012d40: 6772 6570 2022 5245 434f 5645 5249 4e47  grep "RECOVERING
+00012d50: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
+00012d60: 2773 6c65 6570 2032 3030 272c 0a20 2020  'sleep 200',.   
+00012d70: 2020 2020 2020 2020 2066 277b 5f53 504f           f'{_SPO
+00012d80: 545f 5155 4555 455f 5741 4954 7d7c 2067  T_QUEUE_WAIT}| g
+00012d90: 7265 7020 7b6e 616d 657d 207c 2068 6561  rep {name} | hea
+00012da0: 6420 2d6e 3120 7c20 6772 6570 2022 5255  d -n1 | grep "RU
+00012db0: 4e4e 494e 4722 272c 0a20 2020 2020 2020  NNING"',.       
+00012dc0: 2020 2020 2066 2752 554e 5f49 443d 2428       f'RUN_ID=$(
+00012dd0: 6361 7420 2f74 6d70 2f7b 6e61 6d65 7d2d  cat /tmp/{name}-
+00012de0: 7275 6e2d 6964 293b 2065 6368 6f20 2452  run-id); echo $R
+00012df0: 554e 5f49 443b 2073 6b79 2073 706f 7420  UN_ID; sky spot 
+00012e00: 6c6f 6773 202d 6e20 7b6e 616d 657d 202d  logs -n {name} -
+00012e10: 2d6e 6f2d 666f 6c6c 6f77 207c 2067 7265  -no-follow | gre
+00012e20: 7020 534b 5950 494c 4f54 5f54 4153 4b5f  p SKYPILOT_TASK_
+00012e30: 4944 3a20 7c20 6772 6570 2022 2452 554e  ID: | grep "$RUN
+00012e40: 5f49 4422 272c 0a20 2020 2020 2020 2020  _ID"',.         
+00012e50: 2020 2066 2752 554e 5f49 4453 3d24 2873     f'RUN_IDS=$(s
+00012e60: 6b79 2073 706f 7420 6c6f 6773 202d 6e20  ky spot logs -n 
+00012e70: 7b6e 616d 657d 202d 2d6e 6f2d 666f 6c6c  {name} --no-foll
+00012e80: 6f77 207c 2067 7265 7020 2d41 2034 2053  ow | grep -A 4 S
+00012e90: 4b59 5049 4c4f 545f 5441 534b 5f49 4453  KYPILOT_TASK_IDS
+00012ea0: 207c 2063 7574 202d 6422 2922 202d 6632   | cut -d")" -f2
+00012eb0: 293b 2065 6368 6f20 2224 5255 4e5f 4944  ); echo "$RUN_ID
+00012ec0: 5322 207c 2074 6565 202f 746d 702f 7b6e  S" | tee /tmp/{n
+00012ed0: 616d 657d 2d72 756e 2d69 6473 2d6e 6577  ame}-run-ids-new
+00012ee0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+00012ef0: 2764 6966 6620 2f74 6d70 2f7b 6e61 6d65  'diff /tmp/{name
+00012f00: 7d2d 7275 6e2d 6964 7320 2f74 6d70 2f7b  }-run-ids /tmp/{
+00012f10: 6e61 6d65 7d2d 7275 6e2d 6964 732d 6e65  name}-run-ids-ne
+00012f20: 7727 2c0a 2020 2020 2020 2020 2020 2020  w',.            
+00012f30: 6627 6361 7420 2f74 6d70 2f7b 6e61 6d65  f'cat /tmp/{name
+00012f40: 7d2d 7275 6e2d 6964 7320 7c20 7365 6420  }-run-ids | sed 
+00012f50: 2d6e 2032 7020 7c20 6772 6570 2060 6361  -n 2p | grep `ca
+00012f60: 7420 2f74 6d70 2f7b 6e61 6d65 7d2d 7275  t /tmp/{name}-ru
+00012f70: 6e2d 6964 6027 2c0a 2020 2020 2020 2020  n-id`',.        
+00012f80: 5d2c 0a20 2020 2020 2020 205f 5350 4f54  ],.        _SPOT
+00012f90: 5f43 414e 4345 4c5f 5741 4954 2e66 6f72  _CANCEL_WAIT.for
+00012fa0: 6d61 7428 6a6f 625f 6e61 6d65 3d6e 616d  mat(job_name=nam
+00012fb0: 6529 2c0a 2020 2020 2020 2020 7469 6d65  e),.        time
+00012fc0: 6f75 743d 3235 202a 2036 302c 0a20 2020  out=25 * 60,.   
+00012fd0: 2029 0a20 2020 2072 756e 5f6f 6e65 5f74   ).    run_one_t
+00012fe0: 6573 7428 7465 7374 290a 0a0a 4070 7974  est(test)...@pyt
+00012ff0: 6573 742e 6d61 726b 2e6e 6f5f 6c61 6d62  est.mark.no_lamb
+00013000: 6461 5f63 6c6f 7564 2020 2320 4c61 6d62  da_cloud  # Lamb
+00013010: 6461 2043 6c6f 7564 2064 6f65 7320 6e6f  da Cloud does no
+00013020: 7420 7375 7070 6f72 7420 7370 6f74 2069  t support spot i
+00013030: 6e73 7461 6e63 6573 0a40 7079 7465 7374  nstances.@pytest
+00013040: 2e6d 6172 6b2e 6e6f 5f69 626d 2020 2320  .mark.no_ibm  # 
+00013050: 4942 4d20 436c 6f75 6420 646f 6573 206e  IBM Cloud does n
+00013060: 6f74 2073 7570 706f 7274 2073 706f 7420  ot support spot 
+00013070: 696e 7374 616e 6365 730a 4070 7974 6573  instances.@pytes
+00013080: 742e 6d61 726b 2e6e 6f5f 7363 7020 2023  t.mark.no_scp  #
+00013090: 2053 4350 2064 6f65 7320 6e6f 7420 7375   SCP does not su
+000130a0: 7070 6f72 7420 7370 6f74 2069 6e73 7461  pport spot insta
+000130b0: 6e63 6573 0a40 7079 7465 7374 2e6d 6172  nces.@pytest.mar
+000130c0: 6b2e 6d61 6e61 6765 645f 7370 6f74 0a64  k.managed_spot.d
+000130d0: 6566 2074 6573 745f 7370 6f74 5f72 6563  ef test_spot_rec
+000130e0: 6f76 6572 795f 6465 6661 756c 745f 7265  overy_default_re
+000130f0: 736f 7572 6365 7328 6765 6e65 7269 635f  sources(generic_
+00013100: 636c 6f75 643a 2073 7472 293a 0a20 2020  cloud: str):.   
+00013110: 2022 2222 5465 7374 206d 616e 6167 6564   """Test managed
+00013120: 2073 706f 7420 7265 636f 7665 7279 2066   spot recovery f
+00013130: 6f72 2064 6566 6175 6c74 2072 6573 6f75  or default resou
+00013140: 7263 6573 2e22 2222 0a20 2020 206e 616d  rces.""".    nam
+00013150: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
+00013160: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
+00013170: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
+00013180: 2027 6d61 6e61 6765 642d 7370 6f74 2d72   'managed-spot-r
+00013190: 6563 6f76 6572 792d 6465 6661 756c 742d  ecovery-default-
+000131a0: 7265 736f 7572 6365 7327 2c0a 2020 2020  resources',.    
+000131b0: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+000131c0: 2020 6627 736b 7920 7370 6f74 206c 6175    f'sky spot lau
+000131d0: 6e63 6820 2d6e 207b 6e61 6d65 7d20 2d2d  nch -n {name} --
+000131e0: 636c 6f75 6420 7b67 656e 6572 6963 5f63  cloud {generic_c
+000131f0: 6c6f 7564 7d20 2273 6c65 6570 2033 3020  loud} "sleep 30 
+00013200: 2626 2073 7564 6f20 7368 7574 646f 776e  && sudo shutdown
+00013210: 206e 6f77 2026 2620 736c 6565 7020 3130   now && sleep 10
+00013220: 3030 2220 2d79 202d 6427 2c0a 2020 2020  00" -y -d',.    
+00013230: 2020 2020 2020 2020 2773 6c65 6570 2033          'sleep 3
+00013240: 3630 272c 0a20 2020 2020 2020 2020 2020  60',.           
+00013250: 2066 277b 5f53 504f 545f 5155 4555 455f   f'{_SPOT_QUEUE_
+00013260: 5741 4954 7d7c 2067 7265 7020 7b6e 616d  WAIT}| grep {nam
+00013270: 657d 207c 2068 6561 6420 2d6e 3120 7c20  e} | head -n1 | 
+00013280: 6772 6570 2022 5255 4e4e 494e 475c 7c52  grep "RUNNING\|R
+00013290: 4543 4f56 4552 494e 4722 272c 0a20 2020  ECOVERING"',.   
+000132a0: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+000132b0: 5f53 504f 545f 4341 4e43 454c 5f57 4149  _SPOT_CANCEL_WAI
+000132c0: 542e 666f 726d 6174 286a 6f62 5f6e 616d  T.format(job_nam
+000132d0: 653d 6e61 6d65 292c 0a20 2020 2020 2020  e=name),.       
+000132e0: 2074 696d 656f 7574 3d32 3520 2a20 3630   timeout=25 * 60
+000132f0: 2c0a 2020 2020 290a 2020 2020 7275 6e5f  ,.    ).    run_
+00013300: 6f6e 655f 7465 7374 2874 6573 7429 0a0a  one_test(test)..
+00013310: 0a40 7079 7465 7374 2e6d 6172 6b2e 6177  .@pytest.mark.aw
+00013320: 730a 4070 7974 6573 742e 6d61 726b 2e6d  s.@pytest.mark.m
+00013330: 616e 6167 6564 5f73 706f 740a 6465 6620  anaged_spot.def 
+00013340: 7465 7374 5f73 706f 745f 7265 636f 7665  test_spot_recove
+00013350: 7279 5f6d 756c 7469 5f6e 6f64 655f 6177  ry_multi_node_aw
+00013360: 7328 6177 735f 636f 6e66 6967 5f72 6567  s(aws_config_reg
+00013370: 696f 6e29 3a0a 2020 2020 2222 2254 6573  ion):.    """Tes
+00013380: 7420 6d61 6e61 6765 6420 7370 6f74 2072  t managed spot r
+00013390: 6563 6f76 6572 792e 2222 220a 2020 2020  ecovery.""".    
+000133a0: 6e61 6d65 203d 205f 6765 745f 636c 7573  name = _get_clus
+000133b0: 7465 725f 6e61 6d65 2829 0a20 2020 2072  ter_name().    r
+000133c0: 6567 696f 6e20 3d20 6177 735f 636f 6e66  egion = aws_conf
+000133d0: 6967 5f72 6567 696f 6e0a 2020 2020 7465  ig_region.    te
+000133e0: 7374 203d 2054 6573 7428 0a20 2020 2020  st = Test(.     
+000133f0: 2020 2027 7370 6f74 5f72 6563 6f76 6572     'spot_recover
+00013400: 795f 6d75 6c74 695f 6e6f 6465 5f61 7773  y_multi_node_aws
+00013410: 272c 0a20 2020 2020 2020 205b 0a20 2020  ',.        [.   
+00013420: 2020 2020 2020 2020 2066 2773 6b79 2073           f'sky s
+00013430: 706f 7420 6c61 756e 6368 202d 2d63 6c6f  pot launch --clo
+00013440: 7564 2061 7773 202d 2d72 6567 696f 6e20  ud aws --region 
+00013450: 7b72 6567 696f 6e7d 202d 6e20 7b6e 616d  {region} -n {nam
+00013460: 657d 202d 2d6e 756d 2d6e 6f64 6573 2032  e} --num-nodes 2
+00013470: 2022 6563 686f 2053 4b59 5049 4c4f 545f   "echo SKYPILOT_
+00013480: 5441 534b 5f49 443a 205c 2453 4b59 5049  TASK_ID: \$SKYPI
+00013490: 4c4f 545f 5441 534b 5f49 443b 2073 6c65  LOT_TASK_ID; sle
+000134a0: 6570 2031 3830 3022 2020 2d79 202d 6427  ep 1800"  -y -d'
+000134b0: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
+000134c0: 6c65 6570 2034 3530 272c 0a20 2020 2020  leep 450',.     
+000134d0: 2020 2020 2020 2066 277b 5f53 504f 545f         f'{_SPOT_
+000134e0: 5155 4555 455f 5741 4954 7d7c 2067 7265  QUEUE_WAIT}| gre
+000134f0: 7020 7b6e 616d 657d 207c 2068 6561 6420  p {name} | head 
+00013500: 2d6e 3120 7c20 6772 6570 2022 5255 4e4e  -n1 | grep "RUNN
+00013510: 494e 4722 272c 0a20 2020 2020 2020 2020  ING"',.         
+00013520: 2020 2066 2752 554e 5f49 443d 2428 736b     f'RUN_ID=$(sk
+00013530: 7920 7370 6f74 206c 6f67 7320 2d6e 207b  y spot logs -n {
+00013540: 6e61 6d65 7d20 2d2d 6e6f 2d66 6f6c 6c6f  name} --no-follo
+00013550: 7720 7c20 6772 6570 2053 4b59 5049 4c4f  w | grep SKYPILO
+00013560: 545f 5441 534b 5f49 4420 7c20 6375 7420  T_TASK_ID | cut 
+00013570: 2d64 3a20 2d66 3229 3b20 6563 686f 2022  -d: -f2); echo "
+00013580: 2452 554e 5f49 4422 207c 2074 6565 202f  $RUN_ID" | tee /
+00013590: 746d 702f 7b6e 616d 657d 2d72 756e 2d69  tmp/{name}-run-i
+000135a0: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
+000135b0: 2320 5465 726d 696e 6174 6520 7468 6520  # Terminate the 
+000135c0: 776f 726b 6572 206d 616e 7561 6c6c 792e  worker manually.
+000135d0: 0a20 2020 2020 2020 2020 2020 2028 6627  .            (f'
+000135e0: 6177 7320 6563 3220 7465 726d 696e 6174  aws ec2 terminat
+000135f0: 652d 696e 7374 616e 6365 7320 2d2d 7265  e-instances --re
+00013600: 6769 6f6e 207b 7265 6769 6f6e 7d20 2d2d  gion {region} --
+00013610: 696e 7374 616e 6365 2d69 6473 2024 2827  instance-ids $('
+00013620: 0a20 2020 2020 2020 2020 2020 2020 6627  .             f'
+00013630: 6177 7320 6563 3220 6465 7363 7269 6265  aws ec2 describe
+00013640: 2d69 6e73 7461 6e63 6573 202d 2d72 6567  -instances --reg
+00013650: 696f 6e20 7b72 6567 696f 6e7d 2027 0a20  ion {region} '. 
+00013660: 2020 2020 2020 2020 2020 2020 6627 2d2d              f'--
+00013670: 6669 6c74 6572 7320 4e61 6d65 3d74 6167  filters Name=tag
+00013680: 3a72 6179 2d63 6c75 7374 6572 2d6e 616d  :ray-cluster-nam
+00013690: 652c 5661 6c75 6573 3d7b 6e61 6d65 7d2a  e,Values={name}*
+000136a0: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+000136b0: 274e 616d 653d 7461 673a 7261 792d 6e6f  'Name=tag:ray-no
+000136c0: 6465 2d74 7970 652c 5661 6c75 6573 3d77  de-type,Values=w
+000136d0: 6f72 6b65 7220 270a 2020 2020 2020 2020  orker '.        
+000136e0: 2020 2020 2066 272d 2d71 7565 7279 2052       f'--query R
+000136f0: 6573 6572 7661 7469 6f6e 735b 5d2e 496e  eservations[].In
+00013700: 7374 616e 6365 735b 5d2e 496e 7374 616e  stances[].Instan
+00013710: 6365 4964 2027 0a20 2020 2020 2020 2020  ceId '.         
+00013720: 2020 2020 272d 2d6f 7574 7075 7420 7465      '--output te
+00013730: 7874 2927 292c 0a20 2020 2020 2020 2020  xt)'),.         
+00013740: 2020 2027 736c 6565 7020 3530 272c 0a20     'sleep 50',. 
+00013750: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
+00013760: 504f 545f 5155 4555 455f 5741 4954 7d7c  POT_QUEUE_WAIT}|
+00013770: 2067 7265 7020 7b6e 616d 657d 207c 2068   grep {name} | h
+00013780: 6561 6420 2d6e 3120 7c20 6772 6570 2022  ead -n1 | grep "
+00013790: 5245 434f 5645 5249 4e47 2227 2c0a 2020  RECOVERING"',.  
+000137a0: 2020 2020 2020 2020 2020 2773 6c65 6570            'sleep
+000137b0: 2035 3630 272c 0a20 2020 2020 2020 2020   560',.         
+000137c0: 2020 2066 277b 5f53 504f 545f 5155 4555     f'{_SPOT_QUEU
+000137d0: 455f 5741 4954 7d7c 2067 7265 7020 7b6e  E_WAIT}| grep {n
+000137e0: 616d 657d 207c 2068 6561 6420 2d6e 3120  ame} | head -n1 
+000137f0: 7c20 6772 6570 2022 5255 4e4e 494e 4722  | grep "RUNNING"
+00013800: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+00013810: 2752 554e 5f49 443d 2428 6361 7420 2f74  'RUN_ID=$(cat /t
+00013820: 6d70 2f7b 6e61 6d65 7d2d 7275 6e2d 6964  mp/{name}-run-id
+00013830: 293b 2065 6368 6f20 2452 554e 5f49 443b  ); echo $RUN_ID;
+00013840: 2073 6b79 2073 706f 7420 6c6f 6773 202d   sky spot logs -
+00013850: 6e20 7b6e 616d 657d 202d 2d6e 6f2d 666f  n {name} --no-fo
+00013860: 6c6c 6f77 207c 2067 7265 7020 534b 5950  llow | grep SKYP
+00013870: 494c 4f54 5f54 4153 4b5f 4944 207c 2063  ILOT_TASK_ID | c
+00013880: 7574 202d 643a 202d 6632 207c 2067 7265  ut -d: -f2 | gre
+00013890: 7020 2224 5255 4e5f 4944 2227 2c0a 2020  p "$RUN_ID"',.  
+000138a0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+000138b0: 205f 5350 4f54 5f43 414e 4345 4c5f 5741   _SPOT_CANCEL_WA
+000138c0: 4954 2e66 6f72 6d61 7428 6a6f 625f 6e61  IT.format(job_na
+000138d0: 6d65 3d6e 616d 6529 2c0a 2020 2020 2020  me=name),.      
+000138e0: 2020 7469 6d65 6f75 743d 3330 202a 2036    timeout=30 * 6
+000138f0: 302c 0a20 2020 2029 0a20 2020 2072 756e  0,.    ).    run
+00013900: 5f6f 6e65 5f74 6573 7428 7465 7374 290a  _one_test(test).
+00013910: 0a0a 4070 7974 6573 742e 6d61 726b 2e67  ..@pytest.mark.g
+00013920: 6370 0a40 7079 7465 7374 2e6d 6172 6b2e  cp.@pytest.mark.
+00013930: 6d61 6e61 6765 645f 7370 6f74 0a64 6566  managed_spot.def
+00013940: 2074 6573 745f 7370 6f74 5f72 6563 6f76   test_spot_recov
+00013950: 6572 795f 6d75 6c74 695f 6e6f 6465 5f67  ery_multi_node_g
+00013960: 6370 2829 3a0a 2020 2020 2222 2254 6573  cp():.    """Tes
+00013970: 7420 6d61 6e61 6765 6420 7370 6f74 2072  t managed spot r
+00013980: 6563 6f76 6572 792e 2222 220a 2020 2020  ecovery.""".    
+00013990: 6e61 6d65 203d 205f 6765 745f 636c 7573  name = _get_clus
+000139a0: 7465 725f 6e61 6d65 2829 0a20 2020 207a  ter_name().    z
+000139b0: 6f6e 6520 3d20 2775 732d 7765 7374 322d  one = 'us-west2-
+000139c0: 6127 0a20 2020 2023 2055 7365 2027 3a27  a'.    # Use ':'
+000139d0: 2074 6f20 6d61 7463 6820 6173 2074 6865   to match as the
+000139e0: 2063 6c75 7374 6572 206e 616d 6520 7769   cluster name wi
+000139f0: 6c6c 2063 6f6e 7461 696e 2074 6865 2073  ll contain the s
+00013a00: 7566 6669 7820 7769 7468 206a 6f62 2069  uffix with job i
+00013a10: 640a 2020 2020 7175 6572 795f 636d 6420  d.    query_cmd 
+00013a20: 3d20 280a 2020 2020 2020 2020 6627 6763  = (.        f'gc
+00013a30: 6c6f 7564 2063 6f6d 7075 7465 2069 6e73  loud compute ins
+00013a40: 7461 6e63 6573 206c 6973 7420 2d2d 6669  tances list --fi
+00013a50: 6c74 6572 3d27 0a20 2020 2020 2020 2066  lter='.        f
+00013a60: 2722 286c 6162 656c 732e 7261 792d 636c  '"(labels.ray-cl
+00013a70: 7573 7465 722d 6e61 6d65 3a7b 6e61 6d65  uster-name:{name
+00013a80: 7d20 414e 4420 6c61 6265 6c73 2e72 6179  } AND labels.ray
+00013a90: 2d6e 6f64 652d 7479 7065 3d77 6f72 6b65  -node-type=worke
+00013aa0: 7229 2220 270a 2020 2020 2020 2020 6627  r)" '.        f'
+00013ab0: 2d2d 7a6f 6e65 733d 7b7a 6f6e 657d 202d  --zones={zone} -
+00013ac0: 2d66 6f72 6d61 743d 2276 616c 7565 286e  -format="value(n
+00013ad0: 616d 6529 2227 290a 2020 2020 7465 726d  ame)"').    term
+00013ae0: 696e 6174 655f 636d 6420 3d20 2866 2767  inate_cmd = (f'g
+00013af0: 636c 6f75 6420 636f 6d70 7574 6520 696e  cloud compute in
+00013b00: 7374 616e 6365 7320 6465 6c65 7465 202d  stances delete -
+00013b10: 2d7a 6f6e 653d 7b7a 6f6e 657d 270a 2020  -zone={zone}'.  
+00013b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b30: 2020 2066 2720 2d2d 7175 6965 7420 2428     f' --quiet $(
+00013b40: 7b71 7565 7279 5f63 6d64 7d29 2729 0a20  {query_cmd})'). 
+00013b50: 2020 2074 6573 7420 3d20 5465 7374 280a     test = Test(.
+00013b60: 2020 2020 2020 2020 2773 706f 745f 7265          'spot_re
+00013b70: 636f 7665 7279 5f6d 756c 7469 5f6e 6f64  covery_multi_nod
+00013b80: 655f 6763 7027 2c0a 2020 2020 2020 2020  e_gcp',.        
+00013b90: 5b0a 2020 2020 2020 2020 2020 2020 6627  [.            f'
+00013ba0: 736b 7920 7370 6f74 206c 6175 6e63 6820  sky spot launch 
+00013bb0: 2d2d 636c 6f75 6420 6763 7020 2d2d 7a6f  --cloud gcp --zo
+00013bc0: 6e65 207b 7a6f 6e65 7d20 2d6e 207b 6e61  ne {zone} -n {na
+00013bd0: 6d65 7d20 2d2d 6e75 6d2d 6e6f 6465 7320  me} --num-nodes 
+00013be0: 3220 2265 6368 6f20 534b 5950 494c 4f54  2 "echo SKYPILOT
+00013bf0: 5f54 4153 4b5f 4944 3a20 5c24 534b 5950  _TASK_ID: \$SKYP
+00013c00: 494c 4f54 5f54 4153 4b5f 4944 3b20 736c  ILOT_TASK_ID; sl
+00013c10: 6565 7020 3138 3030 2220 202d 7920 2d64  eep 1800"  -y -d
+00013c20: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
+00013c30: 736c 6565 7020 3430 3027 2c0a 2020 2020  sleep 400',.    
+00013c40: 2020 2020 2020 2020 6627 7b5f 5350 4f54          f'{_SPOT
+00013c50: 5f51 5545 5545 5f57 4149 547d 7c20 6772  _QUEUE_WAIT}| gr
+00013c60: 6570 207b 6e61 6d65 7d20 7c20 6865 6164  ep {name} | head
+00013c70: 202d 6e31 207c 2067 7265 7020 2252 554e   -n1 | grep "RUN
+00013c80: 4e49 4e47 2227 2c0a 2020 2020 2020 2020  NING"',.        
+00013c90: 2020 2020 6627 5255 4e5f 4944 3d24 2873      f'RUN_ID=$(s
+00013ca0: 6b79 2073 706f 7420 6c6f 6773 202d 6e20  ky spot logs -n 
+00013cb0: 7b6e 616d 657d 202d 2d6e 6f2d 666f 6c6c  {name} --no-foll
+00013cc0: 6f77 207c 2067 7265 7020 534b 5950 494c  ow | grep SKYPIL
+00013cd0: 4f54 5f54 4153 4b5f 4944 207c 2063 7574  OT_TASK_ID | cut
+00013ce0: 202d 643a 202d 6632 293b 2065 6368 6f20   -d: -f2); echo 
+00013cf0: 2224 5255 4e5f 4944 2220 7c20 7465 6520  "$RUN_ID" | tee 
+00013d00: 2f74 6d70 2f7b 6e61 6d65 7d2d 7275 6e2d  /tmp/{name}-run-
+00013d10: 6964 272c 0a20 2020 2020 2020 2020 2020  id',.           
+00013d20: 2023 2054 6572 6d69 6e61 7465 2074 6865   # Terminate the
+00013d30: 2077 6f72 6b65 7220 6d61 6e75 616c 6c79   worker manually
+00013d40: 2e0a 2020 2020 2020 2020 2020 2020 7465  ..            te
+00013d50: 726d 696e 6174 655f 636d 642c 0a20 2020  rminate_cmd,.   
+00013d60: 2020 2020 2020 2020 2027 736c 6565 7020           'sleep 
+00013d70: 3530 272c 0a20 2020 2020 2020 2020 2020  50',.           
+00013d80: 2066 277b 5f53 504f 545f 5155 4555 455f   f'{_SPOT_QUEUE_
+00013d90: 5741 4954 7d7c 2067 7265 7020 7b6e 616d  WAIT}| grep {nam
+00013da0: 657d 207c 2068 6561 6420 2d6e 3120 7c20  e} | head -n1 | 
+00013db0: 6772 6570 2022 5245 434f 5645 5249 4e47  grep "RECOVERING
+00013dc0: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
+00013dd0: 2773 6c65 6570 2034 3230 272c 0a20 2020  'sleep 420',.   
+00013de0: 2020 2020 2020 2020 2066 277b 5f53 504f           f'{_SPO
+00013df0: 545f 5155 4555 455f 5741 4954 7d7c 2067  T_QUEUE_WAIT}| g
+00013e00: 7265 7020 7b6e 616d 657d 207c 2068 6561  rep {name} | hea
+00013e10: 6420 2d6e 3120 7c20 6772 6570 2022 5255  d -n1 | grep "RU
+00013e20: 4e4e 494e 4722 272c 0a20 2020 2020 2020  NNING"',.       
+00013e30: 2020 2020 2066 2752 554e 5f49 443d 2428       f'RUN_ID=$(
+00013e40: 6361 7420 2f74 6d70 2f7b 6e61 6d65 7d2d  cat /tmp/{name}-
+00013e50: 7275 6e2d 6964 293b 2065 6368 6f20 2452  run-id); echo $R
+00013e60: 554e 5f49 443b 2073 6b79 2073 706f 7420  UN_ID; sky spot 
+00013e70: 6c6f 6773 202d 6e20 7b6e 616d 657d 202d  logs -n {name} -
+00013e80: 2d6e 6f2d 666f 6c6c 6f77 207c 2067 7265  -no-follow | gre
+00013e90: 7020 534b 5950 494c 4f54 5f54 4153 4b5f  p SKYPILOT_TASK_
+00013ea0: 4944 207c 2063 7574 202d 643a 202d 6632  ID | cut -d: -f2
+00013eb0: 207c 2067 7265 7020 2224 5255 4e5f 4944   | grep "$RUN_ID
+00013ec0: 2227 2c0a 2020 2020 2020 2020 5d2c 0a20  "',.        ],. 
+00013ed0: 2020 2020 2020 205f 5350 4f54 5f43 414e         _SPOT_CAN
+00013ee0: 4345 4c5f 5741 4954 2e66 6f72 6d61 7428  CEL_WAIT.format(
+00013ef0: 6a6f 625f 6e61 6d65 3d6e 616d 6529 2c0a  job_name=name),.
+00013f00: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
+00013f10: 3235 202a 2036 302c 0a20 2020 2029 0a20  25 * 60,.    ). 
+00013f20: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
+00013f30: 7465 7374 290a 0a0a 4070 7974 6573 742e  test)...@pytest.
+00013f40: 6d61 726b 2e61 7773 0a40 7079 7465 7374  mark.aws.@pytest
+00013f50: 2e6d 6172 6b2e 6d61 6e61 6765 645f 7370  .mark.managed_sp
+00013f60: 6f74 0a64 6566 2074 6573 745f 7370 6f74  ot.def test_spot
+00013f70: 5f63 616e 6365 6c6c 6174 696f 6e5f 6177  _cancellation_aw
+00013f80: 7328 6177 735f 636f 6e66 6967 5f72 6567  s(aws_config_reg
+00013f90: 696f 6e29 3a0a 2020 2020 6e61 6d65 203d  ion):.    name =
+00013fa0: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
+00013fb0: 6d65 2829 0a20 2020 2072 6567 696f 6e20  me().    region 
+00013fc0: 3d20 6177 735f 636f 6e66 6967 5f72 6567  = aws_config_reg
+00013fd0: 696f 6e0a 2020 2020 7465 7374 203d 2054  ion.    test = T
+00013fe0: 6573 7428 0a20 2020 2020 2020 2027 7370  est(.        'sp
+00013ff0: 6f74 5f63 616e 6365 6c6c 6174 696f 6e5f  ot_cancellation_
+00014000: 6177 7327 2c0a 2020 2020 2020 2020 5b0a  aws',.        [.
+00014010: 2020 2020 2020 2020 2020 2020 2320 5465              # Te
+00014020: 7374 2063 616e 6365 6c6c 6174 696f 6e20  st cancellation 
+00014030: 6475 7269 6e67 2073 706f 7420 636c 7573  during spot clus
+00014040: 7465 7220 6265 696e 6720 6c61 756e 6368  ter being launch
+00014050: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+00014060: 6627 736b 7920 7370 6f74 206c 6175 6e63  f'sky spot launc
+00014070: 6820 2d2d 636c 6f75 6420 6177 7320 2d2d  h --cloud aws --
+00014080: 7265 6769 6f6e 207b 7265 6769 6f6e 7d20  region {region} 
+00014090: 2d6e 207b 6e61 6d65 7d20 2273 6c65 6570  -n {name} "sleep
+000140a0: 2031 3030 3022 2020 2d79 202d 6427 2c0a   1000"  -y -d',.
+000140b0: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
+000140c0: 6570 2036 3027 2c0a 2020 2020 2020 2020  ep 60',.        
+000140d0: 2020 2020 6627 7b5f 5350 4f54 5f51 5545      f'{_SPOT_QUE
+000140e0: 5545 5f57 4149 547d 7c20 6772 6570 207b  UE_WAIT}| grep {
+000140f0: 6e61 6d65 7d20 7c20 6865 6164 202d 6e31  name} | head -n1
+00014100: 207c 2067 7265 7020 2253 5441 5254 494e   | grep "STARTIN
+00014110: 4722 272c 0a20 2020 2020 2020 2020 2020  G"',.           
+00014120: 205f 5350 4f54 5f43 414e 4345 4c5f 5741   _SPOT_CANCEL_WA
+00014130: 4954 2e66 6f72 6d61 7428 6a6f 625f 6e61  IT.format(job_na
+00014140: 6d65 3d6e 616d 6529 2c0a 2020 2020 2020  me=name),.      
+00014150: 2020 2020 2020 2773 6c65 6570 2035 272c        'sleep 5',
+00014160: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
+00014170: 5f53 504f 545f 5155 4555 455f 5741 4954  _SPOT_QUEUE_WAIT
+00014180: 7d7c 2067 7265 7020 7b6e 616d 657d 207c  }| grep {name} |
+00014190: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
+000141a0: 2022 4341 4e43 454c 4c49 4e47 5c7c 4341   "CANCELLING\|CA
+000141b0: 4e43 454c 4c45 4422 272c 0a20 2020 2020  NCELLED"',.     
+000141c0: 2020 2020 2020 2027 736c 6565 7020 3132         'sleep 12
+000141d0: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
+000141e0: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
+000141f0: 4149 547d 7c20 6772 6570 207b 6e61 6d65  AIT}| grep {name
+00014200: 7d20 7c20 6865 6164 202d 6e31 207c 2067  } | head -n1 | g
+00014210: 7265 7020 2243 414e 4345 4c4c 4544 2227  rep "CANCELLED"'
+00014220: 2c0a 2020 2020 2020 2020 2020 2020 2866  ,.            (f
+00014230: 2773 3d24 2861 7773 2065 6332 2064 6573  's=$(aws ec2 des
+00014240: 6372 6962 652d 696e 7374 616e 6365 7320  cribe-instances 
+00014250: 2d2d 7265 6769 6f6e 207b 7265 6769 6f6e  --region {region
+00014260: 7d20 270a 2020 2020 2020 2020 2020 2020  } '.            
+00014270: 2066 272d 2d66 696c 7465 7273 204e 616d   f'--filters Nam
+00014280: 653d 7461 673a 7261 792d 636c 7573 7465  e=tag:ray-cluste
+00014290: 722d 6e61 6d65 2c56 616c 7565 733d 7b6e  r-name,Values={n
+000142a0: 616d 657d 2d2a 2027 0a20 2020 2020 2020  ame}-* '.       
+000142b0: 2020 2020 2020 6627 2d2d 7175 6572 7920        f'--query 
+000142c0: 5265 7365 7276 6174 696f 6e73 5b5d 2e49  Reservations[].I
+000142d0: 6e73 7461 6e63 6573 5b5d 2e53 7461 7465  nstances[].State
+000142e0: 5b5d 2e4e 616d 6520 270a 2020 2020 2020  [].Name '.      
+000142f0: 2020 2020 2020 2027 2d2d 6f75 7470 7574         '--output
+00014300: 2074 6578 7429 2026 2620 6563 686f 2022   text) && echo "
+00014310: 2473 2220 2626 2065 6368 6f3b 205b 5b20  $s" && echo; [[ 
+00014320: 2d7a 2022 2473 2220 5d5d 207c 7c20 5b5b  -z "$s" ]] || [[
+00014330: 2022 2473 2220 3d20 2274 6572 6d69 6e61   "$s" = "termina
+00014340: 7465 6422 205d 5d20 7c7c 205b 5b20 2224  ted" ]] || [[ "$
+00014350: 7322 203d 2022 7368 7574 7469 6e67 2d64  s" = "shutting-d
+00014360: 6f77 6e22 205d 5d27 0a20 2020 2020 2020  own" ]]'.       
+00014370: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+00014380: 2020 2020 2320 5465 7374 2063 616e 6365      # Test cance
+00014390: 6c6c 696e 6720 7468 6520 7370 6f74 2063  lling the spot c
+000143a0: 6c75 7374 6572 2064 7572 696e 6720 7370  luster during sp
+000143b0: 6f74 206a 6f62 2062 6569 6e67 2073 6574  ot job being set
+000143c0: 7570 2e0a 2020 2020 2020 2020 2020 2020  up..            
+000143d0: 6627 736b 7920 7370 6f74 206c 6175 6e63  f'sky spot launc
+000143e0: 6820 2d2d 636c 6f75 6420 6177 7320 2d2d  h --cloud aws --
+000143f0: 7265 6769 6f6e 207b 7265 6769 6f6e 7d20  region {region} 
+00014400: 2d6e 207b 6e61 6d65 7d2d 3220 7465 7374  -n {name}-2 test
+00014410: 732f 7465 7374 5f79 616d 6c73 2f74 6573  s/test_yamls/tes
+00014420: 745f 6c6f 6e67 5f73 6574 7570 2e79 616d  t_long_setup.yam
+00014430: 6c20 202d 7920 2d64 272c 0a20 2020 2020  l  -y -d',.     
+00014440: 2020 2020 2020 2027 736c 6565 7020 3330         'sleep 30
+00014450: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
+00014460: 5f53 504f 545f 4341 4e43 454c 5f57 4149  _SPOT_CANCEL_WAI
+00014470: 542e 666f 726d 6174 286a 6f62 5f6e 616d  T.format(job_nam
+00014480: 653d 6627 7b6e 616d 657d 2d32 2729 2c0a  e=f'{name}-2'),.
+00014490: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
+000144a0: 6570 2035 272c 0a20 2020 2020 2020 2020  ep 5',.         
+000144b0: 2020 2066 277b 5f53 504f 545f 5155 4555     f'{_SPOT_QUEU
+000144c0: 455f 5741 4954 7d7c 2067 7265 7020 7b6e  E_WAIT}| grep {n
+000144d0: 616d 657d 2d32 207c 2068 6561 6420 2d6e  ame}-2 | head -n
+000144e0: 3120 7c20 6772 6570 2022 4341 4e43 454c  1 | grep "CANCEL
+000144f0: 4c49 4e47 5c7c 4341 4e43 454c 4c45 4422  LING\|CANCELLED"
+00014500: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
+00014510: 736c 6565 7020 3132 3027 2c0a 2020 2020  sleep 120',.    
+00014520: 2020 2020 2020 2020 6627 7b5f 5350 4f54          f'{_SPOT
+00014530: 5f51 5545 5545 5f57 4149 547d 7c20 6772  _QUEUE_WAIT}| gr
+00014540: 6570 207b 6e61 6d65 7d2d 3220 7c20 6865  ep {name}-2 | he
+00014550: 6164 202d 6e31 207c 2067 7265 7020 2243  ad -n1 | grep "C
+00014560: 414e 4345 4c4c 4544 2227 2c0a 2020 2020  ANCELLED"',.    
+00014570: 2020 2020 2020 2020 2866 2773 3d24 2861          (f's=$(a
+00014580: 7773 2065 6332 2064 6573 6372 6962 652d  ws ec2 describe-
+00014590: 696e 7374 616e 6365 7320 2d2d 7265 6769  instances --regi
+000145a0: 6f6e 207b 7265 6769 6f6e 7d20 270a 2020  on {region} '.  
+000145b0: 2020 2020 2020 2020 2020 2066 272d 2d66             f'--f
+000145c0: 696c 7465 7273 204e 616d 653d 7461 673a  ilters Name=tag:
+000145d0: 7261 792d 636c 7573 7465 722d 6e61 6d65  ray-cluster-name
+000145e0: 2c56 616c 7565 733d 7b6e 616d 657d 2d32  ,Values={name}-2
+000145f0: 2d2a 2027 0a20 2020 2020 2020 2020 2020  -* '.           
+00014600: 2020 6627 2d2d 7175 6572 7920 5265 7365    f'--query Rese
+00014610: 7276 6174 696f 6e73 5b5d 2e49 6e73 7461  rvations[].Insta
+00014620: 6e63 6573 5b5d 2e53 7461 7465 5b5d 2e4e  nces[].State[].N
+00014630: 616d 6520 270a 2020 2020 2020 2020 2020  ame '.          
+00014640: 2020 2027 2d2d 6f75 7470 7574 2074 6578     '--output tex
+00014650: 7429 2026 2620 6563 686f 2022 2473 2220  t) && echo "$s" 
+00014660: 2626 2065 6368 6f3b 205b 5b20 2d7a 2022  && echo; [[ -z "
+00014670: 2473 2220 5d5d 207c 7c20 5b5b 2022 2473  $s" ]] || [[ "$s
+00014680: 2220 3d20 2274 6572 6d69 6e61 7465 6422  " = "terminated"
+00014690: 205d 5d20 7c7c 205b 5b20 2224 7322 203d   ]] || [[ "$s" =
+000146a0: 2022 7368 7574 7469 6e67 2d64 6f77 6e22   "shutting-down"
+000146b0: 205d 5d27 0a20 2020 2020 2020 2020 2020   ]]'.           
+000146c0: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+000146d0: 2320 5465 7374 2063 616e 6365 6c6c 6174  # Test cancellat
+000146e0: 696f 6e20 6475 7269 6e67 2073 706f 7420  ion during spot 
+000146f0: 6a6f 6220 6973 2072 6563 6f76 6572 696e  job is recoverin
+00014700: 672e 0a20 2020 2020 2020 2020 2020 2066  g..            f
+00014710: 2773 6b79 2073 706f 7420 6c61 756e 6368  'sky spot launch
+00014720: 202d 2d63 6c6f 7564 2061 7773 202d 2d72   --cloud aws --r
+00014730: 6567 696f 6e20 7b72 6567 696f 6e7d 202d  egion {region} -
+00014740: 6e20 7b6e 616d 657d 2d33 2022 736c 6565  n {name}-3 "slee
+00014750: 7020 3130 3030 2220 202d 7920 2d64 272c  p 1000"  -y -d',
+00014760: 0a20 2020 2020 2020 2020 2020 2027 736c  .            'sl
+00014770: 6565 7020 3330 3027 2c0a 2020 2020 2020  eep 300',.      
+00014780: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
+00014790: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
+000147a0: 207b 6e61 6d65 7d2d 3320 7c20 6865 6164   {name}-3 | head
+000147b0: 202d 6e31 207c 2067 7265 7020 2252 554e   -n1 | grep "RUN
+000147c0: 4e49 4e47 2227 2c0a 2020 2020 2020 2020  NING"',.        
+000147d0: 2020 2020 2320 5465 726d 696e 6174 6520      # Terminate 
+000147e0: 7468 6520 636c 7573 7465 7220 6d61 6e75  the cluster manu
+000147f0: 616c 6c79 2e0a 2020 2020 2020 2020 2020  ally..          
+00014800: 2020 2866 2761 7773 2065 6332 2074 6572    (f'aws ec2 ter
+00014810: 6d69 6e61 7465 2d69 6e73 7461 6e63 6573  minate-instances
+00014820: 202d 2d72 6567 696f 6e20 7b72 6567 696f   --region {regio
+00014830: 6e7d 202d 2d69 6e73 7461 6e63 652d 6964  n} --instance-id
+00014840: 7320 2428 270a 2020 2020 2020 2020 2020  s $('.          
+00014850: 2020 2066 2761 7773 2065 6332 2064 6573     f'aws ec2 des
+00014860: 6372 6962 652d 696e 7374 616e 6365 7320  cribe-instances 
+00014870: 2d2d 7265 6769 6f6e 207b 7265 6769 6f6e  --region {region
+00014880: 7d20 270a 2020 2020 2020 2020 2020 2020  } '.            
+00014890: 2066 272d 2d66 696c 7465 7273 204e 616d   f'--filters Nam
+000148a0: 653d 7461 673a 7261 792d 636c 7573 7465  e=tag:ray-cluste
+000148b0: 722d 6e61 6d65 2c56 616c 7565 733d 7b6e  r-name,Values={n
+000148c0: 616d 657d 2d33 2d2a 2027 0a20 2020 2020  ame}-3-* '.     
+000148d0: 2020 2020 2020 2020 6627 2d2d 7175 6572          f'--quer
+000148e0: 7920 5265 7365 7276 6174 696f 6e73 5b5d  y Reservations[]
+000148f0: 2e49 6e73 7461 6e63 6573 5b5d 2e49 6e73  .Instances[].Ins
+00014900: 7461 6e63 6549 6420 270a 2020 2020 2020  tanceId '.      
+00014910: 2020 2020 2020 2027 2d2d 6f75 7470 7574         '--output
+00014920: 2074 6578 7429 2729 2c0a 2020 2020 2020   text)'),.      
+00014930: 2020 2020 2020 2773 6c65 6570 2031 3230        'sleep 120
+00014940: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+00014950: 277b 5f53 504f 545f 5155 4555 455f 5741  '{_SPOT_QUEUE_WA
+00014960: 4954 7d7c 2067 7265 7020 7b6e 616d 657d  IT}| grep {name}
+00014970: 2d33 207c 2068 6561 6420 2d6e 3120 7c20  -3 | head -n1 | 
+00014980: 6772 6570 2022 5245 434f 5645 5249 4e47  grep "RECOVERING
+00014990: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
+000149a0: 5f53 504f 545f 4341 4e43 454c 5f57 4149  _SPOT_CANCEL_WAI
+000149b0: 542e 666f 726d 6174 286a 6f62 5f6e 616d  T.format(job_nam
+000149c0: 653d 6627 7b6e 616d 657d 2d33 2729 2c0a  e=f'{name}-3'),.
+000149d0: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
+000149e0: 6570 2035 272c 0a20 2020 2020 2020 2020  ep 5',.         
+000149f0: 2020 2066 277b 5f53 504f 545f 5155 4555     f'{_SPOT_QUEU
+00014a00: 455f 5741 4954 7d7c 2067 7265 7020 7b6e  E_WAIT}| grep {n
+00014a10: 616d 657d 2d33 207c 2068 6561 6420 2d6e  ame}-3 | head -n
+00014a20: 3120 7c20 6772 6570 2022 4341 4e43 454c  1 | grep "CANCEL
+00014a30: 4c49 4e47 5c7c 4341 4e43 454c 4c45 4422  LING\|CANCELLED"
+00014a40: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
+00014a50: 736c 6565 7020 3132 3027 2c0a 2020 2020  sleep 120',.    
+00014a60: 2020 2020 2020 2020 6627 7b5f 5350 4f54          f'{_SPOT
+00014a70: 5f51 5545 5545 5f57 4149 547d 7c20 6772  _QUEUE_WAIT}| gr
+00014a80: 6570 207b 6e61 6d65 7d2d 3320 7c20 6865  ep {name}-3 | he
+00014a90: 6164 202d 6e31 207c 2067 7265 7020 2243  ad -n1 | grep "C
+00014aa0: 414e 4345 4c4c 4544 2227 2c0a 2020 2020  ANCELLED"',.    
+00014ab0: 2020 2020 2020 2020 2320 5468 6520 636c          # The cl
+00014ac0: 7573 7465 7220 7368 6f75 6c64 2062 6520  uster should be 
+00014ad0: 7465 726d 696e 6174 6564 2028 7368 7574  terminated (shut
+00014ae0: 7469 6e67 2d64 6f77 6e29 2061 6674 6572  ting-down) after
+00014af0: 2063 616e 6365 6c6c 6174 696f 6e2e 2057   cancellation. W
+00014b00: 6520 646f 6e27 7420 7573 6520 7468 6520  e don't use the 
+00014b10: 603d 6020 6f70 6572 6174 6f72 2068 6572  `=` operator her
+00014b20: 6520 6265 6361 7573 650a 2020 2020 2020  e because.      
+00014b30: 2020 2020 2020 2320 7468 6572 6520 6361        # there ca
+00014b40: 6e20 6265 206d 756c 7469 706c 6520 564d  n be multiple VM
+00014b50: 2077 6974 6820 7468 6520 7361 6d65 206e   with the same n
+00014b60: 616d 6520 6475 6520 746f 2074 6865 2072  ame due to the r
+00014b70: 6563 6f76 6572 792e 0a20 2020 2020 2020  ecovery..       
+00014b80: 2020 2020 2028 6627 733d 2428 6177 7320       (f's=$(aws 
+00014b90: 6563 3220 6465 7363 7269 6265 2d69 6e73  ec2 describe-ins
+00014ba0: 7461 6e63 6573 202d 2d72 6567 696f 6e20  tances --region 
+00014bb0: 7b72 6567 696f 6e7d 2027 0a20 2020 2020  {region} '.     
+00014bc0: 2020 2020 2020 2020 6627 2d2d 6669 6c74          f'--filt
+00014bd0: 6572 7320 4e61 6d65 3d74 6167 3a72 6179  ers Name=tag:ray
+00014be0: 2d63 6c75 7374 6572 2d6e 616d 652c 5661  -cluster-name,Va
+00014bf0: 6c75 6573 3d7b 6e61 6d65 7d2d 332d 2a20  lues={name}-3-* 
+00014c00: 270a 2020 2020 2020 2020 2020 2020 2066  '.             f
+00014c10: 272d 2d71 7565 7279 2052 6573 6572 7661  '--query Reserva
+00014c20: 7469 6f6e 735b 5d2e 496e 7374 616e 6365  tions[].Instance
+00014c30: 735b 5d2e 5374 6174 655b 5d2e 4e61 6d65  s[].State[].Name
+00014c40: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+00014c50: 272d 2d6f 7574 7075 7420 7465 7874 2920  '--output text) 
+00014c60: 2626 2065 6368 6f20 2224 7322 2026 2620  && echo "$s" && 
+00014c70: 6563 686f 3b20 5b5b 202d 7a20 2224 7322  echo; [[ -z "$s"
+00014c80: 205d 5d20 7c7c 2065 6368 6f20 2224 7322   ]] || echo "$s"
+00014c90: 207c 2067 7265 7020 2d76 202d 4520 2270   | grep -v -E "p
+00014ca0: 656e 6469 6e67 7c72 756e 6e69 6e67 7c73  ending|running|s
+00014cb0: 746f 7070 6564 7c73 746f 7070 696e 6722  topped|stopping"
+00014cc0: 270a 2020 2020 2020 2020 2020 2020 292c  '.            ),
+00014cd0: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
+00014ce0: 2020 2020 7469 6d65 6f75 743d 3235 202a      timeout=25 *
+00014cf0: 2036 3029 0a20 2020 2072 756e 5f6f 6e65   60).    run_one
+00014d00: 5f74 6573 7428 7465 7374 290a 0a0a 4070  _test(test)...@p
+00014d10: 7974 6573 742e 6d61 726b 2e67 6370 0a40  ytest.mark.gcp.@
+00014d20: 7079 7465 7374 2e6d 6172 6b2e 6d61 6e61  pytest.mark.mana
+00014d30: 6765 645f 7370 6f74 0a64 6566 2074 6573  ged_spot.def tes
+00014d40: 745f 7370 6f74 5f63 616e 6365 6c6c 6174  t_spot_cancellat
+00014d50: 696f 6e5f 6763 7028 293a 0a20 2020 206e  ion_gcp():.    n
+00014d60: 616d 6520 3d20 5f67 6574 5f63 6c75 7374  ame = _get_clust
+00014d70: 6572 5f6e 616d 6528 290a 2020 2020 7a6f  er_name().    zo
+00014d80: 6e65 203d 2027 7573 2d77 6573 7433 2d62  ne = 'us-west3-b
+00014d90: 270a 2020 2020 7175 6572 795f 7374 6174  '.    query_stat
+00014da0: 655f 636d 6420 3d20 2827 6763 6c6f 7564  e_cmd = ('gcloud
+00014db0: 2063 6f6d 7075 7465 2069 6e73 7461 6e63   compute instanc
+00014dc0: 6573 206c 6973 7420 270a 2020 2020 2020  es list '.      
+00014dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014de0: 2066 272d 2d66 696c 7465 723d 2228 6c61   f'--filter="(la
+00014df0: 6265 6c73 2e72 6179 2d63 6c75 7374 6572  bels.ray-cluster
+00014e00: 2d6e 616d 653a 7b6e 616d 657d 2922 2027  -name:{name})" '
+00014e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014e20: 2020 2020 2020 2020 272d 2d66 6f72 6d61          '--forma
+00014e30: 743d 2276 616c 7565 2873 7461 7475 7329  t="value(status)
+00014e40: 2227 290a 2020 2020 7175 6572 795f 636d  "').    query_cm
+00014e50: 6420 3d20 2866 2767 636c 6f75 6420 636f  d = (f'gcloud co
+00014e60: 6d70 7574 6520 696e 7374 616e 6365 7320  mpute instances 
+00014e70: 6c69 7374 202d 2d66 696c 7465 723d 270a  list --filter='.
+00014e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e90: 2066 2722 286c 6162 656c 732e 7261 792d   f'"(labels.ray-
+00014ea0: 636c 7573 7465 722d 6e61 6d65 3a7b 6e61  cluster-name:{na
+00014eb0: 6d65 7d29 2220 270a 2020 2020 2020 2020  me})" '.        
+00014ec0: 2020 2020 2020 2020 2066 272d 2d7a 6f6e           f'--zon
+00014ed0: 6573 3d7b 7a6f 6e65 7d20 2d2d 666f 726d  es={zone} --form
+00014ee0: 6174 3d22 7661 6c75 6528 6e61 6d65 2922  at="value(name)"
+00014ef0: 2729 0a20 2020 2074 6572 6d69 6e61 7465  ').    terminate
+00014f00: 5f63 6d64 203d 2028 6627 6763 6c6f 7564  _cmd = (f'gcloud
+00014f10: 2063 6f6d 7075 7465 2069 6e73 7461 6e63   compute instanc
+00014f20: 6573 2064 656c 6574 6520 2d2d 7a6f 6e65  es delete --zone
+00014f30: 3d7b 7a6f 6e65 7d27 0a20 2020 2020 2020  ={zone}'.       
+00014f40: 2020 2020 2020 2020 2020 2020 2020 6627                f'
+00014f50: 202d 2d71 7569 6574 2024 287b 7175 6572   --quiet $({quer
+00014f60: 795f 636d 647d 2927 290a 2020 2020 7465  y_cmd})').    te
+00014f70: 7374 203d 2054 6573 7428 0a20 2020 2020  st = Test(.     
+00014f80: 2020 2027 7370 6f74 5f63 616e 6365 6c6c     'spot_cancell
+00014f90: 6174 696f 6e5f 6763 7027 2c0a 2020 2020  ation_gcp',.    
+00014fa0: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+00014fb0: 2020 2320 5465 7374 2063 616e 6365 6c6c    # Test cancell
+00014fc0: 6174 696f 6e20 6475 7269 6e67 2073 706f  ation during spo
+00014fd0: 7420 636c 7573 7465 7220 6265 696e 6720  t cluster being 
+00014fe0: 6c61 756e 6368 6564 2e0a 2020 2020 2020  launched..      
+00014ff0: 2020 2020 2020 6627 736b 7920 7370 6f74        f'sky spot
+00015000: 206c 6175 6e63 6820 2d2d 636c 6f75 6420   launch --cloud 
+00015010: 6763 7020 2d2d 7a6f 6e65 207b 7a6f 6e65  gcp --zone {zone
+00015020: 7d20 2d6e 207b 6e61 6d65 7d20 2273 6c65  } -n {name} "sle
+00015030: 6570 2031 3030 3022 2020 2d79 202d 6427  ep 1000"  -y -d'
+00015040: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
+00015050: 6c65 6570 2036 3027 2c0a 2020 2020 2020  leep 60',.      
+00015060: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
+00015070: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
+00015080: 207b 6e61 6d65 7d20 7c20 6865 6164 202d   {name} | head -
+00015090: 6e31 207c 2067 7265 7020 2253 5441 5254  n1 | grep "START
+000150a0: 494e 4722 272c 0a20 2020 2020 2020 2020  ING"',.         
+000150b0: 2020 205f 5350 4f54 5f43 414e 4345 4c5f     _SPOT_CANCEL_
+000150c0: 5741 4954 2e66 6f72 6d61 7428 6a6f 625f  WAIT.format(job_
+000150d0: 6e61 6d65 3d6e 616d 6529 2c0a 2020 2020  name=name),.    
+000150e0: 2020 2020 2020 2020 2773 6c65 6570 2035          'sleep 5
+000150f0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+00015100: 277b 5f53 504f 545f 5155 4555 455f 5741  '{_SPOT_QUEUE_WA
+00015110: 4954 7d7c 2067 7265 7020 7b6e 616d 657d  IT}| grep {name}
+00015120: 207c 2068 6561 6420 2d6e 3120 7c20 6772   | head -n1 | gr
+00015130: 6570 2022 4341 4e43 454c 4c49 4e47 5c7c  ep "CANCELLING\|
+00015140: 4341 4e43 454c 4c45 4422 272c 0a20 2020  CANCELLED"',.   
+00015150: 2020 2020 2020 2020 2027 736c 6565 7020           'sleep 
+00015160: 3132 3027 2c0a 2020 2020 2020 2020 2020  120',.          
+00015170: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
+00015180: 5f57 4149 547d 7c20 6772 6570 207b 6e61  _WAIT}| grep {na
+00015190: 6d65 7d20 7c20 6865 6164 202d 6e31 207c  me} | head -n1 |
+000151a0: 2067 7265 7020 2243 414e 4345 4c4c 4544   grep "CANCELLED
+000151b0: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
+000151c0: 2320 5465 7374 2063 616e 6365 6c6c 696e  # Test cancellin
+000151d0: 6720 7468 6520 7370 6f74 2063 6c75 7374  g the spot clust
+000151e0: 6572 2064 7572 696e 6720 7370 6f74 206a  er during spot j
+000151f0: 6f62 2062 6569 6e67 2073 6574 7570 2e0a  ob being setup..
+00015200: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+00015210: 7920 7370 6f74 206c 6175 6e63 6820 2d2d  y spot launch --
+00015220: 636c 6f75 6420 6763 7020 2d2d 7a6f 6e65  cloud gcp --zone
+00015230: 207b 7a6f 6e65 7d20 2d6e 207b 6e61 6d65   {zone} -n {name
+00015240: 7d2d 3220 7465 7374 732f 7465 7374 5f79  }-2 tests/test_y
+00015250: 616d 6c73 2f74 6573 745f 6c6f 6e67 5f73  amls/test_long_s
+00015260: 6574 7570 2e79 616d 6c20 202d 7920 2d64  etup.yaml  -y -d
+00015270: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
+00015280: 736c 6565 7020 3330 3027 2c0a 2020 2020  sleep 300',.    
+00015290: 2020 2020 2020 2020 5f53 504f 545f 4341          _SPOT_CA
+000152a0: 4e43 454c 5f57 4149 542e 666f 726d 6174  NCEL_WAIT.format
+000152b0: 286a 6f62 5f6e 616d 653d 6627 7b6e 616d  (job_name=f'{nam
+000152c0: 657d 2d32 2729 2c0a 2020 2020 2020 2020  e}-2'),.        
+000152d0: 2020 2020 2773 6c65 6570 2035 272c 0a20      'sleep 5',. 
+000152e0: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
+000152f0: 504f 545f 5155 4555 455f 5741 4954 7d7c  POT_QUEUE_WAIT}|
+00015300: 2067 7265 7020 7b6e 616d 657d 2d32 207c   grep {name}-2 |
+00015310: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
+00015320: 2022 4341 4e43 454c 4c49 4e47 5c7c 4341   "CANCELLING\|CA
+00015330: 4e43 454c 4c45 4422 272c 0a20 2020 2020  NCELLED"',.     
+00015340: 2020 2020 2020 2027 736c 6565 7020 3132         'sleep 12
+00015350: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
+00015360: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
+00015370: 4149 547d 7c20 6772 6570 207b 6e61 6d65  AIT}| grep {name
+00015380: 7d2d 3220 7c20 6865 6164 202d 6e31 207c  }-2 | head -n1 |
+00015390: 2067 7265 7020 2243 414e 4345 4c4c 4544   grep "CANCELLED
+000153a0: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
+000153b0: 2320 5465 7374 2063 616e 6365 6c6c 6174  # Test cancellat
+000153c0: 696f 6e20 6475 7269 6e67 2073 706f 7420  ion during spot 
+000153d0: 6a6f 6220 6973 2072 6563 6f76 6572 696e  job is recoverin
+000153e0: 672e 0a20 2020 2020 2020 2020 2020 2066  g..            f
+000153f0: 2773 6b79 2073 706f 7420 6c61 756e 6368  'sky spot launch
+00015400: 202d 2d63 6c6f 7564 2067 6370 202d 2d7a   --cloud gcp --z
+00015410: 6f6e 6520 7b7a 6f6e 657d 202d 6e20 7b6e  one {zone} -n {n
+00015420: 616d 657d 2d33 2022 736c 6565 7020 3130  ame}-3 "sleep 10
+00015430: 3030 2220 202d 7920 2d64 272c 0a20 2020  00"  -y -d',.   
+00015440: 2020 2020 2020 2020 2027 736c 6565 7020           'sleep 
+00015450: 3330 3027 2c0a 2020 2020 2020 2020 2020  300',.          
+00015460: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
+00015470: 5f57 4149 547d 7c20 6772 6570 207b 6e61  _WAIT}| grep {na
+00015480: 6d65 7d2d 3320 7c20 6865 6164 202d 6e31  me}-3 | head -n1
+00015490: 207c 2067 7265 7020 2252 554e 4e49 4e47   | grep "RUNNING
+000154a0: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
+000154b0: 2320 5465 726d 696e 6174 6520 7468 6520  # Terminate the 
+000154c0: 636c 7573 7465 7220 6d61 6e75 616c 6c79  cluster manually
+000154d0: 2e0a 2020 2020 2020 2020 2020 2020 7465  ..            te
+000154e0: 726d 696e 6174 655f 636d 642c 0a20 2020  rminate_cmd,.   
+000154f0: 2020 2020 2020 2020 2027 736c 6565 7020           'sleep 
+00015500: 3130 3027 2c0a 2020 2020 2020 2020 2020  100',.          
+00015510: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
+00015520: 5f57 4149 547d 7c20 6772 6570 207b 6e61  _WAIT}| grep {na
+00015530: 6d65 7d2d 3320 7c20 6865 6164 202d 6e31  me}-3 | head -n1
+00015540: 207c 2067 7265 7020 2252 4543 4f56 4552   | grep "RECOVER
+00015550: 494e 4722 272c 0a20 2020 2020 2020 2020  ING"',.         
+00015560: 2020 205f 5350 4f54 5f43 414e 4345 4c5f     _SPOT_CANCEL_
+00015570: 5741 4954 2e66 6f72 6d61 7428 6a6f 625f  WAIT.format(job_
+00015580: 6e61 6d65 3d66 277b 6e61 6d65 7d2d 3327  name=f'{name}-3'
+00015590: 292c 0a20 2020 2020 2020 2020 2020 2027  ),.            '
+000155a0: 736c 6565 7020 3527 2c0a 2020 2020 2020  sleep 5',.      
+000155b0: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
+000155c0: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
+000155d0: 207b 6e61 6d65 7d2d 3320 7c20 6865 6164   {name}-3 | head
+000155e0: 202d 6e31 207c 2067 7265 7020 2243 414e   -n1 | grep "CAN
+000155f0: 4345 4c4c 494e 475c 7c43 414e 4345 4c4c  CELLING\|CANCELL
+00015600: 4544 2227 2c0a 2020 2020 2020 2020 2020  ED"',.          
+00015610: 2020 2773 6c65 6570 2031 3230 272c 0a20    'sleep 120',. 
+00015620: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
+00015630: 504f 545f 5155 4555 455f 5741 4954 7d7c  POT_QUEUE_WAIT}|
+00015640: 2067 7265 7020 7b6e 616d 657d 2d33 207c   grep {name}-3 |
+00015650: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
+00015660: 2022 4341 4e43 454c 4c45 4422 272c 0a20   "CANCELLED"',. 
+00015670: 2020 2020 2020 2020 2020 2023 2054 6865             # The
+00015680: 2063 6c75 7374 6572 2073 686f 756c 6420   cluster should 
+00015690: 6265 2074 6572 6d69 6e61 7465 6420 2853  be terminated (S
+000156a0: 544f 5050 494e 4729 2061 6674 6572 2063  TOPPING) after c
+000156b0: 616e 6365 6c6c 6174 696f 6e2e 2057 6520  ancellation. We 
+000156c0: 646f 6e27 7420 7573 6520 7468 6520 603d  don't use the `=
+000156d0: 6020 6f70 6572 6174 6f72 2068 6572 6520  ` operator here 
+000156e0: 6265 6361 7573 650a 2020 2020 2020 2020  because.        
+000156f0: 2020 2020 2320 7468 6572 6520 6361 6e20      # there can 
+00015700: 6265 206d 756c 7469 706c 6520 564d 2077  be multiple VM w
+00015710: 6974 6820 7468 6520 7361 6d65 206e 616d  ith the same nam
+00015720: 6520 6475 6520 746f 2074 6865 2072 6563  e due to the rec
+00015730: 6f76 6572 792e 0a20 2020 2020 2020 2020  overy..         
+00015740: 2020 2028 6627 733d 2428 7b71 7565 7279     (f's=$({query
+00015750: 5f73 7461 7465 5f63 6d64 7d29 2026 2620  _state_cmd}) && 
+00015760: 6563 686f 2022 2473 2220 2626 2065 6368  echo "$s" && ech
+00015770: 6f3b 205b 5b20 2d7a 2022 2473 2220 5d5d  o; [[ -z "$s" ]]
+00015780: 207c 7c20 6563 686f 2022 2473 2220 7c20   || echo "$s" | 
+00015790: 6772 6570 202d 7620 2d45 2022 5052 4f56  grep -v -E "PROV
+000157a0: 4953 494f 4e49 4e47 7c53 5441 4749 4e47  ISIONING|STAGING
+000157b0: 7c52 554e 4e49 4e47 7c52 4550 4149 5249  |RUNNING|REPAIRI
+000157c0: 4e47 7c54 4552 4d49 4e41 5445 447c 5355  NG|TERMINATED|SU
+000157d0: 5350 454e 4449 4e47 7c53 5553 5045 4e44  SPENDING|SUSPEND
+000157e0: 4544 7c53 5553 5045 4e44 4544 2227 0a20  ED|SUSPENDED"'. 
+000157f0: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+00015800: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+00015810: 2074 696d 656f 7574 3d32 3520 2a20 3630   timeout=25 * 60
+00015820: 290a 2020 2020 7275 6e5f 6f6e 655f 7465  ).    run_one_te
+00015830: 7374 2874 6573 7429 0a0a 0a23 202d 2d2d  st(test)...# ---
+00015840: 2d2d 2d2d 2d2d 2d20 5465 7374 696e 6720  ------- Testing 
+00015850: 7374 6f72 6167 6520 666f 7220 6d61 6e61  storage for mana
+00015860: 6765 6420 7370 6f74 202d 2d2d 2d2d 2d2d  ged spot -------
+00015870: 2d2d 2d0a 4070 7974 6573 742e 6d61 726b  ---.@pytest.mark
+00015880: 2e6e 6f5f 6c61 6d62 6461 5f63 6c6f 7564  .no_lambda_cloud
+00015890: 2020 2320 4c61 6d62 6461 2043 6c6f 7564    # Lambda Cloud
+000158a0: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
+000158b0: 7420 7370 6f74 2069 6e73 7461 6e63 6573  t spot instances
+000158c0: 0a40 7079 7465 7374 2e6d 6172 6b2e 6e6f  .@pytest.mark.no
+000158d0: 5f69 626d 2020 2320 4942 4d20 436c 6f75  _ibm  # IBM Clou
+000158e0: 6420 646f 6573 206e 6f74 2073 7570 706f  d does not suppo
+000158f0: 7274 2073 706f 7420 696e 7374 616e 6365  rt spot instance
+00015900: 730a 4070 7974 6573 742e 6d61 726b 2e6e  s.@pytest.mark.n
+00015910: 6f5f 7363 7020 2023 2053 4350 2064 6f65  o_scp  # SCP doe
+00015920: 7320 6e6f 7420 7375 7070 6f72 7420 7370  s not support sp
+00015930: 6f74 2069 6e73 7461 6e63 6573 0a40 7079  ot instances.@py
+00015940: 7465 7374 2e6d 6172 6b2e 6d61 6e61 6765  test.mark.manage
+00015950: 645f 7370 6f74 0a64 6566 2074 6573 745f  d_spot.def test_
+00015960: 7370 6f74 5f73 746f 7261 6765 2867 656e  spot_storage(gen
+00015970: 6572 6963 5f63 6c6f 7564 3a20 7374 7229  eric_cloud: str)
+00015980: 3a0a 2020 2020 2222 2254 6573 7420 7374  :.    """Test st
+00015990: 6f72 6167 6520 7769 7468 206d 616e 6167  orage with manag
+000159a0: 6564 2073 706f 7422 2222 0a20 2020 206e  ed spot""".    n
+000159b0: 616d 6520 3d20 5f67 6574 5f63 6c75 7374  ame = _get_clust
+000159c0: 6572 5f6e 616d 6528 290a 2020 2020 7961  er_name().    ya
+000159d0: 6d6c 5f73 7472 203d 2070 6174 686c 6962  ml_str = pathlib
+000159e0: 2e50 6174 6828 0a20 2020 2020 2020 2027  .Path(.        '
+000159f0: 6578 616d 706c 6573 2f6d 616e 6167 6564  examples/managed
+00015a00: 5f73 706f 745f 7769 7468 5f73 746f 7261  _spot_with_stora
+00015a10: 6765 2e79 616d 6c27 292e 7265 6164 5f74  ge.yaml').read_t
+00015a20: 6578 7428 290a 2020 2020 7374 6f72 6167  ext().    storag
+00015a30: 655f 6e61 6d65 203d 2066 2773 6b79 2d74  e_name = f'sky-t
+00015a40: 6573 742d 7b69 6e74 2874 696d 652e 7469  est-{int(time.ti
+00015a50: 6d65 2829 297d 270a 2020 2020 7961 6d6c  me())}'.    yaml
+00015a60: 5f73 7472 203d 2079 616d 6c5f 7374 722e  _str = yaml_str.
+00015a70: 7265 706c 6163 6528 2773 6b79 2d77 6f72  replace('sky-wor
+00015a80: 6b64 6972 2d7a 6877 7527 2c20 7374 6f72  kdir-zhwu', stor
+00015a90: 6167 655f 6e61 6d65 290a 2020 2020 7769  age_name).    wi
+00015aa0: 7468 2074 656d 7066 696c 652e 4e61 6d65  th tempfile.Name
+00015ab0: 6454 656d 706f 7261 7279 4669 6c65 2873  dTemporaryFile(s
+00015ac0: 7566 6669 783d 272e 7961 6d6c 272c 206d  uffix='.yaml', m
+00015ad0: 6f64 653d 2777 2729 2061 7320 663a 0a20  ode='w') as f:. 
+00015ae0: 2020 2020 2020 2066 2e77 7269 7465 2879         f.write(y
+00015af0: 616d 6c5f 7374 7229 0a20 2020 2020 2020  aml_str).       
+00015b00: 2066 2e66 6c75 7368 2829 0a20 2020 2020   f.flush().     
+00015b10: 2020 2066 696c 655f 7061 7468 203d 2066     file_path = f
+00015b20: 2e6e 616d 650a 2020 2020 2020 2020 7465  .name.        te
+00015b30: 7374 203d 2054 6573 7428 0a20 2020 2020  st = Test(.     
+00015b40: 2020 2020 2020 2027 7370 6f74 5f73 746f         'spot_sto
+00015b50: 7261 6765 272c 0a20 2020 2020 2020 2020  rage',.         
+00015b60: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+00015b70: 2020 2020 202a 7374 6f72 6167 655f 7365       *storage_se
+00015b80: 7475 705f 636f 6d6d 616e 6473 2c0a 2020  tup_commands,.  
+00015b90: 2020 2020 2020 2020 2020 2020 2020 6627                f'
+00015ba0: 736b 7920 7370 6f74 206c 6175 6e63 6820  sky spot launch 
+00015bb0: 2d6e 207b 6e61 6d65 7d20 2d2d 636c 6f75  -n {name} --clou
+00015bc0: 6420 7b67 656e 6572 6963 5f63 6c6f 7564  d {generic_cloud
+00015bd0: 7d20 7b66 696c 655f 7061 7468 7d20 2d79  } {file_path} -y
+00015be0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00015bf0: 2020 2027 736c 6565 7020 3630 272c 2020     'sleep 60',  
+00015c00: 2320 5761 6974 2074 6865 2073 706f 7420  # Wait the spot 
+00015c10: 7175 6575 6520 746f 2062 6520 7570 6461  queue to be upda
+00015c20: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
+00015c30: 2020 2020 6627 7b5f 5350 4f54 5f51 5545      f'{_SPOT_QUE
+00015c40: 5545 5f57 4149 547d 7c20 6772 6570 207b  UE_WAIT}| grep {
+00015c50: 6e61 6d65 7d20 7c20 6772 6570 2053 5543  name} | grep SUC
+00015c60: 4345 4544 4544 272c 0a20 2020 2020 2020  CEEDED',.       
+00015c70: 2020 2020 2020 2020 2066 275b 2024 2861           f'[ $(a
+00015c80: 7773 2073 3361 7069 206c 6973 742d 6275  ws s3api list-bu
+00015c90: 636b 6574 7320 2d2d 7175 6572 7920 2242  ckets --query "B
+00015ca0: 7563 6b65 7473 5b3f 636f 6e74 6169 6e73  uckets[?contains
+00015cb0: 284e 616d 652c 205c 277b 7374 6f72 6167  (Name, \'{storag
+00015cc0: 655f 6e61 6d65 7d5c 2729 5d2e 4e61 6d65  e_name}\')].Name
+00015cd0: 2220 2d2d 6f75 7470 7574 2074 6578 7420  " --output text 
+00015ce0: 7c20 7763 202d 6c29 202d 6571 2030 205d  | wc -l) -eq 0 ]
+00015cf0: 270a 2020 2020 2020 2020 2020 2020 5d2c  '.            ],
+00015d00: 0a20 2020 2020 2020 2020 2020 205f 5350  .            _SP
+00015d10: 4f54 5f43 414e 4345 4c5f 5741 4954 2e66  OT_CANCEL_WAIT.f
+00015d20: 6f72 6d61 7428 6a6f 625f 6e61 6d65 3d6e  ormat(job_name=n
+00015d30: 616d 6529 2c0a 2020 2020 2020 2020 2020  ame),.          
+00015d40: 2020 2320 496e 6372 6561 7365 2074 696d    # Increase tim
+00015d50: 656f 7574 2073 696e 6365 2073 6b79 2073  eout since sky s
+00015d60: 706f 7420 7175 6575 6520 2d72 2063 616e  pot queue -r can
+00015d70: 2062 6520 626c 6f63 6b65 6420 6279 206f   be blocked by o
+00015d80: 7468 6572 2073 706f 7420 7465 7374 732e  ther spot tests.
+00015d90: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+00015da0: 656f 7574 3d32 3020 2a20 3630 2c0a 2020  eout=20 * 60,.  
+00015db0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00015dc0: 7275 6e5f 6f6e 655f 7465 7374 2874 6573  run_one_test(tes
+00015dd0: 7429 0a0a 0a23 202d 2d2d 2d2d 2d2d 2d2d  t)...# ---------
+00015de0: 2d20 5465 7374 696e 6720 7370 6f74 2054  - Testing spot T
+00015df0: 5055 202d 2d2d 2d2d 2d2d 2d2d 2d0a 4070  PU ----------.@p
+00015e00: 7974 6573 742e 6d61 726b 2e67 6370 0a40  ytest.mark.gcp.@
+00015e10: 7079 7465 7374 2e6d 6172 6b2e 6d61 6e61  pytest.mark.mana
+00015e20: 6765 645f 7370 6f74 0a64 6566 2074 6573  ged_spot.def tes
+00015e30: 745f 7370 6f74 5f74 7075 2829 3a0a 2020  t_spot_tpu():.  
+00015e40: 2020 2222 2254 6573 7420 6d61 6e61 6765    """Test manage
+00015e50: 6420 7370 6f74 206f 6e20 5450 552e 2222  d spot on TPU.""
+00015e60: 220a 2020 2020 6e61 6d65 203d 205f 6765  ".    name = _ge
+00015e70: 745f 636c 7573 7465 725f 6e61 6d65 2829  t_cluster_name()
+00015e80: 0a20 2020 2074 6573 7420 3d20 5465 7374  .    test = Test
+00015e90: 280a 2020 2020 2020 2020 2774 6573 742d  (.        'test-
+00015ea0: 7370 6f74 2d74 7075 272c 0a20 2020 2020  spot-tpu',.     
+00015eb0: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+00015ec0: 2066 2773 6b79 2073 706f 7420 6c61 756e   f'sky spot laun
+00015ed0: 6368 202d 6e20 7b6e 616d 657d 2065 7861  ch -n {name} exa
+00015ee0: 6d70 6c65 732f 7470 752f 7470 7576 6d5f  mples/tpu/tpuvm_
+00015ef0: 6d6e 6973 742e 7961 6d6c 202d 7920 2d64  mnist.yaml -y -d
+00015f00: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
+00015f10: 736c 6565 7020 3527 2c0a 2020 2020 2020  sleep 5',.      
+00015f20: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
+00015f30: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
+00015f40: 207b 6e61 6d65 7d20 7c20 6865 6164 202d   {name} | head -
+00015f50: 6e31 207c 2067 7265 7020 5354 4152 5449  n1 | grep STARTI
+00015f60: 4e47 272c 0a20 2020 2020 2020 2020 2020  NG',.           
+00015f70: 2027 736c 6565 7020 3732 3027 2c20 2023   'sleep 720',  #
+00015f80: 2054 5055 2074 616b 6573 2061 2077 6869   TPU takes a whi
+00015f90: 6c65 2074 6f20 6c61 756e 6368 0a20 2020  le to launch.   
+00015fa0: 2020 2020 2020 2020 2066 277b 5f53 504f           f'{_SPO
+00015fb0: 545f 5155 4555 455f 5741 4954 7d7c 2067  T_QUEUE_WAIT}| g
+00015fc0: 7265 7020 7b6e 616d 657d 207c 2068 6561  rep {name} | hea
+00015fd0: 6420 2d6e 3120 7c20 6772 6570 2022 5255  d -n1 | grep "RU
+00015fe0: 4e4e 494e 475c 7c53 5543 4345 4544 4544  NNING\|SUCCEEDED
+00015ff0: 2227 2c0a 2020 2020 2020 2020 5d2c 0a20  "',.        ],. 
+00016000: 2020 2020 2020 205f 5350 4f54 5f43 414e         _SPOT_CAN
+00016010: 4345 4c5f 5741 4954 2e66 6f72 6d61 7428  CEL_WAIT.format(
+00016020: 6a6f 625f 6e61 6d65 3d6e 616d 6529 2c0a  job_name=name),.
+00016030: 2020 2020 2020 2020 2320 496e 6372 6561          # Increa
+00016040: 7365 2074 696d 656f 7574 2073 696e 6365  se timeout since
+00016050: 2073 6b79 2073 706f 7420 7175 6575 6520   sky spot queue 
+00016060: 2d72 2063 616e 2062 6520 626c 6f63 6b65  -r can be blocke
+00016070: 6420 6279 206f 7468 6572 2073 706f 7420  d by other spot 
+00016080: 7465 7374 732e 0a20 2020 2020 2020 2074  tests..        t
+00016090: 696d 656f 7574 3d32 3020 2a20 3630 2c0a  imeout=20 * 60,.
+000160a0: 2020 2020 290a 2020 2020 7275 6e5f 6f6e      ).    run_on
+000160b0: 655f 7465 7374 2874 6573 7429 0a0a 0a23  e_test(test)...#
+000160c0: 202d 2d2d 2d2d 2d2d 2d2d 2d20 5465 7374   ---------- Test
+000160d0: 696e 6720 656e 7620 666f 7220 7370 6f74  ing env for spot
+000160e0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 4070 7974   ----------.@pyt
+000160f0: 6573 742e 6d61 726b 2e6e 6f5f 6c61 6d62  est.mark.no_lamb
+00016100: 6461 5f63 6c6f 7564 2020 2320 4c61 6d62  da_cloud  # Lamb
+00016110: 6461 2043 6c6f 7564 2064 6f65 7320 6e6f  da Cloud does no
+00016120: 7420 7375 7070 6f72 7420 7370 6f74 2069  t support spot i
+00016130: 6e73 7461 6e63 6573 0a40 7079 7465 7374  nstances.@pytest
+00016140: 2e6d 6172 6b2e 6e6f 5f69 626d 2020 2320  .mark.no_ibm  # 
+00016150: 4942 4d20 436c 6f75 6420 646f 6573 206e  IBM Cloud does n
+00016160: 6f74 2073 7570 706f 7274 2073 706f 7420  ot support spot 
+00016170: 696e 7374 616e 6365 730a 4070 7974 6573  instances.@pytes
+00016180: 742e 6d61 726b 2e6e 6f5f 7363 7020 2023  t.mark.no_scp  #
+00016190: 2053 4350 2064 6f65 7320 6e6f 7420 7375   SCP does not su
+000161a0: 7070 6f72 7420 7370 6f74 2069 6e73 7461  pport spot insta
+000161b0: 6e63 6573 0a40 7079 7465 7374 2e6d 6172  nces.@pytest.mar
+000161c0: 6b2e 6d61 6e61 6765 645f 7370 6f74 0a64  k.managed_spot.d
+000161d0: 6566 2074 6573 745f 7370 6f74 5f69 6e6c  ef test_spot_inl
+000161e0: 696e 655f 656e 7628 6765 6e65 7269 635f  ine_env(generic_
+000161f0: 636c 6f75 643a 2073 7472 293a 0a20 2020  cloud: str):.   
+00016200: 2022 2222 5465 7374 2073 706f 7420 656e   """Test spot en
+00016210: 7622 2222 0a20 2020 206e 616d 6520 3d20  v""".    name = 
+00016220: 5f67 6574 5f63 6c75 7374 6572 5f6e 616d  _get_cluster_nam
+00016230: 6528 290a 2020 2020 7465 7374 203d 2054  e().    test = T
+00016240: 6573 7428 0a20 2020 2020 2020 2027 7465  est(.        'te
+00016250: 7374 2d73 706f 742d 696e 6c69 6e65 2d65  st-spot-inline-e
+00016260: 6e76 272c 0a20 2020 2020 2020 205b 0a20  nv',.        [. 
+00016270: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+00016280: 2073 706f 7420 6c61 756e 6368 202d 6e20   spot launch -n 
+00016290: 7b6e 616d 657d 202d 7920 2d2d 636c 6f75  {name} -y --clou
+000162a0: 6420 7b67 656e 6572 6963 5f63 6c6f 7564  d {generic_cloud
+000162b0: 7d20 2d2d 656e 7620 5445 5354 5f45 4e56  } --env TEST_ENV
+000162c0: 3d22 6865 6c6c 6f20 776f 726c 6422 202d  ="hello world" -
+000162d0: 2d20 2228 5b5b 2021 202d 7a20 5c5c 225c  - "([[ ! -z \\"\
+000162e0: 2454 4553 545f 454e 565c 5c22 205d 5d20  $TEST_ENV\\" ]] 
+000162f0: 2626 205b 5b20 2120 2d7a 205c 5c22 5c24  && [[ ! -z \\"\$
+00016300: 534b 5950 494c 4f54 5f4e 4f44 455f 4950  SKYPILOT_NODE_IP
+00016310: 535c 5c22 205d 5d20 2626 205b 5b20 2120  S\\" ]] && [[ ! 
+00016320: 2d7a 205c 5c22 5c24 534b 5950 494c 4f54  -z \\"\$SKYPILOT
+00016330: 5f4e 4f44 455f 5241 4e4b 5c5c 2220 5d5d  _NODE_RANK\\" ]]
+00016340: 2920 7c7c 2065 7869 7420 3122 272c 0a20  ) || exit 1"',. 
+00016350: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
+00016360: 7020 3230 272c 0a20 2020 2020 2020 2020  p 20',.         
+00016370: 2020 2066 277b 5f53 504f 545f 5155 4555     f'{_SPOT_QUEU
+00016380: 455f 5741 4954 7d20 7c20 6772 6570 207b  E_WAIT} | grep {
+00016390: 6e61 6d65 7d20 7c20 6772 6570 2053 5543  name} | grep SUC
+000163a0: 4345 4544 4544 272c 0a20 2020 2020 2020  CEEDED',.       
+000163b0: 205d 2c0a 2020 2020 2020 2020 5f53 504f   ],.        _SPO
+000163c0: 545f 4341 4e43 454c 5f57 4149 542e 666f  T_CANCEL_WAIT.fo
+000163d0: 726d 6174 286a 6f62 5f6e 616d 653d 6e61  rmat(job_name=na
+000163e0: 6d65 292c 0a20 2020 2020 2020 2023 2049  me),.        # I
+000163f0: 6e63 7265 6173 6520 7469 6d65 6f75 7420  ncrease timeout 
+00016400: 7369 6e63 6520 736b 7920 7370 6f74 2071  since sky spot q
+00016410: 7565 7565 202d 7220 6361 6e20 6265 2062  ueue -r can be b
+00016420: 6c6f 636b 6564 2062 7920 6f74 6865 7220  locked by other 
+00016430: 7370 6f74 2074 6573 7473 2e0a 2020 2020  spot tests..    
+00016440: 2020 2020 7469 6d65 6f75 743d 3230 202a      timeout=20 *
+00016450: 2036 302c 0a20 2020 2029 0a20 2020 2072   60,.    ).    r
+00016460: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
+00016470: 290a 0a0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d  )...# ----------
+00016480: 2054 6573 7469 6e67 2065 6e76 202d 2d2d   Testing env ---
+00016490: 2d2d 2d2d 2d2d 2d0a 6465 6620 7465 7374  -------.def test
+000164a0: 5f69 6e6c 696e 655f 656e 7628 6765 6e65  _inline_env(gene
+000164b0: 7269 635f 636c 6f75 643a 2073 7472 293a  ric_cloud: str):
+000164c0: 0a20 2020 2022 2222 5465 7374 2065 6e76  .    """Test env
+000164d0: 2222 220a 2020 2020 6e61 6d65 203d 205f  """.    name = _
+000164e0: 6765 745f 636c 7573 7465 725f 6e61 6d65  get_cluster_name
+000164f0: 2829 0a20 2020 2074 6573 7420 3d20 5465  ().    test = Te
+00016500: 7374 280a 2020 2020 2020 2020 2774 6573  st(.        'tes
+00016510: 742d 696e 6c69 6e65 2d65 6e76 272c 0a20  t-inline-env',. 
+00016520: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00016530: 2020 2020 2066 2773 6b79 206c 6175 6e63       f'sky launc
+00016540: 6820 2d63 207b 6e61 6d65 7d20 2d79 202d  h -c {name} -y -
+00016550: 2d63 6c6f 7564 207b 6765 6e65 7269 635f  -cloud {generic_
+00016560: 636c 6f75 647d 202d 2d65 6e76 2054 4553  cloud} --env TES
+00016570: 545f 454e 563d 2268 656c 6c6f 2077 6f72  T_ENV="hello wor
+00016580: 6c64 2220 2d2d 2022 285b 5b20 2120 2d7a  ld" -- "([[ ! -z
+00016590: 205c 5c22 5c24 5445 5354 5f45 4e56 5c5c   \\"\$TEST_ENV\\
+000165a0: 2220 5d5d 2026 2620 5b5b 2021 202d 7a20  " ]] && [[ ! -z 
+000165b0: 5c5c 225c 2453 4b59 5049 4c4f 545f 4e4f  \\"\$SKYPILOT_NO
+000165c0: 4445 5f49 5053 5c5c 2220 5d5d 2026 2620  DE_IPS\\" ]] && 
+000165d0: 5b5b 2021 202d 7a20 5c5c 225c 2453 4b59  [[ ! -z \\"\$SKY
+000165e0: 5049 4c4f 545f 4e4f 4445 5f52 414e 4b5c  PILOT_NODE_RANK\
+000165f0: 5c22 205d 5d29 207c 7c20 6578 6974 2031  \" ]]) || exit 1
+00016600: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
+00016610: 6627 736b 7920 6c6f 6773 207b 6e61 6d65  f'sky logs {name
+00016620: 7d20 3120 2d2d 7374 6174 7573 272c 0a20  } 1 --status',. 
+00016630: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+00016640: 2065 7865 6320 7b6e 616d 657d 202d 2d65   exec {name} --e
+00016650: 6e76 2054 4553 545f 454e 5632 3d22 7375  nv TEST_ENV2="su
+00016660: 6363 6573 7322 2022 285b 5b20 2120 2d7a  ccess" "([[ ! -z
+00016670: 205c 5c22 5c24 5445 5354 5f45 4e56 325c   \\"\$TEST_ENV2\
+00016680: 5c22 205d 5d20 2626 205b 5b20 2120 2d7a  \" ]] && [[ ! -z
+00016690: 205c 5c22 5c24 534b 5950 494c 4f54 5f4e   \\"\$SKYPILOT_N
+000166a0: 4f44 455f 4950 535c 5c22 205d 5d20 2626  ODE_IPS\\" ]] &&
+000166b0: 205b 5b20 2120 2d7a 205c 5c22 5c24 534b   [[ ! -z \\"\$SK
+000166c0: 5950 494c 4f54 5f4e 4f44 455f 5241 4e4b  YPILOT_NODE_RANK
+000166d0: 5c5c 2220 5d5d 2920 7c7c 2065 7869 7420  \\" ]]) || exit 
+000166e0: 3122 272c 0a20 2020 2020 2020 2020 2020  1"',.           
+000166f0: 2066 2773 6b79 206c 6f67 7320 7b6e 616d   f'sky logs {nam
+00016700: 657d 2032 202d 2d73 7461 7475 7327 2c0a  e} 2 --status',.
+00016710: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00016720: 2020 2066 2773 6b79 2064 6f77 6e20 2d79     f'sky down -y
+00016730: 207b 6e61 6d65 7d27 2c0a 2020 2020 290a   {name}',.    ).
+00016740: 2020 2020 7275 6e5f 6f6e 655f 7465 7374      run_one_test
+00016750: 2874 6573 7429 0a0a 0a23 202d 2d2d 2d2d  (test)...# -----
+00016760: 2d2d 2d2d 2d20 5465 7374 696e 6720 6375  ----- Testing cu
+00016770: 7374 6f6d 2069 6d61 6765 202d 2d2d 2d2d  stom image -----
+00016780: 2d2d 2d2d 2d0a 4070 7974 6573 742e 6d61  -----.@pytest.ma
+00016790: 726b 2e61 7773 0a64 6566 2074 6573 745f  rk.aws.def test_
+000167a0: 6375 7374 6f6d 5f69 6d61 6765 2829 3a0a  custom_image():.
+000167b0: 2020 2020 2222 2254 6573 7420 6375 7374      """Test cust
+000167c0: 6f6d 2069 6d61 6765 2222 220a 2020 2020  om image""".    
+000167d0: 6e61 6d65 203d 205f 6765 745f 636c 7573  name = _get_clus
+000167e0: 7465 725f 6e61 6d65 2829 0a20 2020 2074  ter_name().    t
+000167f0: 6573 7420 3d20 5465 7374 280a 2020 2020  est = Test(.    
+00016800: 2020 2020 2774 6573 742d 6375 7374 6f6d      'test-custom
+00016810: 2d69 6d61 6765 272c 0a20 2020 2020 2020  -image',.       
+00016820: 205b 0a20 2020 2020 2020 2020 2020 2066   [.            f
+00016830: 2773 6b79 206c 6175 6e63 6820 2d63 207b  'sky launch -c {
+00016840: 6e61 6d65 7d20 2d2d 7265 7472 792d 756e  name} --retry-un
+00016850: 7469 6c2d 7570 202d 7920 6578 616d 706c  til-up -y exampl
+00016860: 6573 2f63 7573 746f 6d5f 696d 6167 652e  es/custom_image.
+00016870: 7961 6d6c 272c 0a20 2020 2020 2020 2020  yaml',.         
+00016880: 2020 2066 2773 6b79 206c 6f67 7320 7b6e     f'sky logs {n
+00016890: 616d 657d 2031 202d 2d73 7461 7475 7327  ame} 1 --status'
+000168a0: 2c0a 2020 2020 2020 2020 5d2c 0a20 2020  ,.        ],.   
+000168b0: 2020 2020 2066 2773 6b79 2064 6f77 6e20       f'sky down 
+000168c0: 2d79 207b 6e61 6d65 7d27 2c0a 2020 2020  -y {name}',.    
+000168d0: 2020 2020 7469 6d65 6f75 743d 3330 202a      timeout=30 *
+000168e0: 2036 302c 0a20 2020 2029 0a20 2020 2072   60,.    ).    r
+000168f0: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
+00016900: 290a 0a0a 4070 7974 6573 742e 6d61 726b  )...@pytest.mark
+00016910: 2e73 6c6f 770a 6465 6620 7465 7374 5f61  .slow.def test_a
+00016920: 7a75 7265 5f73 7461 7274 5f73 746f 705f  zure_start_stop_
+00016930: 7477 6f5f 6e6f 6465 7328 293a 0a20 2020  two_nodes():.   
+00016940: 206e 616d 6520 3d20 5f67 6574 5f63 6c75   name = _get_clu
+00016950: 7374 6572 5f6e 616d 6528 290a 2020 2020  ster_name().    
+00016960: 7465 7374 203d 2054 6573 7428 0a20 2020  test = Test(.   
+00016970: 2020 2020 2027 617a 7572 652d 7374 6172       'azure-star
+00016980: 742d 7374 6f70 2d74 776f 2d6e 6f64 6573  t-stop-two-nodes
+00016990: 272c 0a20 2020 2020 2020 205b 0a20 2020  ',.        [.   
+000169a0: 2020 2020 2020 2020 2066 2773 6b79 206c           f'sky l
+000169b0: 6175 6e63 6820 2d2d 6e75 6d2d 6e6f 6465  aunch --num-node
+000169c0: 733d 3220 2d79 202d 6320 7b6e 616d 657d  s=2 -y -c {name}
+000169d0: 2065 7861 6d70 6c65 732f 617a 7572 655f   examples/azure_
+000169e0: 7374 6172 745f 7374 6f70 2e79 616d 6c27  start_stop.yaml'
+000169f0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+00016a00: 736b 7920 6578 6563 202d 2d6e 756d 2d6e  sky exec --num-n
+00016a10: 6f64 6573 3d32 207b 6e61 6d65 7d20 6578  odes=2 {name} ex
+00016a20: 616d 706c 6573 2f61 7a75 7265 5f73 7461  amples/azure_sta
+00016a30: 7274 5f73 746f 702e 7961 6d6c 272c 0a20  rt_stop.yaml',. 
+00016a40: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+00016a50: 206c 6f67 7320 7b6e 616d 657d 2031 202d   logs {name} 1 -
+00016a60: 2d73 7461 7475 7327 2c20 2023 2045 6e73  -status',  # Ens
+00016a70: 7572 6520 7468 6520 6a6f 6220 7375 6363  ure the job succ
+00016a80: 6565 6465 642e 0a20 2020 2020 2020 2020  eeded..         
+00016a90: 2020 2066 2773 6b79 2073 746f 7020 2d79     f'sky stop -y
+00016aa0: 207b 6e61 6d65 7d27 2c0a 2020 2020 2020   {name}',.      
+00016ab0: 2020 2020 2020 6627 736b 7920 7374 6172        f'sky star
+00016ac0: 7420 2d79 207b 6e61 6d65 7d27 2c0a 2020  t -y {name}',.  
+00016ad0: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
+00016ae0: 6578 6563 202d 2d6e 756d 2d6e 6f64 6573  exec --num-nodes
+00016af0: 3d32 207b 6e61 6d65 7d20 6578 616d 706c  =2 {name} exampl
+00016b00: 6573 2f61 7a75 7265 5f73 7461 7274 5f73  es/azure_start_s
+00016b10: 746f 702e 7961 6d6c 272c 0a20 2020 2020  top.yaml',.     
+00016b20: 2020 2020 2020 2066 2773 6b79 206c 6f67         f'sky log
+00016b30: 7320 7b6e 616d 657d 2032 202d 2d73 7461  s {name} 2 --sta
+00016b40: 7475 7327 2c20 2023 2045 6e73 7572 6520  tus',  # Ensure 
+00016b50: 7468 6520 6a6f 6220 7375 6363 6565 6465  the job succeede
+00016b60: 642e 0a20 2020 2020 2020 205d 2c0a 2020  d..        ],.  
+00016b70: 2020 2020 2020 6627 736b 7920 646f 776e        f'sky down
+00016b80: 202d 7920 7b6e 616d 657d 272c 0a20 2020   -y {name}',.   
+00016b90: 2020 2020 2074 696d 656f 7574 3d33 3020       timeout=30 
+00016ba0: 2a20 3630 2c20 2023 2033 3020 6d69 6e73  * 60,  # 30 mins
+00016bb0: 2020 2869 7420 7461 6b65 7320 6172 6f75    (it takes arou
+00016bc0: 6e64 207e 3233 206d 696e 7329 0a20 2020  nd ~23 mins).   
+00016bd0: 2029 0a20 2020 2072 756e 5f6f 6e65 5f74   ).    run_one_t
+00016be0: 6573 7428 7465 7374 290a 0a0a 2320 2d2d  est(test)...# --
+00016bf0: 2d2d 2d2d 2d2d 2d2d 2054 6573 7469 6e67  -------- Testing
+00016c00: 2065 6e76 2066 6f72 2064 6973 6b20 7469   env for disk ti
+00016c10: 6572 202d 2d2d 2d2d 2d2d 2d2d 2d0a 4070  er ----------.@p
+00016c20: 7974 6573 742e 6d61 726b 2e61 7773 0a64  ytest.mark.aws.d
+00016c30: 6566 2074 6573 745f 6177 735f 6469 736b  ef test_aws_disk
+00016c40: 5f74 6965 7228 293a 0a0a 2020 2020 6465  _tier():..    de
+00016c50: 6620 5f67 6574 5f61 7773 5f71 7565 7279  f _get_aws_query
+00016c60: 5f63 6f6d 6d61 6e64 2872 6567 696f 6e2c  _command(region,
+00016c70: 2069 6e73 7461 6e63 655f 6964 2c20 6669   instance_id, fi
+00016c80: 656c 642c 2065 7870 6563 7465 6429 3a0a  eld, expected):.
+00016c90: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+00016ca0: 6627 6177 7320 6563 3220 6465 7363 7269  f'aws ec2 descri
+00016cb0: 6265 2d76 6f6c 756d 6573 202d 2d72 6567  be-volumes --reg
+00016cc0: 696f 6e20 7b72 6567 696f 6e7d 2027 0a20  ion {region} '. 
+00016cd0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00016ce0: 272d 2d66 696c 7465 7273 204e 616d 653d  '--filters Name=
+00016cf0: 6174 7461 6368 6d65 6e74 2e69 6e73 7461  attachment.insta
+00016d00: 6e63 652d 6964 2c56 616c 7565 733d 7b69  nce-id,Values={i
+00016d10: 6e73 7461 6e63 655f 6964 7d20 270a 2020  nstance_id} '.  
+00016d20: 2020 2020 2020 2020 2020 2020 2020 6627                f'
+00016d30: 2d2d 7175 6572 7920 566f 6c75 6d65 735b  --query Volumes[
+00016d40: 2a5d 2e7b 6669 656c 647d 207c 2067 7265  *].{field} | gre
+00016d50: 7020 7b65 7870 6563 7465 647d 203b 2027  p {expected} ; '
+00016d60: 290a 0a20 2020 2066 6f72 2064 6973 6b5f  )..    for disk_
+00016d70: 7469 6572 2069 6e20 5b27 6c6f 7727 2c20  tier in ['low', 
+00016d80: 276d 6564 6975 6d27 2c20 2768 6967 6827  'medium', 'high'
+00016d90: 5d3a 0a20 2020 2020 2020 2073 7065 6373  ]:.        specs
+00016da0: 203d 2041 5753 2e5f 6765 745f 6469 736b   = AWS._get_disk
+00016db0: 5f73 7065 6373 2864 6973 6b5f 7469 6572  _specs(disk_tier
+00016dc0: 290a 2020 2020 2020 2020 6e61 6d65 203d  ).        name =
+00016dd0: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
+00016de0: 6d65 2829 202b 2027 2d27 202b 2064 6973  me() + '-' + dis
+00016df0: 6b5f 7469 6572 0a20 2020 2020 2020 2072  k_tier.        r
+00016e00: 6567 696f 6e20 3d20 2775 732d 7765 7374  egion = 'us-west
+00016e10: 2d32 270a 2020 2020 2020 2020 7465 7374  -2'.        test
+00016e20: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
+00016e30: 2020 2020 2027 6177 732d 6469 736b 2d74       'aws-disk-t
+00016e40: 6965 7227 2c0a 2020 2020 2020 2020 2020  ier',.          
+00016e50: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
+00016e60: 2020 2020 6627 736b 7920 6c61 756e 6368      f'sky launch
+00016e70: 202d 7920 2d63 207b 6e61 6d65 7d20 2d2d   -y -c {name} --
+00016e80: 636c 6f75 6420 6177 7320 2d2d 7265 6769  cloud aws --regi
+00016e90: 6f6e 207b 7265 6769 6f6e 7d20 270a 2020  on {region} '.  
+00016ea0: 2020 2020 2020 2020 2020 2020 2020 6627                f'
+00016eb0: 2d2d 6469 736b 2d74 6965 7220 7b64 6973  --disk-tier {dis
+00016ec0: 6b5f 7469 6572 7d20 6563 686f 2022 6865  k_tier} echo "he
+00016ed0: 6c6c 6f20 736b 7922 272c 0a20 2020 2020  llo sky"',.     
+00016ee0: 2020 2020 2020 2020 2020 2066 2769 643d             f'id=
+00016ef0: 6061 7773 2065 6332 2064 6573 6372 6962  `aws ec2 describ
+00016f00: 652d 696e 7374 616e 6365 7320 2d2d 7265  e-instances --re
+00016f10: 6769 6f6e 207b 7265 6769 6f6e 7d20 2d2d  gion {region} --
+00016f20: 6669 6c74 6572 7320 270a 2020 2020 2020  filters '.      
+00016f30: 2020 2020 2020 2020 2020 6627 4e61 6d65            f'Name
+00016f40: 3d74 6167 3a72 6179 2d63 6c75 7374 6572  =tag:ray-cluster
+00016f50: 2d6e 616d 652c 5661 6c75 6573 3d7b 6e61  -name,Values={na
+00016f60: 6d65 7d20 2d2d 7175 6572 7920 270a 2020  me} --query '.  
+00016f70: 2020 2020 2020 2020 2020 2020 2020 6627                f'
+00016f80: 5265 7365 7276 6174 696f 6e73 5b5d 2e49  Reservations[].I
+00016f90: 6e73 7461 6e63 6573 5b5d 2e49 6e73 7461  nstances[].Insta
+00016fa0: 6e63 6549 6420 2d2d 6f75 7470 7574 2074  nceId --output t
+00016fb0: 6578 7460 3b20 2720 2b0a 2020 2020 2020  ext`; ' +.      
+00016fc0: 2020 2020 2020 2020 2020 5f67 6574 5f61            _get_a
+00016fd0: 7773 5f71 7565 7279 5f63 6f6d 6d61 6e64  ws_query_command
+00016fe0: 2872 6567 696f 6e2c 2027 2469 6427 2c20  (region, '$id', 
+00016ff0: 2756 6f6c 756d 6554 7970 6527 2c0a 2020  'VolumeType',.  
+00017000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017020: 2020 2020 2073 7065 6373 5b27 6469 736b       specs['disk
+00017030: 5f74 6965 7227 5d29 202b 0a20 2020 2020  _tier']) +.     
+00017040: 2020 2020 2020 2020 2020 2028 2727 2069             ('' i
+00017050: 6620 6469 736b 5f74 6965 7220 3d3d 2027  f disk_tier == '
+00017060: 6c6f 7727 2065 6c73 650a 2020 2020 2020  low' else.      
+00017070: 2020 2020 2020 2020 2020 2028 5f67 6574             (_get
+00017080: 5f61 7773 5f71 7565 7279 5f63 6f6d 6d61  _aws_query_comma
+00017090: 6e64 2872 6567 696f 6e2c 2027 2469 6427  nd(region, '$id'
+000170a0: 2c20 2749 6f70 7327 2c0a 2020 2020 2020  , 'Iops',.      
+000170b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170d0: 2020 2073 7065 6373 5b27 6469 736b 5f69     specs['disk_i
+000170e0: 6f70 7327 5d29 202b 0a20 2020 2020 2020  ops']) +.       
+000170f0: 2020 2020 2020 2020 2020 205f 6765 745f             _get_
+00017100: 6177 735f 7175 6572 795f 636f 6d6d 616e  aws_query_comman
+00017110: 6428 7265 6769 6f6e 2c20 2724 6964 272c  d(region, '$id',
+00017120: 2027 5468 726f 7567 6870 7574 272c 0a20   'Throughput',. 
+00017130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017150: 2020 2020 2020 2020 7370 6563 735b 2764          specs['d
+00017160: 6973 6b5f 7468 726f 7567 6870 7574 275d  isk_throughput']
+00017170: 2929 292c 0a20 2020 2020 2020 2020 2020  ))),.           
+00017180: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
+00017190: 6627 736b 7920 646f 776e 202d 7920 7b6e  f'sky down -y {n
+000171a0: 616d 657d 272c 0a20 2020 2020 2020 2020  ame}',.         
+000171b0: 2020 2074 696d 656f 7574 3d31 3020 2a20     timeout=10 * 
+000171c0: 3630 2c20 2023 2031 3020 6d69 6e73 2020  60,  # 10 mins  
+000171d0: 2869 7420 7461 6b65 7320 6172 6f75 6e64  (it takes around
+000171e0: 207e 3620 6d69 6e73 290a 2020 2020 2020   ~6 mins).      
+000171f0: 2020 290a 2020 2020 2020 2020 7275 6e5f    ).        run_
+00017200: 6f6e 655f 7465 7374 2874 6573 7429 0a0a  one_test(test)..
+00017210: 0a40 7079 7465 7374 2e6d 6172 6b2e 6763  .@pytest.mark.gc
+00017220: 700a 6465 6620 7465 7374 5f67 6370 5f64  p.def test_gcp_d
+00017230: 6973 6b5f 7469 6572 2829 3a0a 2020 2020  isk_tier():.    
+00017240: 666f 7220 6469 736b 5f74 6965 7220 696e  for disk_tier in
+00017250: 205b 276c 6f77 272c 2027 6d65 6469 756d   ['low', 'medium
+00017260: 272c 2027 6869 6768 275d 3a0a 2020 2020  ', 'high']:.    
+00017270: 2020 2020 7479 7065 203d 2047 4350 2e5f      type = GCP._
+00017280: 6765 745f 6469 736b 5f74 7970 6528 6469  get_disk_type(di
+00017290: 736b 5f74 6965 7229 0a20 2020 2020 2020  sk_tier).       
+000172a0: 206e 616d 6520 3d20 5f67 6574 5f63 6c75   name = _get_clu
+000172b0: 7374 6572 5f6e 616d 6528 2920 2b20 272d  ster_name() + '-
+000172c0: 2720 2b20 6469 736b 5f74 6965 720a 2020  ' + disk_tier.  
+000172d0: 2020 2020 2020 7265 6769 6f6e 203d 2027        region = '
+000172e0: 7573 2d77 6573 7432 270a 2020 2020 2020  us-west2'.      
+000172f0: 2020 7465 7374 203d 2054 6573 7428 0a20    test = Test(. 
+00017300: 2020 2020 2020 2020 2020 2027 6763 702d             'gcp-
+00017310: 6469 736b 2d74 6965 7227 2c0a 2020 2020  disk-tier',.    
+00017320: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
+00017330: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
+00017340: 6c61 756e 6368 202d 7920 2d63 207b 6e61  launch -y -c {na
+00017350: 6d65 7d20 2d2d 636c 6f75 6420 6763 7020  me} --cloud gcp 
+00017360: 2d2d 7265 6769 6f6e 207b 7265 6769 6f6e  --region {region
+00017370: 7d20 270a 2020 2020 2020 2020 2020 2020  } '.            
+00017380: 2020 2020 6627 2d2d 6469 736b 2d74 6965      f'--disk-tie
+00017390: 7220 7b64 6973 6b5f 7469 6572 7d20 6563  r {disk_tier} ec
+000173a0: 686f 2022 6865 6c6c 6f20 736b 7922 272c  ho "hello sky"',
+000173b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000173c0: 2066 276e 616d 653d 6067 636c 6f75 6420   f'name=`gcloud 
+000173d0: 636f 6d70 7574 6520 696e 7374 616e 6365  compute instance
+000173e0: 7320 6c69 7374 202d 2d66 696c 7465 723d  s list --filter=
+000173f0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00017400: 2020 6627 226c 6162 656c 732e 7261 792d    f'"labels.ray-
+00017410: 636c 7573 7465 722d 6e61 6d65 3a7b 6e61  cluster-name:{na
+00017420: 6d65 7d22 202d 2d66 6f72 6d61 743d 2276  me}" --format="v
+00017430: 616c 7565 286e 616d 6529 2260 3b20 270a  alue(name)"`; '.
+00017440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017450: 6627 6763 6c6f 7564 2063 6f6d 7075 7465  f'gcloud compute
+00017460: 2064 6973 6b73 206c 6973 7420 2d2d 6669   disks list --fi
+00017470: 6c74 6572 3d22 6e61 6d65 3d24 6e61 6d65  lter="name=$name
+00017480: 2220 270a 2020 2020 2020 2020 2020 2020  " '.            
+00017490: 2020 2020 6627 2d2d 666f 726d 6174 3d22      f'--format="
+000174a0: 7661 6c75 6528 7479 7065 2922 207c 2067  value(type)" | g
+000174b0: 7265 7020 7b74 7970 657d 2027 0a20 2020  rep {type} '.   
+000174c0: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+000174d0: 2020 2020 2020 2020 6627 736b 7920 646f          f'sky do
+000174e0: 776e 202d 7920 7b6e 616d 657d 272c 0a20  wn -y {name}',. 
+000174f0: 2020 2020 2020 2020 2020 2074 696d 656f             timeo
+00017500: 7574 3d36 202a 2036 302c 2020 2320 3620  ut=6 * 60,  # 6 
+00017510: 6d69 6e73 2020 2869 7420 7461 6b65 7320  mins  (it takes 
+00017520: 6172 6f75 6e64 207e 3320 6d69 6e73 290a  around ~3 mins).
+00017530: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00017540: 2020 7275 6e5f 6f6e 655f 7465 7374 2874    run_one_test(t
+00017550: 6573 7429 0a0a 0a40 7079 7465 7374 2e6d  est)...@pytest.m
+00017560: 6172 6b2e 617a 7572 650a 6465 6620 7465  ark.azure.def te
+00017570: 7374 5f61 7a75 7265 5f64 6973 6b5f 7469  st_azure_disk_ti
+00017580: 6572 2829 3a0a 2020 2020 666f 7220 6469  er():.    for di
+00017590: 736b 5f74 6965 7220 696e 205b 276c 6f77  sk_tier in ['low
+000175a0: 272c 2027 6d65 6469 756d 275d 3a0a 2020  ', 'medium']:.  
+000175b0: 2020 2020 2020 7479 7065 203d 2041 7a75        type = Azu
+000175c0: 7265 2e5f 6765 745f 6469 736b 5f74 7970  re._get_disk_typ
+000175d0: 6528 6469 736b 5f74 6965 7229 0a20 2020  e(disk_tier).   
+000175e0: 2020 2020 206e 616d 6520 3d20 5f67 6574       name = _get
+000175f0: 5f63 6c75 7374 6572 5f6e 616d 6528 2920  _cluster_name() 
+00017600: 2b20 272d 2720 2b20 6469 736b 5f74 6965  + '-' + disk_tie
+00017610: 720a 2020 2020 2020 2020 7265 6769 6f6e  r.        region
+00017620: 203d 2027 7765 7374 7573 3227 0a20 2020   = 'westus2'.   
+00017630: 2020 2020 2074 6573 7420 3d20 5465 7374       test = Test
+00017640: 280a 2020 2020 2020 2020 2020 2020 2761  (.            'a
+00017650: 7a75 7265 2d64 6973 6b2d 7469 6572 272c  zure-disk-tier',
+00017660: 0a20 2020 2020 2020 2020 2020 205b 0a20  .            [. 
+00017670: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00017680: 2773 6b79 206c 6175 6e63 6820 2d79 202d  'sky launch -y -
+00017690: 6320 7b6e 616d 657d 202d 2d63 6c6f 7564  c {name} --cloud
+000176a0: 2061 7a75 7265 202d 2d72 6567 696f 6e20   azure --region 
+000176b0: 7b72 6567 696f 6e7d 2027 0a20 2020 2020  {region} '.     
+000176c0: 2020 2020 2020 2020 2020 2066 272d 2d64             f'--d
+000176d0: 6973 6b2d 7469 6572 207b 6469 736b 5f74  isk-tier {disk_t
+000176e0: 6965 727d 2065 6368 6f20 2268 656c 6c6f  ier} echo "hello
+000176f0: 2073 6b79 2227 2c0a 2020 2020 2020 2020   sky"',.        
+00017700: 2020 2020 2020 2020 6627 617a 2072 6573          f'az res
+00017710: 6f75 7263 6520 6c69 7374 202d 2d74 6167  ource list --tag
+00017720: 2072 6179 2d63 6c75 7374 6572 2d6e 616d   ray-cluster-nam
+00017730: 653d 7b6e 616d 657d 202d 2d71 7565 7279  e={name} --query
+00017740: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+00017750: 2020 2066 2722 5b3f 7479 7065 3d3d 5c27     f'"[?type==\'
+00017760: 4d69 6372 6f73 6f66 742e 436f 6d70 7574  Microsoft.Comput
+00017770: 652f 6469 736b 735c 275d 2e73 6b75 2e6e  e/disks\'].sku.n
+00017780: 616d 6522 2027 0a20 2020 2020 2020 2020  ame" '.         
+00017790: 2020 2020 2020 2066 272d 2d6f 7574 7075         f'--outpu
+000177a0: 7420 7473 7620 7c20 6772 6570 207b 7479  t tsv | grep {ty
+000177b0: 7065 7d27 0a20 2020 2020 2020 2020 2020  pe}'.           
+000177c0: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
+000177d0: 6627 736b 7920 646f 776e 202d 7920 7b6e  f'sky down -y {n
+000177e0: 616d 657d 272c 0a20 2020 2020 2020 2020  ame}',.         
+000177f0: 2020 2074 696d 656f 7574 3d32 3020 2a20     timeout=20 * 
+00017800: 3630 2c20 2023 2032 3020 6d69 6e73 2020  60,  # 20 mins  
+00017810: 2869 7420 7461 6b65 7320 6172 6f75 6e64  (it takes around
+00017820: 207e 3132 206d 696e 7329 0a20 2020 2020   ~12 mins).     
+00017830: 2020 2029 0a20 2020 2020 2020 2072 756e     ).        run
+00017840: 5f6f 6e65 5f74 6573 7428 7465 7374 290a  _one_test(test).
+00017850: 0a0a 2320 2d2d 2d2d 2d2d 2054 6573 7469  ..# ------ Testi
+00017860: 6e67 205a 6572 6f20 5175 6f74 6120 4661  ng Zero Quota Fa
+00017870: 696c 6f76 6572 202d 2d2d 2d2d 2d0a 4070  ilover ------.@p
+00017880: 7974 6573 742e 6d61 726b 2e61 7773 0a64  ytest.mark.aws.d
+00017890: 6566 2074 6573 745f 6177 735f 7a65 726f  ef test_aws_zero
+000178a0: 5f71 756f 7461 5f66 6169 6c6f 7665 7228  _quota_failover(
+000178b0: 293a 0a0a 2020 2020 6e61 6d65 203d 205f  ):..    name = _
+000178c0: 6765 745f 636c 7573 7465 725f 6e61 6d65  get_cluster_name
+000178d0: 2829 0a20 2020 2072 6567 696f 6e20 3d20  ().    region = 
+000178e0: 6765 745f 6177 735f 7265 6769 6f6e 5f66  get_aws_region_f
+000178f0: 6f72 5f71 756f 7461 5f66 6169 6c6f 7665  or_quota_failove
+00017900: 7228 290a 0a20 2020 2069 6620 6e6f 7420  r()..    if not 
+00017910: 7265 6769 6f6e 3a0a 2020 2020 2020 2020  region:.        
+00017920: 7265 7475 726e 0a0a 2020 2020 7465 7374  return..    test
+00017930: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
+00017940: 2027 6177 732d 7a65 726f 2d71 756f 7461   'aws-zero-quota
+00017950: 2d66 6169 6c6f 7665 7227 2c0a 2020 2020  -failover',.    
+00017960: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+00017970: 2020 6627 736b 7920 6c61 756e 6368 202d    f'sky launch -
+00017980: 7920 2d63 207b 6e61 6d65 7d20 2d2d 636c  y -c {name} --cl
+00017990: 6f75 6420 6177 7320 2d2d 7265 6769 6f6e  oud aws --region
+000179a0: 207b 7265 6769 6f6e 7d20 2d2d 6770 7573   {region} --gpus
+000179b0: 2056 3130 303a 3820 2d2d 7573 652d 7370   V100:8 --use-sp
+000179c0: 6f74 207c 2067 7265 7020 2246 6f75 6e64  ot | grep "Found
+000179d0: 206e 6f20 7175 6f74 6122 272c 0a20 2020   no quota"',.   
+000179e0: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+000179f0: 6627 736b 7920 646f 776e 202d 7920 7b6e  f'sky down -y {n
+00017a00: 616d 657d 272c 0a20 2020 2029 0a20 2020  ame}',.    ).   
+00017a10: 2072 756e 5f6f 6e65 5f74 6573 7428 7465   run_one_test(te
+00017a20: 7374 290a 0a0a 2320 2d2d 2d2d 2d2d 2d20  st)...# ------- 
+00017a30: 5465 7374 696e 6720 7573 6572 2072 6179  Testing user ray
+00017a40: 2063 6c75 7374 6572 202d 2d2d 2d2d 2d2d   cluster -------
+00017a50: 2d0a 6465 6620 7465 7374 5f75 7365 725f  -.def test_user_
+00017a60: 7261 795f 636c 7573 7465 7228 293a 0a20  ray_cluster():. 
+00017a70: 2020 206e 616d 6520 3d20 5f67 6574 5f63     name = _get_c
+00017a80: 6c75 7374 6572 5f6e 616d 6528 290a 2020  luster_name().  
+00017a90: 2020 7465 7374 203d 2054 6573 7428 0a20    test = Test(. 
+00017aa0: 2020 2020 2020 2027 7573 6572 2d72 6179         'user-ray
+00017ab0: 2d63 6c75 7374 6572 272c 0a20 2020 2020  -cluster',.     
+00017ac0: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+00017ad0: 2066 2773 6b79 206c 6175 6e63 6820 2d79   f'sky launch -y
+00017ae0: 202d 6320 7b6e 616d 657d 2022 7261 7920   -c {name} "ray 
+00017af0: 7374 6172 7420 2d2d 6865 6164 2227 2c0a  start --head"',.
+00017b00: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+00017b10: 7920 6578 6563 207b 6e61 6d65 7d20 2265  y exec {name} "e
+00017b20: 6368 6f20 6869 2227 2c0a 2020 2020 2020  cho hi"',.      
+00017b30: 2020 2020 2020 6627 736b 7920 6c6f 6773        f'sky logs
+00017b40: 207b 6e61 6d65 7d20 3120 2d2d 7374 6174   {name} 1 --stat
+00017b50: 7573 272c 0a20 2020 2020 2020 2020 2020  us',.           
+00017b60: 2066 2773 6b79 2073 7461 7475 7320 2d72   f'sky status -r
+00017b70: 207c 2067 7265 7020 7b6e 616d 657d 207c   | grep {name} |
+00017b80: 2067 7265 7020 5550 272c 0a20 2020 2020   grep UP',.     
+00017b90: 2020 2020 2020 2066 2773 6b79 2065 7865         f'sky exe
+00017ba0: 6320 7b6e 616d 657d 2022 6563 686f 2062  c {name} "echo b
+00017bb0: 7965 2227 2c0a 2020 2020 2020 2020 2020  ye"',.          
+00017bc0: 2020 6627 736b 7920 6c6f 6773 207b 6e61    f'sky logs {na
+00017bd0: 6d65 7d20 3220 2d2d 7374 6174 7573 272c  me} 2 --status',
+00017be0: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
+00017bf0: 2020 2020 6627 736b 7920 646f 776e 202d      f'sky down -
+00017c00: 7920 7b6e 616d 657d 272c 0a20 2020 2029  y {name}',.    )
+00017c10: 0a20 2020 2072 756e 5f6f 6e65 5f74 6573  .    run_one_tes
+00017c20: 7428 7465 7374 290a 0a0a 2320 2d2d 2d2d  t(test)...# ----
+00017c30: 2d2d 2d20 5465 7374 696e 6720 7468 6520  --- Testing the 
+00017c40: 636f 7265 2041 5049 202d 2d2d 2d2d 2d2d  core API -------
+00017c50: 2d0a 2320 4d6f 7374 206f 6620 7468 6520  -.# Most of the 
+00017c60: 636f 7265 2041 5049 7320 6861 7665 2062  core APIs have b
+00017c70: 6565 6e20 7465 7374 6564 2069 6e20 7468  een tested in th
+00017c80: 6520 434c 4920 7465 7374 732e 0a23 2054  e CLI tests..# T
+00017c90: 6865 7365 2074 6573 7473 2061 7265 2066  hese tests are f
+00017ca0: 6f72 2074 6573 7469 6e67 2074 6865 2072  or testing the r
+00017cb0: 6574 7572 6e20 7661 6c75 6520 6f66 2074  eturn value of t
+00017cc0: 6865 2041 5049 7320 6e6f 7420 6675 6c6c  he APIs not full
+00017cd0: 7920 7573 6564 2069 6e20 434c 492e 0a64  y used in CLI..d
+00017ce0: 6566 2074 6573 745f 636f 7265 5f61 7069  ef test_core_api
+00017cf0: 2829 3a0a 2020 2020 6e61 6d65 203d 205f  ():.    name = _
+00017d00: 6765 745f 636c 7573 7465 725f 6e61 6d65  get_cluster_name
+00017d10: 2829 0a20 2020 2073 6b79 2e6c 6175 6e63  ().    sky.launc
+00017d20: 680a 2020 2020 2320 544f 444f 287a 6877  h.    # TODO(zhw
+00017d30: 7529 3a20 4164 6420 6120 7465 7374 2066  u): Add a test f
+00017d40: 6f72 2063 6f72 6520 6170 692e 0a0a 0a23  or core api....#
+00017d50: 202d 2d2d 2d2d 2d2d 2d2d 2d20 5465 7374   ---------- Test
+00017d60: 696e 6720 5374 6f72 6167 6520 2d2d 2d2d  ing Storage ----
+00017d70: 2d2d 2d2d 2d2d 0a63 6c61 7373 2054 6573  ------.class Tes
+00017d80: 7453 746f 7261 6765 5769 7468 4372 6564  tStorageWithCred
+00017d90: 656e 7469 616c 733a 0a20 2020 2022 2222  entials:.    """
+00017da0: 5374 6f72 6167 6520 7465 7374 7320 7768  Storage tests wh
+00017db0: 6963 6820 7265 7175 6972 6520 6372 6564  ich require cred
+00017dc0: 656e 7469 616c 7320 616e 6420 6e65 7477  entials and netw
+00017dd0: 6f72 6b20 636f 6e6e 6563 7469 6f6e 2222  ork connection""
+00017de0: 220a 0a20 2020 2041 5753 5f49 4e56 414c  "..    AWS_INVAL
+00017df0: 4944 5f4e 414d 4553 203d 205b 0a20 2020  ID_NAMES = [.   
+00017e00: 2020 2020 2027 6162 272c 2020 2320 6c65       'ab',  # le
+00017e10: 7373 2074 6861 6e20 3320 6368 6172 6163  ss than 3 charac
+00017e20: 7465 7273 0a20 2020 2020 2020 2027 6162  ters.        'ab
+00017e30: 6364 6566 6768 696a 6b6c 6d6e 6f70 7172  cdefghijklmnopqr
+00017e40: 7374 7576 7778 797a 6162 6364 6566 6768  stuvwxyzabcdefgh
+00017e50: 696a 6b6c 6d6e 6f70 7172 7374 7576 7778  ijklmnopqrstuvwx
+00017e60: 797a 6162 6364 6566 6768 696a 6b6c 6d6e  yzabcdefghijklmn
+00017e70: 6f70 7172 7374 7576 7778 797a 3127 2c0a  opqrstuvwxyz1',.
+00017e80: 2020 2020 2020 2020 2320 6d6f 7265 2074          # more t
+00017e90: 6861 6e20 3633 2063 6861 7261 6374 6572  han 63 character
+00017ea0: 730a 2020 2020 2020 2020 2741 6263 6465  s.        'Abcde
+00017eb0: 6627 2c20 2023 2063 6f6e 7461 696e 7320  f',  # contains 
+00017ec0: 616e 2075 7070 6572 6361 7365 206c 6574  an uppercase let
+00017ed0: 7465 720a 2020 2020 2020 2020 2761 6263  ter.        'abc
+00017ee0: 2064 6566 272c 2020 2320 636f 6e74 6169   def',  # contai
+00017ef0: 6e73 2061 2073 7061 6365 0a20 2020 2020  ns a space.     
+00017f00: 2020 2027 6162 632e 2e64 6566 272c 2020     'abc..def',  
+00017f10: 2320 7477 6f20 6164 6a61 6365 6e74 2070  # two adjacent p
+00017f20: 6572 696f 6473 0a20 2020 2020 2020 2027  eriods.        '
+00017f30: 3139 322e 3136 382e 352e 3427 2c20 2023  192.168.5.4',  #
+00017f40: 2066 6f72 6d61 7474 6564 2061 7320 616e   formatted as an
+00017f50: 2049 5020 6164 6472 6573 730a 2020 2020   IP address.    
+00017f60: 2020 2020 2778 6e2d 2d62 7563 6b65 7427      'xn--bucket'
+00017f70: 2c20 2023 2073 7461 7274 7320 7769 7468  ,  # starts with
+00017f80: 2027 786e 2d2d 2720 7072 6566 6978 0a20   'xn--' prefix. 
+00017f90: 2020 2020 2020 2027 6275 636b 6574 2d73         'bucket-s
+00017fa0: 3361 6c69 6173 272c 2020 2320 656e 6473  3alias',  # ends
+00017fb0: 2077 6974 6820 272d 7333 616c 6961 7327   with '-s3alias'
+00017fc0: 2073 7566 6669 780a 2020 2020 2020 2020   suffix.        
+00017fd0: 2762 7563 6b65 742d 2d6f 6c2d 7333 272c  'bucket--ol-s3',
+00017fe0: 2020 2320 656e 6473 2077 6974 6820 272d    # ends with '-
+00017ff0: 2d6f 6c2d 7333 2720 7375 6666 6978 0a20  -ol-s3' suffix. 
+00018000: 2020 2020 2020 2027 2e61 6263 272c 2020         '.abc',  
+00018010: 2320 7374 6172 7473 2077 6974 6820 6120  # starts with a 
+00018020: 646f 740a 2020 2020 2020 2020 2761 6263  dot.        'abc
+00018030: 2e27 2c20 2023 2065 6e64 7320 7769 7468  .',  # ends with
+00018040: 2061 2064 6f74 0a20 2020 2020 2020 2027   a dot.        '
+00018050: 2d61 6263 272c 2020 2320 7374 6172 7473  -abc',  # starts
+00018060: 2077 6974 6820 6120 6879 7068 656e 0a20   with a hyphen. 
+00018070: 2020 2020 2020 2027 6162 632d 272c 2020         'abc-',  
+00018080: 2320 656e 6473 2077 6974 6820 6120 6879  # ends with a hy
+00018090: 7068 656e 0a20 2020 205d 0a0a 2020 2020  phen.    ]..    
+000180a0: 4743 535f 494e 5641 4c49 445f 4e41 4d45  GCS_INVALID_NAME
+000180b0: 5320 3d20 5b0a 2020 2020 2020 2020 2761  S = [.        'a
+000180c0: 6227 2c20 2023 206c 6573 7320 7468 616e  b',  # less than
+000180d0: 2033 2063 6861 7261 6374 6572 730a 2020   3 characters.  
+000180e0: 2020 2020 2020 2761 6263 6465 6667 6869        'abcdefghi
+000180f0: 6a6b 6c6d 6e6f 7071 7273 7475 7677 7879  jklmnopqrstuvwxy
+00018100: 7a61 6263 6465 6667 6869 6a6b 6c6d 6e6f  zabcdefghijklmno
+00018110: 7071 7273 7475 7677 7879 7a61 6263 6465  pqrstuvwxyzabcde
+00018120: 6667 6869 6a6b 6c6d 6e6f 7071 7273 7475  fghijklmnopqrstu
+00018130: 7677 7879 7a31 272c 0a20 2020 2020 2020  vwxyz1',.       
+00018140: 2023 206d 6f72 6520 7468 616e 2036 3320   # more than 63 
+00018150: 6368 6172 6163 7465 7273 2028 7769 7468  characters (with
+00018160: 6f75 7420 646f 7473 290a 2020 2020 2020  out dots).      
+00018170: 2020 2741 6263 6465 6627 2c20 2023 2063    'Abcdef',  # c
+00018180: 6f6e 7461 696e 7320 616e 2075 7070 6572  ontains an upper
+00018190: 6361 7365 206c 6574 7465 720a 2020 2020  case letter.    
+000181a0: 2020 2020 2761 6263 2064 6566 272c 2020      'abc def',  
+000181b0: 2320 636f 6e74 6169 6e73 2061 2073 7061  # contains a spa
+000181c0: 6365 0a20 2020 2020 2020 2027 6162 632e  ce.        'abc.
+000181d0: 2e64 6566 272c 2020 2320 7477 6f20 6164  .def',  # two ad
+000181e0: 6a61 6365 6e74 2070 6572 696f 6473 0a20  jacent periods. 
+000181f0: 2020 2020 2020 2027 6162 635f 2e64 6566         'abc_.def
+00018200: 2e67 6869 2e6a 6b6c 6d6e 6f70 7172 7374  .ghi.jklmnopqrst
+00018210: 7576 7778 797a 6162 6364 6566 6768 696a  uvwxyzabcdefghij
+00018220: 6b6c 6d6e 6f70 7172 7374 7576 7778 797a  klmnopqrstuvwxyz
+00018230: 6162 6364 6566 6768 696a 6b6c 6d6e 6f70  abcdefghijklmnop
+00018240: 7172 7374 7576 7778 797a 3127 0a20 2020  qrstuvwxyz1'.   
+00018250: 2020 2020 2023 204d 6f72 6520 7468 616e       # More than
+00018260: 2036 3320 6368 6172 6163 7465 7273 2062   63 characters b
+00018270: 6574 7765 656e 2064 6f74 730a 2020 2020  etween dots.    
+00018280: 2020 2020 2761 6263 5f2e 6465 662e 6768      'abc_.def.gh
+00018290: 692e 6a6b 6c6d 6e6f 7071 7273 7475 7677  i.jklmnopqrstuvw
+000182a0: 7879 7a61 6263 6465 6667 6869 6a6b 6c6d  xyzabcdefghijklm
+000182b0: 6e6f 7071 6667 6869 6a6b 6c6d 6e6f 7071  nopqfghijklmnopq
+000182c0: 7273 7475 7677 2720 2a20 352c 0a20 2020  rstuvw' * 5,.   
+000182d0: 2020 2020 2023 206d 6f72 6520 7468 616e       # more than
+000182e0: 2032 3232 2063 6861 7261 6374 6572 7320   222 characters 
+000182f0: 2877 6974 6820 646f 7473 290a 2020 2020  (with dots).    
+00018300: 2020 2020 2731 3932 2e31 3638 2e35 2e34      '192.168.5.4
+00018310: 272c 2020 2320 666f 726d 6174 7465 6420  ',  # formatted 
+00018320: 6173 2061 6e20 4950 2061 6464 7265 7373  as an IP address
+00018330: 0a20 2020 2020 2020 2027 676f 6f67 6275  .        'googbu
+00018340: 636b 6574 272c 2020 2320 7374 6172 7473  cket',  # starts
+00018350: 2077 6974 6820 2767 6f6f 6727 2070 7265   with 'goog' pre
+00018360: 6669 780a 2020 2020 2020 2020 2767 6f6f  fix.        'goo
+00018370: 676c 6562 7563 6b65 7427 2c20 2023 2063  glebucket',  # c
+00018380: 6f6e 7461 696e 7320 2767 6f6f 676c 6527  ontains 'google'
+00018390: 0a20 2020 2020 2020 2027 6730 3067 6c65  .        'g00gle
+000183a0: 6275 636b 6574 272c 2020 2320 7661 7269  bucket',  # vari
+000183b0: 616e 7420 6f66 2027 676f 6f67 6c65 270a  ant of 'google'.
+000183c0: 2020 2020 2020 2020 2767 6f30 676c 6562          'go0gleb
+000183d0: 7563 6b65 7427 2c20 2023 2076 6172 6961  ucket',  # varia
+000183e0: 6e74 206f 6620 2767 6f6f 676c 6527 0a20  nt of 'google'. 
+000183f0: 2020 2020 2020 2027 6730 6f67 6c65 6275         'g0oglebu
+00018400: 636b 6574 272c 2020 2320 7661 7269 616e  cket',  # varian
+00018410: 7420 6f66 2027 676f 6f67 6c65 270a 2020  t of 'google'.  
+00018420: 2020 2020 2020 272e 6162 6327 2c20 2023        '.abc',  #
+00018430: 2073 7461 7274 7320 7769 7468 2061 2064   starts with a d
+00018440: 6f74 0a20 2020 2020 2020 2027 6162 632e  ot.        'abc.
+00018450: 272c 2020 2320 656e 6473 2077 6974 6820  ',  # ends with 
+00018460: 6120 646f 740a 2020 2020 2020 2020 275f  a dot.        '_
+00018470: 6162 6327 2c20 2023 2073 7461 7274 7320  abc',  # starts 
+00018480: 7769 7468 2061 6e20 756e 6465 7273 636f  with an undersco
+00018490: 7265 0a20 2020 2020 2020 2027 6162 635f  re.        'abc_
+000184a0: 272c 2020 2320 656e 6473 2077 6974 6820  ',  # ends with 
+000184b0: 616e 2075 6e64 6572 7363 6f72 650a 2020  an underscore.  
+000184c0: 2020 5d0a 0a20 2020 2040 7374 6174 6963    ]..    @static
+000184d0: 6d65 7468 6f64 0a20 2020 2064 6566 2063  method.    def c
+000184e0: 6c69 5f64 656c 6574 655f 636d 6428 7374  li_delete_cmd(st
+000184f0: 6f72 655f 7479 7065 2c20 6275 636b 6574  ore_type, bucket
+00018500: 5f6e 616d 6529 3a0a 2020 2020 2020 2020  _name):.        
+00018510: 6966 2073 746f 7265 5f74 7970 6520 3d3d  if store_type ==
+00018520: 2073 746f 7261 6765 5f6c 6962 2e53 746f   storage_lib.Sto
+00018530: 7265 5479 7065 2e53 333a 0a20 2020 2020  reType.S3:.     
+00018540: 2020 2020 2020 2075 726c 203d 2066 2773         url = f's
+00018550: 333a 2f2f 7b62 7563 6b65 745f 6e61 6d65  3://{bucket_name
+00018560: 7d27 0a20 2020 2020 2020 2020 2020 2072  }'.            r
+00018570: 6574 7572 6e20 6627 6177 7320 7333 2072  eturn f'aws s3 r
+00018580: 6220 7b75 726c 7d20 2d2d 666f 7263 6527  b {url} --force'
+00018590: 0a20 2020 2020 2020 2069 6620 7374 6f72  .        if stor
+000185a0: 655f 7479 7065 203d 3d20 7374 6f72 6167  e_type == storag
+000185b0: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
+000185c0: 4743 533a 0a20 2020 2020 2020 2020 2020  GCS:.           
+000185d0: 2075 726c 203d 2066 2767 733a 2f2f 7b62   url = f'gs://{b
+000185e0: 7563 6b65 745f 6e61 6d65 7d27 0a20 2020  ucket_name}'.   
+000185f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00018600: 6627 6773 7574 696c 202d 6d20 726d 202d  f'gsutil -m rm -
+00018610: 7220 7b75 726c 7d27 0a20 2020 2020 2020  r {url}'.       
+00018620: 2069 6620 7374 6f72 655f 7479 7065 203d   if store_type =
+00018630: 3d20 7374 6f72 6167 655f 6c69 622e 5374  = storage_lib.St
+00018640: 6f72 6554 7970 652e 5232 3a0a 2020 2020  oreType.R2:.    
+00018650: 2020 2020 2020 2020 656e 6470 6f69 6e74          endpoint
+00018660: 5f75 726c 203d 2063 6c6f 7564 666c 6172  _url = cloudflar
+00018670: 652e 6372 6561 7465 5f65 6e64 706f 696e  e.create_endpoin
+00018680: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00018690: 7572 6c20 3d20 6627 7333 3a2f 2f7b 6275  url = f's3://{bu
+000186a0: 636b 6574 5f6e 616d 657d 270a 2020 2020  cket_name}'.    
+000186b0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+000186c0: 2741 5753 5f53 4841 5245 445f 4352 4544  'AWS_SHARED_CRED
+000186d0: 454e 5449 414c 535f 4649 4c45 3d7b 636c  ENTIALS_FILE={cl
+000186e0: 6f75 6466 6c61 7265 2e52 325f 4352 4544  oudflare.R2_CRED
+000186f0: 454e 5449 414c 535f 5041 5448 7d20 6177  ENTIALS_PATH} aw
+00018700: 7320 7333 2072 6220 7b75 726c 7d20 2d2d  s s3 rb {url} --
+00018710: 666f 7263 6520 2d2d 656e 6470 6f69 6e74  force --endpoint
+00018720: 207b 656e 6470 6f69 6e74 5f75 726c 7d20   {endpoint_url} 
+00018730: 2d2d 7072 6f66 696c 653d 7232 270a 0a20  --profile=r2'.. 
+00018740: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+00018750: 0a20 2020 2064 6566 2063 6c69 5f6c 735f  .    def cli_ls_
+00018760: 636d 6428 7374 6f72 655f 7479 7065 2c20  cmd(store_type, 
+00018770: 6275 636b 6574 5f6e 616d 652c 2073 7566  bucket_name, suf
+00018780: 6669 783d 2727 293a 0a20 2020 2020 2020  fix=''):.       
+00018790: 2069 6620 7374 6f72 655f 7479 7065 203d   if store_type =
+000187a0: 3d20 7374 6f72 6167 655f 6c69 622e 5374  = storage_lib.St
+000187b0: 6f72 6554 7970 652e 5333 3a0a 2020 2020  oreType.S3:.    
+000187c0: 2020 2020 2020 2020 6966 2073 7566 6669          if suffi
+000187d0: 783a 0a20 2020 2020 2020 2020 2020 2020  x:.             
+000187e0: 2020 2075 726c 203d 2066 2773 333a 2f2f     url = f's3://
+000187f0: 7b62 7563 6b65 745f 6e61 6d65 7d2f 7b73  {bucket_name}/{s
+00018800: 7566 6669 787d 270a 2020 2020 2020 2020  uffix}'.        
+00018810: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00018820: 2020 2020 2020 2020 2020 7572 6c20 3d20            url = 
+00018830: 6627 7333 3a2f 2f7b 6275 636b 6574 5f6e  f's3://{bucket_n
+00018840: 616d 657d 270a 2020 2020 2020 2020 2020  ame}'.          
+00018850: 2020 7265 7475 726e 2066 2761 7773 2073    return f'aws s
+00018860: 3320 6c73 207b 7572 6c7d 270a 2020 2020  3 ls {url}'.    
+00018870: 2020 2020 6966 2073 746f 7265 5f74 7970      if store_typ
+00018880: 6520 3d3d 2073 746f 7261 6765 5f6c 6962  e == storage_lib
+00018890: 2e53 746f 7265 5479 7065 2e47 4353 3a0a  .StoreType.GCS:.
+000188a0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000188b0: 7566 6669 783a 0a20 2020 2020 2020 2020  uffix:.         
+000188c0: 2020 2020 2020 2075 726c 203d 2066 2767         url = f'g
+000188d0: 733a 2f2f 7b62 7563 6b65 745f 6e61 6d65  s://{bucket_name
+000188e0: 7d2f 7b73 7566 6669 787d 270a 2020 2020  }/{suffix}'.    
+000188f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00018900: 2020 2020 2020 2020 2020 2020 2020 7572                ur
+00018910: 6c20 3d20 6627 6773 3a2f 2f7b 6275 636b  l = f'gs://{buck
+00018920: 6574 5f6e 616d 657d 270a 2020 2020 2020  et_name}'.      
+00018930: 2020 2020 2020 7265 7475 726e 2066 2767        return f'g
+00018940: 7375 7469 6c20 6c73 207b 7572 6c7d 270a  sutil ls {url}'.
+00018950: 2020 2020 2020 2020 6966 2073 746f 7265          if store
+00018960: 5f74 7970 6520 3d3d 2073 746f 7261 6765  _type == storage
+00018970: 5f6c 6962 2e53 746f 7265 5479 7065 2e52  _lib.StoreType.R
+00018980: 323a 0a20 2020 2020 2020 2020 2020 2065  2:.            e
+00018990: 6e64 706f 696e 745f 7572 6c20 3d20 636c  ndpoint_url = cl
+000189a0: 6f75 6466 6c61 7265 2e63 7265 6174 655f  oudflare.create_
+000189b0: 656e 6470 6f69 6e74 2829 0a20 2020 2020  endpoint().     
+000189c0: 2020 2020 2020 2069 6620 7375 6666 6978         if suffix
+000189d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000189e0: 2020 7572 6c20 3d20 6627 7333 3a2f 2f7b    url = f's3://{
+000189f0: 6275 636b 6574 5f6e 616d 657d 2f7b 7375  bucket_name}/{su
+00018a00: 6666 6978 7d27 0a20 2020 2020 2020 2020  ffix}'.         
+00018a10: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00018a20: 2020 2020 2020 2020 2075 726c 203d 2066           url = f
+00018a30: 2773 333a 2f2f 7b62 7563 6b65 745f 6e61  's3://{bucket_na
+00018a40: 6d65 7d27 0a20 2020 2020 2020 2020 2020  me}'.           
+00018a50: 2072 6574 7572 6e20 6627 4157 535f 5348   return f'AWS_SH
+00018a60: 4152 4544 5f43 5245 4445 4e54 4941 4c53  ARED_CREDENTIALS
+00018a70: 5f46 494c 453d 7b63 6c6f 7564 666c 6172  _FILE={cloudflar
+00018a80: 652e 5232 5f43 5245 4445 4e54 4941 4c53  e.R2_CREDENTIALS
+00018a90: 5f50 4154 487d 2061 7773 2073 3320 6c73  _PATH} aws s3 ls
+00018aa0: 207b 7572 6c7d 202d 2d65 6e64 706f 696e   {url} --endpoin
+00018ab0: 7420 7b65 6e64 706f 696e 745f 7572 6c7d  t {endpoint_url}
+00018ac0: 202d 2d70 726f 6669 6c65 3d72 3227 0a0a   --profile=r2'..
+00018ad0: 2020 2020 4070 7974 6573 742e 6669 7874      @pytest.fixt
+00018ae0: 7572 650a 2020 2020 6465 6620 746d 705f  ure.    def tmp_
+00018af0: 736f 7572 6365 2873 656c 662c 2074 6d70  source(self, tmp
+00018b00: 5f70 6174 6829 3a0a 2020 2020 2020 2020  _path):.        
+00018b10: 2320 4372 6561 7465 7320 6120 7465 6d70  # Creates a temp
+00018b20: 6f72 6172 7920 6469 7265 6374 6f72 7920  orary directory 
+00018b30: 7769 7468 2061 2066 696c 6520 696e 2069  with a file in i
+00018b40: 740a 2020 2020 2020 2020 746d 705f 6469  t.        tmp_di
+00018b50: 7220 3d20 746d 705f 7061 7468 202f 2027  r = tmp_path / '
+00018b60: 746d 702d 736f 7572 6365 270a 2020 2020  tmp-source'.    
+00018b70: 2020 2020 746d 705f 6469 722e 6d6b 6469      tmp_dir.mkdi
+00018b80: 7228 290a 2020 2020 2020 2020 746d 705f  r().        tmp_
+00018b90: 6669 6c65 203d 2074 6d70 5f64 6972 202f  file = tmp_dir /
+00018ba0: 2027 746d 702d 6669 6c65 270a 2020 2020   'tmp-file'.    
+00018bb0: 2020 2020 746d 705f 6669 6c65 2e77 7269      tmp_file.wri
+00018bc0: 7465 5f74 6578 7428 2774 6573 7427 290a  te_text('test').
+00018bd0: 2020 2020 2020 2020 6369 7263 6c65 5f6c          circle_l
+00018be0: 696e 6b20 3d20 746d 705f 6469 7220 2f20  ink = tmp_dir / 
+00018bf0: 2763 6972 636c 652d 6c69 6e6b 270a 2020  'circle-link'.  
+00018c00: 2020 2020 2020 6369 7263 6c65 5f6c 696e        circle_lin
+00018c10: 6b2e 7379 6d6c 696e 6b5f 746f 2874 6d70  k.symlink_to(tmp
+00018c20: 5f64 6972 2c20 7461 7267 6574 5f69 735f  _dir, target_is_
+00018c30: 6469 7265 6374 6f72 793d 5472 7565 290a  directory=True).
+00018c40: 2020 2020 2020 2020 7969 656c 6420 7374          yield st
+00018c50: 7228 746d 705f 6469 7229 0a0a 2020 2020  r(tmp_dir)..    
+00018c60: 4070 7974 6573 742e 6669 7874 7572 650a  @pytest.fixture.
+00018c70: 2020 2020 6465 6620 746d 705f 6275 636b      def tmp_buck
+00018c80: 6574 5f6e 616d 6528 7365 6c66 293a 0a20  et_name(self):. 
+00018c90: 2020 2020 2020 2023 2043 7265 6174 6573         # Creates
+00018ca0: 2061 2074 656d 706f 7261 7279 2062 7563   a temporary buc
+00018cb0: 6b65 7420 6e61 6d65 0a20 2020 2020 2020  ket name.       
+00018cc0: 2023 2074 696d 652e 7469 6d65 2829 2072   # time.time() r
+00018cd0: 6574 7572 6e73 2076 6172 7969 6e67 2070  eturns varying p
+00018ce0: 7265 6369 7369 6f6e 206f 6e20 6469 6666  recision on diff
+00018cf0: 6572 656e 7420 7379 7374 656d 732c 2073  erent systems, s
+00018d00: 6f20 7765 0a20 2020 2020 2020 2023 2072  o we.        # r
+00018d10: 6570 6c61 6365 2074 6865 2064 6563 696d  eplace the decim
+00018d20: 616c 2070 6f69 6e74 2061 6e64 2075 7365  al point and use
+00018d30: 2077 6861 7465 7665 7220 7072 6563 6973   whatever precis
+00018d40: 696f 6e20 7765 2063 616e 2067 6574 2e0a  ion we can get..
+00018d50: 2020 2020 2020 2020 7469 6d65 7374 616d          timestam
+00018d60: 7020 3d20 7374 7228 7469 6d65 2e74 696d  p = str(time.tim
+00018d70: 6528 2929 2e72 6570 6c61 6365 2827 2e27  e()).replace('.'
+00018d80: 2c20 2727 290a 2020 2020 2020 2020 7969  , '').        yi
+00018d90: 656c 6420 6627 736b 792d 7465 7374 2d7b  eld f'sky-test-{
+00018da0: 7469 6d65 7374 616d 707d 270a 0a20 2020  timestamp}'..   
+00018db0: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
+00018dc0: 2020 2064 6566 2079 6965 6c64 5f73 746f     def yield_sto
+00018dd0: 7261 6765 5f6f 626a 6563 7428 0a20 2020  rage_object(.   
+00018de0: 2020 2020 2020 2020 206e 616d 653a 204f           name: O
+00018df0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00018e00: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00018e10: 2073 6f75 7263 653a 204f 7074 696f 6e61   source: Optiona
+00018e20: 6c5b 7374 6f72 6167 655f 6c69 622e 5061  l[storage_lib.Pa
+00018e30: 7468 5d20 3d20 4e6f 6e65 2c0a 2020 2020  th] = None,.    
+00018e40: 2020 2020 2020 2020 7374 6f72 6573 3a20          stores: 
+00018e50: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
+00018e60: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
+00018e70: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
 00018e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e90: 2020 2020 2020 2020 2020 7374 6f72 6573            stores
-00018ea0: 3d73 746f 7265 732c 0a20 2020 2020 2020  =stores,.       
-00018eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ed0: 2020 2070 6572 7369 7374 656e 743d 7065     persistent=pe
-00018ee0: 7273 6973 7465 6e74 2c0a 2020 2020 2020  rsistent,.      
-00018ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f10: 2020 2020 6d6f 6465 3d6d 6f64 6529 0a20      mode=mode). 
-00018f20: 2020 2020 2020 2079 6965 6c64 2073 746f         yield sto
-00018f30: 7261 6765 5f6f 626a 0a20 2020 2020 2020  rage_obj.       
-00018f40: 2068 616e 646c 6520 3d20 676c 6f62 616c   handle = global
-00018f50: 5f75 7365 725f 7374 6174 652e 6765 745f  _user_state.get_
-00018f60: 6861 6e64 6c65 5f66 726f 6d5f 7374 6f72  handle_from_stor
-00018f70: 6167 655f 6e61 6d65 280a 2020 2020 2020  age_name(.      
-00018f80: 2020 2020 2020 7374 6f72 6167 655f 6f62        storage_ob
-00018f90: 6a2e 6e61 6d65 290a 2020 2020 2020 2020  j.name).        
-00018fa0: 6966 2068 616e 646c 653a 0a20 2020 2020  if handle:.     
-00018fb0: 2020 2020 2020 2023 2049 6620 6861 6e64         # If hand
-00018fc0: 6c65 2065 7869 7374 732c 2064 656c 6574  le exists, delet
-00018fd0: 6520 6d61 6e75 616c 6c79 0a20 2020 2020  e manually.     
-00018fe0: 2020 2020 2020 2023 2054 4f44 4f28 726f         # TODO(ro
-00018ff0: 6d69 6c62 293a 2054 6869 7320 6973 2070  milb): This is p
-00019000: 6f74 656e 7469 616c 6c79 2072 6973 6b79  otentially risky
-00019010: 202d 2069 6620 7468 6520 6465 6c65 7465   - if the delete
-00019020: 206d 6574 686f 6420 6861 730a 2020 2020   method has.    
-00019030: 2020 2020 2020 2020 2320 2020 6275 6773          #   bugs
-00019040: 2c20 7468 6973 2063 616e 2063 6175 7365  , this can cause
-00019050: 2072 6573 6f75 7263 6520 6c65 616b 732e   resource leaks.
-00019060: 2049 6465 616c 6c79 2077 6520 7368 6f75   Ideally we shou
-00019070: 6c64 206d 616e 7561 6c6c 790a 2020 2020  ld manually.    
-00019080: 2020 2020 2020 2020 2320 2020 656a 6563          #   ejec
-00019090: 7420 7374 6f72 6167 6520 6672 6f6d 2067  t storage from g
-000190a0: 6c6f 6261 6c5f 7573 6572 5f73 7461 7465  lobal_user_state
-000190b0: 2061 6e64 2064 656c 6574 6520 7468 6520   and delete the 
-000190c0: 6275 636b 6574 2075 7369 6e67 0a20 2020  bucket using.   
-000190d0: 2020 2020 2020 2020 2023 2020 2062 6f74           #   bot
-000190e0: 6f33 2064 6972 6563 746c 792e 0a20 2020  o3 directly..   
-000190f0: 2020 2020 2020 2020 2073 746f 7261 6765           storage
-00019100: 5f6f 626a 2e64 656c 6574 6528 290a 0a20  _obj.delete().. 
-00019110: 2020 2040 7079 7465 7374 2e66 6978 7475     @pytest.fixtu
-00019120: 7265 0a20 2020 2064 6566 2074 6d70 5f73  re.    def tmp_s
-00019130: 6372 6174 6368 5f73 746f 7261 6765 5f6f  cratch_storage_o
-00019140: 626a 2873 656c 662c 2074 6d70 5f62 7563  bj(self, tmp_buc
-00019150: 6b65 745f 6e61 6d65 293a 0a20 2020 2020  ket_name):.     
-00019160: 2020 2023 2043 7265 6174 6573 2061 2073     # Creates a s
-00019170: 746f 7261 6765 206f 626a 6563 7420 7769  torage object wi
-00019180: 7468 206e 6f20 736f 7572 6365 2074 6f20  th no source to 
-00019190: 6372 6561 7465 2061 2073 6372 6174 6368  create a scratch
-000191a0: 2073 746f 7261 6765 2e0a 2020 2020 2020   storage..      
-000191b0: 2020 2320 5374 6f72 6573 206d 7573 7420    # Stores must 
-000191c0: 6265 2061 6464 6564 2069 6e20 7468 6520  be added in the 
-000191d0: 7465 7374 2e0a 2020 2020 2020 2020 7969  test..        yi
-000191e0: 656c 6420 6672 6f6d 2073 656c 662e 7969  eld from self.yi
-000191f0: 656c 645f 7374 6f72 6167 655f 6f62 6a65  eld_storage_obje
-00019200: 6374 286e 616d 653d 746d 705f 6275 636b  ct(name=tmp_buck
-00019210: 6574 5f6e 616d 6529 0a0a 2020 2020 4070  et_name)..    @p
-00019220: 7974 6573 742e 6669 7874 7572 650a 2020  ytest.fixture.  
-00019230: 2020 6465 6620 746d 705f 6d75 6c74 6970    def tmp_multip
-00019240: 6c65 5f73 6372 6174 6368 5f73 746f 7261  le_scratch_stora
-00019250: 6765 5f6f 626a 2873 656c 6629 3a0a 2020  ge_obj(self):.  
-00019260: 2020 2020 2020 2320 4372 6561 7465 7320        # Creates 
-00019270: 6120 6c69 7374 206f 6620 3520 7374 6f72  a list of 5 stor
-00019280: 6167 6520 6f62 6a65 6374 7320 7769 7468  age objects with
-00019290: 206e 6f20 736f 7572 6365 2074 6f20 6372   no source to cr
-000192a0: 6561 7465 0a20 2020 2020 2020 2023 206d  eate.        # m
-000192b0: 756c 7469 706c 6520 7363 7261 7463 6820  ultiple scratch 
-000192c0: 7374 6f72 6167 6573 2e0a 2020 2020 2020  storages..      
-000192d0: 2020 2320 5374 6f72 6573 2066 6f72 2065    # Stores for e
-000192e0: 6163 6820 6f62 6a65 6374 2069 6e20 7468  ach object in th
-000192f0: 6520 6c69 7374 206d 7573 7420 6265 2061  e list must be a
-00019300: 6464 6564 2069 6e20 7468 6520 7465 7374  dded in the test
-00019310: 2e0a 2020 2020 2020 2020 7374 6f72 6167  ..        storag
-00019320: 655f 6d75 6c74 5f6f 626a 203d 205b 5d0a  e_mult_obj = [].
-00019330: 2020 2020 2020 2020 666f 7220 5f20 696e          for _ in
-00019340: 2072 616e 6765 2835 293a 0a20 2020 2020   range(5):.     
-00019350: 2020 2020 2020 2074 696d 6573 7461 6d70         timestamp
-00019360: 203d 2073 7472 2874 696d 652e 7469 6d65   = str(time.time
-00019370: 2829 292e 7265 706c 6163 6528 272e 272c  ()).replace('.',
-00019380: 2027 2729 0a20 2020 2020 2020 2020 2020   '').           
-00019390: 2073 746f 7265 5f6f 626a 203d 2073 746f   store_obj = sto
-000193a0: 7261 6765 5f6c 6962 2e53 746f 7261 6765  rage_lib.Storage
-000193b0: 286e 616d 653d 6627 736b 792d 7465 7374  (name=f'sky-test
-000193c0: 2d7b 7469 6d65 7374 616d 707d 2729 0a20  -{timestamp}'). 
-000193d0: 2020 2020 2020 2020 2020 2073 746f 7261             stora
-000193e0: 6765 5f6d 756c 745f 6f62 6a2e 6170 7065  ge_mult_obj.appe
-000193f0: 6e64 2873 746f 7265 5f6f 626a 290a 2020  nd(store_obj).  
-00019400: 2020 2020 2020 7969 656c 6420 7374 6f72        yield stor
-00019410: 6167 655f 6d75 6c74 5f6f 626a 0a20 2020  age_mult_obj.   
-00019420: 2020 2020 2066 6f72 2073 746f 7261 6765       for storage
-00019430: 5f6f 626a 2069 6e20 7374 6f72 6167 655f  _obj in storage_
-00019440: 6d75 6c74 5f6f 626a 3a0a 2020 2020 2020  mult_obj:.      
-00019450: 2020 2020 2020 6861 6e64 6c65 203d 2067        handle = g
-00019460: 6c6f 6261 6c5f 7573 6572 5f73 7461 7465  lobal_user_state
-00019470: 2e67 6574 5f68 616e 646c 655f 6672 6f6d  .get_handle_from
-00019480: 5f73 746f 7261 6765 5f6e 616d 6528 0a20  _storage_name(. 
-00019490: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000194a0: 746f 7261 6765 5f6f 626a 2e6e 616d 6529  torage_obj.name)
-000194b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000194c0: 6861 6e64 6c65 3a0a 2020 2020 2020 2020  handle:.        
-000194d0: 2020 2020 2020 2020 2320 4966 2068 616e          # If han
-000194e0: 646c 6520 6578 6973 7473 2c20 6465 6c65  dle exists, dele
-000194f0: 7465 206d 616e 7561 6c6c 790a 2020 2020  te manually.    
-00019500: 2020 2020 2020 2020 2020 2020 2320 544f              # TO
-00019510: 444f 2872 6f6d 696c 6229 3a20 5468 6973  DO(romilb): This
-00019520: 2069 7320 706f 7465 6e74 6961 6c6c 7920   is potentially 
-00019530: 7269 736b 7920 2d20 6966 2074 6865 2064  risky - if the d
-00019540: 656c 6574 6520 6d65 7468 6f64 2068 6173  elete method has
-00019550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019560: 2023 2062 7567 732c 2074 6869 7320 6361   # bugs, this ca
-00019570: 6e20 6361 7573 6520 7265 736f 7572 6365  n cause resource
-00019580: 206c 6561 6b73 2e20 4964 6561 6c6c 7920   leaks. Ideally 
-00019590: 7765 2073 686f 756c 6420 6d61 6e75 616c  we should manual
-000195a0: 6c79 0a20 2020 2020 2020 2020 2020 2020  ly.             
-000195b0: 2020 2023 2065 6a65 6374 2073 746f 7261     # eject stora
-000195c0: 6765 2066 726f 6d20 676c 6f62 616c 5f75  ge from global_u
-000195d0: 7365 725f 7374 6174 6520 616e 6420 6465  ser_state and de
-000195e0: 6c65 7465 2074 6865 2062 7563 6b65 7420  lete the bucket 
-000195f0: 7573 696e 670a 2020 2020 2020 2020 2020  using.          
-00019600: 2020 2020 2020 2320 626f 746f 3320 6469        # boto3 di
-00019610: 7265 6374 6c79 2e0a 2020 2020 2020 2020  rectly..        
-00019620: 2020 2020 2020 2020 7374 6f72 6167 655f          storage_
-00019630: 6f62 6a2e 6465 6c65 7465 2829 0a0a 2020  obj.delete()..  
-00019640: 2020 4070 7974 6573 742e 6669 7874 7572    @pytest.fixtur
-00019650: 650a 2020 2020 6465 6620 746d 705f 6c6f  e.    def tmp_lo
-00019660: 6361 6c5f 7374 6f72 6167 655f 6f62 6a28  cal_storage_obj(
-00019670: 7365 6c66 2c20 746d 705f 6275 636b 6574  self, tmp_bucket
-00019680: 5f6e 616d 652c 2074 6d70 5f73 6f75 7263  _name, tmp_sourc
-00019690: 6529 3a0a 2020 2020 2020 2020 2320 4372  e):.        # Cr
-000196a0: 6561 7465 7320 6120 7465 6d70 6f72 6172  eates a temporar
-000196b0: 7920 7374 6f72 6167 6520 6f62 6a65 6374  y storage object
-000196c0: 2e20 5374 6f72 6573 206d 7573 7420 6265  . Stores must be
-000196d0: 2061 6464 6564 2069 6e20 7468 6520 7465   added in the te
-000196e0: 7374 2e0a 2020 2020 2020 2020 7969 656c  st..        yiel
-000196f0: 6420 6672 6f6d 2073 656c 662e 7969 656c  d from self.yiel
-00019700: 645f 7374 6f72 6167 655f 6f62 6a65 6374  d_storage_object
-00019710: 286e 616d 653d 746d 705f 6275 636b 6574  (name=tmp_bucket
-00019720: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
-00019730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019750: 2020 2020 736f 7572 6365 3d74 6d70 5f73      source=tmp_s
-00019760: 6f75 7263 6529 0a0a 2020 2020 4070 7974  ource)..    @pyt
-00019770: 6573 742e 6669 7874 7572 650a 2020 2020  est.fixture.    
-00019780: 6465 6620 746d 705f 6c6f 6361 6c5f 6c69  def tmp_local_li
-00019790: 7374 5f73 746f 7261 6765 5f6f 626a 2873  st_storage_obj(s
-000197a0: 656c 662c 2074 6d70 5f62 7563 6b65 745f  elf, tmp_bucket_
-000197b0: 6e61 6d65 2c20 746d 705f 736f 7572 6365  name, tmp_source
-000197c0: 293a 0a20 2020 2020 2020 2023 2043 7265  ):.        # Cre
-000197d0: 6174 6573 2061 2074 656d 7020 7374 6f72  ates a temp stor
-000197e0: 6167 6520 6f62 6a65 6374 2077 6869 6368  age object which
-000197f0: 2075 7365 7320 6120 6c69 7374 206f 6620   uses a list of 
-00019800: 7061 7468 7320 6173 2073 6f75 7263 652e  paths as source.
-00019810: 0a20 2020 2020 2020 2023 2053 746f 7265  .        # Store
-00019820: 7320 6d75 7374 2062 6520 6164 6465 6420  s must be added 
-00019830: 696e 2074 6865 2074 6573 742e 2041 6674  in the test. Aft
-00019840: 6572 2075 706c 6f61 642c 2074 6865 2062  er upload, the b
-00019850: 7563 6b65 7420 7368 6f75 6c64 0a20 2020  ucket should.   
-00019860: 2020 2020 2023 2068 6176 6520 7477 6f20       # have two 
-00019870: 6669 6c65 7320 2d20 2f74 6d70 2d66 696c  files - /tmp-fil
-00019880: 6520 616e 6420 2f74 6d70 2d73 6f75 7263  e and /tmp-sourc
-00019890: 652f 746d 702d 6669 6c65 0a20 2020 2020  e/tmp-file.     
-000198a0: 2020 206c 6973 745f 736f 7572 6365 203d     list_source =
-000198b0: 205b 746d 705f 736f 7572 6365 2c20 746d   [tmp_source, tm
-000198c0: 705f 736f 7572 6365 202b 2027 2f74 6d70  p_source + '/tmp
-000198d0: 2d66 696c 6527 5d0a 2020 2020 2020 2020  -file'].        
-000198e0: 7969 656c 6420 6672 6f6d 2073 656c 662e  yield from self.
-000198f0: 7969 656c 645f 7374 6f72 6167 655f 6f62  yield_storage_ob
-00019900: 6a65 6374 286e 616d 653d 746d 705f 6275  ject(name=tmp_bu
-00019910: 636b 6574 5f6e 616d 652c 0a20 2020 2020  cket_name,.     
-00019920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019940: 2020 2020 2020 2020 736f 7572 6365 3d6c          source=l
-00019950: 6973 745f 736f 7572 6365 290a 0a20 2020  ist_source)..   
-00019960: 2040 7079 7465 7374 2e66 6978 7475 7265   @pytest.fixture
-00019970: 0a20 2020 2064 6566 2074 6d70 5f62 756c  .    def tmp_bul
-00019980: 6b5f 6465 6c5f 7374 6f72 6167 655f 6f62  k_del_storage_ob
-00019990: 6a28 7365 6c66 2c20 746d 705f 6275 636b  j(self, tmp_buck
-000199a0: 6574 5f6e 616d 6529 3a0a 2020 2020 2020  et_name):.      
-000199b0: 2020 2320 4372 6561 7465 7320 6120 7465    # Creates a te
-000199c0: 6d70 6f72 6172 7920 7374 6f72 6167 6520  mporary storage 
-000199d0: 6f62 6a65 6374 2066 6f72 2074 6573 7469  object for testi
-000199e0: 6e67 2062 756c 6b20 6465 6c65 7469 6f6e  ng bulk deletion
-000199f0: 2e0a 2020 2020 2020 2020 2320 5374 6f72  ..        # Stor
-00019a00: 6573 206d 7573 7420 6265 2061 6464 6564  es must be added
-00019a10: 2069 6e20 7468 6520 7465 7374 2e0a 2020   in the test..  
-00019a20: 2020 2020 2020 7769 7468 2074 656d 7066        with tempf
-00019a30: 696c 652e 5465 6d70 6f72 6172 7944 6972  ile.TemporaryDir
-00019a40: 6563 746f 7279 2829 2061 7320 746d 7064  ectory() as tmpd
-00019a50: 6972 3a0a 2020 2020 2020 2020 2020 2020  ir:.            
-00019a60: 7375 6270 726f 6365 7373 2e63 6865 636b  subprocess.check
-00019a70: 5f6f 7574 7075 7428 6627 6d6b 6469 7220  _output(f'mkdir 
-00019a80: 2d70 207b 746d 7064 6972 7d2f 666f 6c64  -p {tmpdir}/fold
-00019a90: 6572 7b7b 3030 302e 2e32 3535 7d7d 272c  er{{000..255}}',
-00019aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018e90: 2020 2020 2020 2073 746f 7261 6765 5f6c         storage_l
+00018ea0: 6962 2e41 6273 7472 6163 7453 746f 7265  ib.AbstractStore
+00018eb0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+00018ec0: 2020 2020 2020 2070 6572 7369 7374 656e         persisten
+00018ed0: 743a 204f 7074 696f 6e61 6c5b 626f 6f6c  t: Optional[bool
+00018ee0: 5d20 3d20 5472 7565 2c0a 2020 2020 2020  ] = True,.      
+00018ef0: 2020 2020 2020 6d6f 6465 3a20 7374 6f72        mode: stor
+00018f00: 6167 655f 6c69 622e 5374 6f72 6167 654d  age_lib.StorageM
+00018f10: 6f64 6520 3d20 7374 6f72 6167 655f 6c69  ode = storage_li
+00018f20: 622e 5374 6f72 6167 654d 6f64 652e 4d4f  b.StorageMode.MO
+00018f30: 554e 5429 3a0a 2020 2020 2020 2020 2320  UNT):.        # 
+00018f40: 4372 6561 7465 7320 6120 7465 6d70 6f72  Creates a tempor
+00018f50: 6172 7920 7374 6f72 6167 6520 6f62 6a65  ary storage obje
+00018f60: 6374 2e20 5374 6f72 6573 206d 7573 7420  ct. Stores must 
+00018f70: 6265 2061 6464 6564 2069 6e20 7468 6520  be added in the 
+00018f80: 7465 7374 2e0a 2020 2020 2020 2020 7374  test..        st
+00018f90: 6f72 6167 655f 6f62 6a20 3d20 7374 6f72  orage_obj = stor
+00018fa0: 6167 655f 6c69 622e 5374 6f72 6167 6528  age_lib.Storage(
+00018fb0: 6e61 6d65 3d6e 616d 652c 0a20 2020 2020  name=name,.     
+00018fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fe0: 2020 2020 2073 6f75 7263 653d 736f 7572       source=sour
+00018ff0: 6365 2c0a 2020 2020 2020 2020 2020 2020  ce,.            
+00019000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019010: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00019020: 6f72 6573 3d73 746f 7265 732c 0a20 2020  ores=stores,.   
+00019030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019050: 2020 2020 2020 2070 6572 7369 7374 656e         persisten
+00019060: 743d 7065 7273 6973 7465 6e74 2c0a 2020  t=persistent,.  
+00019070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019090: 2020 2020 2020 2020 6d6f 6465 3d6d 6f64          mode=mod
+000190a0: 6529 0a20 2020 2020 2020 2079 6965 6c64  e).        yield
+000190b0: 2073 746f 7261 6765 5f6f 626a 0a20 2020   storage_obj.   
+000190c0: 2020 2020 2068 616e 646c 6520 3d20 676c       handle = gl
+000190d0: 6f62 616c 5f75 7365 725f 7374 6174 652e  obal_user_state.
+000190e0: 6765 745f 6861 6e64 6c65 5f66 726f 6d5f  get_handle_from_
+000190f0: 7374 6f72 6167 655f 6e61 6d65 280a 2020  storage_name(.  
+00019100: 2020 2020 2020 2020 2020 7374 6f72 6167            storag
+00019110: 655f 6f62 6a2e 6e61 6d65 290a 2020 2020  e_obj.name).    
+00019120: 2020 2020 6966 2068 616e 646c 653a 0a20      if handle:. 
+00019130: 2020 2020 2020 2020 2020 2023 2049 6620             # If 
+00019140: 6861 6e64 6c65 2065 7869 7374 732c 2064  handle exists, d
+00019150: 656c 6574 6520 6d61 6e75 616c 6c79 0a20  elete manually. 
+00019160: 2020 2020 2020 2020 2020 2023 2054 4f44             # TOD
+00019170: 4f28 726f 6d69 6c62 293a 2054 6869 7320  O(romilb): This 
+00019180: 6973 2070 6f74 656e 7469 616c 6c79 2072  is potentially r
+00019190: 6973 6b79 202d 2069 6620 7468 6520 6465  isky - if the de
+000191a0: 6c65 7465 206d 6574 686f 6420 6861 730a  lete method has.
+000191b0: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+000191c0: 6275 6773 2c20 7468 6973 2063 616e 2063  bugs, this can c
+000191d0: 6175 7365 2072 6573 6f75 7263 6520 6c65  ause resource le
+000191e0: 616b 732e 2049 6465 616c 6c79 2077 6520  aks. Ideally we 
+000191f0: 7368 6f75 6c64 206d 616e 7561 6c6c 790a  should manually.
+00019200: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+00019210: 656a 6563 7420 7374 6f72 6167 6520 6672  eject storage fr
+00019220: 6f6d 2067 6c6f 6261 6c5f 7573 6572 5f73  om global_user_s
+00019230: 7461 7465 2061 6e64 2064 656c 6574 6520  tate and delete 
+00019240: 7468 6520 6275 636b 6574 2075 7369 6e67  the bucket using
+00019250: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+00019260: 2062 6f74 6f33 2064 6972 6563 746c 792e   boto3 directly.
+00019270: 0a20 2020 2020 2020 2020 2020 2073 746f  .            sto
+00019280: 7261 6765 5f6f 626a 2e64 656c 6574 6528  rage_obj.delete(
+00019290: 290a 0a20 2020 2040 7079 7465 7374 2e66  )..    @pytest.f
+000192a0: 6978 7475 7265 0a20 2020 2064 6566 2074  ixture.    def t
+000192b0: 6d70 5f73 6372 6174 6368 5f73 746f 7261  mp_scratch_stora
+000192c0: 6765 5f6f 626a 2873 656c 662c 2074 6d70  ge_obj(self, tmp
+000192d0: 5f62 7563 6b65 745f 6e61 6d65 293a 0a20  _bucket_name):. 
+000192e0: 2020 2020 2020 2023 2043 7265 6174 6573         # Creates
+000192f0: 2061 2073 746f 7261 6765 206f 626a 6563   a storage objec
+00019300: 7420 7769 7468 206e 6f20 736f 7572 6365  t with no source
+00019310: 2074 6f20 6372 6561 7465 2061 2073 6372   to create a scr
+00019320: 6174 6368 2073 746f 7261 6765 2e0a 2020  atch storage..  
+00019330: 2020 2020 2020 2320 5374 6f72 6573 206d        # Stores m
+00019340: 7573 7420 6265 2061 6464 6564 2069 6e20  ust be added in 
+00019350: 7468 6520 7465 7374 2e0a 2020 2020 2020  the test..      
+00019360: 2020 7969 656c 6420 6672 6f6d 2073 656c    yield from sel
+00019370: 662e 7969 656c 645f 7374 6f72 6167 655f  f.yield_storage_
+00019380: 6f62 6a65 6374 286e 616d 653d 746d 705f  object(name=tmp_
+00019390: 6275 636b 6574 5f6e 616d 6529 0a0a 2020  bucket_name)..  
+000193a0: 2020 4070 7974 6573 742e 6669 7874 7572    @pytest.fixtur
+000193b0: 650a 2020 2020 6465 6620 746d 705f 6d75  e.    def tmp_mu
+000193c0: 6c74 6970 6c65 5f73 6372 6174 6368 5f73  ltiple_scratch_s
+000193d0: 746f 7261 6765 5f6f 626a 2873 656c 6629  torage_obj(self)
+000193e0: 3a0a 2020 2020 2020 2020 2320 4372 6561  :.        # Crea
+000193f0: 7465 7320 6120 6c69 7374 206f 6620 3520  tes a list of 5 
+00019400: 7374 6f72 6167 6520 6f62 6a65 6374 7320  storage objects 
+00019410: 7769 7468 206e 6f20 736f 7572 6365 2074  with no source t
+00019420: 6f20 6372 6561 7465 0a20 2020 2020 2020  o create.       
+00019430: 2023 206d 756c 7469 706c 6520 7363 7261   # multiple scra
+00019440: 7463 6820 7374 6f72 6167 6573 2e0a 2020  tch storages..  
+00019450: 2020 2020 2020 2320 5374 6f72 6573 2066        # Stores f
+00019460: 6f72 2065 6163 6820 6f62 6a65 6374 2069  or each object i
+00019470: 6e20 7468 6520 6c69 7374 206d 7573 7420  n the list must 
+00019480: 6265 2061 6464 6564 2069 6e20 7468 6520  be added in the 
+00019490: 7465 7374 2e0a 2020 2020 2020 2020 7374  test..        st
+000194a0: 6f72 6167 655f 6d75 6c74 5f6f 626a 203d  orage_mult_obj =
+000194b0: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
+000194c0: 5f20 696e 2072 616e 6765 2835 293a 0a20  _ in range(5):. 
+000194d0: 2020 2020 2020 2020 2020 2074 696d 6573             times
+000194e0: 7461 6d70 203d 2073 7472 2874 696d 652e  tamp = str(time.
+000194f0: 7469 6d65 2829 292e 7265 706c 6163 6528  time()).replace(
+00019500: 272e 272c 2027 2729 0a20 2020 2020 2020  '.', '').       
+00019510: 2020 2020 2073 746f 7265 5f6f 626a 203d       store_obj =
+00019520: 2073 746f 7261 6765 5f6c 6962 2e53 746f   storage_lib.Sto
+00019530: 7261 6765 286e 616d 653d 6627 736b 792d  rage(name=f'sky-
+00019540: 7465 7374 2d7b 7469 6d65 7374 616d 707d  test-{timestamp}
+00019550: 2729 0a20 2020 2020 2020 2020 2020 2073  ').            s
+00019560: 746f 7261 6765 5f6d 756c 745f 6f62 6a2e  torage_mult_obj.
+00019570: 6170 7065 6e64 2873 746f 7265 5f6f 626a  append(store_obj
+00019580: 290a 2020 2020 2020 2020 7969 656c 6420  ).        yield 
+00019590: 7374 6f72 6167 655f 6d75 6c74 5f6f 626a  storage_mult_obj
+000195a0: 0a20 2020 2020 2020 2066 6f72 2073 746f  .        for sto
+000195b0: 7261 6765 5f6f 626a 2069 6e20 7374 6f72  rage_obj in stor
+000195c0: 6167 655f 6d75 6c74 5f6f 626a 3a0a 2020  age_mult_obj:.  
+000195d0: 2020 2020 2020 2020 2020 6861 6e64 6c65            handle
+000195e0: 203d 2067 6c6f 6261 6c5f 7573 6572 5f73   = global_user_s
+000195f0: 7461 7465 2e67 6574 5f68 616e 646c 655f  tate.get_handle_
+00019600: 6672 6f6d 5f73 746f 7261 6765 5f6e 616d  from_storage_nam
+00019610: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+00019620: 2020 2073 746f 7261 6765 5f6f 626a 2e6e     storage_obj.n
+00019630: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
+00019640: 2069 6620 6861 6e64 6c65 3a0a 2020 2020   if handle:.    
+00019650: 2020 2020 2020 2020 2020 2020 2320 4966              # If
+00019660: 2068 616e 646c 6520 6578 6973 7473 2c20   handle exists, 
+00019670: 6465 6c65 7465 206d 616e 7561 6c6c 790a  delete manually.
+00019680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019690: 2320 544f 444f 2872 6f6d 696c 6229 3a20  # TODO(romilb): 
+000196a0: 5468 6973 2069 7320 706f 7465 6e74 6961  This is potentia
+000196b0: 6c6c 7920 7269 736b 7920 2d20 6966 2074  lly risky - if t
+000196c0: 6865 2064 656c 6574 6520 6d65 7468 6f64  he delete method
+000196d0: 2068 6173 0a20 2020 2020 2020 2020 2020   has.           
+000196e0: 2020 2020 2023 2062 7567 732c 2074 6869       # bugs, thi
+000196f0: 7320 6361 6e20 6361 7573 6520 7265 736f  s can cause reso
+00019700: 7572 6365 206c 6561 6b73 2e20 4964 6561  urce leaks. Idea
+00019710: 6c6c 7920 7765 2073 686f 756c 6420 6d61  lly we should ma
+00019720: 6e75 616c 6c79 0a20 2020 2020 2020 2020  nually.         
+00019730: 2020 2020 2020 2023 2065 6a65 6374 2073         # eject s
+00019740: 746f 7261 6765 2066 726f 6d20 676c 6f62  torage from glob
+00019750: 616c 5f75 7365 725f 7374 6174 6520 616e  al_user_state an
+00019760: 6420 6465 6c65 7465 2074 6865 2062 7563  d delete the buc
+00019770: 6b65 7420 7573 696e 670a 2020 2020 2020  ket using.      
+00019780: 2020 2020 2020 2020 2020 2320 626f 746f            # boto
+00019790: 3320 6469 7265 6374 6c79 2e0a 2020 2020  3 directly..    
+000197a0: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
+000197b0: 6167 655f 6f62 6a2e 6465 6c65 7465 2829  age_obj.delete()
+000197c0: 0a0a 2020 2020 4070 7974 6573 742e 6669  ..    @pytest.fi
+000197d0: 7874 7572 650a 2020 2020 6465 6620 746d  xture.    def tm
+000197e0: 705f 6c6f 6361 6c5f 7374 6f72 6167 655f  p_local_storage_
+000197f0: 6f62 6a28 7365 6c66 2c20 746d 705f 6275  obj(self, tmp_bu
+00019800: 636b 6574 5f6e 616d 652c 2074 6d70 5f73  cket_name, tmp_s
+00019810: 6f75 7263 6529 3a0a 2020 2020 2020 2020  ource):.        
+00019820: 2320 4372 6561 7465 7320 6120 7465 6d70  # Creates a temp
+00019830: 6f72 6172 7920 7374 6f72 6167 6520 6f62  orary storage ob
+00019840: 6a65 6374 2e20 5374 6f72 6573 206d 7573  ject. Stores mus
+00019850: 7420 6265 2061 6464 6564 2069 6e20 7468  t be added in th
+00019860: 6520 7465 7374 2e0a 2020 2020 2020 2020  e test..        
+00019870: 7969 656c 6420 6672 6f6d 2073 656c 662e  yield from self.
+00019880: 7969 656c 645f 7374 6f72 6167 655f 6f62  yield_storage_ob
+00019890: 6a65 6374 286e 616d 653d 746d 705f 6275  ject(name=tmp_bu
+000198a0: 636b 6574 5f6e 616d 652c 0a20 2020 2020  cket_name,.     
+000198b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198d0: 2020 2020 2020 2020 736f 7572 6365 3d74          source=t
+000198e0: 6d70 5f73 6f75 7263 6529 0a0a 2020 2020  mp_source)..    
+000198f0: 4070 7974 6573 742e 6669 7874 7572 650a  @pytest.fixture.
+00019900: 2020 2020 6465 6620 746d 705f 6c6f 6361      def tmp_loca
+00019910: 6c5f 6c69 7374 5f73 746f 7261 6765 5f6f  l_list_storage_o
+00019920: 626a 2873 656c 662c 2074 6d70 5f62 7563  bj(self, tmp_buc
+00019930: 6b65 745f 6e61 6d65 2c20 746d 705f 736f  ket_name, tmp_so
+00019940: 7572 6365 293a 0a20 2020 2020 2020 2023  urce):.        #
+00019950: 2043 7265 6174 6573 2061 2074 656d 7020   Creates a temp 
+00019960: 7374 6f72 6167 6520 6f62 6a65 6374 2077  storage object w
+00019970: 6869 6368 2075 7365 7320 6120 6c69 7374  hich uses a list
+00019980: 206f 6620 7061 7468 7320 6173 2073 6f75   of paths as sou
+00019990: 7263 652e 0a20 2020 2020 2020 2023 2053  rce..        # S
+000199a0: 746f 7265 7320 6d75 7374 2062 6520 6164  tores must be ad
+000199b0: 6465 6420 696e 2074 6865 2074 6573 742e  ded in the test.
+000199c0: 2041 6674 6572 2075 706c 6f61 642c 2074   After upload, t
+000199d0: 6865 2062 7563 6b65 7420 7368 6f75 6c64  he bucket should
+000199e0: 0a20 2020 2020 2020 2023 2068 6176 6520  .        # have 
+000199f0: 7477 6f20 6669 6c65 7320 2d20 2f74 6d70  two files - /tmp
+00019a00: 2d66 696c 6520 616e 6420 2f74 6d70 2d73  -file and /tmp-s
+00019a10: 6f75 7263 652f 746d 702d 6669 6c65 0a20  ource/tmp-file. 
+00019a20: 2020 2020 2020 206c 6973 745f 736f 7572         list_sour
+00019a30: 6365 203d 205b 746d 705f 736f 7572 6365  ce = [tmp_source
+00019a40: 2c20 746d 705f 736f 7572 6365 202b 2027  , tmp_source + '
+00019a50: 2f74 6d70 2d66 696c 6527 5d0a 2020 2020  /tmp-file'].    
+00019a60: 2020 2020 7969 656c 6420 6672 6f6d 2073      yield from s
+00019a70: 656c 662e 7969 656c 645f 7374 6f72 6167  elf.yield_storag
+00019a80: 655f 6f62 6a65 6374 286e 616d 653d 746d  e_object(name=tm
+00019a90: 705f 6275 636b 6574 5f6e 616d 652c 0a20  p_bucket_name,. 
+00019aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ac0: 2020 2020 2073 6865 6c6c 3d54 7275 6529       shell=True)
-00019ad0: 0a20 2020 2020 2020 2020 2020 2073 7562  .            sub
-00019ae0: 7072 6f63 6573 732e 6368 6563 6b5f 6f75  process.check_ou
-00019af0: 7470 7574 2866 2774 6f75 6368 207b 746d  tput(f'touch {tm
-00019b00: 7064 6972 7d2f 7465 7374 7b7b 3030 302e  pdir}/test{{000.
-00019b10: 2e32 3535 7d7d 2e74 7874 272c 0a20 2020  .255}}.txt',.   
-00019b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b40: 2073 6865 6c6c 3d54 7275 6529 0a20 2020   shell=True).   
-00019b50: 2020 2020 2020 2020 2073 7562 7072 6f63           subproc
-00019b60: 6573 732e 6368 6563 6b5f 6f75 7470 7574  ess.check_output
-00019b70: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00019b80: 2020 6627 746f 7563 6820 7b74 6d70 6469    f'touch {tmpdi
-00019b90: 727d 2f66 6f6c 6465 727b 7b30 3030 2e2e  r}/folder{{000..
-00019ba0: 3235 357d 7d2f 7465 7374 2e74 7874 272c  255}}/test.txt',
-00019bb0: 2073 6865 6c6c 3d54 7275 6529 0a20 2020   shell=True).   
-00019bc0: 2020 2020 2020 2020 2079 6965 6c64 2066           yield f
-00019bd0: 726f 6d20 7365 6c66 2e79 6965 6c64 5f73  rom self.yield_s
-00019be0: 746f 7261 6765 5f6f 626a 6563 7428 6e61  torage_object(na
-00019bf0: 6d65 3d74 6d70 5f62 7563 6b65 745f 6e61  me=tmp_bucket_na
-00019c00: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-00019c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c30: 2020 2020 2073 6f75 7263 653d 746d 7064       source=tmpd
-00019c40: 6972 290a 0a20 2020 2040 7079 7465 7374  ir)..    @pytest
-00019c50: 2e66 6978 7475 7265 0a20 2020 2064 6566  .fixture.    def
-00019c60: 2074 6d70 5f63 6f70 795f 6d6e 745f 6578   tmp_copy_mnt_ex
-00019c70: 6973 7469 6e67 5f73 746f 7261 6765 5f6f  isting_storage_o
-00019c80: 626a 2873 656c 662c 2074 6d70 5f73 6372  bj(self, tmp_scr
-00019c90: 6174 6368 5f73 746f 7261 6765 5f6f 626a  atch_storage_obj
-00019ca0: 293a 0a20 2020 2020 2020 2023 2043 7265  ):.        # Cre
-00019cb0: 6174 6573 2061 2063 6f70 7920 6d6f 756e  ates a copy moun
-00019cc0: 7420 7374 6f72 6167 6520 7768 6963 6820  t storage which 
-00019cd0: 7265 7573 6573 2061 6e20 6578 6973 7469  reuses an existi
-00019ce0: 6e67 2073 746f 7261 6765 206f 626a 6563  ng storage objec
-00019cf0: 742e 0a20 2020 2020 2020 2074 6d70 5f73  t..        tmp_s
-00019d00: 6372 6174 6368 5f73 746f 7261 6765 5f6f  cratch_storage_o
-00019d10: 626a 2e61 6464 5f73 746f 7265 2873 746f  bj.add_store(sto
-00019d20: 7261 6765 5f6c 6962 2e53 746f 7265 5479  rage_lib.StoreTy
-00019d30: 7065 2e53 3329 0a20 2020 2020 2020 2073  pe.S3).        s
-00019d40: 746f 7261 6765 5f6e 616d 6520 3d20 746d  torage_name = tm
-00019d50: 705f 7363 7261 7463 685f 7374 6f72 6167  p_scratch_storag
-00019d60: 655f 6f62 6a2e 6e61 6d65 0a0a 2020 2020  e_obj.name..    
-00019d70: 2020 2020 2320 5472 7920 746f 2069 6e69      # Try to ini
-00019d80: 7469 616c 697a 6520 616e 6f74 6865 7220  tialize another 
-00019d90: 7374 6f72 6167 6520 7769 7468 2074 6865  storage with the
-00019da0: 2073 746f 7261 6765 206f 626a 6563 7420   storage object 
-00019db0: 6372 6561 7465 640a 2020 2020 2020 2020  created.        
-00019dc0: 2320 6162 6f76 652c 2062 7574 206e 6f77  # above, but now
-00019dd0: 2069 6e20 434f 5059 206d 6f64 652e 2054   in COPY mode. T
-00019de0: 6869 7320 7368 6f75 6c64 2073 7563 6365  his should succe
-00019df0: 6564 2e0a 2020 2020 2020 2020 7969 656c  ed..        yiel
-00019e00: 6420 6672 6f6d 2073 656c 662e 7969 656c  d from self.yiel
-00019e10: 645f 7374 6f72 6167 655f 6f62 6a65 6374  d_storage_object
-00019e20: 286e 616d 653d 7374 6f72 6167 655f 6e61  (name=storage_na
-00019e30: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-00019e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019e60: 206d 6f64 653d 7374 6f72 6167 655f 6c69   mode=storage_li
-00019e70: 622e 5374 6f72 6167 654d 6f64 652e 434f  b.StorageMode.CO
-00019e80: 5059 290a 0a20 2020 2040 7079 7465 7374  PY)..    @pytest
-00019e90: 2e66 6978 7475 7265 0a20 2020 2064 6566  .fixture.    def
-00019ea0: 2074 6d70 5f61 7773 636c 695f 6275 636b   tmp_awscli_buck
-00019eb0: 6574 2873 656c 662c 2074 6d70 5f62 7563  et(self, tmp_buc
-00019ec0: 6b65 745f 6e61 6d65 293a 0a20 2020 2020  ket_name):.     
-00019ed0: 2020 2023 2043 7265 6174 6573 2061 2074     # Creates a t
-00019ee0: 656d 706f 7261 7279 2062 7563 6b65 7420  emporary bucket 
-00019ef0: 7573 696e 6720 6177 7363 6c69 0a20 2020  using awscli.   
-00019f00: 2020 2020 2073 7562 7072 6f63 6573 732e       subprocess.
-00019f10: 6368 6563 6b5f 6361 6c6c 285b 2761 7773  check_call(['aws
-00019f20: 272c 2027 7333 272c 2027 6d62 272c 2066  ', 's3', 'mb', f
-00019f30: 2773 333a 2f2f 7b74 6d70 5f62 7563 6b65  's3://{tmp_bucke
-00019f40: 745f 6e61 6d65 7d27 5d29 0a20 2020 2020  t_name}']).     
-00019f50: 2020 2079 6965 6c64 2074 6d70 5f62 7563     yield tmp_buc
-00019f60: 6b65 745f 6e61 6d65 0a20 2020 2020 2020  ket_name.       
-00019f70: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
-00019f80: 6b5f 6361 6c6c 280a 2020 2020 2020 2020  k_call(.        
-00019f90: 2020 2020 5b27 6177 7327 2c20 2773 3327      ['aws', 's3'
-00019fa0: 2c20 2772 6227 2c20 6627 7333 3a2f 2f7b  , 'rb', f's3://{
-00019fb0: 746d 705f 6275 636b 6574 5f6e 616d 657d  tmp_bucket_name}
-00019fc0: 272c 2027 2d2d 666f 7263 6527 5d29 0a0a  ', '--force'])..
-00019fd0: 2020 2020 4070 7974 6573 742e 6669 7874      @pytest.fixt
-00019fe0: 7572 650a 2020 2020 6465 6620 746d 705f  ure.    def tmp_
-00019ff0: 6773 7574 696c 5f62 7563 6b65 7428 7365  gsutil_bucket(se
-0001a000: 6c66 2c20 746d 705f 6275 636b 6574 5f6e  lf, tmp_bucket_n
-0001a010: 616d 6529 3a0a 2020 2020 2020 2020 2320  ame):.        # 
-0001a020: 4372 6561 7465 7320 6120 7465 6d70 6f72  Creates a tempor
-0001a030: 6172 7920 6275 636b 6574 2075 7369 6e67  ary bucket using
-0001a040: 2067 7375 7469 6c0a 2020 2020 2020 2020   gsutil.        
-0001a050: 7375 6270 726f 6365 7373 2e63 6865 636b  subprocess.check
-0001a060: 5f63 616c 6c28 5b27 6773 7574 696c 272c  _call(['gsutil',
-0001a070: 2027 6d62 272c 2066 2767 733a 2f2f 7b74   'mb', f'gs://{t
-0001a080: 6d70 5f62 7563 6b65 745f 6e61 6d65 7d27  mp_bucket_name}'
-0001a090: 5d29 0a20 2020 2020 2020 2079 6965 6c64  ]).        yield
-0001a0a0: 2074 6d70 5f62 7563 6b65 745f 6e61 6d65   tmp_bucket_name
-0001a0b0: 0a20 2020 2020 2020 2073 7562 7072 6f63  .        subproc
-0001a0c0: 6573 732e 6368 6563 6b5f 6361 6c6c 285b  ess.check_call([
-0001a0d0: 2767 7375 7469 6c27 2c20 2772 6d27 2c20  'gsutil', 'rm', 
-0001a0e0: 272d 7227 2c20 6627 6773 3a2f 2f7b 746d  '-r', f'gs://{tm
-0001a0f0: 705f 6275 636b 6574 5f6e 616d 657d 275d  p_bucket_name}']
-0001a100: 290a 0a20 2020 2040 7079 7465 7374 2e66  )..    @pytest.f
-0001a110: 6978 7475 7265 0a20 2020 2064 6566 2074  ixture.    def t
-0001a120: 6d70 5f61 7773 636c 695f 6275 636b 6574  mp_awscli_bucket
-0001a130: 5f72 3228 7365 6c66 2c20 746d 705f 6275  _r2(self, tmp_bu
-0001a140: 636b 6574 5f6e 616d 6529 3a0a 2020 2020  cket_name):.    
-0001a150: 2020 2020 2320 4372 6561 7465 7320 6120      # Creates a 
-0001a160: 7465 6d70 6f72 6172 7920 6275 636b 6574  temporary bucket
-0001a170: 2075 7369 6e67 2061 7773 636c 690a 2020   using awscli.  
-0001a180: 2020 2020 2020 656e 6470 6f69 6e74 5f75        endpoint_u
-0001a190: 726c 203d 2063 6c6f 7564 666c 6172 652e  rl = cloudflare.
-0001a1a0: 6372 6561 7465 5f65 6e64 706f 696e 7428  create_endpoint(
-0001a1b0: 290a 2020 2020 2020 2020 7375 6270 726f  ).        subpro
-0001a1c0: 6365 7373 2e63 6865 636b 5f63 616c 6c28  cess.check_call(
-0001a1d0: 0a20 2020 2020 2020 2020 2020 2066 2741  .            f'A
-0001a1e0: 5753 5f53 4841 5245 445f 4352 4544 454e  WS_SHARED_CREDEN
-0001a1f0: 5449 414c 535f 4649 4c45 3d7b 636c 6f75  TIALS_FILE={clou
-0001a200: 6466 6c61 7265 2e52 325f 4352 4544 454e  dflare.R2_CREDEN
-0001a210: 5449 414c 535f 5041 5448 7d20 6177 7320  TIALS_PATH} aws 
-0001a220: 7333 206d 6220 7333 3a2f 2f7b 746d 705f  s3 mb s3://{tmp_
-0001a230: 6275 636b 6574 5f6e 616d 657d 202d 2d65  bucket_name} --e
-0001a240: 6e64 706f 696e 7420 7b65 6e64 706f 696e  ndpoint {endpoin
-0001a250: 745f 7572 6c7d 202d 2d70 726f 6669 6c65  t_url} --profile
-0001a260: 3d72 3227 2c0a 2020 2020 2020 2020 2020  =r2',.          
-0001a270: 2020 7368 656c 6c3d 5472 7565 290a 2020    shell=True).  
-0001a280: 2020 2020 2020 7969 656c 6420 746d 705f        yield tmp_
-0001a290: 6275 636b 6574 5f6e 616d 650a 2020 2020  bucket_name.    
-0001a2a0: 2020 2020 7375 6270 726f 6365 7373 2e63      subprocess.c
-0001a2b0: 6865 636b 5f63 616c 6c28 0a20 2020 2020  heck_call(.     
-0001a2c0: 2020 2020 2020 2066 2741 5753 5f53 4841         f'AWS_SHA
-0001a2d0: 5245 445f 4352 4544 454e 5449 414c 535f  RED_CREDENTIALS_
-0001a2e0: 4649 4c45 3d7b 636c 6f75 6466 6c61 7265  FILE={cloudflare
-0001a2f0: 2e52 325f 4352 4544 454e 5449 414c 535f  .R2_CREDENTIALS_
-0001a300: 5041 5448 7d20 6177 7320 7333 2072 6220  PATH} aws s3 rb 
-0001a310: 7333 3a2f 2f7b 746d 705f 6275 636b 6574  s3://{tmp_bucket
-0001a320: 5f6e 616d 657d 202d 2d66 6f72 6365 202d  _name} --force -
-0001a330: 2d65 6e64 706f 696e 7420 7b65 6e64 706f  -endpoint {endpo
-0001a340: 696e 745f 7572 6c7d 202d 2d70 726f 6669  int_url} --profi
-0001a350: 6c65 3d72 3227 2c0a 2020 2020 2020 2020  le=r2',.        
-0001a360: 2020 2020 7368 656c 6c3d 5472 7565 290a      shell=True).
-0001a370: 0a20 2020 2040 7079 7465 7374 2e66 6978  .    @pytest.fix
-0001a380: 7475 7265 0a20 2020 2064 6566 2074 6d70  ture.    def tmp
-0001a390: 5f70 7562 6c69 635f 7374 6f72 6167 655f  _public_storage_
-0001a3a0: 6f62 6a28 7365 6c66 2c20 7265 7175 6573  obj(self, reques
-0001a3b0: 7429 3a0a 2020 2020 2020 2020 2320 496e  t):.        # In
-0001a3c0: 6974 6961 6c69 7a65 7320 6120 7374 6f72  itializes a stor
-0001a3d0: 6167 6520 6f62 6a65 6374 2077 6974 6820  age object with 
-0001a3e0: 6120 7075 626c 6963 2062 7563 6b65 740a  a public bucket.
-0001a3f0: 2020 2020 2020 2020 7374 6f72 6167 655f          storage_
-0001a400: 6f62 6a20 3d20 7374 6f72 6167 655f 6c69  obj = storage_li
-0001a410: 622e 5374 6f72 6167 6528 736f 7572 6365  b.Storage(source
-0001a420: 3d72 6571 7565 7374 2e70 6172 616d 290a  =request.param).
-0001a430: 2020 2020 2020 2020 7969 656c 6420 7374          yield st
-0001a440: 6f72 6167 655f 6f62 6a0a 2020 2020 2020  orage_obj.      
-0001a450: 2020 2320 5468 6973 2064 6f65 7320 6e6f    # This does no
-0001a460: 7420 7265 7175 6972 6520 616e 7920 6465  t require any de
-0001a470: 6c65 7469 6f6e 206c 6f67 6963 2062 6563  letion logic bec
-0001a480: 6175 7365 2069 7420 6973 2061 2070 7562  ause it is a pub
-0001a490: 6c69 6320 6275 636b 6574 0a20 2020 2020  lic bucket.     
-0001a4a0: 2020 2023 2061 6e64 2073 686f 756c 6420     # and should 
-0001a4b0: 6e6f 7420 6765 7420 6164 6465 6420 746f  not get added to
-0001a4c0: 2067 6c6f 6261 6c5f 7573 6572 5f73 7461   global_user_sta
-0001a4d0: 7465 2e0a 0a20 2020 2040 7079 7465 7374  te...    @pytest
-0001a4e0: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
-0001a4f0: 6528 2773 746f 7265 5f74 7970 6527 2c20  e('store_type', 
-0001a500: 5b0a 2020 2020 2020 2020 7374 6f72 6167  [.        storag
-0001a510: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
-0001a520: 5333 2c20 7374 6f72 6167 655f 6c69 622e  S3, storage_lib.
-0001a530: 5374 6f72 6554 7970 652e 4743 532c 0a20  StoreType.GCS,. 
-0001a540: 2020 2020 2020 2070 7974 6573 742e 7061         pytest.pa
-0001a550: 7261 6d28 7374 6f72 6167 655f 6c69 622e  ram(storage_lib.
-0001a560: 5374 6f72 6554 7970 652e 5232 2c20 6d61  StoreType.R2, ma
-0001a570: 726b 733d 7079 7465 7374 2e6d 6172 6b2e  rks=pytest.mark.
-0001a580: 636c 6f75 6466 6c61 7265 290a 2020 2020  cloudflare).    
-0001a590: 5d29 0a20 2020 2064 6566 2074 6573 745f  ]).    def test_
-0001a5a0: 6e65 775f 6275 636b 6574 5f63 7265 6174  new_bucket_creat
-0001a5b0: 696f 6e5f 616e 645f 6465 6c65 7469 6f6e  ion_and_deletion
-0001a5c0: 2873 656c 662c 2074 6d70 5f6c 6f63 616c  (self, tmp_local
-0001a5d0: 5f73 746f 7261 6765 5f6f 626a 2c0a 2020  _storage_obj,.  
-0001a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a600: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
-0001a610: 655f 7479 7065 293a 0a20 2020 2020 2020  e_type):.       
-0001a620: 2023 2043 7265 6174 6573 2061 206e 6577   # Creates a new
-0001a630: 2062 7563 6b65 7420 7769 7468 2061 206c   bucket with a l
-0001a640: 6f63 616c 2073 6f75 7263 652c 2075 706c  ocal source, upl
-0001a650: 6f61 6473 2066 696c 6573 2074 6f20 6974  oads files to it
-0001a660: 0a20 2020 2020 2020 2023 2061 6e64 2064  .        # and d
-0001a670: 656c 6574 6573 2069 742e 0a20 2020 2020  eletes it..     
-0001a680: 2020 2074 6d70 5f6c 6f63 616c 5f73 746f     tmp_local_sto
-0001a690: 7261 6765 5f6f 626a 2e61 6464 5f73 746f  rage_obj.add_sto
-0001a6a0: 7265 2873 746f 7265 5f74 7970 6529 0a0a  re(store_type)..
-0001a6b0: 2020 2020 2020 2020 2320 5275 6e20 736b          # Run sk
-0001a6c0: 7920 7374 6f72 6167 6520 6c73 2074 6f20  y storage ls to 
-0001a6d0: 6368 6563 6b20 6966 2073 746f 7261 6765  check if storage
-0001a6e0: 206f 626a 6563 7420 6578 6973 7473 2069   object exists i
-0001a6f0: 6e20 7468 6520 6f75 7470 7574 0a20 2020  n the output.   
-0001a700: 2020 2020 206f 7574 203d 2073 7562 7072       out = subpr
-0001a710: 6f63 6573 732e 6368 6563 6b5f 6f75 7470  ocess.check_outp
-0001a720: 7574 285b 2773 6b79 272c 2027 7374 6f72  ut(['sky', 'stor
-0001a730: 6167 6527 2c20 276c 7327 5d29 0a20 2020  age', 'ls']).   
-0001a740: 2020 2020 2061 7373 6572 7420 746d 705f       assert tmp_
-0001a750: 6c6f 6361 6c5f 7374 6f72 6167 655f 6f62  local_storage_ob
-0001a760: 6a2e 6e61 6d65 2069 6e20 6f75 742e 6465  j.name in out.de
-0001a770: 636f 6465 2827 7574 662d 3827 290a 0a20  code('utf-8').. 
-0001a780: 2020 2020 2020 2023 2052 756e 2073 6b79         # Run sky
-0001a790: 2073 746f 7261 6765 2064 656c 6574 6520   storage delete 
-0001a7a0: 746f 2064 656c 6574 6520 7468 6520 7374  to delete the st
-0001a7b0: 6f72 6167 6520 6f62 6a65 6374 0a20 2020  orage object.   
-0001a7c0: 2020 2020 2073 7562 7072 6f63 6573 732e       subprocess.
-0001a7d0: 6368 6563 6b5f 6f75 7470 7574 280a 2020  check_output(.  
-0001a7e0: 2020 2020 2020 2020 2020 5b27 736b 7927            ['sky'
-0001a7f0: 2c20 2773 746f 7261 6765 272c 2027 6465  , 'storage', 'de
-0001a800: 6c65 7465 272c 2074 6d70 5f6c 6f63 616c  lete', tmp_local
-0001a810: 5f73 746f 7261 6765 5f6f 626a 2e6e 616d  _storage_obj.nam
-0001a820: 655d 290a 0a20 2020 2020 2020 2023 2052  e])..        # R
-0001a830: 756e 2073 6b79 2073 746f 7261 6765 206c  un sky storage l
-0001a840: 7320 746f 2063 6865 636b 2069 6620 7374  s to check if st
-0001a850: 6f72 6167 6520 6f62 6a65 6374 2069 7320  orage object is 
-0001a860: 6465 6c65 7465 640a 2020 2020 2020 2020  deleted.        
-0001a870: 6f75 7420 3d20 7375 6270 726f 6365 7373  out = subprocess
-0001a880: 2e63 6865 636b 5f6f 7574 7075 7428 5b27  .check_output(['
-0001a890: 736b 7927 2c20 2773 746f 7261 6765 272c  sky', 'storage',
-0001a8a0: 2027 6c73 275d 290a 2020 2020 2020 2020   'ls']).        
-0001a8b0: 6173 7365 7274 2074 6d70 5f6c 6f63 616c  assert tmp_local
-0001a8c0: 5f73 746f 7261 6765 5f6f 626a 2e6e 616d  _storage_obj.nam
-0001a8d0: 6520 6e6f 7420 696e 206f 7574 2e64 6563  e not in out.dec
-0001a8e0: 6f64 6528 2775 7466 2d38 2729 0a0a 2020  ode('utf-8')..  
-0001a8f0: 2020 4070 7974 6573 742e 6d61 726b 2e78    @pytest.mark.x
-0001a900: 6469 7374 5f67 726f 7570 2827 6d75 6c74  dist_group('mult
-0001a910: 6970 6c65 5f62 7563 6b65 745f 6465 6c65  iple_bucket_dele
-0001a920: 7469 6f6e 2729 0a20 2020 2040 7079 7465  tion').    @pyte
-0001a930: 7374 2e6d 6172 6b2e 7061 7261 6d65 7472  st.mark.parametr
-0001a940: 697a 6528 2773 746f 7265 5f74 7970 6527  ize('store_type'
-0001a950: 2c20 5b0a 2020 2020 2020 2020 7374 6f72  , [.        stor
-0001a960: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
-0001a970: 652e 5333 2c20 7374 6f72 6167 655f 6c69  e.S3, storage_li
-0001a980: 622e 5374 6f72 6554 7970 652e 4743 532c  b.StoreType.GCS,
-0001a990: 0a20 2020 2020 2020 2070 7974 6573 742e  .        pytest.
-0001a9a0: 7061 7261 6d28 7374 6f72 6167 655f 6c69  param(storage_li
-0001a9b0: 622e 5374 6f72 6554 7970 652e 5232 2c20  b.StoreType.R2, 
-0001a9c0: 6d61 726b 733d 7079 7465 7374 2e6d 6172  marks=pytest.mar
-0001a9d0: 6b2e 636c 6f75 6466 6c61 7265 290a 2020  k.cloudflare).  
-0001a9e0: 2020 5d29 0a20 2020 2064 6566 2074 6573    ]).    def tes
-0001a9f0: 745f 6d75 6c74 6970 6c65 5f62 7563 6b65  t_multiple_bucke
-0001aa00: 7473 5f63 7265 6174 696f 6e5f 616e 645f  ts_creation_and_
-0001aa10: 6465 6c65 7469 6f6e 280a 2020 2020 2020  deletion(.      
-0001aa20: 2020 2020 2020 7365 6c66 2c20 746d 705f        self, tmp_
-0001aa30: 6d75 6c74 6970 6c65 5f73 6372 6174 6368  multiple_scratch
-0001aa40: 5f73 746f 7261 6765 5f6f 626a 2c20 7374  _storage_obj, st
-0001aa50: 6f72 655f 7479 7065 293a 0a20 2020 2020  ore_type):.     
-0001aa60: 2020 2023 2043 7265 6174 6573 206d 756c     # Creates mul
-0001aa70: 7469 706c 6520 6e65 7720 6275 636b 6574  tiple new bucket
-0001aa80: 7328 3520 6275 636b 6574 7329 2077 6974  s(5 buckets) wit
-0001aa90: 6820 6120 6c6f 6361 6c20 736f 7572 6365  h a local source
-0001aaa0: 0a20 2020 2020 2020 2023 2061 6e64 2064  .        # and d
-0001aab0: 656c 6574 6573 2074 6865 6d2e 0a20 2020  eletes them..   
-0001aac0: 2020 2020 2073 746f 7261 6765 5f6f 626a       storage_obj
-0001aad0: 5f6e 616d 6520 3d20 5b5d 0a20 2020 2020  _name = [].     
-0001aae0: 2020 2066 6f72 2073 746f 7265 5f6f 626a     for store_obj
-0001aaf0: 2069 6e20 746d 705f 6d75 6c74 6970 6c65   in tmp_multiple
-0001ab00: 5f73 6372 6174 6368 5f73 746f 7261 6765  _scratch_storage
-0001ab10: 5f6f 626a 3a0a 2020 2020 2020 2020 2020  _obj:.          
-0001ab20: 2020 7374 6f72 655f 6f62 6a2e 6164 645f    store_obj.add_
-0001ab30: 7374 6f72 6528 7374 6f72 655f 7479 7065  store(store_type
-0001ab40: 290a 2020 2020 2020 2020 2020 2020 7374  ).            st
-0001ab50: 6f72 6167 655f 6f62 6a5f 6e61 6d65 2e61  orage_obj_name.a
-0001ab60: 7070 656e 6428 7374 6f72 655f 6f62 6a2e  ppend(store_obj.
-0001ab70: 6e61 6d65 290a 0a20 2020 2020 2020 2023  name)..        #
-0001ab80: 2052 756e 2073 6b79 2073 746f 7261 6765   Run sky storage
-0001ab90: 206c 7320 746f 2063 6865 636b 2069 6620   ls to check if 
-0001aba0: 616c 6c20 7374 6f72 6167 6520 6f62 6a65  all storage obje
-0001abb0: 6374 7320 6578 6973 7473 2069 6e20 7468  cts exists in th
-0001abc0: 650a 2020 2020 2020 2020 2320 6f75 7470  e.        # outp
-0001abd0: 7574 2066 696c 7465 7265 6420 6279 2073  ut filtered by s
-0001abe0: 746f 7265 2074 7970 650a 2020 2020 2020  tore type.      
-0001abf0: 2020 6f75 745f 616c 6c20 3d20 7375 6270    out_all = subp
-0001ac00: 726f 6365 7373 2e63 6865 636b 5f6f 7574  rocess.check_out
-0001ac10: 7075 7428 5b27 736b 7927 2c20 2773 746f  put(['sky', 'sto
-0001ac20: 7261 6765 272c 2027 6c73 275d 290a 2020  rage', 'ls']).  
-0001ac30: 2020 2020 2020 6f75 7420 3d20 5b0a 2020        out = [.  
-0001ac40: 2020 2020 2020 2020 2020 6974 656d 2e73            item.s
-0001ac50: 706c 6974 2829 5b30 5d0a 2020 2020 2020  plit()[0].      
-0001ac60: 2020 2020 2020 666f 7220 6974 656d 2069        for item i
-0001ac70: 6e20 6f75 745f 616c 6c2e 6465 636f 6465  n out_all.decode
-0001ac80: 2827 7574 662d 3827 292e 7370 6c69 746c  ('utf-8').splitl
-0001ac90: 696e 6573 2829 0a20 2020 2020 2020 2020  ines().         
-0001aca0: 2020 2069 6620 7374 6f72 655f 7479 7065     if store_type
-0001acb0: 2e76 616c 7565 2069 6e20 6974 656d 0a20  .value in item. 
-0001acc0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-0001acd0: 2061 7373 6572 7420 616c 6c28 5b69 7465   assert all([ite
-0001ace0: 6d20 696e 206f 7574 2066 6f72 2069 7465  m in out for ite
-0001acf0: 6d20 696e 2073 746f 7261 6765 5f6f 626a  m in storage_obj
-0001ad00: 5f6e 616d 655d 290a 0a20 2020 2020 2020  _name])..       
-0001ad10: 2023 2052 756e 2073 6b79 2073 746f 7261   # Run sky stora
-0001ad20: 6765 2064 656c 6574 6520 616c 6c20 746f  ge delete all to
-0001ad30: 2064 656c 6574 6520 616c 6c20 7374 6f72   delete all stor
-0001ad40: 6167 6520 6f62 6a65 6374 730a 2020 2020  age objects.    
-0001ad50: 2020 2020 7375 6270 726f 6365 7373 2e63      subprocess.c
-0001ad60: 6865 636b 5f6f 7574 7075 7428 5b27 736b  heck_output(['sk
-0001ad70: 7927 2c20 2773 746f 7261 6765 272c 2027  y', 'storage', '
-0001ad80: 6465 6c65 7465 272c 2027 2d61 275d 290a  delete', '-a']).
-0001ad90: 0a20 2020 2020 2020 2023 2052 756e 2073  .        # Run s
-0001ada0: 6b79 2073 746f 7261 6765 206c 7320 746f  ky storage ls to
-0001adb0: 2063 6865 636b 2069 6620 616c 6c20 7374   check if all st
-0001adc0: 6f72 6167 6520 6f62 6a65 6374 7320 6669  orage objects fi
-0001add0: 6c74 6572 6564 2062 7920 7374 6f72 650a  ltered by store.
-0001ade0: 2020 2020 2020 2020 2320 7479 7065 2061          # type a
-0001adf0: 7265 2064 656c 6574 6564 0a20 2020 2020  re deleted.     
-0001ae00: 2020 206f 7574 5f61 6c6c 203d 2073 7562     out_all = sub
-0001ae10: 7072 6f63 6573 732e 6368 6563 6b5f 6f75  process.check_ou
-0001ae20: 7470 7574 285b 2773 6b79 272c 2027 7374  tput(['sky', 'st
-0001ae30: 6f72 6167 6527 2c20 276c 7327 5d29 0a20  orage', 'ls']). 
-0001ae40: 2020 2020 2020 206f 7574 203d 205b 0a20         out = [. 
-0001ae50: 2020 2020 2020 2020 2020 2069 7465 6d2e             item.
-0001ae60: 7370 6c69 7428 295b 305d 0a20 2020 2020  split()[0].     
-0001ae70: 2020 2020 2020 2066 6f72 2069 7465 6d20         for item 
-0001ae80: 696e 206f 7574 5f61 6c6c 2e64 6563 6f64  in out_all.decod
-0001ae90: 6528 2775 7466 2d38 2729 2e73 706c 6974  e('utf-8').split
-0001aea0: 6c69 6e65 7328 290a 2020 2020 2020 2020  lines().        
-0001aeb0: 2020 2020 6966 2073 746f 7265 5f74 7970      if store_typ
-0001aec0: 652e 7661 6c75 6520 696e 2069 7465 6d0a  e.value in item.
-0001aed0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-0001aee0: 2020 6173 7365 7274 2061 6c6c 285b 6974    assert all([it
-0001aef0: 656d 206e 6f74 2069 6e20 6f75 7420 666f  em not in out fo
-0001af00: 7220 6974 656d 2069 6e20 7374 6f72 6167  r item in storag
-0001af10: 655f 6f62 6a5f 6e61 6d65 5d29 0a0a 2020  e_obj_name])..  
-0001af20: 2020 4070 7974 6573 742e 6d61 726b 2e70    @pytest.mark.p
-0001af30: 6172 616d 6574 7269 7a65 2827 7374 6f72  arametrize('stor
-0001af40: 655f 7479 7065 272c 205b 0a20 2020 2020  e_type', [.     
-0001af50: 2020 2073 746f 7261 6765 5f6c 6962 2e53     storage_lib.S
-0001af60: 746f 7265 5479 7065 2e53 332c 2073 746f  toreType.S3, sto
-0001af70: 7261 6765 5f6c 6962 2e53 746f 7265 5479  rage_lib.StoreTy
-0001af80: 7065 2e47 4353 2c0a 2020 2020 2020 2020  pe.GCS,.        
-0001af90: 7079 7465 7374 2e70 6172 616d 2873 746f  pytest.param(sto
-0001afa0: 7261 6765 5f6c 6962 2e53 746f 7265 5479  rage_lib.StoreTy
-0001afb0: 7065 2e52 322c 206d 6172 6b73 3d70 7974  pe.R2, marks=pyt
-0001afc0: 6573 742e 6d61 726b 2e63 6c6f 7564 666c  est.mark.cloudfl
-0001afd0: 6172 6529 0a20 2020 205d 290a 2020 2020  are).    ]).    
-0001afe0: 6465 6620 7465 7374 5f62 7563 6b65 745f  def test_bucket_
-0001aff0: 6578 7465 726e 616c 5f64 656c 6574 696f  external_deletio
-0001b000: 6e28 7365 6c66 2c20 746d 705f 7363 7261  n(self, tmp_scra
-0001b010: 7463 685f 7374 6f72 6167 655f 6f62 6a2c  tch_storage_obj,
-0001b020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b040: 2020 2020 2020 2073 746f 7265 5f74 7970         store_typ
-0001b050: 6529 3a0a 2020 2020 2020 2020 2320 4372  e):.        # Cr
-0001b060: 6561 7465 7320 6120 6275 636b 6574 2c20  eates a bucket, 
-0001b070: 6465 6c65 7465 7320 6974 2065 7874 6572  deletes it exter
-0001b080: 6e61 6c6c 7920 7573 696e 6720 636c 6f75  nally using clou
-0001b090: 6420 636c 6920 636f 6d6d 616e 6473 0a20  d cli commands. 
-0001b0a0: 2020 2020 2020 2023 2061 6e64 2074 6865         # and the
-0001b0b0: 6e20 7472 6965 7320 746f 2064 656c 6574  n tries to delet
-0001b0c0: 6520 6974 2075 7369 6e67 2073 6b79 2073  e it using sky s
-0001b0d0: 746f 7261 6765 2064 656c 6574 652e 0a20  torage delete.. 
-0001b0e0: 2020 2020 2020 2074 6d70 5f73 6372 6174         tmp_scrat
-0001b0f0: 6368 5f73 746f 7261 6765 5f6f 626a 2e61  ch_storage_obj.a
-0001b100: 6464 5f73 746f 7265 2873 746f 7265 5f74  dd_store(store_t
-0001b110: 7970 6529 0a0a 2020 2020 2020 2020 2320  ype)..        # 
-0001b120: 5275 6e20 736b 7920 7374 6f72 6167 6520  Run sky storage 
-0001b130: 6c73 2074 6f20 6368 6563 6b20 6966 2073  ls to check if s
-0001b140: 746f 7261 6765 206f 626a 6563 7420 6578  torage object ex
-0001b150: 6973 7473 2069 6e20 7468 6520 6f75 7470  ists in the outp
-0001b160: 7574 0a20 2020 2020 2020 206f 7574 203d  ut.        out =
-0001b170: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
-0001b180: 6b5f 6f75 7470 7574 285b 2773 6b79 272c  k_output(['sky',
-0001b190: 2027 7374 6f72 6167 6527 2c20 276c 7327   'storage', 'ls'
-0001b1a0: 5d29 0a20 2020 2020 2020 2061 7373 6572  ]).        asser
-0001b1b0: 7420 746d 705f 7363 7261 7463 685f 7374  t tmp_scratch_st
-0001b1c0: 6f72 6167 655f 6f62 6a2e 6e61 6d65 2069  orage_obj.name i
-0001b1d0: 6e20 6f75 742e 6465 636f 6465 2827 7574  n out.decode('ut
-0001b1e0: 662d 3827 290a 0a20 2020 2020 2020 2023  f-8')..        #
-0001b1f0: 2044 656c 6574 6520 6275 636b 6574 2065   Delete bucket e
-0001b200: 7874 6572 6e61 6c6c 790a 2020 2020 2020  xternally.      
-0001b210: 2020 636d 6420 3d20 7365 6c66 2e63 6c69    cmd = self.cli
-0001b220: 5f64 656c 6574 655f 636d 6428 7374 6f72  _delete_cmd(stor
-0001b230: 655f 7479 7065 2c20 746d 705f 7363 7261  e_type, tmp_scra
-0001b240: 7463 685f 7374 6f72 6167 655f 6f62 6a2e  tch_storage_obj.
-0001b250: 6e61 6d65 290a 2020 2020 2020 2020 7375  name).        su
-0001b260: 6270 726f 6365 7373 2e63 6865 636b 5f6f  bprocess.check_o
-0001b270: 7574 7075 7428 636d 642c 2073 6865 6c6c  utput(cmd, shell
-0001b280: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
-0001b290: 2320 5275 6e20 736b 7920 7374 6f72 6167  # Run sky storag
-0001b2a0: 6520 6465 6c65 7465 2074 6f20 6465 6c65  e delete to dele
-0001b2b0: 7465 2074 6865 2073 746f 7261 6765 206f  te the storage o
-0001b2c0: 626a 6563 740a 2020 2020 2020 2020 6f75  bject.        ou
-0001b2d0: 7420 3d20 7375 6270 726f 6365 7373 2e63  t = subprocess.c
-0001b2e0: 6865 636b 5f6f 7574 7075 7428 0a20 2020  heck_output(.   
-0001b2f0: 2020 2020 2020 2020 205b 2773 6b79 272c           ['sky',
-0001b300: 2027 7374 6f72 6167 6527 2c20 2764 656c   'storage', 'del
-0001b310: 6574 6527 2c20 746d 705f 7363 7261 7463  ete', tmp_scratc
-0001b320: 685f 7374 6f72 6167 655f 6f62 6a2e 6e61  h_storage_obj.na
-0001b330: 6d65 5d29 0a20 2020 2020 2020 2023 204d  me]).        # M
-0001b340: 616b 6520 7375 7265 2062 7563 6b65 7420  ake sure bucket 
-0001b350: 7761 7320 6e6f 7420 6372 6561 7465 6420  was not created 
-0001b360: 6475 7269 6e67 2064 656c 6574 696f 6e20  during deletion 
-0001b370: 2873 6565 2069 7373 7565 2023 3133 3232  (see issue #1322
-0001b380: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
-0001b390: 2027 6372 6561 7465 6427 206e 6f74 2069   'created' not i
-0001b3a0: 6e20 6f75 742e 6465 636f 6465 2827 7574  n out.decode('ut
-0001b3b0: 662d 3827 292e 6c6f 7765 7228 290a 0a20  f-8').lower().. 
-0001b3c0: 2020 2020 2020 2023 2052 756e 2073 6b79         # Run sky
-0001b3d0: 2073 746f 7261 6765 206c 7320 746f 2063   storage ls to c
-0001b3e0: 6865 636b 2069 6620 7374 6f72 6167 6520  heck if storage 
-0001b3f0: 6f62 6a65 6374 2069 7320 6465 6c65 7465  object is delete
-0001b400: 640a 2020 2020 2020 2020 6f75 7420 3d20  d.        out = 
-0001b410: 7375 6270 726f 6365 7373 2e63 6865 636b  subprocess.check
-0001b420: 5f6f 7574 7075 7428 5b27 736b 7927 2c20  _output(['sky', 
-0001b430: 2773 746f 7261 6765 272c 2027 6c73 275d  'storage', 'ls']
-0001b440: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
-0001b450: 2074 6d70 5f73 6372 6174 6368 5f73 746f   tmp_scratch_sto
-0001b460: 7261 6765 5f6f 626a 2e6e 616d 6520 6e6f  rage_obj.name no
-0001b470: 7420 696e 206f 7574 2e64 6563 6f64 6528  t in out.decode(
-0001b480: 2775 7466 2d38 2729 0a0a 2020 2020 4070  'utf-8')..    @p
-0001b490: 7974 6573 742e 6d61 726b 2e70 6172 616d  ytest.mark.param
-0001b4a0: 6574 7269 7a65 2827 7374 6f72 655f 7479  etrize('store_ty
-0001b4b0: 7065 272c 205b 0a20 2020 2020 2020 2073  pe', [.        s
-0001b4c0: 746f 7261 6765 5f6c 6962 2e53 746f 7265  torage_lib.Store
-0001b4d0: 5479 7065 2e53 332c 2073 746f 7261 6765  Type.S3, storage
-0001b4e0: 5f6c 6962 2e53 746f 7265 5479 7065 2e47  _lib.StoreType.G
-0001b4f0: 4353 2c0a 2020 2020 2020 2020 7079 7465  CS,.        pyte
-0001b500: 7374 2e70 6172 616d 2873 746f 7261 6765  st.param(storage
-0001b510: 5f6c 6962 2e53 746f 7265 5479 7065 2e52  _lib.StoreType.R
-0001b520: 322c 206d 6172 6b73 3d70 7974 6573 742e  2, marks=pytest.
-0001b530: 6d61 726b 2e63 6c6f 7564 666c 6172 6529  mark.cloudflare)
-0001b540: 0a20 2020 205d 290a 2020 2020 6465 6620  .    ]).    def 
-0001b550: 7465 7374 5f62 7563 6b65 745f 6275 6c6b  test_bucket_bulk
-0001b560: 5f64 656c 6574 696f 6e28 7365 6c66 2c20  _deletion(self, 
-0001b570: 7374 6f72 655f 7479 7065 2c20 746d 705f  store_type, tmp_
-0001b580: 6275 6c6b 5f64 656c 5f73 746f 7261 6765  bulk_del_storage
-0001b590: 5f6f 626a 293a 0a20 2020 2020 2020 2023  _obj):.        #
-0001b5a0: 2043 7265 6174 6573 2061 2074 656d 7020   Creates a temp 
-0001b5b0: 666f 6c64 6572 2077 6974 6820 6f76 6572  folder with over
-0001b5c0: 2032 3536 2066 696c 6573 2061 6e64 2066   256 files and f
-0001b5d0: 6f6c 6465 7273 2c20 7570 6c6f 6164 0a20  olders, upload. 
-0001b5e0: 2020 2020 2020 2023 2066 696c 6573 2061         # files a
-0001b5f0: 6e64 2066 6f6c 6465 7273 2074 6f20 6120  nd folders to a 
-0001b600: 6e65 7720 6275 636b 6574 2c20 7468 656e  new bucket, then
-0001b610: 2064 656c 6574 6520 6275 636b 6574 2e0a   delete bucket..
-0001b620: 2020 2020 2020 2020 746d 705f 6275 6c6b          tmp_bulk
-0001b630: 5f64 656c 5f73 746f 7261 6765 5f6f 626a  _del_storage_obj
-0001b640: 2e61 6464 5f73 746f 7265 2873 746f 7265  .add_store(store
-0001b650: 5f74 7970 6529 0a0a 2020 2020 2020 2020  _type)..        
-0001b660: 7375 6270 726f 6365 7373 2e63 6865 636b  subprocess.check
-0001b670: 5f6f 7574 7075 7428 0a20 2020 2020 2020  _output(.       
-0001b680: 2020 2020 205b 2773 6b79 272c 2027 7374       ['sky', 'st
-0001b690: 6f72 6167 6527 2c20 2764 656c 6574 6527  orage', 'delete'
-0001b6a0: 2c20 746d 705f 6275 6c6b 5f64 656c 5f73  , tmp_bulk_del_s
-0001b6b0: 746f 7261 6765 5f6f 626a 2e6e 616d 655d  torage_obj.name]
-0001b6c0: 290a 0a20 2020 2020 2020 206f 7574 7075  )..        outpu
-0001b6d0: 7420 3d20 7375 6270 726f 6365 7373 2e63  t = subprocess.c
-0001b6e0: 6865 636b 5f6f 7574 7075 7428 5b27 736b  heck_output(['sk
-0001b6f0: 7927 2c20 2773 746f 7261 6765 272c 2027  y', 'storage', '
-0001b700: 6c73 275d 290a 2020 2020 2020 2020 6173  ls']).        as
-0001b710: 7365 7274 2074 6d70 5f62 756c 6b5f 6465  sert tmp_bulk_de
-0001b720: 6c5f 7374 6f72 6167 655f 6f62 6a2e 6e61  l_storage_obj.na
-0001b730: 6d65 206e 6f74 2069 6e20 6f75 7470 7574  me not in output
-0001b740: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
-0001b750: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
-0001b760: 726b 2e70 6172 616d 6574 7269 7a65 280a  rk.parametrize(.
-0001b770: 2020 2020 2020 2020 2774 6d70 5f70 7562          'tmp_pub
-0001b780: 6c69 635f 7374 6f72 6167 655f 6f62 6a2c  lic_storage_obj,
-0001b790: 2073 746f 7265 5f74 7970 6527 2c0a 2020   store_type',.  
-0001b7a0: 2020 2020 2020 5b28 2773 333a 2f2f 7463        [('s3://tc
-0001b7b0: 6761 2d32 2d6f 7065 6e27 2c20 7374 6f72  ga-2-open', stor
-0001b7c0: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
-0001b7d0: 652e 5333 292c 0a20 2020 2020 2020 2020  e.S3),.         
-0001b7e0: 2827 7333 3a2f 2f64 6967 6974 616c 636f  ('s3://digitalco
-0001b7f0: 7270 6f72 6127 2c20 7374 6f72 6167 655f  rpora', storage_
-0001b800: 6c69 622e 5374 6f72 6554 7970 652e 5333  lib.StoreType.S3
-0001b810: 292c 0a20 2020 2020 2020 2020 2827 6773  ),.         ('gs
-0001b820: 3a2f 2f67 6370 2d70 7562 6c69 632d 6461  ://gcp-public-da
-0001b830: 7461 2d73 656e 7469 6e65 6c2d 3227 2c20  ta-sentinel-2', 
-0001b840: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
-0001b850: 6554 7970 652e 4743 5329 5d2c 0a20 2020  eType.GCS)],.   
-0001b860: 2020 2020 2069 6e64 6972 6563 743d 5b27       indirect=['
-0001b870: 746d 705f 7075 626c 6963 5f73 746f 7261  tmp_public_stora
-0001b880: 6765 5f6f 626a 275d 290a 2020 2020 6465  ge_obj']).    de
-0001b890: 6620 7465 7374 5f70 7562 6c69 635f 6275  f test_public_bu
-0001b8a0: 636b 6574 2873 656c 662c 2074 6d70 5f70  cket(self, tmp_p
-0001b8b0: 7562 6c69 635f 7374 6f72 6167 655f 6f62  ublic_storage_ob
-0001b8c0: 6a2c 2073 746f 7265 5f74 7970 6529 3a0a  j, store_type):.
-0001b8d0: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
-0001b8e0: 7320 6120 6e65 7720 6275 636b 6574 2077  s a new bucket w
-0001b8f0: 6974 6820 6120 7075 626c 6963 2073 6f75  ith a public sou
-0001b900: 7263 6520 616e 6420 7665 7269 6669 6573  rce and verifies
-0001b910: 2074 6861 7420 6974 2069 7320 6e6f 740a   that it is not.
-0001b920: 2020 2020 2020 2020 2320 6164 6465 6420          # added 
-0001b930: 746f 2067 6c6f 6261 6c5f 7573 6572 5f73  to global_user_s
-0001b940: 7461 7465 2e0a 2020 2020 2020 2020 746d  tate..        tm
-0001b950: 705f 7075 626c 6963 5f73 746f 7261 6765  p_public_storage
-0001b960: 5f6f 626a 2e61 6464 5f73 746f 7265 2873  _obj.add_store(s
-0001b970: 746f 7265 5f74 7970 6529 0a0a 2020 2020  tore_type)..    
-0001b980: 2020 2020 2320 5275 6e20 736b 7920 7374      # Run sky st
-0001b990: 6f72 6167 6520 6c73 2074 6f20 6368 6563  orage ls to chec
-0001b9a0: 6b20 6966 2073 746f 7261 6765 206f 626a  k if storage obj
-0001b9b0: 6563 7420 6578 6973 7473 2069 6e20 7468  ect exists in th
-0001b9c0: 6520 6f75 7470 7574 0a20 2020 2020 2020  e output.       
-0001b9d0: 206f 7574 203d 2073 7562 7072 6f63 6573   out = subproces
-0001b9e0: 732e 6368 6563 6b5f 6f75 7470 7574 285b  s.check_output([
-0001b9f0: 2773 6b79 272c 2027 7374 6f72 6167 6527  'sky', 'storage'
-0001ba00: 2c20 276c 7327 5d29 0a20 2020 2020 2020  , 'ls']).       
-0001ba10: 2061 7373 6572 7420 746d 705f 7075 626c   assert tmp_publ
-0001ba20: 6963 5f73 746f 7261 6765 5f6f 626a 2e6e  ic_storage_obj.n
-0001ba30: 616d 6520 6e6f 7420 696e 206f 7574 2e64  ame not in out.d
-0001ba40: 6563 6f64 6528 2775 7466 2d38 2729 0a0a  ecode('utf-8')..
-0001ba50: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-0001ba60: 2e70 6172 616d 6574 7269 7a65 2827 6e6f  .parametrize('no
-0001ba70: 6e65 7869 7374 5f62 7563 6b65 745f 7572  nexist_bucket_ur
-0001ba80: 6c27 2c20 5b0a 2020 2020 2020 2020 2773  l', [.        's
-0001ba90: 333a 2f2f 7b72 616e 646f 6d5f 6e61 6d65  3://{random_name
-0001baa0: 7d27 2c20 2767 733a 2f2f 7b72 616e 646f  }', 'gs://{rando
-0001bab0: 6d5f 6e61 6d65 7d27 2c0a 2020 2020 2020  m_name}',.      
-0001bac0: 2020 7079 7465 7374 2e70 6172 616d 2827    pytest.param('
-0001bad0: 7232 3a2f 2f7b 7261 6e64 6f6d 5f6e 616d  r2://{random_nam
-0001bae0: 657d 272c 206d 6172 6b73 3d70 7974 6573  e}', marks=pytes
-0001baf0: 742e 6d61 726b 2e63 6c6f 7564 666c 6172  t.mark.cloudflar
-0001bb00: 6529 0a20 2020 205d 290a 2020 2020 6465  e).    ]).    de
-0001bb10: 6620 7465 7374 5f6e 6f6e 6578 6973 7465  f test_nonexiste
-0001bb20: 6e74 5f62 7563 6b65 7428 7365 6c66 2c20  nt_bucket(self, 
-0001bb30: 6e6f 6e65 7869 7374 5f62 7563 6b65 745f  nonexist_bucket_
-0001bb40: 7572 6c29 3a0a 2020 2020 2020 2020 2320  url):.        # 
-0001bb50: 4174 7465 6d70 7473 2074 6f20 6372 6561  Attempts to crea
-0001bb60: 7465 2066 6574 6368 2061 2073 7472 6f61  te fetch a stroa
-0001bb70: 6765 2077 6974 6820 6120 6e6f 6e2d 6578  ge with a non-ex
-0001bb80: 6973 7465 6e74 2073 6f75 7263 652e 0a20  istent source.. 
-0001bb90: 2020 2020 2020 2023 2047 656e 6572 6174         # Generat
-0001bba0: 6520 6120 7261 6e64 6f6d 2062 7563 6b65  e a random bucke
-0001bbb0: 7420 6e61 6d65 2061 6e64 2076 6572 6966  t name and verif
-0001bbc0: 7920 6974 2064 6f65 736e 2774 2065 7869  y it doesn't exi
-0001bbd0: 7374 3a0a 2020 2020 2020 2020 7265 7472  st:.        retr
-0001bbe0: 795f 636f 756e 7420 3d20 300a 2020 2020  y_count = 0.    
-0001bbf0: 2020 2020 7768 696c 6520 5472 7565 3a0a      while True:.
-0001bc00: 2020 2020 2020 2020 2020 2020 6e6f 6e65              none
-0001bc10: 7869 7374 5f62 7563 6b65 745f 6e61 6d65  xist_bucket_name
-0001bc20: 203d 2073 7472 2875 7569 642e 7575 6964   = str(uuid.uuid
-0001bc30: 3428 2929 0a20 2020 2020 2020 2020 2020  4()).           
-0001bc40: 2069 6620 6e6f 6e65 7869 7374 5f62 7563   if nonexist_buc
-0001bc50: 6b65 745f 7572 6c2e 7374 6172 7473 7769  ket_url.startswi
-0001bc60: 7468 2827 7333 2729 3a0a 2020 2020 2020  th('s3'):.      
-0001bc70: 2020 2020 2020 2020 2020 636f 6d6d 616e            comman
-0001bc80: 6420 3d20 6627 6177 7320 7333 6170 6920  d = f'aws s3api 
-0001bc90: 6865 6164 2d62 7563 6b65 7420 2d2d 6275  head-bucket --bu
-0001bca0: 636b 6574 207b 6e6f 6e65 7869 7374 5f62  cket {nonexist_b
-0001bcb0: 7563 6b65 745f 6e61 6d65 7d27 0a20 2020  ucket_name}'.   
-0001bcc0: 2020 2020 2020 2020 2020 2020 2065 7870               exp
-0001bcd0: 6563 7465 645f 6f75 7470 7574 203d 2027  ected_output = '
-0001bce0: 3430 3427 0a20 2020 2020 2020 2020 2020  404'.           
-0001bcf0: 2065 6c69 6620 6e6f 6e65 7869 7374 5f62   elif nonexist_b
-0001bd00: 7563 6b65 745f 7572 6c2e 7374 6172 7473  ucket_url.starts
-0001bd10: 7769 7468 2827 6773 2729 3a0a 2020 2020  with('gs'):.    
-0001bd20: 2020 2020 2020 2020 2020 2020 636f 6d6d              comm
-0001bd30: 616e 6420 3d20 6627 6773 7574 696c 206c  and = f'gsutil l
-0001bd40: 7320 7b6e 6f6e 6578 6973 745f 6275 636b  s {nonexist_buck
-0001bd50: 6574 5f75 726c 2e66 6f72 6d61 7428 7261  et_url.format(ra
-0001bd60: 6e64 6f6d 5f6e 616d 653d 6e6f 6e65 7869  ndom_name=nonexi
-0001bd70: 7374 5f62 7563 6b65 745f 6e61 6d65 297d  st_bucket_name)}
-0001bd80: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-0001bd90: 2020 6578 7065 6374 6564 5f6f 7574 7075    expected_outpu
-0001bda0: 7420 3d20 2742 7563 6b65 744e 6f74 466f  t = 'BucketNotFo
-0001bdb0: 756e 6445 7863 6570 7469 6f6e 270a 2020  undException'.  
-0001bdc0: 2020 2020 2020 2020 2020 656c 6966 206e            elif n
-0001bdd0: 6f6e 6578 6973 745f 6275 636b 6574 5f75  onexist_bucket_u
-0001bde0: 726c 2e73 7461 7274 7377 6974 6828 2772  rl.startswith('r
-0001bdf0: 3227 293a 0a20 2020 2020 2020 2020 2020  2'):.           
-0001be00: 2020 2020 2065 6e64 706f 696e 745f 7572       endpoint_ur
-0001be10: 6c20 3d20 636c 6f75 6466 6c61 7265 2e63  l = cloudflare.c
-0001be20: 7265 6174 655f 656e 6470 6f69 6e74 2829  reate_endpoint()
-0001be30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001be40: 2063 6f6d 6d61 6e64 203d 2066 2741 5753   command = f'AWS
-0001be50: 5f53 4841 5245 445f 4352 4544 454e 5449  _SHARED_CREDENTI
-0001be60: 414c 535f 4649 4c45 3d7b 636c 6f75 6466  ALS_FILE={cloudf
-0001be70: 6c61 7265 2e52 325f 4352 4544 454e 5449  lare.R2_CREDENTI
-0001be80: 414c 535f 5041 5448 7d20 6177 7320 7333  ALS_PATH} aws s3
-0001be90: 6170 6920 6865 6164 2d62 7563 6b65 7420  api head-bucket 
-0001bea0: 2d2d 6275 636b 6574 207b 6e6f 6e65 7869  --bucket {nonexi
-0001beb0: 7374 5f62 7563 6b65 745f 6e61 6d65 7d20  st_bucket_name} 
-0001bec0: 2d2d 656e 6470 6f69 6e74 207b 656e 6470  --endpoint {endp
-0001bed0: 6f69 6e74 5f75 726c 7d20 2d2d 7072 6f66  oint_url} --prof
-0001bee0: 696c 653d 7232 270a 2020 2020 2020 2020  ile=r2'.        
-0001bef0: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-0001bf00: 5f6f 7574 7075 7420 3d20 2734 3034 270a  _output = '404'.
-0001bf10: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0001bf20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001bf30: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0001bf40: 6f72 2827 556e 7375 7070 6f72 7465 6420  or('Unsupported 
-0001bf50: 6275 636b 6574 2074 7970 6520 270a 2020  bucket type '.  
-0001bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0001bf80: 277b 6e6f 6e65 7869 7374 5f62 7563 6b65  '{nonexist_bucke
-0001bf90: 745f 7572 6c7d 2729 0a0a 2020 2020 2020  t_url}')..      
-0001bfa0: 2020 2020 2020 2320 4368 6563 6b20 6966        # Check if
-0001bfb0: 2062 7563 6b65 7420 6578 6973 7473 2075   bucket exists u
-0001bfc0: 7369 6e67 2074 6865 2063 6c69 3a0a 2020  sing the cli:.  
-0001bfd0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-0001bfe0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0001bff0: 7574 203d 2073 7562 7072 6f63 6573 732e  ut = subprocess.
-0001c000: 6368 6563 6b5f 6f75 7470 7574 2863 6f6d  check_output(com
-0001c010: 6d61 6e64 2c0a 2020 2020 2020 2020 2020  mand,.          
-0001c020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c040: 2020 2020 7374 6465 7272 3d73 7562 7072      stderr=subpr
-0001c050: 6f63 6573 732e 5354 444f 5554 2c0a 2020  ocess.STDOUT,.  
-0001c060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c080: 2020 2020 2020 2020 2020 2020 7368 656c              shel
-0001c090: 6c3d 5472 7565 290a 2020 2020 2020 2020  l=True).        
-0001c0a0: 2020 2020 6578 6365 7074 2073 7562 7072      except subpr
-0001c0b0: 6f63 6573 732e 4361 6c6c 6564 5072 6f63  ocess.CalledProc
-0001c0c0: 6573 7345 7272 6f72 2061 7320 653a 0a20  essError as e:. 
-0001c0d0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0001c0e0: 7574 203d 2065 2e6f 7574 7075 740a 2020  ut = e.output.  
-0001c0f0: 2020 2020 2020 2020 2020 6f75 7420 3d20            out = 
-0001c100: 6f75 742e 6465 636f 6465 2827 7574 662d  out.decode('utf-
-0001c110: 3827 290a 2020 2020 2020 2020 2020 2020  8').            
-0001c120: 6966 2065 7870 6563 7465 645f 6f75 7470  if expected_outp
-0001c130: 7574 2069 6e20 6f75 743a 0a20 2020 2020  ut in out:.     
-0001c140: 2020 2020 2020 2020 2020 2062 7265 616b             break
-0001c150: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0001c160: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001c170: 2020 2072 6574 7279 5f63 6f75 6e74 202b     retry_count +
-0001c180: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-0001c190: 2020 2020 6966 2072 6574 7279 5f63 6f75      if retry_cou
-0001c1a0: 6e74 203e 2033 3a0a 2020 2020 2020 2020  nt > 3:.        
-0001c1b0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0001c1c0: 6520 5275 6e74 696d 6545 7272 6f72 2827  e RuntimeError('
-0001c1d0: 556e 6162 6c65 2074 6f20 6669 6e64 2061  Unable to find a
-0001c1e0: 206e 6f6e 6578 6973 7465 6e74 2062 7563   nonexistent buc
-0001c1f0: 6b65 7420 270a 2020 2020 2020 2020 2020  ket '.          
+00019ac0: 2020 2020 2020 2020 2020 2020 736f 7572              sour
+00019ad0: 6365 3d6c 6973 745f 736f 7572 6365 290a  ce=list_source).
+00019ae0: 0a20 2020 2040 7079 7465 7374 2e66 6978  .    @pytest.fix
+00019af0: 7475 7265 0a20 2020 2064 6566 2074 6d70  ture.    def tmp
+00019b00: 5f62 756c 6b5f 6465 6c5f 7374 6f72 6167  _bulk_del_storag
+00019b10: 655f 6f62 6a28 7365 6c66 2c20 746d 705f  e_obj(self, tmp_
+00019b20: 6275 636b 6574 5f6e 616d 6529 3a0a 2020  bucket_name):.  
+00019b30: 2020 2020 2020 2320 4372 6561 7465 7320        # Creates 
+00019b40: 6120 7465 6d70 6f72 6172 7920 7374 6f72  a temporary stor
+00019b50: 6167 6520 6f62 6a65 6374 2066 6f72 2074  age object for t
+00019b60: 6573 7469 6e67 2062 756c 6b20 6465 6c65  esting bulk dele
+00019b70: 7469 6f6e 2e0a 2020 2020 2020 2020 2320  tion..        # 
+00019b80: 5374 6f72 6573 206d 7573 7420 6265 2061  Stores must be a
+00019b90: 6464 6564 2069 6e20 7468 6520 7465 7374  dded in the test
+00019ba0: 2e0a 2020 2020 2020 2020 7769 7468 2074  ..        with t
+00019bb0: 656d 7066 696c 652e 5465 6d70 6f72 6172  empfile.Temporar
+00019bc0: 7944 6972 6563 746f 7279 2829 2061 7320  yDirectory() as 
+00019bd0: 746d 7064 6972 3a0a 2020 2020 2020 2020  tmpdir:.        
+00019be0: 2020 2020 7375 6270 726f 6365 7373 2e63      subprocess.c
+00019bf0: 6865 636b 5f6f 7574 7075 7428 6627 6d6b  heck_output(f'mk
+00019c00: 6469 7220 2d70 207b 746d 7064 6972 7d2f  dir -p {tmpdir}/
+00019c10: 666f 6c64 6572 7b7b 3030 302e 2e32 3535  folder{{000..255
+00019c20: 7d7d 272c 0a20 2020 2020 2020 2020 2020  }}',.           
+00019c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c40: 2020 2020 2020 2020 2073 6865 6c6c 3d54           shell=T
+00019c50: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+00019c60: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
+00019c70: 6b5f 6f75 7470 7574 2866 2774 6f75 6368  k_output(f'touch
+00019c80: 207b 746d 7064 6972 7d2f 7465 7374 7b7b   {tmpdir}/test{{
+00019c90: 3030 302e 2e32 3535 7d7d 2e74 7874 272c  000..255}}.txt',
+00019ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019cc0: 2020 2020 2073 6865 6c6c 3d54 7275 6529       shell=True)
+00019cd0: 0a20 2020 2020 2020 2020 2020 2073 7562  .            sub
+00019ce0: 7072 6f63 6573 732e 6368 6563 6b5f 6f75  process.check_ou
+00019cf0: 7470 7574 280a 2020 2020 2020 2020 2020  tput(.          
+00019d00: 2020 2020 2020 6627 746f 7563 6820 7b74        f'touch {t
+00019d10: 6d70 6469 727d 2f66 6f6c 6465 727b 7b30  mpdir}/folder{{0
+00019d20: 3030 2e2e 3235 357d 7d2f 7465 7374 2e74  00..255}}/test.t
+00019d30: 7874 272c 2073 6865 6c6c 3d54 7275 6529  xt', shell=True)
+00019d40: 0a20 2020 2020 2020 2020 2020 2079 6965  .            yie
+00019d50: 6c64 2066 726f 6d20 7365 6c66 2e79 6965  ld from self.yie
+00019d60: 6c64 5f73 746f 7261 6765 5f6f 626a 6563  ld_storage_objec
+00019d70: 7428 6e61 6d65 3d74 6d70 5f62 7563 6b65  t(name=tmp_bucke
+00019d80: 745f 6e61 6d65 2c0a 2020 2020 2020 2020  t_name,.        
+00019d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019db0: 2020 2020 2020 2020 2073 6f75 7263 653d           source=
+00019dc0: 746d 7064 6972 290a 0a20 2020 2040 7079  tmpdir)..    @py
+00019dd0: 7465 7374 2e66 6978 7475 7265 0a20 2020  test.fixture.   
+00019de0: 2064 6566 2074 6d70 5f63 6f70 795f 6d6e   def tmp_copy_mn
+00019df0: 745f 6578 6973 7469 6e67 5f73 746f 7261  t_existing_stora
+00019e00: 6765 5f6f 626a 2873 656c 662c 2074 6d70  ge_obj(self, tmp
+00019e10: 5f73 6372 6174 6368 5f73 746f 7261 6765  _scratch_storage
+00019e20: 5f6f 626a 293a 0a20 2020 2020 2020 2023  _obj):.        #
+00019e30: 2043 7265 6174 6573 2061 2063 6f70 7920   Creates a copy 
+00019e40: 6d6f 756e 7420 7374 6f72 6167 6520 7768  mount storage wh
+00019e50: 6963 6820 7265 7573 6573 2061 6e20 6578  ich reuses an ex
+00019e60: 6973 7469 6e67 2073 746f 7261 6765 206f  isting storage o
+00019e70: 626a 6563 742e 0a20 2020 2020 2020 2074  bject..        t
+00019e80: 6d70 5f73 6372 6174 6368 5f73 746f 7261  mp_scratch_stora
+00019e90: 6765 5f6f 626a 2e61 6464 5f73 746f 7265  ge_obj.add_store
+00019ea0: 2873 746f 7261 6765 5f6c 6962 2e53 746f  (storage_lib.Sto
+00019eb0: 7265 5479 7065 2e53 3329 0a20 2020 2020  reType.S3).     
+00019ec0: 2020 2073 746f 7261 6765 5f6e 616d 6520     storage_name 
+00019ed0: 3d20 746d 705f 7363 7261 7463 685f 7374  = tmp_scratch_st
+00019ee0: 6f72 6167 655f 6f62 6a2e 6e61 6d65 0a0a  orage_obj.name..
+00019ef0: 2020 2020 2020 2020 2320 5472 7920 746f          # Try to
+00019f00: 2069 6e69 7469 616c 697a 6520 616e 6f74   initialize anot
+00019f10: 6865 7220 7374 6f72 6167 6520 7769 7468  her storage with
+00019f20: 2074 6865 2073 746f 7261 6765 206f 626a   the storage obj
+00019f30: 6563 7420 6372 6561 7465 640a 2020 2020  ect created.    
+00019f40: 2020 2020 2320 6162 6f76 652c 2062 7574      # above, but
+00019f50: 206e 6f77 2069 6e20 434f 5059 206d 6f64   now in COPY mod
+00019f60: 652e 2054 6869 7320 7368 6f75 6c64 2073  e. This should s
+00019f70: 7563 6365 6564 2e0a 2020 2020 2020 2020  ucceed..        
+00019f80: 7969 656c 6420 6672 6f6d 2073 656c 662e  yield from self.
+00019f90: 7969 656c 645f 7374 6f72 6167 655f 6f62  yield_storage_ob
+00019fa0: 6a65 6374 286e 616d 653d 7374 6f72 6167  ject(name=storag
+00019fb0: 655f 6e61 6d65 2c0a 2020 2020 2020 2020  e_name,.        
+00019fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019fe0: 2020 2020 206d 6f64 653d 7374 6f72 6167       mode=storag
+00019ff0: 655f 6c69 622e 5374 6f72 6167 654d 6f64  e_lib.StorageMod
+0001a000: 652e 434f 5059 290a 0a20 2020 2040 7079  e.COPY)..    @py
+0001a010: 7465 7374 2e66 6978 7475 7265 0a20 2020  test.fixture.   
+0001a020: 2064 6566 2074 6d70 5f61 7773 636c 695f   def tmp_awscli_
+0001a030: 6275 636b 6574 2873 656c 662c 2074 6d70  bucket(self, tmp
+0001a040: 5f62 7563 6b65 745f 6e61 6d65 293a 0a20  _bucket_name):. 
+0001a050: 2020 2020 2020 2023 2043 7265 6174 6573         # Creates
+0001a060: 2061 2074 656d 706f 7261 7279 2062 7563   a temporary buc
+0001a070: 6b65 7420 7573 696e 6720 6177 7363 6c69  ket using awscli
+0001a080: 0a20 2020 2020 2020 2073 7562 7072 6f63  .        subproc
+0001a090: 6573 732e 6368 6563 6b5f 6361 6c6c 285b  ess.check_call([
+0001a0a0: 2761 7773 272c 2027 7333 272c 2027 6d62  'aws', 's3', 'mb
+0001a0b0: 272c 2066 2773 333a 2f2f 7b74 6d70 5f62  ', f's3://{tmp_b
+0001a0c0: 7563 6b65 745f 6e61 6d65 7d27 5d29 0a20  ucket_name}']). 
+0001a0d0: 2020 2020 2020 2079 6965 6c64 2074 6d70         yield tmp
+0001a0e0: 5f62 7563 6b65 745f 6e61 6d65 0a20 2020  _bucket_name.   
+0001a0f0: 2020 2020 2073 7562 7072 6f63 6573 732e       subprocess.
+0001a100: 6368 6563 6b5f 6361 6c6c 280a 2020 2020  check_call(.    
+0001a110: 2020 2020 2020 2020 5b27 6177 7327 2c20          ['aws', 
+0001a120: 2773 3327 2c20 2772 6227 2c20 6627 7333  's3', 'rb', f's3
+0001a130: 3a2f 2f7b 746d 705f 6275 636b 6574 5f6e  ://{tmp_bucket_n
+0001a140: 616d 657d 272c 2027 2d2d 666f 7263 6527  ame}', '--force'
+0001a150: 5d29 0a0a 2020 2020 4070 7974 6573 742e  ])..    @pytest.
+0001a160: 6669 7874 7572 650a 2020 2020 6465 6620  fixture.    def 
+0001a170: 746d 705f 6773 7574 696c 5f62 7563 6b65  tmp_gsutil_bucke
+0001a180: 7428 7365 6c66 2c20 746d 705f 6275 636b  t(self, tmp_buck
+0001a190: 6574 5f6e 616d 6529 3a0a 2020 2020 2020  et_name):.      
+0001a1a0: 2020 2320 4372 6561 7465 7320 6120 7465    # Creates a te
+0001a1b0: 6d70 6f72 6172 7920 6275 636b 6574 2075  mporary bucket u
+0001a1c0: 7369 6e67 2067 7375 7469 6c0a 2020 2020  sing gsutil.    
+0001a1d0: 2020 2020 7375 6270 726f 6365 7373 2e63      subprocess.c
+0001a1e0: 6865 636b 5f63 616c 6c28 5b27 6773 7574  heck_call(['gsut
+0001a1f0: 696c 272c 2027 6d62 272c 2066 2767 733a  il', 'mb', f'gs:
+0001a200: 2f2f 7b74 6d70 5f62 7563 6b65 745f 6e61  //{tmp_bucket_na
+0001a210: 6d65 7d27 5d29 0a20 2020 2020 2020 2079  me}']).        y
+0001a220: 6965 6c64 2074 6d70 5f62 7563 6b65 745f  ield tmp_bucket_
+0001a230: 6e61 6d65 0a20 2020 2020 2020 2073 7562  name.        sub
+0001a240: 7072 6f63 6573 732e 6368 6563 6b5f 6361  process.check_ca
+0001a250: 6c6c 285b 2767 7375 7469 6c27 2c20 2772  ll(['gsutil', 'r
+0001a260: 6d27 2c20 272d 7227 2c20 6627 6773 3a2f  m', '-r', f'gs:/
+0001a270: 2f7b 746d 705f 6275 636b 6574 5f6e 616d  /{tmp_bucket_nam
+0001a280: 657d 275d 290a 0a20 2020 2040 7079 7465  e}'])..    @pyte
+0001a290: 7374 2e66 6978 7475 7265 0a20 2020 2064  st.fixture.    d
+0001a2a0: 6566 2074 6d70 5f61 7773 636c 695f 6275  ef tmp_awscli_bu
+0001a2b0: 636b 6574 5f72 3228 7365 6c66 2c20 746d  cket_r2(self, tm
+0001a2c0: 705f 6275 636b 6574 5f6e 616d 6529 3a0a  p_bucket_name):.
+0001a2d0: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+0001a2e0: 7320 6120 7465 6d70 6f72 6172 7920 6275  s a temporary bu
+0001a2f0: 636b 6574 2075 7369 6e67 2061 7773 636c  cket using awscl
+0001a300: 690a 2020 2020 2020 2020 656e 6470 6f69  i.        endpoi
+0001a310: 6e74 5f75 726c 203d 2063 6c6f 7564 666c  nt_url = cloudfl
+0001a320: 6172 652e 6372 6561 7465 5f65 6e64 706f  are.create_endpo
+0001a330: 696e 7428 290a 2020 2020 2020 2020 7375  int().        su
+0001a340: 6270 726f 6365 7373 2e63 6865 636b 5f63  bprocess.check_c
+0001a350: 616c 6c28 0a20 2020 2020 2020 2020 2020  all(.           
+0001a360: 2066 2741 5753 5f53 4841 5245 445f 4352   f'AWS_SHARED_CR
+0001a370: 4544 454e 5449 414c 535f 4649 4c45 3d7b  EDENTIALS_FILE={
+0001a380: 636c 6f75 6466 6c61 7265 2e52 325f 4352  cloudflare.R2_CR
+0001a390: 4544 454e 5449 414c 535f 5041 5448 7d20  EDENTIALS_PATH} 
+0001a3a0: 6177 7320 7333 206d 6220 7333 3a2f 2f7b  aws s3 mb s3://{
+0001a3b0: 746d 705f 6275 636b 6574 5f6e 616d 657d  tmp_bucket_name}
+0001a3c0: 202d 2d65 6e64 706f 696e 7420 7b65 6e64   --endpoint {end
+0001a3d0: 706f 696e 745f 7572 6c7d 202d 2d70 726f  point_url} --pro
+0001a3e0: 6669 6c65 3d72 3227 2c0a 2020 2020 2020  file=r2',.      
+0001a3f0: 2020 2020 2020 7368 656c 6c3d 5472 7565        shell=True
+0001a400: 290a 2020 2020 2020 2020 7969 656c 6420  ).        yield 
+0001a410: 746d 705f 6275 636b 6574 5f6e 616d 650a  tmp_bucket_name.
+0001a420: 2020 2020 2020 2020 7375 6270 726f 6365          subproce
+0001a430: 7373 2e63 6865 636b 5f63 616c 6c28 0a20  ss.check_call(. 
+0001a440: 2020 2020 2020 2020 2020 2066 2741 5753             f'AWS
+0001a450: 5f53 4841 5245 445f 4352 4544 454e 5449  _SHARED_CREDENTI
+0001a460: 414c 535f 4649 4c45 3d7b 636c 6f75 6466  ALS_FILE={cloudf
+0001a470: 6c61 7265 2e52 325f 4352 4544 454e 5449  lare.R2_CREDENTI
+0001a480: 414c 535f 5041 5448 7d20 6177 7320 7333  ALS_PATH} aws s3
+0001a490: 2072 6220 7333 3a2f 2f7b 746d 705f 6275   rb s3://{tmp_bu
+0001a4a0: 636b 6574 5f6e 616d 657d 202d 2d66 6f72  cket_name} --for
+0001a4b0: 6365 202d 2d65 6e64 706f 696e 7420 7b65  ce --endpoint {e
+0001a4c0: 6e64 706f 696e 745f 7572 6c7d 202d 2d70  ndpoint_url} --p
+0001a4d0: 726f 6669 6c65 3d72 3227 2c0a 2020 2020  rofile=r2',.    
+0001a4e0: 2020 2020 2020 2020 7368 656c 6c3d 5472          shell=Tr
+0001a4f0: 7565 290a 0a20 2020 2040 7079 7465 7374  ue)..    @pytest
+0001a500: 2e66 6978 7475 7265 0a20 2020 2064 6566  .fixture.    def
+0001a510: 2074 6d70 5f70 7562 6c69 635f 7374 6f72   tmp_public_stor
+0001a520: 6167 655f 6f62 6a28 7365 6c66 2c20 7265  age_obj(self, re
+0001a530: 7175 6573 7429 3a0a 2020 2020 2020 2020  quest):.        
+0001a540: 2320 496e 6974 6961 6c69 7a65 7320 6120  # Initializes a 
+0001a550: 7374 6f72 6167 6520 6f62 6a65 6374 2077  storage object w
+0001a560: 6974 6820 6120 7075 626c 6963 2062 7563  ith a public buc
+0001a570: 6b65 740a 2020 2020 2020 2020 7374 6f72  ket.        stor
+0001a580: 6167 655f 6f62 6a20 3d20 7374 6f72 6167  age_obj = storag
+0001a590: 655f 6c69 622e 5374 6f72 6167 6528 736f  e_lib.Storage(so
+0001a5a0: 7572 6365 3d72 6571 7565 7374 2e70 6172  urce=request.par
+0001a5b0: 616d 290a 2020 2020 2020 2020 7969 656c  am).        yiel
+0001a5c0: 6420 7374 6f72 6167 655f 6f62 6a0a 2020  d storage_obj.  
+0001a5d0: 2020 2020 2020 2320 5468 6973 2064 6f65        # This doe
+0001a5e0: 7320 6e6f 7420 7265 7175 6972 6520 616e  s not require an
+0001a5f0: 7920 6465 6c65 7469 6f6e 206c 6f67 6963  y deletion logic
+0001a600: 2062 6563 6175 7365 2069 7420 6973 2061   because it is a
+0001a610: 2070 7562 6c69 6320 6275 636b 6574 0a20   public bucket. 
+0001a620: 2020 2020 2020 2023 2061 6e64 2073 686f         # and sho
+0001a630: 756c 6420 6e6f 7420 6765 7420 6164 6465  uld not get adde
+0001a640: 6420 746f 2067 6c6f 6261 6c5f 7573 6572  d to global_user
+0001a650: 5f73 7461 7465 2e0a 0a20 2020 2040 7079  _state...    @py
+0001a660: 7465 7374 2e6d 6172 6b2e 7061 7261 6d65  test.mark.parame
+0001a670: 7472 697a 6528 2773 746f 7265 5f74 7970  trize('store_typ
+0001a680: 6527 2c20 5b0a 2020 2020 2020 2020 7374  e', [.        st
+0001a690: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
+0001a6a0: 7970 652e 5333 2c20 7374 6f72 6167 655f  ype.S3, storage_
+0001a6b0: 6c69 622e 5374 6f72 6554 7970 652e 4743  lib.StoreType.GC
+0001a6c0: 532c 0a20 2020 2020 2020 2070 7974 6573  S,.        pytes
+0001a6d0: 742e 7061 7261 6d28 7374 6f72 6167 655f  t.param(storage_
+0001a6e0: 6c69 622e 5374 6f72 6554 7970 652e 5232  lib.StoreType.R2
+0001a6f0: 2c20 6d61 726b 733d 7079 7465 7374 2e6d  , marks=pytest.m
+0001a700: 6172 6b2e 636c 6f75 6466 6c61 7265 290a  ark.cloudflare).
+0001a710: 2020 2020 5d29 0a20 2020 2064 6566 2074      ]).    def t
+0001a720: 6573 745f 6e65 775f 6275 636b 6574 5f63  est_new_bucket_c
+0001a730: 7265 6174 696f 6e5f 616e 645f 6465 6c65  reation_and_dele
+0001a740: 7469 6f6e 2873 656c 662c 2074 6d70 5f6c  tion(self, tmp_l
+0001a750: 6f63 616c 5f73 746f 7261 6765 5f6f 626a  ocal_storage_obj
+0001a760: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001a770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a790: 7374 6f72 655f 7479 7065 293a 0a20 2020  store_type):.   
+0001a7a0: 2020 2020 2023 2043 7265 6174 6573 2061       # Creates a
+0001a7b0: 206e 6577 2062 7563 6b65 7420 7769 7468   new bucket with
+0001a7c0: 2061 206c 6f63 616c 2073 6f75 7263 652c   a local source,
+0001a7d0: 2075 706c 6f61 6473 2066 696c 6573 2074   uploads files t
+0001a7e0: 6f20 6974 0a20 2020 2020 2020 2023 2061  o it.        # a
+0001a7f0: 6e64 2064 656c 6574 6573 2069 742e 0a20  nd deletes it.. 
+0001a800: 2020 2020 2020 2074 6d70 5f6c 6f63 616c         tmp_local
+0001a810: 5f73 746f 7261 6765 5f6f 626a 2e61 6464  _storage_obj.add
+0001a820: 5f73 746f 7265 2873 746f 7265 5f74 7970  _store(store_typ
+0001a830: 6529 0a0a 2020 2020 2020 2020 2320 5275  e)..        # Ru
+0001a840: 6e20 736b 7920 7374 6f72 6167 6520 6c73  n sky storage ls
+0001a850: 2074 6f20 6368 6563 6b20 6966 2073 746f   to check if sto
+0001a860: 7261 6765 206f 626a 6563 7420 6578 6973  rage object exis
+0001a870: 7473 2069 6e20 7468 6520 6f75 7470 7574  ts in the output
+0001a880: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
+0001a890: 7562 7072 6f63 6573 732e 6368 6563 6b5f  ubprocess.check_
+0001a8a0: 6f75 7470 7574 285b 2773 6b79 272c 2027  output(['sky', '
+0001a8b0: 7374 6f72 6167 6527 2c20 276c 7327 5d29  storage', 'ls'])
+0001a8c0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0001a8d0: 746d 705f 6c6f 6361 6c5f 7374 6f72 6167  tmp_local_storag
+0001a8e0: 655f 6f62 6a2e 6e61 6d65 2069 6e20 6f75  e_obj.name in ou
+0001a8f0: 742e 6465 636f 6465 2827 7574 662d 3827  t.decode('utf-8'
+0001a900: 290a 0a20 2020 2020 2020 2023 2052 756e  )..        # Run
+0001a910: 2073 6b79 2073 746f 7261 6765 2064 656c   sky storage del
+0001a920: 6574 6520 746f 2064 656c 6574 6520 7468  ete to delete th
+0001a930: 6520 7374 6f72 6167 6520 6f62 6a65 6374  e storage object
+0001a940: 0a20 2020 2020 2020 2073 7562 7072 6f63  .        subproc
+0001a950: 6573 732e 6368 6563 6b5f 6f75 7470 7574  ess.check_output
+0001a960: 280a 2020 2020 2020 2020 2020 2020 5b27  (.            ['
+0001a970: 736b 7927 2c20 2773 746f 7261 6765 272c  sky', 'storage',
+0001a980: 2027 6465 6c65 7465 272c 2074 6d70 5f6c   'delete', tmp_l
+0001a990: 6f63 616c 5f73 746f 7261 6765 5f6f 626a  ocal_storage_obj
+0001a9a0: 2e6e 616d 655d 290a 0a20 2020 2020 2020  .name])..       
+0001a9b0: 2023 2052 756e 2073 6b79 2073 746f 7261   # Run sky stora
+0001a9c0: 6765 206c 7320 746f 2063 6865 636b 2069  ge ls to check i
+0001a9d0: 6620 7374 6f72 6167 6520 6f62 6a65 6374  f storage object
+0001a9e0: 2069 7320 6465 6c65 7465 640a 2020 2020   is deleted.    
+0001a9f0: 2020 2020 6f75 7420 3d20 7375 6270 726f      out = subpro
+0001aa00: 6365 7373 2e63 6865 636b 5f6f 7574 7075  cess.check_outpu
+0001aa10: 7428 5b27 736b 7927 2c20 2773 746f 7261  t(['sky', 'stora
+0001aa20: 6765 272c 2027 6c73 275d 290a 2020 2020  ge', 'ls']).    
+0001aa30: 2020 2020 6173 7365 7274 2074 6d70 5f6c      assert tmp_l
+0001aa40: 6f63 616c 5f73 746f 7261 6765 5f6f 626a  ocal_storage_obj
+0001aa50: 2e6e 616d 6520 6e6f 7420 696e 206f 7574  .name not in out
+0001aa60: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
+0001aa70: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
+0001aa80: 726b 2e78 6469 7374 5f67 726f 7570 2827  rk.xdist_group('
+0001aa90: 6d75 6c74 6970 6c65 5f62 7563 6b65 745f  multiple_bucket_
+0001aaa0: 6465 6c65 7469 6f6e 2729 0a20 2020 2040  deletion').    @
+0001aab0: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
+0001aac0: 6d65 7472 697a 6528 2773 746f 7265 5f74  metrize('store_t
+0001aad0: 7970 6527 2c20 5b0a 2020 2020 2020 2020  ype', [.        
+0001aae0: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
+0001aaf0: 6554 7970 652e 5333 2c20 7374 6f72 6167  eType.S3, storag
+0001ab00: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
+0001ab10: 4743 532c 0a20 2020 2020 2020 2070 7974  GCS,.        pyt
+0001ab20: 6573 742e 7061 7261 6d28 7374 6f72 6167  est.param(storag
+0001ab30: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
+0001ab40: 5232 2c20 6d61 726b 733d 7079 7465 7374  R2, marks=pytest
+0001ab50: 2e6d 6172 6b2e 636c 6f75 6466 6c61 7265  .mark.cloudflare
+0001ab60: 290a 2020 2020 5d29 0a20 2020 2064 6566  ).    ]).    def
+0001ab70: 2074 6573 745f 6d75 6c74 6970 6c65 5f62   test_multiple_b
+0001ab80: 7563 6b65 7473 5f63 7265 6174 696f 6e5f  uckets_creation_
+0001ab90: 616e 645f 6465 6c65 7469 6f6e 280a 2020  and_deletion(.  
+0001aba0: 2020 2020 2020 2020 2020 7365 6c66 2c20            self, 
+0001abb0: 746d 705f 6d75 6c74 6970 6c65 5f73 6372  tmp_multiple_scr
+0001abc0: 6174 6368 5f73 746f 7261 6765 5f6f 626a  atch_storage_obj
+0001abd0: 2c20 7374 6f72 655f 7479 7065 293a 0a20  , store_type):. 
+0001abe0: 2020 2020 2020 2023 2043 7265 6174 6573         # Creates
+0001abf0: 206d 756c 7469 706c 6520 6e65 7720 6275   multiple new bu
+0001ac00: 636b 6574 7328 3520 6275 636b 6574 7329  ckets(5 buckets)
+0001ac10: 2077 6974 6820 6120 6c6f 6361 6c20 736f   with a local so
+0001ac20: 7572 6365 0a20 2020 2020 2020 2023 2061  urce.        # a
+0001ac30: 6e64 2064 656c 6574 6573 2074 6865 6d2e  nd deletes them.
+0001ac40: 0a20 2020 2020 2020 2073 746f 7261 6765  .        storage
+0001ac50: 5f6f 626a 5f6e 616d 6520 3d20 5b5d 0a20  _obj_name = []. 
+0001ac60: 2020 2020 2020 2066 6f72 2073 746f 7265         for store
+0001ac70: 5f6f 626a 2069 6e20 746d 705f 6d75 6c74  _obj in tmp_mult
+0001ac80: 6970 6c65 5f73 6372 6174 6368 5f73 746f  iple_scratch_sto
+0001ac90: 7261 6765 5f6f 626a 3a0a 2020 2020 2020  rage_obj:.      
+0001aca0: 2020 2020 2020 7374 6f72 655f 6f62 6a2e        store_obj.
+0001acb0: 6164 645f 7374 6f72 6528 7374 6f72 655f  add_store(store_
+0001acc0: 7479 7065 290a 2020 2020 2020 2020 2020  type).          
+0001acd0: 2020 7374 6f72 6167 655f 6f62 6a5f 6e61    storage_obj_na
+0001ace0: 6d65 2e61 7070 656e 6428 7374 6f72 655f  me.append(store_
+0001acf0: 6f62 6a2e 6e61 6d65 290a 0a20 2020 2020  obj.name)..     
+0001ad00: 2020 2023 2052 756e 2073 6b79 2073 746f     # Run sky sto
+0001ad10: 7261 6765 206c 7320 746f 2063 6865 636b  rage ls to check
+0001ad20: 2069 6620 616c 6c20 7374 6f72 6167 6520   if all storage 
+0001ad30: 6f62 6a65 6374 7320 6578 6973 7473 2069  objects exists i
+0001ad40: 6e20 7468 650a 2020 2020 2020 2020 2320  n the.        # 
+0001ad50: 6f75 7470 7574 2066 696c 7465 7265 6420  output filtered 
+0001ad60: 6279 2073 746f 7265 2074 7970 650a 2020  by store type.  
+0001ad70: 2020 2020 2020 6f75 745f 616c 6c20 3d20        out_all = 
+0001ad80: 7375 6270 726f 6365 7373 2e63 6865 636b  subprocess.check
+0001ad90: 5f6f 7574 7075 7428 5b27 736b 7927 2c20  _output(['sky', 
+0001ada0: 2773 746f 7261 6765 272c 2027 6c73 275d  'storage', 'ls']
+0001adb0: 290a 2020 2020 2020 2020 6f75 7420 3d20  ).        out = 
+0001adc0: 5b0a 2020 2020 2020 2020 2020 2020 6974  [.            it
+0001add0: 656d 2e73 706c 6974 2829 5b30 5d0a 2020  em.split()[0].  
+0001ade0: 2020 2020 2020 2020 2020 666f 7220 6974            for it
+0001adf0: 656d 2069 6e20 6f75 745f 616c 6c2e 6465  em in out_all.de
+0001ae00: 636f 6465 2827 7574 662d 3827 292e 7370  code('utf-8').sp
+0001ae10: 6c69 746c 696e 6573 2829 0a20 2020 2020  litlines().     
+0001ae20: 2020 2020 2020 2069 6620 7374 6f72 655f         if store_
+0001ae30: 7479 7065 2e76 616c 7565 2069 6e20 6974  type.value in it
+0001ae40: 656d 0a20 2020 2020 2020 205d 0a20 2020  em.        ].   
+0001ae50: 2020 2020 2061 7373 6572 7420 616c 6c28       assert all(
+0001ae60: 5b69 7465 6d20 696e 206f 7574 2066 6f72  [item in out for
+0001ae70: 2069 7465 6d20 696e 2073 746f 7261 6765   item in storage
+0001ae80: 5f6f 626a 5f6e 616d 655d 290a 0a20 2020  _obj_name])..   
+0001ae90: 2020 2020 2023 2052 756e 2073 6b79 2073       # Run sky s
+0001aea0: 746f 7261 6765 2064 656c 6574 6520 616c  torage delete al
+0001aeb0: 6c20 746f 2064 656c 6574 6520 616c 6c20  l to delete all 
+0001aec0: 7374 6f72 6167 6520 6f62 6a65 6374 730a  storage objects.
+0001aed0: 2020 2020 2020 2020 7375 6270 726f 6365          subproce
+0001aee0: 7373 2e63 6865 636b 5f6f 7574 7075 7428  ss.check_output(
+0001aef0: 5b27 736b 7927 2c20 2773 746f 7261 6765  ['sky', 'storage
+0001af00: 272c 2027 6465 6c65 7465 272c 2027 2d61  ', 'delete', '-a
+0001af10: 275d 290a 0a20 2020 2020 2020 2023 2052  '])..        # R
+0001af20: 756e 2073 6b79 2073 746f 7261 6765 206c  un sky storage l
+0001af30: 7320 746f 2063 6865 636b 2069 6620 616c  s to check if al
+0001af40: 6c20 7374 6f72 6167 6520 6f62 6a65 6374  l storage object
+0001af50: 7320 6669 6c74 6572 6564 2062 7920 7374  s filtered by st
+0001af60: 6f72 650a 2020 2020 2020 2020 2320 7479  ore.        # ty
+0001af70: 7065 2061 7265 2064 656c 6574 6564 0a20  pe are deleted. 
+0001af80: 2020 2020 2020 206f 7574 5f61 6c6c 203d         out_all =
+0001af90: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
+0001afa0: 6b5f 6f75 7470 7574 285b 2773 6b79 272c  k_output(['sky',
+0001afb0: 2027 7374 6f72 6167 6527 2c20 276c 7327   'storage', 'ls'
+0001afc0: 5d29 0a20 2020 2020 2020 206f 7574 203d  ]).        out =
+0001afd0: 205b 0a20 2020 2020 2020 2020 2020 2069   [.            i
+0001afe0: 7465 6d2e 7370 6c69 7428 295b 305d 0a20  tem.split()[0]. 
+0001aff0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+0001b000: 7465 6d20 696e 206f 7574 5f61 6c6c 2e64  tem in out_all.d
+0001b010: 6563 6f64 6528 2775 7466 2d38 2729 2e73  ecode('utf-8').s
+0001b020: 706c 6974 6c69 6e65 7328 290a 2020 2020  plitlines().    
+0001b030: 2020 2020 2020 2020 6966 2073 746f 7265          if store
+0001b040: 5f74 7970 652e 7661 6c75 6520 696e 2069  _type.value in i
+0001b050: 7465 6d0a 2020 2020 2020 2020 5d0a 2020  tem.        ].  
+0001b060: 2020 2020 2020 6173 7365 7274 2061 6c6c        assert all
+0001b070: 285b 6974 656d 206e 6f74 2069 6e20 6f75  ([item not in ou
+0001b080: 7420 666f 7220 6974 656d 2069 6e20 7374  t for item in st
+0001b090: 6f72 6167 655f 6f62 6a5f 6e61 6d65 5d29  orage_obj_name])
+0001b0a0: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
+0001b0b0: 726b 2e70 6172 616d 6574 7269 7a65 2827  rk.parametrize('
+0001b0c0: 7374 6f72 655f 7479 7065 272c 205b 0a20  store_type', [. 
+0001b0d0: 2020 2020 2020 2073 746f 7261 6765 5f6c         storage_l
+0001b0e0: 6962 2e53 746f 7265 5479 7065 2e53 332c  ib.StoreType.S3,
+0001b0f0: 2073 746f 7261 6765 5f6c 6962 2e53 746f   storage_lib.Sto
+0001b100: 7265 5479 7065 2e47 4353 2c0a 2020 2020  reType.GCS,.    
+0001b110: 2020 2020 7079 7465 7374 2e70 6172 616d      pytest.param
+0001b120: 2873 746f 7261 6765 5f6c 6962 2e53 746f  (storage_lib.Sto
+0001b130: 7265 5479 7065 2e52 322c 206d 6172 6b73  reType.R2, marks
+0001b140: 3d70 7974 6573 742e 6d61 726b 2e63 6c6f  =pytest.mark.clo
+0001b150: 7564 666c 6172 6529 0a20 2020 205d 290a  udflare).    ]).
+0001b160: 2020 2020 6465 6620 7465 7374 5f62 7563      def test_buc
+0001b170: 6b65 745f 6578 7465 726e 616c 5f64 656c  ket_external_del
+0001b180: 6574 696f 6e28 7365 6c66 2c20 746d 705f  etion(self, tmp_
+0001b190: 7363 7261 7463 685f 7374 6f72 6167 655f  scratch_storage_
+0001b1a0: 6f62 6a2c 0a20 2020 2020 2020 2020 2020  obj,.           
+0001b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b1c0: 2020 2020 2020 2020 2020 2073 746f 7265             store
+0001b1d0: 5f74 7970 6529 3a0a 2020 2020 2020 2020  _type):.        
+0001b1e0: 2320 4372 6561 7465 7320 6120 6275 636b  # Creates a buck
+0001b1f0: 6574 2c20 6465 6c65 7465 7320 6974 2065  et, deletes it e
+0001b200: 7874 6572 6e61 6c6c 7920 7573 696e 6720  xternally using 
+0001b210: 636c 6f75 6420 636c 6920 636f 6d6d 616e  cloud cli comman
+0001b220: 6473 0a20 2020 2020 2020 2023 2061 6e64  ds.        # and
+0001b230: 2074 6865 6e20 7472 6965 7320 746f 2064   then tries to d
+0001b240: 656c 6574 6520 6974 2075 7369 6e67 2073  elete it using s
+0001b250: 6b79 2073 746f 7261 6765 2064 656c 6574  ky storage delet
+0001b260: 652e 0a20 2020 2020 2020 2074 6d70 5f73  e..        tmp_s
+0001b270: 6372 6174 6368 5f73 746f 7261 6765 5f6f  cratch_storage_o
+0001b280: 626a 2e61 6464 5f73 746f 7265 2873 746f  bj.add_store(sto
+0001b290: 7265 5f74 7970 6529 0a0a 2020 2020 2020  re_type)..      
+0001b2a0: 2020 2320 5275 6e20 736b 7920 7374 6f72    # Run sky stor
+0001b2b0: 6167 6520 6c73 2074 6f20 6368 6563 6b20  age ls to check 
+0001b2c0: 6966 2073 746f 7261 6765 206f 626a 6563  if storage objec
+0001b2d0: 7420 6578 6973 7473 2069 6e20 7468 6520  t exists in the 
+0001b2e0: 6f75 7470 7574 0a20 2020 2020 2020 206f  output.        o
+0001b2f0: 7574 203d 2073 7562 7072 6f63 6573 732e  ut = subprocess.
+0001b300: 6368 6563 6b5f 6f75 7470 7574 285b 2773  check_output(['s
+0001b310: 6b79 272c 2027 7374 6f72 6167 6527 2c20  ky', 'storage', 
+0001b320: 276c 7327 5d29 0a20 2020 2020 2020 2061  'ls']).        a
+0001b330: 7373 6572 7420 746d 705f 7363 7261 7463  ssert tmp_scratc
+0001b340: 685f 7374 6f72 6167 655f 6f62 6a2e 6e61  h_storage_obj.na
+0001b350: 6d65 2069 6e20 6f75 742e 6465 636f 6465  me in out.decode
+0001b360: 2827 7574 662d 3827 290a 0a20 2020 2020  ('utf-8')..     
+0001b370: 2020 2023 2044 656c 6574 6520 6275 636b     # Delete buck
+0001b380: 6574 2065 7874 6572 6e61 6c6c 790a 2020  et externally.  
+0001b390: 2020 2020 2020 636d 6420 3d20 7365 6c66        cmd = self
+0001b3a0: 2e63 6c69 5f64 656c 6574 655f 636d 6428  .cli_delete_cmd(
+0001b3b0: 7374 6f72 655f 7479 7065 2c20 746d 705f  store_type, tmp_
+0001b3c0: 7363 7261 7463 685f 7374 6f72 6167 655f  scratch_storage_
+0001b3d0: 6f62 6a2e 6e61 6d65 290a 2020 2020 2020  obj.name).      
+0001b3e0: 2020 7375 6270 726f 6365 7373 2e63 6865    subprocess.che
+0001b3f0: 636b 5f6f 7574 7075 7428 636d 642c 2073  ck_output(cmd, s
+0001b400: 6865 6c6c 3d54 7275 6529 0a0a 2020 2020  hell=True)..    
+0001b410: 2020 2020 2320 5275 6e20 736b 7920 7374      # Run sky st
+0001b420: 6f72 6167 6520 6465 6c65 7465 2074 6f20  orage delete to 
+0001b430: 6465 6c65 7465 2074 6865 2073 746f 7261  delete the stora
+0001b440: 6765 206f 626a 6563 740a 2020 2020 2020  ge object.      
+0001b450: 2020 6f75 7420 3d20 7375 6270 726f 6365    out = subproce
+0001b460: 7373 2e63 6865 636b 5f6f 7574 7075 7428  ss.check_output(
+0001b470: 0a20 2020 2020 2020 2020 2020 205b 2773  .            ['s
+0001b480: 6b79 272c 2027 7374 6f72 6167 6527 2c20  ky', 'storage', 
+0001b490: 2764 656c 6574 6527 2c20 746d 705f 7363  'delete', tmp_sc
+0001b4a0: 7261 7463 685f 7374 6f72 6167 655f 6f62  ratch_storage_ob
+0001b4b0: 6a2e 6e61 6d65 5d29 0a20 2020 2020 2020  j.name]).       
+0001b4c0: 2023 204d 616b 6520 7375 7265 2062 7563   # Make sure buc
+0001b4d0: 6b65 7420 7761 7320 6e6f 7420 6372 6561  ket was not crea
+0001b4e0: 7465 6420 6475 7269 6e67 2064 656c 6574  ted during delet
+0001b4f0: 696f 6e20 2873 6565 2069 7373 7565 2023  ion (see issue #
+0001b500: 3133 3232 290a 2020 2020 2020 2020 6173  1322).        as
+0001b510: 7365 7274 2027 6372 6561 7465 6427 206e  sert 'created' n
+0001b520: 6f74 2069 6e20 6f75 742e 6465 636f 6465  ot in out.decode
+0001b530: 2827 7574 662d 3827 292e 6c6f 7765 7228  ('utf-8').lower(
+0001b540: 290a 0a20 2020 2020 2020 2023 2052 756e  )..        # Run
+0001b550: 2073 6b79 2073 746f 7261 6765 206c 7320   sky storage ls 
+0001b560: 746f 2063 6865 636b 2069 6620 7374 6f72  to check if stor
+0001b570: 6167 6520 6f62 6a65 6374 2069 7320 6465  age object is de
+0001b580: 6c65 7465 640a 2020 2020 2020 2020 6f75  leted.        ou
+0001b590: 7420 3d20 7375 6270 726f 6365 7373 2e63  t = subprocess.c
+0001b5a0: 6865 636b 5f6f 7574 7075 7428 5b27 736b  heck_output(['sk
+0001b5b0: 7927 2c20 2773 746f 7261 6765 272c 2027  y', 'storage', '
+0001b5c0: 6c73 275d 290a 2020 2020 2020 2020 6173  ls']).        as
+0001b5d0: 7365 7274 2074 6d70 5f73 6372 6174 6368  sert tmp_scratch
+0001b5e0: 5f73 746f 7261 6765 5f6f 626a 2e6e 616d  _storage_obj.nam
+0001b5f0: 6520 6e6f 7420 696e 206f 7574 2e64 6563  e not in out.dec
+0001b600: 6f64 6528 2775 7466 2d38 2729 0a0a 2020  ode('utf-8')..  
+0001b610: 2020 4070 7974 6573 742e 6d61 726b 2e70    @pytest.mark.p
+0001b620: 6172 616d 6574 7269 7a65 2827 7374 6f72  arametrize('stor
+0001b630: 655f 7479 7065 272c 205b 0a20 2020 2020  e_type', [.     
+0001b640: 2020 2073 746f 7261 6765 5f6c 6962 2e53     storage_lib.S
+0001b650: 746f 7265 5479 7065 2e53 332c 2073 746f  toreType.S3, sto
+0001b660: 7261 6765 5f6c 6962 2e53 746f 7265 5479  rage_lib.StoreTy
+0001b670: 7065 2e47 4353 2c0a 2020 2020 2020 2020  pe.GCS,.        
+0001b680: 7079 7465 7374 2e70 6172 616d 2873 746f  pytest.param(sto
+0001b690: 7261 6765 5f6c 6962 2e53 746f 7265 5479  rage_lib.StoreTy
+0001b6a0: 7065 2e52 322c 206d 6172 6b73 3d70 7974  pe.R2, marks=pyt
+0001b6b0: 6573 742e 6d61 726b 2e63 6c6f 7564 666c  est.mark.cloudfl
+0001b6c0: 6172 6529 0a20 2020 205d 290a 2020 2020  are).    ]).    
+0001b6d0: 6465 6620 7465 7374 5f62 7563 6b65 745f  def test_bucket_
+0001b6e0: 6275 6c6b 5f64 656c 6574 696f 6e28 7365  bulk_deletion(se
+0001b6f0: 6c66 2c20 7374 6f72 655f 7479 7065 2c20  lf, store_type, 
+0001b700: 746d 705f 6275 6c6b 5f64 656c 5f73 746f  tmp_bulk_del_sto
+0001b710: 7261 6765 5f6f 626a 293a 0a20 2020 2020  rage_obj):.     
+0001b720: 2020 2023 2043 7265 6174 6573 2061 2074     # Creates a t
+0001b730: 656d 7020 666f 6c64 6572 2077 6974 6820  emp folder with 
+0001b740: 6f76 6572 2032 3536 2066 696c 6573 2061  over 256 files a
+0001b750: 6e64 2066 6f6c 6465 7273 2c20 7570 6c6f  nd folders, uplo
+0001b760: 6164 0a20 2020 2020 2020 2023 2066 696c  ad.        # fil
+0001b770: 6573 2061 6e64 2066 6f6c 6465 7273 2074  es and folders t
+0001b780: 6f20 6120 6e65 7720 6275 636b 6574 2c20  o a new bucket, 
+0001b790: 7468 656e 2064 656c 6574 6520 6275 636b  then delete buck
+0001b7a0: 6574 2e0a 2020 2020 2020 2020 746d 705f  et..        tmp_
+0001b7b0: 6275 6c6b 5f64 656c 5f73 746f 7261 6765  bulk_del_storage
+0001b7c0: 5f6f 626a 2e61 6464 5f73 746f 7265 2873  _obj.add_store(s
+0001b7d0: 746f 7265 5f74 7970 6529 0a0a 2020 2020  tore_type)..    
+0001b7e0: 2020 2020 7375 6270 726f 6365 7373 2e63      subprocess.c
+0001b7f0: 6865 636b 5f6f 7574 7075 7428 0a20 2020  heck_output(.   
+0001b800: 2020 2020 2020 2020 205b 2773 6b79 272c           ['sky',
+0001b810: 2027 7374 6f72 6167 6527 2c20 2764 656c   'storage', 'del
+0001b820: 6574 6527 2c20 746d 705f 6275 6c6b 5f64  ete', tmp_bulk_d
+0001b830: 656c 5f73 746f 7261 6765 5f6f 626a 2e6e  el_storage_obj.n
+0001b840: 616d 655d 290a 0a20 2020 2020 2020 206f  ame])..        o
+0001b850: 7574 7075 7420 3d20 7375 6270 726f 6365  utput = subproce
+0001b860: 7373 2e63 6865 636b 5f6f 7574 7075 7428  ss.check_output(
+0001b870: 5b27 736b 7927 2c20 2773 746f 7261 6765  ['sky', 'storage
+0001b880: 272c 2027 6c73 275d 290a 2020 2020 2020  ', 'ls']).      
+0001b890: 2020 6173 7365 7274 2074 6d70 5f62 756c    assert tmp_bul
+0001b8a0: 6b5f 6465 6c5f 7374 6f72 6167 655f 6f62  k_del_storage_ob
+0001b8b0: 6a2e 6e61 6d65 206e 6f74 2069 6e20 6f75  j.name not in ou
+0001b8c0: 7470 7574 2e64 6563 6f64 6528 2775 7466  tput.decode('utf
+0001b8d0: 2d38 2729 0a0a 2020 2020 4070 7974 6573  -8')..    @pytes
+0001b8e0: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
+0001b8f0: 7a65 280a 2020 2020 2020 2020 2774 6d70  ze(.        'tmp
+0001b900: 5f70 7562 6c69 635f 7374 6f72 6167 655f  _public_storage_
+0001b910: 6f62 6a2c 2073 746f 7265 5f74 7970 6527  obj, store_type'
+0001b920: 2c0a 2020 2020 2020 2020 5b28 2773 333a  ,.        [('s3:
+0001b930: 2f2f 7463 6761 2d32 2d6f 7065 6e27 2c20  //tcga-2-open', 
+0001b940: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
+0001b950: 6554 7970 652e 5333 292c 0a20 2020 2020  eType.S3),.     
+0001b960: 2020 2020 2827 7333 3a2f 2f64 6967 6974      ('s3://digit
+0001b970: 616c 636f 7270 6f72 6127 2c20 7374 6f72  alcorpora', stor
+0001b980: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
+0001b990: 652e 5333 292c 0a20 2020 2020 2020 2020  e.S3),.         
+0001b9a0: 2827 6773 3a2f 2f67 6370 2d70 7562 6c69  ('gs://gcp-publi
+0001b9b0: 632d 6461 7461 2d73 656e 7469 6e65 6c2d  c-data-sentinel-
+0001b9c0: 3227 2c20 7374 6f72 6167 655f 6c69 622e  2', storage_lib.
+0001b9d0: 5374 6f72 6554 7970 652e 4743 5329 5d2c  StoreType.GCS)],
+0001b9e0: 0a20 2020 2020 2020 2069 6e64 6972 6563  .        indirec
+0001b9f0: 743d 5b27 746d 705f 7075 626c 6963 5f73  t=['tmp_public_s
+0001ba00: 746f 7261 6765 5f6f 626a 275d 290a 2020  torage_obj']).  
+0001ba10: 2020 6465 6620 7465 7374 5f70 7562 6c69    def test_publi
+0001ba20: 635f 6275 636b 6574 2873 656c 662c 2074  c_bucket(self, t
+0001ba30: 6d70 5f70 7562 6c69 635f 7374 6f72 6167  mp_public_storag
+0001ba40: 655f 6f62 6a2c 2073 746f 7265 5f74 7970  e_obj, store_typ
+0001ba50: 6529 3a0a 2020 2020 2020 2020 2320 4372  e):.        # Cr
+0001ba60: 6561 7465 7320 6120 6e65 7720 6275 636b  eates a new buck
+0001ba70: 6574 2077 6974 6820 6120 7075 626c 6963  et with a public
+0001ba80: 2073 6f75 7263 6520 616e 6420 7665 7269   source and veri
+0001ba90: 6669 6573 2074 6861 7420 6974 2069 7320  fies that it is 
+0001baa0: 6e6f 740a 2020 2020 2020 2020 2320 6164  not.        # ad
+0001bab0: 6465 6420 746f 2067 6c6f 6261 6c5f 7573  ded to global_us
+0001bac0: 6572 5f73 7461 7465 2e0a 2020 2020 2020  er_state..      
+0001bad0: 2020 746d 705f 7075 626c 6963 5f73 746f    tmp_public_sto
+0001bae0: 7261 6765 5f6f 626a 2e61 6464 5f73 746f  rage_obj.add_sto
+0001baf0: 7265 2873 746f 7265 5f74 7970 6529 0a0a  re(store_type)..
+0001bb00: 2020 2020 2020 2020 2320 5275 6e20 736b          # Run sk
+0001bb10: 7920 7374 6f72 6167 6520 6c73 2074 6f20  y storage ls to 
+0001bb20: 6368 6563 6b20 6966 2073 746f 7261 6765  check if storage
+0001bb30: 206f 626a 6563 7420 6578 6973 7473 2069   object exists i
+0001bb40: 6e20 7468 6520 6f75 7470 7574 0a20 2020  n the output.   
+0001bb50: 2020 2020 206f 7574 203d 2073 7562 7072       out = subpr
+0001bb60: 6f63 6573 732e 6368 6563 6b5f 6f75 7470  ocess.check_outp
+0001bb70: 7574 285b 2773 6b79 272c 2027 7374 6f72  ut(['sky', 'stor
+0001bb80: 6167 6527 2c20 276c 7327 5d29 0a20 2020  age', 'ls']).   
+0001bb90: 2020 2020 2061 7373 6572 7420 746d 705f       assert tmp_
+0001bba0: 7075 626c 6963 5f73 746f 7261 6765 5f6f  public_storage_o
+0001bbb0: 626a 2e6e 616d 6520 6e6f 7420 696e 206f  bj.name not in o
+0001bbc0: 7574 2e64 6563 6f64 6528 2775 7466 2d38  ut.decode('utf-8
+0001bbd0: 2729 0a0a 2020 2020 4070 7974 6573 742e  ')..    @pytest.
+0001bbe0: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
+0001bbf0: 2827 6e6f 6e65 7869 7374 5f62 7563 6b65  ('nonexist_bucke
+0001bc00: 745f 7572 6c27 2c20 5b0a 2020 2020 2020  t_url', [.      
+0001bc10: 2020 2773 333a 2f2f 7b72 616e 646f 6d5f    's3://{random_
+0001bc20: 6e61 6d65 7d27 2c20 2767 733a 2f2f 7b72  name}', 'gs://{r
+0001bc30: 616e 646f 6d5f 6e61 6d65 7d27 2c0a 2020  andom_name}',.  
+0001bc40: 2020 2020 2020 7079 7465 7374 2e70 6172        pytest.par
+0001bc50: 616d 2827 7232 3a2f 2f7b 7261 6e64 6f6d  am('r2://{random
+0001bc60: 5f6e 616d 657d 272c 206d 6172 6b73 3d70  _name}', marks=p
+0001bc70: 7974 6573 742e 6d61 726b 2e63 6c6f 7564  ytest.mark.cloud
+0001bc80: 666c 6172 6529 0a20 2020 205d 290a 2020  flare).    ]).  
+0001bc90: 2020 6465 6620 7465 7374 5f6e 6f6e 6578    def test_nonex
+0001bca0: 6973 7465 6e74 5f62 7563 6b65 7428 7365  istent_bucket(se
+0001bcb0: 6c66 2c20 6e6f 6e65 7869 7374 5f62 7563  lf, nonexist_buc
+0001bcc0: 6b65 745f 7572 6c29 3a0a 2020 2020 2020  ket_url):.      
+0001bcd0: 2020 2320 4174 7465 6d70 7473 2074 6f20    # Attempts to 
+0001bce0: 6372 6561 7465 2066 6574 6368 2061 2073  create fetch a s
+0001bcf0: 7472 6f61 6765 2077 6974 6820 6120 6e6f  troage with a no
+0001bd00: 6e2d 6578 6973 7465 6e74 2073 6f75 7263  n-existent sourc
+0001bd10: 652e 0a20 2020 2020 2020 2023 2047 656e  e..        # Gen
+0001bd20: 6572 6174 6520 6120 7261 6e64 6f6d 2062  erate a random b
+0001bd30: 7563 6b65 7420 6e61 6d65 2061 6e64 2076  ucket name and v
+0001bd40: 6572 6966 7920 6974 2064 6f65 736e 2774  erify it doesn't
+0001bd50: 2065 7869 7374 3a0a 2020 2020 2020 2020   exist:.        
+0001bd60: 7265 7472 795f 636f 756e 7420 3d20 300a  retry_count = 0.
+0001bd70: 2020 2020 2020 2020 7768 696c 6520 5472          while Tr
+0001bd80: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
+0001bd90: 6e6f 6e65 7869 7374 5f62 7563 6b65 745f  nonexist_bucket_
+0001bda0: 6e61 6d65 203d 2073 7472 2875 7569 642e  name = str(uuid.
+0001bdb0: 7575 6964 3428 2929 0a20 2020 2020 2020  uuid4()).       
+0001bdc0: 2020 2020 2069 6620 6e6f 6e65 7869 7374       if nonexist
+0001bdd0: 5f62 7563 6b65 745f 7572 6c2e 7374 6172  _bucket_url.star
+0001bde0: 7473 7769 7468 2827 7333 2729 3a0a 2020  tswith('s3'):.  
+0001bdf0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0001be00: 6d6d 616e 6420 3d20 6627 6177 7320 7333  mmand = f'aws s3
+0001be10: 6170 6920 6865 6164 2d62 7563 6b65 7420  api head-bucket 
+0001be20: 2d2d 6275 636b 6574 207b 6e6f 6e65 7869  --bucket {nonexi
+0001be30: 7374 5f62 7563 6b65 745f 6e61 6d65 7d27  st_bucket_name}'
+0001be40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001be50: 2065 7870 6563 7465 645f 6f75 7470 7574   expected_output
+0001be60: 203d 2027 3430 3427 0a20 2020 2020 2020   = '404'.       
+0001be70: 2020 2020 2065 6c69 6620 6e6f 6e65 7869       elif nonexi
+0001be80: 7374 5f62 7563 6b65 745f 7572 6c2e 7374  st_bucket_url.st
+0001be90: 6172 7473 7769 7468 2827 6773 2729 3a0a  artswith('gs'):.
+0001bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001beb0: 636f 6d6d 616e 6420 3d20 6627 6773 7574  command = f'gsut
+0001bec0: 696c 206c 7320 7b6e 6f6e 6578 6973 745f  il ls {nonexist_
+0001bed0: 6275 636b 6574 5f75 726c 2e66 6f72 6d61  bucket_url.forma
+0001bee0: 7428 7261 6e64 6f6d 5f6e 616d 653d 6e6f  t(random_name=no
+0001bef0: 6e65 7869 7374 5f62 7563 6b65 745f 6e61  nexist_bucket_na
+0001bf00: 6d65 297d 270a 2020 2020 2020 2020 2020  me)}'.          
+0001bf10: 2020 2020 2020 6578 7065 6374 6564 5f6f        expected_o
+0001bf20: 7574 7075 7420 3d20 2742 7563 6b65 744e  utput = 'BucketN
+0001bf30: 6f74 466f 756e 6445 7863 6570 7469 6f6e  otFoundException
+0001bf40: 270a 2020 2020 2020 2020 2020 2020 656c  '.            el
+0001bf50: 6966 206e 6f6e 6578 6973 745f 6275 636b  if nonexist_buck
+0001bf60: 6574 5f75 726c 2e73 7461 7274 7377 6974  et_url.startswit
+0001bf70: 6828 2772 3227 293a 0a20 2020 2020 2020  h('r2'):.       
+0001bf80: 2020 2020 2020 2020 2065 6e64 706f 696e           endpoin
+0001bf90: 745f 7572 6c20 3d20 636c 6f75 6466 6c61  t_url = cloudfla
+0001bfa0: 7265 2e63 7265 6174 655f 656e 6470 6f69  re.create_endpoi
+0001bfb0: 6e74 2829 0a20 2020 2020 2020 2020 2020  nt().           
+0001bfc0: 2020 2020 2063 6f6d 6d61 6e64 203d 2066       command = f
+0001bfd0: 2741 5753 5f53 4841 5245 445f 4352 4544  'AWS_SHARED_CRED
+0001bfe0: 454e 5449 414c 535f 4649 4c45 3d7b 636c  ENTIALS_FILE={cl
+0001bff0: 6f75 6466 6c61 7265 2e52 325f 4352 4544  oudflare.R2_CRED
+0001c000: 454e 5449 414c 535f 5041 5448 7d20 6177  ENTIALS_PATH} aw
+0001c010: 7320 7333 6170 6920 6865 6164 2d62 7563  s s3api head-buc
+0001c020: 6b65 7420 2d2d 6275 636b 6574 207b 6e6f  ket --bucket {no
+0001c030: 6e65 7869 7374 5f62 7563 6b65 745f 6e61  nexist_bucket_na
+0001c040: 6d65 7d20 2d2d 656e 6470 6f69 6e74 207b  me} --endpoint {
+0001c050: 656e 6470 6f69 6e74 5f75 726c 7d20 2d2d  endpoint_url} --
+0001c060: 7072 6f66 696c 653d 7232 270a 2020 2020  profile=r2'.    
+0001c070: 2020 2020 2020 2020 2020 2020 6578 7065              expe
+0001c080: 6374 6564 5f6f 7574 7075 7420 3d20 2734  cted_output = '4
+0001c090: 3034 270a 2020 2020 2020 2020 2020 2020  04'.            
+0001c0a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001c0b0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+0001c0c0: 6545 7272 6f72 2827 556e 7375 7070 6f72  eError('Unsuppor
+0001c0d0: 7465 6420 6275 636b 6574 2074 7970 6520  ted bucket type 
+0001c0e0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+0001c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c100: 2020 2066 277b 6e6f 6e65 7869 7374 5f62     f'{nonexist_b
+0001c110: 7563 6b65 745f 7572 6c7d 2729 0a0a 2020  ucket_url}')..  
+0001c120: 2020 2020 2020 2020 2020 2320 4368 6563            # Chec
+0001c130: 6b20 6966 2062 7563 6b65 7420 6578 6973  k if bucket exis
+0001c140: 7473 2075 7369 6e67 2074 6865 2063 6c69  ts using the cli
+0001c150: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
+0001c160: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+0001c170: 2020 206f 7574 203d 2073 7562 7072 6f63     out = subproc
+0001c180: 6573 732e 6368 6563 6b5f 6f75 7470 7574  ess.check_output
+0001c190: 2863 6f6d 6d61 6e64 2c0a 2020 2020 2020  (command,.      
+0001c1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c1c0: 2020 2020 2020 2020 7374 6465 7272 3d73          stderr=s
+0001c1d0: 7562 7072 6f63 6573 732e 5354 444f 5554  ubprocess.STDOUT
+0001c1e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c210: 2020 2020 2020 2020 2020 2020 2027 746f               'to
-0001c220: 2075 7365 2e20 5468 6973 2069 7320 6869   use. This is hi
-0001c230: 676c 7920 756e 6c69 6b65 6c79 202d 2027  gly unlikely - '
-0001c240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c260: 2020 2020 2020 2020 2763 6865 636b 2069          'check i
-0001c270: 6620 7468 6520 7465 7374 7320 6172 6520  f the tests are 
-0001c280: 636f 7272 6563 742e 2729 0a0a 2020 2020  correct.')..    
-0001c290: 2020 2020 7769 7468 2070 7974 6573 742e      with pytest.
-0001c2a0: 7261 6973 6573 280a 2020 2020 2020 2020  raises(.        
-0001c2b0: 2020 2020 2020 2020 736b 792e 6578 6365          sky.exce
-0001c2c0: 7074 696f 6e73 2e53 746f 7261 6765 4275  ptions.StorageBu
-0001c2d0: 636b 6574 4765 7445 7272 6f72 2c0a 2020  cketGetError,.  
-0001c2e0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-0001c2f0: 7463 683d 2741 7474 656d 7074 6564 2074  tch='Attempted t
-0001c300: 6f20 636f 6e6e 6563 7420 746f 2061 206e  o connect to a n
-0001c310: 6f6e 2d65 7869 7374 656e 7420 6275 636b  on-existent buck
-0001c320: 6574 2729 3a0a 2020 2020 2020 2020 2020  et'):.          
-0001c330: 2020 7374 6f72 6167 655f 6f62 6a20 3d20    storage_obj = 
-0001c340: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
-0001c350: 6167 6528 736f 7572 6365 3d6e 6f6e 6578  age(source=nonex
-0001c360: 6973 745f 6275 636b 6574 5f75 726c 2e66  ist_bucket_url.f
-0001c370: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-0001c380: 2020 2020 2020 2072 616e 646f 6d5f 6e61         random_na
-0001c390: 6d65 3d6e 6f6e 6578 6973 745f 6275 636b  me=nonexist_buck
-0001c3a0: 6574 5f6e 616d 6529 290a 0a20 2020 2040  et_name))..    @
-0001c3b0: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
-0001c3c0: 6d65 7472 697a 6528 2770 7269 7661 7465  metrize('private
-0001c3d0: 5f62 7563 6b65 7427 2c0a 2020 2020 2020  _bucket',.      
-0001c3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c3f0: 2020 2020 2020 205b 6627 7333 3a2f 2f69         [f's3://i
-0001c400: 6d61 6765 6e65 7427 2c20 6627 6773 3a2f  magenet', f'gs:/
-0001c410: 2f69 6d61 6765 6e65 7427 5d29 0a20 2020  /imagenet']).   
-0001c420: 2064 6566 2074 6573 745f 7072 6976 6174   def test_privat
-0001c430: 655f 6275 636b 6574 2873 656c 662c 2070  e_bucket(self, p
-0001c440: 7269 7661 7465 5f62 7563 6b65 7429 3a0a  rivate_bucket):.
-0001c450: 2020 2020 2020 2020 2320 4174 7465 6d70          # Attemp
-0001c460: 7473 2074 6f20 6163 6365 7373 2070 7269  ts to access pri
-0001c470: 7661 7465 2062 7563 6b65 7473 206e 6f74  vate buckets not
-0001c480: 2062 656c 6f6e 6769 6e67 2074 6f20 7468   belonging to th
-0001c490: 6520 7573 6572 2e0a 2020 2020 2020 2020  e user..        
-0001c4a0: 2320 5468 6573 6520 6275 636b 6574 7320  # These buckets 
-0001c4b0: 6172 6520 6b6e 6f77 6e20 746f 2062 6520  are known to be 
-0001c4c0: 7072 6976 6174 652c 2062 7574 206d 6179  private, but may
-0001c4d0: 206e 6565 6420 746f 2062 6520 7570 6461   need to be upda
-0001c4e0: 7465 6420 6966 0a20 2020 2020 2020 2023  ted if.        #
-0001c4f0: 2074 6865 7920 6172 6520 7265 6d6f 7665   they are remove
-0001c500: 6420 6279 2074 6865 6972 206f 776e 6572  d by their owner
-0001c510: 732e 0a20 2020 2020 2020 2070 7269 7661  s..        priva
-0001c520: 7465 5f62 7563 6b65 745f 6e61 6d65 203d  te_bucket_name =
-0001c530: 2075 726c 6c69 622e 7061 7273 652e 7572   urllib.parse.ur
-0001c540: 6c73 706c 6974 2870 7269 7661 7465 5f62  lsplit(private_b
-0001c550: 7563 6b65 7429 2e6e 6574 6c6f 630a 2020  ucket).netloc.  
-0001c560: 2020 2020 2020 7769 7468 2070 7974 6573        with pytes
-0001c570: 742e 7261 6973 6573 280a 2020 2020 2020  t.raises(.      
-0001c580: 2020 2020 2020 2020 2020 736b 792e 6578            sky.ex
-0001c590: 6365 7074 696f 6e73 2e53 746f 7261 6765  ceptions.Storage
-0001c5a0: 4275 636b 6574 4765 7445 7272 6f72 2c0a  BucketGetError,.
-0001c5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c5c0: 6d61 7463 683d 7374 6f72 6167 655f 6c69  match=storage_li
-0001c5d0: 622e 5f42 5543 4b45 545f 4641 494c 5f54  b._BUCKET_FAIL_T
-0001c5e0: 4f5f 434f 4e4e 4543 545f 4d45 5353 4147  O_CONNECT_MESSAG
-0001c5f0: 452e 666f 726d 6174 280a 2020 2020 2020  E.format(.      
-0001c600: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-0001c610: 6d65 3d70 7269 7661 7465 5f62 7563 6b65  me=private_bucke
-0001c620: 745f 6e61 6d65 2929 3a0a 2020 2020 2020  t_name)):.      
-0001c630: 2020 2020 2020 7374 6f72 6167 655f 6f62        storage_ob
-0001c640: 6a20 3d20 7374 6f72 6167 655f 6c69 622e  j = storage_lib.
-0001c650: 5374 6f72 6167 6528 736f 7572 6365 3d70  Storage(source=p
-0001c660: 7269 7661 7465 5f62 7563 6b65 7429 0a0a  rivate_bucket)..
-0001c670: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-0001c680: 2e70 6172 616d 6574 7269 7a65 2827 6578  .parametrize('ex
-0001c690: 745f 6275 636b 6574 5f66 6978 7475 7265  t_bucket_fixture
-0001c6a0: 2c20 7374 6f72 655f 7479 7065 272c 0a20  , store_type',. 
-0001c6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c6c0: 2020 2020 2020 2020 2020 2020 5b28 2774              [('t
-0001c6d0: 6d70 5f61 7773 636c 695f 6275 636b 6574  mp_awscli_bucket
-0001c6e0: 272c 2073 746f 7261 6765 5f6c 6962 2e53  ', storage_lib.S
-0001c6f0: 746f 7265 5479 7065 2e53 3329 2c0a 2020  toreType.S3),.  
-0001c700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c710: 2020 2020 2020 2020 2020 2020 2827 746d              ('tm
-0001c720: 705f 6773 7574 696c 5f62 7563 6b65 7427  p_gsutil_bucket'
-0001c730: 2c20 7374 6f72 6167 655f 6c69 622e 5374  , storage_lib.St
-0001c740: 6f72 6554 7970 652e 4743 5329 2c0a 2020  oreType.GCS),.  
-0001c750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c760: 2020 2020 2020 2020 2020 2020 7079 7465              pyte
-0001c770: 7374 2e70 6172 616d 2827 746d 705f 6177  st.param('tmp_aw
-0001c780: 7363 6c69 5f62 7563 6b65 745f 7232 272c  scli_bucket_r2',
-0001c790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c7b0: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
-0001c7c0: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
-0001c7d0: 652e 5232 2c0a 2020 2020 2020 2020 2020  e.R2,.          
-0001c7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c800: 206d 6172 6b73 3d70 7974 6573 742e 6d61   marks=pytest.ma
-0001c810: 726b 2e63 6c6f 7564 666c 6172 6529 5d29  rk.cloudflare)])
-0001c820: 0a20 2020 2064 6566 2074 6573 745f 7570  .    def test_up
-0001c830: 6c6f 6164 5f74 6f5f 6578 6973 7469 6e67  load_to_existing
-0001c840: 5f62 7563 6b65 7428 7365 6c66 2c20 6578  _bucket(self, ex
-0001c850: 745f 6275 636b 6574 5f66 6978 7475 7265  t_bucket_fixture
-0001c860: 2c20 7265 7175 6573 742c 0a20 2020 2020  , request,.     
-0001c870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c890: 2020 746d 705f 736f 7572 6365 2c20 7374    tmp_source, st
-0001c8a0: 6f72 655f 7479 7065 293a 0a20 2020 2020  ore_type):.     
-0001c8b0: 2020 2023 2054 7269 6573 2075 706c 6f61     # Tries uploa
-0001c8c0: 6469 6e67 2065 7869 7374 696e 6720 6669  ding existing fi
-0001c8d0: 6c65 7320 746f 206e 6577 6c79 2063 7265  les to newly cre
-0001c8e0: 6174 6564 2062 7563 6b65 7420 286f 7574  ated bucket (out
-0001c8f0: 7369 6465 206f 660a 2020 2020 2020 2020  side of.        
-0001c900: 2320 736b 7929 2061 6e64 2076 6572 6966  # sky) and verif
-0001c910: 6965 7320 7468 6174 2066 696c 6573 2061  ies that files a
-0001c920: 7265 2077 7269 7474 656e 2e0a 2020 2020  re written..    
-0001c930: 2020 2020 6275 636b 6574 5f6e 616d 6520      bucket_name 
-0001c940: 3d20 7265 7175 6573 742e 6765 7466 6978  = request.getfix
-0001c950: 7475 7265 7661 6c75 6528 6578 745f 6275  turevalue(ext_bu
-0001c960: 636b 6574 5f66 6978 7475 7265 290a 2020  cket_fixture).  
-0001c970: 2020 2020 2020 7374 6f72 6167 655f 6f62        storage_ob
-0001c980: 6a20 3d20 7374 6f72 6167 655f 6c69 622e  j = storage_lib.
-0001c990: 5374 6f72 6167 6528 6e61 6d65 3d62 7563  Storage(name=buc
-0001c9a0: 6b65 745f 6e61 6d65 2c20 736f 7572 6365  ket_name, source
-0001c9b0: 3d74 6d70 5f73 6f75 7263 6529 0a20 2020  =tmp_source).   
-0001c9c0: 2020 2020 2073 746f 7261 6765 5f6f 626a       storage_obj
-0001c9d0: 2e61 6464 5f73 746f 7265 2873 746f 7265  .add_store(store
-0001c9e0: 5f74 7970 6529 0a0a 2020 2020 2020 2020  _type)..        
-0001c9f0: 2320 4368 6563 6b20 6966 2074 6d70 5f73  # Check if tmp_s
-0001ca00: 6f75 7263 652f 746d 702d 6669 6c65 2065  ource/tmp-file e
-0001ca10: 7869 7374 7320 696e 2074 6865 2062 7563  xists in the buc
-0001ca20: 6b65 7420 7573 696e 6720 6177 7320 636c  ket using aws cl
-0001ca30: 690a 2020 2020 2020 2020 6f75 7420 3d20  i.        out = 
-0001ca40: 7375 6270 726f 6365 7373 2e63 6865 636b  subprocess.check
-0001ca50: 5f6f 7574 7075 7428 7365 6c66 2e63 6c69  _output(self.cli
-0001ca60: 5f6c 735f 636d 6428 7374 6f72 655f 7479  _ls_cmd(store_ty
-0001ca70: 7065 2c20 6275 636b 6574 5f6e 616d 6529  pe, bucket_name)
-0001ca80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001caa0: 2020 2020 2020 2020 7368 656c 6c3d 5472          shell=Tr
-0001cab0: 7565 290a 2020 2020 2020 2020 6173 7365  ue).        asse
-0001cac0: 7274 2027 746d 702d 6669 6c65 2720 696e  rt 'tmp-file' in
-0001cad0: 206f 7574 2e64 6563 6f64 6528 2775 7466   out.decode('utf
-0001cae0: 2d38 2729 2c20 5c0a 2020 2020 2020 2020  -8'), \.        
-0001caf0: 2020 2020 2746 696c 6520 6e6f 7420 666f      'File not fo
-0001cb00: 756e 6420 696e 2062 7563 6b65 7420 2d20  und in bucket - 
-0001cb10: 6f75 7470 7574 2077 6173 203a 207b 7d27  output was : {}'
-0001cb20: 2e66 6f72 6d61 7428 6f75 742e 6465 636f  .format(out.deco
-0001cb30: 6465 0a20 2020 2020 2020 2020 2020 2020  de.             
-0001cb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cb70: 2020 2028 2775 7466 2d38 2729 290a 0a20     ('utf-8')).. 
-0001cb80: 2020 2020 2020 2023 2043 6865 636b 2073         # Check s
-0001cb90: 796d 6c69 6e6b 7320 2d20 7379 6d6c 696e  ymlinks - symlin
-0001cba0: 6b73 2064 6f6e 2774 2067 6574 2063 6f70  ks don't get cop
-0001cbb0: 6965 6420 6279 2073 6b79 2073 746f 7261  ied by sky stora
-0001cbc0: 6765 0a20 2020 2020 2020 2061 7373 6572  ge.        asser
-0001cbd0: 7420 2870 6174 686c 6962 2e50 6174 6828  t (pathlib.Path(
-0001cbe0: 746d 705f 736f 7572 6365 2920 2f20 2763  tmp_source) / 'c
-0001cbf0: 6972 636c 652d 6c69 6e6b 2729 2e69 735f  ircle-link').is_
-0001cc00: 7379 6d6c 696e 6b28 292c 2028 0a20 2020  symlink(), (.   
-0001cc10: 2020 2020 2020 2020 2027 6369 7263 6c65           'circle
-0001cc20: 2d6c 696e 6b20 7761 7320 6e6f 7420 666f  -link was not fo
-0001cc30: 756e 6420 696e 2074 6865 2075 706c 6f61  und in the uploa
-0001cc40: 6420 736f 7572 6365 202d 2027 0a20 2020  d source - '.   
-0001cc50: 2020 2020 2020 2020 2027 6172 6520 7468           'are th
-0001cc60: 6520 7465 7374 2066 6978 7475 7265 7320  e test fixtures 
-0001cc70: 636f 7272 6563 743f 2729 0a20 2020 2020  correct?').     
-0001cc80: 2020 2061 7373 6572 7420 2763 6972 636c     assert 'circl
-0001cc90: 652d 6c69 6e6b 2720 6e6f 7420 696e 206f  e-link' not in o
-0001cca0: 7574 2e64 6563 6f64 6528 2775 7466 2d38  ut.decode('utf-8
-0001ccb0: 2729 2c20 280a 2020 2020 2020 2020 2020  '), (.          
-0001ccc0: 2020 2753 796d 6c69 6e6b 2066 6f75 6e64    'Symlink found
-0001ccd0: 2069 6e20 6275 636b 6574 202d 206c 7320   in bucket - ls 
-0001cce0: 6f75 7470 7574 2077 6173 203a 207b 7d27  output was : {}'
-0001ccf0: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-0001cd00: 2020 2020 2020 2020 206f 7574 2e64 6563           out.dec
-0001cd10: 6f64 6528 2775 7466 2d38 2729 2929 0a0a  ode('utf-8')))..
-0001cd20: 2020 2020 2020 2020 2320 5275 6e20 736b          # Run sk
-0001cd30: 7920 7374 6f72 6167 6520 6c73 2074 6f20  y storage ls to 
-0001cd40: 6368 6563 6b20 6966 2073 746f 7261 6765  check if storage
-0001cd50: 206f 626a 6563 7420 6578 6973 7473 2069   object exists i
-0001cd60: 6e20 7468 6520 6f75 7470 7574 2e0a 2020  n the output..  
-0001cd70: 2020 2020 2020 2320 4974 2073 686f 756c        # It shoul
-0001cd80: 6420 6e6f 7420 6578 6973 7420 6265 6361  d not exist beca
-0001cd90: 7573 6520 7468 6520 6275 636b 6574 2077  use the bucket w
-0001cda0: 6173 2063 7265 6174 6564 2065 7874 6572  as created exter
-0001cdb0: 6e61 6c6c 792e 0a20 2020 2020 2020 206f  nally..        o
-0001cdc0: 7574 203d 2073 7562 7072 6f63 6573 732e  ut = subprocess.
-0001cdd0: 6368 6563 6b5f 6f75 7470 7574 285b 2773  check_output(['s
-0001cde0: 6b79 272c 2027 7374 6f72 6167 6527 2c20  ky', 'storage', 
-0001cdf0: 276c 7327 5d29 0a20 2020 2020 2020 2061  'ls']).        a
-0001ce00: 7373 6572 7420 7374 6f72 6167 655f 6f62  ssert storage_ob
-0001ce10: 6a2e 6e61 6d65 206e 6f74 2069 6e20 6f75  j.name not in ou
-0001ce20: 742e 6465 636f 6465 2827 7574 662d 3827  t.decode('utf-8'
-0001ce30: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-0001ce40: 636f 7079 5f6d 6f75 6e74 5f65 7869 7374  copy_mount_exist
-0001ce50: 696e 675f 7374 6f72 6167 6528 7365 6c66  ing_storage(self
-0001ce60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001ce70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ce80: 2020 2020 2020 2020 2020 2074 6d70 5f63             tmp_c
-0001ce90: 6f70 795f 6d6e 745f 6578 6973 7469 6e67  opy_mnt_existing
-0001cea0: 5f73 746f 7261 6765 5f6f 626a 293a 0a20  _storage_obj):. 
-0001ceb0: 2020 2020 2020 2023 2043 7265 6174 6573         # Creates
-0001cec0: 2061 2062 7563 6b65 7420 7769 7468 206e   a bucket with n
-0001ced0: 6f20 736f 7572 6365 2069 6e20 4d4f 554e  o source in MOUN
-0001cee0: 5420 6d6f 6465 2028 656d 7074 7920 6275  T mode (empty bu
-0001cef0: 636b 6574 292c 2061 6e64 0a20 2020 2020  cket), and.     
-0001cf00: 2020 2023 2074 6865 6e20 7472 6965 7320     # then tries 
-0001cf10: 746f 206c 6f61 6420 7468 6520 7361 6d65  to load the same
-0001cf20: 2073 746f 7261 6765 2069 6e20 434f 5059   storage in COPY
-0001cf30: 206d 6f64 652e 0a20 2020 2020 2020 2074   mode..        t
-0001cf40: 6d70 5f63 6f70 795f 6d6e 745f 6578 6973  mp_copy_mnt_exis
-0001cf50: 7469 6e67 5f73 746f 7261 6765 5f6f 626a  ting_storage_obj
-0001cf60: 2e61 6464 5f73 746f 7265 2873 746f 7261  .add_store(stora
-0001cf70: 6765 5f6c 6962 2e53 746f 7265 5479 7065  ge_lib.StoreType
-0001cf80: 2e53 3329 0a20 2020 2020 2020 2073 746f  .S3).        sto
-0001cf90: 7261 6765 5f6e 616d 6520 3d20 746d 705f  rage_name = tmp_
-0001cfa0: 636f 7079 5f6d 6e74 5f65 7869 7374 696e  copy_mnt_existin
-0001cfb0: 675f 7374 6f72 6167 655f 6f62 6a2e 6e61  g_storage_obj.na
-0001cfc0: 6d65 0a0a 2020 2020 2020 2020 2320 4368  me..        # Ch
-0001cfd0: 6563 6b20 6073 6b79 2073 746f 7261 6765  eck `sky storage
-0001cfe0: 206c 7360 2074 6f20 656e 7375 7265 2073   ls` to ensure s
-0001cff0: 746f 7261 6765 206f 626a 6563 7420 6578  torage object ex
-0001d000: 6973 7473 0a20 2020 2020 2020 206f 7574  ists.        out
-0001d010: 203d 2073 7562 7072 6f63 6573 732e 6368   = subprocess.ch
-0001d020: 6563 6b5f 6f75 7470 7574 285b 2773 6b79  eck_output(['sky
-0001d030: 272c 2027 7374 6f72 6167 6527 2c20 276c  ', 'storage', 'l
-0001d040: 7327 5d29 2e64 6563 6f64 6528 2775 7466  s']).decode('utf
-0001d050: 2d38 2729 0a20 2020 2020 2020 2061 7373  -8').        ass
-0001d060: 6572 7420 7374 6f72 6167 655f 6e61 6d65  ert storage_name
-0001d070: 2069 6e20 6f75 742c 2066 2753 746f 7261   in out, f'Stora
-0001d080: 6765 207b 7374 6f72 6167 655f 6e61 6d65  ge {storage_name
-0001d090: 7d20 6e6f 7420 666f 756e 6420 696e 2073  } not found in s
-0001d0a0: 6b79 2073 746f 7261 6765 206c 732e 270a  ky storage ls.'.
-0001d0b0: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
-0001d0c0: 6b2e 7061 7261 6d65 7472 697a 6528 2773  k.parametrize('s
-0001d0d0: 746f 7265 5f74 7970 6527 2c20 5b0a 2020  tore_type', [.  
-0001d0e0: 2020 2020 2020 7374 6f72 6167 655f 6c69        storage_li
-0001d0f0: 622e 5374 6f72 6554 7970 652e 5333 2c20  b.StoreType.S3, 
-0001d100: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
-0001d110: 6554 7970 652e 4743 532c 0a20 2020 2020  eType.GCS,.     
-0001d120: 2020 2070 7974 6573 742e 7061 7261 6d28     pytest.param(
-0001d130: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
-0001d140: 6554 7970 652e 5232 2c20 6d61 726b 733d  eType.R2, marks=
-0001d150: 7079 7465 7374 2e6d 6172 6b2e 636c 6f75  pytest.mark.clou
-0001d160: 6466 6c61 7265 290a 2020 2020 5d29 0a20  dflare).    ]). 
-0001d170: 2020 2064 6566 2074 6573 745f 6c69 7374     def test_list
-0001d180: 5f73 6f75 7263 6528 7365 6c66 2c20 746d  _source(self, tm
-0001d190: 705f 6c6f 6361 6c5f 6c69 7374 5f73 746f  p_local_list_sto
-0001d1a0: 7261 6765 5f6f 626a 2c20 7374 6f72 655f  rage_obj, store_
-0001d1b0: 7479 7065 293a 0a20 2020 2020 2020 2023  type):.        #
-0001d1c0: 2055 7365 7320 6120 6c69 7374 2069 6e20   Uses a list in 
-0001d1d0: 7468 6520 736f 7572 6365 2066 6965 6c64  the source field
-0001d1e0: 2074 6f20 7370 6563 6966 7920 6120 6669   to specify a fi
-0001d1f0: 6c65 2061 6e64 2061 2064 6972 6563 746f  le and a directo
-0001d200: 7279 2074 6f0a 2020 2020 2020 2020 2320  ry to.        # 
-0001d210: 6265 2075 706c 6f61 6465 6420 746f 2074  be uploaded to t
-0001d220: 6865 2073 746f 7261 6765 206f 626a 6563  he storage objec
-0001d230: 742e 0a20 2020 2020 2020 2074 6d70 5f6c  t..        tmp_l
-0001d240: 6f63 616c 5f6c 6973 745f 7374 6f72 6167  ocal_list_storag
-0001d250: 655f 6f62 6a2e 6164 645f 7374 6f72 6528  e_obj.add_store(
-0001d260: 7374 6f72 655f 7479 7065 290a 0a20 2020  store_type)..   
-0001d270: 2020 2020 2023 2043 6865 636b 2069 6620       # Check if 
-0001d280: 746d 702d 6669 6c65 2065 7869 7374 7320  tmp-file exists 
-0001d290: 696e 2074 6865 2062 7563 6b65 7420 726f  in the bucket ro
-0001d2a0: 6f74 2075 7369 6e67 2063 6c69 0a20 2020  ot using cli.   
-0001d2b0: 2020 2020 206f 7574 203d 2073 7562 7072       out = subpr
-0001d2c0: 6f63 6573 732e 6368 6563 6b5f 6f75 7470  ocess.check_outp
-0001d2d0: 7574 2873 656c 662e 636c 695f 6c73 5f63  ut(self.cli_ls_c
-0001d2e0: 6d64 280a 2020 2020 2020 2020 2020 2020  md(.            
-0001d2f0: 7374 6f72 655f 7479 7065 2c20 746d 705f  store_type, tmp_
-0001d300: 6c6f 6361 6c5f 6c69 7374 5f73 746f 7261  local_list_stora
-0001d310: 6765 5f6f 626a 2e6e 616d 6529 2c0a 2020  ge_obj.name),.  
-0001d320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d340: 2020 2020 7368 656c 6c3d 5472 7565 290a      shell=True).
-0001d350: 2020 2020 2020 2020 6173 7365 7274 2027          assert '
-0001d360: 746d 702d 6669 6c65 2720 696e 206f 7574  tmp-file' in out
-0001d370: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
-0001d380: 2c20 5c0a 2020 2020 2020 2020 2020 2020  , \.            
-0001d390: 2746 696c 6520 6e6f 7420 666f 756e 6420  'File not found 
-0001d3a0: 696e 2062 7563 6b65 7420 2d20 6f75 7470  in bucket - outp
-0001d3b0: 7574 2077 6173 203a 207b 7d27 2e66 6f72  ut was : {}'.for
-0001d3c0: 6d61 7428 6f75 742e 6465 636f 6465 0a20  mat(out.decode. 
-0001d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d400: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-0001d410: 2775 7466 2d38 2729 290a 0a20 2020 2020  'utf-8'))..     
-0001d420: 2020 2023 2043 6865 636b 2069 6620 746d     # Check if tm
-0001d430: 702d 6669 6c65 2065 7869 7374 7320 696e  p-file exists in
-0001d440: 2074 6865 2062 7563 6b65 742f 746d 702d   the bucket/tmp-
-0001d450: 736f 7572 6365 2075 7369 6e67 2063 6c69  source using cli
-0001d460: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
-0001d470: 7562 7072 6f63 6573 732e 6368 6563 6b5f  ubprocess.check_
-0001d480: 6f75 7470 7574 2873 656c 662e 636c 695f  output(self.cli_
-0001d490: 6c73 5f63 6d64 280a 2020 2020 2020 2020  ls_cmd(.        
-0001d4a0: 2020 2020 7374 6f72 655f 7479 7065 2c20      store_type, 
-0001d4b0: 746d 705f 6c6f 6361 6c5f 6c69 7374 5f73  tmp_local_list_s
-0001d4c0: 746f 7261 6765 5f6f 626a 2e6e 616d 652c  torage_obj.name,
-0001d4d0: 2027 746d 702d 736f 7572 6365 2f27 292c   'tmp-source/'),
-0001d4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d500: 2020 2020 2020 2073 6865 6c6c 3d54 7275         shell=Tru
-0001d510: 6529 0a20 2020 2020 2020 2061 7373 6572  e).        asser
-0001d520: 7420 2774 6d70 2d66 696c 6527 2069 6e20  t 'tmp-file' in 
-0001d530: 6f75 742e 6465 636f 6465 2827 7574 662d  out.decode('utf-
-0001d540: 3827 292c 205c 0a20 2020 2020 2020 2020  8'), \.         
-0001d550: 2020 2027 4669 6c65 206e 6f74 2066 6f75     'File not fou
-0001d560: 6e64 2069 6e20 6275 636b 6574 202d 206f  nd in bucket - o
-0001d570: 7574 7075 7420 7761 7320 3a20 7b7d 272e  utput was : {}'.
-0001d580: 666f 726d 6174 286f 7574 2e64 6563 6f64  format(out.decod
-0001d590: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0001d5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d5d0: 2020 2827 7574 662d 3827 2929 0a0a 2020    ('utf-8'))..  
-0001d5e0: 2020 4070 7974 6573 742e 6d61 726b 2e70    @pytest.mark.p
-0001d5f0: 6172 616d 6574 7269 7a65 2827 696e 7661  arametrize('inva
-0001d600: 6c69 645f 6e61 6d65 5f6c 6973 742c 2073  lid_name_list, s
-0001d610: 746f 7265 5f74 7970 6527 2c0a 2020 2020  tore_type',.    
-0001d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d630: 2020 2020 2020 2020 205b 2841 5753 5f49           [(AWS_I
-0001d640: 4e56 414c 4944 5f4e 414d 4553 2c20 7374  NVALID_NAMES, st
-0001d650: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
-0001d660: 7970 652e 5333 292c 0a20 2020 2020 2020  ype.S3),.       
+0001c210: 7368 656c 6c3d 5472 7565 290a 2020 2020  shell=True).    
+0001c220: 2020 2020 2020 2020 6578 6365 7074 2073          except s
+0001c230: 7562 7072 6f63 6573 732e 4361 6c6c 6564  ubprocess.Called
+0001c240: 5072 6f63 6573 7345 7272 6f72 2061 7320  ProcessError as 
+0001c250: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001c260: 2020 206f 7574 203d 2065 2e6f 7574 7075     out = e.outpu
+0001c270: 740a 2020 2020 2020 2020 2020 2020 6f75  t.            ou
+0001c280: 7420 3d20 6f75 742e 6465 636f 6465 2827  t = out.decode('
+0001c290: 7574 662d 3827 290a 2020 2020 2020 2020  utf-8').        
+0001c2a0: 2020 2020 6966 2065 7870 6563 7465 645f      if expected_
+0001c2b0: 6f75 7470 7574 2069 6e20 6f75 743a 0a20  output in out:. 
+0001c2c0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0001c2d0: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
+0001c2e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0001c2f0: 2020 2020 2020 2072 6574 7279 5f63 6f75         retry_cou
+0001c300: 6e74 202b 3d20 310a 2020 2020 2020 2020  nt += 1.        
+0001c310: 2020 2020 2020 2020 6966 2072 6574 7279          if retry
+0001c320: 5f63 6f75 6e74 203e 2033 3a0a 2020 2020  _count > 3:.    
+0001c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c340: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
+0001c350: 6f72 2827 556e 6162 6c65 2074 6f20 6669  or('Unable to fi
+0001c360: 6e64 2061 206e 6f6e 6578 6973 7465 6e74  nd a nonexistent
+0001c370: 2062 7563 6b65 7420 270a 2020 2020 2020   bucket '.      
+0001c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c3a0: 2027 746f 2075 7365 2e20 5468 6973 2069   'to use. This i
+0001c3b0: 7320 6869 676c 7920 756e 6c69 6b65 6c79  s higly unlikely
+0001c3c0: 202d 2027 0a20 2020 2020 2020 2020 2020   - '.           
+0001c3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c3e0: 2020 2020 2020 2020 2020 2020 2763 6865              'che
+0001c3f0: 636b 2069 6620 7468 6520 7465 7374 7320  ck if the tests 
+0001c400: 6172 6520 636f 7272 6563 742e 2729 0a0a  are correct.')..
+0001c410: 2020 2020 2020 2020 7769 7468 2070 7974          with pyt
+0001c420: 6573 742e 7261 6973 6573 280a 2020 2020  est.raises(.    
+0001c430: 2020 2020 2020 2020 2020 2020 736b 792e              sky.
+0001c440: 6578 6365 7074 696f 6e73 2e53 746f 7261  exceptions.Stora
+0001c450: 6765 4275 636b 6574 4765 7445 7272 6f72  geBucketGetError
+0001c460: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001c470: 2020 6d61 7463 683d 2741 7474 656d 7074    match='Attempt
+0001c480: 6564 2074 6f20 636f 6e6e 6563 7420 746f  ed to connect to
+0001c490: 2061 206e 6f6e 2d65 7869 7374 656e 7420   a non-existent 
+0001c4a0: 6275 636b 6574 2729 3a0a 2020 2020 2020  bucket'):.      
+0001c4b0: 2020 2020 2020 7374 6f72 6167 655f 6f62        storage_ob
+0001c4c0: 6a20 3d20 7374 6f72 6167 655f 6c69 622e  j = storage_lib.
+0001c4d0: 5374 6f72 6167 6528 736f 7572 6365 3d6e  Storage(source=n
+0001c4e0: 6f6e 6578 6973 745f 6275 636b 6574 5f75  onexist_bucket_u
+0001c4f0: 726c 2e66 6f72 6d61 7428 0a20 2020 2020  rl.format(.     
+0001c500: 2020 2020 2020 2020 2020 2072 616e 646f             rando
+0001c510: 6d5f 6e61 6d65 3d6e 6f6e 6578 6973 745f  m_name=nonexist_
+0001c520: 6275 636b 6574 5f6e 616d 6529 290a 0a20  bucket_name)).. 
+0001c530: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+0001c540: 7061 7261 6d65 7472 697a 6528 2770 7269  parametrize('pri
+0001c550: 7661 7465 5f62 7563 6b65 7427 2c0a 2020  vate_bucket',.  
+0001c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c570: 2020 2020 2020 2020 2020 205b 6627 7333             [f's3
+0001c580: 3a2f 2f69 6d61 6765 6e65 7427 2c20 6627  ://imagenet', f'
+0001c590: 6773 3a2f 2f69 6d61 6765 6e65 7427 5d29  gs://imagenet'])
+0001c5a0: 0a20 2020 2064 6566 2074 6573 745f 7072  .    def test_pr
+0001c5b0: 6976 6174 655f 6275 636b 6574 2873 656c  ivate_bucket(sel
+0001c5c0: 662c 2070 7269 7661 7465 5f62 7563 6b65  f, private_bucke
+0001c5d0: 7429 3a0a 2020 2020 2020 2020 2320 4174  t):.        # At
+0001c5e0: 7465 6d70 7473 2074 6f20 6163 6365 7373  tempts to access
+0001c5f0: 2070 7269 7661 7465 2062 7563 6b65 7473   private buckets
+0001c600: 206e 6f74 2062 656c 6f6e 6769 6e67 2074   not belonging t
+0001c610: 6f20 7468 6520 7573 6572 2e0a 2020 2020  o the user..    
+0001c620: 2020 2020 2320 5468 6573 6520 6275 636b      # These buck
+0001c630: 6574 7320 6172 6520 6b6e 6f77 6e20 746f  ets are known to
+0001c640: 2062 6520 7072 6976 6174 652c 2062 7574   be private, but
+0001c650: 206d 6179 206e 6565 6420 746f 2062 6520   may need to be 
+0001c660: 7570 6461 7465 6420 6966 0a20 2020 2020  updated if.     
+0001c670: 2020 2023 2074 6865 7920 6172 6520 7265     # they are re
+0001c680: 6d6f 7665 6420 6279 2074 6865 6972 206f  moved by their o
+0001c690: 776e 6572 732e 0a20 2020 2020 2020 2070  wners..        p
+0001c6a0: 7269 7661 7465 5f62 7563 6b65 745f 6e61  rivate_bucket_na
+0001c6b0: 6d65 203d 2075 726c 6c69 622e 7061 7273  me = urllib.pars
+0001c6c0: 652e 7572 6c73 706c 6974 2870 7269 7661  e.urlsplit(priva
+0001c6d0: 7465 5f62 7563 6b65 7429 2e6e 6574 6c6f  te_bucket).netlo
+0001c6e0: 630a 2020 2020 2020 2020 7769 7468 2070  c.        with p
+0001c6f0: 7974 6573 742e 7261 6973 6573 280a 2020  ytest.raises(.  
+0001c700: 2020 2020 2020 2020 2020 2020 2020 736b                sk
+0001c710: 792e 6578 6365 7074 696f 6e73 2e53 746f  y.exceptions.Sto
+0001c720: 7261 6765 4275 636b 6574 4765 7445 7272  rageBucketGetErr
+0001c730: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
+0001c740: 2020 2020 6d61 7463 683d 7374 6f72 6167      match=storag
+0001c750: 655f 6c69 622e 5f42 5543 4b45 545f 4641  e_lib._BUCKET_FA
+0001c760: 494c 5f54 4f5f 434f 4e4e 4543 545f 4d45  IL_TO_CONNECT_ME
+0001c770: 5353 4147 452e 666f 726d 6174 280a 2020  SSAGE.format(.  
+0001c780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c790: 2020 6e61 6d65 3d70 7269 7661 7465 5f62    name=private_b
+0001c7a0: 7563 6b65 745f 6e61 6d65 2929 3a0a 2020  ucket_name)):.  
+0001c7b0: 2020 2020 2020 2020 2020 7374 6f72 6167            storag
+0001c7c0: 655f 6f62 6a20 3d20 7374 6f72 6167 655f  e_obj = storage_
+0001c7d0: 6c69 622e 5374 6f72 6167 6528 736f 7572  lib.Storage(sour
+0001c7e0: 6365 3d70 7269 7661 7465 5f62 7563 6b65  ce=private_bucke
+0001c7f0: 7429 0a0a 2020 2020 4070 7974 6573 742e  t)..    @pytest.
+0001c800: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
+0001c810: 2827 6578 745f 6275 636b 6574 5f66 6978  ('ext_bucket_fix
+0001c820: 7475 7265 2c20 7374 6f72 655f 7479 7065  ture, store_type
+0001c830: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+0001c840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c850: 5b28 2774 6d70 5f61 7773 636c 695f 6275  [('tmp_awscli_bu
+0001c860: 636b 6574 272c 2073 746f 7261 6765 5f6c  cket', storage_l
+0001c870: 6962 2e53 746f 7265 5479 7065 2e53 3329  ib.StoreType.S3)
+0001c880: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001c890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c8a0: 2827 746d 705f 6773 7574 696c 5f62 7563  ('tmp_gsutil_buc
+0001c8b0: 6b65 7427 2c20 7374 6f72 6167 655f 6c69  ket', storage_li
+0001c8c0: 622e 5374 6f72 6554 7970 652e 4743 5329  b.StoreType.GCS)
+0001c8d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001c8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c8f0: 7079 7465 7374 2e70 6172 616d 2827 746d  pytest.param('tm
+0001c900: 705f 6177 7363 6c69 5f62 7563 6b65 745f  p_awscli_bucket_
+0001c910: 7232 272c 0a20 2020 2020 2020 2020 2020  r2',.           
+0001c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c940: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
+0001c950: 6554 7970 652e 5232 2c0a 2020 2020 2020  eType.R2,.      
+0001c960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c980: 2020 2020 206d 6172 6b73 3d70 7974 6573       marks=pytes
+0001c990: 742e 6d61 726b 2e63 6c6f 7564 666c 6172  t.mark.cloudflar
+0001c9a0: 6529 5d29 0a20 2020 2064 6566 2074 6573  e)]).    def tes
+0001c9b0: 745f 7570 6c6f 6164 5f74 6f5f 6578 6973  t_upload_to_exis
+0001c9c0: 7469 6e67 5f62 7563 6b65 7428 7365 6c66  ting_bucket(self
+0001c9d0: 2c20 6578 745f 6275 636b 6574 5f66 6978  , ext_bucket_fix
+0001c9e0: 7475 7265 2c20 7265 7175 6573 742c 0a20  ture, request,. 
+0001c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ca00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ca10: 2020 2020 2020 746d 705f 736f 7572 6365        tmp_source
+0001ca20: 2c20 7374 6f72 655f 7479 7065 293a 0a20  , store_type):. 
+0001ca30: 2020 2020 2020 2023 2054 7269 6573 2075         # Tries u
+0001ca40: 706c 6f61 6469 6e67 2065 7869 7374 696e  ploading existin
+0001ca50: 6720 6669 6c65 7320 746f 206e 6577 6c79  g files to newly
+0001ca60: 2063 7265 6174 6564 2062 7563 6b65 7420   created bucket 
+0001ca70: 286f 7574 7369 6465 206f 660a 2020 2020  (outside of.    
+0001ca80: 2020 2020 2320 736b 7929 2061 6e64 2076      # sky) and v
+0001ca90: 6572 6966 6965 7320 7468 6174 2066 696c  erifies that fil
+0001caa0: 6573 2061 7265 2077 7269 7474 656e 2e0a  es are written..
+0001cab0: 2020 2020 2020 2020 6275 636b 6574 5f6e          bucket_n
+0001cac0: 616d 6520 3d20 7265 7175 6573 742e 6765  ame = request.ge
+0001cad0: 7466 6978 7475 7265 7661 6c75 6528 6578  tfixturevalue(ex
+0001cae0: 745f 6275 636b 6574 5f66 6978 7475 7265  t_bucket_fixture
+0001caf0: 290a 2020 2020 2020 2020 7374 6f72 6167  ).        storag
+0001cb00: 655f 6f62 6a20 3d20 7374 6f72 6167 655f  e_obj = storage_
+0001cb10: 6c69 622e 5374 6f72 6167 6528 6e61 6d65  lib.Storage(name
+0001cb20: 3d62 7563 6b65 745f 6e61 6d65 2c20 736f  =bucket_name, so
+0001cb30: 7572 6365 3d74 6d70 5f73 6f75 7263 6529  urce=tmp_source)
+0001cb40: 0a20 2020 2020 2020 2073 746f 7261 6765  .        storage
+0001cb50: 5f6f 626a 2e61 6464 5f73 746f 7265 2873  _obj.add_store(s
+0001cb60: 746f 7265 5f74 7970 6529 0a0a 2020 2020  tore_type)..    
+0001cb70: 2020 2020 2320 4368 6563 6b20 6966 2074      # Check if t
+0001cb80: 6d70 5f73 6f75 7263 652f 746d 702d 6669  mp_source/tmp-fi
+0001cb90: 6c65 2065 7869 7374 7320 696e 2074 6865  le exists in the
+0001cba0: 2062 7563 6b65 7420 7573 696e 6720 6177   bucket using aw
+0001cbb0: 7320 636c 690a 2020 2020 2020 2020 6f75  s cli.        ou
+0001cbc0: 7420 3d20 7375 6270 726f 6365 7373 2e63  t = subprocess.c
+0001cbd0: 6865 636b 5f6f 7574 7075 7428 7365 6c66  heck_output(self
+0001cbe0: 2e63 6c69 5f6c 735f 636d 6428 7374 6f72  .cli_ls_cmd(stor
+0001cbf0: 655f 7479 7065 2c20 6275 636b 6574 5f6e  e_type, bucket_n
+0001cc00: 616d 6529 2c0a 2020 2020 2020 2020 2020  ame),.          
+0001cc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cc20: 2020 2020 2020 2020 2020 2020 7368 656c              shel
+0001cc30: 6c3d 5472 7565 290a 2020 2020 2020 2020  l=True).        
+0001cc40: 6173 7365 7274 2027 746d 702d 6669 6c65  assert 'tmp-file
+0001cc50: 2720 696e 206f 7574 2e64 6563 6f64 6528  ' in out.decode(
+0001cc60: 2775 7466 2d38 2729 2c20 5c0a 2020 2020  'utf-8'), \.    
+0001cc70: 2020 2020 2020 2020 2746 696c 6520 6e6f          'File no
+0001cc80: 7420 666f 756e 6420 696e 2062 7563 6b65  t found in bucke
+0001cc90: 7420 2d20 6f75 7470 7574 2077 6173 203a  t - output was :
+0001cca0: 207b 7d27 2e66 6f72 6d61 7428 6f75 742e   {}'.format(out.
+0001ccb0: 6465 636f 6465 0a20 2020 2020 2020 2020  decode.         
+0001ccc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ccf0: 2020 2020 2020 2028 2775 7466 2d38 2729         ('utf-8')
+0001cd00: 290a 0a20 2020 2020 2020 2023 2043 6865  )..        # Che
+0001cd10: 636b 2073 796d 6c69 6e6b 7320 2d20 7379  ck symlinks - sy
+0001cd20: 6d6c 696e 6b73 2064 6f6e 2774 2067 6574  mlinks don't get
+0001cd30: 2063 6f70 6965 6420 6279 2073 6b79 2073   copied by sky s
+0001cd40: 746f 7261 6765 0a20 2020 2020 2020 2061  torage.        a
+0001cd50: 7373 6572 7420 2870 6174 686c 6962 2e50  ssert (pathlib.P
+0001cd60: 6174 6828 746d 705f 736f 7572 6365 2920  ath(tmp_source) 
+0001cd70: 2f20 2763 6972 636c 652d 6c69 6e6b 2729  / 'circle-link')
+0001cd80: 2e69 735f 7379 6d6c 696e 6b28 292c 2028  .is_symlink(), (
+0001cd90: 0a20 2020 2020 2020 2020 2020 2027 6369  .            'ci
+0001cda0: 7263 6c65 2d6c 696e 6b20 7761 7320 6e6f  rcle-link was no
+0001cdb0: 7420 666f 756e 6420 696e 2074 6865 2075  t found in the u
+0001cdc0: 706c 6f61 6420 736f 7572 6365 202d 2027  pload source - '
+0001cdd0: 0a20 2020 2020 2020 2020 2020 2027 6172  .            'ar
+0001cde0: 6520 7468 6520 7465 7374 2066 6978 7475  e the test fixtu
+0001cdf0: 7265 7320 636f 7272 6563 743f 2729 0a20  res correct?'). 
+0001ce00: 2020 2020 2020 2061 7373 6572 7420 2763         assert 'c
+0001ce10: 6972 636c 652d 6c69 6e6b 2720 6e6f 7420  ircle-link' not 
+0001ce20: 696e 206f 7574 2e64 6563 6f64 6528 2775  in out.decode('u
+0001ce30: 7466 2d38 2729 2c20 280a 2020 2020 2020  tf-8'), (.      
+0001ce40: 2020 2020 2020 2753 796d 6c69 6e6b 2066        'Symlink f
+0001ce50: 6f75 6e64 2069 6e20 6275 636b 6574 202d  ound in bucket -
+0001ce60: 206c 7320 6f75 7470 7574 2077 6173 203a   ls output was :
+0001ce70: 207b 7d27 2e66 6f72 6d61 7428 0a20 2020   {}'.format(.   
+0001ce80: 2020 2020 2020 2020 2020 2020 206f 7574               out
+0001ce90: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
+0001cea0: 2929 0a0a 2020 2020 2020 2020 2320 5275  ))..        # Ru
+0001ceb0: 6e20 736b 7920 7374 6f72 6167 6520 6c73  n sky storage ls
+0001cec0: 2074 6f20 6368 6563 6b20 6966 2073 746f   to check if sto
+0001ced0: 7261 6765 206f 626a 6563 7420 6578 6973  rage object exis
+0001cee0: 7473 2069 6e20 7468 6520 6f75 7470 7574  ts in the output
+0001cef0: 2e0a 2020 2020 2020 2020 2320 4974 2073  ..        # It s
+0001cf00: 686f 756c 6420 6e6f 7420 6578 6973 7420  hould not exist 
+0001cf10: 6265 6361 7573 6520 7468 6520 6275 636b  because the buck
+0001cf20: 6574 2077 6173 2063 7265 6174 6564 2065  et was created e
+0001cf30: 7874 6572 6e61 6c6c 792e 0a20 2020 2020  xternally..     
+0001cf40: 2020 206f 7574 203d 2073 7562 7072 6f63     out = subproc
+0001cf50: 6573 732e 6368 6563 6b5f 6f75 7470 7574  ess.check_output
+0001cf60: 285b 2773 6b79 272c 2027 7374 6f72 6167  (['sky', 'storag
+0001cf70: 6527 2c20 276c 7327 5d29 0a20 2020 2020  e', 'ls']).     
+0001cf80: 2020 2061 7373 6572 7420 7374 6f72 6167     assert storag
+0001cf90: 655f 6f62 6a2e 6e61 6d65 206e 6f74 2069  e_obj.name not i
+0001cfa0: 6e20 6f75 742e 6465 636f 6465 2827 7574  n out.decode('ut
+0001cfb0: 662d 3827 290a 0a20 2020 2064 6566 2074  f-8')..    def t
+0001cfc0: 6573 745f 636f 7079 5f6d 6f75 6e74 5f65  est_copy_mount_e
+0001cfd0: 7869 7374 696e 675f 7374 6f72 6167 6528  xisting_storage(
+0001cfe0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+0001cff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d000: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0001d010: 6d70 5f63 6f70 795f 6d6e 745f 6578 6973  mp_copy_mnt_exis
+0001d020: 7469 6e67 5f73 746f 7261 6765 5f6f 626a  ting_storage_obj
+0001d030: 293a 0a20 2020 2020 2020 2023 2043 7265  ):.        # Cre
+0001d040: 6174 6573 2061 2062 7563 6b65 7420 7769  ates a bucket wi
+0001d050: 7468 206e 6f20 736f 7572 6365 2069 6e20  th no source in 
+0001d060: 4d4f 554e 5420 6d6f 6465 2028 656d 7074  MOUNT mode (empt
+0001d070: 7920 6275 636b 6574 292c 2061 6e64 0a20  y bucket), and. 
+0001d080: 2020 2020 2020 2023 2074 6865 6e20 7472         # then tr
+0001d090: 6965 7320 746f 206c 6f61 6420 7468 6520  ies to load the 
+0001d0a0: 7361 6d65 2073 746f 7261 6765 2069 6e20  same storage in 
+0001d0b0: 434f 5059 206d 6f64 652e 0a20 2020 2020  COPY mode..     
+0001d0c0: 2020 2074 6d70 5f63 6f70 795f 6d6e 745f     tmp_copy_mnt_
+0001d0d0: 6578 6973 7469 6e67 5f73 746f 7261 6765  existing_storage
+0001d0e0: 5f6f 626a 2e61 6464 5f73 746f 7265 2873  _obj.add_store(s
+0001d0f0: 746f 7261 6765 5f6c 6962 2e53 746f 7265  torage_lib.Store
+0001d100: 5479 7065 2e53 3329 0a20 2020 2020 2020  Type.S3).       
+0001d110: 2073 746f 7261 6765 5f6e 616d 6520 3d20   storage_name = 
+0001d120: 746d 705f 636f 7079 5f6d 6e74 5f65 7869  tmp_copy_mnt_exi
+0001d130: 7374 696e 675f 7374 6f72 6167 655f 6f62  sting_storage_ob
+0001d140: 6a2e 6e61 6d65 0a0a 2020 2020 2020 2020  j.name..        
+0001d150: 2320 4368 6563 6b20 6073 6b79 2073 746f  # Check `sky sto
+0001d160: 7261 6765 206c 7360 2074 6f20 656e 7375  rage ls` to ensu
+0001d170: 7265 2073 746f 7261 6765 206f 626a 6563  re storage objec
+0001d180: 7420 6578 6973 7473 0a20 2020 2020 2020  t exists.       
+0001d190: 206f 7574 203d 2073 7562 7072 6f63 6573   out = subproces
+0001d1a0: 732e 6368 6563 6b5f 6f75 7470 7574 285b  s.check_output([
+0001d1b0: 2773 6b79 272c 2027 7374 6f72 6167 6527  'sky', 'storage'
+0001d1c0: 2c20 276c 7327 5d29 2e64 6563 6f64 6528  , 'ls']).decode(
+0001d1d0: 2775 7466 2d38 2729 0a20 2020 2020 2020  'utf-8').       
+0001d1e0: 2061 7373 6572 7420 7374 6f72 6167 655f   assert storage_
+0001d1f0: 6e61 6d65 2069 6e20 6f75 742c 2066 2753  name in out, f'S
+0001d200: 746f 7261 6765 207b 7374 6f72 6167 655f  torage {storage_
+0001d210: 6e61 6d65 7d20 6e6f 7420 666f 756e 6420  name} not found 
+0001d220: 696e 2073 6b79 2073 746f 7261 6765 206c  in sky storage l
+0001d230: 732e 270a 0a20 2020 2040 7079 7465 7374  s.'..    @pytest
+0001d240: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
+0001d250: 6528 2773 746f 7265 5f74 7970 6527 2c20  e('store_type', 
+0001d260: 5b0a 2020 2020 2020 2020 7374 6f72 6167  [.        storag
+0001d270: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
+0001d280: 5333 2c20 7374 6f72 6167 655f 6c69 622e  S3, storage_lib.
+0001d290: 5374 6f72 6554 7970 652e 4743 532c 0a20  StoreType.GCS,. 
+0001d2a0: 2020 2020 2020 2070 7974 6573 742e 7061         pytest.pa
+0001d2b0: 7261 6d28 7374 6f72 6167 655f 6c69 622e  ram(storage_lib.
+0001d2c0: 5374 6f72 6554 7970 652e 5232 2c20 6d61  StoreType.R2, ma
+0001d2d0: 726b 733d 7079 7465 7374 2e6d 6172 6b2e  rks=pytest.mark.
+0001d2e0: 636c 6f75 6466 6c61 7265 290a 2020 2020  cloudflare).    
+0001d2f0: 5d29 0a20 2020 2064 6566 2074 6573 745f  ]).    def test_
+0001d300: 6c69 7374 5f73 6f75 7263 6528 7365 6c66  list_source(self
+0001d310: 2c20 746d 705f 6c6f 6361 6c5f 6c69 7374  , tmp_local_list
+0001d320: 5f73 746f 7261 6765 5f6f 626a 2c20 7374  _storage_obj, st
+0001d330: 6f72 655f 7479 7065 293a 0a20 2020 2020  ore_type):.     
+0001d340: 2020 2023 2055 7365 7320 6120 6c69 7374     # Uses a list
+0001d350: 2069 6e20 7468 6520 736f 7572 6365 2066   in the source f
+0001d360: 6965 6c64 2074 6f20 7370 6563 6966 7920  ield to specify 
+0001d370: 6120 6669 6c65 2061 6e64 2061 2064 6972  a file and a dir
+0001d380: 6563 746f 7279 2074 6f0a 2020 2020 2020  ectory to.      
+0001d390: 2020 2320 6265 2075 706c 6f61 6465 6420    # be uploaded 
+0001d3a0: 746f 2074 6865 2073 746f 7261 6765 206f  to the storage o
+0001d3b0: 626a 6563 742e 0a20 2020 2020 2020 2074  bject..        t
+0001d3c0: 6d70 5f6c 6f63 616c 5f6c 6973 745f 7374  mp_local_list_st
+0001d3d0: 6f72 6167 655f 6f62 6a2e 6164 645f 7374  orage_obj.add_st
+0001d3e0: 6f72 6528 7374 6f72 655f 7479 7065 290a  ore(store_type).
+0001d3f0: 0a20 2020 2020 2020 2023 2043 6865 636b  .        # Check
+0001d400: 2069 6620 746d 702d 6669 6c65 2065 7869   if tmp-file exi
+0001d410: 7374 7320 696e 2074 6865 2062 7563 6b65  sts in the bucke
+0001d420: 7420 726f 6f74 2075 7369 6e67 2063 6c69  t root using cli
+0001d430: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
+0001d440: 7562 7072 6f63 6573 732e 6368 6563 6b5f  ubprocess.check_
+0001d450: 6f75 7470 7574 2873 656c 662e 636c 695f  output(self.cli_
+0001d460: 6c73 5f63 6d64 280a 2020 2020 2020 2020  ls_cmd(.        
+0001d470: 2020 2020 7374 6f72 655f 7479 7065 2c20      store_type, 
+0001d480: 746d 705f 6c6f 6361 6c5f 6c69 7374 5f73  tmp_local_list_s
+0001d490: 746f 7261 6765 5f6f 626a 2e6e 616d 6529  torage_obj.name)
+0001d4a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001d4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d4c0: 2020 2020 2020 2020 7368 656c 6c3d 5472          shell=Tr
+0001d4d0: 7565 290a 2020 2020 2020 2020 6173 7365  ue).        asse
+0001d4e0: 7274 2027 746d 702d 6669 6c65 2720 696e  rt 'tmp-file' in
+0001d4f0: 206f 7574 2e64 6563 6f64 6528 2775 7466   out.decode('utf
+0001d500: 2d38 2729 2c20 5c0a 2020 2020 2020 2020  -8'), \.        
+0001d510: 2020 2020 2746 696c 6520 6e6f 7420 666f      'File not fo
+0001d520: 756e 6420 696e 2062 7563 6b65 7420 2d20  und in bucket - 
+0001d530: 6f75 7470 7574 2077 6173 203a 207b 7d27  output was : {}'
+0001d540: 2e66 6f72 6d61 7428 6f75 742e 6465 636f  .format(out.deco
+0001d550: 6465 0a20 2020 2020 2020 2020 2020 2020  de.             
+0001d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d590: 2020 2028 2775 7466 2d38 2729 290a 0a20     ('utf-8')).. 
+0001d5a0: 2020 2020 2020 2023 2043 6865 636b 2069         # Check i
+0001d5b0: 6620 746d 702d 6669 6c65 2065 7869 7374  f tmp-file exist
+0001d5c0: 7320 696e 2074 6865 2062 7563 6b65 742f  s in the bucket/
+0001d5d0: 746d 702d 736f 7572 6365 2075 7369 6e67  tmp-source using
+0001d5e0: 2063 6c69 0a20 2020 2020 2020 206f 7574   cli.        out
+0001d5f0: 203d 2073 7562 7072 6f63 6573 732e 6368   = subprocess.ch
+0001d600: 6563 6b5f 6f75 7470 7574 2873 656c 662e  eck_output(self.
+0001d610: 636c 695f 6c73 5f63 6d64 280a 2020 2020  cli_ls_cmd(.    
+0001d620: 2020 2020 2020 2020 7374 6f72 655f 7479          store_ty
+0001d630: 7065 2c20 746d 705f 6c6f 6361 6c5f 6c69  pe, tmp_local_li
+0001d640: 7374 5f73 746f 7261 6765 5f6f 626a 2e6e  st_storage_obj.n
+0001d650: 616d 652c 2027 746d 702d 736f 7572 6365  ame, 'tmp-source
+0001d660: 2f27 292c 0a20 2020 2020 2020 2020 2020  /'),.           
 0001d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d680: 2020 2020 2020 2028 4743 535f 494e 5641         (GCS_INVA
-0001d690: 4c49 445f 4e41 4d45 532c 2073 746f 7261  LID_NAMES, stora
-0001d6a0: 6765 5f6c 6962 2e53 746f 7265 5479 7065  ge_lib.StoreType
-0001d6b0: 2e47 4353 292c 0a20 2020 2020 2020 2020  .GCS),.         
-0001d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d6d0: 2020 2020 2070 7974 6573 742e 7061 7261       pytest.para
-0001d6e0: 6d28 4157 535f 494e 5641 4c49 445f 4e41  m(AWS_INVALID_NA
-0001d6f0: 4d45 532c 0a20 2020 2020 2020 2020 2020  MES,.           
-0001d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d720: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
-0001d730: 6554 7970 652e 5232 2c0a 2020 2020 2020  eType.R2,.      
+0001d680: 2020 2020 2020 2020 2020 2073 6865 6c6c             shell
+0001d690: 3d54 7275 6529 0a20 2020 2020 2020 2061  =True).        a
+0001d6a0: 7373 6572 7420 2774 6d70 2d66 696c 6527  ssert 'tmp-file'
+0001d6b0: 2069 6e20 6f75 742e 6465 636f 6465 2827   in out.decode('
+0001d6c0: 7574 662d 3827 292c 205c 0a20 2020 2020  utf-8'), \.     
+0001d6d0: 2020 2020 2020 2027 4669 6c65 206e 6f74         'File not
+0001d6e0: 2066 6f75 6e64 2069 6e20 6275 636b 6574   found in bucket
+0001d6f0: 202d 206f 7574 7075 7420 7761 7320 3a20   - output was : 
+0001d700: 7b7d 272e 666f 726d 6174 286f 7574 2e64  {}'.format(out.d
+0001d710: 6563 6f64 650a 2020 2020 2020 2020 2020  ecode.          
+0001d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001d740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d760: 2020 2020 206d 6172 6b73 3d70 7974 6573       marks=pytes
-0001d770: 742e 6d61 726b 2e63 6c6f 7564 666c 6172  t.mark.cloudflar
-0001d780: 6529 5d29 0a20 2020 2064 6566 2074 6573  e)]).    def tes
-0001d790: 745f 696e 7661 6c69 645f 6e61 6d65 7328  t_invalid_names(
-0001d7a0: 7365 6c66 2c20 696e 7661 6c69 645f 6e61  self, invalid_na
-0001d7b0: 6d65 5f6c 6973 742c 2073 746f 7265 5f74  me_list, store_t
-0001d7c0: 7970 6529 3a0a 2020 2020 2020 2020 2320  ype):.        # 
-0001d7d0: 5573 6573 2061 206c 6973 7420 696e 2074  Uses a list in t
-0001d7e0: 6865 2073 6f75 7263 6520 6669 656c 6420  he source field 
-0001d7f0: 746f 2073 7065 6369 6679 2061 2066 696c  to specify a fil
-0001d800: 6520 616e 6420 6120 6469 7265 6374 6f72  e and a director
-0001d810: 7920 746f 0a20 2020 2020 2020 2023 2062  y to.        # b
-0001d820: 6520 7570 6c6f 6164 6564 2074 6f20 7468  e uploaded to th
-0001d830: 6520 7374 6f72 6167 6520 6f62 6a65 6374  e storage object
-0001d840: 2e0a 2020 2020 2020 2020 666f 7220 6e61  ..        for na
-0001d850: 6d65 2069 6e20 696e 7661 6c69 645f 6e61  me in invalid_na
-0001d860: 6d65 5f6c 6973 743a 0a20 2020 2020 2020  me_list:.       
-0001d870: 2020 2020 2077 6974 6820 7079 7465 7374       with pytest
-0001d880: 2e72 6169 7365 7328 736b 792e 6578 6365  .raises(sky.exce
-0001d890: 7074 696f 6e73 2e53 746f 7261 6765 4e61  ptions.StorageNa
-0001d8a0: 6d65 4572 726f 7229 3a0a 2020 2020 2020  meError):.      
-0001d8b0: 2020 2020 2020 2020 2020 7374 6f72 6167            storag
-0001d8c0: 655f 6f62 6a20 3d20 7374 6f72 6167 655f  e_obj = storage_
-0001d8d0: 6c69 622e 5374 6f72 6167 6528 6e61 6d65  lib.Storage(name
-0001d8e0: 3d6e 616d 6529 0a20 2020 2020 2020 2020  =name).         
-0001d8f0: 2020 2020 2020 2073 746f 7261 6765 5f6f         storage_o
-0001d900: 626a 2e61 6464 5f73 746f 7265 2873 746f  bj.add_store(sto
-0001d910: 7265 5f74 7970 6529 0a0a 0a23 202d 2d2d  re_type)...# ---
-0001d920: 2d2d 2d2d 2d2d 2d20 5465 7374 696e 6720  ------- Testing 
-0001d930: 5941 4d4c 2053 7065 6373 202d 2d2d 2d2d  YAML Specs -----
-0001d940: 2d2d 2d2d 2d0a 2320 4f75 7220 736b 7920  -----.# Our sky 
-0001d950: 7374 6f72 6167 6520 7265 7175 6972 6573  storage requires
-0001d960: 2063 7265 6465 6e74 6961 6c73 2074 6f20   credentials to 
-0001d970: 6368 6563 6b20 7468 6520 6275 636b 6574  check the bucket
-0001d980: 2065 7869 7374 616e 6365 2077 6865 6e0a   existance when.
-0001d990: 2320 6c6f 6164 696e 6720 6120 7461 736b  # loading a task
-0001d9a0: 2066 726f 6d20 7468 6520 7961 6d6c 2066   from the yaml f
-0001d9b0: 696c 652c 2073 6f20 7765 2063 616e 6e6f  ile, so we canno
-0001d9c0: 7420 6d61 6b65 2069 7420 6120 756e 6974  t make it a unit
-0001d9d0: 2074 6573 742e 0a63 6c61 7373 2054 6573   test..class Tes
-0001d9e0: 7459 616d 6c53 7065 6373 3a0a 2020 2020  tYamlSpecs:.    
-0001d9f0: 2320 544f 444f 287a 6877 7529 3a20 4164  # TODO(zhwu): Ad
-0001da00: 6420 7465 7374 2066 6f72 2060 746f 5f79  d test for `to_y
-0001da10: 616d 6c5f 636f 6e66 6967 6020 666f 7220  aml_config` for 
-0001da20: 7468 6520 5374 6f72 6167 6520 6f62 6a65  the Storage obje
-0001da30: 6374 2e0a 2020 2020 2320 2057 6520 7368  ct..    #  We sh
-0001da40: 6f75 6c64 206e 6f74 2075 7365 2060 6578  ould not use `ex
-0001da50: 616d 706c 6573 2f73 746f 7261 6765 5f64  amples/storage_d
-0001da60: 656d 6f2e 7961 6d6c 6020 6865 7265 2c20  emo.yaml` here, 
-0001da70: 7369 6e63 6520 6974 2072 6571 7569 7265  since it require
-0001da80: 730a 2020 2020 2320 2075 7365 7273 2074  s.    #  users t
-0001da90: 6f20 656e 7375 7265 2062 7563 6b65 7420  o ensure bucket 
-0001daa0: 6e61 6d65 7320 746f 206e 6f74 2065 7869  names to not exi
-0001dab0: 7374 2061 6e64 2f6f 7220 6265 2075 6e69  st and/or be uni
-0001dac0: 7175 652e 0a20 2020 205f 5445 5354 5f59  que..    _TEST_Y
-0001dad0: 414d 4c5f 5041 5448 5320 3d20 5b0a 2020  AML_PATHS = [.  
-0001dae0: 2020 2020 2020 2765 7861 6d70 6c65 732f        'examples/
-0001daf0: 6d69 6e69 6d61 6c2e 7961 6d6c 272c 2027  minimal.yaml', '
-0001db00: 6578 616d 706c 6573 2f6d 616e 6167 6564  examples/managed
-0001db10: 5f73 706f 742e 7961 6d6c 272c 0a20 2020  _spot.yaml',.   
-0001db20: 2020 2020 2027 6578 616d 706c 6573 2f75       'examples/u
-0001db30: 7369 6e67 5f66 696c 655f 6d6f 756e 7473  sing_file_mounts
-0001db40: 2e79 616d 6c27 2c20 2765 7861 6d70 6c65  .yaml', 'example
-0001db50: 732f 7265 736e 6574 5f61 7070 2e79 616d  s/resnet_app.yam
-0001db60: 6c27 2c0a 2020 2020 2020 2020 2765 7861  l',.        'exa
-0001db70: 6d70 6c65 732f 6d75 6c74 695f 686f 7374  mples/multi_host
-0001db80: 6e61 6d65 2e79 616d 6c27 0a20 2020 205d  name.yaml'.    ]
-0001db90: 0a0a 2020 2020 6465 6620 5f69 735f 6469  ..    def _is_di
-0001dba0: 6374 5f73 7562 7365 7428 7365 6c66 2c20  ct_subset(self, 
-0001dbb0: 6431 2c20 6432 293a 0a20 2020 2020 2020  d1, d2):.       
-0001dbc0: 2022 2222 4368 6563 6b20 6966 2064 3120   """Check if d1 
-0001dbd0: 6973 2074 6865 2073 7562 7365 7420 6f66  is the subset of
-0001dbe0: 2064 322e 2222 220a 2020 2020 2020 2020   d2.""".        
-0001dbf0: 666f 7220 6b2c 2076 2069 6e20 6431 2e69  for k, v in d1.i
-0001dc00: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
-0001dc10: 2020 2020 6966 206b 206e 6f74 2069 6e20      if k not in 
-0001dc20: 6432 3a0a 2020 2020 2020 2020 2020 2020  d2:.            
-0001dc30: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-0001dc40: 6528 762c 206c 6973 7429 206f 7220 6973  e(v, list) or is
-0001dc50: 696e 7374 616e 6365 2876 2c20 6469 6374  instance(v, dict
-0001dc60: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001dc70: 2020 2020 2020 2061 7373 6572 7420 6c65         assert le
-0001dc80: 6e28 7629 203d 3d20 302c 2028 6b2c 2076  n(v) == 0, (k, v
-0001dc90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001dca0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0001dcb0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-0001dcc0: 7274 2046 616c 7365 2c20 286b 2c20 7629  rt False, (k, v)
-0001dcd0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-0001dce0: 6620 6973 696e 7374 616e 6365 2876 2c20  f isinstance(v, 
-0001dcf0: 6469 6374 293a 0a20 2020 2020 2020 2020  dict):.         
-0001dd00: 2020 2020 2020 2061 7373 6572 7420 6973         assert is
-0001dd10: 696e 7374 616e 6365 2864 325b 6b5d 2c20  instance(d2[k], 
-0001dd20: 6469 6374 292c 2028 6b2c 2076 2c20 6432  dict), (k, v, d2
-0001dd30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001dd40: 2020 7365 6c66 2e5f 6973 5f64 6963 745f    self._is_dict_
-0001dd50: 7375 6273 6574 2876 2c20 6432 5b6b 5d29  subset(v, d2[k])
-0001dd60: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-0001dd70: 6620 6973 696e 7374 616e 6365 2876 2c20  f isinstance(v, 
-0001dd80: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-0001dd90: 2020 2020 2020 6966 206b 203d 3d20 2761        if k == 'a
-0001dda0: 6363 656c 6572 6174 6f72 7327 3a0a 2020  ccelerators':.  
-0001ddb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ddc0: 2020 7265 736f 7572 6365 7320 3d20 736b    resources = sk
-0001ddd0: 792e 5265 736f 7572 6365 7328 290a 2020  y.Resources().  
-0001dde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ddf0: 2020 7265 736f 7572 6365 732e 5f73 6574    resources._set
-0001de00: 5f61 6363 656c 6572 6174 6f72 7328 762c  _accelerators(v,
-0001de10: 204e 6f6e 6529 0a20 2020 2020 2020 2020   None).         
-0001de20: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-0001de30: 7420 7265 736f 7572 6365 732e 6163 6365  t resources.acce
-0001de40: 6c65 7261 746f 7273 203d 3d20 6432 5b6b  lerators == d2[k
-0001de50: 5d2c 2028 6b2c 2076 2c20 6432 290a 2020  ], (k, v, d2).  
-0001de60: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0001de70: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001de80: 2020 2020 2020 2020 6173 7365 7274 2076          assert v
-0001de90: 2e6c 6f77 6572 2829 203d 3d20 6432 5b6b  .lower() == d2[k
-0001dea0: 5d2e 6c6f 7765 7228 292c 2028 6b2c 2076  ].lower(), (k, v
-0001deb0: 2c20 6432 5b6b 5d29 0a20 2020 2020 2020  , d2[k]).       
-0001dec0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0001ded0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-0001dee0: 7420 7620 3d3d 2064 325b 6b5d 2c20 286b  t v == d2[k], (k
-0001def0: 2c20 762c 2064 325b 6b5d 290a 0a20 2020  , v, d2[k])..   
-0001df00: 2064 6566 205f 6368 6563 6b5f 6571 7569   def _check_equi
-0001df10: 7661 6c65 6e74 2873 656c 662c 2079 616d  valent(self, yam
-0001df20: 6c5f 7061 7468 293a 0a20 2020 2020 2020  l_path):.       
-0001df30: 2022 2222 4368 6563 6b20 6966 2074 6865   """Check if the
-0001df40: 2079 616d 6c20 6973 2065 7175 6976 616c   yaml is equival
-0001df50: 656e 7420 6166 7465 7220 6c6f 6164 2061  ent after load a
-0001df60: 6e64 2064 756d 7020 6167 6169 6e2e 2222  nd dump again.""
-0001df70: 220a 2020 2020 2020 2020 6f72 6967 696e  ".        origin
-0001df80: 5f74 6173 6b5f 636f 6e66 6967 203d 2063  _task_config = c
-0001df90: 6f6d 6d6f 6e5f 7574 696c 732e 7265 6164  ommon_utils.read
-0001dfa0: 5f79 616d 6c28 7961 6d6c 5f70 6174 6829  _yaml(yaml_path)
-0001dfb0: 0a0a 2020 2020 2020 2020 7461 736b 203d  ..        task =
-0001dfc0: 2073 6b79 2e54 6173 6b2e 6672 6f6d 5f79   sky.Task.from_y
-0001dfd0: 616d 6c28 7961 6d6c 5f70 6174 6829 0a20  aml(yaml_path). 
-0001dfe0: 2020 2020 2020 206e 6577 5f74 6173 6b5f         new_task_
-0001dff0: 636f 6e66 6967 203d 2074 6173 6b2e 746f  config = task.to
-0001e000: 5f79 616d 6c5f 636f 6e66 6967 2829 0a20  _yaml_config(). 
-0001e010: 2020 2020 2020 2023 2064 3120 3c3d 2064         # d1 <= d
-0001e020: 320a 2020 2020 2020 2020 7365 6c66 2e5f  2.        self._
-0001e030: 6973 5f64 6963 745f 7375 6273 6574 286f  is_dict_subset(o
-0001e040: 7269 6769 6e5f 7461 736b 5f63 6f6e 6669  rigin_task_confi
-0001e050: 672c 206e 6577 5f74 6173 6b5f 636f 6e66  g, new_task_conf
-0001e060: 6967 290a 0a20 2020 2064 6566 2074 6573  ig)..    def tes
-0001e070: 745f 6c6f 6164 5f64 756d 705f 7961 6d6c  t_load_dump_yaml
-0001e080: 5f63 6f6e 6669 675f 6571 7569 7661 6c65  _config_equivale
-0001e090: 6e74 2873 656c 6629 3a0a 2020 2020 2020  nt(self):.      
-0001e0a0: 2020 2222 2254 6573 7420 6966 2074 6865    """Test if the
-0001e0b0: 2079 616d 6c20 636f 6e66 6967 2069 7320   yaml config is 
-0001e0c0: 6571 7569 7661 6c65 6e74 2061 6674 6572  equivalent after
-0001e0d0: 206c 6f61 6420 616e 6420 6475 6d70 2061   load and dump a
-0001e0e0: 6761 696e 2e22 2222 0a20 2020 2020 2020  gain.""".       
-0001e0f0: 2070 6174 686c 6962 2e50 6174 6828 277e   pathlib.Path('~
-0001e100: 2f64 6174 6173 6574 7327 292e 6578 7061  /datasets').expa
-0001e110: 6e64 7573 6572 2829 2e6d 6b64 6972 2865  nduser().mkdir(e
-0001e120: 7869 7374 5f6f 6b3d 5472 7565 290a 2020  xist_ok=True).  
-0001e130: 2020 2020 2020 7061 7468 6c69 622e 5061        pathlib.Pa
-0001e140: 7468 2827 7e2f 746d 7066 696c 6527 292e  th('~/tmpfile').
-0001e150: 6578 7061 6e64 7573 6572 2829 2e74 6f75  expanduser().tou
-0001e160: 6368 2829 0a20 2020 2020 2020 2070 6174  ch().        pat
-0001e170: 686c 6962 2e50 6174 6828 277e 2f2e 7373  hlib.Path('~/.ss
-0001e180: 6827 292e 6578 7061 6e64 7573 6572 2829  h').expanduser()
-0001e190: 2e6d 6b64 6972 2865 7869 7374 5f6f 6b3d  .mkdir(exist_ok=
-0001e1a0: 5472 7565 290a 2020 2020 2020 2020 7061  True).        pa
-0001e1b0: 7468 6c69 622e 5061 7468 2827 7e2f 2e73  thlib.Path('~/.s
-0001e1c0: 7368 2f69 645f 7273 612e 7075 6227 292e  sh/id_rsa.pub').
-0001e1d0: 6578 7061 6e64 7573 6572 2829 2e74 6f75  expanduser().tou
-0001e1e0: 6368 2829 0a20 2020 2020 2020 2070 6174  ch().        pat
-0001e1f0: 686c 6962 2e50 6174 6828 277e 2f74 6d70  hlib.Path('~/tmp
-0001e200: 2d77 6f72 6b64 6972 2729 2e65 7870 616e  -workdir').expan
-0001e210: 6475 7365 7228 292e 6d6b 6469 7228 6578  duser().mkdir(ex
-0001e220: 6973 745f 6f6b 3d54 7275 6529 0a20 2020  ist_ok=True).   
-0001e230: 2020 2020 2070 6174 686c 6962 2e50 6174       pathlib.Pat
-0001e240: 6828 277e 2f44 6f77 6e6c 6f61 6473 2f74  h('~/Downloads/t
-0001e250: 7075 2729 2e65 7870 616e 6475 7365 7228  pu').expanduser(
-0001e260: 292e 6d6b 6469 7228 7061 7265 6e74 733d  ).mkdir(parents=
-0001e270: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-0001e280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e2b0: 2065 7869 7374 5f6f 6b3d 5472 7565 290a   exist_ok=True).
-0001e2c0: 2020 2020 2020 2020 666f 7220 7961 6d6c          for yaml
-0001e2d0: 5f70 6174 6820 696e 2073 656c 662e 5f54  _path in self._T
-0001e2e0: 4553 545f 5941 4d4c 5f50 4154 4853 3a0a  EST_YAML_PATHS:.
-0001e2f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001e300: 2e5f 6368 6563 6b5f 6571 7569 7661 6c65  ._check_equivale
-0001e310: 6e74 2879 616d 6c5f 7061 7468 290a       nt(yaml_path).
+0001d750: 2020 2020 2020 2827 7574 662d 3827 2929        ('utf-8'))
+0001d760: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
+0001d770: 726b 2e70 6172 616d 6574 7269 7a65 2827  rk.parametrize('
+0001d780: 696e 7661 6c69 645f 6e61 6d65 5f6c 6973  invalid_name_lis
+0001d790: 742c 2073 746f 7265 5f74 7970 6527 2c0a  t, store_type',.
+0001d7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d7b0: 2020 2020 2020 2020 2020 2020 205b 2841               [(A
+0001d7c0: 5753 5f49 4e56 414c 4944 5f4e 414d 4553  WS_INVALID_NAMES
+0001d7d0: 2c20 7374 6f72 6167 655f 6c69 622e 5374  , storage_lib.St
+0001d7e0: 6f72 6554 7970 652e 5333 292c 0a20 2020  oreType.S3),.   
+0001d7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d800: 2020 2020 2020 2020 2020 2028 4743 535f             (GCS_
+0001d810: 494e 5641 4c49 445f 4e41 4d45 532c 2073  INVALID_NAMES, s
+0001d820: 746f 7261 6765 5f6c 6962 2e53 746f 7265  torage_lib.Store
+0001d830: 5479 7065 2e47 4353 292c 0a20 2020 2020  Type.GCS),.     
+0001d840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d850: 2020 2020 2020 2020 2070 7974 6573 742e           pytest.
+0001d860: 7061 7261 6d28 4157 535f 494e 5641 4c49  param(AWS_INVALI
+0001d870: 445f 4e41 4d45 532c 0a20 2020 2020 2020  D_NAMES,.       
+0001d880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d8a0: 2020 2020 7374 6f72 6167 655f 6c69 622e      storage_lib.
+0001d8b0: 5374 6f72 6554 7970 652e 5232 2c0a 2020  StoreType.R2,.  
+0001d8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d8e0: 2020 2020 2020 2020 206d 6172 6b73 3d70           marks=p
+0001d8f0: 7974 6573 742e 6d61 726b 2e63 6c6f 7564  ytest.mark.cloud
+0001d900: 666c 6172 6529 5d29 0a20 2020 2064 6566  flare)]).    def
+0001d910: 2074 6573 745f 696e 7661 6c69 645f 6e61   test_invalid_na
+0001d920: 6d65 7328 7365 6c66 2c20 696e 7661 6c69  mes(self, invali
+0001d930: 645f 6e61 6d65 5f6c 6973 742c 2073 746f  d_name_list, sto
+0001d940: 7265 5f74 7970 6529 3a0a 2020 2020 2020  re_type):.      
+0001d950: 2020 2320 5573 6573 2061 206c 6973 7420    # Uses a list 
+0001d960: 696e 2074 6865 2073 6f75 7263 6520 6669  in the source fi
+0001d970: 656c 6420 746f 2073 7065 6369 6679 2061  eld to specify a
+0001d980: 2066 696c 6520 616e 6420 6120 6469 7265   file and a dire
+0001d990: 6374 6f72 7920 746f 0a20 2020 2020 2020  ctory to.       
+0001d9a0: 2023 2062 6520 7570 6c6f 6164 6564 2074   # be uploaded t
+0001d9b0: 6f20 7468 6520 7374 6f72 6167 6520 6f62  o the storage ob
+0001d9c0: 6a65 6374 2e0a 2020 2020 2020 2020 666f  ject..        fo
+0001d9d0: 7220 6e61 6d65 2069 6e20 696e 7661 6c69  r name in invali
+0001d9e0: 645f 6e61 6d65 5f6c 6973 743a 0a20 2020  d_name_list:.   
+0001d9f0: 2020 2020 2020 2020 2077 6974 6820 7079           with py
+0001da00: 7465 7374 2e72 6169 7365 7328 736b 792e  test.raises(sky.
+0001da10: 6578 6365 7074 696f 6e73 2e53 746f 7261  exceptions.Stora
+0001da20: 6765 4e61 6d65 4572 726f 7229 3a0a 2020  geNameError):.  
+0001da30: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0001da40: 6f72 6167 655f 6f62 6a20 3d20 7374 6f72  orage_obj = stor
+0001da50: 6167 655f 6c69 622e 5374 6f72 6167 6528  age_lib.Storage(
+0001da60: 6e61 6d65 3d6e 616d 6529 0a20 2020 2020  name=name).     
+0001da70: 2020 2020 2020 2020 2020 2073 746f 7261             stora
+0001da80: 6765 5f6f 626a 2e61 6464 5f73 746f 7265  ge_obj.add_store
+0001da90: 2873 746f 7265 5f74 7970 6529 0a0a 0a23  (store_type)...#
+0001daa0: 202d 2d2d 2d2d 2d2d 2d2d 2d20 5465 7374   ---------- Test
+0001dab0: 696e 6720 5941 4d4c 2053 7065 6373 202d  ing YAML Specs -
+0001dac0: 2d2d 2d2d 2d2d 2d2d 2d0a 2320 4f75 7220  ---------.# Our 
+0001dad0: 736b 7920 7374 6f72 6167 6520 7265 7175  sky storage requ
+0001dae0: 6972 6573 2063 7265 6465 6e74 6961 6c73  ires credentials
+0001daf0: 2074 6f20 6368 6563 6b20 7468 6520 6275   to check the bu
+0001db00: 636b 6574 2065 7869 7374 616e 6365 2077  cket existance w
+0001db10: 6865 6e0a 2320 6c6f 6164 696e 6720 6120  hen.# loading a 
+0001db20: 7461 736b 2066 726f 6d20 7468 6520 7961  task from the ya
+0001db30: 6d6c 2066 696c 652c 2073 6f20 7765 2063  ml file, so we c
+0001db40: 616e 6e6f 7420 6d61 6b65 2069 7420 6120  annot make it a 
+0001db50: 756e 6974 2074 6573 742e 0a63 6c61 7373  unit test..class
+0001db60: 2054 6573 7459 616d 6c53 7065 6373 3a0a   TestYamlSpecs:.
+0001db70: 2020 2020 2320 544f 444f 287a 6877 7529      # TODO(zhwu)
+0001db80: 3a20 4164 6420 7465 7374 2066 6f72 2060  : Add test for `
+0001db90: 746f 5f79 616d 6c5f 636f 6e66 6967 6020  to_yaml_config` 
+0001dba0: 666f 7220 7468 6520 5374 6f72 6167 6520  for the Storage 
+0001dbb0: 6f62 6a65 6374 2e0a 2020 2020 2320 2057  object..    #  W
+0001dbc0: 6520 7368 6f75 6c64 206e 6f74 2075 7365  e should not use
+0001dbd0: 2060 6578 616d 706c 6573 2f73 746f 7261   `examples/stora
+0001dbe0: 6765 5f64 656d 6f2e 7961 6d6c 6020 6865  ge_demo.yaml` he
+0001dbf0: 7265 2c20 7369 6e63 6520 6974 2072 6571  re, since it req
+0001dc00: 7569 7265 730a 2020 2020 2320 2075 7365  uires.    #  use
+0001dc10: 7273 2074 6f20 656e 7375 7265 2062 7563  rs to ensure buc
+0001dc20: 6b65 7420 6e61 6d65 7320 746f 206e 6f74  ket names to not
+0001dc30: 2065 7869 7374 2061 6e64 2f6f 7220 6265   exist and/or be
+0001dc40: 2075 6e69 7175 652e 0a20 2020 205f 5445   unique..    _TE
+0001dc50: 5354 5f59 414d 4c5f 5041 5448 5320 3d20  ST_YAML_PATHS = 
+0001dc60: 5b0a 2020 2020 2020 2020 2765 7861 6d70  [.        'examp
+0001dc70: 6c65 732f 6d69 6e69 6d61 6c2e 7961 6d6c  les/minimal.yaml
+0001dc80: 272c 2027 6578 616d 706c 6573 2f6d 616e  ', 'examples/man
+0001dc90: 6167 6564 5f73 706f 742e 7961 6d6c 272c  aged_spot.yaml',
+0001dca0: 0a20 2020 2020 2020 2027 6578 616d 706c  .        'exampl
+0001dcb0: 6573 2f75 7369 6e67 5f66 696c 655f 6d6f  es/using_file_mo
+0001dcc0: 756e 7473 2e79 616d 6c27 2c20 2765 7861  unts.yaml', 'exa
+0001dcd0: 6d70 6c65 732f 7265 736e 6574 5f61 7070  mples/resnet_app
+0001dce0: 2e79 616d 6c27 2c0a 2020 2020 2020 2020  .yaml',.        
+0001dcf0: 2765 7861 6d70 6c65 732f 6d75 6c74 695f  'examples/multi_
+0001dd00: 686f 7374 6e61 6d65 2e79 616d 6c27 0a20  hostname.yaml'. 
+0001dd10: 2020 205d 0a0a 2020 2020 6465 6620 5f69     ]..    def _i
+0001dd20: 735f 6469 6374 5f73 7562 7365 7428 7365  s_dict_subset(se
+0001dd30: 6c66 2c20 6431 2c20 6432 293a 0a20 2020  lf, d1, d2):.   
+0001dd40: 2020 2020 2022 2222 4368 6563 6b20 6966       """Check if
+0001dd50: 2064 3120 6973 2074 6865 2073 7562 7365   d1 is the subse
+0001dd60: 7420 6f66 2064 322e 2222 220a 2020 2020  t of d2.""".    
+0001dd70: 2020 2020 666f 7220 6b2c 2076 2069 6e20      for k, v in 
+0001dd80: 6431 2e69 7465 6d73 2829 3a0a 2020 2020  d1.items():.    
+0001dd90: 2020 2020 2020 2020 6966 206b 206e 6f74          if k not
+0001dda0: 2069 6e20 6432 3a0a 2020 2020 2020 2020   in d2:.        
+0001ddb0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+0001ddc0: 7461 6e63 6528 762c 206c 6973 7429 206f  tance(v, list) o
+0001ddd0: 7220 6973 696e 7374 616e 6365 2876 2c20  r isinstance(v, 
+0001dde0: 6469 6374 293a 0a20 2020 2020 2020 2020  dict):.         
+0001ddf0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+0001de00: 7420 6c65 6e28 7629 203d 3d20 302c 2028  t len(v) == 0, (
+0001de10: 6b2c 2076 290a 2020 2020 2020 2020 2020  k, v).          
+0001de20: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0001de30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de40: 6173 7365 7274 2046 616c 7365 2c20 286b  assert False, (k
+0001de50: 2c20 7629 0a20 2020 2020 2020 2020 2020  , v).           
+0001de60: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+0001de70: 2876 2c20 6469 6374 293a 0a20 2020 2020  (v, dict):.     
+0001de80: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+0001de90: 7420 6973 696e 7374 616e 6365 2864 325b  t isinstance(d2[
+0001dea0: 6b5d 2c20 6469 6374 292c 2028 6b2c 2076  k], dict), (k, v
+0001deb0: 2c20 6432 290a 2020 2020 2020 2020 2020  , d2).          
+0001dec0: 2020 2020 2020 7365 6c66 2e5f 6973 5f64        self._is_d
+0001ded0: 6963 745f 7375 6273 6574 2876 2c20 6432  ict_subset(v, d2
+0001dee0: 5b6b 5d29 0a20 2020 2020 2020 2020 2020  [k]).           
+0001def0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+0001df00: 2876 2c20 7374 7229 3a0a 2020 2020 2020  (v, str):.      
+0001df10: 2020 2020 2020 2020 2020 6966 206b 203d            if k =
+0001df20: 3d20 2761 6363 656c 6572 6174 6f72 7327  = 'accelerators'
+0001df30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001df40: 2020 2020 2020 7265 736f 7572 6365 7320        resources 
+0001df50: 3d20 736b 792e 5265 736f 7572 6365 7328  = sky.Resources(
+0001df60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001df70: 2020 2020 2020 7265 736f 7572 6365 732e        resources.
+0001df80: 5f73 6574 5f61 6363 656c 6572 6174 6f72  _set_accelerator
+0001df90: 7328 762c 204e 6f6e 6529 0a20 2020 2020  s(v, None).     
+0001dfa0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0001dfb0: 7373 6572 7420 7265 736f 7572 6365 732e  ssert resources.
+0001dfc0: 6163 6365 6c65 7261 746f 7273 203d 3d20  accelerators == 
+0001dfd0: 6432 5b6b 5d2c 2028 6b2c 2076 2c20 6432  d2[k], (k, v, d2
+0001dfe0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001dff0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001e000: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+0001e010: 7274 2076 2e6c 6f77 6572 2829 203d 3d20  rt v.lower() == 
+0001e020: 6432 5b6b 5d2e 6c6f 7765 7228 292c 2028  d2[k].lower(), (
+0001e030: 6b2c 2076 2c20 6432 5b6b 5d29 0a20 2020  k, v, d2[k]).   
+0001e040: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0001e050: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0001e060: 7373 6572 7420 7620 3d3d 2064 325b 6b5d  ssert v == d2[k]
+0001e070: 2c20 286b 2c20 762c 2064 325b 6b5d 290a  , (k, v, d2[k]).
+0001e080: 0a20 2020 2064 6566 205f 6368 6563 6b5f  .    def _check_
+0001e090: 6571 7569 7661 6c65 6e74 2873 656c 662c  equivalent(self,
+0001e0a0: 2079 616d 6c5f 7061 7468 293a 0a20 2020   yaml_path):.   
+0001e0b0: 2020 2020 2022 2222 4368 6563 6b20 6966       """Check if
+0001e0c0: 2074 6865 2079 616d 6c20 6973 2065 7175   the yaml is equ
+0001e0d0: 6976 616c 656e 7420 6166 7465 7220 6c6f  ivalent after lo
+0001e0e0: 6164 2061 6e64 2064 756d 7020 6167 6169  ad and dump agai
+0001e0f0: 6e2e 2222 220a 2020 2020 2020 2020 6f72  n.""".        or
+0001e100: 6967 696e 5f74 6173 6b5f 636f 6e66 6967  igin_task_config
+0001e110: 203d 2063 6f6d 6d6f 6e5f 7574 696c 732e   = common_utils.
+0001e120: 7265 6164 5f79 616d 6c28 7961 6d6c 5f70  read_yaml(yaml_p
+0001e130: 6174 6829 0a0a 2020 2020 2020 2020 7461  ath)..        ta
+0001e140: 736b 203d 2073 6b79 2e54 6173 6b2e 6672  sk = sky.Task.fr
+0001e150: 6f6d 5f79 616d 6c28 7961 6d6c 5f70 6174  om_yaml(yaml_pat
+0001e160: 6829 0a20 2020 2020 2020 206e 6577 5f74  h).        new_t
+0001e170: 6173 6b5f 636f 6e66 6967 203d 2074 6173  ask_config = tas
+0001e180: 6b2e 746f 5f79 616d 6c5f 636f 6e66 6967  k.to_yaml_config
+0001e190: 2829 0a20 2020 2020 2020 2023 2064 3120  ().        # d1 
+0001e1a0: 3c3d 2064 320a 2020 2020 2020 2020 7365  <= d2.        se
+0001e1b0: 6c66 2e5f 6973 5f64 6963 745f 7375 6273  lf._is_dict_subs
+0001e1c0: 6574 286f 7269 6769 6e5f 7461 736b 5f63  et(origin_task_c
+0001e1d0: 6f6e 6669 672c 206e 6577 5f74 6173 6b5f  onfig, new_task_
+0001e1e0: 636f 6e66 6967 290a 0a20 2020 2064 6566  config)..    def
+0001e1f0: 2074 6573 745f 6c6f 6164 5f64 756d 705f   test_load_dump_
+0001e200: 7961 6d6c 5f63 6f6e 6669 675f 6571 7569  yaml_config_equi
+0001e210: 7661 6c65 6e74 2873 656c 6629 3a0a 2020  valent(self):.  
+0001e220: 2020 2020 2020 2222 2254 6573 7420 6966        """Test if
+0001e230: 2074 6865 2079 616d 6c20 636f 6e66 6967   the yaml config
+0001e240: 2069 7320 6571 7569 7661 6c65 6e74 2061   is equivalent a
+0001e250: 6674 6572 206c 6f61 6420 616e 6420 6475  fter load and du
+0001e260: 6d70 2061 6761 696e 2e22 2222 0a20 2020  mp again.""".   
+0001e270: 2020 2020 2070 6174 686c 6962 2e50 6174       pathlib.Pat
+0001e280: 6828 277e 2f64 6174 6173 6574 7327 292e  h('~/datasets').
+0001e290: 6578 7061 6e64 7573 6572 2829 2e6d 6b64  expanduser().mkd
+0001e2a0: 6972 2865 7869 7374 5f6f 6b3d 5472 7565  ir(exist_ok=True
+0001e2b0: 290a 2020 2020 2020 2020 7061 7468 6c69  ).        pathli
+0001e2c0: 622e 5061 7468 2827 7e2f 746d 7066 696c  b.Path('~/tmpfil
+0001e2d0: 6527 292e 6578 7061 6e64 7573 6572 2829  e').expanduser()
+0001e2e0: 2e74 6f75 6368 2829 0a20 2020 2020 2020  .touch().       
+0001e2f0: 2070 6174 686c 6962 2e50 6174 6828 277e   pathlib.Path('~
+0001e300: 2f2e 7373 6827 292e 6578 7061 6e64 7573  /.ssh').expandus
+0001e310: 6572 2829 2e6d 6b64 6972 2865 7869 7374  er().mkdir(exist
+0001e320: 5f6f 6b3d 5472 7565 290a 2020 2020 2020  _ok=True).      
+0001e330: 2020 7061 7468 6c69 622e 5061 7468 2827    pathlib.Path('
+0001e340: 7e2f 2e73 7368 2f69 645f 7273 612e 7075  ~/.ssh/id_rsa.pu
+0001e350: 6227 292e 6578 7061 6e64 7573 6572 2829  b').expanduser()
+0001e360: 2e74 6f75 6368 2829 0a20 2020 2020 2020  .touch().       
+0001e370: 2070 6174 686c 6962 2e50 6174 6828 277e   pathlib.Path('~
+0001e380: 2f74 6d70 2d77 6f72 6b64 6972 2729 2e65  /tmp-workdir').e
+0001e390: 7870 616e 6475 7365 7228 292e 6d6b 6469  xpanduser().mkdi
+0001e3a0: 7228 6578 6973 745f 6f6b 3d54 7275 6529  r(exist_ok=True)
+0001e3b0: 0a20 2020 2020 2020 2070 6174 686c 6962  .        pathlib
+0001e3c0: 2e50 6174 6828 277e 2f44 6f77 6e6c 6f61  .Path('~/Downloa
+0001e3d0: 6473 2f74 7075 2729 2e65 7870 616e 6475  ds/tpu').expandu
+0001e3e0: 7365 7228 292e 6d6b 6469 7228 7061 7265  ser().mkdir(pare
+0001e3f0: 6e74 733d 5472 7565 2c0a 2020 2020 2020  nts=True,.      
+0001e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e430: 2020 2020 2065 7869 7374 5f6f 6b3d 5472       exist_ok=Tr
+0001e440: 7565 290a 2020 2020 2020 2020 666f 7220  ue).        for 
+0001e450: 7961 6d6c 5f70 6174 6820 696e 2073 656c  yaml_path in sel
+0001e460: 662e 5f54 4553 545f 5941 4d4c 5f50 4154  f._TEST_YAML_PAT
+0001e470: 4853 3a0a 2020 2020 2020 2020 2020 2020  HS:.            
+0001e480: 7365 6c66 2e5f 6368 6563 6b5f 6571 7569  self._check_equi
+0001e490: 7661 6c65 6e74 2879 616d 6c5f 7061 7468  valent(yaml_path
+0001e4a0: 290a                                     ).
```

### Comparing `skypilot-nightly-1.0.0.dev20230715/tests/test_spot.py` & `skypilot-nightly-1.0.0.dev20230716/tests/test_spot.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/tests/test_storage.py` & `skypilot-nightly-1.0.0.dev20230716/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230715/tests/test_wheels.py` & `skypilot-nightly-1.0.0.dev20230716/tests/test_wheels.py`

 * *Files identical despite different names*

