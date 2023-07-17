# Comparing `tmp/udps-0.1.20.tar.gz` & `tmp/udps-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udps-0.1.20.tar", max compression
+gzip compressed data, was "udps-0.1.21.tar", max compression
```

## Comparing `udps-0.1.20.tar` & `udps-0.1.21.tar`

### file list

```diff
@@ -1,253 +1,253 @@
--rw-r--r--   0        0        0    11357 2023-07-05 09:51:27.775414 udps-0.1.20/LICENSE
--rw-r--r--   0        0        0     2471 2023-07-05 09:51:27.775414 udps-0.1.20/README.md
--rw-r--r--   0        0        0     3071 2023-07-05 09:51:27.775414 udps-0.1.20/pyproject.toml
--rw-r--r--   0        0        0       44 2023-07-05 09:51:27.775414 udps-0.1.20/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.775414 udps-0.1.20/tests/mocks/__init__.py
--rw-r--r--   0        0        0      721 2023-07-05 09:51:27.775414 udps-0.1.20/tests/mocks/mock_writers.py
--rw-r--r--   0        0        0     1028 2023-07-05 09:51:27.775414 udps-0.1.20/tests/test_authz_analyzer.py
--rw-r--r--   0        0        0     6246 2023-07-05 09:51:27.775414 udps-0.1.20/tests/test_cli.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.775414 udps-0.1.20/tests/test_writers/__init__.py
--rw-r--r--   0        0        0     1355 2023-07-05 09:51:27.775414 udps-0.1.20/tests/test_writers/test_csv_writer.py
--rw-r--r--   0        0        0      953 2023-07-05 09:51:27.775414 udps-0.1.20/tests/test_writers/test_multijson_writer.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/__init__.py
--rw-r--r--   0        0        0        1 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/__init__.py
--rw-r--r--   0        0        0    14110 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json
--rw-r--r--   0        0        0    11644 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json
--rw-r--r--   0        0        0    14917 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json
--rw-r--r--   0        0        0     9884 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json
--rw-r--r--   0        0        0    20662 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json
--rw-r--r--   0        0        0    31812 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json
--rw-r--r--   0        0        0    18235 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json
--rw-r--r--   0        0        0    17618 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json
--rw-r--r--   0        0        0     7529 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json
--rw-r--r--   0        0        0     7744 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json
--rw-r--r--   0        0        0     4073 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json
--rw-r--r--   0        0        0    24204 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_identity_center/iam_identity_center_with_users_and_groups.json
--rw-r--r--   0        0        0    20163 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json
--rw-r--r--   0        0        0    13494 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json
--rw-r--r--   0        0        0     8446 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json
--rw-r--r--   0        0        0    16466 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json
--rw-r--r--   0        0        0    16126 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json
--rw-r--r--   0        0        0    14831 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json
--rw-r--r--   0        0        0     3066 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json
--rw-r--r--   0        0        0     5550 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json
--rw-r--r--   0        0        0     5906 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json
--rw-r--r--   0        0        0     4446 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json
--rw-r--r--   0        0        0     8937 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json
--rw-r--r--   0        0        0    20162 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json
--rw-r--r--   0        0        0    10324 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json
--rw-r--r--   0        0        0     6886 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json
--rw-r--r--   0        0        0    23422 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json
--rw-r--r--   0        0        0     2358 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json
--rw-r--r--   0        0        0     7124 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json
--rw-r--r--   0        0        0     4549 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json
--rw-r--r--   0        0        0     5215 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json
--rw-r--r--   0        0        0     5987 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json
--rw-r--r--   0        0        0     5862 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json
--rw-r--r--   0        0        0     3396 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json
--rw-r--r--   0        0        0     2298 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json
--rw-r--r--   0        0        0     5264 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json
--rw-r--r--   0        0        0     4596 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json
--rw-r--r--   0        0        0     3653 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json
--rw-r--r--   0        0        0     4392 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json
--rw-r--r--   0        0        0    26158 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json
--rw-r--r--   0        0        0    10097 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json
--rw-r--r--   0        0        0     8580 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json
--rw-r--r--   0        0        0    33775 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json
--rw-r--r--   0        0        0    16439 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json
--rw-r--r--   0        0        0    13955 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json
--rw-r--r--   0        0        0    18162 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json
--rw-r--r--   0        0        0     3040 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json
--rw-r--r--   0        0        0     5254 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json
--rw-r--r--   0        0        0     3569 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json
--rw-r--r--   0        0        0     4436 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json
--rw-r--r--   0        0        0    14441 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json
--rw-r--r--   0        0        0     3582 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py
--rw-r--r--   0        0        0     4890 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py
--rw-r--r--   0        0        0     4842 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/utils/__init__.py
--rw-r--r--   0        0        0     2831 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py
--rw-r--r--   0        0        0     1595 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json
--rw-r--r--   0        0        0     3805 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_iam_identity_center_user_and_group.json
--rw-r--r--   0        0        0     2597 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json
--rw-r--r--   0        0        0     2321 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json
--rw-r--r--   0        0        0     4018 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json
--rw-r--r--   0        0        0     5298 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json
--rw-r--r--   0        0        0     1579 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/test_exporter.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/utils/__init__.py
--rw-r--r--   0        0        0     1731 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/bigquery/__init__.py
--rw-r--r--   0        0        0     5596 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/bigquery/generate_authz_entry.py
--rw-r--r--   0        0        0     7137 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/bigquery/mocks.py
--rw-r--r--   0        0        0    15539 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/bigquery/test_bigquery.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/databricks/__init__.py
--rw-r--r--   0        0        0    17596 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/databricks/generate_authz_entry.py
--rw-r--r--   0        0        0     9136 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/databricks/mocks.py
--rw-r--r--   0        0        0    13149 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/databricks/test_analyzer.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/mongodb/__init__.py
--rw-r--r--   0        0        0    14532 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/mongodb/test_atlas_organization_users.py
--rw-r--r--   0        0        0     7391 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/mongodb/test_mongodb.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/postgres/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/postgres/mocks/__init__.py
--rw-r--r--   0        0        0     1195 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py
--rw-r--r--   0        0        0    12910 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/postgres/test_postgress_analyzer.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/redshift/__init__.py
--rw-r--r--   0        0        0    12179 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/redshift/test_redshift.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/snowflake/__init__.py
--rw-r--r--   0        0        0    19120 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/snowflake/test_snowflake_analyzer.py
--rw-r--r--   0        0        0     1086 2023-07-05 09:51:27.779414 udps-0.1.20/universal_data_permissions_scanner/__init__.py
--rw-r--r--   0        0        0    11523 2023-07-05 09:51:27.779414 udps-0.1.20/universal_data_permissions_scanner/cli.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/universal_data_permissions_scanner/datastores/__init__.py
--rw-r--r--   0        0        0      626 2023-07-05 09:51:27.779414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/__init__.py
--rw-r--r--   0        0        0      113 2023-07-05 09:51:27.779414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/__init__.py
--rw-r--r--   0        0        0     3252 2023-07-05 09:51:27.779414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/analyzer.py
--rw-r--r--   0        0        0     7808 2023-07-05 09:51:27.779414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/exporter.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/__init__.py
--rw-r--r--   0        0        0    13042 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/analyzer.py
--rw-r--r--   0        0        0       90 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/all_databases.sql
--rw-r--r--   0        0        0      141 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/all_tables.sql
--rw-r--r--   0        0        0      111 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashare_consumers.sql
--rw-r--r--   0        0        0       14 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashare_desc.sql
--rw-r--r--   0        0        0      125 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashares.sql
--rw-r--r--   0        0        0      893 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities.sql
--rw-r--r--   0        0        0      262 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities_privileges.sql
--rw-r--r--   0        0        0     5539 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/exporter.py
--rw-r--r--   0        0        0     3524 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/model.py
--rw-r--r--   0        0        0      660 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/service.py
--rw-r--r--   0        0        0      120 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/__init__.py
--rw-r--r--   0        0        0     3041 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py
--rw-r--r--   0        0        0     2045 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/__init__.py
--rw-r--r--   0        0        0     5682 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py
--rw-r--r--   0        0        0     3505 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py
--rw-r--r--   0        0        0     2481 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py
--rw-r--r--   0        0        0     6201 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py
--rw-r--r--   0        0        0     3963 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py
--rw-r--r--   0        0        0      254 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/__init__.py
--rw-r--r--   0        0        0       87 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/effect.py
--rw-r--r--   0        0        0      263 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/group_policy.py
--rw-r--r--   0        0        0      415 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy.py
--rw-r--r--   0        0        0     6232 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py
--rw-r--r--   0        0        0    10500 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py
--rw-r--r--   0        0        0      373 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_utils.py
--rw-r--r--   0        0        0      261 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/user_policy.py
--rw-r--r--   0        0        0      263 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/public_block_access_config.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/__init__.py
--rw-r--r--   0        0        0      261 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/role_policy.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/__init__.py
--rw-r--r--   0        0        0     5655 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_entities.py
--rw-r--r--   0        0        0     1961 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_groups.py
--rw-r--r--   0        0        0     1824 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_users.py
--rw-r--r--   0        0        0     2502 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/permission_sets.py
--rw-r--r--   0        0        0     1046 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/logger.py
--rw-r--r--   0        0        0      263 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/__init__.py
--rw-r--r--   0        0        0    18760 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py
--rw-r--r--   0        0        0      172 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/__init__.py
--rw-r--r--   0        0        0    12130 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py
--rw-r--r--   0        0        0     1267 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py
--rw-r--r--   0        0        0    12938 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py
--rw-r--r--   0        0        0     3704 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py
--rw-r--r--   0        0        0    10597 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/__init__.py
--rw-r--r--   0        0        0    12040 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py
--rw-r--r--   0        0        0     8007 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py
--rw-r--r--   0        0        0    15325 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py
--rw-r--r--   0        0        0    26419 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py
--rw-r--r--   0        0        0     6471 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py
--rw-r--r--   0        0        0      513 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py
--rw-r--r--   0        0        0     8549 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/__init__.py
--rw-r--r--   0        0        0     5233 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py
--rw-r--r--   0        0        0     4475 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py
--rw-r--r--   0        0        0     1644 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/__init__.py
--rw-r--r--   0        0        0     2905 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py
--rw-r--r--   0        0        0     6158 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py
--rw-r--r--   0        0        0     2185 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/__init__.py
--rw-r--r--   0        0        0     2147 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py
--rw-r--r--   0        0        0     7453 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py
--rw-r--r--   0        0        0     2289 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py
--rw-r--r--   0        0        0     2594 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/__init__.py
--rw-r--r--   0        0        0     3377 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py
--rw-r--r--   0        0        0     1054 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py
--rw-r--r--   0        0        0    17633 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py
--rw-r--r--   0        0        0     7562 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py
--rw-r--r--   0        0        0     1894 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py
--rw-r--r--   0        0        0      398 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_base.py
--rw-r--r--   0        0        0     1973 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py
--rw-r--r--   0        0        0     3041 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py
--rw-r--r--   0        0        0      397 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_base.py
--rw-r--r--   0        0        0      561 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py
--rw-r--r--   0        0        0     2501 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py
--rw-r--r--   0        0        0     9989 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/__init__.py
--rw-r--r--   0        0        0      482 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/assume_role.py
--rw-r--r--   0        0        0      879 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py
--rw-r--r--   0        0        0     1000 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py
--rw-r--r--   0        0        0     2747 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py
--rw-r--r--   0        0        0      173 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/serde.py
--rw-r--r--   0        0        0      131 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/bigquery/__init__.py
--rw-r--r--   0        0        0    11747 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/bigquery/analyzer.py
--rw-r--r--   0        0        0    12689 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/bigquery/policy_tree.py
--rw-r--r--   0        0        0     7740 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/bigquery/service.py
--rw-r--r--   0        0        0      138 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/__init__.py
--rw-r--r--   0        0        0     6516 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/analyzer.py
--rw-r--r--   0        0        0       53 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/exceptions.py
--rw-r--r--   0        0        0     8187 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/identities.py
--rw-r--r--   0        0        0     1331 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/model.py
--rw-r--r--   0        0        0    10555 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/policy_tree.py
--rw-r--r--   0        0        0      138 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/__init__.py
--rw-r--r--   0        0        0      138 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/authentication/__init__.py
--rw-r--r--   0        0        0      879 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/authentication/authentication.py
--rw-r--r--   0        0        0      110 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/authentication/basic.py
--rw-r--r--   0        0        0     1894 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/authentication/oauth.py
--rw-r--r--   0        0        0     2448 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/model.py
--rw-r--r--   0        0        0     1425 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/scim.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/__init__.py
--rw-r--r--   0        0        0    16135 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/analyzer.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/__init__.py
--rw-r--r--   0        0        0    17422 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/analyzer.py
--rw-r--r--   0        0        0     6172 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/model.py
--rw-r--r--   0        0        0     2527 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/permission_resolvers.py
--rw-r--r--   0        0        0     5892 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/service.py
--rw-r--r--   0        0        0     2394 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/service_model.py
--rw-r--r--   0        0        0     2197 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/model.py
--rw-r--r--   0        0        0     1553 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/resolvers.py
--rw-r--r--   0        0        0     1448 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/service.py
--rw-r--r--   0        0        0     1196 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/service_model.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/__init__.py
--rw-r--r--   0        0        0    10604 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/analyzer.py
--rw-r--r--   0        0        0       71 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/commands/all_databases.sql
--rw-r--r--   0        0        0      369 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/commands/all_tables.sql
--rw-r--r--   0        0        0      272 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/commands/roles.sql
--rw-r--r--   0        0        0      313 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/commands/roles_grants.sql
--rw-r--r--   0        0        0     2404 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/database_query_results.py
--rw-r--r--   0        0        0      822 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/deployment.py
--rw-r--r--   0        0        0     2687 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/exporter.py
--rw-r--r--   0        0        0     1891 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/model.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/__init__.py
--rw-r--r--   0        0        0    12836 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/analyzer.py
--rw-r--r--   0        0        0      389 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/commands/grants_roles.sql
--rw-r--r--   0        0        0       20 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/commands/grants_to_share.sql
--rw-r--r--   0        0        0       11 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/commands/shares.sql
--rw-r--r--   0        0        0      535 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/commands/user_grants.sql
--rw-r--r--   0        0        0     5827 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/exporter.py
--rw-r--r--   0        0        0     4685 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/model.py
--rw-r--r--   0        0        0     1048 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/service.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/errors/__init__.py
--rw-r--r--   0        0        0       45 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/errors/failed_connection_errors.py
--rw-r--r--   0        0        0     7158 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/main.py
--rw-r--r--   0        0        0      195 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/models/__init__.py
--rw-r--r--   0        0        0     7583 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/models/model.py
--rw-r--r--   0        0        0        0 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/utils/__init__.py
--rw-r--r--   0        0        0      651 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/utils/logger.py
--rw-r--r--   0        0        0      452 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/writers/__init__.py
--rw-r--r--   0        0        0     1020 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/writers/base_writers.py
--rw-r--r--   0        0        0      728 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/writers/csv_writer.py
--rw-r--r--   0        0        0     1138 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/writers/get_writers.py
--rw-r--r--   0        0        0     2090 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/writers/multi_json_exporter.py
--rw-r--r--   0        0        0     5032 1970-01-01 00:00:00.000000 udps-0.1.20/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-17 10:35:27.787029 udps-0.1.21/LICENSE
+-rw-r--r--   0        0        0     2471 2023-07-17 10:35:27.787029 udps-0.1.21/README.md
+-rw-r--r--   0        0        0     3112 2023-07-17 10:35:27.791029 udps-0.1.21/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-07-17 10:35:27.791029 udps-0.1.21/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.791029 udps-0.1.21/tests/mocks/__init__.py
+-rw-r--r--   0        0        0      721 2023-07-17 10:35:27.791029 udps-0.1.21/tests/mocks/mock_writers.py
+-rw-r--r--   0        0        0     1028 2023-07-17 10:35:27.791029 udps-0.1.21/tests/test_authz_analyzer.py
+-rw-r--r--   0        0        0     6246 2023-07-17 10:35:27.791029 udps-0.1.21/tests/test_cli.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.791029 udps-0.1.21/tests/test_writers/__init__.py
+-rw-r--r--   0        0        0     1355 2023-07-17 10:35:27.791029 udps-0.1.21/tests/test_writers/test_csv_writer.py
+-rw-r--r--   0        0        0      953 2023-07-17 10:35:27.791029 udps-0.1.21/tests/test_writers/test_multijson_writer.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/__init__.py
+-rw-r--r--   0        0        0        1 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/__init__.py
+-rw-r--r--   0        0        0    14110 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json
+-rw-r--r--   0        0        0    11644 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json
+-rw-r--r--   0        0        0    14917 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json
+-rw-r--r--   0        0        0     9884 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json
+-rw-r--r--   0        0        0    20662 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json
+-rw-r--r--   0        0        0    31812 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json
+-rw-r--r--   0        0        0    18235 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json
+-rw-r--r--   0        0        0    17618 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json
+-rw-r--r--   0        0        0     7529 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json
+-rw-r--r--   0        0        0     7744 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json
+-rw-r--r--   0        0        0     4073 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json
+-rw-r--r--   0        0        0    24204 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_identity_center/iam_identity_center_with_users_and_groups.json
+-rw-r--r--   0        0        0    20163 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json
+-rw-r--r--   0        0        0    13494 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json
+-rw-r--r--   0        0        0     8446 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json
+-rw-r--r--   0        0        0    16466 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json
+-rw-r--r--   0        0        0    16126 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json
+-rw-r--r--   0        0        0    14831 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json
+-rw-r--r--   0        0        0     3066 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json
+-rw-r--r--   0        0        0     5550 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json
+-rw-r--r--   0        0        0     5906 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json
+-rw-r--r--   0        0        0     4446 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json
+-rw-r--r--   0        0        0     8937 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json
+-rw-r--r--   0        0        0    20162 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json
+-rw-r--r--   0        0        0    10324 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json
+-rw-r--r--   0        0        0     6886 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json
+-rw-r--r--   0        0        0    23422 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json
+-rw-r--r--   0        0        0     2358 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json
+-rw-r--r--   0        0        0     7124 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json
+-rw-r--r--   0        0        0     4549 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json
+-rw-r--r--   0        0        0     5215 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json
+-rw-r--r--   0        0        0     5987 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json
+-rw-r--r--   0        0        0     5862 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json
+-rw-r--r--   0        0        0     3396 2023-07-17 10:35:27.791029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json
+-rw-r--r--   0        0        0     2298 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json
+-rw-r--r--   0        0        0     5264 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json
+-rw-r--r--   0        0        0     4596 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json
+-rw-r--r--   0        0        0     3653 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json
+-rw-r--r--   0        0        0     4392 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json
+-rw-r--r--   0        0        0    26158 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json
+-rw-r--r--   0        0        0    10097 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json
+-rw-r--r--   0        0        0     8580 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json
+-rw-r--r--   0        0        0    33775 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json
+-rw-r--r--   0        0        0    16439 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json
+-rw-r--r--   0        0        0    13955 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json
+-rw-r--r--   0        0        0    18162 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json
+-rw-r--r--   0        0        0     3040 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json
+-rw-r--r--   0        0        0     5254 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json
+-rw-r--r--   0        0        0     3569 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json
+-rw-r--r--   0        0        0     4436 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json
+-rw-r--r--   0        0        0    14441 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json
+-rw-r--r--   0        0        0     3582 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py
+-rw-r--r--   0        0        0     4890 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py
+-rw-r--r--   0        0        0     4842 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/utils/__init__.py
+-rw-r--r--   0        0        0     2831 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py
+-rw-r--r--   0        0        0     1595 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json
+-rw-r--r--   0        0        0     3805 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_iam_identity_center_user_and_group.json
+-rw-r--r--   0        0        0     2597 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json
+-rw-r--r--   0        0        0     2321 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json
+-rw-r--r--   0        0        0     4018 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json
+-rw-r--r--   0        0        0     5298 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json
+-rw-r--r--   0        0        0     1579 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/test_exporter.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/utils/__init__.py
+-rw-r--r--   0        0        0     1731 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/bigquery/__init__.py
+-rw-r--r--   0        0        0     5596 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/bigquery/generate_authz_entry.py
+-rw-r--r--   0        0        0     7137 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/bigquery/mocks.py
+-rw-r--r--   0        0        0    15539 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/bigquery/test_bigquery.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/databricks/__init__.py
+-rw-r--r--   0        0        0    17596 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/databricks/generate_authz_entry.py
+-rw-r--r--   0        0        0     9136 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/databricks/mocks.py
+-rw-r--r--   0        0        0    13149 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/databricks/test_analyzer.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/mongodb/__init__.py
+-rw-r--r--   0        0        0    14532 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/mongodb/test_atlas_organization_users.py
+-rw-r--r--   0        0        0     7391 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/mongodb/test_mongodb.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/postgres/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/postgres/mocks/__init__.py
+-rw-r--r--   0        0        0     1195 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py
+-rw-r--r--   0        0        0    12910 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/postgres/test_postgress_analyzer.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/redshift/__init__.py
+-rw-r--r--   0        0        0    12179 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/redshift/test_redshift.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/snowflake/__init__.py
+-rw-r--r--   0        0        0    19120 2023-07-17 10:35:27.795029 udps-0.1.21/tests/tests_datastores/snowflake/test_snowflake_analyzer.py
+-rw-r--r--   0        0        0     1086 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/__init__.py
+-rw-r--r--   0        0        0    11767 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/cli.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/__init__.py
+-rw-r--r--   0        0        0      626 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/__init__.py
+-rw-r--r--   0        0        0     3252 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/analyzer.py
+-rw-r--r--   0        0        0     7808 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/exporter.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/__init__.py
+-rw-r--r--   0        0        0    13070 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/analyzer.py
+-rw-r--r--   0        0        0       90 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/all_databases.sql
+-rw-r--r--   0        0        0      141 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/all_tables.sql
+-rw-r--r--   0        0        0      111 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashare_consumers.sql
+-rw-r--r--   0        0        0       14 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashare_desc.sql
+-rw-r--r--   0        0        0      125 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashares.sql
+-rw-r--r--   0        0        0      893 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities.sql
+-rw-r--r--   0        0        0      262 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities_privileges.sql
+-rw-r--r--   0        0        0     5539 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/exporter.py
+-rw-r--r--   0        0        0     3524 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/model.py
+-rw-r--r--   0        0        0      660 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/service.py
+-rw-r--r--   0        0        0      120 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/__init__.py
+-rw-r--r--   0        0        0     3041 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py
+-rw-r--r--   0        0        0     2045 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/__init__.py
+-rw-r--r--   0        0        0     5682 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py
+-rw-r--r--   0        0        0     3505 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py
+-rw-r--r--   0        0        0     2481 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py
+-rw-r--r--   0        0        0     6201 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py
+-rw-r--r--   0        0        0     3963 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py
+-rw-r--r--   0        0        0      254 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/__init__.py
+-rw-r--r--   0        0        0       87 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/effect.py
+-rw-r--r--   0        0        0      263 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/group_policy.py
+-rw-r--r--   0        0        0      415 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy.py
+-rw-r--r--   0        0        0     6232 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py
+-rw-r--r--   0        0        0    10500 2023-07-17 10:35:27.795029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py
+-rw-r--r--   0        0        0      373 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_utils.py
+-rw-r--r--   0        0        0      261 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/user_policy.py
+-rw-r--r--   0        0        0      263 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/public_block_access_config.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/__init__.py
+-rw-r--r--   0        0        0      261 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/role_policy.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/__init__.py
+-rw-r--r--   0        0        0     5655 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_entities.py
+-rw-r--r--   0        0        0     1961 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_groups.py
+-rw-r--r--   0        0        0     1824 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_users.py
+-rw-r--r--   0        0        0     2502 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/permission_sets.py
+-rw-r--r--   0        0        0     1046 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/logger.py
+-rw-r--r--   0        0        0      263 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/__init__.py
+-rw-r--r--   0        0        0    18760 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py
+-rw-r--r--   0        0        0      172 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/__init__.py
+-rw-r--r--   0        0        0    12130 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py
+-rw-r--r--   0        0        0     1267 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py
+-rw-r--r--   0        0        0    12938 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py
+-rw-r--r--   0        0        0     3704 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py
+-rw-r--r--   0        0        0    10597 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/__init__.py
+-rw-r--r--   0        0        0    12040 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py
+-rw-r--r--   0        0        0     8007 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py
+-rw-r--r--   0        0        0    15325 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py
+-rw-r--r--   0        0        0    26419 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py
+-rw-r--r--   0        0        0     6471 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py
+-rw-r--r--   0        0        0      513 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py
+-rw-r--r--   0        0        0     8549 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/__init__.py
+-rw-r--r--   0        0        0     5233 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py
+-rw-r--r--   0        0        0     4475 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py
+-rw-r--r--   0        0        0     1644 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/__init__.py
+-rw-r--r--   0        0        0     2905 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py
+-rw-r--r--   0        0        0     6158 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py
+-rw-r--r--   0        0        0     2185 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/__init__.py
+-rw-r--r--   0        0        0     2147 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py
+-rw-r--r--   0        0        0     7453 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py
+-rw-r--r--   0        0        0     2289 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py
+-rw-r--r--   0        0        0     2594 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/__init__.py
+-rw-r--r--   0        0        0     3377 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py
+-rw-r--r--   0        0        0     1054 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py
+-rw-r--r--   0        0        0    17633 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py
+-rw-r--r--   0        0        0     7562 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py
+-rw-r--r--   0        0        0     1894 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py
+-rw-r--r--   0        0        0      398 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_base.py
+-rw-r--r--   0        0        0     1973 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py
+-rw-r--r--   0        0        0     3041 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py
+-rw-r--r--   0        0        0      397 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_base.py
+-rw-r--r--   0        0        0      561 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py
+-rw-r--r--   0        0        0     2501 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py
+-rw-r--r--   0        0        0     9989 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/__init__.py
+-rw-r--r--   0        0        0      482 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/assume_role.py
+-rw-r--r--   0        0        0      879 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py
+-rw-r--r--   0        0        0     1000 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py
+-rw-r--r--   0        0        0     2747 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py
+-rw-r--r--   0        0        0      173 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/serde.py
+-rw-r--r--   0        0        0      131 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/bigquery/__init__.py
+-rw-r--r--   0        0        0    11747 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/bigquery/analyzer.py
+-rw-r--r--   0        0        0    12689 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/bigquery/policy_tree.py
+-rw-r--r--   0        0        0     7740 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/bigquery/service.py
+-rw-r--r--   0        0        0      138 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/__init__.py
+-rw-r--r--   0        0        0     6516 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/analyzer.py
+-rw-r--r--   0        0        0       53 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/exceptions.py
+-rw-r--r--   0        0        0     8187 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/identities.py
+-rw-r--r--   0        0        0     1331 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/model.py
+-rw-r--r--   0        0        0    10555 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/policy_tree.py
+-rw-r--r--   0        0        0      138 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/service/__init__.py
+-rw-r--r--   0        0        0      138 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/service/authentication/__init__.py
+-rw-r--r--   0        0        0      879 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/service/authentication/authentication.py
+-rw-r--r--   0        0        0      110 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/service/authentication/basic.py
+-rw-r--r--   0        0        0     1894 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/service/authentication/oauth.py
+-rw-r--r--   0        0        0     2448 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/service/model.py
+-rw-r--r--   0        0        0     1425 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/service/scim.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/__init__.py
+-rw-r--r--   0        0        0    16135 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/analyzer.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/atlas/__init__.py
+-rw-r--r--   0        0        0    17422 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/atlas/analyzer.py
+-rw-r--r--   0        0        0     6172 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/atlas/model.py
+-rw-r--r--   0        0        0     2527 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/atlas/permission_resolvers.py
+-rw-r--r--   0        0        0     5892 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/atlas/service.py
+-rw-r--r--   0        0        0     2394 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/atlas/service_model.py
+-rw-r--r--   0        0        0     2197 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/model.py
+-rw-r--r--   0        0        0     1553 2023-07-17 10:35:27.799029 udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/resolvers.py
+-rw-r--r--   0        0        0     1448 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/service.py
+-rw-r--r--   0        0        0     1196 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/service_model.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/postgres/__init__.py
+-rw-r--r--   0        0        0    10604 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/postgres/analyzer.py
+-rw-r--r--   0        0        0       71 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/postgres/commands/all_databases.sql
+-rw-r--r--   0        0        0      369 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/postgres/commands/all_tables.sql
+-rw-r--r--   0        0        0      272 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/postgres/commands/roles.sql
+-rw-r--r--   0        0        0      313 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/postgres/commands/roles_grants.sql
+-rw-r--r--   0        0        0     2404 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/postgres/database_query_results.py
+-rw-r--r--   0        0        0      822 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/postgres/deployment.py
+-rw-r--r--   0        0        0     2687 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/postgres/exporter.py
+-rw-r--r--   0        0        0     1891 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/postgres/model.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/snowflake/__init__.py
+-rw-r--r--   0        0        0    12974 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/snowflake/analyzer.py
+-rw-r--r--   0        0        0      389 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/snowflake/commands/grants_roles.sql
+-rw-r--r--   0        0        0       20 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/snowflake/commands/grants_to_share.sql
+-rw-r--r--   0        0        0       11 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/snowflake/commands/shares.sql
+-rw-r--r--   0        0        0      535 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/snowflake/commands/user_grants.sql
+-rw-r--r--   0        0        0     5827 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/snowflake/exporter.py
+-rw-r--r--   0        0        0     4685 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/snowflake/model.py
+-rw-r--r--   0        0        0     1048 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/datastores/snowflake/service.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/errors/__init__.py
+-rw-r--r--   0        0        0       45 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/errors/failed_connection_errors.py
+-rw-r--r--   0        0        0     7191 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/main.py
+-rw-r--r--   0        0        0      195 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/models/__init__.py
+-rw-r--r--   0        0        0     7583 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/models/model.py
+-rw-r--r--   0        0        0        0 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/utils/__init__.py
+-rw-r--r--   0        0        0      651 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/utils/logger.py
+-rw-r--r--   0        0        0      452 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/writers/__init__.py
+-rw-r--r--   0        0        0     1020 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/writers/base_writers.py
+-rw-r--r--   0        0        0      728 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/writers/csv_writer.py
+-rw-r--r--   0        0        0     1138 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/writers/get_writers.py
+-rw-r--r--   0        0        0     2090 2023-07-17 10:35:27.803030 udps-0.1.21/universal_data_permissions_scanner/writers/multi_json_exporter.py
+-rw-r--r--   0        0        0     5078 1970-01-01 00:00:00.000000 udps-0.1.21/PKG-INFO
```

### Comparing `udps-0.1.20/LICENSE` & `udps-0.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/README.md` & `udps-0.1.21/README.md`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/pyproject.toml` & `udps-0.1.21/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool]
 [tool.poetry]
 name = "udps"
-version = "0.1.20"
+version = "0.1.21"
 homepage = "https://github.com/satoricyber/universal-data-permissions-scanner"
 description = "Analyze authorization."
 authors = ["SatoriCyber"]
 readme = "README.md"
 classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
 ]
 packages = [
     { include = "universal_data_permissions_scanner" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.11"
+python = ">=3.8.1,<3.12"
 click = "8.1.3"
 snowflake-connector-python = "=3.0.2"
-google-cloud-bigquery = ">=2.1.0,<3.0"
+google-cloud-bigquery = ">=3.4.2"
 google-cloud-resource-manager = ">=1.6.3,<2.0"
 google-api-python-client = "~2.66.0"
 boto3 = "^1.26.27"
 pydantic = "^1.10.2"
 networkx = "^2.8.8"
 pyserde = "^0.9.6"
 psycopg2 = "^2.9.5"
```

### Comparing `udps-0.1.20/tests/mocks/mock_writers.py` & `udps-0.1.21/tests/mocks/mock_writers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/test_authz_analyzer.py` & `udps-0.1.21/tests/test_authz_analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/test_cli.py` & `udps-0.1.21/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/test_writers/test_csv_writer.py` & `udps-0.1.21/tests/test_writers/test_csv_writer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/test_writers/test_multijson_writer.py` & `udps-0.1.21/tests/test_writers/test_multijson_writer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_identity_center/iam_identity_center_with_users_and_groups.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_identity_center/iam_identity_center_with_users_and_groups.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py` & `udps-0.1.21/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json` & `udps-0.1.21/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_iam_identity_center_user_and_group.json` & `udps-0.1.21/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_iam_identity_center_user_and_group.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json` & `udps-0.1.21/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json` & `udps-0.1.21/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json` & `udps-0.1.21/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json` & `udps-0.1.21/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/test_exporter.py` & `udps-0.1.21/tests/tests_datastores/aws/test_exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py` & `udps-0.1.21/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/bigquery/generate_authz_entry.py` & `udps-0.1.21/tests/tests_datastores/bigquery/generate_authz_entry.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/bigquery/mocks.py` & `udps-0.1.21/tests/tests_datastores/bigquery/mocks.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/bigquery/test_bigquery.py` & `udps-0.1.21/tests/tests_datastores/bigquery/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/databricks/generate_authz_entry.py` & `udps-0.1.21/tests/tests_datastores/databricks/generate_authz_entry.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/databricks/mocks.py` & `udps-0.1.21/tests/tests_datastores/databricks/mocks.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/databricks/test_analyzer.py` & `udps-0.1.21/tests/tests_datastores/databricks/test_analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/mongodb/test_atlas_organization_users.py` & `udps-0.1.21/tests/tests_datastores/mongodb/test_atlas_organization_users.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/mongodb/test_mongodb.py` & `udps-0.1.21/tests/tests_datastores/mongodb/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py` & `udps-0.1.21/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/postgres/test_postgress_analyzer.py` & `udps-0.1.21/tests/tests_datastores/postgres/test_postgress_analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/redshift/test_redshift.py` & `udps-0.1.21/tests/tests_datastores/redshift/test_redshift.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/tests/tests_datastores/snowflake/test_snowflake_analyzer.py` & `udps-0.1.21/tests/tests_datastores/snowflake/test_snowflake_analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/__init__.py` & `udps-0.1.21/universal_data_permissions_scanner/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for authz-analyzer."""
 
 __author__ = """SatoriCyber"""
 __email__ = 'contact@satoricyber.com'
-__version__ = '0.1.20'
+__version__ = '0.1.21'
 
 from universal_data_permissions_scanner.datastores.aws.analyzer import AwsAssumeRoleInput, AWSAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.aws.analyzer.redshift.analyzer import RedshiftAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.bigquery.analyzer import BigQueryAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.databricks.analyzer import DatabricksAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.mongodb.analyzer import MongoDBAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.mongodb.atlas.analyzer import MongoDBAtlasAuthzAnalyzer  # type: ignore
```

### Comparing `udps-0.1.20/universal_data_permissions_scanner/cli.py` & `udps-0.1.21/universal_data_permissions_scanner/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,31 +70,43 @@
 @click.option('--host', '-t', required=False, type=str, help="Hostname")
 @click.option('--warehouse', '-w', required=False, type=str, help="Warehouse")
 def snowflake(
     ctx: click.Context,
     username: str,
     password: Optional[str],
     account: str,
-    host: str,
+    host: Optional[str],
     warehouse: Optional[str],
     rsa_key: Optional[TextIO],
     rsa_pass: Optional[str],
 ):
     """Analyze Snowflake Authorization"""
     if not any([password, rsa_key]):
         click.echo('Error: Required at least one of the options: --password / -p or --rsa / -r')
         return
 
     rsa: Optional[str] = None
     if rsa_key is not None:
         rsa = rsa_key.read()
 
     output_path = Path(ctx.obj['OUT'])
+    kwargs = {}
+    if host is not None:
+        kwargs['host'] = host
     run_snowflake(
-        ctx.obj['LOGGER'], username, password, account, host, warehouse, ctx.obj["FORMAT"], output_path, rsa, rsa_pass
+        logger=ctx.obj['LOGGER'],
+        username=username,
+        password=password,
+        account=account,
+        warehouse=warehouse,
+        output_format=ctx.obj["FORMAT"],
+        output_path=output_path,
+        rsa_key=rsa,
+        rsa_pass=rsa_pass,
+        **kwargs,
     )
 
 
 @main.command()
 @click.pass_context
 @click.option('--project', '-p', required=True, type=str, help="GCP project ID, for example: acme-webapp-prod")
 @click.option('--key-file', '-k', required=False, type=str, help="Path to GCP service account file")
```

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/__init__.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/analyzer.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/exporter.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/analyzer.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Only users can be members of groups, i.e. a group cannot be a member of other groups
 Only users can own relations
 Both users and groups can have privileges granted to them
 
 The database will not let you set up circular membership loops.
 """
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from logging import Logger
 from pathlib import Path
 from typing import Any, Dict, Optional, Set, Union
 
 import redshift_connector  # type: ignore
 
 from universal_data_permissions_scanner.datastores.aws.analyzer.redshift import exporter
@@ -47,15 +47,15 @@
 @dataclass
 class RedshiftAuthzAnalyzer:
     """Analyze authorization for Redshift."""
 
     cursors: Dict[DatabaseName, redshift_connector.Cursor]
     writer: BaseWriter
     logger: Logger
-    service: RedshiftService = RedshiftService()
+    service: RedshiftService = field(default_factory=RedshiftService)
 
     @classmethod
     def connect(  # pylint: disable=too-many-locals
         cls,
         username: str,
         password: str,
         host: str,
```

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities.sql` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities.sql`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/exporter.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/model.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/service.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_entities.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_entities.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_groups.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_groups.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_users.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_users.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/permission_sets.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/permission_sets.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/logger.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/logger.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/bigquery/analyzer.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/bigquery/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/bigquery/policy_tree.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/bigquery/policy_tree.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/bigquery/service.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/bigquery/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/analyzer.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/identities.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/identities.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/model.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/policy_tree.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/policy_tree.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/authentication/authentication.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/service/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/authentication/oauth.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/service/authentication/oauth.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/model.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/service/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/scim.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/databricks/service/scim.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/analyzer.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/analyzer.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/atlas/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/model.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/atlas/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/permission_resolvers.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/atlas/permission_resolvers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/service.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/atlas/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/service_model.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/atlas/service_model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/model.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/resolvers.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/resolvers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/service.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/service_model.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/mongodb/service_model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/analyzer.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/postgres/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/database_query_results.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/postgres/database_query_results.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/deployment.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/postgres/deployment.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/exporter.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/postgres/exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/model.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/postgres/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/analyzer.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/snowflake/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,39 +60,41 @@
     service: SnowflakeService
     writer: BaseWriter
     logger: Logger
 
     @classmethod
     def connect(  # pylint: disable=too-many-locals
         cls,
-        host: str,
         account: str,
         username: str,
         warehouse: Optional[str],
         logger: Optional[Logger] = None,
         output_format: OutputFormat = OutputFormat.CSV,
         output_path: Union[Path, str] = Path.cwd() / DEFAULT_OUTPUT_FILE,
         rsa_key: Optional[str] = None,
         rsa_pass: Optional[str] = None,
         **snowflake_connection_kwargs: Any,
     ):
         """Connect to Snowflake and return an analyzer.
 
         Args:
-            host (str): Snowflake host
             account (str): Snowflake account
             username (str): Snowflake username to connect with
             password (Optional[str]): Snowflake password to connect with
             rsa_key: (Optional[str]): Snowflake rsa key to connect with
             rsa_pass: (Optional[str]): RSA password to decrypt rsa key
             warehouse (str): Snowflake warehouse to use
             logger (Optional[Logger], optional): Python logger. Defaults to None.
             output_path (Union[Path, str], optional): Path to write the file. Defaults to ./authz-analyzer-export.
             output_format (OutputFormat, optional): Output format. Defaults to OutputFormat.CSV.
+            snowflake_connection_kwargs:
+                host (str): Snowflake host
+                application (str): Snowflake application name
         """
+        snowflake_connection_kwargs.setdefault("application", "Satori_UDPS")
         if logger is None:
             logger = get_logger(False)
 
         writer = get_writer(filename=output_path, output_format=output_format)
 
         # Handle case sensitive warehouse name, wrap with quotes
         if warehouse is not None:
@@ -100,15 +102,14 @@
 
         if rsa_key is not None:
             snowflake_connection_kwargs["private_key"] = SnowflakeAuthzAnalyzer._read_private_key(rsa_key, rsa_pass)
 
         try:
             connector = snowflake.connector.connect(  # type: ignore
                 user=username,
-                host=host,
                 account=account,
                 warehouse=warehouse,
                 **snowflake_connection_kwargs,
             )
         except Exception as err:
             raise ConnectionFailure from err
```

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/commands/user_grants.sql` & `udps-0.1.21/universal_data_permissions_scanner/datastores/snowflake/commands/user_grants.sql`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/exporter.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/snowflake/exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/model.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/snowflake/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/service.py` & `udps-0.1.21/universal_data_permissions_scanner/datastores/snowflake/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/main.py` & `udps-0.1.21/universal_data_permissions_scanner/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Main module."""
 from logging import Logger
 from pathlib import Path
-from typing import List, Optional
+from typing import Any, List, Optional
 
 from universal_data_permissions_scanner import (
     AwsAssumeRoleInput,
     AWSAuthzAnalyzer,
     BigQueryAuthzAnalyzer,
     MongoDBAtlasAuthzAnalyzer,
     MongoDBAuthzAnalyzer,
@@ -20,44 +20,45 @@
 
 
 def run_snowflake(
     logger: Logger,
     username: str,
     password: Optional[str],
     account: str,
-    host: str,
     warehouse: Optional[str],
     output_format: OutputFormat,
     output_path: Path,
     rsa_key: Optional[str],
     rsa_pass: Optional[str],
+    **kwargs: Any,
 ):
     """Run snowflake analyzer.
 
     Args:
         logger (Logger): Logger
         username (str): Username
         password (str): Password
         account (str): Snowflake account to analyzer
-        host (str): Snowflake host
         warehouse (str): Warehouse
         output_format (OutputFormat): Output format, CSV or JSON
         output_path (str): Where to write the output
+        kwargs:
+            host (str): Snowflake host
     """
     snowflake_analyzer = SnowflakeAuthzAnalyzer.connect(
-        host=host,
         username=username,
         password=password,
         warehouse=warehouse,
         account=account,
         output_path=output_path,
         output_format=output_format,
         logger=logger,
         rsa_key=rsa_key,
         rsa_pass=rsa_pass,
+        kwargs=kwargs,
     )
     snowflake_analyzer.run()
 
 
 # AWS S3 runner
 def run_aws_s3(
     logger: Logger,
```

### Comparing `udps-0.1.20/universal_data_permissions_scanner/models/model.py` & `udps-0.1.21/universal_data_permissions_scanner/models/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/utils/logger.py` & `udps-0.1.21/universal_data_permissions_scanner/utils/logger.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/writers/base_writers.py` & `udps-0.1.21/universal_data_permissions_scanner/writers/base_writers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/writers/csv_writer.py` & `udps-0.1.21/universal_data_permissions_scanner/writers/csv_writer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/writers/get_writers.py` & `udps-0.1.21/universal_data_permissions_scanner/writers/get_writers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/universal_data_permissions_scanner/writers/multi_json_exporter.py` & `udps-0.1.21/universal_data_permissions_scanner/writers/multi_json_exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.20/PKG-INFO` & `udps-0.1.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: udps
-Version: 0.1.20
+Version: 0.1.21
 Summary: Analyze authorization.
 Home-page: https://github.com/satoricyber/universal-data-permissions-scanner
 Author: SatoriCyber
-Requires-Python: >=3.8.1,<3.11
+Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: release
 Provides-Extra: test
 Requires-Dist: black (>=22.12.0,<23.0.0) ; extra == "test"
 Requires-Dist: boto3 (>=1.26.27,<2.0.0)
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "test"
 Requires-Dist: click (==8.1.3)
 Requires-Dist: databricks-cli (>=0.17.4,<0.18.0)
 Requires-Dist: google-api-python-client (>=2.66.0,<2.67.0)
 Requires-Dist: google-api-python-client-stubs (>=1.13.0,<2.0.0) ; extra == "test"
-Requires-Dist: google-cloud-bigquery (>=2.1.0,<3.0)
+Requires-Dist: google-cloud-bigquery (>=3.4.2)
 Requires-Dist: google-cloud-iam (>=2.10.0,<3.0.0)
 Requires-Dist: google-cloud-resource-manager (>=1.6.3,<2.0)
 Requires-Dist: isort (>=5.11.3,<6.0.0) ; extra == "test"
 Requires-Dist: markdown-it-py (>=2.2.0,<3.0.0)
 Requires-Dist: mkdocs (>=1.4.2,<2.0.0) ; extra == "release"
 Requires-Dist: mkdocs-include-markdown-plugin (>=4.0.3,<5.0.0) ; extra == "release"
 Requires-Dist: mkdocs-material (>=9.0.12,<10.0.0) ; extra == "release"
```

