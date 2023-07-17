# Comparing `tmp/harness-featureflags-1.2.1.tar.gz` & `tmp/harness-featureflags-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harness-featureflags-1.2.1.tar", last modified: Tue Jul  4 17:04:29 2023, max compression
+gzip compressed data, was "harness-featureflags-1.2.2.tar", last modified: Mon Jul 17 13:59:54 2023, max compression
```

## Comparing `harness-featureflags-1.2.1.tar` & `harness-featureflags-1.2.2.tar`

### file list

```diff
@@ -1,239 +1,239 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.685721 harness-featureflags-1.2.1/
--rw-r--r--   0 root         (0) root         (0)      163 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     3655 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/HISTORY.rst
--rw-r--r--   0 root         (0) root         (0)      585 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      262 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5307 2023-07-04 17:04:29.685721 harness-featureflags-1.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4373 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.657719 harness-featureflags-1.2.1/docs/
--rw-r--r--   0 root         (0) root         (0)      621 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/authors.rst
--rwxr-xr-x   0 root         (0) root         (0)     4958 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)       33 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/contributing.rst
--rw-r--r--   0 root         (0) root         (0)     1753 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/featureflags.api.default.rst
--rw-r--r--   0 root         (0) root         (0)      591 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/featureflags.api.rst
--rw-r--r--   0 root         (0) root         (0)      183 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/featureflags.client.rst
--rw-r--r--   0 root         (0) root         (0)      195 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/featureflags.evaluation.rst
--rw-r--r--   0 root         (0) root         (0)     3689 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/featureflags.evaluations.rst
--rw-r--r--   0 root         (0) root         (0)     1378 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/featureflags.ftypes.rst
--rw-r--r--   0 root         (0) root         (0)     2781 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/featureflags.models.rst
--rw-r--r--   0 root         (0) root         (0)     1916 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/featureflags.rest.api.default.rst
--rw-r--r--   0 root         (0) root         (0)      263 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/featureflags.rest.api.rst
--rw-r--r--   0 root         (0) root         (0)     4302 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/featureflags.rest.models.rst
--rw-r--r--   0 root         (0) root         (0)      621 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/featureflags.rest.rst
--rw-r--r--   0 root         (0) root         (0)     1853 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/featureflags.rst
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/history.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.657719 harness-featureflags-1.2.1/docs/images/
--rw-r--r--   0 root         (0) root         (0)   100515 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/images/ff-gui.png
--rw-r--r--   0 root         (0) root         (0)      333 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     1215 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      782 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/modules.rst
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/readme.rst
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/docs/usage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.661719 harness-featureflags-1.2.1/featureflags/
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12117 2023-07-04 17:03:05.000000 harness-featureflags-1.2.1/featureflags/analytics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.662719 harness-featureflags-1.2.1/featureflags/api/
--rw-r--r--   0 root         (0) root         (0)      173 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/api/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.663720 harness-featureflags-1.2.1/featureflags/api/default/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/api/default/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-07-04 17:03:04.000000 harness-featureflags-1.2.1/featureflags/api/default/authenticate.py
--rw-r--r--   0 root         (0) root         (0)     2872 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/api/default/get_all_segments.py
--rw-r--r--   0 root         (0) root         (0)     2995 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/api/default/get_feature_config.py
--rw-r--r--   0 root         (0) root         (0)     2943 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/api/default/get_feature_config_by_identifier.py
--rw-r--r--   0 root         (0) root         (0)     2538 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/api/default/get_segment_by_identifier.py
--rw-r--r--   0 root         (0) root         (0)     1907 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/api/default/post_metrics.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/api/default/stream.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/api/types.py
--rw-r--r--   0 root         (0) root         (0)     9676 2023-07-04 17:03:04.000000 harness-featureflags-1.2.1/featureflags/client.py
--rw-r--r--   0 root         (0) root         (0)     2603 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.666720 harness-featureflags-1.2.1/featureflags/evaluations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2878 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/auth_target.py
--rw-r--r--   0 root         (0) root         (0)     3892 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/clause.py
--rw-r--r--   0 root         (0) root         (0)      273 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/constants.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/distribution.py
--rw-r--r--   0 root         (0) root         (0)      124 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/enum.py
--rw-r--r--   0 root         (0) root         (0)    13944 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/evaluator.py
--rw-r--r--   0 root         (0) root         (0)     9128 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/feature.py
--rw-r--r--   0 root         (0) root         (0)     1548 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/prerequisite.py
--rw-r--r--   0 root         (0) root         (0)     5429 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/segment.py
--rw-r--r--   0 root         (0) root         (0)     2063 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/serve.py
--rw-r--r--   0 root         (0) root         (0)     3165 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/serving_rule.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/strategy.py
--rw-r--r--   0 root         (0) root         (0)     1544 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/tag.py
--rw-r--r--   0 root         (0) root         (0)     4378 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/target.py
--rw-r--r--   0 root         (0) root         (0)     1339 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/target_attributes.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/target_map.py
--rw-r--r--   0 root         (0) root         (0)     5352 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/variation.py
--rw-r--r--   0 root         (0) root         (0)     2564 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/variation_map.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/evaluations/weighted_variation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.667720 harness-featureflags-1.2.1/featureflags/ftypes/
--rw-r--r--   0 root         (0) root         (0)      242 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/ftypes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/ftypes/boolean.py
--rw-r--r--   0 root         (0) root         (0)     1304 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/ftypes/integer.py
--rw-r--r--   0 root         (0) root         (0)     2469 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/ftypes/interface.py
--rw-r--r--   0 root         (0) root         (0)     1009 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/ftypes/json.py
--rw-r--r--   0 root         (0) root         (0)     1317 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/ftypes/number.py
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/ftypes/string.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/ftypes/utils.py
--rw-r--r--   0 root         (0) root         (0)     1041 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/interface.py
--rw-r--r--   0 root         (0) root         (0)     1218 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/lru_cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.669720 harness-featureflags-1.2.1/featureflags/models/
--rw-r--r--   0 root         (0) root         (0)      809 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/models/authentication_request.py
--rw-r--r--   0 root         (0) root         (0)     2708 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/models/authentication_request_target.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/models/authentication_request_target_attributes.py
--rw-r--r--   0 root         (0) root         (0)     1421 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/models/authentication_response.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/models/error.py
--rw-r--r--   0 root         (0) root         (0)     1421 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/models/key_value.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/models/message.py
--rw-r--r--   0 root         (0) root         (0)     2827 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/models/metrics.py
--rw-r--r--   0 root         (0) root         (0)     2372 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/models/metrics_data.py
--rw-r--r--   0 root         (0) root         (0)      155 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/models/metrics_data_metrics_type.py
--rw-r--r--   0 root         (0) root         (0)     2131 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/models/pagination.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/models/target_data.py
--rw-r--r--   0 root         (0) root         (0)       92 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/models/unset.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/persisting.py
--rw-r--r--   0 root         (0) root         (0)     4963 2023-07-04 17:03:04.000000 harness-featureflags-1.2.1/featureflags/polling.py
--rw-r--r--   0 root         (0) root         (0)     8198 2023-07-04 17:03:04.000000 harness-featureflags-1.2.1/featureflags/repository.py
--rw-r--r--   0 root         (0) root         (0)     4298 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/sdk_logging_codes.py
--rw-r--r--   0 root         (0) root         (0)     7069 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/sse_client.py
--rw-r--r--   0 root         (0) root         (0)     6712 2023-07-04 17:03:04.000000 harness-featureflags-1.2.1/featureflags/streaming.py
--rw-r--r--   0 root         (0) root         (0)      151 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/featureflags/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.669720 harness-featureflags-1.2.1/harness_featureflags.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5307 2023-07-04 17:04:29.000000 harness-featureflags-1.2.1/harness_featureflags.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15040 2023-07-04 17:04:29.000000 harness-featureflags-1.2.1/harness_featureflags.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 17:04:29.000000 harness-featureflags-1.2.1/harness_featureflags.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 17:04:29.000000 harness-featureflags-1.2.1/harness_featureflags.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       86 2023-07-04 17:04:29.000000 harness-featureflags-1.2.1/harness_featureflags.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 17:04:29.000000 harness-featureflags-1.2.1/harness_featureflags.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      454 2023-07-04 17:04:29.686721 harness-featureflags-1.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.669720 harness-featureflags-1.2.1/tests/
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.670720 harness-featureflags-1.2.1/tests/integration/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.672720 harness-featureflags-1.2.1/tests/integration/ff-test-cases/
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/.git
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.602716 harness-featureflags-1.2.1/tests/integration/ff-test-cases/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.672720 harness-featureflags-1.2.1/tests/integration/ff-test-cases/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      333 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/.github/workflows/ci.yml
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2746 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/Makefile
--rw-r--r--   0 root         (0) root         (0)     3334 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/README.md
--rw-r--r--   0 root         (0) root         (0)    15527 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/client-v1.yaml
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/go.mod
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.673720 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.675720 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/
--rw-r--r--   0 root         (0) root         (0)    16904 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Bool_State_Disabled_On_False_Off_False_Should_Return_False.json
--rw-r--r--   0 root         (0) root         (0)    16898 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Bool_State_Disabled_On_False_Off_True_Should_Return_True.json
--rw-r--r--   0 root         (0) root         (0)    16901 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Bool_State_Disabled_On_True_Off_False_Should_Return_False.json
--rw-r--r--   0 root         (0) root         (0)    16895 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Bool_State_Disabled_On_True_Off_True_Should_Return_True.json
--rw-r--r--   0 root         (0) root         (0)    17222 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_JSON_State_Disabled_On_complexJSON_Off_emptyJSON_Should_Return_validJSON.json
--rw-r--r--   0 root         (0) root         (0)    17197 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_JSON_State_Disabled_On_validJSON_Off_emptyJSON_Should_Return_emptyJSON.json
--rw-r--r--   0 root         (0) root         (0)    17019 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Number_State_Disabled_On_011_Off_2_Should_Return_2.json
--rw-r--r--   0 root         (0) root         (0)    17041 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Number_State_Disabled_On_324523_Off_011_Should_Return_011.json
--rw-r--r--   0 root         (0) root         (0)    20249 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_String_State_Disabled_On_sonnet19_Off_sonnet53_Should_Return_sonnet53.json
--rw-r--r--   0 root         (0) root         (0)    20313 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_String_State_Disabled_On_sonnet53_Off_sonnet19_Should_Return_sonnet19.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.677720 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/
--rw-r--r--   0 root         (0) root         (0)    16899 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Bool_State_Enabled_On_False_Off_False_Should_Return_False.json
--rw-r--r--   0 root         (0) root         (0)    16894 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Bool_State_Enabled_On_False_Off_True_Should_Return_True.json
--rw-r--r--   0 root         (0) root         (0)    16895 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Bool_State_Enabled_On_True_Off_False_Should_Return_False.json
--rw-r--r--   0 root         (0) root         (0)    16890 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Bool_State_Enabled_On_True_Off_True_Should_Return_True.json
--rw-r--r--   0 root         (0) root         (0)    17241 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_JSON_State_Enabled_On_complexJSON_Off_emptyJSON_Should_Return_complexJSON.json
--rw-r--r--   0 root         (0) root         (0)    17211 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_JSON_State_Enabled_On_validJSON_Off_emptyJSON_Should_Return_validJSON.json
--rw-r--r--   0 root         (0) root         (0)    17021 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Number_State_Enabled_On_011_Off_2_Should_Return_011.json
--rw-r--r--   0 root         (0) root         (0)    17041 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Number_State_Enabled_On_324523_Off_011_Should_Return_324523.json
--rw-r--r--   0 root         (0) root         (0)    20308 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_String_State_Enabled_On_sonnet19_Off_sonnet53_Should_Return_sonnet19.json
--rw-r--r--   0 root         (0) root         (0)    20244 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_String_State_Enabled_On_sonnet53_Off_sonnet19_Should_Return_sonnet53.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.678720 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/
--rw-r--r--   0 root         (0) root         (0)    17239 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_EqualsThree_Should_Return_false_for_Target_three.json
--rw-r--r--   0 root         (0) root         (0)    17230 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_EqualsThree_Should_Return_true_for_Target_one.json
--rw-r--r--   0 root         (0) root         (0)    17276 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_GroupWithMultipleOrRules_Should_Return_true_for_Target_three.json
--rw-r--r--   0 root         (0) root         (0)    17243 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_InOneTwoThree_Should_Return_true_for_Target_three.json
--rw-r--r--   0 root         (0) root         (0)    17270 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_IncludeAndExcludeGroup_Should_Return_true_for_Target_three.json
--rw-r--r--   0 root         (0) root         (0)    17240 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_IncludedOnly_Should_Return_true_for_Target_three.json
--rw-r--r--   0 root         (0) root         (0)    17275 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_StartsWithTExcludesThree_Should_Return_true_for_Target_three.json
--rw-r--r--   0 root         (0) root         (0)    17232 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_StartsWithT_Should_Return_false_for_Target_one.json
--rw-r--r--   0 root         (0) root         (0)    17237 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_StartsWithT_Should_Return_true_for_Target_three.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.682721 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/
--rw-r--r--   0 root         (0) root         (0)    17050 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolBool_State_Enabled_On_True_Off_False_Prerequisites_AlwaysOff_Should_Return_False.json
--rw-r--r--   0 root         (0) root         (0)    17048 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolBool_State_Enabled_On_True_Off_False_Prerequisites_AlwaysOff_Should_Return_True.json
--rw-r--r--   0 root         (0) root         (0)    17045 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolBool_State_Enabled_On_True_Off_True_Prerequisites_AlwaysOn_Should_Return_False.json
--rw-r--r--   0 root         (0) root         (0)    17041 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolBool_State_Enabled_On_True_Off_True_Prerequisites_AlwaysOn_Should_Return_True.json
--rw-r--r--   0 root         (0) root         (0)    17039 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolInt_State_Enabled_On_True_Off_False_Prerequisites_AlwaysOff_Should_Return_False.json
--rw-r--r--   0 root         (0) root         (0)    17039 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolInt_State_Enabled_On_True_Off_False_Prerequisites_AlwaysOff_Should_Return_True.json
--rw-r--r--   0 root         (0) root         (0)    17036 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolInt_State_Enabled_On_True_Off_True_Prerequisites_AlwaysOn_Should_Return_False.json
--rw-r--r--   0 root         (0) root         (0)    17030 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolInt_State_Enabled_On_True_Off_True_Prerequisites_AlwaysOn_Should_Return_True.json
--rw-r--r--   0 root         (0) root         (0)    17169 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntBool_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_011.json
--rw-r--r--   0 root         (0) root         (0)    17163 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntBool_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_2.json
--rw-r--r--   0 root         (0) root         (0)    17166 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntBool_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_011.json
--rw-r--r--   0 root         (0) root         (0)    17158 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntBool_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_2.json
--rw-r--r--   0 root         (0) root         (0)    17158 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntInt_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_011.json
--rw-r--r--   0 root         (0) root         (0)    17154 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntInt_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_2.json
--rw-r--r--   0 root         (0) root         (0)    17157 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntInt_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_011.json
--rw-r--r--   0 root         (0) root         (0)    17147 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntInt_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_2.json
--rw-r--r--   0 root         (0) root         (0)    17173 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntJson_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_011.json
--rw-r--r--   0 root         (0) root         (0)    17164 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntJson_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_2.json
--rw-r--r--   0 root         (0) root         (0)    17167 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntJson_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_011.json
--rw-r--r--   0 root         (0) root         (0)    17162 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntJson_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_2.json
--rw-r--r--   0 root         (0) root         (0)    17183 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntString_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_011.json
--rw-r--r--   0 root         (0) root         (0)    17176 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntString_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_2.json
--rw-r--r--   0 root         (0) root         (0)    17179 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntString_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_011.json
--rw-r--r--   0 root         (0) root         (0)    17172 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntString_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_2.json
--rw-r--r--   0 root         (0) root         (0)    17353 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_JsonJson_State_Enabled_On_com_Off_val_Prerequisites_AlwaysOff_Should_Return_Com.json
--rw-r--r--   0 root         (0) root         (0)    17335 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_JsonJson_State_Enabled_On_com_Off_val_Prerequisites_AlwaysOff_Should_Return_Val.json
--rw-r--r--   0 root         (0) root         (0)    17351 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_JsonJson_State_Enabled_On_com_Off_val_Prerequisites_AlwaysOn_Should_Return_Com.json
--rw-r--r--   0 root         (0) root         (0)    17329 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_JsonJson_State_Enabled_On_com_Off_val_Prerequisites_AlwaysOn_Should_Return_Val.json
--rw-r--r--   0 root         (0) root         (0)    20370 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_StrStr_State_Enabled_On_s19_Off_s53_Prerequisites_AlwaysOff_Should_Return_off.json
--rw-r--r--   0 root         (0) root         (0)    20432 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_StrStr_State_Enabled_On_s19_Off_s53_Prerequisites_AlwaysOff_Should_Return_on.json
--rw-r--r--   0 root         (0) root         (0)    20366 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_StrStr_State_Enabled_On_s19_Off_s53_Prerequisites_AlwaysOn_Should_Return_Off.json
--rw-r--r--   0 root         (0) root         (0)    20428 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_StrStr_State_Enabled_On_s19_Off_s53_Prerequisites_AlwaysOn_Should_Return_On.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.683721 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/
--rw-r--r--   0 root         (0) root         (0)    17225 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Bool_State_Disabled_Should_Return_Default_Off_Value.json
--rw-r--r--   0 root         (0) root         (0)    17229 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Bool_State_Enabled_Should_Return_false_for_Target_four.json
--rw-r--r--   0 root         (0) root         (0)    17545 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Bool_State_Enabled_Should_Return_false_for_Target_six.json
--rw-r--r--   0 root         (0) root         (0)    17229 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Bool_State_Enabled_Should_Return_true_for_Target_three.json
--rw-r--r--   0 root         (0) root         (0)    17879 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_JSON_State_Enabled_Should_Return_complexJSON_for_Target_five.json
--rw-r--r--   0 root         (0) root         (0)    17836 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_JSON_State_Enabled_Should_Return_emptyJSON_for_Target_four.json
--rw-r--r--   0 root         (0) root         (0)    17870 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_JSON_State_Enabled_Should_Return_validJSON_for_Target_anonymous.json
--rw-r--r--   0 root         (0) root         (0)    17673 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Number_State_Enabled_Should_Return_2_for_Target_four.json
--rw-r--r--   0 root         (0) root         (0)    17688 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Number_State_Enabled_Should_Return_324523_for_Target_five.json
--rw-r--r--   0 root         (0) root         (0)    17705 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Number_State_Enabled_Should_Return_sonnet53_for_Target_anonymous.json
--rw-r--r--   0 root         (0) root         (0)    20968 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_String_State_Enabled_Should_Return_sonnet53_for_Target_anonymous.json
--rw-r--r--   0 root         (0) root         (0)    20889 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_String_State_Enabled_Should_Return_sonnet53_for_Target_four.json
--rw-r--r--   0 root         (0) root         (0)    21601 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_String_State_Enabled_Should_Return_thehobbit_for_Target_five.json
--rw-r--r--   0 root         (0) root         (0)     1475 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/bool_on_simple_rule.json
--rw-r--r--   0 root         (0) root         (0)     1038 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/off_flag.json
--rw-r--r--   0 root         (0) root         (0)     1084 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/off_off_no_rules.json
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/on_off_no_rules.json
--rw-r--r--   0 root         (0) root         (0)     2430 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/prereq.json
--rw-r--r--   0 root         (0) root         (0)     1762 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/rules_priority.json
--rw-r--r--   0 root         (0) root         (0)     1574 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/segment_includes_target.json
--rw-r--r--   0 root         (0) root         (0)     1279 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/test_empty_or_missing_target_attributes.json
--rw-r--r--   0 root         (0) root         (0)     6749 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/types.gen.go
--rw-r--r--   0 root         (0) root         (0)      384 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/types.go
--rw-r--r--   0 root         (0) root         (0)     2697 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/validator.go
--rw-r--r--   0 root         (0) root         (0)      128 2023-07-04 17:02:26.000000 harness-featureflags-1.2.1/tests/integration/ff-test-cases/validator_test.go
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/tests/integration/test_clause.py
--rw-r--r--   0 root         (0) root         (0)     4273 2023-07-04 17:03:04.000000 harness-featureflags-1.2.1/tests/integration/test_evaluator.py
--rw-r--r--   0 root         (0) root         (0)     3885 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/tests/integration/test_feature.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/tests/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 17:04:29.685721 harness-featureflags-1.2.1/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/tests/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)      349 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/tests/unit/test_boolean.py
--rw-r--r--   0 root         (0) root         (0)     1608 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/tests/unit/test_clause.py
--rw-r--r--   0 root         (0) root         (0)     7062 2023-07-04 17:03:04.000000 harness-featureflags-1.2.1/tests/unit/test_evaluator.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/tests/unit/test_feature.py
--rw-r--r--   0 root         (0) root         (0)     1073 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/tests/unit/test_integer.py
--rw-r--r--   0 root         (0) root         (0)     2701 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/tests/unit/test_lru.py
--rw-r--r--   0 root         (0) root         (0)     1092 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/tests/unit/test_number.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/tests/unit/test_sdk_logging_codes.py
--rw-r--r--   0 root         (0) root         (0)     7669 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/tests/unit/test_sse_client.py
--rw-r--r--   0 root         (0) root         (0)     1589 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/tests/unit/test_string.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/tests/unit/test_target.py
--rw-r--r--   0 root         (0) root         (0)     1137 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/tests/unit/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2363 2023-07-04 17:02:21.000000 harness-featureflags-1.2.1/tests/unit/test_variation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.757832 harness-featureflags-1.2.2/
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     3655 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/HISTORY.rst
+-rw-r--r--   0 root         (0) root         (0)      585 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      262 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5307 2023-07-17 13:59:54.757832 harness-featureflags-1.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4373 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.687827 harness-featureflags-1.2.2/docs/
+-rw-r--r--   0 root         (0) root         (0)      621 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/authors.rst
+-rwxr-xr-x   0 root         (0) root         (0)     4958 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)       33 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/featureflags.api.default.rst
+-rw-r--r--   0 root         (0) root         (0)      591 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/featureflags.api.rst
+-rw-r--r--   0 root         (0) root         (0)      183 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/featureflags.client.rst
+-rw-r--r--   0 root         (0) root         (0)      195 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/featureflags.evaluation.rst
+-rw-r--r--   0 root         (0) root         (0)     3689 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/featureflags.evaluations.rst
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/featureflags.ftypes.rst
+-rw-r--r--   0 root         (0) root         (0)     2781 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/featureflags.models.rst
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/featureflags.rest.api.default.rst
+-rw-r--r--   0 root         (0) root         (0)      263 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/featureflags.rest.api.rst
+-rw-r--r--   0 root         (0) root         (0)     4302 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/featureflags.rest.models.rst
+-rw-r--r--   0 root         (0) root         (0)      621 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/featureflags.rest.rst
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/featureflags.rst
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/history.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.687827 harness-featureflags-1.2.2/docs/images/
+-rw-r--r--   0 root         (0) root         (0)   100515 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/images/ff-gui.png
+-rw-r--r--   0 root         (0) root         (0)      333 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      782 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/modules.rst
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/readme.rst
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/docs/usage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.688827 harness-featureflags-1.2.2/featureflags/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12117 2023-07-17 13:58:24.000000 harness-featureflags-1.2.2/featureflags/analytics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.688827 harness-featureflags-1.2.2/featureflags/api/
+-rw-r--r--   0 root         (0) root         (0)      173 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/api/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.689827 harness-featureflags-1.2.2/featureflags/api/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/api/default/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-07-17 13:58:23.000000 harness-featureflags-1.2.2/featureflags/api/default/authenticate.py
+-rw-r--r--   0 root         (0) root         (0)     2872 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/api/default/get_all_segments.py
+-rw-r--r--   0 root         (0) root         (0)     2995 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/api/default/get_feature_config.py
+-rw-r--r--   0 root         (0) root         (0)     2943 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/api/default/get_feature_config_by_identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/api/default/get_segment_by_identifier.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/api/default/post_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/api/default/stream.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/api/types.py
+-rw-r--r--   0 root         (0) root         (0)     9805 2023-07-17 13:58:23.000000 harness-featureflags-1.2.2/featureflags/client.py
+-rw-r--r--   0 root         (0) root         (0)     2603 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.691827 harness-featureflags-1.2.2/featureflags/evaluations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2878 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/auth_target.py
+-rw-r--r--   0 root         (0) root         (0)     3892 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/clause.py
+-rw-r--r--   0 root         (0) root         (0)      273 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/constants.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/distribution.py
+-rw-r--r--   0 root         (0) root         (0)      124 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/enum.py
+-rw-r--r--   0 root         (0) root         (0)    13944 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     9128 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/feature.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/prerequisite.py
+-rw-r--r--   0 root         (0) root         (0)     5429 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/segment.py
+-rw-r--r--   0 root         (0) root         (0)     2063 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/serve.py
+-rw-r--r--   0 root         (0) root         (0)     3165 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/serving_rule.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/strategy.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/tag.py
+-rw-r--r--   0 root         (0) root         (0)     4378 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/target.py
+-rw-r--r--   0 root         (0) root         (0)     1339 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/target_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/target_map.py
+-rw-r--r--   0 root         (0) root         (0)     5352 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/variation.py
+-rw-r--r--   0 root         (0) root         (0)     2564 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/variation_map.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/evaluations/weighted_variation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.692827 harness-featureflags-1.2.2/featureflags/ftypes/
+-rw-r--r--   0 root         (0) root         (0)      242 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/ftypes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/ftypes/boolean.py
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/ftypes/integer.py
+-rw-r--r--   0 root         (0) root         (0)     2469 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/ftypes/interface.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/ftypes/json.py
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/ftypes/number.py
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/ftypes/string.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/ftypes/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/interface.py
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/lru_cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.693827 harness-featureflags-1.2.2/featureflags/models/
+-rw-r--r--   0 root         (0) root         (0)      809 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/models/authentication_request.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/models/authentication_request_target.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/models/authentication_request_target_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/models/authentication_response.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/models/error.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/models/key_value.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/models/message.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/models/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     2372 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/models/metrics_data.py
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/models/metrics_data_metrics_type.py
+-rw-r--r--   0 root         (0) root         (0)     2131 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/models/pagination.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/models/target_data.py
+-rw-r--r--   0 root         (0) root         (0)       92 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/models/unset.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/persisting.py
+-rw-r--r--   0 root         (0) root         (0)     4963 2023-07-17 13:58:23.000000 harness-featureflags-1.2.2/featureflags/polling.py
+-rw-r--r--   0 root         (0) root         (0)     8198 2023-07-17 13:58:23.000000 harness-featureflags-1.2.2/featureflags/repository.py
+-rw-r--r--   0 root         (0) root         (0)     4298 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/sdk_logging_codes.py
+-rw-r--r--   0 root         (0) root         (0)     7069 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/sse_client.py
+-rw-r--r--   0 root         (0) root         (0)     6712 2023-07-17 13:58:23.000000 harness-featureflags-1.2.2/featureflags/streaming.py
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/featureflags/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.693827 harness-featureflags-1.2.2/harness_featureflags.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5307 2023-07-17 13:59:54.000000 harness-featureflags-1.2.2/harness_featureflags.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15040 2023-07-17 13:59:54.000000 harness-featureflags-1.2.2/harness_featureflags.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 13:59:54.000000 harness-featureflags-1.2.2/harness_featureflags.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 13:59:54.000000 harness-featureflags-1.2.2/harness_featureflags.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       86 2023-07-17 13:59:54.000000 harness-featureflags-1.2.2/harness_featureflags.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 13:59:54.000000 harness-featureflags-1.2.2/harness_featureflags.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      454 2023-07-17 13:59:54.757832 harness-featureflags-1.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.694827 harness-featureflags-1.2.2/tests/
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.694827 harness-featureflags-1.2.2/tests/integration/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.695827 harness-featureflags-1.2.2/tests/integration/ff-test-cases/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/.git
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.683826 harness-featureflags-1.2.2/tests/integration/ff-test-cases/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.695827 harness-featureflags-1.2.2/tests/integration/ff-test-cases/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      333 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/.github/workflows/ci.yml
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     2746 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/Makefile
+-rw-r--r--   0 root         (0) root         (0)     3334 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/README.md
+-rw-r--r--   0 root         (0) root         (0)    15527 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/client-v1.yaml
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/go.mod
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.696827 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.697827 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/
+-rw-r--r--   0 root         (0) root         (0)    16904 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Bool_State_Disabled_On_False_Off_False_Should_Return_False.json
+-rw-r--r--   0 root         (0) root         (0)    16898 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Bool_State_Disabled_On_False_Off_True_Should_Return_True.json
+-rw-r--r--   0 root         (0) root         (0)    16901 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Bool_State_Disabled_On_True_Off_False_Should_Return_False.json
+-rw-r--r--   0 root         (0) root         (0)    16895 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Bool_State_Disabled_On_True_Off_True_Should_Return_True.json
+-rw-r--r--   0 root         (0) root         (0)    17222 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_JSON_State_Disabled_On_complexJSON_Off_emptyJSON_Should_Return_validJSON.json
+-rw-r--r--   0 root         (0) root         (0)    17197 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_JSON_State_Disabled_On_validJSON_Off_emptyJSON_Should_Return_emptyJSON.json
+-rw-r--r--   0 root         (0) root         (0)    17019 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Number_State_Disabled_On_011_Off_2_Should_Return_2.json
+-rw-r--r--   0 root         (0) root         (0)    17041 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Number_State_Disabled_On_324523_Off_011_Should_Return_011.json
+-rw-r--r--   0 root         (0) root         (0)    20249 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_String_State_Disabled_On_sonnet19_Off_sonnet53_Should_Return_sonnet53.json
+-rw-r--r--   0 root         (0) root         (0)    20313 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_String_State_Disabled_On_sonnet53_Off_sonnet19_Should_Return_sonnet19.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.698827 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/
+-rw-r--r--   0 root         (0) root         (0)    16899 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Bool_State_Enabled_On_False_Off_False_Should_Return_False.json
+-rw-r--r--   0 root         (0) root         (0)    16894 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Bool_State_Enabled_On_False_Off_True_Should_Return_True.json
+-rw-r--r--   0 root         (0) root         (0)    16895 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Bool_State_Enabled_On_True_Off_False_Should_Return_False.json
+-rw-r--r--   0 root         (0) root         (0)    16890 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Bool_State_Enabled_On_True_Off_True_Should_Return_True.json
+-rw-r--r--   0 root         (0) root         (0)    17241 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_JSON_State_Enabled_On_complexJSON_Off_emptyJSON_Should_Return_complexJSON.json
+-rw-r--r--   0 root         (0) root         (0)    17211 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_JSON_State_Enabled_On_validJSON_Off_emptyJSON_Should_Return_validJSON.json
+-rw-r--r--   0 root         (0) root         (0)    17021 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Number_State_Enabled_On_011_Off_2_Should_Return_011.json
+-rw-r--r--   0 root         (0) root         (0)    17041 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Number_State_Enabled_On_324523_Off_011_Should_Return_324523.json
+-rw-r--r--   0 root         (0) root         (0)    20308 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_String_State_Enabled_On_sonnet19_Off_sonnet53_Should_Return_sonnet19.json
+-rw-r--r--   0 root         (0) root         (0)    20244 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_String_State_Enabled_On_sonnet53_Off_sonnet19_Should_Return_sonnet53.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.699828 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/
+-rw-r--r--   0 root         (0) root         (0)    17239 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_EqualsThree_Should_Return_false_for_Target_three.json
+-rw-r--r--   0 root         (0) root         (0)    17230 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_EqualsThree_Should_Return_true_for_Target_one.json
+-rw-r--r--   0 root         (0) root         (0)    17276 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_GroupWithMultipleOrRules_Should_Return_true_for_Target_three.json
+-rw-r--r--   0 root         (0) root         (0)    17243 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_InOneTwoThree_Should_Return_true_for_Target_three.json
+-rw-r--r--   0 root         (0) root         (0)    17270 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_IncludeAndExcludeGroup_Should_Return_true_for_Target_three.json
+-rw-r--r--   0 root         (0) root         (0)    17240 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_IncludedOnly_Should_Return_true_for_Target_three.json
+-rw-r--r--   0 root         (0) root         (0)    17275 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_StartsWithTExcludesThree_Should_Return_true_for_Target_three.json
+-rw-r--r--   0 root         (0) root         (0)    17232 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_StartsWithT_Should_Return_false_for_Target_one.json
+-rw-r--r--   0 root         (0) root         (0)    17237 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_StartsWithT_Should_Return_true_for_Target_three.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.703828 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/
+-rw-r--r--   0 root         (0) root         (0)    17050 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolBool_State_Enabled_On_True_Off_False_Prerequisites_AlwaysOff_Should_Return_False.json
+-rw-r--r--   0 root         (0) root         (0)    17048 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolBool_State_Enabled_On_True_Off_False_Prerequisites_AlwaysOff_Should_Return_True.json
+-rw-r--r--   0 root         (0) root         (0)    17045 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolBool_State_Enabled_On_True_Off_True_Prerequisites_AlwaysOn_Should_Return_False.json
+-rw-r--r--   0 root         (0) root         (0)    17041 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolBool_State_Enabled_On_True_Off_True_Prerequisites_AlwaysOn_Should_Return_True.json
+-rw-r--r--   0 root         (0) root         (0)    17039 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolInt_State_Enabled_On_True_Off_False_Prerequisites_AlwaysOff_Should_Return_False.json
+-rw-r--r--   0 root         (0) root         (0)    17039 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolInt_State_Enabled_On_True_Off_False_Prerequisites_AlwaysOff_Should_Return_True.json
+-rw-r--r--   0 root         (0) root         (0)    17036 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolInt_State_Enabled_On_True_Off_True_Prerequisites_AlwaysOn_Should_Return_False.json
+-rw-r--r--   0 root         (0) root         (0)    17030 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolInt_State_Enabled_On_True_Off_True_Prerequisites_AlwaysOn_Should_Return_True.json
+-rw-r--r--   0 root         (0) root         (0)    17169 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntBool_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_011.json
+-rw-r--r--   0 root         (0) root         (0)    17163 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntBool_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_2.json
+-rw-r--r--   0 root         (0) root         (0)    17166 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntBool_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_011.json
+-rw-r--r--   0 root         (0) root         (0)    17158 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntBool_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_2.json
+-rw-r--r--   0 root         (0) root         (0)    17158 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntInt_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_011.json
+-rw-r--r--   0 root         (0) root         (0)    17154 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntInt_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_2.json
+-rw-r--r--   0 root         (0) root         (0)    17157 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntInt_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_011.json
+-rw-r--r--   0 root         (0) root         (0)    17147 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntInt_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_2.json
+-rw-r--r--   0 root         (0) root         (0)    17173 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntJson_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_011.json
+-rw-r--r--   0 root         (0) root         (0)    17164 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntJson_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_2.json
+-rw-r--r--   0 root         (0) root         (0)    17167 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntJson_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_011.json
+-rw-r--r--   0 root         (0) root         (0)    17162 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntJson_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_2.json
+-rw-r--r--   0 root         (0) root         (0)    17183 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntString_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_011.json
+-rw-r--r--   0 root         (0) root         (0)    17176 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntString_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_2.json
+-rw-r--r--   0 root         (0) root         (0)    17179 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntString_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_011.json
+-rw-r--r--   0 root         (0) root         (0)    17172 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntString_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_2.json
+-rw-r--r--   0 root         (0) root         (0)    17353 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_JsonJson_State_Enabled_On_com_Off_val_Prerequisites_AlwaysOff_Should_Return_Com.json
+-rw-r--r--   0 root         (0) root         (0)    17335 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_JsonJson_State_Enabled_On_com_Off_val_Prerequisites_AlwaysOff_Should_Return_Val.json
+-rw-r--r--   0 root         (0) root         (0)    17351 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_JsonJson_State_Enabled_On_com_Off_val_Prerequisites_AlwaysOn_Should_Return_Com.json
+-rw-r--r--   0 root         (0) root         (0)    17329 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_JsonJson_State_Enabled_On_com_Off_val_Prerequisites_AlwaysOn_Should_Return_Val.json
+-rw-r--r--   0 root         (0) root         (0)    20370 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_StrStr_State_Enabled_On_s19_Off_s53_Prerequisites_AlwaysOff_Should_Return_off.json
+-rw-r--r--   0 root         (0) root         (0)    20432 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_StrStr_State_Enabled_On_s19_Off_s53_Prerequisites_AlwaysOff_Should_Return_on.json
+-rw-r--r--   0 root         (0) root         (0)    20366 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_StrStr_State_Enabled_On_s19_Off_s53_Prerequisites_AlwaysOn_Should_Return_Off.json
+-rw-r--r--   0 root         (0) root         (0)    20428 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_StrStr_State_Enabled_On_s19_Off_s53_Prerequisites_AlwaysOn_Should_Return_On.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.704828 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/
+-rw-r--r--   0 root         (0) root         (0)    17225 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Bool_State_Disabled_Should_Return_Default_Off_Value.json
+-rw-r--r--   0 root         (0) root         (0)    17229 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Bool_State_Enabled_Should_Return_false_for_Target_four.json
+-rw-r--r--   0 root         (0) root         (0)    17545 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Bool_State_Enabled_Should_Return_false_for_Target_six.json
+-rw-r--r--   0 root         (0) root         (0)    17229 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Bool_State_Enabled_Should_Return_true_for_Target_three.json
+-rw-r--r--   0 root         (0) root         (0)    17879 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_JSON_State_Enabled_Should_Return_complexJSON_for_Target_five.json
+-rw-r--r--   0 root         (0) root         (0)    17836 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_JSON_State_Enabled_Should_Return_emptyJSON_for_Target_four.json
+-rw-r--r--   0 root         (0) root         (0)    17870 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_JSON_State_Enabled_Should_Return_validJSON_for_Target_anonymous.json
+-rw-r--r--   0 root         (0) root         (0)    17673 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Number_State_Enabled_Should_Return_2_for_Target_four.json
+-rw-r--r--   0 root         (0) root         (0)    17688 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Number_State_Enabled_Should_Return_324523_for_Target_five.json
+-rw-r--r--   0 root         (0) root         (0)    17705 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Number_State_Enabled_Should_Return_sonnet53_for_Target_anonymous.json
+-rw-r--r--   0 root         (0) root         (0)    20968 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_String_State_Enabled_Should_Return_sonnet53_for_Target_anonymous.json
+-rw-r--r--   0 root         (0) root         (0)    20889 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_String_State_Enabled_Should_Return_sonnet53_for_Target_four.json
+-rw-r--r--   0 root         (0) root         (0)    21601 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_String_State_Enabled_Should_Return_thehobbit_for_Target_five.json
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/bool_on_simple_rule.json
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/off_flag.json
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/off_off_no_rules.json
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/on_off_no_rules.json
+-rw-r--r--   0 root         (0) root         (0)     2430 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/prereq.json
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/rules_priority.json
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/segment_includes_target.json
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/test_empty_or_missing_target_attributes.json
+-rw-r--r--   0 root         (0) root         (0)     6749 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/types.gen.go
+-rw-r--r--   0 root         (0) root         (0)      384 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/types.go
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/validator.go
+-rw-r--r--   0 root         (0) root         (0)      128 2023-07-17 13:57:43.000000 harness-featureflags-1.2.2/tests/integration/ff-test-cases/validator_test.go
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/tests/integration/test_clause.py
+-rw-r--r--   0 root         (0) root         (0)     4273 2023-07-17 13:58:23.000000 harness-featureflags-1.2.2/tests/integration/test_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     3885 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/tests/integration/test_feature.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:59:54.757832 harness-featureflags-1.2.2/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/tests/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      349 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/tests/unit/test_boolean.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/tests/unit/test_clause.py
+-rw-r--r--   0 root         (0) root         (0)     7062 2023-07-17 13:58:23.000000 harness-featureflags-1.2.2/tests/unit/test_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/tests/unit/test_feature.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/tests/unit/test_integer.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/tests/unit/test_lru.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/tests/unit/test_number.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/tests/unit/test_sdk_logging_codes.py
+-rw-r--r--   0 root         (0) root         (0)     7669 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/tests/unit/test_sse_client.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/tests/unit/test_string.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/tests/unit/test_target.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/tests/unit/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2363 2023-07-17 13:57:37.000000 harness-featureflags-1.2.2/tests/unit/test_variation.py
```

### Comparing `harness-featureflags-1.2.1/CONTRIBUTING.rst` & `harness-featureflags-1.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/LICENSE` & `harness-featureflags-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/PKG-INFO` & `harness-featureflags-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harness-featureflags
-Version: 1.2.1
+Version: 1.2.2
 Summary: Feature flag server SDK for python
 Home-page: https://github.com/harness/ff-python-server-sdk
 Author: Enver Bisevac
 Author-email: enver.bisevac@harness.io
 License: Apache Software License 2.0
 Keywords: featureflags
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `harness-featureflags-1.2.1/README.md` & `harness-featureflags-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/docs/Makefile` & `harness-featureflags-1.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/docs/conf.py` & `harness-featureflags-1.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/docs/featureflags.api.default.rst` & `harness-featureflags-1.2.2/docs/featureflags.api.default.rst`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/docs/featureflags.api.rst` & `harness-featureflags-1.2.2/docs/featureflags.api.rst`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/docs/featureflags.evaluations.rst` & `harness-featureflags-1.2.2/docs/featureflags.evaluations.rst`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/docs/featureflags.ftypes.rst` & `harness-featureflags-1.2.2/docs/featureflags.ftypes.rst`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/docs/featureflags.models.rst` & `harness-featureflags-1.2.2/docs/featureflags.models.rst`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/docs/featureflags.rest.api.default.rst` & `harness-featureflags-1.2.2/docs/featureflags.rest.api.default.rst`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/docs/featureflags.rest.models.rst` & `harness-featureflags-1.2.2/docs/featureflags.rest.models.rst`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/docs/featureflags.rest.rst` & `harness-featureflags-1.2.2/docs/featureflags.rest.rst`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/docs/featureflags.rst` & `harness-featureflags-1.2.2/docs/featureflags.rst`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/docs/images/ff-gui.png` & `harness-featureflags-1.2.2/docs/images/ff-gui.png`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/docs/installation.rst` & `harness-featureflags-1.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/docs/make.bat` & `harness-featureflags-1.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/analytics.py` & `harness-featureflags-1.2.2/featureflags/analytics.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/api/client.py` & `harness-featureflags-1.2.2/featureflags/api/client.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/api/default/authenticate.py` & `harness-featureflags-1.2.2/featureflags/api/default/authenticate.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/api/default/get_all_segments.py` & `harness-featureflags-1.2.2/featureflags/api/default/get_all_segments.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/api/default/get_feature_config.py` & `harness-featureflags-1.2.2/featureflags/api/default/get_feature_config.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/api/default/get_feature_config_by_identifier.py` & `harness-featureflags-1.2.2/featureflags/api/default/get_feature_config_by_identifier.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/api/default/get_segment_by_identifier.py` & `harness-featureflags-1.2.2/featureflags/api/default/get_segment_by_identifier.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/api/default/post_metrics.py` & `harness-featureflags-1.2.2/featureflags/api/default/post_metrics.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/api/default/stream.py` & `harness-featureflags-1.2.2/featureflags/api/default/stream.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/api/types.py` & `harness-featureflags-1.2.2/featureflags/api/types.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/client.py` & `harness-featureflags-1.2.2/featureflags/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,16 +162,18 @@
             },
             max_auth_retries=self._config.max_auth_retries
         )
         # Additional headers used to track usage
         additional_headers = {
             "User-Agent": "PythonSDK/" + VERSION,
             "Harness-SDK-Info": f'Python {VERSION} Server',
-            "Harness-EnvironmentID": self._environment_id,
-            "Harness-AccountID": decoded["accountID"]}
+            "Harness-EnvironmentID": self._environment_id}
+        # At present the FF Relay Proxy does not send the accountID claim
+        if "accountID" in decoded:
+            additional_headers["Harness-AccountID"] = decoded["accountID"]
         self._client = self._client.with_headers(additional_headers)
 
     def bool_variation(self, identifier: str, target: Target,
                        default: bool) -> bool:
         variation = self._evaluator.evaluate(identifier, target)
         # Only register metrics if analytics is enabled,
         # and sometimes when the SDK starts up we can
```

### Comparing `harness-featureflags-1.2.1/featureflags/config.py` & `harness-featureflags-1.2.2/featureflags/config.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/evaluations/auth_target.py` & `harness-featureflags-1.2.2/featureflags/evaluations/auth_target.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/evaluations/clause.py` & `harness-featureflags-1.2.2/featureflags/evaluations/clause.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/evaluations/distribution.py` & `harness-featureflags-1.2.2/featureflags/evaluations/distribution.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/evaluations/evaluator.py` & `harness-featureflags-1.2.2/featureflags/evaluations/evaluator.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/evaluations/feature.py` & `harness-featureflags-1.2.2/featureflags/evaluations/feature.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/evaluations/prerequisite.py` & `harness-featureflags-1.2.2/featureflags/evaluations/prerequisite.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/evaluations/segment.py` & `harness-featureflags-1.2.2/featureflags/evaluations/segment.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/evaluations/serve.py` & `harness-featureflags-1.2.2/featureflags/evaluations/serve.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/evaluations/serving_rule.py` & `harness-featureflags-1.2.2/featureflags/evaluations/serving_rule.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/evaluations/tag.py` & `harness-featureflags-1.2.2/featureflags/evaluations/tag.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/evaluations/target.py` & `harness-featureflags-1.2.2/featureflags/evaluations/target.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/evaluations/target_attributes.py` & `harness-featureflags-1.2.2/featureflags/evaluations/target_attributes.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/evaluations/target_map.py` & `harness-featureflags-1.2.2/featureflags/evaluations/target_map.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/evaluations/variation.py` & `harness-featureflags-1.2.2/featureflags/evaluations/variation.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/evaluations/variation_map.py` & `harness-featureflags-1.2.2/featureflags/evaluations/variation_map.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/evaluations/weighted_variation.py` & `harness-featureflags-1.2.2/featureflags/evaluations/weighted_variation.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/ftypes/boolean.py` & `harness-featureflags-1.2.2/featureflags/ftypes/boolean.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/ftypes/integer.py` & `harness-featureflags-1.2.2/featureflags/ftypes/integer.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/ftypes/interface.py` & `harness-featureflags-1.2.2/featureflags/ftypes/interface.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/ftypes/json.py` & `harness-featureflags-1.2.2/featureflags/ftypes/json.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/ftypes/number.py` & `harness-featureflags-1.2.2/featureflags/ftypes/number.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/ftypes/string.py` & `harness-featureflags-1.2.2/featureflags/ftypes/string.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/interface.py` & `harness-featureflags-1.2.2/featureflags/interface.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/lru_cache.py` & `harness-featureflags-1.2.2/featureflags/lru_cache.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/models/__init__.py` & `harness-featureflags-1.2.2/featureflags/models/__init__.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/models/authentication_request.py` & `harness-featureflags-1.2.2/featureflags/models/authentication_request.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/models/authentication_request_target.py` & `harness-featureflags-1.2.2/featureflags/models/authentication_request_target.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/models/authentication_request_target_attributes.py` & `harness-featureflags-1.2.2/featureflags/models/authentication_request_target_attributes.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/models/authentication_response.py` & `harness-featureflags-1.2.2/featureflags/models/authentication_response.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/models/error.py` & `harness-featureflags-1.2.2/featureflags/models/error.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/models/key_value.py` & `harness-featureflags-1.2.2/featureflags/models/key_value.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/models/message.py` & `harness-featureflags-1.2.2/featureflags/models/message.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/models/metrics.py` & `harness-featureflags-1.2.2/featureflags/models/metrics.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/models/metrics_data.py` & `harness-featureflags-1.2.2/featureflags/models/metrics_data.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/models/pagination.py` & `harness-featureflags-1.2.2/featureflags/models/pagination.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/models/target_data.py` & `harness-featureflags-1.2.2/featureflags/models/target_data.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/persisting.py` & `harness-featureflags-1.2.2/featureflags/persisting.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/polling.py` & `harness-featureflags-1.2.2/featureflags/polling.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/repository.py` & `harness-featureflags-1.2.2/featureflags/repository.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/sdk_logging_codes.py` & `harness-featureflags-1.2.2/featureflags/sdk_logging_codes.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/sse_client.py` & `harness-featureflags-1.2.2/featureflags/sse_client.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/featureflags/streaming.py` & `harness-featureflags-1.2.2/featureflags/streaming.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/harness_featureflags.egg-info/PKG-INFO` & `harness-featureflags-1.2.2/harness_featureflags.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harness-featureflags
-Version: 1.2.1
+Version: 1.2.2
 Summary: Feature flag server SDK for python
 Home-page: https://github.com/harness/ff-python-server-sdk
 Author: Enver Bisevac
 Author-email: enver.bisevac@harness.io
 License: Apache Software License 2.0
 Keywords: featureflags
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `harness-featureflags-1.2.1/harness_featureflags.egg-info/SOURCES.txt` & `harness-featureflags-1.2.2/harness_featureflags.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/setup.py` & `harness-featureflags-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     keywords="featureflags",
     name="harness-featureflags",
     packages=find_packages(include=["featureflags", "featureflags.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/harness/ff-python-server-sdk",
-    version='1.2.1',
+    version='1.2.2',
     zip_safe=False,
 )
```

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/Makefile` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/Makefile`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/README.md` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/README.md`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/client-v1.yaml` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/client-v1.yaml`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Bool_State_Disabled_On_False_Off_False_Should_Return_False.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Bool_State_Disabled_On_False_Off_False_Should_Return_False.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Bool_State_Disabled_On_False_Off_True_Should_Return_True.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Bool_State_Disabled_On_False_Off_True_Should_Return_True.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Bool_State_Disabled_On_True_Off_False_Should_Return_False.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Bool_State_Disabled_On_True_Off_False_Should_Return_False.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Bool_State_Disabled_On_True_Off_True_Should_Return_True.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Bool_State_Disabled_On_True_Off_True_Should_Return_True.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_JSON_State_Disabled_On_complexJSON_Off_emptyJSON_Should_Return_validJSON.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_JSON_State_Disabled_On_complexJSON_Off_emptyJSON_Should_Return_validJSON.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_JSON_State_Disabled_On_validJSON_Off_emptyJSON_Should_Return_emptyJSON.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_JSON_State_Disabled_On_validJSON_Off_emptyJSON_Should_Return_emptyJSON.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Number_State_Disabled_On_011_Off_2_Should_Return_2.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Number_State_Disabled_On_011_Off_2_Should_Return_2.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Number_State_Disabled_On_324523_Off_011_Should_Return_011.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_Number_State_Disabled_On_324523_Off_011_Should_Return_011.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_String_State_Disabled_On_sonnet19_Off_sonnet53_Should_Return_sonnet53.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_String_State_Disabled_On_sonnet19_Off_sonnet53_Should_Return_sonnet53.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_String_State_Disabled_On_sonnet53_Off_sonnet19_Should_Return_sonnet19.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOffRules/DefaultOffRules_Type_String_State_Disabled_On_sonnet53_Off_sonnet19_Should_Return_sonnet19.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Bool_State_Enabled_On_False_Off_False_Should_Return_False.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Bool_State_Enabled_On_False_Off_False_Should_Return_False.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Bool_State_Enabled_On_False_Off_True_Should_Return_True.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Bool_State_Enabled_On_False_Off_True_Should_Return_True.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Bool_State_Enabled_On_True_Off_False_Should_Return_False.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Bool_State_Enabled_On_True_Off_False_Should_Return_False.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Bool_State_Enabled_On_True_Off_True_Should_Return_True.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Bool_State_Enabled_On_True_Off_True_Should_Return_True.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_JSON_State_Enabled_On_complexJSON_Off_emptyJSON_Should_Return_complexJSON.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_JSON_State_Enabled_On_complexJSON_Off_emptyJSON_Should_Return_complexJSON.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_JSON_State_Enabled_On_validJSON_Off_emptyJSON_Should_Return_validJSON.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_JSON_State_Enabled_On_validJSON_Off_emptyJSON_Should_Return_validJSON.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Number_State_Enabled_On_011_Off_2_Should_Return_011.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Number_State_Enabled_On_011_Off_2_Should_Return_011.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Number_State_Enabled_On_324523_Off_011_Should_Return_324523.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_Number_State_Enabled_On_324523_Off_011_Should_Return_324523.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_String_State_Enabled_On_sonnet19_Off_sonnet53_Should_Return_sonnet19.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_String_State_Enabled_On_sonnet19_Off_sonnet53_Should_Return_sonnet19.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_String_State_Enabled_On_sonnet53_Off_sonnet19_Should_Return_sonnet53.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/DefaultOnRules/DefaultOnRules_Type_String_State_Enabled_On_sonnet53_Off_sonnet19_Should_Return_sonnet53.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_EqualsThree_Should_Return_false_for_Target_three.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_EqualsThree_Should_Return_false_for_Target_three.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_EqualsThree_Should_Return_true_for_Target_one.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_EqualsThree_Should_Return_true_for_Target_one.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_GroupWithMultipleOrRules_Should_Return_true_for_Target_three.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_GroupWithMultipleOrRules_Should_Return_true_for_Target_three.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_InOneTwoThree_Should_Return_true_for_Target_three.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_InOneTwoThree_Should_Return_true_for_Target_three.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_IncludeAndExcludeGroup_Should_Return_true_for_Target_three.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_IncludeAndExcludeGroup_Should_Return_true_for_Target_three.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_IncludedOnly_Should_Return_true_for_Target_three.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_IncludedOnly_Should_Return_true_for_Target_three.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_StartsWithTExcludesThree_Should_Return_true_for_Target_three.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_StartsWithTExcludesThree_Should_Return_true_for_Target_three.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_StartsWithT_Should_Return_false_for_Target_one.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_StartsWithT_Should_Return_false_for_Target_one.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_StartsWithT_Should_Return_true_for_Target_three.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/GroupRules/GroupRules_Type_Bool_State_Enabled_StartsWithT_Should_Return_true_for_Target_three.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolBool_State_Enabled_On_True_Off_False_Prerequisites_AlwaysOff_Should_Return_False.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolBool_State_Enabled_On_True_Off_False_Prerequisites_AlwaysOff_Should_Return_False.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolBool_State_Enabled_On_True_Off_False_Prerequisites_AlwaysOff_Should_Return_True.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolBool_State_Enabled_On_True_Off_False_Prerequisites_AlwaysOff_Should_Return_True.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolBool_State_Enabled_On_True_Off_True_Prerequisites_AlwaysOn_Should_Return_False.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolBool_State_Enabled_On_True_Off_True_Prerequisites_AlwaysOn_Should_Return_False.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolBool_State_Enabled_On_True_Off_True_Prerequisites_AlwaysOn_Should_Return_True.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolBool_State_Enabled_On_True_Off_True_Prerequisites_AlwaysOn_Should_Return_True.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolInt_State_Enabled_On_True_Off_False_Prerequisites_AlwaysOff_Should_Return_False.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolInt_State_Enabled_On_True_Off_False_Prerequisites_AlwaysOff_Should_Return_False.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolInt_State_Enabled_On_True_Off_False_Prerequisites_AlwaysOff_Should_Return_True.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolInt_State_Enabled_On_True_Off_False_Prerequisites_AlwaysOff_Should_Return_True.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolInt_State_Enabled_On_True_Off_True_Prerequisites_AlwaysOn_Should_Return_False.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolInt_State_Enabled_On_True_Off_True_Prerequisites_AlwaysOn_Should_Return_False.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolInt_State_Enabled_On_True_Off_True_Prerequisites_AlwaysOn_Should_Return_True.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_BoolInt_State_Enabled_On_True_Off_True_Prerequisites_AlwaysOn_Should_Return_True.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntBool_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_011.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntBool_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_011.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntBool_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_2.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntBool_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_2.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntBool_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_011.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntBool_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_011.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntBool_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_2.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntBool_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_2.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntInt_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_011.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntInt_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_011.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntInt_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_2.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntInt_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_2.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntInt_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_011.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntInt_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_011.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntInt_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_2.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntInt_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_2.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntJson_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_011.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntJson_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_011.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntJson_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_2.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntJson_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_2.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntJson_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_011.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntJson_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_011.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntJson_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_2.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntJson_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_2.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntString_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_011.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntString_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_011.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntString_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_2.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntString_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOff_Should_Return_2.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntString_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_011.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntString_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_011.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntString_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_2.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_IntString_State_Enabled_On_2_Off_011_Prerequisites_AlwaysOn_Should_Return_2.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_JsonJson_State_Enabled_On_com_Off_val_Prerequisites_AlwaysOff_Should_Return_Com.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_JsonJson_State_Enabled_On_com_Off_val_Prerequisites_AlwaysOff_Should_Return_Com.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_JsonJson_State_Enabled_On_com_Off_val_Prerequisites_AlwaysOff_Should_Return_Val.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_JsonJson_State_Enabled_On_com_Off_val_Prerequisites_AlwaysOff_Should_Return_Val.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_JsonJson_State_Enabled_On_com_Off_val_Prerequisites_AlwaysOn_Should_Return_Com.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_JsonJson_State_Enabled_On_com_Off_val_Prerequisites_AlwaysOn_Should_Return_Com.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_JsonJson_State_Enabled_On_com_Off_val_Prerequisites_AlwaysOn_Should_Return_Val.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_JsonJson_State_Enabled_On_com_Off_val_Prerequisites_AlwaysOn_Should_Return_Val.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_StrStr_State_Enabled_On_s19_Off_s53_Prerequisites_AlwaysOff_Should_Return_off.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_StrStr_State_Enabled_On_s19_Off_s53_Prerequisites_AlwaysOff_Should_Return_off.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_StrStr_State_Enabled_On_s19_Off_s53_Prerequisites_AlwaysOff_Should_Return_on.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_StrStr_State_Enabled_On_s19_Off_s53_Prerequisites_AlwaysOff_Should_Return_on.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_StrStr_State_Enabled_On_s19_Off_s53_Prerequisites_AlwaysOn_Should_Return_Off.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_StrStr_State_Enabled_On_s19_Off_s53_Prerequisites_AlwaysOn_Should_Return_Off.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/Prerequisites/Type_StrStr_State_Enabled_On_s19_Off_s53_Prerequisites_AlwaysOn_Should_Return_On.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/Prerequisites/Type_StrStr_State_Enabled_On_s19_Off_s53_Prerequisites_AlwaysOn_Should_Return_On.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Bool_State_Disabled_Should_Return_Default_Off_Value.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Bool_State_Disabled_Should_Return_Default_Off_Value.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Bool_State_Enabled_Should_Return_false_for_Target_four.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Bool_State_Enabled_Should_Return_false_for_Target_four.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Bool_State_Enabled_Should_Return_false_for_Target_six.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Bool_State_Enabled_Should_Return_false_for_Target_six.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Bool_State_Enabled_Should_Return_true_for_Target_three.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Bool_State_Enabled_Should_Return_true_for_Target_three.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_JSON_State_Enabled_Should_Return_complexJSON_for_Target_five.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_JSON_State_Enabled_Should_Return_complexJSON_for_Target_five.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_JSON_State_Enabled_Should_Return_emptyJSON_for_Target_four.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_JSON_State_Enabled_Should_Return_emptyJSON_for_Target_four.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_JSON_State_Enabled_Should_Return_validJSON_for_Target_anonymous.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_JSON_State_Enabled_Should_Return_validJSON_for_Target_anonymous.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Number_State_Enabled_Should_Return_2_for_Target_four.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Number_State_Enabled_Should_Return_2_for_Target_four.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Number_State_Enabled_Should_Return_324523_for_Target_five.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Number_State_Enabled_Should_Return_324523_for_Target_five.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Number_State_Enabled_Should_Return_sonnet53_for_Target_anonymous.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_Number_State_Enabled_Should_Return_sonnet53_for_Target_anonymous.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_String_State_Enabled_Should_Return_sonnet53_for_Target_anonymous.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_String_State_Enabled_Should_Return_sonnet53_for_Target_anonymous.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_String_State_Enabled_Should_Return_sonnet53_for_Target_four.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_String_State_Enabled_Should_Return_sonnet53_for_Target_four.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_String_State_Enabled_Should_Return_thehobbit_for_Target_five.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/TargetRules/TargetRules_Type_String_State_Enabled_Should_Return_thehobbit_for_Target_five.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/bool_on_simple_rule.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/bool_on_simple_rule.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/off_flag.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/off_flag.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/off_off_no_rules.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/off_off_no_rules.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/on_off_no_rules.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/on_off_no_rules.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/prereq.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/prereq.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/rules_priority.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/rules_priority.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/segment_includes_target.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/segment_includes_target.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/tests/test_empty_or_missing_target_attributes.json` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/tests/test_empty_or_missing_target_attributes.json`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/types.gen.go` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/types.gen.go`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/ff-test-cases/validator.go` & `harness-featureflags-1.2.2/tests/integration/ff-test-cases/validator.go`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/test_clause.py` & `harness-featureflags-1.2.2/tests/integration/test_clause.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/test_evaluator.py` & `harness-featureflags-1.2.2/tests/integration/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/integration/test_feature.py` & `harness-featureflags-1.2.2/tests/integration/test_feature.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/test_client.py` & `harness-featureflags-1.2.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/unit/test_clause.py` & `harness-featureflags-1.2.2/tests/unit/test_clause.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/unit/test_evaluator.py` & `harness-featureflags-1.2.2/tests/unit/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/unit/test_integer.py` & `harness-featureflags-1.2.2/tests/unit/test_integer.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/unit/test_lru.py` & `harness-featureflags-1.2.2/tests/unit/test_lru.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/unit/test_number.py` & `harness-featureflags-1.2.2/tests/unit/test_number.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/unit/test_sdk_logging_codes.py` & `harness-featureflags-1.2.2/tests/unit/test_sdk_logging_codes.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/unit/test_sse_client.py` & `harness-featureflags-1.2.2/tests/unit/test_sse_client.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/unit/test_string.py` & `harness-featureflags-1.2.2/tests/unit/test_string.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/unit/test_target.py` & `harness-featureflags-1.2.2/tests/unit/test_target.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/unit/test_utils.py` & `harness-featureflags-1.2.2/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `harness-featureflags-1.2.1/tests/unit/test_variation.py` & `harness-featureflags-1.2.2/tests/unit/test_variation.py`

 * *Files identical despite different names*

