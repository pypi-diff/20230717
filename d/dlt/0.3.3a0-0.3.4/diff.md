# Comparing `tmp/dlt-0.3.3a0.tar.gz` & `tmp/dlt-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.3.3a0.tar", max compression
+gzip compressed data, was "dlt-0.3.4.tar", max compression
```

## Comparing `dlt-0.3.3a0.tar` & `dlt-0.3.4.tar`

### file list

```diff
@@ -1,223 +1,224 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.3.3a0/LICENSE.txt
--rw-r--r--   0        0        0     4144 2023-06-21 13:07:51.602230 dlt-0.3.3a0/README.md
--rw-r--r--   0        0        0     1708 2023-06-21 13:07:51.602230 dlt-0.3.3a0/dlt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.3.3a0/dlt/cli/__init__.py
--rw-r--r--   0        0        0    17127 2023-06-26 19:21:47.823243 dlt-0.3.3a0/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     3974 2023-06-23 11:37:08.764341 dlt-0.3.3a0/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    15046 2023-06-21 13:07:51.602230 dlt-0.3.3a0/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0    14849 2023-06-22 15:45:03.707967 dlt-0.3.3a0/dlt/cli/deploy_command_helpers.py
--rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.3.3a0/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-06-07 10:42:04.941010 dlt-0.3.3a0/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    18756 2023-06-07 10:42:04.941010 dlt-0.3.3a0/dlt/cli/init_command.py
--rw-r--r--   0        0        0    10508 2023-06-22 15:45:03.707967 dlt-0.3.3a0/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0     9588 2023-06-21 13:07:51.602230 dlt-0.3.3a0/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     4505 2023-05-24 16:38:22.528779 dlt-0.3.3a0/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1899 2023-05-23 16:25:33.987923 dlt-0.3.3a0/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     3753 2023-05-29 18:11:09.008705 dlt-0.3.3a0/dlt/cli/utils.py
--rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.3.3a0/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.3.3a0/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      442 2023-05-29 14:13:02.418979 dlt-0.3.3a0/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     5078 2023-05-24 16:38:22.528779 dlt-0.3.3a0/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     3469 2023-06-03 16:59:51.259756 dlt-0.3.3a0/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     6741 2023-05-29 14:13:02.418979 dlt-0.3.3a0/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     7912 2023-06-20 19:08:58.883105 dlt-0.3.3a0/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1791 2023-05-14 20:33:31.539348 dlt-0.3.3a0/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      344 2023-06-21 13:07:51.602230 dlt-0.3.3a0/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0      664 2023-05-29 14:13:02.418979 dlt-0.3.3a0/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1116 2023-05-07 23:03:04.659469 dlt-0.3.3a0/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1335 2023-05-07 23:03:04.659469 dlt-0.3.3a0/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     1981 2023-05-07 23:03:04.659469 dlt-0.3.3a0/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0     3662 2023-05-29 14:13:02.418979 dlt-0.3.3a0/dlt/common/configuration/providers/google_secrets.py
--rw-r--r--   0        0        0     1306 2023-05-24 16:38:22.538779 dlt-0.3.3a0/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0    12880 2023-06-21 13:07:51.602230 dlt-0.3.3a0/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    18788 2023-06-20 20:37:15.263105 dlt-0.3.3a0/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0      971 2023-05-29 14:13:02.418979 dlt-0.3.3a0/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1817 2023-05-07 23:03:04.659469 dlt-0.3.3a0/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0     2109 2023-05-29 14:13:02.418979 dlt-0.3.3a0/dlt/common/configuration/specs/aws_credentials.py
--rw-r--r--   0        0        0    14214 2023-05-29 14:13:02.418979 dlt-0.3.3a0/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     5483 2023-05-29 14:13:02.418979 dlt-0.3.3a0/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     3387 2023-06-07 08:32:53.261010 dlt-0.3.3a0/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     1818 2023-05-24 16:38:22.538779 dlt-0.3.3a0/dlt/common/configuration/specs/connection_string_credentials.py
--rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.3.3a0/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    12725 2023-05-07 23:03:04.669469 dlt-0.3.3a0/dlt/common/configuration/specs/gcp_credentials.py
--rw-r--r--   0        0        0      725 2023-05-07 23:03:04.669469 dlt-0.3.3a0/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.3.3a0/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0     6036 2023-05-29 14:13:02.418979 dlt-0.3.3a0/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.3.3a0/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.3.3a0/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.3.3a0/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.3.3a0/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     6203 2023-06-22 15:45:03.707967 dlt-0.3.3a0/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     2727 2023-06-22 15:45:03.707967 dlt-0.3.3a0/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.3.3a0/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     8392 2023-06-28 21:18:39.080000 dlt-0.3.3a0/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0      189 2023-05-29 18:11:09.008705 dlt-0.3.3a0/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     2250 2023-06-22 15:45:03.707967 dlt-0.3.3a0/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0    11099 2023-05-29 18:11:09.008705 dlt-0.3.3a0/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     6465 2023-06-08 07:50:27.863474 dlt-0.3.3a0/dlt/common/exceptions.py
--rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.3.3a0/dlt/common/git.py
--rw-r--r--   0        0        0     5253 2023-05-14 20:33:31.539348 dlt-0.3.3a0/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.3.3a0/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.3.3a0/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.3.3a0/dlt/common/jsonpath.py
--rw-r--r--   0        0        0        0 2023-06-22 15:45:03.707967 dlt-0.3.3a0/dlt/common/libs/__init__.py
--rw-r--r--   0        0        0     1041 2023-06-22 15:45:03.707967 dlt-0.3.3a0/dlt/common/libs/pyarrow.py
--rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.3.3a0/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1197 2023-05-07 23:03:04.669469 dlt-0.3.3a0/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.3.3a0/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.3.3a0/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    13382 2023-05-14 20:33:31.539348 dlt-0.3.3a0/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.3.3a0/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.3.3a0/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.3.3a0/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.3.3a0/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.3.3a0/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.3.3a0/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.3.3a0/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.3.3a0/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.3.3a0/dlt/common/pendulum.py
--rw-r--r--   0        0        0    19069 2023-06-22 15:45:03.707967 dlt-0.3.3a0/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.3.3a0/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.3.3a0/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.3.3a0/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.3.3a0/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.3.3a0/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      705 2023-05-24 16:38:22.538779 dlt-0.3.3a0/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     2635 2023-05-14 11:08:47.420838 dlt-0.3.3a0/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.3.3a0/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.3.3a0/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.3.3a0/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.3.3a0/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5590 2023-05-07 23:03:04.669469 dlt-0.3.3a0/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.3.3a0/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    13923 2023-06-07 08:32:53.261010 dlt-0.3.3a0/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     4501 2023-05-14 20:33:31.539348 dlt-0.3.3a0/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.3.3a0/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.3.3a0/dlt/common/runtime/logger.py
--rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.3.3a0/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     7170 2023-05-14 20:33:31.539348 dlt-0.3.3a0/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.3.3a0/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.3.3a0/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.3.3a0/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.3.3a0/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.3.3a0/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.3.3a0/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.3.3a0/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    25164 2023-05-29 14:13:02.418979 dlt-0.3.3a0/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.3.3a0/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    23080 2023-06-07 08:32:53.261010 dlt-0.3.3a0/dlt/common/schema/utils.py
--rw-r--r--   0        0        0     1467 2023-05-24 16:38:22.538779 dlt-0.3.3a0/dlt/common/source.py
--rw-r--r--   0        0        0      554 2023-05-24 16:38:22.538779 dlt-0.3.3a0/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1649 2023-05-24 16:38:22.538779 dlt-0.3.3a0/dlt/common/storages/configuration.py
--rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.3.3a0/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     3107 2023-06-07 08:32:53.261010 dlt-0.3.3a0/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0    11872 2023-06-21 13:07:51.612230 dlt-0.3.3a0/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2690 2023-05-24 16:38:22.538779 dlt-0.3.3a0/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    21812 2023-05-24 16:38:22.538779 dlt-0.3.3a0/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2409 2023-05-24 16:38:22.538779 dlt-0.3.3a0/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8600 2023-06-07 08:32:53.261010 dlt-0.3.3a0/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     9506 2023-06-25 19:18:14.825402 dlt-0.3.3a0/dlt/common/storages/transactional_file.py
--rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.3.3a0/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2634 2023-05-07 23:03:04.669469 dlt-0.3.3a0/dlt/common/time.py
--rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.3.3a0/dlt/common/typing.py
--rw-r--r--   0        0        0    14285 2023-06-21 13:07:51.612230 dlt-0.3.3a0/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.3.3a0/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.3.3a0/dlt/common/wei.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.3.3a0/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.3.3a0/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     1824 2023-06-22 15:45:03.707967 dlt-0.3.3a0/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    12577 2023-06-28 21:18:39.080000 dlt-0.3.3a0/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0      386 2023-05-07 23:03:04.669469 dlt-0.3.3a0/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0    10366 2023-06-28 21:18:39.080000 dlt-0.3.3a0/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     1946 2023-06-25 20:39:31.755402 dlt-0.3.3a0/dlt/destinations/duckdb/__init__.py
--rw-r--r--   0        0        0     7342 2023-06-28 21:18:39.080000 dlt-0.3.3a0/dlt/destinations/duckdb/configuration.py
--rw-r--r--   0        0        0     4114 2023-06-26 21:15:51.953243 dlt-0.3.3a0/dlt/destinations/duckdb/duck.py
--rw-r--r--   0        0        0     6635 2023-06-28 21:18:39.080000 dlt-0.3.3a0/dlt/destinations/duckdb/sql_client.py
--rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.3.3a0/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.3.3a0/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     4989 2023-05-29 14:13:02.418979 dlt-0.3.3a0/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.3.3a0/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     1270 2023-06-25 11:33:44.534161 dlt-0.3.3a0/dlt/destinations/filesystem/__init__.py
--rw-r--r--   0        0        0     2253 2023-05-29 14:13:02.418979 dlt-0.3.3a0/dlt/destinations/filesystem/configuration.py
--rw-r--r--   0        0        0     5111 2023-06-25 19:18:14.825402 dlt-0.3.3a0/dlt/destinations/filesystem/filesystem.py
--rw-r--r--   0        0        0     1419 2023-05-29 14:13:02.418979 dlt-0.3.3a0/dlt/destinations/filesystem/filesystem_client.py
--rw-r--r--   0        0        0     5028 2023-06-21 13:07:51.612230 dlt-0.3.3a0/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    16267 2023-06-28 21:18:39.080000 dlt-0.3.3a0/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.3.3a0/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0     1981 2023-06-28 21:18:39.080000 dlt-0.3.3a0/dlt/destinations/motherduck/__init__.py
--rw-r--r--   0        0        0     1807 2023-06-28 21:18:39.080000 dlt-0.3.3a0/dlt/destinations/motherduck/configuration.py
--rw-r--r--   0        0        0      968 2023-06-28 21:18:39.080000 dlt-0.3.3a0/dlt/destinations/motherduck/motherduck.py
--rw-r--r--   0        0        0     1391 2023-06-28 21:18:39.080000 dlt-0.3.3a0/dlt/destinations/motherduck/sql_client.py
--rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.3.3a0/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.3.3a0/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0     1377 2023-06-22 15:45:03.707967 dlt-0.3.3a0/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.3.3a0/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     5781 2023-06-28 21:18:39.080000 dlt-0.3.3a0/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.3.3a0/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.3.3a0/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      570 2023-05-07 23:03:04.669469 dlt-0.3.3a0/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     4868 2023-06-28 21:18:39.080000 dlt-0.3.3a0/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     1916 2023-06-23 11:37:08.764341 dlt-0.3.3a0/dlt/destinations/snowflake/__init__.py
--rw-r--r--   0        0        0     4076 2023-06-25 11:33:44.534161 dlt-0.3.3a0/dlt/destinations/snowflake/configuration.py
--rw-r--r--   0        0        0     7479 2023-06-23 11:37:08.764341 dlt-0.3.3a0/dlt/destinations/snowflake/snowflake.py
--rw-r--r--   0        0        0     6820 2023-06-28 21:18:39.080000 dlt-0.3.3a0/dlt/destinations/snowflake/sql_client.py
--rw-r--r--   0        0        0     7776 2023-06-28 21:18:39.080000 dlt-0.3.3a0/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    10489 2023-06-28 21:18:39.080000 dlt-0.3.3a0/dlt/destinations/sql_merge_job.py
--rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.3.3a0/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.3a0/dlt/extract/__init__.py
--rw-r--r--   0        0        0    26516 2023-06-07 08:32:53.261010 dlt-0.3.3a0/dlt/extract/decorators.py
--rw-r--r--   0        0        0    12995 2023-06-07 08:32:53.261010 dlt-0.3.3a0/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     8312 2023-06-21 13:07:51.612230 dlt-0.3.3a0/dlt/extract/extract.py
--rw-r--r--   0        0        0    14954 2023-05-24 16:38:22.538779 dlt-0.3.3a0/dlt/extract/incremental.py
--rw-r--r--   0        0        0    35424 2023-06-25 11:33:44.534161 dlt-0.3.3a0/dlt/extract/pipe.py
--rw-r--r--   0        0        0     9683 2023-05-24 16:38:22.538779 dlt-0.3.3a0/dlt/extract/schema.py
--rw-r--r--   0        0        0    38391 2023-06-21 13:07:51.612230 dlt-0.3.3a0/dlt/extract/source.py
--rw-r--r--   0        0        0     4308 2023-05-24 16:38:22.538779 dlt-0.3.3a0/dlt/extract/typing.py
--rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.3.3a0/dlt/extract/utils.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.3.3a0/dlt/helpers/__init__.py
--rw-r--r--   0        0        0    13783 2023-05-28 13:56:42.341452 dlt-0.3.3a0/dlt/helpers/airflow_helper.py
--rw-r--r--   0        0        0     3110 2023-06-23 11:37:08.764341 dlt-0.3.3a0/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.3.3a0/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6219 2023-06-28 21:18:39.080000 dlt-0.3.3a0/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.3.3a0/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     5085 2023-06-28 21:18:39.080000 dlt-0.3.3a0/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.3.3a0/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     2490 2023-05-29 14:13:02.438979 dlt-0.3.3a0/dlt/helpers/pandas_helper.py
--rw-r--r--   0        0        0    13378 2023-05-29 14:13:02.438979 dlt-0.3.3a0/dlt/helpers/streamlit_helper.py
--rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.3.3a0/dlt/load/__init__.py
--rw-r--r--   0        0        0     1005 2023-05-24 16:38:22.538779 dlt-0.3.3a0/dlt/load/configuration.py
--rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.3.3a0/dlt/load/exceptions.py
--rw-r--r--   0        0        0    19925 2023-06-08 14:19:13.923473 dlt-0.3.3a0/dlt/load/load.py
--rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.3.3a0/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1101 2023-05-24 16:38:22.538779 dlt-0.3.3a0/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.3a0/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    16488 2023-06-22 15:45:03.707967 dlt-0.3.3a0/dlt/normalize/normalize.py
--rw-r--r--   0        0        0    13137 2023-06-22 15:45:03.707967 dlt-0.3.3a0/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     1971 2023-06-22 15:45:03.707967 dlt-0.3.3a0/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      379 2023-05-24 16:38:22.538779 dlt-0.3.3a0/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.3.3a0/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     3100 2023-05-28 13:56:42.341452 dlt-0.3.3a0/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     8733 2023-06-07 08:32:53.271010 dlt-0.3.3a0/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.3.3a0/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    59746 2023-06-22 15:45:03.707967 dlt-0.3.3a0/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.3.3a0/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     4186 2023-06-07 08:32:53.271010 dlt-0.3.3a0/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0     7990 2023-06-21 13:07:51.612230 dlt-0.3.3a0/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     4625 2023-05-29 18:11:09.018705 dlt-0.3.3a0/dlt/pipeline/track.py
--rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.3.3a0/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.3.3a0/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.3.3a0/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.3.3a0/dlt/reflection/names.py
--rw-r--r--   0        0        0     5617 2023-05-07 23:03:04.669469 dlt-0.3.3a0/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.3.3a0/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      124 2023-05-07 23:03:04.669469 dlt-0.3.3a0/dlt/sources/__init__.py
--rw-r--r--   0        0        0      320 2023-05-07 23:03:04.669469 dlt-0.3.3a0/dlt/sources/credentials.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.3.3a0/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.3.3a0/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0     9243 2023-05-29 14:13:02.418979 dlt-0.3.3a0/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.3.3a0/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.3.3a0/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.3.3a0/dlt/version.py
--rw-r--r--   0        0        0     4496 2023-06-28 21:18:39.090000 dlt-0.3.3a0/pyproject.toml
--rw-r--r--   0        0        0     7797 1970-01-01 00:00:00.000000 dlt-0.3.3a0/setup.py
--rw-r--r--   0        0        0     7785 1970-01-01 00:00:00.000000 dlt-0.3.3a0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.3.4/LICENSE.txt
+-rw-r--r--   0        0        0     4144 2023-07-08 12:23:15.759697 dlt-0.3.4/README.md
+-rw-r--r--   0        0        0     1708 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    17127 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     3974 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    15046 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0    14849 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/deploy_command_helpers.py
+-rw-r--r--   0        0        0     1853 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    18756 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    10508 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0     9588 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     4505 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1899 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     2308 2023-07-17 05:20:41.255677 dlt-0.3.4/dlt/cli/utils.py
+-rw-r--r--   0        0        0      307 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.3.4/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      480 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     5078 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     3469 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     6741 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0     7912 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1791 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      344 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0      664 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1116 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1335 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     1981 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0     3662 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/providers/google_secrets.py
+-rw-r--r--   0        0        0     1306 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0    12880 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    18788 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0     1002 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1817 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0     2128 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/configuration/specs/aws_credentials.py
+-rw-r--r--   0        0        0    14214 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     5476 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     3387 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     1818 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/specs/connection_string_credentials.py
+-rw-r--r--   0        0        0     2125 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    12537 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/common/configuration/specs/gcp_credentials.py
+-rw-r--r--   0        0        0      725 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0     2712 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0     6559 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      142 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6306 2023-07-15 10:14:14.845022 dlt-0.3.4/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      214 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      260 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     6203 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     2727 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0      962 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0     8426 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0      189 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     3158 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0    11909 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     8111 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     4954 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/git.py
+-rw-r--r--   0        0        0     5253 2023-07-15 10:57:51.195021 dlt-0.3.4/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1802 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2939 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1536 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/libs/__init__.py
+-rw-r--r--   0        0        0     1657 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/libs/pyarrow.py
+-rw-r--r--   0        0        0      232 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1197 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      472 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1644 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    13382 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0       64 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      807 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0     1069 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      792 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     3753 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     3002 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      358 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     2337 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      451 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    19531 2023-07-17 05:20:41.255677 dlt-0.3.4/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      374 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     4891 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5069 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      174 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      705 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     2635 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4046 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3145 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5590 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       36 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    13923 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     4501 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0      771 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     4002 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runtime/logger.py
+-rw-r--r--   0        0        0     2052 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     7234 2023-07-17 05:20:41.255677 dlt-0.3.4/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2492 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     2027 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      616 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0     2798 2023-07-17 05:20:41.255677 dlt-0.3.4/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      387 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     1927 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     2974 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0    25164 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     3004 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    23295 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0     1467 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/source.py
+-rw-r--r--   0        0        0      554 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     1649 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/configuration.py
+-rw-r--r--   0        0        0     1906 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     3107 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0    11872 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0     2690 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    21812 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     2409 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     8600 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     9506 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/transactional_file.py
+-rw-r--r--   0        0        0     2525 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     2634 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/time.py
+-rw-r--r--   0        0        0     4736 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/typing.py
+-rw-r--r--   0        0        0    14285 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/utils.py
+-rw-r--r--   0        0        0     3686 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/validation.py
+-rw-r--r--   0        0        0     1185 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/wei.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      437 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/bigquery/README.md
+-rw-r--r--   0        0        0     2136 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/bigquery/__init__.py
+-rw-r--r--   0        0        0    14030 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/bigquery/bigquery.py
+-rw-r--r--   0        0        0     1757 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/destinations/bigquery/configuration.py
+-rw-r--r--   0        0        0    10509 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/bigquery/sql_client.py
+-rw-r--r--   0        0        0     2257 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/duckdb/__init__.py
+-rw-r--r--   0        0        0     7342 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/duckdb/configuration.py
+-rw-r--r--   0        0        0     4135 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/duckdb/duck.py
+-rw-r--r--   0        0        0     6635 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1761 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/dummy/__init__.py
+-rw-r--r--   0        0        0      736 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/dummy/configuration.py
+-rw-r--r--   0        0        0     4989 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/dummy/dummy.py
+-rw-r--r--   0        0        0     4184 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0     1270 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/filesystem/__init__.py
+-rw-r--r--   0        0        0     2260 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/filesystem/configuration.py
+-rw-r--r--   0        0        0     5918 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/filesystem/filesystem.py
+-rw-r--r--   0        0        0     1419 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/filesystem/filesystem_client.py
+-rw-r--r--   0        0        0     5046 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    17153 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     2057 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0     2201 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/motherduck/__init__.py
+-rw-r--r--   0        0        0     1807 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/motherduck/configuration.py
+-rw-r--r--   0        0        0      968 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/motherduck/motherduck.py
+-rw-r--r--   0        0        0     1391 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/motherduck/sql_client.py
+-rw-r--r--   0        0        0      251 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/postgres/README.md
+-rw-r--r--   0        0        0     2312 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/postgres/__init__.py
+-rw-r--r--   0        0        0     1377 2023-07-13 15:13:56.520313 dlt-0.3.4/dlt/destinations/postgres/configuration.py
+-rw-r--r--   0        0        0     3176 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/postgres/postgres.py
+-rw-r--r--   0        0        0     5781 2023-07-15 10:59:55.545022 dlt-0.3.4/dlt/destinations/postgres/sql_client.py
+-rw-r--r--   0        0        0     1159 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/redshift/README.md
+-rw-r--r--   0        0        0     2237 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/redshift/__init__.py
+-rw-r--r--   0        0        0      623 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/redshift/configuration.py
+-rw-r--r--   0        0        0     8620 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/redshift/redshift.py
+-rw-r--r--   0        0        0     2255 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/snowflake/__init__.py
+-rw-r--r--   0        0        0     4075 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/snowflake/configuration.py
+-rw-r--r--   0        0        0     9021 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/snowflake/snowflake.py
+-rw-r--r--   0        0        0     7069 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/snowflake/sql_client.py
+-rw-r--r--   0        0        0     7776 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    10489 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/sql_merge_job.py
+-rw-r--r--   0        0        0     1931 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/typing.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.4/dlt/extract/__init__.py
+-rw-r--r--   0        0        0    26516 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    12995 2023-07-15 16:23:33.345022 dlt-0.3.4/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0     8312 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/extract/extract.py
+-rw-r--r--   0        0        0    18469 2023-07-15 16:23:33.345022 dlt-0.3.4/dlt/extract/incremental.py
+-rw-r--r--   0        0        0    35605 2023-07-15 16:23:33.345022 dlt-0.3.4/dlt/extract/pipe.py
+-rw-r--r--   0        0        0     9683 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/extract/schema.py
+-rw-r--r--   0        0        0    38391 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/extract/source.py
+-rw-r--r--   0        0        0     4308 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/extract/typing.py
+-rw-r--r--   0        0        0      593 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/extract/utils.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.3.4/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0    13867 2023-07-17 05:20:41.255677 dlt-0.3.4/dlt/helpers/airflow_helper.py
+-rw-r--r--   0        0        0     3167 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1220 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6669 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      758 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     5220 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    13214 2023-07-17 05:20:41.255677 dlt-0.3.4/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     2490 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/helpers/pandas_helper.py
+-rw-r--r--   0        0        0    13378 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/helpers/streamlit_helper.py
+-rw-r--r--   0        0        0       31 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/load/__init__.py
+-rw-r--r--   0        0        0     1005 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/load/configuration.py
+-rw-r--r--   0        0        0     1993 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    22228 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/load/load.py
+-rw-r--r--   0        0        0       32 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1101 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.4/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    16488 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0    13633 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     2009 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      379 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4829 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     3100 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     8711 2023-07-17 05:20:41.255677 dlt-0.3.4/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      122 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    64550 2023-07-17 05:20:41.265677 dlt-0.3.4/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0      985 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     4186 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0     9132 2023-07-17 05:20:41.265677 dlt-0.3.4/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     4894 2023-07-17 05:20:41.265677 dlt-0.3.4/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       91 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.3.4/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      563 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/reflection/names.py
+-rw-r--r--   0        0        0     5617 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6186 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      124 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/sources/__init__.py
+-rw-r--r--   0        0        0      320 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/sources/credentials.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0      832 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0    10837 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1757 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      234 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/sources/helpers/requests/typing.py
+-rw-r--r--   0        0        0      679 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1125 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/version.py
+-rw-r--r--   0        0        0     4459 2023-07-17 05:20:41.265677 dlt-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     7760 1970-01-01 00:00:00.000000 dlt-0.3.4/setup.py
+-rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 dlt-0.3.4/PKG-INFO
```

### Comparing `dlt-0.3.3a0/LICENSE.txt` & `dlt-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/README.md` & `dlt-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/__init__.py` & `dlt-0.3.4/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/cli/_dlt.py` & `dlt-0.3.4/dlt/cli/_dlt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/cli/config_toml_writer.py` & `dlt-0.3.4/dlt/cli/config_toml_writer.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/cli/deploy_command.py` & `dlt-0.3.4/dlt/cli/deploy_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/cli/deploy_command_helpers.py` & `dlt-0.3.4/dlt/cli/deploy_command_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/cli/echo.py` & `dlt-0.3.4/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/cli/init_command.py` & `dlt-0.3.4/dlt/cli/init_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/cli/pipeline_command.py` & `dlt-0.3.4/dlt/cli/pipeline_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/cli/pipeline_files.py` & `dlt-0.3.4/dlt/cli/pipeline_files.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/cli/source_detection.py` & `dlt-0.3.4/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/cli/telemetry_command.py` & `dlt-0.3.4/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/arithmetics.py` & `dlt-0.3.4/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/accessors.py` & `dlt-0.3.4/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/container.py` & `dlt-0.3.4/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/exceptions.py` & `dlt-0.3.4/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/inject.py` & `dlt-0.3.4/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/paths.py` & `dlt-0.3.4/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/providers/airflow.py` & `dlt-0.3.4/dlt/common/configuration/providers/airflow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/providers/context.py` & `dlt-0.3.4/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/providers/dictionary.py` & `dlt-0.3.4/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/providers/environ.py` & `dlt-0.3.4/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/providers/google_secrets.py` & `dlt-0.3.4/dlt/common/configuration/providers/google_secrets.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/providers/provider.py` & `dlt-0.3.4/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/providers/toml.py` & `dlt-0.3.4/dlt/common/configuration/providers/toml.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/resolve.py` & `dlt-0.3.4/dlt/common/configuration/resolve.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/specs/__init__.py` & `dlt-0.3.4/dlt/common/configuration/specs/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .run_configuration import RunConfiguration  # noqa: F401
 from .base_configuration import BaseConfiguration, CredentialsConfiguration, CredentialsWithDefault, ContainerInjectableContext, extract_inner_hint, is_base_configuration_inner_hint, configspec  # noqa: F401
 from .config_section_context import ConfigSectionContext  # noqa: F401
 
 from .gcp_credentials import GcpServiceAccountCredentialsWithoutDefaults, GcpServiceAccountCredentials, GcpOAuthCredentialsWithoutDefaults, GcpOAuthCredentials, GcpCredentials  # noqa: F401
 from .connection_string_credentials import ConnectionStringCredentials  # noqa: F401
 from .api_credentials import OAuth2Credentials  # noqa: F401
-from .aws_credentials import AwsCredentials  # noqa: F401
+from .aws_credentials import AwsCredentials, AwsCredentialsWithoutDefaults  # noqa: F401
 
 
 # backward compatibility for service account credentials
 from .gcp_credentials import GcpServiceAccountCredentialsWithoutDefaults as GcpClientCredentials, GcpServiceAccountCredentials as GcpClientCredentialsWithDefault  # noqa: F401
```

### Comparing `dlt-0.3.3a0/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.3.4/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/specs/aws_credentials.py` & `dlt-0.3.4/dlt/common/configuration/specs/aws_credentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,57 @@
-from typing import Optional, TYPE_CHECKING, Dict
+from typing import Optional, TYPE_CHECKING, Dict, Any
 
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.typing import TSecretStrValue
 from dlt.common.configuration.specs import CredentialsConfiguration, CredentialsWithDefault, configspec
 from dlt import version
 
-if TYPE_CHECKING:
-    from botocore.credentials import Credentials
-    from boto3 import Session
-
 
 @configspec
-class AwsCredentials(CredentialsConfiguration, CredentialsWithDefault):
+class AwsCredentialsWithoutDefaults(CredentialsConfiguration):
+    # credentials without boto implementation
     aws_access_key_id: str = None
     aws_secret_access_key: TSecretStrValue = None
     aws_session_token: Optional[TSecretStrValue] = None
     aws_profile: Optional[str] = None
 
+    def to_s3fs_credentials(self) -> Dict[str, Optional[str]]:
+        """Dict of keyword arguments that can be passed to s3fs"""
+        return dict(
+            key=self.aws_access_key_id,
+            secret=self.aws_secret_access_key,
+            token=self.aws_session_token,
+            profile=self.aws_profile
+        )
+
+    def to_native_representation(self) -> Dict[str, Optional[str]]:
+        """Return a dict that can be passed as kwargs to boto3 session"""
+        d = dict(self)
+        d['profile_name'] = d.pop('aws_profile')  # boto3 argument doesn't match env var name
+        return d
+
+
+@configspec
+class AwsCredentials(AwsCredentialsWithoutDefaults, CredentialsWithDefault):
+
     def on_partial(self) -> None:
         # Try get default credentials
         session = self._to_session()
         self.aws_profile = session.profile_name
         default = session.get_credentials()
         if not default:
             return None
         self.aws_access_key_id = default.access_key
         self.aws_secret_access_key = default.secret_key
         self.aws_session_token = default.token
         if not self.is_partial():
             self.resolve()
 
-    def _to_session(self) -> "Session":
+    def _to_session(self) -> Any:
         try:
             import boto3
         except ImportError:
             raise MissingDependencyException(self.__class__.__name__, [f"{version.DLT_PKG_NAME}[s3]"])
         return boto3.Session(**self.to_native_representation())
 
-    def to_native_credentials(self) -> Optional["Credentials"]:
+    def to_native_credentials(self) -> Optional[Any]:
         return self._to_session().get_credentials()
-
-    def to_s3fs_credentials(self) -> Dict[str, Optional[str]]:
-        """Dict of keyword arguments that can be passed to s3fs"""
-        return dict(
-            key=self.aws_access_key_id,
-            secret=self.aws_secret_access_key,
-            token=self.aws_session_token,
-            profile=self.aws_profile
-        )
-
-    def to_native_representation(self) -> Dict[str, Optional[str]]:
-        """Return a dict that can be passed as kwargs to boto3 session"""
-        d = dict(self)
-        d['profile_name'] = d.pop('aws_profile')  # boto3 argument doesn't match env var name
-        return d
```

### Comparing `dlt-0.3.3a0/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.3.4/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.3.4/dlt/common/configuration/specs/config_providers_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-
-
 import contextlib
 import io
-from typing import Any, List
+from typing import List
 from dlt.common.configuration.exceptions import DuplicateConfigProviderException
 from dlt.common.configuration.providers import ConfigProvider, EnvironProvider, ContextProvider, SecretsTomlProvider, ConfigTomlProvider, GoogleSecretsProvider
 from dlt.common.configuration.specs.base_configuration import ContainerInjectableContext
 from dlt.common.configuration.specs import GcpServiceAccountCredentials, BaseConfiguration, configspec, known_sections
 from dlt.common.runtime.exec_info import is_airflow_installed
```

### Comparing `dlt-0.3.3a0/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.3.4/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/specs/connection_string_credentials.py` & `dlt-0.3.4/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/specs/exceptions.py` & `dlt-0.3.4/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/specs/gcp_credentials.py` & `dlt-0.3.4/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from typing import Any, ClassVar, Final, List, Tuple, Union
+from typing import Any, Final, List, Tuple, Union
 from deprecated import deprecated
 
 from dlt.common import json, pendulum
 from dlt.common.configuration.specs.api_credentials import OAuth2Credentials
 from dlt.common.configuration.specs.exceptions import InvalidGoogleNativeCredentialsType, InvalidGoogleOauth2Json, InvalidGoogleServicesJson, NativeValueError, OAuth2ScopesRequired
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.typing import DictStrAny, TSecretValue, StrAny
@@ -13,21 +13,16 @@
 
 @configspec
 class GcpCredentials(CredentialsConfiguration):
     token_uri: Final[str] = "https://oauth2.googleapis.com/token"
     auth_uri: Final[str] = "https://accounts.google.com/o/oauth2/auth"
 
     project_id: str = None
-    location: str = "US"
 
-    http_timeout: float = 15.0
-    file_upload_timeout: float = 30 * 60.0
-    retry_deadline: float = 60  # how long to retry the operation in case of error, the backoff 60s
-
-    __config_gen_annotations__: ClassVar[List[str]] = ["location"]
+    location: str = "US"  # DEPRECATED! and present only for backward compatibility. please set bigquery location in BigQuery configuration
 
     def parse_native_representation(self, native_value: Any) -> None:
         if not isinstance(native_value, str):
             raise InvalidGoogleNativeCredentialsType(self.__class__, native_value)
 
     def to_native_representation(self) -> str:
         return json.dumps(dict(self))
@@ -36,15 +31,15 @@
         """Returns respective native credentials for service account or oauth2 that can be passed to google clients"""
         pass
 
     def _from_info_dict(self, info: StrAny) -> None:
         self.update(info)
 
     def __str__(self) -> str:
-        return f"{self.project_id}[{self.location}]"
+        return f"{self.project_id}"
 
 
 @configspec
 class GcpServiceAccountCredentialsWithoutDefaults(GcpCredentials):
     private_key: TSecretValue = None
     client_email: str = None
     type: Final[str] = "service_account"  # noqa: A003
@@ -92,15 +87,15 @@
         if isinstance(self.private_key, ServiceAccountCredentials):
             # private key holds the native instance if it was passed to parse_native_representation
             return self.private_key
         else:
             return ServiceAccountCredentials.from_service_account_info(self)
 
     def __str__(self) -> str:
-        return f"{self.client_email}@{self.project_id}[{self.location}]"
+        return f"{self.client_email}@{self.project_id}"
 
 
 @configspec
 class GcpOAuthCredentialsWithoutDefaults(GcpCredentials, OAuth2Credentials):
     # only desktop app supported
     refresh_token: TSecretValue
     client_type: Final[str] = "installed"
@@ -207,15 +202,15 @@
     def _info_dict(self) -> DictStrAny:
         info_dict = dict(self)
         # for desktop app
         info_dict["redirect_uris"] = ["http://localhost"]
         return info_dict
 
     def __str__(self) -> str:
-        return f"{self.client_id}@{self.project_id}[{self.location}]"
+        return f"{self.client_id}@{self.project_id}"
 
 
 @configspec
 class GcpDefaultCredentials(CredentialsWithDefault, GcpCredentials):
 
     _LAST_FAILED_DEFAULT: float = 0.0
```

### Comparing `dlt-0.3.3a0/dlt/common/configuration/specs/known_sections.py` & `dlt-0.3.4/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.3.4/dlt/common/configuration/specs/run_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,22 @@
     pipeline_name: Optional[str] = None
     sentry_dsn: Optional[str] = None  # keep None to disable Sentry
     slack_incoming_hook: Optional[TSecretStrValue] = None
     dlthub_telemetry: bool = True  # enable or disable dlthub telemetry
     dlthub_telemetry_segment_write_key: str = "a1F2gc6cNYw2plyAt02sZouZcsRjG7TD"
     log_format: str = '{asctime}|[{levelname:<21}]|{process}|{name}|{filename}|{funcName}:{lineno}|{message}'
     log_level: str = "WARNING"
-    request_timeout: Tuple[int, int] = (15, 300)  # default request timeout for all http clients
+    request_timeout: float = 60
+    """Timeout for http requests"""
+    request_max_attempts: int = 5
+    """Max retry attempts for http clients"""
+    request_backoff_factor: float = 1
+    """Multiplier applied to exponential retry delay for http requests"""
+    request_max_retry_delay: float = 300
+    """Maximum delay between http request retries"""
     config_files_storage_path: str = "/run/config/"
 
     __section__ = "runtime"
 
     def on_resolved(self) -> None:
         # generate pipeline name from the entry point script name
         if not self.pipeline_name:
```

### Comparing `dlt-0.3.3a0/dlt/common/configuration/utils.py` & `dlt-0.3.4/dlt/common/configuration/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import ast
 import contextlib
 import tomlkit
-from typing import Any, Dict, Mapping, NamedTuple, Optional, Type, Sequence
+from typing import Any, Dict, Mapping, NamedTuple, Optional, Tuple, Type, Sequence
+from collections.abc import Mapping as C_Mapping
 
 from dlt.common import json
 from dlt.common.typing import AnyType, TAny
 from dlt.common.data_types import coerce_value, py_type_to_sc_type
 from dlt.common.configuration.providers import EnvironProvider
 from dlt.common.configuration.exceptions import ConfigValueCannotBeCoercedException, LookupTrace
 from dlt.common.configuration.specs.base_configuration import BaseConfiguration, is_base_configuration_inner_hint
@@ -127,21 +128,30 @@
         _RESOLVED_TRACES[path] = ResolvedValueTrace(key, resolved_trace.value, default_value, hint, resolved_trace.sections, resolved_trace.provider, config)
 
 
 def get_resolved_traces() -> Dict[str, ResolvedValueTrace]:
     return _RESOLVED_TRACES
 
 
-def add_config_to_env(config: BaseConfiguration) ->  None:
-    """Writes values in configuration back into environment using the naming convention of EnvironProvider"""
-    return add_config_dict_to_env(dict(config), config.__section__, overwrite_keys=True)
+def add_config_to_env(config: BaseConfiguration, sections: Tuple[str, ...] = ()) ->  None:
+    """Writes values in configuration back into environment using the naming convention of EnvironProvider. Will descend recursively if embedded BaseConfiguration instances are found"""
+    if config.__section__:
+        sections += (config.__section__, )
+    return add_config_dict_to_env(dict(config), sections, overwrite_keys=True)
 
 
-def add_config_dict_to_env(dict_: Mapping[str, Any], section: str = None, overwrite_keys: bool = False) -> None:
-    """Writes values in dict_ back into environment using the naming convention of EnvironProvider. Applies `section` if specified. Does not overwrite existing keys by default"""
+def add_config_dict_to_env(dict_: Mapping[str, Any], sections: Tuple[str, ...] = (), overwrite_keys: bool = False) -> None:
+    """Writes values in dict_ back into environment using the naming convention of EnvironProvider. Applies `sections` if specified. Does not overwrite existing keys by default"""
     for k, v in dict_.items():
-        env_key = EnvironProvider.get_key_name(k, section)
-        if env_key not in os.environ or overwrite_keys:
-            if v is None:
-                os.environ.pop(env_key, None)
+        if isinstance(v, BaseConfiguration):
+            if not v.__section__:
+                embedded_sections = sections + (k, )
             else:
-                os.environ[env_key] = serialize_value(v)
+                embedded_sections = sections
+            add_config_to_env(v, embedded_sections)
+        else:
+            env_key = EnvironProvider.get_key_name(k, *sections)
+            if env_key not in os.environ or overwrite_keys:
+                if v is None:
+                    os.environ.pop(env_key, None)
+                else:
+                    os.environ[env_key] = serialize_value(v)
```

### Comparing `dlt-0.3.3a0/dlt/common/data_types/type_helpers.py` & `dlt-0.3.4/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/data_writers/buffered.py` & `dlt-0.3.4/dlt/common/data_writers/buffered.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/data_writers/escape.py` & `dlt-0.3.4/dlt/common/data_writers/escape.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/data_writers/exceptions.py` & `dlt-0.3.4/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/data_writers/writers.py` & `dlt-0.3.4/dlt/common/data_writers/writers.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,17 @@
         self.parquet_version = version
         self.parquet_data_page_size = data_page_size
 
     def write_header(self, columns_schema: TTableSchemaColumns) -> None:
         from dlt.common.libs.pyarrow import pyarrow, get_py_arrow_datatype
 
         # build schema
-        self.schema = pyarrow.schema([pyarrow.field(name, get_py_arrow_datatype(schema_item["data_type"]), nullable=schema_item["nullable"]) for name, schema_item in columns_schema.items()])
+        self.schema = pyarrow.schema(
+            [pyarrow.field(name, get_py_arrow_datatype(schema_item["data_type"], self._caps), nullable=schema_item["nullable"]) for name, schema_item in columns_schema.items()]
+        )
         # find row items that are of the complex type (could be abstracted out for use in other writers?)
         self.complex_indices = [i for i, field in columns_schema.items() if field["data_type"] == "complex"]
         self.writer = pyarrow.parquet.ParquetWriter(self._f, self.schema, flavor=self.parquet_flavor, version=self.parquet_version, data_page_size=self.parquet_data_page_size)
 
 
     def write_data(self, rows: Sequence[Any]) -> None:
         super().write_data(rows)
```

### Comparing `dlt-0.3.3a0/dlt/common/destination/capabilities.py` & `dlt-0.3.4/dlt/destinations/duckdb/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,50 @@
-from typing import Any, Callable, ClassVar, List, Literal
+from typing import Type
 
-from dlt.common.configuration.utils import serialize_value
-from dlt.common.configuration import configspec
-from dlt.common.configuration.specs import ContainerInjectableContext
-from dlt.common.utils import identity
-
-
-# known loader file formats
-# jsonl - new line separated json documents
-# puae-jsonl - internal extract -> normalize format bases on jsonl
-# insert_values - insert SQL statements
-# sql - any sql statement
-TLoaderFileFormat = Literal["jsonl", "puae-jsonl", "insert_values", "sql", "parquet"]
-
-
-@configspec(init=True)
-class DestinationCapabilitiesContext(ContainerInjectableContext):
-    """Injectable destination capabilities required for many Pipeline stages ie. normalize"""
-    preferred_loader_file_format: TLoaderFileFormat
-    supported_loader_file_formats: List[TLoaderFileFormat]
-    escape_identifier: Callable[[str], str]
-    escape_literal: Callable[[Any], Any]
-    max_identifier_length: int
-    max_column_identifier_length: int
-    max_query_length: int
-    is_max_query_length_in_bytes: bool
-    max_text_data_type_length: int
-    is_max_text_data_type_length_in_bytes: bool
-    supports_ddl_transactions: bool
-    naming_convention: str = "snake_case"
-    alter_add_multi_column: bool = True
-
-    # do not allow to create default value, destination caps must be always explicitly inserted into container
-    can_create_default: ClassVar[bool] = False
-
-    @staticmethod
-    def generic_capabilities(preferred_loader_file_format: TLoaderFileFormat = None) -> "DestinationCapabilitiesContext":
-        caps = DestinationCapabilitiesContext()
-        caps.preferred_loader_file_format = preferred_loader_file_format
-        caps.supported_loader_file_formats = ["jsonl", "insert_values", "parquet"]
-        caps.escape_identifier = identity
-        caps.escape_literal = serialize_value
-        caps.max_identifier_length = 65536
-        caps.max_column_identifier_length = 65536
-        caps.max_query_length = 32 * 1024 * 1024
-        caps.is_max_query_length_in_bytes = True
-        caps.max_text_data_type_length = 1024 * 1024 * 1024
-        caps.is_max_text_data_type_length_in_bytes = True
-        caps.supports_ddl_transactions = True
-        return caps
+from dlt.common.schema.schema import Schema
+from dlt.common.configuration import with_config, known_sections
+from dlt.common.configuration.accessors import config
+from dlt.common.data_writers.escape import escape_postgres_identifier, escape_duckdb_literal
+from dlt.common.destination import DestinationCapabilitiesContext
+from dlt.common.destination.reference import JobClientBase, DestinationClientConfiguration
+from dlt.common.arithmetics import DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE
+
+from dlt.destinations.duckdb.configuration import DuckDbClientConfiguration
+
+
+@with_config(spec=DuckDbClientConfiguration, sections=(known_sections.DESTINATION, "duckdb",))
+def _configure(config: DuckDbClientConfiguration = config.value) -> DuckDbClientConfiguration:
+    return config
+
+
+def capabilities() -> DestinationCapabilitiesContext:
+    caps = DestinationCapabilitiesContext()
+    caps.preferred_loader_file_format = "insert_values"
+    caps.supported_loader_file_formats = ["insert_values", "parquet", "sql"]
+    caps.preferred_staging_file_format = None
+    caps.supported_staging_file_formats = []
+    caps.escape_identifier = escape_postgres_identifier
+    caps.escape_literal = escape_duckdb_literal
+    caps.decimal_precision = (DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE)
+    caps.wei_precision = (DEFAULT_NUMERIC_PRECISION, 0)
+    caps.max_identifier_length = 65536
+    caps.max_column_identifier_length = 65536
+    caps.naming_convention = "duck_case"
+    caps.max_query_length = 32 * 1024 * 1024
+    caps.is_max_query_length_in_bytes = True
+    caps.max_text_data_type_length = 1024 * 1024 * 1024
+    caps.is_max_text_data_type_length_in_bytes = True
+    caps.supports_ddl_transactions = True
+    caps.alter_add_multi_column = False
+
+    return caps
+
+
+def client(schema: Schema, initial_config: DestinationClientConfiguration = config.value) -> JobClientBase:
+    # import client when creating instance so capabilities and config specs can be accessed without dependencies installed
+    from dlt.destinations.duckdb.duck import DuckDbClient
+
+    return DuckDbClient(schema, _configure(initial_config))  # type: ignore
+
+
+def spec() -> Type[DestinationClientConfiguration]:
+    return DuckDbClientConfiguration
```

### Comparing `dlt-0.3.3a0/dlt/common/destination/reference.py` & `dlt-0.3.4/dlt/common/destination/reference.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,76 @@
 from abc import ABC, abstractmethod
 from importlib import import_module
 from types import TracebackType, ModuleType
-from typing import ClassVar, Final, Optional, Literal, Sequence, Iterable, Type, Protocol, Union, TYPE_CHECKING, cast
+from typing import ClassVar, Final, Optional, Literal, Sequence, Iterable, Type, Protocol, Union, TYPE_CHECKING, cast, List
 
 from dlt.common import logger
 from dlt.common.exceptions import IdentifierTooLongException, InvalidDestinationReference, UnknownDestinationModule
 from dlt.common.schema import Schema, TTableSchema, TSchemaTables
 from dlt.common.schema.exceptions import InvalidDatasetName
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import BaseConfiguration, CredentialsConfiguration
 from dlt.common.configuration.accessors import config
 from dlt.common.destination.capabilities import DestinationCapabilitiesContext
 from dlt.common.schema.utils import is_complete_column
 from dlt.common.storages import FileStorage
 from dlt.common.storages.load_storage import ParsedLoadJobFileName
 from dlt.common.utils import get_module_name
+from dlt.common.configuration.specs import GcpCredentials, AwsCredentialsWithoutDefaults
 
 
 @configspec(init=True)
 class DestinationClientConfiguration(BaseConfiguration):
     destination_name: str = None  # which destination to load data to
     credentials: Optional[CredentialsConfiguration]
 
     def __str__(self) -> str:
         """Return displayable destination location"""
         return str(self.credentials)
 
     if TYPE_CHECKING:
-        def __init__(self, destination_name: str = None, credentials: Optional[CredentialsConfiguration] = None) -> None:
+        def __init__(self, destination_name: str = None, credentials: Optional[CredentialsConfiguration] = None
+) -> None:
             ...
 
 
 @configspec(init=True)
 class DestinationClientDwhConfiguration(DestinationClientConfiguration):
     # keep default/initial value if present
     dataset_name: Final[str] = None
     """dataset name in the destination to load data to, for schemas that are not default schema, it is used as dataset prefix"""
     default_schema_name: Optional[str] = None
     """name of default schema to be used to name effective dataset to load data to"""
+    staging_credentials: Optional[CredentialsConfiguration] = None
 
     if TYPE_CHECKING:
         def __init__(
             self,
             destination_name: str = None,
             credentials: Optional[CredentialsConfiguration] = None,
             dataset_name: str = None,
-            default_schema_name: Optional[str] = None
+            default_schema_name: Optional[str] = None,
+            staging_credentials: Optional[CredentialsConfiguration] = None
         ) -> None:
             ...
 
+@configspec(init=True)
+class DestinationClientStagingConfiguration(DestinationClientDwhConfiguration):
+    as_staging: bool = False
+
+    if TYPE_CHECKING:
+        def __init__(
+            self,
+            destination_name: str = None,
+            credentials: Union[AwsCredentialsWithoutDefaults, GcpCredentials] = None,
+            dataset_name: str = None,
+            default_schema_name: Optional[str] = None,
+            as_staging: bool = False,
+        ) -> None:
+            ...
 
 TLoadJobState = Literal["running", "failed", "retry", "completed"]
 
 
 class LoadJob:
     """Represents a job that loads a single file
 
@@ -102,15 +120,16 @@
     def new_file_path(self) -> str:
         """Path to a newly created temporary job file. If empty, no followup job should be created"""
         pass
 
 
 class FollowupJob:
     """Adds a trait that allows to create a followup job"""
-    pass
+    def create_followup_jobs(self, next_state: str) -> List[NewLoadJob]:
+        return []
 
 
 class JobClientBase(ABC):
 
     capabilities: ClassVar[DestinationCapabilitiesContext] = None
 
     def __init__(self, schema: Schema, config: DestinationClientConfiguration) -> None:
```

### Comparing `dlt-0.3.3a0/dlt/common/exceptions.py` & `dlt-0.3.4/dlt/common/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, AnyStr, Sequence, Optional
+from typing import Any, AnyStr, List, Sequence, Optional, Iterable
 
 
 class DltException(Exception):
     def __reduce__(self) -> Any:
         """Enables exceptions with parametrized constructor to be pickled"""
         return type(self).__new__, (type(self), *self.args), self.__dict__
 
@@ -115,31 +115,60 @@
     pass
 
 
 class DestinationTransientException(DestinationException, TransientException):
     pass
 
 
+class DestinationLoadingViaStagingNotSupported(DestinationTerminalException):
+    def __init__(self, destination: str) -> None:
+        self.destination = destination
+        super().__init__(f"Destination {destination} does not support loading via staging.")
+
+
+class DestinationNoStagingMode(DestinationTerminalException):
+    def __init__(self, destination: str) -> None:
+        self.destination = destination
+        super().__init__(f"Destination {destination} cannot be used as a staging")
+
+
+class DestinationIncompatibleLoaderFileFormatException(DestinationTerminalException):
+    def __init__(self, destination: str, staging: str, file_format: str, supported_formats: Iterable[str]) -> None:
+        self.destination = destination
+        self.staging = staging
+        self.file_format = file_format
+        self.supported_formats = supported_formats
+        supported_formats_str = ", ".join(supported_formats)
+        if self.staging:
+            if not supported_formats:
+                msg = f"Staging {staging} cannot be used with destination {destination} because they have no file formats in common."
+            else:
+                msg = f"Unsupported file format {file_format} for destination {destination} in combination with staging destination {staging}. Supported formats: {supported_formats_str}"
+        else:
+            msg = f"Unsupported file format {file_format} destination {destination}. Supported formats: {supported_formats_str}. Check the staging option in the dlt.pipeline for additional formats."
+        super().__init__(msg)
+
+
 class IdentifierTooLongException(DestinationTerminalException):
     def __init__(self, destination_name: str, identifier_type: str, identifier_name: str, max_identifier_length: int) -> None:
         self.destination_name = destination_name
         self.identifier_type = identifier_type
         self.identifier_name = identifier_name
         self.max_identifier_length = max_identifier_length
         super().__init__(f"The length of {identifier_type} {identifier_name} exceeds {max_identifier_length} allowed for {destination_name}")
 
 
 class DestinationHasFailedJobs(DestinationTerminalException):
-    def __init__(self, destination_name: str, load_id: str) -> None:
+    def __init__(self, destination_name: str, load_id: str, failed_jobs: List[Any]) -> None:
         self.destination_name = destination_name
         self.load_id = load_id
+        self.failed_jobs = failed_jobs
         super().__init__(f"Destination {destination_name} has failed jobs in load package {load_id}")
 
 
-
 class PipelineException(DltException):
     def __init__(self, pipeline_name: str, msg: str) -> None:
         """Base class for all pipeline exceptions. Should not be raised."""
         self.pipeline_name = pipeline_name
         super().__init__(msg)
```

### Comparing `dlt-0.3.3a0/dlt/common/git.py` & `dlt-0.3.4/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/json/__init__.py` & `dlt-0.3.4/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/json/_orjson.py` & `dlt-0.3.4/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/json/_simplejson.py` & `dlt-0.3.4/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/jsonpath.py` & `dlt-0.3.4/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/normalizers/configuration.py` & `dlt-0.3.4/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/normalizers/json/__init__.py` & `dlt-0.3.4/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/normalizers/json/relational.py` & `dlt-0.3.4/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/normalizers/naming/direct.py` & `dlt-0.3.4/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.3.4/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.3.4/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/normalizers/naming/naming.py` & `dlt-0.3.4/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.3.4/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/normalizers/utils.py` & `dlt-0.3.4/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/pipeline.py` & `dlt-0.3.4/dlt/common/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import datetime  # noqa: 251
 import humanize
-import inspect
 import contextlib
 from typing import Any, Callable, ClassVar, Dict, List, NamedTuple, Optional, Protocol, Sequence, TYPE_CHECKING, Tuple, TypedDict
 
 from dlt.common import pendulum, logger
 from dlt.common.configuration import configspec
 from dlt.common.configuration import known_sections
 from dlt.common.configuration.container import Container
@@ -21,16 +20,24 @@
 from dlt.common.source import get_current_pipe_name
 from dlt.common.storages.load_storage import LoadPackageInfo
 from dlt.common.typing import DictStrAny, REPattern
 from dlt.common.jsonpath import delete_matches, TAnyJsonPath
 from dlt.common.data_writers.writers import TLoaderFileFormat
 
 
+class ExtractDataInfo(TypedDict):
+    name: str
+    data_type: str
+
+
 class ExtractInfo(NamedTuple):
     """A tuple holding information on extracted data items. Returned by pipeline `extract` method."""
+
+    extract_data_info: List[ExtractDataInfo]
+
     def asdict(self) -> DictStrAny:
         return {}
 
     def asstr(self, verbosity: int = 0) -> str:
         return ""
 
     def __str__(self) -> str:
@@ -50,14 +57,16 @@
 
 
 class LoadInfo(NamedTuple):
     """A tuple holding the information on recently loaded packages. Returned by pipeline `run` and `load` methods"""
     pipeline: "SupportsPipeline"
     destination_name: str
     destination_displayable_credentials: str
+    staging_name: str
+    staging_displayable_credentials: str
     dataset_name: str
     loads_ids: List[str]
     """ids of the loaded packages"""
     load_packages: List[LoadPackageInfo]
     """Information on loaded packages"""
     started_at: datetime.datetime
     first_run: bool
@@ -75,14 +84,17 @@
         msg = f"Pipeline {self.pipeline.pipeline_name} completed in "
         if self.started_at:
             elapsed = pendulum.now() - self.started_at
             msg += humanize.precisedelta(elapsed)
         else:
             msg += "---"
         msg += f"\n{len(self.loads_ids)} load package(s) were loaded to destination {self.destination_name} and into dataset {self.dataset_name}\n"
+        if self.staging_name:
+            msg += f"The {self.staging_name} staging destination used {self.staging_displayable_credentials} location to stage data\n"
+
         msg += f"The {self.destination_name} destination used {self.destination_displayable_credentials} location to store data"
         for load_package in self.load_packages:
             cstr = load_package.state.upper() if load_package.completed_at else "NOT COMPLETED"
             # now enumerate all complete loads if we have any failed packages
             # complete but failed job will not raise any exceptions
             failed_jobs = load_package.jobs["failed_jobs"]
             jobs_str = "no failed jobs" if not failed_jobs else f"{len(failed_jobs)} FAILED job(s)!"
@@ -102,16 +114,17 @@
             if len(load_package.jobs["failed_jobs"]):
                 return True
         return False
 
     def raise_on_failed_jobs(self) -> None:
         """Raises `DestinationHasFailedJobs` exception if any of the load packages has a failed job."""
         for load_package in self.load_packages:
-            if len(load_package.jobs["failed_jobs"]):
-                raise DestinationHasFailedJobs(self.destination_name, load_package.load_id)
+            failed_jobs = load_package.jobs["failed_jobs"]
+            if len(failed_jobs):
+                raise DestinationHasFailedJobs(self.destination_name, load_package.load_id, failed_jobs)
 
     def __str__(self) -> str:
         return self.asstr(verbosity=1)
 
 class TPipelineLocalState(TypedDict, total=False):
     first_run: bool
     """Indicates a first run of the pipeline, where run ends with successful loading of data"""
@@ -124,14 +137,15 @@
     pipeline_name: str
     dataset_name: str
     default_schema_name: Optional[str]
     """Name of the first schema added to the pipeline to which all the resources without schemas will be added"""
     schema_names: Optional[List[str]]
     """All the schemas present within the pipeline working directory"""
     destination: Optional[str]
+    staging: Optional[str]
 
     # properties starting with _ are not automatically applied to pipeline object when state is restored
     _state_version: int
     _state_engine_version: int
     _local: TPipelineLocalState
     """A section of state that is not synchronized with the destination and does not participate in change merging and version control"""
 
@@ -198,15 +212,16 @@
         *,
         destination: TDestinationReferenceArg = None,
         dataset_name: str = None,
         credentials: Any = None,
         table_name: str = None,
         write_disposition: TWriteDisposition = None,
         columns: Sequence[TColumnSchema] = None,
-        schema: Schema = None
+        schema: Schema = None,
+        loader_file_format: TLoaderFileFormat = None
     ) -> LoadInfo:
         ...
 
 
 @configspec(init=True)
 class PipelineContext(ContainerInjectableContext):
     _deferred_pipeline: Callable[[], SupportsPipeline]
```

### Comparing `dlt-0.3.3a0/dlt/common/reflection/spec.py` & `dlt-0.3.4/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/reflection/utils.py` & `dlt-0.3.4/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/runners/configuration.py` & `dlt-0.3.4/dlt/common/runners/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/runners/pool_runner.py` & `dlt-0.3.4/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/runners/runnable.py` & `dlt-0.3.4/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/runners/stdout.py` & `dlt-0.3.4/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/runners/synth_pickle.py` & `dlt-0.3.4/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/runners/venv.py` & `dlt-0.3.4/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/runtime/collector.py` & `dlt-0.3.4/dlt/common/runtime/collector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/runtime/exec_info.py` & `dlt-0.3.4/dlt/common/runtime/exec_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/runtime/init.py` & `dlt-0.3.4/dlt/common/runtime/init.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,20 +4,24 @@
 _INITIALIZED = False
 _RUN_CONFIGURATION: RunConfiguration = None
 
 
 def initialize_runtime(config: RunConfiguration) -> None:
     from dlt.common.runtime.logger import init_logging
     from dlt.common.runtime.telemetry import start_telemetry
+    from dlt.sources.helpers import requests
 
     global _INITIALIZED, _RUN_CONFIGURATION
 
     # initialize or re-initialize logging with new settings
     init_logging(config)
 
+    # Init or update default requests client config
+    requests.init(config)
+
     # initialize only once
     if not _INITIALIZED:
         start_telemetry(config)
         _INITIALIZED = True
 
     # store last config
     _RUN_CONFIGURATION = config
```

### Comparing `dlt-0.3.3a0/dlt/common/runtime/logger.py` & `dlt-0.3.4/dlt/common/runtime/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/runtime/prometheus.py` & `dlt-0.3.4/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/runtime/segment.py` & `dlt-0.3.4/dlt/common/runtime/segment.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 import requests
 import platform
 from concurrent.futures import ThreadPoolExecutor
 from typing import Literal, Optional
 from dlt.common.configuration.paths import get_dlt_data_dir
 
 from dlt.common.runtime import logger
+
 from dlt.common.configuration.specs import RunConfiguration
 from dlt.common.runtime.exec_info import exec_info_names, in_continuous_integration
 from dlt.common.typing import DictStrAny, StrAny
 from dlt.common.utils import uniq_id
 from dlt.version import __version__, DLT_PKG_NAME
 
-TEventCategory = Literal["pipeline", "command"]
+TEventCategory = Literal["pipeline", "command", "helper"]
 
 _THREAD_POOL: ThreadPoolExecutor = None
 _SESSION: requests.Session = None
 _WRITE_KEY: str = None
 _SEGMENT_REQUEST_TIMEOUT = (1.0, 1.0)  # short connect & send timeouts
 _SEGMENT_ENDPOINT = "https://api.segment.io/v1/track"
 _SEGMENT_CONTEXT: DictStrAny = None
@@ -198,17 +199,18 @@
         # If _WRITE_KEY is empty or `None`, telemetry has not been enabled
         logger.debug("Skipping request to external service: telemetry key not set.")
         return
 
     headers = _segment_request_header(_WRITE_KEY)
 
     def _future_send() -> None:
+        # import time
         # start_ts = time.time()
         resp = _SESSION.post(_SEGMENT_ENDPOINT, headers=headers, json=payload, timeout=_SEGMENT_REQUEST_TIMEOUT)
-        # print(f"sending to Segment done {resp.status_code} {time.time() - start_ts}")
+        # print(f"SENDING TO Segment done {resp.status_code} {time.time() - start_ts} {base64.b64decode(_WRITE_KEY)}")
         # handle different failure cases
         if resp.status_code != 200:
             logger.debug(
                 f"Segment telemetry request returned a {resp.status_code} response. "
                 f"Body: {resp.text}"
             )
         else:
```

### Comparing `dlt-0.3.3a0/dlt/common/runtime/sentry.py` & `dlt-0.3.4/dlt/common/runtime/sentry.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from dlt.common.runtime.exec_info import dlt_version_info, kube_pod_info, github_info
 
 
 def init_sentry(config: RunConfiguration) -> None:
     version = dlt_version_info(config.pipeline_name)
     sys_ver = version["dlt_version"]
     release = sys_ver + "_" + version.get("commit_sha", "")
-    _SentryHttpTransport.timeout = config.request_timeout[0]
+    _SentryHttpTransport.timeout = config.request_timeout
     # TODO: ignore certain loggers ie. dbt loggers
     # https://docs.sentry.io/platforms/python/guides/logging/
     sentry_sdk.init(
         config.sentry_dsn,
         before_send=before_send,
         traces_sample_rate=1.0,
         # disable tornado, boto3, sql alchemy etc.
@@ -49,15 +49,15 @@
 def before_send(event: DictStrAny, _unused_hint: Optional[StrAny] = None) -> Optional[DictStrAny]:
     """Called by sentry before sending event. Does nothing, patch this function in the module for custom behavior"""
     return event
 
 
 class _SentryHttpTransport(HttpTransport):
 
-    timeout: int = 0
+    timeout: float = 0
 
     def _get_pool_options(self, *a: Any, **kw: Any) -> DictStrAny:
         rv = HttpTransport._get_pool_options(self, *a, **kw)
         rv['timeout'] = self.timeout
         return rv
```

### Comparing `dlt-0.3.3a0/dlt/common/runtime/signals.py` & `dlt-0.3.4/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/runtime/slack.py` & `dlt-0.3.4/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/schema/detections.py` & `dlt-0.3.4/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/schema/exceptions.py` & `dlt-0.3.4/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/schema/schema.py` & `dlt-0.3.4/dlt/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/schema/typing.py` & `dlt-0.3.4/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/schema/utils.py` & `dlt-0.3.4/dlt/common/schema/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,14 +414,19 @@
     parent = table.get("parent")
     if parent:
         return get_write_disposition(tables, parent)
 
     raise ValueError(f"No write disposition found in the chain of tables for '{table_name}'.")
 
 
+def table_schema_has_type(table: TTableSchema, _typ: TDataType) -> bool:
+    """Checks if `table` schema contains column with type _typ"""
+    return any(c["data_type"] == _typ for c in table["columns"].values())
+
+
 def get_top_level_table(tables: TSchemaTables, table_name: str) -> TTableSchema:
     """Finds top level (without parent) of a `table_name` following the ancestry hierarchy."""
     table = tables[table_name]
     parent = table.get("parent")
     if parent:
         return get_top_level_table(tables, parent)
     return table
```

### Comparing `dlt-0.3.3a0/dlt/common/source.py` & `dlt-0.3.4/dlt/common/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/storages/__init__.py` & `dlt-0.3.4/dlt/common/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/storages/configuration.py` & `dlt-0.3.4/dlt/common/storages/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/storages/data_item_storage.py` & `dlt-0.3.4/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/storages/exceptions.py` & `dlt-0.3.4/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/storages/file_storage.py` & `dlt-0.3.4/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/storages/live_schema_storage.py` & `dlt-0.3.4/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/storages/load_storage.py` & `dlt-0.3.4/dlt/common/storages/load_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/storages/normalize_storage.py` & `dlt-0.3.4/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/storages/schema_storage.py` & `dlt-0.3.4/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/storages/transactional_file.py` & `dlt-0.3.4/dlt/common/storages/transactional_file.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/storages/versioned_storage.py` & `dlt-0.3.4/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/time.py` & `dlt-0.3.4/dlt/common/time.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/typing.py` & `dlt-0.3.4/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/utils.py` & `dlt-0.3.4/dlt/common/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/validation.py` & `dlt-0.3.4/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/common/wei.py` & `dlt-0.3.4/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/destinations/bigquery/__init__.py` & `dlt-0.3.4/dlt/destinations/bigquery/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,29 +2,34 @@
 from dlt.common.data_writers.escape import escape_bigquery_identifier
 
 from dlt.common.schema.schema import Schema
 from dlt.common.configuration import with_config, known_sections
 from dlt.common.configuration.accessors import config
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import JobClientBase, DestinationClientConfiguration
+from dlt.common.arithmetics import DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE
 
 from dlt.destinations.bigquery.configuration import BigQueryClientConfiguration
 
 
 @with_config(spec=BigQueryClientConfiguration, sections=(known_sections.DESTINATION, "bigquery",))
 def _configure(config: BigQueryClientConfiguration = config.value) -> BigQueryClientConfiguration:
     return config
 
 
 def capabilities() -> DestinationCapabilitiesContext:
     caps = DestinationCapabilitiesContext()
     caps.preferred_loader_file_format = "jsonl"
     caps.supported_loader_file_formats = ["jsonl", "sql", "parquet"]
+    caps.preferred_staging_file_format = "parquet"
+    caps.supported_staging_file_formats = ["parquet", "jsonl"]
     caps.escape_identifier = escape_bigquery_identifier
     caps.escape_literal = None
+    caps.decimal_precision = (DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE)
+    caps.wei_precision = (76, 38)
     caps.max_identifier_length = 1024
     caps.max_column_identifier_length = 300
     caps.max_query_length = 1024 * 1024
     caps.is_max_query_length_in_bytes = False
     caps.max_text_data_type_length = 10 * 1024 * 1024
     caps.is_max_text_data_type_length_in_bytes = True
     caps.supports_ddl_transactions = False
```

### Comparing `dlt-0.3.3a0/dlt/destinations/bigquery/bigquery.py` & `dlt-0.3.4/dlt/destinations/bigquery/bigquery.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,43 @@
+import os
 from pathlib import Path
-from typing import ClassVar, Dict, Optional, Sequence, Tuple, List, cast
+from typing import ClassVar, Dict, Optional, Sequence, Tuple, List, cast, Type
 import google.cloud.bigquery as bigquery  # noqa: I250
 from google.cloud import exceptions as gcp_exceptions
 from google.api_core import exceptions as api_core_exceptions
 
 from dlt.common import json, logger
-from dlt.common.arithmetics import DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE
-from dlt.common.configuration.specs import GcpServiceAccountCredentialsWithoutDefaults
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import FollowupJob, NewLoadJob, TLoadJobState, LoadJob
 from dlt.common.data_types import TDataType
 from dlt.common.storages.file_storage import FileStorage
 from dlt.common.schema import TColumnSchema, Schema, TTableSchemaColumns
 from dlt.common.schema.typing import TTableSchema, TWriteDisposition
 
 from dlt.destinations.job_client_impl import SqlJobClientBase
 from dlt.destinations.exceptions import DestinationSchemaWillNotUpdate, DestinationTransientException, LoadJobNotExistsException, LoadJobTerminalException, LoadJobUnknownTableException
 
 from dlt.destinations.bigquery import capabilities
 from dlt.destinations.bigquery.configuration import BigQueryClientConfiguration
 from dlt.destinations.bigquery.sql_client import BigQuerySqlClient, BQ_TERMINAL_REASONS
 from dlt.destinations.sql_merge_job import SqlMergeJob
+from dlt.destinations.job_impl import NewReferenceJob
 
+from dlt.common.schema.utils import table_schema_has_type
 
 SCT_TO_BQT: Dict[TDataType, str] = {
     "complex": "JSON",
     "text": "STRING",
     "double": "FLOAT64",
     "bool": "BOOLEAN",
     "date": "DATE",
     "timestamp": "TIMESTAMP",
     "bigint": "INTEGER",
     "binary": "BYTES",
-    "decimal": f"NUMERIC({DEFAULT_NUMERIC_PRECISION},{DEFAULT_NUMERIC_SCALE})",
+    "decimal": "NUMERIC(%i,%i)",
     "wei": "BIGNUMERIC"  # non parametrized should hold wei values
 }
 
 BQT_TO_SCT: Dict[str, TDataType] = {
     "STRING": "text",
     "FLOAT": "double",
     "BOOLEAN": "bool",
@@ -46,23 +47,29 @@
     "BYTES": "binary",
     "NUMERIC": "decimal",
     "BIGNUMERIC": "decimal",
     "JSON": "complex"
 }
 
 class BigQueryLoadJob(LoadJob, FollowupJob):
-    def __init__(self, file_name: str, bq_load_job: bigquery.LoadJob, credentials: GcpServiceAccountCredentialsWithoutDefaults) -> None:
+    def __init__(
+        self,
+        file_name: str,
+        bq_load_job: bigquery.LoadJob,
+        http_timeout: float,
+        retry_deadline: float
+    ) -> None:
         self.bq_load_job = bq_load_job
-        self.credentials = credentials
-        self.default_retry = bigquery.DEFAULT_RETRY.with_deadline(credentials.retry_deadline)
+        self.default_retry = bigquery.DEFAULT_RETRY.with_deadline(retry_deadline)
+        self.http_timeout = http_timeout
         super().__init__(file_name)
 
     def state(self) -> TLoadJobState:
         # check server if done
-        done = self.bq_load_job.done(retry=self.default_retry, timeout=self.credentials.http_timeout)
+        done = self.bq_load_job.done(retry=self.default_retry, timeout=self.http_timeout)
         if done:
             # rows processed
             if self.bq_load_job.output_rows is not None and self.bq_load_job.error_result is None:
                 return "completed"
             else:
                 reason = self.bq_load_job.error_result.get("reason")
                 if reason in BQ_TERMINAL_REASONS:
@@ -110,15 +117,18 @@
 class BigQueryClient(SqlJobClientBase):
 
     capabilities: ClassVar[DestinationCapabilitiesContext] = capabilities()
 
     def __init__(self, schema: Schema, config: BigQueryClientConfiguration) -> None:
         sql_client = BigQuerySqlClient(
             self.make_dataset_name(schema, config.dataset_name, config.default_schema_name),
-            config.credentials
+            config.credentials,
+            config.get_location(),
+            config.http_timeout,
+            config.retry_deadline
         )
         super().__init__(schema, config, sql_client)
         self.config: BigQueryClientConfiguration = config
         self.sql_client: BigQuerySqlClient = sql_client  # type: ignore
 
     def create_merge_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
         return BigQueryMergeJob.from_table_chain(table_chain, self.sql_client)
@@ -136,47 +146,49 @@
         """
         job = super().restore_file_load(file_path)
         if not job:
             try:
                 job = BigQueryLoadJob(
                     FileStorage.get_file_name_from_file_path(file_path),
                     self._retrieve_load_job(file_path),
-                    self.config.credentials
-                    #self.sql_client.native_connection()
+                    self.config.http_timeout,
+                    self.config.retry_deadline
                 )
             except api_core_exceptions.GoogleAPICallError as gace:
                 reason = BigQuerySqlClient._get_reason_from_errors(gace)
                 if reason == "notFound":
                     raise LoadJobNotExistsException(file_path)
                 elif reason in BQ_TERMINAL_REASONS:
-                    raise LoadJobTerminalException(file_path)
+                    raise LoadJobTerminalException(file_path, f"The server reason was: {reason}")
                 else:
                     raise DestinationTransientException(gace)
         return job
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         job = super().start_file_load(table, file_path, load_id)
+
         if not job:
             try:
                 job = BigQueryLoadJob(
                     FileStorage.get_file_name_from_file_path(file_path),
-                    self._create_load_job(table["name"], table["write_disposition"], file_path),
-                    self.config.credentials
+                    self._create_load_job(table, file_path),
+                    self.config.http_timeout,
+                    self.config.retry_deadline
                 )
             except api_core_exceptions.GoogleAPICallError as gace:
                 reason = BigQuerySqlClient._get_reason_from_errors(gace)
                 if reason == "notFound":
                     # google.api_core.exceptions.NotFound: 404 - table not found
                     raise LoadJobUnknownTableException(table["name"], file_path)
                 elif reason == "duplicate":
                     # google.api_core.exceptions.Conflict: 409 PUT - already exists
                     return self.restore_file_load(file_path)
                 elif reason in BQ_TERMINAL_REASONS:
                     # google.api_core.exceptions.BadRequest - will not be processed ie bad job name
-                    raise LoadJobTerminalException(file_path)
+                    raise LoadJobTerminalException(file_path, f"The server reason was: {reason}")
                 else:
                     raise DestinationTransientException(gace)
         return job
 
     def _get_table_update_sql(self, table_name: str, new_columns: Sequence[TColumnSchema], generate_alter: bool, separate_alters: bool = False) -> List[str]:
         sql = super()._get_table_update_sql(table_name, new_columns, generate_alter)
         canonical_name = self.sql_client.make_qualified_table_name(table_name)
@@ -201,15 +213,15 @@
 
     def get_storage_table(self, table_name: str) -> Tuple[bool, TTableSchemaColumns]:
         schema_table: TTableSchemaColumns = {}
         try:
             table = self.sql_client.native_connection.get_table(
                 self.sql_client.make_qualified_table_name(table_name, escape=False),
                 retry=self.sql_client._default_retry,
-                timeout=self.config.credentials.http_timeout
+                timeout=self.config.http_timeout
             )
             partition_field = table.time_partitioning.field if table.time_partitioning else None
             for c in table.schema:
                 schema_c: TColumnSchema = {
                     "name": c.name,
                     "nullable": c.is_nullable,
                     "data_type": self._from_db_type(c.field_type, c.precision, c.scale),
@@ -221,49 +233,79 @@
                     "partition": c.name == partition_field
                 }
                 schema_table[c.name] = schema_c
             return True, schema_table
         except gcp_exceptions.NotFound:
             return False, schema_table
 
-    def _create_load_job(self, table_name: str, write_disposition: TWriteDisposition, file_path: str) -> bigquery.LoadJob:
+    def _create_load_job(self, table: TTableSchema, file_path: str) -> bigquery.LoadJob:
+        table_name = table["name"]
+        write_disposition = table["write_disposition"]
         # append to table for merge loads (append to stage) and regular appends
         bq_wd = bigquery.WriteDisposition.WRITE_TRUNCATE if write_disposition == "replace" else bigquery.WriteDisposition.WRITE_APPEND
 
+        # determine wether we load from local or uri
+        bucket_path = None
+        ext: str = os.path.splitext(file_path)[1][1:]
+        if NewReferenceJob.is_reference_job(file_path):
+            bucket_path = NewReferenceJob.resolve_reference(file_path)
+            ext = os.path.splitext(bucket_path)[1][1:]
+
         # choose correct source format
         source_format = bigquery.SourceFormat.NEWLINE_DELIMITED_JSON
-        if file_path.endswith("parquet"):
+        decimal_target_types: List[str] = None
+        if ext == "parquet":
+            # if table contains complex types, we cannot load with parquet
+            if table_schema_has_type(table, "complex"):
+                raise LoadJobTerminalException(file_path, "Bigquery cannot load into JSON data type from parquet. Use jsonl instead.")
             source_format = bigquery.SourceFormat.PARQUET
+            # parquet needs NUMERIC type autodetection
+            decimal_target_types = ["NUMERIC", "BIGNUMERIC"]
 
         # if merge then load to staging
         with self.sql_client.with_staging_dataset(write_disposition == "merge"):
             job_id = BigQueryLoadJob.get_job_id_from_file_path(file_path)
             job_config = bigquery.LoadJobConfig(
                 autodetect=False,
                 write_disposition=bq_wd,
                 create_disposition=bigquery.CreateDisposition.CREATE_NEVER,
                 source_format=source_format,
+                decimal_target_types=decimal_target_types,
                 ignore_unknown_values=False,
                 max_bad_records=0)
+
+            if bucket_path:
+                return self.sql_client.native_connection.load_table_from_uri(
+                        bucket_path,
+                        self.sql_client.make_qualified_table_name(table_name, escape=False),
+                        job_id=job_id,
+                        job_config=job_config,
+                        timeout=self.config.file_upload_timeout
+                    )
+
             with open(file_path, "rb") as f:
                 return self.sql_client.native_connection.load_table_from_file(
                         f,
                         self.sql_client.make_qualified_table_name(table_name, escape=False),
                         job_id=job_id,
                         job_config=job_config,
-                        timeout=self.config.credentials.file_upload_timeout
+                        timeout=self.config.file_upload_timeout
                     )
 
     def _retrieve_load_job(self, file_path: str) -> bigquery.LoadJob:
         job_id = BigQueryLoadJob.get_job_id_from_file_path(file_path)
         return cast(bigquery.LoadJob, self.sql_client.native_connection.get_job(job_id))
 
-    @staticmethod
-    def _to_db_type(sc_t: TDataType) -> str:
+    @classmethod
+    def _to_db_type(cls, sc_t: TDataType) -> str:
+        if sc_t == "decimal":
+            return SCT_TO_BQT["decimal"] % cls.capabilities.decimal_precision
         return SCT_TO_BQT[sc_t]
 
-    @staticmethod
-    def _from_db_type(bq_t: str, precision: Optional[int], scale: Optional[int]) -> TDataType:
+    @classmethod
+    def _from_db_type(cls, bq_t: str, precision: Optional[int], scale: Optional[int]) -> TDataType:
         if bq_t == "BIGNUMERIC":
             if precision is None:  # biggest numeric possible
                 return "wei"
         return BQT_TO_SCT.get(bq_t, "text")
+
+
```

### Comparing `dlt-0.3.3a0/dlt/destinations/bigquery/sql_client.py` & `dlt-0.3.4/dlt/destinations/bigquery/sql_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from contextlib import contextmanager
-from typing import Any, AnyStr, ClassVar, Iterator, List, Optional, Sequence
+from typing import Any, AnyStr, ClassVar, Iterator, List, Optional, Sequence, Type
 
 import google.cloud.bigquery as bigquery  # noqa: I250
 from google.cloud.bigquery import dbapi as bq_dbapi
 from google.cloud.bigquery.dbapi import Connection as DbApiConnection, Cursor as BQDbApiCursor
 from google.cloud import exceptions as gcp_exceptions
 from google.cloud.bigquery.dbapi import exceptions as dbapi_exceptions
 from google.api_core import exceptions as api_core_exceptions
@@ -43,38 +43,48 @@
 
 
 class BigQuerySqlClient(SqlClientBase[bigquery.Client], DBTransaction):
 
     dbapi: ClassVar[DBApi] = bq_dbapi
     capabilities: ClassVar[DestinationCapabilitiesContext] = capabilities()
 
-    def __init__(self, dataset_name: str, credentials: GcpServiceAccountCredentialsWithoutDefaults) -> None:
+    def __init__(
+        self,
+        dataset_name: str,
+        credentials: GcpServiceAccountCredentialsWithoutDefaults,
+        location: str = "US",
+        http_timeout: float = 15.0,
+        retry_deadline: float = 60.0
+    ) -> None:
         self._client: bigquery.Client = None
         self.credentials: GcpServiceAccountCredentialsWithoutDefaults = credentials
+        self.location = location
+        self.http_timeout = http_timeout
         super().__init__(credentials.project_id, dataset_name)
 
-        self._default_retry = bigquery.DEFAULT_RETRY.with_deadline(credentials.retry_deadline)
+        self._default_retry = bigquery.DEFAULT_RETRY.with_deadline(retry_deadline)
         self._default_query = bigquery.QueryJobConfig(default_dataset=self.fully_qualified_dataset_name(escape=False))
         self._session_query: bigquery.QueryJobConfig = None
 
+
     @raise_open_connection_error
     def open_connection(self) -> bigquery.Client:
         self._client = bigquery.Client(
             self.credentials.project_id,
             credentials=self.credentials.to_native_credentials(),
-            location=self.credentials.location
+            location=self.location
         )
 
         # patch the client query so our defaults are used
         query_orig = self._client.query
 
         def query_patch(
             query: str,
             retry: Any = self._default_retry,
-            timeout: Any = self.credentials.http_timeout,
+            timeout: Any = self.http_timeout,
             **kwargs: Any
         ) -> Any:
             return query_orig(query, retry=retry, timeout=timeout, **kwargs)
 
         self._client.query = query_patch  # type: ignore
         return self._client
 
@@ -136,34 +146,34 @@
 
     @property
     def native_connection(self) -> bigquery.Client:
         return self._client
 
     def has_dataset(self) -> bool:
         try:
-            self._client.get_dataset(self.fully_qualified_dataset_name(escape=False), retry=self._default_retry, timeout=self.credentials.http_timeout)
+            self._client.get_dataset(self.fully_qualified_dataset_name(escape=False), retry=self._default_retry, timeout=self.http_timeout)
             return True
         except gcp_exceptions.NotFound:
             return False
 
     def create_dataset(self) -> None:
         self._client.create_dataset(
             self.fully_qualified_dataset_name(escape=False),
             exists_ok=False,
             retry=self._default_retry,
-            timeout=self.credentials.http_timeout
+            timeout=self.http_timeout
         )
 
     def drop_dataset(self) -> None:
         self._client.delete_dataset(
             self.fully_qualified_dataset_name(escape=False),
             not_found_ok=True,
             delete_contents=True,
             retry=self._default_retry,
-            timeout=self.credentials.http_timeout
+            timeout=self.http_timeout
         )
 
     def execute_sql(self, sql: AnyStr, *args: Any, **kwargs: Any) -> Optional[Sequence[Sequence[Any]]]:
         with self.execute_query(sql, *args, **kwargs) as curr:
             if not curr.description:
                 return None
             else:
```

### Comparing `dlt-0.3.3a0/dlt/destinations/duckdb/__init__.py` & `dlt-0.3.4/dlt/destinations/postgres/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 from typing import Type
 
 from dlt.common.schema.schema import Schema
 from dlt.common.configuration import with_config, known_sections
 from dlt.common.configuration.accessors import config
-from dlt.common.data_writers.escape import escape_postgres_identifier, escape_duckdb_literal
+from dlt.common.data_writers.escape import escape_postgres_identifier, escape_postgres_literal
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import JobClientBase, DestinationClientConfiguration
+from dlt.common.arithmetics import DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE
+from dlt.common.wei import EVM_DECIMAL_PRECISION
 
-from dlt.destinations.duckdb.configuration import DuckDbClientConfiguration
+from dlt.destinations.postgres.configuration import PostgresClientConfiguration
 
 
-@with_config(spec=DuckDbClientConfiguration, sections=(known_sections.DESTINATION, "duckdb",))
-def _configure(config: DuckDbClientConfiguration = config.value) -> DuckDbClientConfiguration:
+@with_config(spec=PostgresClientConfiguration, sections=(known_sections.DESTINATION, "postgres",))
+def _configure(config: PostgresClientConfiguration = config.value) -> PostgresClientConfiguration:
     return config
 
 
 def capabilities() -> DestinationCapabilitiesContext:
+    # https://www.postgresql.org/docs/current/limits.html
     caps = DestinationCapabilitiesContext()
     caps.preferred_loader_file_format = "insert_values"
-    caps.supported_loader_file_formats = ["insert_values", "parquet", "sql"]
+    caps.supported_loader_file_formats = ["insert_values", "sql"]
+    caps.preferred_staging_file_format = None
+    caps.supported_staging_file_formats = []
     caps.escape_identifier = escape_postgres_identifier
-    caps.escape_literal = escape_duckdb_literal
-    caps.max_identifier_length = 65536
-    caps.max_column_identifier_length = 65536
-    caps.naming_convention = "duck_case"
+    caps.escape_literal = escape_postgres_literal
+    caps.decimal_precision = (DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE)
+    caps.wei_precision = (2*EVM_DECIMAL_PRECISION, EVM_DECIMAL_PRECISION)
+    caps.max_identifier_length = 63
+    caps.max_column_identifier_length = 63
     caps.max_query_length = 32 * 1024 * 1024
     caps.is_max_query_length_in_bytes = True
     caps.max_text_data_type_length = 1024 * 1024 * 1024
     caps.is_max_text_data_type_length_in_bytes = True
     caps.supports_ddl_transactions = True
-    caps.alter_add_multi_column = False
 
     return caps
 
 
 def client(schema: Schema, initial_config: DestinationClientConfiguration = config.value) -> JobClientBase:
     # import client when creating instance so capabilities and config specs can be accessed without dependencies installed
-    from dlt.destinations.duckdb.duck import DuckDbClient
+    from dlt.destinations.postgres.postgres import PostgresClient
 
-    return DuckDbClient(schema, _configure(initial_config))  # type: ignore
+    return PostgresClient(schema, _configure(initial_config))  # type: ignore
 
 
 def spec() -> Type[DestinationClientConfiguration]:
-    return DuckDbClientConfiguration
+    return PostgresClientConfiguration
```

### Comparing `dlt-0.3.3a0/dlt/destinations/duckdb/configuration.py` & `dlt-0.3.4/dlt/destinations/duckdb/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/destinations/duckdb/duck.py` & `dlt-0.3.4/dlt/destinations/duckdb/duck.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 from typing import ClassVar, Dict, Optional
 
-from dlt.common.arithmetics import DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.data_types import TDataType
 from dlt.common.schema import TColumnSchema, TColumnHint, Schema
+from dlt.common.destination.reference import LoadJob, FollowupJob, TLoadJobState
+from dlt.common.schema.typing import TTableSchema, TWriteDisposition
+from dlt.common.storages.file_storage import FileStorage
 
 from dlt.destinations.insert_job_client import InsertValuesJobClient
 
 from dlt.destinations.duckdb import capabilities
 from dlt.destinations.duckdb.sql_client import DuckDbSqlClient
 from dlt.destinations.duckdb.configuration import DuckDbClientConfiguration
 
-from dlt.common.destination.reference import LoadJob, FollowupJob, TLoadJobState
-
-from dlt.common.schema.typing import TTableSchema, TWriteDisposition
-
-from dlt.common.storages.file_storage import FileStorage
-
 
 SCT_TO_PGT: Dict[TDataType, str] = {
     "complex": "JSON",
     "text": "VARCHAR",
     "double": "DOUBLE",
     "bool": "BOOLEAN",
     "date": "DATE",
     "timestamp": "TIMESTAMP WITH TIME ZONE",
     "bigint": "BIGINT",
     "binary": "BLOB",
-    "decimal": f"DECIMAL({DEFAULT_NUMERIC_PRECISION},{DEFAULT_NUMERIC_SCALE})"
+    "decimal": "DECIMAL(%i,%i)"
 }
 
 PGT_TO_SCT: Dict[str, TDataType] = {
     "VARCHAR": "text",
     "JSON": "complex",
     "DOUBLE": "double",
     "BOOLEAN": "bool",
@@ -85,21 +81,23 @@
         return super().start_file_load(table, file_path, load_id)
 
     def _get_column_def_sql(self, c: TColumnSchema) -> str:
         hints_str = " ".join(self.active_hints.get(h, "") for h in self.active_hints.keys() if c.get(h, False) is True)
         column_name = self.capabilities.escape_identifier(c["name"])
         return f"{column_name} {self._to_db_type(c['data_type'])} {hints_str} {self._gen_not_null(c['nullable'])}"
 
-    @staticmethod
-    def _to_db_type(sc_t: TDataType) -> str:
+    @classmethod
+    def _to_db_type(cls, sc_t: TDataType) -> str:
         if sc_t == "wei":
-            return "DECIMAL(38,0)"
+            return SCT_TO_PGT["decimal"] % cls.capabilities.wei_precision
+        if sc_t == "decimal":
+            return SCT_TO_PGT["decimal"] % cls.capabilities.decimal_precision
         return SCT_TO_PGT[sc_t]
 
-    @staticmethod
-    def _from_db_type(pq_t: str, precision: Optional[int], scale: Optional[int]) -> TDataType:
+    @classmethod
+    def _from_db_type(cls, pq_t: str, precision: Optional[int], scale: Optional[int]) -> TDataType:
         # duckdb provides the types with scale and precision
         pq_t = pq_t.split("(")[0].upper()
         if pq_t == "DECIMAL":
             if precision == 38 and scale == 0:
                 return "wei"
         return PGT_TO_SCT[pq_t]
```

### Comparing `dlt-0.3.3a0/dlt/destinations/duckdb/sql_client.py` & `dlt-0.3.4/dlt/destinations/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/destinations/dummy/__init__.py` & `dlt-0.3.4/dlt/destinations/dummy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 
 
 def capabilities() -> DestinationCapabilitiesContext:
     config = _configure()
     caps = DestinationCapabilitiesContext()
     caps.preferred_loader_file_format = config.loader_file_format
     caps.supported_loader_file_formats = [config.loader_file_format]
-
+    caps.preferred_staging_file_format = None
+    caps.supported_staging_file_formats = []
     caps.max_identifier_length = 127
     caps.max_column_identifier_length = 127
     caps.max_query_length = 8 * 1024 * 1024
     caps.is_max_query_length_in_bytes = True
     caps.max_text_data_type_length = 65536
     caps.is_max_text_data_type_length_in_bytes = True
     caps.supports_ddl_transactions = False
```

### Comparing `dlt-0.3.3a0/dlt/destinations/dummy/configuration.py` & `dlt-0.3.4/dlt/destinations/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/destinations/dummy/dummy.py` & `dlt-0.3.4/dlt/destinations/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/destinations/exceptions.py` & `dlt-0.3.4/dlt/destinations/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 
 class LoadJobNotExistsException(DestinationTerminalException):
     def __init__(self, job_id: str) -> None:
         super().__init__(f"Job with id/file name {job_id} not found")
 
 
 class LoadJobTerminalException(DestinationTerminalException):
-    def __init__(self, file_path: str) -> None:
-        super().__init__(f"Job with id/file name {file_path} encountered unrecoverable problem")
+    def __init__(self, file_path: str, message: str) -> None:
+        super().__init__(f"Job with id/file name {file_path} encountered unrecoverable problem: {message}")
 
 
 class LoadJobUnknownTableException(DestinationTerminalException):
     def __init__(self, table_name: str, file_name: str) -> None:
         self.table_name = table_name
         super().__init__(f"Client does not know table {table_name} for load file {file_name}")
```

### Comparing `dlt-0.3.3a0/dlt/destinations/filesystem/__init__.py` & `dlt-0.3.4/dlt/destinations/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/destinations/filesystem/configuration.py` & `dlt-0.3.4/dlt/destinations/filesystem/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from urllib.parse import urlparse
 
 from typing import Final, Type, Optional, Union
 
 from dlt.common.configuration import configspec, resolve_type
-from dlt.common.destination.reference import CredentialsConfiguration, DestinationClientDwhConfiguration
+from dlt.common.destination.reference import CredentialsConfiguration, DestinationClientStagingConfiguration
 from dlt.common.configuration.specs import GcpCredentials, GcpServiceAccountCredentials, AwsCredentials, GcpOAuthCredentials
 
 from dlt.common.configuration.exceptions import ConfigurationValueError
 
 
 PROTOCOL_CREDENTIALS = {
     "gs": Union[GcpServiceAccountCredentials, GcpOAuthCredentials],
     "gcs": Union[GcpServiceAccountCredentials, GcpOAuthCredentials],
     "gdrive": GcpOAuthCredentials,
     "s3": AwsCredentials
 }
 
 
 @configspec(init=True)
-class FilesystemClientConfiguration(DestinationClientDwhConfiguration):
-    credentials: Union[AwsCredentials, GcpCredentials]
-
+class FilesystemClientConfiguration(DestinationClientStagingConfiguration):
     destination_name: Final[str] = "filesystem"  # type: ignore
+    credentials: Union[AwsCredentials, GcpCredentials]
     bucket_url: str
 
     @property
     def protocol(self) -> str:
         url = urlparse(self.bucket_url)
         return url.scheme or "file"
```

### Comparing `dlt-0.3.3a0/dlt/destinations/filesystem/filesystem.py` & `dlt-0.3.4/dlt/destinations/filesystem/filesystem.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import posixpath
 import threading
+import os
 from types import TracebackType
-from typing import ClassVar, List, Sequence, Type, Iterable
+from typing import ClassVar, List, Sequence, Type, Iterable, cast
 from fsspec import AbstractFileSystem
 
 from dlt.common.schema import Schema, TTableSchema
 from dlt.common.schema.typing import TWriteDisposition, LOADS_TABLE_NAME
 from dlt.common.storages import FileStorage
 from dlt.common.destination import DestinationCapabilitiesContext
-from dlt.common.destination.reference import NewLoadJob, TLoadJobState, LoadJob, JobClientBase
+from dlt.common.destination.reference import NewLoadJob, TLoadJobState, LoadJob, JobClientBase, FollowupJob
 from dlt.destinations.job_impl import EmptyLoadJob
 from dlt.destinations.filesystem import capabilities
 from dlt.destinations.filesystem.configuration import FilesystemClientConfiguration
 from dlt.destinations.filesystem.filesystem_client import client_from_config
 from dlt.common.storages import LoadStorage
+from dlt.destinations.job_impl import NewLoadJobImpl
+from dlt.destinations.job_impl import NewReferenceJob
 
 
 class LoadFilesystemJob(LoadJob):
     def __init__(
             self,
             local_path: str,
             dataset_path: str,
@@ -25,14 +28,17 @@
             config: FilesystemClientConfiguration,
             write_disposition: TWriteDisposition,
             has_merge_keys: bool,
             schema_name: str,
             load_id: str
     ) -> None:
         file_name = FileStorage.get_file_name_from_file_path(local_path)
+        self.config = config
+        self.dataset_path = dataset_path
+
         super().__init__(file_name)
         fs_client, _ = client_from_config(config)
 
         # fallback to replace for merge without any merge keys
         if write_disposition == 'merge':
             write_disposition = 'append' if has_merge_keys else 'replace'
 
@@ -45,29 +51,41 @@
             items = [item for item in all_files if item.startswith(search_prefix)]
             # NOTE: deleting in chunks on s3 does not raise on access denied, file non existing and probably other errors
             # if items:
             #     fs_client.rm(items[0])
             for item in items:
                 fs_client.rm_file(item)
 
-        destination_file_name = LoadFilesystemJob.make_destination_filename(file_name, schema_name, load_id)
-        fs_client.put_file(local_path, posixpath.join(dataset_path, destination_file_name))
+        self.destination_file_name = LoadFilesystemJob.make_destination_filename(file_name, schema_name, load_id)
+        fs_client.put_file(local_path, self.make_remote_path())
 
     @staticmethod
     def make_destination_filename(file_name: str, schema_name: str, load_id: str) -> str:
         job_info = LoadStorage.parse_job_file_name(file_name)
         return f"{schema_name}.{job_info.table_name}.{load_id}.{job_info.file_id}.{job_info.file_format}"
 
+    def make_remote_path(self) -> str:
+        return f"{self.config.protocol}://{posixpath.join(self.dataset_path, self.destination_file_name)}"
+
     def state(self) -> TLoadJobState:
         return "completed"
 
     def exception(self) -> str:
         raise NotImplementedError()
 
 
+class FollowupFilesystemJob(FollowupJob, LoadFilesystemJob):
+    def create_followup_jobs(self, next_state: str) -> List[NewLoadJob]:
+        jobs = super().create_followup_jobs(next_state)
+        if next_state == "completed":
+            ref_job = NewReferenceJob(file_name=self.file_name(), status="running", remote_path=self.make_remote_path())
+            jobs.append(ref_job)
+        return jobs
+
+
 class FilesystemClient(JobClientBase):
     """filesystem client storing jobs in memory"""
 
     capabilities: ClassVar[DestinationCapabilitiesContext] = capabilities()
     fs_client: AbstractFileSystem
     fs_path: str
 
@@ -83,16 +101,17 @@
     def initialize_storage(self, staging: bool = False, truncate_tables: Iterable[str] = None) -> None:
         self.fs_client.makedirs(self.dataset_path, exist_ok=True)
 
     def is_storage_initialized(self, staging: bool = False) -> bool:
         return self.fs_client.isdir(self.dataset_path)  # type: ignore[no-any-return]
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
+        cls = FollowupFilesystemJob if self.config.as_staging else LoadFilesystemJob
         has_merge_keys = any(col['merge_key'] or col['primary_key'] for col in table['columns'].values())
-        return LoadFilesystemJob(
+        return cls(
             file_path,
             self.dataset_path,
             config=self.config,
             write_disposition=table['write_disposition'],
             has_merge_keys=has_merge_keys,
             schema_name=self.schema.name,
             load_id=load_id
@@ -100,14 +119,15 @@
 
     def restore_file_load(self, file_path: str) -> LoadJob:
         return EmptyLoadJob.from_file_path(file_path, "completed")
 
     def create_merge_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
         return None
 
+
     def complete_load(self, load_id: str) -> None:
         schema_name = self.schema.name
         table_name = LOADS_TABLE_NAME
         file_name = f"{schema_name}.{table_name}.{load_id}"
         self.fs_client.touch(posixpath.join(self.dataset_path, file_name))
 
     def __enter__(self) -> "FilesystemClient":
```

### Comparing `dlt-0.3.3a0/dlt/destinations/filesystem/filesystem_client.py` & `dlt-0.3.4/dlt/destinations/filesystem/filesystem_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/destinations/insert_job_client.py` & `dlt-0.3.4/dlt/destinations/insert_job_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
-from typing import Any, Iterator, List
+import abc
+from typing import Any, Iterator, List, Type
 
 from dlt.common.destination.reference import LoadJob, FollowupJob, TLoadJobState
 from dlt.common.schema.typing import TTableSchema, TWriteDisposition
 from dlt.common.storages import FileStorage
 
 from dlt.destinations.sql_client import SqlClientBase
 from dlt.destinations.job_impl import EmptyLoadJob
@@ -98,7 +99,8 @@
     def _get_in_table_constraints_sql(self, t: TTableSchema) -> str:
         # get primary key
         pass
 
     def _get_out_table_constrains_sql(self, t: TTableSchema) -> str:
         # set non unique indexes
         pass
+
```

### Comparing `dlt-0.3.3a0/dlt/destinations/job_client_impl.py` & `dlt-0.3.4/dlt/destinations/job_client_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 
 from dlt.common import json, pendulum, logger
 from dlt.common.data_types import TDataType
 from dlt.common.schema.typing import COLUMN_HINTS, LOADS_TABLE_NAME, VERSION_TABLE_NAME, TColumnSchemaBase, TTableSchema
 from dlt.common.schema.utils import add_missing_hints
 from dlt.common.storages import FileStorage
 from dlt.common.schema import TColumnSchema, Schema, TTableSchemaColumns, TSchemaTables
-from dlt.common.destination.reference import DestinationClientConfiguration, DestinationClientDwhConfiguration, NewLoadJob, TLoadJobState, LoadJob, JobClientBase
+from dlt.common.destination.reference import DestinationClientConfiguration, DestinationClientDwhConfiguration, NewLoadJob, TLoadJobState, LoadJob, JobClientBase, FollowupJob, DestinationClientStagingConfiguration, CredentialsConfiguration
 from dlt.common.utils import concat_strings_with_limit
 from dlt.destinations.exceptions import DatabaseUndefinedRelation, DestinationSchemaWillNotUpdate
-from dlt.destinations.job_impl import EmptyLoadJobWithoutFollowup
+from dlt.destinations.job_impl import EmptyLoadJobWithoutFollowup, NewReferenceJob
 from dlt.destinations.sql_merge_job import SqlMergeJob
 
 from dlt.destinations.typing import TNativeConn
 from dlt.destinations.sql_client import SqlClientBase
+from dlt.common.configuration import with_config, known_sections
 
 
 class StorageSchemaInfo(NamedTuple):
     version_hash: str
     schema_name: str
     version: int
     engine_version: str
@@ -54,14 +55,31 @@
         raise NotImplementedError()
 
     @staticmethod
     def is_sql_job(file_path: str) -> bool:
         return os.path.splitext(file_path)[1][1:] == "sql"
 
 
+class CopyRemoteFileLoadJob(LoadJob, FollowupJob):
+    def __init__(self, table: TTableSchema, file_path: str, sql_client: SqlClientBase[Any], staging_credentials: Optional[CredentialsConfiguration] = None) -> None:
+        super().__init__(FileStorage.get_file_name_from_file_path(file_path))
+        self._sql_client = sql_client
+        self._staging_credentials = staging_credentials
+
+        self.execute(table, NewReferenceJob.resolve_reference(file_path))
+
+    def execute(self, table: TTableSchema, bucket_path: str) -> None:
+        # implement in child implementations
+        raise NotImplementedError()
+
+    def state(self) -> TLoadJobState:
+        # this job is always done
+        return "completed"
+
+
 class SqlJobClientBase(JobClientBase):
 
     VERSION_TABLE_SCHEMA_COLUMNS: ClassVar[str] = "version_hash, schema_name, version, engine_version, inserted_at, schema"
 
     def __init__(self, schema: Schema, config: DestinationClientConfiguration,  sql_client: SqlClientBase[TNativeConn]) -> None:
         super().__init__(schema, config)
         self.sql_client = sql_client
@@ -182,22 +200,22 @@
                 "name": c[0],
                 "nullable": _null_to_bool(c[2]),
                 "data_type": self._from_db_type(c[1], c[3], c[4]),
             }
             schema_table[c[0]] = add_missing_hints(schema_c)
         return True, schema_table
 
-    @staticmethod
+    @classmethod
     @abstractmethod
-    def _to_db_type(schema_type: TDataType) -> str:
+    def _to_db_type(cls, schema_type: TDataType) -> str:
         pass
 
-    @staticmethod
+    @classmethod
     @abstractmethod
-    def _from_db_type(db_type: str, precision: Optional[int], scale: Optional[int]) -> TDataType:
+    def _from_db_type(cls, db_type: str, precision: Optional[int], scale: Optional[int]) -> TDataType:
         pass
 
     def get_newest_schema_from_storage(self) -> StorageSchemaInfo:
         name = self.sql_client.make_qualified_table_name(VERSION_TABLE_NAME)
         query = f"SELECT {self.VERSION_TABLE_SCHEMA_COLUMNS} FROM {name} WHERE schema_name = %s ORDER BY inserted_at DESC;"
         return self._row_to_schema_info(query, self.schema.name)
 
@@ -338,7 +356,8 @@
             schema_str = base64.b64encode(zlib.compress(schema_bytes, level=9)).decode("ascii")
         # insert
         name = self.sql_client.make_qualified_table_name(VERSION_TABLE_NAME)
         # values =  schema.version_hash, schema.name, schema.version, schema.ENGINE_VERSION, str(now_ts), schema_str
         self.sql_client.execute_sql(
             f"INSERT INTO {name}({self.VERSION_TABLE_SCHEMA_COLUMNS}) VALUES (%s, %s, %s, %s, %s, %s);", schema.stored_version_hash, schema.name, schema.version, schema.ENGINE_VERSION, now_ts, schema_str
         )
+
```

### Comparing `dlt-0.3.3a0/dlt/destinations/job_impl.py` & `dlt-0.3.4/dlt/destinations/job_impl.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import tempfile  # noqa: 251
 
 from dlt.common.storages import FileStorage
 
 from dlt.common.destination.reference import NewLoadJob, FollowupJob, TLoadJobState, LoadJob
-
+from dlt.common.storages.load_storage import ParsedLoadJobFileName
 
 class EmptyLoadJobWithoutFollowup(LoadJob):
     def __init__(self, file_name: str, status: TLoadJobState, exception: str = None) -> None:
         self._status = status
         self._exception = exception
         super().__init__(file_name)
 
@@ -32,8 +32,26 @@
         temp_file = os.path.join(tempfile.gettempdir(), self._file_name)
         with open(temp_file, "w", encoding="utf-8") as f:
             f.write(data)
         self._new_file_path = temp_file
 
     def new_file_path(self) -> str:
         """Path to a newly created temporary job file"""
-        return self._new_file_path
+        return self._new_file_path
+
+class NewReferenceJob(NewLoadJobImpl):
+
+    def __init__(self, file_name: str, status: TLoadJobState, exception: str = None, remote_path: str = None) -> None:
+        file_name = os.path.splitext(file_name)[0] + ".reference"
+        super().__init__(file_name, status, exception)
+        self._remote_path = remote_path
+        self._save_text_file(remote_path)
+
+    @staticmethod
+    def is_reference_job(file_path: str) -> bool:
+        return os.path.splitext(file_path)[1][1:] == "reference"
+
+    @staticmethod
+    def resolve_reference(file_path: str) -> str:
+        with open(file_path, "r+", encoding="utf-8") as f:
+            # Reading from a file
+            return f.read()
```

### Comparing `dlt-0.3.3a0/dlt/destinations/motherduck/__init__.py` & `dlt-0.3.4/dlt/destinations/motherduck/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from dlt.common.schema.schema import Schema
 from dlt.common.configuration import with_config, known_sections
 from dlt.common.configuration.accessors import config
 from dlt.common.data_writers.escape import escape_postgres_identifier, escape_duckdb_literal
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import JobClientBase, DestinationClientConfiguration
+from dlt.common.arithmetics import DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE
 
 from dlt.destinations.motherduck.configuration import MotherDuckClientConfiguration
 
 
 @with_config(spec=MotherDuckClientConfiguration, sections=(known_sections.DESTINATION, "motherduck",))
 def _configure(config: MotherDuckClientConfiguration = config.value) -> MotherDuckClientConfiguration:
     return config
@@ -17,14 +18,16 @@
 
 def capabilities() -> DestinationCapabilitiesContext:
     caps = DestinationCapabilitiesContext()
     caps.preferred_loader_file_format = "parquet"
     caps.supported_loader_file_formats = ["parquet", "insert_values", "sql"]
     caps.escape_identifier = escape_postgres_identifier
     caps.escape_literal = escape_duckdb_literal
+    caps.decimal_precision = (DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE)
+    caps.wei_precision = (DEFAULT_NUMERIC_PRECISION, 0)
     caps.max_identifier_length = 65536
     caps.max_column_identifier_length = 65536
     caps.naming_convention = "duck_case"
     caps.max_query_length = 512 * 1024
     caps.is_max_query_length_in_bytes = True
     caps.max_text_data_type_length = 1024 * 1024 * 1024
     caps.is_max_text_data_type_length_in_bytes = True
```

### Comparing `dlt-0.3.3a0/dlt/destinations/motherduck/configuration.py` & `dlt-0.3.4/dlt/destinations/motherduck/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/destinations/motherduck/motherduck.py` & `dlt-0.3.4/dlt/destinations/motherduck/motherduck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/destinations/motherduck/sql_client.py` & `dlt-0.3.4/dlt/destinations/motherduck/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/destinations/postgres/__init__.py` & `dlt-0.3.4/dlt/destinations/redshift/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 from typing import Type
 
 from dlt.common.schema.schema import Schema
 from dlt.common.configuration import with_config, known_sections
 from dlt.common.configuration.accessors import config
-from dlt.common.data_writers.escape import escape_postgres_identifier, escape_postgres_literal
+from dlt.common.data_writers.escape import escape_redshift_identifier, escape_redshift_literal
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import JobClientBase, DestinationClientConfiguration
+from dlt.common.arithmetics import DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE
 
-from dlt.destinations.postgres.configuration import PostgresClientConfiguration
+from dlt.destinations.redshift.configuration import RedshiftClientConfiguration
 
 
-@with_config(spec=PostgresClientConfiguration, sections=(known_sections.DESTINATION, "postgres",))
-def _configure(config: PostgresClientConfiguration = config.value) -> PostgresClientConfiguration:
+@with_config(spec=RedshiftClientConfiguration, sections=(known_sections.DESTINATION, "redshift",))
+def _configure(config: RedshiftClientConfiguration = config.value) -> RedshiftClientConfiguration:
     return config
 
 
 def capabilities() -> DestinationCapabilitiesContext:
-    # https://www.postgresql.org/docs/current/limits.html
     caps = DestinationCapabilitiesContext()
     caps.preferred_loader_file_format = "insert_values"
     caps.supported_loader_file_formats = ["insert_values", "sql"]
-    caps.escape_identifier = escape_postgres_identifier
-    caps.escape_literal = escape_postgres_literal
-    caps.max_identifier_length = 63
-    caps.max_column_identifier_length = 63
-    caps.max_query_length = 32 * 1024 * 1024
+    caps.preferred_staging_file_format = "jsonl"
+    caps.supported_staging_file_formats = ["jsonl", "parquet"]
+    caps.escape_identifier = escape_redshift_identifier
+    caps.escape_literal = escape_redshift_literal
+    caps.decimal_precision = (DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE)
+    caps.wei_precision = (DEFAULT_NUMERIC_PRECISION, 0)
+    caps.max_identifier_length = 127
+    caps.max_column_identifier_length = 127
+    caps.max_query_length = 16 * 1024 * 1024
     caps.is_max_query_length_in_bytes = True
-    caps.max_text_data_type_length = 1024 * 1024 * 1024
+    caps.max_text_data_type_length = 65535
     caps.is_max_text_data_type_length_in_bytes = True
     caps.supports_ddl_transactions = True
+    caps.alter_add_multi_column = False
 
     return caps
 
 
 def client(schema: Schema, initial_config: DestinationClientConfiguration = config.value) -> JobClientBase:
     # import client when creating instance so capabilities and config specs can be accessed without dependencies installed
-    from dlt.destinations.postgres.postgres import PostgresClient
+    from dlt.destinations.redshift.redshift import RedshiftClient
 
-    return PostgresClient(schema, _configure(initial_config))  # type: ignore
+    return RedshiftClient(schema, _configure(initial_config))  # type: ignore
 
 
 def spec() -> Type[DestinationClientConfiguration]:
-    return PostgresClientConfiguration
+    return RedshiftClientConfiguration
```

### Comparing `dlt-0.3.3a0/dlt/destinations/postgres/configuration.py` & `dlt-0.3.4/dlt/destinations/postgres/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/destinations/postgres/postgres.py` & `dlt-0.3.4/dlt/destinations/postgres/postgres.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "text": "varchar",
     "double": "double precision",
     "bool": "boolean",
     "timestamp": "timestamp with time zone",
     "date": "date",
     "bigint": "bigint",
     "binary": "bytea",
-    "decimal": f"numeric({DEFAULT_NUMERIC_PRECISION},{DEFAULT_NUMERIC_SCALE})"
+    "decimal": "numeric(%i,%i)"
 }
 
 PGT_TO_SCT: Dict[str, TDataType] = {
     "varchar": "text",
     "jsonb": "complex",
     "double precision": "double",
     "boolean": "bool",
@@ -66,19 +66,24 @@
         self.active_hints = HINT_TO_POSTGRES_ATTR if self.config.create_indexes else {}
 
     def _get_column_def_sql(self, c: TColumnSchema) -> str:
         hints_str = " ".join(self.active_hints.get(h, "") for h in self.active_hints.keys() if c.get(h, False) is True)
         column_name = self.capabilities.escape_identifier(c["name"])
         return f"{column_name} {self._to_db_type(c['data_type'])} {hints_str} {self._gen_not_null(c['nullable'])}"
 
-    @staticmethod
-    def _to_db_type(sc_t: TDataType) -> str:
+    @classmethod
+    def _to_db_type(cls, sc_t: TDataType) -> str:
+        if sc_t == "wei":
+            return SCT_TO_PGT["decimal"] % cls.capabilities.wei_precision
+        if sc_t == "decimal":
+            return SCT_TO_PGT["decimal"] % cls.capabilities.decimal_precision
+
         if sc_t == "wei":
             return f"numeric({2*EVM_DECIMAL_PRECISION},{EVM_DECIMAL_PRECISION})"
         return SCT_TO_PGT[sc_t]
 
-    @staticmethod
-    def _from_db_type(pq_t: str, precision: Optional[int], scale: Optional[int]) -> TDataType:
+    @classmethod
+    def _from_db_type(cls, pq_t: str, precision: Optional[int], scale: Optional[int]) -> TDataType:
         if pq_t == "numeric":
-            if precision == 2*EVM_DECIMAL_PRECISION and scale == EVM_DECIMAL_PRECISION:
+            if (precision, scale) == cls.capabilities.wei_precision:
                 return "wei"
         return PGT_TO_SCT.get(pq_t, "text")
```

### Comparing `dlt-0.3.3a0/dlt/destinations/postgres/sql_client.py` & `dlt-0.3.4/dlt/destinations/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/destinations/redshift/README.md` & `dlt-0.3.4/dlt/destinations/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/destinations/redshift/configuration.py` & `dlt-0.3.4/dlt/destinations/redshift/configuration.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Final
+from typing import Final, Optional
 
 from dlt.common.typing import TSecretValue
 from dlt.common.configuration import configspec
 
 from dlt.destinations.postgres.configuration import PostgresCredentials, PostgresClientConfiguration
 
 
@@ -14,7 +14,8 @@
     host: str = None
 
 
 @configspec(init=True)
 class RedshiftClientConfiguration(PostgresClientConfiguration):
     destination_name: Final[str] = "redshift"  # type: ignore
     credentials: RedshiftCredentials
+    staging_iam_role: Optional[str] = None
```

### Comparing `dlt-0.3.3a0/dlt/destinations/snowflake/__init__.py` & `dlt-0.3.4/dlt/destinations/snowflake/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,28 +3,33 @@
 
 from dlt.common.schema.schema import Schema
 from dlt.common.configuration import with_config, known_sections
 from dlt.common.configuration.accessors import config
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import JobClientBase, DestinationClientConfiguration
 from dlt.common.data_writers.escape import escape_snowflake_identifier
+from dlt.common.arithmetics import DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE
 
 from dlt.destinations.snowflake.configuration import SnowflakeClientConfiguration
 
 
 @with_config(spec=SnowflakeClientConfiguration, sections=(known_sections.DESTINATION, "snowflake",))
 def _configure(config: SnowflakeClientConfiguration = config.value) -> SnowflakeClientConfiguration:
     return config
 
 
 def capabilities() -> DestinationCapabilitiesContext:
     caps = DestinationCapabilitiesContext()
     caps.preferred_loader_file_format = "jsonl"
     caps.supported_loader_file_formats = ["jsonl", "parquet", "sql"]
+    caps.preferred_staging_file_format = "jsonl"
+    caps.supported_staging_file_formats = ["jsonl", "parquet", "sql"]
     caps.escape_identifier = escape_snowflake_identifier
+    caps.decimal_precision = (DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE)
+    caps.wei_precision = (DEFAULT_NUMERIC_PRECISION, 0)
     caps.max_identifier_length = 255
     caps.max_column_identifier_length = 255
     caps.max_query_length = 2 * 1024 * 1024
     caps.is_max_query_length_in_bytes = True
     caps.max_text_data_type_length = 16 * 1024 * 1024
     caps.is_max_text_data_type_length_in_bytes = True
     caps.supports_ddl_transactions = True
```

### Comparing `dlt-0.3.3a0/dlt/destinations/snowflake/configuration.py` & `dlt-0.3.4/dlt/destinations/snowflake/configuration.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -86,8 +86,8 @@
 class SnowflakeClientConfiguration(DestinationClientDwhConfiguration):
     destination_name: Final[str] = "snowflake"  # type: ignore[misc]
     credentials: SnowflakeCredentials
 
     stage_name: Optional[str] = None
     """Use an existing named stage instead of the default. Default uses the implicit table stage per table"""
     keep_staged_files: bool = True
-    """Whether to keep or delete the staged files after COPY INTO succeeds"""
+    """Whether to keep or delete the staged files after COPY INTO succeeds"""
```

### Comparing `dlt-0.3.3a0/dlt/destinations/snowflake/snowflake.py` & `dlt-0.3.4/dlt/destinations/snowflake/snowflake.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,116 @@
-from pathlib import Path
-from typing import ClassVar, Dict, Optional, Sequence, Tuple, List, cast, Iterable
+from typing import ClassVar, Dict, Optional, Sequence, Tuple, List
+from urllib.parse import urlparse
 
-from dlt.common import json, logger
 from dlt.common.arithmetics import DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE
-from dlt.common.configuration.specs import GcpServiceAccountCredentialsWithoutDefaults
 from dlt.common.destination import DestinationCapabilitiesContext
-from dlt.common.destination.reference import FollowupJob, NewLoadJob, TLoadJobState, LoadJob
+from dlt.common.destination.reference import FollowupJob, TLoadJobState, LoadJob, CredentialsConfiguration
+from dlt.common.configuration.specs import AwsCredentialsWithoutDefaults
 from dlt.common.data_types import TDataType
 from dlt.common.storages.file_storage import FileStorage
-from dlt.common.schema import TColumnSchema, Schema, TTableSchemaColumns, TSchemaTables
+from dlt.common.schema import TColumnSchema, Schema, TTableSchemaColumns
 from dlt.common.schema.typing import TTableSchema, TWriteDisposition
-from dlt.common.wei import EVM_DECIMAL_PRECISION
+
 
 from dlt.destinations.job_client_impl import SqlJobClientBase
 from dlt.destinations.job_impl import EmptyLoadJob
-from dlt.destinations.exceptions import DestinationSchemaWillNotUpdate, DestinationTransientException, LoadJobNotExistsException, LoadJobTerminalException, LoadJobUnknownTableException
+from dlt.destinations.exceptions import LoadJobTerminalException
 
 from dlt.destinations.snowflake import capabilities
 from dlt.destinations.snowflake.configuration import SnowflakeClientConfiguration
 from dlt.destinations.snowflake.sql_client import SnowflakeSqlClient
-from dlt.destinations.sql_merge_job import SqlMergeJob
 from dlt.destinations.snowflake.sql_client import SnowflakeSqlClient
+from dlt.destinations.job_impl import NewReferenceJob
 
 BIGINT_PRECISION = 19
 MAX_NUMERIC_PRECISION = 38
 
 
-SCT_TO_BQT: Dict[TDataType, str] = {
+SCT_TO_SNOW: Dict[TDataType, str] = {
     "complex": "VARIANT",
     "text": "VARCHAR",
     "double": "FLOAT",
     "bool": "BOOLEAN",
     "date": "DATE",
     "timestamp": "TIMESTAMP_TZ",
     "bigint": f"NUMBER({BIGINT_PRECISION},0)",  # Snowflake has no integer types
     "binary": "BINARY",
-    "decimal": f"NUMBER({DEFAULT_NUMERIC_PRECISION},{DEFAULT_NUMERIC_SCALE})",
+    "decimal": "NUMBER(%i,%i)",
 }
 
-BQT_TO_SCT: Dict[str, TDataType] = {
+SNOW_TO_SCT: Dict[str, TDataType] = {
     "VARCHAR": "text",
     "FLOAT": "double",
     "BOOLEAN": "bool",
     "DATE": "date",
     "TIMESTAMP_TZ": "timestamp",
     "BINARY": "binary",
     "VARIANT": "complex"
 }
 
+
 class SnowflakeLoadJob(LoadJob, FollowupJob):
     def __init__(
             self, file_path: str, table_name: str, write_disposition: TWriteDisposition, load_id: str, client: SnowflakeSqlClient,
-            stage_name: Optional[str] = None, keep_staged_files: bool = True
+            stage_name: Optional[str] = None, keep_staged_files: bool = True, staging_credentials: Optional[CredentialsConfiguration] = None
     ) -> None:
         file_name = FileStorage.get_file_name_from_file_path(file_path)
         super().__init__(file_name)
 
         with client.with_staging_dataset(write_disposition == "merge"):
             qualified_table_name = client.make_qualified_table_name(table_name)
 
-            if stage_name:
-                # Concat "SCHEMA_NAME".stage_name
-                stage_name = client.make_qualified_table_name(stage_name)
-                # Create the stage if it doesn't exist
-                client.execute_sql(f"CREATE STAGE IF NOT EXISTS {stage_name}")
+            # extract and prepare some vars
+            bucket_path = NewReferenceJob.resolve_reference(file_path) if NewReferenceJob.is_reference_job(file_path) else ""
+            file_name = FileStorage.get_file_name_from_file_path(bucket_path) if bucket_path else file_name
+            from_clause = ""
+            credentials_clause = ""
+            files_clause = ""
+            stage_file_path = ""
+
+            if bucket_path:
+                # s3 credentials case
+                if bucket_path.startswith("s3://") and staging_credentials and isinstance(staging_credentials, AwsCredentialsWithoutDefaults):
+                    credentials_clause = f"""CREDENTIALS=(AWS_KEY_ID='{staging_credentials.aws_access_key_id}' AWS_SECRET_KEY='{staging_credentials.aws_secret_access_key}')"""
+                    from_clause = f"FROM '{bucket_path}'"
+                else:
+                    if not stage_name:
+                        # when loading from bucket stage must be given
+                        raise LoadJobTerminalException(file_path, f"Cannot load from bucket path {bucket_path} without a stage name. See https://dlthub.com/docs/dlt-ecosystem/destinations/snowflake for instructions on setting up the `stage_name`")
+                    from_clause = f"FROM @{stage_name}/"
+                    files_clause = f"FILES = ('{urlparse(bucket_path).path.lstrip('/')}')"
             else:
-                # Use implicit table stage by default: "SCHEMA_NAME"."%TABLE_NAME"
-                stage_name = client.make_qualified_table_name('%'+table_name)
+                # this means we have a local file
+                if not stage_name:
+                    # Use implicit table stage by default: "SCHEMA_NAME"."%TABLE_NAME"
+                    stage_name = client.make_qualified_table_name('%'+table_name)
+                stage_file_path = f'@{stage_name}/"{load_id}"/{file_name}'
+                from_clause = f"FROM {stage_file_path}"
 
+            # decide on source format, stage_file_path will either be a local file or a bucket path
             source_format = "( TYPE = 'JSON', BINARY_FORMAT = 'BASE64' )"
-            if file_path.endswith("parquet"):
-                source_format = "(TYPE = 'PARQUET')"
+            if file_name.endswith("parquet"):
+                source_format = "(TYPE = 'PARQUET', BINARY_AS_TEXT = FALSE)"
 
-            stage_file_path = f'@{stage_name}/"{load_id}"/{file_name}'
             with client.begin_transaction():
-                # PUT and copy files in one transaction
-                client.execute_sql(f'PUT file://{file_path} @{stage_name}/"{load_id}" OVERWRITE = TRUE, AUTO_COMPRESS = FALSE')
                 if write_disposition == "replace":
                     client.execute_sql(f"TRUNCATE TABLE IF EXISTS {qualified_table_name}")
+                # PUT and COPY in one tx if local file, otherwise only copy
+                if not bucket_path:
+                    client.execute_sql(f'PUT file://{file_path} @{stage_name}/"{load_id}" OVERWRITE = TRUE, AUTO_COMPRESS = FALSE')
                 client.execute_sql(
                     f"""COPY INTO {qualified_table_name}
-                    FROM {stage_file_path}
+                    {from_clause}
+                    {files_clause}
+                    {credentials_clause}
                     FILE_FORMAT = {source_format}
                     MATCH_BY_COLUMN_NAME='CASE_INSENSITIVE'
                     """
                 )
-                if not keep_staged_files:
+                if stage_file_path and not keep_staged_files:
                     client.execute_sql(f'REMOVE {stage_file_path}')
 
 
     def state(self) -> TLoadJobState:
         return "completed"
 
     def exception(self) -> str:
@@ -111,15 +132,16 @@
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         job = super().start_file_load(table, file_path, load_id)
 
         if not job:
             job = SnowflakeLoadJob(
                 file_path, table['name'], table['write_disposition'], load_id, self.sql_client,
-                stage_name=self.config.stage_name, keep_staged_files=self.config.keep_staged_files
+                stage_name=self.config.stage_name, keep_staged_files=self.config.keep_staged_files,
+                staging_credentials=self.config.staging_credentials
             )
         return job
 
     def restore_file_load(self, file_path: str) -> LoadJob:
         return EmptyLoadJob.from_file_path(file_path, "completed")
 
     def _make_add_column_sql(self, new_columns: Sequence[TColumnSchema]) -> List[str]:
@@ -132,29 +154,31 @@
         cluster_list = [self.capabilities.escape_identifier(c['name']) for c in new_columns if c.get('cluster')]
 
         if cluster_list:
             sql[0] = sql[0] + "\nCLUSTER BY (" + ",".join(cluster_list) + ")"
 
         return sql
 
-    @staticmethod
-    def _to_db_type(sc_t: TDataType) -> str:
-        if sc_t == 'wei':
-            return "NUMBER(38,0)"
-        return SCT_TO_BQT[sc_t]
+    @classmethod
+    def _to_db_type(cls, sc_t: TDataType) -> str:
+        if sc_t == "wei":
+            return SCT_TO_SNOW["decimal"] % cls.capabilities.wei_precision
+        if sc_t == "decimal":
+            return SCT_TO_SNOW["decimal"] % cls.capabilities.decimal_precision
+        return SCT_TO_SNOW[sc_t]
 
-    @staticmethod
-    def _from_db_type(bq_t: str, precision: Optional[int], scale: Optional[int]) -> TDataType:
+    @classmethod
+    def _from_db_type(cls, bq_t: str, precision: Optional[int], scale: Optional[int]) -> TDataType:
         if bq_t == "NUMBER":
             if precision == BIGINT_PRECISION and scale == 0:
                 return 'bigint'
-            elif precision == MAX_NUMERIC_PRECISION and scale == 0:
+            elif (precision, scale) == cls.capabilities.wei_precision:
                 return 'wei'
             return 'decimal'
-        return BQT_TO_SCT.get(bq_t, "text")
+        return SNOW_TO_SCT.get(bq_t, "text")
 
     def _get_column_def_sql(self, c: TColumnSchema) -> str:
         name = self.capabilities.escape_identifier(c["name"])
         return f"{name} {self._to_db_type(c['data_type'])} {self._gen_not_null(c['nullable'])}"
 
     def get_storage_table(self, table_name: str) -> Tuple[bool, TTableSchemaColumns]:
         table_name = table_name.upper()  # All snowflake tables are uppercased in information schema
```

### Comparing `dlt-0.3.3a0/dlt/destinations/snowflake/sql_client.py` & `dlt-0.3.4/dlt/destinations/snowflake/sql_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,22 @@
 
     def __init__(self, dataset_name: str, credentials: SnowflakeCredentials) -> None:
         super().__init__(credentials.database, dataset_name)
         self._conn: snowflake_lib.SnowflakeConnection = None
         self.credentials = credentials
 
     def open_connection(self) -> snowflake_lib.SnowflakeConnection:
+        conn_params = self.credentials.to_connector_params()
+        # set the timezone to UTC so when loading from file formats that do not have timezones
+        # we get dlt expected UTC
+        if "timezone" not in conn_params:
+            conn_params["timezone"] = "UTC"
         self._conn = snowflake_lib.connect(
             schema=self.fully_qualified_dataset_name(),
-            **self.credentials.to_connector_params()
+            **conn_params
         )
         return self._conn
 
     @raise_open_connection_error
     def close_connection(self) -> None:
         if self._conn:
             self._conn.close()
```

### Comparing `dlt-0.3.3a0/dlt/destinations/sql_client.py` & `dlt-0.3.4/dlt/destinations/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/destinations/sql_merge_job.py` & `dlt-0.3.4/dlt/destinations/sql_merge_job.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/destinations/typing.py` & `dlt-0.3.4/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/extract/decorators.py` & `dlt-0.3.4/dlt/extract/decorators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/extract/exceptions.py` & `dlt-0.3.4/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/extract/extract.py` & `dlt-0.3.4/dlt/extract/extract.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/extract/incremental.py` & `dlt-0.3.4/dlt/extract/incremental.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime  # noqa: I251
 
 import dlt
 from dlt.common.json import json
 from dlt.common.jsonpath import compile_path, find_values, JSONPath
 from dlt.common.typing import TDataItem, TDataItems, TFun, extract_inner_type, is_optional_type
 from dlt.common.schema.typing import TColumnKey
-from dlt.common.configuration import configspec
+from dlt.common.configuration import configspec, ConfigurationValueError
 from dlt.common.configuration.specs import BaseConfiguration
 from dlt.common.pipeline import resource_state
 from dlt.common.utils import digest128
 from dlt.extract.exceptions import IncrementalUnboundError, PipeException
 from dlt.extract.pipe import Pipe
 from dlt.extract.utils import resolve_column_value
 from dlt.extract.typing import FilterItem, SupportsPipe, TTableHintTemplate
@@ -71,31 +71,37 @@
     >>> info = p.run(r, destination="duckdb")
 
     Args:
         cursor_path: The name or a JSON path to an cursor field. Uses the same names of fields as in your JSON document, before they are normalized to store in the database.
         initial_value: Optional value used for `last_value` when no state is available, e.g. on the first run of the pipeline. If not provided `last_value` will be `None` on the first run.
         last_value_func: Callable used to determine which cursor value to save in state. It is called with a list of the stored state value and all cursor vals from currently processing items. Default is `max`
         primary_key: Optional primary key used to deduplicate data. If not provided, a primary key defined by the resource will be used. Pass a tuple to define a compound key. Pass empty tuple to disable unique checks
+        end_value: Optional value used to load a limited range of records between `initial_value` and `end_value`. The resource generator is stopped when this value is reached.
+            Use in conjunction with `initial_value`, e.g. load records from given month `incremental(initial_value="2022-01-01T00:00:00Z", end_value="2022-02-01T00:00:00Z")`
     """
     cursor_path: str = None
+    # TODO: Support typevar here
     initial_value: Optional[Any] = None
+    end_value: Optional[Any] = None
 
     def __init__(
             self,
             cursor_path: str = dlt.config.value,
             initial_value: Optional[TCursorValue]=None,
             last_value_func: Optional[LastValueFunc[TCursorValue]]=max,
-            primary_key: Optional[TTableHintTemplate[TColumnKey]] = None
+            primary_key: Optional[TTableHintTemplate[TColumnKey]] = None,
+            end_value: Optional[TCursorValue] = None
     ) -> None:
         self.cursor_path = cursor_path
         if self.cursor_path:
             self.cursor_path_p: JSONPath = compile_path(cursor_path)
         self.last_value_func = last_value_func
         self.initial_value = initial_value
         """Initial value of last_value"""
+        self.end_value = end_value
         self.start_value: Any = initial_value
         """Value of last_value at the beginning of current pipeline run"""
         self.resource_name: Optional[str] = None
         self.primary_key: Optional[TTableHintTemplate[TColumnKey]] = primary_key
         self._cached_state: IncrementalColumnState = None
         """State dictionary cached on first access"""
         super().__init__(self.transform)
@@ -105,36 +111,79 @@
         """Create Incremental instance from existing state."""
         state = Incremental._get_state(resource_name, cursor_path)
         i = cls(cursor_path, state["initial_value"])
         i.resource_name = resource_name
         return i
 
     def copy(self) -> "Incremental[TCursorValue]":
-        return self.__class__(self.cursor_path, initial_value=self.initial_value, last_value_func=self.last_value_func, primary_key=self.primary_key)
+        return self.__class__(
+            self.cursor_path, initial_value=self.initial_value, last_value_func=self.last_value_func, primary_key=self.primary_key, end_value=self.end_value
+        )
+
+    def merge(self, other: "Incremental[TCursorValue]") -> "Incremental[TCursorValue]":
+        """Create a new incremental instance which merges the two instances.
+        Only properties which are not `None` from `other` override the current instance properties.
+
+        This supports use cases with partial overrides, such as:
+        >>> def my_resource(updated=incremental('updated', initial_value='1970-01-01'))
+        >>>     ...
+        >>>
+        >>> my_resource(updated=incremental(initial_value='2023-01-01', end_value='2023-02-01'))
+        """
+        kwargs = dict(self, last_value_func=self.last_value_func, primary_key=self.primary_key)
+        for key, value in dict(other, last_value_func=other.last_value_func, primary_key=other.primary_key).items():
+            if value is not None:
+                kwargs[key] = value
+        return self.__class__(**kwargs)
 
     def on_resolved(self) -> None:
         self.cursor_path_p = compile_path(self.cursor_path)
+        if self.end_value is not None and self.initial_value is None:
+            raise ConfigurationValueError(
+                "Incremental 'end_value' was specified without 'initial_value'. 'initial_value' is required when using 'end_value'."
+            )
+        # Ensure end value is "higher" than initial value
+        if self.end_value is not None and self.last_value_func([self.end_value, self.initial_value]) != self.end_value:
+            if self.last_value_func in (min, max):
+                adject = 'higher' if self.last_value_func is max else 'lower'
+                msg = f"Incremental 'initial_value' ({self.initial_value}) is {adject} than 'end_value` ({self.end_value}). 'end_value' must be {adject} than 'initial_value'"
+            else:
+                msg = (
+                    f"Incremental 'initial_value' ({self.initial_value}) is greater than 'end_value' ({self.end_value}) as determined by the custom 'last_value_func'. "
+                    f"The result of '{self.last_value_func.__name__}([end_value, initial_value])' must equal 'end_value'"
+                )
+            raise ConfigurationValueError(msg)
 
     def parse_native_representation(self, native_value: Any) -> None:
         if isinstance(native_value, Incremental):
             self.cursor_path = native_value.cursor_path
             self.initial_value = native_value.initial_value
             self.last_value_func = native_value.last_value_func
+            self.end_value = native_value.end_value
             self.cursor_path_p = self.cursor_path_p
             self.resource_name = self.resource_name
         else:  # TODO: Maybe check if callable(getattr(native_value, '__lt__', None))
             # Passing bare value `incremental=44` gets parsed as initial_value
             self.initial_value = native_value
         if not self.is_partial():
             self.resolve()
 
     def get_state(self) -> IncrementalColumnState:
         """Returns an Incremental state for a particular cursor column"""
         if not self.resource_name:
             raise IncrementalUnboundError(self.cursor_path)
+
+        if self.end_value is not None:
+            # End value uses mock state. We don't want to write it.
+            return {
+                'initial_value': self.initial_value,
+                'last_value': self.initial_value,
+                'unique_hashes': []
+            }
+
         self._cached_state = Incremental._get_state(self.resource_name, self.cursor_path)
         if len(self._cached_state) == 0:
             # set the default like this, setdefault evaluates the default no matter if it is needed or not. and our default is heavy
             self._cached_state.update(
                 {
                     "initial_value": self.initial_value,
                     "last_value": self.initial_value,
@@ -171,21 +220,28 @@
 
         row_values = find_values(self.cursor_path_p, row)
         if not row_values:
             raise IncrementalCursorPathMissing(self.resource_name, self.cursor_path, row)
 
         incremental_state = self._cached_state
         last_value = incremental_state['last_value']
+
         row_value = row_values[0]
 
         # For datetime cursor, ensure the value is a timezone aware datetime.
         # The object saved in state will always be a tz aware pendulum datetime so this ensures values are comparable
         if isinstance(row_value, datetime):
             row_value = pendulum.instance(row_value)
 
+        # Check whether end_value has been reached
+        if self.end_value is not None and (
+            row_value == self.end_value or self.last_value_func((row_value, self.end_value)) != self.end_value
+        ):
+            raise StopIteration()
+
         check_values = (row_value,) + ((last_value, ) if last_value is not None else ())
         new_value = self.last_value_func(check_values)
         if last_value == new_value:
             # we store row id for all records with the current "last_value" in state and use it to deduplicate
             if self.last_value_func((row_value, )) == last_value:
                 unique_value = self.unique_value(row)
                 # if unique value exists then use it to deduplicate
@@ -261,32 +317,38 @@
             assert p is not None
             new_incremental: Incremental[Any] = None
             bound_args = sig.bind(*args, **kwargs)
 
             if p.name in bound_args.arguments:
                 explicit_value = bound_args.arguments[p.name]
                 if isinstance(explicit_value, Incremental):
-                    # Explicit Incremental instance is untouched
-                    new_incremental = explicit_value.copy()
+                    # Explicit Incremental instance is merged with default
+                    # allowing e.g. to only update initial_value/end_value but keeping default cursor_path
+                    if isinstance(p.default, Incremental):
+                        new_incremental = p.default.merge(explicit_value)
+                    else:
+                        new_incremental = explicit_value.copy()
                 elif isinstance(p.default, Incremental):
                     # Passing only initial value explicitly updates the default instance
                     new_incremental = p.default.copy()
                     new_incremental.initial_value = explicit_value
             elif isinstance(p.default, Incremental):
                 new_incremental = p.default.copy()
 
+
             if not new_incremental or new_incremental.is_partial():
                 if is_optional_type(p.annotation):
                     bound_args.arguments[p.name] = None  # Remove partial spec
                     return func(*bound_args.args, **bound_args.kwargs)
                 raise ValueError(f"{p.name} Incremental has no default")
             # set the incremental only if not yet set or if it was passed explicitly
             # NOTE: the _incremental may be also set by applying hints to the resource see `set_template` in `DltResource`
             if p.name in bound_args.arguments or not self._incremental:
                 self._incremental = new_incremental
+            self._incremental.resolve()
             # in case of transformers the bind will be called before this wrapper is set: because transformer is called for a first time late in the pipe
             self._incremental.bind(Pipe(self.resource_name))
             bound_args.arguments[p.name] = self._incremental
             return func(*bound_args.args, **bound_args.kwargs)
 
         return _wrap  # type: ignore
```

### Comparing `dlt-0.3.3a0/dlt/extract/pipe.py` & `dlt-0.3.4/dlt/extract/pipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -577,14 +577,17 @@
                     next_meta = next_item.meta
                     next_item = next_item.data
             except TypeError as ty_ex:
                 assert callable(step)
                 raise InvalidStepFunctionArguments(pipe_item.pipe.name, get_callable_name(step), inspect.signature(step), str(ty_ex))
             except (PipelineException, ExtractorException, DltSourceException, PipeException):
                 raise
+            except StopIteration:
+                # To avoid catching StopIteration in the general Exception handler below, we just want to stop the generator
+                raise
             except Exception as ex:
                 raise ResourceExtractionError(pipe_item.pipe.name, step, str(ex), "transform") from ex
             # create next pipe item if a value was returned. A None means that item was consumed/filtered out and should not be further processed
             if next_item is not None:
                 pipe_item = ResolvablePipeItem(next_item, pipe_item.step + 1, pipe_item.pipe, next_meta)
             else:
                 pipe_item = None
```

### Comparing `dlt-0.3.3a0/dlt/extract/schema.py` & `dlt-0.3.4/dlt/extract/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/extract/source.py` & `dlt-0.3.4/dlt/extract/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/extract/typing.py` & `dlt-0.3.4/dlt/extract/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/extract/utils.py` & `dlt-0.3.4/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/helpers/airflow_helper.py` & `dlt-0.3.4/dlt/helpers/airflow_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 from tempfile import gettempdir
 from typing import Any, Callable, List, Literal, Sequence
 from tenacity import retry_if_exception, wait_exponential, stop_after_attempt, Retrying, RetryCallState
 
 from dlt.common.exceptions import MissingDependencyException
+from dlt.common.runtime.telemetry import with_telemetry
 
 try:
     from airflow.configuration import conf
     from airflow.utils.task_group import TaskGroup
-    #from airflow.decorators import task
     from airflow.operators.python import PythonOperator
     from airflow.operators.python import get_current_context
 except ImportError:
     raise MissingDependencyException("Airflow", ["airflow>=2.0.0"])
 
 
 import dlt
@@ -114,14 +114,15 @@
             data_dir = os.path.join(local_data_folder or gettempdir(), f"dlt_{uniq_id(8)}")
         os.environ["DLT_DATA_DIR"] = data_dir
 
         # delete existing config providers in container, they will get reloaded on next use
         if ConfigProvidersContext in Container():
             del Container()[ConfigProvidersContext]
 
+    @with_telemetry("helper", "airflow_add_run", False, "decompose")
     def add_run(
         self,
         pipeline: Pipeline,
         data: Any,
         *,
         decompose: Literal["none", "serialize"] = "none",
         table_name: str = None,
```

### Comparing `dlt-0.3.3a0/dlt/helpers/dbt/__init__.py` & `dlt-0.3.4/dlt/helpers/dbt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from dlt.common.destination.reference import DestinationClientDwhConfiguration
 from dlt.common.configuration.specs import CredentialsWithDefault
 from dlt.common.typing import TSecretValue
 from dlt.version import get_installed_requirement_string
 
 from dlt.helpers.dbt.runner import create_runner, DBTPackageRunner
 
-DEFAULT_DBT_VERSION = ">=1.1,<1.5"
+DEFAULT_DBT_VERSION = ">=1.1,<1.6"
 
 
 def _default_profile_name(credentials: DestinationClientDwhConfiguration) -> str:
     profile_name = credentials.destination_name
     # in case of credentials with default add default to the profile name
     if isinstance(credentials.credentials, CredentialsWithDefault):
         if credentials.credentials.has_default_credentials():
@@ -34,14 +34,17 @@
             semver.parse(dbt_version)
             dbt_version = "==" + dbt_version
     else:
         dbt_version = ""
 
     all_packages = destination_names + ["core"]
     for idx, package in enumerate(all_packages):
+        # TODO: if we have more cases like this, move to destination capabilities
+        if package == "motherduck":
+            package = "duckdb"
         package_w_ver = "dbt-" + package + dbt_version
         # verify package
         pkg_resources.Requirement.parse(package_w_ver)
         all_packages[idx] = package_w_ver
 
     dlt_requirement = get_installed_requirement_string()
 
@@ -64,19 +67,17 @@
     working_dir: str,
     package_location: str,
     package_repository_branch: str = None,
     package_repository_ssh_key: TSecretValue = TSecretValue(""),  # noqa
     auto_full_refresh_when_out_of_sync: bool = None
 ) -> DBTPackageRunner:
     default_profile_name = _default_profile_name(destination_configuration)
-    dataset_name = destination_configuration.dataset_name
     return create_runner(
         venv,
-        destination_configuration.credentials,
+        destination_configuration,
         working_dir,
-        dataset_name,
         package_location,
         package_repository_branch=package_repository_branch,
         package_repository_ssh_key=package_repository_ssh_key,
         package_profile_name=default_profile_name,
         auto_full_refresh_when_out_of_sync=auto_full_refresh_when_out_of_sync
     )
```

### Comparing `dlt-0.3.3a0/dlt/helpers/dbt/configuration.py` & `dlt-0.3.4/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.3.4/dlt/helpers/dbt/dbt_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,22 +12,29 @@
 try:
     # block disabling root logger
     import logbook.compat
     logbook.compat.redirect_logging = lambda : None
 
     # can only import DBT after redirect is disabled
     # https://stackoverflow.com/questions/48619517/call-a-click-command-from-code
-    import dbt.main
+
     import dbt.logger
     from dbt.events import functions
     from dbt.contracts import results as dbt_results
 except ImportError:
     raise MissingDependencyException("DBT Core", ["dbt-core"])
 
 try:
+    # dbt <1.5
+    from dbt.main import handle_and_check
+except ImportError:
+    # dbt >=1.5
+    from dbt.cli.main import dbtRunner
+
+try:
     from dbt.exceptions import FailFastException  # type: ignore
 except ImportError:
     from dbt.exceptions import FailFastError as FailFastException
 
 _DBT_LOGGER_INITIALIZED = False
 
 
@@ -122,16 +129,27 @@
     working_dir = os.getcwd()
     os.chdir(package_path)
     try:
         results: dbt_results.ExecutionResult = None
         success: bool = None
         # dbt uses logbook which does not run on python 10. below is a hack that allows that
         warnings.filterwarnings("ignore", category=DeprecationWarning, module="logbook")
-        with dbt.main.log_manager.applicationbound():
-            results, success = dbt.main.handle_and_check((global_args or []) + [command] + args)  # type: ignore
+        runner_args = (global_args or []) + [command] + args # type: ignore
+
+        with dbt.logger.log_manager.applicationbound():
+            try:
+                # dbt 1.5
+                runner = dbtRunner()
+                run_result = runner.invoke(runner_args)
+                success = run_result.success
+                results = run_result.result  # type: ignore
+            except NameError:
+                # dbt < 1.5
+                results, success = handle_and_check(runner_args)
+
         assert type(success) is bool
         parsed_results = parse_dbt_execution_results(results)
         if not success:
             dbt_exc = DBTProcessingError(command, parsed_results, results)
             # detect incremental model out of sync
             if is_incremental_schema_out_of_sync_error(results):
                 raise IncrementalSchemaOutOfSyncError(dbt_exc)
```

### Comparing `dlt-0.3.3a0/dlt/helpers/dbt/exceptions.py` & `dlt-0.3.4/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/helpers/dbt/profiles.yml` & `dlt-0.3.4/dlt/helpers/dbt/profiles.yml`

 * *Files 13% similar despite different names*

```diff
@@ -3,125 +3,125 @@
   send_anonymous_usage_stats: False
 
 redshift:
   target: analytics
   outputs:
     analytics:
       type: redshift
-      host: "{{ env_var('CREDENTIALS__HOST') }}"
-      user: "{{ env_var('CREDENTIALS__USERNAME') }}"
-      password: "{{ env_var('CREDENTIALS__PASSWORD') }}"
-      port: "{{ env_var('CREDENTIALS__PORT', 5439) | as_number }}"
-      dbname: "{{ env_var('CREDENTIALS__DATABASE') }}"
+      host: "{{ env_var('DLT__CREDENTIALS__HOST') }}"
+      user: "{{ env_var('DLT__CREDENTIALS__USERNAME') }}"
+      password: "{{ env_var('DLT__CREDENTIALS__PASSWORD') }}"
+      port: "{{ env_var('DLT__CREDENTIALS__PORT', 5439) | as_number }}"
+      dbname: "{{ env_var('DLT__CREDENTIALS__DATABASE') }}"
       schema: "{{ var('destination_dataset_name', var('source_dataset_name')) }}"
       threads: 4
       keepalives_idle: 0 # default 0, indicating the system default
-      connect_timeout: "{{ env_var('CREDENTIALS__CONNECT_TIMEOUT') | as_number}}"
+      connect_timeout: "{{ env_var('DLT__CREDENTIALS__CONNECT_TIMEOUT') | as_number}}"
       # search_path: public # optional, not recommended
       #sslmode: [optional, set the sslmode used to connect to the database (in case this parameter is set, will look for ca in ~/.postgresql/root.crt)]
       ra3: true # enables cross-database sources
 
 
 postgres:
   target: analytics
   outputs:
     analytics:
       type: postgres
-      host: "{{ env_var('CREDENTIALS__HOST') }}"
-      user: "{{ env_var('CREDENTIALS__USERNAME') }}"
-      password: "{{ env_var('CREDENTIALS__PASSWORD') }}"
-      port: "{{ env_var('CREDENTIALS__PORT', 5432) | as_number }}"
-      dbname: "{{ env_var('CREDENTIALS__DATABASE') }}"
+      host: "{{ env_var('DLT__CREDENTIALS__HOST') }}"
+      user: "{{ env_var('DLT__CREDENTIALS__USERNAME') }}"
+      password: "{{ env_var('DLT__CREDENTIALS__PASSWORD') }}"
+      port: "{{ env_var('DLT__CREDENTIALS__PORT', 5432) | as_number }}"
+      dbname: "{{ env_var('DLT__CREDENTIALS__DATABASE') }}"
       schema: "{{ var('destination_dataset_name', var('source_dataset_name')) }}"
       threads: 4
       keepalives_idle: 0 # default 0, indicating the system default
-      connect_timeout: "{{ env_var('CREDENTIALS__CONNECT_TIMEOUT') | as_number}}"
+      connect_timeout: "{{ env_var('DLT__CREDENTIALS__CONNECT_TIMEOUT') | as_number}}"
       # search_path: public # optional, not recommended
       #sslmode: [optional, set the sslmode used to connect to the database (in case this parameter is set, will look for ca in ~/.postgresql/root.crt)]
       ra3: true # enables cross-database sources
 
 bigquery_default:
   target: analytics
   outputs:
     analytics:
       type: bigquery
       method: oauth
-      project: "{{ env_var('CREDENTIALS__PROJECT_ID') }}"
-      location: "{{ env_var('CREDENTIALS__LOCATION') }}"
+      project: "{{ env_var('DLT__CREDENTIALS__PROJECT_ID') }}"
+      location: "{{ env_var('DLT__LOCATION') }}"
       schema: "{{ var('destination_dataset_name', var('source_dataset_name')) }}"
       threads: 4
       keepalives_idle: 0 # default 0, indicating the system default
-      job_creation_timeout_seconds: "{{ env_var('CREDENTIALS__HTTP_TIMEOUT') | as_number}}"
-      job_retry_deadline_seconds: "{{ env_var('CREDENTIALS__RETRY_DEADLINE') | as_number}}"
+      job_creation_timeout_seconds: "{{ env_var('DLT__HTTP_TIMEOUT') | as_number}}"
+      job_retry_deadline_seconds: "{{ env_var('DLT__RETRY_DEADLINE') | as_number}}"
 
 bigquery:
   target: analytics
   outputs:
     analytics:
       type: bigquery
       method: service-account-json
-      project: "{{ env_var('CREDENTIALS__PROJECT_ID') }}"
-      location: "{{ env_var('CREDENTIALS__LOCATION') }}"
+      project: "{{ env_var('DLT__CREDENTIALS__PROJECT_ID') }}"
+      location: "{{ env_var('DLT__LOCATION') }}"
       schema: "{{ var('destination_dataset_name', var('source_dataset_name')) }}"
       keyfile_json:
         type: service_account
-        project_id: "{{ env_var('CREDENTIALS__PROJECT_ID') }}"
-        private_key: "{{ env_var('CREDENTIALS__PRIVATE_KEY') }}"
-        client_email: "{{ env_var('CREDENTIALS__CLIENT_EMAIL') }}"
-        token_uri: "{{ env_var('CREDENTIALS__TOKEN_URI') }}"
+        project_id: "{{ env_var('DLT__CREDENTIALS__PROJECT_ID') }}"
+        private_key: "{{ env_var('DLT__CREDENTIALS__PRIVATE_KEY') }}"
+        client_email: "{{ env_var('DLT__CREDENTIALS__CLIENT_EMAIL') }}"
+        token_uri: "{{ env_var('DLT__CREDENTIALS__TOKEN_URI') }}"
       threads: 4
       keepalives_idle: 0 # default 0, indicating the system default
-      job_creation_timeout_seconds: "{{ env_var('CREDENTIALS__HTTP_TIMEOUT') | as_number}}"
-      job_retry_deadline_seconds: "{{ env_var('CREDENTIALS__RETRY_DEADLINE') | as_number}}"
+      job_creation_timeout_seconds: "{{ env_var('DLT__HTTP_TIMEOUT') | as_number}}"
+      job_retry_deadline_seconds: "{{ env_var('DLT__RETRY_DEADLINE') | as_number}}"
 
 duckdb:
   target: analytics
   outputs:
     analytics:
       type: duckdb
       schema: "{{ var('destination_dataset_name', var('source_dataset_name')) }}"
-      path: "{{ env_var('CREDENTIALS__DATABASE') }}"
+      path: "{{ env_var('DLT__CREDENTIALS__DATABASE') }}"
       extensions:
         - httpfs
         - parquet
       # TODO: emit the config of duck db
 
 motherduck:
   target: analytics
   outputs:
     analytics:
       type: duckdb
       schema: "{{ var('destination_dataset_name', var('source_dataset_name')) }}"
-      path: "md:{{ env_var('CREDENTIALS__DATABASE') }}?token={{env_var('CREDENTIALS__PASSWORD')}}"
+      path: "md:{{ env_var('DLT__CREDENTIALS__DATABASE') }}?token={{env_var('DLT__CREDENTIALS__PASSWORD')}}"
 
 # snowflake with password auth
 snowflake:
   target: analytics
   outputs:
     analytics:
       type: snowflake
-      account: "{{ env_var('CREDENTIALS__HOST') }}"
-      user: "{{ env_var('CREDENTIALS__USERNAME') }}"
-      password: "{{ env_var('CREDENTIALS__PASSWORD') }}"
-      database: "{{ env_var('CREDENTIALS__DATABASE') }}"
-      role: "{{ env_var('CREDENTIALS__ROLE', '') }}"
+      account: "{{ env_var('DLT__CREDENTIALS__HOST') }}"
+      user: "{{ env_var('DLT__CREDENTIALS__USERNAME') }}"
+      password: "{{ env_var('DLT__CREDENTIALS__PASSWORD') }}"
+      database: "{{ env_var('DLT__CREDENTIALS__DATABASE') }}"
+      role: "{{ env_var('DLT__CREDENTIALS__ROLE', '') }}"
       schema: "{{ var('destination_dataset_name', var('source_dataset_name')) }}"
-      warehouse: "{{ env_var('CREDENTIALS__WAREHOUSE') }}"
+      warehouse: "{{ env_var('DLT__CREDENTIALS__WAREHOUSE', '') }}"
       threads: 4
 
 
 # snowflake with private key auth
 snowflake_pkey:
   target: analytics
   outputs:
     analytics:
       type: snowflake
-      account: "{{ env_var('CREDENTIALS__HOST') }}"
-      user: "{{ env_var('CREDENTIALS__USERNAME') }}"
-      database: "{{ env_var('CREDENTIALS__DATABASE') }}"
-      password: "{{ env_var('CREDENTIALS__PASSWORD') }}"
-      role: "{{ env_var('CREDENTIALS__ROLE', '') }}"
-      schema: "{{ var('destination_dataset_name', var('source_dataset_name')) }}"
-      warehouse: "{{ env_var('CREDENTIALS__WAREHOUSE') }}"
-      private_key: "{{ env_var('CREDENTIALS__PRIVATE_KEY') }}"
-      private_key_passphrase: "{{ env_var('CREDENTIALS__PRIVATE_KEY_PASSPHRASE', '') }}"
+      account: "{{ env_var('DLT__CREDENTIALS__HOST') }}"
+      user: "{{ env_var('DLT__CREDENTIALS__USERNAME') }}"
+      database: "{{ env_var('DLT__CREDENTIALS__DATABASE') }}"
+      password: "{{ env_var('DLT__CREDENTIALS__PASSWORD') }}"
+      role: "{{ env_var('DLT__CREDENTIALS__ROLE', '') }}"
+      schema: "{{ var('destination_dataset_name', var('source_dataset_name')) }}"
+      warehouse: "{{ env_var('DLT__CREDENTIALS__WAREHOUSE', '') }}"
+      private_key: "{{ env_var('DLT__CREDENTIALS__PRIVATE_KEY') }}"
+      private_key_passphrase: "{{ env_var('DLT__CREDENTIALS__PRIVATE_KEY_PASSPHRASE', '') }}"
       threads: 4
```

### Comparing `dlt-0.3.3a0/dlt/helpers/dbt/runner.py` & `dlt-0.3.4/dlt/helpers/dbt/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,40 +2,42 @@
 from subprocess import CalledProcessError
 import giturlparse
 from typing import Sequence
 
 import dlt
 from dlt.common import logger
 from dlt.common.configuration import with_config, known_sections
-from dlt.common.configuration.specs import CredentialsConfiguration
 from dlt.common.configuration.utils import add_config_to_env
+from dlt.common.destination.reference import DestinationClientDwhConfiguration
 from dlt.common.runners import Venv
 from dlt.common.runners.stdout import iter_stdout_with_result
 from dlt.common.typing import StrAny, TSecretValue
 from dlt.common.runtime.logger import is_json_logging
 from dlt.common.storages import FileStorage
 from dlt.common.git import git_custom_key_command, ensure_remote_head, force_clone_repo
 from dlt.common.utils import with_custom_environ
 
 from dlt.helpers.dbt.configuration import DBTRunnerConfiguration
 from dlt.helpers.dbt.exceptions import IncrementalSchemaOutOfSyncError, PrerequisitesException, DBTNodeResult, DBTProcessingError
 
+from dlt.common.runtime.telemetry import with_telemetry
+
 
 class DBTPackageRunner:
     """A Python wrapper over a dbt package
 
     The created wrapper minimizes the required effort to run `dbt` packages on datasets created with `dlt`. It clones the package repo and keeps it up to data,
     shares the `dlt` destination credentials with `dbt` and allows the isolated execution with `venv` parameter.
     The wrapper creates a `dbt` profile from a passed `dlt` credentials and executes the transformations in `source_dataset_name` schema. Additional configuration is
     passed via DBTRunnerConfiguration instance
     """
 
     def __init__(self,
         venv: Venv,
-        credentials: CredentialsConfiguration,
+        credentials: DestinationClientDwhConfiguration,
         working_dir: str,
         source_dataset_name: str,
         config: DBTRunnerConfiguration
     ) -> None:
         self.venv = venv
         self.credentials = credentials
         self.working_dir = working_dir
@@ -94,17 +96,17 @@
                 logger.info(f"Package will be cloned due to {type(err).__name__}:{str(err)}")
                 logger.info(f"Will clone {self.config.package_location} head {self.config.package_repository_branch} into {self.package_path}")
                 force_clone_repo(self.config.package_location, self.repo_storage, self.cloned_package_name, self.config.package_repository_branch, with_git_command=ssh_command)
 
     @with_custom_environ
     def _run_dbt_command(self, command: str, command_args: Sequence[str] = None, package_vars: StrAny = None) -> Sequence[DBTNodeResult]:
         logger.info(f"Exec dbt command: {command} {command_args} {package_vars} on profile {self.config.package_profile_name}")
-        # write credentials to environ to pass them to dbt
+        # write credentials to environ to pass them to dbt, add DLT__ prefix
         if self.credentials:
-            add_config_to_env(self.credentials)
+            add_config_to_env(self.credentials, ("dlt", ))
         args = [
             self.config.runtime.log_level,
             is_json_logging(self.config.runtime.log_format),
             self.package_path,
             command,
             self.config.package_profiles_dir,
             self.config.package_profile_name,
@@ -252,22 +254,22 @@
             raise
         except DBTProcessingError as runerr:
             self._log_dbt_run_results(runerr.run_results)
             # pass exception to the runner
             raise
 
 
+@with_telemetry("helper", "dbt_create_runner", False, "package_profile_name")
 @with_config(spec=DBTRunnerConfiguration, sections=(known_sections.DBT_PACKAGE_RUNNER,))
 def create_runner(
     venv: Venv,
-    credentials: CredentialsConfiguration,
+    credentials: DestinationClientDwhConfiguration,
     working_dir: str,
-    dataset_name: str,
     package_location: str = dlt.config.value,
     package_repository_branch: str = None,
     package_repository_ssh_key: TSecretValue = TSecretValue(""),  # noqa
     package_profiles_dir: str = None,
     package_profile_name: str = None,
     auto_full_refresh_when_out_of_sync: bool = None,
     config: DBTRunnerConfiguration = None
     ) -> DBTPackageRunner:
-    return DBTPackageRunner(venv, credentials, working_dir, dataset_name, config)
+    return DBTPackageRunner(venv, credentials, working_dir, credentials.dataset_name, config)
```

### Comparing `dlt-0.3.3a0/dlt/helpers/pandas_helper.py` & `dlt-0.3.4/dlt/helpers/pandas_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/helpers/streamlit_helper.py` & `dlt-0.3.4/dlt/helpers/streamlit_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/load/configuration.py` & `dlt-0.3.4/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/load/exceptions.py` & `dlt-0.3.4/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/load/load.py` & `dlt-0.3.4/dlt/load/load.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,70 @@
 from functools import reduce
 import datetime  # noqa: 251
 from typing import Dict, List, Optional, Tuple
 from multiprocessing.pool import ThreadPool
+import os
 
 from dlt.common import sleep, logger
 from dlt.common.configuration import with_config, known_sections
 from dlt.common.configuration.accessors import config
 from dlt.common.pipeline import LoadInfo, SupportsPipeline
 from dlt.common.schema.utils import get_child_tables, get_top_level_table, get_write_disposition
 from dlt.common.storages.load_storage import LoadPackageInfo, ParsedLoadJobFileName, TJobState
 from dlt.common.typing import StrAny
 from dlt.common.runners import TRunMetrics, Runnable, workermethod
 from dlt.common.runtime.collector import Collector, NULL_COLLECTOR
 from dlt.common.runtime.logger import pretty_format_exception
 from dlt.common.exceptions import TerminalValueError
 from dlt.common.schema import Schema
-from dlt.common.schema.typing import TTableSchema, TWriteDisposition
+from dlt.common.schema.typing import VERSION_TABLE_NAME, TTableSchema, TWriteDisposition
 from dlt.common.storages import LoadStorage
-from dlt.common.destination.reference import DestinationClientDwhConfiguration, FollowupJob, JobClientBase, DestinationReference, LoadJob, NewLoadJob, TLoadJobState, DestinationClientConfiguration
+from dlt.common.destination.reference import DestinationClientDwhConfiguration, FollowupJob, JobClientBase, DestinationReference, LoadJob, NewLoadJob, TLoadJobState, DestinationClientConfiguration, DestinationClientStagingConfiguration
+from dlt.destinations.filesystem.filesystem import LoadFilesystemJob
 
 from dlt.destinations.job_impl import EmptyLoadJob
 from dlt.destinations.exceptions import DestinationTerminalException, DestinationTransientException, LoadJobUnknownTableException
 
 from dlt.load.configuration import LoaderConfiguration
 from dlt.load.exceptions import LoadClientJobFailed, LoadClientJobRetry, LoadClientUnsupportedWriteDisposition, LoadClientUnsupportedFileFormats
 
 
 class Load(Runnable[ThreadPool]):
 
     @with_config(spec=LoaderConfiguration, sections=(known_sections.LOAD,))
     def __init__(
         self,
         destination: DestinationReference,
+        staging: DestinationReference = None,
         collector: Collector = NULL_COLLECTOR,
         is_storage_owner: bool = False,
         config: LoaderConfiguration = config.value,
-        initial_client_config: DestinationClientConfiguration = config.value
+        initial_client_config: DestinationClientConfiguration = config.value,
+        initial_staging_client_config: DestinationClientConfiguration = config.value
     ) -> None:
         self.config = config
         self.collector = collector
         self.initial_client_config = initial_client_config
+        self.initial_staging_client_config = initial_staging_client_config
         self.destination = destination
         self.capabilities = destination.capabilities()
+        self.staging = staging
         self.pool: ThreadPool = None
         self.load_storage: LoadStorage = self.create_storage(is_storage_owner)
         self._processed_load_ids: Dict[str, int] = {}
 
 
     def create_storage(self, is_storage_owner: bool) -> LoadStorage:
+        supported_file_formats = self.capabilities.supported_loader_file_formats
+        if self.staging:
+            supported_file_formats = self.staging.capabilities().supported_loader_file_formats + ["reference", "sql"]
         load_storage = LoadStorage(
             is_storage_owner,
             self.capabilities.preferred_loader_file_format,
-            self.capabilities.supported_loader_file_formats,
+            supported_file_formats,
             config=self.config._load_storage_config
         )
         return load_storage
 
     @staticmethod
     def get_load_table(schema: Schema, file_name: str) -> TTableSchema:
         table_name = LoadStorage.parse_job_file_name(file_name).table_name
@@ -69,17 +78,19 @@
             raise LoadJobUnknownTableException(table_name, file_name)
 
     @staticmethod
     @workermethod
     def w_spool_job(self: "Load", file_path: str, load_id: str, schema: Schema) -> Optional[LoadJob]:
         job: LoadJob = None
         try:
-            with self.destination.client(schema, self.initial_client_config) as client:
+            # if we have a staging destination and the file is not a reference, send to staging
+            client = self.get_staging_client(schema) if self.is_staging_job(file_path) else self.get_destination_client(schema)
+            with client as client:
                 job_info = self.load_storage.parse_job_file_name(file_path)
-                if job_info.file_format not in self.capabilities.supported_loader_file_formats:
+                if job_info.file_format not in self.load_storage.supported_file_formats:
                     raise LoadClientUnsupportedFileFormats(job_info.file_format, self.capabilities.supported_loader_file_formats, file_path)
                 logger.info(f"Will load file {file_path} with table name {job_info.table_name}")
                 table = self.get_load_table(schema, file_path)
                 if table["write_disposition"] not in ["append", "replace", "merge"]:
                     raise LoadClientUnsupportedWriteDisposition(job_info.table_name, table["write_disposition"], file_path)
                 job = client.start_file_load(table, self.load_storage.storage.make_full_path(file_path), load_id)
         except (DestinationTerminalException, TerminalValueError):
@@ -108,26 +119,31 @@
         param_chunk = [(id(self), file, load_id, schema) for file in load_files]
         # exceptions should not be raised, None as job is a temporary failure
         # other jobs should not be affected
         jobs: List[LoadJob] = self.pool.starmap(Load.w_spool_job, param_chunk)
         # remove None jobs and check the rest
         return file_count, [job for job in jobs if job is not None]
 
-    def retrieve_jobs(self, client: JobClientBase, load_id: str) -> Tuple[int, List[LoadJob]]:
+    def is_staging_job(self, file_path: str) -> bool:
+        return self.staging is not None and os.path.splitext(file_path)[1][1:] in self.staging.capabilities().supported_loader_file_formats
+
+    def retrieve_jobs(self, client: JobClientBase, load_id: str, staging_client: JobClientBase = None) -> Tuple[int, List[LoadJob]]:
         jobs: List[LoadJob] = []
 
         # list all files that were started but not yet completed
         started_jobs = self.load_storage.list_started_jobs(load_id)
+
         logger.info(f"Found {len(started_jobs)} that are already started and should be continued")
         if len(started_jobs) == 0:
             return 0, jobs
 
         for file_path in started_jobs:
             try:
                 logger.info(f"Will retrieve {file_path}")
+                client = staging_client if self.is_staging_job(file_path) else client
                 job = client.restore_file_load(file_path)
             except DestinationTerminalException:
                 logger.exception(f"Job retrieval for {file_path} failed, job will be terminated")
                 job = EmptyLoadJob.from_file_path(file_path, "failed", pretty_format_exception())
                 # proceed to appending job, do not reraise
             except (DestinationTransientException, Exception):
                 # raise on all temporary exceptions, typically network / server problems
@@ -140,42 +156,46 @@
         jobs_info: List[ParsedLoadJobFileName] = []
         new_job_files = self.load_storage.list_new_jobs(load_id)
         for job_file in new_job_files:
             if not disposition or self.get_load_table(schema, job_file)["write_disposition"] == disposition:
                 jobs_info.append(LoadStorage.parse_job_file_name(job_file))
         return jobs_info
 
-    def create_merge_job(self, load_id: str, schema: Schema, top_merged_table: TTableSchema, starting_job: LoadJob) -> NewLoadJob:
+    def get_completed_table_chain(self, load_id: str, schema: Schema, top_merged_table: TTableSchema, starting_job_id: str) -> List[TTableSchema]:
+        """Gets a table chain starting from the `top_merged_table` containing only tables with completed/failed jobs. None is returned if there's any job that is not completed"""
         # returns ordered list of tables from parent to child leaf tables
         table_chain: List[TTableSchema] = []
         # make sure all the jobs for the table chain is completed
         for table in get_child_tables(schema.tables, top_merged_table["name"]):
             table_jobs = self.load_storage.list_jobs_for_table(load_id, table["name"])
             # if no jobs for table then skip the table in the chain. we assume that if parent has no jobs, the child would also have no jobs
             # so it will be eliminated by this loop as well
             if not table_jobs:
                 continue
             # all jobs must be completed in order for merge to be created
-            if any(job.state not in ("failed_jobs", "completed_jobs") and job.job_file_info.job_id() != starting_job.job_file_info().job_id() for job in table_jobs):
+            if any(job.state not in ("failed_jobs", "completed_jobs") and job.job_file_info.job_id() != starting_job_id for job in table_jobs):
                 return None
             table_chain.append(table)
         # there must be at least 1 job
         assert len(table_chain) > 0
-        # all tables completed, create merge sql job
-        return self.destination.client(schema, self.initial_client_config).create_merge_job(table_chain)
+        return table_chain
 
     def create_followup_jobs(self, load_id: str, state: TLoadJobState, starting_job: LoadJob, schema: Schema) -> List[NewLoadJob]:
         jobs: List[NewLoadJob] = []
         if isinstance(starting_job, FollowupJob):
-            if state == "completed":
-                top_merged_table = get_top_level_table(schema.tables, self.get_load_table(schema, starting_job.file_name())["name"])
-                if top_merged_table["write_disposition"] == "merge":
-                    job = self.create_merge_job(load_id, schema, top_merged_table, starting_job)
-                    if job:
-                        jobs.append(job)
+            # check for merge jobs only for non-staging jobs. we may move that logic to the interface
+            starting_job_file_name = starting_job.file_name()
+            if state == "completed" and not self.is_staging_job(starting_job_file_name):
+                top_job_table = get_top_level_table(schema.tables, self.get_load_table(schema, starting_job_file_name)["name"])
+                if top_job_table["write_disposition"] == "merge":
+                    # if all tables completed, create merge sql job on destination client
+                    if table_chain := self.get_completed_table_chain(load_id, schema, top_job_table, starting_job.job_file_info().job_id()):
+                        if job := self.destination.client(schema, self.initial_client_config).create_merge_job(table_chain):
+                            jobs.append(job)
+            jobs = jobs + starting_job.create_followup_jobs(state)
         return jobs
 
     def complete_jobs(self, load_id: str, jobs: List[LoadJob], schema: Schema) -> List[LoadJob]:
         remaining_jobs: List[LoadJob] = []
         logger.info(f"Will complete {len(jobs)} for {load_id}")
         for ii in range(len(jobs)):
             job = jobs[ii]
@@ -216,51 +236,58 @@
             if state in ["failed", "completed"]:
                 self.collector.update("Jobs")
                 if state == "failed":
                     self.collector.update("Jobs", 1, message="WARNING: Some of the jobs failed!", label="Failed")
 
         return remaining_jobs
 
+    def get_destination_client(self, schema: Schema) -> JobClientBase:
+        return self.destination.client(schema, self.initial_client_config)
+
     def complete_package(self, load_id: str, schema: Schema, aborted: bool = False) -> None:
         # do not commit load id for aborted packages
         if not aborted:
-            with self.destination.client(schema, self.initial_client_config) as job_client:
+            with self.get_destination_client(schema) as job_client:
                 job_client.complete_load(load_id)
         self.load_storage.complete_load_package(load_id, aborted)
         logger.info(f"All jobs completed, archiving package {load_id} with aborted set to {aborted}")
         self._processed_load_ids[load_id] = 1
 
     def load_single_package(self, load_id: str, schema: Schema) -> None:
         # initialize analytical storage ie. create dataset required by passed schema
         job_client: JobClientBase
-        with self.destination.client(schema, self.initial_client_config) as job_client:
+        with self.get_destination_client(schema) as job_client:
             expected_update = self.load_storage.begin_schema_update(load_id)
             if expected_update is not None:
                 # update the default dataset
                 logger.info(f"Client for {job_client.config.destination_name} will start initialize storage")
                 job_client.initialize_storage()
                 logger.info(f"Client for {job_client.config.destination_name} will update schema to package schema")
                 all_jobs = self.get_new_jobs_info(load_id, schema)
-                all_tables = [job.table_name for job in all_jobs]
-                dlt_tables = [t["name"] for t in schema.dlt_tables()]
+                all_tables = set(job.table_name for job in all_jobs)
+                dlt_tables = set(t["name"] for t in schema.dlt_tables())
                 # only update tables that are present in the load package
-                applied_update = job_client.update_storage_schema(only_tables=set(all_tables+dlt_tables), expected_update=expected_update)
+                applied_update = job_client.update_storage_schema(only_tables=all_tables | dlt_tables, expected_update=expected_update)
                 # update the staging dataset
                 merge_jobs = self.get_new_jobs_info(load_id, schema, "merge")
                 if merge_jobs:
                     logger.info(f"Client for {job_client.config.destination_name} will start initialize STAGING storage")
                     job_client.initialize_storage(staging=True)
                     logger.info(f"Client for {job_client.config.destination_name} will UPDATE STAGING SCHEMA to package schema")
-                    merge_tables = [job.table_name for job in merge_jobs]
-                    job_client.update_storage_schema(staging=True, only_tables=set(merge_tables+dlt_tables), expected_update=expected_update)
+                    merge_tables = set(job.table_name for job in merge_jobs)
+                    job_client.update_storage_schema(staging=True, only_tables=merge_tables | {VERSION_TABLE_NAME}, expected_update=expected_update)
                     logger.info(f"Client for {job_client.config.destination_name} will TRUNCATE STAGING TABLES: {merge_tables}")
                     job_client.initialize_storage(staging=True, truncate_tables=merge_tables)
                 self.load_storage.commit_schema_update(load_id, applied_update)
             # spool or retrieve unfinished jobs
-            jobs_count, jobs = self.retrieve_jobs(job_client, load_id)
+            if self.staging:
+                with self.get_staging_client(schema) as staging_client:
+                    jobs_count, jobs = self.retrieve_jobs(job_client, load_id, staging_client)
+            else:
+                jobs_count, jobs = self.retrieve_jobs(job_client, load_id)
 
         if not jobs:
             # jobs count is a total number of jobs including those that could not be initialized
             jobs_count, jobs = self.spool_new_jobs(load_id, schema)
         # if there are no existing or new jobs we complete the package
         if jobs_count == 0:
             self.complete_package(load_id, schema, False)
@@ -297,14 +324,17 @@
                 # this will raise on signal
                 sleep(1)
             except LoadClientJobFailed:
                 # the package is completed and skipped
                 self.complete_package(load_id, schema, True)
                 raise
 
+    def get_staging_client(self, schema: Schema) -> JobClientBase:
+        return self.staging.client(schema, self.initial_staging_client_config)
+
     def run(self, pool: ThreadPool) -> TRunMetrics:
         # store pool
         self.pool = pool
 
         logger.info("Running file loading")
         # get list of loads and order by name ASC to execute schema updates
         loads = self.load_storage.list_packages()
@@ -319,14 +349,15 @@
         logger.info(f"Loaded schema name {schema.name} and version {schema.stored_version}")
 
         # get top load id and mark as being processed
         # TODO: another place where tracing must be refactored
         self._processed_load_ids[load_id] = None
         with self.collector(f"Load {schema.name} in {load_id}"):
             self.load_single_package(load_id, schema)
+
         return TRunMetrics(False, len(self.load_storage.list_packages()))
 
     def get_load_info(self, pipeline: SupportsPipeline, started_at: datetime.datetime = None) -> LoadInfo:
         # TODO: Load must provide a clear interface to get last loads and metrics
         # TODO: LoadInfo should hold many datasets
         load_ids = list(self._processed_load_ids.keys())
         load_packages: List[LoadPackageInfo] = []
@@ -336,13 +367,15 @@
         if isinstance(self.initial_client_config, DestinationClientDwhConfiguration):
             dataset_name = self.initial_client_config.dataset_name
 
         return LoadInfo(
             pipeline,
             self.initial_client_config.destination_name,
             str(self.initial_client_config),
+            self.initial_staging_client_config.destination_name if self.initial_staging_client_config else None,
+            str(self.initial_staging_client_config) if self.initial_staging_client_config else None,
             dataset_name,
             list(load_ids),
             load_packages,
             started_at,
             pipeline.first_run
         )
```

### Comparing `dlt-0.3.3a0/dlt/normalize/configuration.py` & `dlt-0.3.4/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/normalize/normalize.py` & `dlt-0.3.4/dlt/normalize/normalize.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/pipeline/__init__.py` & `dlt-0.3.4/dlt/pipeline/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,21 @@
 
 @overload
 def pipeline(
     pipeline_name: str = None,
     pipelines_dir: str = None,
     pipeline_salt: TSecretValue = None,
     destination: TDestinationReferenceArg = None,
+    staging: TDestinationReferenceArg = None,
     dataset_name: str = None,
     import_schema_path: str = None,
     export_schema_path: str = None,
     full_refresh: bool = False,
     credentials: Any = None,
-    progress: TCollectorArg = _NULL_COLLECTOR
+    progress: TCollectorArg = _NULL_COLLECTOR,
 ) -> Pipeline:
     """Creates a new instance of `dlt` pipeline, which moves the data from the source ie. a REST API to a destination ie. database or a data lake.
 
     ### Summary
     The `pipeline` functions allows you to pass the destination name to which the data should be loaded, the name of the dataset and several other options that govern loading of the data.
     The created `Pipeline` object lets you load the data from any source with `run` method or to have more granular control over the loading process with `extract`, `normalize` and `load` methods.
 
@@ -48,14 +49,17 @@
 
         pipeline_salt (TSecretValue, optional): A random value used for deterministic hashing during data anonymization. Defaults to a value derived from the pipeline name.
         Default value should not be used for any cryptographic purposes.
 
         destination (str | DestinationReference, optional): A name of the destination to which dlt will load the data, or a destination module imported from `dlt.destination`.
         May also be provided to `run` method of the `pipeline`.
 
+        staging (str | DestinationReference, optional): A name of the destination where dlt will stage the data before final loading, or a destination module imported from `dlt.destination`.
+        May also be provided to `run` method of the `pipeline`.
+
         dataset_name (str, optional): A name of the dataset to which the data will be loaded. A dataset is a logical group of tables ie. `schema` in relational databases or folder grouping many files.
         May also be provided later to the `run` or `load` methods of the `Pipeline`. If not provided at all then defaults to the `pipeline_name`
 
         import_schema_path (str, optional): A path from which the schema `yaml` file will be imported on each pipeline run. Defaults to None which disables importing.
 
         export_schema_path (str, optional): A path where the schema `yaml` file will be exported after every schema change. Defaults to None which disables exporting.
 
@@ -82,14 +86,15 @@
 
 @with_config(spec=PipelineConfiguration, auto_pipeline_section=True)
 def pipeline(
     pipeline_name: str = None,
     pipelines_dir: str = None,
     pipeline_salt: TSecretValue = None,
     destination: TDestinationReferenceArg = None,
+    staging: TDestinationReferenceArg = None,
     dataset_name: str = None,
     import_schema_path: str = None,
     export_schema_path: str = None,
     full_refresh: bool = False,
     credentials: Any = None,
     progress: TCollectorArg = _NULL_COLLECTOR,
     **kwargs: Any
@@ -109,21 +114,24 @@
             pass
 
     # if working_dir not provided use temp folder
     if not pipelines_dir:
         pipelines_dir = get_dlt_pipelines_dir()
 
     destination = DestinationReference.from_name(destination or kwargs["destination_name"])
+    staging = DestinationReference.from_name(staging or kwargs.get("staging_name", None)) if staging is not None else None
+
     progress = collector_from_name(progress)
     # create new pipeline instance
     p = Pipeline(
         pipeline_name,
         pipelines_dir,
         pipeline_salt,
         destination,
+        staging,
         dataset_name,
         credentials,
         import_schema_path,
         export_schema_path,
         full_refresh,
         progress,
         False,
@@ -145,15 +153,15 @@
 ) -> Pipeline:
     ensure_correct_pipeline_kwargs(attach, **kwargs)
     # if working_dir not provided use temp folder
     if not pipelines_dir:
         pipelines_dir = get_dlt_pipelines_dir()
     progress = collector_from_name(progress)
     # create new pipeline instance
-    p = Pipeline(pipeline_name, pipelines_dir, pipeline_salt, None, None, None, None, None, full_refresh, progress, True, last_config(**kwargs), kwargs["runtime"])
+    p = Pipeline(pipeline_name, pipelines_dir, pipeline_salt, None, None, None, None, None, None, full_refresh, progress, True, last_config(**kwargs), kwargs["runtime"])
     # set it as current pipeline
     p.activate()
     return p
 
 
 def run(
     data: Any,
```

### Comparing `dlt-0.3.3a0/dlt/pipeline/configuration.py` & `dlt-0.3.4/dlt/pipeline/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import RunConfiguration, BaseConfiguration
 from dlt.common.typing import AnyFun, TSecretValue
 from dlt.common.utils import digest256
 from dlt.common.data_writers import TLoaderFileFormat
 
 
-
 @configspec
 class PipelineConfiguration(BaseConfiguration):
     pipeline_name: Optional[str] = None
     pipelines_dir: Optional[str] = None
     destination_name: Optional[str] = None
+    staging_name: Optional[str] = None
     loader_file_format: Optional[TLoaderFileFormat] = None
     dataset_name: Optional[str] = None
     pipeline_salt: Optional[TSecretValue] = None
     restore_from_destination: bool = True
     """Enables the `run` method of the `Pipeline` object to restore the pipeline state and schemas from the destination"""
     enable_runtime_trace: bool = True
     """Enables the tracing. Tracing saves the execution trace locally and is required by `dlt deploy`."""
```

### Comparing `dlt-0.3.3a0/dlt/pipeline/dbt.py` & `dlt-0.3.4/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/pipeline/exceptions.py` & `dlt-0.3.4/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/pipeline/helpers.py` & `dlt-0.3.4/dlt/pipeline/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import contextlib
-from typing import Callable, Sequence, Iterable, Optional, Any, List, Iterator, Dict, Union, TypedDict
+from typing import Callable, Sequence, Iterable, Optional, Any, List, Dict, Tuple, Union, TypedDict
 from itertools import chain
 
 from dlt.common.jsonpath import resolve_paths, TAnyJsonPath, compile_paths
-
 from dlt.common.exceptions import TerminalException
-from dlt.common.schema.utils import get_child_tables, group_tables_by_resource, compile_simple_regexes, compile_simple_regex
+from dlt.common.schema.utils import group_tables_by_resource, compile_simple_regexes, compile_simple_regex
 from dlt.common.schema.typing import TSimpleRegex
 from dlt.common.typing import REPattern
-from dlt.destinations.exceptions import DatabaseUndefinedRelation
+from dlt.common.pipeline import TSourceState, _reset_resource_state, _sources_state, _delete_source_state_keys, _get_matching_resources
 
+from dlt.destinations.exceptions import DatabaseUndefinedRelation
 from dlt.pipeline.exceptions import PipelineStepFailed, PipelineHasPendingDataException
 from dlt.pipeline.typing import TPipelineStep
 from dlt.pipeline import Pipeline
-from dlt.common.pipeline import TSourceState, _reset_resource_state, _sources_state, _delete_source_state_keys, _get_matching_resources
 
 
 def retry_load(retry_on_pipeline_steps: Sequence[TPipelineStep] = ("load",)) -> Callable[[BaseException], bool]:
     """A retry strategy for Tenacity that, with default setting, will repeat `load` step for all exceptions that are not terminal
 
     Use this condition with tenacity `retry_if_exception`. Terminal exceptions are exceptions that will not go away when operations is repeated.
     Examples: missing configuration values, Authentication Errors, terminally failed jobs exceptions etc.
```

### Comparing `dlt-0.3.3a0/dlt/pipeline/pipeline.py` & `dlt-0.3.4/dlt/pipeline/pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 from dlt import version
 from dlt.common import json, logger, pendulum
 from dlt.common.configuration import inject_section, known_sections
 from dlt.common.configuration.specs import RunConfiguration, CredentialsConfiguration
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.exceptions import ConfigFieldMissingException, ContextDefaultCannotBeCreated
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
-from dlt.common.exceptions import MissingDependencyException
+from dlt.common.exceptions import DestinationLoadingViaStagingNotSupported, DestinationNoStagingMode, MissingDependencyException, DestinationIncompatibleLoaderFileFormatException
 from dlt.common.normalizers import default_normalizers, import_normalizers
 from dlt.common.runtime import signals, initialize_runtime
 from dlt.common.schema.exceptions import InvalidDatasetName
 from dlt.common.schema.typing import TColumnKey, TColumnSchema, TSchemaTables, TWriteDisposition
 from dlt.common.storages.load_storage import LoadJobInfo, LoadPackageInfo
 from dlt.common.typing import TFun, TSecretValue
 from dlt.common.runners import pool_runner as runner
 from dlt.common.storages import LiveSchemaStorage, NormalizeStorage, LoadStorage, SchemaStorage, FileStorage, NormalizeStorageConfiguration, SchemaStorageConfiguration, LoadStorageConfiguration
 from dlt.common.destination import DestinationCapabilitiesContext
-from dlt.common.destination.reference import DestinationReference, JobClientBase, DestinationClientConfiguration, DestinationClientDwhConfiguration, TDestinationReferenceArg
+from dlt.common.destination.reference import DestinationReference, JobClientBase, DestinationClientConfiguration, DestinationClientDwhConfiguration, TDestinationReferenceArg, DestinationClientStagingConfiguration, DestinationClientDwhConfiguration
+from dlt.common.destination.capabilities import INTERNAL_LOADER_FILE_FORMATS
 from dlt.common.pipeline import ExtractInfo, LoadInfo, NormalizeInfo, PipelineContext, SupportsPipeline, TPipelineLocalState, TPipelineState, StateInjectableContext
 from dlt.common.schema import Schema
 from dlt.common.utils import is_interactive
 from dlt.common.data_writers import TLoaderFileFormat
 
 from dlt.destinations.exceptions import DatabaseUndefinedRelation
 
@@ -40,15 +41,15 @@
 from dlt.destinations.job_client_impl import SqlJobClientBase
 from dlt.load.configuration import LoaderConfiguration
 from dlt.load import Load
 
 from dlt.pipeline.configuration import PipelineConfiguration
 from dlt.pipeline.progress import _Collector, _NULL_COLLECTOR
 from dlt.pipeline.exceptions import CannotRestorePipelineException, InvalidPipelineName, PipelineConfigMissing, PipelineNotActive, PipelineStepFailed, SqlClientNotAvailable
-from dlt.pipeline.trace import PipelineTrace, PipelineStepTrace, load_trace, merge_traces, start_trace, start_trace_step, end_trace_step, end_trace
+from dlt.pipeline.trace import PipelineTrace, PipelineStepTrace, load_trace, merge_traces, start_trace, start_trace_step, end_trace_step, end_trace, describe_extract_data
 from dlt.pipeline.typing import TPipelineStep
 from dlt.pipeline.state_sync import STATE_ENGINE_VERSION, load_state_from_destination, merge_state_if_changed, migrate_state, state_resource, json_encode_state, json_decode_state
 
 
 def with_state_sync(may_extract_state: bool = False) -> Callable[[TFun], TFun]:
 
     def decorator(f: TFun) -> TFun:
@@ -174,31 +175,33 @@
 
     def __init__(
             self,
             pipeline_name: str,
             pipelines_dir: str,
             pipeline_salt: TSecretValue,
             destination: DestinationReference,
+            staging: DestinationReference,
             dataset_name: str,
             credentials: Any,
             import_schema_path: str,
             export_schema_path: str,
             full_refresh: bool,
             progress: _Collector,
             must_attach_to_local_pipeline: bool,
             config: PipelineConfiguration,
-            runtime: RunConfiguration
+            runtime: RunConfiguration,
         ) -> None:
         """Initializes the Pipeline class which implements `dlt` pipeline. Please use `pipeline` function in `dlt` module to create a new Pipeline instance."""
-
         self.pipeline_salt = pipeline_salt
         self.config = config
         self.runtime_config = runtime
         self.full_refresh = full_refresh
         self.collector = progress or _NULL_COLLECTOR
+        self.destination = None
+        self.staging = None
 
         self._container = Container()
         self._pipeline_instance_id = self._create_pipeline_instance_id()
         self._pipeline_storage: FileStorage = None
         self._schema_storage: LiveSchemaStorage = None
         self._schema_storage_config: SchemaStorageConfiguration = None
         self._normalize_storage_config: NormalizeStorageConfiguration = None
@@ -210,30 +213,35 @@
         initialize_runtime(self.runtime_config)
         # initialize pipeline working dir
         self._init_working_dir(pipeline_name, pipelines_dir)
 
         with self.managed_state() as state:
             # set the pipeline properties from state
             self._state_to_props(state)
+
             # we overwrite the state with the values from init
+            if staging:
+                self._set_staging(staging)
             self._set_destination(destination)  # changing the destination could be dangerous if pipeline has not loaded items
+
             self._set_dataset_name(dataset_name)
             self.credentials = credentials
             self._configure(import_schema_path, export_schema_path, must_attach_to_local_pipeline)
 
     def drop(self) -> "Pipeline":
         """Deletes local pipeline state, schemas and any working files"""
         # reset the pipeline working dir
         self._create_pipeline()
         # clone the pipeline
         return Pipeline(
             self.pipeline_name,
             self.pipelines_dir,
             self.pipeline_salt,
             self.destination,
+            self.staging,
             self.dataset_name,
             self.credentials,
             self._schema_storage.config.import_schema_path,
             self._schema_storage.config.export_schema_path,
             self.full_refresh,
             self.collector,
             False,
@@ -272,26 +280,28 @@
                     extract_ids.append(
                         self._extract_source(storage, source, max_parallel_items, workers)
                     )
                 # commit extract ids
                 # TODO: if we fail here we should probably wipe out the whole extract folder
                 for extract_id in extract_ids:
                     storage.commit_extract_files(extract_id)
-                return ExtractInfo()
+                return ExtractInfo(describe_extract_data(data))
         except Exception as exc:
             # TODO: provide metrics from extractor
-            raise PipelineStepFailed(self, "extract", exc, ExtractInfo()) from exc
+            raise PipelineStepFailed(self, "extract", exc, ExtractInfo(describe_extract_data(data))) from exc
 
     @with_runtime_trace
     @with_schemas_sync
     @with_config_section((known_sections.NORMALIZE,))
     def normalize(self, workers: int = 1, loader_file_format: TLoaderFileFormat = None) -> NormalizeInfo:
         """Normalizes the data prepared with `extract` method, infers the schema and creates load packages for the `load` method. Requires `destination` to be known."""
         if is_interactive() and workers > 1:
             raise NotImplementedError("Do not use normalize workers in interactive mode ie. in notebook")
+        if loader_file_format and loader_file_format in INTERNAL_LOADER_FILE_FORMATS:
+            raise ValueError(f"{loader_file_format} is one of internal dlt file formats.")
         # check if any schema is present, if not then no data was extracted
         if not self.default_schema_name:
             return None
 
         # make sure destination capabilities are available
         self._get_destination_capabilities()
         # create default normalize config
@@ -334,22 +344,28 @@
 
         # check if any schema is present, if not then no data was extracted
         if not self.default_schema_name:
             return None
 
         # make sure that destination is set and client is importable and can be instantiated
         client = self._get_destination_client(self.default_schema)
+        staging_client = None
+        if self.staging:
+            staging_client = self._get_staging_client(self.default_schema)
+            # inject staging config into destination config, TODO: Not super clean I think?
+            if isinstance(client.config, DestinationClientDwhConfiguration) and not client.config.staging_credentials:
+                client.config.staging_credentials = staging_client.config.credentials
 
         # create default loader config and the loader
         load_config = LoaderConfiguration(
             workers=workers,
             raise_on_failed_jobs=raise_on_failed_jobs,
             _load_storage_config=self._load_storage_config
         )
-        load = Load(self.destination, collector=self.collector, is_storage_owner=False, config=load_config, initial_client_config=client.config)
+        load = Load(self.destination, staging=self.staging, collector=self.collector, is_storage_owner=False, config=load_config, initial_client_config=client.config, initial_staging_client_config=staging_client.config if staging_client else None)
         try:
             with signals.delayed_signals():
                 runner.run_pool(load.config, load)
             info = self._get_load_info(load)
             self.first_run = False
             return info
         except Exception as l_ex:
@@ -358,14 +374,15 @@
     @with_runtime_trace
     @with_config_section(("run",))
     def run(
         self,
         data: Any = None,
         *,
         destination: TDestinationReferenceArg = None,
+        staging: TDestinationReferenceArg = None,
         dataset_name: str = None,
         credentials: Any = None,
         table_name: str = None,
         write_disposition: TWriteDisposition = None,
         columns: Sequence[TColumnSchema] = None,
         primary_key: TColumnKey = None,
         schema: Schema = None,
@@ -413,23 +430,24 @@
 
             columns (Sequence[TColumnSchema], optional): A list of column schemas. Typed dictionary describing column names, data types, write disposition and performance hints that gives you full control over the created table schema.
 
             primary_key (str | Sequence[str]): A column name or a list of column names that comprise a private key. Typically used with "merge" write disposition to deduplicate loaded data.
 
             schema (Schema, optional): An explicit `Schema` object in which all table schemas will be grouped. By default `dlt` takes the schema from the source (if passed in `data` argument) or creates a default one itself.
 
-            loader_file_format (Literal["jsonl", "puae-jsonl", "insert_values", "sql", "parquet"], optional). The file format the loader will use to create the load package. Not all file_formats are compatible with all destinations. Defaults to the preferred file format of the selected destination.
+            loader_file_format (Literal["jsonl", "insert_values", "parquet"], optional). The file format the loader will use to create the load package. Not all file_formats are compatible with all destinations. Defaults to the preferred file format of the selected destination.
 
         ### Raises:
             PipelineStepFailed when a problem happened during `extract`, `normalize` or `load` steps.
         ### Returns:
             LoadInfo: Information on loaded data including the list of package ids and failed job statuses. Please not that `dlt` will not raise if a single job terminally fails. Such information is provided via LoadInfo.
         """
         signals.raise_if_signalled()
         self._set_destination(destination)
+        self._set_staging(staging)
         self._set_dataset_name(dataset_name)
 
         # sync state with destination
         if self.config.restore_from_destination and not self.full_refresh and not self._state_restored and (self.destination or destination):
             self.sync_destination(destination, dataset_name)
             # sync only once
             self._state_restored = True
@@ -840,61 +858,81 @@
         # get the current schema and merge tables from source_schema
         # note we are not merging props like max nesting or column propagation
         for table in source_schema.data_tables():
             pipeline_schema.update_schema(pipeline_schema.normalize_table_identifiers(table))
 
         return extract_id
 
-    def _get_destination_client_initial_config(self, credentials: Any = None) -> DestinationClientConfiguration:
-        if not self.destination:
+    def _get_destination_client_initial_config(self, destination: DestinationReference = None, credentials: Any = None, as_staging: bool = False) -> DestinationClientConfiguration:
+        destination = destination or self.destination
+        if not destination:
             raise PipelineConfigMissing(
                 self.pipeline_name,
                 "destination",
                 "load",
                 "Please provide `destination` argument to `pipeline`, `run` or `load` method directly or via .dlt config.toml file or environment variable."
             )
         # create initial destination client config
-        client_spec = self.destination.spec()
+        client_spec = destination.spec()
         # initialize explicit credentials
         credentials = credentials or self.credentials
         if credentials is not None and not isinstance(credentials, CredentialsConfiguration):
             # use passed credentials as initial value. initial value may resolve credentials
             credentials = client_spec.get_resolvable_fields()["credentials"](credentials)
         # this client support schemas and datasets
-        if issubclass(client_spec, DestinationClientDwhConfiguration):
+        default_schema_name = None if self.config.use_single_dataset else self.default_schema_name
+
+        if issubclass(client_spec, DestinationClientStagingConfiguration):
+            return client_spec(dataset_name=self.dataset_name, default_schema_name=default_schema_name, credentials=credentials, as_staging=as_staging)
+        elif issubclass(client_spec, DestinationClientDwhConfiguration):
             # set default schema name to load all incoming data to a single dataset, no matter what is the current schema name
-            default_schema_name = None if self.config.use_single_dataset else self.default_schema_name
             return client_spec(dataset_name=self.dataset_name, default_schema_name=default_schema_name, credentials=credentials)
-        else:
-            return client_spec(credentials=credentials)
+        return client_spec(credentials=credentials)
 
     def _get_destination_client(self, schema: Schema, initial_config: DestinationClientConfiguration = None) -> JobClientBase:
         try:
             # config is not provided then get it with injected credentials
             if not initial_config:
-                initial_config = self._get_destination_client_initial_config()
+                initial_config = self._get_destination_client_initial_config(self.destination)
             return self.destination.client(schema, initial_config)
         except ImportError:
             client_spec = self.destination.spec()
             raise MissingDependencyException(
                 f"{client_spec.destination_name} destination",
                 [f"{version.DLT_PKG_NAME}[{client_spec.destination_name}]"],
                 "Dependencies for specific destinations are available as extras of dlt"
             )
 
+    def _get_staging_client(self, schema: Schema, initial_config: DestinationClientConfiguration = None) -> JobClientBase:
+        try:
+            # config is not provided then get it with injected credentials
+            if not initial_config:
+                initial_config = self._get_destination_client_initial_config(self.staging, as_staging=True)
+            return self.staging.client(schema, initial_config) # type: ignore
+        except ImportError:
+            client_spec = self.destination.spec()
+            raise MissingDependencyException(
+                f"{client_spec.destination_name} destination",
+                [f"{version.DLT_PKG_NAME}[{client_spec.destination_name}]"],
+                "Dependencies for specific destinations are available as extras of dlt"
+            )
+
     def _get_destination_capabilities(self) -> DestinationCapabilitiesContext:
         if not self.destination:
                 raise PipelineConfigMissing(
                     self.pipeline_name,
                     "destination",
                     "normalize",
                     "Please provide `destination` argument to `pipeline`, `run` or `load` method directly or via .dlt config.toml file or environment variable."
                 )
         return self.destination.capabilities()
 
+    def _get_staging_capabilities(self) -> DestinationCapabilitiesContext:
+        return self.staging.capabilities() if self.staging is not None else None # type: ignore
+
     def _validate_pipeline_name(self) -> None:
         try:
             FileStorage.validate_file_name_component(self.pipeline_name)
         except ValueError as ve_ex:
             raise InvalidPipelineName(self.pipeline_name, str(ve_ex))
 
     def _make_schema_with_default_name(self) -> Schema:
@@ -925,29 +963,64 @@
     def _set_destination(self, destination: TDestinationReferenceArg) -> None:
         destination_mod = DestinationReference.from_name(destination)
         self.destination = destination_mod or self.destination
         with self._maybe_destination_capabilities():
             # default normalizers must match the destination
             self._set_default_normalizers()
 
+    def _set_staging(self, staging: TDestinationReferenceArg) -> None:
+        staging_module = DestinationReference.from_name(staging)
+        if staging_module and not issubclass(staging_module.spec(), DestinationClientStagingConfiguration):
+            raise DestinationNoStagingMode(staging_module.__name__)
+        self.staging = staging_module or self.staging
+
     @contextmanager
     def _maybe_destination_capabilities(self, loader_file_format: TLoaderFileFormat = None) -> Iterator[DestinationCapabilitiesContext]:
         try:
             caps: DestinationCapabilitiesContext = None
             injected_caps: ContextManager[DestinationCapabilitiesContext] = None
             if self.destination:
-                injected_caps = self._container.injectable_context(self._get_destination_capabilities())
+                destination_caps = self._get_destination_capabilities()
+                stage_caps = self._get_staging_capabilities()
+                injected_caps = self._container.injectable_context(destination_caps)
                 caps = injected_caps.__enter__()
-                if loader_file_format:
-                    caps.preferred_loader_file_format = loader_file_format
+
+                caps.preferred_loader_file_format = self._resolve_loader_file_format(
+                    DestinationReference.to_name(self.destination),
+                    DestinationReference.to_name(self.staging) if self.staging else None,
+                    destination_caps, stage_caps, loader_file_format)
             yield caps
         finally:
             if injected_caps:
                 injected_caps.__exit__(None, None, None)
 
+    @staticmethod
+    def _resolve_loader_file_format(
+            destination: str,
+            staging: str,
+            dest_caps: DestinationCapabilitiesContext,
+            stage_caps: DestinationCapabilitiesContext,
+            file_format: TLoaderFileFormat) -> TLoaderFileFormat:
+
+        possible_file_formats = dest_caps.supported_loader_file_formats
+        if stage_caps:
+            if not dest_caps.supported_staging_file_formats:
+                raise DestinationLoadingViaStagingNotSupported(destination)
+            possible_file_formats = [f for f in dest_caps.supported_staging_file_formats if f in stage_caps.supported_loader_file_formats]
+        if not file_format:
+            if not stage_caps:
+                file_format = dest_caps.preferred_loader_file_format
+            elif stage_caps and dest_caps.preferred_staging_file_format in possible_file_formats:
+                file_format = dest_caps.preferred_staging_file_format
+            else:
+                file_format = possible_file_formats[0] if len(possible_file_formats) > 0 else None
+        if file_format not in possible_file_formats:
+            raise DestinationIncompatibleLoaderFileFormatException(destination, staging, file_format, set(possible_file_formats) - INTERNAL_LOADER_FILE_FORMATS)
+        return file_format
+
     def _set_default_normalizers(self) -> None:
         self._default_naming, _ = import_normalizers(default_normalizers())
 
     def _set_dataset_name(self, dataset_name: str) -> None:
         if not dataset_name:
             if not self.dataset_name:
                 # set default dataset name from pipeline name
@@ -1120,27 +1193,31 @@
         """Write `state` to pipeline props."""
         for prop in Pipeline.STATE_PROPS:
             if prop in state and not prop.startswith("_"):
                 setattr(self, prop, state[prop])  # type: ignore
         for prop in Pipeline.LOCAL_STATE_PROPS:
             if prop in state["_local"] and not prop.startswith("_"):
                 setattr(self, prop, state["_local"][prop])  # type: ignore
+        if "staging" in state:
+            self._set_staging(DestinationReference.from_name(self.staging))
         if "destination" in state:
             self._set_destination(DestinationReference.from_name(self.destination))
 
     def _props_to_state(self, state: TPipelineState) -> None:
         """Write pipeline props to `state`"""
         for prop in Pipeline.STATE_PROPS:
             if not prop.startswith("_"):
                 state[prop] = getattr(self, prop)  # type: ignore
         for prop in Pipeline.LOCAL_STATE_PROPS:
             if not prop.startswith("_"):
                 state["_local"][prop] = getattr(self, prop)  # type: ignore
         if self.destination:
             state["destination"] = self.destination.__name__
+        if self.staging:
+            state["staging"] = self.staging.__name__
         state["schema_names"] = self._schema_storage.list_schemas()
 
     def _save_state(self, state: TPipelineState) -> None:
         self._pipeline_storage.save(Pipeline.STATE_FILE, json_encode_state(state))
 
     def _extract_state(self, state: TPipelineState) -> TPipelineState:
         # this will extract the state into current load package and update the schema with the _dlt_pipeline_state table
```

### Comparing `dlt-0.3.3a0/dlt/pipeline/progress.py` & `dlt-0.3.4/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/pipeline/state_sync.py` & `dlt-0.3.4/dlt/pipeline/state_sync.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/pipeline/trace.py` & `dlt-0.3.4/dlt/pipeline/trace.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
 import pickle
 import datetime  # noqa: 251
 import dataclasses
-from typing import Any, List, NamedTuple, Optional, Protocol, Sequence
-
+from collections.abc import Sequence as C_Sequence
+from typing import Any, List, Tuple, NamedTuple, Optional, Protocol, Sequence
 import humanize
 
 from dlt.common import pendulum
 from dlt.common.runtime.logger import suppress_and_warn
 from dlt.common.configuration import is_secret_hint
 from dlt.common.configuration.utils import _RESOLVED_TRACES
-from dlt.common.pipeline import SupportsPipeline
+from dlt.common.pipeline import ExtractDataInfo, SupportsPipeline
 from dlt.common.typing import StrAny
 from dlt.common.utils import uniq_id
 
+from dlt.extract.source import DltResource, DltSource
 from dlt.pipeline.typing import TPipelineStep
 from dlt.pipeline.exceptions import PipelineStepFailed
 
 
 TRACE_ENGINE_VERSION = 1
 TRACE_FILE_NAME = "trace.pickle"
 
@@ -208,7 +209,39 @@
 def load_trace(trace_path: str) -> PipelineTrace:
     try:
         with open(os.path.join(trace_path, TRACE_FILE_NAME), mode="rb") as f:
             return pickle.load(f)  # type: ignore
     except (AttributeError, FileNotFoundError):
         # on incompatible pickling / file not found return no trace
         return None
+
+
+def describe_extract_data(data: Any) -> List[ExtractDataInfo]:
+    """Extract source and resource names from data passed to extract"""
+    data_info: List[ExtractDataInfo] = []
+
+    def add_item(item: Any) -> bool:
+        if isinstance(item, (DltResource, DltSource)):
+            # record names of sources/resources
+            data_info.append({
+                "name": item.name,
+                "data_type": "resource" if isinstance(item, DltResource) else "source"
+            })
+            return False
+        else:
+            # anything else
+            data_info.append({
+                "name": "",
+                "data_type": type(item).__name__
+            })
+            return True
+
+    item: Any = data
+    if isinstance(data, C_Sequence) and len(data) > 0:
+        for item in data:
+            # add_item returns True if non named item was returned. in that case we break
+            if add_item(item):
+                break
+        return data_info
+
+    add_item(item)
+    return data_info
```

### Comparing `dlt-0.3.3a0/dlt/pipeline/track.py` & `dlt-0.3.4/dlt/pipeline/track.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sentry_sdk.tracing import Span
 
 from dlt.common import pendulum
 from dlt.common import logger
 from dlt.common.runtime.exec_info import github_info
 from dlt.common.runtime.segment import track as dlthub_telemetry_track
 from dlt.common.runtime.slack import send_slack_message
-from dlt.common.pipeline import LoadInfo, SupportsPipeline
+from dlt.common.pipeline import LoadInfo, ExtractInfo, SupportsPipeline
 from dlt.common.destination import DestinationReference
 
 from dlt.pipeline.typing import TPipelineStep
 from dlt.pipeline.trace import PipelineTrace, PipelineStepTrace
 
 
 def _add_sentry_tags(span: Span, pipeline: SupportsPipeline) -> None:
@@ -76,20 +76,25 @@
         # print(f"---END SENTRY SPAN {trace.transaction_id}:{step.span_id}: {step} SCOPE: {Hub.current.scope}")
         with contextlib.suppress(Exception):
             Hub.current.scope.span.__exit__(None, None, None)
     # disable automatic slack messaging until we can configure messages themselves
     # if step.step == "load":
     #     if pipeline.runtime_config.slack_incoming_hook and step.step_exception is None:
     #         slack_notify_load_success(pipeline.runtime_config.slack_incoming_hook, step_info, trace)
-    dlthub_telemetry_track("pipeline", step.step, {
+    props = {
         "elapsed": (step.finished_at - trace.started_at).total_seconds(),
         "success": step.step_exception is None,
         "destination_name": DestinationReference.to_name(pipeline.destination) if pipeline.destination else None,
         "transaction_id": trace.transaction_id
-    })
+    }
+    # disable automatic slack messaging until we can configure messages themselves
+    if step.step == "extract" and step_info:
+        assert isinstance(step_info, ExtractInfo)
+        props["extract_data"] = step_info.extract_data_info
+    dlthub_telemetry_track("pipeline", step.step, props)
 
 
 def on_end_trace(trace: PipelineTrace, pipeline: SupportsPipeline) -> None:
     if pipeline.runtime_config.sentry_dsn:
         # print(f"---END SENTRY TX: {trace.transaction_id} SCOPE: {Hub.current.scope}")
         with contextlib.suppress(Exception):
             Hub.current.scope.span.__exit__(None, None, None)
```

### Comparing `dlt-0.3.3a0/dlt/reflection/names.py` & `dlt-0.3.4/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/reflection/script_inspector.py` & `dlt-0.3.4/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/reflection/script_visitor.py` & `dlt-0.3.4/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/sources/helpers/requests/retry.py` & `dlt-0.3.4/dlt/sources/helpers/requests/retry.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from email.utils import parsedate_tz, mktime_tz
 import re
 import time
-from typing import Optional, cast, Callable, Type, Union, Sequence, Tuple, List, TYPE_CHECKING, Any
+from typing import Optional, cast, Callable, Type, Union, Sequence, Tuple, List, TYPE_CHECKING, Any, Dict
 from threading import local
 
-from requests import Response, HTTPError, ConnectionError, Timeout, Session as BaseSession
+from requests import Response, HTTPError, Session as BaseSession
+from requests.exceptions import ConnectionError, Timeout, ChunkedEncodingError
 from requests.adapters import HTTPAdapter
 from tenacity import Retrying, retry_if_exception_type, stop_after_attempt, RetryCallState, retry_any, wait_exponential
 from tenacity.retry import retry_base
 
 from dlt.sources.helpers.requests.session import Session, DEFAULT_TIMEOUT
+from dlt.sources.helpers.requests.typing import TRequestTimeout
 from dlt.common.typing import TimedeltaSeconds
+from dlt.common.configuration.specs import RunConfiguration
+from dlt.common.configuration import with_config
 
 
 DEFAULT_RETRY_STATUS = (429, *range(500, 600))
-DEFAULT_RETRY_EXCEPTIONS = (ConnectionError, Timeout)
-DEFAULT_RETRY_ATTEMPTS = 5
-DEFAULT_BACKOFF_FACTOR = 1
+DEFAULT_RETRY_EXCEPTIONS = (ConnectionError, Timeout, ChunkedEncodingError)
 
 RetryPredicate = Callable[[Optional[Response], Optional[BaseException]], bool]
 
 
 def _get_retry_response(retry_state: RetryCallState) -> Optional[Response]:
     ex = retry_state.outcome.exception()
     if ex:
@@ -89,28 +91,29 @@
 def _make_retry(
     status_codes: Sequence[int],
     exceptions: Sequence[Type[Exception]],
     max_attempts: int,
     condition: Union[RetryPredicate, Sequence[RetryPredicate], None],
     backoff_factor: float,
     respect_retry_after_header: bool,
+    max_delay: TimedeltaSeconds,
 )-> Retrying:
     retry_conds = [retry_if_status(status_codes), retry_if_exception_type(tuple(exceptions))]
     if condition is not None:
         if callable(condition):
             retry_condition = [condition]
         retry_conds.extend([retry_if_predicate(c) for c in retry_condition])
 
     wait_cls = wait_exponential_retry_after if respect_retry_after_header else wait_exponential
     return Retrying(
-        wait=wait_cls(multiplier=backoff_factor),
+        wait=wait_cls(multiplier=backoff_factor, max=max_delay),
         retry=(retry_any(*retry_conds)),
         stop=stop_after_attempt(max_attempts),
         reraise=True,
-        retry_error_callback=lambda state: state.outcome.result()
+        retry_error_callback=lambda state: state.outcome.result(),
     )
 
 
 class Client:
     """Wrapper for `requests` to create a `Session` with configurable retry functionality.
 
     ### Summary
@@ -128,51 +131,57 @@
     >>>     if response is None:
     >>>         return False
     >>>     return response.text == 'error'
 
     The retry is triggered when either any of the predicates or the default conditions based on status code/exception are `True`.
 
     ### Args:
-        timeout: Timeout for requests in seconds. May be passed as `timedelta` or `float/int` number of seconds.
+        request_timeout: Timeout for requests in seconds. May be passed as `timedelta` or `float/int` number of seconds.
         max_connections: Max connections per host in the HTTPAdapter pool
         raise_for_status: Whether to raise exception on error status codes (using `response.raise_for_status()`)
         session: Optional `requests.Session` instance to add the retry handler to. A new session is created by default.
         status_codes: Retry when response has any of these status codes. Default `429` and all `5xx` codes. Pass an empty list to disable retry based on status.
         exceptions: Retry on exception of given type(s). Default `(requests.Timeout, requests.ConnectionError)`. Pass an empty list to disable retry on exceptions.
-        max_attempts: Max number of retry attempts before giving up
-        condition: A predicate or a list of predicates to decide whether to retry. If any predicate returns `True` the request is retried
-        backoff_factor: Multiplier used for exponential delay between retries
+        request_max_attempts: Max number of retry attempts before giving up
+        retry_condition: A predicate or a list of predicates to decide whether to retry. If any predicate returns `True` the request is retried
+        request_backoff_factor: Multiplier used for exponential delay between retries
+        request_max_retry_delay: Maximum delay when using exponential backoff
         respect_retry_after_header: Whether to use the `Retry-After` response header (when available) to determine the retry delay
-        **session_attrs: Extra attributes that will be set on the session instance, e.g. `headers: {'Authorization': 'api-key'}` (see `requests.sessions.Session` for possible attributes)
+        session_attrs: Extra attributes that will be set on the session instance, e.g. `{headers: {'Authorization': 'api-key'}}` (see `requests.sessions.Session` for possible attributes)
     """
+    _session_attrs: Dict[str, Any]
+
+    @with_config(spec=RunConfiguration)
     def __init__(
         self,
-        timeout: Optional[TimedeltaSeconds] = DEFAULT_TIMEOUT,
+        request_timeout: Optional[Union[TimedeltaSeconds, Tuple[TimedeltaSeconds, TimedeltaSeconds]]] = DEFAULT_TIMEOUT,
         max_connections: int = 50,
         raise_for_status: bool = True,
         status_codes: Sequence[int] = DEFAULT_RETRY_STATUS,
         exceptions: Sequence[Type[Exception]] = DEFAULT_RETRY_EXCEPTIONS,
-        max_attempts: int = DEFAULT_RETRY_ATTEMPTS,
-        condition: Union[RetryPredicate, Sequence[RetryPredicate], None] = None,
-        backoff_factor: float = DEFAULT_BACKOFF_FACTOR,
+        request_max_attempts: int = RunConfiguration.request_max_attempts,
+        retry_condition: Union[RetryPredicate, Sequence[RetryPredicate], None] = None,
+        request_backoff_factor: float = RunConfiguration.request_backoff_factor,
+        request_max_retry_delay: TimedeltaSeconds = RunConfiguration.request_max_retry_delay,
         respect_retry_after_header: bool = True,
-        **session_attrs: Any
+        session_attrs: Optional[Dict[str, Any]] = None,
     ) -> None:
         self._adapter = HTTPAdapter(pool_maxsize=max_connections)
         self._local = local()
-        self._session_kwargs = dict(timeout=timeout, raise_for_status=raise_for_status)
-        self._retry_kwargs = dict(
+        self._session_kwargs = dict(timeout=request_timeout, raise_for_status=raise_for_status)
+        self._retry_kwargs: Dict[str, Any] = dict(
             status_codes=status_codes,
             exceptions=exceptions,
-            max_attempts=max_attempts,
-            condition=condition,
-            backoff_factor=backoff_factor,
-            respect_retry_after_header=respect_retry_after_header
+            max_attempts=request_max_attempts,
+            condition=retry_condition,
+            backoff_factor=request_backoff_factor,
+            respect_retry_after_header=respect_retry_after_header,
+            max_delay=request_max_retry_delay
         )
-        self._session_attrs = session_attrs
+        self._session_attrs = session_attrs or {}
 
         if TYPE_CHECKING:
             self.get = self.session.get
             self.post = self.session.post
             self.put = self.session.put
             self.patch = self.session.patch
             self.delete = self.session.delete
@@ -185,23 +194,38 @@
         self.put = lambda *a, **kw: self.session.put(*a, **kw)
         self.patch = lambda *a, **kw: self.session.patch(*a, **kw)
         self.delete = lambda *a, **kw: self.session.delete(*a, **kw)
         self.head = lambda *a, **kw: self.session.head(*a, **kw)
         self.options = lambda *a, **kw: self.session.options(*a, **kw)
         self.request = lambda *a, **kw: self.session.request(*a, **kw)
 
+        self._config_version: int = 0  # Incrementing marker to ensure per-thread sessions are recreated on config changes
+
+    def update_from_config(self, config: RunConfiguration) -> None:
+        """Update session/retry settings from RunConfiguration"""
+        self._session_kwargs['timeout'] = config.request_timeout
+        self._retry_kwargs['backoff_factor'] = config.request_backoff_factor
+        self._retry_kwargs['max_delay'] = config.request_max_retry_delay
+        self._retry_kwargs['max_attempts'] = config.request_max_attempts
+        self._config_version += 1
+
     def _make_session(self) -> Session:
         session = Session(**self._session_kwargs)  # type: ignore[arg-type]
         for key, value in self._session_attrs.items():
             setattr(session, key, value)
         session.mount('http://', self._adapter)
         session.mount('https://', self._adapter)
-        retry = _make_retry(**self._retry_kwargs)  # type: ignore[arg-type]
+        retry = _make_retry(**self._retry_kwargs)
         session.request = retry.wraps(session.request)  # type: ignore[method-assign]
         return session
 
     @property
     def session(self) -> Session:
         session: Optional[Session] = getattr(self._local, 'session', None)
-        if session is None:
+        version = self._config_version
+        if session is not None:
+            version = self._local.config_version
+        if session is None or version != self._config_version:
+            # Create a new session if config has changed
             session = self._local.session = self._make_session()
+            self._local.config_version = self._config_version
         return session
```

### Comparing `dlt-0.3.3a0/dlt/sources/helpers/requests/session.py` & `dlt-0.3.4/dlt/sources/helpers/requests/session.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 from requests import Session as BaseSession
 from tenacity import Retrying, retry_if_exception_type
 from typing import Optional, TYPE_CHECKING, Sequence, Union, Tuple, Type, TypeVar
 
+from dlt.sources.helpers.requests.typing import TRequestTimeout
 from dlt.common.typing import TimedeltaSeconds
 from dlt.common.time import to_seconds
 
 
 TSession = TypeVar("TSession", bound=BaseSession)
 
 
-DEFAULT_TIMEOUT = 30
+DEFAULT_TIMEOUT = 60
+
+
+def _timeout_to_seconds(timeout: TRequestTimeout) -> Optional[Union[Tuple[float, float], float]]:
+    return (to_seconds(timeout[0]), to_seconds(timeout[1])) if isinstance(timeout, tuple) else to_seconds(timeout)
 
 
 class Session(BaseSession):
     """Requests session which by default adds a timeout to all requests and calls `raise_for_status()` on response
 
     ### Args
         timeout: Timeout for requests in seconds. May be passed as `timedelta` or `float/int` number of seconds.
+            May be a single value or a tuple for separate (connect, read) timeout.
         raise_for_status: Whether to raise exception on error status codes (using `response.raise_for_status()`)
     """
     def __init__(
         self,
-        timeout: Optional[TimedeltaSeconds] = DEFAULT_TIMEOUT,
+        timeout: Optional[Union[TimedeltaSeconds, Tuple[TimedeltaSeconds, TimedeltaSeconds]]] = DEFAULT_TIMEOUT,
         raise_for_status: bool = True,
     ) -> None:
         super().__init__()
-        self.timeout = to_seconds(timeout)
+        self.timeout = _timeout_to_seconds(timeout)
         self.raise_for_status = raise_for_status
 
     if TYPE_CHECKING:
         request = BaseSession.request
 
     def request(self, *args, **kwargs):  # type: ignore[no-untyped-def,no-redef]
         kwargs.setdefault('timeout', self.timeout)
```

### Comparing `dlt-0.3.3a0/dlt/sources/helpers/transform.py` & `dlt-0.3.4/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/dlt/version.py` & `dlt-0.3.4/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.3a0/pyproject.toml` & `dlt-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.3.3a0"
+version = "0.3.4"
 description = "DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
@@ -59,19 +59,19 @@
 
 grpcio = {version = ">=1.50.0", optional = true}
 google-cloud-bigquery = {version = ">=2.26.0", optional = true}
 pyarrow = {version = ">=8.0.0", optional = true}
 
 duckdb = {version = ">=0.6.1,<0.9.0", optional = true}
 
-dbt-core = {version = ">=1.3.0,<1.5.0", optional = true}
-dbt-redshift = {version = ">=1.3.0,<1.5.0", optional = true}
-dbt-bigquery = {version = ">=1.3.0,<1.5.0", optional = true}
-dbt-duckdb = {version = ">=1.3.0,<1.5.0", optional = true}
-dbt-snowflake = {version = ">=1.3.0,<1.5.0", optional = true}
+dbt-core = {version = ">=1.5.0", optional = true}
+dbt-redshift = {version = ">=1.5.0", optional = true}
+dbt-bigquery = {version = ">=1.5.0", optional = true}
+dbt-duckdb = {version = ">=1.5.0", optional = true}
+dbt-snowflake = {version = ">=1.5.0", optional = true}
 s3fs = {version = "^2023.5.0", optional = true}
 gcsfs = {version = "^2023.5.0", optional = true}
 boto3 = {version = ">=1.26", optional = true}
 fsspec = "^2023.5.0"
 snowflake-connector-python = {version = "^3.0.4", optional = true, extras = ["pandas"]}
```

### Comparing `dlt-0.3.3a0/setup.py` & `dlt-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,19 +76,19 @@
 
 extras_require = \
 {':platform_python_implementation != "PyPy"': ['orjson>=3.8.6,<4.0.0'],
  'bigquery': ['grpcio>=1.50.0',
               'google-cloud-bigquery>=2.26.0',
               'pyarrow>=8.0.0',
               'gcsfs>=2023.5.0,<2024.0.0'],
- 'dbt': ['dbt-core>=1.3.0,<1.5.0',
-         'dbt-redshift>=1.3.0,<1.5.0',
-         'dbt-bigquery>=1.3.0,<1.5.0',
-         'dbt-duckdb>=1.3.0,<1.5.0',
-         'dbt-snowflake>=1.3.0,<1.5.0'],
+ 'dbt': ['dbt-core>=1.5.0',
+         'dbt-redshift>=1.5.0',
+         'dbt-bigquery>=1.5.0',
+         'dbt-duckdb>=1.5.0',
+         'dbt-snowflake>=1.5.0'],
  'duckdb': ['duckdb>=0.6.1,<0.9.0'],
  'filesystem': ['s3fs>=2023.5.0,<2024.0.0', 'boto3>=1.26'],
  'gcp': ['grpcio>=1.50.0',
          'google-cloud-bigquery>=2.26.0',
          'gcsfs>=2023.5.0,<2024.0.0'],
  'gs': ['gcsfs>=2023.5.0,<2024.0.0'],
  'motherduck': ['pyarrow>=8.0.0', 'duckdb>=0.6.1,<0.9.0'],
@@ -101,15 +101,15 @@
  'snowflake': ['snowflake-connector-python[pandas]>=3.0.4,<4.0.0']}
 
 entry_points = \
 {'console_scripts': ['dlt = dlt.cli._dlt:_main']}
 
 setup_kwargs = {
     'name': 'dlt',
-    'version': '0.3.3a0',
+    'version': '0.3.4',
     'description': 'DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.',
     'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nfrom chess import chess # a utility function that grabs data from the chess.com API\n\n# create a dlt pipeline that will load chess game data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'games_data\'\n)\n\n# use chess.com API to grab data about a few players\ndata = chess([\'magnuscarlsen\', \'rpragchess\'], start_month=\'2022/11\', end_month=\'2022/12\')\n\n# extract, normalize, and load the data\npipeline.run(data)\n```\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Sources and Destinations\n\nExplore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/dlt-ecosystem/verified-sources) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/dlt-ecosystem/destinations).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Verified Sources**: Contribute your custom sources to the [dlt-hub/verified-sources](https://github.com/dlt-hub/verified-sources) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
     'author': 'dltHub Inc.',
     'author_email': 'services@dlthub.com',
     'maintainer': 'Marcin Rudolf',
     'maintainer_email': 'marcin@dlthub.com',
     'url': 'https://github.com/dlt-hub',
```

### Comparing `dlt-0.3.3a0/PKG-INFO` & `dlt-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.3.3a0
+Version: 0.3.4
 Summary: DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
@@ -35,19 +35,19 @@
 Provides-Extra: snowflake
 Requires-Dist: PyYAML (>=5.4.1)
 Requires-Dist: SQLAlchemy (>=1.4.0)
 Requires-Dist: astunparse (>=1.6.3)
 Requires-Dist: boto3 (>=1.26); extra == "filesystem" or extra == "s3"
 Requires-Dist: click (>=7.1)
 Requires-Dist: cron-descriptor (>=1.2.32)
-Requires-Dist: dbt-bigquery (>=1.3.0,<1.5.0); extra == "dbt"
-Requires-Dist: dbt-core (>=1.3.0,<1.5.0); extra == "dbt"
-Requires-Dist: dbt-duckdb (>=1.3.0,<1.5.0); extra == "dbt"
-Requires-Dist: dbt-redshift (>=1.3.0,<1.5.0); extra == "dbt"
-Requires-Dist: dbt-snowflake (>=1.3.0,<1.5.0); extra == "dbt"
+Requires-Dist: dbt-bigquery (>=1.5.0); extra == "dbt"
+Requires-Dist: dbt-core (>=1.5.0); extra == "dbt"
+Requires-Dist: dbt-duckdb (>=1.5.0); extra == "dbt"
+Requires-Dist: dbt-redshift (>=1.5.0); extra == "dbt"
+Requires-Dist: dbt-snowflake (>=1.5.0); extra == "dbt"
 Requires-Dist: deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: duckdb (>=0.6.1,<0.9.0); extra == "duckdb" or extra == "motherduck"
 Requires-Dist: fsspec (>=2023.5.0,<2024.0.0)
 Requires-Dist: gcsfs (>=2023.5.0,<2024.0.0); extra == "gcp" or extra == "bigquery" or extra == "gs"
 Requires-Dist: gitpython (>=3.1.29)
 Requires-Dist: giturlparse (>=0.10.0)
 Requires-Dist: google-cloud-bigquery (>=2.26.0); extra == "gcp" or extra == "bigquery"
```

