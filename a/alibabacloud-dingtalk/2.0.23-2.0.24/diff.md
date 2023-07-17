# Comparing `tmp/alibabacloud_dingtalk-2.0.23.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.23.tar", last modified: Wed Jul 12 02:54:07 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.24.tar", last modified: Mon Jul 17 04:23:34 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.23.tar` & `alibabacloud_dingtalk-2.0.24.tar`

### file list

```diff
@@ -1,381 +1,381 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/
--rw-r--r--   0 root         (0) root         (0)    20142 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8552 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15385 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25682 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27728 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90914 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   139242 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   165948 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   323041 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   202090 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   575598 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9614 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10132 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   142048 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   346941 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39942 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   106288 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10446 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   126888 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   172646 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   297108 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   392984 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23872 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33155 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223914 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   552073 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515455 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13874 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16265 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    57073 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    75811 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   219916 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   278738 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269893 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   472940 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   731141 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8259 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8976 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   316592 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   439557 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13914 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21801 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4633 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4901 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92926 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137528 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302740 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   379213 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22430 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    31875 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   610684 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   859772 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135110 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9852 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14366 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148979 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   177099 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   264898 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   419073 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/report_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/report_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8048 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/report_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    12289 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/report_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81780 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    93746 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53470 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89290 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148231 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19158 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32757 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   130783 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32014 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    34941 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   179772 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   377816 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   464194 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   687148 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4490 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12583 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2684 2023-07-12 02:54:07.000000 alibabacloud_dingtalk-2.0.23/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/
+-rw-r--r--   0 root         (0) root         (0)    20207 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15385 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25682 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27728 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90914 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   139242 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   165948 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   323041 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   202090 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   576378 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9614 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10132 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142048 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   346941 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39942 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   106288 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10446 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   126888 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   172646 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   297108 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   392984 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23872 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33155 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223914 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   552073 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16265 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    57073 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    75811 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   219916 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   278738 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269893 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   472940 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   731141 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8259 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8976 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   316592 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   439557 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13914 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21801 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4901 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    95111 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   139534 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302740 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   379213 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22430 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    31875 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   610684 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   859772 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135110 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9852 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14366 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148979 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   177099 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   264898 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   419073 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    12289 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89958 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   102471 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56986 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83842 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   361006 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503423 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53470 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89290 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148231 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19158 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32757 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   130783 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32014 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    34941 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   179772 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   377816 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464194 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   687148 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4490 2023-07-17 04:23:33.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12583 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2685 2023-07-17 04:23:34.000000 alibabacloud_dingtalk-2.0.24/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.23/ChangeLog.md` & `alibabacloud_dingtalk-2.0.24/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-12 Version: 2.0.23
+- Update AddOfficialAccountFollower.
+
 2023-07-05 Version: 2.0.22
 - Update AddOfficialAccountFollower.
 
 2023-06-16 Version: 2.0.21
 - Update AddOfficialAccountFollower.
 
 2023-06-13 Version: 2.0.20
```

### Comparing `alibabacloud_dingtalk-2.0.23/LICENSE` & `alibabacloud_dingtalk-2.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/PKG-INFO` & `alibabacloud_dingtalk-2.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.23
+Version: 2.0.24
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.23/README-CN.md` & `alibabacloud_dingtalk-2.0.24/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/README.md` & `alibabacloud_dingtalk-2.0.24/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6863,14 +6863,15 @@
 
 class QueryReceiptDetailForInvoiceResponseBodyResult(TeaModel):
     def __init__(
         self,
         amount: str = None,
         apply_status: str = None,
         biz_status: str = None,
+        business_id: str = None,
         create_time: str = None,
         creator: QueryReceiptDetailForInvoiceResponseBodyResultCreator = None,
         customer: QueryReceiptDetailForInvoiceResponseBodyResultCustomer = None,
         drawer_email: str = None,
         drawer_telephone: str = None,
         invoice_type: str = None,
         model_id: str = None,
@@ -6887,14 +6888,15 @@
         source: str = None,
         status: str = None,
         title: str = None,
     ):
         self.amount = amount
         self.apply_status = apply_status
         self.biz_status = biz_status
+        self.business_id = business_id
         self.create_time = create_time
         self.creator = creator
         self.customer = customer
         self.drawer_email = drawer_email
         self.drawer_telephone = drawer_telephone
         self.invoice_type = invoice_type
         self.model_id = model_id
@@ -6930,14 +6932,16 @@
         result = dict()
         if self.amount is not None:
             result['amount'] = self.amount
         if self.apply_status is not None:
             result['applyStatus'] = self.apply_status
         if self.biz_status is not None:
             result['bizStatus'] = self.biz_status
+        if self.business_id is not None:
+            result['businessId'] = self.business_id
         if self.create_time is not None:
             result['createTime'] = self.create_time
         if self.creator is not None:
             result['creator'] = self.creator.to_map()
         if self.customer is not None:
             result['customer'] = self.customer.to_map()
         if self.drawer_email is not None:
@@ -6982,14 +6986,16 @@
         m = m or dict()
         if m.get('amount') is not None:
             self.amount = m.get('amount')
         if m.get('applyStatus') is not None:
             self.apply_status = m.get('applyStatus')
         if m.get('bizStatus') is not None:
             self.biz_status = m.get('bizStatus')
+        if m.get('businessId') is not None:
+            self.business_id = m.get('businessId')
         if m.get('createTime') is not None:
             self.create_time = m.get('createTime')
         if m.get('creator') is not None:
             temp_model = QueryReceiptDetailForInvoiceResponseBodyResultCreator()
             self.creator = temp_model.from_map(m['creator'])
         if m.get('customer') is not None:
             temp_model = QueryReceiptDetailForInvoiceResponseBodyResultCustomer()
@@ -7364,14 +7370,15 @@
 
 class QueryReceiptForInvoiceResponseBodyList(TeaModel):
     def __init__(
         self,
         amount: str = None,
         apply_status: str = None,
         biz_status: str = None,
+        business_id: str = None,
         create_time: str = None,
         creator: QueryReceiptForInvoiceResponseBodyListCreator = None,
         customer: QueryReceiptForInvoiceResponseBodyListCustomer = None,
         drawer_email: str = None,
         drawer_telephone: str = None,
         invoice_type: str = None,
         model_id: str = None,
@@ -7388,14 +7395,15 @@
         source: str = None,
         status: str = None,
         title: str = None,
     ):
         self.amount = amount
         self.apply_status = apply_status
         self.biz_status = biz_status
+        self.business_id = business_id
         self.create_time = create_time
         self.creator = creator
         self.customer = customer
         self.drawer_email = drawer_email
         self.drawer_telephone = drawer_telephone
         self.invoice_type = invoice_type
         self.model_id = model_id
@@ -7431,14 +7439,16 @@
         result = dict()
         if self.amount is not None:
             result['amount'] = self.amount
         if self.apply_status is not None:
             result['applyStatus'] = self.apply_status
         if self.biz_status is not None:
             result['bizStatus'] = self.biz_status
+        if self.business_id is not None:
+            result['businessId'] = self.business_id
         if self.create_time is not None:
             result['createTime'] = self.create_time
         if self.creator is not None:
             result['creator'] = self.creator.to_map()
         if self.customer is not None:
             result['customer'] = self.customer.to_map()
         if self.drawer_email is not None:
@@ -7483,14 +7493,16 @@
         m = m or dict()
         if m.get('amount') is not None:
             self.amount = m.get('amount')
         if m.get('applyStatus') is not None:
             self.apply_status = m.get('applyStatus')
         if m.get('bizStatus') is not None:
             self.biz_status = m.get('bizStatus')
+        if m.get('businessId') is not None:
+            self.business_id = m.get('businessId')
         if m.get('createTime') is not None:
             self.create_time = m.get('createTime')
         if m.get('creator') is not None:
             temp_model = QueryReceiptForInvoiceResponseBodyListCreator()
             self.creator = temp_model.from_map(m['creator'])
         if m.get('customer') is not None:
             temp_model = QueryReceiptForInvoiceResponseBodyListCustomer()
@@ -7899,14 +7911,15 @@
         return self
 
 
 class QueryReceiptsBaseInfoResponseBodyList(TeaModel):
     def __init__(
         self,
         amount: str = None,
+        business_id: str = None,
         create_time: str = None,
         creator: QueryReceiptsBaseInfoResponseBodyListCreator = None,
         customer: QueryReceiptsBaseInfoResponseBodyListCustomer = None,
         model_id: str = None,
         principal: QueryReceiptsBaseInfoResponseBodyListPrincipal = None,
         project: QueryReceiptsBaseInfoResponseBodyListProject = None,
         receipt_id: str = None,
@@ -7915,14 +7928,15 @@
         source: str = None,
         status: str = None,
         supplier: QueryReceiptsBaseInfoResponseBodyListSupplier = None,
         title: str = None,
         voucher_status: str = None,
     ):
         self.amount = amount
+        self.business_id = business_id
         self.create_time = create_time
         self.creator = creator
         self.customer = customer
         self.model_id = model_id
         self.principal = principal
         self.project = project
         self.receipt_id = receipt_id
@@ -7950,14 +7964,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.amount is not None:
             result['amount'] = self.amount
+        if self.business_id is not None:
+            result['businessId'] = self.business_id
         if self.create_time is not None:
             result['createTime'] = self.create_time
         if self.creator is not None:
             result['creator'] = self.creator.to_map()
         if self.customer is not None:
             result['customer'] = self.customer.to_map()
         if self.model_id is not None:
@@ -7984,14 +8000,16 @@
             result['voucherStatus'] = self.voucher_status
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('amount') is not None:
             self.amount = m.get('amount')
+        if m.get('businessId') is not None:
+            self.business_id = m.get('businessId')
         if m.get('createTime') is not None:
             self.create_time = m.get('createTime')
         if m.get('creator') is not None:
             temp_model = QueryReceiptsBaseInfoResponseBodyListCreator()
             self.creator = temp_model.from_map(m['creator'])
         if m.get('customer') is not None:
             temp_model = QueryReceiptsBaseInfoResponseBodyListCustomer()
```

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1843,15 +1843,15 @@
             action='DeleteCrmFormInstance',
             version='crm_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/crm/formInstances/{instance_id}',
             method='DELETE',
             auth_type='AK',
             style='ROA',
-            req_body_type='json',
+            req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
             dingtalkcrm__1__0_models.DeleteCrmFormInstanceResponse(),
             self.execute(params, req, runtime)
         )
 
@@ -1881,15 +1881,15 @@
             action='DeleteCrmFormInstance',
             version='crm_1.0',
             protocol='HTTP',
             pathname=f'/v1.0/crm/formInstances/{instance_id}',
             method='DELETE',
             auth_type='AK',
             style='ROA',
-            req_body_type='json',
+            req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
             dingtalkcrm__1__0_models.DeleteCrmFormInstanceResponse(),
             await self.execute_async(params, req, runtime)
         )
```

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.core import TeaCore
+from typing import Dict
 
 from alibabacloud_gateway_spi.client import Client as SPIClient
 from alibabacloud_tea_openapi.client import Client as OpenApiClient
 from alibabacloud_tea_openapi import models as open_api_models
 from alibabacloud_gateway_dingtalk.client import Client as GatewayClientClient
 from alibabacloud_tea_util.client import Client as UtilClient
 from alibabacloud_dingtalk.hrm_1_0 import models as dingtalkhrm__1__0_models
@@ -21,14 +22,15 @@
     def __init__(
         self, 
         config: open_api_models.Config,
     ):
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
+        self._signature_algorithm = 'v2'
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
     def add_hrm_preentry_with_options(
         self,
         request: dingtalkhrm__1__0_models.AddHrmPreentryRequest,
@@ -131,14 +133,72 @@
         self,
         request: dingtalkhrm__1__0_models.AddHrmPreentryRequest,
     ) -> dingtalkhrm__1__0_models.AddHrmPreentryResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkhrm__1__0_models.AddHrmPreentryHeaders()
         return await self.add_hrm_preentry_with_options_async(request, headers, runtime)
 
+    def device_market_manager_with_options(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkhrm__1__0_models.DeviceMarketManagerResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='DeviceMarketManager',
+            version='hrm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/hrm/device/market/manager',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkhrm__1__0_models.DeviceMarketManagerResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def device_market_manager_with_options_async(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkhrm__1__0_models.DeviceMarketManagerResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='DeviceMarketManager',
+            version='hrm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/hrm/device/market/manager',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkhrm__1__0_models.DeviceMarketManagerResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def device_market_manager(self) -> dingtalkhrm__1__0_models.DeviceMarketManagerResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.device_market_manager_with_options(headers, runtime)
+
+    async def device_market_manager_async(self) -> dingtalkhrm__1__0_models.DeviceMarketManagerResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.device_market_manager_with_options_async(headers, runtime)
+
     def e_cert_query_with_options(
         self,
         request: dingtalkhrm__1__0_models.ECertQueryRequest,
         headers: dingtalkhrm__1__0_models.ECertQueryHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkhrm__1__0_models.ECertQueryResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,14 +284,85 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AddHrmPreentryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeviceMarketManagerResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        return self
+
+
+class DeviceMarketManagerResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeviceMarketManagerResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeviceMarketManagerResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ECertQueryHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/live_activities_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/report_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/report_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/report_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/report_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1533,14 +1533,202 @@
         self,
         request: dingtalkrobot__1__0_models.RobotMessageFileDownloadRequest,
     ) -> dingtalkrobot__1__0_models.RobotMessageFileDownloadResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkrobot__1__0_models.RobotMessageFileDownloadHeaders()
         return await self.robot_message_file_download_with_options_async(request, headers, runtime)
 
+    def robot_recall_ding_with_options(
+        self,
+        request: dingtalkrobot__1__0_models.RobotRecallDingRequest,
+        headers: dingtalkrobot__1__0_models.RobotRecallDingHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkrobot__1__0_models.RobotRecallDingResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.open_ding_id):
+            body['openDingId'] = request.open_ding_id
+        if not UtilClient.is_unset(request.robot_code):
+            body['robotCode'] = request.robot_code
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='RobotRecallDing',
+            version='robot_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/robot/ding/recall',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkrobot__1__0_models.RobotRecallDingResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def robot_recall_ding_with_options_async(
+        self,
+        request: dingtalkrobot__1__0_models.RobotRecallDingRequest,
+        headers: dingtalkrobot__1__0_models.RobotRecallDingHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkrobot__1__0_models.RobotRecallDingResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.open_ding_id):
+            body['openDingId'] = request.open_ding_id
+        if not UtilClient.is_unset(request.robot_code):
+            body['robotCode'] = request.robot_code
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='RobotRecallDing',
+            version='robot_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/robot/ding/recall',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkrobot__1__0_models.RobotRecallDingResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def robot_recall_ding(
+        self,
+        request: dingtalkrobot__1__0_models.RobotRecallDingRequest,
+    ) -> dingtalkrobot__1__0_models.RobotRecallDingResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkrobot__1__0_models.RobotRecallDingHeaders()
+        return self.robot_recall_ding_with_options(request, headers, runtime)
+
+    async def robot_recall_ding_async(
+        self,
+        request: dingtalkrobot__1__0_models.RobotRecallDingRequest,
+    ) -> dingtalkrobot__1__0_models.RobotRecallDingResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkrobot__1__0_models.RobotRecallDingHeaders()
+        return await self.robot_recall_ding_with_options_async(request, headers, runtime)
+
+    def robot_send_ding_with_options(
+        self,
+        request: dingtalkrobot__1__0_models.RobotSendDingRequest,
+        headers: dingtalkrobot__1__0_models.RobotSendDingHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkrobot__1__0_models.RobotSendDingResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.content):
+            body['content'] = request.content
+        if not UtilClient.is_unset(request.receiver_user_id_list):
+            body['receiverUserIdList'] = request.receiver_user_id_list
+        if not UtilClient.is_unset(request.remind_type):
+            body['remindType'] = request.remind_type
+        if not UtilClient.is_unset(request.robot_code):
+            body['robotCode'] = request.robot_code
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='RobotSendDing',
+            version='robot_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/robot/ding/send',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkrobot__1__0_models.RobotSendDingResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def robot_send_ding_with_options_async(
+        self,
+        request: dingtalkrobot__1__0_models.RobotSendDingRequest,
+        headers: dingtalkrobot__1__0_models.RobotSendDingHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkrobot__1__0_models.RobotSendDingResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.content):
+            body['content'] = request.content
+        if not UtilClient.is_unset(request.receiver_user_id_list):
+            body['receiverUserIdList'] = request.receiver_user_id_list
+        if not UtilClient.is_unset(request.remind_type):
+            body['remindType'] = request.remind_type
+        if not UtilClient.is_unset(request.robot_code):
+            body['robotCode'] = request.robot_code
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='RobotSendDing',
+            version='robot_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/robot/ding/send',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkrobot__1__0_models.RobotSendDingResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def robot_send_ding(
+        self,
+        request: dingtalkrobot__1__0_models.RobotSendDingRequest,
+    ) -> dingtalkrobot__1__0_models.RobotSendDingResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkrobot__1__0_models.RobotSendDingHeaders()
+        return self.robot_send_ding_with_options(request, headers, runtime)
+
+    async def robot_send_ding_async(
+        self,
+        request: dingtalkrobot__1__0_models.RobotSendDingRequest,
+    ) -> dingtalkrobot__1__0_models.RobotSendDingResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkrobot__1__0_models.RobotSendDingHeaders()
+        return await self.robot_send_ding_with_options_async(request, headers, runtime)
+
     def send_robot_ding_message_with_options(
         self,
         request: dingtalkrobot__1__0_models.SendRobotDingMessageRequest,
         headers: dingtalkrobot__1__0_models.SendRobotDingMessageHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkrobot__1__0_models.SendRobotDingMessageResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import Dict, List
+from typing import Dict, List, Any
 
 
 class BatchOTOQueryHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
@@ -2537,14 +2537,306 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RobotMessageFileDownloadResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RobotRecallDingHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class RobotRecallDingRequest(TeaModel):
+    def __init__(
+        self,
+        open_ding_id: str = None,
+        robot_code: str = None,
+    ):
+        self.open_ding_id = open_ding_id
+        self.robot_code = robot_code
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.open_ding_id is not None:
+            result['openDingId'] = self.open_ding_id
+        if self.robot_code is not None:
+            result['robotCode'] = self.robot_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('openDingId') is not None:
+            self.open_ding_id = m.get('openDingId')
+        if m.get('robotCode') is not None:
+            self.robot_code = m.get('robotCode')
+        return self
+
+
+class RobotRecallDingResponseBody(TeaModel):
+    def __init__(
+        self,
+        open_ding_id: str = None,
+    ):
+        self.open_ding_id = open_ding_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.open_ding_id is not None:
+            result['openDingId'] = self.open_ding_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('openDingId') is not None:
+            self.open_ding_id = m.get('openDingId')
+        return self
+
+
+class RobotRecallDingResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: RobotRecallDingResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = RobotRecallDingResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class RobotSendDingHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class RobotSendDingRequest(TeaModel):
+    def __init__(
+        self,
+        content: str = None,
+        receiver_user_id_list: List[str] = None,
+        remind_type: int = None,
+        robot_code: str = None,
+    ):
+        self.content = content
+        self.receiver_user_id_list = receiver_user_id_list
+        self.remind_type = remind_type
+        self.robot_code = robot_code
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.content is not None:
+            result['content'] = self.content
+        if self.receiver_user_id_list is not None:
+            result['receiverUserIdList'] = self.receiver_user_id_list
+        if self.remind_type is not None:
+            result['remindType'] = self.remind_type
+        if self.robot_code is not None:
+            result['robotCode'] = self.robot_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('content') is not None:
+            self.content = m.get('content')
+        if m.get('receiverUserIdList') is not None:
+            self.receiver_user_id_list = m.get('receiverUserIdList')
+        if m.get('remindType') is not None:
+            self.remind_type = m.get('remindType')
+        if m.get('robotCode') is not None:
+            self.robot_code = m.get('robotCode')
+        return self
+
+
+class RobotSendDingResponseBody(TeaModel):
+    def __init__(
+        self,
+        failed_list: Dict[str, Any] = None,
+        open_ding_id: str = None,
+    ):
+        self.failed_list = failed_list
+        self.open_ding_id = open_ding_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.failed_list is not None:
+            result['failedList'] = self.failed_list
+        if self.open_ding_id is not None:
+            result['openDingId'] = self.open_ding_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('failedList') is not None:
+            self.failed_list = m.get('failedList')
+        if m.get('openDingId') is not None:
+            self.open_ding_id = m.get('openDingId')
+        return self
+
+
+class RobotSendDingResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: RobotSendDingResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = RobotSendDingResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SendRobotDingMessageHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.23
+Version: 2.0.24
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.23/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.24/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.23/setup.py` & `alibabacloud_dingtalk-2.0.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 12/07/2023
+Created on 17/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_tea_util>=0.3.9, <1.0.0",
+    "alibabacloud_tea_util>=0.3.10, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0",
     "alibabacloud_gateway_spi>=0.0.1, <1.0.0",
     "alibabacloud_gateway_dingtalk>=1.0.2, <2.0.0"
 ]
 
 LONG_DESCRIPTION = ''
```

