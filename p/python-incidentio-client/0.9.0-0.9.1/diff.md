# Comparing `tmp/python-incidentio-client-0.9.0.tar.gz` & `tmp/python-incidentio-client-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-incidentio-client-0.9.0.tar", max compression
+gzip compressed data, was "python-incidentio-client-0.9.1.tar", max compression
```

## Comparing `python-incidentio-client-0.9.0.tar` & `python-incidentio-client-0.9.1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0     1072 2022-06-06 09:21:47.923514 python-incidentio-client-0.9.0/LICENSE
--rw-r--r--   0        0        0     3359 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/README.md
--rw-r--r--   0        0        0       99 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/__init__.py
--rw-r--r--   0        0        0       47 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/__init__.py
--rw-r--r--   0        0        0        0 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/actions/__init__.py
--rw-r--r--   0        0        0     4777 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/actions/actions_list.py
--rw-r--r--   0        0        0     2707 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/actions/actions_show.py
--rw-r--r--   0        0        0        0 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/custom_field_options/__init__.py
--rw-r--r--   0        0        0     4414 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/custom_field_options/custom_field_options_create.py
--rw-r--r--   0        0        0     1613 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/custom_field_options/custom_field_options_delete.py
--rw-r--r--   0        0        0     4523 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/custom_field_options/custom_field_options_list.py
--rw-r--r--   0        0        0     2938 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/custom_field_options/custom_field_options_show.py
--rw-r--r--   0        0        0     3986 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/custom_field_options/custom_field_options_update.py
--rw-r--r--   0        0        0        0 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/custom_fields/__init__.py
--rw-r--r--   0        0        0     4239 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/custom_fields/custom_fields_create.py
--rw-r--r--   0        0        0     1578 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/custom_fields/custom_fields_delete.py
--rw-r--r--   0        0        0     2609 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/custom_fields/custom_fields_list.py
--rw-r--r--   0        0        0     2791 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/custom_fields/custom_fields_show.py
--rw-r--r--   0        0        0     4363 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/custom_fields/custom_fields_update.py
--rw-r--r--   0        0        0        0 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/incident_roles/__init__.py
--rw-r--r--   0        0        0     4457 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/incident_roles/incident_roles_create.py
--rw-r--r--   0        0        0     1587 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/incident_roles/incident_roles_delete.py
--rw-r--r--   0        0        0     2631 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/incident_roles/incident_roles_list.py
--rw-r--r--   0        0        0     2813 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/incident_roles/incident_roles_show.py
--rw-r--r--   0        0        0     4685 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/incident_roles/incident_roles_update.py
--rw-r--r--   0        0        0        0 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/incidents/__init__.py
--rw-r--r--   0        0        0    14409 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/incidents/incidents_create.py
--rw-r--r--   0        0        0     4633 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/incidents/incidents_list.py
--rw-r--r--   0        0        0     2715 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/incidents/incidents_show.py
--rw-r--r--   0        0        0        0 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/severities/__init__.py
--rw-r--r--   0        0        0     3694 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/severities/severities_create.py
--rw-r--r--   0        0        0     1561 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/severities/severities_delete.py
--rw-r--r--   0        0        0     2591 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/severities/severities_list.py
--rw-r--r--   0        0        0     2769 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/severities/severities_show.py
--rw-r--r--   0        0        0     3922 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/severities/severities_update.py
--rw-r--r--   0        0        0        0 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/utilities/__init__.py
--rw-r--r--   0        0        0     2660 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/utilities/utilities_identity.py
--rw-r--r--   0        0        0     2547 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/api/utilities/utilities_open_api.py
--rw-r--r--   0        0        0     1660 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/client.py
--rw-r--r--   0        0        0     5299 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/__init__.py
--rw-r--r--   0        0        0     5918 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/action_response_body.py
--rw-r--r--   0        0        0      241 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/action_response_body_status.py
--rw-r--r--   0        0        0     5095 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/actions_list_response_body.py
--rw-r--r--   0        0        0     2666 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/actions_show_response_body.py
--rw-r--r--   0        0        0     2959 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/actor_response_body.py
--rw-r--r--   0        0        0     1751 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/api_key_response_body.py
--rw-r--r--   0        0        0     3891 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_field_entry_payload_request_body.py
--rw-r--r--   0        0        0     5005 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_field_entry_response_body.py
--rw-r--r--   0        0        0     2500 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_field_option_response_body.py
--rw-r--r--   0        0        0     2410 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_field_options_create_request_body.py
--rw-r--r--   0        0        0     2156 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_field_options_create_response_body.py
--rw-r--r--   0        0        0     3187 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_field_options_list_response_body.py
--rw-r--r--   0        0        0     2146 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_field_options_show_response_body.py
--rw-r--r--   0        0        0     1896 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_field_options_update_request_body.py
--rw-r--r--   0        0        0     2156 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_field_options_update_response_body.py
--rw-r--r--   0        0        0     6408 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_field_response_body.py
--rw-r--r--   0        0        0      267 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_field_response_body_field_type.py
--rw-r--r--   0        0        0      216 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_field_response_body_required.py
--rw-r--r--   0        0        0     4286 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_field_type_info_response_body.py
--rw-r--r--   0        0        0      275 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_field_type_info_response_body_field_type.py
--rw-r--r--   0        0        0     3319 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_field_value_payload_request_body.py
--rw-r--r--   0        0        0     3619 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_field_value_response_body.py
--rw-r--r--   0        0        0     4033 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_fields_create_request_body.py
--rw-r--r--   0        0        0      273 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_fields_create_request_body_field_type.py
--rw-r--r--   0        0        0      222 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_fields_create_request_body_required.py
--rw-r--r--   0        0        0     3303 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_fields_create_response_body.py
--rw-r--r--   0        0        0     6023 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_fields_list_response_body.py
--rw-r--r--   0        0        0     3293 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_fields_show_response_body.py
--rw-r--r--   0        0        0     3524 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_fields_update_request_body.py
--rw-r--r--   0        0        0      222 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_fields_update_request_body_required.py
--rw-r--r--   0        0        0     3303 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/custom_fields_update_response_body.py
--rw-r--r--   0        0        0     2653 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/external_issue_reference_response_body.py
--rw-r--r--   0        0        0      269 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/external_issue_reference_response_body_provider.py
--rw-r--r--   0        0        0    23983 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incident_response_body.py
--rw-r--r--   0        0        0      191 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incident_response_body_mode.py
--rw-r--r--   0        0        0      289 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incident_response_body_status.py
--rw-r--r--   0        0        0      181 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incident_response_body_visibility.py
--rw-r--r--   0        0        0     2513 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incident_role_assignment_payload_request_body.py
--rw-r--r--   0        0        0     3478 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incident_role_assignment_response_body.py
--rw-r--r--   0        0        0     4389 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incident_role_response_body.py
--rw-r--r--   0        0        0      203 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incident_role_response_body_role_type.py
--rw-r--r--   0        0        0     2936 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incident_roles_create_request_body.py
--rw-r--r--   0        0        0     2582 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incident_roles_create_response_body.py
--rw-r--r--   0        0        0     5035 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incident_roles_list_response_body.py
--rw-r--r--   0        0        0     2572 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incident_roles_show_response_body.py
--rw-r--r--   0        0        0     2936 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incident_roles_update_request_body.py
--rw-r--r--   0        0        0     2582 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incident_roles_update_response_body.py
--rw-r--r--   0        0        0     2506 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incident_timestamp_response_body.py
--rw-r--r--   0        0        0    11032 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incidents_create_request_body.py
--rw-r--r--   0        0        0      187 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incidents_create_request_body_visibility.py
--rw-r--r--   0        0        0    14887 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incidents_create_response_body.py
--rw-r--r--   0        0        0    40583 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incidents_list_response_body.py
--rw-r--r--   0        0        0    14877 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/incidents_show_response_body.py
--rw-r--r--   0        0        0     2355 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/pagination_meta_response_body.py
--rw-r--r--   0        0        0     2155 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/public_identity_response_body.py
--rw-r--r--   0        0        0     2230 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/severities_create_request_body.py
--rw-r--r--   0        0        0     2150 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/severities_create_response_body.py
--rw-r--r--   0        0        0     3207 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/severities_list_response_body.py
--rw-r--r--   0        0        0     2140 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/severities_show_response_body.py
--rw-r--r--   0        0        0     2230 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/severities_update_request_body.py
--rw-r--r--   0        0        0     2150 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/severities_update_response_body.py
--rw-r--r--   0        0        0     3096 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/severity_response_body.py
--rw-r--r--   0        0        0     2544 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/user_reference_payload_request_body.py
--rw-r--r--   0        0        0     2399 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/user_response_body.py
--rw-r--r--   0        0        0      231 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/user_response_body_role.py
--rw-r--r--   0        0        0     2023 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/utilities_identity_response_body.py
--rw-r--r--   0        0        0     1237 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/models/utilities_open_api_response_200.py
--rw-r--r--   0        0        0        0 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/py.typed
--rw-r--r--   0        0        0     1021 2022-06-06 09:21:47.927513 python-incidentio-client-0.9.0/incident_io_client/types.py
--rw-r--r--   0        0        0     1409 2022-06-06 09:21:47.931513 python-incidentio-client-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4530 2022-06-06 09:21:57.256368 python-incidentio-client-0.9.0/setup.py
--rw-r--r--   0        0        0     4162 2022-06-06 09:21:57.256765 python-incidentio-client-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-06-13 07:20:08.850044 python-incidentio-client-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3359 2022-06-13 07:20:08.850044 python-incidentio-client-0.9.1/README.md
+-rw-r--r--   0        0        0       99 2022-06-13 07:20:08.850044 python-incidentio-client-0.9.1/incident_io_client/__init__.py
+-rw-r--r--   0        0        0       47 2022-06-13 07:20:08.850044 python-incidentio-client-0.9.1/incident_io_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2022-06-13 07:20:08.850044 python-incidentio-client-0.9.1/incident_io_client/api/actions/__init__.py
+-rw-r--r--   0        0        0     4777 2022-06-13 07:20:08.850044 python-incidentio-client-0.9.1/incident_io_client/api/actions/actions_list.py
+-rw-r--r--   0        0        0     2707 2022-06-13 07:20:08.850044 python-incidentio-client-0.9.1/incident_io_client/api/actions/actions_show.py
+-rw-r--r--   0        0        0        0 2022-06-13 07:20:08.850044 python-incidentio-client-0.9.1/incident_io_client/api/custom_field_options/__init__.py
+-rw-r--r--   0        0        0     4414 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/custom_field_options/custom_field_options_create.py
+-rw-r--r--   0        0        0     1613 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/custom_field_options/custom_field_options_delete.py
+-rw-r--r--   0        0        0     4523 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/custom_field_options/custom_field_options_list.py
+-rw-r--r--   0        0        0     2938 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/custom_field_options/custom_field_options_show.py
+-rw-r--r--   0        0        0     3986 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/custom_field_options/custom_field_options_update.py
+-rw-r--r--   0        0        0        0 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/custom_fields/__init__.py
+-rw-r--r--   0        0        0     4239 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/custom_fields/custom_fields_create.py
+-rw-r--r--   0        0        0     1578 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/custom_fields/custom_fields_delete.py
+-rw-r--r--   0        0        0     2609 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/custom_fields/custom_fields_list.py
+-rw-r--r--   0        0        0     2791 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/custom_fields/custom_fields_show.py
+-rw-r--r--   0        0        0     4363 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/custom_fields/custom_fields_update.py
+-rw-r--r--   0        0        0        0 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/incident_roles/__init__.py
+-rw-r--r--   0        0        0     4457 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/incident_roles/incident_roles_create.py
+-rw-r--r--   0        0        0     1587 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/incident_roles/incident_roles_delete.py
+-rw-r--r--   0        0        0     2631 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/incident_roles/incident_roles_list.py
+-rw-r--r--   0        0        0     2813 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/incident_roles/incident_roles_show.py
+-rw-r--r--   0        0        0     4685 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/incident_roles/incident_roles_update.py
+-rw-r--r--   0        0        0        0 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/incidents/__init__.py
+-rw-r--r--   0        0        0    14409 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/incidents/incidents_create.py
+-rw-r--r--   0        0        0     4633 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/incidents/incidents_list.py
+-rw-r--r--   0        0        0     2715 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/incidents/incidents_show.py
+-rw-r--r--   0        0        0        0 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/severities/__init__.py
+-rw-r--r--   0        0        0     3694 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/severities/severities_create.py
+-rw-r--r--   0        0        0     1561 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/severities/severities_delete.py
+-rw-r--r--   0        0        0     2591 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/severities/severities_list.py
+-rw-r--r--   0        0        0     2769 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/severities/severities_show.py
+-rw-r--r--   0        0        0     3922 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/severities/severities_update.py
+-rw-r--r--   0        0        0        0 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/utilities/__init__.py
+-rw-r--r--   0        0        0     2660 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/utilities/utilities_identity.py
+-rw-r--r--   0        0        0     2547 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/api/utilities/utilities_open_api.py
+-rw-r--r--   0        0        0     1660 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/client.py
+-rw-r--r--   0        0        0     5299 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/__init__.py
+-rw-r--r--   0        0        0     5918 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/action_response_body.py
+-rw-r--r--   0        0        0      241 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/action_response_body_status.py
+-rw-r--r--   0        0        0     5095 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/actions_list_response_body.py
+-rw-r--r--   0        0        0     2666 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/actions_show_response_body.py
+-rw-r--r--   0        0        0     2959 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/actor_response_body.py
+-rw-r--r--   0        0        0     1751 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/api_key_response_body.py
+-rw-r--r--   0        0        0     3891 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_field_entry_payload_request_body.py
+-rw-r--r--   0        0        0     5005 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_field_entry_response_body.py
+-rw-r--r--   0        0        0     2500 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_field_option_response_body.py
+-rw-r--r--   0        0        0     2410 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_field_options_create_request_body.py
+-rw-r--r--   0        0        0     2156 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_field_options_create_response_body.py
+-rw-r--r--   0        0        0     3187 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_field_options_list_response_body.py
+-rw-r--r--   0        0        0     2146 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_field_options_show_response_body.py
+-rw-r--r--   0        0        0     1896 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_field_options_update_request_body.py
+-rw-r--r--   0        0        0     2156 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_field_options_update_response_body.py
+-rw-r--r--   0        0        0     6408 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_field_response_body.py
+-rw-r--r--   0        0        0      267 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_field_response_body_field_type.py
+-rw-r--r--   0        0        0      216 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_field_response_body_required.py
+-rw-r--r--   0        0        0     4286 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_field_type_info_response_body.py
+-rw-r--r--   0        0        0      275 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_field_type_info_response_body_field_type.py
+-rw-r--r--   0        0        0     3319 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_field_value_payload_request_body.py
+-rw-r--r--   0        0        0     3619 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_field_value_response_body.py
+-rw-r--r--   0        0        0     4033 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_fields_create_request_body.py
+-rw-r--r--   0        0        0      273 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_fields_create_request_body_field_type.py
+-rw-r--r--   0        0        0      222 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_fields_create_request_body_required.py
+-rw-r--r--   0        0        0     3303 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_fields_create_response_body.py
+-rw-r--r--   0        0        0     6023 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_fields_list_response_body.py
+-rw-r--r--   0        0        0     3293 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_fields_show_response_body.py
+-rw-r--r--   0        0        0     3524 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_fields_update_request_body.py
+-rw-r--r--   0        0        0      222 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_fields_update_request_body_required.py
+-rw-r--r--   0        0        0     3303 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/custom_fields_update_response_body.py
+-rw-r--r--   0        0        0     2653 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/external_issue_reference_response_body.py
+-rw-r--r--   0        0        0      269 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/external_issue_reference_response_body_provider.py
+-rw-r--r--   0        0        0    24249 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incident_response_body.py
+-rw-r--r--   0        0        0      191 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incident_response_body_mode.py
+-rw-r--r--   0        0        0      289 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incident_response_body_status.py
+-rw-r--r--   0        0        0      181 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incident_response_body_visibility.py
+-rw-r--r--   0        0        0     2513 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incident_role_assignment_payload_request_body.py
+-rw-r--r--   0        0        0     3478 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incident_role_assignment_response_body.py
+-rw-r--r--   0        0        0     4389 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incident_role_response_body.py
+-rw-r--r--   0        0        0      203 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incident_role_response_body_role_type.py
+-rw-r--r--   0        0        0     2936 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incident_roles_create_request_body.py
+-rw-r--r--   0        0        0     2582 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incident_roles_create_response_body.py
+-rw-r--r--   0        0        0     5035 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incident_roles_list_response_body.py
+-rw-r--r--   0        0        0     2572 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incident_roles_show_response_body.py
+-rw-r--r--   0        0        0     2936 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incident_roles_update_request_body.py
+-rw-r--r--   0        0        0     2582 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incident_roles_update_response_body.py
+-rw-r--r--   0        0        0     2506 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incident_timestamp_response_body.py
+-rw-r--r--   0        0        0    11298 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incidents_create_request_body.py
+-rw-r--r--   0        0        0      187 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incidents_create_request_body_visibility.py
+-rw-r--r--   0        0        0    14887 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incidents_create_response_body.py
+-rw-r--r--   0        0        0    40583 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incidents_list_response_body.py
+-rw-r--r--   0        0        0    14877 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/incidents_show_response_body.py
+-rw-r--r--   0        0        0     2355 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/pagination_meta_response_body.py
+-rw-r--r--   0        0        0     2155 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/public_identity_response_body.py
+-rw-r--r--   0        0        0     2230 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/severities_create_request_body.py
+-rw-r--r--   0        0        0     2150 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/severities_create_response_body.py
+-rw-r--r--   0        0        0     3207 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/severities_list_response_body.py
+-rw-r--r--   0        0        0     2140 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/severities_show_response_body.py
+-rw-r--r--   0        0        0     2230 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/severities_update_request_body.py
+-rw-r--r--   0        0        0     2150 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/severities_update_response_body.py
+-rw-r--r--   0        0        0     3096 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/severity_response_body.py
+-rw-r--r--   0        0        0     2544 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/user_reference_payload_request_body.py
+-rw-r--r--   0        0        0     2399 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/user_response_body.py
+-rw-r--r--   0        0        0      231 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/user_response_body_role.py
+-rw-r--r--   0        0        0     2023 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/utilities_identity_response_body.py
+-rw-r--r--   0        0        0     1237 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/models/utilities_open_api_response_200.py
+-rw-r--r--   0        0        0        0 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/py.typed
+-rw-r--r--   0        0        0     1021 2022-06-13 07:20:08.854044 python-incidentio-client-0.9.1/incident_io_client/types.py
+-rw-r--r--   0        0        0     1409 2022-06-13 07:20:08.858044 python-incidentio-client-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4530 2022-06-13 07:20:20.542065 python-incidentio-client-0.9.1/setup.py
+-rw-r--r--   0        0        0     4162 2022-06-13 07:20:20.542399 python-incidentio-client-0.9.1/PKG-INFO
```

### Comparing `python-incidentio-client-0.9.0/LICENSE` & `python-incidentio-client-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/README.md` & `python-incidentio-client-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/actions/actions_list.py` & `python-incidentio-client-0.9.1/incident_io_client/api/actions/actions_list.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/actions/actions_show.py` & `python-incidentio-client-0.9.1/incident_io_client/api/actions/actions_show.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/custom_field_options/custom_field_options_create.py` & `python-incidentio-client-0.9.1/incident_io_client/api/custom_field_options/custom_field_options_create.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/custom_field_options/custom_field_options_delete.py` & `python-incidentio-client-0.9.1/incident_io_client/api/custom_field_options/custom_field_options_delete.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/custom_field_options/custom_field_options_list.py` & `python-incidentio-client-0.9.1/incident_io_client/api/custom_field_options/custom_field_options_list.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/custom_field_options/custom_field_options_show.py` & `python-incidentio-client-0.9.1/incident_io_client/api/custom_field_options/custom_field_options_show.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/custom_field_options/custom_field_options_update.py` & `python-incidentio-client-0.9.1/incident_io_client/api/custom_field_options/custom_field_options_update.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/custom_fields/custom_fields_create.py` & `python-incidentio-client-0.9.1/incident_io_client/api/custom_fields/custom_fields_create.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/custom_fields/custom_fields_delete.py` & `python-incidentio-client-0.9.1/incident_io_client/api/custom_fields/custom_fields_delete.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/custom_fields/custom_fields_list.py` & `python-incidentio-client-0.9.1/incident_io_client/api/custom_fields/custom_fields_list.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/custom_fields/custom_fields_show.py` & `python-incidentio-client-0.9.1/incident_io_client/api/custom_fields/custom_fields_show.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/custom_fields/custom_fields_update.py` & `python-incidentio-client-0.9.1/incident_io_client/api/custom_fields/custom_fields_update.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/incident_roles/incident_roles_create.py` & `python-incidentio-client-0.9.1/incident_io_client/api/incident_roles/incident_roles_create.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/incident_roles/incident_roles_delete.py` & `python-incidentio-client-0.9.1/incident_io_client/api/incident_roles/incident_roles_delete.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/incident_roles/incident_roles_list.py` & `python-incidentio-client-0.9.1/incident_io_client/api/incident_roles/incident_roles_list.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/incident_roles/incident_roles_show.py` & `python-incidentio-client-0.9.1/incident_io_client/api/incident_roles/incident_roles_show.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/incident_roles/incident_roles_update.py` & `python-incidentio-client-0.9.1/incident_io_client/api/incident_roles/incident_roles_update.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/incidents/incidents_create.py` & `python-incidentio-client-0.9.1/incident_io_client/api/incidents/incidents_create.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/incidents/incidents_list.py` & `python-incidentio-client-0.9.1/incident_io_client/api/incidents/incidents_list.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/incidents/incidents_show.py` & `python-incidentio-client-0.9.1/incident_io_client/api/incidents/incidents_show.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/severities/severities_create.py` & `python-incidentio-client-0.9.1/incident_io_client/api/severities/severities_create.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/severities/severities_delete.py` & `python-incidentio-client-0.9.1/incident_io_client/api/severities/severities_delete.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/severities/severities_list.py` & `python-incidentio-client-0.9.1/incident_io_client/api/severities/severities_list.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/severities/severities_show.py` & `python-incidentio-client-0.9.1/incident_io_client/api/severities/severities_show.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/severities/severities_update.py` & `python-incidentio-client-0.9.1/incident_io_client/api/severities/severities_update.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/utilities/utilities_identity.py` & `python-incidentio-client-0.9.1/incident_io_client/api/utilities/utilities_identity.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/api/utilities/utilities_open_api.py` & `python-incidentio-client-0.9.1/incident_io_client/api/utilities/utilities_open_api.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/client.py` & `python-incidentio-client-0.9.1/incident_io_client/client.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/__init__.py` & `python-incidentio-client-0.9.1/incident_io_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/action_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/action_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/actions_list_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/actions_list_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/actions_show_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/actions_show_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/actor_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/actor_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/api_key_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/api_key_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_field_entry_payload_request_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_field_entry_payload_request_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_field_entry_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_field_entry_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_field_option_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_field_option_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_field_options_create_request_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_field_options_create_request_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_field_options_create_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_field_options_create_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_field_options_list_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_field_options_list_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_field_options_show_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_field_options_show_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_field_options_update_request_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_field_options_update_request_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_field_options_update_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_field_options_update_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_field_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_field_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_field_type_info_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_field_type_info_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_field_value_payload_request_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_field_value_payload_request_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_field_value_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_field_value_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_fields_create_request_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_fields_create_request_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_fields_create_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_fields_create_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_fields_list_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_fields_list_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_fields_show_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_fields_show_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_fields_update_request_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_fields_update_request_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/custom_fields_update_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/custom_fields_update_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/external_issue_reference_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/external_issue_reference_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/incident_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/incident_response_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,18 @@
         reference (str): Reference to this incident, as displayed across the product Example: INC-123.
         severity (SeverityResponseBody):  Example: {'created_at': '2021-08-17T13:28:57.801578Z', 'description': "It's
             not really that bad, everyone chill", 'id': '01FCNDV6P870EA6S7TK1DSYDG0', 'name': 'Minor', 'rank': 1,
             'updated_at': '2021-08-17T13:28:57.801578Z'}.
         slack_channel_id (str): ID of the Slack channel in the organisation Slack workspace Example: C02AW36C1M5.
         status (IncidentResponseBodyStatus): Current status of the incident Example: triage.
         updated_at (datetime.datetime): When the incident was last updated Example: 2021-08-17T13:28:57.801578Z.
-        visibility (IncidentResponseBodyVisibility): Whether the incident is public or private Example: public.
+        visibility (IncidentResponseBodyVisibility): Whether the incident should be open to anyone in your Slack
+            workspace (public), or invite-only (private). For more information on Private Incidents see our [help
+            centre](https://help.incident.io/en/articles/5947963-can-we-mark-incidents-as-sensitive-and-restrict-access).
+            Example: public.
         call_url (Union[Unset, str]): The call URL attached to this incident Example: https://zoom.us/foo.
         permalink (Union[Unset, str]):  Example: Et amet non sed sit quia..
         postmortem_document_url (Union[Unset, str]): Description of the incident Example:
             https://docs.google.com/my_doc_id.
         slack_channel_name (Union[Unset, str]): Name of the slack channel Example: inc-165-green-parrot.
         summary (Union[Unset, str]): Detailed description of the incident Example: Our database is really really sad,
             and we don't know why yet..
```

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/incident_role_assignment_payload_request_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/incident_role_assignment_payload_request_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/incident_role_assignment_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/incident_role_assignment_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/incident_role_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/incident_role_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/incident_roles_create_request_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/incident_roles_create_request_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/incident_roles_create_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/incident_roles_create_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/incident_roles_list_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/incident_roles_list_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/incident_roles_show_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/incident_roles_show_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/incident_roles_update_request_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/incident_roles_update_request_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/incident_roles_update_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/incident_roles_update_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/incident_timestamp_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/incident_timestamp_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/incidents_create_request_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/incidents_create_request_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,18 @@
             aut rerum fugiat exercitationem maiores.'}, 'incident_role_id': '01FH5TZRWMNAFB0DZ23FD1TV96'}],
             'incident_type_id': 'Quidem amet.', 'name': 'Our database is sad', 'severity_id': 'Aut quis.', 'summary': "Our
             database is really really sad, and we don't know why yet.", 'visibility': 'public'}
 
     Attributes:
         idempotency_key (str): Unique string used to de-duplicate incident create requests Example: alert-uuid.
         severity_id (str):  Example: Dolorum officia..
-        visibility (IncidentsCreateRequestBodyVisibility): Whether the incident is public or private Example: public.
+        visibility (IncidentsCreateRequestBodyVisibility): Whether the incident should be open to anyone in your Slack
+            workspace (public), or invite-only (private). For more information on Private Incidents see our [help
+            centre](https://help.incident.io/en/articles/5947963-can-we-mark-incidents-as-sensitive-and-restrict-access).
+            Example: public.
         custom_field_entries (Union[Unset, List[CustomFieldEntryPayloadRequestBody]]): Set the incident's custom fields
             to these values Example: [{'custom_field_id': '01FCNDV6P870EA6S7TK1DSYDG0', 'values': [{'id':
             '01FCNDV6P870EA6S7TK1DSYDG0', 'value_link': 'https://google.com/', 'value_numeric': '123.456',
             'value_option_id': '01FCNDV6P870EA6S7TK1DSYDG0', 'value_text': 'This is my text field, I hope you like it'},
             {'id': '01FCNDV6P870EA6S7TK1DSYDG0', 'value_link': 'https://google.com/', 'value_numeric': '123.456',
             'value_option_id': '01FCNDV6P870EA6S7TK1DSYDG0', 'value_text': 'This is my text field, I hope you like it'}]},
             {'custom_field_id': '01FCNDV6P870EA6S7TK1DSYDG0', 'values': [{'id': '01FCNDV6P870EA6S7TK1DSYDG0', 'value_link':
```

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/incidents_create_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/incidents_create_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/incidents_list_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/incidents_list_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/incidents_show_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/incidents_show_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/pagination_meta_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/pagination_meta_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/public_identity_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/public_identity_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/severities_create_request_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/severities_create_request_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/severities_create_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/severities_create_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/severities_list_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/severities_list_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/severities_show_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/severities_show_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/severities_update_request_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/severities_update_request_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/severities_update_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/severities_update_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/severity_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/severity_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/user_reference_payload_request_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/user_reference_payload_request_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/user_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/user_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/utilities_identity_response_body.py` & `python-incidentio-client-0.9.1/incident_io_client/models/utilities_identity_response_body.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/models/utilities_open_api_response_200.py` & `python-incidentio-client-0.9.1/incident_io_client/models/utilities_open_api_response_200.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/incident_io_client/types.py` & `python-incidentio-client-0.9.1/incident_io_client/types.py`

 * *Files identical despite different names*

### Comparing `python-incidentio-client-0.9.0/pyproject.toml` & `python-incidentio-client-0.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [tool.isort]
 profile = "black"
 float_to_top = true
 skip_glob = ".venv"
 
 [tool.poetry]
 name = "python-incidentio-client"
-version = "0.9.0"
+version = "0.9.1"
 description = "Python client for Incident.io"
 repository = "https://github.com/expobrain/python-incidentio-client"
 authors = ["Daniele Esposti <daniele.esposti@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "incident_io_client" }]
 
@@ -28,15 +28,15 @@
 attrs = ">=20.1.0"
 python-dateutil = ">=2.8.0"
 
 [tool.poetry.dev-dependencies]
 autoflake = "^1.4"
 black = "^21.12b"
 isort = "^5.10.1"
-mypy = "^0.960"
+mypy = "^0.961"
 flake8 = "^4.0.1"
 types-python-dateutil = "^2.8.17"
 pyupgrade = "^2.30.1"
 openapi-python-client = "^0.10.8"
 types-certifi = "^2021.10.8"
 click = "<8"
 toml = "^0.10.2"
```

### Comparing `python-incidentio-client-0.9.0/setup.py` & `python-incidentio-client-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 {'': ['*']}
 
 install_requires = \
 ['attrs>=20.1.0', 'httpx>=0.15.4', 'python-dateutil>=2.8.0']
 
 setup_kwargs = {
     'name': 'python-incidentio-client',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Python client for Incident.io',
     'long_description': '# python-incident-io-client\n\n![main build status](https://github.com/expobrain/python-incidentio-client/actions/workflows/main.yml/badge.svg?branch=main)\n\nA client library for accessing incident.io.\n\n## Installation\n\nTo install the client:\n\n```shell\npip install python-incidentio-client\n```\n\n## Usage\n\nFirst, create a client:\n\n```python\nfrom incident_io_client import Client\n\nclient = Client(base_url="https://api.incident.io")\n```\n\nIf the endpoints you\'re going to hit require authentication, use `AuthenticatedClient` instead:\n\n```python\nfrom incident_io_client import AuthenticatedClient\n\nclient = AuthenticatedClient(base_url="https://api.incident.io", token="SuperSecretToken")\n```\n\nNow call your endpoint and use your models:\n\n```python\nfrom incident_io_client.models import MyDataModel\nfrom incident_io_client.api.my_tag import get_my_data_model\nfrom incident_io_client.types import Response\n\nmy_data: MyDataModel = get_my_data_model.sync(client=client)\n# or if you need more info (e.g. status_code)\nresponse: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)\n```\n\nOr do the same thing with an async version:\n\n```python\nfrom incident_io_client.models import MyDataModel\nfrom incident_io_client.api.my_tag import get_my_data_model\nfrom incident_io_client.types import Response\n\nmy_data: MyDataModel = await get_my_data_model.asyncio(client=client)\nresponse: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)\n```\n\nBy default, when you\'re calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.incident.io",\n    token="SuperSecretToken",\n    verify_ssl="/path/to/certificate_bundle.pem",\n)\n```\n\nYou can also disable certificate validation altogether, but beware that **this is a security risk**.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.incident.io",\n    token="SuperSecretToken",\n    verify_ssl=False\n)\n```\n\nThings to know:\n\n1. Every path/method combo becomes a Python module with four functions:\n\n   1. `sync`: Blocking request that returns parsed data (if successful) or `None`\n   1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.\n   1. `asyncio`: Like `sync` but the async instead of blocking\n   1. `asyncio_detailed`: Like `sync_detailed` by async instead of blocking\n\n1. All path/query params, and bodies become method arguments.\n1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)\n1. Any endpoint which did not have a tag will be in `incident_io_client.api.default`\n\n## Generate code\n\nThis client is automatically generated from the Swagger 2.x specs downloaded from the [openapi-python-client](https://pypi.org/project/openapi-python-client/)\'s [definition endpoint](https://api-docs.incident.io/#operation/Utilities_OpenAPI); a code generator tool will use the OpenAPI document to generates a sync/async client.\n\nTo generare an updated copy of the client:\n\n```shell\npoetry install\nmake download\npoetry run make generate\n```\n',
     'author': 'Daniele Esposti',
     'author_email': 'daniele.esposti@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/expobrain/python-incidentio-client',
```

### Comparing `python-incidentio-client-0.9.0/PKG-INFO` & `python-incidentio-client-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-incidentio-client
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python client for Incident.io
 Home-page: https://github.com/expobrain/python-incidentio-client
 License: MIT
 Author: Daniele Esposti
 Author-email: daniele.esposti@gmail.com
 Requires-Python: >=3.6.2,<4
 Classifier: License :: OSI Approved :: MIT License
```

