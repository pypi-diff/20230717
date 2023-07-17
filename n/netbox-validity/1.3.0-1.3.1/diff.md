# Comparing `tmp/netbox-validity-1.3.0.tar.gz` & `tmp/netbox-validity-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-validity-1.3.0.tar", last modified: Mon Jun  5 21:12:16 2023, max compression
+gzip compressed data, was "netbox-validity-1.3.1.tar", last modified: Mon Jul 17 20:29:55 2023, max compression
```

## Comparing `netbox-validity-1.3.0.tar` & `netbox-validity-1.3.1.tar`

### file list

```diff
@@ -1,142 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.610605 netbox-validity-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-06-05 21:12:16.610605 netbox-validity-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.594604 netbox-validity-1.3.0/netbox_validity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-06-05 21:12:16.000000 netbox-validity-1.3.0/netbox_validity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-05 21:12:16.000000 netbox-validity-1.3.0/netbox_validity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:12:16.000000 netbox-validity-1.3.0/netbox_validity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-05 21:12:16.000000 netbox-validity-1.3.0/netbox_validity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 21:12:16.000000 netbox-validity-1.3.0/netbox_validity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.598604 netbox-validity-1.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:12:16.610605 netbox-validity-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.598604 netbox-validity-1.3.0/validity/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.598604 netbox-validity-1.3.0/validity/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.598604 netbox-validity-1.3.0/validity/config_compliance/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.598604 netbox-validity-1.3.0/validity/config_compliance/device_config/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/device_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/device_config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/device_config/routeros.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/device_config/ttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/device_config/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/dynamic_pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.598604 netbox-validity-1.3.0/validity/config_compliance/eval/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/eval/default_nameset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/eval/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/eval/eval_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.602604 netbox-validity-1.3.0/validity/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/forms/filterset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/forms/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/forms/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.602604 netbox-validity-1.3.0/validity/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.602604 netbox-validity-1.3.0/validity/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/management/commands/linkscripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.602604 netbox-validity-1.3.0/validity/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/migrations/0002_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/migrations/0003_complianceselector_dp_tag_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/migrations/0004_netbox35_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.602604 netbox-validity-1.3.0/validity/models/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/nameset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.602604 netbox-validity-1.3.0/validity/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/scripts/validity_git.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/scripts/validity_run_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.594604 netbox-validity-1.3.0/validity/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/templates/validity/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/aux_tab_table.html
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/compliance_results.html
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/compliancereport.html
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/complianceselector.html
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/compliancetest.html
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/compliancetestresult.html
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/configserializer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/device_config.html
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/gitrepo.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/templates/validity/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/inc/git_link.html
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/inc/path_with_link.html
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/inc/prism.html
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/inc/report_stats_row.html
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/inc/search_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/nameset.html
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/report_devices.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templatetags/validity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_choices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/tests/test_config_compliance/
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_config_compliance/test_device_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_config_compliance/test_dynamic_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_config_compliance/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/tests/test_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_models/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_models/test_git_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_models/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_models/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_models/test_vdevice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/tests/test_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_scripts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_scripts/test_run_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_utils/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/utils/password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.610605 netbox-validity-1.3.0/validity/views/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/nameset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/test_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.382261 netbox-validity-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-17 20:29:55.382261 netbox-validity-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.358261 netbox-validity-1.3.1/netbox_validity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-17 20:29:55.000000 netbox-validity-1.3.1/netbox_validity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-17 20:29:55.000000 netbox-validity-1.3.1/netbox_validity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:29:55.000000 netbox-validity-1.3.1/netbox_validity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-17 20:29:55.000000 netbox-validity-1.3.1/netbox_validity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 20:29:55.000000 netbox-validity-1.3.1/netbox_validity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.358261 netbox-validity-1.3.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:29:55.386261 netbox-validity-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.362261 netbox-validity-1.3.1/validity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.362261 netbox-validity-1.3.1/validity/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.362261 netbox-validity-1.3.1/validity/config_compliance/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.366261 netbox-validity-1.3.1/validity/config_compliance/device_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/config_compliance/device_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/config_compliance/device_config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/config_compliance/device_config/routeros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/config_compliance/device_config/ttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/config_compliance/device_config/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/config_compliance/dynamic_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.366261 netbox-validity-1.3.1/validity/config_compliance/eval/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/config_compliance/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/config_compliance/eval/default_nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/config_compliance/eval/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/config_compliance/eval/eval_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/config_compliance/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.366261 netbox-validity-1.3.1/validity/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/forms/filterset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/forms/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/forms/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.366261 netbox-validity-1.3.1/validity/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.366261 netbox-validity-1.3.1/validity/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/management/commands/linkscripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.366261 netbox-validity-1.3.1/validity/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/migrations/0002_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/migrations/0003_complianceselector_dp_tag_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/migrations/0004_netbox35_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.370261 netbox-validity-1.3.1/validity/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/models/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/models/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/models/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/models/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/models/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/models/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/models/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/models/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.370261 netbox-validity-1.3.1/validity/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/scripts/validity_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/scripts/validity_run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.354261 netbox-validity-1.3.1/validity/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.370261 netbox-validity-1.3.1/validity/static/validity/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/static/validity/prism-dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/static/validity/prism-light.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/static/validity/prism.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.354261 netbox-validity-1.3.1/validity/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.374261 netbox-validity-1.3.1/validity/templates/validity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templates/validity/aux_tab_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templates/validity/compliance_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templates/validity/compliancereport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templates/validity/complianceselector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templates/validity/compliancetest.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templates/validity/compliancetestresult.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templates/validity/configserializer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templates/validity/device_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templates/validity/gitrepo.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.374261 netbox-validity-1.3.1/validity/templates/validity/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templates/validity/inc/git_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templates/validity/inc/path_with_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templates/validity/inc/prism.html
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templates/validity/inc/report_stats_row.html
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templates/validity/inc/search_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templates/validity/nameset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templates/validity/report_devices.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.374261 netbox-validity-1.3.1/validity/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/templatetags/validity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.378261 netbox-validity-1.3.1/validity/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/test_choices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.378261 netbox-validity-1.3.1/validity/tests/test_config_compliance/
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/test_config_compliance/test_device_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/test_config_compliance/test_dynamic_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/test_config_compliance/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/test_graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.378261 netbox-validity-1.3.1/validity/tests/test_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/test_models/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/test_models/test_git_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/test_models/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/test_models/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/test_models/test_vdevice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.378261 netbox-validity-1.3.1/validity/tests/test_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/test_scripts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/test_scripts/test_run_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.382261 netbox-validity-1.3.1/validity/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/test_utils/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/test_utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.382261 netbox-validity-1.3.1/validity/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/utils/password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:29:55.382261 netbox-validity-1.3.1/validity/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/views/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/views/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/views/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/views/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/views/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/views/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/views/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-17 20:29:41.000000 netbox-validity-1.3.1/validity/views/test_result.py
```

### Comparing `netbox-validity-1.3.0/LICENSE` & `netbox-validity-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/PKG-INFO` & `netbox-validity-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 1.3.0
+Version: 1.3.1
 Summary: NetBox plugin for vendor-agnostic configuration compliance
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netbox-validity Version: 1.3.0 Summary: NetBox
+Metadata-Version: 2.1 Name: netbox-validity Version: 1.3.1 Summary: NetBox
 plugin for vendor-agnostic configuration compliance Author-email: Anton
 Miasnikov
 gmail.com> License: MIT License Copyright (c) 2023 Anton Miasnikov Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

### Comparing `netbox-validity-1.3.0/README.md` & `netbox-validity-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/netbox_validity.egg-info/PKG-INFO` & `netbox-validity-1.3.1/netbox_validity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 1.3.0
+Version: 1.3.1
 Summary: NetBox plugin for vendor-agnostic configuration compliance
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netbox-validity Version: 1.3.0 Summary: NetBox
+Metadata-Version: 2.1 Name: netbox-validity Version: 1.3.1 Summary: NetBox
 plugin for vendor-agnostic configuration compliance Author-email: Anton
 Miasnikov
 gmail.com> License: MIT License Copyright (c) 2023 Anton Miasnikov Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

### Comparing `netbox-validity-1.3.0/netbox_validity.egg-info/SOURCES.txt` & `netbox-validity-1.3.1/netbox_validity.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,17 @@
 validity/models/selector.py
 validity/models/serializer.py
 validity/models/test.py
 validity/models/test_result.py
 validity/scripts/__init__.py
 validity/scripts/validity_git.py
 validity/scripts/validity_run_tests.py
+validity/static/validity/prism-dark.css
+validity/static/validity/prism-light.css
+validity/static/validity/prism.js
 validity/templates/validity/aux_tab_table.html
 validity/templates/validity/compliance_results.html
 validity/templates/validity/compliancereport.html
 validity/templates/validity/complianceselector.html
 validity/templates/validity/compliancetest.html
 validity/templates/validity/compliancetestresult.html
 validity/templates/validity/configserializer.html
```

### Comparing `netbox-validity-1.3.0/pyproject.toml` & `netbox-validity-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-validity"
-version = "1.3.0"
+version = "1.3.1"
 description = "NetBox plugin for vendor-agnostic configuration compliance"
 authors = [
     {name = "Anton Miasnikov", email = "anton2008m@gmail.com"},
 ]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `netbox-validity-1.3.0/validity/__init__.py` & `netbox-validity-1.3.1/validity/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class NetBoxValidityConfig(PluginConfig):
     name = "validity"
     verbose_name = "Validity: Configuration Compliance"
     description = "Vendor-agnostic framework to build your own configuration compliance rule set"
     author = "Anton Miasnikov"
     author_email = "anton2008m@gmail.com"
-    version = "1.3.0"
+    version = "1.3.1"
     base_url = "validity"
     django_apps = ["bootstrap5"]
     min_version = "3.4.0"
 
     # custom field
     netbox_version = NetboxVersion(VERSION)
```

### Comparing `netbox-validity-1.3.0/validity/api/helpers.py` & `netbox-validity-1.3.1/validity/api/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/api/serializers.py` & `netbox-validity-1.3.1/validity/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/api/urls.py` & `netbox-validity-1.3.1/validity/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/api/views.py` & `netbox-validity-1.3.1/validity/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/choices.py` & `netbox-validity-1.3.1/validity/choices.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/config_compliance/device_config/base.py` & `netbox-validity-1.3.1/validity/config_compliance/device_config/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/config_compliance/device_config/routeros.py` & `netbox-validity-1.3.1/validity/config_compliance/device_config/routeros.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/config_compliance/device_config/ttp.py` & `netbox-validity-1.3.1/validity/config_compliance/device_config/ttp.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/config_compliance/device_config/yaml.py` & `netbox-validity-1.3.1/validity/config_compliance/device_config/yaml.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/config_compliance/dynamic_pairs.py` & `netbox-validity-1.3.1/validity/config_compliance/dynamic_pairs.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/config_compliance/eval/default_nameset.py` & `netbox-validity-1.3.1/validity/config_compliance/eval/default_nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/config_compliance/eval/eval.py` & `netbox-validity-1.3.1/validity/config_compliance/eval/eval.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/config_compliance/eval/eval_defaults.py` & `netbox-validity-1.3.1/validity/config_compliance/eval/eval_defaults.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/filtersets.py` & `netbox-validity-1.3.1/validity/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/forms/filterset.py` & `netbox-validity-1.3.1/validity/forms/filterset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/forms/general.py` & `netbox-validity-1.3.1/validity/forms/general.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/forms/helpers.py` & `netbox-validity-1.3.1/validity/forms/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/graphql.py` & `netbox-validity-1.3.1/validity/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/management/commands/linkscripts.py` & `netbox-validity-1.3.1/validity/management/commands/linkscripts.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/managers.py` & `netbox-validity-1.3.1/validity/managers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/migrations/0001_initial.py` & `netbox-validity-1.3.1/validity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/migrations/0002_custom_fields.py` & `netbox-validity-1.3.1/validity/migrations/0002_custom_fields.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/migrations/0004_netbox35_scripts.py` & `netbox-validity-1.3.1/validity/migrations/0004_netbox35_scripts.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/models/base.py` & `netbox-validity-1.3.1/validity/models/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/models/device.py` & `netbox-validity-1.3.1/validity/models/device.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/models/nameset.py` & `netbox-validity-1.3.1/validity/models/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/models/repo.py` & `netbox-validity-1.3.1/validity/models/repo.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/models/selector.py` & `netbox-validity-1.3.1/validity/models/selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/models/serializer.py` & `netbox-validity-1.3.1/validity/models/serializer.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/models/test.py` & `netbox-validity-1.3.1/validity/models/test.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/models/test_result.py` & `netbox-validity-1.3.1/validity/models/test_result.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/navigation.py` & `netbox-validity-1.3.1/validity/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/scripts/validity_git.py` & `netbox-validity-1.3.1/validity/scripts/validity_git.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/scripts/validity_run_tests.py` & `netbox-validity-1.3.1/validity/scripts/validity_run_tests.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/search.py` & `netbox-validity-1.3.1/validity/search.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tables.py` & `netbox-validity-1.3.1/validity/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/templates/validity/aux_tab_table.html` & `netbox-validity-1.3.1/validity/templates/validity/aux_tab_table.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/templates/validity/compliancereport.html` & `netbox-validity-1.3.1/validity/templates/validity/compliancereport.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/templates/validity/complianceselector.html` & `netbox-validity-1.3.1/validity/templates/validity/complianceselector.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/templates/validity/compliancetest.html` & `netbox-validity-1.3.1/validity/templates/validity/compliancetest.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/templates/validity/compliancetestresult.html` & `netbox-validity-1.3.1/validity/templates/validity/compliancetestresult.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/templates/validity/configserializer.html` & `netbox-validity-1.3.1/validity/templates/validity/configserializer.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/templates/validity/device_config.html` & `netbox-validity-1.3.1/validity/templates/validity/device_config.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/templates/validity/gitrepo.html` & `netbox-validity-1.3.1/validity/templates/validity/gitrepo.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/templates/validity/nameset.html` & `netbox-validity-1.3.1/validity/templates/validity/nameset.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/templatetags/validity.py` & `netbox-validity-1.3.1/validity/templatetags/validity.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/base.py` & `netbox-validity-1.3.1/validity/tests/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/conftest.py` & `netbox-validity-1.3.1/validity/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/factories.py` & `netbox-validity-1.3.1/validity/tests/factories.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/test_api.py` & `netbox-validity-1.3.1/validity/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/test_choices.py` & `netbox-validity-1.3.1/validity/tests/test_choices.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/test_config_compliance/test_device_config.py` & `netbox-validity-1.3.1/validity/tests/test_config_compliance/test_device_config.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/test_config_compliance/test_dynamic_pairs.py` & `netbox-validity-1.3.1/validity/tests/test_config_compliance/test_dynamic_pairs.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/test_config_compliance/test_eval.py` & `netbox-validity-1.3.1/validity/tests/test_config_compliance/test_eval.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/test_graphql.py` & `netbox-validity-1.3.1/validity/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/test_models/test_clean.py` & `netbox-validity-1.3.1/validity/tests/test_models/test_clean.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/test_models/test_git_link.py` & `netbox-validity-1.3.1/validity/tests/test_models/test_git_link.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/test_models/test_git_repo.py` & `netbox-validity-1.3.1/validity/tests/test_models/test_git_repo.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/test_models/test_selector.py` & `netbox-validity-1.3.1/validity/tests/test_models/test_selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/test_models/test_vdevice.py` & `netbox-validity-1.3.1/validity/tests/test_models/test_vdevice.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/test_scripts/test_run_tests.py` & `netbox-validity-1.3.1/validity/tests/test_scripts/test_run_tests.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/test_utils/test_git.py` & `netbox-validity-1.3.1/validity/tests/test_utils/test_git.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/test_utils/test_misc.py` & `netbox-validity-1.3.1/validity/tests/test_utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/tests/test_views.py` & `netbox-validity-1.3.1/validity/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/urls.py` & `netbox-validity-1.3.1/validity/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/utils/git.py` & `netbox-validity-1.3.1/validity/utils/git.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/utils/misc.py` & `netbox-validity-1.3.1/validity/utils/misc.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/utils/password.py` & `netbox-validity-1.3.1/validity/utils/password.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/views/__init__.py` & `netbox-validity-1.3.1/validity/views/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/views/base.py` & `netbox-validity-1.3.1/validity/views/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/views/device.py` & `netbox-validity-1.3.1/validity/views/device.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/views/git_repo.py` & `netbox-validity-1.3.1/validity/views/git_repo.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/views/nameset.py` & `netbox-validity-1.3.1/validity/views/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/views/report.py` & `netbox-validity-1.3.1/validity/views/report.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/views/selector.py` & `netbox-validity-1.3.1/validity/views/selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/views/serializer.py` & `netbox-validity-1.3.1/validity/views/serializer.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/views/test.py` & `netbox-validity-1.3.1/validity/views/test.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.3.0/validity/views/test_result.py` & `netbox-validity-1.3.1/validity/views/test_result.py`

 * *Files identical despite different names*

