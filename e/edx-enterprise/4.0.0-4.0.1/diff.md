# Comparing `tmp/edx-enterprise-4.0.0.tar.gz` & `tmp/edx-enterprise-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-4.0.0.tar", last modified: Thu Jul 13 16:31:54 2023, max compression
+gzip compressed data, was "edx-enterprise-4.0.1.tar", last modified: Mon Jul 17 18:43:29 2023, max compression
```

## Comparing `edx-enterprise-4.0.0.tar` & `edx-enterprise-4.0.1.tar`

### file list

```diff
@@ -1,767 +1,767 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.879406 edx-enterprise-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)   137250 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35136 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)   185995 2023-07-13 16:31:54.879406 edx-enterprise-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.815406 edx-enterprise-4.0.0/consent/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.815406 edx-enterprise-4.0.0/consent/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.815406 edx-enterprise-4.0.0/consent/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/api/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.819406 edx-enterprise-4.0.0/consent/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.819406 edx-enterprise-4.0.0/consent/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/migrations/0002_migrate_to_new_data_sharing_consent.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/migrations/0003_historicaldatasharingconsent_history_change_reason.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/migrations/0004_datasharingconsenttextoverrides.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/migrations/0005_auto_20230707_0755.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/consent/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.819406 edx-enterprise-4.0.0/edx_enterprise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)   185995 2023-07-13 16:31:53.000000 edx-enterprise-4.0.0/edx_enterprise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    38833 2023-07-13 16:31:54.000000 edx-enterprise-4.0.0/edx_enterprise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:31:53.000000 edx-enterprise-4.0.0/edx_enterprise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:31:53.000000 edx-enterprise-4.0.0/edx_enterprise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-13 16:31:53.000000 edx-enterprise-4.0.0/edx_enterprise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-13 16:31:53.000000 edx-enterprise-4.0.0/edx_enterprise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.819406 edx-enterprise-4.0.0/enterprise/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.823406 edx-enterprise-4.0.0/enterprise/admin/
--rw-r--r--   0 runner    (1001) docker     (123)    32944 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/admin/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    30210 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/admin/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/admin/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/admin/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36495 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/admin/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/admin/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.823406 edx-enterprise-4.0.0/enterprise/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/throttles.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.823406 edx-enterprise-4.0.0/enterprise/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    57862 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.823406 edx-enterprise-4.0.0/enterprise/api/v1/views/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/views/base_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/views/coupon_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_catalog_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_course_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_customer_branding_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_customer_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_customer_invite_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_customer_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_customer_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    28693 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_subsidy_fulfillment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/views/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/views/pending_enterprise_customer_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api/v1/views/plotly_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.827406 edx-enterprise-4.0.0/enterprise/api_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15199 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api_client/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api_client/ecommerce.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api_client/enterprise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api_client/enterprise_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/api_client/lms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.811406 edx-enterprise-4.0.0/enterprise/conf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.811406 edx-enterprise-4.0.0/enterprise/conf/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.811406 edx-enterprise-4.0.0/enterprise/conf/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.827406 edx-enterprise-4.0.0/enterprise/conf/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/conf/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.827406 edx-enterprise-4.0.0/enterprise/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/config/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.827406 edx-enterprise-4.0.0/enterprise/heartbeat/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/heartbeat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/heartbeat/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/heartbeat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/heartbeat/throttles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/heartbeat/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/heartbeat/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.811406 edx-enterprise-4.0.0/enterprise/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.811406 edx-enterprise-4.0.0/enterprise/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.827406 edx-enterprise-4.0.0/enterprise/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    41500 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.811406 edx-enterprise-4.0.0/enterprise/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.827406 edx-enterprise-4.0.0/enterprise/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   104293 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/locale/eo/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/locale/eo/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.811406 edx-enterprise-4.0.0/enterprise/locale/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.827406 edx-enterprise-4.0.0/enterprise/locale/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/locale/es_419/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    45236 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/locale/es_419/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.827406 edx-enterprise-4.0.0/enterprise/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.827406 edx-enterprise-4.0.0/enterprise/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/commands/backfill_learner_role_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/commands/bulk_update_catalog_query_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/commands/create_enterprise_course_enrollments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/commands/create_missing_dsc_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/commands/email_drip_for_missing_dsc_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/commands/ensure_singular_active_enterprise_customer_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/commands/fix_dsc_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/commands/migrate_enterprise_catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32481 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/commands/monthly_impact_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/commands/nudge_dormant_enrolled_enterprise_learners.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/commands/revert_enrollment_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/commands/save_enterprise_customer_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    14043 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/commands/seed_enterprise_devstack_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/commands/unlink_enterprise_customer_learners.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/commands/update_config_last_errored_at.py
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/management/commands/update_role_assignments_with_customers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.835406 edx-enterprise-4.0.0/enterprise/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0001_auto_20210111_1253.py
--rw-r--r--   0 runner    (1001) docker     (123)    52500 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0001_squashed_0092_auto_20200312_1650.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0093_add_use_enterprise_catalog_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0094_add_use_enterprise_catalog_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0095_auto_20200507_1138.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0096_enterprise_catalog_admin_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0097_auto_20200619_1130.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0098_auto_20200629_1756.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0099_auto_20200702_1537.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0100_add_licensed_enterprise_course_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0101_move_data_to_saved_for_later.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0102_auto_20200708_1615.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0103_remove_marked_done.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0104_sync_query_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0105_add_branding_config_color_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0106_move_branding_config_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0107_remove_branding_config_banner_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0108_add_licensed_enrollment_is_revoked.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0109_remove_use_enterprise_catalog_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0110_add_default_contract_discount.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0111_pendingenterprisecustomeradminuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0112_auto_20200914_0926.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0113_auto_20200914_2054.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0114_auto_20201020_0142.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0115_enterpriseanalyticsuser_historicalenterpriseanalyticsuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0116_auto_20201116_0400.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0116_auto_20201208_1759.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0117_auto_20201215_0258.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0120_systemwiderole_applies_to_all_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0121_systemwiderole_add_ent_cust_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0122_remove_field_sync_enterprise_catalog_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0123_enterprisecustomeridentityprovider_default_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0124_auto_20210301_1309.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0125_add_config_for_role_assign_backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0126_auto_20210308_1522.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0127_enterprisecatalogquery_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0128_enterprisecatalogquery_generate_uuids.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0129_enterprisecatalogquery_uuid_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0130_lms_customer_lp_search_help_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0131_auto_20210517_0924.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0132_auto_20210608_1921.py
--rw-r--r--   0 runner    (1001) docker     (123)    26436 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0133_auto_20210608_1931.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0134_enterprisecustomerreportingconfiguration_enable_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0135_adminnotification_adminnotificationfilter_adminnotificationread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0136_auto_20210629_2129.py
--rw-r--r--   0 runner    (1001) docker     (123)    16936 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0137_enrollment_email_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0138_bulkcatalogqueryupdatecommandconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0139_auto_20210803_1854.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0140_update_enrollment_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0141_make_enterprisecatalogquery_title_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0142_auto_20210907_2059.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0143_auto_20210908_0559.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0144_auto_20211011_1030.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0145_auto_20211013_1018.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0146_enterprise_customer_invite_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0147_auto_20211129_1949.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0148_auto_20211129_2114.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0149_invite_key_required_default_expiry_backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0150_invite_key_expiry_required.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0151_add_is_active_to_invite_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0152_add_should_inactivate_other_customers.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0153_add_enable_browse_and_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0154_alter_systemwideenterpriseuserroleassignment_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0155_add_is_relinkable_to_enterprise_customer_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0156_add_is_active_role_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0157_make_field_nullable_before_removal.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0158_remove_is_active_from_role_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0159_add_enable_learner_portal_offers.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0160_add_enable_portal_learner_credit_management_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0161_alter_enterprisecustomerreportingconfiguration_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0162_add_enable_executive_education_2U_fulfillment.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0163_auto_20220928_1611.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0164_enterprisecatalogquery_include_exec_ed_2u_courses.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0165_alter_enterprisecustomerreportingconfiguration_pgp_encryption_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0166_auto_20221209_0819.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0167_auto_20230209_2108.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0168_auto_20230222_1621.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0169_auto_20230222_1621.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0170_auto_20230301_1627.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0171_auto_20230503_1413.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0172_auto_20230517_1550.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0173_auto_20230531_1459.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/0174_auto_20230608_2041.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/migrations/unique_constraints_pending_users.py
--rw-r--r--   0 runner    (1001) docker     (123)   134534 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/roles_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.835406 edx-enterprise-4.0.0/enterprise/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/settings/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.811406 edx-enterprise-4.0.0/enterprise/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.811406 edx-enterprise-4.0.0/enterprise/static/enterprise/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.835406 edx-enterprise-4.0.0/enterprise/static/enterprise/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/static/enterprise/admin/enterprise_customer_catalog.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.835406 edx-enterprise-4.0.0/enterprise/static/enterprise/bundles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/static/enterprise/bundles/main-admin.style.css
--rw-r--r--   0 runner    (1001) docker     (123)   295145 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/static/enterprise/bundles/main.style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.839406 edx-enterprise-4.0.0/enterprise/static/enterprise/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/static/enterprise/js/course_modal.js
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/static/enterprise/js/enterprise_customer.js
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/static/enterprise/js/enterprise_login_page.js
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/static/enterprise/js/enterprise_selection_page.js
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/static/enterprise/js/grant_data_sharing_permissions.js
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/static/enterprise/js/manage_learners.js
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/static/enterprise/js/program_enrollment_landing_page.js
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.811406 edx-enterprise-4.0.0/enterprise/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.839406 edx-enterprise-4.0.0/enterprise/templates/enterprise/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/_data_sharing_decline_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/_data_sharing_policy.html
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/_data_sharing_policy_paragraph.html
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/_data_sharing_top_paragraph.html
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/_data_sharing_user_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/_enterprise_customer_sidebar.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.839406 edx-enterprise-4.0.0/enterprise/templates/enterprise/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/admin/clear_learners_data_sharing_consent.html
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/admin/enterprise_course_enrollments_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/admin/manage_learners.html
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/admin/oauth_authorization_failed.html
--rw-r--r--   0 runner    (1001) docker     (123)    27091 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/admin/oauth_authorization_successful.html
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/admin/transmit_courses_metadata.html
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/enterprise_course_enrollment_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/enterprise_customer_login_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/enterprise_customer_select_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/enterprise_error_page_with_messages.html
--rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/enterprise_program_enrollment_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/grant_data_sharing_permissions.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.839406 edx-enterprise-4.0.0/enterprise/templates/enterprise/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/templatetags/alert_messages.html
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/templatetags/course_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/templatetags/expand_button.html
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/templatetags/fa_icon.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.839406 edx-enterprise-4.0.0/enterprise/templates/enterprise/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templates/enterprise/widgets/segment-io-django.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.839406 edx-enterprise-4.0.0/enterprise/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/templatetags/enterprise.py
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/tpa_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    84670 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)   112485 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise/views_error_codes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.839406 edx-enterprise-4.0.0/enterprise_learner_portal/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise_learner_portal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.839406 edx-enterprise-4.0.0/enterprise_learner_portal/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise_learner_portal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise_learner_portal/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.843406 edx-enterprise-4.0.0/enterprise_learner_portal/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise_learner_portal/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise_learner_portal/api/v1/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise_learner_portal/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise_learner_portal/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise_learner_portal/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.843406 edx-enterprise-4.0.0/enterprise_learner_portal/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise_learner_portal/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise_learner_portal/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/enterprise_learner_portal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.843406 edx-enterprise-4.0.0/integrated_channels/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.843406 edx-enterprise-4.0.0/integrated_channels/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.843406 edx-enterprise-4.0.0/integrated_channels/api/v1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.843406 edx-enterprise-4.0.0/integrated_channels/api/v1/blackboard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/blackboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/blackboard/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/blackboard/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/blackboard/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.843406 edx-enterprise-4.0.0/integrated_channels/api/v1/canvas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/canvas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/canvas/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/canvas/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/canvas/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.843406 edx-enterprise-4.0.0/integrated_channels/api/v1/cornerstone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/cornerstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/cornerstone/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/cornerstone/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/cornerstone/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.843406 edx-enterprise-4.0.0/integrated_channels/api/v1/degreed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/degreed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/degreed/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/degreed/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/degreed/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.843406 edx-enterprise-4.0.0/integrated_channels/api/v1/degreed2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/degreed2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/degreed2/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/degreed2/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/degreed2/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.843406 edx-enterprise-4.0.0/integrated_channels/api/v1/logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/logs/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/logs/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/logs/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.843406 edx-enterprise-4.0.0/integrated_channels/api/v1/moodle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/moodle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/moodle/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/moodle/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/moodle/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.843406 edx-enterprise-4.0.0/integrated_channels/api/v1/sap_success_factors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/sap_success_factors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/sap_success_factors/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/sap_success_factors/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/sap_success_factors/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/api/v1/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.847406 edx-enterprise-4.0.0/integrated_channels/blackboard/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.847406 edx-enterprise-4.0.0/integrated_channels/blackboard/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    40081 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.847406 edx-enterprise-4.0.0/integrated_channels/blackboard/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.847406 edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0001_initial_squashed_0014_alter_blackboardlearnerassessmentdatatransmissionaudit_enterprise_course_enrollment_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0002_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0003_alter_blackboardlearnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0004_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0005_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0006_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0007_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0008_auto_20220913_2018.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0009_auto_20220929_1720.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0010_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0011_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0012_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0013_alter_blackboardlearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0014_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0015_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.847406 edx-enterprise-4.0.0/integrated_channels/blackboard/transmitters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/blackboard/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.847406 edx-enterprise-4.0.0/integrated_channels/canvas/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.847406 edx-enterprise-4.0.0/integrated_channels/canvas/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    38929 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.847406 edx-enterprise-4.0.0/integrated_channels/canvas/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.851406 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0002_auto_20200806_1632.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0003_delete_canvasglobalconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0004_adding_learner_data_to_canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0005_auto_20200909_1534.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0006_canvaslearnerassessmentdatatransmissionaudit.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0007_auto_20210222_2225.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0008_auto_20210707_0815.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0009_auto_20210708_1639.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0010_auto_20210909_1536.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0011_auto_20210923_1727.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0012_alter_canvasenterprisecustomerconfiguration_enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0013_auto_20211221_1535.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0014_auto_20220126_1837.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0015_auto_20220127_1605.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0016_auto_20220131_1539.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0017_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0018_alter_canvaslearnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0019_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0020_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0021_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0022_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0023_auto_20220913_2018.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0024_auto_20220929_1720.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0025_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0026_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0027_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0028_alter_canvaslearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0029_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0030_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.851406 edx-enterprise-4.0.0/integrated_channels/canvas/transmitters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/canvas/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/catalog_service_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.851406 edx-enterprise-4.0.0/integrated_channels/cornerstone/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.851406 edx-enterprise-4.0.0/integrated_channels/cornerstone/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.851406 edx-enterprise-4.0.0/integrated_channels/cornerstone/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.855406 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0002_cornerstoneglobalconfiguration_subject_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0003_auto_20190621_1000.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0004_cornerstoneglobalconfiguration_languages.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0005_auto_20190925_0730.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0006_auto_20191001_0742.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0007_auto_20210708_1446.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0008_auto_20210909_1536.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0009_auto_20210923_1727.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0010_cornerstonecoursekey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0011_auto_20211103_1855.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0012_alter_cornerstoneenterprisecustomerconfiguration_enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0013_auto_20220126_1837.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0014_auto_20220131_1539.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0015_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0016_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0017_alter_cornerstonelearnerdatatransmissionaudit_course_completed.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0018_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0019_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0020_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0021_cornerstonelearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0022_cornerstonelearnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0023_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0024_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0025_alter_cornerstonelearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0026_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0027_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.855406 edx-enterprise-4.0.0/integrated_channels/cornerstone/transmitters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/cornerstone/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.855406 edx-enterprise-4.0.0/integrated_channels/degreed/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.855406 edx-enterprise-4.0.0/integrated_channels/degreed/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.855406 edx-enterprise-4.0.0/integrated_channels/degreed/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.859406 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0002_auto_20180104_0103.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0003_auto_20180109_0712.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0004_auto_20180306_1251.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0005_auto_20180807_1302.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0006_upgrade_django_simple_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0007_auto_20190925_0730.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0008_auto_20191001_0742.py
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0009_auto_20210119_1546.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0010_auto_20210708_1446.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0011_auto_20210909_1536.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0012_auto_20210923_1727.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0013_alter_degreedenterprisecustomerconfiguration_enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0014_auto_20220126_1837.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0015_auto_20220131_1539.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0016_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0017_alter_degreedlearnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0018_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0019_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0020_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0021_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0022_degreedlearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0023_degreedlearnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0024_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0025_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0026_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0027_alter_degreedlearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0028_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0029_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.859406 edx-enterprise-4.0.0/integrated_channels/degreed/transmitters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed/transmitters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.859406 edx-enterprise-4.0.0/integrated_channels/degreed2/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.859406 edx-enterprise-4.0.0/integrated_channels/degreed2/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.859406 edx-enterprise-4.0.0/integrated_channels/degreed2/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.863406 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0002_auto_20211101_2021.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0003_alter_degreed2enterprisecustomerconfiguration_enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0004_auto_20220126_1837.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0005_auto_20220131_1539.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0006_auto_20220214_1627.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0007_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0008_degreed2learnerdatatransmissionaudit_course_completed.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0009_alter_degreed2learnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0010_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0011_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0012_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0013_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0014_degreed2learnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0015_degreed2learnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0016_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0017_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0018_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0019_alter_degreed2learnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0020_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0021_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.863406 edx-enterprise-4.0.0/integrated_channels/degreed2/transmitters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/degreed2/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.863406 edx-enterprise-4.0.0/integrated_channels/integrated_channel/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.863406 edx-enterprise-4.0.0/integrated_channels/integrated_channel/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/channel_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.863406 edx-enterprise-4.0.0/integrated_channels/integrated_channel/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32507 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    39607 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.863406 edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.863406 edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/backfill_course_end_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/backfill_missing_csod_foreign_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/backfill_missing_foreign_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/backfill_remote_action_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/cleanup_duplicate_assignment_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/mark_orphaned_content_metadata_audits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/reset_csod_remote_deleted_at.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/reset_sapsf_learner_transmissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/transmit_content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/transmit_learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/transmit_subsection_learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/unlink_inactive_sap_learners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/update_content_transmission_catalogs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.867406 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0001_squashed_0007_auto_20190925_0730.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0002_learnerdatatransmissionaudit_subsection_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0003_contentmetadataitemtransmission_content_last_changed.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0004_contentmetadataitemtransmission_enterprise_customer_catalog_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0005_auto_20211005_1052.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0006_contentmetadataitemtransmission_deleted_at.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0007_delete_learnerdatatransmissionaudit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0008_genericlearnerdatatransmissionaudit.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0009_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0010_genericenterprisecustomerpluginconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0011_contentmetadataitemtransmission_plugin_configuration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0012_alter_contentmetadataitemtransmission_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0013_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0014_genericenterprisecustomerpluginconfiguration_dry_run_mode_enabled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0015_auto_20220718_2113.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_content_title.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_marked_for.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0017_contentmetadataitemtransmission_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0018_genericlearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0019_merge_20220928_1842.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0020_auto_20220929_1712.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0021_remove_contentmetadataitemtransmission_api_response_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0022_alter_contentmetadataitemtransmission_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0023_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0024_genericenterprisecustomerpluginconfiguration_deleted_at.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0025_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0026_genericenterprisecustomerpluginconfiguration_last_modified_at.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0027_orphanedcontenttransmissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0028_alter_contentmetadataitemtransmission_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32216 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.867406 edx-enterprise-4.0.0/integrated_channels/integrated_channel/transmitters/
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    23829 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/integrated_channel/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/lms_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.867406 edx-enterprise-4.0.0/integrated_channels/moodle/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.867406 edx-enterprise-4.0.0/integrated_channels/moodle/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.867406 edx-enterprise-4.0.0/integrated_channels/moodle/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.871406 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0002_moodlelearnerdatatransmissionaudit.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0003_auto_20201006_1706.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0004_auto_20201105_1921.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0005_auto_20210708_1446.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0006_auto_20210909_1536.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0007_auto_20210923_1727.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0008_alter_moodleenterprisecustomerconfiguration_enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0009_auto_20220126_1837.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0010_auto_20220131_1539.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0011_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0012_alter_moodlelearnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0013_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0014_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0015_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0016_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0017_moodlelearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0018_moodlelearnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0019_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0020_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0021_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0022_auto_20221220_1527.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0023_alter_moodlelearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0024_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0025_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.871406 edx-enterprise-4.0.0/integrated_channels/moodle/transmitters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/moodle/transmitters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.871406 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.871406 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.871406 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/exporters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/exporters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.875406 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0001_squashed_0022_auto_20200206_1046_squashed_0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_enterprise_course_enrollment_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0002_alter_sapsuccessfactorsenterprisecustomerconfiguration_display_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0003_alter_sapsuccessfactorslearnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0004_auto_20220324_1550_squashed_0006_auto_20220330_1157.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0005_sapsuccessfactorsenterprisecustomerconfiguration_dry_run_mode_enabled.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0006_sapsuccessfactorslearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0007_sapsuccessfactorslearnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0008_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0009_sapsuccessfactorsenterprisecustomerconfiguration_deleted_at.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0010_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0012_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0013_sapsuccessfactorsenterprisecustomerconfiguration_last_modified_at.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.875406 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/transmitters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/sap_success_factors/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17708 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.875406 edx-enterprise-4.0.0/integrated_channels/xapi/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.875406 edx-enterprise-4.0.0/integrated_channels/xapi/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.875406 edx-enterprise-4.0.0/integrated_channels/xapi/management/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.875406 edx-enterprise-4.0.0/integrated_channels/xapi/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/management/commands/send_course_completions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/management/commands/send_course_enrollments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.875406 edx-enterprise-4.0.0/integrated_channels/xapi/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0002_auto_20180726_0142.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0003_auto_20190807_1006.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0004_auto_20190830_0710.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0005_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0006_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0007_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0008_xapilearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0009_xapilearnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0010_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0011_alter_xapilearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.875406 edx-enterprise-4.0.0/integrated_channels/xapi/statements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/statements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/statements/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/statements/learner_course_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/statements/learner_course_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/integrated_channels/xapi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:31:54.879406 edx-enterprise-4.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/celery50.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/common_constraints.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)    20535 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/django.txt
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/doc.in
--rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/edx-platform-constraints.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/js_test.in
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/js_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/test-master.in
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/test-master.txt
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-13 16:31:54.879406 edx-enterprise-4.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4028 2023-07-13 16:30:39.000000 edx-enterprise-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.089456 edx-enterprise-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)   137392 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35136 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)   186201 2023-07-17 18:43:29.089456 edx-enterprise-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.033456 edx-enterprise-4.0.1/consent/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.033456 edx-enterprise-4.0.1/consent/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.033456 edx-enterprise-4.0.1/consent/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/api/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.033456 edx-enterprise-4.0.1/consent/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.033456 edx-enterprise-4.0.1/consent/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/migrations/0002_migrate_to_new_data_sharing_consent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/migrations/0003_historicaldatasharingconsent_history_change_reason.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/migrations/0004_datasharingconsenttextoverrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/migrations/0005_auto_20230707_0755.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/consent/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.033456 edx-enterprise-4.0.1/edx_enterprise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)   186201 2023-07-17 18:43:28.000000 edx-enterprise-4.0.1/edx_enterprise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    38833 2023-07-17 18:43:28.000000 edx-enterprise-4.0.1/edx_enterprise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 18:43:28.000000 edx-enterprise-4.0.1/edx_enterprise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 18:43:28.000000 edx-enterprise-4.0.1/edx_enterprise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-17 18:43:28.000000 edx-enterprise-4.0.1/edx_enterprise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-17 18:43:28.000000 edx-enterprise-4.0.1/edx_enterprise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.037456 edx-enterprise-4.0.1/enterprise/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.037456 edx-enterprise-4.0.1/enterprise/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)    32944 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/admin/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30210 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/admin/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/admin/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/admin/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36495 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/admin/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/admin/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.037456 edx-enterprise-4.0.1/enterprise/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/throttles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.037456 edx-enterprise-4.0.1/enterprise/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57862 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.037456 edx-enterprise-4.0.1/enterprise/api/v1/views/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/views/base_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/views/coupon_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_catalog_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_course_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_customer_branding_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_customer_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_customer_invite_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_customer_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_customer_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28693 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_subsidy_fulfillment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/views/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/views/pending_enterprise_customer_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api/v1/views/plotly_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.037456 edx-enterprise-4.0.1/enterprise/api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15199 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api_client/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api_client/ecommerce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api_client/enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api_client/enterprise_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/api_client/lms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.025456 edx-enterprise-4.0.1/enterprise/conf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.025456 edx-enterprise-4.0.1/enterprise/conf/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.025456 edx-enterprise-4.0.1/enterprise/conf/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.037456 edx-enterprise-4.0.1/enterprise/conf/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/conf/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.041456 edx-enterprise-4.0.1/enterprise/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/config/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.041456 edx-enterprise-4.0.1/enterprise/heartbeat/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/heartbeat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/heartbeat/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/heartbeat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/heartbeat/throttles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/heartbeat/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/heartbeat/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.025456 edx-enterprise-4.0.1/enterprise/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.025456 edx-enterprise-4.0.1/enterprise/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.041456 edx-enterprise-4.0.1/enterprise/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    41500 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.025456 edx-enterprise-4.0.1/enterprise/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.041456 edx-enterprise-4.0.1/enterprise/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   104293 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/locale/eo/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/locale/eo/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.025456 edx-enterprise-4.0.1/enterprise/locale/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.041456 edx-enterprise-4.0.1/enterprise/locale/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/locale/es_419/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    45236 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/locale/es_419/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.041456 edx-enterprise-4.0.1/enterprise/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.041456 edx-enterprise-4.0.1/enterprise/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/commands/backfill_learner_role_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/commands/bulk_update_catalog_query_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/commands/create_enterprise_course_enrollments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/commands/create_missing_dsc_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/commands/email_drip_for_missing_dsc_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/commands/ensure_singular_active_enterprise_customer_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/commands/fix_dsc_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/commands/migrate_enterprise_catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32481 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/commands/monthly_impact_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/commands/nudge_dormant_enrolled_enterprise_learners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/commands/revert_enrollment_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/commands/save_enterprise_customer_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14043 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/commands/seed_enterprise_devstack_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/commands/unlink_enterprise_customer_learners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/commands/update_config_last_errored_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/management/commands/update_role_assignments_with_customers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.049456 edx-enterprise-4.0.1/enterprise/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0001_auto_20210111_1253.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52500 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0001_squashed_0092_auto_20200312_1650.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0093_add_use_enterprise_catalog_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0094_add_use_enterprise_catalog_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0095_auto_20200507_1138.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0096_enterprise_catalog_admin_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0097_auto_20200619_1130.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0098_auto_20200629_1756.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0099_auto_20200702_1537.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0100_add_licensed_enterprise_course_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0101_move_data_to_saved_for_later.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0102_auto_20200708_1615.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0103_remove_marked_done.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0104_sync_query_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0105_add_branding_config_color_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0106_move_branding_config_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0107_remove_branding_config_banner_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0108_add_licensed_enrollment_is_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0109_remove_use_enterprise_catalog_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0110_add_default_contract_discount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0111_pendingenterprisecustomeradminuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0112_auto_20200914_0926.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0113_auto_20200914_2054.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0114_auto_20201020_0142.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0115_enterpriseanalyticsuser_historicalenterpriseanalyticsuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0116_auto_20201116_0400.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0116_auto_20201208_1759.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0117_auto_20201215_0258.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0120_systemwiderole_applies_to_all_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0121_systemwiderole_add_ent_cust_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0122_remove_field_sync_enterprise_catalog_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0123_enterprisecustomeridentityprovider_default_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0124_auto_20210301_1309.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0125_add_config_for_role_assign_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0126_auto_20210308_1522.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0127_enterprisecatalogquery_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0128_enterprisecatalogquery_generate_uuids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0129_enterprisecatalogquery_uuid_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0130_lms_customer_lp_search_help_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0131_auto_20210517_0924.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0132_auto_20210608_1921.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26436 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0133_auto_20210608_1931.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0134_enterprisecustomerreportingconfiguration_enable_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0135_adminnotification_adminnotificationfilter_adminnotificationread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0136_auto_20210629_2129.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16936 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0137_enrollment_email_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0138_bulkcatalogqueryupdatecommandconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0139_auto_20210803_1854.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0140_update_enrollment_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0141_make_enterprisecatalogquery_title_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0142_auto_20210907_2059.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0143_auto_20210908_0559.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0144_auto_20211011_1030.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0145_auto_20211013_1018.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0146_enterprise_customer_invite_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0147_auto_20211129_1949.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0148_auto_20211129_2114.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0149_invite_key_required_default_expiry_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0150_invite_key_expiry_required.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0151_add_is_active_to_invite_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0152_add_should_inactivate_other_customers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0153_add_enable_browse_and_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0154_alter_systemwideenterpriseuserroleassignment_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0155_add_is_relinkable_to_enterprise_customer_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0156_add_is_active_role_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0157_make_field_nullable_before_removal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0158_remove_is_active_from_role_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0159_add_enable_learner_portal_offers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0160_add_enable_portal_learner_credit_management_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0161_alter_enterprisecustomerreportingconfiguration_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0162_add_enable_executive_education_2U_fulfillment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0163_auto_20220928_1611.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0164_enterprisecatalogquery_include_exec_ed_2u_courses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0165_alter_enterprisecustomerreportingconfiguration_pgp_encryption_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0166_auto_20221209_0819.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0167_auto_20230209_2108.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0168_auto_20230222_1621.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0169_auto_20230222_1621.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0170_auto_20230301_1627.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0171_auto_20230503_1413.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0172_auto_20230517_1550.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0173_auto_20230531_1459.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/0174_auto_20230608_2041.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/migrations/unique_constraints_pending_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134534 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/roles_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.049456 edx-enterprise-4.0.1/enterprise/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/settings/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.025456 edx-enterprise-4.0.1/enterprise/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.025456 edx-enterprise-4.0.1/enterprise/static/enterprise/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.049456 edx-enterprise-4.0.1/enterprise/static/enterprise/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/static/enterprise/admin/enterprise_customer_catalog.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.049456 edx-enterprise-4.0.1/enterprise/static/enterprise/bundles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/static/enterprise/bundles/main-admin.style.css
+-rw-r--r--   0 runner    (1001) docker     (123)   295145 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/static/enterprise/bundles/main.style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.049456 edx-enterprise-4.0.1/enterprise/static/enterprise/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/static/enterprise/js/course_modal.js
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/static/enterprise/js/enterprise_customer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/static/enterprise/js/enterprise_login_page.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/static/enterprise/js/enterprise_selection_page.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/static/enterprise/js/grant_data_sharing_permissions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/static/enterprise/js/manage_learners.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/static/enterprise/js/program_enrollment_landing_page.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.025456 edx-enterprise-4.0.1/enterprise/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.053456 edx-enterprise-4.0.1/enterprise/templates/enterprise/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/_data_sharing_decline_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/_data_sharing_policy.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/_data_sharing_policy_paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/_data_sharing_top_paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/_data_sharing_user_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/_enterprise_customer_sidebar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.053456 edx-enterprise-4.0.1/enterprise/templates/enterprise/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/admin/clear_learners_data_sharing_consent.html
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/admin/enterprise_course_enrollments_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/admin/manage_learners.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/admin/oauth_authorization_failed.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27091 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/admin/oauth_authorization_successful.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/admin/transmit_courses_metadata.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/enterprise_course_enrollment_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/enterprise_customer_login_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/enterprise_customer_select_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/enterprise_error_page_with_messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/enterprise_program_enrollment_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/grant_data_sharing_permissions.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.053456 edx-enterprise-4.0.1/enterprise/templates/enterprise/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/templatetags/alert_messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/templatetags/course_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/templatetags/expand_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/templatetags/fa_icon.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.053456 edx-enterprise-4.0.1/enterprise/templates/enterprise/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templates/enterprise/widgets/segment-io-django.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.053456 edx-enterprise-4.0.1/enterprise/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/templatetags/enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/tpa_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85180 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112485 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise/views_error_codes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.053456 edx-enterprise-4.0.1/enterprise_learner_portal/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise_learner_portal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.053456 edx-enterprise-4.0.1/enterprise_learner_portal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise_learner_portal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise_learner_portal/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.053456 edx-enterprise-4.0.1/enterprise_learner_portal/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise_learner_portal/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise_learner_portal/api/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise_learner_portal/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise_learner_portal/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise_learner_portal/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.053456 edx-enterprise-4.0.1/enterprise_learner_portal/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise_learner_portal/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise_learner_portal/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/enterprise_learner_portal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.053456 edx-enterprise-4.0.1/integrated_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.053456 edx-enterprise-4.0.1/integrated_channels/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.053456 edx-enterprise-4.0.1/integrated_channels/api/v1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.053456 edx-enterprise-4.0.1/integrated_channels/api/v1/blackboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/blackboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/blackboard/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/blackboard/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/blackboard/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.057456 edx-enterprise-4.0.1/integrated_channels/api/v1/canvas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/canvas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/canvas/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/canvas/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/canvas/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.057456 edx-enterprise-4.0.1/integrated_channels/api/v1/cornerstone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/cornerstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/cornerstone/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/cornerstone/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/cornerstone/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.057456 edx-enterprise-4.0.1/integrated_channels/api/v1/degreed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/degreed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/degreed/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/degreed/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/degreed/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.057456 edx-enterprise-4.0.1/integrated_channels/api/v1/degreed2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/degreed2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/degreed2/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/degreed2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/degreed2/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.057456 edx-enterprise-4.0.1/integrated_channels/api/v1/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/logs/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/logs/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/logs/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.057456 edx-enterprise-4.0.1/integrated_channels/api/v1/moodle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/moodle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/moodle/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/moodle/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/moodle/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.057456 edx-enterprise-4.0.1/integrated_channels/api/v1/sap_success_factors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/sap_success_factors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/sap_success_factors/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/sap_success_factors/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/sap_success_factors/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/api/v1/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.057456 edx-enterprise-4.0.1/integrated_channels/blackboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.057456 edx-enterprise-4.0.1/integrated_channels/blackboard/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40081 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.057456 edx-enterprise-4.0.1/integrated_channels/blackboard/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.061456 edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0001_initial_squashed_0014_alter_blackboardlearnerassessmentdatatransmissionaudit_enterprise_course_enrollment_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0002_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0003_alter_blackboardlearnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0004_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0005_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0006_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0007_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0008_auto_20220913_2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0009_auto_20220929_1720.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0010_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0011_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0012_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0013_alter_blackboardlearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0014_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0015_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.061456 edx-enterprise-4.0.1/integrated_channels/blackboard/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/blackboard/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.061456 edx-enterprise-4.0.1/integrated_channels/canvas/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.061456 edx-enterprise-4.0.1/integrated_channels/canvas/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38929 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.061456 edx-enterprise-4.0.1/integrated_channels/canvas/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.065456 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0002_auto_20200806_1632.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0003_delete_canvasglobalconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0004_adding_learner_data_to_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0005_auto_20200909_1534.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0006_canvaslearnerassessmentdatatransmissionaudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0007_auto_20210222_2225.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0008_auto_20210707_0815.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0009_auto_20210708_1639.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0010_auto_20210909_1536.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0011_auto_20210923_1727.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0012_alter_canvasenterprisecustomerconfiguration_enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0013_auto_20211221_1535.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0014_auto_20220126_1837.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0015_auto_20220127_1605.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0016_auto_20220131_1539.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0017_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0018_alter_canvaslearnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0019_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0020_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0021_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0022_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0023_auto_20220913_2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0024_auto_20220929_1720.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0025_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0026_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0027_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0028_alter_canvaslearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0029_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0030_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.065456 edx-enterprise-4.0.1/integrated_channels/canvas/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/canvas/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/catalog_service_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.065456 edx-enterprise-4.0.1/integrated_channels/cornerstone/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.065456 edx-enterprise-4.0.1/integrated_channels/cornerstone/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.065456 edx-enterprise-4.0.1/integrated_channels/cornerstone/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.065456 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0002_cornerstoneglobalconfiguration_subject_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0003_auto_20190621_1000.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0004_cornerstoneglobalconfiguration_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0005_auto_20190925_0730.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0006_auto_20191001_0742.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0007_auto_20210708_1446.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0008_auto_20210909_1536.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0009_auto_20210923_1727.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0010_cornerstonecoursekey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0011_auto_20211103_1855.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0012_alter_cornerstoneenterprisecustomerconfiguration_enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0013_auto_20220126_1837.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0014_auto_20220131_1539.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0015_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0016_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0017_alter_cornerstonelearnerdatatransmissionaudit_course_completed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0018_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0019_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0020_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0021_cornerstonelearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0022_cornerstonelearnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0023_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0024_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0025_alter_cornerstonelearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0026_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0027_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.065456 edx-enterprise-4.0.1/integrated_channels/cornerstone/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/cornerstone/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.069456 edx-enterprise-4.0.1/integrated_channels/degreed/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.069456 edx-enterprise-4.0.1/integrated_channels/degreed/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.069456 edx-enterprise-4.0.1/integrated_channels/degreed/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.069456 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0002_auto_20180104_0103.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0003_auto_20180109_0712.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0004_auto_20180306_1251.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0005_auto_20180807_1302.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0006_upgrade_django_simple_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0007_auto_20190925_0730.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0008_auto_20191001_0742.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0009_auto_20210119_1546.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0010_auto_20210708_1446.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0011_auto_20210909_1536.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0012_auto_20210923_1727.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0013_alter_degreedenterprisecustomerconfiguration_enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0014_auto_20220126_1837.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0015_auto_20220131_1539.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0016_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0017_alter_degreedlearnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0018_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0019_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0020_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0021_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0022_degreedlearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0023_degreedlearnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0024_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0025_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0026_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0027_alter_degreedlearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0028_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0029_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.069456 edx-enterprise-4.0.1/integrated_channels/degreed/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed/transmitters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.069456 edx-enterprise-4.0.1/integrated_channels/degreed2/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.069456 edx-enterprise-4.0.1/integrated_channels/degreed2/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.069456 edx-enterprise-4.0.1/integrated_channels/degreed2/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.073456 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0002_auto_20211101_2021.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0003_alter_degreed2enterprisecustomerconfiguration_enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0004_auto_20220126_1837.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0005_auto_20220131_1539.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0006_auto_20220214_1627.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0007_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0008_degreed2learnerdatatransmissionaudit_course_completed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0009_alter_degreed2learnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0010_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0011_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0012_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0013_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0014_degreed2learnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0015_degreed2learnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0016_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0017_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0018_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0019_alter_degreed2learnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0020_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0021_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.073456 edx-enterprise-4.0.1/integrated_channels/degreed2/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/degreed2/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.073456 edx-enterprise-4.0.1/integrated_channels/integrated_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.073456 edx-enterprise-4.0.1/integrated_channels/integrated_channel/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/channel_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.073456 edx-enterprise-4.0.1/integrated_channels/integrated_channel/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32507 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39607 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.073456 edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.077456 edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/backfill_course_end_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/backfill_missing_csod_foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/backfill_missing_foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/backfill_remote_action_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/cleanup_duplicate_assignment_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/mark_orphaned_content_metadata_audits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/reset_csod_remote_deleted_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/reset_sapsf_learner_transmissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/transmit_content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/transmit_learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/transmit_subsection_learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/unlink_inactive_sap_learners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/update_content_transmission_catalogs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.077456 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0001_squashed_0007_auto_20190925_0730.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0002_learnerdatatransmissionaudit_subsection_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0003_contentmetadataitemtransmission_content_last_changed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0004_contentmetadataitemtransmission_enterprise_customer_catalog_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0005_auto_20211005_1052.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0006_contentmetadataitemtransmission_deleted_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0007_delete_learnerdatatransmissionaudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0008_genericlearnerdatatransmissionaudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0009_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0010_genericenterprisecustomerpluginconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0011_contentmetadataitemtransmission_plugin_configuration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0012_alter_contentmetadataitemtransmission_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0013_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0014_genericenterprisecustomerpluginconfiguration_dry_run_mode_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0015_auto_20220718_2113.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_content_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_marked_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0017_contentmetadataitemtransmission_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0018_genericlearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0019_merge_20220928_1842.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0020_auto_20220929_1712.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0021_remove_contentmetadataitemtransmission_api_response_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0022_alter_contentmetadataitemtransmission_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0023_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0024_genericenterprisecustomerpluginconfiguration_deleted_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0025_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0026_genericenterprisecustomerpluginconfiguration_last_modified_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0027_orphanedcontenttransmissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0028_alter_contentmetadataitemtransmission_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32216 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.077456 edx-enterprise-4.0.1/integrated_channels/integrated_channel/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23829 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/integrated_channel/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/lms_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.077456 edx-enterprise-4.0.1/integrated_channels/moodle/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.077456 edx-enterprise-4.0.1/integrated_channels/moodle/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.077456 edx-enterprise-4.0.1/integrated_channels/moodle/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.081456 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0002_moodlelearnerdatatransmissionaudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0003_auto_20201006_1706.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0004_auto_20201105_1921.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0005_auto_20210708_1446.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0006_auto_20210909_1536.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0007_auto_20210923_1727.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0008_alter_moodleenterprisecustomerconfiguration_enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0009_auto_20220126_1837.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0010_auto_20220131_1539.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0011_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0012_alter_moodlelearnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0013_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0014_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0015_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0016_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0017_moodlelearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0018_moodlelearnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0019_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0020_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0021_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0022_auto_20221220_1527.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0023_alter_moodlelearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0024_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0025_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.081456 edx-enterprise-4.0.1/integrated_channels/moodle/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/moodle/transmitters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.081456 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.081456 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.081456 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/exporters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/exporters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.085456 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0001_squashed_0022_auto_20200206_1046_squashed_0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_enterprise_course_enrollment_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0002_alter_sapsuccessfactorsenterprisecustomerconfiguration_display_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0003_alter_sapsuccessfactorslearnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0004_auto_20220324_1550_squashed_0006_auto_20220330_1157.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0005_sapsuccessfactorsenterprisecustomerconfiguration_dry_run_mode_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0006_sapsuccessfactorslearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0007_sapsuccessfactorslearnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0008_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0009_sapsuccessfactorsenterprisecustomerconfiguration_deleted_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0010_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0012_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0013_sapsuccessfactorsenterprisecustomerconfiguration_last_modified_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.085456 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/sap_success_factors/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17708 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.085456 edx-enterprise-4.0.1/integrated_channels/xapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.085456 edx-enterprise-4.0.1/integrated_channels/xapi/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.085456 edx-enterprise-4.0.1/integrated_channels/xapi/management/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.085456 edx-enterprise-4.0.1/integrated_channels/xapi/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/management/commands/send_course_completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/management/commands/send_course_enrollments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.085456 edx-enterprise-4.0.1/integrated_channels/xapi/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0002_auto_20180726_0142.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0003_auto_20190807_1006.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0004_auto_20190830_0710.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0005_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0006_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0007_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0008_xapilearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0009_xapilearnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0010_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0011_alter_xapilearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.085456 edx-enterprise-4.0.1/integrated_channels/xapi/statements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/statements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/statements/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/statements/learner_course_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/statements/learner_course_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/integrated_channels/xapi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:43:29.089456 edx-enterprise-4.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/celery50.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/common_constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20535 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/django.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/doc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/edx-platform-constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/js_test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/js_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/test-master.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/test-master.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-17 18:43:29.089456 edx-enterprise-4.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4028 2023-07-17 18:42:24.000000 edx-enterprise-4.0.1/setup.py
```

### Comparing `edx-enterprise-4.0.0/CHANGELOG.rst` & `edx-enterprise-4.0.1/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,22 @@
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+[4.0.1]
+--------
+chore: upgrade course_enrollment from audit to verified
+
+[4.0.0]
+--------
+chore: upgrade node from version 16 to version 18
+
 [3.69.1]
 --------
 fix: content metadata exporter sanitizing content to delete
 
 [3.69.0]
 --------
 refactor: Replaced the deprecated `NullBooleanField` with `BooleanField(null=True)`
```

### Comparing `edx-enterprise-4.0.0/LICENSE` & `edx-enterprise-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/PKG-INFO` & `edx-enterprise-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-enterprise
-Version: 4.0.0
+Version: 4.0.1
 Summary: Your project description goes here
 Home-page: https://github.com/openedx/edx-enterprise
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Description: enterprise
         ==========
@@ -90,14 +90,22 @@
         
            This project adheres to Semantic Versioning (http://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         ----------
+        [4.0.1]
+        --------
+        chore: upgrade course_enrollment from audit to verified
+        
+        [4.0.0]
+        --------
+        chore: upgrade node from version 16 to version 18
+        
         [3.69.1]
         --------
         fix: content metadata exporter sanitizing content to delete
         
         [3.69.0]
         --------
         refactor: Replaced the deprecated `NullBooleanField` with `BooleanField(null=True)`
```

### Comparing `edx-enterprise-4.0.0/README.rst` & `edx-enterprise-4.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/consent/__init__.py` & `edx-enterprise-4.0.1/consent/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/consent/admin/__init__.py` & `edx-enterprise-4.0.1/consent/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/consent/api/permissions.py` & `edx-enterprise-4.0.1/consent/api/permissions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/consent/api/v1/views.py` & `edx-enterprise-4.0.1/consent/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/consent/errors.py` & `edx-enterprise-4.0.1/consent/errors.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/consent/helpers.py` & `edx-enterprise-4.0.1/consent/helpers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/consent/migrations/0001_initial.py` & `edx-enterprise-4.0.1/consent/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/consent/migrations/0002_migrate_to_new_data_sharing_consent.py` & `edx-enterprise-4.0.1/consent/migrations/0002_migrate_to_new_data_sharing_consent.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/consent/migrations/0004_datasharingconsenttextoverrides.py` & `edx-enterprise-4.0.1/consent/migrations/0004_datasharingconsenttextoverrides.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/consent/migrations/0005_auto_20230707_0755.py` & `edx-enterprise-4.0.1/consent/migrations/0005_auto_20230707_0755.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/consent/mixins.py` & `edx-enterprise-4.0.1/consent/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/consent/models.py` & `edx-enterprise-4.0.1/consent/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/edx_enterprise.egg-info/PKG-INFO` & `edx-enterprise-4.0.1/edx_enterprise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-enterprise
-Version: 4.0.0
+Version: 4.0.1
 Summary: Your project description goes here
 Home-page: https://github.com/openedx/edx-enterprise
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Description: enterprise
         ==========
@@ -90,14 +90,22 @@
         
            This project adheres to Semantic Versioning (http://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         ----------
+        [4.0.1]
+        --------
+        chore: upgrade course_enrollment from audit to verified
+        
+        [4.0.0]
+        --------
+        chore: upgrade node from version 16 to version 18
+        
         [3.69.1]
         --------
         fix: content metadata exporter sanitizing content to delete
         
         [3.69.0]
         --------
         refactor: Replaced the deprecated `NullBooleanField` with `BooleanField(null=True)`
```

### Comparing `edx-enterprise-4.0.0/edx_enterprise.egg-info/SOURCES.txt` & `edx-enterprise-4.0.1/edx_enterprise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/edx_enterprise.egg-info/requires.txt` & `edx-enterprise-4.0.1/edx_enterprise.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/admin/__init__.py` & `edx-enterprise-4.0.1/enterprise/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/admin/actions.py` & `edx-enterprise-4.0.1/enterprise/admin/actions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/admin/forms.py` & `edx-enterprise-4.0.1/enterprise/admin/forms.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/admin/paginator.py` & `edx-enterprise-4.0.1/enterprise/admin/paginator.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/admin/utils.py` & `edx-enterprise-4.0.1/enterprise/admin/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/admin/views.py` & `edx-enterprise-4.0.1/enterprise/admin/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/__init__.py` & `edx-enterprise-4.0.1/enterprise/api/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/filters.py` & `edx-enterprise-4.0.1/enterprise/api/filters.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/pagination.py` & `edx-enterprise-4.0.1/enterprise/api/pagination.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/throttles.py` & `edx-enterprise-4.0.1/enterprise/api/throttles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/utils.py` & `edx-enterprise-4.0.1/enterprise/api/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/decorators.py` & `edx-enterprise-4.0.1/enterprise/api/v1/decorators.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/fields.py` & `edx-enterprise-4.0.1/enterprise/api/v1/fields.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/permissions.py` & `edx-enterprise-4.0.1/enterprise/api/v1/permissions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/serializers.py` & `edx-enterprise-4.0.1/enterprise/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/urls.py` & `edx-enterprise-4.0.1/enterprise/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/views/base_views.py` & `edx-enterprise-4.0.1/enterprise/api/v1/views/base_views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/views/coupon_codes.py` & `edx-enterprise-4.0.1/enterprise/api/v1/views/coupon_codes.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_catalog_query.py` & `edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_catalog_query.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_course_enrollment.py` & `edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_course_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_customer.py` & `edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_customer_branding_configuration.py` & `edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_customer_branding_configuration.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_customer_catalog.py` & `edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_customer_catalog.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_customer_invite_key.py` & `edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_customer_invite_key.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_customer_reporting.py` & `edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_customer_reporting.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_customer_user.py` & `edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_customer_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/views/enterprise_subsidy_fulfillment.py` & `edx-enterprise-4.0.1/enterprise/api/v1/views/enterprise_subsidy_fulfillment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/views/notifications.py` & `edx-enterprise-4.0.1/enterprise/api/v1/views/notifications.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/views/pending_enterprise_customer_user.py` & `edx-enterprise-4.0.1/enterprise/api/v1/views/pending_enterprise_customer_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api/v1/views/plotly_auth.py` & `edx-enterprise-4.0.1/enterprise/api/v1/views/plotly_auth.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api_client/client.py` & `edx-enterprise-4.0.1/enterprise/api_client/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api_client/discovery.py` & `edx-enterprise-4.0.1/enterprise/api_client/discovery.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api_client/ecommerce.py` & `edx-enterprise-4.0.1/enterprise/api_client/ecommerce.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api_client/enterprise.py` & `edx-enterprise-4.0.1/enterprise/api_client/enterprise.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api_client/enterprise_catalog.py` & `edx-enterprise-4.0.1/enterprise/api_client/enterprise_catalog.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/api_client/lms.py` & `edx-enterprise-4.0.1/enterprise/api_client/lms.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/apps.py` & `edx-enterprise-4.0.1/enterprise/apps.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/conf/locale/en/LC_MESSAGES/django.po` & `edx-enterprise-4.0.1/enterprise/conf/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/config/models.py` & `edx-enterprise-4.0.1/enterprise/config/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/constants.py` & `edx-enterprise-4.0.1/enterprise/constants.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/decorators.py` & `edx-enterprise-4.0.1/enterprise/decorators.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/errors.py` & `edx-enterprise-4.0.1/enterprise/errors.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/forms.py` & `edx-enterprise-4.0.1/enterprise/forms.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/heartbeat/checks.py` & `edx-enterprise-4.0.1/enterprise/heartbeat/checks.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/heartbeat/exceptions.py` & `edx-enterprise-4.0.1/enterprise/heartbeat/exceptions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/heartbeat/utils.py` & `edx-enterprise-4.0.1/enterprise/heartbeat/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/heartbeat/views.py` & `edx-enterprise-4.0.1/enterprise/heartbeat/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/locale/en/LC_MESSAGES/django.po` & `edx-enterprise-4.0.1/enterprise/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/locale/en/LC_MESSAGES/djangojs.po` & `edx-enterprise-4.0.1/enterprise/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/locale/eo/LC_MESSAGES/django.po` & `edx-enterprise-4.0.1/enterprise/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/locale/eo/LC_MESSAGES/djangojs.po` & `edx-enterprise-4.0.1/enterprise/locale/eo/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/locale/es_419/LC_MESSAGES/django.mo` & `edx-enterprise-4.0.1/enterprise/locale/es_419/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/locale/es_419/LC_MESSAGES/django.po` & `edx-enterprise-4.0.1/enterprise/locale/es_419/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/logging.py` & `edx-enterprise-4.0.1/enterprise/logging.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/management/commands/backfill_learner_role_assignments.py` & `edx-enterprise-4.0.1/enterprise/management/commands/backfill_learner_role_assignments.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/management/commands/bulk_update_catalog_query_id.py` & `edx-enterprise-4.0.1/enterprise/management/commands/bulk_update_catalog_query_id.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/management/commands/create_enterprise_course_enrollments.py` & `edx-enterprise-4.0.1/enterprise/management/commands/create_enterprise_course_enrollments.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/management/commands/create_missing_dsc_records.py` & `edx-enterprise-4.0.1/enterprise/management/commands/create_missing_dsc_records.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/management/commands/email_drip_for_missing_dsc_records.py` & `edx-enterprise-4.0.1/enterprise/management/commands/email_drip_for_missing_dsc_records.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/management/commands/ensure_singular_active_enterprise_customer_user.py` & `edx-enterprise-4.0.1/enterprise/management/commands/ensure_singular_active_enterprise_customer_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/management/commands/fix_dsc_records.py` & `edx-enterprise-4.0.1/enterprise/management/commands/fix_dsc_records.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/management/commands/migrate_enterprise_catalogs.py` & `edx-enterprise-4.0.1/enterprise/management/commands/migrate_enterprise_catalogs.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/management/commands/monthly_impact_report.py` & `edx-enterprise-4.0.1/enterprise/management/commands/monthly_impact_report.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/management/commands/nudge_dormant_enrolled_enterprise_learners.py` & `edx-enterprise-4.0.1/enterprise/management/commands/nudge_dormant_enrolled_enterprise_learners.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/management/commands/revert_enrollment_objects.py` & `edx-enterprise-4.0.1/enterprise/management/commands/revert_enrollment_objects.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/management/commands/save_enterprise_customer_users.py` & `edx-enterprise-4.0.1/enterprise/management/commands/save_enterprise_customer_users.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/management/commands/seed_enterprise_devstack_data.py` & `edx-enterprise-4.0.1/enterprise/management/commands/seed_enterprise_devstack_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/management/commands/unlink_enterprise_customer_learners.py` & `edx-enterprise-4.0.1/enterprise/management/commands/unlink_enterprise_customer_learners.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/management/commands/update_config_last_errored_at.py` & `edx-enterprise-4.0.1/enterprise/management/commands/update_config_last_errored_at.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/management/commands/update_role_assignments_with_customers.py` & `edx-enterprise-4.0.1/enterprise/management/commands/update_role_assignments_with_customers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/messages.py` & `edx-enterprise-4.0.1/enterprise/messages.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/middleware.py` & `edx-enterprise-4.0.1/enterprise/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0001_auto_20210111_1253.py` & `edx-enterprise-4.0.1/enterprise/migrations/0001_auto_20210111_1253.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0001_squashed_0092_auto_20200312_1650.py` & `edx-enterprise-4.0.1/enterprise/migrations/0001_squashed_0092_auto_20200312_1650.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0093_add_use_enterprise_catalog_flag.py` & `edx-enterprise-4.0.1/enterprise/migrations/0093_add_use_enterprise_catalog_flag.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0094_add_use_enterprise_catalog_sample.py` & `edx-enterprise-4.0.1/enterprise/migrations/0094_add_use_enterprise_catalog_sample.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0095_auto_20200507_1138.py` & `edx-enterprise-4.0.1/enterprise/migrations/0095_auto_20200507_1138.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0096_enterprise_catalog_admin_role.py` & `edx-enterprise-4.0.1/enterprise/migrations/0096_enterprise_catalog_admin_role.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0097_auto_20200619_1130.py` & `edx-enterprise-4.0.1/enterprise/migrations/0097_auto_20200619_1130.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0098_auto_20200629_1756.py` & `edx-enterprise-4.0.1/enterprise/migrations/0098_auto_20200629_1756.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0099_auto_20200702_1537.py` & `edx-enterprise-4.0.1/enterprise/migrations/0099_auto_20200702_1537.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0100_add_licensed_enterprise_course_enrollment.py` & `edx-enterprise-4.0.1/enterprise/migrations/0100_add_licensed_enterprise_course_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0101_move_data_to_saved_for_later.py` & `edx-enterprise-4.0.1/enterprise/migrations/0101_move_data_to_saved_for_later.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0102_auto_20200708_1615.py` & `edx-enterprise-4.0.1/enterprise/migrations/0102_auto_20200708_1615.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0104_sync_query_field.py` & `edx-enterprise-4.0.1/enterprise/migrations/0104_sync_query_field.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0105_add_branding_config_color_fields.py` & `edx-enterprise-4.0.1/enterprise/migrations/0105_add_branding_config_color_fields.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0106_move_branding_config_colors.py` & `edx-enterprise-4.0.1/enterprise/migrations/0106_move_branding_config_colors.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0107_remove_branding_config_banner_fields.py` & `edx-enterprise-4.0.1/enterprise/migrations/0107_remove_branding_config_banner_fields.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0108_add_licensed_enrollment_is_revoked.py` & `edx-enterprise-4.0.1/enterprise/migrations/0108_add_licensed_enrollment_is_revoked.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0109_remove_use_enterprise_catalog_sample.py` & `edx-enterprise-4.0.1/enterprise/migrations/0109_remove_use_enterprise_catalog_sample.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0110_add_default_contract_discount.py` & `edx-enterprise-4.0.1/enterprise/migrations/0110_add_default_contract_discount.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0111_pendingenterprisecustomeradminuser.py` & `edx-enterprise-4.0.1/enterprise/migrations/0111_pendingenterprisecustomeradminuser.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0112_auto_20200914_0926.py` & `edx-enterprise-4.0.1/enterprise/migrations/0112_auto_20200914_0926.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0113_auto_20200914_2054.py` & `edx-enterprise-4.0.1/enterprise/migrations/0113_auto_20200914_2054.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0114_auto_20201020_0142.py` & `edx-enterprise-4.0.1/enterprise/migrations/0114_auto_20201020_0142.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0115_enterpriseanalyticsuser_historicalenterpriseanalyticsuser.py` & `edx-enterprise-4.0.1/enterprise/migrations/0115_enterpriseanalyticsuser_historicalenterpriseanalyticsuser.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0116_auto_20201116_0400.py` & `edx-enterprise-4.0.1/enterprise/migrations/0116_auto_20201116_0400.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0116_auto_20201208_1759.py` & `edx-enterprise-4.0.1/enterprise/migrations/0116_auto_20201208_1759.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0117_auto_20201215_0258.py` & `edx-enterprise-4.0.1/enterprise/migrations/0117_auto_20201215_0258.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0120_systemwiderole_applies_to_all_contexts.py` & `edx-enterprise-4.0.1/enterprise/migrations/0120_systemwiderole_applies_to_all_contexts.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0121_systemwiderole_add_ent_cust_field.py` & `edx-enterprise-4.0.1/enterprise/migrations/0121_systemwiderole_add_ent_cust_field.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0122_remove_field_sync_enterprise_catalog_query.py` & `edx-enterprise-4.0.1/enterprise/migrations/0122_remove_field_sync_enterprise_catalog_query.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0123_enterprisecustomeridentityprovider_default_provider.py` & `edx-enterprise-4.0.1/enterprise/migrations/0123_enterprisecustomeridentityprovider_default_provider.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0124_auto_20210301_1309.py` & `edx-enterprise-4.0.1/enterprise/migrations/0124_auto_20210301_1309.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0125_add_config_for_role_assign_backfill.py` & `edx-enterprise-4.0.1/enterprise/migrations/0125_add_config_for_role_assign_backfill.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0126_auto_20210308_1522.py` & `edx-enterprise-4.0.1/enterprise/migrations/0126_auto_20210308_1522.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0128_enterprisecatalogquery_generate_uuids.py` & `edx-enterprise-4.0.1/enterprise/migrations/0128_enterprisecatalogquery_generate_uuids.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0130_lms_customer_lp_search_help_text.py` & `edx-enterprise-4.0.1/enterprise/migrations/0130_lms_customer_lp_search_help_text.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0131_auto_20210517_0924.py` & `edx-enterprise-4.0.1/enterprise/migrations/0131_auto_20210517_0924.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0132_auto_20210608_1921.py` & `edx-enterprise-4.0.1/enterprise/migrations/0132_auto_20210608_1921.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0133_auto_20210608_1931.py` & `edx-enterprise-4.0.1/enterprise/migrations/0133_auto_20210608_1931.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0134_enterprisecustomerreportingconfiguration_enable_compression.py` & `edx-enterprise-4.0.1/enterprise/migrations/0134_enterprisecustomerreportingconfiguration_enable_compression.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0135_adminnotification_adminnotificationfilter_adminnotificationread.py` & `edx-enterprise-4.0.1/enterprise/migrations/0135_adminnotification_adminnotificationfilter_adminnotificationread.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0136_auto_20210629_2129.py` & `edx-enterprise-4.0.1/enterprise/migrations/0136_auto_20210629_2129.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0137_enrollment_email_update.py` & `edx-enterprise-4.0.1/enterprise/migrations/0137_enrollment_email_update.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0138_bulkcatalogqueryupdatecommandconfiguration.py` & `edx-enterprise-4.0.1/enterprise/migrations/0138_bulkcatalogqueryupdatecommandconfiguration.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0139_auto_20210803_1854.py` & `edx-enterprise-4.0.1/enterprise/migrations/0139_auto_20210803_1854.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0140_update_enrollment_sources.py` & `edx-enterprise-4.0.1/enterprise/migrations/0140_update_enrollment_sources.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0141_make_enterprisecatalogquery_title_unique.py` & `edx-enterprise-4.0.1/enterprise/migrations/0141_make_enterprisecatalogquery_title_unique.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0142_auto_20210907_2059.py` & `edx-enterprise-4.0.1/enterprise/migrations/0142_auto_20210907_2059.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0143_auto_20210908_0559.py` & `edx-enterprise-4.0.1/enterprise/migrations/0143_auto_20210908_0559.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0144_auto_20211011_1030.py` & `edx-enterprise-4.0.1/enterprise/migrations/0144_auto_20211011_1030.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0145_auto_20211013_1018.py` & `edx-enterprise-4.0.1/enterprise/migrations/0145_auto_20211013_1018.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0146_enterprise_customer_invite_key.py` & `edx-enterprise-4.0.1/enterprise/migrations/0146_enterprise_customer_invite_key.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0147_auto_20211129_1949.py` & `edx-enterprise-4.0.1/enterprise/migrations/0147_auto_20211129_1949.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0148_auto_20211129_2114.py` & `edx-enterprise-4.0.1/enterprise/migrations/0148_auto_20211129_2114.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0149_invite_key_required_default_expiry_backfill.py` & `edx-enterprise-4.0.1/enterprise/migrations/0149_invite_key_required_default_expiry_backfill.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0150_invite_key_expiry_required.py` & `edx-enterprise-4.0.1/enterprise/migrations/0150_invite_key_expiry_required.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0151_add_is_active_to_invite_key.py` & `edx-enterprise-4.0.1/enterprise/migrations/0151_add_is_active_to_invite_key.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0152_add_should_inactivate_other_customers.py` & `edx-enterprise-4.0.1/enterprise/migrations/0152_add_should_inactivate_other_customers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0153_add_enable_browse_and_request.py` & `edx-enterprise-4.0.1/enterprise/migrations/0153_add_enable_browse_and_request.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0154_alter_systemwideenterpriseuserroleassignment_unique_together.py` & `edx-enterprise-4.0.1/enterprise/migrations/0154_alter_systemwideenterpriseuserroleassignment_unique_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0155_add_is_relinkable_to_enterprise_customer_user.py` & `edx-enterprise-4.0.1/enterprise/migrations/0155_add_is_relinkable_to_enterprise_customer_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0156_add_is_active_role_assignment.py` & `edx-enterprise-4.0.1/enterprise/migrations/0156_add_is_active_role_assignment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0157_make_field_nullable_before_removal.py` & `edx-enterprise-4.0.1/enterprise/migrations/0157_make_field_nullable_before_removal.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0158_remove_is_active_from_role_assignment.py` & `edx-enterprise-4.0.1/enterprise/migrations/0158_remove_is_active_from_role_assignment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0159_add_enable_learner_portal_offers.py` & `edx-enterprise-4.0.1/enterprise/migrations/0159_add_enable_learner_portal_offers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0160_add_enable_portal_learner_credit_management_screen.py` & `edx-enterprise-4.0.1/enterprise/migrations/0160_add_enable_portal_learner_credit_management_screen.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0161_alter_enterprisecustomerreportingconfiguration_data_type.py` & `edx-enterprise-4.0.1/enterprise/migrations/0161_alter_enterprisecustomerreportingconfiguration_data_type.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0162_add_enable_executive_education_2U_fulfillment.py` & `edx-enterprise-4.0.1/enterprise/migrations/0162_add_enable_executive_education_2U_fulfillment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0163_auto_20220928_1611.py` & `edx-enterprise-4.0.1/enterprise/migrations/0163_auto_20220928_1611.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0164_enterprisecatalogquery_include_exec_ed_2u_courses.py` & `edx-enterprise-4.0.1/enterprise/migrations/0164_enterprisecatalogquery_include_exec_ed_2u_courses.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0165_alter_enterprisecustomerreportingconfiguration_pgp_encryption_key.py` & `edx-enterprise-4.0.1/enterprise/migrations/0165_alter_enterprisecustomerreportingconfiguration_pgp_encryption_key.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0166_auto_20221209_0819.py` & `edx-enterprise-4.0.1/enterprise/migrations/0166_auto_20221209_0819.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0167_auto_20230209_2108.py` & `edx-enterprise-4.0.1/enterprise/migrations/0167_auto_20230209_2108.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0168_auto_20230222_1621.py` & `edx-enterprise-4.0.1/enterprise/migrations/0168_auto_20230222_1621.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0169_auto_20230222_1621.py` & `edx-enterprise-4.0.1/enterprise/migrations/0169_auto_20230222_1621.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0170_auto_20230301_1627.py` & `edx-enterprise-4.0.1/enterprise/migrations/0170_auto_20230301_1627.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0171_auto_20230503_1413.py` & `edx-enterprise-4.0.1/enterprise/migrations/0171_auto_20230503_1413.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0172_auto_20230517_1550.py` & `edx-enterprise-4.0.1/enterprise/migrations/0172_auto_20230517_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0173_auto_20230531_1459.py` & `edx-enterprise-4.0.1/enterprise/migrations/0173_auto_20230531_1459.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/0174_auto_20230608_2041.py` & `edx-enterprise-4.0.1/enterprise/migrations/0174_auto_20230608_2041.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/migrations/unique_constraints_pending_users.py` & `edx-enterprise-4.0.1/enterprise/migrations/unique_constraints_pending_users.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/models.py` & `edx-enterprise-4.0.1/enterprise/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/roles_api.py` & `edx-enterprise-4.0.1/enterprise/roles_api.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/rules.py` & `edx-enterprise-4.0.1/enterprise/rules.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/settings/test.py` & `edx-enterprise-4.0.1/enterprise/settings/test.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/signals.py` & `edx-enterprise-4.0.1/enterprise/signals.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/static/enterprise/admin/enterprise_customer_catalog.js` & `edx-enterprise-4.0.1/enterprise/static/enterprise/admin/enterprise_customer_catalog.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/static/enterprise/bundles/main.style.css` & `edx-enterprise-4.0.1/enterprise/static/enterprise/bundles/main.style.css`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/static/enterprise/js/course_modal.js` & `edx-enterprise-4.0.1/enterprise/static/enterprise/js/course_modal.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/static/enterprise/js/enterprise_customer.js` & `edx-enterprise-4.0.1/enterprise/static/enterprise/js/enterprise_customer.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/static/enterprise/js/enterprise_login_page.js` & `edx-enterprise-4.0.1/enterprise/static/enterprise/js/enterprise_login_page.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/static/enterprise/js/enterprise_selection_page.js` & `edx-enterprise-4.0.1/enterprise/static/enterprise/js/enterprise_selection_page.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/static/enterprise/js/grant_data_sharing_permissions.js` & `edx-enterprise-4.0.1/enterprise/static/enterprise/js/grant_data_sharing_permissions.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/static/enterprise/js/manage_learners.js` & `edx-enterprise-4.0.1/enterprise/static/enterprise/js/manage_learners.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/static/enterprise/js/program_enrollment_landing_page.js` & `edx-enterprise-4.0.1/enterprise/static/enterprise/js/program_enrollment_landing_page.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/tasks.py` & `edx-enterprise-4.0.1/enterprise/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/_data_sharing_decline_modal.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/_data_sharing_decline_modal.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/_data_sharing_policy_paragraph.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/_data_sharing_policy_paragraph.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/_data_sharing_top_paragraph.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/_data_sharing_top_paragraph.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/_data_sharing_user_input.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/_data_sharing_user_input.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/_enterprise_customer_sidebar.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/_enterprise_customer_sidebar.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/admin/clear_learners_data_sharing_consent.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/admin/clear_learners_data_sharing_consent.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/admin/manage_learners.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/admin/manage_learners.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/admin/oauth_authorization_failed.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/admin/oauth_authorization_failed.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/admin/oauth_authorization_successful.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/admin/oauth_authorization_successful.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/admin/transmit_courses_metadata.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/admin/transmit_courses_metadata.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/base.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/base.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/enterprise_course_enrollment_page.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/enterprise_course_enrollment_page.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/enterprise_customer_login_page.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/enterprise_customer_login_page.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/enterprise_customer_select_form.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/enterprise_customer_select_form.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/enterprise_program_enrollment_page.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/enterprise_program_enrollment_page.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/grant_data_sharing_permissions.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/grant_data_sharing_permissions.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/templatetags/course_modal.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/templatetags/course_modal.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templates/enterprise/widgets/segment-io-django.html` & `edx-enterprise-4.0.1/enterprise/templates/enterprise/widgets/segment-io-django.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/templatetags/enterprise.py` & `edx-enterprise-4.0.1/enterprise/templatetags/enterprise.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/tpa_pipeline.py` & `edx-enterprise-4.0.1/enterprise/tpa_pipeline.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/urls.py` & `edx-enterprise-4.0.1/enterprise/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/utils.py` & `edx-enterprise-4.0.1/enterprise/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,21 @@
     PATHWAY_CUSTOMER_ADMIN_ENROLLMENT,
     PROGRAM_TYPE_DESCRIPTION,
     CourseModes,
 )
 from enterprise.logging import getEnterpriseLogger
 
 try:
-    from openedx.features.enterprise_support.enrollments.utils import lms_enroll_user_in_course
+    from openedx.features.enterprise_support.enrollments.utils import (
+        lms_enroll_user_in_course,
+        lms_update_or_create_enrollment,
+    )
 except ImportError:
     lms_enroll_user_in_course = None
+    lms_update_or_create_enrollment = None
 
 try:
     from openedx.core.djangoapps.course_groups.models import CourseUserGroup
     from openedx.core.djangoapps.enrollments.errors import CourseEnrollmentError
 except ImportError:
     CourseUserGroup = None
     CourseEnrollmentError = None
@@ -1788,25 +1792,38 @@
     enterprise_customer_user, __ = enterprise_customer_user_model().objects.get_or_create(
         enterprise_customer=enterprise_customer,
         user_id=user.id
     )
     succeeded = False
     new_enrollment = False
     enterprise_fulfillment_source_uuid = None
+    emet_enable_auto_upgrade_enrollment_mode = getattr(
+        settings,
+        'ENABLE_ENTERPRISE_BACKEND_EMET_AUTO_UPGRADE_ENROLLMENT_MODE',
+        False,
+    )
     try:
-        # enrolls a user in a course per LMS flow, but this method does not create enterprise records yet so we need to
-        # create it immediately after calling lms_enroll_user_in_course. lms_enroll_user_in_course can return None if
-        # Enrollment already exists, does not fail in this case.
-        new_enrollment = lms_enroll_user_in_course(
-            user.username,
-            course_id,
-            course_mode,
-            enterprise_customer.uuid,
-            is_active=True,
-        )
+        # enrolls a user in a course per LMS flow, but this method doesn't create enterprise records
+        # yet so we need to create it immediately after calling lms_update_or_create_enrollment.
+        if emet_enable_auto_upgrade_enrollment_mode:
+            new_enrollment = lms_update_or_create_enrollment(
+                user.username,
+                course_id,
+                course_mode,
+                is_active=True,
+                enterprise_uuid=enterprise_customer.uuid,
+            )
+        else:
+            new_enrollment = lms_enroll_user_in_course(
+                user.username,
+                course_id,
+                course_mode,
+                enterprise_customer.uuid,
+                is_active=True,
+            )
         succeeded = True
         LOGGER.info("Successfully enrolled user %s in course %s", user.id, course_id)
     except (CourseEnrollmentError, CourseUserGroup.DoesNotExist) as error:
         LOGGER.exception("Failed to enroll user %s in course %s", user.id, course_id, exc_info=error)
     if succeeded:
         # If we have a provided enrollment source, use that. Otherwise default to manual.
         if enrollment_source:
```

### Comparing `edx-enterprise-4.0.0/enterprise/validators.py` & `edx-enterprise-4.0.1/enterprise/validators.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/views.py` & `edx-enterprise-4.0.1/enterprise/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise/views_error_codes.txt` & `edx-enterprise-4.0.1/enterprise/views_error_codes.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise_learner_portal/api/v1/serializers.py` & `edx-enterprise-4.0.1/enterprise_learner_portal/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise_learner_portal/api/v1/views.py` & `edx-enterprise-4.0.1/enterprise_learner_portal/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/enterprise_learner_portal/utils.py` & `edx-enterprise-4.0.1/enterprise_learner_portal/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/serializers.py` & `edx-enterprise-4.0.1/integrated_channels/api/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/blackboard/serializers.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/blackboard/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/blackboard/views.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/blackboard/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/canvas/serializers.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/canvas/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/canvas/views.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/canvas/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/cornerstone/serializers.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/cornerstone/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/cornerstone/views.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/cornerstone/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/degreed/serializers.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/degreed/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/degreed/views.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/degreed/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/degreed2/serializers.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/degreed2/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/degreed2/views.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/degreed2/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/logs/serializers.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/logs/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/logs/urls.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/logs/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/logs/views.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/logs/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/mixins.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/moodle/serializers.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/moodle/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/moodle/views.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/moodle/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/sap_success_factors/serializers.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/sap_success_factors/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/sap_success_factors/views.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/sap_success_factors/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/urls.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/api/v1/views.py` & `edx-enterprise-4.0.1/integrated_channels/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/admin/__init__.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/apps.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/apps.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/client.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/exporters/content_metadata.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/exporters/learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0001_initial_squashed_0014_alter_blackboardlearnerassessmentdatatransmissionaudit_enterprise_course_enrollment_id.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0001_initial_squashed_0014_alter_blackboardlearnerassessmentdatatransmissionaudit_enterprise_course_enrollment_id.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0002_auto_20220302_2231.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0002_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0003_alter_blackboardlearnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0003_alter_blackboardlearnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0004_auto_20220324_1550.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0004_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0005_auto_20220325_1757.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0005_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0006_auto_20220405_2311.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0006_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0007_auto_20220523_1625.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0007_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0008_auto_20220913_2018.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0008_auto_20220913_2018.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0009_auto_20220929_1720.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0009_auto_20220929_1720.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0010_auto_20221021_0159.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0010_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0011_auto_20221031_1855.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0011_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0012_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0012_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0013_alter_blackboardlearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0013_alter_blackboardlearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0014_auto_20230105_2122.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0014_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/migrations/0015_auto_20230112_2002.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/migrations/0015_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/models.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/transmitters/content_metadata.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/transmitters/learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/blackboard/views.py` & `edx-enterprise-4.0.1/integrated_channels/blackboard/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/admin/__init__.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/client.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/exporters/content_metadata.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/exporters/learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0001_initial.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0002_auto_20200806_1632.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0002_auto_20200806_1632.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0004_adding_learner_data_to_canvas.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0004_adding_learner_data_to_canvas.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0005_auto_20200909_1534.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0005_auto_20200909_1534.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0006_canvaslearnerassessmentdatatransmissionaudit.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0006_canvaslearnerassessmentdatatransmissionaudit.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0007_auto_20210222_2225.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0007_auto_20210222_2225.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0008_auto_20210707_0815.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0008_auto_20210707_0815.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0009_auto_20210708_1639.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0009_auto_20210708_1639.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0010_auto_20210909_1536.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0010_auto_20210909_1536.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0011_auto_20210923_1727.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0011_auto_20210923_1727.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0012_alter_canvasenterprisecustomerconfiguration_enterprise_customer.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0012_alter_canvasenterprisecustomerconfiguration_enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0013_auto_20211221_1535.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0013_auto_20211221_1535.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0014_auto_20220126_1837.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0014_auto_20220126_1837.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0015_auto_20220127_1605.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0015_auto_20220127_1605.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0016_auto_20220131_1539.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0016_auto_20220131_1539.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0017_auto_20220302_2231.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0017_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0018_alter_canvaslearnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0018_alter_canvaslearnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0019_auto_20220324_1550.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0019_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0020_auto_20220325_1757.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0020_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0021_auto_20220405_2311.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0021_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0022_auto_20220523_1625.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0022_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0023_auto_20220913_2018.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0023_auto_20220913_2018.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0024_auto_20220929_1720.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0024_auto_20220929_1720.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0025_auto_20221021_0159.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0025_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0026_auto_20221031_1855.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0026_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0027_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0027_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0028_alter_canvaslearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0028_alter_canvaslearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0029_auto_20230105_2122.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0029_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/migrations/0030_auto_20230112_2002.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/migrations/0030_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/models.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/transmitters/content_metadata.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/transmitters/learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/utils.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/canvas/views.py` & `edx-enterprise-4.0.1/integrated_channels/canvas/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/catalog_service_utils.py` & `edx-enterprise-4.0.1/integrated_channels/catalog_service_utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/admin/__init__.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/client.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/exporters/content_metadata.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/exporters/learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0001_initial.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0003_auto_20190621_1000.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0003_auto_20190621_1000.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0005_auto_20190925_0730.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0005_auto_20190925_0730.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0006_auto_20191001_0742.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0006_auto_20191001_0742.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0007_auto_20210708_1446.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0007_auto_20210708_1446.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0008_auto_20210909_1536.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0008_auto_20210909_1536.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0009_auto_20210923_1727.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0009_auto_20210923_1727.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0010_cornerstonecoursekey.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0010_cornerstonecoursekey.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0011_auto_20211103_1855.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0011_auto_20211103_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0012_alter_cornerstoneenterprisecustomerconfiguration_enterprise_customer.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0012_alter_cornerstoneenterprisecustomerconfiguration_enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0013_auto_20220126_1837.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0013_auto_20220126_1837.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0014_auto_20220131_1539.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0014_auto_20220131_1539.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0015_auto_20220302_2231.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0015_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0016_auto_20220324_1550.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0016_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0018_auto_20220325_1757.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0018_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0019_auto_20220405_2311.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0019_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0020_auto_20220523_1625.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0020_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0021_cornerstonelearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0021_cornerstonelearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0022_cornerstonelearnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0022_cornerstonelearnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0023_auto_20221021_0159.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0023_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0024_auto_20221031_1855.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0024_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0025_alter_cornerstonelearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0025_alter_cornerstonelearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0026_auto_20230105_2122.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0026_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/migrations/0027_auto_20230112_2002.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/migrations/0027_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/models.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/transmitters/content_metadata.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/transmitters/learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/utils.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/cornerstone/views.py` & `edx-enterprise-4.0.1/integrated_channels/cornerstone/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/admin/__init__.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/client.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/exporters/content_metadata.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/exporters/learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0001_initial.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0002_auto_20180104_0103.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0002_auto_20180104_0103.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0003_auto_20180109_0712.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0003_auto_20180109_0712.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0004_auto_20180306_1251.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0004_auto_20180306_1251.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0005_auto_20180807_1302.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0005_auto_20180807_1302.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0006_upgrade_django_simple_history.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0006_upgrade_django_simple_history.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0007_auto_20190925_0730.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0007_auto_20190925_0730.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0008_auto_20191001_0742.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0008_auto_20191001_0742.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0009_auto_20210119_1546.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0009_auto_20210119_1546.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0010_auto_20210708_1446.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0010_auto_20210708_1446.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0011_auto_20210909_1536.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0011_auto_20210909_1536.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0012_auto_20210923_1727.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0012_auto_20210923_1727.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0013_alter_degreedenterprisecustomerconfiguration_enterprise_customer.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0013_alter_degreedenterprisecustomerconfiguration_enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0014_auto_20220126_1837.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0014_auto_20220126_1837.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0015_auto_20220131_1539.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0015_auto_20220131_1539.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0016_auto_20220302_2231.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0016_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0017_alter_degreedlearnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0017_alter_degreedlearnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0018_auto_20220324_1550.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0018_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0019_auto_20220325_1757.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0019_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0020_auto_20220405_2311.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0020_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0021_auto_20220523_1625.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0021_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0022_degreedlearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0022_degreedlearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0023_degreedlearnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0023_degreedlearnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0024_auto_20221021_0159.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0024_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0025_auto_20221031_1855.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0025_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0026_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0026_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0027_alter_degreedlearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0027_alter_degreedlearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0028_auto_20230105_2122.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0028_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/migrations/0029_auto_20230112_2002.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/migrations/0029_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/models.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/transmitters/content_metadata.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed/transmitters/learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/degreed/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/admin/__init__.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/client.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/exporters/content_metadata.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/exporters/learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0001_initial.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0002_auto_20211101_2021.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0002_auto_20211101_2021.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0003_alter_degreed2enterprisecustomerconfiguration_enterprise_customer.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0003_alter_degreed2enterprisecustomerconfiguration_enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0004_auto_20220126_1837.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0004_auto_20220126_1837.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0005_auto_20220131_1539.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0005_auto_20220131_1539.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0006_auto_20220214_1627.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0006_auto_20220214_1627.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0007_auto_20220302_2231.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0007_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0009_alter_degreed2learnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0009_alter_degreed2learnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0010_auto_20220324_1550.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0010_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0011_auto_20220325_1757.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0011_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0012_auto_20220405_2311.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0012_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0013_auto_20220523_1625.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0013_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0014_degreed2learnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0014_degreed2learnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0015_degreed2learnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0015_degreed2learnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0016_auto_20221021_0159.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0016_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0017_auto_20221031_1855.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0017_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0018_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0018_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0019_alter_degreed2learnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0019_alter_degreed2learnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0020_auto_20230105_2122.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0020_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/migrations/0021_auto_20230112_2002.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/migrations/0021_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/models.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/transmitters/content_metadata.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/degreed2/transmitters/learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/degreed2/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/admin/__init__.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/channel_settings.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/channel_settings.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/client.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/exporters/__init__.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/exporters/content_metadata.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/exporters/learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/__init__.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/backfill_course_end_dates.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/backfill_course_end_dates.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/backfill_missing_csod_foreign_keys.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/backfill_missing_csod_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/backfill_missing_foreign_keys.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/backfill_missing_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/backfill_remote_action_timestamps.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/backfill_remote_action_timestamps.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/cleanup_duplicate_assignment_records.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/cleanup_duplicate_assignment_records.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/mark_orphaned_content_metadata_audits.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/mark_orphaned_content_metadata_audits.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/reset_csod_remote_deleted_at.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/reset_csod_remote_deleted_at.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/reset_sapsf_learner_transmissions.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/reset_sapsf_learner_transmissions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/transmit_content_metadata.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/transmit_content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/transmit_learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/transmit_learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/transmit_subsection_learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/transmit_subsection_learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/unlink_inactive_sap_learners.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/unlink_inactive_sap_learners.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/management/commands/update_content_transmission_catalogs.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/management/commands/update_content_transmission_catalogs.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0001_squashed_0007_auto_20190925_0730.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0001_squashed_0007_auto_20190925_0730.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0003_contentmetadataitemtransmission_content_last_changed.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0003_contentmetadataitemtransmission_content_last_changed.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0004_contentmetadataitemtransmission_enterprise_customer_catalog_uuid.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0004_contentmetadataitemtransmission_enterprise_customer_catalog_uuid.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0008_genericlearnerdatatransmissionaudit.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0008_genericlearnerdatatransmissionaudit.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0009_auto_20220325_1757.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0009_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0010_genericenterprisecustomerpluginconfiguration.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0010_genericenterprisecustomerpluginconfiguration.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0013_auto_20220405_2311.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0013_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0014_genericenterprisecustomerpluginconfiguration_dry_run_mode_enabled.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0014_genericenterprisecustomerpluginconfiguration_dry_run_mode_enabled.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0015_auto_20220718_2113.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0015_auto_20220718_2113.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_marked_for.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_marked_for.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0017_contentmetadataitemtransmission_friendly_status_message.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0017_contentmetadataitemtransmission_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0018_genericlearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0018_genericlearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0020_auto_20220929_1712.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0020_auto_20220929_1712.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0022_alter_contentmetadataitemtransmission_index_together.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0022_alter_contentmetadataitemtransmission_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0023_auto_20221021_0159.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0023_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0025_auto_20230105_2122.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0025_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0026_genericenterprisecustomerpluginconfiguration_last_modified_at.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0026_genericenterprisecustomerpluginconfiguration_last_modified_at.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0027_orphanedcontenttransmissions.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0027_orphanedcontenttransmissions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/migrations/0028_alter_contentmetadataitemtransmission_unique_together.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/migrations/0028_alter_contentmetadataitemtransmission_unique_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/models.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/tasks.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/transmitters/__init__.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/transmitters/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/transmitters/content_metadata.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/integrated_channel/transmitters/learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/integrated_channel/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/lms_utils.py` & `edx-enterprise-4.0.1/integrated_channels/lms_utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/admin/__init__.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/client.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/exporters/content_metadata.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/exporters/learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0001_initial.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0002_moodlelearnerdatatransmissionaudit.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0002_moodlelearnerdatatransmissionaudit.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0003_auto_20201006_1706.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0003_auto_20201006_1706.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0004_auto_20201105_1921.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0004_auto_20201105_1921.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0005_auto_20210708_1446.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0005_auto_20210708_1446.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0006_auto_20210909_1536.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0006_auto_20210909_1536.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0007_auto_20210923_1727.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0007_auto_20210923_1727.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0008_alter_moodleenterprisecustomerconfiguration_enterprise_customer.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0008_alter_moodleenterprisecustomerconfiguration_enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0009_auto_20220126_1837.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0009_auto_20220126_1837.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0010_auto_20220131_1539.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0010_auto_20220131_1539.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0011_auto_20220302_2231.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0011_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0012_alter_moodlelearnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0012_alter_moodlelearnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0013_auto_20220324_1550.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0013_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0014_auto_20220325_1757.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0014_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0015_auto_20220405_2311.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0015_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0016_auto_20220523_1625.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0016_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0017_moodlelearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0017_moodlelearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0018_moodlelearnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0018_moodlelearnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0019_auto_20221021_0159.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0019_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0020_auto_20221031_1855.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0020_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0021_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0021_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0022_auto_20221220_1527.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0022_auto_20221220_1527.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0023_alter_moodlelearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0023_alter_moodlelearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0024_auto_20230105_2122.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0024_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/migrations/0025_auto_20230112_2002.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/migrations/0025_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/models.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/transmitters/content_metadata.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/moodle/transmitters/learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/moodle/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/admin/__init__.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/client.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/constants.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/constants.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/exporters/content_metadata.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/exporters/learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/exporters/utils.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/exporters/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0001_squashed_0022_auto_20200206_1046_squashed_0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_enterprise_course_enrollment_id.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0001_squashed_0022_auto_20200206_1046_squashed_0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_enterprise_course_enrollment_id.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0002_alter_sapsuccessfactorsenterprisecustomerconfiguration_display_name.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0002_alter_sapsuccessfactorsenterprisecustomerconfiguration_display_name.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0003_alter_sapsuccessfactorslearnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0003_alter_sapsuccessfactorslearnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0004_auto_20220324_1550_squashed_0006_auto_20220330_1157.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0004_auto_20220324_1550_squashed_0006_auto_20220330_1157.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0005_sapsuccessfactorsenterprisecustomerconfiguration_dry_run_mode_enabled.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0005_sapsuccessfactorsenterprisecustomerconfiguration_dry_run_mode_enabled.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0006_sapsuccessfactorslearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0006_sapsuccessfactorslearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0007_sapsuccessfactorslearnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0007_sapsuccessfactorslearnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0008_auto_20221021_0159.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0008_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0010_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0010_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0012_auto_20230105_2122.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0012_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/migrations/0013_sapsuccessfactorsenterprisecustomerconfiguration_last_modified_at.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/migrations/0013_sapsuccessfactorsenterprisecustomerconfiguration_last_modified_at.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/models.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/transmitters/content_metadata.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/sap_success_factors/transmitters/learner_data.py` & `edx-enterprise-4.0.1/integrated_channels/sap_success_factors/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/utils.py` & `edx-enterprise-4.0.1/integrated_channels/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/admin/__init__.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/client.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/management/commands/send_course_completions.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/management/commands/send_course_completions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/management/commands/send_course_enrollments.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/management/commands/send_course_enrollments.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0001_initial.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0002_auto_20180726_0142.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0002_auto_20180726_0142.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0003_auto_20190807_1006.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0003_auto_20190807_1006.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0005_auto_20220324_1550.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0005_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0006_auto_20220325_1757.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0006_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0007_auto_20220405_2311.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0007_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0008_xapilearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0008_xapilearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0009_xapilearnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0009_xapilearnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0010_auto_20221021_0159.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0010_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/migrations/0011_alter_xapilearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/migrations/0011_alter_xapilearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/models.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/statements/base.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/statements/base.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/statements/learner_course_completion.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/statements/learner_course_completion.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/statements/learner_course_enrollment.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/statements/learner_course_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/integrated_channels/xapi/utils.py` & `edx-enterprise-4.0.1/integrated_channels/xapi/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/requirements/base.in` & `edx-enterprise-4.0.1/requirements/base.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/requirements/ci.txt` & `edx-enterprise-4.0.1/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/requirements/common_constraints.txt` & `edx-enterprise-4.0.1/requirements/common_constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/requirements/constraints.txt` & `edx-enterprise-4.0.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/requirements/dev.in` & `edx-enterprise-4.0.1/requirements/dev.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/requirements/dev.txt` & `edx-enterprise-4.0.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/requirements/doc.txt` & `edx-enterprise-4.0.1/requirements/doc.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/requirements/edx-platform-constraints.txt` & `edx-enterprise-4.0.1/requirements/edx-platform-constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/requirements/js_test.txt` & `edx-enterprise-4.0.1/requirements/js_test.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/requirements/test-master.txt` & `edx-enterprise-4.0.1/requirements/test-master.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/requirements/test.in` & `edx-enterprise-4.0.1/requirements/test.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/requirements/test.txt` & `edx-enterprise-4.0.1/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.0.0/setup.py` & `edx-enterprise-4.0.1/setup.py`

 * *Files identical despite different names*

