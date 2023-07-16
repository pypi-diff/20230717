# Comparing `tmp/fern_merge-0.0.30.tar.gz` & `tmp/fern_merge-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_merge-0.0.30.tar", max compression
+gzip compressed data, was "fern_merge-0.0.32.tar", max compression
```

## Comparing `fern_merge-0.0.30.tar` & `fern_merge-0.0.32.tar`

### file list

```diff
@@ -1,456 +1,456 @@
--rw-r--r--   0        0        0     2139 2023-07-13 08:58:33.636106 fern_merge-0.0.30/README.md
--rw-r--r--   0        0        0      371 2023-07-13 08:58:33.636106 fern_merge-0.0.30/pyproject.toml
--rw-r--r--   0        0        0      187 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/__init__.py
--rw-r--r--   0        0        0     1547 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/client.py
--rw-r--r--   0        0        0      528 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/core/api_error.py
--rw-r--r--   0        0        0     1101 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      201 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/environment.py
--rw-r--r--   0        0        0        0 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/py.typed
--rw-r--r--   0        0        0      116 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/__init__.py
--rw-r--r--   0        0        0     9656 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/__init__.py
--rw-r--r--   0        0        0    10018 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/client.py
--rw-r--r--   0        0        0     1144 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2284 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2334 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/activities/__init__.py
--rw-r--r--   0        0        0    12088 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/activities/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/applications/__init__.py
--rw-r--r--   0        0        0    14755 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/applications/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/attachments/__init__.py
--rw-r--r--   0        0        0    11850 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/attachments/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2304 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/candidates/__init__.py
--rw-r--r--   0        0        0    16778 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/candidates/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2045 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/departments/__init__.py
--rw-r--r--   0        0        0     5972 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/departments/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/eeocs/__init__.py
--rw-r--r--   0        0        0     8117 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/eeocs/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     2362 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2537 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/interviews/__init__.py
--rw-r--r--   0        0        0    12540 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/interviews/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/issues/__init__.py
--rw-r--r--   0        0        0     6768 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/job_interview_stages/__init__.py
--rw-r--r--   0        0        0     6771 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/job_interview_stages/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/jobs/__init__.py
--rw-r--r--   0        0        0     8227 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/jobs/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/link_token/__init__.py
--rw-r--r--   0        0        0     4924 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0     5305 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/offers/__init__.py
--rw-r--r--   0        0        0     8095 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/offers/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/offices/__init__.py
--rw-r--r--   0        0        0     5900 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/offices/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     4900 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2545 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/reject_reasons/__init__.py
--rw-r--r--   0        0        0     6014 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/reject_reasons/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.636106 fern_merge-0.0.30/src/merge/resources/ats/resources/scorecards/__init__.py
--rw-r--r--   0        0        0     8545 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/resources/scorecards/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     6892 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     2644 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/resources/tags/__init__.py
--rw-r--r--   0        0        0     4201 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/resources/tags/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/resources/users/__init__.py
--rw-r--r--   0        0        0     7399 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/resources/users/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     4455 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    13447 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/__init__.py
--rw-r--r--   0        0        0     1240 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/access_role_enum.py
--rw-r--r--   0        0        0     1483 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/account_token.py
--rw-r--r--   0        0        0      857 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/activities_list_request_remote_fields.py
--rw-r--r--   0        0        0      869 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      873 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      885 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     2705 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/activity.py
--rw-r--r--   0        0        0      189 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/activity_activity_type.py
--rw-r--r--   0        0        0     2155 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/activity_request.py
--rw-r--r--   0        0        0      196 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/activity_request_activity_type.py
--rw-r--r--   0        0        0      187 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/activity_request_visibility.py
--rw-r--r--   0        0        0     1109 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/activity_response.py
--rw-r--r--   0        0        0      705 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/activity_type_enum.py
--rw-r--r--   0        0        0      180 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/activity_visibility.py
--rw-r--r--   0        0        0     2473 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/application.py
--rw-r--r--   0        0        0     2269 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/application_request.py
--rw-r--r--   0        0        0     1121 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/application_response.py
--rw-r--r--   0        0        0     8243 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/applications_list_request_expand.py
--rw-r--r--   0        0        0     8371 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/applications_retrieve_request_expand.py
--rw-r--r--   0        0        0     2146 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/attachment.py
--rw-r--r--   0        0        0      199 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/attachment_attachment_type.py
--rw-r--r--   0        0        0     1820 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/attachment_request.py
--rw-r--r--   0        0        0      206 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/attachment_request_attachment_type.py
--rw-r--r--   0        0        0     1117 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/attachment_response.py
--rw-r--r--   0        0        0      985 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/attachment_type_enum.py
--rw-r--r--   0        0        0     1245 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/available_actions.py
--rw-r--r--   0        0        0     3471 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/candidate.py
--rw-r--r--   0        0        0     3061 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/candidate_request.py
--rw-r--r--   0        0        0     1113 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/candidate_response.py
--rw-r--r--   0        0        0      833 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/candidates_list_request_expand.py
--rw-r--r--   0        0        0      849 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/candidates_retrieve_request_expand.py
--rw-r--r--   0        0        0     1391 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     2324 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/condition_type_enum.py
--rw-r--r--   0        0        0      870 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/debug_model_log_summary.py
--rw-r--r--   0        0        0     1698 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/department.py
--rw-r--r--   0        0        0     1337 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/disability_status_enum.py
--rw-r--r--   0        0        0     4088 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/eeoc.py
--rw-r--r--   0        0        0      201 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/eeoc_disability_status.py
--rw-r--r--   0        0        0      160 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/eeoc_gender.py
--rw-r--r--   0        0        0      152 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/eeoc_race.py
--rw-r--r--   0        0        0      189 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/eeoc_veteran_status.py
--rw-r--r--   0        0        0     3803 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py
--rw-r--r--   0        0        0     3851 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py
--rw-r--r--   0        0        0     3867 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     3915 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1529 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/email_address.py
--rw-r--r--   0        0        0      210 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/email_address_email_address_type.py
--rw-r--r--   0        0        0     1553 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/email_address_request.py
--rw-r--r--   0        0        0      217 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/email_address_request_email_address_type.py
--rw-r--r--   0        0        0      742 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/email_address_type_enum.py
--rw-r--r--   0        0        0      522 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/error_validation_problem.py
--rw-r--r--   0        0        0     1160 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/gender_enum.py
--rw-r--r--   0        0        0     4187 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/interviews_list_request_expand.py
--rw-r--r--   0        0        0     4251 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/interviews_retrieve_request_expand.py
--rw-r--r--   0        0        0     1323 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/issues_list_request_status.py
--rw-r--r--   0        0        0     3428 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/job.py
--rw-r--r--   0        0        0     2387 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/job_interview_stage.py
--rw-r--r--   0        0        0      169 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/job_status.py
--rw-r--r--   0        0        0     1045 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/job_status_enum.py
--rw-r--r--   0        0        0     3771 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/jobs_list_request_expand.py
--rw-r--r--   0        0        0      956 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/jobs_list_request_status.py
--rw-r--r--   0        0        0     3835 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/jobs_retrieve_request_expand.py
--rw-r--r--   0        0        0      835 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0     1037 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0     2786 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/offer.py
--rw-r--r--   0        0        0      177 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/offer_status.py
--rw-r--r--   0        0        0     1832 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/offer_status_enum.py
--rw-r--r--   0        0        0      767 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/offers_list_request_expand.py
--rw-r--r--   0        0        0      783 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/offers_retrieve_request_expand.py
--rw-r--r--   0        0        0     1817 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/office.py
--rw-r--r--   0        0        0      993 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/operator_schema.py
--rw-r--r--   0        0        0     1180 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/overall_recommendation_enum.py
--rw-r--r--   0        0        0      959 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      892 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_activity_list.py
--rw-r--r--   0        0        0      904 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_application_list.py
--rw-r--r--   0        0        0      900 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_attachment_list.py
--rw-r--r--   0        0        0      896 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_candidate_list.py
--rw-r--r--   0        0        0      921 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      900 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_department_list.py
--rw-r--r--   0        0        0      876 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_eeoc_list.py
--rw-r--r--   0        0        0      880 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_issue_list.py
--rw-r--r--   0        0        0      930 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_job_interview_stage_list.py
--rw-r--r--   0        0        0      872 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_job_list.py
--rw-r--r--   0        0        0      880 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_offer_list.py
--rw-r--r--   0        0        0      884 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_office_list.py
--rw-r--r--   0        0        0      909 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_reject_reason_list.py
--rw-r--r--   0        0        0      901 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_remote_user_list.py
--rw-r--r--   0        0        0      933 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_scheduled_interview_list.py
--rw-r--r--   0        0        0      896 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_scorecard_list.py
--rw-r--r--   0        0        0      901 2023-07-13 08:58:33.640106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      872 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/paginated_tag_list.py
--rw-r--r--   0        0        0     3068 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/patched_candidate_request.py
--rw-r--r--   0        0        0     1624 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/phone_number.py
--rw-r--r--   0        0        0      205 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/phone_number_phone_number_type.py
--rw-r--r--   0        0        0     1648 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/phone_number_request.py
--rw-r--r--   0        0        0      212 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/phone_number_request_phone_number_type.py
--rw-r--r--   0        0        0     1039 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/phone_number_type_enum.py
--rw-r--r--   0        0        0     2326 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/race_enum.py
--rw-r--r--   0        0        0      814 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/reason_enum.py
--rw-r--r--   0        0        0     1775 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/reject_reason.py
--rw-r--r--   0        0        0      802 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/remote_data.py
--rw-r--r--   0        0        0      986 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/remote_key.py
--rw-r--r--   0        0        0     1330 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/remote_response.py
--rw-r--r--   0        0        0      195 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/remote_response_response_type.py
--rw-r--r--   0        0        0     2562 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/remote_user.py
--rw-r--r--   0        0        0      183 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/remote_user_access_role.py
--rw-r--r--   0        0        0      723 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/request_format_enum.py
--rw-r--r--   0        0        0      562 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/response_type_enum.py
--rw-r--r--   0        0        0     3187 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/scheduled_interview.py
--rw-r--r--   0        0        0     2464 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/scheduled_interview_request.py
--rw-r--r--   0        0        0      237 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/scheduled_interview_request_status.py
--rw-r--r--   0        0        0     1150 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/scheduled_interview_response.py
--rw-r--r--   0        0        0      230 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/scheduled_interview_status.py
--rw-r--r--   0        0        0      893 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/scheduled_interview_status_enum.py
--rw-r--r--   0        0        0     2692 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/scorecard.py
--rw-r--r--   0        0        0      226 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/scorecard_overall_recommendation.py
--rw-r--r--   0        0        0     1731 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/scorecards_list_request_expand.py
--rw-r--r--   0        0        0     1763 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py
--rw-r--r--   0        0        0      695 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1623 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/tag.py
--rw-r--r--   0        0        0     1659 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/url.py
--rw-r--r--   0        0        0     1683 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/url_request.py
--rw-r--r--   0        0        0      171 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/url_request_url_type.py
--rw-r--r--   0        0        0     1451 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/url_type_enum.py
--rw-r--r--   0        0        0      164 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/url_url_type.py
--rw-r--r--   0        0        0      762 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/validation_problem_source.py
--rw-r--r--   0        0        0     1467 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/veteran_status_enum.py
--rw-r--r--   0        0        0      760 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/visibility_enum.py
--rw-r--r--   0        0        0      915 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/ats/types/webhook_receiver.py
--rw-r--r--   0        0        0    10290 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/__init__.py
--rw-r--r--   0        0        0     9511 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/client.py
--rw-r--r--   0        0        0     1106 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2286 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2336 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2306 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/bank_info/__init__.py
--rw-r--r--   0        0        0     8705 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/bank_info/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/benefits/__init__.py
--rw-r--r--   0        0        0     6633 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/benefits/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/companies/__init__.py
--rw-r--r--   0        0        0     5928 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/companies/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2047 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/employee_payroll_runs/__init__.py
--rw-r--r--   0        0        0     8024 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/employee_payroll_runs/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/employees/__init__.py
--rw-r--r--   0        0        0    17711 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/employees/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/employments/__init__.py
--rw-r--r--   0        0        0     8741 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/employments/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     2364 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2539 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/groups/__init__.py
--rw-r--r--   0        0        0     7291 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/groups/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/issues/__init__.py
--rw-r--r--   0        0        0     6772 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/link_token/__init__.py
--rw-r--r--   0        0        0     4926 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0     5307 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/locations/__init__.py
--rw-r--r--   0        0        0     7265 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/locations/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     4902 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/pay_groups/__init__.py
--rw-r--r--   0        0        0     5946 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/pay_groups/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/payroll_runs/__init__.py
--rw-r--r--   0        0        0     8756 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/payroll_runs/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2547 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     6898 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     2646 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/teams/__init__.py
--rw-r--r--   0        0        0     6609 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/teams/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/time_off/__init__.py
--rw-r--r--   0        0        0    12810 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/time_off/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/time_off_balances/__init__.py
--rw-r--r--   0        0        0     8364 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/time_off_balances/client.py
--rw-r--r--   0        0        0       65 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     4459 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    14549 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/__init__.py
--rw-r--r--   0        0        0     1483 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/account_token.py
--rw-r--r--   0        0        0      555 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/account_type_enum.py
--rw-r--r--   0        0        0     1245 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/available_actions.py
--rw-r--r--   0        0        0     2399 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/bank_info.py
--rw-r--r--   0        0        0      185 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/bank_info_account_type.py
--rw-r--r--   0        0        0      529 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/bank_info_list_request_account_type.py
--rw-r--r--   0        0        0      728 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/bank_info_list_request_order_by.py
--rw-r--r--   0        0        0     2342 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/benefit.py
--rw-r--r--   0        0        0     1391 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     1962 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/company.py
--rw-r--r--   0        0        0     2324 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/condition_type_enum.py
--rw-r--r--   0        0        0    35178 2023-07-13 08:58:33.644106 fern_merge-0.0.30/src/merge/resources/hris/types/country_enum.py
--rw-r--r--   0        0        0      870 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/debug_model_log_summary.py
--rw-r--r--   0        0        0     2140 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/deduction.py
--rw-r--r--   0        0        0     2143 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/earning.py
--rw-r--r--   0        0        0      177 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/earning_type.py
--rw-r--r--   0        0        0      949 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/earning_type_enum.py
--rw-r--r--   0        0        0     6788 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employee.py
--rw-r--r--   0        0        0      205 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employee_employment_status.py
--rw-r--r--   0        0        0      176 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employee_ethnicity.py
--rw-r--r--   0        0        0      164 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employee_gender.py
--rw-r--r--   0        0        0      193 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employee_marital_status.py
--rw-r--r--   0        0        0     2796 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employee_payroll_run.py
--rw-r--r--   0        0        0      829 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py
--rw-r--r--   0        0        0      845 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py
--rw-r--r--   0        0        0     6252 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employee_request.py
--rw-r--r--   0        0        0      212 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employee_request_employment_status.py
--rw-r--r--   0        0        0      183 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employee_request_ethnicity.py
--rw-r--r--   0        0        0      171 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employee_request_gender.py
--rw-r--r--   0        0        0      200 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employee_request_marital_status.py
--rw-r--r--   0        0        0     1109 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employee_response.py
--rw-r--r--   0        0        0      739 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employees_list_request_employment_status.py
--rw-r--r--   0        0        0    80247 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employees_list_request_expand.py
--rw-r--r--   0        0        0     4067 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employees_list_request_remote_fields.py
--rw-r--r--   0        0        0     4115 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py
--rw-r--r--   0        0        0    81343 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employees_retrieve_request_expand.py
--rw-r--r--   0        0        0     4131 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     4179 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0    18682 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employment.py
--rw-r--r--   0        0        0      199 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employment_employment_type.py
--rw-r--r--   0        0        0      183 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employment_flsa_status.py
--rw-r--r--   0        0        0      187 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employment_pay_currency.py
--rw-r--r--   0        0        0      191 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employment_pay_frequency.py
--rw-r--r--   0        0        0      179 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employment_pay_period.py
--rw-r--r--   0        0        0      770 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employment_status_enum.py
--rw-r--r--   0        0        0     1166 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employment_type_enum.py
--rw-r--r--   0        0        0      777 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employments_list_request_expand.py
--rw-r--r--   0        0        0      707 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employments_list_request_order_by.py
--rw-r--r--   0        0        0     4219 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employments_list_request_remote_fields.py
--rw-r--r--   0        0        0     4267 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      793 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employments_retrieve_request_expand.py
--rw-r--r--   0        0        0     4283 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     4331 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0      522 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/error_validation_problem.py
--rw-r--r--   0        0        0     2511 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/ethnicity_enum.py
--rw-r--r--   0        0        0      986 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/flsa_status_enum.py
--rw-r--r--   0        0        0     1146 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/gender_enum.py
--rw-r--r--   0        0        0     2225 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/group.py
--rw-r--r--   0        0        0      169 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/group_type.py
--rw-r--r--   0        0        0     1136 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/group_type_enum.py
--rw-r--r--   0        0        0      180 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/ignore_common_model_request_reason.py
--rw-r--r--   0        0        0     1323 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/issue.py
--rw-r--r--   0        0        0      177 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/issue_status.py
--rw-r--r--   0        0        0      555 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/issues_list_request_status.py
--rw-r--r--   0        0        0      835 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0    11870 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/location.py
--rw-r--r--   0        0        0      168 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/location_country.py
--rw-r--r--   0        0        0      189 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/location_location_type.py
--rw-r--r--   0        0        0      509 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/location_type_enum.py
--rw-r--r--   0        0        0     1685 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/marital_status_enum.py
--rw-r--r--   0        0        0     1037 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/model_operation.py
--rw-r--r--   0        0        0     2012 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      189 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/multipart_form_field_request_encoding.py
--rw-r--r--   0        0        0      993 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/operator_schema.py
--rw-r--r--   0        0        0      959 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      893 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/paginated_bank_info_list.py
--rw-r--r--   0        0        0      888 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/paginated_benefit_list.py
--rw-r--r--   0        0        0      888 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/paginated_company_list.py
--rw-r--r--   0        0        0      921 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      892 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/paginated_employee_list.py
--rw-r--r--   0        0        0      934 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py
--rw-r--r--   0        0        0      900 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/paginated_employment_list.py
--rw-r--r--   0        0        0      880 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/paginated_group_list.py
--rw-r--r--   0        0        0      880 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/paginated_issue_list.py
--rw-r--r--   0        0        0      892 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/paginated_location_list.py
--rw-r--r--   0        0        0      893 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/paginated_pay_group_list.py
--rw-r--r--   0        0        0      901 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/paginated_payroll_run_list.py
--rw-r--r--   0        0        0      901 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      876 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/paginated_team_list.py
--rw-r--r--   0        0        0      918 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/paginated_time_off_balance_list.py
--rw-r--r--   0        0        0      889 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/paginated_time_off_list.py
--rw-r--r--   0        0        0    48882 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/pay_currency_enum.py
--rw-r--r--   0        0        0     1940 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/pay_frequency_enum.py
--rw-r--r--   0        0        0     1754 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/pay_group.py
--rw-r--r--   0        0        0     1798 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/pay_period_enum.py
--rw-r--r--   0        0        0     2811 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/payroll_run.py
--rw-r--r--   0        0        0      175 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/payroll_run_run_state.py
--rw-r--r--   0        0        0      171 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/payroll_run_run_type.py
--rw-r--r--   0        0        0      801 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py
--rw-r--r--   0        0        0     1104 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py
--rw-r--r--   0        0        0      813 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      817 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      829 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1305 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/policy_type_enum.py
--rw-r--r--   0        0        0      814 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/reason_enum.py
--rw-r--r--   0        0        0      802 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/remote_data.py
--rw-r--r--   0        0        0      986 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/remote_key.py
--rw-r--r--   0        0        0     1330 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/remote_response.py
--rw-r--r--   0        0        0      195 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/remote_response_response_type.py
--rw-r--r--   0        0        0      723 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/request_format_enum.py
--rw-r--r--   0        0        0     1312 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/request_type_enum.py
--rw-r--r--   0        0        0      562 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/response_type_enum.py
--rw-r--r--   0        0        0     1032 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/run_state_enum.py
--rw-r--r--   0        0        0     1173 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/run_type_enum.py
--rw-r--r--   0        0        0      695 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1975 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/tax.py
--rw-r--r--   0        0        0     1953 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/team.py
--rw-r--r--   0        0        0     3481 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off.py
--rw-r--r--   0        0        0     2517 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_balance.py
--rw-r--r--   0        0        0      187 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_balance_policy_type.py
--rw-r--r--   0        0        0     1272 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py
--rw-r--r--   0        0        0      751 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_list_request_expand.py
--rw-r--r--   0        0        0     1595 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_list_request_remote_fields.py
--rw-r--r--   0        0        0     1223 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_list_request_request_type.py
--rw-r--r--   0        0        0     1619 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py
--rw-r--r--   0        0        0     1029 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_list_request_status.py
--rw-r--r--   0        0        0     3199 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_request.py
--rw-r--r--   0        0        0      191 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_request_request_type.py
--rw-r--r--   0        0        0      193 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_request_status.py
--rw-r--r--   0        0        0      184 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_request_type.py
--rw-r--r--   0        0        0      166 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_request_units.py
--rw-r--r--   0        0        0     1106 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_response.py
--rw-r--r--   0        0        0      767 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_retrieve_request_expand.py
--rw-r--r--   0        0        0     1627 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     1651 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0      186 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_status.py
--rw-r--r--   0        0        0     1146 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_status_enum.py
--rw-r--r--   0        0        0      159 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/time_off_units.py
--rw-r--r--   0        0        0      495 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/units_enum.py
--rw-r--r--   0        0        0      762 2023-07-13 08:58:33.648106 fern_merge-0.0.30/src/merge/resources/hris/types/validation_problem_source.py
--rw-r--r--   0        0        0      915 2023-07-13 08:58:33.652106 fern_merge-0.0.30/src/merge/resources/hris/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-13 08:58:33.652106 fern_merge-0.0.30/src/merge/resources/hris/types/webhook_receiver.py
--rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 fern_merge-0.0.30/PKG-INFO
+-rw-r--r--   0        0        0     2139 2023-07-16 22:28:32.546961 fern_merge-0.0.32/README.md
+-rw-r--r--   0        0        0      371 2023-07-16 22:28:32.546961 fern_merge-0.0.32/pyproject.toml
+-rw-r--r--   0        0        0      187 2023-07-16 22:28:32.546961 fern_merge-0.0.32/src/merge/__init__.py
+-rw-r--r--   0        0        0     1627 2023-07-16 22:28:32.546961 fern_merge-0.0.32/src/merge/client.py
+-rw-r--r--   0        0        0      519 2023-07-16 22:28:32.546961 fern_merge-0.0.32/src/merge/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-16 22:28:32.546961 fern_merge-0.0.32/src/merge/core/api_error.py
+-rw-r--r--   0        0        0     1101 2023-07-16 22:28:32.546961 fern_merge-0.0.32/src/merge/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2023-07-16 22:28:32.546961 fern_merge-0.0.32/src/merge/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-16 22:28:32.546961 fern_merge-0.0.32/src/merge/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2023-07-16 22:28:32.546961 fern_merge-0.0.32/src/merge/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      201 2023-07-16 22:28:32.546961 fern_merge-0.0.32/src/merge/environment.py
+-rw-r--r--   0        0        0        0 2023-07-16 22:28:32.546961 fern_merge-0.0.32/src/merge/py.typed
+-rw-r--r--   0        0        0      116 2023-07-16 22:28:32.546961 fern_merge-0.0.32/src/merge/resources/__init__.py
+-rw-r--r--   0        0        0     9656 2023-07-16 22:28:32.546961 fern_merge-0.0.32/src/merge/resources/ats/__init__.py
+-rw-r--r--   0        0        0    10018 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/client.py
+-rw-r--r--   0        0        0     1144 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2284 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2334 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/activities/__init__.py
+-rw-r--r--   0        0        0    12564 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/activities/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/applications/__init__.py
+-rw-r--r--   0        0        0    15247 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/applications/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/attachments/__init__.py
+-rw-r--r--   0        0        0    12326 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/attachments/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2304 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/candidates/__init__.py
+-rw-r--r--   0        0        0    17208 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/candidates/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2045 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/departments/__init__.py
+-rw-r--r--   0        0        0     6270 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/departments/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/eeocs/__init__.py
+-rw-r--r--   0        0        0     8547 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/eeocs/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     2362 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2537 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/interviews/__init__.py
+-rw-r--r--   0        0        0    13032 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/interviews/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/issues/__init__.py
+-rw-r--r--   0        0        0     7052 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/job_interview_stages/__init__.py
+-rw-r--r--   0        0        0     7085 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/job_interview_stages/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/jobs/__init__.py
+-rw-r--r--   0        0        0     8673 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/jobs/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     4924 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0     5589 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/offers/__init__.py
+-rw-r--r--   0        0        0     8533 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/offers/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/offices/__init__.py
+-rw-r--r--   0        0        0     6198 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/offices/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     4900 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2545 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/reject_reasons/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/reject_reasons/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/scorecards/__init__.py
+-rw-r--r--   0        0        0     8991 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/scorecards/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     7004 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     2756 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/tags/__init__.py
+-rw-r--r--   0        0        0     4453 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/tags/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/users/__init__.py
+-rw-r--r--   0        0        0     7813 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/users/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     4455 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    13447 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/__init__.py
+-rw-r--r--   0        0        0     1240 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/access_role_enum.py
+-rw-r--r--   0        0        0     1483 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/account_token.py
+-rw-r--r--   0        0        0      857 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/activities_list_request_remote_fields.py
+-rw-r--r--   0        0        0      869 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      873 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      885 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     2705 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/activity.py
+-rw-r--r--   0        0        0      189 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/activity_activity_type.py
+-rw-r--r--   0        0        0     2155 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/activity_request.py
+-rw-r--r--   0        0        0      196 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/activity_request_activity_type.py
+-rw-r--r--   0        0        0      187 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/activity_request_visibility.py
+-rw-r--r--   0        0        0     1109 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/activity_response.py
+-rw-r--r--   0        0        0      705 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/activity_type_enum.py
+-rw-r--r--   0        0        0      180 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/activity_visibility.py
+-rw-r--r--   0        0        0     2473 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/application.py
+-rw-r--r--   0        0        0     2269 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/application_request.py
+-rw-r--r--   0        0        0     1121 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/application_response.py
+-rw-r--r--   0        0        0     8243 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/applications_list_request_expand.py
+-rw-r--r--   0        0        0     8371 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/applications_retrieve_request_expand.py
+-rw-r--r--   0        0        0     2146 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/attachment.py
+-rw-r--r--   0        0        0      199 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/attachment_attachment_type.py
+-rw-r--r--   0        0        0     1820 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/attachment_request.py
+-rw-r--r--   0        0        0      206 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/attachment_request_attachment_type.py
+-rw-r--r--   0        0        0     1117 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/attachment_response.py
+-rw-r--r--   0        0        0      985 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/attachment_type_enum.py
+-rw-r--r--   0        0        0     1245 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/available_actions.py
+-rw-r--r--   0        0        0     3471 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/candidate.py
+-rw-r--r--   0        0        0     3061 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/candidate_request.py
+-rw-r--r--   0        0        0     1113 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/candidate_response.py
+-rw-r--r--   0        0        0      833 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/candidates_list_request_expand.py
+-rw-r--r--   0        0        0      849 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/candidates_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1391 2023-07-16 22:28:32.550961 fern_merge-0.0.32/src/merge/resources/ats/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     2324 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/condition_type_enum.py
+-rw-r--r--   0        0        0      870 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0     1698 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/department.py
+-rw-r--r--   0        0        0     1337 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/disability_status_enum.py
+-rw-r--r--   0        0        0     4088 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/eeoc.py
+-rw-r--r--   0        0        0      201 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/eeoc_disability_status.py
+-rw-r--r--   0        0        0      160 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/eeoc_gender.py
+-rw-r--r--   0        0        0      152 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/eeoc_race.py
+-rw-r--r--   0        0        0      189 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/eeoc_veteran_status.py
+-rw-r--r--   0        0        0     3803 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py
+-rw-r--r--   0        0        0     3851 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0     3867 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     3915 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1529 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/email_address.py
+-rw-r--r--   0        0        0      210 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/email_address_email_address_type.py
+-rw-r--r--   0        0        0     1553 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/email_address_request.py
+-rw-r--r--   0        0        0      217 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/email_address_request_email_address_type.py
+-rw-r--r--   0        0        0      742 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/email_address_type_enum.py
+-rw-r--r--   0        0        0      522 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/error_validation_problem.py
+-rw-r--r--   0        0        0     1160 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/gender_enum.py
+-rw-r--r--   0        0        0     4187 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/interviews_list_request_expand.py
+-rw-r--r--   0        0        0     4251 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/interviews_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1323 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/issues_list_request_status.py
+-rw-r--r--   0        0        0     3428 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/job.py
+-rw-r--r--   0        0        0     2387 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/job_interview_stage.py
+-rw-r--r--   0        0        0      169 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/job_status.py
+-rw-r--r--   0        0        0     1045 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/job_status_enum.py
+-rw-r--r--   0        0        0     3771 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/jobs_list_request_expand.py
+-rw-r--r--   0        0        0      956 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/jobs_list_request_status.py
+-rw-r--r--   0        0        0     3835 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/jobs_retrieve_request_expand.py
+-rw-r--r--   0        0        0      835 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0     1037 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0     2786 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/offer.py
+-rw-r--r--   0        0        0      177 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/offer_status.py
+-rw-r--r--   0        0        0     1832 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/offer_status_enum.py
+-rw-r--r--   0        0        0      767 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/offers_list_request_expand.py
+-rw-r--r--   0        0        0      783 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/offers_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1817 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/office.py
+-rw-r--r--   0        0        0      993 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/operator_schema.py
+-rw-r--r--   0        0        0     1180 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/overall_recommendation_enum.py
+-rw-r--r--   0        0        0      959 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      892 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_activity_list.py
+-rw-r--r--   0        0        0      904 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_application_list.py
+-rw-r--r--   0        0        0      900 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_attachment_list.py
+-rw-r--r--   0        0        0      896 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_candidate_list.py
+-rw-r--r--   0        0        0      921 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      900 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_department_list.py
+-rw-r--r--   0        0        0      876 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_eeoc_list.py
+-rw-r--r--   0        0        0      880 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      930 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_job_interview_stage_list.py
+-rw-r--r--   0        0        0      872 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_job_list.py
+-rw-r--r--   0        0        0      880 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_offer_list.py
+-rw-r--r--   0        0        0      884 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_office_list.py
+-rw-r--r--   0        0        0      909 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_reject_reason_list.py
+-rw-r--r--   0        0        0      901 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_remote_user_list.py
+-rw-r--r--   0        0        0      933 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_scheduled_interview_list.py
+-rw-r--r--   0        0        0      896 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_scorecard_list.py
+-rw-r--r--   0        0        0      901 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      872 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/paginated_tag_list.py
+-rw-r--r--   0        0        0     3068 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/patched_candidate_request.py
+-rw-r--r--   0        0        0     1624 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/phone_number.py
+-rw-r--r--   0        0        0      205 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/phone_number_phone_number_type.py
+-rw-r--r--   0        0        0     1648 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/phone_number_request.py
+-rw-r--r--   0        0        0      212 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/phone_number_request_phone_number_type.py
+-rw-r--r--   0        0        0     1039 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/phone_number_type_enum.py
+-rw-r--r--   0        0        0     2326 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/race_enum.py
+-rw-r--r--   0        0        0      814 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/reason_enum.py
+-rw-r--r--   0        0        0     1775 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/reject_reason.py
+-rw-r--r--   0        0        0      802 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/remote_data.py
+-rw-r--r--   0        0        0      986 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/remote_key.py
+-rw-r--r--   0        0        0     1330 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/remote_response.py
+-rw-r--r--   0        0        0      195 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/remote_response_response_type.py
+-rw-r--r--   0        0        0     2562 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/remote_user.py
+-rw-r--r--   0        0        0      183 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/remote_user_access_role.py
+-rw-r--r--   0        0        0      723 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/request_format_enum.py
+-rw-r--r--   0        0        0      562 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/response_type_enum.py
+-rw-r--r--   0        0        0     3187 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/scheduled_interview.py
+-rw-r--r--   0        0        0     2464 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/scheduled_interview_request.py
+-rw-r--r--   0        0        0      237 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/scheduled_interview_request_status.py
+-rw-r--r--   0        0        0     1150 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/scheduled_interview_response.py
+-rw-r--r--   0        0        0      230 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/scheduled_interview_status.py
+-rw-r--r--   0        0        0      893 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/scheduled_interview_status_enum.py
+-rw-r--r--   0        0        0     2692 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/scorecard.py
+-rw-r--r--   0        0        0      226 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/scorecard_overall_recommendation.py
+-rw-r--r--   0        0        0     1731 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/scorecards_list_request_expand.py
+-rw-r--r--   0        0        0     1763 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py
+-rw-r--r--   0        0        0      695 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1623 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/tag.py
+-rw-r--r--   0        0        0     1659 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/url.py
+-rw-r--r--   0        0        0     1683 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/url_request.py
+-rw-r--r--   0        0        0      171 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/url_request_url_type.py
+-rw-r--r--   0        0        0     1451 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/url_type_enum.py
+-rw-r--r--   0        0        0      164 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/url_url_type.py
+-rw-r--r--   0        0        0      762 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/validation_problem_source.py
+-rw-r--r--   0        0        0     1467 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/veteran_status_enum.py
+-rw-r--r--   0        0        0      760 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/visibility_enum.py
+-rw-r--r--   0        0        0      915 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/ats/types/webhook_receiver.py
+-rw-r--r--   0        0        0    10290 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/hris/__init__.py
+-rw-r--r--   0        0        0     9511 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/hris/client.py
+-rw-r--r--   0        0        0     1106 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/hris/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/hris/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2286 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/hris/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/hris/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2336 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/hris/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/hris/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2306 2023-07-16 22:28:32.554961 fern_merge-0.0.32/src/merge/resources/hris/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/bank_info/__init__.py
+-rw-r--r--   0        0        0     9159 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/bank_info/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/benefits/__init__.py
+-rw-r--r--   0        0        0     6947 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/benefits/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/companies/__init__.py
+-rw-r--r--   0        0        0     6226 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/companies/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2047 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/employee_payroll_runs/__init__.py
+-rw-r--r--   0        0        0     8378 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/employee_payroll_runs/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/employees/__init__.py
+-rw-r--r--   0        0        0    18323 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/employees/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/employments/__init__.py
+-rw-r--r--   0        0        0     9179 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/employments/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     2364 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2539 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/groups/__init__.py
+-rw-r--r--   0        0        0     7705 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/groups/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/issues/__init__.py
+-rw-r--r--   0        0        0     7056 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     4926 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0     5591 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/locations/__init__.py
+-rw-r--r--   0        0        0     7671 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/locations/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     4902 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/pay_groups/__init__.py
+-rw-r--r--   0        0        0     6244 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/pay_groups/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/payroll_runs/__init__.py
+-rw-r--r--   0        0        0     9202 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/payroll_runs/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2547 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     7010 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     2758 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/teams/__init__.py
+-rw-r--r--   0        0        0     6923 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/teams/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/time_off/__init__.py
+-rw-r--r--   0        0        0    13310 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/time_off/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/time_off_balances/__init__.py
+-rw-r--r--   0        0        0     8802 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/time_off_balances/client.py
+-rw-r--r--   0        0        0       65 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     4459 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    14549 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/account_token.py
+-rw-r--r--   0        0        0      555 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/account_type_enum.py
+-rw-r--r--   0        0        0     1245 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/available_actions.py
+-rw-r--r--   0        0        0     2399 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/bank_info.py
+-rw-r--r--   0        0        0      185 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/bank_info_account_type.py
+-rw-r--r--   0        0        0      529 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/bank_info_list_request_account_type.py
+-rw-r--r--   0        0        0      728 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/bank_info_list_request_order_by.py
+-rw-r--r--   0        0        0     2342 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/benefit.py
+-rw-r--r--   0        0        0     1391 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     1962 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/company.py
+-rw-r--r--   0        0        0     2324 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/condition_type_enum.py
+-rw-r--r--   0        0        0    35178 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/country_enum.py
+-rw-r--r--   0        0        0      870 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0     2140 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/deduction.py
+-rw-r--r--   0        0        0     2143 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/earning.py
+-rw-r--r--   0        0        0      177 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/earning_type.py
+-rw-r--r--   0        0        0      949 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/earning_type_enum.py
+-rw-r--r--   0        0        0     6788 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employee.py
+-rw-r--r--   0        0        0      205 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employee_employment_status.py
+-rw-r--r--   0        0        0      176 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employee_ethnicity.py
+-rw-r--r--   0        0        0      164 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employee_gender.py
+-rw-r--r--   0        0        0      193 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employee_marital_status.py
+-rw-r--r--   0        0        0     2796 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employee_payroll_run.py
+-rw-r--r--   0        0        0      829 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py
+-rw-r--r--   0        0        0      845 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py
+-rw-r--r--   0        0        0     6252 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employee_request.py
+-rw-r--r--   0        0        0      212 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employee_request_employment_status.py
+-rw-r--r--   0        0        0      183 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employee_request_ethnicity.py
+-rw-r--r--   0        0        0      171 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employee_request_gender.py
+-rw-r--r--   0        0        0      200 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employee_request_marital_status.py
+-rw-r--r--   0        0        0     1109 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employee_response.py
+-rw-r--r--   0        0        0      739 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employees_list_request_employment_status.py
+-rw-r--r--   0        0        0    80247 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employees_list_request_expand.py
+-rw-r--r--   0        0        0     4067 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employees_list_request_remote_fields.py
+-rw-r--r--   0        0        0     4115 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0    81343 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employees_retrieve_request_expand.py
+-rw-r--r--   0        0        0     4131 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     4179 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0    18682 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employment.py
+-rw-r--r--   0        0        0      199 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employment_employment_type.py
+-rw-r--r--   0        0        0      183 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employment_flsa_status.py
+-rw-r--r--   0        0        0      187 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employment_pay_currency.py
+-rw-r--r--   0        0        0      191 2023-07-16 22:28:32.558961 fern_merge-0.0.32/src/merge/resources/hris/types/employment_pay_frequency.py
+-rw-r--r--   0        0        0      179 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/employment_pay_period.py
+-rw-r--r--   0        0        0      770 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/employment_status_enum.py
+-rw-r--r--   0        0        0     1166 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/employment_type_enum.py
+-rw-r--r--   0        0        0      777 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/employments_list_request_expand.py
+-rw-r--r--   0        0        0      707 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/employments_list_request_order_by.py
+-rw-r--r--   0        0        0     4219 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/employments_list_request_remote_fields.py
+-rw-r--r--   0        0        0     4267 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      793 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/employments_retrieve_request_expand.py
+-rw-r--r--   0        0        0     4283 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     4331 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0      522 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/error_validation_problem.py
+-rw-r--r--   0        0        0     2511 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/ethnicity_enum.py
+-rw-r--r--   0        0        0      986 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/flsa_status_enum.py
+-rw-r--r--   0        0        0     1146 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/gender_enum.py
+-rw-r--r--   0        0        0     2225 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/group.py
+-rw-r--r--   0        0        0      169 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/group_type.py
+-rw-r--r--   0        0        0     1136 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/group_type_enum.py
+-rw-r--r--   0        0        0      180 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/ignore_common_model_request_reason.py
+-rw-r--r--   0        0        0     1323 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/issues_list_request_status.py
+-rw-r--r--   0        0        0      835 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0    11870 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/location.py
+-rw-r--r--   0        0        0      168 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/location_country.py
+-rw-r--r--   0        0        0      189 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/location_location_type.py
+-rw-r--r--   0        0        0      509 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/location_type_enum.py
+-rw-r--r--   0        0        0     1685 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/marital_status_enum.py
+-rw-r--r--   0        0        0     1037 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0      993 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/operator_schema.py
+-rw-r--r--   0        0        0      959 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      893 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/paginated_bank_info_list.py
+-rw-r--r--   0        0        0      888 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/paginated_benefit_list.py
+-rw-r--r--   0        0        0      888 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/paginated_company_list.py
+-rw-r--r--   0        0        0      921 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      892 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/paginated_employee_list.py
+-rw-r--r--   0        0        0      934 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py
+-rw-r--r--   0        0        0      900 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/paginated_employment_list.py
+-rw-r--r--   0        0        0      880 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/paginated_group_list.py
+-rw-r--r--   0        0        0      880 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      892 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/paginated_location_list.py
+-rw-r--r--   0        0        0      893 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/paginated_pay_group_list.py
+-rw-r--r--   0        0        0      901 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/paginated_payroll_run_list.py
+-rw-r--r--   0        0        0      901 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      876 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/paginated_team_list.py
+-rw-r--r--   0        0        0      918 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/paginated_time_off_balance_list.py
+-rw-r--r--   0        0        0      889 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/paginated_time_off_list.py
+-rw-r--r--   0        0        0    48882 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/pay_currency_enum.py
+-rw-r--r--   0        0        0     1940 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/pay_frequency_enum.py
+-rw-r--r--   0        0        0     1754 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/pay_group.py
+-rw-r--r--   0        0        0     1798 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/pay_period_enum.py
+-rw-r--r--   0        0        0     2811 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/payroll_run.py
+-rw-r--r--   0        0        0      175 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/payroll_run_run_state.py
+-rw-r--r--   0        0        0      171 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/payroll_run_run_type.py
+-rw-r--r--   0        0        0      801 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py
+-rw-r--r--   0        0        0     1104 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py
+-rw-r--r--   0        0        0      813 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      817 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      829 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1305 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/policy_type_enum.py
+-rw-r--r--   0        0        0      814 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/reason_enum.py
+-rw-r--r--   0        0        0      802 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/remote_data.py
+-rw-r--r--   0        0        0      986 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/remote_key.py
+-rw-r--r--   0        0        0     1330 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/remote_response.py
+-rw-r--r--   0        0        0      195 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/remote_response_response_type.py
+-rw-r--r--   0        0        0      723 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/request_format_enum.py
+-rw-r--r--   0        0        0     1312 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/request_type_enum.py
+-rw-r--r--   0        0        0      562 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/response_type_enum.py
+-rw-r--r--   0        0        0     1032 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/run_state_enum.py
+-rw-r--r--   0        0        0     1173 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/run_type_enum.py
+-rw-r--r--   0        0        0      695 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1975 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/tax.py
+-rw-r--r--   0        0        0     1953 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/team.py
+-rw-r--r--   0        0        0     3481 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off.py
+-rw-r--r--   0        0        0     2517 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_balance.py
+-rw-r--r--   0        0        0      187 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_balance_policy_type.py
+-rw-r--r--   0        0        0     1272 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py
+-rw-r--r--   0        0        0      751 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_list_request_expand.py
+-rw-r--r--   0        0        0     1595 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_list_request_remote_fields.py
+-rw-r--r--   0        0        0     1223 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_list_request_request_type.py
+-rw-r--r--   0        0        0     1619 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1029 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_list_request_status.py
+-rw-r--r--   0        0        0     3199 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_request.py
+-rw-r--r--   0        0        0      191 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_request_request_type.py
+-rw-r--r--   0        0        0      193 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_request_status.py
+-rw-r--r--   0        0        0      184 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_request_type.py
+-rw-r--r--   0        0        0      166 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_request_units.py
+-rw-r--r--   0        0        0     1106 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_response.py
+-rw-r--r--   0        0        0      767 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1627 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     1651 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0      186 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_status.py
+-rw-r--r--   0        0        0     1146 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_status_enum.py
+-rw-r--r--   0        0        0      159 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/time_off_units.py
+-rw-r--r--   0        0        0      495 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/units_enum.py
+-rw-r--r--   0        0        0      762 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/validation_problem_source.py
+-rw-r--r--   0        0        0      915 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-16 22:28:32.562961 fern_merge-0.0.32/src/merge/resources/hris/types/webhook_receiver.py
+-rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 fern_merge-0.0.32/PKG-INFO
```

### Comparing `fern_merge-0.0.30/README.md` & `fern_merge-0.0.32/README.md`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/client.py` & `fern_merge-0.0.32/src/merge/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         self,
         *,
         environment: MergeEnvironment = MergeEnvironment.PRODUCTION,
         account_token: typing.Optional[str] = None,
         api_key: str,
         timeout: typing.Optional[float] = 60
     ):
+        self._environment = environment
         self._client_wrapper = SyncClientWrapper(
             account_token=account_token, api_key=api_key, httpx_client=httpx.Client(timeout=timeout)
         )
         self.ats = AtsClient(environment=environment, client_wrapper=self._client_wrapper)
         self.hris = HrisClient(environment=environment, client_wrapper=self._client_wrapper)
 
 
@@ -31,12 +32,13 @@
         self,
         *,
         environment: MergeEnvironment = MergeEnvironment.PRODUCTION,
         account_token: typing.Optional[str] = None,
         api_key: str,
         timeout: typing.Optional[float] = 60
     ):
+        self._environment = environment
         self._client_wrapper = AsyncClientWrapper(
             account_token=account_token, api_key=api_key, httpx_client=httpx.AsyncClient(timeout=timeout)
         )
         self.ats = AsyncAtsClient(environment=environment, client_wrapper=self._client_wrapper)
         self.hris = AsyncHrisClient(environment=environment, client_wrapper=self._client_wrapper)
```

### Comparing `fern_merge-0.0.30/src/merge/core/__init__.py` & `fern_merge-0.0.32/src/merge/core/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .api_error import ApiError
 from .client_wrapper import AsyncClientWrapper, BaseClientWrapper, SyncClientWrapper
 from .datetime_utils import serialize_datetime
 from .jsonable_encoder import jsonable_encoder
-from .remove_none_from_headers import remove_none_from_headers
+from .remove_none_from_dict import remove_none_from_dict
 
 __all__ = [
     "ApiError",
     "AsyncClientWrapper",
     "BaseClientWrapper",
     "SyncClientWrapper",
     "jsonable_encoder",
-    "remove_none_from_headers",
+    "remove_none_from_dict",
     "serialize_datetime",
 ]
```

### Comparing `fern_merge-0.0.30/src/merge/core/client_wrapper.py` & `fern_merge-0.0.32/src/merge/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/core/datetime_utils.py` & `fern_merge-0.0.32/src/merge/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/core/jsonable_encoder.py` & `fern_merge-0.0.32/src/merge/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/__init__.py` & `fern_merge-0.0.32/src/merge/resources/ats/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/__init__.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/account_details/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/account_token/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/activities/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/activities/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import pydantic
 import typing_extensions
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.activities_list_request_remote_fields import ActivitiesListRequestRemoteFields
 from ...types.activities_list_request_show_enum_origins import ActivitiesListRequestShowEnumOrigins
 from ...types.activities_retrieve_request_remote_fields import ActivitiesRetrieveRequestRemoteFields
 from ...types.activities_retrieve_request_show_enum_origins import ActivitiesRetrieveRequestShowEnumOrigins
 from ...types.activity import Activity
 from ...types.activity_request import ActivityRequest
@@ -48,29 +49,31 @@
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[ActivitiesListRequestShowEnumOrigins] = None,
         user_id: typing.Optional[str] = None,
     ) -> PaginatedActivityList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/activities"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-                "user_id": user_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                    "user_id": user_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedActivityList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -85,15 +88,15 @@
         run_async: typing.Optional[bool] = None,
         model: ActivityRequest,
         remote_user_id: str,
     ) -> ActivityResponse:
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/activities"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model, "remote_user_id": remote_user_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ActivityResponse, _response.json())  # type: ignore
         try:
@@ -110,20 +113,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[ActivitiesRetrieveRequestRemoteFields] = None,
         show_enum_origins: typing.Optional[ActivitiesRetrieveRequestShowEnumOrigins] = None,
     ) -> Activity:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/activities/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Activity, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -170,29 +175,31 @@
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[ActivitiesListRequestShowEnumOrigins] = None,
         user_id: typing.Optional[str] = None,
     ) -> PaginatedActivityList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/activities"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-                "user_id": user_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                    "user_id": user_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedActivityList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -207,15 +214,15 @@
         run_async: typing.Optional[bool] = None,
         model: ActivityRequest,
         remote_user_id: str,
     ) -> ActivityResponse:
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/activities"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model, "remote_user_id": remote_user_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ActivityResponse, _response.json())  # type: ignore
         try:
@@ -232,20 +239,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[ActivitiesRetrieveRequestRemoteFields] = None,
         show_enum_origins: typing.Optional[ActivitiesRetrieveRequestShowEnumOrigins] = None,
     ) -> Activity:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/activities/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Activity, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/applications/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/applications/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.application import Application
 from ...types.application_request import ApplicationRequest
 from ...types.application_response import ApplicationResponse
 from ...types.applications_list_request_expand import ApplicationsListRequestExpand
 from ...types.applications_retrieve_request_expand import ApplicationsRetrieveRequestExpand
 from ...types.meta_response import MetaResponse
@@ -48,32 +49,34 @@
         reject_reason_id: typing.Optional[str] = None,
         remote_id: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
     ) -> PaginatedApplicationList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/applications"),
-            params={
-                "candidate_id": candidate_id,
-                "created_after": created_after,
-                "created_before": created_before,
-                "credited_to_id": credited_to_id,
-                "current_stage_id": current_stage_id,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "job_id": job_id,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "reject_reason_id": reject_reason_id,
-                "remote_id": remote_id,
-                "source": source,
-            },
+            params=remove_none_from_dict(
+                {
+                    "candidate_id": candidate_id,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "credited_to_id": credited_to_id,
+                    "current_stage_id": current_stage_id,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "job_id": job_id,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "reject_reason_id": reject_reason_id,
+                    "remote_id": remote_id,
+                    "source": source,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedApplicationList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -88,15 +91,15 @@
         run_async: typing.Optional[bool] = None,
         model: ApplicationRequest,
         remote_user_id: str,
     ) -> ApplicationResponse:
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/applications"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model, "remote_user_id": remote_user_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ApplicationResponse, _response.json())  # type: ignore
         try:
@@ -111,15 +114,15 @@
         *,
         expand: typing.Optional[ApplicationsRetrieveRequestExpand] = None,
         include_remote_data: typing.Optional[bool] = None,
     ) -> Application:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/applications/{id}"),
-            params={"expand": expand, "include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Application, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -140,15 +143,15 @@
         if job_interview_stage is not OMIT:
             _request["job_interview_stage"] = job_interview_stage
         if remote_user_id is not OMIT:
             _request["remote_user_id"] = remote_user_id
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/applications/{id}/change-stage"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ApplicationResponse, _response.json())  # type: ignore
         try:
@@ -157,15 +160,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def meta_post_retrieve(self, *, application_remote_template_id: typing.Optional[str] = None) -> MetaResponse:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/applications/meta/post"),
-            params={"application_remote_template_id": application_remote_template_id},
+            params=remove_none_from_dict({"application_remote_template_id": application_remote_template_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -200,32 +203,34 @@
         reject_reason_id: typing.Optional[str] = None,
         remote_id: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
     ) -> PaginatedApplicationList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/applications"),
-            params={
-                "candidate_id": candidate_id,
-                "created_after": created_after,
-                "created_before": created_before,
-                "credited_to_id": credited_to_id,
-                "current_stage_id": current_stage_id,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "job_id": job_id,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "reject_reason_id": reject_reason_id,
-                "remote_id": remote_id,
-                "source": source,
-            },
+            params=remove_none_from_dict(
+                {
+                    "candidate_id": candidate_id,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "credited_to_id": credited_to_id,
+                    "current_stage_id": current_stage_id,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "job_id": job_id,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "reject_reason_id": reject_reason_id,
+                    "remote_id": remote_id,
+                    "source": source,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedApplicationList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -240,15 +245,15 @@
         run_async: typing.Optional[bool] = None,
         model: ApplicationRequest,
         remote_user_id: str,
     ) -> ApplicationResponse:
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/applications"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model, "remote_user_id": remote_user_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ApplicationResponse, _response.json())  # type: ignore
         try:
@@ -263,15 +268,15 @@
         *,
         expand: typing.Optional[ApplicationsRetrieveRequestExpand] = None,
         include_remote_data: typing.Optional[bool] = None,
     ) -> Application:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/applications/{id}"),
-            params={"expand": expand, "include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Application, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -292,15 +297,15 @@
         if job_interview_stage is not OMIT:
             _request["job_interview_stage"] = job_interview_stage
         if remote_user_id is not OMIT:
             _request["remote_user_id"] = remote_user_id
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/applications/{id}/change-stage"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ApplicationResponse, _response.json())  # type: ignore
         try:
@@ -309,15 +314,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def meta_post_retrieve(self, *, application_remote_template_id: typing.Optional[str] = None) -> MetaResponse:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/applications/meta/post"),
-            params={"application_remote_template_id": application_remote_template_id},
+            params=remove_none_from_dict({"application_remote_template_id": application_remote_template_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MetaResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/attachments/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/attachments/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import pydantic
 import typing_extensions
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.attachment import Attachment
 from ...types.attachment_request import AttachmentRequest
 from ...types.attachment_response import AttachmentResponse
 from ...types.meta_response import MetaResponse
 from ...types.paginated_attachment_list import PaginatedAttachmentList
 
@@ -44,29 +45,31 @@
         remote_fields: typing.Optional[typing_extensions.Literal["attachment_type"]] = None,
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["attachment_type"]] = None,
     ) -> PaginatedAttachmentList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/attachments"),
-            params={
-                "candidate_id": candidate_id,
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "candidate_id": candidate_id,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedAttachmentList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -81,15 +84,15 @@
         run_async: typing.Optional[bool] = None,
         model: AttachmentRequest,
         remote_user_id: str,
     ) -> AttachmentResponse:
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/attachments"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model, "remote_user_id": remote_user_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AttachmentResponse, _response.json())  # type: ignore
         try:
@@ -106,20 +109,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[typing_extensions.Literal["attachment_type"]] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["attachment_type"]] = None,
     ) -> Attachment:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/attachments/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Attachment, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -166,29 +171,31 @@
         remote_fields: typing.Optional[typing_extensions.Literal["attachment_type"]] = None,
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["attachment_type"]] = None,
     ) -> PaginatedAttachmentList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/attachments"),
-            params={
-                "candidate_id": candidate_id,
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "candidate_id": candidate_id,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedAttachmentList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -203,15 +210,15 @@
         run_async: typing.Optional[bool] = None,
         model: AttachmentRequest,
         remote_user_id: str,
     ) -> AttachmentResponse:
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/attachments"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model, "remote_user_id": remote_user_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AttachmentResponse, _response.json())  # type: ignore
         try:
@@ -228,20 +235,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[typing_extensions.Literal["attachment_type"]] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["attachment_type"]] = None,
     ) -> Attachment:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/attachments/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Attachment, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/available_actions/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/candidates/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/candidates/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.candidate import Candidate
 from ...types.candidate_request import CandidateRequest
 from ...types.candidate_response import CandidateResponse
 from ...types.candidates_list_request_expand import CandidatesListRequestExpand
 from ...types.candidates_retrieve_request_expand import CandidatesRetrieveRequestExpand
 from ...types.meta_response import MetaResponse
@@ -48,30 +49,32 @@
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
         tags: typing.Optional[str] = None,
     ) -> PaginatedCandidateList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/candidates"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "email_addresses": email_addresses,
-                "expand": expand,
-                "first_name": first_name,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "last_name": last_name,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-                "tags": tags,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "email_addresses": email_addresses,
+                    "expand": expand,
+                    "first_name": first_name,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "last_name": last_name,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                    "tags": tags,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedCandidateList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -86,15 +89,15 @@
         run_async: typing.Optional[bool] = None,
         model: CandidateRequest,
         remote_user_id: str,
     ) -> CandidateResponse:
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/candidates"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model, "remote_user_id": remote_user_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CandidateResponse, _response.json())  # type: ignore
         try:
@@ -109,15 +112,15 @@
         *,
         expand: typing.Optional[CandidatesRetrieveRequestExpand] = None,
         include_remote_data: typing.Optional[bool] = None,
     ) -> Candidate:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/candidates/{id}"),
-            params={"expand": expand, "include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Candidate, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -133,15 +136,15 @@
         run_async: typing.Optional[bool] = None,
         model: PatchedCandidateRequest,
         remote_user_id: str,
     ) -> CandidateResponse:
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/candidates/{id}"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model, "remote_user_id": remote_user_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CandidateResponse, _response.json())  # type: ignore
         try:
@@ -224,30 +227,32 @@
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
         tags: typing.Optional[str] = None,
     ) -> PaginatedCandidateList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/candidates"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "email_addresses": email_addresses,
-                "expand": expand,
-                "first_name": first_name,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "last_name": last_name,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-                "tags": tags,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "email_addresses": email_addresses,
+                    "expand": expand,
+                    "first_name": first_name,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "last_name": last_name,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                    "tags": tags,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedCandidateList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -262,15 +267,15 @@
         run_async: typing.Optional[bool] = None,
         model: CandidateRequest,
         remote_user_id: str,
     ) -> CandidateResponse:
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/candidates"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model, "remote_user_id": remote_user_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CandidateResponse, _response.json())  # type: ignore
         try:
@@ -285,15 +290,15 @@
         *,
         expand: typing.Optional[CandidatesRetrieveRequestExpand] = None,
         include_remote_data: typing.Optional[bool] = None,
     ) -> Candidate:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/candidates/{id}"),
-            params={"expand": expand, "include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Candidate, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -309,15 +314,15 @@
         run_async: typing.Optional[bool] = None,
         model: PatchedCandidateRequest,
         remote_user_id: str,
     ) -> CandidateResponse:
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/candidates/{id}"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model, "remote_user_id": remote_user_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CandidateResponse, _response.json())  # type: ignore
         try:
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/delete_account/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/departments/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/departments/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.department import Department
 from ...types.paginated_department_list import PaginatedDepartmentList
 
 
 class DepartmentsClient:
     def __init__(
@@ -32,25 +33,27 @@
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedDepartmentList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/departments"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedDepartmentList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -58,15 +61,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Department:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/departments/{id}"),
-            params={"include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Department, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -94,25 +97,27 @@
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedDepartmentList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/departments"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedDepartmentList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -120,15 +125,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Department:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/departments/{id}"),
-            params={"include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Department, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/eeocs/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/eeocs/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 import typing_extensions
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.eeoc import Eeoc
 from ...types.eeocs_list_request_remote_fields import EeocsListRequestRemoteFields
 from ...types.eeocs_list_request_show_enum_origins import EeocsListRequestShowEnumOrigins
 from ...types.eeocs_retrieve_request_remote_fields import EeocsRetrieveRequestRemoteFields
 from ...types.eeocs_retrieve_request_show_enum_origins import EeocsRetrieveRequestShowEnumOrigins
 from ...types.paginated_eeoc_list import PaginatedEeocList
@@ -41,29 +42,31 @@
         remote_fields: typing.Optional[EeocsListRequestRemoteFields] = None,
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[EeocsListRequestShowEnumOrigins] = None,
     ) -> PaginatedEeocList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/eeocs"),
-            params={
-                "candidate_id": candidate_id,
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "candidate_id": candidate_id,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedEeocList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -79,20 +82,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[EeocsRetrieveRequestRemoteFields] = None,
         show_enum_origins: typing.Optional[EeocsRetrieveRequestShowEnumOrigins] = None,
     ) -> Eeoc:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/eeocs/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Eeoc, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -124,29 +129,31 @@
         remote_fields: typing.Optional[EeocsListRequestRemoteFields] = None,
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[EeocsListRequestShowEnumOrigins] = None,
     ) -> PaginatedEeocList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/eeocs"),
-            params={
-                "candidate_id": candidate_id,
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "candidate_id": candidate_id,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedEeocList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -162,20 +169,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[EeocsRetrieveRequestRemoteFields] = None,
         show_enum_origins: typing.Optional[EeocsRetrieveRequestShowEnumOrigins] = None,
     ) -> Eeoc:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/eeocs/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Eeoc, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/force_resync/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/generate_key/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/interviews/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/interviews/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import pydantic
 import typing_extensions
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.interviews_list_request_expand import InterviewsListRequestExpand
 from ...types.interviews_retrieve_request_expand import InterviewsRetrieveRequestExpand
 from ...types.meta_response import MetaResponse
 from ...types.paginated_scheduled_interview_list import PaginatedScheduledInterviewList
 from ...types.scheduled_interview import ScheduledInterview
 from ...types.scheduled_interview_request import ScheduledInterviewRequest
@@ -48,31 +49,33 @@
         remote_fields: typing.Optional[typing_extensions.Literal["status"]] = None,
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["status"]] = None,
     ) -> PaginatedScheduledInterviewList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/interviews"),
-            params={
-                "application_id": application_id,
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "job_interview_stage_id": job_interview_stage_id,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "organizer_id": organizer_id,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "application_id": application_id,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "job_interview_stage_id": job_interview_stage_id,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "organizer_id": organizer_id,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedScheduledInterviewList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -87,15 +90,15 @@
         run_async: typing.Optional[bool] = None,
         model: ScheduledInterviewRequest,
         remote_user_id: str,
     ) -> ScheduledInterviewResponse:
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/interviews"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model, "remote_user_id": remote_user_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ScheduledInterviewResponse, _response.json())  # type: ignore
         try:
@@ -112,20 +115,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[typing_extensions.Literal["status"]] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["status"]] = None,
     ) -> ScheduledInterview:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/interviews/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ScheduledInterview, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -174,31 +179,33 @@
         remote_fields: typing.Optional[typing_extensions.Literal["status"]] = None,
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["status"]] = None,
     ) -> PaginatedScheduledInterviewList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/interviews"),
-            params={
-                "application_id": application_id,
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "job_interview_stage_id": job_interview_stage_id,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "organizer_id": organizer_id,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "application_id": application_id,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "job_interview_stage_id": job_interview_stage_id,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "organizer_id": organizer_id,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedScheduledInterviewList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -213,15 +220,15 @@
         run_async: typing.Optional[bool] = None,
         model: ScheduledInterviewRequest,
         remote_user_id: str,
     ) -> ScheduledInterviewResponse:
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/interviews"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model, "remote_user_id": remote_user_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ScheduledInterviewResponse, _response.json())  # type: ignore
         try:
@@ -238,20 +245,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[typing_extensions.Literal["status"]] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["status"]] = None,
     ) -> ScheduledInterview:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/interviews/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ScheduledInterview, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/issues/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/issues/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.issue import Issue
 from ...types.issues_list_request_status import IssuesListRequestStatus
 from ...types.paginated_issue_list import PaginatedIssueList
 
 
 class IssuesClient:
@@ -37,29 +38,31 @@
         page_size: typing.Optional[int] = None,
         start_date: typing.Optional[str] = None,
         status: typing.Optional[IssuesListRequestStatus] = None,
     ) -> PaginatedIssueList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/issues"),
-            params={
-                "account_token": account_token,
-                "cursor": cursor,
-                "end_date": end_date,
-                "end_user_organization_name": end_user_organization_name,
-                "first_incident_time_after": first_incident_time_after,
-                "first_incident_time_before": first_incident_time_before,
-                "include_muted": include_muted,
-                "integration_name": integration_name,
-                "last_incident_time_after": last_incident_time_after,
-                "last_incident_time_before": last_incident_time_before,
-                "page_size": page_size,
-                "start_date": start_date,
-                "status": status,
-            },
+            params=remove_none_from_dict(
+                {
+                    "account_token": account_token,
+                    "cursor": cursor,
+                    "end_date": end_date,
+                    "end_user_organization_name": end_user_organization_name,
+                    "first_incident_time_after": first_incident_time_after,
+                    "first_incident_time_before": first_incident_time_before,
+                    "include_muted": include_muted,
+                    "integration_name": integration_name,
+                    "last_incident_time_after": last_incident_time_after,
+                    "last_incident_time_before": last_incident_time_before,
+                    "page_size": page_size,
+                    "start_date": start_date,
+                    "status": status,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedIssueList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -106,29 +109,31 @@
         page_size: typing.Optional[int] = None,
         start_date: typing.Optional[str] = None,
         status: typing.Optional[IssuesListRequestStatus] = None,
     ) -> PaginatedIssueList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/issues"),
-            params={
-                "account_token": account_token,
-                "cursor": cursor,
-                "end_date": end_date,
-                "end_user_organization_name": end_user_organization_name,
-                "first_incident_time_after": first_incident_time_after,
-                "first_incident_time_before": first_incident_time_before,
-                "include_muted": include_muted,
-                "integration_name": integration_name,
-                "last_incident_time_after": last_incident_time_after,
-                "last_incident_time_before": last_incident_time_before,
-                "page_size": page_size,
-                "start_date": start_date,
-                "status": status,
-            },
+            params=remove_none_from_dict(
+                {
+                    "account_token": account_token,
+                    "cursor": cursor,
+                    "end_date": end_date,
+                    "end_user_organization_name": end_user_organization_name,
+                    "first_incident_time_after": first_incident_time_after,
+                    "first_incident_time_before": first_incident_time_before,
+                    "include_muted": include_muted,
+                    "integration_name": integration_name,
+                    "last_incident_time_after": last_incident_time_after,
+                    "last_incident_time_before": last_incident_time_before,
+                    "page_size": page_size,
+                    "start_date": start_date,
+                    "status": status,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedIssueList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/job_interview_stages/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/job_interview_stages/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 import typing_extensions
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.job_interview_stage import JobInterviewStage
 from ...types.paginated_job_interview_stage_list import PaginatedJobInterviewStageList
 
 
 class JobInterviewStagesClient:
     def __init__(
@@ -35,27 +36,29 @@
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedJobInterviewStageList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/job-interview-stages"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "job_id": job_id,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "job_id": job_id,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedJobInterviewStageList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -69,15 +72,15 @@
         *,
         expand: typing.Optional[typing_extensions.Literal["job"]] = None,
         include_remote_data: typing.Optional[bool] = None,
     ) -> JobInterviewStage:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/job-interview-stages/{id}"),
-            params={"expand": expand, "include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(JobInterviewStage, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -107,27 +110,29 @@
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedJobInterviewStageList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/job-interview-stages"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "job_id": job_id,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "job_id": job_id,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedJobInterviewStageList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -141,15 +146,15 @@
         *,
         expand: typing.Optional[typing_extensions.Literal["job"]] = None,
         include_remote_data: typing.Optional[bool] = None,
     ) -> JobInterviewStage:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/job-interview-stages/{id}"),
-            params={"expand": expand, "include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(JobInterviewStage, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/jobs/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/jobs/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 import typing_extensions
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.job import Job
 from ...types.jobs_list_request_expand import JobsListRequestExpand
 from ...types.jobs_list_request_status import JobsListRequestStatus
 from ...types.jobs_retrieve_request_expand import JobsRetrieveRequestExpand
 from ...types.paginated_job_list import PaginatedJobList
 
@@ -42,31 +43,33 @@
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["status"]] = None,
         status: typing.Optional[JobsListRequestStatus] = None,
     ) -> PaginatedJobList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/jobs"),
-            params={
-                "code": code,
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "offices": offices,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-                "status": status,
-            },
+            params=remove_none_from_dict(
+                {
+                    "code": code,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "offices": offices,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                    "status": status,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedJobList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -82,20 +85,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[typing_extensions.Literal["status"]] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["status"]] = None,
     ) -> Job:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/jobs/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Job, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -129,31 +134,33 @@
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["status"]] = None,
         status: typing.Optional[JobsListRequestStatus] = None,
     ) -> PaginatedJobList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/jobs"),
-            params={
-                "code": code,
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "offices": offices,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-                "status": status,
-            },
+            params=remove_none_from_dict(
+                {
+                    "code": code,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "offices": offices,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                    "status": status,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedJobList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -169,20 +176,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[typing_extensions.Literal["status"]] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["status"]] = None,
     ) -> Job:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/jobs/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Job, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/link_token/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/linked_accounts/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/linked_accounts/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.linked_accounts_list_request_category import LinkedAccountsListRequestCategory
 from ...types.paginated_account_details_and_actions_list import PaginatedAccountDetailsAndActionsList
 
 
 class LinkedAccountsClient:
     def __init__(
@@ -36,29 +37,31 @@
         is_test_account: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         status: typing.Optional[str] = None,
     ) -> PaginatedAccountDetailsAndActionsList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/linked-accounts"),
-            params={
-                "category": category,
-                "cursor": cursor,
-                "end_user_email_address": end_user_email_address,
-                "end_user_organization_name": end_user_organization_name,
-                "end_user_origin_id": end_user_origin_id,
-                "end_user_origin_ids": end_user_origin_ids,
-                "id": id,
-                "ids": ids,
-                "include_duplicates": include_duplicates,
-                "integration_name": integration_name,
-                "is_test_account": is_test_account,
-                "page_size": page_size,
-                "status": status,
-            },
+            params=remove_none_from_dict(
+                {
+                    "category": category,
+                    "cursor": cursor,
+                    "end_user_email_address": end_user_email_address,
+                    "end_user_organization_name": end_user_organization_name,
+                    "end_user_origin_id": end_user_origin_id,
+                    "end_user_origin_ids": end_user_origin_ids,
+                    "id": id,
+                    "ids": ids,
+                    "include_duplicates": include_duplicates,
+                    "integration_name": integration_name,
+                    "is_test_account": is_test_account,
+                    "page_size": page_size,
+                    "status": status,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedAccountDetailsAndActionsList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -90,29 +93,31 @@
         is_test_account: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         status: typing.Optional[str] = None,
     ) -> PaginatedAccountDetailsAndActionsList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/linked-accounts"),
-            params={
-                "category": category,
-                "cursor": cursor,
-                "end_user_email_address": end_user_email_address,
-                "end_user_organization_name": end_user_organization_name,
-                "end_user_origin_id": end_user_origin_id,
-                "end_user_origin_ids": end_user_origin_ids,
-                "id": id,
-                "ids": ids,
-                "include_duplicates": include_duplicates,
-                "integration_name": integration_name,
-                "is_test_account": is_test_account,
-                "page_size": page_size,
-                "status": status,
-            },
+            params=remove_none_from_dict(
+                {
+                    "category": category,
+                    "cursor": cursor,
+                    "end_user_email_address": end_user_email_address,
+                    "end_user_organization_name": end_user_organization_name,
+                    "end_user_origin_id": end_user_origin_id,
+                    "end_user_origin_ids": end_user_origin_ids,
+                    "id": id,
+                    "ids": ids,
+                    "include_duplicates": include_duplicates,
+                    "integration_name": integration_name,
+                    "is_test_account": is_test_account,
+                    "page_size": page_size,
+                    "status": status,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedAccountDetailsAndActionsList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/offers/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/locations/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,182 +5,173 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 import typing_extensions
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
-from ...types.offer import Offer
-from ...types.offers_list_request_expand import OffersListRequestExpand
-from ...types.offers_retrieve_request_expand import OffersRetrieveRequestExpand
-from ...types.paginated_offer_list import PaginatedOfferList
+from ...types.location import Location
+from ...types.paginated_location_list import PaginatedLocationList
 
 
-class OffersClient:
+class LocationsClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def list(
         self,
         *,
-        application_id: typing.Optional[str] = None,
         created_after: typing.Optional[str] = None,
         created_before: typing.Optional[str] = None,
-        creator_id: typing.Optional[str] = None,
         cursor: typing.Optional[str] = None,
-        expand: typing.Optional[OffersListRequestExpand] = None,
         include_deleted_data: typing.Optional[bool] = None,
         include_remote_data: typing.Optional[bool] = None,
         modified_after: typing.Optional[str] = None,
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
-        remote_fields: typing.Optional[typing_extensions.Literal["status"]] = None,
+        remote_fields: typing.Optional[typing_extensions.Literal["location_type"]] = None,
         remote_id: typing.Optional[str] = None,
-        show_enum_origins: typing.Optional[typing_extensions.Literal["status"]] = None,
-    ) -> PaginatedOfferList:
+        show_enum_origins: typing.Optional[typing_extensions.Literal["location_type"]] = None,
+    ) -> PaginatedLocationList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/offers"),
-            params={
-                "application_id": application_id,
-                "created_after": created_after,
-                "created_before": created_before,
-                "creator_id": creator_id,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/locations"),
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaginatedOfferList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaginatedLocationList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def retrieve(
         self,
         id: str,
         *,
-        expand: typing.Optional[OffersRetrieveRequestExpand] = None,
         include_remote_data: typing.Optional[bool] = None,
-        remote_fields: typing.Optional[typing_extensions.Literal["status"]] = None,
-        show_enum_origins: typing.Optional[typing_extensions.Literal["status"]] = None,
-    ) -> Offer:
+        remote_fields: typing.Optional[typing_extensions.Literal["location_type"]] = None,
+        show_enum_origins: typing.Optional[typing_extensions.Literal["location_type"]] = None,
+    ) -> Location:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/offers/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/locations/{id}"),
+            params=remove_none_from_dict(
+                {
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Offer, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Location, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncOffersClient:
+class AsyncLocationsClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def list(
         self,
         *,
-        application_id: typing.Optional[str] = None,
         created_after: typing.Optional[str] = None,
         created_before: typing.Optional[str] = None,
-        creator_id: typing.Optional[str] = None,
         cursor: typing.Optional[str] = None,
-        expand: typing.Optional[OffersListRequestExpand] = None,
         include_deleted_data: typing.Optional[bool] = None,
         include_remote_data: typing.Optional[bool] = None,
         modified_after: typing.Optional[str] = None,
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
-        remote_fields: typing.Optional[typing_extensions.Literal["status"]] = None,
+        remote_fields: typing.Optional[typing_extensions.Literal["location_type"]] = None,
         remote_id: typing.Optional[str] = None,
-        show_enum_origins: typing.Optional[typing_extensions.Literal["status"]] = None,
-    ) -> PaginatedOfferList:
+        show_enum_origins: typing.Optional[typing_extensions.Literal["location_type"]] = None,
+    ) -> PaginatedLocationList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/offers"),
-            params={
-                "application_id": application_id,
-                "created_after": created_after,
-                "created_before": created_before,
-                "creator_id": creator_id,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/locations"),
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaginatedOfferList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaginatedLocationList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def retrieve(
         self,
         id: str,
         *,
-        expand: typing.Optional[OffersRetrieveRequestExpand] = None,
         include_remote_data: typing.Optional[bool] = None,
-        remote_fields: typing.Optional[typing_extensions.Literal["status"]] = None,
-        show_enum_origins: typing.Optional[typing_extensions.Literal["status"]] = None,
-    ) -> Offer:
+        remote_fields: typing.Optional[typing_extensions.Literal["location_type"]] = None,
+        show_enum_origins: typing.Optional[typing_extensions.Literal["location_type"]] = None,
+    ) -> Location:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/offers/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/locations/{id}"),
+            params=remove_none_from_dict(
+                {
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Offer, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Location, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/offices/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/offices/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.office import Office
 from ...types.paginated_office_list import PaginatedOfficeList
 
 
 class OfficesClient:
     def __init__(
@@ -32,25 +33,27 @@
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedOfficeList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/offices"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedOfficeList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -58,15 +61,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Office:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/offices/{id}"),
-            params={"include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Office, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -94,25 +97,27 @@
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedOfficeList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/offices"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedOfficeList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -120,15 +125,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Office:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/offices/{id}"),
-            params={"include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Office, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/passthrough/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/regenerate_key/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/reject_reasons/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/reject_reasons/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.paginated_reject_reason_list import PaginatedRejectReasonList
 from ...types.reject_reason import RejectReason
 
 
 class RejectReasonsClient:
     def __init__(
@@ -32,25 +33,27 @@
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedRejectReasonList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/reject-reasons"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedRejectReasonList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -58,15 +61,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> RejectReason:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/reject-reasons/{id}"),
-            params={"include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RejectReason, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -94,25 +97,27 @@
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedRejectReasonList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/reject-reasons"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedRejectReasonList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -120,15 +125,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> RejectReason:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/reject-reasons/{id}"),
-            params={"include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RejectReason, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/scorecards/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/scorecards/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 import typing_extensions
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.paginated_scorecard_list import PaginatedScorecardList
 from ...types.scorecard import Scorecard
 from ...types.scorecards_list_request_expand import ScorecardsListRequestExpand
 from ...types.scorecards_retrieve_request_expand import ScorecardsRetrieveRequestExpand
 
 
@@ -41,31 +42,33 @@
         remote_fields: typing.Optional[typing_extensions.Literal["overall_recommendation"]] = None,
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["overall_recommendation"]] = None,
     ) -> PaginatedScorecardList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/scorecards"),
-            params={
-                "application_id": application_id,
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "interview_id": interview_id,
-                "interviewer_id": interviewer_id,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "application_id": application_id,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "interview_id": interview_id,
+                    "interviewer_id": interviewer_id,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedScorecardList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -81,20 +84,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[typing_extensions.Literal["overall_recommendation"]] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["overall_recommendation"]] = None,
     ) -> Scorecard:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/scorecards/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Scorecard, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -128,31 +133,33 @@
         remote_fields: typing.Optional[typing_extensions.Literal["overall_recommendation"]] = None,
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["overall_recommendation"]] = None,
     ) -> PaginatedScorecardList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/scorecards"),
-            params={
-                "application_id": application_id,
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "interview_id": interview_id,
-                "interviewer_id": interviewer_id,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "application_id": application_id,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "interview_id": interview_id,
+                    "interviewer_id": interviewer_id,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedScorecardList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -168,20 +175,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[typing_extensions.Literal["overall_recommendation"]] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["overall_recommendation"]] = None,
     ) -> Scorecard:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/scorecards/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Scorecard, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/selective_sync/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/selective_sync/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.linked_account_selective_sync_configuration import LinkedAccountSelectiveSyncConfiguration
 from ...types.linked_account_selective_sync_configuration_request import LinkedAccountSelectiveSyncConfigurationRequest
 from ...types.paginated_condition_schema_list import PaginatedConditionSchemaList
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
@@ -24,15 +25,15 @@
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def configurations_list(self) -> typing.List[LinkedAccountSelectiveSyncConfiguration]:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/selective-sync/configurations"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -41,15 +42,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def configurations_update(
         self, *, sync_configurations: typing.List[LinkedAccountSelectiveSyncConfigurationRequest]
     ) -> typing.List[LinkedAccountSelectiveSyncConfiguration]:
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/selective-sync/configurations"),
             json=jsonable_encoder({"sync_configurations": sync_configurations}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
@@ -63,16 +64,16 @@
         *,
         common_model: typing.Optional[str] = None,
         cursor: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
     ) -> PaginatedConditionSchemaList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/selective-sync/meta"),
-            params={"common_model": common_model, "cursor": cursor, "page_size": page_size},
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/selective-sync/meta"),
+            params=remove_none_from_dict({"common_model": common_model, "cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedConditionSchemaList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -87,15 +88,15 @@
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def configurations_list(self) -> typing.List[LinkedAccountSelectiveSyncConfiguration]:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/selective-sync/configurations"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -104,15 +105,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def configurations_update(
         self, *, sync_configurations: typing.List[LinkedAccountSelectiveSyncConfigurationRequest]
     ) -> typing.List[LinkedAccountSelectiveSyncConfiguration]:
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/selective-sync/configurations"),
             json=jsonable_encoder({"sync_configurations": sync_configurations}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
@@ -126,16 +127,16 @@
         *,
         common_model: typing.Optional[str] = None,
         cursor: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
     ) -> PaginatedConditionSchemaList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/selective-sync/meta"),
-            params={"common_model": common_model, "cursor": cursor, "page_size": page_size},
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/selective-sync/meta"),
+            params=remove_none_from_dict({"common_model": common_model, "cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedConditionSchemaList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/sync_status/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/sync_status/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.paginated_sync_status_list import PaginatedSyncStatusList
 
 
 class SyncStatusClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
@@ -20,16 +21,16 @@
         self._client_wrapper = client_wrapper
 
     def list(
         self, *, cursor: typing.Optional[str] = None, page_size: typing.Optional[int] = None
     ) -> PaginatedSyncStatusList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/sync-status"),
-            params={"cursor": cursor, "page_size": page_size},
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/sync-status"),
+            params=remove_none_from_dict({"cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedSyncStatusList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -46,16 +47,16 @@
         self._client_wrapper = client_wrapper
 
     async def list(
         self, *, cursor: typing.Optional[str] = None, page_size: typing.Optional[int] = None
     ) -> PaginatedSyncStatusList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/sync-status"),
-            params={"cursor": cursor, "page_size": page_size},
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/sync-status"),
+            params=remove_none_from_dict({"cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedSyncStatusList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/tags/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/tags/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.paginated_tag_list import PaginatedTagList
 
 
 class TagsClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
@@ -31,25 +32,27 @@
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedTagList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/tags"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedTagList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -77,25 +80,27 @@
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedTagList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/tags"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedTagList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/users/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/users/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 import typing_extensions
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.paginated_remote_user_list import PaginatedRemoteUserList
 from ...types.remote_user import RemoteUser
 
 
 class UsersClient:
     def __init__(
@@ -36,28 +37,30 @@
         remote_fields: typing.Optional[typing_extensions.Literal["access_role"]] = None,
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["access_role"]] = None,
     ) -> PaginatedRemoteUserList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/users"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "email": email,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "email": email,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedRemoteUserList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -72,19 +75,21 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[typing_extensions.Literal["access_role"]] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["access_role"]] = None,
     ) -> RemoteUser:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/users/{id}"),
-            params={
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteUser, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -115,28 +120,30 @@
         remote_fields: typing.Optional[typing_extensions.Literal["access_role"]] = None,
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["access_role"]] = None,
     ) -> PaginatedRemoteUserList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/users"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "email": email,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "email": email,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedRemoteUserList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -151,19 +158,21 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[typing_extensions.Literal["access_role"]] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["access_role"]] = None,
     ) -> RemoteUser:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/users/{id}"),
-            params={
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RemoteUser, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/resources/webhook_receivers/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/__init__.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/access_role_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/access_role_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/account_details.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/account_details.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/account_details_and_actions.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/account_details_and_actions_integration.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/account_details_and_actions_status_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/account_integration.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/account_token.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/account_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/activities_list_request_remote_fields.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/activities_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/activity.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/activity.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/activity_request.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/activity_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/activity_response.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/activity_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/activity_type_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/activity_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/application.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/application.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/application_request.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/application_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/application_response.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/application_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/applications_list_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/applications_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/applications_retrieve_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/applications_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/attachment.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/attachment.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/attachment_request.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/attachment_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/attachment_response.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/attachment_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/attachment_type_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/attachment_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/available_actions.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/candidate.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/candidate.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/candidate_request.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/candidate_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/candidate_response.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/candidate_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/candidates_list_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/candidates_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/candidates_retrieve_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/candidates_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/categories_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/category_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/common_model_scopes_body_request.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/condition_schema.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/condition_type_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/debug_mode_log.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/debug_model_log_summary.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/department.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/department.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/disability_status_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/disability_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/eeoc.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/eeoc.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/email_address.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/email_address.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/email_address_request.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/email_address_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/email_address_type_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/email_address_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/enabled_actions_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/encoding_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/error_validation_problem.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/gender_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/gender_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/interviews_list_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/interviews_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/interviews_retrieve_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/interviews_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/issue.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/issue.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/issue_status_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/job.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/job.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/job_interview_stage.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/job_interview_stage.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/job_status_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/job_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/jobs_list_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/jobs_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/jobs_list_request_status.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/jobs_list_request_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/jobs_retrieve_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/jobs_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/link_token.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/link_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/linked_account_condition.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/linked_account_condition_request.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/linked_account_status.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/linked_accounts_list_request_category.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/meta_response.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/method_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/model_operation.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/multipart_form_field_request.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/offer.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/offer.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/offer_status_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/offer_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/offers_list_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/offers_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/offers_retrieve_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/offers_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/office.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/office.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/operator_schema.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/overall_recommendation_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/overall_recommendation_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_activity_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_activity_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_application_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_application_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_attachment_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_attachment_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_candidate_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_candidate_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_condition_schema_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_department_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_department_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_eeoc_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_eeoc_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_issue_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_job_interview_stage_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_job_interview_stage_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_job_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_job_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_offer_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_offer_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_office_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_office_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_reject_reason_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_reject_reason_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_remote_user_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_remote_user_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_scheduled_interview_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_scheduled_interview_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_scorecard_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_scorecard_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_sync_status_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/paginated_tag_list.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/paginated_tag_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/patched_candidate_request.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/patched_candidate_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/phone_number.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/phone_number_request.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/phone_number_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/phone_number_type_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/phone_number_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/race_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/race_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/reason_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/reason_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/reject_reason.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/reject_reason.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/remote_data.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/remote_key.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/remote_response.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/remote_user.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/remote_user.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/request_format_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/response_type_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/scheduled_interview.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/scheduled_interview.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/scheduled_interview_request.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/scheduled_interview_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/scheduled_interview_response.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/scheduled_interview_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/scheduled_interview_status_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/scheduled_interview_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/scorecard.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/scorecard.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/scorecards_list_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/scorecards_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/sync_status.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/sync_status_status_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/tag.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/tag.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/url.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/url.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/url_request.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/url_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/url_type_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/url_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/validation_problem_source.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/veteran_status_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/veteran_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/visibility_enum.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/visibility_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/warning_validation_problem.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/ats/types/webhook_receiver.py` & `fern_merge-0.0.32/src/merge/resources/ats/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/__init__.py` & `fern_merge-0.0.32/src/merge/resources/hris/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/__init__.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/account_details/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/account_token/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/available_actions/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/bank_info/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/bank_info/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 import typing_extensions
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.bank_info import BankInfo
 from ...types.bank_info_list_request_account_type import BankInfoListRequestAccountType
 from ...types.bank_info_list_request_order_by import BankInfoListRequestOrderBy
 from ...types.paginated_bank_info_list import PaginatedBankInfoList
 
 
@@ -42,32 +43,34 @@
         remote_fields: typing.Optional[typing_extensions.Literal["account_type"]] = None,
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["account_type"]] = None,
     ) -> PaginatedBankInfoList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/bank-info"),
-            params={
-                "account_type": account_type,
-                "bank_name": bank_name,
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "employee_id": employee_id,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "order_by": order_by,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "account_type": account_type,
+                    "bank_name": bank_name,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "employee_id": employee_id,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "order_by": order_by,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedBankInfoList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -83,20 +86,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[typing_extensions.Literal["account_type"]] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["account_type"]] = None,
     ) -> BankInfo:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/bank-info/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BankInfo, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -131,32 +136,34 @@
         remote_fields: typing.Optional[typing_extensions.Literal["account_type"]] = None,
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["account_type"]] = None,
     ) -> PaginatedBankInfoList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/bank-info"),
-            params={
-                "account_type": account_type,
-                "bank_name": bank_name,
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "employee_id": employee_id,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "order_by": order_by,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "account_type": account_type,
+                    "bank_name": bank_name,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "employee_id": employee_id,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "order_by": order_by,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedBankInfoList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -172,20 +179,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[typing_extensions.Literal["account_type"]] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["account_type"]] = None,
     ) -> BankInfo:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/bank-info/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BankInfo, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/benefits/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/benefits/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 import typing_extensions
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.benefit import Benefit
 from ...types.paginated_benefit_list import PaginatedBenefitList
 
 
 class BenefitsClient:
     def __init__(
@@ -35,27 +36,29 @@
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedBenefitList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/benefits"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "employee_id": employee_id,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "employee_id": employee_id,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedBenefitList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -69,15 +72,15 @@
         *,
         expand: typing.Optional[typing_extensions.Literal["employee"]] = None,
         include_remote_data: typing.Optional[bool] = None,
     ) -> Benefit:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/benefits/{id}"),
-            params={"expand": expand, "include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Benefit, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -107,27 +110,29 @@
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedBenefitList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/benefits"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "employee_id": employee_id,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "employee_id": employee_id,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedBenefitList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -141,15 +146,15 @@
         *,
         expand: typing.Optional[typing_extensions.Literal["employee"]] = None,
         include_remote_data: typing.Optional[bool] = None,
     ) -> Benefit:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/benefits/{id}"),
-            params={"expand": expand, "include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Benefit, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/companies/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/companies/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.company import Company
 from ...types.paginated_company_list import PaginatedCompanyList
 
 
 class CompaniesClient:
     def __init__(
@@ -32,25 +33,27 @@
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedCompanyList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/companies"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedCompanyList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -58,15 +61,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Company:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/companies/{id}"),
-            params={"include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -94,25 +97,27 @@
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedCompanyList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/companies"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedCompanyList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -120,15 +125,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> Company:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/companies/{id}"),
-            params={"include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/delete_account/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/employee_payroll_runs/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/employee_payroll_runs/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.employee_payroll_run import EmployeePayrollRun
 from ...types.employee_payroll_runs_list_request_expand import EmployeePayrollRunsListRequestExpand
 from ...types.employee_payroll_runs_retrieve_request_expand import EmployeePayrollRunsRetrieveRequestExpand
 from ...types.paginated_employee_payroll_run_list import PaginatedEmployeePayrollRunList
 
 
@@ -41,32 +42,34 @@
         remote_id: typing.Optional[str] = None,
         started_after: typing.Optional[str] = None,
         started_before: typing.Optional[str] = None,
     ) -> PaginatedEmployeePayrollRunList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/employee-payroll-runs"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "employee_id": employee_id,
-                "ended_after": ended_after,
-                "ended_before": ended_before,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "payroll_run_id": payroll_run_id,
-                "remote_id": remote_id,
-                "started_after": started_after,
-                "started_before": started_before,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "employee_id": employee_id,
+                    "ended_after": ended_after,
+                    "ended_before": ended_before,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "payroll_run_id": payroll_run_id,
+                    "remote_id": remote_id,
+                    "started_after": started_after,
+                    "started_before": started_before,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedEmployeePayrollRunList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -80,15 +83,15 @@
         *,
         expand: typing.Optional[EmployeePayrollRunsRetrieveRequestExpand] = None,
         include_remote_data: typing.Optional[bool] = None,
     ) -> EmployeePayrollRun:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/employee-payroll-runs/{id}"),
-            params={"expand": expand, "include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EmployeePayrollRun, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -123,32 +126,34 @@
         remote_id: typing.Optional[str] = None,
         started_after: typing.Optional[str] = None,
         started_before: typing.Optional[str] = None,
     ) -> PaginatedEmployeePayrollRunList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/employee-payroll-runs"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "employee_id": employee_id,
-                "ended_after": ended_after,
-                "ended_before": ended_before,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "payroll_run_id": payroll_run_id,
-                "remote_id": remote_id,
-                "started_after": started_after,
-                "started_before": started_before,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "employee_id": employee_id,
+                    "ended_after": ended_after,
+                    "ended_before": ended_before,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "payroll_run_id": payroll_run_id,
+                    "remote_id": remote_id,
+                    "started_after": started_after,
+                    "started_before": started_before,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedEmployeePayrollRunList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -162,15 +167,15 @@
         *,
         expand: typing.Optional[EmployeePayrollRunsRetrieveRequestExpand] = None,
         include_remote_data: typing.Optional[bool] = None,
     ) -> EmployeePayrollRun:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/employee-payroll-runs/{id}"),
-            params={"expand": expand, "include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EmployeePayrollRun, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/employees/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/employees/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.employee import Employee
 from ...types.employee_request import EmployeeRequest
 from ...types.employee_response import EmployeeResponse
 from ...types.employees_list_request_employment_status import EmployeesListRequestEmploymentStatus
 from ...types.employees_list_request_expand import EmployeesListRequestExpand
 from ...types.employees_list_request_remote_fields import EmployeesListRequestRemoteFields
@@ -67,45 +68,47 @@
         terminated_before: typing.Optional[str] = None,
         work_email: typing.Optional[str] = None,
         work_location_id: typing.Optional[str] = None,
     ) -> PaginatedEmployeeList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/employees"),
-            params={
-                "company_id": company_id,
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "display_full_name": display_full_name,
-                "employment_status": employment_status,
-                "expand": expand,
-                "first_name": first_name,
-                "groups": groups,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "include_sensitive_fields": include_sensitive_fields,
-                "last_name": last_name,
-                "manager_id": manager_id,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "pay_group_id": pay_group_id,
-                "personal_email": personal_email,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-                "started_after": started_after,
-                "started_before": started_before,
-                "team_id": team_id,
-                "terminated_after": terminated_after,
-                "terminated_before": terminated_before,
-                "work_email": work_email,
-                "work_location_id": work_location_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "company_id": company_id,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "display_full_name": display_full_name,
+                    "employment_status": employment_status,
+                    "expand": expand,
+                    "first_name": first_name,
+                    "groups": groups,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "include_sensitive_fields": include_sensitive_fields,
+                    "last_name": last_name,
+                    "manager_id": manager_id,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "pay_group_id": pay_group_id,
+                    "personal_email": personal_email,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                    "started_after": started_after,
+                    "started_before": started_before,
+                    "team_id": team_id,
+                    "terminated_after": terminated_after,
+                    "terminated_before": terminated_before,
+                    "work_email": work_email,
+                    "work_location_id": work_location_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedEmployeeList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -119,15 +122,15 @@
         is_debug_mode: typing.Optional[bool] = None,
         run_async: typing.Optional[bool] = None,
         model: EmployeeRequest,
     ) -> EmployeeResponse:
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/employees"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EmployeeResponse, _response.json())  # type: ignore
         try:
@@ -145,21 +148,23 @@
         include_sensitive_fields: typing.Optional[bool] = None,
         remote_fields: typing.Optional[EmployeesRetrieveRequestRemoteFields] = None,
         show_enum_origins: typing.Optional[EmployeesRetrieveRequestShowEnumOrigins] = None,
     ) -> Employee:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/employees/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "include_sensitive_fields": include_sensitive_fields,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "include_sensitive_fields": include_sensitive_fields,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Employee, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -243,45 +248,47 @@
         terminated_before: typing.Optional[str] = None,
         work_email: typing.Optional[str] = None,
         work_location_id: typing.Optional[str] = None,
     ) -> PaginatedEmployeeList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/employees"),
-            params={
-                "company_id": company_id,
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "display_full_name": display_full_name,
-                "employment_status": employment_status,
-                "expand": expand,
-                "first_name": first_name,
-                "groups": groups,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "include_sensitive_fields": include_sensitive_fields,
-                "last_name": last_name,
-                "manager_id": manager_id,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "pay_group_id": pay_group_id,
-                "personal_email": personal_email,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-                "started_after": started_after,
-                "started_before": started_before,
-                "team_id": team_id,
-                "terminated_after": terminated_after,
-                "terminated_before": terminated_before,
-                "work_email": work_email,
-                "work_location_id": work_location_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "company_id": company_id,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "display_full_name": display_full_name,
+                    "employment_status": employment_status,
+                    "expand": expand,
+                    "first_name": first_name,
+                    "groups": groups,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "include_sensitive_fields": include_sensitive_fields,
+                    "last_name": last_name,
+                    "manager_id": manager_id,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "pay_group_id": pay_group_id,
+                    "personal_email": personal_email,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                    "started_after": started_after,
+                    "started_before": started_before,
+                    "team_id": team_id,
+                    "terminated_after": terminated_after,
+                    "terminated_before": terminated_before,
+                    "work_email": work_email,
+                    "work_location_id": work_location_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedEmployeeList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -295,15 +302,15 @@
         is_debug_mode: typing.Optional[bool] = None,
         run_async: typing.Optional[bool] = None,
         model: EmployeeRequest,
     ) -> EmployeeResponse:
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/employees"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EmployeeResponse, _response.json())  # type: ignore
         try:
@@ -321,21 +328,23 @@
         include_sensitive_fields: typing.Optional[bool] = None,
         remote_fields: typing.Optional[EmployeesRetrieveRequestRemoteFields] = None,
         show_enum_origins: typing.Optional[EmployeesRetrieveRequestShowEnumOrigins] = None,
     ) -> Employee:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/employees/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "include_sensitive_fields": include_sensitive_fields,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "include_sensitive_fields": include_sensitive_fields,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Employee, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/employments/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/employments/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.employment import Employment
 from ...types.employments_list_request_expand import EmploymentsListRequestExpand
 from ...types.employments_list_request_order_by import EmploymentsListRequestOrderBy
 from ...types.employments_list_request_remote_fields import EmploymentsListRequestRemoteFields
 from ...types.employments_list_request_show_enum_origins import EmploymentsListRequestShowEnumOrigins
 from ...types.employments_retrieve_request_expand import EmploymentsRetrieveRequestExpand
@@ -44,30 +45,32 @@
         remote_fields: typing.Optional[EmploymentsListRequestRemoteFields] = None,
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[EmploymentsListRequestShowEnumOrigins] = None,
     ) -> PaginatedEmploymentList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/employments"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "employee_id": employee_id,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "order_by": order_by,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "employee_id": employee_id,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "order_by": order_by,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedEmploymentList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -83,20 +86,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[EmploymentsRetrieveRequestRemoteFields] = None,
         show_enum_origins: typing.Optional[EmploymentsRetrieveRequestShowEnumOrigins] = None,
     ) -> Employment:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/employments/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Employment, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -129,30 +134,32 @@
         remote_fields: typing.Optional[EmploymentsListRequestRemoteFields] = None,
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[EmploymentsListRequestShowEnumOrigins] = None,
     ) -> PaginatedEmploymentList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/employments"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "employee_id": employee_id,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "order_by": order_by,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "employee_id": employee_id,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "order_by": order_by,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedEmploymentList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -168,20 +175,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[EmploymentsRetrieveRequestRemoteFields] = None,
         show_enum_origins: typing.Optional[EmploymentsRetrieveRequestShowEnumOrigins] = None,
     ) -> Employment:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/employments/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Employment, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/force_resync/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/generate_key/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/groups/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/groups/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 import typing_extensions
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.group import Group
 from ...types.paginated_group_list import PaginatedGroupList
 
 
 class GroupsClient:
     def __init__(
@@ -36,28 +37,30 @@
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["type"]] = None,
         types: typing.Optional[str] = None,
     ) -> PaginatedGroupList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/groups"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-                "types": types,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                    "types": types,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedGroupList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -72,19 +75,21 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[typing_extensions.Literal["type"]] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["type"]] = None,
     ) -> Group:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/groups/{id}"),
-            params={
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Group, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -115,28 +120,30 @@
         remote_id: typing.Optional[str] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["type"]] = None,
         types: typing.Optional[str] = None,
     ) -> PaginatedGroupList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/groups"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-                "types": types,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                    "types": types,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedGroupList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -151,19 +158,21 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[typing_extensions.Literal["type"]] = None,
         show_enum_origins: typing.Optional[typing_extensions.Literal["type"]] = None,
     ) -> Group:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/groups/{id}"),
-            params={
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Group, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/issues/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/issues/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.issue import Issue
 from ...types.issues_list_request_status import IssuesListRequestStatus
 from ...types.paginated_issue_list import PaginatedIssueList
 
 
 class IssuesClient:
@@ -37,29 +38,31 @@
         page_size: typing.Optional[int] = None,
         start_date: typing.Optional[str] = None,
         status: typing.Optional[IssuesListRequestStatus] = None,
     ) -> PaginatedIssueList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/issues"),
-            params={
-                "account_token": account_token,
-                "cursor": cursor,
-                "end_date": end_date,
-                "end_user_organization_name": end_user_organization_name,
-                "first_incident_time_after": first_incident_time_after,
-                "first_incident_time_before": first_incident_time_before,
-                "include_muted": include_muted,
-                "integration_name": integration_name,
-                "last_incident_time_after": last_incident_time_after,
-                "last_incident_time_before": last_incident_time_before,
-                "page_size": page_size,
-                "start_date": start_date,
-                "status": status,
-            },
+            params=remove_none_from_dict(
+                {
+                    "account_token": account_token,
+                    "cursor": cursor,
+                    "end_date": end_date,
+                    "end_user_organization_name": end_user_organization_name,
+                    "first_incident_time_after": first_incident_time_after,
+                    "first_incident_time_before": first_incident_time_before,
+                    "include_muted": include_muted,
+                    "integration_name": integration_name,
+                    "last_incident_time_after": last_incident_time_after,
+                    "last_incident_time_before": last_incident_time_before,
+                    "page_size": page_size,
+                    "start_date": start_date,
+                    "status": status,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedIssueList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -106,29 +109,31 @@
         page_size: typing.Optional[int] = None,
         start_date: typing.Optional[str] = None,
         status: typing.Optional[IssuesListRequestStatus] = None,
     ) -> PaginatedIssueList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/issues"),
-            params={
-                "account_token": account_token,
-                "cursor": cursor,
-                "end_date": end_date,
-                "end_user_organization_name": end_user_organization_name,
-                "first_incident_time_after": first_incident_time_after,
-                "first_incident_time_before": first_incident_time_before,
-                "include_muted": include_muted,
-                "integration_name": integration_name,
-                "last_incident_time_after": last_incident_time_after,
-                "last_incident_time_before": last_incident_time_before,
-                "page_size": page_size,
-                "start_date": start_date,
-                "status": status,
-            },
+            params=remove_none_from_dict(
+                {
+                    "account_token": account_token,
+                    "cursor": cursor,
+                    "end_date": end_date,
+                    "end_user_organization_name": end_user_organization_name,
+                    "first_incident_time_after": first_incident_time_after,
+                    "first_incident_time_before": first_incident_time_before,
+                    "include_muted": include_muted,
+                    "integration_name": integration_name,
+                    "last_incident_time_after": last_incident_time_after,
+                    "last_incident_time_before": last_incident_time_before,
+                    "page_size": page_size,
+                    "start_date": start_date,
+                    "status": status,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedIssueList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/link_token/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/linked_accounts/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/linked_accounts/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.linked_accounts_list_request_category import LinkedAccountsListRequestCategory
 from ...types.paginated_account_details_and_actions_list import PaginatedAccountDetailsAndActionsList
 
 
 class LinkedAccountsClient:
     def __init__(
@@ -36,29 +37,31 @@
         is_test_account: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         status: typing.Optional[str] = None,
     ) -> PaginatedAccountDetailsAndActionsList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/linked-accounts"),
-            params={
-                "category": category,
-                "cursor": cursor,
-                "end_user_email_address": end_user_email_address,
-                "end_user_organization_name": end_user_organization_name,
-                "end_user_origin_id": end_user_origin_id,
-                "end_user_origin_ids": end_user_origin_ids,
-                "id": id,
-                "ids": ids,
-                "include_duplicates": include_duplicates,
-                "integration_name": integration_name,
-                "is_test_account": is_test_account,
-                "page_size": page_size,
-                "status": status,
-            },
+            params=remove_none_from_dict(
+                {
+                    "category": category,
+                    "cursor": cursor,
+                    "end_user_email_address": end_user_email_address,
+                    "end_user_organization_name": end_user_organization_name,
+                    "end_user_origin_id": end_user_origin_id,
+                    "end_user_origin_ids": end_user_origin_ids,
+                    "id": id,
+                    "ids": ids,
+                    "include_duplicates": include_duplicates,
+                    "integration_name": integration_name,
+                    "is_test_account": is_test_account,
+                    "page_size": page_size,
+                    "status": status,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedAccountDetailsAndActionsList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -90,29 +93,31 @@
         is_test_account: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         status: typing.Optional[str] = None,
     ) -> PaginatedAccountDetailsAndActionsList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/linked-accounts"),
-            params={
-                "category": category,
-                "cursor": cursor,
-                "end_user_email_address": end_user_email_address,
-                "end_user_organization_name": end_user_organization_name,
-                "end_user_origin_id": end_user_origin_id,
-                "end_user_origin_ids": end_user_origin_ids,
-                "id": id,
-                "ids": ids,
-                "include_duplicates": include_duplicates,
-                "integration_name": integration_name,
-                "is_test_account": is_test_account,
-                "page_size": page_size,
-                "status": status,
-            },
+            params=remove_none_from_dict(
+                {
+                    "category": category,
+                    "cursor": cursor,
+                    "end_user_email_address": end_user_email_address,
+                    "end_user_organization_name": end_user_organization_name,
+                    "end_user_origin_id": end_user_origin_id,
+                    "end_user_origin_ids": end_user_origin_ids,
+                    "id": id,
+                    "ids": ids,
+                    "include_duplicates": include_duplicates,
+                    "integration_name": integration_name,
+                    "is_test_account": is_test_account,
+                    "page_size": page_size,
+                    "status": status,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedAccountDetailsAndActionsList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/locations/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/time_off_balances/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,164 +5,190 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 import typing_extensions
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
-from ...types.location import Location
-from ...types.paginated_location_list import PaginatedLocationList
+from ...types.paginated_time_off_balance_list import PaginatedTimeOffBalanceList
+from ...types.time_off_balance import TimeOffBalance
+from ...types.time_off_balances_list_request_policy_type import TimeOffBalancesListRequestPolicyType
 
 
-class LocationsClient:
+class TimeOffBalancesClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def list(
         self,
         *,
         created_after: typing.Optional[str] = None,
         created_before: typing.Optional[str] = None,
         cursor: typing.Optional[str] = None,
+        employee_id: typing.Optional[str] = None,
+        expand: typing.Optional[typing_extensions.Literal["employee"]] = None,
         include_deleted_data: typing.Optional[bool] = None,
         include_remote_data: typing.Optional[bool] = None,
         modified_after: typing.Optional[str] = None,
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
-        remote_fields: typing.Optional[typing_extensions.Literal["location_type"]] = None,
+        policy_type: typing.Optional[TimeOffBalancesListRequestPolicyType] = None,
+        remote_fields: typing.Optional[typing_extensions.Literal["policy_type"]] = None,
         remote_id: typing.Optional[str] = None,
-        show_enum_origins: typing.Optional[typing_extensions.Literal["location_type"]] = None,
-    ) -> PaginatedLocationList:
+        show_enum_origins: typing.Optional[typing_extensions.Literal["policy_type"]] = None,
+    ) -> PaginatedTimeOffBalanceList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/locations"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/time-off-balances"),
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "employee_id": employee_id,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "policy_type": policy_type,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaginatedLocationList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaginatedTimeOffBalanceList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def retrieve(
         self,
         id: str,
         *,
+        expand: typing.Optional[typing_extensions.Literal["employee"]] = None,
         include_remote_data: typing.Optional[bool] = None,
-        remote_fields: typing.Optional[typing_extensions.Literal["location_type"]] = None,
-        show_enum_origins: typing.Optional[typing_extensions.Literal["location_type"]] = None,
-    ) -> Location:
+        remote_fields: typing.Optional[typing_extensions.Literal["policy_type"]] = None,
+        show_enum_origins: typing.Optional[typing_extensions.Literal["policy_type"]] = None,
+    ) -> TimeOffBalance:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/locations/{id}"),
-            params={
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/time-off-balances/{id}"),
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Location, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TimeOffBalance, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncLocationsClient:
+class AsyncTimeOffBalancesClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def list(
         self,
         *,
         created_after: typing.Optional[str] = None,
         created_before: typing.Optional[str] = None,
         cursor: typing.Optional[str] = None,
+        employee_id: typing.Optional[str] = None,
+        expand: typing.Optional[typing_extensions.Literal["employee"]] = None,
         include_deleted_data: typing.Optional[bool] = None,
         include_remote_data: typing.Optional[bool] = None,
         modified_after: typing.Optional[str] = None,
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
-        remote_fields: typing.Optional[typing_extensions.Literal["location_type"]] = None,
+        policy_type: typing.Optional[TimeOffBalancesListRequestPolicyType] = None,
+        remote_fields: typing.Optional[typing_extensions.Literal["policy_type"]] = None,
         remote_id: typing.Optional[str] = None,
-        show_enum_origins: typing.Optional[typing_extensions.Literal["location_type"]] = None,
-    ) -> PaginatedLocationList:
+        show_enum_origins: typing.Optional[typing_extensions.Literal["policy_type"]] = None,
+    ) -> PaginatedTimeOffBalanceList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/locations"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/time-off-balances"),
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "employee_id": employee_id,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "policy_type": policy_type,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaginatedLocationList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaginatedTimeOffBalanceList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def retrieve(
         self,
         id: str,
         *,
+        expand: typing.Optional[typing_extensions.Literal["employee"]] = None,
         include_remote_data: typing.Optional[bool] = None,
-        remote_fields: typing.Optional[typing_extensions.Literal["location_type"]] = None,
-        show_enum_origins: typing.Optional[typing_extensions.Literal["location_type"]] = None,
-    ) -> Location:
+        remote_fields: typing.Optional[typing_extensions.Literal["policy_type"]] = None,
+        show_enum_origins: typing.Optional[typing_extensions.Literal["policy_type"]] = None,
+    ) -> TimeOffBalance:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/locations/{id}"),
-            params={
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/time-off-balances/{id}"),
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Location, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(TimeOffBalance, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/passthrough/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/pay_groups/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/pay_groups/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.paginated_pay_group_list import PaginatedPayGroupList
 from ...types.pay_group import PayGroup
 
 
 class PayGroupsClient:
     def __init__(
@@ -32,25 +33,27 @@
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedPayGroupList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/pay-groups"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedPayGroupList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -58,15 +61,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> PayGroup:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/pay-groups/{id}"),
-            params={"include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PayGroup, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -94,25 +97,27 @@
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedPayGroupList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/pay-groups"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedPayGroupList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -120,15 +125,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def retrieve(self, id: str, *, include_remote_data: typing.Optional[bool] = None) -> PayGroup:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/pay-groups/{id}"),
-            params={"include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PayGroup, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/payroll_runs/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/payroll_runs/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.paginated_payroll_run_list import PaginatedPayrollRunList
 from ...types.payroll_run import PayrollRun
 from ...types.payroll_runs_list_request_remote_fields import PayrollRunsListRequestRemoteFields
 from ...types.payroll_runs_list_request_run_type import PayrollRunsListRequestRunType
 from ...types.payroll_runs_list_request_show_enum_origins import PayrollRunsListRequestShowEnumOrigins
 from ...types.payroll_runs_retrieve_request_remote_fields import PayrollRunsRetrieveRequestRemoteFields
@@ -44,32 +45,34 @@
         show_enum_origins: typing.Optional[PayrollRunsListRequestShowEnumOrigins] = None,
         started_after: typing.Optional[str] = None,
         started_before: typing.Optional[str] = None,
     ) -> PaginatedPayrollRunList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/payroll-runs"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "ended_after": ended_after,
-                "ended_before": ended_before,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "run_type": run_type,
-                "show_enum_origins": show_enum_origins,
-                "started_after": started_after,
-                "started_before": started_before,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "ended_after": ended_after,
+                    "ended_before": ended_before,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "run_type": run_type,
+                    "show_enum_origins": show_enum_origins,
+                    "started_after": started_after,
+                    "started_before": started_before,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedPayrollRunList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -84,19 +87,21 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[PayrollRunsRetrieveRequestRemoteFields] = None,
         show_enum_origins: typing.Optional[PayrollRunsRetrieveRequestShowEnumOrigins] = None,
     ) -> PayrollRun:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/payroll-runs/{id}"),
-            params={
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PayrollRun, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -131,32 +136,34 @@
         show_enum_origins: typing.Optional[PayrollRunsListRequestShowEnumOrigins] = None,
         started_after: typing.Optional[str] = None,
         started_before: typing.Optional[str] = None,
     ) -> PaginatedPayrollRunList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/payroll-runs"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "ended_after": ended_after,
-                "ended_before": ended_before,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "run_type": run_type,
-                "show_enum_origins": show_enum_origins,
-                "started_after": started_after,
-                "started_before": started_before,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "ended_after": ended_after,
+                    "ended_before": ended_before,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "run_type": run_type,
+                    "show_enum_origins": show_enum_origins,
+                    "started_after": started_after,
+                    "started_before": started_before,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedPayrollRunList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -171,19 +178,21 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[PayrollRunsRetrieveRequestRemoteFields] = None,
         show_enum_origins: typing.Optional[PayrollRunsRetrieveRequestShowEnumOrigins] = None,
     ) -> PayrollRun:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/payroll-runs/{id}"),
-            params={
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PayrollRun, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/regenerate_key/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/selective_sync/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/selective_sync/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.linked_account_selective_sync_configuration import LinkedAccountSelectiveSyncConfiguration
 from ...types.linked_account_selective_sync_configuration_request import LinkedAccountSelectiveSyncConfigurationRequest
 from ...types.paginated_condition_schema_list import PaginatedConditionSchemaList
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
@@ -24,15 +25,15 @@
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def configurations_list(self) -> typing.List[LinkedAccountSelectiveSyncConfiguration]:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/selective-sync/configurations"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -41,15 +42,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def configurations_update(
         self, *, sync_configurations: typing.List[LinkedAccountSelectiveSyncConfigurationRequest]
     ) -> typing.List[LinkedAccountSelectiveSyncConfiguration]:
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/selective-sync/configurations"),
             json=jsonable_encoder({"sync_configurations": sync_configurations}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
@@ -63,16 +64,16 @@
         *,
         common_model: typing.Optional[str] = None,
         cursor: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
     ) -> PaginatedConditionSchemaList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/selective-sync/meta"),
-            params={"common_model": common_model, "cursor": cursor, "page_size": page_size},
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/selective-sync/meta"),
+            params=remove_none_from_dict({"common_model": common_model, "cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedConditionSchemaList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -87,15 +88,15 @@
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def configurations_list(self) -> typing.List[LinkedAccountSelectiveSyncConfiguration]:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/selective-sync/configurations"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -104,15 +105,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def configurations_update(
         self, *, sync_configurations: typing.List[LinkedAccountSelectiveSyncConfigurationRequest]
     ) -> typing.List[LinkedAccountSelectiveSyncConfiguration]:
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/selective-sync/configurations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/selective-sync/configurations"),
             json=jsonable_encoder({"sync_configurations": sync_configurations}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[LinkedAccountSelectiveSyncConfiguration], _response.json())  # type: ignore
         try:
@@ -126,16 +127,16 @@
         *,
         common_model: typing.Optional[str] = None,
         cursor: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
     ) -> PaginatedConditionSchemaList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/selective-sync/meta"),
-            params={"common_model": common_model, "cursor": cursor, "page_size": page_size},
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/selective-sync/meta"),
+            params=remove_none_from_dict({"common_model": common_model, "cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedConditionSchemaList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/sync_status/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/sync_status/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.paginated_sync_status_list import PaginatedSyncStatusList
 
 
 class SyncStatusClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
@@ -20,16 +21,16 @@
         self._client_wrapper = client_wrapper
 
     def list(
         self, *, cursor: typing.Optional[str] = None, page_size: typing.Optional[int] = None
     ) -> PaginatedSyncStatusList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/sync-status"),
-            params={"cursor": cursor, "page_size": page_size},
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/sync-status"),
+            params=remove_none_from_dict({"cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedSyncStatusList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -46,16 +47,16 @@
         self._client_wrapper = client_wrapper
 
     async def list(
         self, *, cursor: typing.Optional[str] = None, page_size: typing.Optional[int] = None
     ) -> PaginatedSyncStatusList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/sync-status"),
-            params={"cursor": cursor, "page_size": page_size},
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/sync-status"),
+            params=remove_none_from_dict({"cursor": cursor, "page_size": page_size}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedSyncStatusList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/teams/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/teams/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 import typing_extensions
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.paginated_team_list import PaginatedTeamList
 from ...types.team import Team
 
 
 class TeamsClient:
     def __init__(
@@ -35,27 +36,29 @@
         page_size: typing.Optional[int] = None,
         parent_team_id: typing.Optional[str] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedTeamList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/teams"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "parent_team_id": parent_team_id,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "parent_team_id": parent_team_id,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedTeamList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -69,15 +72,15 @@
         *,
         expand: typing.Optional[typing_extensions.Literal["parent_team"]] = None,
         include_remote_data: typing.Optional[bool] = None,
     ) -> Team:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/teams/{id}"),
-            params={"expand": expand, "include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Team, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -107,27 +110,29 @@
         page_size: typing.Optional[int] = None,
         parent_team_id: typing.Optional[str] = None,
         remote_id: typing.Optional[str] = None,
     ) -> PaginatedTeamList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/teams"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "parent_team_id": parent_team_id,
-                "remote_id": remote_id,
-            },
+            params=remove_none_from_dict(
+                {
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "parent_team_id": parent_team_id,
+                    "remote_id": remote_id,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedTeamList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -141,15 +146,15 @@
         *,
         expand: typing.Optional[typing_extensions.Literal["parent_team"]] = None,
         include_remote_data: typing.Optional[bool] = None,
     ) -> Team:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/teams/{id}"),
-            params={"expand": expand, "include_remote_data": include_remote_data},
+            params=remove_none_from_dict({"expand": expand, "include_remote_data": include_remote_data}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Team, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/time_off/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/time_off/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
 from ...types.meta_response import MetaResponse
 from ...types.paginated_time_off_list import PaginatedTimeOffList
 from ...types.time_off import TimeOff
 from ...types.time_off_list_request_expand import TimeOffListRequestExpand
 from ...types.time_off_list_request_remote_fields import TimeOffListRequestRemoteFields
 from ...types.time_off_list_request_request_type import TimeOffListRequestRequestType
@@ -54,32 +55,34 @@
         request_type: typing.Optional[TimeOffListRequestRequestType] = None,
         show_enum_origins: typing.Optional[TimeOffListRequestShowEnumOrigins] = None,
         status: typing.Optional[TimeOffListRequestStatus] = None,
     ) -> PaginatedTimeOffList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/time-off"),
-            params={
-                "approver_id": approver_id,
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "employee_id": employee_id,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "request_type": request_type,
-                "show_enum_origins": show_enum_origins,
-                "status": status,
-            },
+            params=remove_none_from_dict(
+                {
+                    "approver_id": approver_id,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "employee_id": employee_id,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "request_type": request_type,
+                    "show_enum_origins": show_enum_origins,
+                    "status": status,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedTimeOffList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -93,15 +96,15 @@
         is_debug_mode: typing.Optional[bool] = None,
         run_async: typing.Optional[bool] = None,
         model: TimeOffRequest,
     ) -> TimeOffResponse:
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/time-off"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TimeOffResponse, _response.json())  # type: ignore
         try:
@@ -118,20 +121,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[TimeOffRetrieveRequestRemoteFields] = None,
         show_enum_origins: typing.Optional[TimeOffRetrieveRequestShowEnumOrigins] = None,
     ) -> TimeOff:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/time-off/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TimeOff, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -181,32 +186,34 @@
         request_type: typing.Optional[TimeOffListRequestRequestType] = None,
         show_enum_origins: typing.Optional[TimeOffListRequestShowEnumOrigins] = None,
         status: typing.Optional[TimeOffListRequestStatus] = None,
     ) -> PaginatedTimeOffList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/time-off"),
-            params={
-                "approver_id": approver_id,
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "employee_id": employee_id,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "request_type": request_type,
-                "show_enum_origins": show_enum_origins,
-                "status": status,
-            },
+            params=remove_none_from_dict(
+                {
+                    "approver_id": approver_id,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "cursor": cursor,
+                    "employee_id": employee_id,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "request_type": request_type,
+                    "show_enum_origins": show_enum_origins,
+                    "status": status,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaginatedTimeOffList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -220,15 +227,15 @@
         is_debug_mode: typing.Optional[bool] = None,
         run_async: typing.Optional[bool] = None,
         model: TimeOffRequest,
     ) -> TimeOffResponse:
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/time-off"),
-            params={"is_debug_mode": is_debug_mode, "run_async": run_async},
+            params=remove_none_from_dict({"is_debug_mode": is_debug_mode, "run_async": run_async}),
             json=jsonable_encoder({"model": model}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TimeOffResponse, _response.json())  # type: ignore
         try:
@@ -245,20 +252,22 @@
         include_remote_data: typing.Optional[bool] = None,
         remote_fields: typing.Optional[TimeOffRetrieveRequestRemoteFields] = None,
         show_enum_origins: typing.Optional[TimeOffRetrieveRequestShowEnumOrigins] = None,
     ) -> TimeOff:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/time-off/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TimeOff, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/time_off_balances/client.py` & `fern_merge-0.0.32/src/merge/resources/ats/resources/offers/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,181 +5,191 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 import typing_extensions
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.remove_none_from_dict import remove_none_from_dict
 from .....environment import MergeEnvironment
-from ...types.paginated_time_off_balance_list import PaginatedTimeOffBalanceList
-from ...types.time_off_balance import TimeOffBalance
-from ...types.time_off_balances_list_request_policy_type import TimeOffBalancesListRequestPolicyType
+from ...types.offer import Offer
+from ...types.offers_list_request_expand import OffersListRequestExpand
+from ...types.offers_retrieve_request_expand import OffersRetrieveRequestExpand
+from ...types.paginated_offer_list import PaginatedOfferList
 
 
-class TimeOffBalancesClient:
+class OffersClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def list(
         self,
         *,
+        application_id: typing.Optional[str] = None,
         created_after: typing.Optional[str] = None,
         created_before: typing.Optional[str] = None,
+        creator_id: typing.Optional[str] = None,
         cursor: typing.Optional[str] = None,
-        employee_id: typing.Optional[str] = None,
-        expand: typing.Optional[typing_extensions.Literal["employee"]] = None,
+        expand: typing.Optional[OffersListRequestExpand] = None,
         include_deleted_data: typing.Optional[bool] = None,
         include_remote_data: typing.Optional[bool] = None,
         modified_after: typing.Optional[str] = None,
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
-        policy_type: typing.Optional[TimeOffBalancesListRequestPolicyType] = None,
-        remote_fields: typing.Optional[typing_extensions.Literal["policy_type"]] = None,
+        remote_fields: typing.Optional[typing_extensions.Literal["status"]] = None,
         remote_id: typing.Optional[str] = None,
-        show_enum_origins: typing.Optional[typing_extensions.Literal["policy_type"]] = None,
-    ) -> PaginatedTimeOffBalanceList:
+        show_enum_origins: typing.Optional[typing_extensions.Literal["status"]] = None,
+    ) -> PaginatedOfferList:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/time-off-balances"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "employee_id": employee_id,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "policy_type": policy_type,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/offers"),
+            params=remove_none_from_dict(
+                {
+                    "application_id": application_id,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "creator_id": creator_id,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaginatedTimeOffBalanceList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaginatedOfferList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def retrieve(
         self,
         id: str,
         *,
-        expand: typing.Optional[typing_extensions.Literal["employee"]] = None,
+        expand: typing.Optional[OffersRetrieveRequestExpand] = None,
         include_remote_data: typing.Optional[bool] = None,
-        remote_fields: typing.Optional[typing_extensions.Literal["policy_type"]] = None,
-        show_enum_origins: typing.Optional[typing_extensions.Literal["policy_type"]] = None,
-    ) -> TimeOffBalance:
+        remote_fields: typing.Optional[typing_extensions.Literal["status"]] = None,
+        show_enum_origins: typing.Optional[typing_extensions.Literal["status"]] = None,
+    ) -> Offer:
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/time-off-balances/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/offers/{id}"),
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TimeOffBalance, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Offer, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncTimeOffBalancesClient:
+class AsyncOffersClient:
     def __init__(
         self, *, environment: MergeEnvironment = MergeEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
     ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def list(
         self,
         *,
+        application_id: typing.Optional[str] = None,
         created_after: typing.Optional[str] = None,
         created_before: typing.Optional[str] = None,
+        creator_id: typing.Optional[str] = None,
         cursor: typing.Optional[str] = None,
-        employee_id: typing.Optional[str] = None,
-        expand: typing.Optional[typing_extensions.Literal["employee"]] = None,
+        expand: typing.Optional[OffersListRequestExpand] = None,
         include_deleted_data: typing.Optional[bool] = None,
         include_remote_data: typing.Optional[bool] = None,
         modified_after: typing.Optional[str] = None,
         modified_before: typing.Optional[str] = None,
         page_size: typing.Optional[int] = None,
-        policy_type: typing.Optional[TimeOffBalancesListRequestPolicyType] = None,
-        remote_fields: typing.Optional[typing_extensions.Literal["policy_type"]] = None,
+        remote_fields: typing.Optional[typing_extensions.Literal["status"]] = None,
         remote_id: typing.Optional[str] = None,
-        show_enum_origins: typing.Optional[typing_extensions.Literal["policy_type"]] = None,
-    ) -> PaginatedTimeOffBalanceList:
+        show_enum_origins: typing.Optional[typing_extensions.Literal["status"]] = None,
+    ) -> PaginatedOfferList:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/hris/v1/time-off-balances"),
-            params={
-                "created_after": created_after,
-                "created_before": created_before,
-                "cursor": cursor,
-                "employee_id": employee_id,
-                "expand": expand,
-                "include_deleted_data": include_deleted_data,
-                "include_remote_data": include_remote_data,
-                "modified_after": modified_after,
-                "modified_before": modified_before,
-                "page_size": page_size,
-                "policy_type": policy_type,
-                "remote_fields": remote_fields,
-                "remote_id": remote_id,
-                "show_enum_origins": show_enum_origins,
-            },
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/ats/v1/offers"),
+            params=remove_none_from_dict(
+                {
+                    "application_id": application_id,
+                    "created_after": created_after,
+                    "created_before": created_before,
+                    "creator_id": creator_id,
+                    "cursor": cursor,
+                    "expand": expand,
+                    "include_deleted_data": include_deleted_data,
+                    "include_remote_data": include_remote_data,
+                    "modified_after": modified_after,
+                    "modified_before": modified_before,
+                    "page_size": page_size,
+                    "remote_fields": remote_fields,
+                    "remote_id": remote_id,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(PaginatedTimeOffBalanceList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(PaginatedOfferList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def retrieve(
         self,
         id: str,
         *,
-        expand: typing.Optional[typing_extensions.Literal["employee"]] = None,
+        expand: typing.Optional[OffersRetrieveRequestExpand] = None,
         include_remote_data: typing.Optional[bool] = None,
-        remote_fields: typing.Optional[typing_extensions.Literal["policy_type"]] = None,
-        show_enum_origins: typing.Optional[typing_extensions.Literal["policy_type"]] = None,
-    ) -> TimeOffBalance:
+        remote_fields: typing.Optional[typing_extensions.Literal["status"]] = None,
+        show_enum_origins: typing.Optional[typing_extensions.Literal["status"]] = None,
+    ) -> Offer:
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/hris/v1/time-off-balances/{id}"),
-            params={
-                "expand": expand,
-                "include_remote_data": include_remote_data,
-                "remote_fields": remote_fields,
-                "show_enum_origins": show_enum_origins,
-            },
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/ats/v1/offers/{id}"),
+            params=remove_none_from_dict(
+                {
+                    "expand": expand,
+                    "include_remote_data": include_remote_data,
+                    "remote_fields": remote_fields,
+                    "show_enum_origins": show_enum_origins,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(TimeOffBalance, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Offer, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/resources/webhook_receivers/client.py` & `fern_merge-0.0.32/src/merge/resources/hris/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/__init__.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/account_details.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/account_details.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/account_details_and_actions.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/account_details_and_actions_integration.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/account_details_and_actions_status_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/account_integration.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/account_token.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/account_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/account_type_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/account_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/available_actions.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/bank_info.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/bank_info.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/bank_info_list_request_account_type.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/bank_info_list_request_account_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/bank_info_list_request_order_by.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/bank_info_list_request_order_by.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/benefit.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/benefit.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/categories_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/category_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/common_model_scopes_body_request.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/company.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/company.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/condition_schema.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/condition_type_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/country_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/country_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/debug_mode_log.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/debug_model_log_summary.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/deduction.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/deduction.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/earning.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/earning.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/earning_type_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/earning_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employee.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employee.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employee_payroll_run.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employee_payroll_run.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employee_request.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employee_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employee_response.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employee_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employees_list_request_employment_status.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employees_list_request_employment_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employees_list_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employees_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employees_list_request_remote_fields.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employees_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employees_retrieve_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employees_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employment.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employment.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employment_status_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employment_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employment_type_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employment_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employments_list_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employments_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employments_list_request_order_by.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employments_list_request_order_by.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employments_list_request_remote_fields.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employments_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employments_retrieve_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employments_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/enabled_actions_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/encoding_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/error_validation_problem.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/ethnicity_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/ethnicity_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/flsa_status_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/flsa_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/gender_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/gender_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/group.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/group.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/group_type_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/group_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/issue.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/issue.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/issue_status_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/link_token.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/link_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/linked_account_condition.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/linked_account_condition_request.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/linked_account_status.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/linked_accounts_list_request_category.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/location.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/location.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/marital_status_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/marital_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/meta_response.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/method_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/model_operation.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/multipart_form_field_request.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/multipart_form_field_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/operator_schema.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/paginated_bank_info_list.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/paginated_bank_info_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/paginated_benefit_list.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/paginated_benefit_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/paginated_company_list.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/paginated_company_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/paginated_condition_schema_list.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/paginated_employee_list.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/paginated_employee_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/paginated_employment_list.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/paginated_employment_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/paginated_group_list.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/paginated_group_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/paginated_issue_list.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/paginated_location_list.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/paginated_location_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/paginated_pay_group_list.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/paginated_pay_group_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/paginated_payroll_run_list.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/paginated_payroll_run_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/paginated_sync_status_list.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/paginated_team_list.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/paginated_team_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/paginated_time_off_balance_list.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/paginated_time_off_balance_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/paginated_time_off_list.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/paginated_time_off_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/pay_currency_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/pay_currency_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/pay_frequency_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/pay_frequency_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/pay_group.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/pay_group.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/pay_period_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/pay_period_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/payroll_run.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/payroll_run.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/policy_type_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/policy_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/reason_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/reason_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/remote_data.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/remote_key.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/remote_response.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/request_format_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/request_type_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/request_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/response_type_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/run_state_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/run_state_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/run_type_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/run_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/sync_status.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/sync_status_status_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/tax.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/tax.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/team.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/team.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/time_off.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/time_off.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/time_off_balance.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/time_off_balance.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/time_off_list_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/time_off_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/time_off_list_request_remote_fields.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/time_off_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/time_off_list_request_request_type.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/time_off_list_request_request_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/time_off_list_request_status.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/time_off_list_request_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/time_off_request.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/time_off_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/time_off_response.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/time_off_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/time_off_retrieve_request_expand.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/time_off_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/time_off_status_enum.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/time_off_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/validation_problem_source.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/warning_validation_problem.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/src/merge/resources/hris/types/webhook_receiver.py` & `fern_merge-0.0.32/src/merge/resources/hris/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.30/PKG-INFO` & `fern_merge-0.0.32/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-merge
-Version: 0.0.30
+Version: 0.0.32
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

