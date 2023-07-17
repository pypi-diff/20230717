# Comparing `tmp/python-coiote-2.3.0.tar.gz` & `tmp/python-coiote-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-coiote-2.3.0.tar", last modified: Wed Jun 28 14:11:29 2023, max compression
+gzip compressed data, was "python-coiote-2.4.0.tar", last modified: Mon Jul 17 12:54:34 2023, max compression
```

## Comparing `python-coiote-2.3.0.tar` & `python-coiote-2.4.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 michalgrabowski   (501) staff       (20)        0 2023-06-28 14:11:28.992536 python-coiote-2.3.0/
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     1064 2022-11-21 13:49:36.000000 python-coiote-2.3.0/LICENSE
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     3506 2023-06-28 14:11:28.992885 python-coiote-2.3.0/PKG-INFO
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     3107 2023-06-28 14:07:21.000000 python-coiote-2.3.0/README.md
--rw-r--r--   0 michalgrabowski   (501) staff       (20)       84 2022-11-21 13:49:36.000000 python-coiote-2.3.0/pyproject.toml
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      634 2023-06-28 14:11:28.999258 python-coiote-2.3.0/setup.cfg
-drwxr-xr-x   0 michalgrabowski   (501) staff       (20)        0 2023-06-28 14:11:28.911905 python-coiote-2.3.0/src/
-drwxr-xr-x   0 michalgrabowski   (501) staff       (20)        0 2023-06-28 14:11:28.918592 python-coiote-2.3.0/src/coiote/
--rw-r--r--   0 michalgrabowski   (501) staff       (20)        0 2022-11-21 13:49:36.000000 python-coiote-2.3.0/src/coiote/__init__.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     2650 2023-01-16 14:51:40.000000 python-coiote-2.3.0/src/coiote/auth.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     3637 2023-06-27 13:48:34.000000 python-coiote-2.3.0/src/coiote/client.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     2991 2022-11-28 13:40:10.000000 python-coiote-2.3.0/src/coiote/device_client.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     4910 2023-06-28 08:45:59.000000 python-coiote-2.3.0/src/coiote/utils.py
-drwxr-xr-x   0 michalgrabowski   (501) staff       (20)        0 2023-06-28 14:11:28.944130 python-coiote-2.3.0/src/coiote/v3/
--rw-r--r--   0 michalgrabowski   (501) staff       (20)        0 2022-11-21 13:49:36.000000 python-coiote-2.3.0/src/coiote/v3/__init__.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     1715 2022-12-01 11:38:08.000000 python-coiote-2.3.0/src/coiote/v3/assigned_device_properties.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      636 2022-12-01 10:28:34.000000 python-coiote-2.3.0/src/coiote/v3/aws_integration.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      557 2022-12-01 10:28:49.000000 python-coiote-2.3.0/src/coiote/v3/cert_auth.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      719 2022-12-01 11:42:16.000000 python-coiote-2.3.0/src/coiote/v3/data_model.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     3000 2023-06-28 13:29:01.000000 python-coiote-2.3.0/src/coiote/v3/device_events.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     3576 2023-02-23 22:49:53.000000 python-coiote-2.3.0/src/coiote/v3/device_monitoring.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     1032 2022-12-01 11:44:20.000000 python-coiote-2.3.0/src/coiote/v3/device_resources.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     1804 2022-12-01 12:22:39.000000 python-coiote-2.3.0/src/coiote/v3/device_tests.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     2634 2022-12-01 10:30:06.000000 python-coiote-2.3.0/src/coiote/v3/devices.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      683 2022-12-01 12:03:45.000000 python-coiote-2.3.0/src/coiote/v3/dialects.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     1378 2022-12-01 10:39:53.000000 python-coiote-2.3.0/src/coiote/v3/domains.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     3369 2022-12-01 10:42:06.000000 python-coiote-2.3.0/src/coiote/v3/extensions.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     1332 2022-12-01 10:42:38.000000 python-coiote-2.3.0/src/coiote/v3/groups.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      702 2022-12-01 10:42:53.000000 python-coiote-2.3.0/src/coiote/v3/lifecycle_management.py
-drwxr-xr-x   0 michalgrabowski   (501) staff       (20)        0 2023-06-28 14:11:28.981785 python-coiote-2.3.0/src/coiote/v3/model/
--rw-r--r--   0 michalgrabowski   (501) staff       (20)        0 2022-11-21 13:49:36.000000 python-coiote-2.3.0/src/coiote/v3/model/__init__.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      901 2022-11-25 10:05:01.000000 python-coiote-2.3.0/src/coiote/v3/model/assigned_device_properties.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      117 2022-11-23 15:40:45.000000 python-coiote-2.3.0/src/coiote/v3/model/aws_integration.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)       94 2022-11-23 16:04:00.000000 python-coiote-2.3.0/src/coiote/v3/model/cert_auth.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      168 2022-11-21 13:49:36.000000 python-coiote-2.3.0/src/coiote/v3/model/data_model.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     2253 2023-06-28 13:09:08.000000 python-coiote-2.3.0/src/coiote/v3/model/device_events.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      546 2022-11-24 14:28:00.000000 python-coiote-2.3.0/src/coiote/v3/model/device_monitoring.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     1759 2022-11-28 13:27:27.000000 python-coiote-2.3.0/src/coiote/v3/model/device_resources.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      458 2022-11-24 13:12:26.000000 python-coiote-2.3.0/src/coiote/v3/model/device_tests.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     2591 2022-11-28 13:52:30.000000 python-coiote-2.3.0/src/coiote/v3/model/devices.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)       81 2022-11-23 14:06:11.000000 python-coiote-2.3.0/src/coiote/v3/model/dialects.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      213 2022-11-21 14:18:19.000000 python-coiote-2.3.0/src/coiote/v3/model/domains.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      614 2022-11-24 14:04:54.000000 python-coiote-2.3.0/src/coiote/v3/model/extensions.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      208 2022-11-25 09:08:50.000000 python-coiote-2.3.0/src/coiote/v3/model/groups.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      114 2022-11-23 15:19:01.000000 python-coiote-2.3.0/src/coiote/v3/model/lifecycle_management.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      840 2022-11-25 11:08:18.000000 python-coiote-2.3.0/src/coiote/v3/model/observations.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     1616 2022-11-28 13:57:29.000000 python-coiote-2.3.0/src/coiote/v3/model/resources.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      195 2022-11-23 13:38:55.000000 python-coiote-2.3.0/src/coiote/v3/model/setting_values.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      706 2022-11-22 11:48:03.000000 python-coiote-2.3.0/src/coiote/v3/model/task_reports.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      367 2022-11-21 13:49:36.000000 python-coiote-2.3.0/src/coiote/v3/model/task_templates.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     1588 2022-11-28 13:27:31.000000 python-coiote-2.3.0/src/coiote/v3/model/tasks.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     1085 2022-11-22 11:19:31.000000 python-coiote-2.3.0/src/coiote/v3/model/users.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     2340 2022-12-01 10:43:35.000000 python-coiote-2.3.0/src/coiote/v3/observations.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     1393 2022-12-01 10:44:07.000000 python-coiote-2.3.0/src/coiote/v3/resources.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)      673 2022-12-01 10:44:17.000000 python-coiote-2.3.0/src/coiote/v3/sessions.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     1313 2022-12-01 10:44:59.000000 python-coiote-2.3.0/src/coiote/v3/setting_values.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     2262 2022-12-01 10:45:40.000000 python-coiote-2.3.0/src/coiote/v3/task_reports.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     1259 2022-12-01 10:46:10.000000 python-coiote-2.3.0/src/coiote/v3/task_templates.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     3384 2022-12-01 10:47:03.000000 python-coiote-2.3.0/src/coiote/v3/tasks.py
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     1733 2022-12-01 10:47:49.000000 python-coiote-2.3.0/src/coiote/v3/users.py
-drwxr-xr-x   0 michalgrabowski   (501) staff       (20)        0 2023-06-28 14:11:28.991872 python-coiote-2.3.0/src/python_coiote.egg-info/
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     3506 2023-06-28 14:11:28.000000 python-coiote-2.3.0/src/python_coiote.egg-info/PKG-INFO
--rw-r--r--   0 michalgrabowski   (501) staff       (20)     1817 2023-06-28 14:11:28.000000 python-coiote-2.3.0/src/python_coiote.egg-info/SOURCES.txt
--rw-r--r--   0 michalgrabowski   (501) staff       (20)        1 2023-06-28 14:11:28.000000 python-coiote-2.3.0/src/python_coiote.egg-info/dependency_links.txt
--rw-r--r--   0 michalgrabowski   (501) staff       (20)       85 2023-06-28 14:11:28.000000 python-coiote-2.3.0/src/python_coiote.egg-info/requires.txt
--rw-r--r--   0 michalgrabowski   (501) staff       (20)        7 2023-06-28 14:11:28.000000 python-coiote-2.3.0/src/python_coiote.egg-info/top_level.txt
+drwxr-xr-x   0 michalgrabowski   (501) staff       (20)        0 2023-07-17 12:54:34.645228 python-coiote-2.4.0/
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     1064 2022-11-21 13:49:36.000000 python-coiote-2.4.0/LICENSE
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     3506 2023-07-17 12:54:34.645410 python-coiote-2.4.0/PKG-INFO
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     3107 2023-06-28 14:07:21.000000 python-coiote-2.4.0/README.md
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)       84 2022-11-21 13:49:36.000000 python-coiote-2.4.0/pyproject.toml
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      634 2023-07-17 12:54:34.646503 python-coiote-2.4.0/setup.cfg
+drwxr-xr-x   0 michalgrabowski   (501) staff       (20)        0 2023-07-17 12:54:34.560272 python-coiote-2.4.0/src/
+drwxr-xr-x   0 michalgrabowski   (501) staff       (20)        0 2023-07-17 12:54:34.578134 python-coiote-2.4.0/src/coiote/
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)        0 2022-11-21 13:49:36.000000 python-coiote-2.4.0/src/coiote/__init__.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     2650 2023-01-16 14:51:40.000000 python-coiote-2.4.0/src/coiote/auth.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     3637 2023-06-27 13:48:34.000000 python-coiote-2.4.0/src/coiote/client.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     2991 2022-11-28 13:40:10.000000 python-coiote-2.4.0/src/coiote/device_client.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     4910 2023-06-28 08:45:59.000000 python-coiote-2.4.0/src/coiote/utils.py
+drwxr-xr-x   0 michalgrabowski   (501) staff       (20)        0 2023-07-17 12:54:34.602549 python-coiote-2.4.0/src/coiote/v3/
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)        0 2022-11-21 13:49:36.000000 python-coiote-2.4.0/src/coiote/v3/__init__.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     1715 2022-12-01 11:38:08.000000 python-coiote-2.4.0/src/coiote/v3/assigned_device_properties.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      636 2022-12-01 10:28:34.000000 python-coiote-2.4.0/src/coiote/v3/aws_integration.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      557 2022-12-01 10:28:49.000000 python-coiote-2.4.0/src/coiote/v3/cert_auth.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      719 2022-12-01 11:42:16.000000 python-coiote-2.4.0/src/coiote/v3/data_model.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     4113 2023-07-17 12:40:41.000000 python-coiote-2.4.0/src/coiote/v3/device_events.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     3576 2023-02-23 22:49:53.000000 python-coiote-2.4.0/src/coiote/v3/device_monitoring.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     1032 2022-12-01 11:44:20.000000 python-coiote-2.4.0/src/coiote/v3/device_resources.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     1804 2022-12-01 12:22:39.000000 python-coiote-2.4.0/src/coiote/v3/device_tests.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     2634 2022-12-01 10:30:06.000000 python-coiote-2.4.0/src/coiote/v3/devices.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      683 2022-12-01 12:03:45.000000 python-coiote-2.4.0/src/coiote/v3/dialects.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     1378 2022-12-01 10:39:53.000000 python-coiote-2.4.0/src/coiote/v3/domains.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     3369 2022-12-01 10:42:06.000000 python-coiote-2.4.0/src/coiote/v3/extensions.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     1332 2022-12-01 10:42:38.000000 python-coiote-2.4.0/src/coiote/v3/groups.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      702 2022-12-01 10:42:53.000000 python-coiote-2.4.0/src/coiote/v3/lifecycle_management.py
+drwxr-xr-x   0 michalgrabowski   (501) staff       (20)        0 2023-07-17 12:54:34.641425 python-coiote-2.4.0/src/coiote/v3/model/
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)        0 2022-11-21 13:49:36.000000 python-coiote-2.4.0/src/coiote/v3/model/__init__.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      901 2022-11-25 10:05:01.000000 python-coiote-2.4.0/src/coiote/v3/model/assigned_device_properties.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      117 2022-11-23 15:40:45.000000 python-coiote-2.4.0/src/coiote/v3/model/aws_integration.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)       94 2022-11-23 16:04:00.000000 python-coiote-2.4.0/src/coiote/v3/model/cert_auth.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      168 2022-11-21 13:49:36.000000 python-coiote-2.4.0/src/coiote/v3/model/data_model.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     2591 2023-07-17 12:17:38.000000 python-coiote-2.4.0/src/coiote/v3/model/device_events.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      546 2022-11-24 14:28:00.000000 python-coiote-2.4.0/src/coiote/v3/model/device_monitoring.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     1759 2022-11-28 13:27:27.000000 python-coiote-2.4.0/src/coiote/v3/model/device_resources.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      458 2022-11-24 13:12:26.000000 python-coiote-2.4.0/src/coiote/v3/model/device_tests.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     2591 2022-11-28 13:52:30.000000 python-coiote-2.4.0/src/coiote/v3/model/devices.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)       81 2022-11-23 14:06:11.000000 python-coiote-2.4.0/src/coiote/v3/model/dialects.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      213 2022-11-21 14:18:19.000000 python-coiote-2.4.0/src/coiote/v3/model/domains.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      614 2022-11-24 14:04:54.000000 python-coiote-2.4.0/src/coiote/v3/model/extensions.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      208 2022-11-25 09:08:50.000000 python-coiote-2.4.0/src/coiote/v3/model/groups.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      114 2022-11-23 15:19:01.000000 python-coiote-2.4.0/src/coiote/v3/model/lifecycle_management.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      840 2022-11-25 11:08:18.000000 python-coiote-2.4.0/src/coiote/v3/model/observations.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     1616 2022-11-28 13:57:29.000000 python-coiote-2.4.0/src/coiote/v3/model/resources.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      195 2022-11-23 13:38:55.000000 python-coiote-2.4.0/src/coiote/v3/model/setting_values.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      706 2022-11-22 11:48:03.000000 python-coiote-2.4.0/src/coiote/v3/model/task_reports.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      367 2022-11-21 13:49:36.000000 python-coiote-2.4.0/src/coiote/v3/model/task_templates.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     1588 2022-11-28 13:27:31.000000 python-coiote-2.4.0/src/coiote/v3/model/tasks.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     1085 2022-11-22 11:19:31.000000 python-coiote-2.4.0/src/coiote/v3/model/users.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     2340 2022-12-01 10:43:35.000000 python-coiote-2.4.0/src/coiote/v3/observations.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     1393 2022-12-01 10:44:07.000000 python-coiote-2.4.0/src/coiote/v3/resources.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)      673 2022-12-01 10:44:17.000000 python-coiote-2.4.0/src/coiote/v3/sessions.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     1313 2022-12-01 10:44:59.000000 python-coiote-2.4.0/src/coiote/v3/setting_values.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     2262 2022-12-01 10:45:40.000000 python-coiote-2.4.0/src/coiote/v3/task_reports.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     1259 2022-12-01 10:46:10.000000 python-coiote-2.4.0/src/coiote/v3/task_templates.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     3384 2022-12-01 10:47:03.000000 python-coiote-2.4.0/src/coiote/v3/tasks.py
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     1733 2022-12-01 10:47:49.000000 python-coiote-2.4.0/src/coiote/v3/users.py
+drwxr-xr-x   0 michalgrabowski   (501) staff       (20)        0 2023-07-17 12:54:34.644849 python-coiote-2.4.0/src/python_coiote.egg-info/
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     3506 2023-07-17 12:54:34.000000 python-coiote-2.4.0/src/python_coiote.egg-info/PKG-INFO
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)     1817 2023-07-17 12:54:34.000000 python-coiote-2.4.0/src/python_coiote.egg-info/SOURCES.txt
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)        1 2023-07-17 12:54:34.000000 python-coiote-2.4.0/src/python_coiote.egg-info/dependency_links.txt
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)       85 2023-07-17 12:54:34.000000 python-coiote-2.4.0/src/python_coiote.egg-info/requires.txt
+-rw-r--r--   0 michalgrabowski   (501) staff       (20)        7 2023-07-17 12:54:34.000000 python-coiote-2.4.0/src/python_coiote.egg-info/top_level.txt
```

### Comparing `python-coiote-2.3.0/LICENSE` & `python-coiote-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/PKG-INFO` & `python-coiote-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-coiote
-Version: 2.3.0
+Version: 2.4.0
 Summary: Interact with Coiote DM API
 Maintainer: Michał Grabowski
 Maintainer-email: m.grabowski@avsystem.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `python-coiote-2.3.0/README.md` & `python-coiote-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/setup.cfg` & `python-coiote-2.4.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-coiote
-version = 2.3.0
+version = 2.4.0
 maintainer = Michał Grabowski
 maintainer_email = m.grabowski@avsystem.com
 description = Interact with Coiote DM API
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `python-coiote-2.3.0/src/coiote/auth.py` & `python-coiote-2.4.0/src/coiote/auth.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/client.py` & `python-coiote-2.4.0/src/coiote/client.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/device_client.py` & `python-coiote-2.4.0/src/coiote/device_client.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/utils.py` & `python-coiote-2.4.0/src/coiote/utils.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/assigned_device_properties.py` & `python-coiote-2.4.0/src/coiote/v3/assigned_device_properties.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/aws_integration.py` & `python-coiote-2.4.0/src/coiote/v3/aws_integration.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/cert_auth.py` & `python-coiote-2.4.0/src/coiote/v3/cert_auth.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/data_model.py` & `python-coiote-2.4.0/src/coiote/v3/data_model.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/device_events.py` & `python-coiote-2.4.0/src/coiote/v3/device_events.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,23 +30,44 @@
         if handler_type == HandlerType.Kafka:
             return self.session.put(self.get_url(f"/kafka/{id}"), json=asdict(update_data))
         else:
             return self.session.put(self.get_url(f"/webhook/{id}"), json=asdict(update_data))
 
     @api_call(HandlerTestResult)
     def test_handler(self, id: str):
-        return self.session.post(self.get_url(f"/test/{id}"))
+        return self.session.post(self.get_url(f"/test/existing/{id}"))
+
+    @api_call(HandlerTestResult)
+    def test_handler(self, id: Optional[str] = None, handler_data: Optional[EventHandlerConfiguration] = None):
+        if id is None and handler_data is None:
+            raise ValueError(
+                "To test a handler, you must provide either an ID for a handler that already exists, or entire configuration for a fresh one")
+        if id is not None:
+            return self.session.post(self.get_url(f"/test/existing/{id}"))
+        elif handler_data is not None:
+            return self.__test_new_handler(handler_data)
+
+    def __test_new_handler(self, handler_data: EventHandlerConfiguration):
+        domain = handler_data.domain
+        if domain:
+            domain_params = {"domain": domain}
+        else:
+            domain_params = {}
+        if handler_data.type == HandlerType.Kafka:
+            return self.session.post(self.get_url(f"/test/kafka"), json=asdict(handler_data), params=domain_params)
+        else:
+            return self.session.post(self.get_url(f"/test/webhook"), json=asdict(handler_data), params=domain_params)
 
     @api_call(str)
     def create_handler(self, create_data: EventHandlerConfiguration):
         domain = create_data.domain
         if domain:
             domain_params = {"domain": domain}
         else:
-            {}
+            domain_params = {}
         if create_data.type == HandlerType.Kafka:
             return self.session.post(self.get_url(f"/kafka"), json=asdict(create_data), params=domain_params)
         else:
             return self.session.post(self.get_url(f"/webhook"), json=asdict(create_data), params=domain_params)
 
     def create_influx_handler(self,
                               name: str,
```

### Comparing `python-coiote-2.3.0/src/coiote/v3/device_monitoring.py` & `python-coiote-2.4.0/src/coiote/v3/device_monitoring.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/device_resources.py` & `python-coiote-2.4.0/src/coiote/v3/device_resources.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/device_tests.py` & `python-coiote-2.4.0/src/coiote/v3/device_tests.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/devices.py` & `python-coiote-2.4.0/src/coiote/v3/devices.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/dialects.py` & `python-coiote-2.4.0/src/coiote/v3/dialects.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/domains.py` & `python-coiote-2.4.0/src/coiote/v3/domains.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/extensions.py` & `python-coiote-2.4.0/src/coiote/v3/extensions.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/groups.py` & `python-coiote-2.4.0/src/coiote/v3/groups.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/lifecycle_management.py` & `python-coiote-2.4.0/src/coiote/v3/lifecycle_management.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/model/assigned_device_properties.py` & `python-coiote-2.4.0/src/coiote/v3/model/assigned_device_properties.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/model/device_events.py` & `python-coiote-2.4.0/src/coiote/v3/model/device_events.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,56 +55,65 @@
     type: str = "token"
 
 
 WebhookAuth = Union[BasicAuth, Token]
 
 
 class WebhookFormat(str, AutoNamedEnum):
-    Raw = "raw"
+    Generic = "generic"
     InfluxDb = "influxDb"
 
 
+class WebhookMethod(str, AutoNamedEnum):
+    Post = "post"
+    Put = "put"
+    Patch = "patch"
+
+
 @dataclass
 class WebhookConnectionConfig:
     uri: str
     auth: Optional[WebhookAuth] = None
     additionalHeaders: Dict[str, str] = field(default_factory=dict)
     format: Optional[WebhookFormat] = None
+    method: Optional[WebhookMethod] = WebhookMethod.Post
 
 
 @dataclass
 class KafkaFromPropertiesConnectionConfig:
     topic: str
+    headers: Dict[str, str] = field(default_factory=dict)
     type: str = "domainProperty"
 
 
 @dataclass
-class RawKafkaConnectionConfig:
+class CustomKafkaConnectionConfig:
     value: str
     topic: str
-    type: str = "raw"
+    headers: Dict[str, str] = field(default_factory=dict)
+    type: str = "custom"
 
 
 KafkaConnectionConfig = Union[KafkaFromPropertiesConnectionConfig,
-                              RawKafkaConnectionConfig]
+                              CustomKafkaConnectionConfig]
 
 
 @dataclass
 class EventHandlerConfiguration:
     type: HandlerType
     name: str
     enabled: bool
     filter: EventHandlerFilter
     connectionConfig: Union[WebhookConnectionConfig, KafkaConnectionConfig]
-    domain: str
-    description: str
+    domain: Optional[str] = None
+    description: Optional[str] = None
 
 
 @dataclass
 class EventHandler(EventHandlerConfiguration):
-    id: str
+    id: Optional[str] = None
 
 
 @dataclass
 class HandlerTestResult:
     successful: bool
     message: Optional[str] = None
```

### Comparing `python-coiote-2.3.0/src/coiote/v3/model/device_monitoring.py` & `python-coiote-2.4.0/src/coiote/v3/model/device_monitoring.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/model/device_resources.py` & `python-coiote-2.4.0/src/coiote/v3/model/device_resources.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/model/devices.py` & `python-coiote-2.4.0/src/coiote/v3/model/devices.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/model/extensions.py` & `python-coiote-2.4.0/src/coiote/v3/model/extensions.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/model/observations.py` & `python-coiote-2.4.0/src/coiote/v3/model/observations.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/model/resources.py` & `python-coiote-2.4.0/src/coiote/v3/model/resources.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/model/task_reports.py` & `python-coiote-2.4.0/src/coiote/v3/model/task_reports.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/model/tasks.py` & `python-coiote-2.4.0/src/coiote/v3/model/tasks.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/model/users.py` & `python-coiote-2.4.0/src/coiote/v3/model/users.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/observations.py` & `python-coiote-2.4.0/src/coiote/v3/observations.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/resources.py` & `python-coiote-2.4.0/src/coiote/v3/resources.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/sessions.py` & `python-coiote-2.4.0/src/coiote/v3/sessions.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/setting_values.py` & `python-coiote-2.4.0/src/coiote/v3/setting_values.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/task_reports.py` & `python-coiote-2.4.0/src/coiote/v3/task_reports.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/task_templates.py` & `python-coiote-2.4.0/src/coiote/v3/task_templates.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/tasks.py` & `python-coiote-2.4.0/src/coiote/v3/tasks.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/coiote/v3/users.py` & `python-coiote-2.4.0/src/coiote/v3/users.py`

 * *Files identical despite different names*

### Comparing `python-coiote-2.3.0/src/python_coiote.egg-info/PKG-INFO` & `python-coiote-2.4.0/src/python_coiote.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-coiote
-Version: 2.3.0
+Version: 2.4.0
 Summary: Interact with Coiote DM API
 Maintainer: Michał Grabowski
 Maintainer-email: m.grabowski@avsystem.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `python-coiote-2.3.0/src/python_coiote.egg-info/SOURCES.txt` & `python-coiote-2.4.0/src/python_coiote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

