# Comparing `tmp/cgcsdk-0.9.1.tar.gz` & `tmp/cgcsdk-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgcsdk-0.9.1.tar", last modified: Wed Jun 14 08:46:44 2023, max compression
+gzip compressed data, was "cgcsdk-0.9.2.tar", last modified: Mon Jul 17 12:09:53 2023, max compression
```

## Comparing `cgcsdk-0.9.1.tar` & `cgcsdk-0.9.2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.238045 cgcsdk-0.9.1/
--rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.9.1/LICENSE
--rw-rw-rw-   0        0        0      112 2023-06-13 11:20:10.000000 cgcsdk-0.9.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1101 2023-06-14 08:46:44.237157 cgcsdk-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:43.972209 cgcsdk-0.9.1/cgc/
--rw-rw-rw-   0        0        0      209 2023-06-14 08:41:05.000000 cgcsdk-0.9.1/cgc/.env
--rw-rw-rw-   0        0        0     4687 2023-06-14 08:43:44.000000 cgcsdk-0.9.1/cgc/CHANGELOG.md
--rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-0.9.1/cgc/__init__.py
--rw-rw-rw-   0        0        0     1377 2023-05-18 09:42:45.000000 cgcsdk-0.9.1/cgc/cgc.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:43.987927 cgcsdk-0.9.1/cgc/commands/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.1/cgc/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.004788 cgcsdk-0.9.1/cgc/commands/auth/
--rw-rw-rw-   0        0        0      399 2023-05-18 12:02:14.000000 cgcsdk-0.9.1/cgc/commands/auth/__init__.py
--rw-rw-rw-   0        0        0     2824 2023-05-19 11:45:44.000000 cgcsdk-0.9.1/cgc/commands/auth/auth_cmd.py
--rw-rw-rw-   0        0        0     1783 2023-05-19 13:13:56.000000 cgcsdk-0.9.1/cgc/commands/auth/auth_responses.py
--rw-rw-rw-   0        0        0     3893 2023-05-18 13:54:23.000000 cgcsdk-0.9.1/cgc/commands/auth/auth_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.030461 cgcsdk-0.9.1/cgc/commands/billing/
--rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-0.9.1/cgc/commands/billing/__init__.py
--rw-rw-rw-   0        0        0     3450 2023-04-14 14:28:08.000000 cgcsdk-0.9.1/cgc/commands/billing/billing_cmd.py
--rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-0.9.1/cgc/commands/billing/billing_responses.py
--rw-rw-rw-   0        0        0     4711 2023-06-14 08:36:45.000000 cgcsdk-0.9.1/cgc/commands/billing/billing_utils.py
--rw-rw-rw-   0        0        0     4061 2023-05-23 09:09:29.000000 cgcsdk-0.9.1/cgc/commands/cgc_cmd.py
--rw-rw-rw-   0        0        0     2026 2023-04-21 11:24:43.000000 cgcsdk-0.9.1/cgc/commands/cgc_cmd_responses.py
--rw-rw-rw-   0        0        0     1207 2023-05-19 10:34:54.000000 cgcsdk-0.9.1/cgc/commands/cgc_helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.057307 cgcsdk-0.9.1/cgc/commands/compute/
--rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.9.1/cgc/commands/compute/__init__.py
--rw-rw-rw-   0        0        0     4783 2023-04-18 09:56:45.000000 cgcsdk-0.9.1/cgc/commands/compute/compute_cmd.py
--rw-rw-rw-   0        0        0      959 2023-06-13 11:20:10.000000 cgcsdk-0.9.1/cgc/commands/compute/compute_models.py
--rw-rw-rw-   0        0        0     5175 2023-04-18 11:02:46.000000 cgcsdk-0.9.1/cgc/commands/compute/compute_responses.py
--rw-rw-rw-   0        0        0     3353 2023-04-14 14:28:08.000000 cgcsdk-0.9.1/cgc/commands/compute/compute_utills.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.064932 cgcsdk-0.9.1/cgc/commands/db/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.9.1/cgc/commands/db/__init__.py
--rw-rw-rw-   0        0        0     3293 2023-04-18 10:50:41.000000 cgcsdk-0.9.1/cgc/commands/db/db_cmd.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.071689 cgcsdk-0.9.1/cgc/commands/debug/
--rw-rw-rw-   0        0        0        0 2023-04-18 09:56:45.000000 cgcsdk-0.9.1/cgc/commands/debug/__init__.py
--rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-0.9.1/cgc/commands/debug/debug_cmd.py
--rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.9.1/cgc/commands/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.077743 cgcsdk-0.9.1/cgc/commands/resource/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.9.1/cgc/commands/resource/__init__.py
--rw-rw-rw-   0        0        0     3156 2023-04-18 09:56:45.000000 cgcsdk-0.9.1/cgc/commands/resource/resource_cmd.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.094389 cgcsdk-0.9.1/cgc/commands/volume/
--rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.9.1/cgc/commands/volume/__init__.py
--rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.9.1/cgc/commands/volume/data_model.py
--rw-rw-rw-   0        0        0     6784 2023-03-22 14:29:23.000000 cgcsdk-0.9.1/cgc/commands/volume/volume_cmd.py
--rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.9.1/cgc/commands/volume/volume_responses.py
--rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.9.1/cgc/commands/volume/volume_utils.py
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.1/cgc/config.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.110643 cgcsdk-0.9.1/cgc/sdk/
--rw-rw-rw-   0        0        0      194 2023-04-18 09:56:45.000000 cgcsdk-0.9.1/cgc/sdk/__init__.py
--rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-0.9.1/cgc/sdk/handlers.py
--rw-rw-rw-   0        0        0     7221 2023-04-18 13:47:14.000000 cgcsdk-0.9.1/cgc/sdk/mongodb.py
--rw-rw-rw-   0        0        0     1637 2023-04-18 10:57:57.000000 cgcsdk-0.9.1/cgc/sdk/postgresql.py
--rw-rw-rw-   0        0        0     2840 2023-05-29 15:06:35.000000 cgcsdk-0.9.1/cgc/sdk/redis.py
--rw-rw-rw-   0        0        0     1452 2023-05-31 13:31:37.000000 cgcsdk-0.9.1/cgc/server.crt
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.116837 cgcsdk-0.9.1/cgc/telemetry/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.1/cgc/telemetry/__init__.py
--rw-rw-rw-   0        0        0     3175 2023-05-18 12:51:21.000000 cgcsdk-0.9.1/cgc/telemetry/basic.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.123399 cgcsdk-0.9.1/cgc/tests/
--rw-rw-rw-   0        0        0   102744 2023-04-18 11:02:26.000000 cgcsdk-0.9.1/cgc/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.156525 cgcsdk-0.9.1/cgc/tests/desired_responses/
--rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.9.1/cgc/tests/desired_responses/test_billing_invoice.txt
--rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.9.1/cgc/tests/desired_responses/test_billing_status.txt
--rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.9.1/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
--rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.9.1/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
--rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.9.1/cgc/tests/desired_responses/test_compute_list.txt
--rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.9.1/cgc/tests/desired_responses/test_compute_list_no_labels.txt
--rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.9.1/cgc/tests/desired_responses/test_tabulate_response.txt
--rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.9.1/cgc/tests/desired_responses/test_volume_list.txt
--rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-0.9.1/cgc/tests/responses_tests.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.189977 cgcsdk-0.9.1/cgc/utils/
--rw-rw-rw-   0        0        0     3466 2023-06-13 12:13:50.000000 cgcsdk-0.9.1/cgc/utils/__init__.py
--rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.9.1/cgc/utils/click_group.py
--rw-rw-rw-   0        0        0     2729 2023-05-23 09:02:22.000000 cgcsdk-0.9.1/cgc/utils/config_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.199734 cgcsdk-0.9.1/cgc/utils/consts/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.1/cgc/utils/consts/__init__.py
--rw-rw-rw-   0        0        0     1221 2023-06-13 11:20:10.000000 cgcsdk-0.9.1/cgc/utils/consts/env_consts.py
--rw-rw-rw-   0        0        0     1218 2023-06-13 09:54:33.000000 cgcsdk-0.9.1/cgc/utils/consts/message_consts.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.212955 cgcsdk-0.9.1/cgc/utils/cryptography/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.1/cgc/utils/cryptography/__init__.py
--rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.9.1/cgc/utils/cryptography/aes_crypto.py
--rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.9.1/cgc/utils/cryptography/encryption_module.py
--rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.9.1/cgc/utils/cryptography/rsa_crypto.py
--rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.9.1/cgc/utils/custom_exceptions.py
--rw-rw-rw-   0        0        0     1773 2023-05-23 09:05:26.000000 cgcsdk-0.9.1/cgc/utils/message_utils.py
--rw-rw-rw-   0        0        0     2488 2023-05-23 09:03:57.000000 cgcsdk-0.9.1/cgc/utils/prepare_headers.py
--rw-rw-rw-   0        0        0     2050 2023-06-13 11:20:10.000000 cgcsdk-0.9.1/cgc/utils/requests_helper.py
--rw-rw-rw-   0        0        0     4913 2023-05-19 13:09:48.000000 cgcsdk-0.9.1/cgc/utils/response_utils.py
--rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.9.1/cgc/utils/update.py
--rw-rw-rw-   0        0        0     3267 2023-06-13 11:20:10.000000 cgcsdk-0.9.1/cgc/utils/version_control.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:46:44.233230 cgcsdk-0.9.1/cgcsdk.egg-info/
--rw-rw-rw-   0        0        0     1101 2023-06-14 08:46:43.000000 cgcsdk-0.9.1/cgcsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2446 2023-06-14 08:46:43.000000 cgcsdk-0.9.1/cgcsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:46:43.000000 cgcsdk-0.9.1/cgcsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-14 08:46:43.000000 cgcsdk-0.9.1/cgcsdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      124 2023-06-14 08:46:43.000000 cgcsdk-0.9.1/cgcsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-14 08:46:43.000000 cgcsdk-0.9.1/cgcsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.9.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 08:46:44.239027 cgcsdk-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0     2096 2023-06-13 11:20:10.000000 cgcsdk-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:53.191239 cgcsdk-0.9.2/
+-rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.9.2/LICENSE
+-rw-rw-rw-   0        0        0      112 2023-06-13 11:20:10.000000 cgcsdk-0.9.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1101 2023-07-17 12:09:53.189423 cgcsdk-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.9.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:52.747890 cgcsdk-0.9.2/cgc/
+-rw-rw-rw-   0        0        0      209 2023-07-17 12:07:43.000000 cgcsdk-0.9.2/cgc/.env
+-rw-rw-rw-   0        0        0     4881 2023-07-17 12:07:43.000000 cgcsdk-0.9.2/cgc/CHANGELOG.md
+-rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-0.9.2/cgc/__init__.py
+-rw-rw-rw-   0        0        0     1377 2023-05-18 09:42:45.000000 cgcsdk-0.9.2/cgc/cgc.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:52.770366 cgcsdk-0.9.2/cgc/commands/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.2/cgc/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:52.797707 cgcsdk-0.9.2/cgc/commands/auth/
+-rw-rw-rw-   0        0        0      399 2023-05-18 12:02:14.000000 cgcsdk-0.9.2/cgc/commands/auth/__init__.py
+-rw-rw-rw-   0        0        0     2824 2023-05-19 11:45:44.000000 cgcsdk-0.9.2/cgc/commands/auth/auth_cmd.py
+-rw-rw-rw-   0        0        0     1783 2023-05-19 13:13:56.000000 cgcsdk-0.9.2/cgc/commands/auth/auth_responses.py
+-rw-rw-rw-   0        0        0     3893 2023-05-18 13:54:23.000000 cgcsdk-0.9.2/cgc/commands/auth/auth_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:52.825395 cgcsdk-0.9.2/cgc/commands/billing/
+-rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-0.9.2/cgc/commands/billing/__init__.py
+-rw-rw-rw-   0        0        0     3450 2023-04-14 14:28:08.000000 cgcsdk-0.9.2/cgc/commands/billing/billing_cmd.py
+-rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-0.9.2/cgc/commands/billing/billing_responses.py
+-rw-rw-rw-   0        0        0     4711 2023-06-14 08:36:45.000000 cgcsdk-0.9.2/cgc/commands/billing/billing_utils.py
+-rw-rw-rw-   0        0        0     4061 2023-05-23 09:09:29.000000 cgcsdk-0.9.2/cgc/commands/cgc_cmd.py
+-rw-rw-rw-   0        0        0     2026 2023-04-21 11:24:43.000000 cgcsdk-0.9.2/cgc/commands/cgc_cmd_responses.py
+-rw-rw-rw-   0        0        0     1207 2023-05-19 10:34:54.000000 cgcsdk-0.9.2/cgc/commands/cgc_helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:52.855129 cgcsdk-0.9.2/cgc/commands/compute/
+-rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.9.2/cgc/commands/compute/__init__.py
+-rw-rw-rw-   0        0        0     5757 2023-07-17 12:07:43.000000 cgcsdk-0.9.2/cgc/commands/compute/compute_cmd.py
+-rw-rw-rw-   0        0        0      959 2023-06-13 11:20:10.000000 cgcsdk-0.9.2/cgc/commands/compute/compute_models.py
+-rw-rw-rw-   0        0        0     5169 2023-07-17 12:07:43.000000 cgcsdk-0.9.2/cgc/commands/compute/compute_responses.py
+-rw-rw-rw-   0        0        0     3353 2023-04-14 14:28:08.000000 cgcsdk-0.9.2/cgc/commands/compute/compute_utills.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:52.867900 cgcsdk-0.9.2/cgc/commands/db/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.9.2/cgc/commands/db/__init__.py
+-rw-rw-rw-   0        0        0     3293 2023-04-18 10:50:41.000000 cgcsdk-0.9.2/cgc/commands/db/db_cmd.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:52.880716 cgcsdk-0.9.2/cgc/commands/debug/
+-rw-rw-rw-   0        0        0        0 2023-04-18 09:56:45.000000 cgcsdk-0.9.2/cgc/commands/debug/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-0.9.2/cgc/commands/debug/debug_cmd.py
+-rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.9.2/cgc/commands/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:52.893296 cgcsdk-0.9.2/cgc/commands/resource/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.9.2/cgc/commands/resource/__init__.py
+-rw-rw-rw-   0        0        0     3156 2023-04-18 09:56:45.000000 cgcsdk-0.9.2/cgc/commands/resource/resource_cmd.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:52.925088 cgcsdk-0.9.2/cgc/commands/volume/
+-rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.9.2/cgc/commands/volume/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.9.2/cgc/commands/volume/data_model.py
+-rw-rw-rw-   0        0        0     6839 2023-07-17 12:07:43.000000 cgcsdk-0.9.2/cgc/commands/volume/volume_cmd.py
+-rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.9.2/cgc/commands/volume/volume_responses.py
+-rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.9.2/cgc/commands/volume/volume_utils.py
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.2/cgc/config.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:52.948195 cgcsdk-0.9.2/cgc/sdk/
+-rw-rw-rw-   0        0        0      194 2023-04-18 09:56:45.000000 cgcsdk-0.9.2/cgc/sdk/__init__.py
+-rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-0.9.2/cgc/sdk/handlers.py
+-rw-rw-rw-   0        0        0     7221 2023-04-18 13:47:14.000000 cgcsdk-0.9.2/cgc/sdk/mongodb.py
+-rw-rw-rw-   0        0        0     1637 2023-04-18 10:57:57.000000 cgcsdk-0.9.2/cgc/sdk/postgresql.py
+-rw-rw-rw-   0        0        0     2844 2023-07-17 12:07:43.000000 cgcsdk-0.9.2/cgc/sdk/redis.py
+-rw-rw-rw-   0        0        0     1452 2023-05-31 13:31:37.000000 cgcsdk-0.9.2/cgc/server.crt
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:52.959240 cgcsdk-0.9.2/cgc/telemetry/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.2/cgc/telemetry/__init__.py
+-rw-rw-rw-   0        0        0     3175 2023-05-18 12:51:21.000000 cgcsdk-0.9.2/cgc/telemetry/basic.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:52.967868 cgcsdk-0.9.2/cgc/tests/
+-rw-rw-rw-   0        0        0   102743 2023-07-17 12:07:43.000000 cgcsdk-0.9.2/cgc/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:53.010320 cgcsdk-0.9.2/cgc/tests/desired_responses/
+-rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.9.2/cgc/tests/desired_responses/test_billing_invoice.txt
+-rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.9.2/cgc/tests/desired_responses/test_billing_status.txt
+-rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.9.2/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
+-rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.9.2/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
+-rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.9.2/cgc/tests/desired_responses/test_compute_list.txt
+-rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.9.2/cgc/tests/desired_responses/test_compute_list_no_labels.txt
+-rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.9.2/cgc/tests/desired_responses/test_tabulate_response.txt
+-rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.9.2/cgc/tests/desired_responses/test_volume_list.txt
+-rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-0.9.2/cgc/tests/responses_tests.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:53.056630 cgcsdk-0.9.2/cgc/utils/
+-rw-rw-rw-   0        0        0     3466 2023-06-13 12:13:50.000000 cgcsdk-0.9.2/cgc/utils/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.9.2/cgc/utils/click_group.py
+-rw-rw-rw-   0        0        0     2729 2023-05-23 09:02:22.000000 cgcsdk-0.9.2/cgc/utils/config_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:53.080412 cgcsdk-0.9.2/cgc/utils/consts/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.2/cgc/utils/consts/__init__.py
+-rw-rw-rw-   0        0        0     1221 2023-06-13 11:20:10.000000 cgcsdk-0.9.2/cgc/utils/consts/env_consts.py
+-rw-rw-rw-   0        0        0     1218 2023-06-13 09:54:33.000000 cgcsdk-0.9.2/cgc/utils/consts/message_consts.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:53.138531 cgcsdk-0.9.2/cgc/utils/cryptography/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.9.2/cgc/utils/cryptography/__init__.py
+-rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.9.2/cgc/utils/cryptography/aes_crypto.py
+-rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.9.2/cgc/utils/cryptography/encryption_module.py
+-rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.9.2/cgc/utils/cryptography/rsa_crypto.py
+-rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.9.2/cgc/utils/custom_exceptions.py
+-rw-rw-rw-   0        0        0     1773 2023-05-23 09:05:26.000000 cgcsdk-0.9.2/cgc/utils/message_utils.py
+-rw-rw-rw-   0        0        0     2488 2023-05-23 09:03:57.000000 cgcsdk-0.9.2/cgc/utils/prepare_headers.py
+-rw-rw-rw-   0        0        0     2050 2023-06-13 11:20:10.000000 cgcsdk-0.9.2/cgc/utils/requests_helper.py
+-rw-rw-rw-   0        0        0     4913 2023-05-19 13:09:48.000000 cgcsdk-0.9.2/cgc/utils/response_utils.py
+-rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.9.2/cgc/utils/update.py
+-rw-rw-rw-   0        0        0     3267 2023-06-13 11:20:10.000000 cgcsdk-0.9.2/cgc/utils/version_control.py
+drwxrwxrwx   0        0        0        0 2023-07-17 12:09:53.184256 cgcsdk-0.9.2/cgcsdk.egg-info/
+-rw-rw-rw-   0        0        0     1101 2023-07-17 12:09:52.000000 cgcsdk-0.9.2/cgcsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2446 2023-07-17 12:09:52.000000 cgcsdk-0.9.2/cgcsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 12:09:52.000000 cgcsdk-0.9.2/cgcsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-17 12:09:52.000000 cgcsdk-0.9.2/cgcsdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      124 2023-07-17 12:09:52.000000 cgcsdk-0.9.2/cgcsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-17 12:09:52.000000 cgcsdk-0.9.2/cgcsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 12:09:53.191239 cgcsdk-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     2096 2023-06-13 11:20:10.000000 cgcsdk-0.9.2/setup.py
```

### Comparing `cgcsdk-0.9.1/PKG-INFO` & `cgcsdk-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.9.1
+Version: 0.9.2
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.9.1/cgc/CHANGELOG.md` & `cgcsdk-0.9.2/cgc/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # Change Log
 
+## 0.9.2
+
+Release on July 17, 2023
+
+* hotfix to message when cgc compute filebrowser create due to default username changes
+* added notes for compute.create in code
+* hotfix for cgc.sdk.redis
+
 ## 0.9.1
 
-Release on June 14,2023
+Release on June 14, 2023
 
 * cgc billing - updated which values from response are taken to show
   * cost_total in billing was shown correctly - no changes
   * start, end, time: updated with correct key:value pairs from response
 
 ## 0.9.0
```

### Comparing `cgcsdk-0.9.1/cgc/cgc.py` & `cgcsdk-0.9.2/cgc/cgc.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/commands/auth/auth_cmd.py` & `cgcsdk-0.9.2/cgc/commands/auth/auth_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/commands/auth/auth_responses.py` & `cgcsdk-0.9.2/cgc/commands/auth/auth_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/commands/auth/auth_utils.py` & `cgcsdk-0.9.2/cgc/commands/auth/auth_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/commands/billing/__init__.py` & `cgcsdk-0.9.2/cgc/commands/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/commands/billing/billing_cmd.py` & `cgcsdk-0.9.2/cgc/commands/billing/billing_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/commands/billing/billing_responses.py` & `cgcsdk-0.9.2/cgc/commands/billing/billing_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/commands/billing/billing_utils.py` & `cgcsdk-0.9.2/cgc/commands/billing/billing_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/commands/cgc_cmd.py` & `cgcsdk-0.9.2/cgc/commands/cgc_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/commands/cgc_cmd_responses.py` & `cgcsdk-0.9.2/cgc/commands/cgc_cmd_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/commands/cgc_helpers.py` & `cgcsdk-0.9.2/cgc/commands/cgc_helpers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/commands/compute/compute_cmd.py` & `cgcsdk-0.9.2/cgc/commands/db/db_cmd.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,32 @@
 import json
 import click
 
-from cgc.commands.compute.compute_models import EntityList, GPUsList
-from cgc.commands.compute.compute_responses import (
-    compute_create_filebrowser_response,
-    compute_create_response,
-    compute_list_response,
-)
+from cgc.commands.compute.compute_responses import compute_list_response
+from cgc.commands.compute.compute_models import DatabasesList
+from cgc.commands.compute.compute_responses import compute_create_response
 from cgc.commands.compute.compute_utills import compute_create_payload
+from cgc.commands.resource.resource_cmd import resource_delete
 from cgc.utils.prepare_headers import get_api_url_and_prepare_headers
 from cgc.utils.response_utils import retrieve_and_validate_response_send_metric
 from cgc.utils.click_group import CustomGroup, CustomCommand
 from cgc.utils.requests_helper import call_api, EndpointTypes
-from cgc.commands.resource.resource_cmd import resource_delete
-
 
-@click.group(name="compute", cls=CustomGroup)
-def compute_group():
-    """
-    Management of compute resources.
-    """
 
-
-@click.group(name="filebrowser", cls=CustomGroup)
-def filebrowser_group():
+@click.group(name="db", cls=CustomGroup)
+def db_group():
     """
-    Management of filebrowser.
+    Management of db resources.
     """
 
 
-@filebrowser_group.command("create", cls=CustomCommand)
-def compute_filebrowser_create():
-    """Create a filebrowser service"""
-    api_url, headers = get_api_url_and_prepare_headers()
-    url = f"{api_url}/v1/api/resource/filebrowser_create"
-    metric = "compute.create_filebrowser"
-    __payload = {"puid": 0, "pgid": 0}
-    __res = call_api(
-        request=EndpointTypes.post,
-        url=url,
-        headers=headers,
-        data=json.dumps(__payload),
-    )
-    click.echo(
-        compute_create_filebrowser_response(
-            retrieve_and_validate_response_send_metric(__res, metric)
-        )
-    )
-
-
-@filebrowser_group.command("delete", cls=CustomCommand)
-def compute_filebrowser_delete():
-    """Delete a filebrowser service"""
-    resource_delete("filebrowser")
-
-
-@compute_group.command("create", cls=CustomCommand)
-@click.argument("entity", type=click.Choice(EntityList.get_list()))
+@db_group.command("create", cls=CustomCommand)
+@click.argument("entity", type=click.Choice(DatabasesList.get_list()))
 @click.option("-n", "--name", "name", type=click.STRING, required=True)
 @click.option(
-    "-g",
-    "--gpu",
-    "gpu",
-    type=click.INT,
-    default=0,
-    help="How much GPU cards app will use",
-)
-@click.option(
-    "-gt",
-    "--gpu-type",
-    "gpu_type",
-    type=click.Choice(GPUsList.get_list(), case_sensitive=False),
-    default="A5000",
-    help="Graphic card used by the app",
-)
-@click.option(
     "-c",
     "--cpu",
     "cpu",
     type=click.INT,
     default=1,
     help="How much CPU cores app can use",
 )
@@ -91,92 +39,83 @@
     help="How much Gi RAM app can use",
 )
 @click.option(
     "-v",
     "--volume",
     "volumes",
     multiple=True,
-    help="List of volume names to be mounted with default mount path",
+    help="Volume name to be mounted with default mount path",
 )
-def compute_create(
+def db_create(
     entity: str,
-    gpu: int,
-    gpu_type: str,
     cpu: int,
     memory: int,
     volumes: list[str],
     name: str,
 ):
     """
     Create an app in user namespace.
     \f
     :param entity: name of entity to create
     :type entity: str
-    :param gpu: number of gpus to be used by app
-    :type gpu: int
     :param cpu: number of cores to be used by app
     :type cpu: int
     :param memory: GB of memory to be used by app
     :type memory: int
     :param volumes: list of volumes to mount
     :type volumes: list[str]
     :param name: name of app
     :type name: str
     """
     api_url, headers = get_api_url_and_prepare_headers()
     url = f"{api_url}/v1/api/resource/create"
-    metric = "compute.create"
+    metric = "db.create"
     __payload = compute_create_payload(
         name=name,
         entity=entity,
         cpu=cpu,
         memory=memory,
-        gpu=gpu,
         volumes=volumes,
-        gpu_type=gpu_type,
     )
     __res = call_api(
         request=EndpointTypes.post,
         url=url,
         headers=headers,
         data=json.dumps(__payload),
     )
     click.echo(
         compute_create_response(
             retrieve_and_validate_response_send_metric(__res, metric)
         )
     )
 
 
-@compute_group.command("delete", cls=CustomCommand)
+@db_group.command("delete", cls=CustomCommand)
 @click.argument("name", type=click.STRING)
-def compute_delete_cmd(name: str):
+def db_delete_cmd(name: str):
     """
     Delete an app from user namespace.
     \f
     :param name: name of app to delete
     :type name: str
     """
     resource_delete(name)
 
 
-compute_group.add_command(filebrowser_group)
-
-
-@compute_group.command("list", cls=CustomCommand)
+@db_group.command("list", cls=CustomCommand)
 @click.option(
     "-d", "--detailed", "detailed", type=click.BOOL, is_flag=True, default=False
 )
 def resource_list(detailed: bool):
     """
     List all apps for user namespace.
     """
     api_url, headers = get_api_url_and_prepare_headers()
-    url = f"{api_url}/v1/api/resource/list?resource_type=compute"
-    metric = "compute.list"
+    url = f"{api_url}/v1/api/resource/list?resource_type=db"
+    metric = "db.list"
     __res = call_api(
         request=EndpointTypes.get,
         url=url,
         headers=headers,
     )
     table = compute_list_response(
         detailed,
```

### Comparing `cgcsdk-0.9.1/cgc/commands/compute/compute_models.py` & `cgcsdk-0.9.2/cgc/commands/compute/compute_models.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/commands/compute/compute_responses.py` & `cgcsdk-0.9.2/cgc/commands/compute/compute_responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     :return: Response string.
     :rtype: str
     """
 
     namespace = data["details"]["namespace"]
     app_url = data["details"]["created_template"]["pod_url"]
     app_token = data["details"]["created_template"]["app_token"]
-    return f"Filebrowser creation started!\nWill be accessible at: {app_url}\nUsername: {namespace}\nPassword: {app_token}"
+    return f"Filebrowser creation started!\nWill be accessible at: {app_url}\nUsername: admin\nPassword: {app_token}"
 
 
 @key_error_decorator_for_helpers
 def compute_create_response(data: dict) -> str:
     """Create response string for compute create command.
 
     :param response: dict object from API response.
```

### Comparing `cgcsdk-0.9.1/cgc/commands/compute/compute_utills.py` & `cgcsdk-0.9.2/cgc/commands/compute/compute_utills.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/commands/db/db_cmd.py` & `cgcsdk-0.9.2/cgc/commands/resource/resource_cmd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,125 +1,100 @@
-import json
 import click
+import json
+
+from cgc.commands.compute.compute_models import EntityList, DatabasesList
+from cgc.commands.compute.compute_responses import (
+    template_list_response,
+    template_get_start_path_response,
+    compute_restart_response,
+    compute_delete_response,
+)
+
+from cgc.commands.compute.compute_utills import compute_delete_payload
 
-from cgc.commands.compute.compute_responses import compute_list_response
-from cgc.commands.compute.compute_models import DatabasesList
-from cgc.commands.compute.compute_responses import compute_create_response
-from cgc.commands.compute.compute_utills import compute_create_payload
-from cgc.commands.resource.resource_cmd import resource_delete
 from cgc.utils.prepare_headers import get_api_url_and_prepare_headers
 from cgc.utils.response_utils import retrieve_and_validate_response_send_metric
 from cgc.utils.click_group import CustomGroup, CustomCommand
 from cgc.utils.requests_helper import call_api, EndpointTypes
 
 
-@click.group(name="db", cls=CustomGroup)
-def db_group():
+@click.group(name="resource", cls=CustomGroup, hidden=True)
+def resource_group():
     """
-    Management of db resources.
+    Management of templates.
     """
 
 
-@db_group.command("create", cls=CustomCommand)
-@click.argument("entity", type=click.Choice(DatabasesList.get_list()))
-@click.option("-n", "--name", "name", type=click.STRING, required=True)
-@click.option(
-    "-c",
-    "--cpu",
-    "cpu",
-    type=click.INT,
-    default=1,
-    help="How much CPU cores app can use",
-)
-@click.option(
-    "-m",
-    "--memory",
-    "memory",
-    type=click.INT,
-    default=2,
-    help="How much Gi RAM app can use",
-)
-@click.option(
-    "-v",
-    "--volume",
-    "volumes",
-    multiple=True,
-    help="Volume name to be mounted with default mount path",
+@resource_group.command("list_templates", cls=CustomCommand)
+def template_list():
+    """Lists all available templates"""
+    api_url, headers = get_api_url_and_prepare_headers()
+    url = f"{api_url}/v1/api/resource/list_available_templates"
+    metric = "resource.template.list"
+    __res = call_api(request=EndpointTypes.get, url=url, headers=headers)
+    click.echo(
+        template_list_response(
+            retrieve_and_validate_response_send_metric(__res, metric)
+        )
+    )
+
+
+@resource_group.command("get_start_path", cls=CustomCommand)
+@click.argument(
+    "template", type=click.Choice([*EntityList.get_list(), *DatabasesList.get_list()])
 )
-def db_create(
-    entity: str,
-    cpu: int,
-    memory: int,
-    volumes: list[str],
-    name: str,
-):
-    """
-    Create an app in user namespace.
-    \f
-    :param entity: name of entity to create
-    :type entity: str
-    :param cpu: number of cores to be used by app
-    :type cpu: int
-    :param memory: GB of memory to be used by app
-    :type memory: int
-    :param volumes: list of volumes to mount
-    :type volumes: list[str]
-    :param name: name of app
-    :type name: str
-    """
+def template_get_start_path(template: str):
+    """Displays start path of specified template"""
     api_url, headers = get_api_url_and_prepare_headers()
-    url = f"{api_url}/v1/api/resource/create"
-    metric = "db.create"
-    __payload = compute_create_payload(
-        name=name,
-        entity=entity,
-        cpu=cpu,
-        memory=memory,
-        volumes=volumes,
+    url = f"{api_url}/v1/api/resource/get_template_start_path?template_name={template}"
+    metric = "resource.template.get_start_path"
+    __res = call_api(request=EndpointTypes.get, url=url, headers=headers)
+    click.echo(
+        template_get_start_path_response(
+            retrieve_and_validate_response_send_metric(__res, metric)
+        )
     )
+
+
+@resource_group.command("restart", cls=CustomCommand)
+@click.argument("name", type=click.STRING)
+def compute_restart(name: str):
+    """Restarts the specified app"""
+    api_url, headers = get_api_url_and_prepare_headers()
+    url = f"{api_url}/v1/api/resource/restart"
+    metric = "resource.restart"
+    __payload = {"name": name}
     __res = call_api(
         request=EndpointTypes.post,
         url=url,
         headers=headers,
         data=json.dumps(__payload),
     )
     click.echo(
-        compute_create_response(
+        compute_restart_response(
             retrieve_and_validate_response_send_metric(__res, metric)
         )
     )
 
 
-@db_group.command("delete", cls=CustomCommand)
-@click.argument("name", type=click.STRING)
-def db_delete_cmd(name: str):
+def resource_delete(name: str):
     """
-    Delete an app from user namespace.
+    Delete an app using backend endpoint.
     \f
     :param name: name of app to delete
     :type name: str
     """
-    resource_delete(name)
-
-
-@db_group.command("list", cls=CustomCommand)
-@click.option(
-    "-d", "--detailed", "detailed", type=click.BOOL, is_flag=True, default=False
-)
-def resource_list(detailed: bool):
-    """
-    List all apps for user namespace.
-    """
     api_url, headers = get_api_url_and_prepare_headers()
-    url = f"{api_url}/v1/api/resource/list?resource_type=db"
-    metric = "db.list"
+    url = f"{api_url}/v1/api/resource/delete"
+    metric = "resource.delete"
+    __payload = compute_delete_payload(name=name)
     __res = call_api(
-        request=EndpointTypes.get,
+        request=EndpointTypes.delete,
         url=url,
         headers=headers,
+        data=json.dumps(__payload),
     )
-    table = compute_list_response(
-        detailed,
-        retrieve_and_validate_response_send_metric(__res, metric),
+    click.echo(
+        compute_delete_response(
+            retrieve_and_validate_response_send_metric(__res, metric)
+        )
     )
-
-    click.echo(table)
```

### Comparing `cgcsdk-0.9.1/cgc/commands/volume/data_model.py` & `cgcsdk-0.9.2/cgc/commands/volume/data_model.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/commands/volume/volume_cmd.py` & `cgcsdk-0.9.2/cgc/commands/volume/volume_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,22 @@
     click.echo(
         volume_list_response(retrieve_and_validate_response_send_metric(__res, metric))
     )
 
 
 @volume_group.command("create", cls=CustomCommand)
 @click.argument("name")
-@click.option("-s", "--size", "size", type=click.IntRange(1, 1000), required=True)
+@click.option(
+    "-s",
+    "--size",
+    "size",
+    help="Volume size in GiB",
+    type=click.IntRange(1, 1000),
+    required=True,
+)
 @click.option(
     "-t",
     "--type",
     "disk_type",
     type=click.Choice(["ssd", "nvme"]),
     default="ssd",
     help="Type of disk",
@@ -67,15 +74,15 @@
     help="Volume access mode",
 )
 def volume_create(name: str, size: int, disk_type: str, access: str):
     """Create volume in user namespace.
     \f
     :param name: name of volume
     :type name: str
-    :param size: size of volume in GB
+    :param size: size of volume in GiB
     :type size: int
     :param type: type of volume - HDD, SSD or NVMe
     :type type: str
     :param access: access type of volume - RWO or RWX
     :type access: str
     """
     api_url, headers = get_api_url_and_prepare_headers()
```

### Comparing `cgcsdk-0.9.1/cgc/commands/volume/volume_responses.py` & `cgcsdk-0.9.2/cgc/commands/volume/volume_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/commands/volume/volume_utils.py` & `cgcsdk-0.9.2/cgc/commands/volume/volume_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/sdk/handlers.py` & `cgcsdk-0.9.2/cgc/sdk/handlers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/sdk/mongodb.py` & `cgcsdk-0.9.2/cgc/sdk/mongodb.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/sdk/postgresql.py` & `cgcsdk-0.9.2/cgc/sdk/postgresql.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/sdk/redis.py` & `cgcsdk-0.9.2/cgc/sdk/redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,8 +84,8 @@
                 init_access(True)
     except NameError:
         if not async_client:
             init_access()
         else:
             init_access(True)
         pass
-    return _redis_access if async_client else _redis_access_async
+    return _redis_access if not async_client else _redis_access_async
```

### Comparing `cgcsdk-0.9.1/cgc/server.crt` & `cgcsdk-0.9.2/cgc/server.crt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/telemetry/basic.py` & `cgcsdk-0.9.2/cgc/telemetry/basic.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/tests/__init__.py` & `cgcsdk-0.9.2/cgc/tests/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1805,15 +1805,15 @@
     )
     test_compute_get_start_path = "Start path for datascience-jupyter: /home/jovyan."
     test_compute_list_empty = "[33mNo apps to list.[0m"
     test_compute_list_no_labels = ""
     test_compute_create_filebrowser = (
         "Filebrowser creation started!\n"
         "Will be accessible at: https://filebrowser.pytest.dev.quantdevlabs.com\n"
-        "Username: pytest\n"
+        "Username: admin\n"
         "Password: 9bb9c88f8fc14eadba5c5fbdafc06275"
     )
     test_compute_create = (
         "nvidia-pytorch app test1 creation started!\n"
         "Will be accessible at: https://test1.pytest.dev.quantdevlabs.com\n"
         "App token: 1ce03c31ab9c40df8594d97b301eaaea\n"
         "To monitor the startup status use command: cgc compute list"
```

### Comparing `cgcsdk-0.9.1/cgc/tests/desired_responses/test_billing_invoice.txt` & `cgcsdk-0.9.2/cgc/tests/desired_responses/test_billing_invoice.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/tests/desired_responses/test_billing_status.txt` & `cgcsdk-0.9.2/cgc/tests/desired_responses/test_billing_status.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/tests/desired_responses/test_compute_list.txt` & `cgcsdk-0.9.2/cgc/tests/desired_responses/test_compute_list.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/tests/desired_responses/test_tabulate_response.txt` & `cgcsdk-0.9.2/cgc/tests/desired_responses/test_tabulate_response.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/tests/responses_tests.py` & `cgcsdk-0.9.2/cgc/tests/responses_tests.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/utils/__init__.py` & `cgcsdk-0.9.2/cgc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/utils/click_group.py` & `cgcsdk-0.9.2/cgc/utils/click_group.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/utils/config_utils.py` & `cgcsdk-0.9.2/cgc/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/utils/consts/env_consts.py` & `cgcsdk-0.9.2/cgc/utils/consts/env_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/utils/consts/message_consts.py` & `cgcsdk-0.9.2/cgc/utils/consts/message_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/utils/cryptography/aes_crypto.py` & `cgcsdk-0.9.2/cgc/utils/cryptography/aes_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/utils/cryptography/encryption_module.py` & `cgcsdk-0.9.2/cgc/utils/cryptography/encryption_module.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/utils/cryptography/rsa_crypto.py` & `cgcsdk-0.9.2/cgc/utils/cryptography/rsa_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/utils/custom_exceptions.py` & `cgcsdk-0.9.2/cgc/utils/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/utils/message_utils.py` & `cgcsdk-0.9.2/cgc/utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/utils/prepare_headers.py` & `cgcsdk-0.9.2/cgc/utils/prepare_headers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/utils/requests_helper.py` & `cgcsdk-0.9.2/cgc/utils/requests_helper.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/utils/response_utils.py` & `cgcsdk-0.9.2/cgc/utils/response_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgc/utils/version_control.py` & `cgcsdk-0.9.2/cgc/utils/version_control.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/cgcsdk.egg-info/PKG-INFO` & `cgcsdk-0.9.2/cgcsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.9.1
+Version: 0.9.2
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.9.1/cgcsdk.egg-info/SOURCES.txt` & `cgcsdk-0.9.2/cgcsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.9.1/setup.py` & `cgcsdk-0.9.2/setup.py`

 * *Files identical despite different names*

