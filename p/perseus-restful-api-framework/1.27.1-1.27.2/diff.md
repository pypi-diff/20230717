# Comparing `tmp/perseus_restful_api_framework-1.27.1.tar.gz` & `tmp/perseus_restful_api_framework-1.27.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perseus_restful_api_framework-1.27.1.tar", max compression
+gzip compressed data, was "perseus_restful_api_framework-1.27.2.tar", max compression
```

## Comparing `perseus_restful_api_framework-1.27.1.tar` & `perseus_restful_api_framework-1.27.2.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0    10202 2023-07-11 02:57:49.328434 perseus_restful_api_framework-1.27.1/CHANGELOG.md
--rw-r--r--   0        0        0     1089 2020-11-12 14:26:46.553799 perseus_restful_api_framework-1.27.1/LICENSE
--rw-r--r--   0        0        0     4530 2022-10-02 05:19:36.696561 perseus_restful_api_framework-1.27.1/README.md
--rw-r--r--   0        0        0     1140 2023-07-11 02:57:02.853879 perseus_restful_api_framework-1.27.1/pyproject.toml
--rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.404748 perseus_restful_api_framework-1.27.1/src/majormode/__init__.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.404886 perseus_restful_api_framework-1.27.1/src/majormode/perseus/__init__.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.405009 perseus_restful_api_framework-1.27.1/src/majormode/perseus/agent/__init__.py
--rwxr-xr-x   0        0        0    11953 2023-02-09 01:22:31.663266 perseus_restful_api_framework-1.27.1/src/majormode/perseus/agent/email_address_verification_agent.py
--rw-r--r--   0        0        0     3603 2023-02-09 01:21:55.716946 perseus_restful_api_framework-1.27.1/src/majormode/perseus/agent/email_sender_agent.py
--rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.405462 perseus_restful_api_framework-1.27.1/src/majormode/perseus/bootstrap/__init__.py
--rw-r--r--   0        0        0    17545 2023-02-09 01:22:31.663215 perseus_restful_api_framework-1.27.1/src/majormode/perseus/bootstrap/tornado_handler.py
--rw-r--r--   0        0        0     4900 2022-11-23 10:31:53.406176 perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_currency_dataset.sql
--rwxr-xr-x   0        0        0     1892 2023-02-09 01:21:55.716943 perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_exception_function.sql
--rw-r--r--   0        0        0     1547 2022-11-23 10:31:53.406510 perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_geometry_function.sql
--rwxr-xr-x   0        0        0     1215 2022-11-23 10:31:53.406646 perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_label_type.sql
--rwxr-xr-x   0        0        0     2684 2022-11-23 10:31:53.406769 perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_locale_function.sql
--rwxr-xr-x   0        0        0     1269 2022-11-23 10:31:53.406909 perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_object_constant.sql
--rw-r--r--   0        0        0     6696 2022-11-23 10:31:53.407036 perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_object_table.sql
--rwxr-xr-x   0        0        0     1037 2022-11-23 10:31:53.407142 perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_visibility_constant.sql
--rwxr-xr-x   0        0        0    13514 2023-02-09 01:22:42.266123 perseus_restful_api_framework-1.27.1/src/majormode/perseus/manage.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.407888 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/__init__.py
--rwxr-xr-x   0        0        0      778 2022-11-23 10:31:53.408088 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/__init__.py
--rwxr-xr-x   0        0        0   169815 2023-07-11 02:41:20.297680 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/account_service.py
--rw-r--r--   0        0        0    53061 2023-02-08 13:43:19.667427 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/contact_service.py
--rwxr-xr-x   0        0        0     4095 2023-07-11 00:53:28.787995 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_account_constraint.sql
--rwxr-xr-x   0        0        0     7947 2023-01-30 00:41:55.092554 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_account_function.sql
--rw-r--r--   0        0        0     1287 2022-11-23 10:31:53.411326 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_account_index.sql
--rwxr-xr-x   0        0        0    21758 2023-07-11 00:53:51.665719 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_account_table.sql
--rwxr-xr-x   0        0        0     1093 2022-11-23 10:31:53.412248 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_session_constraint.sql
--rwxr-xr-x   0        0        0     1101 2022-11-23 10:31:53.412521 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_session_function.sql
--rwxr-xr-x   0        0        0      989 2022-11-23 10:31:53.412719 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_session_index.sql
--rwxr-xr-x   0        0        0     1637 2022-11-23 10:31:53.413015 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_session_table.sql
--rwxr-xr-x   0        0        0     2093 2022-11-23 10:31:53.413203 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table.718.sql
--rwxr-xr-x   0        0        0      870 2022-11-23 10:31:53.413470 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.11.9.sql
--rwxr-xr-x   0        0        0     1033 2022-11-23 10:31:53.413751 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.12.0.sql
--rw-r--r--   0        0        0     1115 2022-11-23 10:31:53.414028 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.12.9.sql
--rw-r--r--   0        0        0     2599 2022-11-23 10:31:53.414316 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.17.14.sql
--rw-r--r--   0        0        0     1182 2022-11-23 10:31:53.414599 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.17.31.sql
--rw-r--r--   0        0        0      854 2022-11-23 10:31:53.416384 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.21.0.sql
--rw-r--r--   0        0        0     1877 2022-11-23 10:31:53.416723 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.22.0.sql
--rw-r--r--   0        0        0     1139 2022-11-23 10:31:53.417010 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.24.0.sql
--rw-r--r--   0        0        0     1179 2023-01-30 00:54:22.647572 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.25.12.sql
--rw-r--r--   0        0        0     3165 2023-03-10 00:12:11.857881 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.25.19.sql
--rw-r--r--   0        0        0     6259 2022-11-23 10:31:53.422782 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/oauth_service.py
--rwxr-xr-x   0        0        0    15044 2023-06-12 12:14:13.452381 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/session_service.py
--rw-r--r--   0        0        0      371 2022-11-23 10:31:53.423592 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/template/default_verify_email_eng-US.txt
--rw-r--r--   0        0        0      496 2022-11-23 10:31:53.423820 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/template/default_verify_email_fra-FR.txt
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.424102 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/test/__init__.py
--rwxr-xr-x   0        0        0     7955 2022-11-23 10:31:53.424296 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/test/account_service_unittest.py
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.424502 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/__init__.py
--rwxr-xr-x   0        0        0    36170 2023-02-09 01:22:42.266180 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/application_service.py
--rwxr-xr-x   0        0        0     1581 2022-11-23 10:31:53.426329 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/db/create_application_constraint.sql
--rwxr-xr-x   0        0        0     1226 2022-11-23 10:31:53.426580 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/db/create_application_index.sql
--rwxr-xr-x   0        0        0     5129 2022-11-23 10:31:53.426913 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/db/create_application_table.sql
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.428345 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/test/__init__.py
--rwxr-xr-x   0        0        0     5285 2023-01-30 01:58:24.717658 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/test/application_service_unittest.py
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.429024 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/__init__.py
--rw-r--r--   0        0        0    38030 2023-02-09 01:22:31.541021 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/area_service.py
--rwxr-xr-x   0        0        0     5918 2022-11-23 10:31:53.430300 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/data/vietnam/area2sql.py
--rw-r--r--   0        0        0     5064 2022-11-23 10:31:53.430550 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/data/vietnam/area_extractor.py
--rw-r--r--   0        0        0  5506086 2022-11-23 10:31:53.441911 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/data/vietnam/vietnamese_administrative_area_boundaries.json.zip
--rwxr-xr-x   0        0        0     1534 2022-11-23 10:31:53.442964 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_constraint.sql
--rw-r--r--   0        0        0     3013 2022-11-23 10:31:53.443144 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_dataset.sql
--rw-r--r--   0        0        0    27948 2022-11-23 10:31:53.443409 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_function.sql
--rw-r--r--   0        0        0     1324 2022-11-23 10:31:53.443571 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_index.sql
--rwxr-xr-x   0        0        0     5732 2022-11-23 10:31:53.443741 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_table.sql
--rwxr-xr-x   0        0        0     2447 2022-11-23 10:31:53.443964 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_type.sql
--rwxr-xr-x   0        0        0     1097 2022-11-23 10:31:53.444132 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_geoip_constraint.sql
--rw-r--r--   0        0        0      908 2022-11-23 10:31:53.444276 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_geoip_index.sql
--rw-r--r--   0        0        0     7276 2022-11-23 10:31:53.444639 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_geoip_table.sql
--rwxr-xr-x   0        0        0      923 2022-11-23 10:31:53.444789 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_mobile-phone-operator_index.sql
--rwxr-xr-x   0        0        0     1631 2022-11-23 10:31:53.444977 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_mobile-phone-operator_table.sql
--rw-r--r--   0        0        0     5679 2022-11-23 10:31:53.445111 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_rir_table.sql
--rw-r--r--   0        0        0     1597 2022-11-23 10:31:53.445206 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/migrate_area_dataset.sql
--rw-r--r--   0        0        0     1512 2022-11-23 10:31:53.445958 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/script/_geolite_importer.py
--rw-r--r--   0        0        0     6460 2022-11-23 10:31:53.446070 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/script/_rir_importer.py
--rwxr-xr-x   0        0        0    17479 2022-11-23 10:31:53.446283 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/script/geoip2sql.py
--rw-r--r--   0        0        0    64867 2023-07-10 03:10:00.295237 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/base_http_handler.py
--rw-r--r--   0        0        0     1331 2022-11-23 10:31:53.448135 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/base_job_service.py
--rwxr-xr-x   0        0        0     3067 2023-02-09 01:22:42.266212 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/base_rdbms_service.py
--rwxr-xr-x   0        0        0     4565 2023-02-09 01:21:55.697787 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/base_service.py
--rwxr-xr-x   0        0        0      778 2022-11-23 10:31:53.448685 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/__init__.py
--rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.448883 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/agent/__init__.py
--rwxr-xr-x   0        0        0    13128 2022-11-23 10:31:53.449162 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/agent/push_notification.py
--rw-r--r--   0        0        0      899 2022-11-23 10:31:53.449426 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/db/create_notification_constraint.sql
--rw-r--r--   0        0        0     1167 2022-11-23 10:31:53.449636 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/db/create_notification_index.sql
--rw-r--r--   0        0        0    10511 2022-11-23 10:31:53.449859 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/db/create_notification_table.sql
--rw-r--r--   0        0        0     2254 2022-11-23 10:31:53.450914 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/gcm.py
--rw-r--r--   0        0        0    65115 2023-02-09 01:22:31.540956 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/notification_service.py
--rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.451539 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/__init__.py
--rw-r--r--   0        0        0      802 2022-11-23 10:31:53.451813 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/doc/api/get_ping.rst
--rw-r--r--   0        0        0      927 2023-02-08 01:28:29.061642 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/doc/api/get_status.rst
--rw-r--r--   0        0        0      609 2023-02-08 01:24:00.319004 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/doc/api/index.rst
--rw-r--r--   0        0        0     7536 2022-11-23 10:31:53.452507 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/status_service.py
--rw-r--r--   0        0        0     2427 2022-11-23 10:31:53.452658 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/status_service_http_handler.py
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.453023 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/__init__.py
--rw-r--r--   0        0        0     2469 2022-11-23 10:31:53.453234 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/agent/team_invite.py
--rw-r--r--   0        0        0     2647 2022-11-23 10:31:53.453512 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/create_team_constraint.sql
--rw-r--r--   0        0        0     3769 2022-11-23 10:31:53.453654 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/create_team_function.sql
--rw-r--r--   0        0        0      968 2023-05-19 09:03:02.094015 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/create_team_index.sql
--rw-r--r--   0        0        0     9034 2023-05-19 09:32:28.819485 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/create_team_table.sql
--rw-r--r--   0        0        0      253 2022-11-23 10:31:53.454170 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/migrate_20190501.sql
--rw-r--r--   0        0        0     2513 2022-11-23 10:31:53.454566 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/migrate_team_table@1.13.3.sql
--rwxr-xr-x   0        0        0   124076 2023-05-25 02:34:43.732136 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/team_service.py
--rw-r--r--   0        0        0      623 2022-11-23 10:31:53.458700 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/template/default_invite_email.txt
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.458921 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/test/__init__.py
--rwxr-xr-x   0        0        0     6049 2022-11-23 10:31:53.459109 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/test/team_service_unittest.py
--rw-r--r--   0        0        0      830 2022-11-23 10:31:53.459329 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/__init__.py
--rw-r--r--   0        0        0     2734 2023-02-08 01:36:23.016572 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/doc/api/get_version.rst
--rw-r--r--   0        0        0     1913 2023-02-08 01:37:27.596508 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/doc/api/index.rst
--rwxr-xr-x   0        0        0      836 2022-11-23 10:31:53.461396 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/test/__init__.py
--rwxr-xr-x   0        0        0     4574 2022-11-23 10:31:53.461950 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/test/version_service_unittest.py
--rwxr-xr-x   0        0        0     2448 2023-01-17 06:08:31.898328 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/version_service.py
--rw-r--r--   0        0        0     1720 2023-01-17 03:47:01.966678 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/version_service_http_handler.py
--rw-r--r--   0        0        0     6855 1970-01-01 00:00:00.000000 perseus_restful_api_framework-1.27.1/setup.py
--rw-r--r--   0        0        0     5871 1970-01-01 00:00:00.000000 perseus_restful_api_framework-1.27.1/PKG-INFO
+-rw-r--r--   0        0        0    10273 2023-07-17 09:05:55.274101 perseus_restful_api_framework-1.27.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1089 2020-11-12 14:26:46.553799 perseus_restful_api_framework-1.27.2/LICENSE
+-rw-r--r--   0        0        0     4530 2022-10-02 05:19:36.696561 perseus_restful_api_framework-1.27.2/README.md
+-rw-r--r--   0        0        0     1140 2023-07-17 09:05:55.282215 perseus_restful_api_framework-1.27.2/pyproject.toml
+-rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.404748 perseus_restful_api_framework-1.27.2/src/majormode/__init__.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.404886 perseus_restful_api_framework-1.27.2/src/majormode/perseus/__init__.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.405009 perseus_restful_api_framework-1.27.2/src/majormode/perseus/agent/__init__.py
+-rwxr-xr-x   0        0        0    11953 2023-02-09 01:22:31.663266 perseus_restful_api_framework-1.27.2/src/majormode/perseus/agent/email_address_verification_agent.py
+-rw-r--r--   0        0        0     3603 2023-02-09 01:21:55.716946 perseus_restful_api_framework-1.27.2/src/majormode/perseus/agent/email_sender_agent.py
+-rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.405462 perseus_restful_api_framework-1.27.2/src/majormode/perseus/bootstrap/__init__.py
+-rw-r--r--   0        0        0    17545 2023-02-09 01:22:31.663215 perseus_restful_api_framework-1.27.2/src/majormode/perseus/bootstrap/tornado_handler.py
+-rw-r--r--   0        0        0     4900 2022-11-23 10:31:53.406176 perseus_restful_api_framework-1.27.2/src/majormode/perseus/db/create_currency_dataset.sql
+-rwxr-xr-x   0        0        0     1892 2023-02-09 01:21:55.716943 perseus_restful_api_framework-1.27.2/src/majormode/perseus/db/create_exception_function.sql
+-rw-r--r--   0        0        0     1547 2022-11-23 10:31:53.406510 perseus_restful_api_framework-1.27.2/src/majormode/perseus/db/create_geometry_function.sql
+-rwxr-xr-x   0        0        0     1215 2022-11-23 10:31:53.406646 perseus_restful_api_framework-1.27.2/src/majormode/perseus/db/create_label_type.sql
+-rwxr-xr-x   0        0        0     2684 2022-11-23 10:31:53.406769 perseus_restful_api_framework-1.27.2/src/majormode/perseus/db/create_locale_function.sql
+-rwxr-xr-x   0        0        0     1269 2022-11-23 10:31:53.406909 perseus_restful_api_framework-1.27.2/src/majormode/perseus/db/create_object_constant.sql
+-rw-r--r--   0        0        0     6696 2022-11-23 10:31:53.407036 perseus_restful_api_framework-1.27.2/src/majormode/perseus/db/create_object_table.sql
+-rwxr-xr-x   0        0        0     1037 2022-11-23 10:31:53.407142 perseus_restful_api_framework-1.27.2/src/majormode/perseus/db/create_visibility_constant.sql
+-rwxr-xr-x   0        0        0    13514 2023-02-09 01:22:42.266123 perseus_restful_api_framework-1.27.2/src/majormode/perseus/manage.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.407888 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/__init__.py
+-rwxr-xr-x   0        0        0      778 2022-11-23 10:31:53.408088 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/__init__.py
+-rwxr-xr-x   0        0        0   170013 2023-07-11 08:24:37.386873 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/account_service.py
+-rw-r--r--   0        0        0    53061 2023-02-08 13:43:19.667427 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/contact_service.py
+-rwxr-xr-x   0        0        0     4095 2023-07-11 00:53:28.787995 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/create_account_constraint.sql
+-rwxr-xr-x   0        0        0     7947 2023-01-30 00:41:55.092554 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/create_account_function.sql
+-rw-r--r--   0        0        0     1287 2022-11-23 10:31:53.411326 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/create_account_index.sql
+-rwxr-xr-x   0        0        0    21758 2023-07-11 00:53:51.665719 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/create_account_table.sql
+-rwxr-xr-x   0        0        0     1093 2022-11-23 10:31:53.412248 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/create_session_constraint.sql
+-rwxr-xr-x   0        0        0     1101 2022-11-23 10:31:53.412521 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/create_session_function.sql
+-rwxr-xr-x   0        0        0      989 2022-11-23 10:31:53.412719 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/create_session_index.sql
+-rwxr-xr-x   0        0        0     1637 2022-11-23 10:31:53.413015 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/create_session_table.sql
+-rwxr-xr-x   0        0        0     2093 2022-11-23 10:31:53.413203 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table.718.sql
+-rwxr-xr-x   0        0        0      870 2022-11-23 10:31:53.413470 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.11.9.sql
+-rwxr-xr-x   0        0        0     1033 2022-11-23 10:31:53.413751 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.12.0.sql
+-rw-r--r--   0        0        0     1115 2022-11-23 10:31:53.414028 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.12.9.sql
+-rw-r--r--   0        0        0     2599 2022-11-23 10:31:53.414316 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.17.14.sql
+-rw-r--r--   0        0        0     1182 2022-11-23 10:31:53.414599 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.17.31.sql
+-rw-r--r--   0        0        0      854 2022-11-23 10:31:53.416384 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.21.0.sql
+-rw-r--r--   0        0        0     1877 2022-11-23 10:31:53.416723 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.22.0.sql
+-rw-r--r--   0        0        0     1139 2022-11-23 10:31:53.417010 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.24.0.sql
+-rw-r--r--   0        0        0     1179 2023-01-30 00:54:22.647572 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.25.12.sql
+-rw-r--r--   0        0        0     3165 2023-03-10 00:12:11.857881 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.25.19.sql
+-rw-r--r--   0        0        0     6259 2022-11-23 10:31:53.422782 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/oauth_service.py
+-rwxr-xr-x   0        0        0    15044 2023-06-12 12:14:13.452381 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/session_service.py
+-rw-r--r--   0        0        0      371 2022-11-23 10:31:53.423592 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/template/default_verify_email_eng-US.txt
+-rw-r--r--   0        0        0      496 2022-11-23 10:31:53.423820 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/template/default_verify_email_fra-FR.txt
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.424102 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/test/__init__.py
+-rwxr-xr-x   0        0        0     7955 2022-11-23 10:31:53.424296 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/test/account_service_unittest.py
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.424502 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/application/__init__.py
+-rwxr-xr-x   0        0        0    36170 2023-02-09 01:22:42.266180 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/application/application_service.py
+-rwxr-xr-x   0        0        0     1581 2022-11-23 10:31:53.426329 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/application/db/create_application_constraint.sql
+-rwxr-xr-x   0        0        0     1226 2022-11-23 10:31:53.426580 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/application/db/create_application_index.sql
+-rwxr-xr-x   0        0        0     5129 2022-11-23 10:31:53.426913 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/application/db/create_application_table.sql
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.428345 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/application/test/__init__.py
+-rwxr-xr-x   0        0        0     5285 2023-01-30 01:58:24.717658 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/application/test/application_service_unittest.py
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.429024 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/__init__.py
+-rw-r--r--   0        0        0    38030 2023-02-09 01:22:31.541021 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/area_service.py
+-rwxr-xr-x   0        0        0     5918 2022-11-23 10:31:53.430300 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/data/vietnam/area2sql.py
+-rw-r--r--   0        0        0     5064 2022-11-23 10:31:53.430550 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/data/vietnam/area_extractor.py
+-rw-r--r--   0        0        0  5506086 2022-11-23 10:31:53.441911 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/data/vietnam/vietnamese_administrative_area_boundaries.json.zip
+-rwxr-xr-x   0        0        0     1534 2022-11-23 10:31:53.442964 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_area_constraint.sql
+-rw-r--r--   0        0        0     3013 2022-11-23 10:31:53.443144 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_area_dataset.sql
+-rw-r--r--   0        0        0    27948 2022-11-23 10:31:53.443409 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_area_function.sql
+-rw-r--r--   0        0        0     1324 2022-11-23 10:31:53.443571 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_area_index.sql
+-rwxr-xr-x   0        0        0     5732 2022-11-23 10:31:53.443741 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_area_table.sql
+-rwxr-xr-x   0        0        0     2447 2022-11-23 10:31:53.443964 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_area_type.sql
+-rwxr-xr-x   0        0        0     1097 2022-11-23 10:31:53.444132 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_geoip_constraint.sql
+-rw-r--r--   0        0        0      908 2022-11-23 10:31:53.444276 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_geoip_index.sql
+-rw-r--r--   0        0        0     7276 2022-11-23 10:31:53.444639 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_geoip_table.sql
+-rwxr-xr-x   0        0        0      923 2022-11-23 10:31:53.444789 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_mobile-phone-operator_index.sql
+-rwxr-xr-x   0        0        0     1631 2022-11-23 10:31:53.444977 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_mobile-phone-operator_table.sql
+-rw-r--r--   0        0        0     5679 2022-11-23 10:31:53.445111 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_rir_table.sql
+-rw-r--r--   0        0        0     1597 2022-11-23 10:31:53.445206 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/migrate_area_dataset.sql
+-rw-r--r--   0        0        0     1512 2022-11-23 10:31:53.445958 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/script/_geolite_importer.py
+-rw-r--r--   0        0        0     6460 2022-11-23 10:31:53.446070 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/script/_rir_importer.py
+-rwxr-xr-x   0        0        0    17479 2022-11-23 10:31:53.446283 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/script/geoip2sql.py
+-rw-r--r--   0        0        0    64867 2023-07-10 03:10:00.295237 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/base_http_handler.py
+-rw-r--r--   0        0        0     1331 2022-11-23 10:31:53.448135 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/base_job_service.py
+-rwxr-xr-x   0        0        0     3067 2023-02-09 01:22:42.266212 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/base_rdbms_service.py
+-rwxr-xr-x   0        0        0     4565 2023-02-09 01:21:55.697787 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/base_service.py
+-rwxr-xr-x   0        0        0      778 2022-11-23 10:31:53.448685 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/notification/__init__.py
+-rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.448883 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/notification/agent/__init__.py
+-rwxr-xr-x   0        0        0    13128 2022-11-23 10:31:53.449162 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/notification/agent/push_notification.py
+-rw-r--r--   0        0        0     1303 2023-07-17 03:52:42.352618 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/notification/db/create_notification_constraint.sql
+-rw-r--r--   0        0        0      800 2023-07-17 03:53:34.255240 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/notification/db/create_notification_index.sql
+-rw-r--r--   0        0        0    10620 2023-07-17 08:05:00.943082 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/notification/db/create_notification_table.sql
+-rw-r--r--   0        0        0     2254 2022-11-23 10:31:53.450914 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/notification/gcm.py
+-rw-r--r--   0        0        0    65678 2023-07-17 09:00:05.551715 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/notification/notification_service.py
+-rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.451539 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/status/__init__.py
+-rw-r--r--   0        0        0      802 2022-11-23 10:31:53.451813 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/status/doc/api/get_ping.rst
+-rw-r--r--   0        0        0      927 2023-02-08 01:28:29.061642 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/status/doc/api/get_status.rst
+-rw-r--r--   0        0        0      609 2023-02-08 01:24:00.319004 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/status/doc/api/index.rst
+-rw-r--r--   0        0        0     7536 2022-11-23 10:31:53.452507 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/status/status_service.py
+-rw-r--r--   0        0        0     2427 2022-11-23 10:31:53.452658 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/status/status_service_http_handler.py
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.453023 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/__init__.py
+-rw-r--r--   0        0        0     2469 2022-11-23 10:31:53.453234 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/agent/team_invite.py
+-rw-r--r--   0        0        0     2647 2022-11-23 10:31:53.453512 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/db/create_team_constraint.sql
+-rw-r--r--   0        0        0     3769 2022-11-23 10:31:53.453654 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/db/create_team_function.sql
+-rw-r--r--   0        0        0      968 2023-05-19 09:03:02.094015 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/db/create_team_index.sql
+-rw-r--r--   0        0        0     9034 2023-05-19 09:32:28.819485 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/db/create_team_table.sql
+-rw-r--r--   0        0        0      253 2022-11-23 10:31:53.454170 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/db/migrate_20190501.sql
+-rw-r--r--   0        0        0     2513 2022-11-23 10:31:53.454566 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/db/migrate_team_table@1.13.3.sql
+-rwxr-xr-x   0        0        0   124076 2023-05-25 02:34:43.732136 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/team_service.py
+-rw-r--r--   0        0        0      623 2022-11-23 10:31:53.458700 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/template/default_invite_email.txt
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.458921 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/test/__init__.py
+-rwxr-xr-x   0        0        0     6049 2022-11-23 10:31:53.459109 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/test/team_service_unittest.py
+-rw-r--r--   0        0        0      830 2022-11-23 10:31:53.459329 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/version/__init__.py
+-rw-r--r--   0        0        0     2734 2023-02-08 01:36:23.016572 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/version/doc/api/get_version.rst
+-rw-r--r--   0        0        0     1913 2023-02-08 01:37:27.596508 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/version/doc/api/index.rst
+-rwxr-xr-x   0        0        0      836 2022-11-23 10:31:53.461396 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/version/test/__init__.py
+-rwxr-xr-x   0        0        0     4574 2022-11-23 10:31:53.461950 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/version/test/version_service_unittest.py
+-rwxr-xr-x   0        0        0     2448 2023-01-17 06:08:31.898328 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/version/version_service.py
+-rw-r--r--   0        0        0     1720 2023-01-17 03:47:01.966678 perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/version/version_service_http_handler.py
+-rw-r--r--   0        0        0     6855 1970-01-01 00:00:00.000000 perseus_restful_api_framework-1.27.2/setup.py
+-rw-r--r--   0        0        0     5871 1970-01-01 00:00:00.000000 perseus_restful_api_framework-1.27.2/PKG-INFO
```

### Comparing `perseus_restful_api_framework-1.27.1/CHANGELOG.md` & `perseus_restful_api_framework-1.27.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), 
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.27.2] - 2023-07-11
+# Changed
+- Cleanse the Notification Service
+
 ## [1.27.1] - 2023-07-11
 # Added
 - Add user account's preferences management
 
 ## [1.27.0] - 2023-07-10
 # Changed
 - HTTP request handlers return a dictionary object itself instead of embedding it in a `{ "data": dict }`
```

### Comparing `perseus_restful_api_framework-1.27.1/LICENSE` & `perseus_restful_api_framework-1.27.2/LICENSE`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/README.md` & `perseus_restful_api_framework-1.27.2/README.md`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/pyproject.toml` & `perseus_restful_api_framework-1.27.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 keywords = ["perseus", "resful", "api", "server", "framework"]
 license = "Proprietary"
 name = "perseus-restful-api-framework"
 packages = [{ include = "majormode", from = "src" }]
 readme = "README.md"
 repository = "https://github.com/majormode/perseus-restful-api-server-framework"
-version = "1.27.1"
+version = "1.27.2"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 psutil = "^5.9.4"
 tornado = "^6.2"
 perseus-core-library = "^1.18.24"
 pillow = "^9.4.0"
```

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/__init__.py` & `perseus_restful_api_framework-1.27.2/src/majormode/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/__init__.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/agent/__init__.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/agent/email_address_verification_agent.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/agent/email_address_verification_agent.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/agent/email_sender_agent.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/agent/email_sender_agent.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/bootstrap/__init__.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/bootstrap/tornado_handler.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/bootstrap/tornado_handler.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_currency_dataset.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/db/create_currency_dataset.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_exception_function.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/db/create_exception_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_geometry_function.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/db/create_geometry_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_label_type.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/db/create_label_type.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_locale_function.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/db/create_locale_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_object_constant.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/db/create_object_constant.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_object_table.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/db/create_object_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_visibility_constant.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/db/create_visibility_constant.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/manage.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/manage.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/__init__.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/__init__.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/account_service.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/account_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -2480,34 +2480,39 @@
 
 
         :param app_id: Identification of the client application such as a Web,
             a desktop, or a mobile application, that accesses the service.
 
         :param username: A username to check whether it is already registered
             by an existing user or not.  A username is unique across the
-            platform.  A username is not case sensitive.
+            platform.  A username is not case-sensitive.
 
         :return: `True` if the username is not registered by any existing
             account; `False` otherwise.
         """
         with self.acquire_rdbms_connection() as connection:
             cursor = connection.execute(
                 """
                 SELECT 
                     true
                   FROM 
                     account
                   WHERE
                     lower(username) = lower(%(username)s)
-                    AND object_status = %(OBJECT_STATUS_ENABLED)s
+                    AND object_status IN (
+                        %(OBJECT_STATUS_DISABLED)s,
+                        %(OBJECT_STATUS_ENABLED)s
+                    )
                 """,
                 {
+                    'OBJECT_STATUS_DISABLED': ObjectStatus.disabled,
                     'OBJECT_STATUS_ENABLED': ObjectStatus.enabled,
-                    'username': username
-                })
+                    'username': username,
+                }
+            )
 
             return cursor.get_row_count() == 0
 
     def request_password_reset(
             self,
             app_id,
             contact,
@@ -3366,15 +3371,15 @@
                 """
                 UPDATE
                     account
                   SET
                     username = NULL,
                     update_time = current_timestamp
                   WHERE
-                    username = %(username)s
+                    lower(username) = lower(%(username)s)
                 """,
                 {
                     'username': username,
                 }
             )
 
             # Set the username to the specified user account.
```

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/contact_service.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/contact_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_account_constraint.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/create_account_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_account_function.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/create_account_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_account_index.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/create_account_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_account_table.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/create_account_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_session_constraint.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/create_session_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_session_function.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/create_session_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_session_index.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/create_session_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_session_table.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/create_session_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table.718.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table.718.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.11.9.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.11.9.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.12.0.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.12.0.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.12.9.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.12.9.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.17.14.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.17.14.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.17.31.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.17.31.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.21.0.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.21.0.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.22.0.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.22.0.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.24.0.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.24.0.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.25.12.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.25.12.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.25.19.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/db/migrate_account_table@1.25.19.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/oauth_service.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/oauth_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/session_service.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/session_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/test/__init__.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/test/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/test/account_service_unittest.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/account/test/account_service_unittest.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/__init__.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/application/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/application_service.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/application/application_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/db/create_application_constraint.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/application/db/create_application_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/db/create_application_index.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/application/db/create_application_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/db/create_application_table.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/application/db/create_application_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/test/__init__.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/application/test/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/test/application_service_unittest.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/application/test/application_service_unittest.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/__init__.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/area_service.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/area_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/data/vietnam/area2sql.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/data/vietnam/area2sql.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/data/vietnam/area_extractor.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/data/vietnam/area_extractor.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/data/vietnam/vietnamese_administrative_area_boundaries.json.zip` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/data/vietnam/vietnamese_administrative_area_boundaries.json.zip`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_constraint.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_area_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_dataset.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_area_dataset.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_function.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_area_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_index.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_area_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_table.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_area_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_type.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_area_type.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_geoip_constraint.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_geoip_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_geoip_index.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_geoip_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_geoip_table.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_geoip_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_mobile-phone-operator_index.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_mobile-phone-operator_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_mobile-phone-operator_table.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_mobile-phone-operator_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_rir_table.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/create_rir_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/migrate_area_dataset.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/db/migrate_area_dataset.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/script/_geolite_importer.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/script/_geolite_importer.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/script/_rir_importer.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/script/_rir_importer.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/script/geoip2sql.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/area/script/geoip2sql.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/base_http_handler.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/base_http_handler.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/base_job_service.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/base_job_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/base_rdbms_service.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/base_rdbms_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/base_service.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/base_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/__init__.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/agent/__init__.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/notification/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/agent/push_notification.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/notification/agent/push_notification.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/db/create_notification_constraint.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/notification/db/create_notification_constraint.sql`

 * *Files 22% similar despite different names*

```diff
@@ -14,7 +14,21 @@
  * LOSSES OR DAMAGES SUFFERED BY LICENSEE AS A RESULT OF USING, MODIFYING
  * OR DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES.
  */
 
 ALTER TABLE notification
   ADD CONSTRAINT pk_notification_id
       PRIMARY KEY (notification_id);
+
+/**
+ * Ensure that a device can only register once to the push notification
+ * service for a given device platform (Android, iOS, Windows mobile),
+ * for a specific mobile application, and on behalf of a given user.
+ */
+ALTER TABLE notification_device
+  ADD CONSTRAINT cst_notification_device_unique
+      UNIQUE (
+        device_id,
+        device_platform,
+        app_id,
+        account_id
+      );
```

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/db/create_notification_index.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/db/create_team_index.sql`

 * *Files 23% similar despite different names*

```diff
@@ -9,21 +9,18 @@
  *
  * MAJORMODE MAKES NO REPRESENTATIONS OR WARRANTIES ABOUT THE SUITABILITY
  * OF THE SOFTWARE, EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
  * TO THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR
  * PURPOSE, OR NON-INFRINGEMENT.  MAJORMODE SHALL NOT BE LIABLE FOR ANY
  * LOSSES OR DAMAGES SUFFERED BY LICENSEE AS A RESULT OF USING, MODIFYING
  * OR DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES.
- */
+*/
 
-/**
- * Ensure that a device can only register once to the push notification
- * service for a given device platform (Android, iOS, Windows mobile),
- * for a specific mobile application, and on behalf of a given user.
- */
-CREATE UNIQUE INDEX cst_notification_device_unique
-  ON notification_device (
-    device_id,
-    device_platform,
-    app_id,
-    account_id
+CREATE UNIQUE INDEX idx_team_name
+  ON team (lower(name));
+
+
+CREATE UNIQUE INDEX idx_team_contact
+  ON team_contact (
+    lower(property_value),
+    property_name
   );
```

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/gcm.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/notification/gcm.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/notification_service.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/notification/notification_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,29 +19,30 @@
 # TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 import datetime
 import json
 import socket
 import urllib.request
+from uuid import UUID
 
 from majormode.perseus.constant.http import HttpMethod
 from majormode.perseus.constant.notification import DevicePlatform
+from majormode.perseus.constant.notification import NotificationMode
 from majormode.perseus.constant.obj import ObjectStatus
 from majormode.perseus.constant.sort_order import SortOrder
 from majormode.perseus.model import obj
 from majormode.perseus.model.locale import Locale
 from majormode.perseus.utils import cast
 from majormode.perseus.utils.date_util import ISO8601DateTime
+from majormode.perseus.utils.rdbms import RdbmsConnection
 
 from majormode.perseus.service.application.application_service import ApplicationService
 from majormode.perseus.service.base_rdbms_service import BaseRdbmsService
 from majormode.perseus.service.notification.gcm import GoogleCloudMessagingRequest
-from majormode.perseus.service.team.team_service import TeamService
-import settings
 
 
 class NotificationService(BaseRdbmsService):
     """
     A notification is a lightweight message that needs to be delivered to
     one or more recipients.  It informs the recipients about an event
     that occurs, which might require fetching additional data from the
@@ -49,24 +50,24 @@
 
     A recipient is generally a client application that acts on behalf of a
     user, but it could also be an agent or botnet that controls a device.
 
     A message can be delivered to a recipient using different styles of
     network communication:
 
-    * `email`: the message is delivered in an Internet electronic mail
+    - ``email``: the message is delivered in an Internet electronic mail
       message to the specified recipients based on a store-and-forward
       model.
 
-    * `push`: the message is delivered to the specified recipients
+    - ``push``: the message is delivered to the specified recipients
       when the request for the transmission of information is initiated
       by the publisher or server platform and pushed out to the receiver
       or client application.
 
-    * `pull`: the message is delivered to the specified recipients
+    - ``pull``: the message is delivered to the specified recipients
       when the request for the transmission of information is initiated
       by the receiver or client application, and then is responded by the
       publisher or server platform.  Push style requires recipients to
       register with the server platform before it can receive messages
       using this mode.
     """
 
@@ -89,354 +90,410 @@
     # apps like instant messaging can consume the message directly).  The
     # GCM service handles all aspects of queueing of messages and delivery
     # to the target Android application running on the target device.
     GCM_SERVER_HTTP_URL = 'https://gcm-http.googleapis.com/gcm/send'
 
     def __add_device_registration(
             self,
-            device_id,
+            device_id: str,
             device_platform,
-            app_id,
-            device_token,
-            account_id=None,
-            connection=None,
-            locale=None,
-            utc_offset=None):
+            app_id: UUID,
+            device_token: str,
+            account_id: UUID = None,
+            connection: RdbmsConnection = None,
+            language: Locale = None,
+            utc_offset: int = None) -> any:
         """
         Register a mobile device to the push notification service
 
 
-        @param device_id: Identification of a mobile device that registers
+        :param device_id: The identifier of a mobile device that registers
             to push notification service.
 
-        @param device_platform: An item of the enumeration `DevicePlatform`.
+        :param device_platform: The mobile platform of the device.
 
-        @param app_id: Identification of the mobile application that
-            registers the mobile device to push notification service.
+        :param app_id: The identifier of the client application that registers
+            the mobile device to the push notification service.
 
-        @param device_token: Token that identifies the device by the push
+        :param device_token: A token that identifies the device by the push
             notification provider of the device platform.
 
-        @param account_id: Identification of the account of a user who
-            registers his mobile device to push notification service.
+        :param account_id: The identifier of the account of a user who
+            registers his mobile device to the push notification service.
 
-        @param connection: An object `RdbmsConnection`.
+        :param connection: A connection to the notification database.
 
-        @param locale: Preferred language to new messages' textual content in.
-            This argument is ignored if the mobile device is registered to
-            push notification on behalf of a user. Messages will be send in
-            the current preferred language of the user.
+        :param language: The preferred language to write message in to this
+            mobile device.
 
-        @param utc_offset: Difference between the location of the device and
+            This argument cannot be passed with the argument ``account_id`` as
+            messages will be written in the preferred language of the user).
+
+        :param utc_offset: Difference between the location of the device and
             UTC (Universal Time Coordinated).
 
 
-        @return: An object containing the following attributes:
+        :return: An object containing the following attributes:
 
-            * `device_id` (required): Identification of the mobile device that
-              registers to push notification service.
+            - ``device_id: str`` (required): The identifier of the mobile device
+              that registers to push notification service.
 
-            * `object_status` (required): Current status of the registration of
-              this device to push notification service.
+            - ``object_status: ObjectStatus`` (required): THe current status of the
+              registration of this device to push notification service.
 
-            * `registration_id` (required): Identification of the registration of
-              the mobile device to the push notification service.
+            - ``registration_id: UUID`` (required): The identifier of the
+              registration of the mobile device to the push notification service.
 
-            * `update_time` (required): Time of the most recent modification of
-              information of the mobile device's registration to the push
-              notification service.
+            - ``update_time: ISO8601DateTime`` (required): The time of the most
+              recent modification of the properties of the mobile device's
+              registration to the push notification service.
         """
         with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
-            cursor = connection.execute("""
+            cursor = connection.execute('''
                 INSERT INTO notification_device (
                     device_token,
                     device_id,
                     device_platform,
                     account_id,
                     utc_offset,
-                    locale,
+                    language,
                     app_id)
                   VALUES (
                     %(device_token)s,
                     %(device_id)s,
                     %(device_platform)s,
                     %(account_id)s,
                     %(utc_offset)s,
-                    %(locale)s,
+                    %(language)s,
                     %(app_id)s
                   )
                   RETURNING
                     device_id,
                     object_status,
                     registration_id,
                     update_time
-                """,
+                ''',
                 {
                     'account_id': account_id,
                     'app_id': app_id,
                     'device_id': device_id,
                     'device_platform': device_platform,
                     'device_token': device_token,
-                    'locale': None if account_id else locale,
-                    'utc_offset': utc_offset
+                    'language': None if account_id else language,
+                    'utc_offset': utc_offset,
                 }
             )
 
             row = cursor.fetch_one()
             device_registration = row.get_object({
                 'object_status': ObjectStatus,
                 'registration_id': cast.string_to_uuid,
                 'update_time': cast.string_to_timestamp,
             })
 
             return device_registration
 
+    def __filter_already_notified_recipients(
+            self,
+            notification_type: str,
+            recipient_ids: list[str],
+            connection: RdbmsConnection = None,
+            sender_id: str = None) -> list[str]:
+        """
+        Return the list of recipients who already received a similar
+        notification.
+
+
+        :param notification_type: The type of the notification to be sent, such
+            as for instance `on_something_happened`.
+
+        :param recipient_ids: The identifier of a recipient, or a list of
+            identifiers of recipients, to send the notification to.
+
+        :param connection: A connection to the notification database.
+
+        :param sender_id: The identifier of the sender on behalf whom the
+            notification is sent to the recipients.
+
+
+        :return: The list of recipients who have already received a similar
+            notification.
+        """
+        with self.acquire_rdbms_connection(auto_commit=False, connection=connection) as connection:
+            cursor = connection.execute(
+                '''
+                SELECT DISTINCT 
+                    recipient_id
+                  FROM 
+                    notification
+                  WHERE
+                    notification_type = %(notification_type)s
+                    AND recipient_id IN (%[recipient_ids]s)
+                    AND (%(sender_id)s IS NULL OR sender_id = %(sender_id)s)
+                    AND NOT is_read
+                ''',
+                {
+                    'notification_type': notification_type,
+                    'recipient_ids': recipient_ids,
+                    'sender_id': sender_id,
+                }
+            )
+
+            recipient_ids = [
+                row.get_value('recipient_id')
+                for row in cursor.fetch_all()
+            ]
+
+            return recipient_ids
+
     def __get_device_registration(
             self,
-            device_id,
-            app_id,
-            account_id=None,
-            connection=None):
+            device_id: str,
+            app_id: UUID,
+            account_id: UUID = None,
+            connection: RdbmsConnection = None):
         """
-        Return the registration of a mobile device to push notification
+        Return the registration of a mobile device to the push notification
         service
 
 
-        @param device_id: Identification of a mobile device that registered
+        :param device_id: Identification of a mobile device that registered
             to push notification service.
 
-        @param app_id: Identification of the mobile application that
+        :param app_id: Identification of the mobile application that
             registered the mobile device to push notification service.
 
-        @param account_id: Identification of the account of a user who
+        :param account_id: Identification of the account of a user who
             registered his mobile device to push notification service.
 
-        @param connection: An object `RdbmsConnection`.
-
-
-        @return: An object containing the following attributes:
+        :param connection: A connection to the notification database.
 
-            * `account_id` (optional): Identification of the account of the user
-              who registered his mobile device to push notification service.
 
-            * `app_id` (required): Identification of the mobile application that
-              registered the mobile device to push notification service.
+        :return: An object containing the following attributes:
 
-            * `device_id` (required): Identification of the mobile device that
-              registered to push notification service.
+            - ``account_id: UUID` (optional): The account identifier of the user who
+              registered his mobile device to push notification service.
 
-            * `device_platform` (required): An item of the enumeration
-              `DevicePlatform` describing the platform of the mobile device.
+            - ``app_id: UUID`` (required): The identifier of the client application
+              that registered the mobile device to the push notification service.
 
-            * `device_token` (required): Token that identifies the mobile device
-              by the push notification provider of the device platform.
+            - ``device_id: str`` (required): The identifier of the mobile device.
 
-            * `locale` (optional): Preferred language to receive new message's
-              textual content in.  This argument is not used if the device
-              registered to push notification service on behalf of a user, but the
-              preferred language of this user.
-
-            * `object_status` (required): Current status of the registration of
-              this device to push notification service
+            - ``device_platform: DevicePlatform`` (required): The mobile platform
+              of the device.
 
-            * `registration_id` (required): Identification of the registration of
-              the mobile device to the push notification service.
+            - ``device_token: str`` (required): The token that identifies the
+              mobile device by the push notification provider of the device
+              platform.
 
-            * `update_time` (required): Time of the most recent modification of
-              information of the mobile device's registration to the push
-              notification service.
+            - ``language: Locale`` (optional): The preferred language to receive
+              message's textual content in.  This argument is not defined if the
+              device registered to push notification service on behalf of a user.
+              The preferred language of this user would be actually used>
+
+            - ``object_status: ObjectStatus`` (required): The current status of the
+              registration of this device to the push notification service.
+
+            - ``registration_id: UUID`` (required): The identifier of the
+              registration of the mobile device to the push notification service.
+
+            - ``update_time: ISO8601DateTime`` (required): The time of the most
+              recent modification of the properties of the mobile device's
+              registration to the push notification service.
 
-            * `utc_offset` (optional): Difference between the location of the
-               mobile device and UTC (Universal Time Coordinated).
+            - ``utc_offset: int`` (optional): The difference between the location of
+              the mobile device and UTC (Universal Time Coordinated).
         """
         with self.acquire_rdbms_connection(auto_commit=False, connection=connection) as connection:
             cursor = connection.execute(
-                """
+                '''
                 SELECT
                     account_id,
                     app_id,
                     device_id,
                     device_platform,
                     device_token,
-                    locale,
+                    language,
                     object_status,
                     registration_id,
                     update_time,
                     utc_offset
                   FROM 
                     notification_device
                   WHERE
                     device_id = %(device_id)s
                     AND ((account_id IS NULL AND %(account_id)s IS NULL)
                          OR account_id = %(account_id)s)
                     AND app_id = %(app_id)s
-                """,
+                ''',
                 {
                     'account_id': account_id,
                     'app_id': app_id,
-                    'device_id': device_id
-                })
+                    'device_id': device_id,
+                }
+            )
 
             row = cursor.fetch_one()
 
             device_registration = row and row.get_object({
                 'account_id': cast.string_to_uuid,
                 'app_id': cast.string_to_uuid,
                 'device_platform': DevicePlatform,
-                'locale': cast.string_to_locale,
+                'language': cast.string_to_locale,
                 'object_status': ObjectStatus,
                 'registration_id': cast.string_to_uuid,
                 'update_time': cast.string_to_timestamp,
             })
 
             return device_registration
 
     def __update_device_registration_token(
             self,
-            registration_id,
-            device_token,
-            connection=None):
+            registration_id: UUID,
+            device_token: str,
+            connection: RdbmsConnection = None):
         """
-        Update the token of a device registered to push notification service
+        Update the token of a device registered to the push notification
+        service.
 
 
-        @param registration_id: Identification of the registration of a device
-            to push notification service
+        :param registration_id: The identifier of the registration of a device
+            to the push notification service.
 
-        @param device_token: Token that identifies the device by the push
+        :param device_token: A token that identifies the device by the push
             notification provider of the device platform.
 
-        @param connection: An object `RdbmsConnection` with auto commit.
+        :param connection: A connection to the notification database.
 
 
-        @return: An object containing the following attributes:
+        :return: An object containing the following attributes:
 
-            * `device_id` (required): Identification of the mobile device that
-              registers to push notification service.
+            - ``device_id: str`` (required): The identifier of the mobile device
+              that registers to push notification service.
 
-            * `object_status` (required): Current status of the registration of
-              this device to push notification service.
+            - ``object_status: ObjectStatus`` (required): The current status of the
+              registration of this device to push notification service.
 
-            * `registration_id` (required): Identification of the registration of
-              the mobile device to the push notification service.
+            - ``registration_id: UUID`` (required): The identifier of the
+              registration of the mobile device to the push notification service.
 
-            * `update_time` (required): Time of the most recent modification of
-              information of the mobile device's registration to the push
-              notification service.
+            - ``update_time: ISO8601DateTime`` (required): The time of the most
+              recent modification of information of the mobile device's registration
+              to the push notification service.
         """
         with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
             cursor = connection.execute(
-                """
+                '''
                 UPDATE 
                     notification_device
                   SET
                     device_token = %(device_token)s,
                     update_time = current_timestamp
                   WHERE
                     registration_id = %(registration_id)s
                   RETURNING
                     device_id,
                     object_status,
                     registration_id,
                     update_time
-                """,
+                ''',
                 {
                     'registration_id': registration_id,
-                    'device_token': device_token
-                })
+                    'device_token': device_token,
+                }
+            )
 
             row = cursor.fetch_one()
             device_registration = row.get_object({
                 'object_status': ObjectStatus,
                 'registration_id': cast.string_to_uuid,
                 'update_time': cast.string_to_timestamp,
             })
 
             return device_registration
 
-    def _push_android_notification(
+    def __push_android_notification(
             self,
-            google_api_key,
-            device_tokens,
-            notification,
-            delay_while_idle=None,
-            gcm_server_http_url=GCM_SERVER_HTTP_URL,
-            time_to_live=None):
+            google_api_key: str,
+            device_tokens: list[str],
+            notification: dict[str, str],
+            delay_while_idle: int = None,
+            gcm_server_http_url: str = GCM_SERVER_HTTP_URL,
+            time_to_live: int = None) -> any:
         """
         Push a notification to an Android device using Google Firebase Cloud
-        Messaging (FCM) HTTP connection server, and return the result returned
-        by the FCM connection server.
+        Messaging (FCM) HTTP connection server.
 
 
-        @note: If your organization has a firewall that restricts the traffic
+        :note: If your organization has a firewall that restricts the traffic
             to or from the Internet, you need to configure it to allow
             connectivity with GCM in order for your GCM client apps to receive
-            messages. The ports to open are: 5228, 5229, and 5230. GCM
-            typically only uses 5228, but it sometimes uses 5229 and 5230. GCM
-            doesn't provide specific IPs, so you should allow your firewall to
-            accept outgoing connections to all IP addresses contained in the
-            IP blocks listed in Google's ASN of 15169.
+            messages.  The ports to open are: 5228, 5229, and 5230. GCM
+            typically only uses 5228, but it sometimes uses 5229 and 5230.
+            GCM doesn't provide specific IPs, so you should allow your
+            firewall to accept outgoing connections to all IP addresses
+            contained in the IP blocks listed in Google's ASN of 15169.
 
 
-        @param google_api_key: API key saved that gives the application server
+        :param google_api_key: The API key that gives the application server
             authorized access to Google services.
 
-        @param device_tokens: a list of devices (registration tokens, or IDs as
+        :param device_tokens: A list of devices (registration tokens, or IDs as
             issued by the GCM connection servers to the client application)
-             receiving a multicast message. It must contain at least 1 and at
-             most 1000 registration IDs.
+            receiving a multicast message.  It must contain at least 1 and at
+            most 1000 registration IDs.
 
-        @param notification: dictionary of key-value pairs of the notification.
-            The key should not be a reserved word ("from" or any word starting
-            with "google" or "gcm"). Values in string types are recommended.
-            You have to convert values in objects or other non-string data
-            types (e.g., integers or booleans) to string.
+        :param notification: A dictionary of key-value pairs of the
+            notifications.  The key should not be a reserved word ("from" or
+            any word starting with "google" or "gcm").  Values in string types
+            are recommended.  You have to convert values in objects or other
+            non-string data types (e.g., integers or booleans) to string.
 
-        @param delay_while_idle: indicate whether the notification should not
+        :param delay_while_idle: Indicate whether the notification should not
             be sent until the device becomes active.
 
-        @param gcm_server_http_url: a specific URL to send the message to GCM
+        :param gcm_server_http_url: A specific URL to send the message to GCM
             connection server.
 
-        @param time_to_live: specify how long in seconds the message should be
+        :param time_to_live: Specify how long in seconds the message should be
             kept in GCM storage if the device is offline.  The maximum time to
             live supported is 4 weeks.  The default value is 4 weeks.
 
 
-        @return: `None` if the JSON request failed, otherwise a JSON object
+        :return: ``None`` if the JSON request failed, otherwise a JSON object
             that contains the Downstream HTTP message response body:
 
-            * `multicast_id:integer` (required): unique ID (number) identifying
+            - ``multicast_id: int`` (required): A unique ID (number) identifying
               the multicast message.
 
-            * `success:integer` (required): number of messages that were
+            - ``success: int`` (required): The number of messages that were
               processed without an error.
 
-            * `failure:integer` (required): number of messages that could not be
+            - ``failure: int`` (required): The number of messages that could not be
               processed.
 
-            * `canonical_ids:integer` (required): number of results that contain
+            - ``canonical_ids: int`` (required): The number of results that contain
               a canonical registration token.
 
-            * `results:list` (optional): array of objects representing the status
-              of the messages processed. The objects are listed in the same order
+            - ``results: list`` (optional): array of objects representing the status
+              of the messages processed.  The objects are listed in the same order
               as the request (i.e., for each registration ID in the request, its
               result is listed in the same index in the response):
 
-              * `message_id:string`: specify a unique ID for each successfully
-                processed message.
+            - ``message_id: str`` (required): specify a unique ID for each
+              successfully processed message.
 
-              * `registration_id:string` (optional): specify the canonical
-                registration token for the client app that the message was processed
-                and sent to. Sender should use this value as the registration token
-                for future requests. Otherwise, the messages might be rejected.
-
-              * `error:string`: specify the error that occurred when processing
-                the message for the recipient. The possible values can be found in
-                `table 11 <https://developers.google.com/cloud-messaging/server-ref#table11>`_.
+            - ``registration_id: str`` (optional): specify the canonical
+            registration token for the client app that the message was processed
+            and sent to. Sender should use this value as the registration token
+            for future requests. Otherwise, the messages might be rejected.
+
+            - ``error: str``: specify the error that occurred when processing
+            the message for the recipient. The possible values can be found in
+            `table 11 <https://developers.google.com/cloud-messaging/server-ref#table11>`_.
         """
         is_multicast_message = isinstance(device_tokens, (list, set, tuple))
 
         post_parameters = dict()
         post_parameters['registration_ids' if is_multicast_message else 'to'] = device_tokens
 
         if delay_while_idle:
@@ -473,180 +530,182 @@
         except socket.timeout:
             raise self.SocketTimeoutException()
 
         response = data or json.loads(data)
 
         return response
 
-    def get_notification(self, notification_id):
+    def get_notification(self, notification_id: UUID) -> any:
         """
         Return the properties of the specified notification.
 
 
-        @param notification_id: identification of the notification to return
-            the properties.
+        :param notification_id: The identifier of a notification.
 
 
-        @return: An object containing the following members:
+        :return: An object containing the following members:
 
-            * `creation_time` (required): time when the sender originated
-              the notification to the intended recipient.
+            - ``creation_time: ISO8601DateTime`` (required): The time when the
+              sender originated the notification to the intended recipient.
 
-            * `is_read` (required): indicate whether the notification
-               has been read by the intended recipient.
+            - ``is_read: bool`` (required): Indicate whether the notification has
+              been read by the intended recipient.
 
-            * `notification_id` (required): identification of the
+            - ``notification_id: UUID`` (required): The identifier of the
               notification.
 
-            * `notification_type` (required): string representation of the
-              type of the notification, as selected by the sender that
-              originated this notification to the intended recipient.
+            - ``notification_type: str`` (required): A string representation of the
+              type of the notification, as selected by the sender that originated
+              this notification to the intended recipient.
 
-            * `payload` (optional): an arbitrary JSON expression added by
+            - ``payload: json`` (optional): an arbitrary JSON expression added by
               the sender to provide information about the context of this
               notification.
 
-            * `schedule_time` (required): time when this notification is
-              scheduled to be sent to the intended recipient.
-              The notification is not visible to the intended recipient prior
-              to this time.
+            - ``schedule_time: ISO8601DateTime`` (required): THe time when this
+              notification is scheduled to be sent to the intended recipient.  The
+              notification is not visible to the intended recipient prior to this
+              time.
 
-            * `sender_id` (optional): the identification of the sender that
+            - ``sender_id: str`` (optional): The identifier of the sender that
               originated the notification.
 
-            * `update_time` (required): time of the most recent modification
-              of an attribute of the notification, such as its read status.
+            - ``update_time: ISO8601DateTime`` (required): The time of the most
+              recent modification of an attribute of the notification, such as its
+              read status.
         """
         with self.acquire_rdbms_connection() as connection:
             cursor = connection.execute(
-                """
+                '''
                 SELECT 
+                    creation_time,
+                    is_read,
                     notification_id,
                     notification_type,
-                    is_read,
-                    sender_id,
                     payload,
                     schedule_time,
-                    creation_time,
+                    sender_id,
                     update_time
                   FROM
                     notification
                   WHERE
                     notification_id = %(notification_id)s
-                """,
+                ''',
                 {
-                    'notification_id': notification_id
-                })
+                    'notification_id': notification_id,
+                }
+            )
 
             row = cursor.fetch_one()
             if row is None:
                 raise self.UndefinedObjectException(f'undefined notification "{notification_id}"')
 
             notification = row.get_object({
                 'creation_time': cast.string_to_timestamp,
                 'notification_id': cast.string_to_uuid,
                 'payload': cast.string_to_json,
                 'schedule_time': cast.string_to_timestamp,
-                'update_time': cast.string_to_timestamp
+                'update_time': cast.string_to_timestamp,
             })
 
             return notification
 
     def get_notifications(
             self,
-            app_id,
-            recipient_id,
-            connection=None,
-            end_time=None,
-            include_read=False,
-            limit=BaseRdbmsService.DEFAULT_LIMIT,
-            mark_read=True,
-            offset=0,
-            notification_types=None,
-            sort_order=SortOrder.ascending,
-            start_time=None):
+            app_id: UUID,
+            recipient_id: str,
+            connection: RdbmsConnection = None,
+            end_time: ISO8601DateTime = None,
+            include_read: bool = False,
+            limit: int = None,
+            mark_read: bool = True,
+            offset: int = None,
+            notification_types: list[str] = None,
+            sort_order: SortOrder = None,
+            start_time: ISO8601DateTime = None) -> list[any]:
         """
         Return a list of notifications that have been sent to the specified
         recipient.
 
 
-        @param app_id: Identification of the client application such as a Web,
-            a desktop, or a mobile application, that accesses the service.
+        :param app_id: The identifier of the client application that accesses
+            the service.
 
-        @param recipient_id: Identification of a recipient that may have been
+        :param recipient_id: The identifier of a recipient that may have been
             issued notifications, such as, for instance the identification of
-            a user account, or the identification of a device, such as an
-            International Mobile Equipment Identity (IMEI) for Android device,
-            or an alphanumeric string for iOS device.
+            a user account, or the identification of a device.
 
-        @param connection: An object `RdbmsConnection`.  Auto commit MUST be
-            enabled if the argument `mark_read` is equal to `True`.
+        :param connection: A connection to the notification database.
 
-        @param end_time: Indicate the latest time of submission to return
-            notifications.
+        :param end_time: The latest time of submission to return notifications.
 
-        @param include_read: Indicate whether to include notifications that
+        :param include_read: Indicate whether to include notifications that
             have been already read.
 
-        @param limit: Constrain the number of notifications that are returned
+        :param limit: Constrain the number of notifications that are returned
             to the specified number.  Default value is
-            `NotificationService.DEFAULT_LIMIT`.  Maximum value is
-            is `NotificationService.MAXIMUM_LIMIT`.
+            ``NotificationService.DEFAULT_LIMIT``.  Maximum value is
+            ``NotificationService.MAXIMUM_LIMIT``.
 
-        @param mark_read: Indicate whether to mark as read every notification
+        :param mark_read: Indicate whether to mark as read every notification
             that are returned.
 
-        @param notification_types: A list of notification types the recipient
+        :param notification_types: A list of notification types the recipient
             is interested in, or whatever notification if not defined.
 
-        @param offset: Require to skip that many records before beginning to
-            return notifications.  Default value is `0`.  If both `offset`
-            and `limit` are specified, then `offset` records are skipped
+        :param offset: Require to skip that many records before beginning to
+            return notifications.  Default value is ``0``.  If both ``offset``
+            and ``limit`` are specified, then ``offset`` records are skipped
             before starting to count the limit notifications that are
             returned.
 
-        @param sort_order: Ascending order sorts notifications by ascending
-            schedule time, while descending order sorts notifications by
-            descending schedule time.
+        :param sort_order: The order to sort notifications by their schedule
+            time.  Default to ``SortOrder.ascending``.
 
-        @param start_time: Indicate the earliest time of submission to return
+        :param start_time: The earliest time of submission to return
             notifications.
 
 
-        @return: A list of instances containing the following members:
+        :return: A list of objects containing the following members:
 
-            * `creation_time` (required): Time when the sender originated the
-              notification to the intended recipient.
+            - ``creation_time: ISO8601DateTime`` (required): The time when the
+              sender originated the notification to the intended recipient.
 
-            * `is_read` (required): Indicate whether the notification has been read
-              by the intended recipient.
+            - ``is_read: bool`` (required): Indicate whether the notification has
+              been read by the intended recipient.
 
-            * `notification_id` (required): Identification of the  notification.
+            - ``notification_id: UUID`` (required): The identifier of the  notification.
 
-            * `notification_type` (required): String representation of the type of
-              the notification, as selected by the sender that originated this
-              notification to the intended recipient.
+            - ``notification_type: str`` (required): A string representation of the
+              type of the notification, as selected by the sender that originated
+              this notification to the intended recipient.
 
-            * `payload` (optional): An arbitrary JSON expression added by the
-              sender to provide information about the context of this notification.
+            - ``payload: json`` (optional): An arbitrary JSON expression added by
+              the sender to provide information about the context of this
+              notification.
 
-            * `schedule_time` (required): Time when this notification is scheduled
-              to be sent to the intended recipient.  The notification is not visible
-              to the intended recipient prior to this time.
+            - ``schedule_time: ISO8601DateTime`` (required): The time when this
+              notification is scheduled to be sent to the intended recipient.  The
+              notification is not visible to the intended recipient prior to this
+              time.
 
-            * `sender_id` (optional): The identification of the sender that
+            - ``sender_id: str`` (optional): The identifier of the sender that
               originated the notification.
 
-            * `update_time` (required): Time of the most recent modification of an
-              attribute of the notification, such as its read status.
+            - ``update_time: ISO8601DateTime`` (required): Time of the most recent
+              modification of an attribute of the notification, such as its read
+              status.
         """
+        if sort_order is None:
+            sort_order = SortOrder.ascending
+
         with self.acquire_rdbms_connection(auto_commit=mark_read, connection=connection) as connection:
             if mark_read:
                 cursor = connection.execute(
-                    f"""
+                    f'''
                     UPDATE 
                         notification
                       SET
                         is_read = true
                       WHERE
                         notification_id IN (
                           SELECT 
@@ -669,29 +728,30 @@
                         notification_type,
                         is_read,
                         sender_id,
                         payload,
                         schedule_time,
                         creation_time,
                         update_time
-                    """,
+                    ''',
                     {
                         'OBJECT_STATUS_ENABLED': ObjectStatus.enabled,
                         'end_time': end_time,
                         'include_read': include_read,
-                        'limit': min(limit, self.MAXIMUM_LIMIT) or self.DEFAULT_LIMIT,
+                        'limit': min(limit or self.DEFAULT_LIMIT, self.MAXIMUM_LIMIT),
                         'notification_types': notification_types,
                         'offset': offset,
                         'recipient_id': recipient_id,
-                        'start_time': start_time
-                    })
+                        'start_time': start_time,
+                    }
+                )
 
             else:
                 cursor = connection.execute(
-                    f"""
+                    f'''
                     SELECT 
                         notification_id,
                         notification_type,
                         is_read,
                         sender_id,
                         payload,
                         schedule_time,
@@ -706,472 +766,429 @@
                         AND (%(include_read)s OR NOT is_read)
                         AND (%(notification_types)s IS NULL OR notification_type IN (%(notification_types)s))
                         AND object_status = %(OBJECT_STATUS_ENABLED)s
                       ORDER BY
                         creation_time {'ASC' if sort_order == SortOrder.ascending else 'DESC'}
                       OFFSET %(offset)s
                       LIMIT %(limit)s
-                    """,
+                    ''',
                     {
                         'OBJECT_STATUS_ENABLED': ObjectStatus.enabled,
                         'end_time': end_time,
                         'include_read': include_read,
-                        'limit': min(limit, self.MAXIMUM_LIMIT) or self.DEFAULT_LIMIT,
+                        'limit': min(limit or self.DEFAULT_LIMIT, self.MAXIMUM_LIMIT),
                         'notification_types': notification_types,
                         'offset': offset,
                         'recipient_id': recipient_id,
-                        'start_time': start_time
-                    })
+                        'start_time': start_time,
+                    }
+                )
 
             notifications = [
                 row.get_object({
                     'creation_time': cast.string_to_timestamp,
                     'notification_id': cast.string_to_uuid,
                     'payload': cast.string_to_json,
                     'schedule_time': cast.string_to_timestamp,
-                    'update_time': cast.string_to_timestamp
+                    'update_time': cast.string_to_timestamp,
                 })
                 for row in cursor.fetch_all()
             ]
 
             return notifications
 
     def register_device(
             self,
-            app_id,
-            device_id,
-            device_token,
-            device_platform,
-            account_id=None,
-            connection=None,
-            locale=None,
-            topics=None,
-            utc_offset=None):
+            app_id: UUID,
+            device_id: str,
+            device_token: str,
+            device_platform: DevicePlatform,
+            account_id: UUID = None,
+            connection: RdbmsConnection = None,
+            language: Locale = None,
+            topics: list[str] = None,
+            utc_offset: int = None) -> any:
         """
         Register a device to receive push notification messages from the
         platform.
 
 
-        @note: the function registers the device on behalf of the application
+        :note: The function registers the device on behalf of the application
             identification of the server platform, not the identification of
             the client application itself.  An instance of a server platform
             is specific to a particular service to which client applications,
             whatever their platform (Android, iOS, Web, etc.) and therefore
             whatever their application identification, are interested in
             receiving push notifications.
 
 
-        @todo: the argument "topics" is not used at the moment.
+        :todo: The argument "topics" is not used at the moment.
 
 
-        @param app_id: Identification of the client application such as a Web,
-            a desktop, or a mobile application, that accesses the service.
+        :param app_id: The identifier of the client application that accesses
+            the service.
 
-        @param device_id: Identification of the device, which depends on the
+        :param device_id: The identifier of the device, which depends on the
             device platform:
 
-            * Android: International Mobile Equipment Identity (IMEI) number
-              of the device.
+            - Android: On Android 8.0 (API level 26) and higher versions of the
+              platform, a 64-bit number (expressed as a hexadecimal string), unique
+              to each combination of app-signing key, user, and device.  The value
+              may change if a factory reset is performed on the device or if an
+              APK signing key changes.
 
-            * iOS: unique identifier of the iOS device, previously the
+            - iOS: The unique identifier of the iOS device, previously the
               Unique Device Identifier (UDID) of the device, which is a
               40-character string that is tied to this specific Apple device.
               It could be a SecureUDID, which is an open-source sandboxed UDID
               solution aimed at solving the main privacy issues that caused
               Apple to deprecate UDIDs.
 
-        @param device_token: Token that identifies the device by the push
+        :param device_token: A token that identifies the device by the push
             notification provider of the device platform.
 
-            * Android: token identifying the device to push the notification
-              to, i.e., the registration ID.  A device token is an opaque
-              identifier of a device that Android Google Cloud Messaging (GCM)
-              gives to the device when it first connects with it.  The device
-              shares the device token with its provider. The device token is
-              analogous to a phone number; it contains information that enables
-              GCM to locate the device on which the client application is
-              installed.  GCM also uses it to authenticate the routing of a
-              notification.
-
-            * iOS: token identifying the iOS device to push the notification
-              to.  A device token is an opaque identifier of a device that APNs
-              gives to the device when it first connects with it.  The device
-              shares the device token with its provider. Thereafter, this token
-              accompanies each notification from the provider.  The device
-              token is analogous to a phone number; it contains information
-              that enables APNs to locate the device on which the client
-              application is installed. APNs also uses it to authenticate the
-              routing of a notification.  A device token is not the same thing
-              as the device UDID returned by the `uniqueIdentifier` property
-              of `UIDevice`.
-
-        @param device_platform: Indicate the platform of the end user's mobile
-            device:
+            - Android: A token identifying the device to push the notification to,
+              i.e., the registration ID.  A device token is an opaque identifier
+              of a device that Android Google Cloud Messaging (GCM) gives to the
+              device when it first connects with it.  The device shares the device
+              token with its provider.  The device token is analogous to a phone
+              number; it contains information that enables GCM to locate the device
+              on which the client application is installed.  GCM also uses it to
+              authenticate the routing of a notification.
+
+            - iOS: A token identifying the iOS device to push the notification to.
+              A device token is an opaque identifier of a device that APNs gives to
+              the device when it first connects with it.  The device shares the
+              device token with its provider. Thereafter, this token accompanies
+              each notification from the provider.  The device token is analogous
+              to a phone number; it contains information that enables APNs to locate
+              the device on which the client application is installed. APNs also
+              uses it to authenticate the routing of a notification.  A device token
+              is not the same thing as the device UDID returned by the
+              ``uniqueIdentifier`` property of ``UIDevice``.
+
+        :param device_platform: The platform of the end user's mobile device:
 
-            * `ios`: Apple iOS
+            - `ios`: Apple iOS
 
-            * `android`: Google Android
+            - `android`: Google Android
 
-            * `windows`: Windows Phone
+            - `windows`: Windows Phone
 
-        @param account_id: Identification of the account of the user on behalf
+        :param account_id: The identifier of the account of the user on behalf
             of whom the device is registered to receive push notification
             messages.
 
-        @param connection: An object `RdbmsConnection` with auto commit.
+        :param connection: A connection to the notification database.
 
-        @param locale: Represent the language that the end user prefers
-            receiving new content in.  A locale corresponds to a tag
-            respecting RFC 4646, expressed by a ISO 639-3 alpha-3 code
-            element, optionally followed by a dash character `-` and a ISO
-            3166-1 alpha-2 code.  For example: "eng" (which denotes a standard
-            English), "eng-US" (which denotes an American English).  If this
-            argument is not specified, the locale corresponds to the preferred
-            language that the user has defined in his profile.
+        :param language: The language that the end user prefers receiving new
+            content in.
 
-        @param topics: A list of keywords representing topics the end user is
+        :param topics: A list of keywords representing topics the end user is
             interested in to be pushed new content whenever related to one of
             those topics.  The list of supported keywords is specific to the
             publisher service of the client application and as such the
             developer of the client application has to refer to the technical
             documentation of the publisher service.
 
-        @param utc_offset: Difference between the location of the device and
-            UTC (Universal Time Coordinated).  UTC is also known as GMT or
+        :param utc_offset: The difference between the location of the device
+            and UTC (Universal Time Coordinated).  UTC is also known as GMT or
             Greenwich Mean Time or Zulu Time.
 
 
-        @return: An object containing the following attributes:
+        :return: An object containing the following attributes:
 
-            * `device_id` (required): Identification of the mobile device that
-              registers to push notification service.
+            - ``device_id: str`` (required): The identifier of the mobile device
+              that registers to push notification service.
 
-            * `object_status` (required): Current status of the registration of
-              this device to push notification service.
+            - ``object_status: ObjectStatus` (required): The current status of the
+              registration of this device to push notification service.
 
-            * `registration_id` (required): Identification of the registration of
-              the mobile device to the push notification service.
+            - ``registration_id: UUID`` (required): The identifier of the
+              registration of the mobile device to the push notification service.
 
-            * `update_time` (required): Time of the most recent modification of
-              information of the mobile device's registration to the push
-              notification service.
+            - ``update_time: ISO8601DateTime`` (required): The time of the most
+              recent modification of properties of the mobile device's registration
+              to the push notification service.
         """
-
         with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
             ApplicationService().get_application_with_id(app_id, check_status=True, connection=connection)
 
             device_registration = self.__get_device_registration(
                 device_id,
                 app_id,
                 account_id=account_id,
-                connection=connection)
+                connection=connection
+            )
 
             if device_registration is None:
                 device_registration = self.__add_device_registration(
                     device_id,
                     device_platform,
                     app_id,
                     device_token,
                     account_id=account_id,
                     connection=connection,
-                    locale=locale,
-                    utc_offset=utc_offset)
+                    language=language,
+                    utc_offset=utc_offset
+                )
             elif device_registration.device_token != device_token:
                 device_registration = self.__update_device_registration_token(
                     device_registration.registration_id,
                     device_token,
-                    connection=connection)
+                    connection=connection
+                )
 
             return device_registration
 
     def send_notification(
             self,
-            app_id,
-            notification_type,
-            connection=None,
-            recipient_ids=None,
-            team_id=None,
-            if_not_exists=False,
-            lifespan=DEFAULT_LIFESPAN,
-            notification_mode=None,
-            package=None,
-            payload=None,
-            sender_id=None,
-            schedule_time=None,
-            recipient_timezones=None):
+            app_id: UUID,
+            notification_type: str,
+            connection: RdbmsConnection = None,
+            recipient_ids: str or list[str] = None,
+            if_not_exists: bool = False,
+            lifespan: int = DEFAULT_LIFESPAN,
+            notification_mode: NotificationMode = None,
+            # package_name: str = None,
+            payload: json = None,
+            sender_id: str = None,
+            schedule_time: ISO8601DateTime = None,
+            recipient_timezones: dict[str, int] = None) -> any:
         """
         Send a notification to the intended recipient(s) as soon as possible
         or at a given time.
 
         The notification and its content is stored for later delivery up to a
         maximum period of time, the lifespan of the notification, also known
         as its time-to-live(TTL).  The primary reason for this is that a
         device may be unavailable (e.g., turned off, no network coverage).
 
 
-        @param app_id: identification of the client application such as a Web,
-            a desktop, or a mobile application, that accesses the service.
-
-        @param notification_type: type of the notification to be sent, such as
-            for instance `on_something_happened`.
+        :param app_id: The identifier of the client application that accesses
+            the service.
 
-        @param connection: a `RdbmsConnection` instance to be used
-            supporting the Python clause `with ...:`.
+        :param notification_type: The type of the notification to be sent, such
+            as for instance `on_something_happened`.
 
-        @param recipient_ids: identification of a recipient, or a list of
-            identifications of recipients, to send the notification to.
+        :param connection: A connection to the notification database.
 
-        @param team_id: identification of a team to send the notification to
-            all the members.
+        :param recipient_ids: The identifier of a recipient, or a list of
+            identifiers of recipients, to send the notification to.
 
-        @param if_not_exists: indicate whether the notification needs to be
+        :param if_not_exists: Indicate whether the notification needs to be
             ignored for a particular recipient if the latter already received
             a notification of the same type that the recipient has not yet
             read.  The function doesn't check whether a previous notification
             of the same type may have a different payload.
 
-        @param lifespan: period of time expressed in seconds during which
+        :param lifespan: The period of time expressed in seconds during which
             information of the notification reasonably may be expected
             usefully to inform an action or interest of the intended
             recipients.  After the lifespan expires, provision of the
             notification to the recipients may be prevented; the notification
             and its content may be deleted.  The maximum lifespan is
-            `NotificationService.MAXIMUM_LIFESPAN`.
+            ``NotificationService.MAXIMUM_LIFESPAN``.
 
-        @param notification_mode: an item of the enumeration `NotificationMode`
-            to indicate the mode to deliver this notification to the
-            recipients:
-
-            * `pull` (default): indicate that a notification message is
-              delivered to the specified recipients when the request for the
-              transmission of information is initiated by the receiver or client
-              application, and then is responded by the publisher or server
-              platform.
+        :param notification_mode: The mode to deliver this notification to the
+            recipients.
 
-            * `push`: indicate that a notification message is delivered to the
-              specified recipients when the request for the transmission of
-              information is initiated by the publisher or server platform and
-              pushed out to the receiver or client application.
-
-        @param payload: any arbitrary JSON expression added by the sender to
+        :param payload: Any arbitrary JSON expression added by the sender to
             provide information about the context of this notification.
 
-        @param sender_id: identification of the sender on behalf whom the
+        :param sender_id: The identifier of the sender on behalf whom the
             notification is sent to the recipients.
 
-        @param schedule_time: Time when this notification needs to be sent to
-            the intended recipient.  The notification is not visible to the
+        :param schedule_time: The time when this notification needs to be sent
+            to the intended recipient.  The notification is not visible to the
             intended recipient prior to this time.  If not specified, the
             notification is sent as soon as possible.
 
-        @param recipient_timezones: dictionary of time zones of the intended
+        :param recipient_timezones: A dictionary of time zones of the intended
             recipients for which the schedule time is expected to be in their
-            local time.  The key corresponds to the identification of an
-            intended recipient, and the value corresponds to time zone of this
+            local time.  The key corresponds to the identifier of an intended
+            recipient, and the value corresponds to time zone of this
             particular recipient.
 
             When a time zone is defined for a particular recipient, the
             function understands that the schedule time of the notification
             for this recipient has to be converted to the local time of this
-            recipient.  The function converts `schedule_time` to UTC, and it
+            recipient.  The function converts ``schedule_time`` to UTC, and it
             strips the time zone information to get a local time to which the
             function adds the recipient's time zone.
 
             For instance, if the specified schedule time is
-            `2013-12-20 15:00:00+07` and the time zone `+7` is specified
+            ``2013-12-20 15:00:00+07`` and the time zone ``+7`` is specified
             for a recipient, the schedule time is assumed to be the local time
-            `2013-12-20 08:00:00` for the region, i.e., time zone, of this
+            ``2013-12-20 08:00:00`` for the region, i.e., time zone, of this
             recipient.  The resulting schedule time with time zone for this
-            recipient is then `2013-12-20 08:00:00+07`
+            recipient is then ``2013-12-20 08:00:00+07``
 
 
-        @return: a list of instances containing the following members:
+        :return: A list of objects containing the following attributes:
 
-            * `notification_id`: Identification of the notification sent to a
-              particular recipient.
+            - ``notification_id: UUID`` (required): The identifier of the
+              notification sent to a particular recipient.
 
-            * `recipient_id`: String representation of the identification of
-              the recipient intended to be delivered this notification.
+            - ``recipient_id: str``: The string representation of the identification
+              of the recipient intended to be delivered this notification.
         """
-        if not recipient_ids and team_id is None:
+        if not recipient_ids:
             return
 
-        # Convert the argument `recipient_ids` to a list if it's not already
-        # a list, a set, or a tuple.
-        recipient_ids = [] if recipient_ids is None \
-            else set([str(recipient_ids)] if not isinstance(recipient_ids, (list, set, tuple)) \
-            else [str(recipient_id) for recipient_id in recipient_ids])
-
-        # If an organisation has been specified, retrieve the list of all its
-        # members to send the notification to.
-        if team_id:
-            offset = 0
-
-            while True:
-                accounts = TeamService().get_members(
-                    app_id,
-                    team_id,
-                    limit=TeamService.DEFAULT_LIMIT,
-                    offset=offset)
-
-                recipient_ids.update([str(account.account_id) for account in accounts])
-                if len(accounts) < TeamService.DEFAULT_LIMIT:
-                    break
+        if not isinstance(recipient_ids, (list, set, tuple)):
+            recipient_ids = [recipient_ids]
 
-                offset += len(accounts)
+        # Remove any duplicated recipient identifiers.
+        recipient_ids = list(set([
+            str(recipient_id)
+            for recipient_id in recipient_ids
+        ]))
 
         with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
-            # Filter out the recipients that have already been sent this
-            # notification type but they have not read it yet.
+            # Remove any recipients who would have already received a similar
+            # notification.
             if if_not_exists:
-                cursor = connection.execute(
-                    """
-                    SELECT DISTINCT 
-                        recipient_id
-                      FROM 
-                        notification
-                      WHERE
-                        notification_type = %(notification_type)s
-                        AND recipient_id IN (%[recipient_ids]s)
-                        AND (%(sender_id)s IS NULL OR sender_id = %(sender_id)s)
-                        AND NOT is_read
-                    """,
-                    {
-                        'notification_type': notification_type,
-                        'recipient_ids': recipient_ids,
-                        'sender_id': sender_id
-                    })
+                already_notified_recipient_ids = self.__filter_already_notified_recipients(
+                    notification_type,
+                    recipient_ids,
+                    connection=connection,
+                    sender_id=sender_id
+                )
 
-                recipient_ids = set(recipient_ids) - set([ row.get_value('recipient_id') for row in cursor.fetch_all() ])
+                recipient_ids = list(set(recipient_ids) - set(already_notified_recipient_ids))
 
                 if len(recipient_ids) == 0:
                     return
 
+            # Determine the expiration time of this notification.
             expiration_time = ISO8601DateTime.now() + datetime.timedelta(
                 seconds=max(lifespan or self.DEFAULT_LIFESPAN, self.MAXIMUM_LIFESPAN))
 
-            print('######################')
-            print(type(obj.stringify(payload)))
-            print(str(payload))
-            print(type(str(payload)))
-            print('######################')
-
             # Register this notification for every recipient.
             cursor = connection.execute(
-                """
-                INSERT INTO notification(
+                '''
+                INSERT INTO notification (
                     notification_type,
                     notification_mode,
                     recipient_id,
                     sender_id,
                     payload,
                     schedule_time,
                     expiration_time,
-                    app_id)
+                    app_id
+                  )
                   VALUES
                     %[values]s
                   RETURNING
                     notification_id,
                     recipient_id
-                """,
+                ''',
                 {
                     'values': [
                         (
                             notification_type,
-                            notification_mode or NotificationService.NotificationMode.push,
+                            notification_mode or NotificationMode.push,
                             recipient_id,
                             sender_id,
                             payload and str(payload),
                             schedule_time,
                             expiration_time,
                             # ('DEFAULT', ) if schedule_time is None
                             #     else schedule_time if (recipient_timezones is None or recipient_timezones.get(recipient_id) is None)
                             #     else cast.string_to_timestamp('%s%+03d' % (str(schedule_time)[:-6], recipient_timezones[recipient_id])),
                             # (("current_timestamp + '%d seconds'::interval" % max(lifespan, self.MAXIMUM_LIFESPAN)), ),
                             app_id,
                         )
                         for recipient_id in recipient_ids
                     ]
-                })
+                }
+            )
 
-            return [
+            notifications = [
                 row.get_object({
-                    'notification_id': cast.string_to_uuid
+                    'notification_id': cast.string_to_uuid,
                 })
                 for row in cursor.fetch_all()
             ]
 
+            return notifications
+
     def unregister_device(
             self,
-            app_id,
-            device_id,
-            account_id=None):
+            app_id: UUID,
+            device_id: str,
+            account_id: UUID = None) -> None:
         """
-        Unregister a device from receiving push notification messages from the
-        platform.
+        Unregister a device from receiving push notification messages.
 
 
-        @param app_id: identification of the client application such as a Web,
-            a desktop, or a mobile application, that accesses the service.
+        :param app_id: The identifier of the client application that accesses
+            the service.
 
-        @param device_id: identification of the device, which depends on the
-            device platform:
+        :param device_id: The device's identifier, which depends on the device
+            platform:
 
-            * Android: International Mobile Equipment Identity (IMEI) number
-              of the device.
+            - Android: On Android 8.0 (API level 26) and higher versions of the
+              platform, a 64-bit number (expressed as a hexadecimal string), unique
+              to each combination of app-signing key, user, and device.  The value
+              may change if a factory reset is performed on the device or if an
+              APK signing key changes.
 
-            * iOS: unique identifier of the iOS device, previously the
+            - iOS: unique identifier of the iOS device, previously the
               Unique Device Identifier (UDID) of the device, which is a
               40-character string that is tied to this specific Apple device.
               It could be a SecureUDID, which is an open-source sandboxed UDID
               solution aimed at solving the main privacy issues that caused
               Apple to deprecate UDIDs.
 
-        @param account_id: identification of the account of the user on behalf
+        :param account_id: The identifier of the account of the user on behalf
             of whom the device is unregistered from receiving push
             notification messages.
         """
         with self.acquire_rdbms_connection(True) as connection:
-            connection.execute("""
+            connection.execute(
+                '''
                 DELETE FROM 
                     notification_device
                   WHERE 
                     device_id = %(device_id)s
-                    AND ((account_id IS NULL AND %(account_id)s IS NULL) OR
-                         (account_id = %(account_id)s))
+                    AND ((account_id IS NULL AND %(account_id)s IS NULL) 
+                         OR (account_id = %(account_id)s))
                     AND app_id = %(app_id)s
-                """,
+                ''',
                 {
                     'account_id': account_id,
                     'app_id': app_id,
-                    'device_id': device_id
-                })
+                    'device_id': device_id,
+                }
+            )
 
 
 
 
 
 
 
 
 # def flush_notifications(self, app_id, account_id,
 #         service_name=None, notification_types=None):
 #     """
 #     Flush all the notifications originated from the given client
 #     application that were sent to the specified user.
 #
-#     @param app_id: identification of the client application such as a Web,
+#     :param app_id: identification of the client application such as a Web,
 #         a desktop, or a mobile application, that accesses the service.
-#     @param account_id: identification of the account of the user to flush
+#     :param account_id: identification of the account of the user to flush
 #         all the notifications he receives from the given application.
-#     @param service_name: code name of the service that originated the
+#     :param service_name: code name of the service that originated the
 #         notifications to flush.  By convention, the code name of the
 #         service corresponds to the Python class of this service (cf.
 #         `self.__class__.__name__`).
-#     @param notification_types: a list of types of the notifications to
+#     :param notification_types: a list of types of the notifications to
 #         flush.  If no list is provided, the function flushes all the
 #         notifications that the client application posted to the user.
 #     """
 #     with self.acquire_rdbms_connection(True) as connection:
 #         if notification_types is None:
 #             connection.execute("""
 #                 DELETE FROM notification
@@ -1201,24 +1218,24 @@
 
 # def mark_notifications(self, app_id, account_id, notification_ids,
 #         mark_read=True):
 #     """
 #     Update the read mark of a list of notifications sent to the specified
 #     user.
 #
-#     @param app_id: identification of the client application such as a Web,
+#     :param app_id: identification of the client application such as a Web,
 #            a desktop, or a mobile application, that accesses the service.
 #
-#     @param account_id: identification of the account of a user whom the
+#     :param account_id: identification of the account of a user whom the
 #            specified notifications have been sent to.
 #
-#     @param notification_ids: a list of notification to mark as read or
+#     :param notification_ids: a list of notification to mark as read or
 #            unread.
 #
-#     @param mark_read: indicate whether to mark as read the specified
+#     :param mark_read: indicate whether to mark as read the specified
 #         notifications.
 #     """
 #     if notification_ids is None:
 #         return
 #
 #     if type(notification_ids) not in (list, set, tuple):
 #         notification_ids = [ notification_ids ]
@@ -1257,69 +1274,69 @@
 #
 #
 # The function checks whether the  payload, if any provided, is of a
 # simple type such as a number (integer, decimal, complex) or a string.
 # If not, the function convert the payload to a string representation
 # of a JSON expression.
 #
-# @warning: this function is for internal usage only; it MUST not be
+# :warning: this function is for internal usage only; it MUST not be
 #     surfaced to any client applications through a RESTful API.
 #
-# @param app_id: identification of the client application such as a Web,
+# :param app_id: identification of the client application such as a Web,
 #     a desktop, or a mobile application, that accesses the service.
-# @param notification_type: type of the notification such as
+# :param notification_type: type of the notification such as
 #     `on_something_happened`.
-# @param notification_mode:
+# :param notification_mode:
 #
-# @param account_ids: list of account identifications of users to send
+# :param account_ids: list of account identifications of users to send
 #     the notification to.
-# @param device_ids: list of identifications of devices to send the
+# :param device_ids: list of identifications of devices to send the
 #     notification to.
 #
-# @param payload: content of the notification to send to the recipients.
+# :param payload: content of the notification to send to the recipients.
 #     The content could be a simple string caption, or an object which
 #     the function converts its JSON expression.into a string
 #     representation.
-# @param lifespan: duration in minutes the notification lives before it
+# :param lifespan: duration in minutes the notification lives before it
 #     is deleted.  If not defined, the notification persists forever as
 #     long as it is not read.
-# @param topics: a list of keywords indicating the subjects of this
+# :param topics: a list of keywords indicating the subjects of this
 #     notifications.  Only the subscribers who have registered for these
 #     topics will be pushed this notification.
 #
-# @param schedule_time: schedule the notification to automatically be
+# :param schedule_time: schedule the notification to automatically be
 #     sent later at the given time.  If not specified, the notification
 #     is sent as soon as possible.
-# @param use_local_time: indicate whether the schedule time is assumed
+# :param use_local_time: indicate whether the schedule time is assumed
 #     to be in local time of a particular device.  If so, the
 #     `schedule_time` is converted to UTC, and the time zone
 #     information is then stripped out to provide a local time.  For
 #     instance, if the specified schedule time is `2013-12-20 13:00:00+07`
 #     and the argument `use_local_time` is set to `True`, the
 #     schedule time is assumed to be the local time `2013-12-20 06:00:00`
 #     for the region, i.e., time zone, of a particular device to send
 #     the notification to.
 #
-# @param is_broadcast: indicate whether the notification needs to be
-#     sent to every users who subscribed for receiving notification from
+# :param is_broadcast: indicate whether the notification needs to be
+#     sent to every user who subscribed for receiving notification from
 #     this application (determined by `app_id`), or more generally
 #     from the product this application belongs to (if the argument
 #     `is_product_based` is `True`).
 #         """
 #
 #         if account_ids is None and device_ids is None:
 #             raise self.InvalidArgumentException('No recipient has been specified')
 #
 #         if schedule_time and expiration_time and schedule_time > expiration_time:
 #             raise self.InvalidArgumentException('The expiration time of a message MUST be posterior to the specified schedule time')
 #
 #         # If the payload of the message is not a simple type, convert it to a
 #         # string representation of a JSON expression.
 #         #
-#         # @note: `basestring` includes `str` and `unicode`.
+#         # :note: `basestring` includes `str` and `unicode`.
 #         if payload and not isinstance(payload,  (basestring, int, long, float, complex)):
 #             payload = obj.jsonify(payload)
 
 
 # def send_device_notification(self, app_id, notification_type, device_ids,
 #         notification_mode=NotificationMode.push,
 #         if_not_exists=False,
@@ -1332,52 +1349,52 @@
 #
 #     The notification and its content is stored for later delivery up to a
 #     maximum period of time, the lifespan of the notification, also known
 #     as its time-to-live(TTL).  The primary reason for this is that a
 #     device may be unavailable (e.g., turned off, no network coverage).
 #
 #
-#     @param app_id: identification of the client application such as a Web,
+#     :param app_id: identification of the client application such as a Web,
 #         a desktop, or a mobile application, that accesses the service.
 #
-#     @param notification_type: type of the notification to be sent, such as
+#     :param notification_type: type of the notification to be sent, such as
 #         for instance `on_something_happened`.
 #
-#     @param device_ids: identification of the device, or a list of
+#     :param device_ids: identification of the device, or a list of
 #         identifications of devices, to send the notification to.
 #
-#     @param if_not_exists: indicate whether the notification needs to be
+#     :param if_not_exists: indicate whether the notification needs to be
 #         ignored for a particular device if the latter already received a
 #         notification of the same type that the device has not yet read.
 #         The function doesn't check whether a previous notification of the
 #         same type may have a different payload.
 #
-#     @param lifespan: period of time expressed in seconds during which
+#     :param lifespan: period of time expressed in seconds during which
 #         information of the notification reasonably may be expected
 #         usefully to inform an action or interest of the intended devices.
 #         After the lifespan expires, provision of the notification to the
 #         devices may be prevented; the notification and its content may be
 #         deleted.  The maximum lifespan is `NotificationService.MAXIMUM_LIFESPAN`.
 #
-#     @param payload: any arbitrary JSON expression added by the sender to
+#     :param payload: any arbitrary JSON expression added by the sender to
 #         provide information about the context of this notification.
 #
-#     @param sender_id: identification of the sender on behalf whom the
+#     :param sender_id: identification of the sender on behalf whom the
 #         notification is sent to the devices.
 #
 #
-#     @return: a list of instances containing the following members:
+#     :return: a list of instances containing the following members:
 #
-#         * `creation_time` (required): time when the notification was
+#         - `creation_time` (required): time when the notification was
 #           registered to the platform.
 #
-#         * `device_id` (required): identification of a device that is sent
+#         - `device_id` (required): identification of a device that is sent
 #           this notification.
 #
-#         * `notification_id` (required): identification of the notification
+#         - `notification_id` (required): identification of the notification
 #           sent to the device.
 #     """
 #     if device_ids is None:
 #         return
 #
 #     if not isinstance(device_ids, (list, set, tuple)):
 #         device_ids = [ device_ids ]
@@ -1429,15 +1446,15 @@
 #                 for row in cursor.fetch_all() ]
 
 
 # def send_notifications(self, app_id, notification_type, recipient_ids, payloads,
 #         if_not_exists=False,
 #         lifespan=DEFAULT_LIFESPAN,
 #         notification_mode=NotificationMode.pull,
-#         package=None,
+#         package_name=None,
 #         sender_id=None,
 #         schedule_time=None,
 #         recipient_timezones=None):
 #
 #     if not recipient_ids:
 #         return
 #
@@ -1470,28 +1487,28 @@
 #                 notification_mode,
 #                 recipient_id,
 #                 sender_id,
 #                 payload,
 #                 schedule_time,
 #                 expiration_time,
 #                 app_id,
-#                 package)
+#                 package_name)
 #               VALUES %[values]s
 #               RETURNING notification_id,
 #                         recipient_id""",
 #             { 'values': [
 #                     (notification_type,
 #                      notification_mode,
 #                      recipient_id,
 #                      sender_id,
 #                      json_payload,
 #                      (True, 'DEFAULT') if schedule_time is None \
 #                         else schedule_time if (recipient_timezones is None or recipient_timezones.get(recipient_id) is None) \
 #                         else cast.string_to_timestamp('%s%+03d' % (str(schedule_time)[:-6] ), recipient_timezones[recipient_id]),
 #                      (True, "current_timestamp + '%d seconds'::interval" % max(lifespan, self.MAXIMUM_LIFESPAN)),
 #                      app_id,
-#                      package)
+#                      package_name)
 #                     for json_payload in json_payloads
 #                         for recipient_id in recipient_ids ] })
 #
 #         return [ row.get_object({ 'notification_id': cast.string_to_uuid })
 #                 for row in cursor.fetch_all() ]
```

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/__init__.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/status/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/doc/api/get_ping.rst` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/status/doc/api/get_ping.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/doc/api/get_status.rst` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/status/doc/api/get_status.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/doc/api/index.rst` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/status/doc/api/index.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/status_service.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/status/status_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/status_service_http_handler.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/status/status_service_http_handler.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/__init__.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/agent/team_invite.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/agent/team_invite.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/create_team_constraint.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/db/create_team_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/create_team_function.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/db/create_team_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/create_team_index.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/notification/db/create_notification_index.sql`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,8 @@
  *
  * MAJORMODE MAKES NO REPRESENTATIONS OR WARRANTIES ABOUT THE SUITABILITY
  * OF THE SOFTWARE, EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
  * TO THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR
  * PURPOSE, OR NON-INFRINGEMENT.  MAJORMODE SHALL NOT BE LIABLE FOR ANY
  * LOSSES OR DAMAGES SUFFERED BY LICENSEE AS A RESULT OF USING, MODIFYING
  * OR DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES.
-*/
-
-CREATE UNIQUE INDEX idx_team_name
-  ON team (lower(name));
-
-
-CREATE UNIQUE INDEX idx_team_contact
-  ON team_contact (
-    lower(property_value),
-    property_name
-  );
+ */
```

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/create_team_table.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/db/create_team_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/migrate_team_table@1.13.3.sql` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/db/migrate_team_table@1.13.3.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/team_service.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/team_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/template/default_invite_email.txt` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/template/default_invite_email.txt`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/test/__init__.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/test/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/test/team_service_unittest.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/team/test/team_service_unittest.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/__init__.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/version/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/doc/api/get_version.rst` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/version/doc/api/get_version.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/doc/api/index.rst` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/version/doc/api/index.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/test/__init__.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/version/test/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/test/version_service_unittest.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/version/test/version_service_unittest.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/version_service.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/version/version_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/version_service_http_handler.py` & `perseus_restful_api_framework-1.27.2/src/majormode/perseus/service/version/version_service_http_handler.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.1/setup.py` & `perseus_restful_api_framework-1.27.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
  'prosoponym>=1.0.7,<2.0.0',
  'psutil>=5.9.4,<6.0.0',
  'pymemcache>=4.0.0,<5.0.0',
  'tornado>=6.2,<7.0']
 
 setup_kwargs = {
     'name': 'perseus-restful-api-framework',
-    'version': '1.27.1',
+    'version': '1.27.2',
     'description': 'Python server framework for quickly building RESTful APIs with minimal effort',
     'long_description': '# Perseus: RESTful API Server Framework\n\nPerseus is a Python framework for quickly building RESTful API servers with minimal effort.\n\nPerseus provides an initial set of core services that supports the following features:\n\n- Client application registration with API keys generation\n- Client application access control with RESTful request signature\n- Client application and RESTful API server version compatibility check\n- User authentication and session management\n- Team/group management\n- RESTful request logging with data sensitiveness support\n- RESTful service automatic discovery\n- HTTP request query parameters & body JSON message automatically parsing (depending on the HTTP method used) with data type check and conversion\n\nPerseus is based on [Tornado](https://www.tornadoweb.org/) for handling client network connection.\n\n## RESTful API Request Handler\n\n```python\nfrom majormode.perseus.service.base_http_handler import HttpRequest\nfrom majormode.perseus.service.base_http_handler import HttpRequestHandler\nfrom majormode.perseus.service.base_http_handler import http_request\n\nimport AttendantService\n\n\nclass AttendantServiceHttpRequestHandler(HttpRequestHandler):\n    @http_request(r\'^/attendant/session$\',\n                  http_method=HttpRequest.HttpMethod.POST,\n                  authentication_required=False,\n                  sensitive_data=True,\n                  signature_required=False)\n    def sign_in(self, request):\n        email_address = request.get_argument(\n            \'email_address\',\n            data_type=HttpRequest.ArgumentDataType.email_address,\n            is_required=True)\n\n        password = request.get_argument(\n            \'password\',\n            data_type=HttpRequest.ArgumentDataType.string,\n            is_required=True)\n\n        return AttendantService().sign_in(request.app_id, email_address, password)\n```\n\n## Configure the environment variables\n\n```env\n# Copyright (C) 2021 Majormode.  All rights reserved.\n#\n# Permission is hereby granted, free of charge, to any person obtaining\n# a copy of this software and associated documentation files (the\n# "Software"), to deal in the Software without restriction, including\n# without limitation the rights to use, copy, modify, merge, publish,\n# distribute, sublicense, and/or sell copies of the Software, and to\n# permit persons to whom the Software is furnished to do so, subject to\n# the following conditions:\n#\n# The above copyright notice and this permission notice shall be\n# included in all copies or substantial portions of the Software.\n#\n# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,\n# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n# MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n# IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\n# CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\n# TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\n# SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n\n# Connection properties of the RESTful API server instances.  Defaults\n# to 127.0.0.1:8081.\nAPI_SERVER_HOSTNAME=127.0.0.1\nAPI_SERVER_PORTS=\n\n# Root path of the Network File System (NFS) -- referring to the\n# distributed file system (not the protocol) -- where the Content\n# Delivery Network (CDN) files are stored into, such as avatars, etc.\nCDN_NFS_ROOT_PATH=\n\n# Hostname of the Content Delivery Network (CDN) server that hosts media\n# files such as avatars, etc.\nCDN_URL_HOSTNAME=\n\n# Environment stage of the API server instances.  Possible values are:\n#\n# - dev\n# - int\n# - staging\n# - prod\n#\n# Defaults to `dev`.\nENVIRONMENT_STAGE=\n\n# Connection properties to a Memcached server (a distributed memory\n# object caching system).  Defaults to 127.0.0.1:11211.\nMEMCACHED_HOSTNAME = \'127.0.0.1\'\nMEMCACHED_PORT = 11211\n\n# Threshold for the logger to level.  Logging messages which are less\n# severe than the specified level will be ignored; logging messages\n# which have this severity level or higher will be emitted.  Possible\n# values are:\n#\n# - debug\n# - info\n# - warning\n# - error\n# - critical\n#\n# Default to \'debug\'.\nLOGGING_LEVEL=\n\n# Environment variables to select default parameter values to connect\n# to PostgreSQL Relational Database Management System.\nPG_HOSTNAME=localhost\nPG_PORT=5432\nPG_DATABASE_NAME=\nPG_USERNAME=\nPG_PASSWORD=\n```\n\n## Run the RESTful API Server Processes\n\n```bash\n$ fab start --port=65180,65181,...\n```\n\nHashtags/Topics: `#perseus` `#restful` `#api` `#server` `#framework` `#python`\n',
     'author': 'Daniel CAUNE',
     'author_email': 'daniel.caune@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/majormode/perseus-restful-api-server-framework',
```

### Comparing `perseus_restful_api_framework-1.27.1/PKG-INFO` & `perseus_restful_api_framework-1.27.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perseus-restful-api-framework
-Version: 1.27.1
+Version: 1.27.2
 Summary: Python server framework for quickly building RESTful APIs with minimal effort
 Home-page: https://github.com/majormode/perseus-restful-api-server-framework
 License: Proprietary
 Keywords: perseus,resful,api,server,framework
 Author: Daniel CAUNE
 Author-email: daniel.caune@gmail.com
 Requires-Python: >=3.9,<4.0
```

