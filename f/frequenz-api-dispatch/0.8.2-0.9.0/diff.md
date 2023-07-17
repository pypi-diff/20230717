# Comparing `tmp/frequenz-api-dispatch-0.8.2.tar.gz` & `tmp/frequenz-api-dispatch-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-api-dispatch-0.8.2.tar", last modified: Mon Jun 19 15:30:43 2023, max compression
+gzip compressed data, was "frequenz-api-dispatch-0.9.0.tar", last modified: Mon Jul 17 12:16:25 2023, max compression
```

## Comparing `frequenz-api-dispatch-0.8.2.tar` & `frequenz-api-dispatch-0.9.0.tar`

### file list

```diff
@@ -1,109 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.027608 frequenz-api-dispatch-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (122)      258 2023-06-19 15:30:27.000000 frequenz-api-dispatch-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-06-19 15:30:43.027608 frequenz-api-dispatch-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-06-19 15:30:27.000000 frequenz-api-dispatch-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-06-19 15:30:27.000000 frequenz-api-dispatch-0.8.2/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-06-19 15:30:27.000000 frequenz-api-dispatch-0.8.2/ci.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/proto/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/proto/frequenz/api/dispatch/
--rw-r--r--   0 runner    (1001) docker     (122)     5467 2023-06-19 15:30:27.000000 frequenz-api-dispatch-0.8.2/proto/frequenz/api/dispatch/dispatch.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/proto/frequenz/api/dispatch/fcr/
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-06-19 15:30:27.000000 frequenz-api-dispatch-0.8.2/proto/frequenz/api/dispatch/fcr/prequalification.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/py/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/py/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/py/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/py/frequenz/api/dispatch/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-19 15:30:27.000000 frequenz-api-dispatch-0.8.2/py/frequenz/api/dispatch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/py/frequenz/api/dispatch/fcr/
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-19 15:30:27.000000 frequenz-api-dispatch-0.8.2/py/frequenz/api/dispatch/fcr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:27.000000 frequenz-api-dispatch-0.8.2/py/frequenz/api/dispatch/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/py/frequenz_api_dispatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-06-19 15:30:42.000000 frequenz-api-dispatch-0.8.2/py/frequenz_api_dispatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3880 2023-06-19 15:30:43.000000 frequenz-api-dispatch-0.8.2/py/frequenz_api_dispatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 15:30:42.000000 frequenz-api-dispatch-0.8.2/py/frequenz_api_dispatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      524 2023-06-19 15:30:42.000000 frequenz-api-dispatch-0.8.2/py/frequenz_api_dispatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-19 15:30:42.000000 frequenz-api-dispatch-0.8.2/py/frequenz_api_dispatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-06-19 15:30:27.000000 frequenz-api-dispatch-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-19 15:30:43.027608 frequenz-api-dispatch-0.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.019609 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/annotations.proto
--rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/auth.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/backend.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/billing.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/client.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/config_change.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/consumer.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/context.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/control.proto
--rw-r--r--   0 runner    (1001) docker     (122)     8657 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/distribution.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/documentation.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/endpoint.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/field_behavior.proto
--rw-r--r--   0 runner    (1001) docker     (122)    12099 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/http.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/httpbody.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/label.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/launch_stage.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/log.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3209 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/logging.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/metric.proto
--rw-r--r--   0 runner    (1001) docker     (122)     5512 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/monitored_resource.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/monitoring.proto
--rw-r--r--   0 runner    (1001) docker     (122)    10854 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/quota.proto
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/resource.proto
--rw-r--r--   0 runner    (1001) docker     (122)    14929 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/routing.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/service.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/source_info.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3472 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/system_parameter.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/usage.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.019609 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/cloud/extended_operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/iam/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/iam/admin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.019609 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/iam/admin/v1/
--rw-r--r--   0 runner    (1001) docker     (122)    41483 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/iam/admin/v1/iam.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.019609 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/iam/v1/
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/iam/v1/iam_policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.019609 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/iam/v1/logging/
--rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/iam/v1/options.proto
--rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/iam/v1/policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/logging/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.023609 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/logging/type/
--rw-r--r--   0 runner    (1001) docker     (122)     3389 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/logging/type/http_request.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/logging/type/log_severity.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.023609 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/longrunning/
--rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/longrunning/operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.023609 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/rpc/
--rw-r--r--   0 runner    (1001) docker     (122)     7125 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/rpc/code.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.023609 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/rpc/context/
--rw-r--r--   0 runner    (1001) docker     (122)    12015 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/rpc/context/attribute_context.proto
--rw-r--r--   0 runner    (1001) docker     (122)     9504 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/rpc/error_details.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/rpc/status.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.023609 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/calendar_period.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/color.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/date.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/datetime.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/dayofweek.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/expr.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/fraction.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/latlng.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/money.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/month.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6239 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/postal_address.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/quaternion.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-06-19 15:30:28.000000 frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/timeofday.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/submodules/frequenz-api-common/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/submodules/frequenz-api-common/proto/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/submodules/frequenz-api-common/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.015609 frequenz-api-dispatch-0.8.2/submodules/frequenz-api-common/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.023609 frequenz-api-dispatch-0.8.2/submodules/frequenz-api-common/proto/frequenz/api/common/
--rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-06-19 15:30:29.000000 frequenz-api-dispatch-0.8.2/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 15:30:43.027608 frequenz-api-dispatch-0.8.2/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)     6145 2023-06-19 15:30:29.000000 frequenz-api-dispatch-0.8.2/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-06-19 15:30:29.000000 frequenz-api-dispatch-0.8.2/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.858466 frequenz-api-dispatch-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-07-17 12:16:03.000000 frequenz-api-dispatch-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-07-17 12:16:25.858466 frequenz-api-dispatch-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-17 12:16:03.000000 frequenz-api-dispatch-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-07-17 12:16:03.000000 frequenz-api-dispatch-0.9.0/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-07-17 12:16:03.000000 frequenz-api-dispatch-0.9.0/ci.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.838466 frequenz-api-dispatch-0.9.0/proto/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.838466 frequenz-api-dispatch-0.9.0/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.838466 frequenz-api-dispatch-0.9.0/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.842466 frequenz-api-dispatch-0.9.0/proto/frequenz/api/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (122)     4770 2023-07-17 12:16:03.000000 frequenz-api-dispatch-0.9.0/proto/frequenz/api/dispatch/dispatch.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.838466 frequenz-api-dispatch-0.9.0/py/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.838466 frequenz-api-dispatch-0.9.0/py/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.838466 frequenz-api-dispatch-0.9.0/py/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.842466 frequenz-api-dispatch-0.9.0/py/frequenz/api/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-17 12:16:03.000000 frequenz-api-dispatch-0.9.0/py/frequenz/api/dispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:03.000000 frequenz-api-dispatch-0.9.0/py/frequenz/api/dispatch/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.846466 frequenz-api-dispatch-0.9.0/py/frequenz_api_dispatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-07-17 12:16:25.000000 frequenz-api-dispatch-0.9.0/py/frequenz_api_dispatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3784 2023-07-17 12:16:25.000000 frequenz-api-dispatch-0.9.0/py/frequenz_api_dispatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 12:16:25.000000 frequenz-api-dispatch-0.9.0/py/frequenz_api_dispatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      524 2023-07-17 12:16:25.000000 frequenz-api-dispatch-0.9.0/py/frequenz_api_dispatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-17 12:16:25.000000 frequenz-api-dispatch-0.9.0/py/frequenz_api_dispatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-07-17 12:16:03.000000 frequenz-api-dispatch-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-17 12:16:25.858466 frequenz-api-dispatch-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.842466 frequenz-api-dispatch-0.9.0/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.838466 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.842466 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.850466 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/annotations.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/auth.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/backend.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/billing.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/client.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/config_change.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/consumer.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/context.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/control.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     8657 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/distribution.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/documentation.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/endpoint.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/field_behavior.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    12099 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/http.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/httpbody.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/label.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/launch_stage.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/log.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3209 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/logging.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/metric.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     5512 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/monitored_resource.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/monitoring.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    10854 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/quota.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/resource.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    14929 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/routing.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/service.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/source_info.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3472 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/system_parameter.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/usage.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.850466 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/cloud/extended_operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.842466 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/iam/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.838466 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/iam/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.850466 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/iam/admin/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)    41483 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.854466 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/iam/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.854466 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/iam/v1/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/iam/v1/options.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/iam/v1/policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.842466 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/logging/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.854466 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/logging/type/
+-rw-r--r--   0 runner    (1001) docker     (122)     3389 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/logging/type/http_request.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/logging/type/log_severity.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.854466 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/longrunning/
+-rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/longrunning/operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.854466 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/rpc/
+-rw-r--r--   0 runner    (1001) docker     (122)     7125 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/rpc/code.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.854466 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/rpc/context/
+-rw-r--r--   0 runner    (1001) docker     (122)    12015 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     9504 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/rpc/error_details.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/rpc/status.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.858466 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/calendar_period.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/color.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/date.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/datetime.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/dayofweek.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/expr.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/fraction.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/latlng.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/money.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/month.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6239 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/postal_address.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/quaternion.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-07-17 12:16:05.000000 frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/timeofday.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.842466 frequenz-api-dispatch-0.9.0/submodules/frequenz-api-common/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.842466 frequenz-api-dispatch-0.9.0/submodules/frequenz-api-common/proto/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.842466 frequenz-api-dispatch-0.9.0/submodules/frequenz-api-common/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.842466 frequenz-api-dispatch-0.9.0/submodules/frequenz-api-common/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.858466 frequenz-api-dispatch-0.9.0/submodules/frequenz-api-common/proto/frequenz/api/common/
+-rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-07-17 12:16:06.000000 frequenz-api-dispatch-0.9.0/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 12:16:25.858466 frequenz-api-dispatch-0.9.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)     6145 2023-07-17 12:16:06.000000 frequenz-api-dispatch-0.9.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-07-17 12:16:06.000000 frequenz-api-dispatch-0.9.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
```

### Comparing `frequenz-api-dispatch-0.8.2/PKG-INFO` & `frequenz-api-dispatch-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-dispatch
-Version: 0.8.2
+Version: 0.9.0
 Summary: Frequenz dispatch gRPC API and bindings
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-dispatch/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-dispatch
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-dispatch/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-dispatch/discussions/categories/support
```

### Comparing `frequenz-api-dispatch-0.8.2/README.md` & `frequenz-api-dispatch-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/ci.yaml` & `frequenz-api-dispatch-0.9.0/ci.yaml`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/proto/frequenz/api/dispatch/dispatch.proto` & `frequenz-api-dispatch-0.9.0/proto/frequenz/api/dispatch/dispatch.proto`

 * *Files 22% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 
 syntax = "proto3";
 
 package frequenz.api.dispatch;
 
 import "google/api/annotations.proto";
 import "google/protobuf/empty.proto";
+import "google/protobuf/struct.proto";
 import "google/protobuf/timestamp.proto";
 
 import "frequenz/api/common/components.proto";
 
-import "frequenz/api/dispatch/fcr/prequalification.proto";
-
 service DispatchService {
   // Returns a list of all dispatches
   rpc ListDispatches(DispatchFilter) returns (DispatchList) {
     option (google.api.http) = {
       get: "/v1/dispatches"
     };
   }
@@ -39,51 +38,48 @@
   rpc UpdateDispatch(DispatchUpdateRequest) returns (google.protobuf.Empty) {
     option (google.api.http) = {
       patch: "/v1/dispatches"
     };
   }
 }
 
-// Possible dispatch types
-enum DispatchType {
-  // Unspecified dispatch type, used mainly for error handling
-  DISPATCH_TYPE_UNSPECIFIED = 0;
-
-  // Shutdown dispatch event
-  DISPATCH_TYPE_SHUTDOWN = 1;
+// Message representing one dispatch
+message Dispatch {
+  // The dispatch identifier
+  uint64 id = 1;
 
-  // Charge battery dispatch event
-  DISPATCH_TYPE_BATTERY_CHARGE = 2;
+  // The microgrid identifier
+  uint64 microgrid_id = 2;
 
-  // Discharge battery dispatch event
-  DISPATCH_TYPE_BATTERY_DISCHARGE = 3;
+  // The dispatch type.
+  // Contains user-defined information about what "type" of dispatch this is.
+  // Downstream applications that consume the dispatch API are responsible for
+  // understanding and processing this field.
+  string type = 3;
 
-  // Frequency containment reserve dispatch event
-  DISPATCH_TYPE_FCR = 4;
+  // The start time
+  google.protobuf.Timestamp start_time = 4;
 
-  // FCR prequalification, charge test
-  DISPATCH_TYPE_FCR_PREQUALIFICATION_CHARGE = 5;
+  // The end time
+  google.protobuf.Timestamp end_time = 5;
 
-  // FCR prequalification, discharge test
-  DISPATCH_TYPE_FCR_PREQUALIFICATION_DISCHARGE = 6;
-}
+  // The component selector
+  DispatchComponentSelector selector = 6;
 
-// Possible dispatch statuses
-enum DispatchStatus {
-  // Unspecified dispatch status, used mainly for error handling
-  DISPATCH_STATUS_UNSPECIFIED = 0;
+  // The creation time
+  google.protobuf.Timestamp create_time = 7;
 
-  // Active dispatch status
-  DISPATCH_STATUS_ACTIVE = 1;
+  // The "active" status
+  bool is_active = 8;
 
-  // Inactive dispatch status
-  DISPATCH_STATUS_INACTIVE = 2;
+  // The "dry run" status
+  bool is_dry_run = 9;
 
-  // Simulated dispatch status
-  DISPATCH_STATUS_SIMULATE = 3;
+  // The dispatch payload
+  google.protobuf.Struct payload = 10;
 }
 
 // Filter parameter for specifying multiple time intervals
 message TimeIntervalFilter {
   // Filter by start_time >= this timestamp
   google.protobuf.Timestamp start_from = 1;
 
@@ -120,111 +116,88 @@
   // Filter by dispatch ID
   repeated uint64 ids = 1;
 
   // Filter by microgrid ID
   repeated uint64 microgrid_ids = 2;
 
   // Filter by dispatch type
-  repeated DispatchType types = 3;
+  repeated string types = 3;
 
   // Filter by component ID or category
   repeated DispatchComponentSelector selectors = 4;
 
   // Filter by time interval
   TimeIntervalFilter time_interval = 5;
-}
-
-message DispatchSettings {
-  oneof settings {
-    fcr.prequalification.FcrPrequalificationSettings fcr_prequal_settings = 1;
-  }
-}
-
-// Message representing one dispatch
-message Dispatch {
-  // The dispatch identifier
-  uint64 id = 1;
 
-  // The microgrid identifier
-  uint64 microgrid_id = 2;
+  // Filter by "active" status
+  optional bool is_active = 6;
 
-  // The type of dispatch
-  DispatchType type = 3;
-
-  // The start time
-  google.protobuf.Timestamp start_time = 4;
-
-  // The end time
-  google.protobuf.Timestamp end_time = 5;
-
-  // The component selector
-  DispatchComponentSelector selector = 6;
-
-  // The creation time
-  google.protobuf.Timestamp create_time = 7;
-
-  // The dispatch status
-  DispatchStatus status = 8;
-
-  // The dispatch settings
-  DispatchSettings settings = 9;
+  // Filter by "dry run" status
+  optional bool is_dry_run = 7;
 }
 
+
 // A list of dispatches
 message DispatchList {
   // The dispatches
   repeated Dispatch dispatches = 1;
 }
 
 // Message to create a new dispatch with the given attributes
 message DispatchCreateRequest {
   // The microgrid identifier
   uint64 microgrid_id = 1;
 
   // The type of dispatch
-  DispatchType type = 2;
+  string type = 2;
 
   // The start time
   google.protobuf.Timestamp start_time = 3;
 
   // The end time
   google.protobuf.Timestamp end_time = 4;
 
   // The component selector
   DispatchComponentSelector selector = 5;
 
-  // The dispatch status
-  DispatchStatus status = 6;
+  // The "active" status
+  bool is_active = 6;
 
-  // The dispatch settings
-  DispatchSettings settings = 7;
+  // The "dry run" status
+  bool is_dry_run = 7;
+
+  // The dispatch payload
+  google.protobuf.Struct payload = 8;
 }
 
 // Message to update the dispatch with the given ID, with the given attributes
 message DispatchUpdateRequest {
   // The dispatch identifier
   uint64 id = 1;
 
   // The microgrid identifier
   optional uint64 microgrid_id = 2;
 
   // The type of dispatch
-  optional DispatchType type = 3;
+  optional string type = 3;
 
   // The start time
-  optional google.protobuf.Timestamp start_time = 4;
+  google.protobuf.Timestamp start_time = 4;
 
   // The end time
-  optional google.protobuf.Timestamp end_time = 5;
+  google.protobuf.Timestamp end_time = 5;
 
   // The component selector
-  optional DispatchComponentSelector selector = 6;
+  DispatchComponentSelector selector = 6;
 
   // The creation time
-  optional google.protobuf.Timestamp create_time = 7;
+  google.protobuf.Timestamp create_time = 7;
+
+  // The "active" status
+  optional bool is_active = 8;
 
-  // The dispatch status
-  optional DispatchStatus status = 8;
+  // The "dry run" status
+  optional bool is_dry_run = 9;
 
-  // The dispatch settings
-  optional DispatchSettings settings = 9;
+  // The dispatch payload
+  google.protobuf.Struct payload = 10;
 }
```

### Comparing `frequenz-api-dispatch-0.8.2/py/frequenz_api_dispatch.egg-info/PKG-INFO` & `frequenz-api-dispatch-0.9.0/py/frequenz_api_dispatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-dispatch
-Version: 0.8.2
+Version: 0.9.0
 Summary: Frequenz dispatch gRPC API and bindings
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-dispatch/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-dispatch
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-dispatch/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-dispatch/discussions/categories/support
```

### Comparing `frequenz-api-dispatch-0.8.2/py/frequenz_api_dispatch.egg-info/SOURCES.txt` & `frequenz-api-dispatch-0.9.0/py/frequenz_api_dispatch.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 MANIFEST.in
 README.md
 RELEASE_NOTES.md
 ci.yaml
 pyproject.toml
 proto/frequenz/api/dispatch/dispatch.proto
-proto/frequenz/api/dispatch/fcr/prequalification.proto
 py/frequenz/api/dispatch/__init__.py
 py/frequenz/api/dispatch/py.typed
-py/frequenz/api/dispatch/fcr/__init__.py
 py/frequenz_api_dispatch.egg-info/PKG-INFO
 py/frequenz_api_dispatch.egg-info/SOURCES.txt
 py/frequenz_api_dispatch.egg-info/dependency_links.txt
 py/frequenz_api_dispatch.egg-info/requires.txt
 py/frequenz_api_dispatch.egg-info/top_level.txt
 submodules/api-common-protos/google/api/annotations.proto
 submodules/api-common-protos/google/api/auth.proto
```

### Comparing `frequenz-api-dispatch-0.8.2/py/frequenz_api_dispatch.egg-info/requires.txt` & `frequenz-api-dispatch-0.9.0/py/frequenz_api_dispatch.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/pyproject.toml` & `frequenz-api-dispatch-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/annotations.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/auth.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/auth.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/backend.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/backend.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/billing.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/billing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/client.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/client.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/config_change.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/config_change.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/consumer.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/consumer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/context.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/control.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/control.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/distribution.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/distribution.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/documentation.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/documentation.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/endpoint.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/endpoint.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/field_behavior.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/field_behavior.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/http.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/httpbody.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/httpbody.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/label.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/label.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/launch_stage.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/launch_stage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/log.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/log.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/logging.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/logging.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/metric.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/metric.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/monitored_resource.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/monitored_resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/monitoring.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/monitoring.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/quota.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/quota.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/resource.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/routing.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/routing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/service.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/service.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/source_info.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/source_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/system_parameter.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/system_parameter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/api/usage.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/api/usage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/cloud/extended_operations.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/cloud/extended_operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/iam/admin/v1/iam.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/iam/v1/iam_policy.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/iam/v1/options.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/iam/v1/options.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/iam/v1/policy.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/iam/v1/policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/logging/type/http_request.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/logging/type/http_request.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/logging/type/log_severity.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/logging/type/log_severity.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/longrunning/operations.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/longrunning/operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/rpc/code.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/rpc/code.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/rpc/context/attribute_context.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/rpc/error_details.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/rpc/error_details.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/rpc/status.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/calendar_period.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/calendar_period.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/color.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/color.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/date.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/date.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/datetime.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/datetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/dayofweek.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/dayofweek.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/expr.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/expr.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/fraction.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/fraction.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/latlng.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/latlng.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/money.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/money.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/month.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/month.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/postal_address.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/postal_address.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/quaternion.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/quaternion.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/api-common-protos/google/type/timeofday.proto` & `frequenz-api-dispatch-0.9.0/submodules/api-common-protos/google/type/timeofday.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto` & `frequenz-api-dispatch-0.9.0/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto` & `frequenz-api-dispatch-0.9.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.2/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto` & `frequenz-api-dispatch-0.9.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto`

 * *Files identical despite different names*

