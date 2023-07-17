# Comparing `tmp/spaceone-dashboard-1.12.dev7.tar.gz` & `tmp/spaceone-dashboard-1.12.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaceone-dashboard-1.12.dev7.tar", last modified: Mon Jul  3 10:19:02 2023, max compression
+gzip compressed data, was "spaceone-dashboard-1.12.dev8.tar", last modified: Mon Jul 17 06:07:17 2023, max compression
```

## Comparing `spaceone-dashboard-1.12.dev7.tar` & `spaceone-dashboard-1.12.dev8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:19:02.826405 spaceone-dashboard-1.12.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-03 10:19:02.826405 spaceone-dashboard-1.12.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 10:19:02.826405 spaceone-dashboard-1.12.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:19:02.818405 spaceone-dashboard-1.12.dev7/spaceone/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:19:02.822405 spaceone-dashboard-1.12.dev7/spaceone/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:19:02.822405 spaceone-dashboard-1.12.dev7/spaceone/dashboard/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/conf/global_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/conf/proto_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:19:02.822405 spaceone-dashboard-1.12.dev7/spaceone/dashboard/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:19:02.822405 spaceone-dashboard-1.12.dev7/spaceone/dashboard/error/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/error/common_dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:19:02.822405 spaceone-dashboard-1.12.dev7/spaceone/dashboard/info/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/info/common_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/info/custom_widget_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/info/domain_dashboard_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/info/domain_dashboard_version_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/info/project_dashboard_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/info/project_dashboard_version_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:19:02.822405 spaceone-dashboard-1.12.dev7/spaceone/dashboard/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:19:02.822405 spaceone-dashboard-1.12.dev7/spaceone/dashboard/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/interface/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:19:02.822405 spaceone-dashboard-1.12.dev7/spaceone/dashboard/interface/grpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/interface/grpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/interface/grpc/v1/custom_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/interface/grpc/v1/domain_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/interface/grpc/v1/project_dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:19:02.822405 spaceone-dashboard-1.12.dev7/spaceone/dashboard/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:19:02.826405 spaceone-dashboard-1.12.dev7/spaceone/dashboard/manager/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/manager/custom_widget_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/manager/domain_dashboard_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/manager/domain_dashboard_version_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/manager/project_dashboard_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/manager/project_dashboard_version_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:19:02.826405 spaceone-dashboard-1.12.dev7/spaceone/dashboard/model/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/model/custom_widget_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/model/domain_dashboard_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/model/domain_dashboard_version_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/model/project_dashboard_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/model/project_dashboard_version_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:19:02.826405 spaceone-dashboard-1.12.dev7/spaceone/dashboard/service/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/service/custom_widget_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/service/domain_dashboard_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-07-03 10:18:51.000000 spaceone-dashboard-1.12.dev7/spaceone/dashboard/service/project_dashboard_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:19:02.826405 spaceone-dashboard-1.12.dev7/spaceone_dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-03 10:19:02.000000 spaceone-dashboard-1.12.dev7/spaceone_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-03 10:19:02.000000 spaceone-dashboard-1.12.dev7/spaceone_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:19:02.000000 spaceone-dashboard-1.12.dev7/spaceone_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:19:02.000000 spaceone-dashboard-1.12.dev7/spaceone_dashboard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-03 10:19:02.000000 spaceone-dashboard-1.12.dev7/spaceone_dashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 10:19:02.000000 spaceone-dashboard-1.12.dev7/spaceone_dashboard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:17.957476 spaceone-dashboard-1.12.dev8/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-17 06:07:17.957476 spaceone-dashboard-1.12.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 06:07:17.957476 spaceone-dashboard-1.12.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:17.949476 spaceone-dashboard-1.12.dev8/spaceone/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:17.949476 spaceone-dashboard-1.12.dev8/spaceone/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:17.949476 spaceone-dashboard-1.12.dev8/spaceone/dashboard/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/conf/global_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/conf/proto_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:17.949476 spaceone-dashboard-1.12.dev8/spaceone/dashboard/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:17.949476 spaceone-dashboard-1.12.dev8/spaceone/dashboard/error/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/error/common_dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:17.949476 spaceone-dashboard-1.12.dev8/spaceone/dashboard/info/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/info/common_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/info/custom_widget_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/info/domain_dashboard_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/info/domain_dashboard_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/info/project_dashboard_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/info/project_dashboard_version_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:17.949476 spaceone-dashboard-1.12.dev8/spaceone/dashboard/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:17.949476 spaceone-dashboard-1.12.dev8/spaceone/dashboard/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/interface/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:17.953476 spaceone-dashboard-1.12.dev8/spaceone/dashboard/interface/grpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/interface/grpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/interface/grpc/v1/custom_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/interface/grpc/v1/domain_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/interface/grpc/v1/project_dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:17.953476 spaceone-dashboard-1.12.dev8/spaceone/dashboard/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:17.953476 spaceone-dashboard-1.12.dev8/spaceone/dashboard/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/manager/custom_widget_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/manager/domain_dashboard_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/manager/domain_dashboard_version_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/manager/project_dashboard_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/manager/project_dashboard_version_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:17.953476 spaceone-dashboard-1.12.dev8/spaceone/dashboard/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/model/custom_widget_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/model/domain_dashboard_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/model/domain_dashboard_version_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/model/project_dashboard_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/model/project_dashboard_version_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:17.953476 spaceone-dashboard-1.12.dev8/spaceone/dashboard/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/service/custom_widget_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/service/domain_dashboard_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-07-17 06:07:06.000000 spaceone-dashboard-1.12.dev8/spaceone/dashboard/service/project_dashboard_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:07:17.957476 spaceone-dashboard-1.12.dev8/spaceone_dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-17 06:07:17.000000 spaceone-dashboard-1.12.dev8/spaceone_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-17 06:07:17.000000 spaceone-dashboard-1.12.dev8/spaceone_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 06:07:17.000000 spaceone-dashboard-1.12.dev8/spaceone_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 06:07:17.000000 spaceone-dashboard-1.12.dev8/spaceone_dashboard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 06:07:17.000000 spaceone-dashboard-1.12.dev8/spaceone_dashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 06:07:17.000000 spaceone-dashboard-1.12.dev8/spaceone_dashboard.egg-info/top_level.txt
```

### Comparing `spaceone-dashboard-1.12.dev7/setup.py` & `spaceone-dashboard-1.12.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/conf/global_conf.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/conf/global_conf.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/info/custom_widget_info.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/info/custom_widget_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/info/domain_dashboard_info.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/info/domain_dashboard_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/info/domain_dashboard_version_info.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/info/domain_dashboard_version_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/info/project_dashboard_info.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/info/project_dashboard_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/info/project_dashboard_version_info.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/info/project_dashboard_version_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/interface/grpc/v1/custom_widget.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/interface/grpc/v1/custom_widget.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/interface/grpc/v1/domain_dashboard.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/interface/grpc/v1/domain_dashboard.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/interface/grpc/v1/project_dashboard.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/interface/grpc/v1/project_dashboard.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/manager/custom_widget_manager.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/manager/custom_widget_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/manager/domain_dashboard_manager.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/manager/domain_dashboard_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/manager/domain_dashboard_version_manager.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/manager/domain_dashboard_version_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/manager/project_dashboard_manager.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/manager/project_dashboard_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/manager/project_dashboard_version_manager.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/manager/project_dashboard_version_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/model/custom_widget_model.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/model/custom_widget_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/model/domain_dashboard_model.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/model/domain_dashboard_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/model/domain_dashboard_version_model.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/model/domain_dashboard_version_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/model/project_dashboard_model.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/model/project_dashboard_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/model/project_dashboard_version_model.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/model/project_dashboard_version_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/service/custom_widget_service.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/service/custom_widget_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/service/domain_dashboard_service.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/service/domain_dashboard_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone/dashboard/service/project_dashboard_service.py` & `spaceone-dashboard-1.12.dev8/spaceone/dashboard/service/project_dashboard_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-dashboard-1.12.dev7/spaceone_dashboard.egg-info/SOURCES.txt` & `spaceone-dashboard-1.12.dev8/spaceone_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

