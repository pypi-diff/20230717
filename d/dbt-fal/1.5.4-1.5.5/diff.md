# Comparing `tmp/dbt_fal-1.5.4.tar.gz` & `tmp/dbt_fal-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_fal-1.5.4.tar", max compression
+gzip compressed data, was "dbt_fal-1.5.5.tar", max compression
```

## Comparing `dbt_fal-1.5.4.tar` & `dbt_fal-1.5.5.tar`

### file list

```diff
@@ -1,45 +1,90 @@
--rw-r--r--   0        0        0     3009 2023-06-28 15:00:34.374002 dbt_fal-1.5.4/README.md
--rw-r--r--   0        0        0     1588 2023-06-28 15:00:45.601976 dbt_fal-1.5.4/pyproject.toml
--rw-r--r--   0        0        0      639 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal/__init__.py
--rw-r--r--   0        0        0       18 2023-06-28 15:00:46.069974 dbt_fal-1.5.4/src/dbt/adapters/fal/__version__.py
--rw-r--r--   0        0        0      392 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal/connections.py
--rw-r--r--   0        0        0     3369 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal/impl.py
--rw-r--r--   0        0        0     2768 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal/load_db_profile.py
--rw-r--r--   0        0        0     4091 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal/wrappers.py
--rw-r--r--   0        0        0      344 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/__init__.py
--rw-r--r--   0        0        0       18 2023-06-28 15:00:46.069974 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/__version__.py
--rw-r--r--   0        0        0     4820 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/adapter.py
--rw-r--r--   0        0        0     8381 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/adapter_support.py
--rw-r--r--   0        0        0     1627 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/connections.py
--rw-r--r--   0        0        0     8714 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/impl.py
--rw-r--r--   0        0        0     3192 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/support/athena.py
--rw-r--r--   0        0        0     2686 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/support/bigquery.py
--rw-r--r--   0        0        0      980 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/support/duckdb.py
--rw-r--r--   0        0        0     2977 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/support/postgres.py
--rw-r--r--   0        0        0     1633 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/support/redshift.py
--rw-r--r--   0        0        0     2781 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/support/snowflake.py
--rw-r--r--   0        0        0      821 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/support/trino.py
--rw-r--r--   0        0        0       25 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/telemetry/__init__.py
--rw-r--r--   0        0        0    10763 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/telemetry/telemetry.py
--rw-r--r--   0        0        0     6572 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/teleport.py
--rw-r--r--   0        0        0     1153 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/teleport_adapter_support.py
--rw-r--r--   0        0        0     4719 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py
--rw-r--r--   0        0        0     2972 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py
--rw-r--r--   0        0        0     1256 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/utils/__init__.py
--rw-r--r--   0        0        0     9804 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/utils/environments.py
--rw-r--r--   0        0        0     1970 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/utils/yaml_helper.py
--rw-r--r--   0        0        0      208 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/fal/adapters/python/__init__.py
--rw-r--r--   0        0        0    11898 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/fal/adapters/python/connections.py
--rw-r--r--   0        0        0    10015 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/fal/adapters/python/impl.py
--rw-r--r--   0        0        0      181 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/fal/adapters/teleport/__init__.py
--rw-r--r--   0        0        0     3498 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/fal/adapters/teleport/impl.py
--rw-r--r--   0        0        0     2310 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/fal/adapters/teleport/info.py
--rw-r--r--   0        0        0       52 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/include/fal/__init__.py
--rw-r--r--   0        0        0       70 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/include/fal/dbt_project.yml
--rw-r--r--   0        0        0     1213 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/include/fal/macros/materializations/table.sql
--rw-r--r--   0        0        0      265 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/include/fal/macros/teleport_duckdb.sql
--rw-r--r--   0        0        0      921 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/include/fal/macros/teleport_snowflake.sql
--rw-r--r--   0        0        0       52 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/include/fal_experimental/__init__.py
--rw-r--r--   0        0        0       83 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/include/fal_experimental/dbt_project.yml
--rw-r--r--   0        0        0      989 2023-06-28 15:00:34.378003 dbt_fal-1.5.4/src/dbt/include/fal_experimental/macros/materializations/table.sql
--rw-r--r--   0        0        0     4628 1970-01-01 00:00:00.000000 dbt_fal-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0    10531 2023-07-17 21:28:50.436197 dbt_fal-1.5.5/README.md
+-rw-r--r--   0        0        0     2356 2023-07-17 21:29:03.528260 dbt_fal-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0      639 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal/__init__.py
+-rw-r--r--   0        0        0       18 2023-07-17 21:29:04.036263 dbt_fal-1.5.5/src/dbt/adapters/fal/__version__.py
+-rw-r--r--   0        0        0      392 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal/connections.py
+-rw-r--r--   0        0        0     3369 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal/impl.py
+-rw-r--r--   0        0        0     2768 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal/load_db_profile.py
+-rw-r--r--   0        0        0     4091 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal/wrappers.py
+-rw-r--r--   0        0        0      344 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/__init__.py
+-rw-r--r--   0        0        0       18 2023-07-17 21:29:04.036263 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/__version__.py
+-rw-r--r--   0        0        0     4861 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/adapter.py
+-rw-r--r--   0        0        0     8381 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/adapter_support.py
+-rw-r--r--   0        0        0     1627 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/connections.py
+-rw-r--r--   0        0        0     8714 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/impl.py
+-rw-r--r--   0        0        0     3192 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/support/athena.py
+-rw-r--r--   0        0        0     2686 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/support/bigquery.py
+-rw-r--r--   0        0        0      980 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/support/duckdb.py
+-rw-r--r--   0        0        0     2977 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/support/postgres.py
+-rw-r--r--   0        0        0     1633 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/support/redshift.py
+-rw-r--r--   0        0        0     2781 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/support/snowflake.py
+-rw-r--r--   0        0        0      821 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/support/trino.py
+-rw-r--r--   0        0        0       25 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/telemetry/__init__.py
+-rw-r--r--   0        0        0    10767 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/telemetry/telemetry.py
+-rw-r--r--   0        0        0     6572 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/teleport.py
+-rw-r--r--   0        0        0     1153 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/teleport_adapter_support.py
+-rw-r--r--   0        0        0     4719 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py
+-rw-r--r--   0        0        0     2972 2023-07-17 21:28:50.448197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py
+-rw-r--r--   0        0        0     1256 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/utils/__init__.py
+-rw-r--r--   0        0        0     9804 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/utils/environments.py
+-rw-r--r--   0        0        0     1970 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/utils/yaml_helper.py
+-rw-r--r--   0        0        0      208 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/dbt/fal/adapters/python/__init__.py
+-rw-r--r--   0        0        0    11898 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/dbt/fal/adapters/python/connections.py
+-rw-r--r--   0        0        0    10015 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/dbt/fal/adapters/python/impl.py
+-rw-r--r--   0        0        0      181 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/dbt/fal/adapters/teleport/__init__.py
+-rw-r--r--   0        0        0     3498 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/dbt/fal/adapters/teleport/impl.py
+-rw-r--r--   0        0        0     2310 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/dbt/fal/adapters/teleport/info.py
+-rw-r--r--   0        0        0       52 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/dbt/include/fal/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/dbt/include/fal/dbt_project.yml
+-rw-r--r--   0        0        0     1213 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/dbt/include/fal/macros/materializations/table.sql
+-rw-r--r--   0        0        0      265 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/dbt/include/fal/macros/teleport_duckdb.sql
+-rw-r--r--   0        0        0      921 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/dbt/include/fal/macros/teleport_snowflake.sql
+-rw-r--r--   0        0        0       52 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/dbt/include/fal_experimental/__init__.py
+-rw-r--r--   0        0        0       83 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/dbt/include/fal_experimental/dbt_project.yml
+-rw-r--r--   0        0        0      989 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/dbt/include/fal_experimental/macros/materializations/table.sql
+-rw-r--r--   0        0        0     1829 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/__init__.py
+-rw-r--r--   0        0        0      238 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/cli/__init__.py
+-rw-r--r--   0        0        0     7458 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/cli/args.py
+-rw-r--r--   0        0        0     1432 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/cli/cli.py
+-rw-r--r--   0        0        0     5482 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/cli/dbt_runner.py
+-rw-r--r--   0        0        0     5857 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/cli/fal_runner.py
+-rw-r--r--   0        0        0     4475 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/cli/flow_runner.py
+-rw-r--r--   0        0        0       56 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/cli/model_generator/__init__.py
+-rw-r--r--   0        0        0     5543 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/cli/model_generator/model_generator.py
+-rw-r--r--   0        0        0     3180 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/cli/model_generator/module_check.py
+-rw-r--r--   0        0        0     9759 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/cli/selectors.py
+-rw-r--r--   0        0        0    12349 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/fal_script.py
+-rw-r--r--   0        0        0        0 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/feature_store/__init__.py
+-rw-r--r--   0        0        0      401 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/feature_store/feature.py
+-rw-r--r--   0        0        0        0 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/integration/__init__.py
+-rw-r--r--   0        0        0    24589 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/integration/lib.py
+-rw-r--r--   0        0        0     3273 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/integration/logger.py
+-rw-r--r--   0        0        0     1867 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/integration/magics.py
+-rw-r--r--   0        0        0     9103 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/integration/parse.py
+-rw-r--r--   0        0        0    27168 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/integration/project.py
+-rw-r--r--   0        0        0        0 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/integration/utils/__init__.py
+-rw-r--r--   0        0        0     1970 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/integration/utils/yaml_helper.py
+-rw-r--r--   0        0        0      317 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/integration/version.py
+-rw-r--r--   0        0        0     1530 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/new/project.py
+-rw-r--r--   0        0        0     8411 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/node_graph.py
+-rw-r--r--   0        0        0        0 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/packages/__init__.py
+-rw-r--r--   0        0        0     1603 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/packages/bridge.py
+-rw-r--r--   0        0        0     4948 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/packages/dependency_analysis.py
+-rw-r--r--   0        0        0      805 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/packages/environments/__init__.py
+-rw-r--r--   0        0        0     9499 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/packages/environments/base.py
+-rw-r--r--   0        0        0     4407 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/packages/environments/conda.py
+-rw-r--r--   0        0        0     3381 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/packages/environments/virtual_env.py
+-rw-r--r--   0        0        0     4823 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/packages/isolated_runner.py
+-rw-r--r--   0        0        0        0 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/planner/__init__.py
+-rw-r--r--   0        0        0     5669 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/planner/executor.py
+-rw-r--r--   0        0        0     6496 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/planner/plan.py
+-rw-r--r--   0        0        0     6790 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/planner/schedule.py
+-rw-r--r--   0        0        0     9079 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/planner/tasks.py
+-rw-r--r--   0        0        0        0 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/telemetry/__init__.py
+-rw-r--r--   0        0        0    11441 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/telemetry/telemetry.py
+-rw-r--r--   0        0        0     3060 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/typing.py
+-rw-r--r--   0        0        0     1728 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/src/fal/dbt/utils.py
+-rw-r--r--   0        0        0       33 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/tests/_fal_testing/__init__.py
+-rw-r--r--   0        0        0     1794 2023-07-17 21:28:50.452197 dbt_fal-1.5.5/tests/_fal_testing/utils.py
+-rw-r--r--   0        0        0    12556 1970-01-01 00:00:00.000000 dbt_fal-1.5.5/PKG-INFO
```

### Comparing `dbt_fal-1.5.4/pyproject.toml` & `dbt_fal-1.5.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,99 @@
 [tool.poetry]
 name = "dbt-fal"
-version = "1.5.4"
-description = "Simplest way to run dbt python models."
+version = "1.5.5"
+description = "Run python scripts from any dbt project."
 readme = "README.md"
-homepage = "https://github.com/fal-ai/fal/blob/-/projects/adapter"
+homepage = "https://github.com/fal-ai/fal"
 repository = "https://github.com/fal-ai/fal"
 authors = [ "Features & Labels <hello@fal.ai>" ]
 packages = [
-    { include = "dbt", from = "src" }
+    { include = "dbt", from = "src" },
+    # cli package
+    { include = "fal", from = "src" },
+    { include = "_fal_testing", from = "tests" },
 ]
 
 keywords = [ "dbt", "pandas", "fal", "runtime" ]
 classifiers = [
     "Development Status :: 4 - Beta"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.2, <3.12"
-dbt-core = ">=1.5.0, <1.6"
-posthog = "^1.4.5"
+dbt-core = ">=1.5,<=1.5.1"
 pandas = "^1.3.4"
+posthog = "^1.4.5"
 "backports.functools_lru_cache" = "^1.6.4"
+
+# cli
+PyYAML = "^6.0"
+agate-sql = "^0.5.8"
+astor = "^0.8.1"
+deprecation = "^2.1.0"
+
+## Environment management related dependencies
+## TODO use fal-serverless instead
+platformdirs = "^2.5.2"
+virtualenv = "^20.16.2"
+dill = ">=0.3.6,<0.3.7"
+
+# dbt-fal
 sqlalchemy = "^1.4.41"
 
 # Adapters
 
 ## snowflake
 snowflake-connector-python = { version = "~=3.0", extras = ["pandas"], optional = true }
 
 ## bigquery
 ### version defined by dbt-bigquery, installs pyarrow<8
 google-cloud-bigquery = { version = "~3.5.0", extras = ["pandas"], optional = true }
 
 ## redshift
 awswrangler = { version = ">=3.0.0", extras = ["redshift"], optional = true, python = ">=3.8" }
+sqlalchemy-redshift = { version = "^0.8.9", optional = true }
+
+## duckdb
+duckdb-engine = { version = "^0.1.8", optional = true }
 
 ## trino
 trino = { version = "~0.321.0", extras = ["sqlalchemy"], optional = true }
 
 # teleport
 s3fs = { version = ">=2022.8.2", optional = true }
 
 # fal cloud
 packaging = ">=23"
 fal-serverless = "^0.6.35"
 importlib-metadata = "^6.0.0"
 
-[tool.poetry.dev-dependencies]
-pytest = "^5.2"
-
 [tool.poetry.extras]
 postgres = []
 snowflake = ["snowflake-connector-python"]
 bigquery = ["google-cloud-bigquery"]
-redshift = ["awswrangler"]
-duckdb = []
+redshift = ["awswrangler", "sqlalchemy-redshift"]
+duckdb = ["duckdb-engine"]
 athena = []
 trino = ["trino"]
 teleport = ["s3fs"]
 
+[tool.poetry.group.dev]
+optional = true
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^5.2"
+black = "^22.3"
+behave = "^1.2.6"
+mock = "^4.0.3"
+pytest-mock = "^3.7.0"
+matplotlib = "^3.5.2"
+requests = "^2.27.1"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+dbt-fal = "fal.dbt.cli:cli"
+# NOTE: deprecated use
+fal = "fal.dbt.cli:fal_cli"
```

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal/__init__.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal/impl.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal/load_db_profile.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal/load_db_profile.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal/wrappers.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal/wrappers.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/adapter.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,38 +108,42 @@
         local_packages=compressed_local_packages
     )
 
     if environment.kind == "local":
         result = execute_model()
         return result
 
+    extra = {}
+    if is_remote:
+        # Machine type is only applicable in FalServerlesshost
+        extra = {"machine_type": environment.machine_type}
+
     if environment.kind == "virtualenv":
         requirements = environment.config.get("requirements", [])
         requirements += deps
         isolated_function = isolated(
             kind="virtualenv",
             host=environment.host,
-            requirements=requirements
+            requirements=requirements,
+            **extra
         )(execute_model)
     elif environment.kind == "conda":
         dependencies = environment.config.pop("packages", [])
         dependencies.append({"pip": deps})
         env_dict = {
             "name": "dbt_fal_env",
             "channels": ["conda-forge", "defaults"],
             "dependencies": dependencies
         }
         isolated_function = isolated(
             kind="conda",
             host=environment.host,
-            env_dict=env_dict)(execute_model)
+            env_dict=env_dict,
+            **extra
+        )(execute_model)
     else:
         # We should not reach this point, because environment types are validated when the
         # environment objects are created (in utils/environments.py).
         raise Exception(f"Environment type not supported: {environment.kind}")
 
-    # Machine type is only applicable in FalServerlesshost
-    if is_remote:
-        isolated_function = isolated_function.on(machine_type=environment.machine_type)
-
     result = isolated_function()
     return result
```

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/adapter_support.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/adapter_support.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/connections.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/impl.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/support/athena.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/support/athena.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/support/bigquery.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/support/bigquery.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/support/duckdb.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/support/duckdb.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/support/postgres.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/support/postgres.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/support/redshift.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/support/redshift.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/support/snowflake.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/support/snowflake.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/support/trino.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/support/trino.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/telemetry/telemetry.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/telemetry/telemetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     target = config.to_target_dict()
     return target["type"]
 
 
 def fal_installed_version():
     """Returns: fal version"""
     try:
-        return pkg_resources.get_distribution("fal").version
+        return pkg_resources.get_distribution("dbt-fal").version
     except ImportError:
         return
 
 
 def is_airflow():
     """Returns: True for Airflow env"""
     return "AIRFLOW_CONFIG" in os.environ or "AIRFLOW_HOME" in os.environ
```

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/teleport.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/teleport.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/teleport_adapter_support.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/teleport_adapter_support.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/utils/__init__.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/utils/environments.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/utils/environments.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/adapters/fal_experimental/utils/yaml_helper.py` & `dbt_fal-1.5.5/src/dbt/adapters/fal_experimental/utils/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/fal/adapters/python/connections.py` & `dbt_fal-1.5.5/src/dbt/fal/adapters/python/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/fal/adapters/python/impl.py` & `dbt_fal-1.5.5/src/dbt/fal/adapters/python/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/fal/adapters/teleport/impl.py` & `dbt_fal-1.5.5/src/dbt/fal/adapters/teleport/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/fal/adapters/teleport/info.py` & `dbt_fal-1.5.5/src/dbt/fal/adapters/teleport/info.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/include/fal/macros/materializations/table.sql` & `dbt_fal-1.5.5/src/dbt/include/fal/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/include/fal/macros/teleport_snowflake.sql` & `dbt_fal-1.5.5/src/dbt/include/fal/macros/teleport_snowflake.sql`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.4/src/dbt/include/fal_experimental/macros/materializations/table.sql` & `dbt_fal-1.5.5/src/dbt/include/fal_experimental/macros/materializations/table.sql`

 * *Files identical despite different names*

