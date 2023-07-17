# Comparing `tmp/avista_digital_exchange_sdk-0.3.0.tar.gz` & `tmp/avista_digital_exchange_sdk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avista_digital_exchange_sdk-0.3.0.tar", last modified: Thu Jun 15 18:41:10 2023, max compression
+gzip compressed data, was "avista_digital_exchange_sdk-0.3.1.tar", last modified: Mon Jul 17 19:09:25 2023, max compression
```

## Comparing `avista_digital_exchange_sdk-0.3.0.tar` & `avista_digital_exchange_sdk-0.3.1.tar`

### file list

```diff
@@ -1,268 +1,264 @@
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.330997 avista_digital_exchange_sdk-0.3.0/
--rw-r--r--   0 Justin     (502) staff       (20)    35148 2022-09-13 20:02:44.000000 avista_digital_exchange_sdk-0.3.0/LICENSE
--rw-r--r--   0 Justin     (502) staff       (20)    74798 2023-06-15 18:41:10.330617 avista_digital_exchange_sdk-0.3.0/PKG-INFO
--rw-r--r--   0 Justin     (502) staff       (20)    33555 2023-06-15 18:40:21.000000 avista_digital_exchange_sdk-0.3.0/README.md
--rw-r--r--   0 Justin     (502) staff       (20)      910 2023-06-15 18:28:56.000000 avista_digital_exchange_sdk-0.3.0/pyproject.toml
--rw-r--r--   0 Justin     (502) staff       (20)       38 2023-06-15 18:41:10.331095 avista_digital_exchange_sdk-0.3.0/setup.cfg
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.178336 avista_digital_exchange_sdk-0.3.0/src/
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.192415 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/
--rw-r--r--   0 Justin     (502) staff       (20)     4968 2023-06-15 18:28:20.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/DxTypes.py
--rw-r--r--   0 Justin     (502) staff       (20)      213 2023-06-14 18:10:08.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/__init__.py
--rw-r--r--   0 Justin     (502) staff       (20)     1628 2023-06-15 18:31:43.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/avista_digital_exchange.py
--rw-r--r--   0 Justin     (502) staff       (20)     3268 2023-06-15 18:28:32.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/client.py
--rw-r--r--   0 Justin     (502) staff       (20)     3384 2022-12-02 17:38:29.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/collaborativeUtil.py
--rw-r--r--   0 Justin     (502) staff       (20)     6799 2023-06-15 18:28:11.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/dataCaptureUtil.py
--rw-r--r--   0 Justin     (502) staff       (20)     2784 2022-12-02 17:57:07.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/dataStoreUtil.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.223612 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/
--rw-r--r--   0 Justin     (502) staff       (20)        0 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/__init__.py
--rw-r--r--   0 Justin     (502) staff       (20)     1989 2022-09-29 18:39:50.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/collaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     1630 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/collaborative_member_organization.py
--rw-r--r--   0 Justin     (502) staff       (20)      852 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/collaborative_member_user.py
--rw-r--r--   0 Justin     (502) staff       (20)     6818 2022-10-10 19:11:23.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/data_store.py
--rw-r--r--   0 Justin     (502) staff       (20)     6384 2022-12-19 18:46:23.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/data_store_directory.py
--rw-r--r--   0 Justin     (502) staff       (20)     6657 2022-12-19 18:45:32.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/data_store_file.py
--rw-r--r--   0 Justin     (502) staff       (20)     2124 2022-10-05 17:07:09.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/data_store_object.py
--rw-r--r--   0 Justin     (502) staff       (20)     1751 2023-01-24 17:50:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/digital_twin_model.py
--rw-r--r--   0 Justin     (502) staff       (20)     1414 2022-12-05 17:33:37.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_last_values.py
--rw-r--r--   0 Justin     (502) staff       (20)     1214 2022-11-28 17:35:44.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_property.py
--rw-r--r--   0 Justin     (502) staff       (20)      990 2022-11-29 01:10:28.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_property_input.py
--rw-r--r--   0 Justin     (502) staff       (20)      681 2022-11-29 19:31:15.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_query_filter_input.py
--rw-r--r--   0 Justin     (502) staff       (20)     1020 2022-12-02 19:07:37.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry.py
--rw-r--r--   0 Justin     (502) staff       (20)     1340 2022-12-03 00:58:02.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry_data_record.py
--rw-r--r--   0 Justin     (502) staff       (20)      924 2022-12-01 19:36:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_attribute_value.py
--rw-r--r--   0 Justin     (502) staff       (20)      403 2022-12-09 00:20:12.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_attribute_value_input.py
--rw-r--r--   0 Justin     (502) staff       (20)     1175 2022-11-22 17:09:32.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_data_record.py
--rw-r--r--   0 Justin     (502) staff       (20)      860 2022-11-22 17:17:39.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_data_record_error.py
--rw-r--r--   0 Justin     (502) staff       (20)     1816 2022-12-19 19:40:35.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_data_record_input.py
--rw-r--r--   0 Justin     (502) staff       (20)     1479 2022-11-28 18:00:38.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_data_record_with_errors.py
--rw-r--r--   0 Justin     (502) staff       (20)     1834 2022-12-03 00:56:11.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_endpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     1396 2022-11-30 19:33:37.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_endpoint_data.py
--rw-r--r--   0 Justin     (502) staff       (20)     1807 2022-12-05 17:37:27.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_endpoints_last_values_query_result.py
--rw-r--r--   0 Justin     (502) staff       (20)      726 2022-12-01 19:24:03.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_generate_query_result_export.py
--rw-r--r--   0 Justin     (502) staff       (20)     1889 2022-12-13 17:12:23.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_query_by_time_range_result.py
--rw-r--r--   0 Justin     (502) staff       (20)     2008 2022-12-13 17:11:14.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_query_export.py
--rw-r--r--   0 Justin     (502) staff       (20)     1161 2023-01-24 17:48:06.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/model_property.py
--rw-r--r--   0 Justin     (502) staff       (20)     1795 2023-01-25 00:41:35.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/model_property_input.py
--rw-r--r--   0 Justin     (502) staff       (20)     1017 2023-01-24 17:48:35.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/model_telemetry.py
--rw-r--r--   0 Justin     (502) staff       (20)      984 2023-01-25 00:48:12.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/model_telemetry_input.py
--rw-r--r--   0 Justin     (502) staff       (20)      785 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/organization.py
--rw-r--r--   0 Justin     (502) staff       (20)      732 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/presigned_url.py
--rw-r--r--   0 Justin     (502) staff       (20)     1521 2022-12-08 19:15:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/publish_iot_data_result.py
--rw-r--r--   0 Justin     (502) staff       (20)      727 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/server_response.py
--rw-r--r--   0 Justin     (502) staff       (20)     2594 2022-10-05 21:52:25.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/service.py
--rw-r--r--   0 Justin     (502) staff       (20)     1423 2022-09-29 19:12:44.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute.py
--rw-r--r--   0 Justin     (502) staff       (20)      811 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute_data.py
--rw-r--r--   0 Justin     (502) staff       (20)     1408 2022-09-30 17:03:56.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_asset_data.py
--rw-r--r--   0 Justin     (502) staff       (20)     1902 2022-09-29 19:12:59.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_assets_and_last_values_result.py
--rw-r--r--   0 Justin     (502) staff       (20)     1384 2022-10-05 16:49:01.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_db.py
--rw-r--r--   0 Justin     (502) staff       (20)      732 2022-09-29 19:13:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_dimension.py
--rw-r--r--   0 Justin     (502) staff       (20)      809 2022-09-29 19:11:31.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_generate_query_export_result.py
--rw-r--r--   0 Justin     (502) staff       (20)     3466 2022-09-30 16:48:18.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_input_record.py
--rw-r--r--   0 Justin     (502) staff       (20)      640 2022-09-29 19:17:22.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_measure_value.py
--rw-r--r--   0 Justin     (502) staff       (20)      911 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_publish_input.py
--rw-r--r--   0 Justin     (502) staff       (20)      837 2022-09-29 19:18:29.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_publish_response.py
--rw-r--r--   0 Justin     (502) staff       (20)     1925 2022-09-30 00:39:31.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_query_export.py
--rw-r--r--   0 Justin     (502) staff       (20)     1334 2022-09-29 19:45:45.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_query_result.py
--rw-r--r--   0 Justin     (502) staff       (20)     1602 2022-09-29 19:30:48.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/timestream_query_result.py
--rw-r--r--   0 Justin     (502) staff       (20)     1579 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/user.py
--rw-r--r--   0 Justin     (502) staff       (20)      176 2022-11-21 23:52:33.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/endpointUtil.py
--rw-r--r--   0 Justin     (502) staff       (20)     2597 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/exceptions.py
--rw-r--r--   0 Justin     (502) staff       (20)      460 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/globals.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.180063 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.179651 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.308398 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/
--rw-r--r--   0 Justin     (502) staff       (20)    94862 2023-06-08 22:03:56.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/__init__.py
--rw-r--r--   0 Justin     (502) staff       (20)     7371 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/async_base_client.py
--rw-r--r--   0 Justin     (502) staff       (20)     1951 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/base_model.py
--rw-r--r--   0 Justin     (502) staff       (20)   200424 2023-06-08 22:03:56.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/client.py
--rw-r--r--   0 Justin     (502) staff       (20)    10097 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_add_service_to_collaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     5538 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_get_collaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     7019 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_list_collaborative_member_organization_requests.py
--rw-r--r--   0 Justin     (502) staff       (20)    10164 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_list_collaborative_services.py
--rw-r--r--   0 Justin     (502) staff       (20)     5658 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_list_collaboratives.py
--rw-r--r--   0 Justin     (502) staff       (20)     6603 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_list_collaboratives_service_shared_with.py
--rw-r--r--   0 Justin     (502) staff       (20)    10537 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_remove_service_from_collaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     5561 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_update_collaborative_member_organization.py
--rw-r--r--   0 Justin     (502) staff       (20)      668 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_attach_file.py
--rw-r--r--   0 Justin     (502) staff       (20)     4109 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_create_capture.py
--rw-r--r--   0 Justin     (502) staff       (20)     1005 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_delete_attachment.py
--rw-r--r--   0 Justin     (502) staff       (20)     4109 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_delete_capture.py
--rw-r--r--   0 Justin     (502) staff       (20)     3969 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_capture.py
--rw-r--r--   0 Justin     (502) staff       (20)     1222 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_capture_authentication_token.py
--rw-r--r--   0 Justin     (502) staff       (20)      987 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_data_export_download_url.py
--rw-r--r--   0 Justin     (502) staff       (20)     1899 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_data_model.py
--rw-r--r--   0 Justin     (502) staff       (20)      731 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_data_model_export.py
--rw-r--r--   0 Justin     (502) staff       (20)      857 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_file_attachment_download_url.py
--rw-r--r--   0 Justin     (502) staff       (20)      406 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_python_s_d_k_sample.py
--rw-r--r--   0 Justin     (502) staff       (20)     4281 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_handle_completion.py
--rw-r--r--   0 Justin     (502) staff       (20)     1017 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_list_attachments.py
--rw-r--r--   0 Justin     (502) staff       (20)     4561 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_list_captures.py
--rw-r--r--   0 Justin     (502) staff       (20)     4528 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_notify_capture_complete.py
--rw-r--r--   0 Justin     (502) staff       (20)     1833 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_publish_data.py
--rw-r--r--   0 Justin     (502) staff       (20)     1221 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_regenerate_authentication_token.py
--rw-r--r--   0 Justin     (502) staff       (20)     4063 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_start_capture.py
--rw-r--r--   0 Justin     (502) staff       (20)     4009 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_stop_capture.py
--rw-r--r--   0 Justin     (502) staff       (20)     4109 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_update_capture.py
--rw-r--r--   0 Justin     (502) staff       (20)     2017 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_update_data_model.py
--rw-r--r--   0 Justin     (502) staff       (20)      760 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_upload_data_model_file.py
--rw-r--r--   0 Justin     (502) staff       (20)     3906 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/enums.py
--rw-r--r--   0 Justin     (502) staff       (20)     2366 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/exceptions.py
--rw-r--r--   0 Justin     (502) staff       (20)     5844 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/input_types.py
--rw-r--r--   0 Justin     (502) staff       (20)     2516 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_add_endpoints_to_group.py
--rw-r--r--   0 Justin     (502) staff       (20)      599 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_cancel_query.py
--rw-r--r--   0 Justin     (502) staff       (20)     1762 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_create_endpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     2254 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_create_group.py
--rw-r--r--   0 Justin     (502) staff       (20)      577 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_create_hub.py
--rw-r--r--   0 Justin     (502) staff       (20)     1616 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_create_model.py
--rw-r--r--   0 Justin     (502) staff       (20)     1866 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_create_new_model_version.py
--rw-r--r--   0 Justin     (502) staff       (20)     1762 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_delete_endpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     2254 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_delete_group.py
--rw-r--r--   0 Justin     (502) staff       (20)      577 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_delete_hub.py
--rw-r--r--   0 Justin     (502) staff       (20)     1616 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_delete_model.py
--rw-r--r--   0 Justin     (502) staff       (20)      761 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_generate_query_result_export.py
--rw-r--r--   0 Justin     (502) staff       (20)     1696 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_get_endpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     1004 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_get_endpoint_token.py
--rw-r--r--   0 Justin     (502) staff       (20)     2128 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_get_group.py
--rw-r--r--   0 Justin     (502) staff       (20)      547 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_get_hub.py
--rw-r--r--   0 Justin     (502) staff       (20)     1536 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_get_model.py
--rw-r--r--   0 Justin     (502) staff       (20)      383 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_get_model_in_d_t_d_l_format.py
--rw-r--r--   0 Justin     (502) staff       (20)     2327 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_endpoint_last_values.py
--rw-r--r--   0 Justin     (502) staff       (20)     1896 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_endpoints_in_hub.py
--rw-r--r--   0 Justin     (502) staff       (20)     2228 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_groups.py
--rw-r--r--   0 Justin     (502) staff       (20)     2544 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_groups_endpoints_last_values.py
--rw-r--r--   0 Justin     (502) staff       (20)      603 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_hubs.py
--rw-r--r--   0 Justin     (502) staff       (20)     2488 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_hubs_endpoints_last_values.py
--rw-r--r--   0 Justin     (502) staff       (20)     1610 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_models.py
--rw-r--r--   0 Justin     (502) staff       (20)      830 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_notify_query_export_complete.py
--rw-r--r--   0 Justin     (502) staff       (20)     2275 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_publish.py
--rw-r--r--   0 Justin     (502) staff       (20)      947 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_query_by_time_range.py
--rw-r--r--   0 Justin     (502) staff       (20)     1074 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_regenerate_endpoint_token.py
--rw-r--r--   0 Justin     (502) staff       (20)     2772 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_remove_endpoints_from_group.py
--rw-r--r--   0 Justin     (502) staff       (20)     1762 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_endpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     2055 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_endpoint_properties.py
--rw-r--r--   0 Justin     (502) staff       (20)     2254 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_group.py
--rw-r--r--   0 Justin     (502) staff       (20)      577 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_hub.py
--rw-r--r--   0 Justin     (502) staff       (20)     1616 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_model.py
--rw-r--r--   0 Justin     (502) staff       (20)     2139 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_model_used_by_endpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)      835 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/notifications_notify_upload_complete.py
--rw-r--r--   0 Justin     (502) staff       (20)     1776 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_capture_publish_data.py
--rw-r--r--   0 Justin     (502) staff       (20)     2410 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_iot_publish.py
--rw-r--r--   0 Justin     (502) staff       (20)     4062 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_notify_capture_complete.py
--rw-r--r--   0 Justin     (502) staff       (20)      850 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_notify_iot_query_export_complete.py
--rw-r--r--   0 Justin     (502) staff       (20)      949 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_notify_time_series_query_export_complete.py
--rw-r--r--   0 Justin     (502) staff       (20)      724 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_notify_upload_complete.py
--rw-r--r--   0 Justin     (502) staff       (20)     3635 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_start_capture.py
--rw-r--r--   0 Justin     (502) staff       (20)     3595 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_stop_capture.py
--rw-r--r--   0 Justin     (502) staff       (20)     1407 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_time_series_db_publish.py
--rw-r--r--   0 Justin     (502) staff       (20)     5852 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_add_collaborative_member.py
--rw-r--r--   0 Justin     (502) staff       (20)     5695 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_create_collaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)      782 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_create_organization.py
--rw-r--r--   0 Justin     (502) staff       (20)     1429 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_create_user.py
--rw-r--r--   0 Justin     (502) staff       (20)     5695 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_delete_collaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)      782 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_delete_organization.py
--rw-r--r--   0 Justin     (502) staff       (20)     1429 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_delete_user.py
--rw-r--r--   0 Justin     (502) staff       (20)     6082 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_delete_users_collaboratives.py
--rw-r--r--   0 Justin     (502) staff       (20)     9601 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_delete_users_services.py
--rw-r--r--   0 Justin     (502) staff       (20)     5539 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_get_collaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)      752 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_get_organization.py
--rw-r--r--   0 Justin     (502) staff       (20)     1381 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_get_user.py
--rw-r--r--   0 Justin     (502) staff       (20)     5659 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_list_collaboratives.py
--rw-r--r--   0 Justin     (502) staff       (20)      794 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_list_organizations.py
--rw-r--r--   0 Justin     (502) staff       (20)     1429 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_list_users.py
--rw-r--r--   0 Justin     (502) staff       (20)     6603 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_migrate_users_collaboratives_ownership.py
--rw-r--r--   0 Justin     (502) staff       (20)    10518 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_migrate_users_services_ownership.py
--rw-r--r--   0 Justin     (502) staff       (20)     6014 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_remove_collaborative_member.py
--rw-r--r--   0 Justin     (502) staff       (20)     1610 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_resend_user_invitation.py
--rw-r--r--   0 Justin     (502) staff       (20)     5695 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_update_collaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     6014 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_update_collaborative_member.py
--rw-r--r--   0 Justin     (502) staff       (20)      782 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_update_organization.py
--rw-r--r--   0 Justin     (502) staff       (20)     1429 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_update_user.py
--rw-r--r--   0 Justin     (502) staff       (20)      220 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/scalars.py
--rw-r--r--   0 Justin     (502) staff       (20)      778 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_create_data_store.py
--rw-r--r--   0 Justin     (502) staff       (20)     3907 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_create_data_store_directory.py
--rw-r--r--   0 Justin     (502) staff       (20)      719 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_create_data_store_file.py
--rw-r--r--   0 Justin     (502) staff       (20)     1403 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_create_data_store_file_data_view.py
--rw-r--r--   0 Justin     (502) staff       (20)      778 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_delete_data_store.py
--rw-r--r--   0 Justin     (502) staff       (20)     3907 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_delete_data_store_directory.py
--rw-r--r--   0 Justin     (502) staff       (20)     1321 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_delete_data_store_file.py
--rw-r--r--   0 Justin     (502) staff       (20)     1403 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_delete_data_store_file_data_view.py
--rw-r--r--   0 Justin     (502) staff       (20)      748 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_get_data_store.py
--rw-r--r--   0 Justin     (502) staff       (20)     3775 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_get_data_store_directory.py
--rw-r--r--   0 Justin     (502) staff       (20)     1291 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_get_data_store_file.py
--rw-r--r--   0 Justin     (502) staff       (20)      801 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_get_data_store_file_download_url.py
--rw-r--r--   0 Justin     (502) staff       (20)      791 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_get_data_store_zip_download_url.py
--rw-r--r--   0 Justin     (502) staff       (20)      790 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_list_data_stores.py
--rw-r--r--   0 Justin     (502) staff       (20)      778 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_update_data_store.py
--rw-r--r--   0 Justin     (502) staff       (20)     3907 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_update_data_store_directory.py
--rw-r--r--   0 Justin     (502) staff       (20)     1321 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_update_data_store_file.py
--rw-r--r--   0 Justin     (502) staff       (20)      772 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_cancel_database_query.py
--rw-r--r--   0 Justin     (502) staff       (20)      866 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_create_database.py
--rw-r--r--   0 Justin     (502) staff       (20)      866 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_delete_database.py
--rw-r--r--   0 Justin     (502) staff       (20)      985 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_generate_query_result_export_file.py
--rw-r--r--   0 Justin     (502) staff       (20)      836 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_get_database.py
--rw-r--r--   0 Justin     (502) staff       (20)     2463 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_list_all_asset_last_values.py
--rw-r--r--   0 Justin     (502) staff       (20)      878 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_list_databases.py
--rw-r--r--   0 Justin     (502) staff       (20)     1052 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_notify_time_series_query_export_complete.py
--rw-r--r--   0 Justin     (502) staff       (20)     1695 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_publish_to_database.py
--rw-r--r--   0 Justin     (502) staff       (20)     1015 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_query_database.py
--rw-r--r--   0 Justin     (502) staff       (20)      905 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_query_database_with_timestream_query.py
--rw-r--r--   0 Justin     (502) staff       (20)      866 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_update_database.py
--rw-r--r--   0 Justin     (502) staff       (20)     1104 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/user_create_authentication_token.py
--rw-r--r--   0 Justin     (502) staff       (20)     1104 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/user_delete_authentication_token.py
--rw-r--r--   0 Justin     (502) staff       (20)     1548 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/user_get_user_session.py
--rw-r--r--   0 Justin     (502) staff       (20)     1110 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/user_list_authentication_tokens.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.308881 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/gqlg/
--rw-r--r--   0 Justin     (502) staff       (20)      507 2023-06-08 16:25:42.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/gqlg/condenseQueries.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.316975 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/
--rw-r--r--   0 Justin     (502) staff       (20)     1489 2022-09-29 19:23:24.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_addServiceToCollaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     1469 2022-09-29 19:24:19.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_removeServiceFromCollaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)      329 2023-05-17 16:29:16.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/dataCapture_publishData.py
--rw-r--r--   0 Justin     (502) staff       (20)     1055 2022-12-02 17:40:14.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_cancelQuery.py
--rw-r--r--   0 Justin     (502) staff       (20)     1401 2023-02-15 19:36:31.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_createEndpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     1703 2023-02-14 23:10:32.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_createModel.py
--rw-r--r--   0 Justin     (502) staff       (20)     1333 2022-12-01 20:55:30.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_generateQueryResultExport.py
--rw-r--r--   0 Justin     (502) staff       (20)     1374 2022-11-23 17:59:59.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_publish.py
--rw-r--r--   0 Justin     (502) staff       (20)     1375 2022-11-29 01:46:34.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_updateEndpointProperties.py
--rw-r--r--   0 Justin     (502) staff       (20)     1410 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/mutation.py
--rw-r--r--   0 Justin     (502) staff       (20)     1602 2022-09-29 19:24:48.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/storage_createDataStoreFile.py
--rw-r--r--   0 Justin     (502) staff       (20)     1199 2022-09-29 19:25:14.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/storage_deleteDataStoreFile.py
--rw-r--r--   0 Justin     (502) staff       (20)     1204 2022-09-29 19:25:37.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_cancelDatabaseQuery.py
--rw-r--r--   0 Justin     (502) staff       (20)     1503 2022-09-29 19:25:41.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_generateQueryResultExportFile.py
--rw-r--r--   0 Justin     (502) staff       (20)     1825 2022-09-29 19:22:38.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_publishToDatabase.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.326347 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/
--rw-r--r--   0 Justin     (502) staff       (20)        0 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/__init__.py
--rw-r--r--   0 Justin     (502) staff       (20)     1273 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/collaborative_getCollaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     1470 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativeServices.py
--rw-r--r--   0 Justin     (502) staff       (20)     1247 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaboratives.py
--rw-r--r--   0 Justin     (502) staff       (20)     1776 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativesServiceSharedWith.py
--rw-r--r--   0 Justin     (502) staff       (20)     1205 2022-12-03 00:56:58.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/iot_getEndpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     1779 2022-11-28 19:19:16.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/iot_listEndpointLastValues.py
--rw-r--r--   0 Justin     (502) staff       (20)     2454 2022-12-01 19:24:44.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/iot_queryByTimeRange.py
--rw-r--r--   0 Justin     (502) staff       (20)     1394 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/query.py
--rw-r--r--   0 Justin     (502) staff       (20)     1189 2022-10-05 16:34:47.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStore.py
--rw-r--r--   0 Justin     (502) staff       (20)     1327 2022-10-05 21:54:09.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreDirectory.py
--rw-r--r--   0 Justin     (502) staff       (20)     1264 2022-10-05 21:53:38.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFile.py
--rw-r--r--   0 Justin     (502) staff       (20)     1417 2022-12-20 17:42:57.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFileDownloadUrl.py
--rw-r--r--   0 Justin     (502) staff       (20)     1195 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_listDataStores.py
--rw-r--r--   0 Justin     (502) staff       (20)     1277 2022-09-29 18:46:04.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_getDatabase.py
--rw-r--r--   0 Justin     (502) staff       (20)     1839 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listAllAssetLastValues.py
--rw-r--r--   0 Justin     (502) staff       (20)     1216 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listDatabases.py
--rw-r--r--   0 Justin     (502) staff       (20)     3214 2022-09-30 00:23:31.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabase.py
--rw-r--r--   0 Justin     (502) staff       (20)     2085 2022-09-29 19:12:18.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabaseWithTimestreamQuery.py
--rw-r--r--   0 Justin     (502) staff       (20)     1021 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/user_getUserSession.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.328368 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_subscriptions/
--rw-r--r--   0 Justin     (502) staff       (20)     3353 2022-12-13 17:40:26.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyIotQueryExportComplete.py
--rw-r--r--   0 Justin     (502) staff       (20)     3526 2022-09-29 19:46:08.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyTimeSeriesQueryExportComplete.py
--rw-r--r--   0 Justin     (502) staff       (20)     1486 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_subscriptions/subscription.py
--rw-r--r--   0 Justin     (502) staff       (20)     8438 2023-06-06 23:25:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/iotUtil.py
--rw-r--r--   0 Justin     (502) staff       (20)     1000 2023-06-13 20:20:28.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/logger.py
--rw-r--r--   0 Justin     (502) staff       (20)     6848 2023-01-25 00:06:56.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/subscriptionClient.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.195057 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk.egg-info/
--rw-r--r--   0 Justin     (502) staff       (20)    74798 2023-06-15 18:41:10.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk.egg-info/PKG-INFO
--rw-r--r--   0 Justin     (502) staff       (20)    22060 2023-06-15 18:41:10.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 Justin     (502) staff       (20)        1 2023-06-15 18:41:10.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 Justin     (502) staff       (20)       28 2023-06-15 18:41:10.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.330009 avista_digital_exchange_sdk-0.3.0/tests/
--rw-r--r--   0 Justin     (502) staff       (20)      469 2023-06-15 18:37:15.000000 avista_digital_exchange_sdk-0.3.0/tests/test.py
--rw-r--r--   0 Justin     (502) staff       (20)      162 2023-06-15 16:15:35.000000 avista_digital_exchange_sdk-0.3.0/tests/test_dataCapture_publishData.py
--rw-r--r--   0 Justin     (502) staff       (20)     1599 2023-06-15 18:37:22.000000 avista_digital_exchange_sdk-0.3.0/tests/test_iot_publishData.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 19:09:25.236614 avista_digital_exchange_sdk-0.3.1/
+-rw-r--r--   0 Justin     (502) staff       (20)    35148 2022-09-13 20:02:44.000000 avista_digital_exchange_sdk-0.3.1/LICENSE
+-rw-r--r--   0 Justin     (502) staff       (20)    74798 2023-07-17 19:09:25.236143 avista_digital_exchange_sdk-0.3.1/PKG-INFO
+-rw-r--r--   0 Justin     (502) staff       (20)    33555 2023-06-15 18:40:21.000000 avista_digital_exchange_sdk-0.3.1/README.md
+-rw-r--r--   0 Justin     (502) staff       (20)      936 2023-07-17 19:09:14.000000 avista_digital_exchange_sdk-0.3.1/pyproject.toml
+-rw-r--r--   0 Justin     (502) staff       (20)       38 2023-07-17 19:09:25.236733 avista_digital_exchange_sdk-0.3.1/setup.cfg
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 19:09:25.123790 avista_digital_exchange_sdk-0.3.1/src/
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 19:09:25.132214 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/
+-rw-r--r--   0 Justin     (502) staff       (20)     4950 2023-07-17 17:55:00.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/DxTypes.py
+-rw-r--r--   0 Justin     (502) staff       (20)      213 2023-06-14 18:10:08.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/__init__.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 19:09:25.199066 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/
+-rw-r--r--   0 Justin     (502) staff       (20)    94776 2023-07-17 18:23:29.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/__init__.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1951 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/base_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)   200668 2023-07-17 18:23:29.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/client.py
+-rw-r--r--   0 Justin     (502) staff       (20)    10104 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_add_service_to_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5545 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_get_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     7026 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaborative_member_organization_requests.py
+-rw-r--r--   0 Justin     (502) staff       (20)    10171 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaborative_services.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5665 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaboratives.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6610 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaboratives_service_shared_with.py
+-rw-r--r--   0 Justin     (502) staff       (20)    10544 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_remove_service_from_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5568 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_update_collaborative_member_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)      675 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_attach_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4116 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_create_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1088 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_delete_attachment.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4116 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_delete_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1238 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_active_capture_data_export_download_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3976 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1229 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_capture_authentication_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1100 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_export_download_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1906 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)      738 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_model_export.py
+-rw-r--r--   0 Justin     (502) staff       (20)      864 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_file_attachment_download_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)      413 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_python_s_d_k_sample.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4288 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_handle_completion.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1100 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_list_attachments.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4568 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_list_captures.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4535 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_notify_capture_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1840 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_publish_data.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1228 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_regenerate_authentication_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4070 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_start_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4016 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_stop_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4116 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_update_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2024 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_update_data_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4137 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/enums.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2418 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/exceptions.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5844 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/input_types.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2523 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_add_endpoints_to_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)      606 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_cancel_query.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1769 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2261 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)      584 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_hub.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1623 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1873 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_new_model_version.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1769 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2261 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)      584 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_hub.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1623 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)      768 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_generate_query_result_export.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1703 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1011 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_endpoint_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2135 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)      554 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_hub.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1543 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)      390 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_model_in_d_t_d_l_format.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2334 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_endpoint_last_values.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1903 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_endpoints_in_hub.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2235 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_groups.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2551 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_groups_endpoints_last_values.py
+-rw-r--r--   0 Justin     (502) staff       (20)      610 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_hubs.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2495 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_hubs_endpoints_last_values.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1617 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_models.py
+-rw-r--r--   0 Justin     (502) staff       (20)      837 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_notify_query_export_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2282 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_publish.py
+-rw-r--r--   0 Justin     (502) staff       (20)      954 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_query_by_time_range.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1081 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_regenerate_endpoint_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2779 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_remove_endpoints_from_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1769 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2062 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_endpoint_properties.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2261 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)      584 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_hub.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1623 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2146 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_model_used_by_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     8790 2023-07-17 19:05:03.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/modified_async_base_client.py
+-rw-r--r--   0 Justin     (502) staff       (20)      842 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/notifications_notify_upload_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1783 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_capture_publish_data.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2417 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_iot_publish.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4069 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_capture_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)      857 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_iot_query_export_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)      956 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_time_series_query_export_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)      731 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_upload_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3642 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_start_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3602 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_stop_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1414 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_time_series_db_publish.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5859 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_add_collaborative_member.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5702 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)      789 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1436 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_user.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5702 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)      789 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1436 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_user.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6089 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_users_collaboratives.py
+-rw-r--r--   0 Justin     (502) staff       (20)     9608 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_users_services.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5546 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)      759 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1388 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_user.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5666 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_collaboratives.py
+-rw-r--r--   0 Justin     (502) staff       (20)      801 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_organizations.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1436 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_users.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6610 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_migrate_users_collaboratives_ownership.py
+-rw-r--r--   0 Justin     (502) staff       (20)    10525 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_migrate_users_services_ownership.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6021 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_remove_collaborative_member.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1617 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_resend_user_invitation.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5702 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6021 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_collaborative_member.py
+-rw-r--r--   0 Justin     (502) staff       (20)      789 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1436 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_user.py
+-rw-r--r--   0 Justin     (502) staff       (20)      220 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/scalars.py
+-rw-r--r--   0 Justin     (502) staff       (20)      785 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3914 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_directory.py
+-rw-r--r--   0 Justin     (502) staff       (20)      726 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1410 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_file_data_view.py
+-rw-r--r--   0 Justin     (502) staff       (20)      785 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3914 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_directory.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1328 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1410 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_file_data_view.py
+-rw-r--r--   0 Justin     (502) staff       (20)      755 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3782 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_directory.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1298 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)      808 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_file_download_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)      798 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_zip_download_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)      797 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_list_data_stores.py
+-rw-r--r--   0 Justin     (502) staff       (20)      785 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3914 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store_directory.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1328 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)      779 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_cancel_database_query.py
+-rw-r--r--   0 Justin     (502) staff       (20)      873 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_create_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)      873 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_delete_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)      992 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_generate_query_result_export_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)      843 2023-07-17 18:23:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_get_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2470 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_list_all_asset_last_values.py
+-rw-r--r--   0 Justin     (502) staff       (20)      885 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_list_databases.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1059 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_notify_time_series_query_export_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1702 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_publish_to_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1022 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_query_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)      912 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_query_database_with_timestream_query.py
+-rw-r--r--   0 Justin     (502) staff       (20)      873 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_update_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1111 2023-07-17 18:23:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/user_create_authentication_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1111 2023-07-17 18:23:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/user_delete_authentication_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1555 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/user_get_user_session.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1117 2023-07-17 18:23:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/user_list_authentication_tokens.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1629 2023-07-10 20:54:52.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/avista_digital_exchange.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4712 2023-07-17 17:54:14.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/client.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3384 2022-12-02 17:38:29.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/collaborativeUtil.py
+-rw-r--r--   0 Justin     (502) staff       (20)     7112 2023-07-17 17:55:03.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/dataCaptureUtil.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2784 2022-12-02 17:57:07.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/dataStoreUtil.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 19:09:25.217977 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/
+-rw-r--r--   0 Justin     (502) staff       (20)        0 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/__init__.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1989 2022-09-29 18:39:50.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1630 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/collaborative_member_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)      852 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/collaborative_member_user.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6818 2022-10-10 19:11:23.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/data_store.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6384 2022-12-19 18:46:23.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/data_store_directory.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6657 2022-12-19 18:45:32.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/data_store_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2124 2022-10-05 17:07:09.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/data_store_object.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1751 2023-01-24 17:50:55.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/digital_twin_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1414 2022-12-05 17:33:37.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/endpoint_last_values.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1214 2022-11-28 17:35:44.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/endpoint_property.py
+-rw-r--r--   0 Justin     (502) staff       (20)      990 2022-11-29 01:10:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/endpoint_property_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)      681 2022-11-29 19:31:15.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/endpoint_query_filter_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1020 2022-12-02 19:07:37.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1340 2022-12-03 00:58:02.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry_data_record.py
+-rw-r--r--   0 Justin     (502) staff       (20)      924 2022-12-01 19:36:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_attribute_value.py
+-rw-r--r--   0 Justin     (502) staff       (20)      403 2022-12-09 00:20:12.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_attribute_value_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1175 2022-11-22 17:09:32.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_data_record.py
+-rw-r--r--   0 Justin     (502) staff       (20)      860 2022-11-22 17:17:39.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_data_record_error.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1816 2022-12-19 19:40:35.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_data_record_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1479 2022-11-28 18:00:38.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_data_record_with_errors.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1834 2022-12-03 00:56:11.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1396 2022-11-30 19:33:37.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_endpoint_data.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1807 2022-12-05 17:37:27.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_endpoints_last_values_query_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)      726 2022-12-01 19:24:03.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_generate_query_result_export.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1889 2022-12-13 17:12:23.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_query_by_time_range_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2008 2022-12-13 17:11:14.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_query_export.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1161 2023-01-24 17:48:06.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/model_property.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1795 2023-01-25 00:41:35.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/model_property_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1017 2023-01-24 17:48:35.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/model_telemetry.py
+-rw-r--r--   0 Justin     (502) staff       (20)      984 2023-01-25 00:48:12.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/model_telemetry_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)      785 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)      732 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/presigned_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1521 2022-12-08 19:15:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/publish_iot_data_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)      727 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/server_response.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2594 2022-10-05 21:52:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/service.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1423 2022-09-29 19:12:44.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute.py
+-rw-r--r--   0 Justin     (502) staff       (20)      811 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute_data.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1408 2022-09-30 17:03:56.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_asset_data.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1902 2022-09-29 19:12:59.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_assets_and_last_values_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1384 2022-10-05 16:49:01.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_db.py
+-rw-r--r--   0 Justin     (502) staff       (20)      732 2022-09-29 19:13:54.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_dimension.py
+-rw-r--r--   0 Justin     (502) staff       (20)      809 2022-09-29 19:11:31.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_generate_query_export_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3466 2022-09-30 16:48:18.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_input_record.py
+-rw-r--r--   0 Justin     (502) staff       (20)      640 2022-09-29 19:17:22.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_measure_value.py
+-rw-r--r--   0 Justin     (502) staff       (20)      911 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_publish_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)      837 2022-09-29 19:18:29.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_publish_response.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1925 2022-09-30 00:39:31.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_query_export.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1334 2022-09-29 19:45:45.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_query_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1602 2022-09-29 19:30:48.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/timestream_query_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1579 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/user.py
+-rw-r--r--   0 Justin     (502) staff       (20)      176 2022-11-21 23:52:33.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/endpointUtil.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2597 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/exceptions.py
+-rw-r--r--   0 Justin     (502) staff       (20)      460 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/globals.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 19:09:25.224593 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/
+-rw-r--r--   0 Justin     (502) staff       (20)     1489 2022-09-29 19:23:24.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_addServiceToCollaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1469 2022-09-29 19:24:19.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_removeServiceFromCollaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)      329 2023-05-17 16:29:16.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/dataCapture_publishData.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1055 2022-12-02 17:40:14.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_cancelQuery.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1401 2023-02-15 19:36:31.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_createEndpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1703 2023-02-14 23:10:32.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_createModel.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1333 2022-12-01 20:55:30.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_generateQueryResultExport.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1374 2022-11-23 17:59:59.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_publish.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1375 2022-11-29 01:46:34.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_updateEndpointProperties.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1410 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/mutation.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1602 2022-09-29 19:24:48.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/storage_createDataStoreFile.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1199 2022-09-29 19:25:14.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/storage_deleteDataStoreFile.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1204 2022-09-29 19:25:37.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_cancelDatabaseQuery.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1503 2022-09-29 19:25:41.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_generateQueryResultExportFile.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1825 2022-09-29 19:22:38.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_publishToDatabase.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 19:09:25.232264 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/
+-rw-r--r--   0 Justin     (502) staff       (20)        0 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/__init__.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1273 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/collaborative_getCollaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1470 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativeServices.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1247 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaboratives.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1776 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativesServiceSharedWith.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1205 2022-12-03 00:56:58.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/iot_getEndpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1779 2022-11-28 19:19:16.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/iot_listEndpointLastValues.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2454 2022-12-01 19:24:44.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/iot_queryByTimeRange.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1394 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/query.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1189 2022-10-05 16:34:47.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStore.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1327 2022-10-05 21:54:09.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreDirectory.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1264 2022-10-05 21:53:38.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFile.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1417 2022-12-20 17:42:57.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFileDownloadUrl.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1195 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/storage_listDataStores.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1277 2022-09-29 18:46:04.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_getDatabase.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1839 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listAllAssetLastValues.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1216 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listDatabases.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3214 2022-09-30 00:23:31.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabase.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2085 2022-09-29 19:12:18.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabaseWithTimestreamQuery.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1021 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/user_getUserSession.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 19:09:25.233578 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_subscriptions/
+-rw-r--r--   0 Justin     (502) staff       (20)     3353 2022-12-13 17:40:26.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyIotQueryExportComplete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3526 2022-09-29 19:46:08.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyTimeSeriesQueryExportComplete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1486 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_subscriptions/subscription.py
+-rw-r--r--   0 Justin     (502) staff       (20)     8418 2023-07-17 17:09:02.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/iotUtil.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1000 2023-06-13 20:20:28.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/logger.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6848 2023-07-14 23:41:31.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/subscriptionClient.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 19:09:25.134388 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk.egg-info/
+-rw-r--r--   0 Justin     (502) staff       (20)    74798 2023-07-17 19:09:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 Justin     (502) staff       (20)    19498 2023-07-17 19:09:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 Justin     (502) staff       (20)        1 2023-07-17 19:09:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 Justin     (502) staff       (20)       28 2023-07-17 19:09:25.000000 avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-07-17 19:09:25.235312 avista_digital_exchange_sdk-0.3.1/tests/
+-rw-r--r--   0 Justin     (502) staff       (20)      711 2023-07-17 18:43:02.000000 avista_digital_exchange_sdk-0.3.1/tests/test.py
+-rw-r--r--   0 Justin     (502) staff       (20)      162 2023-06-15 16:15:35.000000 avista_digital_exchange_sdk-0.3.1/tests/test_dataCapture_publishData.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1541 2023-06-27 21:36:07.000000 avista_digital_exchange_sdk-0.3.1/tests/test_iot_publishData.py
```

### Comparing `avista_digital_exchange_sdk-0.3.0/LICENSE` & `avista_digital_exchange_sdk-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/PKG-INFO` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: avista_digital_exchange_sdk
-Version: 0.3.0
+Name: avista-digital-exchange-sdk
+Version: 0.3.1
 Summary: SDK to programmatically access the Avista Digital Exchange
 Author-email: Justin Whicker <jwhicker@urbanova.org>, Jon Thompson <jon.thompson@avistacorp.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `avista_digital_exchange_sdk-0.3.0/README.md` & `avista_digital_exchange_sdk-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/pyproject.toml` & `avista_digital_exchange_sdk-0.3.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0","websocket-client","requests", "py-graphql-mapper", "ariadne-codegen"] # , "pip-system-certs"
+requires = ["setuptools>=61.0","requests","requests", "httpx", "pydantic==1.10.8", "certifi", "websockets"] #  "py-graphql-mapper", "pip-system-certs"
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "avista_digital_exchange_sdk"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Justin Whicker", email="jwhicker@urbanova.org"},
   {  name="Jon Thompson", email="jon.thompson@avistacorp.com" }
 ]
 description = "SDK to programmatically access the Avista Digital Exchange"
 readme = "README.md"
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/DxTypes.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/DxTypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from enum import Enum
 import json
 from typing import List
 
-from .graphql_codegen.ariadne.graphql_client.data_capture_publish_data import DataCapturePublishDataDataCapturePublishData
+from .async_graphql_client.data_capture_publish_data import DataCapturePublishDataDataCapturePublishData
 
 
 class TimeUnitEnum(Enum):
     MILLISECONDS = 1
 
 
 class DxTypeBaseClass(object):
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/avista_digital_exchange.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/avista_digital_exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class AvistaDigitalExchange(object):
 
     def __init__(self, token, debug=False):
         if type(debug) is not bool:
             raise InvalidParameterException(
                 "AvistaDigitalExchange debug parameter must be a bool")
-        self._stage: str = "PRODUCTION"
+        self._stage: str = "DEVELOPMENT"
         self._debug: bool = debug
         self._token: str = token
         self._client: Client = Client(self._token, self._stage, self._debug)
         self._logger: Logger = logging.getLogger(name="dx-logger")
         self._logger.setLevel(20)
         self.iot: IoTUtil = IoTUtil(self._debug, self._client)
         # self.collaboratives = CollaborativeUtil(self._debug, self._client)
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/client.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,63 @@
+import json
+from base64 import b64encode, decode
 import requests
 from . import globals
 from .subscriptionClient import Subscription
-from .graphql_codegen.ariadne.graphql_client.client import Client as AriadneGraphqlClient
+from .async_graphql_client.client import Client as GeneratedGraphqlClient
 
 
 class Client:
-    updatedGqlClient: AriadneGraphqlClient
+    updatedGqlClient: GeneratedGraphqlClient
 
     def __init__(self, token, stage, debug):
         APPSYNC_API_ENDPOINT_URL_dev = 'https://annsvlcb4vew7msipwjyzzvyhi.appsync-api.us-west-2.amazonaws.com/graphql'
         APPSYNC_API_ENDPOINT_URL_prod = 'https://rrfs7pb7ancybo7bom7uxcsaxq.appsync-api.us-west-2.amazonaws.com/graphql'
+
         self.token = token
         self._debug = debug
         self._stage = stage
         if self._stage == "PRODUCTION":
             self.APPSYNC_API_ENDPOINT_URL = APPSYNC_API_ENDPOINT_URL_prod
         else:
             self.APPSYNC_API_ENDPOINT_URL = APPSYNC_API_ENDPOINT_URL_dev
+
+        self.APPSYNC_API_WS_URL = self.APPSYNC_API_ENDPOINT_URL.replace(
+            'https', 'wss').replace('appsync-api', 'appsync-realtime-api')
+        self.APPSYNC_HOST = self.APPSYNC_API_ENDPOINT_URL.replace(
+            'https://', '').replace('/graphql', '')
         self.setupUpdatedGqlClient()
         return
 
     def setupUpdatedGqlClient(self):
         import httpx
         headers = {'Accept': 'application/json',
                    'Content-Type': 'application/json',
-                   'Authorization': self.token}
-        self.updatedGqlClient = AriadneGraphqlClient(url=self.APPSYNC_API_ENDPOINT_URL,
-                                                     headers=headers,
-                                                     http_client=httpx.AsyncClient(headers=headers, timeout=60))
+                   'Authorization': self.token, }
+        wsHeaders = {
+            'Authorization': self.token,
+            'HOST': self.APPSYNC_HOST}
+        wsExtensions = {'authorization': {
+            'host': self.APPSYNC_HOST,
+            'Authorization': self.token
+        }}
+
+        # ssl._create_default_https_context = ssl._create_unverified_context
+        print(self.APPSYNC_API_ENDPOINT_URL)
+        print(self.APPSYNC_API_WS_URL)
+        self.updatedGqlClient = GeneratedGraphqlClient(url=self.APPSYNC_API_ENDPOINT_URL,
+                                                       ws_url="wss://annsvlcb4vew7msipwjyzzvyhi.appsync-realtime-api.us-west-2.amazonaws.com/graphql"
+                                                       + '?header=' +
+                                                       headerEncode(
+                                                         wsHeaders) + '&payload=e30=',
+                                                       #  ws_headers=wsHeaders,
+                                                       #  ws_origin=self.APPSYNC_HOST,
+                                                       ws_extensions=wsExtensions,
+                                                       headers=headers,
+                                                       http_client=httpx.AsyncClient(headers=headers, timeout=60))
 
     def performQuery(self, queryString):
         if self._debug:
             print(f'DEBUG - {queryString}')
         response = None
 
         try:
@@ -73,7 +99,11 @@
 
     def getSubscriptionClient(self, subscriptionName, subscriptionQueryString, subscriptionMessageQueue, subscriptionErrorQueue):
         if self._debug:
             print(f'subscribing to {subscriptionQueryString}...')
         subscription = Subscription(
             self._debug, subscriptionName, subscriptionQueryString, self.APPSYNC_API_ENDPOINT_URL, self.token, subscriptionMessageQueue, subscriptionErrorQueue)
         return subscription
+
+
+def headerEncode(header_obj):
+    return b64encode(json.dumps(header_obj).encode('utf-8')).decode('utf-8')
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/collaborativeUtil.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/collaborativeUtil.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/dataCaptureUtil.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/dataCaptureUtil.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 
 from logging import Logger
 from typing import List
-from .graphql_codegen.ariadne.graphql_client import exceptions, input_types
+from .async_graphql_client import exceptions, input_types
 from .client import Client as DxClient
 from . import DxTypes
 
 
 class DataCaptureUtil(object):
     _debug: bool
     _client: DxClient
     _logger: Logger
 
     def __init__(self, debug: bool, client: DxClient, logger: Logger):
         self._debug = debug
         self._client = client
         self._logger = logger
 
+    async def listenForCaptureData(self, captureId: str):
+        print("Subscribing to capture data....")
+        async for item in self._client.updatedGqlClient.on_capture_publish_data(
+                capture_id=captureId):
+            print("In for loop...")
+            print("Subscription item....")
+            print(item)
+
     async def publishData(self, captureId: str, data: List[DxTypes.CaptureDataRecordInput]) -> DxTypes.PublishCaptureDataResult:
         if self._debug:
             print("DataCapture.publishData: - processing data input")
 
         # Format data records argument
         dataRecords: List[input_types.DataCaptureDataRecordInput] = []
         for record in data:
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/dataStoreUtil.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/dataStoreUtil.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/collaborative.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/collaborative.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/collaborative_member_organization.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/collaborative_member_organization.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/collaborative_member_user.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/collaborative_member_user.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/data_store.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/data_store.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/data_store_directory.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/data_store_directory.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/data_store_file.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/data_store_file.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/data_store_object.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/data_store_object.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/digital_twin_model.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/digital_twin_model.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_last_values.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/endpoint_last_values.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_property.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/endpoint_property.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_property_input.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/endpoint_property_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_query_filter_input.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/endpoint_query_filter_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry_data_record.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry_data_record.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_attribute_value.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_attribute_value.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_data_record.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_data_record.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_data_record_error.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_data_record_error.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_data_record_input.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_data_record_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_data_record_with_errors.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_data_record_with_errors.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_endpoint.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_endpoint.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_endpoint_data.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_endpoint_data.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_endpoints_last_values_query_result.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_endpoints_last_values_query_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_generate_query_result_export.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_generate_query_result_export.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_query_by_time_range_result.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_query_by_time_range_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_query_export.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/iot_query_export.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/model_property.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/model_property.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/model_property_input.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/model_property_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/model_telemetry.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/model_telemetry.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/model_telemetry_input.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/model_telemetry_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/organization.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/organization.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/presigned_url.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/presigned_url.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/publish_iot_data_result.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/publish_iot_data_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/server_response.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/server_response.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/service.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/service.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute_data.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute_data.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_asset_data.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_asset_data.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_assets_and_last_values_result.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_assets_and_last_values_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_db.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_db.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_dimension.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_dimension.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_generate_query_export_result.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_generate_query_export_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_input_record.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_input_record.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_measure_value.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_measure_value.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_publish_input.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_publish_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_publish_response.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_publish_response.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_query_export.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_query_export.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_query_result.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/time_series_query_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/timestream_query_result.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/timestream_query_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/user.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/data_types/user.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/exceptions.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/__init__.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
+# Generated by ariadne-codegen on 2023-07-17 11:23
 
-from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel
 from .client import Client
 from .collaborative_add_service_to_collaborative import (
     CollaborativeAddServiceToCollaborative,
     CollaborativeAddServiceToCollaborativeCollaborativeAddServiceToCollaborative,
     CollaborativeAddServiceToCollaborativeCollaborativeAddServiceToCollaborativeDataCapture,
     CollaborativeAddServiceToCollaborativeCollaborativeAddServiceToCollaborativeDataCaptureDataModel,
@@ -130,14 +129,18 @@
     DataCaptureDeleteCaptureDataCaptureDeleteCapture,
     DataCaptureDeleteCaptureDataCaptureDeleteCaptureDataModel,
     DataCaptureDeleteCaptureDataCaptureDeleteCaptureDataModelItems,
     DataCaptureDeleteCaptureDataCaptureDeleteCaptureDataModelItemsAttributes,
     DataCaptureDeleteCaptureDataCaptureDeleteCaptureStateHistory,
     DataCaptureDeleteCaptureDataCaptureDeleteCaptureTimeSettings,
 )
+from .data_capture_get_active_capture_data_export_download_url import (
+    DataCaptureGetActiveCaptureDataExportDownloadUrl,
+    DataCaptureGetActiveCaptureDataExportDownloadUrlDataCaptureGetActiveCaptureDataExportDownloadUrl,
+)
 from .data_capture_get_capture import (
     DataCaptureGetCapture,
     DataCaptureGetCaptureDataCaptureGetCapture,
     DataCaptureGetCaptureDataCaptureGetCaptureDataModel,
     DataCaptureGetCaptureDataCaptureGetCaptureDataModelItems,
     DataCaptureGetCaptureDataCaptureGetCaptureDataModelItemsAttributes,
     DataCaptureGetCaptureDataCaptureGetCaptureStateHistory,
@@ -238,27 +241,25 @@
 )
 from .data_capture_update_data_model import (
     DataCaptureUpdateDataModel,
     DataCaptureUpdateDataModelDataCaptureUpdateDataModel,
     DataCaptureUpdateDataModelDataCaptureUpdateDataModelItems,
     DataCaptureUpdateDataModelDataCaptureUpdateDataModelItemsAttributes,
 )
-from .data_capture_upload_data_model_file import (
-    DataCaptureUploadDataModelFile,
-    DataCaptureUploadDataModelFileDataCaptureUploadDataModelFile,
-)
 from .enums import (
     AuthenticationTokenType,
     CaptureSortBy,
     CollaborativeMemberOrganizationState,
     CollaborativeMemberPermission,
     DataCaptureAssetAttributeSchemaType,
     DataCaptureAssetAttributeType,
+    DataCaptureAttachmentError,
     DataCaptureAttachmentType,
     DataCaptureDataExportState,
+    DataCaptureDataExportType,
     DataCaptureDataModelState,
     DataCaptureRecordError,
     DataCaptureState,
     DataCaptureTimeConfigType,
     DataCaptureTimeConfigurationState,
     DataCaptureType,
     DataStoreObjectType,
@@ -272,21 +273,14 @@
     ServiceType,
     TimeSeriesDbQueryType,
     TimeSeriesQueryOutputFileType,
     TimeUnit,
     UserAccountState,
     UserRole,
 )
-from .exceptions import (
-    GraphQLClientError,
-    GraphQLClientGraphQLError,
-    GraphQLClientGraphQLMultiError,
-    GraphQLClientHttpError,
-    GraphQlClientInvalidResponseError,
-)
 from .input_types import (
     DataCaptureAssetAttributeInput,
     DataCaptureAssetInput,
     DataCaptureAttributeValueInput,
     DataCaptureDataModelInput,
     DataCaptureDataRecordInput,
     DataStoreObjectIdInput,
@@ -486,14 +480,15 @@
 )
 from .iot_update_model_used_by_endpoint import (
     IotUpdateModelUsedByEndpoint,
     IotUpdateModelUsedByEndpointIotUpdateModelUsedByEndpoint,
     IotUpdateModelUsedByEndpointIotUpdateModelUsedByEndpointProperties,
     IotUpdateModelUsedByEndpointIotUpdateModelUsedByEndpointTelemetry,
 )
+from .modified_async_base_client import AsyncBaseClient
 from .notifications_notify_upload_complete import (
     NotificationsNotifyUploadComplete,
     NotificationsNotifyUploadCompleteNotificationsNotifyUploadComplete,
 )
 from .on_capture_publish_data import (
     OnCapturePublishData,
     OnCapturePublishDataOnCapturePublishData,
@@ -1005,36 +1000,40 @@
     "CollaborativeUpdateCollaborativeMemberOrganizationCollaborativeUpdateCollaborativeMemberOrganizationUsersInCollaborativeUserOrganization",
     "DataCaptureAssetAttributeInput",
     "DataCaptureAssetAttributeSchemaType",
     "DataCaptureAssetAttributeType",
     "DataCaptureAssetInput",
     "DataCaptureAttachFile",
     "DataCaptureAttachFileDataCaptureAttachFile",
+    "DataCaptureAttachmentError",
     "DataCaptureAttachmentType",
     "DataCaptureAttributeValueInput",
     "DataCaptureCreateCapture",
     "DataCaptureCreateCaptureDataCaptureCreateCapture",
     "DataCaptureCreateCaptureDataCaptureCreateCaptureDataModel",
     "DataCaptureCreateCaptureDataCaptureCreateCaptureDataModelItems",
     "DataCaptureCreateCaptureDataCaptureCreateCaptureDataModelItemsAttributes",
     "DataCaptureCreateCaptureDataCaptureCreateCaptureStateHistory",
     "DataCaptureCreateCaptureDataCaptureCreateCaptureTimeSettings",
     "DataCaptureDataExportState",
+    "DataCaptureDataExportType",
     "DataCaptureDataModelInput",
     "DataCaptureDataModelState",
     "DataCaptureDataRecordInput",
     "DataCaptureDeleteAttachment",
     "DataCaptureDeleteAttachmentDataCaptureDeleteAttachment",
     "DataCaptureDeleteCapture",
     "DataCaptureDeleteCaptureDataCaptureDeleteCapture",
     "DataCaptureDeleteCaptureDataCaptureDeleteCaptureDataModel",
     "DataCaptureDeleteCaptureDataCaptureDeleteCaptureDataModelItems",
     "DataCaptureDeleteCaptureDataCaptureDeleteCaptureDataModelItemsAttributes",
     "DataCaptureDeleteCaptureDataCaptureDeleteCaptureStateHistory",
     "DataCaptureDeleteCaptureDataCaptureDeleteCaptureTimeSettings",
+    "DataCaptureGetActiveCaptureDataExportDownloadUrl",
+    "DataCaptureGetActiveCaptureDataExportDownloadUrlDataCaptureGetActiveCaptureDataExportDownloadUrl",
     "DataCaptureGetCapture",
     "DataCaptureGetCaptureAuthenticationToken",
     "DataCaptureGetCaptureAuthenticationTokenDataCaptureGetCaptureAuthenticationToken",
     "DataCaptureGetCaptureDataCaptureGetCapture",
     "DataCaptureGetCaptureDataCaptureGetCaptureDataModel",
     "DataCaptureGetCaptureDataCaptureGetCaptureDataModelItems",
     "DataCaptureGetCaptureDataCaptureGetCaptureDataModelItemsAttributes",
@@ -1108,27 +1107,20 @@
     "DataCaptureUpdateCaptureDataCaptureUpdateCaptureDataModelItemsAttributes",
     "DataCaptureUpdateCaptureDataCaptureUpdateCaptureStateHistory",
     "DataCaptureUpdateCaptureDataCaptureUpdateCaptureTimeSettings",
     "DataCaptureUpdateDataModel",
     "DataCaptureUpdateDataModelDataCaptureUpdateDataModel",
     "DataCaptureUpdateDataModelDataCaptureUpdateDataModelItems",
     "DataCaptureUpdateDataModelDataCaptureUpdateDataModelItemsAttributes",
-    "DataCaptureUploadDataModelFile",
-    "DataCaptureUploadDataModelFileDataCaptureUploadDataModelFile",
     "DataStoreObjectIdInput",
     "DataStoreObjectType",
     "DimensionValueType",
     "EndpointPropertyInput",
     "EndpointQueryFilter",
     "ExportFileFormat",
-    "GraphQLClientError",
-    "GraphQLClientGraphQLError",
-    "GraphQLClientGraphQLMultiError",
-    "GraphQLClientHttpError",
-    "GraphQlClientInvalidResponseError",
     "IotAddEndpointsToGroup",
     "IotAddEndpointsToGroupIotAddEndpointsToGroup",
     "IotAddEndpointsToGroupIotAddEndpointsToGroupEndpoints",
     "IotAddEndpointsToGroupIotAddEndpointsToGroupEndpointsProperties",
     "IotAddEndpointsToGroupIotAddEndpointsToGroupEndpointsTelemetry",
     "IotAttributeValueInput",
     "IotCancelQuery",
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/async_base_client.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/modified_async_base_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+# Generated by ariadne-codegen on 2023-07-17 11:23
+
 # Generated by ariadne-codegen on 2023-06-08 15:03
 
+from typing import Any, Dict, List, Optional, Union
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
+import signal
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
 
 from .base_model import UNSET
 from .exceptions import (
@@ -22,59 +26,67 @@
     from websockets.client import connect as ws_connect
     from websockets.typing import Data, Origin, Subprotocol
 except ImportError:
     from contextlib import asynccontextmanager
 
     @asynccontextmanager  # type: ignore
     async def ws_connect(*args, **kwargs):  # pylint: disable=unused-argument
-        raise NotImplementedError("Subscriptions require 'websockets' package.")
+        raise NotImplementedError(
+            "Subscriptions require 'websockets' package.")
         yield  # pylint: disable=unreachable
 
     WebSocketClientProtocol = Any  # type: ignore
     Data = Any  # type: ignore
     Origin = Any  # type: ignore
     Subprotocol = Any  # type: ignore
 
 
 Self = TypeVar("Self", bound="AsyncBaseClient")
 
-GRAPHQL_TRANSPORT_WS = "graphql-transport-ws"
+GRAPHQL_TRANSPORT_WS = "graphql-ws"
 
 
 class GraphQLTransportWSMessageType(str, enum.Enum):
     CONNECTION_INIT = "connection_init"
     CONNECTION_ACK = "connection_ack"
     PING = "ping"
     PONG = "pong"
     SUBSCRIBE = "subscribe"
     NEXT = "next"
     ERROR = "error"
     COMPLETE = "complete"
+    KA = "ka"
+    START = "start"
+    START_ACK = "start_ack"
+    DATA = "data"
+    STOP = "stop"
 
 
 class AsyncBaseClient:
     def __init__(
         self,
         url: str = "",
         headers: Optional[Dict[str, str]] = None,
         http_client: Optional[httpx.AsyncClient] = None,
         ws_url: str = "",
         ws_headers: Optional[Dict[str, Any]] = None,
         ws_origin: Optional[str] = None,
         ws_connection_init_payload: Optional[Dict[str, Any]] = None,
+        ws_extensions: Optional[Dict[str, Any]] = None
     ) -> None:
         self.url = url
         self.headers = headers
         self.http_client = (
             http_client if http_client else httpx.AsyncClient(headers=headers)
         )
         self.ws_url = ws_url
         self.ws_headers = ws_headers or {}
         self.ws_origin = Origin(ws_origin) if ws_origin else None
         self.ws_connection_init_payload = ws_connection_init_payload
+        self.ws_extensions = ws_extensions
 
     async def __aenter__(self: Self) -> Self:
         return self
 
     async def __aexit__(
         self,
         exc_type: object,
@@ -84,18 +96,20 @@
         await self.http_client.aclose()
 
     async def execute(
         self, query: str, variables: Optional[Dict[str, Any]] = None
     ) -> httpx.Response:
         payload: Dict[str, Any] = {"query": query}
         if variables:
-            payload["variables"] = self._convert_dict_to_json_serializable(variables)
+            payload["variables"] = self._convert_dict_to_json_serializable(
+                variables)
         content = json.dumps(payload, default=pydantic_encoder)
         return await self.http_client.post(
-            url=self.url, content=content, headers={"Content-Type": "application/json"}
+            url=self.url, content=content, headers={
+                "Content-Type": "application/json"}
         )
 
     def get_data(self, response: httpx.Response) -> Dict[str, Any]:
         if not response.is_success:
             raise GraphQLClientHttpError(
                 status_code=response.status_code, response=response
             )
@@ -118,30 +132,41 @@
 
         return cast(dict[str, Any], data)
 
     async def execute_ws(
         self, query: str, variables: Optional[Dict[str, Any]] = None
     ) -> AsyncIterator[Dict[str, Any]]:
         operation_id = str(uuid4())
+
         async with ws_connect(
             self.ws_url,
-            subprotocols=[Subprotocol(GRAPHQL_TRANSPORT_WS)],
+            subprotocols=["graphql-ws"],
             origin=self.ws_origin,
             extra_headers=self.ws_headers,
         ) as websocket:
+            def quitHandler(signum, frame):
+                # Stop subscription on terminate
+                print("Cancelling data subscription....")
+                self._send_stop(websocket=websocket, operation_id=operation_id)
+                exit()
+
+            signal.signal(signal.SIGINT, quitHandler)
+
             await self._send_connection_init(websocket)
+
             await self._send_subscribe(
                 websocket,
                 operation_id=operation_id,
                 query=query,
                 variables=variables,
             )
 
             async for message in websocket:
                 data = await self._handle_ws_message(message, websocket)
+                print(data)
                 if data:
                     yield data
 
     def _convert_dict_to_json_serializable(
         self, dict_: Dict[str, Any]
     ) -> Dict[str, Any]:
         return {
@@ -170,21 +195,36 @@
         websocket: WebSocketClientProtocol,
         operation_id: str,
         query: str,
         variables: Optional[Dict[str, Any]] = None,
     ) -> None:
         payload: Dict[str, Any] = {
             "id": operation_id,
-            "type": GraphQLTransportWSMessageType.SUBSCRIBE.value,
-            "payload": {"query": query},
+            "type": GraphQLTransportWSMessageType.START.value,
+            "payload": {
+                "data": json.dumps({
+                    "query": query,
+                    "variables":
+                        variables,
+                    "operationName": "onCapturePublishData"
+                }),
+                "extensions": self.ws_extensions
+            },
+        }
+        await websocket.send(json.dumps(payload))
+
+    async def _send_stop(
+        self,
+        websocket: WebSocketClientProtocol,
+        operation_id: str
+    ) -> None:
+        payload: Dict[str, Any] = {
+            "id": operation_id,
+            "type": GraphQLTransportWSMessageType.STOP.value,
         }
-        if variables:
-            payload["payload"]["variables"] = self._convert_dict_to_json_serializable(
-                variables
-            )
         await websocket.send(json.dumps(payload))
 
     async def _handle_ws_message(
         self, message: Data, websocket: WebSocketClientProtocol
     ) -> Optional[Dict[str, Any]]:
         try:
             message_dict = json.loads(message)
@@ -193,24 +233,31 @@
 
         type_ = message_dict.get("type")
         payload = message_dict.get("payload", {})
 
         if not type_ or type_ not in {t.value for t in GraphQLTransportWSMessageType}:
             raise GraphQLClientInvalidMessageFormat(message=message)
 
+        if type_ == GraphQLTransportWSMessageType.KA:
+            print("ka message received")
+        elif type_ == GraphQLTransportWSMessageType.DATA:
+            print("data message received")
+            return cast(Dict[str, Any], payload["data"])
+        elif type_ == GraphQLTransportWSMessageType.ERROR:
+            print("error message received")
+            raise GraphQLClientGraphQLMultiError.from_errors_dicts(
+                errors_dicts=payload, data=message_dict
+            )
+        return None
         if type_ == GraphQLTransportWSMessageType.NEXT:
             if "data" not in payload:
                 raise GraphQLClientInvalidMessageFormat(message=message)
             return cast(Dict[str, Any], payload["data"])
 
         if type_ == GraphQLTransportWSMessageType.COMPLETE:
             await websocket.close()
         elif type_ == GraphQLTransportWSMessageType.PING:
             await websocket.send(
                 json.dumps({"type": GraphQLTransportWSMessageType.PONG.value})
             )
-        elif type_ == GraphQLTransportWSMessageType.ERROR:
-            raise GraphQLClientGraphQLMultiError.from_errors_dicts(
-                errors_dicts=payload, data=message_dict
-            )
 
         return None
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/base_model.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
+# Generated by ariadne-codegen on 2023-07-17 11:23
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/client.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import AsyncIterator, List, Optional, Union
 
-from .async_base_client import AsyncBaseClient
 from .base_model import UNSET, UnsetType
 from .collaborative_add_service_to_collaborative import (
     CollaborativeAddServiceToCollaborative,
 )
 from .collaborative_get_collaborative import CollaborativeGetCollaborative
 from .collaborative_list_collaborative_member_organization_requests import (
     CollaborativeListCollaborativeMemberOrganizationRequests,
@@ -25,14 +24,17 @@
 from .collaborative_update_collaborative_member_organization import (
     CollaborativeUpdateCollaborativeMemberOrganization,
 )
 from .data_capture_attach_file import DataCaptureAttachFile
 from .data_capture_create_capture import DataCaptureCreateCapture
 from .data_capture_delete_attachment import DataCaptureDeleteAttachment
 from .data_capture_delete_capture import DataCaptureDeleteCapture
+from .data_capture_get_active_capture_data_export_download_url import (
+    DataCaptureGetActiveCaptureDataExportDownloadUrl,
+)
 from .data_capture_get_capture import DataCaptureGetCapture
 from .data_capture_get_capture_authentication_token import (
     DataCaptureGetCaptureAuthenticationToken,
 )
 from .data_capture_get_data_export_download_url import (
     DataCaptureGetDataExportDownloadUrl,
 )
@@ -50,15 +52,14 @@
 from .data_capture_regenerate_authentication_token import (
     DataCaptureRegenerateAuthenticationToken,
 )
 from .data_capture_start_capture import DataCaptureStartCapture
 from .data_capture_stop_capture import DataCaptureStopCapture
 from .data_capture_update_capture import DataCaptureUpdateCapture
 from .data_capture_update_data_model import DataCaptureUpdateDataModel
-from .data_capture_upload_data_model_file import DataCaptureUploadDataModelFile
 from .enums import (
     CollaborativeMemberOrganizationState,
     CollaborativeMemberPermission,
     DataCaptureTimeConfigType,
     DataCaptureType,
     ExportFileFormat,
     ServiceType,
@@ -111,14 +112,15 @@
 from .iot_remove_endpoints_from_group import IotRemoveEndpointsFromGroup
 from .iot_update_endpoint import IotUpdateEndpoint
 from .iot_update_endpoint_properties import IotUpdateEndpointProperties
 from .iot_update_group import IotUpdateGroup
 from .iot_update_hub import IotUpdateHub
 from .iot_update_model import IotUpdateModel
 from .iot_update_model_used_by_endpoint import IotUpdateModelUsedByEndpoint
+from .modified_async_base_client import AsyncBaseClient
 from .notifications_notify_upload_complete import NotificationsNotifyUploadComplete
 from .on_capture_publish_data import OnCapturePublishData
 from .on_iot_publish import OnIotPublish
 from .on_notify_capture_complete import OnNotifyCaptureComplete
 from .on_notify_iot_query_export_complete import OnNotifyIotQueryExportComplete
 from .on_notify_time_series_query_export_complete import (
     OnNotifyTimeSeriesQueryExportComplete,
@@ -3283,47 +3285,29 @@
             mutation dataCapture_deleteAttachment($attachmentId: ID!, $captureId: ID!) {
               dataCapture_deleteAttachment(attachmentId: $attachmentId, captureId: $captureId) {
                 attachmentId
                 attachmentType
                 dateCreated
                 dateUpdated
                 description
+                error
                 name
                 ownerUserId
               }
             }
             """
         )
         variables: dict[str, object] = {
             "attachmentId": attachment_id,
             "captureId": capture_id,
         }
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return DataCaptureDeleteAttachment.parse_obj(data)
 
-    async def data_capture_upload_data_model_file(
-        self, capture_id: str, file_name: str
-    ) -> DataCaptureUploadDataModelFile:
-        query = gql(
-            """
-            mutation dataCapture_uploadDataModelFile($captureId: ID!, $fileName: String!) {
-              dataCapture_uploadDataModelFile(captureId: $captureId, fileName: $fileName) {
-                itemId
-                uploadId
-                url
-              }
-            }
-            """
-        )
-        variables: dict[str, object] = {"captureId": capture_id, "fileName": file_name}
-        response = await self.execute(query=query, variables=variables)
-        data = self.get_data(response)
-        return DataCaptureUploadDataModelFile.parse_obj(data)
-
     async def platform_admin_update_user(
         self,
         user_id: str,
         first_name: Union[Optional[str], UnsetType] = UNSET,
         last_name: Union[Optional[str], UnsetType] = UNSET,
         user_account_state: Union[Optional[UserAccountState], UnsetType] = UNSET,
         user_roles: Union[Optional[List[Optional[UserRole]]], UnsetType] = UNSET,
@@ -3896,14 +3880,37 @@
             "includeEndpoints": include_endpoints,
             "iotHubId": iot_hub_id,
         }
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return IotListGroups.parse_obj(data)
 
+    async def data_capture_get_active_capture_data_export_download_url(
+        self, capture_id: str
+    ) -> DataCaptureGetActiveCaptureDataExportDownloadUrl:
+        query = gql(
+            """
+            query dataCapture_getActiveCaptureDataExportDownloadUrl($captureId: ID!) {
+              dataCapture_getActiveCaptureDataExportDownloadUrl(captureId: $captureId) {
+                dateCompleted
+                dateStarted
+                exportType
+                logs
+                name
+                state
+                url
+              }
+            }
+            """
+        )
+        variables: dict[str, object] = {"captureId": capture_id}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return DataCaptureGetActiveCaptureDataExportDownloadUrl.parse_obj(data)
+
     async def time_series_db_query_database(
         self,
         assets: List[TimeSeriesQueryAssetInput],
         query_type: TimeSeriesDbQueryType,
         time_series_db_id: str,
         client_token: Union[Optional[str], UnsetType] = UNSET,
         end_time: Union[Optional[str], UnsetType] = UNSET,
@@ -3957,15 +3964,16 @@
     ) -> DataCaptureGetDataExportDownloadUrl:
         query = gql(
             """
             query dataCapture_getDataExportDownloadUrl($captureId: ID!) {
               dataCapture_getDataExportDownloadUrl(captureId: $captureId) {
                 dateCompleted
                 dateStarted
-                errors
+                exportType
+                logs
                 name
                 state
                 url
               }
             }
             """
         )
@@ -4212,14 +4220,15 @@
                 nextToken: $nextToken
               ) {
                 attachmentId
                 attachmentType
                 dateCreated
                 dateUpdated
                 description
+                error
                 name
                 ownerUserId
               }
             }
             """
         )
         variables: dict[str, object] = {
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_add_service_to_collaborative.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_add_service_to_collaborative.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_get_collaborative.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_get_collaborative.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_list_collaborative_member_organization_requests.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaborative_member_organization_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_list_collaborative_services.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaborative_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_list_collaboratives.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaboratives.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_list_collaboratives_service_shared_with.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_list_collaboratives_service_shared_with.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_remove_service_from_collaborative.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_remove_service_from_collaborative.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_update_collaborative_member_organization.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/collaborative_update_collaborative_member_organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_attach_file.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_attach_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_create_capture.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_create_capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_delete_attachment.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_delete_attachment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
-from .enums import DataCaptureAttachmentType
+from .enums import DataCaptureAttachmentError, DataCaptureAttachmentType
 
 
 class DataCaptureDeleteAttachment(BaseModel):
     data_capture_delete_attachment: Optional[
         "DataCaptureDeleteAttachmentDataCaptureDeleteAttachment"
     ] = Field(alias="dataCapture_deleteAttachment")
 
 
 class DataCaptureDeleteAttachmentDataCaptureDeleteAttachment(BaseModel):
     attachment_id: str = Field(alias="attachmentId")
     attachment_type: DataCaptureAttachmentType = Field(alias="attachmentType")
     date_created: Optional[str] = Field(alias="dateCreated")
     date_updated: Optional[str] = Field(alias="dateUpdated")
     description: Optional[str]
+    error: Optional[DataCaptureAttachmentError]
     name: Optional[str]
     owner_user_id: str = Field(alias="ownerUserId")
 
 
 DataCaptureDeleteAttachment.update_forward_refs()
 DataCaptureDeleteAttachmentDataCaptureDeleteAttachment.update_forward_refs()
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_delete_capture.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_delete_capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_capture.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_capture_authentication_token.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_capture_authentication_token.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import AuthenticationTokenType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_data_export_download_url.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_export_download_url.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
-from .enums import DataCaptureDataExportState
+from .enums import DataCaptureDataExportState, DataCaptureDataExportType
 
 
 class DataCaptureGetDataExportDownloadUrl(BaseModel):
     data_capture_get_data_export_download_url: Optional[
         "DataCaptureGetDataExportDownloadUrlDataCaptureGetDataExportDownloadUrl"
     ] = Field(alias="dataCapture_getDataExportDownloadUrl")
 
 
 class DataCaptureGetDataExportDownloadUrlDataCaptureGetDataExportDownloadUrl(BaseModel):
     date_completed: Optional[str] = Field(alias="dateCompleted")
     date_started: Optional[str] = Field(alias="dateStarted")
-    errors: Optional[List[Optional[str]]]
+    export_type: Optional[DataCaptureDataExportType] = Field(alias="exportType")
+    logs: Optional[List[Optional[str]]]
     name: Optional[str]
     state: DataCaptureDataExportState
     url: Optional[str]
 
 
 DataCaptureGetDataExportDownloadUrl.update_forward_refs()
 DataCaptureGetDataExportDownloadUrlDataCaptureGetDataExportDownloadUrl.update_forward_refs()
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_data_model.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_file_attachment_download_url.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_file_attachment_download_url.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_handle_completion.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_handle_completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_list_attachments.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_list_attachments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
-from .enums import DataCaptureAttachmentType
+from .enums import DataCaptureAttachmentError, DataCaptureAttachmentType
 
 
 class DataCaptureListAttachments(BaseModel):
     data_capture_list_attachments: Optional[
         List[Optional["DataCaptureListAttachmentsDataCaptureListAttachments"]]
     ] = Field(alias="dataCapture_listAttachments")
 
 
 class DataCaptureListAttachmentsDataCaptureListAttachments(BaseModel):
     attachment_id: str = Field(alias="attachmentId")
     attachment_type: DataCaptureAttachmentType = Field(alias="attachmentType")
     date_created: Optional[str] = Field(alias="dateCreated")
     date_updated: Optional[str] = Field(alias="dateUpdated")
     description: Optional[str]
+    error: Optional[DataCaptureAttachmentError]
     name: Optional[str]
     owner_user_id: str = Field(alias="ownerUserId")
 
 
 DataCaptureListAttachments.update_forward_refs()
 DataCaptureListAttachmentsDataCaptureListAttachments.update_forward_refs()
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_list_captures.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_list_captures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_notify_capture_complete.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_notify_capture_complete.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_publish_data.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_publish_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import DataCaptureRecordError
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_regenerate_authentication_token.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_regenerate_authentication_token.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import AuthenticationTokenType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_start_capture.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_start_capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_stop_capture.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_stop_capture.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_update_capture.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_update_capture.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_update_data_model.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_update_data_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_upload_data_model_file.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/data_capture_get_data_model_export.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 
 
-class DataCaptureUploadDataModelFile(BaseModel):
-    data_capture_upload_data_model_file: Optional[
-        "DataCaptureUploadDataModelFileDataCaptureUploadDataModelFile"
-    ] = Field(alias="dataCapture_uploadDataModelFile")
+class DataCaptureGetDataModelExport(BaseModel):
+    data_capture_get_data_model_export: Optional[
+        "DataCaptureGetDataModelExportDataCaptureGetDataModelExport"
+    ] = Field(alias="dataCapture_getDataModelExport")
 
 
-class DataCaptureUploadDataModelFileDataCaptureUploadDataModelFile(BaseModel):
-    item_id: Optional[str] = Field(alias="itemId")
-    upload_id: Optional[str] = Field(alias="uploadId")
-    url: Optional[str]
+class DataCaptureGetDataModelExportDataCaptureGetDataModelExport(BaseModel):
+    capture_id: str = Field(alias="captureId")
+    contents: str
+    file_name: str = Field(alias="fileName")
 
 
-DataCaptureUploadDataModelFile.update_forward_refs()
-DataCaptureUploadDataModelFileDataCaptureUploadDataModelFile.update_forward_refs()
+DataCaptureGetDataModelExport.update_forward_refs()
+DataCaptureGetDataModelExportDataCaptureGetDataModelExport.update_forward_refs()
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/enums.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/enums.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
+# Generated by ariadne-codegen on 2023-07-17 11:23
 # Source: ../input/schema.graphql
 
 from enum import Enum
 
 
 class AuthenticationTokenType(str, Enum):
     DATA_CAPTURE_READ_WRITE = "DATA_CAPTURE_READ_WRITE"
@@ -36,25 +36,34 @@
     string = "string"
 
 
 class DataCaptureAssetAttributeType(str, Enum):
     TELEMETRY = "TELEMETRY"
 
 
+class DataCaptureAttachmentError(str, Enum):
+    FILE_UPLOAD_INCOMPLETE = "FILE_UPLOAD_INCOMPLETE"
+
+
 class DataCaptureAttachmentType(str, Enum):
     FILE = "FILE"
 
 
 class DataCaptureDataExportState(str, Enum):
     COMPLETE = "COMPLETE"
     FAILED = "FAILED"
     IN_PROGRESS = "IN_PROGRESS"
     NOT_CREATED = "NOT_CREATED"
 
 
+class DataCaptureDataExportType(str, Enum):
+    ACTIVE_CAPTURE_EXPORT = "ACTIVE_CAPTURE_EXPORT"
+    FULL_EXPORT = "FULL_EXPORT"
+
+
 class DataCaptureDataModelState(str, Enum):
     ERROR = "ERROR"
     GOOD = "GOOD"
 
 
 class DataCaptureRecordError(str, Enum):
     InvalidAttributeId = "InvalidAttributeId"
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/exceptions.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
+# Generated by ariadne-codegen on 2023-07-17 11:23
+
+# Generated by ariadne-codegen on 2023-07-17 11:03
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/input_types.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
+# Generated by ariadne-codegen on 2023-07-17 11:23
 # Source: ../input/schema.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_add_endpoints_to_group.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_add_endpoints_to_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_cancel_query.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_cancel_query.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_create_endpoint.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_endpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_create_group.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_create_hub.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_hub.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_create_model.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_create_new_model_version.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_create_new_model_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_delete_endpoint.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_endpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_delete_group.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_delete_hub.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_hub.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_delete_model.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_delete_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_generate_query_result_export.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_generate_query_result_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ExportFileFormat
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_get_endpoint.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_get_endpoint_token.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_endpoint_token.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import AuthenticationTokenType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_get_group.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_get_hub.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_hub.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_get_model.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_get_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_endpoint_last_values.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_endpoint_last_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_endpoints_in_hub.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_endpoints_in_hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_groups.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_groups_endpoints_last_values.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_groups_endpoints_last_values.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_hubs.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_hubs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_hubs_endpoints_last_values.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_hubs_endpoints_last_values.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_models.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_list_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_notify_query_export_complete.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_notify_query_export_complete.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ExportFileFormat
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_publish.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_publish.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import IotDataRecordErrorType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_query_by_time_range.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_query_by_time_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_regenerate_endpoint_token.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_regenerate_endpoint_token.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import AuthenticationTokenType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_remove_endpoints_from_group.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_remove_endpoints_from_group.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_endpoint.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_endpoint_properties.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_endpoint_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_group.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_group.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_hub.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_hub.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_model.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_model_used_by_endpoint.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/iot_update_model_used_by_endpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ModelAttributeType, ModelSchemaType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/notifications_notify_upload_complete.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/notifications_notify_upload_complete.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_capture_publish_data.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_capture_publish_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import DataCaptureRecordError
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_iot_publish.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_iot_publish.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import IotDataRecordErrorType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_notify_capture_complete.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_capture_complete.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_notify_iot_query_export_complete.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_iot_query_export_complete.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import ExportFileFormat
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_notify_time_series_query_export_complete.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_time_series_query_export_complete.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import TimeSeriesQueryOutputFileType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_notify_upload_complete.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_notify_upload_complete.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_start_capture.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_start_capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_stop_capture.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_stop_capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_time_series_db_publish.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/on_time_series_db_publish.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import MeasureValueType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_add_collaborative_member.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_add_collaborative_member.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_create_collaborative.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_collaborative.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_create_organization.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_organization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_create_user.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_create_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import UserAccountState, UserRole
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_delete_collaborative.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_collaborative.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_delete_organization.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_organization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_delete_user.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_user.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import UserAccountState, UserRole
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_delete_users_collaboratives.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_users_collaboratives.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_delete_users_services.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_delete_users_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_get_collaborative.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_collaborative.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_get_organization.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_organization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_get_user.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_get_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import UserAccountState, UserRole
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_list_collaboratives.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_collaboratives.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_list_organizations.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_organizations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_list_users.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_list_users.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import UserAccountState, UserRole
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_migrate_users_collaboratives_ownership.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_migrate_users_collaboratives_ownership.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_migrate_users_services_ownership.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_migrate_users_services_ownership.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_remove_collaborative_member.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_remove_collaborative_member.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_resend_user_invitation.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_resend_user_invitation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import UserAccountState, UserRole
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_update_collaborative.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_collaborative.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_update_collaborative_member.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_collaborative_member.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_update_organization.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_organization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_update_user.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/platform_admin_update_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import UserAccountState, UserRole
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_create_data_store.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_create_data_store_directory.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import DataStoreObjectType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_create_data_store_file.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_create_data_store_file_data_view.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_create_data_store_file_data_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_delete_data_store.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_delete_data_store_directory.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import DataStoreObjectType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_delete_data_store_file.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_delete_data_store_file_data_view.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_delete_data_store_file_data_view.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_get_data_store.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_get_data_store_directory.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import DataStoreObjectType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_get_data_store_file.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_get_data_store_file_download_url.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_file_download_url.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_get_data_store_zip_download_url.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_get_data_store_zip_download_url.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_list_data_stores.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_list_data_stores.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_update_data_store.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_update_data_store_directory.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import DataStoreObjectType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_update_data_store_file.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/storage_update_data_store_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_cancel_database_query.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_cancel_database_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_create_database.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_create_database.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_delete_database.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_delete_database.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_generate_query_result_export_file.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_generate_query_result_export_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import TimeSeriesQueryOutputFileType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_get_database.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_get_database.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_list_all_asset_last_values.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_list_all_asset_last_values.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import MeasureValueType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_list_databases.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_list_databases.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_notify_time_series_query_export_complete.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_notify_time_series_query_export_complete.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import TimeSeriesQueryOutputFileType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_publish_to_database.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_publish_to_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import MeasureValueType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_query_database.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_query_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_query_database_with_timestream_query.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_query_database_with_timestream_query.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_update_database.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/time_series_db_update_database.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/user_create_authentication_token.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/user_create_authentication_token.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import AuthenticationTokenType
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/user_delete_authentication_token.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/user_list_authentication_tokens.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import AuthenticationTokenType
 
 
-class UserDeleteAuthenticationToken(BaseModel):
-    user_delete_authentication_token: Optional[
-        "UserDeleteAuthenticationTokenUserDeleteAuthenticationToken"
-    ] = Field(alias="user_deleteAuthenticationToken")
+class UserListAuthenticationTokens(BaseModel):
+    user_list_authentication_tokens: Optional[
+        List[Optional["UserListAuthenticationTokensUserListAuthenticationTokens"]]
+    ] = Field(alias="user_listAuthenticationTokens")
 
 
-class UserDeleteAuthenticationTokenUserDeleteAuthenticationToken(BaseModel):
+class UserListAuthenticationTokensUserListAuthenticationTokens(BaseModel):
     date_created: str = Field(alias="dateCreated")
     date_expires: str = Field(alias="dateExpires")
     last_active: Optional[str] = Field(alias="lastActive")
     name: str
     scope: Optional[List[Optional[str]]]
     token_id: str = Field(alias="tokenId")
     token_type: Optional[AuthenticationTokenType] = Field(alias="tokenType")
     token_value: Optional[str] = Field(alias="tokenValue")
     user_id: str = Field(alias="userId")
 
 
-UserDeleteAuthenticationToken.update_forward_refs()
-UserDeleteAuthenticationTokenUserDeleteAuthenticationToken.update_forward_refs()
+UserListAuthenticationTokens.update_forward_refs()
+UserListAuthenticationTokensUserListAuthenticationTokens.update_forward_refs()
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/user_get_user_session.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/async_graphql_client/user_get_user_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Generated by ariadne-codegen on 2023-06-08 15:03
-# Source: ../gqlg/output/queries.graphql
+# Generated by ariadne-codegen on 2023-07-17 11:23
+# Source: ../step_1_gqlg/output/queries.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import UserAccountState, UserRole
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_addServiceToCollaborative.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_addServiceToCollaborative.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_removeServiceFromCollaborative.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_removeServiceFromCollaborative.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_cancelQuery.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_cancelQuery.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_createEndpoint.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_createEndpoint.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_createModel.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_createModel.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_generateQueryResultExport.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_generateQueryResultExport.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_publish.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_publish.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_updateEndpointProperties.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_updateEndpointProperties.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/mutation.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/mutation.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/storage_createDataStoreFile.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/storage_createDataStoreFile.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/storage_deleteDataStoreFile.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/storage_deleteDataStoreFile.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_cancelDatabaseQuery.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_cancelDatabaseQuery.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_generateQueryResultExportFile.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_generateQueryResultExportFile.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_publishToDatabase.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_publishToDatabase.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/collaborative_getCollaborative.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/collaborative_getCollaborative.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativeServices.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativeServices.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaboratives.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaboratives.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativesServiceSharedWith.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativesServiceSharedWith.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/iot_getEndpoint.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/iot_getEndpoint.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/iot_listEndpointLastValues.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/iot_listEndpointLastValues.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/iot_queryByTimeRange.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/iot_queryByTimeRange.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/query.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/query.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStore.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStore.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreDirectory.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreDirectory.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFile.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFile.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFileDownloadUrl.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFileDownloadUrl.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_listDataStores.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/storage_listDataStores.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_getDatabase.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_getDatabase.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listAllAssetLastValues.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listAllAssetLastValues.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listDatabases.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listDatabases.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabase.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabase.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabaseWithTimestreamQuery.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabaseWithTimestreamQuery.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/user_getUserSession.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_queries/user_getUserSession.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyIotQueryExportComplete.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyIotQueryExportComplete.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyTimeSeriesQueryExportComplete.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyTimeSeriesQueryExportComplete.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_subscriptions/subscription.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/graphql_subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/iotUtil.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/iotUtil.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,14 @@
             # Stop query
             if queryId is not None:
                 if self._debug:
                     print("Cancelling query....")
                 mutation = iot_cancelQuery(
                     self._client, self._debug, queryId)
                 cancelResult = mutation.performMutation()
-            exit(1)
 
         signal.signal(signal.SIGINT, quitHandler)
 
         while result.nextToken is not None:
             query = iot_queryByTimeRange(
                 self._client, self._debug, endpointFilterInput, startTime, endTime, result.nextToken, result.clientToken, result.queryString, result.queryId)
             result = query.performQuery()
```

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/logger.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/logger.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/subscriptionClient.py` & `avista_digital_exchange_sdk-0.3.1/src/avista_digital_exchange_sdk/subscriptionClient.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk.egg-info/PKG-INFO` & `avista_digital_exchange_sdk-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: avista-digital-exchange-sdk
-Version: 0.3.0
+Name: avista_digital_exchange_sdk
+Version: 0.3.1
 Summary: SDK to programmatically access the Avista Digital Exchange
 Author-email: Justin Whicker <jwhicker@urbanova.org>, Jon Thompson <jon.thompson@avistacorp.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `avista_digital_exchange_sdk-0.3.0/tests/test_iot_publishData.py` & `avista_digital_exchange_sdk-0.3.1/tests/test_iot_publishData.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from src.avista_digital_exchange_sdk import AvistaDigitalExchange
 import math
 import random
 import time
 import datetime
 
 
-async def runTest(dxInstance: AvistaDigitalExchange):
+async def runTest(dxInstance: AvistaDigitalExchange, iotEndpointId: str):
     i = 0
 
     temp = random.uniform(40.0, 50.0)
     humidity = random.uniform(40.0, 45.0)
     pm = random.uniform(5.0, 15.0)
     while i < 100000:
         curTimeMs = int(math.floor(time.time() * 1000))
@@ -37,18 +37,18 @@
                 "Humidity": f'{humidity}',
                 "PM2_5": f'{pm}'
             }
         }
         ]
 
         result = dxInstance.iot.publish(
-            "iotEndpointId.e141dd76-c9c5-452f-b644-f94907d82fbd", inputData)
+            iotEndpointId, inputData)
         print(result)
         result = dxInstance.iot.updateEndpointProperties(
-            "iotEndpointId.e141dd76-c9c5-452f-b644-f94907d82fbd", {
+            iotEndpointId, {
                 'LastReading': {
                     'value': f'{datetime.datetime.now()}'
                 }
             })
         print(result)
 
         time.sleep(1)
```

