# Comparing `tmp/ursactl-0.2.0.tar.gz` & `tmp/ursactl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jgsmith/Code/ursactl/dist/.tmp-daz7ybe8/ursactl-0.2.0.tar", last modified: Sun Jul 16 15:00:16 2023, max compression
+gzip compressed data, was "/Users/jgsmith/Code/ursactl/dist/.tmp-o1pbdmtf/ursactl-0.3.0.tar", last modified: Mon Jul 17 12:48:21 2023, max compression
```

## Comparing `ursactl-0.2.0.tar` & `ursactl-0.3.0.tar`

### file list

```diff
@@ -1,70 +1,73 @@
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/
--rw-r--r--   0 jgsmith    (501) staff       (20)       67 2023-01-01 19:09:45.000000 ursactl-0.2.0/CHANGELOG.md
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-01-01 19:09:45.000000 ursactl-0.2.0/LICENSE.md
--rw-r--r--   0 jgsmith    (501) staff       (20)      135 2023-01-01 19:09:45.000000 ursactl-0.2.0/MANIFEST.in
--rw-r--r--   0 jgsmith    (501) staff       (20)      994 2023-07-16 15:00:16.000000 ursactl-0.2.0/PKG-INFO
--rw-r--r--   0 jgsmith    (501) staff       (20)     1072 2023-02-14 14:26:01.000000 ursactl-0.2.0/README.md
--rw-r--r--   0 jgsmith    (501) staff       (20)       81 2023-01-01 19:09:45.000000 ursactl-0.2.0/pyproject.toml
--rw-r--r--   0 jgsmith    (501) staff       (20)      144 2023-07-08 17:43:40.000000 ursactl-0.2.0/requirements-dev.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-16 14:14:44.000000 ursactl-0.2.0/requirements.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)     1172 2023-07-16 15:00:16.000000 ursactl-0.2.0/setup.cfg
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/tests/
--rw-r--r--   0 jgsmith    (501) staff       (20)      382 2023-01-31 15:40:54.000000 ursactl-0.2.0/tests/test_ursactl.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.2.0/ursactl/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/airflow_provider/
--rw-r--r--   0 jgsmith    (501) staff       (20)      431 2023-05-04 12:27:25.000000 ursactl-0.2.0/ursactl/airflow_provider/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     3787 2023-05-04 12:27:25.000000 ursactl-0.2.0/ursactl/airflow_provider/hooks.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/controllers/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.2.0/ursactl/controllers/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1089 2023-01-31 15:40:54.000000 ursactl-0.2.0/ursactl/controllers/base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     7879 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/controllers/create.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     3313 2023-06-04 21:29:27.000000 ursactl-0.2.0/ursactl/controllers/delete.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1150 2023-03-24 15:51:14.000000 ursactl-0.2.0/ursactl/controllers/get.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1647 2023-07-05 18:27:53.000000 ursactl-0.2.0/ursactl/controllers/init.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     7280 2023-07-10 12:55:55.000000 ursactl-0.2.0/ursactl/controllers/list.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      446 2023-02-16 21:42:16.000000 ursactl-0.2.0/ursactl/controllers/refresh.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2293 2023-06-04 21:29:27.000000 ursactl-0.2.0/ursactl/controllers/run.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1944 2023-05-04 12:27:25.000000 ursactl-0.2.0/ursactl/controllers/send.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      762 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/controllers/show.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      764 2023-04-18 14:46:09.000000 ursactl-0.2.0/ursactl/controllers/stop.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     7698 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/controllers/sync.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     6031 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/controllers/update.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/controllers/utils/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-06-04 21:29:27.000000 ursactl-0.2.0/ursactl/controllers/utils/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     5403 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/controllers/utils/transforms.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/core/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.2.0/ursactl/core/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      543 2023-07-12 14:08:56.000000 ursactl-0.2.0/ursactl/core/_base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1682 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/core/agent.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2301 2023-07-05 18:27:53.000000 ursactl-0.2.0/ursactl/core/dataset.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      301 2023-04-18 14:46:09.000000 ursactl-0.2.0/ursactl/core/exc.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2727 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/core/project.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      865 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/core/running_agent.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/core/services/
--rw-r--r--   0 jgsmith    (501) staff       (20)      871 2023-05-04 12:27:25.000000 ursactl-0.2.0/ursactl/core/services/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1823 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/core/services/_base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)    31479 2023-07-10 12:55:55.000000 ursactl-0.2.0/ursactl/core/services/ape_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     8420 2023-04-21 15:03:51.000000 ursactl-0.2.0/ursactl/core/services/dss_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1916 2023-07-05 18:27:53.000000 ursactl-0.2.0/ursactl/core/services/iam_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)    11923 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/core/services/planning_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2910 2023-05-04 12:27:25.000000 ursactl-0.2.0/ursactl/core/services/project_client.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/core/utils/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-18 13:39:22.000000 ursactl-0.2.0/ursactl/core/utils/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1470 2023-04-18 14:46:09.000000 ursactl-0.2.0/ursactl/core/utils/magic.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      203 2023-07-16 14:59:58.000000 ursactl-0.2.0/ursactl/core/version.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/ext/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.2.0/ursactl/ext/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     4208 2023-07-05 18:27:53.000000 ursactl-0.2.0/ursactl/main.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/plugins/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.2.0/ursactl/plugins/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/templates/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.2.0/ursactl/templates/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl.egg-info/
--rw-r--r--   0 jgsmith    (501) staff       (20)      994 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl.egg-info/PKG-INFO
--rw-r--r--   0 jgsmith    (501) staff       (20)     1518 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl.egg-info/SOURCES.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl.egg-info/dependency_links.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)       46 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl.egg-info/entry_points.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl.egg-info/requires.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        8 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl.egg-info/top_level.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-02-17 20:26:57.000000 ursactl-0.2.0/ursactl.egg-info/zip-safe
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-17 12:48:21.000000 ursactl-0.3.0/
+-rw-r--r--   0 jgsmith    (501) staff       (20)       67 2023-01-01 19:09:45.000000 ursactl-0.3.0/CHANGELOG.md
+-rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-01-01 19:09:45.000000 ursactl-0.3.0/LICENSE.md
+-rw-r--r--   0 jgsmith    (501) staff       (20)      135 2023-01-01 19:09:45.000000 ursactl-0.3.0/MANIFEST.in
+-rw-r--r--   0 jgsmith    (501) staff       (20)      994 2023-07-17 12:48:21.000000 ursactl-0.3.0/PKG-INFO
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1072 2023-02-14 14:26:01.000000 ursactl-0.3.0/README.md
+-rw-r--r--   0 jgsmith    (501) staff       (20)       81 2023-01-01 19:09:45.000000 ursactl-0.3.0/pyproject.toml
+-rw-r--r--   0 jgsmith    (501) staff       (20)      144 2023-07-08 17:43:40.000000 ursactl-0.3.0/requirements-dev.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-16 14:14:44.000000 ursactl-0.3.0/requirements.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1172 2023-07-17 12:48:21.000000 ursactl-0.3.0/setup.cfg
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-17 12:48:21.000000 ursactl-0.3.0/tests/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      382 2023-01-31 15:40:54.000000 ursactl-0.3.0/tests/test_ursactl.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-17 12:48:21.000000 ursactl-0.3.0/ursactl/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.3.0/ursactl/__init__.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-17 12:48:21.000000 ursactl-0.3.0/ursactl/airflow_provider/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      431 2023-05-04 12:27:25.000000 ursactl-0.3.0/ursactl/airflow_provider/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     3787 2023-05-04 12:27:25.000000 ursactl-0.3.0/ursactl/airflow_provider/hooks.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-17 12:48:21.000000 ursactl-0.3.0/ursactl/controllers/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.3.0/ursactl/controllers/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1089 2023-01-31 15:40:54.000000 ursactl-0.3.0/ursactl/controllers/base.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     7879 2023-07-16 14:14:44.000000 ursactl-0.3.0/ursactl/controllers/create.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     3313 2023-06-04 21:29:27.000000 ursactl-0.3.0/ursactl/controllers/delete.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1150 2023-03-24 15:51:14.000000 ursactl-0.3.0/ursactl/controllers/get.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1647 2023-07-05 18:27:53.000000 ursactl-0.3.0/ursactl/controllers/init.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     7280 2023-07-10 12:55:55.000000 ursactl-0.3.0/ursactl/controllers/list.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      446 2023-02-16 21:42:16.000000 ursactl-0.3.0/ursactl/controllers/refresh.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2293 2023-06-04 21:29:27.000000 ursactl-0.3.0/ursactl/controllers/run.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1944 2023-05-04 12:27:25.000000 ursactl-0.3.0/ursactl/controllers/send.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      762 2023-07-16 14:14:44.000000 ursactl-0.3.0/ursactl/controllers/show.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      764 2023-04-18 14:46:09.000000 ursactl-0.3.0/ursactl/controllers/stop.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     7698 2023-07-16 14:14:44.000000 ursactl-0.3.0/ursactl/controllers/sync.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     6031 2023-07-16 14:14:44.000000 ursactl-0.3.0/ursactl/controllers/update.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-17 12:48:21.000000 ursactl-0.3.0/ursactl/controllers/utils/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-06-04 21:29:27.000000 ursactl-0.3.0/ursactl/controllers/utils/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     5403 2023-07-16 14:14:44.000000 ursactl-0.3.0/ursactl/controllers/utils/transforms.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-17 12:48:21.000000 ursactl-0.3.0/ursactl/core/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.3.0/ursactl/core/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      640 2023-07-17 12:46:16.000000 ursactl-0.3.0/ursactl/core/_base.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1501 2023-07-17 12:46:16.000000 ursactl-0.3.0/ursactl/core/agent.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2323 2023-07-17 12:46:16.000000 ursactl-0.3.0/ursactl/core/dataset.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      301 2023-04-18 14:46:09.000000 ursactl-0.3.0/ursactl/core/exc.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2184 2023-07-17 12:46:16.000000 ursactl-0.3.0/ursactl/core/pipeline.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1414 2023-07-17 12:46:16.000000 ursactl-0.3.0/ursactl/core/pipeline_run.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1487 2023-07-17 12:46:16.000000 ursactl-0.3.0/ursactl/core/pipeline_sweep.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     3658 2023-07-17 12:46:16.000000 ursactl-0.3.0/ursactl/core/project.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      865 2023-07-16 14:14:44.000000 ursactl-0.3.0/ursactl/core/running_agent.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-17 12:48:21.000000 ursactl-0.3.0/ursactl/core/services/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      871 2023-05-04 12:27:25.000000 ursactl-0.3.0/ursactl/core/services/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1823 2023-07-16 20:42:41.000000 ursactl-0.3.0/ursactl/core/services/_base.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)    32447 2023-07-17 12:46:16.000000 ursactl-0.3.0/ursactl/core/services/ape_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     8454 2023-07-17 12:46:16.000000 ursactl-0.3.0/ursactl/core/services/dss_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1892 2023-07-17 12:46:16.000000 ursactl-0.3.0/ursactl/core/services/iam_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)    11923 2023-07-16 14:14:44.000000 ursactl-0.3.0/ursactl/core/services/planning_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2910 2023-05-04 12:27:25.000000 ursactl-0.3.0/ursactl/core/services/project_client.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-17 12:48:21.000000 ursactl-0.3.0/ursactl/core/utils/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-18 13:39:22.000000 ursactl-0.3.0/ursactl/core/utils/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1470 2023-04-18 14:46:09.000000 ursactl-0.3.0/ursactl/core/utils/magic.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      203 2023-07-17 12:48:05.000000 ursactl-0.3.0/ursactl/core/version.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-17 12:48:21.000000 ursactl-0.3.0/ursactl/ext/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.3.0/ursactl/ext/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     4208 2023-07-05 18:27:53.000000 ursactl-0.3.0/ursactl/main.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-17 12:48:21.000000 ursactl-0.3.0/ursactl/plugins/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.3.0/ursactl/plugins/__init__.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-17 12:48:21.000000 ursactl-0.3.0/ursactl/templates/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.3.0/ursactl/templates/__init__.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-17 12:48:21.000000 ursactl-0.3.0/ursactl.egg-info/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      994 2023-07-17 12:48:21.000000 ursactl-0.3.0/ursactl.egg-info/PKG-INFO
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1603 2023-07-17 12:48:21.000000 ursactl-0.3.0/ursactl.egg-info/SOURCES.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-07-17 12:48:21.000000 ursactl-0.3.0/ursactl.egg-info/dependency_links.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)       46 2023-07-17 12:48:21.000000 ursactl-0.3.0/ursactl.egg-info/entry_points.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-17 12:48:21.000000 ursactl-0.3.0/ursactl.egg-info/requires.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)        8 2023-07-17 12:48:21.000000 ursactl-0.3.0/ursactl.egg-info/top_level.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-02-17 20:26:57.000000 ursactl-0.3.0/ursactl.egg-info/zip-safe
```

### Comparing `ursactl-0.2.0/PKG-INFO` & `ursactl-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ursactl
-Version: 0.2.0
+Version: 0.3.0
 Summary: command line tool and library for intercting with ursafrontier.cloud
 Author: Ursa Frontier LLC
 Author-email: contact@ursafrontier.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ursactl-0.2.0/README.md` & `ursactl-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/setup.cfg` & `ursactl-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/airflow_provider/hooks.py` & `ursactl-0.3.0/ursactl/airflow_provider/hooks.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/controllers/base.py` & `ursactl-0.3.0/ursactl/controllers/base.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/controllers/create.py` & `ursactl-0.3.0/ursactl/controllers/create.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/controllers/delete.py` & `ursactl-0.3.0/ursactl/controllers/delete.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/controllers/get.py` & `ursactl-0.3.0/ursactl/controllers/get.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/controllers/init.py` & `ursactl-0.3.0/ursactl/controllers/init.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/controllers/list.py` & `ursactl-0.3.0/ursactl/controllers/list.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/controllers/run.py` & `ursactl-0.3.0/ursactl/controllers/run.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/controllers/send.py` & `ursactl-0.3.0/ursactl/controllers/send.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/controllers/show.py` & `ursactl-0.3.0/ursactl/controllers/show.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/controllers/stop.py` & `ursactl-0.3.0/ursactl/controllers/stop.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/controllers/sync.py` & `ursactl-0.3.0/ursactl/controllers/sync.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/controllers/update.py` & `ursactl-0.3.0/ursactl/controllers/update.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/controllers/utils/transforms.py` & `ursactl-0.3.0/ursactl/controllers/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/core/_base.py` & `ursactl-0.3.0/ursactl/core/_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 
 
 class Base:
     """
     Base class for OOP interface classes.
     """
-    def __init__(self, uuid=None, client=None, app=None, **kwargs):
+    def __init__(self, uuid=None, client=None, app=None, project=None, **kwargs):
         self._client = client
         self._app = app
         self._uuid = uuid
+        self.project = project
+
         if any(kwargs):
             self._cached_data = kwargs
+        else:
+            self._cached_data = None
 
     @property
     def app(self):
         if self._app is None:
             from ursactl.main import UrsaCtl
             self._app = UrsaCtl()
             self._app.reload()
```

### Comparing `ursactl-0.2.0/ursactl/core/agent.py` & `ursactl-0.3.0/ursactl/core/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,14 @@
     @property
     def client(self):
         if self._client is None:
             self._client = client('planning', self.app)
         return self._client
 
     @property
-    def project(self):
-        from ursactl.core.project import Project
-
-        return Project(self._data['project_uuid'], app=self.app)
-
-    @property
     def name(self):
         return self._data['name']
 
     @property
     def packages(self):
         return self._data['packages']
 
@@ -34,21 +28,21 @@
         return self._data['behaviors']
 
     def run(self, state=None, predicates=None):
         result = self.client.run_agent(
             self.uuid,
             initial_state=json.dumps(state),
             initial_predicates=json.dumps(predicates),
-            project_uuid=self._data['project_uuid']
+            project_uuid=self.project.uuid
         )
 
         if result['errors']:
             return None
         running_agent_id = result['result']['id']
-        return RunningAgent(uuid=running_agent_id, app=self.app, client=self.client, project_uuid=self._data["project_uuid"])
+        return RunningAgent(uuid=running_agent_id, app=self.app, client=self.client, project=self.project)
 
     @property
     def _data(self):
         if self._cached_data is None:
             if self.uuid is None:
                 self._cached_data = {
                     'name': None,
```

### Comparing `ursactl-0.2.0/ursactl/core/dataset.py` & `ursactl-0.3.0/ursactl/core/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from ursactl.core._base import Base
 
 
 class Dataset(Base):
     """
     Provides access to a dataset.
     """
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._content = None
+
     @property
     def client(self):
         if self._client is None:
             self._client = client('dss', self.app)
         return self._client
 
     def commit(self):
@@ -27,22 +31,16 @@
             if result['accepted']:
                 self._uuid = result['uuid']
                 return True
             return False
         return False
 
     @property
-    def project(self):
-        from ursactl.core.project import Project
-
-        return Project(self._data['projectUuid'], app=self.app)
-
-    @property
-    def name(self):
-        return self._data['name']
+    def path(self):
+        return self._data['path']
 
     @property
     def description(self):
         return self._data['description']
 
     @property
     def type(self):
@@ -71,19 +69,20 @@
         return self._data['updatedAt']
 
     @property
     def _data(self):
         if self._cached_data is None:
             if self.uuid is None:
                 self._cached_data = {
-                    'projectUuid': None,
-                    'name': None,
+                    'path': None,
                     'description': None,
                     'type': None,
                     'size': None,
                     'url': None,
                     'createdAt': None,
                     'updatedAt': None
                 }
             else:
                 self._cached_data = self.client.get_dataset_details(self.uuid)
+                self._cached_data['url'] = self.client.get_dataset_url(self.project.uuid, self.uuid)
+
         return self._cached_data
```

### Comparing `ursactl-0.2.0/ursactl/core/project.py` & `ursactl-0.3.0/ursactl/core/project.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,45 +40,72 @@
         """
         from ursactl.core.agent import Agent
 
         if self.uuid is None:
             return []
         planning_client = client('planning', self.app)
         return (
-            Agent(client=planning_client, app=self.app, project_uuid=self.uuid, **info)
+            Agent(client=planning_client, app=self.app, project=self, **info)
             for info in planning_client.list_agents(project_scope=self.uuid)
         )
 
     def agent(self, name):
         """
         Returns an agent with the given name.
         """
         planning_client = client('planning', self.app)
         info = planning_client.get_agent(name, project_uuid=self.uuid)
-        return self.Agent(uuid=info['id'], client=planning_client, app=self.app, **info)
+        return self.Agent(uuid=info['id'], project=self, client=planning_client, app=self.app, **info)
 
     def Dataset(self, *args, **kwargs):
         from ursactl.core.dataset import Dataset as DatasetClass
 
-        return DatasetClass(*args, project_uuid=self.uuid, **kwargs)
+        return DatasetClass(*args, project=self, app=self.app, **kwargs)
 
     def datasets(self):
         """
         Returns a generator listing all datasets belonging to the project.
         """
         from ursactl.core.dataset import Dataset
 
         if self.uuid is None:
             return []
         dss_client = client('dss', self.app)
         return (
-            Dataset(client=dss_client, app=self.app, project_uuid=self.uuid, **info)
+            Dataset(client=dss_client, app=self.app, project=self, **info)
             for info in dss_client.list_datasets(project_scope=self.uuid)
         )
 
+    def Pipeline(self, *args, **kwargs):
+        from ursactl.core.pipeline import Pipeline as PipelineClass
+
+        return PipelineClass(*args, project=self, **kwargs)
+
+    def pipelines(self):
+        """
+        Returns a generator listing all pipelines belonging to the project.
+        """
+        from ursactl.core.pipeline import Pipeline
+
+        if self.uuid is None:
+            return []
+        ape_client = client('ape', self.app)
+        return (
+            Pipeline(client=ape_client, app=self.app, project=self, **info)
+            for info in ape_client.list_pipelines(project_scope=self.uuid)
+        )
+
+    def pipeline(self, path):
+        """
+        Returns a pipeline with the given path.
+        """
+        ape_client = client('ape', self.app)
+        info = ape_client.get_pipeline(path=path, project_uuid=self.uuid)
+        return self.Pipeline(uuid=info['id'], client=ape_client, app=self.app, **info)
+
     @property
     def _data(self):
         if self._cached_data is None:
             if self.uuid is None:
                 self._cached_data = {
                     'name': None,
                     'description': None,
```

### Comparing `ursactl-0.2.0/ursactl/core/running_agent.py` & `ursactl-0.3.0/ursactl/core/running_agent.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/core/services/__init__.py` & `ursactl-0.3.0/ursactl/core/services/__init__.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/core/services/_base.py` & `ursactl-0.3.0/ursactl/core/services/_base.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/core/services/ape_client.py` & `ursactl-0.3.0/ursactl/core/services/ape_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -426,14 +426,40 @@
             jobStatus
             dataset { path }
         }
     }
 }
 """
 
+GET_PIPELINE_RUN = """\
+query get_pipeline_run($id: ID!) {
+    pipelineRun(id: $id) {
+        dataset { id }
+        jobStatus
+        provenance
+        parameters
+    }
+}
+"""
+
+GET_PIPELINE_SWEEP = """\
+query get_pipeline_sweep($id: ID!) {
+    pipelineSweep(id: $id) {
+        jobStatus
+        pipelineRuns {
+            id
+            dataset { id }
+            jobStatus
+            provenance
+            parameters
+        }
+    }
+}
+"""
+
 
 class ApeClient(Base):
     """
     Client providing access to the APE service.
     """
     def list_transforms(self, project_uuid=None):
         """
@@ -446,15 +472,14 @@
 
         return query_response['data']['project']['transforms']
 
     def get_transform(self, uuid=None, path=None, project_uuid=None):
         """
         Returns more detail about the transform.
         """
-        print(uuid, path, project_uuid)
         if uuid is not None:
             query_response = self.raw_query(query=GET_TRANSFORM_BY_ID_QUERY, variables={
                 'id': uuid
             })
 
             return query_response['data']['transform']
         elif path is not None and path.find(':') == -1 and project_uuid is not None:
@@ -940,14 +965,32 @@
             query_response = self.raw_query(query=GET_PIPELINE_BY_PATH_QUERY, variables={
                 'path': path,
                 'project_id': project_uuid
             })
             return query_response['data']['project']['pipelines'][0]
         return None
 
+    def get_pipeline_run(self, uuid):
+        """
+        Returns more detail about the pipeline run.
+        """
+        query_response = self.raw_query(query=GET_PIPELINE_RUN, variables={
+            'id': uuid
+        })
+        return query_response['data']['pipelineRun']
+
+    def get_pipeline_sweep(self, uuid):
+        """
+        Returns more detail about the pipeline sweep.
+        """
+        query_response = self.raw_query(query=GET_PIPELINE_SWEEP, variables={
+            'id': uuid
+        })
+        return query_response['data']['pipelineSweep']
+
     def list_pipeline_runs(self, pipeline_id=None, project_uuid=None):
         """
         List pipeline runs for a pipeline.
         """
         if pipeline_id is not None:
             if self.is_uuid(pipeline_id):
                 variables = {'id': pipeline_id}
```

### Comparing `ursactl-0.2.0/ursactl/core/services/dss_client.py` & `ursactl-0.3.0/ursactl/core/services/dss_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 DataStore Service client
 """
 
-import io
 import requests
 import urllib.parse
 
 from ursactl.core.exc import UrsaNotAuthorized
 
 from ._base import Base
 
@@ -18,15 +17,15 @@
 }
 """
 
 GET_DATASET_PATH_QUERY = """\
 query get_dataset($id: ID!) {
     dataset(id: $id) {
         path
-        project { id handleName }
+        project { id name user { handle } }
     }
 }
 """
 
 GET_DATASET_QUERY = """\
 query get_dataset($id: ID!) {
     dataset(id: $id) {
@@ -152,17 +151,18 @@
             variables = {
                 'id': dataset
             }
             query_response = self.raw_query(query=GET_DATASET_PATH_QUERY, variables=variables)
             if 'errors' in query_response:
                 return None
             path = query_response['data']['dataset']['path']
-            handle_name = query_response['data']['dataset']['project']['handleName']
-            # owner_handle = query_response['data']['dataset']['project']['user']['handle']
-            # project_name = query_response['data']['dataset']['project']['name']
+            # handle_name = query_response['data']['dataset']['project']['handleName']
+            owner_handle = query_response['data']['dataset']['project']['user']['handle']
+            project_name = query_response['data']['dataset']['project']['name']
+            handle_name = f"{owner_handle}/{project_name}"
             return f"{self.endpoint}api/dss/{urllib.parse.quote(handle_name)}/{urllib.parse.quote(path)}"
         else:
             return f"{self.endpoint}api/dss/{urllib.parse.quote(project_uuid)}/{urllib.parse.quote(dataset)}"
 
     def get_dataset_details(self, dataset_id, project_uuid=None):
         if self.is_uuid(dataset_id):
             variables = {
@@ -206,27 +206,26 @@
                     return self.download_dataset(url, local_path, reauthorize=False)
                 return False
             for chunk in r.iter_content(chunk_size=1024*1024):
                 fd.write(chunk)
         return True
 
     def download_dataset_content(self, url, reauthorize=True):
-        local = io.StringIO()
+        local = bytearray()
         r = requests.get(url, stream=True, headers={
                 "authorization": f"Bearer {self.iam_client.get_token()}"
             })
         if r.status_code >= 400:
             if reauthorize:
                 self.iam_client.clear_token()
                 return self.download_dataset_content(url, reauthorize=False)
             return False
         for chunk in r.iter_content(chunk_size=1024*1024):
-            local.write(chunk)
-        content = local.getvalue()
-        local.close()
+            local += chunk
+        content = local.decode('utf-8')
         return content
 
     def delete_dataset(self, dataset_id, project_uuid=None):
         if self.is_uuid(dataset_id):
             variables = {
                 'id': dataset_id
             }
```

### Comparing `ursactl-0.2.0/ursactl/core/services/iam_client.py` & `ursactl-0.3.0/ursactl/core/services/iam_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         if results:
             return results[0]['token']
 
         # otherwise, get a token, save it to tinydb, and then return it
         response = requests.get(
             f"{self.endpoint}api/token",
             auth=HTTPBasicAuth(api_key, api_secret))
-        print(response)
 
         if response.status_code != 200:
             return
 
         token = response.json()["token"]
         self.app.db.insert({'api_key': api_key, 'token': token})
         return token
```

### Comparing `ursactl-0.2.0/ursactl/core/services/planning_client.py` & `ursactl-0.3.0/ursactl/core/services/planning_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/core/services/project_client.py` & `ursactl-0.3.0/ursactl/core/services/project_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/core/utils/magic.py` & `ursactl-0.3.0/ursactl/core/utils/magic.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl/main.py` & `ursactl-0.3.0/ursactl/main.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.2.0/ursactl.egg-info/PKG-INFO` & `ursactl-0.3.0/ursactl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ursactl
-Version: 0.2.0
+Version: 0.3.0
 Summary: command line tool and library for intercting with ursafrontier.cloud
 Author: Ursa Frontier LLC
 Author-email: contact@ursafrontier.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ursactl-0.2.0/ursactl.egg-info/SOURCES.txt` & `ursactl-0.3.0/ursactl.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -35,14 +35,17 @@
 ursactl/controllers/utils/__init__.py
 ursactl/controllers/utils/transforms.py
 ursactl/core/__init__.py
 ursactl/core/_base.py
 ursactl/core/agent.py
 ursactl/core/dataset.py
 ursactl/core/exc.py
+ursactl/core/pipeline.py
+ursactl/core/pipeline_run.py
+ursactl/core/pipeline_sweep.py
 ursactl/core/project.py
 ursactl/core/running_agent.py
 ursactl/core/version.py
 ursactl/core/services/__init__.py
 ursactl/core/services/_base.py
 ursactl/core/services/ape_client.py
 ursactl/core/services/dss_client.py
```

