# Comparing `tmp/ubiops-3.8.0.tar.gz` & `tmp/ubiops-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ubiops-3.8.0.tar", last modified: Thu Mar 17 08:52:38 2022, max compression
+gzip compressed data, was "dist/ubiops-3.9.0.tar", last modified: Thu May 12 10:25:32 2022, max compression
```

## Comparing `ubiops-3.8.0.tar` & `ubiops-3.9.0.tar`

### file list

```diff
@@ -1,138 +1,139 @@
-drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-03-17 08:52:38.000000 ubiops-3.8.0/
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     1575 2022-03-17 08:52:38.000000 ubiops-3.8.0/PKG-INFO
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    37541 2022-03-17 08:47:49.000000 ubiops-3.8.0/README.md
--rw-r--r--   0 sascha    (1000) sascha    (1000)       69 2022-03-17 08:52:38.000000 ubiops-3.8.0/setup.cfg
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     1029 2022-03-17 08:47:49.000000 ubiops-3.8.0/setup.py
-drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-03-17 08:52:38.000000 ubiops-3.8.0/ubiops/
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     8711 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/__init__.py
-drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-03-17 08:52:38.000000 ubiops-3.8.0/ubiops/api/
--rw-r--r--   0 sascha    (1000) sascha    (1000)      127 2022-03-17 08:24:32.000000 ubiops-3.8.0/ubiops/api/__init__.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)  1648175 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/api/core_api.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    26217 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/api_client.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    13265 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/configuration.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     4461 2022-03-17 08:24:32.000000 ubiops-3.8.0/ubiops/exceptions.py
-drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-03-17 08:52:38.000000 ubiops-3.8.0/ubiops/models/
--rw-r--r--   0 sascha    (1000) sascha    (1000)     8291 2022-03-17 08:24:32.000000 ubiops-3.8.0/ubiops/models/__init__.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5934 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/attachment_fields_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5910 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/attachment_fields_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5395 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/attachment_sources_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5359 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/attachment_sources_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5621 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/attachments_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6337 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/attachments_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     9475 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/audit_list.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     9388 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/blob_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     8254 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/build_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)    11787 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_create.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    15816 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/deployment_create_response.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    16492 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/deployment_detail.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6788 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_input_field_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6542 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_input_field_detail.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5493 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_input_field_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     4788 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_input_field_widget_create.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    11960 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/deployment_instance_type.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    16435 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/deployment_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6810 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_output_field_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6558 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_output_field_detail.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5505 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_output_field_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     4800 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_output_field_widget_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     8362 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_request_batch_create_response.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)    13095 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_request_batch_detail.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     8321 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_request_create_response.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)    10399 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_request_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)    15185 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_request_single_detail.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5267 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_request_update.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)    14381 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_request_update_response.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     9763 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_update.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    20037 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/deployment_version_create.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    28250 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/deployment_version_detail.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    27198 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/deployment_version_list.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    17010 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/deployment_version_update.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     4771 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/deployment_widget_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     9224 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/direct_pipeline_request_deployment_request.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5566 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/environment_variable_copy.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6050 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/environment_variable_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6773 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/environment_variable_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5790 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/export_create.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    11463 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/export_detail.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     8226 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/export_list.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    11515 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/import_detail.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     8278 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/import_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5790 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/import_update.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     9864 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/inherited_environment_variable_list.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    16798 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/logs.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     7447 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/logs_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     4734 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/metrics.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5136 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/notification_group_contact.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5639 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/notification_group_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6396 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/notification_group_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5090 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/notification_group_update.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     6396 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/organization_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     9207 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/organization_detail.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5611 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/organization_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6775 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/organization_update.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     4760 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/organization_user_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     8537 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/organization_user_detail.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     3509 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/organization_user_update.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     3655 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/permission_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)    11538 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_create.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    15696 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/pipeline_create_response.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    16364 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/pipeline_detail.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6744 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_input_field_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6498 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_input_field_detail.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5469 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_input_field_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     4764 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_input_field_widget_create.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    15517 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/pipeline_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6766 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_output_field_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6514 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_output_field_detail.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5481 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_output_field_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     4776 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_output_field_widget_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     8270 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_request_batch_create_response.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)    10180 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_request_create_response.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     7214 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_request_deployment_request.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)    14357 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_request_detail.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)    10283 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_request_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)    16695 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_request_single_detail.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)    12097 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_update.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    14205 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/pipeline_version_create.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    17983 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/pipeline_version_detail.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    15173 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/pipeline_version_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6559 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_version_object_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)    13790 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_version_object_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     4891 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_version_object_update.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    14046 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/pipeline_version_update.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     4747 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/pipeline_widget_list.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     7581 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/project_create.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    11074 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/project_detail.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     9037 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/project_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     7686 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/project_resource_usage.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     6519 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/project_update.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     3666 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/project_user_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6915 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/project_user_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     9227 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/resource_usage.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5673 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/revision_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6320 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/revision_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     7394 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/role_assignment_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     7851 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/role_assignment_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     4899 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/role_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6627 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/role_detail_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5571 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/role_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     4584 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/role_update.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)    13251 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/schedule_create.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    14418 2022-03-17 08:47:49.000000 ubiops-3.8.0/ubiops/models/schedule_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     9061 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/schedule_update.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5587 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/service_user_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     8998 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/service_user_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)    10048 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/service_user_token_detail.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     3884 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/service_user_token_list.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     3799 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/status.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6425 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/usage.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     5271 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/usage_metric.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     9988 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/user_pending_create.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)     6280 2022-03-17 08:24:23.000000 ubiops-3.8.0/ubiops/models/user_pending_detail.py
--rw-r--r--   0 sascha    (1000) sascha    (1000)    12424 2022-03-17 08:24:32.000000 ubiops-3.8.0/ubiops/rest.py
-drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-03-17 08:52:38.000000 ubiops-3.8.0/ubiops.egg-info/
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     1575 2022-03-17 08:52:38.000000 ubiops-3.8.0/ubiops.egg-info/PKG-INFO
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     4925 2022-03-17 08:52:38.000000 ubiops-3.8.0/ubiops.egg-info/SOURCES.txt
--rw-rw-r--   0 sascha    (1000) sascha    (1000)        1 2022-03-17 08:52:38.000000 ubiops-3.8.0/ubiops.egg-info/dependency_links.txt
--rw-rw-r--   0 sascha    (1000) sascha    (1000)       48 2022-03-17 08:52:38.000000 ubiops-3.8.0/ubiops.egg-info/requires.txt
--rw-rw-r--   0 sascha    (1000) sascha    (1000)        7 2022-03-17 08:52:38.000000 ubiops-3.8.0/ubiops.egg-info/top_level.txt
+drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-05-12 10:25:32.000000 ubiops-3.9.0/
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     1575 2022-05-12 10:25:32.000000 ubiops-3.9.0/PKG-INFO
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    37739 2022-05-12 10:15:55.000000 ubiops-3.9.0/README.md
+-rw-r--r--   0 sascha    (1000) sascha    (1000)       69 2022-05-12 10:25:32.000000 ubiops-3.9.0/setup.cfg
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     1029 2022-05-12 10:15:55.000000 ubiops-3.9.0/setup.py
+drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-05-12 10:25:32.000000 ubiops-3.9.0/ubiops/
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     8772 2022-05-12 10:15:55.000000 ubiops-3.9.0/ubiops/__init__.py
+drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-05-12 10:25:32.000000 ubiops-3.9.0/ubiops/api/
+-rw-r--r--   0 sascha    (1000) sascha    (1000)      127 2022-05-12 10:15:55.000000 ubiops-3.9.0/ubiops/api/__init__.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)  1658007 2022-05-12 10:15:55.000000 ubiops-3.9.0/ubiops/api/core_api.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    26217 2022-05-12 10:15:55.000000 ubiops-3.9.0/ubiops/api_client.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    13265 2022-05-12 10:15:55.000000 ubiops-3.9.0/ubiops/configuration.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     4461 2022-05-12 10:15:55.000000 ubiops-3.9.0/ubiops/exceptions.py
+drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-05-12 10:25:32.000000 ubiops-3.9.0/ubiops/models/
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     8352 2022-05-12 10:15:55.000000 ubiops-3.9.0/ubiops/models/__init__.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5944 2022-05-12 10:15:42.000000 ubiops-3.9.0/ubiops/models/attachment_fields_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5920 2022-05-12 10:15:42.000000 ubiops-3.9.0/ubiops/models/attachment_fields_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5405 2022-05-12 10:15:42.000000 ubiops-3.9.0/ubiops/models/attachment_sources_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5369 2022-05-12 10:15:42.000000 ubiops-3.9.0/ubiops/models/attachment_sources_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5631 2022-05-12 10:15:42.000000 ubiops-3.9.0/ubiops/models/attachments_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6347 2022-05-12 10:15:42.000000 ubiops-3.9.0/ubiops/models/attachments_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     9485 2022-05-12 10:15:42.000000 ubiops-3.9.0/ubiops/models/audit_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     9398 2022-05-12 10:15:42.000000 ubiops-3.9.0/ubiops/models/blob_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     8264 2022-05-12 10:15:42.000000 ubiops-3.9.0/ubiops/models/build_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    11797 2022-05-12 10:15:42.000000 ubiops-3.9.0/ubiops/models/deployment_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    15826 2022-05-12 10:15:42.000000 ubiops-3.9.0/ubiops/models/deployment_create_response.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    16502 2022-05-12 10:15:42.000000 ubiops-3.9.0/ubiops/models/deployment_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6798 2022-05-12 10:15:42.000000 ubiops-3.9.0/ubiops/models/deployment_input_field_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6552 2022-05-12 10:15:42.000000 ubiops-3.9.0/ubiops/models/deployment_input_field_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5503 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_input_field_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     4798 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_input_field_widget_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    12755 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_instance_type.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    16445 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6820 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_output_field_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6568 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_output_field_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5515 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_output_field_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     4810 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_output_field_widget_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     8372 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_request_batch_create_response.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    13105 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_request_batch_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     8331 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_request_create_response.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    10409 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_request_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    15195 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_request_single_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5277 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_request_update.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    14391 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_request_update_response.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     9773 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_update.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    18578 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_version_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    26735 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_version_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    25691 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_version_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    17020 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_version_update.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     4781 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/deployment_widget_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     9234 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/direct_pipeline_request_deployment_request.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5576 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/environment_variable_copy.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6060 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/environment_variable_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6783 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/environment_variable_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5800 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/export_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    11473 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/export_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     8236 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/export_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    11525 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/import_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     8288 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/import_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5800 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/import_update.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     9874 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/inherited_environment_variable_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    16808 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/logs.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     7457 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/logs_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     4744 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/metrics.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5146 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/notification_group_contact.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5649 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/notification_group_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6406 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/notification_group_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5100 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/notification_group_update.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6406 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/organization_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     9217 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/organization_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5621 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/organization_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6785 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/organization_update.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     4770 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/organization_user_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     8547 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/organization_user_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     3519 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/organization_user_update.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     3665 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/permission_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    11548 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    15706 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_create_response.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    16374 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6754 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_input_field_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6508 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_input_field_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5479 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_input_field_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     4774 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_input_field_widget_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    15527 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6776 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_output_field_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6524 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_output_field_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5491 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_output_field_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     4786 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_output_field_widget_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     8280 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_request_batch_create_response.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    10190 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_request_create_response.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     7224 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_request_deployment_request.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    14367 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_request_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    10293 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_request_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    16705 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_request_single_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    12107 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_update.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    14215 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_version_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    17993 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_version_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    15183 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_version_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6569 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_version_object_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    12748 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_version_object_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     4901 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_version_object_update.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    14056 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_version_update.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     4757 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/pipeline_widget_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     7591 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/project_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    11084 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/project_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     9047 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/project_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     7696 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/project_resource_usage.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6529 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/project_update.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     3676 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/project_user_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6369 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/project_user_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    11125 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/requests_overview.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     9237 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/resource_usage.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5683 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/revision_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6330 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/revision_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     7404 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/role_assignment_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     7861 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/role_assignment_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     4909 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/role_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6637 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/role_detail_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5581 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/role_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     4594 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/role_update.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    13261 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/schedule_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    13609 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/schedule_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     9071 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/schedule_update.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5597 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/service_user_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     9008 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/service_user_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    10058 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/service_user_token_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     3894 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/service_user_token_list.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     3809 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/status.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     6435 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/usage.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5281 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/usage_metric.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     9998 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/user_pending_create.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)     5734 2022-05-12 10:15:43.000000 ubiops-3.9.0/ubiops/models/user_pending_detail.py
+-rw-r--r--   0 sascha    (1000) sascha    (1000)    12424 2022-05-12 10:15:55.000000 ubiops-3.9.0/ubiops/rest.py
+drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2022-05-12 10:25:32.000000 ubiops-3.9.0/ubiops.egg-info/
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     1575 2022-05-12 10:25:32.000000 ubiops-3.9.0/ubiops.egg-info/PKG-INFO
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)     4960 2022-05-12 10:25:32.000000 ubiops-3.9.0/ubiops.egg-info/SOURCES.txt
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)        1 2022-05-12 10:25:32.000000 ubiops-3.9.0/ubiops.egg-info/dependency_links.txt
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)       48 2022-05-12 10:25:32.000000 ubiops-3.9.0/ubiops.egg-info/requires.txt
+-rw-rw-r--   0 sascha    (1000) sascha    (1000)        7 2022-05-12 10:25:32.000000 ubiops-3.9.0/ubiops.egg-info/top_level.txt
```

### Comparing `ubiops-3.8.0/PKG-INFO` & `ubiops-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiops
-Version: 3.8.0
+Version: 3.9.0
 Summary: UbiOps
 Home-page: https://github.com/UbiOps/client-library-python.git
 Author: UbiOps
 License: Apache 2.0
 Description: # ubiops
         Client Library to interact with the [UbiOps](https://ubiops.com) API (v2.1).
```

### Comparing `ubiops-3.8.0/README.md` & `ubiops-3.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [www.ubiops.com](https://ubiops.com)
 
 Client Library to interact with the UbiOps API.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v2.1
-- Package version: 3.8.0
+- Package version: 3.9.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 For more information, please visit [https://ubiops.com/docs](https://ubiops.com/docs)
 
 ## Requirements.
 
 Python 3.5+
@@ -192,14 +192,15 @@
 *CoreApi* | [**pipelines_update**](docs/CoreApi.md#pipelines_update) | **PATCH** /projects/{project_name}/pipelines/{pipeline_name} | Update a pipeline
 *CoreApi* | [**project_audit_events_list**](docs/CoreApi.md#project_audit_events_list) | **GET** /projects/{project_name}/audit | List audit events in a project
 *CoreApi* | [**project_environment_variables_create**](docs/CoreApi.md#project_environment_variables_create) | **POST** /projects/{project_name}/environment-variables | Create project environment variable
 *CoreApi* | [**project_environment_variables_delete**](docs/CoreApi.md#project_environment_variables_delete) | **DELETE** /projects/{project_name}/environment-variables/{id} | Delete project environment variable
 *CoreApi* | [**project_environment_variables_get**](docs/CoreApi.md#project_environment_variables_get) | **GET** /projects/{project_name}/environment-variables/{id} | Get project environment variable
 *CoreApi* | [**project_environment_variables_list**](docs/CoreApi.md#project_environment_variables_list) | **GET** /projects/{project_name}/environment-variables | List project environment variables
 *CoreApi* | [**project_environment_variables_update**](docs/CoreApi.md#project_environment_variables_update) | **PATCH** /projects/{project_name}/environment-variables/{id} | Update project environment variable
+*CoreApi* | [**project_requests_list**](docs/CoreApi.md#project_requests_list) | **GET** /projects/{project_name}/requests | List requests in project
 *CoreApi* | [**project_users_create**](docs/CoreApi.md#project_users_create) | **POST** /projects/{project_name}/users | Add user to a project
 *CoreApi* | [**project_users_delete**](docs/CoreApi.md#project_users_delete) | **DELETE** /projects/{project_name}/users/{user_id} | Delete user from a project
 *CoreApi* | [**project_users_get**](docs/CoreApi.md#project_users_get) | **GET** /projects/{project_name}/users/{user_id} | Get user in a project
 *CoreApi* | [**project_users_list**](docs/CoreApi.md#project_users_list) | **GET** /projects/{project_name}/users | List users in a project
 *CoreApi* | [**projects_create**](docs/CoreApi.md#projects_create) | **POST** /projects | Create projects
 *CoreApi* | [**projects_delete**](docs/CoreApi.md#projects_delete) | **DELETE** /projects/{project_name} | Delete a project
 *CoreApi* | [**projects_get**](docs/CoreApi.md#projects_get) | **GET** /projects/{project_name} | Get details of a project
@@ -330,14 +331,15 @@
  - [ProjectCreate](docs/ProjectCreate.md)
  - [ProjectDetail](docs/ProjectDetail.md)
  - [ProjectList](docs/ProjectList.md)
  - [ProjectResourceUsage](docs/ProjectResourceUsage.md)
  - [ProjectUpdate](docs/ProjectUpdate.md)
  - [ProjectUserCreate](docs/ProjectUserCreate.md)
  - [ProjectUserList](docs/ProjectUserList.md)
+ - [RequestsOverview](docs/RequestsOverview.md)
  - [ResourceUsage](docs/ResourceUsage.md)
  - [RevisionCreate](docs/RevisionCreate.md)
  - [RevisionList](docs/RevisionList.md)
  - [RoleAssignmentCreate](docs/RoleAssignmentCreate.md)
  - [RoleAssignmentList](docs/RoleAssignmentList.md)
  - [RoleCreate](docs/RoleCreate.md)
  - [RoleDetailList](docs/RoleDetailList.md)
```

### Comparing `ubiops-3.8.0/setup.py` & `ubiops-3.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "ubiops"
-VERSION = "3.8.0"
+VERSION = "3.9.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `ubiops-3.8.0/ubiops/__init__.py` & `ubiops-3.9.0/ubiops/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: v2.1
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "3.8.0"
+__version__ = "3.9.0"
 
 # import apis into sdk package
 from ubiops.api.core_api import CoreApi
 
 # import ApiClient
 from ubiops.api_client import ApiClient
 from ubiops.configuration import Configuration
@@ -119,14 +119,15 @@
 from ubiops.models.project_create import ProjectCreate
 from ubiops.models.project_detail import ProjectDetail
 from ubiops.models.project_list import ProjectList
 from ubiops.models.project_resource_usage import ProjectResourceUsage
 from ubiops.models.project_update import ProjectUpdate
 from ubiops.models.project_user_create import ProjectUserCreate
 from ubiops.models.project_user_list import ProjectUserList
+from ubiops.models.requests_overview import RequestsOverview
 from ubiops.models.resource_usage import ResourceUsage
 from ubiops.models.revision_create import RevisionCreate
 from ubiops.models.revision_list import RevisionList
 from ubiops.models.role_assignment_create import RoleAssignmentCreate
 from ubiops.models.role_assignment_list import RoleAssignmentList
 from ubiops.models.role_create import RoleCreate
 from ubiops.models.role_detail_list import RoleDetailList
```

### Comparing `ubiops-3.8.0/ubiops/api/core_api.py` & `ubiops-3.9.0/ubiops/api/core_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def batch_pipeline_requests_create(self, project_name, pipeline_name, data, **kwargs):  # noqa: E501
         """Create a batch pipeline request  # noqa: E501
 
-         ### Description Make a batch request to the default version of a pipeline. The request follows an asynchronous method, as the requests are queued in our back-end and can be collected at a later time using the pipeline request collect methods.  The maximum number of requests that can be created per batch is 100.  ### Required Parameters  In case of structured input pipeline: A list of dictionaries, where each dictionary contains the input fields of the pipeline as keys. It is also possible to send a single dictionary as input. In case of plain input pipeline: A list of strings. It is also possible to send a single string as input.  ### Optional Parameters These parameters should be given as query parameters - `timeout`: Timeout for the entire pipeline request in seconds. The maximum allowed value is 172800 (48 hours) and the default value is 14400 (4 hours). The deployment request timeouts default to 300 seconds for express deployments in the pipeline and to 14400 seconds for batch deployments. - `notification_group`: Name of a notification group to send notifications (e.g., emails) when the request is completed  #### Request Examples  Multiple structured batch pipeline requests ``` [   {     \"pipeline-input-field-1\": 5.0,     \"pipeline-input-field-2\": \"N\",     \"pipeline-input-field-3\": [0.25, 0.25, 2.1, 16.3]   },   {     \"pipeline-input-field-1\": 3.0,     \"pipeline-input-field-2\": \"S\",     \"pipeline-input-field-3\": [4.23, 3.27, 2.41, 12.4]   } ] ```  Multiple plain batch pipeline requests ``` [   \"plain-data-goes-here\", \"plain-example-data\" ] ```  ### Response Structure  A list of dictionaries containing the details of the created pipeline requests with the following fields:  - `id`: Unique identifier for the pipeline request, which can be used to collect the result  - `pipeline`: Name of the pipeline for which the request is made  - `version`: Name of the pipeline version for which the request is made  - `status`: Status of the request. Always 'pending' when initialised, later it can be 'processing', 'failed' or 'completed'.  - `time_created`: Server time that the request was made (current time)  #### Response Examples  ``` [   {     \"id\": \"69eca481-8576-49e8-8e20-ea56f2005bcb\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"time_created\": \"2020-03-28T20:00:26.613+00:00\"   },   {     \"id\": \"2521378e-263e-4e2e-85e9-a96254b36536\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"time_created\": \"2020-03-28T20:00:26.613+00:00\"   } ] ```   # noqa: E501
+         ### Description Make a batch request to the default version of a pipeline. The request follows an asynchronous method, as the requests are queued in our back-end and can be collected at a later time using the pipeline request collect methods.  The maximum number of requests that can be created per batch is 100.  ### Required Parameters  In case of structured input pipeline: A list of dictionaries, where each dictionary contains the input fields of the pipeline as keys. It is also possible to send a single dictionary as input. In case of plain input pipeline: A list of strings. It is also possible to send a single string as input.  ### Optional Parameters These parameters should be given as query parameters - `timeout`: Timeout for the entire pipeline request in seconds. The maximum allowed value is 172800 (48 hours) and the default value is 14400 (4 hours). The deployment request timeouts default to 14400 seconds for deployments in the pipeline. - `notification_group`: Name of a notification group to send notifications (e.g., emails) when the request is completed  #### Request Examples  Multiple structured batch pipeline requests ``` [   {     \"pipeline-input-field-1\": 5.0,     \"pipeline-input-field-2\": \"N\",     \"pipeline-input-field-3\": [0.25, 0.25, 2.1, 16.3]   },   {     \"pipeline-input-field-1\": 3.0,     \"pipeline-input-field-2\": \"S\",     \"pipeline-input-field-3\": [4.23, 3.27, 2.41, 12.4]   } ] ```  Multiple plain batch pipeline requests ``` [   \"plain-data-goes-here\", \"plain-example-data\" ] ```  ### Response Structure  A list of dictionaries containing the details of the created pipeline requests with the following fields:  - `id`: Unique identifier for the pipeline request, which can be used to collect the result  - `pipeline`: Name of the pipeline for which the request is made  - `version`: Name of the pipeline version for which the request is made  - `status`: Status of the request. Always 'pending' when initialised, later it can be 'processing', 'failed' or 'completed'.  - `time_created`: Server time that the request was made (current time)  #### Response Examples  ``` [   {     \"id\": \"69eca481-8576-49e8-8e20-ea56f2005bcb\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"time_created\": \"2020-03-28T20:00:26.613+00:00\"   },   {     \"id\": \"2521378e-263e-4e2e-85e9-a96254b36536\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"time_created\": \"2020-03-28T20:00:26.613+00:00\"   } ] ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.batch_pipeline_requests_create(project_name, pipeline_name, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -392,15 +392,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.batch_pipeline_requests_create_with_http_info(project_name, pipeline_name, data, **kwargs)  # noqa: E501
 
     def batch_pipeline_requests_create_with_http_info(self, project_name, pipeline_name, data, **kwargs):  # noqa: E501
         """Create a batch pipeline request  # noqa: E501
 
-         ### Description Make a batch request to the default version of a pipeline. The request follows an asynchronous method, as the requests are queued in our back-end and can be collected at a later time using the pipeline request collect methods.  The maximum number of requests that can be created per batch is 100.  ### Required Parameters  In case of structured input pipeline: A list of dictionaries, where each dictionary contains the input fields of the pipeline as keys. It is also possible to send a single dictionary as input. In case of plain input pipeline: A list of strings. It is also possible to send a single string as input.  ### Optional Parameters These parameters should be given as query parameters - `timeout`: Timeout for the entire pipeline request in seconds. The maximum allowed value is 172800 (48 hours) and the default value is 14400 (4 hours). The deployment request timeouts default to 300 seconds for express deployments in the pipeline and to 14400 seconds for batch deployments. - `notification_group`: Name of a notification group to send notifications (e.g., emails) when the request is completed  #### Request Examples  Multiple structured batch pipeline requests ``` [   {     \"pipeline-input-field-1\": 5.0,     \"pipeline-input-field-2\": \"N\",     \"pipeline-input-field-3\": [0.25, 0.25, 2.1, 16.3]   },   {     \"pipeline-input-field-1\": 3.0,     \"pipeline-input-field-2\": \"S\",     \"pipeline-input-field-3\": [4.23, 3.27, 2.41, 12.4]   } ] ```  Multiple plain batch pipeline requests ``` [   \"plain-data-goes-here\", \"plain-example-data\" ] ```  ### Response Structure  A list of dictionaries containing the details of the created pipeline requests with the following fields:  - `id`: Unique identifier for the pipeline request, which can be used to collect the result  - `pipeline`: Name of the pipeline for which the request is made  - `version`: Name of the pipeline version for which the request is made  - `status`: Status of the request. Always 'pending' when initialised, later it can be 'processing', 'failed' or 'completed'.  - `time_created`: Server time that the request was made (current time)  #### Response Examples  ``` [   {     \"id\": \"69eca481-8576-49e8-8e20-ea56f2005bcb\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"time_created\": \"2020-03-28T20:00:26.613+00:00\"   },   {     \"id\": \"2521378e-263e-4e2e-85e9-a96254b36536\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"time_created\": \"2020-03-28T20:00:26.613+00:00\"   } ] ```   # noqa: E501
+         ### Description Make a batch request to the default version of a pipeline. The request follows an asynchronous method, as the requests are queued in our back-end and can be collected at a later time using the pipeline request collect methods.  The maximum number of requests that can be created per batch is 100.  ### Required Parameters  In case of structured input pipeline: A list of dictionaries, where each dictionary contains the input fields of the pipeline as keys. It is also possible to send a single dictionary as input. In case of plain input pipeline: A list of strings. It is also possible to send a single string as input.  ### Optional Parameters These parameters should be given as query parameters - `timeout`: Timeout for the entire pipeline request in seconds. The maximum allowed value is 172800 (48 hours) and the default value is 14400 (4 hours). The deployment request timeouts default to 14400 seconds for deployments in the pipeline. - `notification_group`: Name of a notification group to send notifications (e.g., emails) when the request is completed  #### Request Examples  Multiple structured batch pipeline requests ``` [   {     \"pipeline-input-field-1\": 5.0,     \"pipeline-input-field-2\": \"N\",     \"pipeline-input-field-3\": [0.25, 0.25, 2.1, 16.3]   },   {     \"pipeline-input-field-1\": 3.0,     \"pipeline-input-field-2\": \"S\",     \"pipeline-input-field-3\": [4.23, 3.27, 2.41, 12.4]   } ] ```  Multiple plain batch pipeline requests ``` [   \"plain-data-goes-here\", \"plain-example-data\" ] ```  ### Response Structure  A list of dictionaries containing the details of the created pipeline requests with the following fields:  - `id`: Unique identifier for the pipeline request, which can be used to collect the result  - `pipeline`: Name of the pipeline for which the request is made  - `version`: Name of the pipeline version for which the request is made  - `status`: Status of the request. Always 'pending' when initialised, later it can be 'processing', 'failed' or 'completed'.  - `time_created`: Server time that the request was made (current time)  #### Response Examples  ``` [   {     \"id\": \"69eca481-8576-49e8-8e20-ea56f2005bcb\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"time_created\": \"2020-03-28T20:00:26.613+00:00\"   },   {     \"id\": \"2521378e-263e-4e2e-85e9-a96254b36536\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"time_created\": \"2020-03-28T20:00:26.613+00:00\"   } ] ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.batch_pipeline_requests_create_with_http_info(project_name, pipeline_name, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -521,15 +521,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def batch_pipeline_version_requests_create(self, project_name, pipeline_name, version, data, **kwargs):  # noqa: E501
         """Create a batch pipeline version request  # noqa: E501
 
-         ### Description Make a batch request to a pipeline version. The request follows an asynchronous method, as the requests are queued in our back-end and can be collected at a later time using the pipeline version request collect methods.  The maximum number of requests that can be created per batch is 100.  ### Required Parameters  In case of structured input pipeline: A list of dictionaries, where each dictionary contains the input fields of the pipeline as keys. It is also possible to send a single dictionary as input. In case of plain input pipeline: A list of strings. It is also possible to send a single string as input.  ### Optional Parameters These parameters should be given as query parameters - `timeout`: Timeout for the entire pipeline request in seconds. The maximum allowed value is 172800 (48 hours) and the default value is 14400 (4 hours). The deployment request timeouts default to 300 seconds for express deployments in the pipeline and to 14400 seconds for batch deployments. - `notification_group`: Name of a notification group to send notifications (e.g., emails) when the request is completed  #### Request Examples  Multiple structured batch pipeline requests ``` [   {     \"pipeline-input-field-1\": 5.0,     \"pipeline-input-field-2\": \"N\",     \"pipeline-input-field-3\": [0.25, 0.25, 2.1, 16.3]   },   {     \"pipeline-input-field-1\": 3.0,     \"pipeline-input-field-2\": \"S\",     \"pipeline-input-field-3\": [4.23, 3.27, 2.41, 12.4]   } ] ```  Multiple plain batch pipeline requests ``` [   \"plain-data-goes-here\", \"plain-example-data\" ] ```  ### Response Structure  A list of dictionaries containing the details of the created pipeline version requests with the following fields:  - `id`: Unique identifier for the pipeline version request, which can be used to collect the result  - `pipeline`: Name of the pipeline for which the request is made  - `version`: Name of the pipeline version for which the request is made  - `status`: Status of the request. Always 'pending' when initialised, later it can be 'processing', 'failed' or 'completed'.  - `time_created`: Server time that the request was made (current time)  #### Response Examples  ``` [   {     \"id\": \"69eca481-8576-49e8-8e20-ea56f2005bcb\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"time_created\": \"2020-03-28T20:00:26.613+00:00\"   },   {     \"id\": \"2521378e-263e-4e2e-85e9-a96254b36536\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"time_created\": \"2020-03-28T20:00:26.613+00:00\"   } ] ```   # noqa: E501
+         ### Description Make a batch request to a pipeline version. The request follows an asynchronous method, as the requests are queued in our back-end and can be collected at a later time using the pipeline version request collect methods.  The maximum number of requests that can be created per batch is 100.  ### Required Parameters  In case of structured input pipeline: A list of dictionaries, where each dictionary contains the input fields of the pipeline as keys. It is also possible to send a single dictionary as input. In case of plain input pipeline: A list of strings. It is also possible to send a single string as input.  ### Optional Parameters These parameters should be given as query parameters - `timeout`: Timeout for the entire pipeline request in seconds. The maximum allowed value is 172800 (48 hours) and the default value is 14400 (4 hours). The deployment request timeouts default to 14400 seconds for deployments in the pipeline. - `notification_group`: Name of a notification group to send notifications (e.g., emails) when the request is completed  #### Request Examples  Multiple structured batch pipeline requests ``` [   {     \"pipeline-input-field-1\": 5.0,     \"pipeline-input-field-2\": \"N\",     \"pipeline-input-field-3\": [0.25, 0.25, 2.1, 16.3]   },   {     \"pipeline-input-field-1\": 3.0,     \"pipeline-input-field-2\": \"S\",     \"pipeline-input-field-3\": [4.23, 3.27, 2.41, 12.4]   } ] ```  Multiple plain batch pipeline requests ``` [   \"plain-data-goes-here\", \"plain-example-data\" ] ```  ### Response Structure  A list of dictionaries containing the details of the created pipeline version requests with the following fields:  - `id`: Unique identifier for the pipeline version request, which can be used to collect the result  - `pipeline`: Name of the pipeline for which the request is made  - `version`: Name of the pipeline version for which the request is made  - `status`: Status of the request. Always 'pending' when initialised, later it can be 'processing', 'failed' or 'completed'.  - `time_created`: Server time that the request was made (current time)  #### Response Examples  ``` [   {     \"id\": \"69eca481-8576-49e8-8e20-ea56f2005bcb\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"time_created\": \"2020-03-28T20:00:26.613+00:00\"   },   {     \"id\": \"2521378e-263e-4e2e-85e9-a96254b36536\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"time_created\": \"2020-03-28T20:00:26.613+00:00\"   } ] ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.batch_pipeline_version_requests_create(project_name, pipeline_name, version, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -551,15 +551,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.batch_pipeline_version_requests_create_with_http_info(project_name, pipeline_name, version, data, **kwargs)  # noqa: E501
 
     def batch_pipeline_version_requests_create_with_http_info(self, project_name, pipeline_name, version, data, **kwargs):  # noqa: E501
         """Create a batch pipeline version request  # noqa: E501
 
-         ### Description Make a batch request to a pipeline version. The request follows an asynchronous method, as the requests are queued in our back-end and can be collected at a later time using the pipeline version request collect methods.  The maximum number of requests that can be created per batch is 100.  ### Required Parameters  In case of structured input pipeline: A list of dictionaries, where each dictionary contains the input fields of the pipeline as keys. It is also possible to send a single dictionary as input. In case of plain input pipeline: A list of strings. It is also possible to send a single string as input.  ### Optional Parameters These parameters should be given as query parameters - `timeout`: Timeout for the entire pipeline request in seconds. The maximum allowed value is 172800 (48 hours) and the default value is 14400 (4 hours). The deployment request timeouts default to 300 seconds for express deployments in the pipeline and to 14400 seconds for batch deployments. - `notification_group`: Name of a notification group to send notifications (e.g., emails) when the request is completed  #### Request Examples  Multiple structured batch pipeline requests ``` [   {     \"pipeline-input-field-1\": 5.0,     \"pipeline-input-field-2\": \"N\",     \"pipeline-input-field-3\": [0.25, 0.25, 2.1, 16.3]   },   {     \"pipeline-input-field-1\": 3.0,     \"pipeline-input-field-2\": \"S\",     \"pipeline-input-field-3\": [4.23, 3.27, 2.41, 12.4]   } ] ```  Multiple plain batch pipeline requests ``` [   \"plain-data-goes-here\", \"plain-example-data\" ] ```  ### Response Structure  A list of dictionaries containing the details of the created pipeline version requests with the following fields:  - `id`: Unique identifier for the pipeline version request, which can be used to collect the result  - `pipeline`: Name of the pipeline for which the request is made  - `version`: Name of the pipeline version for which the request is made  - `status`: Status of the request. Always 'pending' when initialised, later it can be 'processing', 'failed' or 'completed'.  - `time_created`: Server time that the request was made (current time)  #### Response Examples  ``` [   {     \"id\": \"69eca481-8576-49e8-8e20-ea56f2005bcb\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"time_created\": \"2020-03-28T20:00:26.613+00:00\"   },   {     \"id\": \"2521378e-263e-4e2e-85e9-a96254b36536\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"time_created\": \"2020-03-28T20:00:26.613+00:00\"   } ] ```   # noqa: E501
+         ### Description Make a batch request to a pipeline version. The request follows an asynchronous method, as the requests are queued in our back-end and can be collected at a later time using the pipeline version request collect methods.  The maximum number of requests that can be created per batch is 100.  ### Required Parameters  In case of structured input pipeline: A list of dictionaries, where each dictionary contains the input fields of the pipeline as keys. It is also possible to send a single dictionary as input. In case of plain input pipeline: A list of strings. It is also possible to send a single string as input.  ### Optional Parameters These parameters should be given as query parameters - `timeout`: Timeout for the entire pipeline request in seconds. The maximum allowed value is 172800 (48 hours) and the default value is 14400 (4 hours). The deployment request timeouts default to 14400 seconds for deployments in the pipeline. - `notification_group`: Name of a notification group to send notifications (e.g., emails) when the request is completed  #### Request Examples  Multiple structured batch pipeline requests ``` [   {     \"pipeline-input-field-1\": 5.0,     \"pipeline-input-field-2\": \"N\",     \"pipeline-input-field-3\": [0.25, 0.25, 2.1, 16.3]   },   {     \"pipeline-input-field-1\": 3.0,     \"pipeline-input-field-2\": \"S\",     \"pipeline-input-field-3\": [4.23, 3.27, 2.41, 12.4]   } ] ```  Multiple plain batch pipeline requests ``` [   \"plain-data-goes-here\", \"plain-example-data\" ] ```  ### Response Structure  A list of dictionaries containing the details of the created pipeline version requests with the following fields:  - `id`: Unique identifier for the pipeline version request, which can be used to collect the result  - `pipeline`: Name of the pipeline for which the request is made  - `version`: Name of the pipeline version for which the request is made  - `status`: Status of the request. Always 'pending' when initialised, later it can be 'processing', 'failed' or 'completed'.  - `time_created`: Server time that the request was made (current time)  #### Response Examples  ``` [   {     \"id\": \"69eca481-8576-49e8-8e20-ea56f2005bcb\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"time_created\": \"2020-03-28T20:00:26.613+00:00\"   },   {     \"id\": \"2521378e-263e-4e2e-85e9-a96254b36536\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"time_created\": \"2020-03-28T20:00:26.613+00:00\"   } ] ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.batch_pipeline_version_requests_create_with_http_info(project_name, pipeline_name, version, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -5684,15 +5684,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def deployment_versions_create(self, project_name, deployment_name, data, **kwargs):  # noqa: E501
         """Create deployment versions  # noqa: E501
 
-         ### Description  Create a version for a deployment. The first version of a deployment is set as default. Provide the parameter 'monitoring' as the name of a notification group to send monitoring notifications to. A notification will be sent in the case of a failed/recovered request. Pass `null` to switch off monitoring notifications for this version. Provide the parameter 'default_notification_group' as the name of a notification group to send notifications when requests for the version are completed. Pass `null` to switch off request notifications for this version. This field is only used for versions with **batch deployment mode**.  ### Required Parameters  - `version`: Name of the version of the deployment  ### Optional Parameters  - `language`: Language in which the version is provided. It can be python3.6, python3.7, python3.8, python3.9, python3.6_cuda, python3.7_cuda, python3.8_cuda, python3.9_cuda or r4.0. The default value is python3.7. - `memory_allocation`: (deprecated) Reserved memory for the version in MiB. This value determines the memory allocated to the version: it should be enough to encompass the deployment file and all requirements that need to be installed. The default value is 2048. The minimum and maximum values are 256 and 16384 respectively. - `instance_type`: Reserved instance type for the version. This value determines the allocation of memory to the version: it should be enough to encompass the deployment file and all requirements that need to be installed. The default value is 2048mb. The minimum and maximum values are 256mb and 16384mb respectively. - `maximum_instances`: Upper bound of number of versions running. The default value is 5. *Indicator of resource capacity:* if many deployment requests need to be handled in a short time, this number can be set higher to avoid long waiting times. - `minimum_instances`: Lower bound of number of versions running. The default value is 0. Set this value greater than 0 to always have a always running version. - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped. The default value is 300, the minimum value is 10 (300 for GPU deployments) and the maximum value is 3600. A high value means that the version stays available longer. Sending requests to a running version means that it will be already initialized and thus take a shorter timer.   - `description`: Description for the version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version. It defaults to 604800 seconds (1 week). - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored - `deployment_mode`: the type of the deployment version. It can be one of the following:     - *express* - Direct requests can be made to the deployment version.     - *batch* - Batch requests can be made to the deployment version.  If the time that a request takes does not matter, keep the default values.  #### Request Examples  ``` {   \"version\": \"version-1\",   \"language\": \"python3.8\" } ```  ``` {   \"version\": \"version-1\",   \"language\": \"r4.0\",   \"instance_type\": \"512mb\" } ```  ```   \"version\": \"version-1\",   \"language\": \"python3.6_cuda\",   \"instance_type\": \"16384mb_t4\",   \"maximum_instances\": 1 ```  ``` {   \"version\": \"version-1\",   \"maximum_instances\": 4,   \"minimum_instances\": 1,   \"monitoring\": \"notification-group-1\" } ```  ### Response Structure  Details of the created version - `id`: Unique identifier for the deployment (UUID) - `deployment`: Deployment name to which the version is associated - `version`: Version name - `description`: Description of the version - `language`: Language in which the version is provided - `status`: The status of the version - `active_revision`: Active revision of the version. It is initialised as None since there are no deployment files uploaded for the version yet. - `latest_build`: Latest build of the version. It is initialised as None since no build is triggered for the version yet. - `memory_allocation`: (deprecated) Reserved memory for the version in MiB - `instance_type`: The reserved instance type for the version - `maximum_instances`: Upper bound of number of versions running - `minimum_instances`: Lower bound of number of versions running - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the version was created - `last_updated`: The date when the version was last updated - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following: *none*, *metadata* or *full*. - `deployment_mode`: the type of the deployment version  #### Response Examples  ``` {   \"id\": \"4ae7d14b-4803-4e16-b96d-3b18caa4b605\",   \"deployment\": \"deployment-1\",   \"version\": \"version-1\",   \"description\": \"\",   \"language\": \"python3.8\",   \"status\": \"unavailable\",   \"active_revision\": null,   \"latest_build\": null,   \"memory_allocation\": 512,   \"instance_type\": \"512mb\",   \"maximum_instances\": 5,   \"minimum_instances\": 0,   \"maximum_idle_time\": 10,   \"labels\": {     \"type\": \"version\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-05-12T16:23:15.456812Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"deployment_mode\": \"express\" } ```   # noqa: E501
+         ### Description  Create a version for a deployment. The first version of a deployment is set as default. Provide the parameter 'monitoring' as the name of a notification group to send monitoring notifications to. A notification will be sent in the case of a failed/recovered request. Pass `null` to switch off monitoring notifications for this version. Provide the parameter 'default_notification_group' as the name of a notification group to send notifications when requests for the version are completed. Pass `null` to switch off request notifications for this version.  ### Required Parameters  - `version`: Name of the version of the deployment  ### Optional Parameters  - `language`: Language in which the version is provided. It can be python3.6, python3.7, python3.8, python3.9, python3.6_cuda, python3.7_cuda, python3.8_cuda, python3.9_cuda or r4.0. The default value is python3.7. - `memory_allocation`: (deprecated) Reserved memory for the version in MiB. This value determines the memory allocated to the version: it should be enough to encompass the deployment file and all requirements that need to be installed. The default value is 2048. The minimum and maximum values are 256 and 16384 respectively. - `instance_type`: Reserved instance type for the version. This value determines the allocation of memory to the version: it should be enough to encompass the deployment file and all requirements that need to be installed. The default value is 2048mb. The minimum and maximum values are 256mb and 16384mb respectively. - `maximum_instances`: Upper bound of number of versions running. The default value is 5. *Indicator of resource capacity:* if many deployment requests need to be handled in a short time, this number can be set higher to avoid long waiting times. - `minimum_instances`: Lower bound of number of versions running. The default value is 0. Set this value greater than 0 to always have a always running version. - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped. The default value is 300, the minimum value is 10 (300 for GPU deployments) and the maximum value is 3600. A high value means that the version stays available longer. Sending requests to a running version means that it will be already initialized and thus take a shorter timer.   - `description`: Description for the version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version. It defaults to 604800 seconds (1 week). - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored  If the time that a request takes does not matter, keep the default values.  #### Request Examples  ``` {   \"version\": \"version-1\",   \"language\": \"python3.8\" } ```  ``` {   \"version\": \"version-1\",   \"language\": \"r4.0\",   \"instance_type\": \"512mb\" } ```  ```   \"version\": \"version-1\",   \"language\": \"python3.6_cuda\",   \"instance_type\": \"16384mb_t4\",   \"maximum_instances\": 1 ```  ``` {   \"version\": \"version-1\",   \"maximum_instances\": 4,   \"minimum_instances\": 1,   \"monitoring\": \"notification-group-1\" } ```  ### Response Structure  Details of the created version - `id`: Unique identifier for the deployment (UUID) - `deployment`: Deployment name to which the version is associated - `version`: Version name - `description`: Description of the version - `language`: Language in which the version is provided - `status`: The status of the version - `active_revision`: Active revision of the version. It is initialised as None since there are no deployment files uploaded for the version yet. - `latest_build`: Latest build of the version. It is initialised as None since no build is triggered for the version yet. - `memory_allocation`: (deprecated) Reserved memory for the version in MiB - `instance_type`: The reserved instance type for the version - `maximum_instances`: Upper bound of number of versions running - `minimum_instances`: Lower bound of number of versions running - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the version was created - `last_updated`: The date when the version was last updated - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following: *none*, *metadata* or *full*.  #### Response Examples  ``` {   \"id\": \"4ae7d14b-4803-4e16-b96d-3b18caa4b605\",   \"deployment\": \"deployment-1\",   \"version\": \"version-1\",   \"description\": \"\",   \"language\": \"python3.8\",   \"status\": \"unavailable\",   \"active_revision\": null,   \"latest_build\": null,   \"memory_allocation\": 512,   \"instance_type\": \"512mb\",   \"maximum_instances\": 5,   \"minimum_instances\": 0,   \"maximum_idle_time\": 10,   \"labels\": {     \"type\": \"version\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-05-12T16:23:15.456812Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\" } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.deployment_versions_create(project_name, deployment_name, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -5711,15 +5711,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.deployment_versions_create_with_http_info(project_name, deployment_name, data, **kwargs)  # noqa: E501
 
     def deployment_versions_create_with_http_info(self, project_name, deployment_name, data, **kwargs):  # noqa: E501
         """Create deployment versions  # noqa: E501
 
-         ### Description  Create a version for a deployment. The first version of a deployment is set as default. Provide the parameter 'monitoring' as the name of a notification group to send monitoring notifications to. A notification will be sent in the case of a failed/recovered request. Pass `null` to switch off monitoring notifications for this version. Provide the parameter 'default_notification_group' as the name of a notification group to send notifications when requests for the version are completed. Pass `null` to switch off request notifications for this version. This field is only used for versions with **batch deployment mode**.  ### Required Parameters  - `version`: Name of the version of the deployment  ### Optional Parameters  - `language`: Language in which the version is provided. It can be python3.6, python3.7, python3.8, python3.9, python3.6_cuda, python3.7_cuda, python3.8_cuda, python3.9_cuda or r4.0. The default value is python3.7. - `memory_allocation`: (deprecated) Reserved memory for the version in MiB. This value determines the memory allocated to the version: it should be enough to encompass the deployment file and all requirements that need to be installed. The default value is 2048. The minimum and maximum values are 256 and 16384 respectively. - `instance_type`: Reserved instance type for the version. This value determines the allocation of memory to the version: it should be enough to encompass the deployment file and all requirements that need to be installed. The default value is 2048mb. The minimum and maximum values are 256mb and 16384mb respectively. - `maximum_instances`: Upper bound of number of versions running. The default value is 5. *Indicator of resource capacity:* if many deployment requests need to be handled in a short time, this number can be set higher to avoid long waiting times. - `minimum_instances`: Lower bound of number of versions running. The default value is 0. Set this value greater than 0 to always have a always running version. - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped. The default value is 300, the minimum value is 10 (300 for GPU deployments) and the maximum value is 3600. A high value means that the version stays available longer. Sending requests to a running version means that it will be already initialized and thus take a shorter timer.   - `description`: Description for the version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version. It defaults to 604800 seconds (1 week). - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored - `deployment_mode`: the type of the deployment version. It can be one of the following:     - *express* - Direct requests can be made to the deployment version.     - *batch* - Batch requests can be made to the deployment version.  If the time that a request takes does not matter, keep the default values.  #### Request Examples  ``` {   \"version\": \"version-1\",   \"language\": \"python3.8\" } ```  ``` {   \"version\": \"version-1\",   \"language\": \"r4.0\",   \"instance_type\": \"512mb\" } ```  ```   \"version\": \"version-1\",   \"language\": \"python3.6_cuda\",   \"instance_type\": \"16384mb_t4\",   \"maximum_instances\": 1 ```  ``` {   \"version\": \"version-1\",   \"maximum_instances\": 4,   \"minimum_instances\": 1,   \"monitoring\": \"notification-group-1\" } ```  ### Response Structure  Details of the created version - `id`: Unique identifier for the deployment (UUID) - `deployment`: Deployment name to which the version is associated - `version`: Version name - `description`: Description of the version - `language`: Language in which the version is provided - `status`: The status of the version - `active_revision`: Active revision of the version. It is initialised as None since there are no deployment files uploaded for the version yet. - `latest_build`: Latest build of the version. It is initialised as None since no build is triggered for the version yet. - `memory_allocation`: (deprecated) Reserved memory for the version in MiB - `instance_type`: The reserved instance type for the version - `maximum_instances`: Upper bound of number of versions running - `minimum_instances`: Lower bound of number of versions running - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the version was created - `last_updated`: The date when the version was last updated - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following: *none*, *metadata* or *full*. - `deployment_mode`: the type of the deployment version  #### Response Examples  ``` {   \"id\": \"4ae7d14b-4803-4e16-b96d-3b18caa4b605\",   \"deployment\": \"deployment-1\",   \"version\": \"version-1\",   \"description\": \"\",   \"language\": \"python3.8\",   \"status\": \"unavailable\",   \"active_revision\": null,   \"latest_build\": null,   \"memory_allocation\": 512,   \"instance_type\": \"512mb\",   \"maximum_instances\": 5,   \"minimum_instances\": 0,   \"maximum_idle_time\": 10,   \"labels\": {     \"type\": \"version\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-05-12T16:23:15.456812Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"deployment_mode\": \"express\" } ```   # noqa: E501
+         ### Description  Create a version for a deployment. The first version of a deployment is set as default. Provide the parameter 'monitoring' as the name of a notification group to send monitoring notifications to. A notification will be sent in the case of a failed/recovered request. Pass `null` to switch off monitoring notifications for this version. Provide the parameter 'default_notification_group' as the name of a notification group to send notifications when requests for the version are completed. Pass `null` to switch off request notifications for this version.  ### Required Parameters  - `version`: Name of the version of the deployment  ### Optional Parameters  - `language`: Language in which the version is provided. It can be python3.6, python3.7, python3.8, python3.9, python3.6_cuda, python3.7_cuda, python3.8_cuda, python3.9_cuda or r4.0. The default value is python3.7. - `memory_allocation`: (deprecated) Reserved memory for the version in MiB. This value determines the memory allocated to the version: it should be enough to encompass the deployment file and all requirements that need to be installed. The default value is 2048. The minimum and maximum values are 256 and 16384 respectively. - `instance_type`: Reserved instance type for the version. This value determines the allocation of memory to the version: it should be enough to encompass the deployment file and all requirements that need to be installed. The default value is 2048mb. The minimum and maximum values are 256mb and 16384mb respectively. - `maximum_instances`: Upper bound of number of versions running. The default value is 5. *Indicator of resource capacity:* if many deployment requests need to be handled in a short time, this number can be set higher to avoid long waiting times. - `minimum_instances`: Lower bound of number of versions running. The default value is 0. Set this value greater than 0 to always have a always running version. - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped. The default value is 300, the minimum value is 10 (300 for GPU deployments) and the maximum value is 3600. A high value means that the version stays available longer. Sending requests to a running version means that it will be already initialized and thus take a shorter timer.   - `description`: Description for the version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version. It defaults to 604800 seconds (1 week). - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored  If the time that a request takes does not matter, keep the default values.  #### Request Examples  ``` {   \"version\": \"version-1\",   \"language\": \"python3.8\" } ```  ``` {   \"version\": \"version-1\",   \"language\": \"r4.0\",   \"instance_type\": \"512mb\" } ```  ```   \"version\": \"version-1\",   \"language\": \"python3.6_cuda\",   \"instance_type\": \"16384mb_t4\",   \"maximum_instances\": 1 ```  ``` {   \"version\": \"version-1\",   \"maximum_instances\": 4,   \"minimum_instances\": 1,   \"monitoring\": \"notification-group-1\" } ```  ### Response Structure  Details of the created version - `id`: Unique identifier for the deployment (UUID) - `deployment`: Deployment name to which the version is associated - `version`: Version name - `description`: Description of the version - `language`: Language in which the version is provided - `status`: The status of the version - `active_revision`: Active revision of the version. It is initialised as None since there are no deployment files uploaded for the version yet. - `latest_build`: Latest build of the version. It is initialised as None since no build is triggered for the version yet. - `memory_allocation`: (deprecated) Reserved memory for the version in MiB - `instance_type`: The reserved instance type for the version - `maximum_instances`: Upper bound of number of versions running - `minimum_instances`: Lower bound of number of versions running - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the version was created - `last_updated`: The date when the version was last updated - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following: *none*, *metadata* or *full*.  #### Response Examples  ``` {   \"id\": \"4ae7d14b-4803-4e16-b96d-3b18caa4b605\",   \"deployment\": \"deployment-1\",   \"version\": \"version-1\",   \"description\": \"\",   \"language\": \"python3.8\",   \"status\": \"unavailable\",   \"active_revision\": null,   \"latest_build\": null,   \"memory_allocation\": 512,   \"instance_type\": \"512mb\",   \"maximum_instances\": 5,   \"minimum_instances\": 0,   \"maximum_idle_time\": 10,   \"labels\": {     \"type\": \"version\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-05-12T16:23:15.456812Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\" } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.deployment_versions_create_with_http_info(project_name, deployment_name, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -5958,15 +5958,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def deployment_versions_get(self, project_name, deployment_name, version, **kwargs):  # noqa: E501
         """Get deployment version  # noqa: E501
 
-         ### Description  Retrieve details of a version of a deployment in a project  ### Response Structure  Details of a version - `id`: Unique identifier for the version (UUID) - `deployment`: Deployment name to which the version is associated - `version`: Version name - `description`: Description of the version - `language`: Language in which the version is provided - `status`: The status of the version - `active_revision`: UUID of the active revision of the version. If no deployment files have been uploaded yet, it is None. - `latest_build`: UUID of the latest build of the version. If no build has been triggered yet, it is None. - `memory_allocation`: (deprecated) Reserved memory for the version in MiB - `instance_type`: The reserved instance type for the version - `maximum_instances`: Upper bound of number of deployment pods running in parallel - `minimum_instances`: Lower bound of number of deployment pods running in parallel - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the version was created - `last_updated`: The date when the version was last updated - `last_file_upload`: The date when a deployment file was last uploaded for the version - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored  - `deployment_mode`: the type of the deployment version  #### Response Examples ``` {   \"id\": \"4ae7d14b-4803-4e16-b96d-3b18caa4b605\",   \"deployment\": \"deployment-1\",   \"version\": \"version-1\",   \"description\": \"\",   \"language\": \"python3.7\",   \"status\": \"available\",   \"active_revision\": \"a74662be-c938-4104-872a-8be1b85f64ff\",   \"latest_build\": \"9f7fd6ec-53b7-41c6-949e-09efc2ee2d31\",   \"memory_allocation\": 512,   \"instance_type\": \"512mb\",   \"maximum_instances\": 4,   \"minimum_instances\": 1,   \"maximum_idle_time\": 10,   \"labels\": {     \"type\": \"version\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"last_file_uploaded\": \"2020-06-21T09:03:01.875391Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"deployment_mode\": \"express\" } ```   # noqa: E501
+         ### Description  Retrieve details of a version of a deployment in a project  ### Response Structure  Details of a version - `id`: Unique identifier for the version (UUID) - `deployment`: Deployment name to which the version is associated - `version`: Version name - `description`: Description of the version - `language`: Language in which the version is provided - `status`: The status of the version - `active_revision`: UUID of the active revision of the version. If no deployment files have been uploaded yet, it is None. - `latest_build`: UUID of the latest build of the version. If no build has been triggered yet, it is None. - `memory_allocation`: (deprecated) Reserved memory for the version in MiB - `instance_type`: The reserved instance type for the version - `maximum_instances`: Upper bound of number of deployment pods running in parallel - `minimum_instances`: Lower bound of number of deployment pods running in parallel - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the version was created - `last_updated`: The date when the version was last updated - `last_file_upload`: The date when a deployment file was last uploaded for the version - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored  #### Response Examples ``` {   \"id\": \"4ae7d14b-4803-4e16-b96d-3b18caa4b605\",   \"deployment\": \"deployment-1\",   \"version\": \"version-1\",   \"description\": \"\",   \"language\": \"python3.7\",   \"status\": \"available\",   \"active_revision\": \"a74662be-c938-4104-872a-8be1b85f64ff\",   \"latest_build\": \"9f7fd6ec-53b7-41c6-949e-09efc2ee2d31\",   \"memory_allocation\": 512,   \"instance_type\": \"512mb\",   \"maximum_instances\": 4,   \"minimum_instances\": 1,   \"maximum_idle_time\": 10,   \"labels\": {     \"type\": \"version\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"last_file_uploaded\": \"2020-06-21T09:03:01.875391Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\" } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.deployment_versions_get(project_name, deployment_name, version, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -5985,15 +5985,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.deployment_versions_get_with_http_info(project_name, deployment_name, version, **kwargs)  # noqa: E501
 
     def deployment_versions_get_with_http_info(self, project_name, deployment_name, version, **kwargs):  # noqa: E501
         """Get deployment version  # noqa: E501
 
-         ### Description  Retrieve details of a version of a deployment in a project  ### Response Structure  Details of a version - `id`: Unique identifier for the version (UUID) - `deployment`: Deployment name to which the version is associated - `version`: Version name - `description`: Description of the version - `language`: Language in which the version is provided - `status`: The status of the version - `active_revision`: UUID of the active revision of the version. If no deployment files have been uploaded yet, it is None. - `latest_build`: UUID of the latest build of the version. If no build has been triggered yet, it is None. - `memory_allocation`: (deprecated) Reserved memory for the version in MiB - `instance_type`: The reserved instance type for the version - `maximum_instances`: Upper bound of number of deployment pods running in parallel - `minimum_instances`: Lower bound of number of deployment pods running in parallel - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the version was created - `last_updated`: The date when the version was last updated - `last_file_upload`: The date when a deployment file was last uploaded for the version - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored  - `deployment_mode`: the type of the deployment version  #### Response Examples ``` {   \"id\": \"4ae7d14b-4803-4e16-b96d-3b18caa4b605\",   \"deployment\": \"deployment-1\",   \"version\": \"version-1\",   \"description\": \"\",   \"language\": \"python3.7\",   \"status\": \"available\",   \"active_revision\": \"a74662be-c938-4104-872a-8be1b85f64ff\",   \"latest_build\": \"9f7fd6ec-53b7-41c6-949e-09efc2ee2d31\",   \"memory_allocation\": 512,   \"instance_type\": \"512mb\",   \"maximum_instances\": 4,   \"minimum_instances\": 1,   \"maximum_idle_time\": 10,   \"labels\": {     \"type\": \"version\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"last_file_uploaded\": \"2020-06-21T09:03:01.875391Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"deployment_mode\": \"express\" } ```   # noqa: E501
+         ### Description  Retrieve details of a version of a deployment in a project  ### Response Structure  Details of a version - `id`: Unique identifier for the version (UUID) - `deployment`: Deployment name to which the version is associated - `version`: Version name - `description`: Description of the version - `language`: Language in which the version is provided - `status`: The status of the version - `active_revision`: UUID of the active revision of the version. If no deployment files have been uploaded yet, it is None. - `latest_build`: UUID of the latest build of the version. If no build has been triggered yet, it is None. - `memory_allocation`: (deprecated) Reserved memory for the version in MiB - `instance_type`: The reserved instance type for the version - `maximum_instances`: Upper bound of number of deployment pods running in parallel - `minimum_instances`: Lower bound of number of deployment pods running in parallel - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the version was created - `last_updated`: The date when the version was last updated - `last_file_upload`: The date when a deployment file was last uploaded for the version - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored  #### Response Examples ``` {   \"id\": \"4ae7d14b-4803-4e16-b96d-3b18caa4b605\",   \"deployment\": \"deployment-1\",   \"version\": \"version-1\",   \"description\": \"\",   \"language\": \"python3.7\",   \"status\": \"available\",   \"active_revision\": \"a74662be-c938-4104-872a-8be1b85f64ff\",   \"latest_build\": \"9f7fd6ec-53b7-41c6-949e-09efc2ee2d31\",   \"memory_allocation\": 512,   \"instance_type\": \"512mb\",   \"maximum_instances\": 4,   \"minimum_instances\": 1,   \"maximum_idle_time\": 10,   \"labels\": {     \"type\": \"version\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"last_file_uploaded\": \"2020-06-21T09:03:01.875391Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\" } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.deployment_versions_get_with_http_info(project_name, deployment_name, version, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -6094,15 +6094,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def deployment_versions_list(self, project_name, deployment_name, **kwargs):  # noqa: E501
         """List deployment versions  # noqa: E501
 
-         ### Description  Versions can be filtered according to the labels they have by giving labels as a query parameter. Versions that have at least one of the labels on which is filtered, are returned.  ### Optional Parameters - `labels`: Filter on labels of the version. Should be given in the format 'label:label_value'. Separate multiple label-pairs with a comma (,). This parameter should be given as query parameter.  ### Response Structure  A list of details of the versions - `id`: Unique identifier for the deployment (UUID) - `deployment`: Deployment name to which the version is associated - `version`: Version name - `description`: Description of the version - `language`: Language in which the version is provided - `status`: The status of the version - `active_revision`: UUID of the active revision of the version. If no deployment files have been uploaded yet, it is None. - `latest_build`: UUID of the latest build of the version. If no build has been triggered yet, it is None. - `memory_allocation`: (deprecated) Reserved memory usage for the version in MiB - `instance_type`: The reserved instance type for the version - `maximum_instances`: Upper bound of number of versions running - `minimum_instances`: Lower bound of number of versions running - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the version was created - `last_updated`: The date when the version was last updated - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored - `deployment_mode`: the type of the deployment version  #### Response Examples ``` [   {     \"id\": \"4ae7d14b-4803-4e16-b96d-3b18caa4b605\",     \"deployment\": \"deployment-1\",     \"version\": \"version-1\",     \"description\": \"\",     \"language\": \"python3.8\",     \"status\": \"available\",     \"active_revision\": \"da27ef7c-aa3f-4963-a815-6ebf1865638e\",     \"latest_build\": \"0f4a94c6-ec4c-4d1e-81d7-8f3e40471f75\",     \"memory_allocation\": 512,     \"instance_type\": \"512mb\",     \"maximum_instances\": 4,     \"minimum_instances\": 1,     \"maximum_idle_time\": 10,     \"labels\": {       \"type\": \"version\"     },     \"creation_date\": \"2020-06-18T08:32:14.876451Z\",     \"last_updated\": \"2020-06-19T10:52:23.124784Z\",     \"monitoring\": \"notification-group-1\",     \"default_notification_group\": null,     \"request_retention_time\": 604800,     \"request_retention_mode\": \"full\",     \"deployment_mode\": \"express\"   },   {     \"id\": \"24f6b80a-08c3-4d52-ac1a-2ea7e70f16a6\",     \"deployment\": \"deployment-1\",     \"version\": \"version-2\",     \"description\": \"\",     \"language\": \"r4.0\",     \"status\": \"available\",     \"active_revision\": \"a74662be-c938-4104-872a-8be1b85f64ff\",     \"latest_build\": \"4534e479-ea2e-4161-876a-1d382191a031\",     \"memory_allocation\": 256,     \"instance_type\": \"256mb\",     \"maximum_instances\": 5,     \"minimum_instances\": 0,     \"maximum_idle_time\": 10,     \"labels\": {       \"type\": \"version\"     },     \"creation_date\": \"2020-05-12T16:23:15.456812Z\",     \"last_updated\": \"2020-06-22T18:04:76.123754Z\",     \"monitoring\": \"notification-group-2\",     \"default_notification_group\": \"notification-group-2\",     \"request_retention_time\": 86400,     \"request_retention_mode\": \"metadata\",     \"deployment_mode\": \"batch\"   } ] ```   # noqa: E501
+         ### Description  Versions can be filtered according to the labels they have by giving labels as a query parameter. Versions that have at least one of the labels on which is filtered, are returned.  ### Optional Parameters - `labels`: Filter on labels of the version. Should be given in the format 'label:label_value'. Separate multiple label-pairs with a comma (,). This parameter should be given as query parameter.  ### Response Structure  A list of details of the versions - `id`: Unique identifier for the deployment (UUID) - `deployment`: Deployment name to which the version is associated - `version`: Version name - `description`: Description of the version - `language`: Language in which the version is provided - `status`: The status of the version - `active_revision`: UUID of the active revision of the version. If no deployment files have been uploaded yet, it is None. - `latest_build`: UUID of the latest build of the version. If no build has been triggered yet, it is None. - `memory_allocation`: (deprecated) Reserved memory usage for the version in MiB - `instance_type`: The reserved instance type for the version - `maximum_instances`: Upper bound of number of versions running - `minimum_instances`: Lower bound of number of versions running - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the version was created - `last_updated`: The date when the version was last updated - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored  #### Response Examples ``` [   {     \"id\": \"4ae7d14b-4803-4e16-b96d-3b18caa4b605\",     \"deployment\": \"deployment-1\",     \"version\": \"version-1\",     \"description\": \"\",     \"language\": \"python3.8\",     \"status\": \"available\",     \"active_revision\": \"da27ef7c-aa3f-4963-a815-6ebf1865638e\",     \"latest_build\": \"0f4a94c6-ec4c-4d1e-81d7-8f3e40471f75\",     \"memory_allocation\": 512,     \"instance_type\": \"512mb\",     \"maximum_instances\": 4,     \"minimum_instances\": 1,     \"maximum_idle_time\": 10,     \"labels\": {       \"type\": \"version\"     },     \"creation_date\": \"2020-06-18T08:32:14.876451Z\",     \"last_updated\": \"2020-06-19T10:52:23.124784Z\",     \"monitoring\": \"notification-group-1\",     \"default_notification_group\": null,     \"request_retention_time\": 604800,     \"request_retention_mode\": \"full\"   },   {     \"id\": \"24f6b80a-08c3-4d52-ac1a-2ea7e70f16a6\",     \"deployment\": \"deployment-1\",     \"version\": \"version-2\",     \"description\": \"\",     \"language\": \"r4.0\",     \"status\": \"available\",     \"active_revision\": \"a74662be-c938-4104-872a-8be1b85f64ff\",     \"latest_build\": \"4534e479-ea2e-4161-876a-1d382191a031\",     \"memory_allocation\": 256,     \"instance_type\": \"256mb\",     \"maximum_instances\": 5,     \"minimum_instances\": 0,     \"maximum_idle_time\": 10,     \"labels\": {       \"type\": \"version\"     },     \"creation_date\": \"2020-05-12T16:23:15.456812Z\",     \"last_updated\": \"2020-06-22T18:04:76.123754Z\",     \"monitoring\": \"notification-group-2\",     \"default_notification_group\": \"notification-group-2\",     \"request_retention_time\": 86400,     \"request_retention_mode\": \"metadata\"   } ] ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.deployment_versions_list(project_name, deployment_name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -6121,15 +6121,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.deployment_versions_list_with_http_info(project_name, deployment_name, **kwargs)  # noqa: E501
 
     def deployment_versions_list_with_http_info(self, project_name, deployment_name, **kwargs):  # noqa: E501
         """List deployment versions  # noqa: E501
 
-         ### Description  Versions can be filtered according to the labels they have by giving labels as a query parameter. Versions that have at least one of the labels on which is filtered, are returned.  ### Optional Parameters - `labels`: Filter on labels of the version. Should be given in the format 'label:label_value'. Separate multiple label-pairs with a comma (,). This parameter should be given as query parameter.  ### Response Structure  A list of details of the versions - `id`: Unique identifier for the deployment (UUID) - `deployment`: Deployment name to which the version is associated - `version`: Version name - `description`: Description of the version - `language`: Language in which the version is provided - `status`: The status of the version - `active_revision`: UUID of the active revision of the version. If no deployment files have been uploaded yet, it is None. - `latest_build`: UUID of the latest build of the version. If no build has been triggered yet, it is None. - `memory_allocation`: (deprecated) Reserved memory usage for the version in MiB - `instance_type`: The reserved instance type for the version - `maximum_instances`: Upper bound of number of versions running - `minimum_instances`: Lower bound of number of versions running - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the version was created - `last_updated`: The date when the version was last updated - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored - `deployment_mode`: the type of the deployment version  #### Response Examples ``` [   {     \"id\": \"4ae7d14b-4803-4e16-b96d-3b18caa4b605\",     \"deployment\": \"deployment-1\",     \"version\": \"version-1\",     \"description\": \"\",     \"language\": \"python3.8\",     \"status\": \"available\",     \"active_revision\": \"da27ef7c-aa3f-4963-a815-6ebf1865638e\",     \"latest_build\": \"0f4a94c6-ec4c-4d1e-81d7-8f3e40471f75\",     \"memory_allocation\": 512,     \"instance_type\": \"512mb\",     \"maximum_instances\": 4,     \"minimum_instances\": 1,     \"maximum_idle_time\": 10,     \"labels\": {       \"type\": \"version\"     },     \"creation_date\": \"2020-06-18T08:32:14.876451Z\",     \"last_updated\": \"2020-06-19T10:52:23.124784Z\",     \"monitoring\": \"notification-group-1\",     \"default_notification_group\": null,     \"request_retention_time\": 604800,     \"request_retention_mode\": \"full\",     \"deployment_mode\": \"express\"   },   {     \"id\": \"24f6b80a-08c3-4d52-ac1a-2ea7e70f16a6\",     \"deployment\": \"deployment-1\",     \"version\": \"version-2\",     \"description\": \"\",     \"language\": \"r4.0\",     \"status\": \"available\",     \"active_revision\": \"a74662be-c938-4104-872a-8be1b85f64ff\",     \"latest_build\": \"4534e479-ea2e-4161-876a-1d382191a031\",     \"memory_allocation\": 256,     \"instance_type\": \"256mb\",     \"maximum_instances\": 5,     \"minimum_instances\": 0,     \"maximum_idle_time\": 10,     \"labels\": {       \"type\": \"version\"     },     \"creation_date\": \"2020-05-12T16:23:15.456812Z\",     \"last_updated\": \"2020-06-22T18:04:76.123754Z\",     \"monitoring\": \"notification-group-2\",     \"default_notification_group\": \"notification-group-2\",     \"request_retention_time\": 86400,     \"request_retention_mode\": \"metadata\",     \"deployment_mode\": \"batch\"   } ] ```   # noqa: E501
+         ### Description  Versions can be filtered according to the labels they have by giving labels as a query parameter. Versions that have at least one of the labels on which is filtered, are returned.  ### Optional Parameters - `labels`: Filter on labels of the version. Should be given in the format 'label:label_value'. Separate multiple label-pairs with a comma (,). This parameter should be given as query parameter.  ### Response Structure  A list of details of the versions - `id`: Unique identifier for the deployment (UUID) - `deployment`: Deployment name to which the version is associated - `version`: Version name - `description`: Description of the version - `language`: Language in which the version is provided - `status`: The status of the version - `active_revision`: UUID of the active revision of the version. If no deployment files have been uploaded yet, it is None. - `latest_build`: UUID of the latest build of the version. If no build has been triggered yet, it is None. - `memory_allocation`: (deprecated) Reserved memory usage for the version in MiB - `instance_type`: The reserved instance type for the version - `maximum_instances`: Upper bound of number of versions running - `minimum_instances`: Lower bound of number of versions running - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the version was created - `last_updated`: The date when the version was last updated - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored  #### Response Examples ``` [   {     \"id\": \"4ae7d14b-4803-4e16-b96d-3b18caa4b605\",     \"deployment\": \"deployment-1\",     \"version\": \"version-1\",     \"description\": \"\",     \"language\": \"python3.8\",     \"status\": \"available\",     \"active_revision\": \"da27ef7c-aa3f-4963-a815-6ebf1865638e\",     \"latest_build\": \"0f4a94c6-ec4c-4d1e-81d7-8f3e40471f75\",     \"memory_allocation\": 512,     \"instance_type\": \"512mb\",     \"maximum_instances\": 4,     \"minimum_instances\": 1,     \"maximum_idle_time\": 10,     \"labels\": {       \"type\": \"version\"     },     \"creation_date\": \"2020-06-18T08:32:14.876451Z\",     \"last_updated\": \"2020-06-19T10:52:23.124784Z\",     \"monitoring\": \"notification-group-1\",     \"default_notification_group\": null,     \"request_retention_time\": 604800,     \"request_retention_mode\": \"full\"   },   {     \"id\": \"24f6b80a-08c3-4d52-ac1a-2ea7e70f16a6\",     \"deployment\": \"deployment-1\",     \"version\": \"version-2\",     \"description\": \"\",     \"language\": \"r4.0\",     \"status\": \"available\",     \"active_revision\": \"a74662be-c938-4104-872a-8be1b85f64ff\",     \"latest_build\": \"4534e479-ea2e-4161-876a-1d382191a031\",     \"memory_allocation\": 256,     \"instance_type\": \"256mb\",     \"maximum_instances\": 5,     \"minimum_instances\": 0,     \"maximum_idle_time\": 10,     \"labels\": {       \"type\": \"version\"     },     \"creation_date\": \"2020-05-12T16:23:15.456812Z\",     \"last_updated\": \"2020-06-22T18:04:76.123754Z\",     \"monitoring\": \"notification-group-2\",     \"default_notification_group\": \"notification-group-2\",     \"request_retention_time\": 86400,     \"request_retention_mode\": \"metadata\"   } ] ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.deployment_versions_list_with_http_info(project_name, deployment_name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -6226,15 +6226,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def deployment_versions_update(self, project_name, deployment_name, version, data, **kwargs):  # noqa: E501
         """Update deployment version  # noqa: E501
 
-         ### Description  Update a version of a deployment in a project. All necessary fields are validated again. When updating labels, the labels will replace the existing value for labels. Provide the parameter 'monitoring' as the name of a notification group to send monitoring notifications to. A notification will be sent in the case of a failed/recovered request. Pass `null` to switch off monitoring notifications for this version. Provide the parameter 'default_notification_group' as the name of a notification group to send notifications when requests for the version are completed. Pass `null` to switch off request notifications for this version. This field is only used for versions with **batch deployment mode**.  ### Optional Parameters  - `version`: New name for the version - `memory_allocation`: (deprecated) New reserved memory for the version in MiB - `instance_type`: New instance type for the version - `maximum_instances`: New upper bound of number of versions running - `minimum_instances`: New lower bound of number of versions running - `maximum_idle_time`: New maximum time in seconds a version stays idle before it is stopped - `description`: New description for the version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label. The new labels will replace the existing value for labels. - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored  #### Request Examples  ``` {   \"version\": \"new-version\" } ```  ``` {   \"instance_type\": \"512mb\",   \"maximum_instances\": 4,   \"minimum_instances\": 1,   \"monitoring\": \"notification-group-1\" } ```  ### Response Structure  Details of the updated version - `id`: Unique identifier for the deployment (UUID) - `deployment`: Deployment name to which the version is associated - `version`: Version name - `description`: Description of the version - `language`: Language in which the version is provided - `status`: The status of the version - `active_revision`: UUID of the active revision of the version. If no deployment files have been uploaded yet, it is None. - `latest_build`: UUID of the latest build of the version. If no build has been triggered yet, it is None. - `memory_allocation`: (deprecated) Reserved memory for the version in MiB - `instance_type`: The reserved instance type for the version - `maximum_instances`: Upper bound of number of versions running - `minimum_instances`: Lower bound of number of versions running - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the version was created - `last_updated`: The date when the version was last updated - `last_file_upload`: The date when a deployment file was last uploaded for the version - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following: *none*, *metadata* or *full*. - `deployment_mode`: the type of the deployment version  #### Response Examples  ``` {   \"id\": \"4ae7d14b-4803-4e16-b96d-3b18caa4b605\",   \"deployment\": \"deployment-1\",   \"version\": \"version-1\",   \"description\": \"\",   \"language\": \"python3.8\",   \"status\": \"available\",   \"active_revision\": \"a74662be-c938-4104-872a-8be1b85f64ff\",   \"latest_build\": \"0d07337e-96d6-4ce6-8c63-c2f07edd2ce4\",   \"memory_allocation\": 512,   \"instance_type\": \"512mb\",   \"maximum_instances\": 4,   \"minimum_instances\": 1,   \"maximum_idle_time\": 10,   \"labels\": {     \"type\": \"version\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-23T18:04:76.123754Z\",   \"last_file_uploaded\": \"2020-06-21T09:03:01.875391Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"deployment_mode\": \"express\" } ```   # noqa: E501
+         ### Description  Update a version of a deployment in a project. All necessary fields are validated again. When updating labels, the labels will replace the existing value for labels. Provide the parameter 'monitoring' as the name of a notification group to send monitoring notifications to. A notification will be sent in the case of a failed/recovered request. Pass `null` to switch off monitoring notifications for this version. Provide the parameter 'default_notification_group' as the name of a notification group to send notifications when requests for the version are completed. Pass `null` to switch off request notifications for this version.  ### Optional Parameters  - `version`: New name for the version - `memory_allocation`: (deprecated) New reserved memory for the version in MiB - `instance_type`: New instance type for the version - `maximum_instances`: New upper bound of number of versions running - `minimum_instances`: New lower bound of number of versions running - `maximum_idle_time`: New maximum time in seconds a version stays idle before it is stopped - `description`: New description for the version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label. The new labels will replace the existing value for labels. - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored  #### Request Examples  ``` {   \"version\": \"new-version\" } ```  ``` {   \"instance_type\": \"512mb\",   \"maximum_instances\": 4,   \"minimum_instances\": 1,   \"monitoring\": \"notification-group-1\" } ```  ### Response Structure  Details of the updated version - `id`: Unique identifier for the deployment (UUID) - `deployment`: Deployment name to which the version is associated - `version`: Version name - `description`: Description of the version - `language`: Language in which the version is provided - `status`: The status of the version - `active_revision`: UUID of the active revision of the version. If no deployment files have been uploaded yet, it is None. - `latest_build`: UUID of the latest build of the version. If no build has been triggered yet, it is None. - `memory_allocation`: (deprecated) Reserved memory for the version in MiB - `instance_type`: The reserved instance type for the version - `maximum_instances`: Upper bound of number of versions running - `minimum_instances`: Lower bound of number of versions running - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the version was created - `last_updated`: The date when the version was last updated - `last_file_upload`: The date when a deployment file was last uploaded for the version - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following: *none*, *metadata* or *full*.  #### Response Examples  ``` {   \"id\": \"4ae7d14b-4803-4e16-b96d-3b18caa4b605\",   \"deployment\": \"deployment-1\",   \"version\": \"version-1\",   \"description\": \"\",   \"language\": \"python3.8\",   \"status\": \"available\",   \"active_revision\": \"a74662be-c938-4104-872a-8be1b85f64ff\",   \"latest_build\": \"0d07337e-96d6-4ce6-8c63-c2f07edd2ce4\",   \"memory_allocation\": 512,   \"instance_type\": \"512mb\",   \"maximum_instances\": 4,   \"minimum_instances\": 1,   \"maximum_idle_time\": 10,   \"labels\": {     \"type\": \"version\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-23T18:04:76.123754Z\",   \"last_file_uploaded\": \"2020-06-21T09:03:01.875391Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\" } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.deployment_versions_update(project_name, deployment_name, version, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -6254,15 +6254,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.deployment_versions_update_with_http_info(project_name, deployment_name, version, data, **kwargs)  # noqa: E501
 
     def deployment_versions_update_with_http_info(self, project_name, deployment_name, version, data, **kwargs):  # noqa: E501
         """Update deployment version  # noqa: E501
 
-         ### Description  Update a version of a deployment in a project. All necessary fields are validated again. When updating labels, the labels will replace the existing value for labels. Provide the parameter 'monitoring' as the name of a notification group to send monitoring notifications to. A notification will be sent in the case of a failed/recovered request. Pass `null` to switch off monitoring notifications for this version. Provide the parameter 'default_notification_group' as the name of a notification group to send notifications when requests for the version are completed. Pass `null` to switch off request notifications for this version. This field is only used for versions with **batch deployment mode**.  ### Optional Parameters  - `version`: New name for the version - `memory_allocation`: (deprecated) New reserved memory for the version in MiB - `instance_type`: New instance type for the version - `maximum_instances`: New upper bound of number of versions running - `minimum_instances`: New lower bound of number of versions running - `maximum_idle_time`: New maximum time in seconds a version stays idle before it is stopped - `description`: New description for the version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label. The new labels will replace the existing value for labels. - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored  #### Request Examples  ``` {   \"version\": \"new-version\" } ```  ``` {   \"instance_type\": \"512mb\",   \"maximum_instances\": 4,   \"minimum_instances\": 1,   \"monitoring\": \"notification-group-1\" } ```  ### Response Structure  Details of the updated version - `id`: Unique identifier for the deployment (UUID) - `deployment`: Deployment name to which the version is associated - `version`: Version name - `description`: Description of the version - `language`: Language in which the version is provided - `status`: The status of the version - `active_revision`: UUID of the active revision of the version. If no deployment files have been uploaded yet, it is None. - `latest_build`: UUID of the latest build of the version. If no build has been triggered yet, it is None. - `memory_allocation`: (deprecated) Reserved memory for the version in MiB - `instance_type`: The reserved instance type for the version - `maximum_instances`: Upper bound of number of versions running - `minimum_instances`: Lower bound of number of versions running - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the version was created - `last_updated`: The date when the version was last updated - `last_file_upload`: The date when a deployment file was last uploaded for the version - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following: *none*, *metadata* or *full*. - `deployment_mode`: the type of the deployment version  #### Response Examples  ``` {   \"id\": \"4ae7d14b-4803-4e16-b96d-3b18caa4b605\",   \"deployment\": \"deployment-1\",   \"version\": \"version-1\",   \"description\": \"\",   \"language\": \"python3.8\",   \"status\": \"available\",   \"active_revision\": \"a74662be-c938-4104-872a-8be1b85f64ff\",   \"latest_build\": \"0d07337e-96d6-4ce6-8c63-c2f07edd2ce4\",   \"memory_allocation\": 512,   \"instance_type\": \"512mb\",   \"maximum_instances\": 4,   \"minimum_instances\": 1,   \"maximum_idle_time\": 10,   \"labels\": {     \"type\": \"version\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-23T18:04:76.123754Z\",   \"last_file_uploaded\": \"2020-06-21T09:03:01.875391Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"deployment_mode\": \"express\" } ```   # noqa: E501
+         ### Description  Update a version of a deployment in a project. All necessary fields are validated again. When updating labels, the labels will replace the existing value for labels. Provide the parameter 'monitoring' as the name of a notification group to send monitoring notifications to. A notification will be sent in the case of a failed/recovered request. Pass `null` to switch off monitoring notifications for this version. Provide the parameter 'default_notification_group' as the name of a notification group to send notifications when requests for the version are completed. Pass `null` to switch off request notifications for this version.  ### Optional Parameters  - `version`: New name for the version - `memory_allocation`: (deprecated) New reserved memory for the version in MiB - `instance_type`: New instance type for the version - `maximum_instances`: New upper bound of number of versions running - `minimum_instances`: New lower bound of number of versions running - `maximum_idle_time`: New maximum time in seconds a version stays idle before it is stopped - `description`: New description for the version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label. The new labels will replace the existing value for labels. - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored  #### Request Examples  ``` {   \"version\": \"new-version\" } ```  ``` {   \"instance_type\": \"512mb\",   \"maximum_instances\": 4,   \"minimum_instances\": 1,   \"monitoring\": \"notification-group-1\" } ```  ### Response Structure  Details of the updated version - `id`: Unique identifier for the deployment (UUID) - `deployment`: Deployment name to which the version is associated - `version`: Version name - `description`: Description of the version - `language`: Language in which the version is provided - `status`: The status of the version - `active_revision`: UUID of the active revision of the version. If no deployment files have been uploaded yet, it is None. - `latest_build`: UUID of the latest build of the version. If no build has been triggered yet, it is None. - `memory_allocation`: (deprecated) Reserved memory for the version in MiB - `instance_type`: The reserved instance type for the version - `maximum_instances`: Upper bound of number of versions running - `minimum_instances`: Lower bound of number of versions running - `maximum_idle_time`: Maximum time in seconds a version stays idle before it is stopped - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the version was created - `last_updated`: The date when the version was last updated - `last_file_upload`: The date when a deployment file was last uploaded for the version - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the version - `request_retention_mode`: Mode of request retention for requests to the version. It can be one of the following: *none*, *metadata* or *full*.  #### Response Examples  ``` {   \"id\": \"4ae7d14b-4803-4e16-b96d-3b18caa4b605\",   \"deployment\": \"deployment-1\",   \"version\": \"version-1\",   \"description\": \"\",   \"language\": \"python3.8\",   \"status\": \"available\",   \"active_revision\": \"a74662be-c938-4104-872a-8be1b85f64ff\",   \"latest_build\": \"0d07337e-96d6-4ce6-8c63-c2f07edd2ce4\",   \"memory_allocation\": 512,   \"instance_type\": \"512mb\",   \"maximum_instances\": 4,   \"minimum_instances\": 1,   \"maximum_idle_time\": 10,   \"labels\": {     \"type\": \"version\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-23T18:04:76.123754Z\",   \"last_file_uploaded\": \"2020-06-21T09:03:01.875391Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\" } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.deployment_versions_update_with_http_info(project_name, deployment_name, version, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -8267,15 +8267,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def imports_update(self, project_name, import_id, data, **kwargs):  # noqa: E501
         """Confirm an import  # noqa: E501
 
-         ### Description Confirm (and update) an import by selecting the objects in the import  ### Optional Parameters - `deployments`: Dictionary containing the deployments to create - `pipelines`: Dictionary containing the pipelines to create - `environment_variables`: Dictionary containing the project-level environment variables to create  #### Request Examples  ``` {     \"deployments\": {     \"deployment-1: {       \"description\": \"\",       \"labels\": {         \"my-label\": \"my-value\"       },       \"default_version\": \"v1\",       \"versions\": {         \"v1\": {           \"zip\": \"deployments/deployment_deployment-1/versions/deployment_deployment-1_version_v1.zip\",           \"description\": \"\",           \"labels\": {},           \"language\": \"python3.7\",           \"deployment_mode\": \"express\",           \"maximum_idle_time\": 300,           \"maximum_instances\": 5,           \"memory_allocation\": 256,           \"minimum_instances\": 0,           \"environment_variables\": {             \"VERSION_ENV_VAR_1\": {               \"value\": \"my-secret-value\",               \"secret\": true             },             \"VERSION_ENV_VAR_2\": {               \"value\": \"test2\"             }           },           \"request_retention_mode\": \"full\",           \"request_retention_time\": 604800         }       },       \"input_type\": \"structured\",       \"output_type\": \"structured\",       \"input_fields\": [         {           \"name\": \"input\",           \"data_type\": \"double\"         }       ],       \"output_fields\": [         {           \"name\": \"output\",           \"data_type\": \"double\"         }       ],       \"environment_variables\": {         \"DEPLOYMENT_ENV_VAR_1\": {           \"value\": \"my-secret-value\",           \"secret\": true         },         \"DEPLOYMENT_ENV_VAR_2\": {           \"value\": \"test\"         }       }     }   },   \"pipelines\": {     \"pipeline-1: {       \"description\": \"\",       \"labels\": {         \"test\": \"label\"       },       \"default_version\": \"v1\",       \"versions\": {         \"v1\": {           \"description\": \"\",           \"labels\": {},           \"objects\": [             {               \"name\": \"obj-1\",               \"reference_name\": \"deployment-1\",               \"reference_version\": \"v1\"             }           ],           \"attachments\": [             {               \"sources\": [                 {                   \"mapping\": [                     {                       \"source_field_name\": \"input\",                       \"destination_field_name\": \"input\"                     }                   ],                   \"source_name\": \"pipeline_start\"                 }               ],               \"destination_name\": \"obj-1\"             },             {               \"sources\": [                 {                   \"mapping\": [                     {                       \"source_field_name\": \"output\",                       \"destination_field_name\": \"output\"                     }                   ],                   \"source_name\": \"obj-1\"                 }               ],               \"destination_name\": \"pipeline_end\"             }           ],           \"request_retention_mode\": \"full\",           \"request_retention_time\": 604800         }       },       \"input_type\": \"structured\",       \"output_type\": \"structured\",       \"input_fields\": [         {           \"name\": \"input\",           \"data_type\": \"double\"         }       ],       \"output_fields\": [         {           \"name\": \"output\",           \"data_type\": \"double\"         }       ]     }   },   \"environment_variables\": {     \"PROJECT_ENV_VAR_1\": {       \"value\": \"value1\",       \"secret\": true     },     \"PROJECT_ENV_VAR_2\": {       \"value\": \"value2\"     }   } } ```  ### Response Structure Details of the updated import - `id`: Unique identifier for the import (UUID) - `status`: Status of the import - `error_message`: The error message in case of a failure - `creation_date`: The date when the import was created - `size`: Size of the import in bytes  #### Response Examples ``` {   \"id\": \"903ccd12-81d1-46e1-9ac9-b9d70af118de\",   \"status\": \"pending\",   \"error_message\": \"\",   \"creation_date\": \"2020-06-18T08:32:14.876451Z\",   \"size\": null } ```   # noqa: E501
+         ### Description Confirm (and update) an import by selecting the objects in the import  ### Optional Parameters - `deployments`: Dictionary containing the deployments to create - `pipelines`: Dictionary containing the pipelines to create - `environment_variables`: Dictionary containing the project-level environment variables to create  #### Request Examples  ``` {     \"deployments\": {     \"deployment-1: {       \"description\": \"\",       \"labels\": {         \"my-label\": \"my-value\"       },       \"default_version\": \"v1\",       \"versions\": {         \"v1\": {           \"zip\": \"deployments/deployment_deployment-1/versions/deployment_deployment-1_version_v1.zip\",           \"description\": \"\",           \"labels\": {},           \"language\": \"python3.7\",           \"maximum_idle_time\": 300,           \"maximum_instances\": 5,           \"memory_allocation\": 256,           \"minimum_instances\": 0,           \"environment_variables\": {             \"VERSION_ENV_VAR_1\": {               \"value\": \"my-secret-value\",               \"secret\": true             },             \"VERSION_ENV_VAR_2\": {               \"value\": \"test2\"             }           },           \"request_retention_mode\": \"full\",           \"request_retention_time\": 604800         }       },       \"input_type\": \"structured\",       \"output_type\": \"structured\",       \"input_fields\": [         {           \"name\": \"input\",           \"data_type\": \"double\"         }       ],       \"output_fields\": [         {           \"name\": \"output\",           \"data_type\": \"double\"         }       ],       \"environment_variables\": {         \"DEPLOYMENT_ENV_VAR_1\": {           \"value\": \"my-secret-value\",           \"secret\": true         },         \"DEPLOYMENT_ENV_VAR_2\": {           \"value\": \"test\"         }       }     }   },   \"pipelines\": {     \"pipeline-1: {       \"description\": \"\",       \"labels\": {         \"test\": \"label\"       },       \"default_version\": \"v1\",       \"versions\": {         \"v1\": {           \"description\": \"\",           \"labels\": {},           \"objects\": [             {               \"name\": \"obj-1\",               \"reference_name\": \"deployment-1\",               \"reference_version\": \"v1\"             }           ],           \"attachments\": [             {               \"sources\": [                 {                   \"mapping\": [                     {                       \"source_field_name\": \"input\",                       \"destination_field_name\": \"input\"                     }                   ],                   \"source_name\": \"pipeline_start\"                 }               ],               \"destination_name\": \"obj-1\"             },             {               \"sources\": [                 {                   \"mapping\": [                     {                       \"source_field_name\": \"output\",                       \"destination_field_name\": \"output\"                     }                   ],                   \"source_name\": \"obj-1\"                 }               ],               \"destination_name\": \"pipeline_end\"             }           ],           \"request_retention_mode\": \"full\",           \"request_retention_time\": 604800         }       },       \"input_type\": \"structured\",       \"output_type\": \"structured\",       \"input_fields\": [         {           \"name\": \"input\",           \"data_type\": \"double\"         }       ],       \"output_fields\": [         {           \"name\": \"output\",           \"data_type\": \"double\"         }       ]     }   },   \"environment_variables\": {     \"PROJECT_ENV_VAR_1\": {       \"value\": \"value1\",       \"secret\": true     },     \"PROJECT_ENV_VAR_2\": {       \"value\": \"value2\"     }   } } ```  ### Response Structure Details of the updated import - `id`: Unique identifier for the import (UUID) - `status`: Status of the import - `error_message`: The error message in case of a failure - `creation_date`: The date when the import was created - `size`: Size of the import in bytes  #### Response Examples ``` {   \"id\": \"903ccd12-81d1-46e1-9ac9-b9d70af118de\",   \"status\": \"pending\",   \"error_message\": \"\",   \"creation_date\": \"2020-06-18T08:32:14.876451Z\",   \"size\": null } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.imports_update(project_name, import_id, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -8294,15 +8294,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.imports_update_with_http_info(project_name, import_id, data, **kwargs)  # noqa: E501
 
     def imports_update_with_http_info(self, project_name, import_id, data, **kwargs):  # noqa: E501
         """Confirm an import  # noqa: E501
 
-         ### Description Confirm (and update) an import by selecting the objects in the import  ### Optional Parameters - `deployments`: Dictionary containing the deployments to create - `pipelines`: Dictionary containing the pipelines to create - `environment_variables`: Dictionary containing the project-level environment variables to create  #### Request Examples  ``` {     \"deployments\": {     \"deployment-1: {       \"description\": \"\",       \"labels\": {         \"my-label\": \"my-value\"       },       \"default_version\": \"v1\",       \"versions\": {         \"v1\": {           \"zip\": \"deployments/deployment_deployment-1/versions/deployment_deployment-1_version_v1.zip\",           \"description\": \"\",           \"labels\": {},           \"language\": \"python3.7\",           \"deployment_mode\": \"express\",           \"maximum_idle_time\": 300,           \"maximum_instances\": 5,           \"memory_allocation\": 256,           \"minimum_instances\": 0,           \"environment_variables\": {             \"VERSION_ENV_VAR_1\": {               \"value\": \"my-secret-value\",               \"secret\": true             },             \"VERSION_ENV_VAR_2\": {               \"value\": \"test2\"             }           },           \"request_retention_mode\": \"full\",           \"request_retention_time\": 604800         }       },       \"input_type\": \"structured\",       \"output_type\": \"structured\",       \"input_fields\": [         {           \"name\": \"input\",           \"data_type\": \"double\"         }       ],       \"output_fields\": [         {           \"name\": \"output\",           \"data_type\": \"double\"         }       ],       \"environment_variables\": {         \"DEPLOYMENT_ENV_VAR_1\": {           \"value\": \"my-secret-value\",           \"secret\": true         },         \"DEPLOYMENT_ENV_VAR_2\": {           \"value\": \"test\"         }       }     }   },   \"pipelines\": {     \"pipeline-1: {       \"description\": \"\",       \"labels\": {         \"test\": \"label\"       },       \"default_version\": \"v1\",       \"versions\": {         \"v1\": {           \"description\": \"\",           \"labels\": {},           \"objects\": [             {               \"name\": \"obj-1\",               \"reference_name\": \"deployment-1\",               \"reference_version\": \"v1\"             }           ],           \"attachments\": [             {               \"sources\": [                 {                   \"mapping\": [                     {                       \"source_field_name\": \"input\",                       \"destination_field_name\": \"input\"                     }                   ],                   \"source_name\": \"pipeline_start\"                 }               ],               \"destination_name\": \"obj-1\"             },             {               \"sources\": [                 {                   \"mapping\": [                     {                       \"source_field_name\": \"output\",                       \"destination_field_name\": \"output\"                     }                   ],                   \"source_name\": \"obj-1\"                 }               ],               \"destination_name\": \"pipeline_end\"             }           ],           \"request_retention_mode\": \"full\",           \"request_retention_time\": 604800         }       },       \"input_type\": \"structured\",       \"output_type\": \"structured\",       \"input_fields\": [         {           \"name\": \"input\",           \"data_type\": \"double\"         }       ],       \"output_fields\": [         {           \"name\": \"output\",           \"data_type\": \"double\"         }       ]     }   },   \"environment_variables\": {     \"PROJECT_ENV_VAR_1\": {       \"value\": \"value1\",       \"secret\": true     },     \"PROJECT_ENV_VAR_2\": {       \"value\": \"value2\"     }   } } ```  ### Response Structure Details of the updated import - `id`: Unique identifier for the import (UUID) - `status`: Status of the import - `error_message`: The error message in case of a failure - `creation_date`: The date when the import was created - `size`: Size of the import in bytes  #### Response Examples ``` {   \"id\": \"903ccd12-81d1-46e1-9ac9-b9d70af118de\",   \"status\": \"pending\",   \"error_message\": \"\",   \"creation_date\": \"2020-06-18T08:32:14.876451Z\",   \"size\": null } ```   # noqa: E501
+         ### Description Confirm (and update) an import by selecting the objects in the import  ### Optional Parameters - `deployments`: Dictionary containing the deployments to create - `pipelines`: Dictionary containing the pipelines to create - `environment_variables`: Dictionary containing the project-level environment variables to create  #### Request Examples  ``` {     \"deployments\": {     \"deployment-1: {       \"description\": \"\",       \"labels\": {         \"my-label\": \"my-value\"       },       \"default_version\": \"v1\",       \"versions\": {         \"v1\": {           \"zip\": \"deployments/deployment_deployment-1/versions/deployment_deployment-1_version_v1.zip\",           \"description\": \"\",           \"labels\": {},           \"language\": \"python3.7\",           \"maximum_idle_time\": 300,           \"maximum_instances\": 5,           \"memory_allocation\": 256,           \"minimum_instances\": 0,           \"environment_variables\": {             \"VERSION_ENV_VAR_1\": {               \"value\": \"my-secret-value\",               \"secret\": true             },             \"VERSION_ENV_VAR_2\": {               \"value\": \"test2\"             }           },           \"request_retention_mode\": \"full\",           \"request_retention_time\": 604800         }       },       \"input_type\": \"structured\",       \"output_type\": \"structured\",       \"input_fields\": [         {           \"name\": \"input\",           \"data_type\": \"double\"         }       ],       \"output_fields\": [         {           \"name\": \"output\",           \"data_type\": \"double\"         }       ],       \"environment_variables\": {         \"DEPLOYMENT_ENV_VAR_1\": {           \"value\": \"my-secret-value\",           \"secret\": true         },         \"DEPLOYMENT_ENV_VAR_2\": {           \"value\": \"test\"         }       }     }   },   \"pipelines\": {     \"pipeline-1: {       \"description\": \"\",       \"labels\": {         \"test\": \"label\"       },       \"default_version\": \"v1\",       \"versions\": {         \"v1\": {           \"description\": \"\",           \"labels\": {},           \"objects\": [             {               \"name\": \"obj-1\",               \"reference_name\": \"deployment-1\",               \"reference_version\": \"v1\"             }           ],           \"attachments\": [             {               \"sources\": [                 {                   \"mapping\": [                     {                       \"source_field_name\": \"input\",                       \"destination_field_name\": \"input\"                     }                   ],                   \"source_name\": \"pipeline_start\"                 }               ],               \"destination_name\": \"obj-1\"             },             {               \"sources\": [                 {                   \"mapping\": [                     {                       \"source_field_name\": \"output\",                       \"destination_field_name\": \"output\"                     }                   ],                   \"source_name\": \"obj-1\"                 }               ],               \"destination_name\": \"pipeline_end\"             }           ],           \"request_retention_mode\": \"full\",           \"request_retention_time\": 604800         }       },       \"input_type\": \"structured\",       \"output_type\": \"structured\",       \"input_fields\": [         {           \"name\": \"input\",           \"data_type\": \"double\"         }       ],       \"output_fields\": [         {           \"name\": \"output\",           \"data_type\": \"double\"         }       ]     }   },   \"environment_variables\": {     \"PROJECT_ENV_VAR_1\": {       \"value\": \"value1\",       \"secret\": true     },     \"PROJECT_ENV_VAR_2\": {       \"value\": \"value2\"     }   } } ```  ### Response Structure Details of the updated import - `id`: Unique identifier for the import (UUID) - `status`: Status of the import - `error_message`: The error message in case of a failure - `creation_date`: The date when the import was created - `size`: Size of the import in bytes  #### Response Examples ``` {   \"id\": \"903ccd12-81d1-46e1-9ac9-b9d70af118de\",   \"status\": \"pending\",   \"error_message\": \"\",   \"creation_date\": \"2020-06-18T08:32:14.876451Z\",   \"size\": null } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.imports_update_with_http_info(project_name, import_id, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -8408,15 +8408,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def instance_types_list(self, organization_name, **kwargs):  # noqa: E501
         """List instance types  # noqa: E501
 
-         ### Description  Get list of available deployment instance types for an organization  ### Response Structure  Details of the instance type - `id`: Unique identifier for the instance type (UUID)   - `name`: Name of the deployment instance type   - `display_name`: Readable name of the deployment instance type   - `memory_allocation`: Integer indicating memory allocation for this instance type (Mi)   - `cpu_allocation`: Integer indicating CPU allocation for this instance type (milliCPU)   - `gpu_allocation`: Integer indicating number of GPU cores for this instance type   - `gpu_enabled`: Boolean indicating if the gpu resource is enabled for this instance type    #### Response Examples  ``` [   {     \"id\": \"abe2e406-fae5-4bcf-a3bc-956d756e4ecb\",     \"name\": \"512mb\",     \"display_name\": \"512 MB\"     \"memory_allocation\": 512,     \"cpu_allocation\": 125,     \"gpu_allocation\": 0,     \"gpu_enabled\": false   } ] ```   # noqa: E501
+         ### Description  Get list of available deployment instance types for an organization  ### Response Structure  Details of the instance type - `id`: Unique identifier for the instance type (UUID)   - `name`: Name of the deployment instance type   - `display_name`: Readable name of the deployment instance type   - `memory_allocation`: Integer indicating memory allocation for this instance type (Mi)   - `cpu_allocation`: Integer indicating CPU allocation for this instance type (milliCPU)   - `gpu_allocation`: Integer indicating number of GPU cores for this instance type   - `gpu_enabled`: Boolean indicating if the GPU resource is enabled for this instance type   - `gpu_type`: Type of the GPU enabled for this instance type    #### Response Examples  ``` [   {     \"id\": \"abe2e406-fae5-4bcf-a3bc-956d756e4ecb\",     \"name\": \"512mb\",     \"display_name\": \"512 MB\",     \"memory_allocation\": 512,     \"cpu_allocation\": 125,     \"gpu_allocation\": 0,     \"gpu_enabled\": false,     \"gpu_type\": null   } ] ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.instance_types_list(organization_name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str organization_name: (required)
@@ -8433,15 +8433,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.instance_types_list_with_http_info(organization_name, **kwargs)  # noqa: E501
 
     def instance_types_list_with_http_info(self, organization_name, **kwargs):  # noqa: E501
         """List instance types  # noqa: E501
 
-         ### Description  Get list of available deployment instance types for an organization  ### Response Structure  Details of the instance type - `id`: Unique identifier for the instance type (UUID)   - `name`: Name of the deployment instance type   - `display_name`: Readable name of the deployment instance type   - `memory_allocation`: Integer indicating memory allocation for this instance type (Mi)   - `cpu_allocation`: Integer indicating CPU allocation for this instance type (milliCPU)   - `gpu_allocation`: Integer indicating number of GPU cores for this instance type   - `gpu_enabled`: Boolean indicating if the gpu resource is enabled for this instance type    #### Response Examples  ``` [   {     \"id\": \"abe2e406-fae5-4bcf-a3bc-956d756e4ecb\",     \"name\": \"512mb\",     \"display_name\": \"512 MB\"     \"memory_allocation\": 512,     \"cpu_allocation\": 125,     \"gpu_allocation\": 0,     \"gpu_enabled\": false   } ] ```   # noqa: E501
+         ### Description  Get list of available deployment instance types for an organization  ### Response Structure  Details of the instance type - `id`: Unique identifier for the instance type (UUID)   - `name`: Name of the deployment instance type   - `display_name`: Readable name of the deployment instance type   - `memory_allocation`: Integer indicating memory allocation for this instance type (Mi)   - `cpu_allocation`: Integer indicating CPU allocation for this instance type (milliCPU)   - `gpu_allocation`: Integer indicating number of GPU cores for this instance type   - `gpu_enabled`: Boolean indicating if the GPU resource is enabled for this instance type   - `gpu_type`: Type of the GPU enabled for this instance type    #### Response Examples  ``` [   {     \"id\": \"abe2e406-fae5-4bcf-a3bc-956d756e4ecb\",     \"name\": \"512mb\",     \"display_name\": \"512 MB\",     \"memory_allocation\": 512,     \"cpu_allocation\": 125,     \"gpu_allocation\": 0,     \"gpu_enabled\": false,     \"gpu_type\": null   } ] ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.instance_types_list_with_http_info(organization_name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str organization_name: (required)
@@ -14195,15 +14195,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def pipeline_version_requests_list(self, project_name, pipeline_name, version, **kwargs):  # noqa: E501
         """List pipeline version requests  # noqa: E501
 
-         ### Description List all batch requests for a pipeline version  ### Optional Parameters The following parameters should be given as query parameters:  - `status`: Status of the request. Can be 'pending', 'processing', 'failed' or 'completed'. - `success`: A boolean value that indicates whether the pipeline version request was successful - `limit`: The maximum number of requests given back, default is 50 - `offset`: The number which forms the starting point of the requests given back. If offset equals 2, then the first 2 requests will be omitted from the list. - `sort`: Direction of sorting according to the creation date of the request, can be 'asc' or 'desc'. The default sorting is done in descending order. - `start_date`: Start date of the interval for which the requests are retrieved, looking at the creation date of the request - `end_date`: End date of the interval for which the requests are retrieved, looking at the creation date of the request - `search_id`: A string to search inside request ids. It will filter all request ids that contain this string  If no start or end date is provided, the most recent requests are returned.  ### Response Structure  A list of dictionaries containing the details of the pipeline version requests with the following fields:  - `id`: Unique identifier for the pipeline version request  - `pipeline`: Name of the pipeline for which the request is made  - `version`: Name of the pipeline version for which the request was made  - `status`: Status of the request  - `success`: A boolean value that indicates whether the pipeline version request was successful. NULL if the request is not yet finished.  - `time_created`: Server time that the request was made (current time)  - `time_started`: Server time that the processing of the request was started  - `time_completed`: Server time that the processing of the request was completed  #### Response Examples  ``` [   {     \"id\": \"69eca481-8576-49e8-8e20-ea56f2005bcb\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"success\": false,     \"time_created\": \"2020-03-28T20:00:26.613+00:00\",     \"time_started\": \"2020-03-28T20:00:41.276+00:00\",     \"time_completed\": \"2020-03-28T20:00:42.241+00:00\"   },   {     \"id\": \"2521378e-263e-4e2e-85e9-a96254b36536\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"completed\",     \"success\": true,     \"time_created\": \"2020-03-28T20:00:26.613+00:00\",     \"time_started\": \"2020-03-28T20:00:41.276+00:00\",     \"time_completed\": \"2020-03-28T20:00:42.241+00:00\"   } ] ```   # noqa: E501
+         ### Description List all requests for a pipeline version  ### Optional Parameters The following parameters should be given as query parameters:  - `status`: Status of the request. Can be 'pending', 'processing', 'failed' or 'completed'. - `success`: A boolean value that indicates whether the pipeline version request was successful - `limit`: The maximum number of requests given back, default is 50 - `offset`: The number which forms the starting point of the requests given back. If offset equals 2, then the first 2 requests will be omitted from the list. - `sort`: Direction of sorting according to the creation date of the request, can be 'asc' or 'desc'. The default sorting is done in descending order. - `start_date`: Start date of the interval for which the requests are retrieved, looking at the creation date of the request - `end_date`: End date of the interval for which the requests are retrieved, looking at the creation date of the request - `search_id`: A string to search inside request ids. It will filter all request ids that contain this string  If no start or end date is provided, the most recent requests are returned.  ### Response Structure  A list of dictionaries containing the details of the pipeline version requests with the following fields:  - `id`: Unique identifier for the pipeline version request  - `pipeline`: Name of the pipeline for which the request is made  - `version`: Name of the pipeline version for which the request was made  - `status`: Status of the request  - `success`: A boolean value that indicates whether the pipeline version request was successful. NULL if the request is not yet finished.  - `time_created`: Server time that the request was made (current time)  - `time_started`: Server time that the processing of the request was started  - `time_completed`: Server time that the processing of the request was completed  #### Response Examples  ``` [   {     \"id\": \"69eca481-8576-49e8-8e20-ea56f2005bcb\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"success\": false,     \"time_created\": \"2020-03-28T20:00:26.613+00:00\",     \"time_started\": \"2020-03-28T20:00:41.276+00:00\",     \"time_completed\": \"2020-03-28T20:00:42.241+00:00\"   },   {     \"id\": \"2521378e-263e-4e2e-85e9-a96254b36536\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"completed\",     \"success\": true,     \"time_created\": \"2020-03-28T20:00:26.613+00:00\",     \"time_started\": \"2020-03-28T20:00:41.276+00:00\",     \"time_completed\": \"2020-03-28T20:00:42.241+00:00\"   } ] ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.pipeline_version_requests_list(project_name, pipeline_name, version, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -14230,15 +14230,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.pipeline_version_requests_list_with_http_info(project_name, pipeline_name, version, **kwargs)  # noqa: E501
 
     def pipeline_version_requests_list_with_http_info(self, project_name, pipeline_name, version, **kwargs):  # noqa: E501
         """List pipeline version requests  # noqa: E501
 
-         ### Description List all batch requests for a pipeline version  ### Optional Parameters The following parameters should be given as query parameters:  - `status`: Status of the request. Can be 'pending', 'processing', 'failed' or 'completed'. - `success`: A boolean value that indicates whether the pipeline version request was successful - `limit`: The maximum number of requests given back, default is 50 - `offset`: The number which forms the starting point of the requests given back. If offset equals 2, then the first 2 requests will be omitted from the list. - `sort`: Direction of sorting according to the creation date of the request, can be 'asc' or 'desc'. The default sorting is done in descending order. - `start_date`: Start date of the interval for which the requests are retrieved, looking at the creation date of the request - `end_date`: End date of the interval for which the requests are retrieved, looking at the creation date of the request - `search_id`: A string to search inside request ids. It will filter all request ids that contain this string  If no start or end date is provided, the most recent requests are returned.  ### Response Structure  A list of dictionaries containing the details of the pipeline version requests with the following fields:  - `id`: Unique identifier for the pipeline version request  - `pipeline`: Name of the pipeline for which the request is made  - `version`: Name of the pipeline version for which the request was made  - `status`: Status of the request  - `success`: A boolean value that indicates whether the pipeline version request was successful. NULL if the request is not yet finished.  - `time_created`: Server time that the request was made (current time)  - `time_started`: Server time that the processing of the request was started  - `time_completed`: Server time that the processing of the request was completed  #### Response Examples  ``` [   {     \"id\": \"69eca481-8576-49e8-8e20-ea56f2005bcb\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"success\": false,     \"time_created\": \"2020-03-28T20:00:26.613+00:00\",     \"time_started\": \"2020-03-28T20:00:41.276+00:00\",     \"time_completed\": \"2020-03-28T20:00:42.241+00:00\"   },   {     \"id\": \"2521378e-263e-4e2e-85e9-a96254b36536\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"completed\",     \"success\": true,     \"time_created\": \"2020-03-28T20:00:26.613+00:00\",     \"time_started\": \"2020-03-28T20:00:41.276+00:00\",     \"time_completed\": \"2020-03-28T20:00:42.241+00:00\"   } ] ```   # noqa: E501
+         ### Description List all requests for a pipeline version  ### Optional Parameters The following parameters should be given as query parameters:  - `status`: Status of the request. Can be 'pending', 'processing', 'failed' or 'completed'. - `success`: A boolean value that indicates whether the pipeline version request was successful - `limit`: The maximum number of requests given back, default is 50 - `offset`: The number which forms the starting point of the requests given back. If offset equals 2, then the first 2 requests will be omitted from the list. - `sort`: Direction of sorting according to the creation date of the request, can be 'asc' or 'desc'. The default sorting is done in descending order. - `start_date`: Start date of the interval for which the requests are retrieved, looking at the creation date of the request - `end_date`: End date of the interval for which the requests are retrieved, looking at the creation date of the request - `search_id`: A string to search inside request ids. It will filter all request ids that contain this string  If no start or end date is provided, the most recent requests are returned.  ### Response Structure  A list of dictionaries containing the details of the pipeline version requests with the following fields:  - `id`: Unique identifier for the pipeline version request  - `pipeline`: Name of the pipeline for which the request is made  - `version`: Name of the pipeline version for which the request was made  - `status`: Status of the request  - `success`: A boolean value that indicates whether the pipeline version request was successful. NULL if the request is not yet finished.  - `time_created`: Server time that the request was made (current time)  - `time_started`: Server time that the processing of the request was started  - `time_completed`: Server time that the processing of the request was completed  #### Response Examples  ``` [   {     \"id\": \"69eca481-8576-49e8-8e20-ea56f2005bcb\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"pending\",     \"success\": false,     \"time_created\": \"2020-03-28T20:00:26.613+00:00\",     \"time_started\": \"2020-03-28T20:00:41.276+00:00\",     \"time_completed\": \"2020-03-28T20:00:42.241+00:00\"   },   {     \"id\": \"2521378e-263e-4e2e-85e9-a96254b36536\",     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"completed\",     \"success\": true,     \"time_created\": \"2020-03-28T20:00:26.613+00:00\",     \"time_started\": \"2020-03-28T20:00:41.276+00:00\",     \"time_completed\": \"2020-03-28T20:00:42.241+00:00\"   } ] ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.pipeline_version_requests_list_with_http_info(project_name, pipeline_name, version, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -14395,15 +14395,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def pipeline_versions_create(self, project_name, pipeline_name, data, **kwargs):  # noqa: E501
         """Create pipeline versions  # noqa: E501
 
-         ### Description  Create a version for a pipeline. The first version of a pipeline is set as default. Provide the parameter 'monitoring' as the name of a notification group to send monitoring notifications to. A notification will be sent in the case of a failed/recovered request. Pass `null` to switch off monitoring notifications for this version. Provide the parameter 'default_notification_group' as the name of a notification group to send notifications when requests for the version are completed. Pass `null` to switch off request notifications for this version. This field is only used for **batch requests** to the version.  ### Required Parameters  - `version`: Name of the version of the pipeline  ### Optional Parameters - `description`: Description of the pipeline version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the pipeline version. It defaults to 604800 seconds (1 week). - `request_retention_mode`: Mode of request retention for requests to the pipeline version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored - `objects`: List of pipeline version objects - `attachments`: List of pipeline version object attachments  #### Request Examples  ``` {   \"version\": \"v1\" } ```  ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": \"notification-group-1\",   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\" } ```  A pipeline version with objects and attachments ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": [\"test@example.com\"],   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [     {       \"name\": \"object-1\",       \"reference_name\": \"deployment-1\",       \"version\": \"v1\"     }   ],   \"attachments\": [     {       \"destination_name\": \"object-1\",       \"sources\": [         {           \"source_name\": \"pipeline_start\",           \"mapping\": [             {               \"source_field_name\": \"example-field\",               \"destination_field_name\": \"example-field\"             }           ]         }       ]     }   ] } ```  ### Response Structure  Details of the created pipeline version - `id`: Unique identifier for the pipeline version (UUID) - `pipeline`: Name of the pipeline to which the version is associated - `version`: Name of the version of the pipeline - `description`: Description of the pipeline version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the pipeline version was created - `last_updated`: The date when the pipeline version was last updated - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the pipeline version - `request_retention_mode`: Mode of request retention for requests to the pipeline version. It can be one of the following: *none*, *metadata* or *full*. - `objects`: List of pipeline version objects - `attachments`: List of pipeline version object attachments  #### Response Examples  ``` {   \"id\": \"6b0cea21-2657-4fa3-a331-de646e3cfdc4\",   \"pipeline\": \"pipeline-1\",   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"tag\": \"production\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [],   \"attachments\": [] } ```  ``` {   \"id\": \"6b0cea21-2657-4fa3-a331-de646e3cfdc4\",   \"pipeline\": \"pipeline-1\",   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"tag\": \"production\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"monitoring\": [\"test@example.com\"],   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [     {       \"name\": \"object-1\",       \"reference_name\": \"deployment-1\",       \"version\": \"v1\"     }   ],   \"attachments\": [     {       \"destination_name\": \"object-1\",       \"sources\": [         {           \"source_name\": \"pipeline_start\",           \"mapping\": [             {               \"source_field_name\": \"example-field\",               \"destination_field_name\": \"example-field\"             }           ]         }       ]     }   ] } ```   # noqa: E501
+         ### Description  Create a version for a pipeline. The first version of a pipeline is set as default. Provide the parameter 'monitoring' as the name of a notification group to send monitoring notifications to. A notification will be sent in the case of a failed/recovered request. Pass `null` to switch off monitoring notifications for this version. Provide the parameter 'default_notification_group' as the name of a notification group to send notifications when requests for the version are completed. Pass `null` to switch off request notifications for this version.  ### Required Parameters  - `version`: Name of the version of the pipeline  ### Optional Parameters - `description`: Description of the pipeline version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the pipeline version. It defaults to 604800 seconds (1 week). - `request_retention_mode`: Mode of request retention for requests to the pipeline version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored - `objects`: List of pipeline version objects - `attachments`: List of pipeline version object attachments  #### Request Examples  ``` {   \"version\": \"v1\" } ```  ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": \"notification-group-1\",   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\" } ```  A pipeline version with objects and attachments ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": [\"test@example.com\"],   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [     {       \"name\": \"object-1\",       \"reference_name\": \"deployment-1\",       \"version\": \"v1\"     }   ],   \"attachments\": [     {       \"destination_name\": \"object-1\",       \"sources\": [         {           \"source_name\": \"pipeline_start\",           \"mapping\": [             {               \"source_field_name\": \"example-field\",               \"destination_field_name\": \"example-field\"             }           ]         }       ]     }   ] } ```  ### Response Structure  Details of the created pipeline version - `id`: Unique identifier for the pipeline version (UUID) - `pipeline`: Name of the pipeline to which the version is associated - `version`: Name of the version of the pipeline - `description`: Description of the pipeline version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the pipeline version was created - `last_updated`: The date when the pipeline version was last updated - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the pipeline version - `request_retention_mode`: Mode of request retention for requests to the pipeline version. It can be one of the following: *none*, *metadata* or *full*. - `objects`: List of pipeline version objects - `attachments`: List of pipeline version object attachments  #### Response Examples  ``` {   \"id\": \"6b0cea21-2657-4fa3-a331-de646e3cfdc4\",   \"pipeline\": \"pipeline-1\",   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"tag\": \"production\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [],   \"attachments\": [] } ```  ``` {   \"id\": \"6b0cea21-2657-4fa3-a331-de646e3cfdc4\",   \"pipeline\": \"pipeline-1\",   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"tag\": \"production\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"monitoring\": [\"test@example.com\"],   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [     {       \"name\": \"object-1\",       \"reference_name\": \"deployment-1\",       \"version\": \"v1\"     }   ],   \"attachments\": [     {       \"destination_name\": \"object-1\",       \"sources\": [         {           \"source_name\": \"pipeline_start\",           \"mapping\": [             {               \"source_field_name\": \"example-field\",               \"destination_field_name\": \"example-field\"             }           ]         }       ]     }   ] } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.pipeline_versions_create(project_name, pipeline_name, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -14422,15 +14422,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.pipeline_versions_create_with_http_info(project_name, pipeline_name, data, **kwargs)  # noqa: E501
 
     def pipeline_versions_create_with_http_info(self, project_name, pipeline_name, data, **kwargs):  # noqa: E501
         """Create pipeline versions  # noqa: E501
 
-         ### Description  Create a version for a pipeline. The first version of a pipeline is set as default. Provide the parameter 'monitoring' as the name of a notification group to send monitoring notifications to. A notification will be sent in the case of a failed/recovered request. Pass `null` to switch off monitoring notifications for this version. Provide the parameter 'default_notification_group' as the name of a notification group to send notifications when requests for the version are completed. Pass `null` to switch off request notifications for this version. This field is only used for **batch requests** to the version.  ### Required Parameters  - `version`: Name of the version of the pipeline  ### Optional Parameters - `description`: Description of the pipeline version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the pipeline version. It defaults to 604800 seconds (1 week). - `request_retention_mode`: Mode of request retention for requests to the pipeline version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored - `objects`: List of pipeline version objects - `attachments`: List of pipeline version object attachments  #### Request Examples  ``` {   \"version\": \"v1\" } ```  ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": \"notification-group-1\",   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\" } ```  A pipeline version with objects and attachments ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": [\"test@example.com\"],   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [     {       \"name\": \"object-1\",       \"reference_name\": \"deployment-1\",       \"version\": \"v1\"     }   ],   \"attachments\": [     {       \"destination_name\": \"object-1\",       \"sources\": [         {           \"source_name\": \"pipeline_start\",           \"mapping\": [             {               \"source_field_name\": \"example-field\",               \"destination_field_name\": \"example-field\"             }           ]         }       ]     }   ] } ```  ### Response Structure  Details of the created pipeline version - `id`: Unique identifier for the pipeline version (UUID) - `pipeline`: Name of the pipeline to which the version is associated - `version`: Name of the version of the pipeline - `description`: Description of the pipeline version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the pipeline version was created - `last_updated`: The date when the pipeline version was last updated - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the pipeline version - `request_retention_mode`: Mode of request retention for requests to the pipeline version. It can be one of the following: *none*, *metadata* or *full*. - `objects`: List of pipeline version objects - `attachments`: List of pipeline version object attachments  #### Response Examples  ``` {   \"id\": \"6b0cea21-2657-4fa3-a331-de646e3cfdc4\",   \"pipeline\": \"pipeline-1\",   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"tag\": \"production\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [],   \"attachments\": [] } ```  ``` {   \"id\": \"6b0cea21-2657-4fa3-a331-de646e3cfdc4\",   \"pipeline\": \"pipeline-1\",   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"tag\": \"production\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"monitoring\": [\"test@example.com\"],   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [     {       \"name\": \"object-1\",       \"reference_name\": \"deployment-1\",       \"version\": \"v1\"     }   ],   \"attachments\": [     {       \"destination_name\": \"object-1\",       \"sources\": [         {           \"source_name\": \"pipeline_start\",           \"mapping\": [             {               \"source_field_name\": \"example-field\",               \"destination_field_name\": \"example-field\"             }           ]         }       ]     }   ] } ```   # noqa: E501
+         ### Description  Create a version for a pipeline. The first version of a pipeline is set as default. Provide the parameter 'monitoring' as the name of a notification group to send monitoring notifications to. A notification will be sent in the case of a failed/recovered request. Pass `null` to switch off monitoring notifications for this version. Provide the parameter 'default_notification_group' as the name of a notification group to send notifications when requests for the version are completed. Pass `null` to switch off request notifications for this version.  ### Required Parameters  - `version`: Name of the version of the pipeline  ### Optional Parameters - `description`: Description of the pipeline version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the pipeline version. It defaults to 604800 seconds (1 week). - `request_retention_mode`: Mode of request retention for requests to the pipeline version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored - `objects`: List of pipeline version objects - `attachments`: List of pipeline version object attachments  #### Request Examples  ``` {   \"version\": \"v1\" } ```  ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": \"notification-group-1\",   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\" } ```  A pipeline version with objects and attachments ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": [\"test@example.com\"],   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [     {       \"name\": \"object-1\",       \"reference_name\": \"deployment-1\",       \"version\": \"v1\"     }   ],   \"attachments\": [     {       \"destination_name\": \"object-1\",       \"sources\": [         {           \"source_name\": \"pipeline_start\",           \"mapping\": [             {               \"source_field_name\": \"example-field\",               \"destination_field_name\": \"example-field\"             }           ]         }       ]     }   ] } ```  ### Response Structure  Details of the created pipeline version - `id`: Unique identifier for the pipeline version (UUID) - `pipeline`: Name of the pipeline to which the version is associated - `version`: Name of the version of the pipeline - `description`: Description of the pipeline version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the pipeline version was created - `last_updated`: The date when the pipeline version was last updated - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the pipeline version - `request_retention_mode`: Mode of request retention for requests to the pipeline version. It can be one of the following: *none*, *metadata* or *full*. - `objects`: List of pipeline version objects - `attachments`: List of pipeline version object attachments  #### Response Examples  ``` {   \"id\": \"6b0cea21-2657-4fa3-a331-de646e3cfdc4\",   \"pipeline\": \"pipeline-1\",   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"tag\": \"production\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [],   \"attachments\": [] } ```  ``` {   \"id\": \"6b0cea21-2657-4fa3-a331-de646e3cfdc4\",   \"pipeline\": \"pipeline-1\",   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"tag\": \"production\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"monitoring\": [\"test@example.com\"],   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [     {       \"name\": \"object-1\",       \"reference_name\": \"deployment-1\",       \"version\": \"v1\"     }   ],   \"attachments\": [     {       \"destination_name\": \"object-1\",       \"sources\": [         {           \"source_name\": \"pipeline_start\",           \"mapping\": [             {               \"source_field_name\": \"example-field\",               \"destination_field_name\": \"example-field\"             }           ]         }       ]     }   ] } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.pipeline_versions_create_with_http_info(project_name, pipeline_name, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -14937,15 +14937,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def pipeline_versions_update(self, project_name, pipeline_name, version, data, **kwargs):  # noqa: E501
         """Update pipeline version  # noqa: E501
 
-         ### Description  Update a pipeline version. When updating labels, the labels will replace the existing value for labels.  Provide the parameter 'monitoring' as the name of a notification group to send monitoring notifications to. A notification will be sent in the case of a failed/recovered request. Pass `null` to switch off monitoring notifications for this version. Provide the parameter 'default_notification_group' as the name of a notification group to send notifications when requests for the version are completed. Pass `null` to switch off request notifications for this version. This field is only used for **batch requests** to the version.  **Attention:** *In case either the `objects` or `attachments` parameter is null or an empty list, all of the objects or attachments of the pipeline will be removed.*  ### Optional Parameters - `version`: Name of the version of the pipeline - `description`: Description of the pipeline version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the pipeline version - `request_retention_mode`: Mode of request retention for requests to the pipeline version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored - `objects`: List of pipeline version objects - `attachments`: List of pipeline version object attachments  #### Request Examples  ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": \"notification-group-1\" } ```  Updating a pipeline version with new objects and attachments ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": [\"test@example.com\"],   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [     {       \"name\": \"object-1\",       \"reference_name\": \"deployment-1\",       \"version\": \"v1\"     }   ],   \"attachments\": [     {       \"destination_name\": \"object-1\",       \"sources\": [         {           \"source_name\": \"pipeline_start\",           \"mapping\": [             {               \"source_field_name\": \"example-field\",               \"destination_field_name\": \"example-field\"             }           ]         }       ]     }   ] } ```  Updating a pipeline version by removing objects and attachments ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": [\"test@example.com\"],   \"objects\": null,   \"attachments\": null } ```  ### Response Structure  Details of the created pipeline - `id`: Unique identifier for the pipeline version (UUID) - `pipeline`: Name of the pipeline to which the version is associated - `version`: Name of the version of the pipeline - `description`: Description of the pipeline version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the pipeline version was created - `last_updated`: The date when the pipeline version was last updated - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the pipeline version - `request_retention_mode`: Mode of request retention for requests to the pipeline version. It can be one of the following: *none*, *metadata* or *full*. - `objects`: List of pipeline version objects - `attachments`: List of pipeline version object attachments  #### Response Examples  ``` {   \"id\": \"6b0cea21-2657-4fa3-a331-de646e3cfdc4\",   \"pipeline\": \"pipeline-1\",   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"tag\": \"production\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [],   \"attachments\": [] } ```  ``` {   \"id\": \"6b0cea21-2657-4fa3-a331-de646e3cfdc4\",   \"pipeline\": \"pipeline-1\",   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"tag\": \"production\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"monitoring\": [\"test@example.com\"],   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [     {       \"name\": \"object-1\",       \"reference_name\": \"deployment-1\",       \"version\": \"v1\"     }   ],   \"attachments\": [     {       \"destination_name\": \"object-1\",       \"sources\": [         {           \"source_name\": \"pipeline_start\",           \"mapping\": [             {               \"source_field_name\": \"example-field\",               \"destination_field_name\": \"example-field\"             }           ]         }       ]     }   ] } ```   # noqa: E501
+         ### Description  Update a pipeline version. When updating labels, the labels will replace the existing value for labels.  Provide the parameter 'monitoring' as the name of a notification group to send monitoring notifications to. A notification will be sent in the case of a failed/recovered request. Pass `null` to switch off monitoring notifications for this version. Provide the parameter 'default_notification_group' as the name of a notification group to send notifications when requests for the version are completed. Pass `null` to switch off request notifications for this version.  **Attention:** *In case either the `objects` or `attachments` parameter is null or an empty list, all of the objects or attachments of the pipeline will be removed.*  ### Optional Parameters - `version`: Name of the version of the pipeline - `description`: Description of the pipeline version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the pipeline version - `request_retention_mode`: Mode of request retention for requests to the pipeline version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored - `objects`: List of pipeline version objects - `attachments`: List of pipeline version object attachments  #### Request Examples  ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": \"notification-group-1\" } ```  Updating a pipeline version with new objects and attachments ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": [\"test@example.com\"],   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [     {       \"name\": \"object-1\",       \"reference_name\": \"deployment-1\",       \"version\": \"v1\"     }   ],   \"attachments\": [     {       \"destination_name\": \"object-1\",       \"sources\": [         {           \"source_name\": \"pipeline_start\",           \"mapping\": [             {               \"source_field_name\": \"example-field\",               \"destination_field_name\": \"example-field\"             }           ]         }       ]     }   ] } ```  Updating a pipeline version by removing objects and attachments ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": [\"test@example.com\"],   \"objects\": null,   \"attachments\": null } ```  ### Response Structure  Details of the created pipeline - `id`: Unique identifier for the pipeline version (UUID) - `pipeline`: Name of the pipeline to which the version is associated - `version`: Name of the version of the pipeline - `description`: Description of the pipeline version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the pipeline version was created - `last_updated`: The date when the pipeline version was last updated - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the pipeline version - `request_retention_mode`: Mode of request retention for requests to the pipeline version. It can be one of the following: *none*, *metadata* or *full*. - `objects`: List of pipeline version objects - `attachments`: List of pipeline version object attachments  #### Response Examples  ``` {   \"id\": \"6b0cea21-2657-4fa3-a331-de646e3cfdc4\",   \"pipeline\": \"pipeline-1\",   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"tag\": \"production\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [],   \"attachments\": [] } ```  ``` {   \"id\": \"6b0cea21-2657-4fa3-a331-de646e3cfdc4\",   \"pipeline\": \"pipeline-1\",   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"tag\": \"production\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"monitoring\": [\"test@example.com\"],   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [     {       \"name\": \"object-1\",       \"reference_name\": \"deployment-1\",       \"version\": \"v1\"     }   ],   \"attachments\": [     {       \"destination_name\": \"object-1\",       \"sources\": [         {           \"source_name\": \"pipeline_start\",           \"mapping\": [             {               \"source_field_name\": \"example-field\",               \"destination_field_name\": \"example-field\"             }           ]         }       ]     }   ] } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.pipeline_versions_update(project_name, pipeline_name, version, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -14965,15 +14965,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.pipeline_versions_update_with_http_info(project_name, pipeline_name, version, data, **kwargs)  # noqa: E501
 
     def pipeline_versions_update_with_http_info(self, project_name, pipeline_name, version, data, **kwargs):  # noqa: E501
         """Update pipeline version  # noqa: E501
 
-         ### Description  Update a pipeline version. When updating labels, the labels will replace the existing value for labels.  Provide the parameter 'monitoring' as the name of a notification group to send monitoring notifications to. A notification will be sent in the case of a failed/recovered request. Pass `null` to switch off monitoring notifications for this version. Provide the parameter 'default_notification_group' as the name of a notification group to send notifications when requests for the version are completed. Pass `null` to switch off request notifications for this version. This field is only used for **batch requests** to the version.  **Attention:** *In case either the `objects` or `attachments` parameter is null or an empty list, all of the objects or attachments of the pipeline will be removed.*  ### Optional Parameters - `version`: Name of the version of the pipeline - `description`: Description of the pipeline version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the pipeline version - `request_retention_mode`: Mode of request retention for requests to the pipeline version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored - `objects`: List of pipeline version objects - `attachments`: List of pipeline version object attachments  #### Request Examples  ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": \"notification-group-1\" } ```  Updating a pipeline version with new objects and attachments ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": [\"test@example.com\"],   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [     {       \"name\": \"object-1\",       \"reference_name\": \"deployment-1\",       \"version\": \"v1\"     }   ],   \"attachments\": [     {       \"destination_name\": \"object-1\",       \"sources\": [         {           \"source_name\": \"pipeline_start\",           \"mapping\": [             {               \"source_field_name\": \"example-field\",               \"destination_field_name\": \"example-field\"             }           ]         }       ]     }   ] } ```  Updating a pipeline version by removing objects and attachments ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": [\"test@example.com\"],   \"objects\": null,   \"attachments\": null } ```  ### Response Structure  Details of the created pipeline - `id`: Unique identifier for the pipeline version (UUID) - `pipeline`: Name of the pipeline to which the version is associated - `version`: Name of the version of the pipeline - `description`: Description of the pipeline version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the pipeline version was created - `last_updated`: The date when the pipeline version was last updated - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the pipeline version - `request_retention_mode`: Mode of request retention for requests to the pipeline version. It can be one of the following: *none*, *metadata* or *full*. - `objects`: List of pipeline version objects - `attachments`: List of pipeline version object attachments  #### Response Examples  ``` {   \"id\": \"6b0cea21-2657-4fa3-a331-de646e3cfdc4\",   \"pipeline\": \"pipeline-1\",   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"tag\": \"production\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [],   \"attachments\": [] } ```  ``` {   \"id\": \"6b0cea21-2657-4fa3-a331-de646e3cfdc4\",   \"pipeline\": \"pipeline-1\",   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"tag\": \"production\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"monitoring\": [\"test@example.com\"],   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [     {       \"name\": \"object-1\",       \"reference_name\": \"deployment-1\",       \"version\": \"v1\"     }   ],   \"attachments\": [     {       \"destination_name\": \"object-1\",       \"sources\": [         {           \"source_name\": \"pipeline_start\",           \"mapping\": [             {               \"source_field_name\": \"example-field\",               \"destination_field_name\": \"example-field\"             }           ]         }       ]     }   ] } ```   # noqa: E501
+         ### Description  Update a pipeline version. When updating labels, the labels will replace the existing value for labels.  Provide the parameter 'monitoring' as the name of a notification group to send monitoring notifications to. A notification will be sent in the case of a failed/recovered request. Pass `null` to switch off monitoring notifications for this version. Provide the parameter 'default_notification_group' as the name of a notification group to send notifications when requests for the version are completed. Pass `null` to switch off request notifications for this version.  **Attention:** *In case either the `objects` or `attachments` parameter is null or an empty list, all of the objects or attachments of the pipeline will be removed.*  ### Optional Parameters - `version`: Name of the version of the pipeline - `description`: Description of the pipeline version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the pipeline version - `request_retention_mode`: Mode of request retention for requests to the pipeline version. It can be one of the following:     - *none* - the requests will not be stored     - *metadata* - only the metadata of the requests will be stored     - *full* - both the metadata and input/output of the requests will be stored - `objects`: List of pipeline version objects - `attachments`: List of pipeline version object attachments  #### Request Examples  ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": \"notification-group-1\" } ```  Updating a pipeline version with new objects and attachments ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": [\"test@example.com\"],   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [     {       \"name\": \"object-1\",       \"reference_name\": \"deployment-1\",       \"version\": \"v1\"     }   ],   \"attachments\": [     {       \"destination_name\": \"object-1\",       \"sources\": [         {           \"source_name\": \"pipeline_start\",           \"mapping\": [             {               \"source_field_name\": \"example-field\",               \"destination_field_name\": \"example-field\"             }           ]         }       ]     }   ] } ```  Updating a pipeline version by removing objects and attachments ``` {   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"type\": \"production\"   },   \"monitoring\": [\"test@example.com\"],   \"objects\": null,   \"attachments\": null } ```  ### Response Structure  Details of the created pipeline - `id`: Unique identifier for the pipeline version (UUID) - `pipeline`: Name of the pipeline to which the version is associated - `version`: Name of the version of the pipeline - `description`: Description of the pipeline version - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label - `creation_date`: The date when the pipeline version was created - `last_updated`: The date when the pipeline version was last updated - `monitoring`: Name of a notification group which contain contacts to send monitoring notifications - `default_notification_group`: Name of a notification group which contain contacts to send notifications when requests for the version are completed - `request_retention_time`: Number of seconds to store requests to the pipeline version - `request_retention_mode`: Mode of request retention for requests to the pipeline version. It can be one of the following: *none*, *metadata* or *full*. - `objects`: List of pipeline version objects - `attachments`: List of pipeline version object attachments  #### Response Examples  ``` {   \"id\": \"6b0cea21-2657-4fa3-a331-de646e3cfdc4\",   \"pipeline\": \"pipeline-1\",   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"tag\": \"production\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"monitoring\": \"notification-group-1\",   \"default_notification_group\": null,   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [],   \"attachments\": [] } ```  ``` {   \"id\": \"6b0cea21-2657-4fa3-a331-de646e3cfdc4\",   \"pipeline\": \"pipeline-1\",   \"version\": \"v1\",   \"description\": \"my description\",   \"labels\": {     \"tag\": \"production\"   },   \"creation_date\": \"2020-05-12T16:23:15.456812Z\",   \"last_updated\": \"2020-06-22T18:04:76.123754Z\",   \"monitoring\": [\"test@example.com\"],   \"request_retention_time\": 604800,   \"request_retention_mode\": \"full\",   \"objects\": [     {       \"name\": \"object-1\",       \"reference_name\": \"deployment-1\",       \"version\": \"v1\"     }   ],   \"attachments\": [     {       \"destination_name\": \"object-1\",       \"sources\": [         {           \"source_name\": \"pipeline_start\",           \"mapping\": [             {               \"source_field_name\": \"example-field\",               \"destination_field_name\": \"example-field\"             }           ]         }       ]     }   ] } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.pipeline_versions_update_with_http_info(project_name, pipeline_name, version, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -16485,14 +16485,138 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def project_requests_list(self, project_name, object_type, **kwargs):  # noqa: E501
+        """List requests in project  # noqa: E501
+
+         ### Description List the deployment/pipeline requests of the given project  ### Required Parameters - `object_type`: The type of the object. It can be either deployment or pipeline.  ### Optional Parameters - `status`: Status of the request. Can be 'pending', 'processing', 'failed', 'completed', 'cancelled' or 'cancelled_pending'. - `success`: A boolean value that indicates whether the deployment request was successful - `limit`: The maximum number of requests given back, default is 50 - `offset`: The number which forms the starting point of the requests given back. If offset equals 2, then the first 2 requests will be omitted from the list. - `sort`: Direction of sorting according to the creation date of the request, can be 'asc' or 'desc'. The default sorting is done in descending order. - `pipeline`: A boolean value that indicates whether the deployment request was part of a pipeline request - `start_date`: Start date of the interval for which the requests are retrieved, looking at the creation date of the request - `end_date`: End date of the interval for which the requests are retrieved, looking at the creation date of the request - `search_id`: A string to search inside request ids. It will filter all request ids that contain this string  ### Response Structure A list of dictionaries containing the metadata of the deployment/pipeline requests with the following fields: - `id`: The UUID of the object - `deployment`: Name of the deployment the request was made to (Optional: in case it's a deployment request. Else NULL) - `pipeline`: Name of the pipeline the request was made to (Optional: in case it's a pipeline request. Else NULL) - `version`: Name of the version the request was made to - `status`: Status of the request - `success`: A boolean value that indicates whether the deployment/pipeline request was successful. NULL if the request is not yet finished. - `time_created`: Server time that the request was made (current time) - `time_started`: Server time that the processing of the request was started - `time_completed`: Server time that the processing of the request was completed   #### Response Examples ``` [   {     \"id\": \"69eca481-8576-49e8-8e20-ea56f2005bcb\",     \"deployment\": \"deployment-1\",     \"pipeline\": null,     \"version\": \"v1\",     \"status\": \"pending\",     \"success\": false,     \"time_created\": \"2020-03-28T20:00:26.613+00:00\",     \"time_started\": \"2020-03-28T20:00:41.276+00:00\",     \"time_completed\": \"2020-03-28T20:00:42.241+00:00\"   },   {     \"id\": \"2521378e-263e-4e2e-85e9-a96254b36536\",     \"deployment\": null,     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"completed\",     \"success\": true,     \"time_created\": \"2020-03-28T20:00:26.613+00:00\",     \"time_started\": \"2020-03-28T20:00:41.276+00:00\",     \"time_completed\": \"2020-03-28T20:00:42.241+00:00\"   } ] ```   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.project_requests_list(project_name, object_type, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str project_name: (required)
+        :param str object_type: (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: list[RequestsOverview]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.project_requests_list_with_http_info(project_name, object_type, **kwargs)  # noqa: E501
+
+    def project_requests_list_with_http_info(self, project_name, object_type, **kwargs):  # noqa: E501
+        """List requests in project  # noqa: E501
+
+         ### Description List the deployment/pipeline requests of the given project  ### Required Parameters - `object_type`: The type of the object. It can be either deployment or pipeline.  ### Optional Parameters - `status`: Status of the request. Can be 'pending', 'processing', 'failed', 'completed', 'cancelled' or 'cancelled_pending'. - `success`: A boolean value that indicates whether the deployment request was successful - `limit`: The maximum number of requests given back, default is 50 - `offset`: The number which forms the starting point of the requests given back. If offset equals 2, then the first 2 requests will be omitted from the list. - `sort`: Direction of sorting according to the creation date of the request, can be 'asc' or 'desc'. The default sorting is done in descending order. - `pipeline`: A boolean value that indicates whether the deployment request was part of a pipeline request - `start_date`: Start date of the interval for which the requests are retrieved, looking at the creation date of the request - `end_date`: End date of the interval for which the requests are retrieved, looking at the creation date of the request - `search_id`: A string to search inside request ids. It will filter all request ids that contain this string  ### Response Structure A list of dictionaries containing the metadata of the deployment/pipeline requests with the following fields: - `id`: The UUID of the object - `deployment`: Name of the deployment the request was made to (Optional: in case it's a deployment request. Else NULL) - `pipeline`: Name of the pipeline the request was made to (Optional: in case it's a pipeline request. Else NULL) - `version`: Name of the version the request was made to - `status`: Status of the request - `success`: A boolean value that indicates whether the deployment/pipeline request was successful. NULL if the request is not yet finished. - `time_created`: Server time that the request was made (current time) - `time_started`: Server time that the processing of the request was started - `time_completed`: Server time that the processing of the request was completed   #### Response Examples ``` [   {     \"id\": \"69eca481-8576-49e8-8e20-ea56f2005bcb\",     \"deployment\": \"deployment-1\",     \"pipeline\": null,     \"version\": \"v1\",     \"status\": \"pending\",     \"success\": false,     \"time_created\": \"2020-03-28T20:00:26.613+00:00\",     \"time_started\": \"2020-03-28T20:00:41.276+00:00\",     \"time_completed\": \"2020-03-28T20:00:42.241+00:00\"   },   {     \"id\": \"2521378e-263e-4e2e-85e9-a96254b36536\",     \"deployment\": null,     \"pipeline\": \"pipeline-1\",     \"version\": \"v1\",     \"status\": \"completed\",     \"success\": true,     \"time_created\": \"2020-03-28T20:00:26.613+00:00\",     \"time_started\": \"2020-03-28T20:00:41.276+00:00\",     \"time_completed\": \"2020-03-28T20:00:42.241+00:00\"   } ] ```   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.project_requests_list_with_http_info(project_name, object_type, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str project_name: (required)
+        :param str object_type: (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(list[RequestsOverview], status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['project_name', 'object_type']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method project_requests_list" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'project_name' is set
+        if self.api_client.client_side_validation and ('project_name' not in local_var_params or  # noqa: E501
+                                                        local_var_params['project_name'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `project_name` when calling `project_requests_list`")  # noqa: E501
+        # verify the required parameter 'object_type' is set
+        if self.api_client.client_side_validation and ('object_type' not in local_var_params or  # noqa: E501
+                                                        local_var_params['object_type'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `object_type` when calling `project_requests_list`")  # noqa: E501
+        if (self.api_client.client_side_validation and 'project_name' in local_var_params
+            and local_var_params['project_name'] is not None):  # noqa: E501
+            if not isinstance(local_var_params['project_name'], str):  # noqa: E501
+                raise ApiValueError("Parameter `project_name` must be a string when calling `project_requests_list`")  # noqa: E501
+        if (self.api_client.client_side_validation and 'object_type' in local_var_params
+            and local_var_params['object_type'] is not None):  # noqa: E501
+            if not isinstance(local_var_params['object_type'], str):  # noqa: E501
+                raise ApiValueError("Parameter `object_type` must be a string when calling `project_requests_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'project_name' in local_var_params:
+            path_params['project_name'] = local_var_params['project_name']  # noqa: E501
+
+        query_params = []
+        if 'object_type' in local_var_params and local_var_params['object_type'] is not None:  # noqa: E501
+            query_params.append(('object_type', local_var_params['object_type']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['api_key']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/projects/{project_name}/requests', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[RequestsOverview]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def project_users_create(self, project_name, data, **kwargs):  # noqa: E501
         """Add user to a project  # noqa: E501
 
          ### Description Add a user to a project. The user making the request must be admin of the organization. The user can later be assigned roles in the project, such as project-admin, project-viewer etc.  ### Required Parameters - `user_id`: UUID of the user    #### Request Examples  ``` {   \"user_id\": \"bd3e25a3-f77a-4cb5-92df-a7e614106e95\" } ```  ### Response Structure  Details of the added user - `id`: Unique identifier for the user (UUID)   - `email`: Email of the user   - `name`: Name of the user   - `surname`: Surname of the user    #### Response Examples  ``` {   \"id\": \"332d7432-2742-4177-99a9-139e91e0110c\",   \"email\": \"test@example.com\",   \"name\": \"user\",   \"surname\": \"name\" } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.project_users_create(project_name, data, async_req=True)
@@ -17320,21 +17444,22 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def projects_list(self, **kwargs):  # noqa: E501
         """List projects  # noqa: E501
 
-         ### Description  List all projects to which the user making request has access. The projects in organizations to which the user belongs are shown.  ### Response Structure A list of details of the projects - `id`: Unique identifier for the project (UUID)   - `name`: Name of the project   - `creation_date`: Time the project was created   - `advanced_permissions`: A boolean to enable/disable advanced permissions for the project   - `organization_name`: Name of the organization in which the project is created  #### Response Examples ``` [   {     \"id\": \"e988ddc0-3ef1-42d2-ab30-9f810a5e7063\",     \"name\": \"project-1\",     \"creation_date\": \"2018-10-26\",     \"advanced_permissions\": false,     \"organization_name\": \"organization-1\"   },   {     \"id\": \"e6a85cd7-94cc-44cf-9fa0-4b462d5a71ab\",     \"name\": \"project-2\",     \"creation_date\": \"2019-06-20\",     \"advanced_permissions\": false,     \"organization_name\": \"organization-2\"   } ] ```   # noqa: E501
+         ### Description  List all projects to which the user making request has access. The projects in organizations to which the user belongs are shown.  ### Response Structure A list of details of the projects - `id`: Unique identifier for the project (UUID)   - `name`: Name of the project   - `creation_date`: Time the project was created   - `advanced_permissions`: A boolean to enable/disable advanced permissions for the project   - `organization_name`: Name of the organization in which the project is created  ### Optional Parameters These parameters should be given as query parameters - `organization`: Name of the organization whose projects should be obtained  #### Response Examples ``` [   {     \"id\": \"e988ddc0-3ef1-42d2-ab30-9f810a5e7063\",     \"name\": \"project-1\",     \"creation_date\": \"2018-10-26\",     \"advanced_permissions\": false,     \"organization_name\": \"organization-1\"   },   {     \"id\": \"e6a85cd7-94cc-44cf-9fa0-4b462d5a71ab\",     \"name\": \"project-2\",     \"creation_date\": \"2019-06-20\",     \"advanced_permissions\": false,     \"organization_name\": \"organization-2\"   } ] ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.projects_list(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param str organization:
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -17344,21 +17469,22 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.projects_list_with_http_info(**kwargs)  # noqa: E501
 
     def projects_list_with_http_info(self, **kwargs):  # noqa: E501
         """List projects  # noqa: E501
 
-         ### Description  List all projects to which the user making request has access. The projects in organizations to which the user belongs are shown.  ### Response Structure A list of details of the projects - `id`: Unique identifier for the project (UUID)   - `name`: Name of the project   - `creation_date`: Time the project was created   - `advanced_permissions`: A boolean to enable/disable advanced permissions for the project   - `organization_name`: Name of the organization in which the project is created  #### Response Examples ``` [   {     \"id\": \"e988ddc0-3ef1-42d2-ab30-9f810a5e7063\",     \"name\": \"project-1\",     \"creation_date\": \"2018-10-26\",     \"advanced_permissions\": false,     \"organization_name\": \"organization-1\"   },   {     \"id\": \"e6a85cd7-94cc-44cf-9fa0-4b462d5a71ab\",     \"name\": \"project-2\",     \"creation_date\": \"2019-06-20\",     \"advanced_permissions\": false,     \"organization_name\": \"organization-2\"   } ] ```   # noqa: E501
+         ### Description  List all projects to which the user making request has access. The projects in organizations to which the user belongs are shown.  ### Response Structure A list of details of the projects - `id`: Unique identifier for the project (UUID)   - `name`: Name of the project   - `creation_date`: Time the project was created   - `advanced_permissions`: A boolean to enable/disable advanced permissions for the project   - `organization_name`: Name of the organization in which the project is created  ### Optional Parameters These parameters should be given as query parameters - `organization`: Name of the organization whose projects should be obtained  #### Response Examples ``` [   {     \"id\": \"e988ddc0-3ef1-42d2-ab30-9f810a5e7063\",     \"name\": \"project-1\",     \"creation_date\": \"2018-10-26\",     \"advanced_permissions\": false,     \"organization_name\": \"organization-1\"   },   {     \"id\": \"e6a85cd7-94cc-44cf-9fa0-4b462d5a71ab\",     \"name\": \"project-2\",     \"creation_date\": \"2019-06-20\",     \"advanced_permissions\": false,     \"organization_name\": \"organization-2\"   } ] ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.projects_list_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param str organization:
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -17367,34 +17493,40 @@
         :return: tuple(list[ProjectList], status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
-        all_params = []  # noqa: E501
+        all_params = ['organization']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method projects_list" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        if (self.api_client.client_side_validation and 'organization' in local_var_params
+            and local_var_params['organization'] is not None):  # noqa: E501
+            if not isinstance(local_var_params['organization'], str):  # noqa: E501
+                raise ApiValueError("Parameter `organization` must be a string when calling `projects_list`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'organization' in local_var_params and local_var_params['organization'] is not None:  # noqa: E501
+            query_params.append(('organization', local_var_params['organization']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -17914,15 +18046,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def request_schedules_create(self, project_name, data, **kwargs):  # noqa: E501
         """Create request schedules  # noqa: E501
 
-         ### Description  Create a new request schedule with the provided name  ### Required Parameters  - `name`: Name of the request. The name is unique per project. It can only consist of lowercase letters, numbers and dashes (-), and must start with a lowercase letter.   - `object_type`: Type of object for which the request is made. Can be either 'deployment' or 'pipeline'.   - `object_name`: Name of deployment or pipeline for which the request is made   - `schedule`: Schedule in crontab format    ### Optional Parameters - `version`: Name of version for which the request schedule is made. If not provided, default version of the deployment/pipeline will be used.   - `request_data`: Input data for the request schedule. For structured deployments/pipelines, it must be a dictionary.   - `timeout`: Timeout of the request in seconds. The maximum and default values depend on the object (deployment or pipeline) and the type of request (batch or direct). - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled. Default is 'True'.   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Request Examples  ``` {   \"name\": \"test-request\",   \"object_type\": \"deployment\",   \"object_name\": \"test-deployment\",   \"version\": \"v1\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"timeout\": 300,   \"enabled\": true,   \"description\": \"Daily request schedule\",   \"labels\": {     \"type\": \"daily\"   } } ```  ### Response Structure  Details of the created request schedule - `name`: Name of the request   - `object_type`: Type of object for which the request is made   - `object_name`: Name of deployment/pipeline for which the request schedule is made   - `schedule`: Schedule in crontab format   - `version`: Name of version for which the request schedule is made   - `request_data`: Input data for the request schedule   - `batch`: Boolean value indicating whether the requests will be performed as batch requests (true) or as direct requests (false). For pipeline schedules, this variable is true by default. For deployment schedules, the deployment mode is used to determine its value. It is false for express mode and true for batch mode.   - `timeout`: Timeout of the request in seconds   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled   - `creation_date`: The date when the request schedule was created   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Response Examples  ``` {   \"id\": \"b4a06aed-f7ab-48b3-b579-b12b62db8058\",   \"name\": \"test-request\",   \"object_type\": \"deployment\",   \"object_name\": \"test-deployment\",   \"version\": \"v1\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"batch\": false,   \"timeout\": 300,   \"enabled\": true,   \"creation_date\": \"2020-09-16T08:06:34.457679Z\",   \"description\": \"Daily request schedule\",   \"labels\": {     \"type\": \"daily\"   } } ```   # noqa: E501
+         ### Description  Create a new request schedule with the provided name  ### Required Parameters  - `name`: Name of the request. The name is unique per project. It can only consist of lowercase letters, numbers and dashes (-), and must start with a lowercase letter.   - `object_type`: Type of object for which the request is made. Can be either 'deployment' or 'pipeline'.   - `object_name`: Name of deployment or pipeline for which the request is made   - `schedule`: Schedule in crontab format    ### Optional Parameters - `version`: Name of version for which the request schedule is made. If not provided, default version of the deployment/pipeline will be used.   - `request_data`: Input data for the request schedule. For structured deployments/pipelines, it must be a dictionary.   - `timeout`: Timeout of the request in seconds. The maximum and default values depend on the object (deployment or pipeline) and the type of request (batch or direct). - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled. Default is 'True'.   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Request Examples  ``` {   \"name\": \"test-request\",   \"object_type\": \"deployment\",   \"object_name\": \"test-deployment\",   \"version\": \"v1\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"timeout\": 300,   \"enabled\": true,   \"description\": \"Daily request schedule\",   \"labels\": {     \"type\": \"daily\"   } } ```  ### Response Structure  Details of the created request schedule - `name`: Name of the request   - `object_type`: Type of object for which the request is made   - `object_name`: Name of deployment/pipeline for which the request schedule is made   - `schedule`: Schedule in crontab format   - `version`: Name of version for which the request schedule is made   - `request_data`: Input data for the request schedule   - `timeout`: Timeout of the request in seconds   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled   - `creation_date`: The date when the request schedule was created   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Response Examples  ``` {   \"id\": \"b4a06aed-f7ab-48b3-b579-b12b62db8058\",   \"name\": \"test-request\",   \"object_type\": \"deployment\",   \"object_name\": \"test-deployment\",   \"version\": \"v1\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"timeout\": 300,   \"enabled\": true,   \"creation_date\": \"2020-09-16T08:06:34.457679Z\",   \"description\": \"Daily request schedule\",   \"labels\": {     \"type\": \"daily\"   } } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.request_schedules_create(project_name, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -17940,15 +18072,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.request_schedules_create_with_http_info(project_name, data, **kwargs)  # noqa: E501
 
     def request_schedules_create_with_http_info(self, project_name, data, **kwargs):  # noqa: E501
         """Create request schedules  # noqa: E501
 
-         ### Description  Create a new request schedule with the provided name  ### Required Parameters  - `name`: Name of the request. The name is unique per project. It can only consist of lowercase letters, numbers and dashes (-), and must start with a lowercase letter.   - `object_type`: Type of object for which the request is made. Can be either 'deployment' or 'pipeline'.   - `object_name`: Name of deployment or pipeline for which the request is made   - `schedule`: Schedule in crontab format    ### Optional Parameters - `version`: Name of version for which the request schedule is made. If not provided, default version of the deployment/pipeline will be used.   - `request_data`: Input data for the request schedule. For structured deployments/pipelines, it must be a dictionary.   - `timeout`: Timeout of the request in seconds. The maximum and default values depend on the object (deployment or pipeline) and the type of request (batch or direct). - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled. Default is 'True'.   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Request Examples  ``` {   \"name\": \"test-request\",   \"object_type\": \"deployment\",   \"object_name\": \"test-deployment\",   \"version\": \"v1\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"timeout\": 300,   \"enabled\": true,   \"description\": \"Daily request schedule\",   \"labels\": {     \"type\": \"daily\"   } } ```  ### Response Structure  Details of the created request schedule - `name`: Name of the request   - `object_type`: Type of object for which the request is made   - `object_name`: Name of deployment/pipeline for which the request schedule is made   - `schedule`: Schedule in crontab format   - `version`: Name of version for which the request schedule is made   - `request_data`: Input data for the request schedule   - `batch`: Boolean value indicating whether the requests will be performed as batch requests (true) or as direct requests (false). For pipeline schedules, this variable is true by default. For deployment schedules, the deployment mode is used to determine its value. It is false for express mode and true for batch mode.   - `timeout`: Timeout of the request in seconds   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled   - `creation_date`: The date when the request schedule was created   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Response Examples  ``` {   \"id\": \"b4a06aed-f7ab-48b3-b579-b12b62db8058\",   \"name\": \"test-request\",   \"object_type\": \"deployment\",   \"object_name\": \"test-deployment\",   \"version\": \"v1\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"batch\": false,   \"timeout\": 300,   \"enabled\": true,   \"creation_date\": \"2020-09-16T08:06:34.457679Z\",   \"description\": \"Daily request schedule\",   \"labels\": {     \"type\": \"daily\"   } } ```   # noqa: E501
+         ### Description  Create a new request schedule with the provided name  ### Required Parameters  - `name`: Name of the request. The name is unique per project. It can only consist of lowercase letters, numbers and dashes (-), and must start with a lowercase letter.   - `object_type`: Type of object for which the request is made. Can be either 'deployment' or 'pipeline'.   - `object_name`: Name of deployment or pipeline for which the request is made   - `schedule`: Schedule in crontab format    ### Optional Parameters - `version`: Name of version for which the request schedule is made. If not provided, default version of the deployment/pipeline will be used.   - `request_data`: Input data for the request schedule. For structured deployments/pipelines, it must be a dictionary.   - `timeout`: Timeout of the request in seconds. The maximum and default values depend on the object (deployment or pipeline) and the type of request (batch or direct). - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled. Default is 'True'.   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Request Examples  ``` {   \"name\": \"test-request\",   \"object_type\": \"deployment\",   \"object_name\": \"test-deployment\",   \"version\": \"v1\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"timeout\": 300,   \"enabled\": true,   \"description\": \"Daily request schedule\",   \"labels\": {     \"type\": \"daily\"   } } ```  ### Response Structure  Details of the created request schedule - `name`: Name of the request   - `object_type`: Type of object for which the request is made   - `object_name`: Name of deployment/pipeline for which the request schedule is made   - `schedule`: Schedule in crontab format   - `version`: Name of version for which the request schedule is made   - `request_data`: Input data for the request schedule   - `timeout`: Timeout of the request in seconds   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled   - `creation_date`: The date when the request schedule was created   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Response Examples  ``` {   \"id\": \"b4a06aed-f7ab-48b3-b579-b12b62db8058\",   \"name\": \"test-request\",   \"object_type\": \"deployment\",   \"object_name\": \"test-deployment\",   \"version\": \"v1\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"timeout\": 300,   \"enabled\": true,   \"creation_date\": \"2020-09-16T08:06:34.457679Z\",   \"description\": \"Daily request schedule\",   \"labels\": {     \"type\": \"daily\"   } } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.request_schedules_create_with_http_info(project_name, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -18164,15 +18296,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def request_schedules_get(self, project_name, schedule_name, **kwargs):  # noqa: E501
         """Get details of a request schedule  # noqa: E501
 
-         ### Description  Retrieve details of a single request schedule  ### Response Structure  Details of a request schedule - `name`: Name of the request   - `object_type`: Type of object for which the request is made   - `object_name`: Name of deployment/pipeline for which the request is made   - `schedule`: Schedule in crontab format   - `version`: Name of version for which the request schedule is made   - `request_data`: Input data for the request schedule   - `batch`: Boolean value indicating whether the requests will be performed as batch requests (true) or as direct requests (false)   - `timeout`: Timeout of the request in seconds   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled   - `creation_date`: The date when the request schedule was created   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Response Examples  ``` {   \"id\": \"b4a06aed-f7ab-48b3-b579-b12b62db8058\",   \"name\": \"test-request\",   \"object_type\": \"deployment\",   \"object_name\": \"test-deployment\",   \"version\": \"v1\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"batch\": false,   \"timeout\": 200,   \"enabled\": true,   \"creation_date\": \"2020-09-16T08:06:34.457679Z\",   \"description\": \"Daily request schedule\",   \"labels\": {     \"type\": \"daily\"   } } ```   # noqa: E501
+         ### Description  Retrieve details of a single request schedule  ### Response Structure  Details of a request schedule - `name`: Name of the request   - `object_type`: Type of object for which the request is made   - `object_name`: Name of deployment/pipeline for which the request is made   - `schedule`: Schedule in crontab format   - `version`: Name of version for which the request schedule is made   - `request_data`: Input data for the request schedule   - `timeout`: Timeout of the request in seconds   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled   - `creation_date`: The date when the request schedule was created   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Response Examples  ``` {   \"id\": \"b4a06aed-f7ab-48b3-b579-b12b62db8058\",   \"name\": \"test-request\",   \"object_type\": \"deployment\",   \"object_name\": \"test-deployment\",   \"version\": \"v1\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"timeout\": 200,   \"enabled\": true,   \"creation_date\": \"2020-09-16T08:06:34.457679Z\",   \"description\": \"Daily request schedule\",   \"labels\": {     \"type\": \"daily\"   } } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.request_schedules_get(project_name, schedule_name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -18190,15 +18322,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.request_schedules_get_with_http_info(project_name, schedule_name, **kwargs)  # noqa: E501
 
     def request_schedules_get_with_http_info(self, project_name, schedule_name, **kwargs):  # noqa: E501
         """Get details of a request schedule  # noqa: E501
 
-         ### Description  Retrieve details of a single request schedule  ### Response Structure  Details of a request schedule - `name`: Name of the request   - `object_type`: Type of object for which the request is made   - `object_name`: Name of deployment/pipeline for which the request is made   - `schedule`: Schedule in crontab format   - `version`: Name of version for which the request schedule is made   - `request_data`: Input data for the request schedule   - `batch`: Boolean value indicating whether the requests will be performed as batch requests (true) or as direct requests (false)   - `timeout`: Timeout of the request in seconds   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled   - `creation_date`: The date when the request schedule was created   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Response Examples  ``` {   \"id\": \"b4a06aed-f7ab-48b3-b579-b12b62db8058\",   \"name\": \"test-request\",   \"object_type\": \"deployment\",   \"object_name\": \"test-deployment\",   \"version\": \"v1\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"batch\": false,   \"timeout\": 200,   \"enabled\": true,   \"creation_date\": \"2020-09-16T08:06:34.457679Z\",   \"description\": \"Daily request schedule\",   \"labels\": {     \"type\": \"daily\"   } } ```   # noqa: E501
+         ### Description  Retrieve details of a single request schedule  ### Response Structure  Details of a request schedule - `name`: Name of the request   - `object_type`: Type of object for which the request is made   - `object_name`: Name of deployment/pipeline for which the request is made   - `schedule`: Schedule in crontab format   - `version`: Name of version for which the request schedule is made   - `request_data`: Input data for the request schedule   - `timeout`: Timeout of the request in seconds   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled   - `creation_date`: The date when the request schedule was created   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Response Examples  ``` {   \"id\": \"b4a06aed-f7ab-48b3-b579-b12b62db8058\",   \"name\": \"test-request\",   \"object_type\": \"deployment\",   \"object_name\": \"test-deployment\",   \"version\": \"v1\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"timeout\": 200,   \"enabled\": true,   \"creation_date\": \"2020-09-16T08:06:34.457679Z\",   \"description\": \"Daily request schedule\",   \"labels\": {     \"type\": \"daily\"   } } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.request_schedules_get_with_http_info(project_name, schedule_name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -18288,15 +18420,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def request_schedules_list(self, project_name, **kwargs):  # noqa: E501
         """List request schedules  # noqa: E501
 
-         ### Description  List the request schedules in a project. The user has to have 'requests.list' permission on either 'deployments.versions' or 'pipelines.versions' to list the request schedules.  ### Response Structure  A list of details of all request schedules in a project - `name`: Name of the request   - `object_type`: Type of object for which the request is made   - `object_name`: Name of deployment/pipeline for which the request is made   - `schedule`: Schedule in crontab format   - `version`: Name of version for which the request schedule is made    - `request_data`: Input data for the request schedule   - `batch`: Boolean value indicating whether the requests will be performed as batch requests (true) or as direct requests (false)   - `timeout`: Timeout of the request in seconds   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled   - `creation_date`: The date when the request schedule was created   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Response Examples  ``` [   {     \"id\": \"b4a06aed-f7ab-48b3-b579-b12b62db8058\",     \"name\": \"test-request\",     \"object_type\": \"deployment\",     \"object_name\": \"test-deployment\",     \"version\": \"v1\",     \"schedule\": \"0 * 3 * *\",     \"request_data\": {       \"input_field_1\": 2345,       \"input_field_2\": 8765     },     \"batch\": false,     \"timeout\": 200\",     \"enabled\": true,     \"creation_date\": \"2020-09-16T08:06:34.457679Z\",     \"description\": \"Daily request schedule\",     \"labels\": {       \"type\": \"daily\"     }   } ] ```   # noqa: E501
+         ### Description  List the request schedules in a project. The user has to have 'requests.list' permission on either 'deployments.versions' or 'pipelines.versions' to list the request schedules.  ### Response Structure  A list of details of all request schedules in a project - `name`: Name of the request   - `object_type`: Type of object for which the request is made   - `object_name`: Name of deployment/pipeline for which the request is made   - `schedule`: Schedule in crontab format   - `version`: Name of version for which the request schedule is made    - `request_data`: Input data for the request schedule   - `timeout`: Timeout of the request in seconds   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled   - `creation_date`: The date when the request schedule was created   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Response Examples  ``` [   {     \"id\": \"b4a06aed-f7ab-48b3-b579-b12b62db8058\",     \"name\": \"test-request\",     \"object_type\": \"deployment\",     \"object_name\": \"test-deployment\",     \"version\": \"v1\",     \"schedule\": \"0 * 3 * *\",     \"request_data\": {       \"input_field_1\": 2345,       \"input_field_2\": 8765     },     \"timeout\": 200\",     \"enabled\": true,     \"creation_date\": \"2020-09-16T08:06:34.457679Z\",     \"description\": \"Daily request schedule\",     \"labels\": {       \"type\": \"daily\"     }   } ] ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.request_schedules_list(project_name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -18313,15 +18445,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.request_schedules_list_with_http_info(project_name, **kwargs)  # noqa: E501
 
     def request_schedules_list_with_http_info(self, project_name, **kwargs):  # noqa: E501
         """List request schedules  # noqa: E501
 
-         ### Description  List the request schedules in a project. The user has to have 'requests.list' permission on either 'deployments.versions' or 'pipelines.versions' to list the request schedules.  ### Response Structure  A list of details of all request schedules in a project - `name`: Name of the request   - `object_type`: Type of object for which the request is made   - `object_name`: Name of deployment/pipeline for which the request is made   - `schedule`: Schedule in crontab format   - `version`: Name of version for which the request schedule is made    - `request_data`: Input data for the request schedule   - `batch`: Boolean value indicating whether the requests will be performed as batch requests (true) or as direct requests (false)   - `timeout`: Timeout of the request in seconds   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled   - `creation_date`: The date when the request schedule was created   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Response Examples  ``` [   {     \"id\": \"b4a06aed-f7ab-48b3-b579-b12b62db8058\",     \"name\": \"test-request\",     \"object_type\": \"deployment\",     \"object_name\": \"test-deployment\",     \"version\": \"v1\",     \"schedule\": \"0 * 3 * *\",     \"request_data\": {       \"input_field_1\": 2345,       \"input_field_2\": 8765     },     \"batch\": false,     \"timeout\": 200\",     \"enabled\": true,     \"creation_date\": \"2020-09-16T08:06:34.457679Z\",     \"description\": \"Daily request schedule\",     \"labels\": {       \"type\": \"daily\"     }   } ] ```   # noqa: E501
+         ### Description  List the request schedules in a project. The user has to have 'requests.list' permission on either 'deployments.versions' or 'pipelines.versions' to list the request schedules.  ### Response Structure  A list of details of all request schedules in a project - `name`: Name of the request   - `object_type`: Type of object for which the request is made   - `object_name`: Name of deployment/pipeline for which the request is made   - `schedule`: Schedule in crontab format   - `version`: Name of version for which the request schedule is made    - `request_data`: Input data for the request schedule   - `timeout`: Timeout of the request in seconds   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled   - `creation_date`: The date when the request schedule was created   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Response Examples  ``` [   {     \"id\": \"b4a06aed-f7ab-48b3-b579-b12b62db8058\",     \"name\": \"test-request\",     \"object_type\": \"deployment\",     \"object_name\": \"test-deployment\",     \"version\": \"v1\",     \"schedule\": \"0 * 3 * *\",     \"request_data\": {       \"input_field_1\": 2345,       \"input_field_2\": 8765     },     \"timeout\": 200\",     \"enabled\": true,     \"creation_date\": \"2020-09-16T08:06:34.457679Z\",     \"description\": \"Daily request schedule\",     \"labels\": {       \"type\": \"daily\"     }   } ] ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.request_schedules_list_with_http_info(project_name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -18400,15 +18532,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def request_schedules_update(self, project_name, schedule_name, data, **kwargs):  # noqa: E501
         """Update a request schedule  # noqa: E501
 
-         ### Description  Update a request schedule in a project. Create permissions on the object are necessary for this action.  ### Optional Parameters - `name`: Name of the request. The name is unique per project. It can only consist of lowercase letters, numbers and dashes (-), and must start with a lowercase letter.   - `schedule`: Schedule in crontab format   - `request_data`: Input data for the request schedule. For structured deployments/pipelines, it must be a dictionary.   - `timeout`: Timeout of the request in seconds. The maximum and default values depend on the object (deployment or pipeline) and the type of request (batch or direct).   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled. Default is 'True'.   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Request Examples  ``` {   \"name\": \"test-request\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"timeout\": 360,   \"enabled\": false } ```  ### Response Structure  Details of the updated request schedule - `name`: Name of the request   - `object_type`: Type of object for which the request is made   - `object_name`: Name of deployment/pipeline for which the request is made   - `schedule`: Schedule in crontab format   - `version`: Name of version for which the request schedule is made   - `request_data`: Input data for the request schedule   - `batch`: Boolean value indicating whether the requests will be performed as batch requests (true) or as direct requests (false)   - `timeout`: Timeout of the request in seconds   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled   - `creation_date`: The date when the request schedule was created   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Response Examples  ``` {   \"id\": \"b4a06aed-f7ab-48b3-b579-b12b62db8058\",   \"name\": \"test-request\",   \"object_type\": \"deployment\",   \"object_name\": \"test-deployment\",   \"version\": \"v1\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"batch\": false,   \"timeout\": 360,   \"enabled\": true,   \"creation_date\": \"2020-09-16T08:06:34.457679Z\",   \"description\": \"Daily request schedule\",   \"labels\": {     \"type\": \"daily\"   } } ```   # noqa: E501
+         ### Description  Update a request schedule in a project. Create permissions on the object are necessary for this action.  ### Optional Parameters - `name`: Name of the request. The name is unique per project. It can only consist of lowercase letters, numbers and dashes (-), and must start with a lowercase letter.   - `schedule`: Schedule in crontab format   - `request_data`: Input data for the request schedule. For structured deployments/pipelines, it must be a dictionary.   - `timeout`: Timeout of the request in seconds. The maximum and default values depend on the object (deployment or pipeline) and the type of request (batch or direct).   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled. Default is 'True'.   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Request Examples  ``` {   \"name\": \"test-request\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"timeout\": 360,   \"enabled\": false } ```  ### Response Structure  Details of the updated request schedule - `name`: Name of the request   - `object_type`: Type of object for which the request is made   - `object_name`: Name of deployment/pipeline for which the request is made   - `schedule`: Schedule in crontab format   - `version`: Name of version for which the request schedule is made   - `request_data`: Input data for the request schedule   - `timeout`: Timeout of the request in seconds   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled   - `creation_date`: The date when the request schedule was created   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Response Examples  ``` {   \"id\": \"b4a06aed-f7ab-48b3-b579-b12b62db8058\",   \"name\": \"test-request\",   \"object_type\": \"deployment\",   \"object_name\": \"test-deployment\",   \"version\": \"v1\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"timeout\": 360,   \"enabled\": true,   \"creation_date\": \"2020-09-16T08:06:34.457679Z\",   \"description\": \"Daily request schedule\",   \"labels\": {     \"type\": \"daily\"   } } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.request_schedules_update(project_name, schedule_name, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
@@ -18427,15 +18559,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.request_schedules_update_with_http_info(project_name, schedule_name, data, **kwargs)  # noqa: E501
 
     def request_schedules_update_with_http_info(self, project_name, schedule_name, data, **kwargs):  # noqa: E501
         """Update a request schedule  # noqa: E501
 
-         ### Description  Update a request schedule in a project. Create permissions on the object are necessary for this action.  ### Optional Parameters - `name`: Name of the request. The name is unique per project. It can only consist of lowercase letters, numbers and dashes (-), and must start with a lowercase letter.   - `schedule`: Schedule in crontab format   - `request_data`: Input data for the request schedule. For structured deployments/pipelines, it must be a dictionary.   - `timeout`: Timeout of the request in seconds. The maximum and default values depend on the object (deployment or pipeline) and the type of request (batch or direct).   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled. Default is 'True'.   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Request Examples  ``` {   \"name\": \"test-request\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"timeout\": 360,   \"enabled\": false } ```  ### Response Structure  Details of the updated request schedule - `name`: Name of the request   - `object_type`: Type of object for which the request is made   - `object_name`: Name of deployment/pipeline for which the request is made   - `schedule`: Schedule in crontab format   - `version`: Name of version for which the request schedule is made   - `request_data`: Input data for the request schedule   - `batch`: Boolean value indicating whether the requests will be performed as batch requests (true) or as direct requests (false)   - `timeout`: Timeout of the request in seconds   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled   - `creation_date`: The date when the request schedule was created   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Response Examples  ``` {   \"id\": \"b4a06aed-f7ab-48b3-b579-b12b62db8058\",   \"name\": \"test-request\",   \"object_type\": \"deployment\",   \"object_name\": \"test-deployment\",   \"version\": \"v1\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"batch\": false,   \"timeout\": 360,   \"enabled\": true,   \"creation_date\": \"2020-09-16T08:06:34.457679Z\",   \"description\": \"Daily request schedule\",   \"labels\": {     \"type\": \"daily\"   } } ```   # noqa: E501
+         ### Description  Update a request schedule in a project. Create permissions on the object are necessary for this action.  ### Optional Parameters - `name`: Name of the request. The name is unique per project. It can only consist of lowercase letters, numbers and dashes (-), and must start with a lowercase letter.   - `schedule`: Schedule in crontab format   - `request_data`: Input data for the request schedule. For structured deployments/pipelines, it must be a dictionary.   - `timeout`: Timeout of the request in seconds. The maximum and default values depend on the object (deployment or pipeline) and the type of request (batch or direct).   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled. Default is 'True'.   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Request Examples  ``` {   \"name\": \"test-request\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"timeout\": 360,   \"enabled\": false } ```  ### Response Structure  Details of the updated request schedule - `name`: Name of the request   - `object_type`: Type of object for which the request is made   - `object_name`: Name of deployment/pipeline for which the request is made   - `schedule`: Schedule in crontab format   - `version`: Name of version for which the request schedule is made   - `request_data`: Input data for the request schedule   - `timeout`: Timeout of the request in seconds   - `enabled`: Boolean value indicating whether the request schedule is enabled or disabled   - `creation_date`: The date when the request schedule was created   - `description`: Description of the request schedule   - `labels`: Dictionary containing key/value pairs where key indicates the label and value is the corresponding value of that label    #### Response Examples  ``` {   \"id\": \"b4a06aed-f7ab-48b3-b579-b12b62db8058\",   \"name\": \"test-request\",   \"object_type\": \"deployment\",   \"object_name\": \"test-deployment\",   \"version\": \"v1\",   \"schedule\": \"0 * 3 * *\",   \"request_data\": {     \"input_field_1\": 2345,     \"input_field_2\": 8765   },   \"timeout\": 360,   \"enabled\": true,   \"creation_date\": \"2020-09-16T08:06:34.457679Z\",   \"description\": \"Daily request schedule\",   \"labels\": {     \"type\": \"daily\"   } } ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.request_schedules_update_with_http_info(project_name, schedule_name, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str project_name: (required)
```

### Comparing `ubiops-3.8.0/ubiops/api_client.py` & `ubiops-3.9.0/ubiops/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'UbiOps/python/3.8.0'
+        self.user_agent = 'UbiOps/python/3.9.0'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ubiops-3.8.0/ubiops/configuration.py` & `ubiops-3.9.0/ubiops/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v2.1\n"\
-               "SDK Package Version: 3.8.0".\
+               "SDK Package Version: 3.9.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ubiops-3.8.0/ubiops/exceptions.py` & `ubiops-3.9.0/ubiops/exceptions.py`

 * *Files identical despite different names*

### Comparing `ubiops-3.8.0/ubiops/models/__init__.py` & `ubiops-3.9.0/ubiops/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 from ubiops.models.project_create import ProjectCreate
 from ubiops.models.project_detail import ProjectDetail
 from ubiops.models.project_list import ProjectList
 from ubiops.models.project_resource_usage import ProjectResourceUsage
 from ubiops.models.project_update import ProjectUpdate
 from ubiops.models.project_user_create import ProjectUserCreate
 from ubiops.models.project_user_list import ProjectUserList
+from ubiops.models.requests_overview import RequestsOverview
 from ubiops.models.resource_usage import ResourceUsage
 from ubiops.models.revision_create import RevisionCreate
 from ubiops.models.revision_list import RevisionList
 from ubiops.models.role_assignment_create import RoleAssignmentCreate
 from ubiops.models.role_assignment_list import RoleAssignmentList
 from ubiops.models.role_create import RoleCreate
 from ubiops.models.role_detail_list import RoleDetailList
```

### Comparing `ubiops-3.8.0/ubiops/models/attachment_fields_create.py` & `ubiops-3.9.0/ubiops/models/attachment_fields_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'source_field_name': 'source_field_name',
         'destination_field_name': 'destination_field_name'
     }
 
-    def __init__(self, source_field_name=None, destination_field_name=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, source_field_name=None, destination_field_name=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """AttachmentFieldsCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._source_field_name = None
         self._destination_field_name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/attachment_fields_list.py` & `ubiops-3.9.0/ubiops/models/attachment_fields_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'source_field_name': 'source_field_name',
         'destination_field_name': 'destination_field_name'
     }
 
-    def __init__(self, source_field_name=None, destination_field_name=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, source_field_name=None, destination_field_name=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """AttachmentFieldsList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._source_field_name = None
         self._destination_field_name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/attachment_sources_create.py` & `ubiops-3.9.0/ubiops/models/attachment_sources_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'source_name': 'source_name',
         'mapping': 'mapping'
     }
 
-    def __init__(self, source_name=None, mapping=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, source_name=None, mapping=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """AttachmentSourcesCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._source_name = None
         self._mapping = None
```

### Comparing `ubiops-3.8.0/ubiops/models/attachment_sources_list.py` & `ubiops-3.9.0/ubiops/models/attachment_sources_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'source_name': 'source_name',
         'mapping': 'mapping'
     }
 
-    def __init__(self, source_name=None, mapping=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, source_name=None, mapping=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """AttachmentSourcesList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._source_name = None
         self._mapping = None
```

### Comparing `ubiops-3.8.0/ubiops/models/attachments_create.py` & `ubiops-3.9.0/ubiops/models/attachments_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'destination_name': 'destination_name',
         'sources': 'sources'
     }
 
-    def __init__(self, destination_name=None, sources=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, destination_name=None, sources=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """AttachmentsCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._destination_name = None
         self._sources = None
```

### Comparing `ubiops-3.8.0/ubiops/models/attachments_list.py` & `ubiops-3.9.0/ubiops/models/attachments_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'id': 'id',
         'destination_name': 'destination_name',
         'sources': 'sources'
     }
 
-    def __init__(self, id=None, destination_name=None, sources=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, destination_name=None, sources=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """AttachmentsList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._destination_name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/audit_list.py` & `ubiops-3.9.0/ubiops/models/audit_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         'action': 'action',
         'user': 'user',
         'event': 'event',
         'object_type': 'object_type',
         'object_name': 'object_name'
     }
 
-    def __init__(self, id=None, date=None, action=None, user=None, event=None, object_type=None, object_name=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, date=None, action=None, user=None, event=None, object_type=None, object_name=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """AuditList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._date = None
```

### Comparing `ubiops-3.8.0/ubiops/models/blob_list.py` & `ubiops-3.9.0/ubiops/models/blob_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         'creation_date': 'creation_date',
         'last_updated': 'last_updated',
         'filename': 'filename',
         'size': 'size',
         'ttl': 'ttl'
     }
 
-    def __init__(self, id=None, created_by=None, creation_date=None, last_updated=None, filename=None, size=None, ttl=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, created_by=None, creation_date=None, last_updated=None, filename=None, size=None, ttl=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """BlobList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._created_by = None
```

### Comparing `ubiops-3.8.0/ubiops/models/build_list.py` & `ubiops-3.9.0/ubiops/models/build_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         'revision': 'revision',
         'creation_date': 'creation_date',
         'status': 'status',
         'error_message': 'error_message',
         'trigger': 'trigger'
     }
 
-    def __init__(self, id=None, revision=None, creation_date=None, status=None, error_message=None, trigger=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, revision=None, creation_date=None, status=None, error_message=None, trigger=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """BuildList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._revision = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_create.py` & `ubiops-3.9.0/ubiops/models/deployment_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         'input_type': 'input_type',
         'output_type': 'output_type',
         'input_fields': 'input_fields',
         'output_fields': 'output_fields',
         'labels': 'labels'
     }
 
-    def __init__(self, name=None, description=None, input_type=None, output_type=None, input_fields=None, output_fields=None, labels=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, description=None, input_type=None, output_type=None, input_fields=None, output_fields=None, labels=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._description = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_create_response.py` & `ubiops-3.9.0/ubiops/models/deployment_create_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         'input_fields': 'input_fields',
         'output_fields': 'output_fields',
         'labels': 'labels',
         'creation_date': 'creation_date',
         'last_updated': 'last_updated'
     }
 
-    def __init__(self, id=None, name=None, project=None, description=None, input_type=None, output_type=None, input_fields=None, output_fields=None, labels=None, creation_date=None, last_updated=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, project=None, description=None, input_type=None, output_type=None, input_fields=None, output_fields=None, labels=None, creation_date=None, last_updated=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentCreateResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_detail.py` & `ubiops-3.9.0/ubiops/models/deployment_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         'output_fields': 'output_fields',
         'labels': 'labels',
         'creation_date': 'creation_date',
         'last_updated': 'last_updated',
         'default_version': 'default_version'
     }
 
-    def __init__(self, id=None, name=None, project=None, description=None, input_type=None, output_type=None, input_fields=None, output_fields=None, labels=None, creation_date=None, last_updated=None, default_version=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, project=None, description=None, input_type=None, output_type=None, input_fields=None, output_fields=None, labels=None, creation_date=None, last_updated=None, default_version=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_input_field_create.py` & `ubiops-3.9.0/ubiops/models/deployment_input_field_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'name': 'name',
         'data_type': 'data_type',
         'widget': 'widget'
     }
 
-    def __init__(self, name=None, data_type=None, widget=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, data_type=None, widget=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentInputFieldCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._data_type = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_input_field_detail.py` & `ubiops-3.9.0/ubiops/models/deployment_input_field_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'name': 'name',
         'data_type': 'data_type',
         'widget': 'widget'
     }
 
-    def __init__(self, name=None, data_type=None, widget=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, data_type=None, widget=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentInputFieldDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._data_type = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_input_field_list.py` & `ubiops-3.9.0/ubiops/models/deployment_input_field_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'name': 'name',
         'data_type': 'data_type'
     }
 
-    def __init__(self, name=None, data_type=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, data_type=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentInputFieldList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._data_type = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_input_field_widget_create.py` & `ubiops-3.9.0/ubiops/models/deployment_input_field_widget_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'type': 'type',
         'configuration': 'configuration'
     }
 
-    def __init__(self, type=None, configuration=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, type=None, configuration=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentInputFieldWidgetCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._type = None
         self._configuration = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_instance_type.py` & `ubiops-3.9.0/ubiops/models/deployment_instance_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,51 +29,56 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'id': 'str',
         'name': 'str',
         'display_name': 'str',
         'memory_allocation': 'int',
         'cpu_allocation': 'int',
         'gpu_allocation': 'int',
         'gpu_enabled': 'str',
         'gpu_memory_allocation': 'int',
         'gpu_type': 'str'
     }
 
     attribute_map = {
+        'id': 'id',
         'name': 'name',
         'display_name': 'display_name',
         'memory_allocation': 'memory_allocation',
         'cpu_allocation': 'cpu_allocation',
         'gpu_allocation': 'gpu_allocation',
         'gpu_enabled': 'gpu_enabled',
         'gpu_memory_allocation': 'gpu_memory_allocation',
         'gpu_type': 'gpu_type'
     }
 
-    def __init__(self, name=None, display_name=None, memory_allocation=None, cpu_allocation=None, gpu_allocation=None, gpu_enabled=None, gpu_memory_allocation=None, gpu_type=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, display_name=None, memory_allocation=None, cpu_allocation=None, gpu_allocation=None, gpu_enabled=None, gpu_memory_allocation=None, gpu_type=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentInstanceType - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._id = None
         self._name = None
         self._display_name = None
         self._memory_allocation = None
         self._cpu_allocation = None
         self._gpu_allocation = None
         self._gpu_enabled = None
         self._gpu_memory_allocation = None
         self._gpu_type = None
         self.discriminator = None
 
+        if id is not None:
+            self.id = id
         self.name = name
         self.display_name = display_name
         if memory_allocation is not None:
             self.memory_allocation = memory_allocation
         if cpu_allocation is not None:
             self.cpu_allocation = cpu_allocation
         if gpu_allocation is not None:
@@ -81,14 +86,38 @@
         if gpu_enabled is not None:
             self.gpu_enabled = gpu_enabled
         if gpu_memory_allocation is not None:
             self.gpu_memory_allocation = gpu_memory_allocation
         self.gpu_type = gpu_type
 
     @property
+    def id(self):
+        """Gets the id of this DeploymentInstanceType.  # noqa: E501
+
+
+        :return: The id of this DeploymentInstanceType.  # noqa: E501
+        :rtype: str
+        """
+        return self._id
+
+    @id.setter
+    def id(self, id):
+        """Sets the id of this DeploymentInstanceType.
+
+
+        :param id: The id of this DeploymentInstanceType.  # noqa: E501
+        :type: str
+        """
+        if (self.local_vars_configuration.client_side_validation and
+                id is not None and not isinstance(id, str)):
+            raise ValueError("Parameter `id` must be a string")  # noqa: E501
+
+        self._id = id
+
+    @property
     def name(self):
         """Gets the name of this DeploymentInstanceType.  # noqa: E501
 
 
         :return: The name of this DeploymentInstanceType.  # noqa: E501
         :rtype: str
         """
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_list.py` & `ubiops-3.9.0/ubiops/models/deployment_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         'output_fields': 'output_fields',
         'labels': 'labels',
         'creation_date': 'creation_date',
         'last_updated': 'last_updated',
         'number_of_versions': 'number_of_versions'
     }
 
-    def __init__(self, id=None, name=None, project=None, description=None, input_type=None, output_type=None, input_fields=None, output_fields=None, labels=None, creation_date=None, last_updated=None, number_of_versions=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, project=None, description=None, input_type=None, output_type=None, input_fields=None, output_fields=None, labels=None, creation_date=None, last_updated=None, number_of_versions=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_output_field_create.py` & `ubiops-3.9.0/ubiops/models/deployment_output_field_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'name': 'name',
         'data_type': 'data_type',
         'widget': 'widget'
     }
 
-    def __init__(self, name=None, data_type=None, widget=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, data_type=None, widget=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentOutputFieldCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._data_type = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_output_field_detail.py` & `ubiops-3.9.0/ubiops/models/deployment_output_field_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'name': 'name',
         'data_type': 'data_type',
         'widget': 'widget'
     }
 
-    def __init__(self, name=None, data_type=None, widget=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, data_type=None, widget=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentOutputFieldDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._data_type = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_output_field_list.py` & `ubiops-3.9.0/ubiops/models/deployment_output_field_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'name': 'name',
         'data_type': 'data_type'
     }
 
-    def __init__(self, name=None, data_type=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, data_type=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentOutputFieldList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._data_type = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_output_field_widget_create.py` & `ubiops-3.9.0/ubiops/models/deployment_output_field_widget_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'type': 'type',
         'configuration': 'configuration'
     }
 
-    def __init__(self, type=None, configuration=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, type=None, configuration=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentOutputFieldWidgetCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._type = None
         self._configuration = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_request_batch_create_response.py` & `ubiops-3.9.0/ubiops/models/deployment_request_batch_create_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         'id': 'id',
         'deployment': 'deployment',
         'version': 'version',
         'status': 'status',
         'time_created': 'time_created'
     }
 
-    def __init__(self, id=None, deployment=None, version=None, status=None, time_created=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, deployment=None, version=None, status=None, time_created=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentRequestBatchCreateResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._deployment = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_request_batch_detail.py` & `ubiops-3.9.0/ubiops/models/deployment_request_batch_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         'time_started': 'time_started',
         'time_completed': 'time_completed',
         'error_message': 'error_message',
         'request_data': 'request_data',
         'result': 'result'
     }
 
-    def __init__(self, id=None, deployment=None, version=None, status=None, success=None, time_created=None, time_started=None, time_completed=None, error_message=None, request_data=None, result=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, deployment=None, version=None, status=None, success=None, time_created=None, time_started=None, time_completed=None, error_message=None, request_data=None, result=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentRequestBatchDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._deployment = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_request_create_response.py` & `ubiops-3.9.0/ubiops/models/deployment_request_create_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         'deployment': 'deployment',
         'version': 'version',
         'success': 'success',
         'result': 'result',
         'error_message': 'error_message'
     }
 
-    def __init__(self, id=None, deployment=None, version=None, success=None, result=None, error_message=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, deployment=None, version=None, success=None, result=None, error_message=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentRequestCreateResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._deployment = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_request_list.py` & `ubiops-3.9.0/ubiops/models/deployment_request_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         'status': 'status',
         'success': 'success',
         'time_created': 'time_created',
         'time_started': 'time_started',
         'time_completed': 'time_completed'
     }
 
-    def __init__(self, id=None, deployment=None, version=None, status=None, success=None, time_created=None, time_started=None, time_completed=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, deployment=None, version=None, status=None, success=None, time_created=None, time_started=None, time_completed=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentRequestList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._deployment = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_request_single_detail.py` & `ubiops-3.9.0/ubiops/models/deployment_request_single_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         'error_message': 'error_message',
         'request_data': 'request_data',
         'result': 'result',
         'notification_group': 'notification_group',
         'origin': 'origin'
     }
 
-    def __init__(self, id=None, deployment=None, version=None, status=None, success=None, time_created=None, time_started=None, time_completed=None, error_message=None, request_data=None, result=None, notification_group=None, origin=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, deployment=None, version=None, status=None, success=None, time_created=None, time_started=None, time_completed=None, error_message=None, request_data=None, result=None, notification_group=None, origin=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentRequestSingleDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._deployment = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_request_update.py` & `ubiops-3.9.0/ubiops/models/deployment_request_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'status': 'status',
         'notification_group': 'notification_group'
     }
 
-    def __init__(self, status=None, notification_group=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, status=None, notification_group=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentRequestUpdate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._status = None
         self._notification_group = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_request_update_response.py` & `ubiops-3.9.0/ubiops/models/deployment_request_update_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         'time_completed': 'time_completed',
         'error_message': 'error_message',
         'request_data': 'request_data',
         'result': 'result',
         'notification_group': 'notification_group'
     }
 
-    def __init__(self, id=None, deployment=None, version=None, status=None, success=None, time_created=None, time_started=None, time_completed=None, error_message=None, request_data=None, result=None, notification_group=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, deployment=None, version=None, status=None, success=None, time_created=None, time_started=None, time_completed=None, error_message=None, request_data=None, result=None, notification_group=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentRequestUpdateResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._deployment = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_update.py` & `ubiops-3.9.0/ubiops/models/deployment_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         'default_version': 'default_version',
         'description': 'description',
         'input_fields': 'input_fields',
         'output_fields': 'output_fields',
         'labels': 'labels'
     }
 
-    def __init__(self, name=None, default_version=None, description=None, input_fields=None, output_fields=None, labels=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, default_version=None, description=None, input_fields=None, output_fields=None, labels=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentUpdate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._default_version = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_version_create.py` & `ubiops-3.9.0/ubiops/models/deployment_version_create.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,14 @@
         'minimum_instances': 'int',
         'maximum_idle_time': 'int',
         'description': 'str',
         'labels': 'dict(str, str)',
         'monitoring': 'str',
         'request_retention_time': 'int',
         'request_retention_mode': 'str',
-        'deployment_mode': 'str',
         'default_notification_group': 'str'
     }
 
     attribute_map = {
         'version': 'version',
         'language': 'language',
         'memory_allocation': 'memory_allocation',
@@ -58,19 +57,18 @@
         'minimum_instances': 'minimum_instances',
         'maximum_idle_time': 'maximum_idle_time',
         'description': 'description',
         'labels': 'labels',
         'monitoring': 'monitoring',
         'request_retention_time': 'request_retention_time',
         'request_retention_mode': 'request_retention_mode',
-        'deployment_mode': 'deployment_mode',
         'default_notification_group': 'default_notification_group'
     }
 
-    def __init__(self, version=None, language='python3.7', memory_allocation=None, instance_type=None, maximum_instances=None, minimum_instances=None, maximum_idle_time=None, description=None, labels=None, monitoring=None, request_retention_time=None, request_retention_mode='full', deployment_mode='express', default_notification_group=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, version=None, language='python3.7', memory_allocation=None, instance_type=None, maximum_instances=None, minimum_instances=None, maximum_idle_time=None, description=None, labels=None, monitoring=None, request_retention_time=None, request_retention_mode='full', default_notification_group=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentVersionCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._version = None
         self._language = None
@@ -80,15 +78,14 @@
         self._minimum_instances = None
         self._maximum_idle_time = None
         self._description = None
         self._labels = None
         self._monitoring = None
         self._request_retention_time = None
         self._request_retention_mode = None
-        self._deployment_mode = None
         self._default_notification_group = None
         self.discriminator = None
 
         self.version = version
         if language is not None:
             self.language = language
         if memory_allocation is not None:
@@ -105,16 +102,14 @@
             self.description = description
         self.labels = labels
         self.monitoring = monitoring
         if request_retention_time is not None:
             self.request_retention_time = request_retention_time
         if request_retention_mode is not None:
             self.request_retention_mode = request_retention_mode
-        if deployment_mode is not None:
-            self.deployment_mode = deployment_mode
         self.default_notification_group = default_notification_group
 
     @property
     def version(self):
         """Gets the version of this DeploymentVersionCreate.  # noqa: E501
 
 
@@ -422,44 +417,14 @@
                 "Invalid value for `request_retention_mode` ({0}), must be one of {1}"  # noqa: E501
                 .format(request_retention_mode, allowed_values)
             )
 
         self._request_retention_mode = request_retention_mode
 
     @property
-    def deployment_mode(self):
-        """Gets the deployment_mode of this DeploymentVersionCreate.  # noqa: E501
-
-
-        :return: The deployment_mode of this DeploymentVersionCreate.  # noqa: E501
-        :rtype: str
-        """
-        return self._deployment_mode
-
-    @deployment_mode.setter
-    def deployment_mode(self, deployment_mode):
-        """Sets the deployment_mode of this DeploymentVersionCreate.
-
-
-        :param deployment_mode: The deployment_mode of this DeploymentVersionCreate.  # noqa: E501
-        :type: str
-        """
-        if (self.local_vars_configuration.client_side_validation and
-                deployment_mode is not None and not isinstance(deployment_mode, str)):
-            raise ValueError("Parameter `deployment_mode` must be a string")  # noqa: E501
-        allowed_values = ["express", "batch"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and deployment_mode not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `deployment_mode` ({0}), must be one of {1}"  # noqa: E501
-                .format(deployment_mode, allowed_values)
-            )
-
-        self._deployment_mode = deployment_mode
-
-    @property
     def default_notification_group(self):
         """Gets the default_notification_group of this DeploymentVersionCreate.  # noqa: E501
 
 
         :return: The default_notification_group of this DeploymentVersionCreate.  # noqa: E501
         :rtype: str
         """
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_version_detail.py` & `ubiops-3.9.0/ubiops/models/deployment_version_detail.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,14 @@
         'labels': 'dict(str, str)',
         'creation_date': 'datetime',
         'last_updated': 'datetime',
         'last_file_upload': 'datetime',
         'monitoring': 'str',
         'request_retention_time': 'int',
         'request_retention_mode': 'str',
-        'deployment_mode': 'str',
         'default_notification_group': 'str'
     }
 
     attribute_map = {
         'id': 'id',
         'deployment': 'deployment',
         'version': 'version',
@@ -74,19 +73,18 @@
         'labels': 'labels',
         'creation_date': 'creation_date',
         'last_updated': 'last_updated',
         'last_file_upload': 'last_file_upload',
         'monitoring': 'monitoring',
         'request_retention_time': 'request_retention_time',
         'request_retention_mode': 'request_retention_mode',
-        'deployment_mode': 'deployment_mode',
         'default_notification_group': 'default_notification_group'
     }
 
-    def __init__(self, id=None, deployment=None, version=None, description=None, language=None, status=None, active_revision=None, latest_build=None, memory_allocation=None, instance_type=None, maximum_instances=None, minimum_instances=None, maximum_idle_time=None, labels=None, creation_date=None, last_updated=None, last_file_upload=None, monitoring=None, request_retention_time=None, request_retention_mode=None, deployment_mode=None, default_notification_group=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, deployment=None, version=None, description=None, language=None, status=None, active_revision=None, latest_build=None, memory_allocation=None, instance_type=None, maximum_instances=None, minimum_instances=None, maximum_idle_time=None, labels=None, creation_date=None, last_updated=None, last_file_upload=None, monitoring=None, request_retention_time=None, request_retention_mode=None, default_notification_group=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentVersionDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._deployment = None
@@ -104,15 +102,14 @@
         self._labels = None
         self._creation_date = None
         self._last_updated = None
         self._last_file_upload = None
         self._monitoring = None
         self._request_retention_time = None
         self._request_retention_mode = None
-        self._deployment_mode = None
         self._default_notification_group = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         self.deployment = deployment
         self.version = version
@@ -143,15 +140,14 @@
         if last_file_upload is not None:
             self.last_file_upload = last_file_upload
         if monitoring is not None:
             self.monitoring = monitoring
         if request_retention_time is not None:
             self.request_retention_time = request_retention_time
         self.request_retention_mode = request_retention_mode
-        self.deployment_mode = deployment_mode
         if default_notification_group is not None:
             self.default_notification_group = default_notification_group
 
     @property
     def id(self):
         """Gets the id of this DeploymentVersionDetail.  # noqa: E501
 
@@ -657,44 +653,14 @@
         if (self.local_vars_configuration.client_side_validation and
                 request_retention_mode is not None and len(request_retention_mode) < 1):
             raise ValueError("Invalid value for `request_retention_mode`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._request_retention_mode = request_retention_mode
 
     @property
-    def deployment_mode(self):
-        """Gets the deployment_mode of this DeploymentVersionDetail.  # noqa: E501
-
-
-        :return: The deployment_mode of this DeploymentVersionDetail.  # noqa: E501
-        :rtype: str
-        """
-        return self._deployment_mode
-
-    @deployment_mode.setter
-    def deployment_mode(self, deployment_mode):
-        """Sets the deployment_mode of this DeploymentVersionDetail.
-
-
-        :param deployment_mode: The deployment_mode of this DeploymentVersionDetail.  # noqa: E501
-        :type: str
-        """
-        if self.local_vars_configuration.client_side_validation and deployment_mode is None:  # noqa: E501
-            raise ValueError("Invalid value for `deployment_mode`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                deployment_mode is not None and not isinstance(deployment_mode, str)):
-            raise ValueError("Parameter `deployment_mode` must be a string")  # noqa: E501
-
-        if (self.local_vars_configuration.client_side_validation and
-                deployment_mode is not None and len(deployment_mode) < 1):
-            raise ValueError("Invalid value for `deployment_mode`, length must be greater than or equal to `1`")  # noqa: E501
-
-        self._deployment_mode = deployment_mode
-
-    @property
     def default_notification_group(self):
         """Gets the default_notification_group of this DeploymentVersionDetail.  # noqa: E501
 
 
         :return: The default_notification_group of this DeploymentVersionDetail.  # noqa: E501
         :rtype: str
         """
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_version_list.py` & `ubiops-3.9.0/ubiops/models/deployment_version_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         'minimum_instances': 'int',
         'maximum_idle_time': 'int',
         'labels': 'dict(str, str)',
         'creation_date': 'datetime',
         'last_updated': 'datetime',
         'request_retention_time': 'int',
         'request_retention_mode': 'str',
-        'deployment_mode': 'str',
         'monitoring': 'str',
         'default_notification_group': 'str'
     }
 
     attribute_map = {
         'id': 'id',
         'deployment': 'deployment',
@@ -71,20 +70,19 @@
         'minimum_instances': 'minimum_instances',
         'maximum_idle_time': 'maximum_idle_time',
         'labels': 'labels',
         'creation_date': 'creation_date',
         'last_updated': 'last_updated',
         'request_retention_time': 'request_retention_time',
         'request_retention_mode': 'request_retention_mode',
-        'deployment_mode': 'deployment_mode',
         'monitoring': 'monitoring',
         'default_notification_group': 'default_notification_group'
     }
 
-    def __init__(self, id=None, deployment=None, version=None, description=None, language=None, status=None, active_revision=None, latest_build=None, memory_allocation=None, instance_type=None, maximum_instances=None, minimum_instances=None, maximum_idle_time=None, labels=None, creation_date=None, last_updated=None, request_retention_time=None, request_retention_mode=None, deployment_mode=None, monitoring=None, default_notification_group=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, deployment=None, version=None, description=None, language=None, status=None, active_revision=None, latest_build=None, memory_allocation=None, instance_type=None, maximum_instances=None, minimum_instances=None, maximum_idle_time=None, labels=None, creation_date=None, last_updated=None, request_retention_time=None, request_retention_mode=None, monitoring=None, default_notification_group=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentVersionList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._deployment = None
@@ -100,15 +98,14 @@
         self._minimum_instances = None
         self._maximum_idle_time = None
         self._labels = None
         self._creation_date = None
         self._last_updated = None
         self._request_retention_time = None
         self._request_retention_mode = None
-        self._deployment_mode = None
         self._monitoring = None
         self._default_notification_group = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         self.deployment = deployment
@@ -136,15 +133,14 @@
         if creation_date is not None:
             self.creation_date = creation_date
         if last_updated is not None:
             self.last_updated = last_updated
         if request_retention_time is not None:
             self.request_retention_time = request_retention_time
         self.request_retention_mode = request_retention_mode
-        self.deployment_mode = deployment_mode
         if monitoring is not None:
             self.monitoring = monitoring
         if default_notification_group is not None:
             self.default_notification_group = default_notification_group
 
     @property
     def id(self):
@@ -607,44 +603,14 @@
         if (self.local_vars_configuration.client_side_validation and
                 request_retention_mode is not None and len(request_retention_mode) < 1):
             raise ValueError("Invalid value for `request_retention_mode`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._request_retention_mode = request_retention_mode
 
     @property
-    def deployment_mode(self):
-        """Gets the deployment_mode of this DeploymentVersionList.  # noqa: E501
-
-
-        :return: The deployment_mode of this DeploymentVersionList.  # noqa: E501
-        :rtype: str
-        """
-        return self._deployment_mode
-
-    @deployment_mode.setter
-    def deployment_mode(self, deployment_mode):
-        """Sets the deployment_mode of this DeploymentVersionList.
-
-
-        :param deployment_mode: The deployment_mode of this DeploymentVersionList.  # noqa: E501
-        :type: str
-        """
-        if self.local_vars_configuration.client_side_validation and deployment_mode is None:  # noqa: E501
-            raise ValueError("Invalid value for `deployment_mode`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                deployment_mode is not None and not isinstance(deployment_mode, str)):
-            raise ValueError("Parameter `deployment_mode` must be a string")  # noqa: E501
-
-        if (self.local_vars_configuration.client_side_validation and
-                deployment_mode is not None and len(deployment_mode) < 1):
-            raise ValueError("Invalid value for `deployment_mode`, length must be greater than or equal to `1`")  # noqa: E501
-
-        self._deployment_mode = deployment_mode
-
-    @property
     def monitoring(self):
         """Gets the monitoring of this DeploymentVersionList.  # noqa: E501
 
 
         :return: The monitoring of this DeploymentVersionList.  # noqa: E501
         :rtype: str
         """
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_version_update.py` & `ubiops-3.9.0/ubiops/models/deployment_version_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         'labels': 'labels',
         'monitoring': 'monitoring',
         'request_retention_time': 'request_retention_time',
         'request_retention_mode': 'request_retention_mode',
         'default_notification_group': 'default_notification_group'
     }
 
-    def __init__(self, version=None, memory_allocation=None, instance_type=None, maximum_instances=None, minimum_instances=None, maximum_idle_time=None, description=None, labels=None, monitoring=None, request_retention_time=None, request_retention_mode=None, default_notification_group=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, version=None, memory_allocation=None, instance_type=None, maximum_instances=None, minimum_instances=None, maximum_idle_time=None, description=None, labels=None, monitoring=None, request_retention_time=None, request_retention_mode=None, default_notification_group=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentVersionUpdate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._version = None
         self._memory_allocation = None
```

### Comparing `ubiops-3.8.0/ubiops/models/deployment_widget_list.py` & `ubiops-3.9.0/ubiops/models/deployment_widget_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'type': 'type',
         'configuration': 'configuration'
     }
 
-    def __init__(self, type=None, configuration=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, type=None, configuration=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DeploymentWidgetList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._type = None
         self._configuration = None
```

### Comparing `ubiops-3.8.0/ubiops/models/direct_pipeline_request_deployment_request.py` & `ubiops-3.9.0/ubiops/models/direct_pipeline_request_deployment_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         'pipeline_object': 'pipeline_object',
         'deployment': 'deployment',
         'version': 'version',
         'success': 'success',
         'error_message': 'error_message'
     }
 
-    def __init__(self, id=None, pipeline_object=None, deployment=None, version=None, success=None, error_message=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, pipeline_object=None, deployment=None, version=None, success=None, error_message=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """DirectPipelineRequestDeploymentRequest - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._pipeline_object = None
```

### Comparing `ubiops-3.8.0/ubiops/models/environment_variable_copy.py` & `ubiops-3.9.0/ubiops/models/environment_variable_copy.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'source_deployment': 'source_deployment',
         'source_version': 'source_version'
     }
 
-    def __init__(self, source_deployment=None, source_version=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, source_deployment=None, source_version=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """EnvironmentVariableCopy - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._source_deployment = None
         self._source_version = None
```

### Comparing `ubiops-3.8.0/ubiops/models/environment_variable_create.py` & `ubiops-3.9.0/ubiops/models/environment_variable_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'name': 'name',
         'value': 'value',
         'secret': 'secret'
     }
 
-    def __init__(self, name=None, value=None, secret=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, value=None, secret=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """EnvironmentVariableCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._value = None
```

### Comparing `ubiops-3.8.0/ubiops/models/environment_variable_list.py` & `ubiops-3.9.0/ubiops/models/environment_variable_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     attribute_map = {
         'id': 'id',
         'name': 'name',
         'value': 'value',
         'secret': 'secret'
     }
 
-    def __init__(self, id=None, name=None, value=None, secret=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, value=None, secret=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """EnvironmentVariableList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/export_create.py` & `ubiops-3.9.0/ubiops/models/export_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'deployments': 'deployments',
         'pipelines': 'pipelines',
         'environment_variables': 'environment_variables'
     }
 
-    def __init__(self, deployments=None, pipelines=None, environment_variables=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, deployments=None, pipelines=None, environment_variables=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ExportCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._deployments = None
         self._pipelines = None
```

### Comparing `ubiops-3.8.0/ubiops/models/export_detail.py` & `ubiops-3.9.0/ubiops/models/export_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         'error_message': 'error_message',
         'size': 'size',
         'deployments': 'deployments',
         'pipelines': 'pipelines',
         'environment_variables': 'environment_variables'
     }
 
-    def __init__(self, id=None, exported_by=None, creation_date=None, status='pending', error_message=None, size=None, deployments=None, pipelines=None, environment_variables=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, exported_by=None, creation_date=None, status='pending', error_message=None, size=None, deployments=None, pipelines=None, environment_variables=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ExportDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._exported_by = None
```

### Comparing `ubiops-3.8.0/ubiops/models/export_list.py` & `ubiops-3.9.0/ubiops/models/export_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         'exported_by': 'exported_by',
         'creation_date': 'creation_date',
         'status': 'status',
         'error_message': 'error_message',
         'size': 'size'
     }
 
-    def __init__(self, id=None, exported_by=None, creation_date=None, status='pending', error_message=None, size=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, exported_by=None, creation_date=None, status='pending', error_message=None, size=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ExportList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._exported_by = None
```

### Comparing `ubiops-3.8.0/ubiops/models/import_detail.py` & `ubiops-3.9.0/ubiops/models/import_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         'error_message': 'error_message',
         'size': 'size',
         'deployments': 'deployments',
         'pipelines': 'pipelines',
         'environment_variables': 'environment_variables'
     }
 
-    def __init__(self, id=None, imported_by=None, creation_date=None, status='pending', error_message=None, size=None, deployments=None, pipelines=None, environment_variables=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, imported_by=None, creation_date=None, status='pending', error_message=None, size=None, deployments=None, pipelines=None, environment_variables=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ImportDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._imported_by = None
```

### Comparing `ubiops-3.8.0/ubiops/models/import_list.py` & `ubiops-3.9.0/ubiops/models/import_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         'imported_by': 'imported_by',
         'creation_date': 'creation_date',
         'status': 'status',
         'error_message': 'error_message',
         'size': 'size'
     }
 
-    def __init__(self, id=None, imported_by=None, creation_date=None, status='pending', error_message=None, size=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, imported_by=None, creation_date=None, status='pending', error_message=None, size=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ImportList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._imported_by = None
```

### Comparing `ubiops-3.8.0/ubiops/models/import_update.py` & `ubiops-3.9.0/ubiops/models/import_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'deployments': 'deployments',
         'pipelines': 'pipelines',
         'environment_variables': 'environment_variables'
     }
 
-    def __init__(self, deployments=None, pipelines=None, environment_variables=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, deployments=None, pipelines=None, environment_variables=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ImportUpdate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._deployments = None
         self._pipelines = None
```

### Comparing `ubiops-3.8.0/ubiops/models/inherited_environment_variable_list.py` & `ubiops-3.9.0/ubiops/models/inherited_environment_variable_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         'name': 'name',
         'value': 'value',
         'secret': 'secret',
         'inheritance_type': 'inheritance_type',
         'inheritance_name': 'inheritance_name'
     }
 
-    def __init__(self, id=None, name=None, value=None, secret=None, inheritance_type=None, inheritance_name=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, value=None, secret=None, inheritance_type=None, inheritance_name=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """InheritedEnvironmentVariableList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/logs.py` & `ubiops-3.9.0/ubiops/models/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         'deployment_request_id': 'deployment_request_id',
         'pipeline_request_id': 'pipeline_request_id',
         'build_id': 'build_id',
         'system': 'system',
         'level': 'level'
     }
 
-    def __init__(self, id=None, log=None, date=None, deployment_name=None, deployment_version=None, pipeline_name=None, pipeline_version=None, pipeline_object_name=None, deployment_request_id=None, pipeline_request_id=None, build_id=None, system=None, level=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, log=None, date=None, deployment_name=None, deployment_version=None, pipeline_name=None, pipeline_version=None, pipeline_object_name=None, deployment_request_id=None, pipeline_request_id=None, build_id=None, system=None, level=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """Logs - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._log = None
```

### Comparing `ubiops-3.8.0/ubiops/models/logs_create.py` & `ubiops-3.9.0/ubiops/models/logs_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         'filters': 'filters',
         'date_range': 'date_range',
         'date': 'date',
         'id': 'id',
         'limit': 'limit'
     }
 
-    def __init__(self, filters=None, date_range=None, date=None, id=None, limit=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, filters=None, date_range=None, date=None, id=None, limit=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """LogsCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._filters = None
         self._date_range = None
```

### Comparing `ubiops-3.8.0/ubiops/models/metrics.py` & `ubiops-3.9.0/ubiops/models/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'value': 'value',
         'start_date': 'start_date',
         'end_date': 'end_date'
     }
 
-    def __init__(self, value=None, start_date=None, end_date=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, value=None, start_date=None, end_date=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """Metrics - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._value = None
         self._start_date = None
```

### Comparing `ubiops-3.8.0/ubiops/models/notification_group_contact.py` & `ubiops-3.9.0/ubiops/models/notification_group_contact.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'type': 'type',
         'configuration': 'configuration'
     }
 
-    def __init__(self, type=None, configuration=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, type=None, configuration=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """NotificationGroupContact - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._type = None
         self._configuration = None
```

### Comparing `ubiops-3.8.0/ubiops/models/notification_group_create.py` & `ubiops-3.9.0/ubiops/models/notification_group_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'name': 'name',
         'contacts': 'contacts'
     }
 
-    def __init__(self, name=None, contacts=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, contacts=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """NotificationGroupCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._contacts = None
```

### Comparing `ubiops-3.8.0/ubiops/models/notification_group_list.py` & `ubiops-3.9.0/ubiops/models/notification_group_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'id': 'id',
         'name': 'name',
         'contacts': 'contacts'
     }
 
-    def __init__(self, id=None, name=None, contacts=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, contacts=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """NotificationGroupList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/notification_group_update.py` & `ubiops-3.9.0/ubiops/models/notification_group_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'name': 'name',
         'contacts': 'contacts'
     }
 
-    def __init__(self, name=None, contacts=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, contacts=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """NotificationGroupUpdate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._contacts = None
```

### Comparing `ubiops-3.8.0/ubiops/models/organization_create.py` & `ubiops-3.9.0/ubiops/models/organization_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'name': 'name',
         'subscription': 'subscription',
         'subscription_end_date': 'subscription_end_date'
     }
 
-    def __init__(self, name=None, subscription=None, subscription_end_date=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, subscription=None, subscription_end_date=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """OrganizationCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._subscription = None
```

### Comparing `ubiops-3.8.0/ubiops/models/organization_detail.py` & `ubiops-3.9.0/ubiops/models/organization_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         'name': 'name',
         'creation_date': 'creation_date',
         'subscription': 'subscription',
         'status': 'status',
         'subscription_self_service': 'subscription_self_service'
     }
 
-    def __init__(self, id=None, name=None, creation_date=None, subscription=None, status=None, subscription_self_service=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, creation_date=None, subscription=None, status=None, subscription_self_service=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """OrganizationDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/organization_list.py` & `ubiops-3.9.0/ubiops/models/organization_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'id': 'id',
         'name': 'name',
         'creation_date': 'creation_date'
     }
 
-    def __init__(self, id=None, name=None, creation_date=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, creation_date=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """OrganizationList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/organization_update.py` & `ubiops-3.9.0/ubiops/models/organization_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     attribute_map = {
         'name': 'name',
         'subscription': 'subscription',
         'subscription_end_date': 'subscription_end_date',
         'subscription_start_date': 'subscription_start_date'
     }
 
-    def __init__(self, name=None, subscription=None, subscription_end_date=None, subscription_start_date=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, subscription=None, subscription_end_date=None, subscription_start_date=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """OrganizationUpdate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._subscription = None
```

### Comparing `ubiops-3.8.0/ubiops/models/organization_user_create.py` & `ubiops-3.9.0/ubiops/models/organization_user_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'email': 'email',
         'admin': 'admin'
     }
 
-    def __init__(self, email=None, admin=False, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, email=None, admin=False, local_vars_configuration=None, **kwargs):  # noqa: E501
         """OrganizationUserCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._email = None
         self._admin = None
```

### Comparing `ubiops-3.8.0/ubiops/models/organization_user_detail.py` & `ubiops-3.9.0/ubiops/models/organization_user_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         'email': 'email',
         'name': 'name',
         'surname': 'surname',
         'status': 'status',
         'admin': 'admin'
     }
 
-    def __init__(self, id=None, email=None, name=None, surname=None, status=None, admin=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, email=None, name=None, surname=None, status=None, admin=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """OrganizationUserDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._email = None
```

### Comparing `ubiops-3.8.0/ubiops/models/organization_user_update.py` & `ubiops-3.9.0/ubiops/models/organization_user_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         'admin': 'bool'
     }
 
     attribute_map = {
         'admin': 'admin'
     }
 
-    def __init__(self, admin=False, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, admin=False, local_vars_configuration=None, **kwargs):  # noqa: E501
         """OrganizationUserUpdate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._admin = None
         self.discriminator = None
```

### Comparing `ubiops-3.8.0/ubiops/models/permission_list.py` & `ubiops-3.9.0/ubiops/models/permission_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         'name': 'str'
     }
 
     attribute_map = {
         'name': 'name'
     }
 
-    def __init__(self, name=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PermissionList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self.discriminator = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_create.py` & `ubiops-3.9.0/ubiops/models/pipeline_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         'input_type': 'input_type',
         'input_fields': 'input_fields',
         'output_type': 'output_type',
         'output_fields': 'output_fields',
         'labels': 'labels'
     }
 
-    def __init__(self, name=None, description=None, input_type=None, input_fields=None, output_type=None, output_fields=None, labels=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, description=None, input_type=None, input_fields=None, output_type=None, output_fields=None, labels=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._description = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_create_response.py` & `ubiops-3.9.0/ubiops/models/pipeline_create_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         'output_type': 'output_type',
         'output_fields': 'output_fields',
         'labels': 'labels',
         'creation_date': 'creation_date',
         'last_updated': 'last_updated'
     }
 
-    def __init__(self, id=None, name=None, project=None, description=None, input_type=None, input_fields=None, output_type=None, output_fields=None, labels=None, creation_date=None, last_updated=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, project=None, description=None, input_type=None, input_fields=None, output_type=None, output_fields=None, labels=None, creation_date=None, last_updated=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineCreateResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_detail.py` & `ubiops-3.9.0/ubiops/models/pipeline_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         'output_fields': 'output_fields',
         'labels': 'labels',
         'creation_date': 'creation_date',
         'last_updated': 'last_updated',
         'default_version': 'default_version'
     }
 
-    def __init__(self, id=None, name=None, project=None, description=None, input_type=None, input_fields=None, output_type=None, output_fields=None, labels=None, creation_date=None, last_updated=None, default_version=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, project=None, description=None, input_type=None, input_fields=None, output_type=None, output_fields=None, labels=None, creation_date=None, last_updated=None, default_version=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_input_field_create.py` & `ubiops-3.9.0/ubiops/models/pipeline_input_field_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'name': 'name',
         'data_type': 'data_type',
         'widget': 'widget'
     }
 
-    def __init__(self, name=None, data_type=None, widget=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, data_type=None, widget=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineInputFieldCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._data_type = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_input_field_detail.py` & `ubiops-3.9.0/ubiops/models/pipeline_input_field_detail.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'name': 'name',
         'data_type': 'data_type',
         'widget': 'widget'
     }
 
-    def __init__(self, name=None, data_type=None, widget=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, data_type=None, widget=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineInputFieldDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._data_type = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_input_field_list.py` & `ubiops-3.9.0/ubiops/models/pipeline_input_field_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'name': 'name',
         'data_type': 'data_type'
     }
 
-    def __init__(self, name=None, data_type=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, data_type=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineInputFieldList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._data_type = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_input_field_widget_create.py` & `ubiops-3.9.0/ubiops/models/pipeline_input_field_widget_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'type': 'type',
         'configuration': 'configuration'
     }
 
-    def __init__(self, type=None, configuration=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, type=None, configuration=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineInputFieldWidgetCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._type = None
         self._configuration = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_list.py` & `ubiops-3.9.0/ubiops/models/pipeline_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         'output_type': 'output_type',
         'output_fields': 'output_fields',
         'labels': 'labels',
         'creation_date': 'creation_date',
         'last_updated': 'last_updated'
     }
 
-    def __init__(self, id=None, name=None, project=None, description=None, input_type=None, input_fields=None, output_type=None, output_fields=None, labels=None, creation_date=None, last_updated=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, project=None, description=None, input_type=None, input_fields=None, output_type=None, output_fields=None, labels=None, creation_date=None, last_updated=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_output_field_create.py` & `ubiops-3.9.0/ubiops/models/pipeline_output_field_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'name': 'name',
         'data_type': 'data_type',
         'widget': 'widget'
     }
 
-    def __init__(self, name=None, data_type=None, widget=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, data_type=None, widget=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineOutputFieldCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._data_type = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_output_field_detail.py` & `ubiops-3.9.0/ubiops/models/pipeline_output_field_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'name': 'name',
         'data_type': 'data_type',
         'widget': 'widget'
     }
 
-    def __init__(self, name=None, data_type=None, widget=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, data_type=None, widget=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineOutputFieldDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._data_type = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_output_field_list.py` & `ubiops-3.9.0/ubiops/models/pipeline_output_field_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'name': 'name',
         'data_type': 'data_type'
     }
 
-    def __init__(self, name=None, data_type=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, data_type=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineOutputFieldList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._data_type = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_output_field_widget_create.py` & `ubiops-3.9.0/ubiops/models/pipeline_output_field_widget_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'type': 'type',
         'configuration': 'configuration'
     }
 
-    def __init__(self, type=None, configuration=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, type=None, configuration=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineOutputFieldWidgetCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._type = None
         self._configuration = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_request_batch_create_response.py` & `ubiops-3.9.0/ubiops/models/pipeline_request_batch_create_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         'id': 'id',
         'pipeline': 'pipeline',
         'version': 'version',
         'status': 'status',
         'time_created': 'time_created'
     }
 
-    def __init__(self, id=None, pipeline=None, version=None, status=None, time_created=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, pipeline=None, version=None, status=None, time_created=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineRequestBatchCreateResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._pipeline = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_request_create_response.py` & `ubiops-3.9.0/ubiops/models/pipeline_request_create_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         'version': 'version',
         'deployment_requests': 'deployment_requests',
         'result': 'result',
         'success': 'success',
         'error_message': 'error_message'
     }
 
-    def __init__(self, id=None, pipeline=None, version=None, deployment_requests=None, result=None, success=None, error_message=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, pipeline=None, version=None, deployment_requests=None, result=None, success=None, error_message=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineRequestCreateResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._pipeline = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_request_deployment_request.py` & `ubiops-3.9.0/ubiops/models/pipeline_request_deployment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     attribute_map = {
         'id': 'id',
         'pipeline_object': 'pipeline_object',
         'deployment': 'deployment',
         'version': 'version'
     }
 
-    def __init__(self, id=None, pipeline_object=None, deployment=None, version=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, pipeline_object=None, deployment=None, version=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineRequestDeploymentRequest - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._pipeline_object = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_request_detail.py` & `ubiops-3.9.0/ubiops/models/pipeline_request_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         'time_completed': 'time_completed',
         'request_data': 'request_data',
         'result': 'result',
         'deployment_requests': 'deployment_requests',
         'error_message': 'error_message'
     }
 
-    def __init__(self, id=None, pipeline=None, version=None, status=None, success=None, time_created=None, time_started=None, time_completed=None, request_data=None, result=None, deployment_requests=None, error_message=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, pipeline=None, version=None, status=None, success=None, time_created=None, time_started=None, time_completed=None, request_data=None, result=None, deployment_requests=None, error_message=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineRequestDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._pipeline = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_request_list.py` & `ubiops-3.9.0/ubiops/models/pipeline_request_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         'status': 'status',
         'success': 'success',
         'time_created': 'time_created',
         'time_started': 'time_started',
         'time_completed': 'time_completed'
     }
 
-    def __init__(self, id=None, pipeline=None, version=None, status=None, success=None, time_created=None, time_started=None, time_completed=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, pipeline=None, version=None, status=None, success=None, time_created=None, time_started=None, time_completed=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineRequestList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._pipeline = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_request_single_detail.py` & `ubiops-3.9.0/ubiops/models/pipeline_request_single_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         'result': 'result',
         'deployment_requests': 'deployment_requests',
         'error_message': 'error_message',
         'notification_group': 'notification_group',
         'origin': 'origin'
     }
 
-    def __init__(self, id=None, pipeline=None, version=None, status=None, success=None, time_created=None, time_started=None, time_completed=None, request_data=None, result=None, deployment_requests=None, error_message=None, notification_group=None, origin=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, pipeline=None, version=None, status=None, success=None, time_created=None, time_started=None, time_completed=None, request_data=None, result=None, deployment_requests=None, error_message=None, notification_group=None, origin=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineRequestSingleDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._pipeline = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_update.py` & `ubiops-3.9.0/ubiops/models/pipeline_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         'input_fields': 'input_fields',
         'output_type': 'output_type',
         'output_fields': 'output_fields',
         'labels': 'labels',
         'default_version': 'default_version'
     }
 
-    def __init__(self, name=None, description=None, input_type=None, input_fields=None, output_type=None, output_fields=None, labels=None, default_version=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, description=None, input_type=None, input_fields=None, output_type=None, output_fields=None, labels=None, default_version=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineUpdate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._description = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_version_create.py` & `ubiops-3.9.0/ubiops/models/pipeline_version_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         'request_retention_time': 'request_retention_time',
         'request_retention_mode': 'request_retention_mode',
         'default_notification_group': 'default_notification_group',
         'objects': 'objects',
         'attachments': 'attachments'
     }
 
-    def __init__(self, version=None, description=None, labels=None, monitoring=None, request_retention_time=None, request_retention_mode='full', default_notification_group=None, objects=None, attachments=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, version=None, description=None, labels=None, monitoring=None, request_retention_time=None, request_retention_mode='full', default_notification_group=None, objects=None, attachments=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineVersionCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._version = None
         self._description = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_version_detail.py` & `ubiops-3.9.0/ubiops/models/pipeline_version_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         'request_retention_time': 'request_retention_time',
         'request_retention_mode': 'request_retention_mode',
         'default_notification_group': 'default_notification_group',
         'objects': 'objects',
         'attachments': 'attachments'
     }
 
-    def __init__(self, id=None, version=None, pipeline=None, description=None, labels=None, creation_date=None, last_updated=None, monitoring=None, request_retention_time=None, request_retention_mode=None, default_notification_group=None, objects=None, attachments=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, version=None, pipeline=None, description=None, labels=None, creation_date=None, last_updated=None, monitoring=None, request_retention_time=None, request_retention_mode=None, default_notification_group=None, objects=None, attachments=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineVersionDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._version = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_version_list.py` & `ubiops-3.9.0/ubiops/models/pipeline_version_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         'last_updated': 'last_updated',
         'monitoring': 'monitoring',
         'request_retention_time': 'request_retention_time',
         'request_retention_mode': 'request_retention_mode',
         'default_notification_group': 'default_notification_group'
     }
 
-    def __init__(self, id=None, version=None, pipeline=None, description=None, labels=None, creation_date=None, last_updated=None, monitoring=None, request_retention_time=None, request_retention_mode=None, default_notification_group=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, version=None, pipeline=None, description=None, labels=None, creation_date=None, last_updated=None, monitoring=None, request_retention_time=None, request_retention_mode=None, default_notification_group=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineVersionList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._version = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_version_object_create.py` & `ubiops-3.9.0/ubiops/models/pipeline_version_object_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'name': 'name',
         'reference_name': 'reference_name',
         'version': 'version'
     }
 
-    def __init__(self, name=None, reference_name=None, version=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, reference_name=None, version=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineVersionObjectCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._reference_name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_version_object_list.py` & `ubiops-3.9.0/ubiops/models/pipeline_version_object_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,57 +35,53 @@
     openapi_types = {
         'id': 'str',
         'name': 'str',
         'reference_name': 'str',
         'version': 'str',
         'input_type': 'str',
         'output_type': 'str',
-        'deployment_mode': 'str',
         'input_fields': 'list[DeploymentInputFieldCreate]',
         'output_fields': 'list[DeploymentOutputFieldCreate]'
     }
 
     attribute_map = {
         'id': 'id',
         'name': 'name',
         'reference_name': 'reference_name',
         'version': 'version',
         'input_type': 'input_type',
         'output_type': 'output_type',
-        'deployment_mode': 'deployment_mode',
         'input_fields': 'input_fields',
         'output_fields': 'output_fields'
     }
 
-    def __init__(self, id=None, name=None, reference_name=None, version=None, input_type=None, output_type=None, deployment_mode=None, input_fields=None, output_fields=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, reference_name=None, version=None, input_type=None, output_type=None, input_fields=None, output_fields=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineVersionObjectList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
         self._reference_name = None
         self._version = None
         self._input_type = None
         self._output_type = None
-        self._deployment_mode = None
         self._input_fields = None
         self._output_fields = None
         self.discriminator = None
 
         self.id = id
         self.name = name
         self.reference_name = reference_name
         self.version = version
         if input_type is not None:
             self.input_type = input_type
         if output_type is not None:
             self.output_type = output_type
-        self.deployment_mode = deployment_mode
         if input_fields is not None:
             self.input_fields = input_fields
         if output_fields is not None:
             self.output_fields = output_fields
 
     @property
     def id(self):
@@ -250,38 +246,14 @@
         if (self.local_vars_configuration.client_side_validation and
                 output_type is not None and len(output_type) < 1):
             raise ValueError("Invalid value for `output_type`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._output_type = output_type
 
     @property
-    def deployment_mode(self):
-        """Gets the deployment_mode of this PipelineVersionObjectList.  # noqa: E501
-
-
-        :return: The deployment_mode of this PipelineVersionObjectList.  # noqa: E501
-        :rtype: str
-        """
-        return self._deployment_mode
-
-    @deployment_mode.setter
-    def deployment_mode(self, deployment_mode):
-        """Sets the deployment_mode of this PipelineVersionObjectList.
-
-
-        :param deployment_mode: The deployment_mode of this PipelineVersionObjectList.  # noqa: E501
-        :type: str
-        """
-        if (self.local_vars_configuration.client_side_validation and
-                deployment_mode is not None and not isinstance(deployment_mode, str)):
-            raise ValueError("Parameter `deployment_mode` must be a string")  # noqa: E501
-
-        self._deployment_mode = deployment_mode
-
-    @property
     def input_fields(self):
         """Gets the input_fields of this PipelineVersionObjectList.  # noqa: E501
 
 
         :return: The input_fields of this PipelineVersionObjectList.  # noqa: E501
         :rtype: list[DeploymentInputFieldCreate]
         """
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_version_object_update.py` & `ubiops-3.9.0/ubiops/models/pipeline_version_object_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'name': 'name',
         'version': 'version'
     }
 
-    def __init__(self, name=None, version=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, version=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineVersionObjectUpdate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._version = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_version_update.py` & `ubiops-3.9.0/ubiops/models/pipeline_version_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         'request_retention_time': 'request_retention_time',
         'request_retention_mode': 'request_retention_mode',
         'default_notification_group': 'default_notification_group',
         'objects': 'objects',
         'attachments': 'attachments'
     }
 
-    def __init__(self, version=None, description=None, labels=None, monitoring=None, request_retention_time=None, request_retention_mode=None, default_notification_group=None, objects=None, attachments=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, version=None, description=None, labels=None, monitoring=None, request_retention_time=None, request_retention_mode=None, default_notification_group=None, objects=None, attachments=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineVersionUpdate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._version = None
         self._description = None
```

### Comparing `ubiops-3.8.0/ubiops/models/pipeline_widget_list.py` & `ubiops-3.9.0/ubiops/models/pipeline_widget_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'type': 'type',
         'configuration': 'configuration'
     }
 
-    def __init__(self, type=None, configuration=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, type=None, configuration=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """PipelineWidgetList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._type = None
         self._configuration = None
```

### Comparing `ubiops-3.8.0/ubiops/models/project_create.py` & `ubiops-3.9.0/ubiops/models/project_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     attribute_map = {
         'name': 'name',
         'organization_name': 'organization_name',
         'advanced_permissions': 'advanced_permissions',
         'credits': 'credits'
     }
 
-    def __init__(self, name=None, organization_name=None, advanced_permissions=False, credits=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, organization_name=None, advanced_permissions=False, credits=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ProjectCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._organization_name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/project_detail.py` & `ubiops-3.9.0/ubiops/models/project_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         'organization_name': 'organization_name',
         'advanced_permissions': 'advanced_permissions',
         'credits': 'credits',
         'suspended': 'suspended',
         'suspended_reason': 'suspended_reason'
     }
 
-    def __init__(self, id=None, name=None, creation_date=None, organization_name=None, advanced_permissions=None, credits=None, suspended=None, suspended_reason=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, creation_date=None, organization_name=None, advanced_permissions=None, credits=None, suspended=None, suspended_reason=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ProjectDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/project_list.py` & `ubiops-3.9.0/ubiops/models/project_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         'name': 'name',
         'creation_date': 'creation_date',
         'advanced_permissions': 'advanced_permissions',
         'credits': 'credits',
         'organization_name': 'organization_name'
     }
 
-    def __init__(self, id=None, name=None, creation_date=None, advanced_permissions=None, credits=None, organization_name=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, creation_date=None, advanced_permissions=None, credits=None, organization_name=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ProjectList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/project_resource_usage.py` & `ubiops-3.9.0/ubiops/models/project_resource_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         'deployments': 'deployments',
         'deployment_versions': 'deployment_versions',
         'pipelines': 'pipelines',
         'pipeline_versions': 'pipeline_versions',
         'gpus': 'gpus'
     }
 
-    def __init__(self, deployments=None, deployment_versions=None, pipelines=None, pipeline_versions=None, gpus=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, deployments=None, deployment_versions=None, pipelines=None, pipeline_versions=None, gpus=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ProjectResourceUsage - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._deployments = None
         self._deployment_versions = None
```

### Comparing `ubiops-3.8.0/ubiops/models/project_update.py` & `ubiops-3.9.0/ubiops/models/project_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     attribute_map = {
         'name': 'name',
         'advanced_permissions': 'advanced_permissions',
         'credits': 'credits',
         'suspend': 'suspend'
     }
 
-    def __init__(self, name=None, advanced_permissions=None, credits=None, suspend=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, advanced_permissions=None, credits=None, suspend=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ProjectUpdate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._advanced_permissions = None
```

### Comparing `ubiops-3.8.0/ubiops/models/project_user_create.py` & `ubiops-3.9.0/ubiops/models/project_user_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         'user_id': 'str'
     }
 
     attribute_map = {
         'user_id': 'user_id'
     }
 
-    def __init__(self, user_id=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, user_id=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ProjectUserCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._user_id = None
         self.discriminator = None
```

### Comparing `ubiops-3.8.0/ubiops/models/project_user_list.py` & `ubiops-3.9.0/ubiops/models/project_user_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,32 +42,30 @@
     attribute_map = {
         'id': 'id',
         'email': 'email',
         'name': 'name',
         'surname': 'surname'
     }
 
-    def __init__(self, id=None, email=None, name=None, surname=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, email=None, name=None, surname=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ProjectUserList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._email = None
         self._name = None
         self._surname = None
         self.discriminator = None
 
         self.id = id
         self.email = email
-        if name is not None:
-            self.name = name
-        if surname is not None:
-            self.surname = surname
+        self.name = name
+        self.surname = surname
 
     @property
     def id(self):
         """Gets the id of this ProjectUserList.  # noqa: E501
 
 
         :return: The id of this ProjectUserList.  # noqa: E501
@@ -139,18 +137,14 @@
         :param name: The name of this ProjectUserList.  # noqa: E501
         :type: str
         """
         if (self.local_vars_configuration.client_side_validation and
                 name is not None and not isinstance(name, str)):
             raise ValueError("Parameter `name` must be a string")  # noqa: E501
 
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) < 1):
-            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
-
         self._name = name
 
     @property
     def surname(self):
         """Gets the surname of this ProjectUserList.  # noqa: E501
 
 
@@ -167,18 +161,14 @@
         :param surname: The surname of this ProjectUserList.  # noqa: E501
         :type: str
         """
         if (self.local_vars_configuration.client_side_validation and
                 surname is not None and not isinstance(surname, str)):
             raise ValueError("Parameter `surname` must be a string")  # noqa: E501
 
-        if (self.local_vars_configuration.client_side_validation and
-                surname is not None and len(surname) < 1):
-            raise ValueError("Invalid value for `surname`, length must be greater than or equal to `1`")  # noqa: E501
-
         self._surname = surname
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
```

### Comparing `ubiops-3.8.0/ubiops/models/resource_usage.py` & `ubiops-3.9.0/ubiops/models/resource_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         'deployments': 'deployments',
         'deployment_versions': 'deployment_versions',
         'pipelines': 'pipelines',
         'pipeline_versions': 'pipeline_versions',
         'gpus': 'gpus'
     }
 
-    def __init__(self, projects=None, users=None, deployments=None, deployment_versions=None, pipelines=None, pipeline_versions=None, gpus=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, projects=None, users=None, deployments=None, deployment_versions=None, pipelines=None, pipeline_versions=None, gpus=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ResourceUsage - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._projects = None
         self._users = None
```

### Comparing `ubiops-3.8.0/ubiops/models/revision_create.py` & `ubiops-3.9.0/ubiops/models/revision_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'success': 'success',
         'revision': 'revision',
         'build': 'build'
     }
 
-    def __init__(self, success=None, revision=None, build=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, success=None, revision=None, build=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """RevisionCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._success = None
         self._revision = None
```

### Comparing `ubiops-3.8.0/ubiops/models/revision_list.py` & `ubiops-3.9.0/ubiops/models/revision_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     attribute_map = {
         'id': 'id',
         'version': 'version',
         'creation_date': 'creation_date',
         'created_by': 'created_by'
     }
 
-    def __init__(self, id=None, version=None, creation_date=None, created_by=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, version=None, creation_date=None, created_by=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """RevisionList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._version = None
```

### Comparing `ubiops-3.8.0/ubiops/models/role_assignment_create.py` & `ubiops-3.9.0/ubiops/models/role_assignment_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     attribute_map = {
         'user_id': 'user_id',
         'role': 'role',
         'object_name': 'object_name',
         'object_type': 'object_type'
     }
 
-    def __init__(self, user_id=None, role=None, object_name=None, object_type=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, user_id=None, role=None, object_name=None, object_type=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """RoleAssignmentCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._user_id = None
         self._role = None
```

### Comparing `ubiops-3.8.0/ubiops/models/role_assignment_list.py` & `ubiops-3.9.0/ubiops/models/role_assignment_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         'id': 'id',
         'user_id': 'user_id',
         'role': 'role',
         'object_name': 'object_name',
         'object_type': 'object_type'
     }
 
-    def __init__(self, id=None, user_id=None, role=None, object_name=None, object_type=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, user_id=None, role=None, object_name=None, object_type=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """RoleAssignmentList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._user_id = None
```

### Comparing `ubiops-3.8.0/ubiops/models/role_create.py` & `ubiops-3.9.0/ubiops/models/role_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'name': 'name',
         'permissions': 'permissions'
     }
 
-    def __init__(self, name=None, permissions=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, permissions=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """RoleCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._permissions = None
```

### Comparing `ubiops-3.8.0/ubiops/models/role_detail_list.py` & `ubiops-3.9.0/ubiops/models/role_detail_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     attribute_map = {
         'id': 'id',
         'name': 'name',
         'default': 'default',
         'permissions': 'permissions'
     }
 
-    def __init__(self, id=None, name=None, default=None, permissions=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, default=None, permissions=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """RoleDetailList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/role_list.py` & `ubiops-3.9.0/ubiops/models/role_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'id': 'id',
         'name': 'name',
         'default': 'default'
     }
 
-    def __init__(self, id=None, name=None, default=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, default=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """RoleList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
```

### Comparing `ubiops-3.8.0/ubiops/models/role_update.py` & `ubiops-3.9.0/ubiops/models/role_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'name': 'name',
         'permissions': 'permissions'
     }
 
-    def __init__(self, name=None, permissions=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, permissions=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """RoleUpdate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._permissions = None
```

### Comparing `ubiops-3.8.0/ubiops/models/schedule_create.py` & `ubiops-3.9.0/ubiops/models/schedule_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         'request_data': 'request_data',
         'timeout': 'timeout',
         'enabled': 'enabled',
         'description': 'description',
         'labels': 'labels'
     }
 
-    def __init__(self, name=None, object_type=None, object_name=None, version=None, schedule=None, request_data=None, timeout=None, enabled=None, description=None, labels=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, object_type=None, object_name=None, version=None, schedule=None, request_data=None, timeout=None, enabled=None, description=None, labels=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ScheduleCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._object_type = None
```

### Comparing `ubiops-3.8.0/ubiops/models/schedule_list.py` & `ubiops-3.9.0/ubiops/models/schedule_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         'id': 'str',
         'name': 'str',
         'object_type': 'str',
         'object_name': 'str',
         'version': 'str',
         'schedule': 'str',
         'request_data': 'object',
-        'batch': 'bool',
         'timeout': 'int',
         'enabled': 'bool',
         'creation_date': 'datetime',
         'description': 'str',
         'labels': 'dict(str, str)'
     }
 
@@ -52,36 +51,34 @@
         'id': 'id',
         'name': 'name',
         'object_type': 'object_type',
         'object_name': 'object_name',
         'version': 'version',
         'schedule': 'schedule',
         'request_data': 'request_data',
-        'batch': 'batch',
         'timeout': 'timeout',
         'enabled': 'enabled',
         'creation_date': 'creation_date',
         'description': 'description',
         'labels': 'labels'
     }
 
-    def __init__(self, id=None, name=None, object_type=None, object_name=None, version=None, schedule=None, request_data=None, batch=None, timeout=None, enabled=None, creation_date=None, description=None, labels=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, name=None, object_type=None, object_name=None, version=None, schedule=None, request_data=None, timeout=None, enabled=None, creation_date=None, description=None, labels=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ScheduleList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
         self._object_type = None
         self._object_name = None
         self._version = None
         self._schedule = None
         self._request_data = None
-        self._batch = None
         self._timeout = None
         self._enabled = None
         self._creation_date = None
         self._description = None
         self._labels = None
         self.discriminator = None
 
@@ -93,16 +90,14 @@
         if object_name is not None:
             self.object_name = object_name
         if version is not None:
             self.version = version
         if schedule is not None:
             self.schedule = schedule
         self.request_data = request_data
-        if batch is not None:
-            self.batch = batch
         if timeout is not None:
             self.timeout = timeout
         self.enabled = enabled
         if creation_date is not None:
             self.creation_date = creation_date
         if description is not None:
             self.description = description
@@ -276,38 +271,14 @@
         :param request_data: The request_data of this ScheduleList.  # noqa: E501
         :type: object
         """
 
         self._request_data = request_data
 
     @property
-    def batch(self):
-        """Gets the batch of this ScheduleList.  # noqa: E501
-
-
-        :return: The batch of this ScheduleList.  # noqa: E501
-        :rtype: bool
-        """
-        return self._batch
-
-    @batch.setter
-    def batch(self, batch):
-        """Sets the batch of this ScheduleList.
-
-
-        :param batch: The batch of this ScheduleList.  # noqa: E501
-        :type: bool
-        """
-        if (self.local_vars_configuration.client_side_validation and
-                batch is not None and not isinstance(batch, bool)):
-            raise ValueError("Parameter `batch` must be a boolean")  # noqa: E501
-
-        self._batch = batch
-
-    @property
     def timeout(self):
         """Gets the timeout of this ScheduleList.  # noqa: E501
 
 
         :return: The timeout of this ScheduleList.  # noqa: E501
         :rtype: int
         """
```

### Comparing `ubiops-3.8.0/ubiops/models/schedule_update.py` & `ubiops-3.9.0/ubiops/models/schedule_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         'request_data': 'request_data',
         'timeout': 'timeout',
         'enabled': 'enabled',
         'description': 'description',
         'labels': 'labels'
     }
 
-    def __init__(self, name=None, schedule=None, request_data=None, timeout=None, enabled=None, description=None, labels=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, schedule=None, request_data=None, timeout=None, enabled=None, description=None, labels=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ScheduleUpdate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._schedule = None
```

### Comparing `ubiops-3.8.0/ubiops/models/service_user_create.py` & `ubiops-3.9.0/ubiops/models/service_user_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'name': 'name',
         'allowed_cors_origins': 'allowed_cors_origins',
         'expiry_date': 'expiry_date'
     }
 
-    def __init__(self, name=None, allowed_cors_origins=None, expiry_date=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, allowed_cors_origins=None, expiry_date=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ServiceUserCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._allowed_cors_origins = None
```

### Comparing `ubiops-3.8.0/ubiops/models/service_user_list.py` & `ubiops-3.9.0/ubiops/models/service_user_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         'email': 'email',
         'name': 'name',
         'creation_date': 'creation_date',
         'allowed_cors_origins': 'allowed_cors_origins',
         'expiry_date': 'expiry_date'
     }
 
-    def __init__(self, id=None, email=None, name=None, creation_date=None, allowed_cors_origins=None, expiry_date=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, email=None, name=None, creation_date=None, allowed_cors_origins=None, expiry_date=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ServiceUserList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._email = None
```

### Comparing `ubiops-3.8.0/ubiops/models/service_user_token_detail.py` & `ubiops-3.9.0/ubiops/models/service_user_token_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         'token': 'token',
         'name': 'name',
         'creation_date': 'creation_date',
         'allowed_cors_origins': 'allowed_cors_origins',
         'expiry_date': 'expiry_date'
     }
 
-    def __init__(self, id=None, email=None, token=None, name=None, creation_date=None, allowed_cors_origins=None, expiry_date=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, email=None, token=None, name=None, creation_date=None, allowed_cors_origins=None, expiry_date=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ServiceUserTokenDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._email = None
```

### Comparing `ubiops-3.8.0/ubiops/models/service_user_token_list.py` & `ubiops-3.9.0/ubiops/models/service_user_token_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         'token': 'str'
     }
 
     attribute_map = {
         'token': 'token'
     }
 
-    def __init__(self, token=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, token=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """ServiceUserTokenList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._token = None
         self.discriminator = None
```

### Comparing `ubiops-3.8.0/ubiops/models/status.py` & `ubiops-3.9.0/ubiops/models/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         'status': 'str'
     }
 
     attribute_map = {
         'status': 'status'
     }
 
-    def __init__(self, status=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, status=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """Status - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._status = None
         self.discriminator = None
```

### Comparing `ubiops-3.8.0/ubiops/models/usage.py` & `ubiops-3.9.0/ubiops/models/usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'object_type': 'object_type',
         'metric': 'metric',
         'usage': 'usage'
     }
 
-    def __init__(self, object_type=None, metric=None, usage=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, object_type=None, metric=None, usage=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """Usage - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._object_type = None
         self._metric = None
```

### Comparing `ubiops-3.8.0/ubiops/models/usage_metric.py` & `ubiops-3.9.0/ubiops/models/usage_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     attribute_map = {
         'start_date': 'start_date',
         'end_date': 'end_date',
         'value': 'value'
     }
 
-    def __init__(self, start_date=None, end_date=None, value=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, start_date=None, end_date=None, value=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """UsageMetric - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._start_date = None
         self._end_date = None
```

### Comparing `ubiops-3.8.0/ubiops/models/user_pending_create.py` & `ubiops-3.9.0/ubiops/models/user_pending_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         'password': 'password',
         'name': 'name',
         'surname': 'surname',
         'terms_conditions': 'terms_conditions',
         'newsletter': 'newsletter'
     }
 
-    def __init__(self, email=None, password=None, name=None, surname=None, terms_conditions=None, newsletter=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, email=None, password=None, name=None, surname=None, terms_conditions=None, newsletter=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """UserPendingCreate - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._email = None
         self._password = None
```

### Comparing `ubiops-3.8.0/ubiops/models/user_pending_detail.py` & `ubiops-3.9.0/ubiops/models/user_pending_detail.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,30 +40,28 @@
 
     attribute_map = {
         'email': 'email',
         'name': 'name',
         'surname': 'surname'
     }
 
-    def __init__(self, email=None, name=None, surname=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, email=None, name=None, surname=None, local_vars_configuration=None, **kwargs):  # noqa: E501
         """UserPendingDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._email = None
         self._name = None
         self._surname = None
         self.discriminator = None
 
         self.email = email
-        if name is not None:
-            self.name = name
-        if surname is not None:
-            self.surname = surname
+        self.name = name
+        self.surname = surname
 
     @property
     def email(self):
         """Gets the email of this UserPendingDetail.  # noqa: E501
 
 
         :return: The email of this UserPendingDetail.  # noqa: E501
@@ -112,18 +110,14 @@
         :param name: The name of this UserPendingDetail.  # noqa: E501
         :type: str
         """
         if (self.local_vars_configuration.client_side_validation and
                 name is not None and not isinstance(name, str)):
             raise ValueError("Parameter `name` must be a string")  # noqa: E501
 
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) < 1):
-            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
-
         self._name = name
 
     @property
     def surname(self):
         """Gets the surname of this UserPendingDetail.  # noqa: E501
 
 
@@ -140,18 +134,14 @@
         :param surname: The surname of this UserPendingDetail.  # noqa: E501
         :type: str
         """
         if (self.local_vars_configuration.client_side_validation and
                 surname is not None and not isinstance(surname, str)):
             raise ValueError("Parameter `surname` must be a string")  # noqa: E501
 
-        if (self.local_vars_configuration.client_side_validation and
-                surname is not None and len(surname) < 1):
-            raise ValueError("Invalid value for `surname`, length must be greater than or equal to `1`")  # noqa: E501
-
         self._surname = surname
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
```

### Comparing `ubiops-3.8.0/ubiops/rest.py` & `ubiops-3.9.0/ubiops/rest.py`

 * *Files identical despite different names*

### Comparing `ubiops-3.8.0/ubiops.egg-info/PKG-INFO` & `ubiops-3.9.0/ubiops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiops
-Version: 3.8.0
+Version: 3.9.0
 Summary: UbiOps
 Home-page: https://github.com/UbiOps/client-library-python.git
 Author: UbiOps
 License: Apache 2.0
 Description: # ubiops
         Client Library to interact with the [UbiOps](https://ubiops.com) API (v2.1).
```

### Comparing `ubiops-3.8.0/ubiops.egg-info/SOURCES.txt` & `ubiops-3.9.0/ubiops.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 ubiops/models/project_create.py
 ubiops/models/project_detail.py
 ubiops/models/project_list.py
 ubiops/models/project_resource_usage.py
 ubiops/models/project_update.py
 ubiops/models/project_user_create.py
 ubiops/models/project_user_list.py
+ubiops/models/requests_overview.py
 ubiops/models/resource_usage.py
 ubiops/models/revision_create.py
 ubiops/models/revision_list.py
 ubiops/models/role_assignment_create.py
 ubiops/models/role_assignment_list.py
 ubiops/models/role_create.py
 ubiops/models/role_detail_list.py
```

