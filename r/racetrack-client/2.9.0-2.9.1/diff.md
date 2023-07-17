# Comparing `tmp/racetrack-client-2.9.0.tar.gz` & `tmp/racetrack-client-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "racetrack-client-2.9.0.tar", last modified: Tue Feb 14 13:17:35 2023, max compression
+gzip compressed data, was "racetrack-client-2.9.1.tar", last modified: Mon Feb 20 09:17:37 2023, max compression
```

## Comparing `racetrack-client-2.9.0.tar` & `racetrack-client-2.9.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-14 13:17:35.387178 racetrack-client-2.9.0/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    10757 2023-01-27 12:44:20.000000 racetrack-client-2.9.0/LICENSE
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3606 2023-02-14 13:17:35.387178 racetrack-client-2.9.0/PKG-INFO
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3058 2023-02-14 12:08:04.000000 racetrack-client-2.9.0/README.md
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-14 13:17:35.383178 racetrack-client-2.9.0/racetrack_client/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       48 2023-02-14 13:10:24.000000 racetrack-client-2.9.0/racetrack_client/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       78 2022-08-04 14:52:29.000000 racetrack-client-2.9.0/racetrack_client/__main__.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-14 13:17:35.383178 racetrack-client-2.9.0/racetrack_client/client/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-08-04 14:52:29.000000 racetrack-client-2.9.0/racetrack_client/client/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     7793 2023-02-14 12:08:04.000000 racetrack-client-2.9.0/racetrack_client/client/deploy.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2353 2022-11-02 10:40:46.000000 racetrack-client-2.9.0/racetrack_client/client/env.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3345 2023-02-14 12:08:04.000000 racetrack-client-2.9.0/racetrack_client/client/logs.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     4720 2023-02-14 12:08:04.000000 racetrack-client-2.9.0/racetrack_client/client/manage.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1302 2023-02-14 12:08:04.000000 racetrack-client-2.9.0/racetrack_client/client/move.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     5397 2023-02-14 12:08:04.000000 racetrack-client-2.9.0/racetrack_client/client/run.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2429 2023-02-14 12:08:04.000000 racetrack-client-2.9.0/racetrack_client/client/socketio.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-14 13:17:35.383178 racetrack-client-2.9.0/racetrack_client/client_config/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-08-04 14:52:29.000000 racetrack-client-2.9.0/racetrack_client/client_config/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2019 2023-01-26 14:12:39.000000 racetrack-client-2.9.0/racetrack_client/client_config/alias.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2070 2023-01-26 14:12:39.000000 racetrack-client-2.9.0/racetrack_client/client_config/auth.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      638 2022-12-20 10:18:06.000000 racetrack-client-2.9.0/racetrack_client/client_config/client_config.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1392 2022-11-29 13:17:16.000000 racetrack-client-2.9.0/racetrack_client/client_config/io.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2120 2023-01-26 14:12:39.000000 racetrack-client-2.9.0/racetrack_client/client_config/update.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-14 13:17:35.383178 racetrack-client-2.9.0/racetrack_client/log/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-08-04 14:52:29.000000 racetrack-client-2.9.0/racetrack_client/log/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1214 2022-12-20 10:18:06.000000 racetrack-client-2.9.0/racetrack_client/log/context_error.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       91 2022-08-04 14:52:29.000000 racetrack-client-2.9.0/racetrack_client/log/errors.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2058 2022-08-04 14:52:29.000000 racetrack-client-2.9.0/racetrack_client/log/exception.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2360 2022-11-02 10:40:46.000000 racetrack-client-2.9.0/racetrack_client/log/logs.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    10571 2023-02-14 12:08:04.000000 racetrack-client-2.9.0/racetrack_client/main.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-14 13:17:35.383178 racetrack-client-2.9.0/racetrack_client/manifest/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       31 2022-08-04 14:52:29.000000 racetrack-client-2.9.0/racetrack_client/manifest/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2642 2023-02-14 12:08:04.000000 racetrack-client-2.9.0/racetrack_client/manifest/load.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3503 2023-02-14 12:08:04.000000 racetrack-client-2.9.0/racetrack_client/manifest/manifest.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1831 2023-01-26 14:12:39.000000 racetrack-client-2.9.0/racetrack_client/manifest/merge.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1769 2023-02-14 12:08:04.000000 racetrack-client-2.9.0/racetrack_client/manifest/validate.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-14 13:17:35.383178 racetrack-client-2.9.0/racetrack_client/plugin/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-11-02 10:40:46.000000 racetrack-client-2.9.0/racetrack_client/plugin/__init__.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-14 13:17:35.383178 racetrack-client-2.9.0/racetrack_client/plugin/bundler/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-11-02 10:40:46.000000 racetrack-client-2.9.0/racetrack_client/plugin/bundler/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2982 2023-01-26 14:12:39.000000 racetrack-client-2.9.0/racetrack_client/plugin/bundler/bundle.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3019 2022-11-02 10:40:46.000000 racetrack-client-2.9.0/racetrack_client/plugin/bundler/filename_matcher.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     7420 2023-02-03 12:28:08.000000 racetrack-client-2.9.0/racetrack_client/plugin/install.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      523 2022-12-20 10:18:06.000000 racetrack-client-2.9.0/racetrack_client/plugin/plugin_manifest.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-14 13:17:35.387178 racetrack-client-2.9.0/racetrack_client/utils/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-08-04 14:52:29.000000 racetrack-client-2.9.0/racetrack_client/utils/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1172 2023-01-27 11:45:30.000000 racetrack-client-2.9.0/racetrack_client/utils/auth.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1182 2022-11-02 10:40:46.000000 racetrack-client-2.9.0/racetrack_client/utils/config.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2892 2022-12-20 10:18:06.000000 racetrack-client-2.9.0/racetrack_client/utils/datamodel.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2655 2022-11-02 10:40:46.000000 racetrack-client-2.9.0/racetrack_client/utils/quantity.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    11450 2023-01-30 11:10:05.000000 racetrack-client-2.9.0/racetrack_client/utils/request.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     5339 2022-11-02 10:40:46.000000 racetrack-client-2.9.0/racetrack_client/utils/semver.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     5824 2023-02-10 13:41:58.000000 racetrack-client-2.9.0/racetrack_client/utils/shell.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      744 2023-01-26 14:12:39.000000 racetrack-client-2.9.0/racetrack_client/utils/table.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2414 2023-01-26 14:12:39.000000 racetrack-client-2.9.0/racetrack_client/utils/time.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      657 2022-11-02 10:40:46.000000 racetrack-client-2.9.0/racetrack_client/utils/url.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-14 13:17:35.383178 racetrack-client-2.9.0/racetrack_client.egg-info/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3606 2023-02-14 13:17:35.000000 racetrack-client-2.9.0/racetrack_client.egg-info/PKG-INFO
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1827 2023-02-14 13:17:35.000000 racetrack-client-2.9.0/racetrack_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        1 2023-02-14 13:17:35.000000 racetrack-client-2.9.0/racetrack_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       57 2023-02-14 13:17:35.000000 racetrack-client-2.9.0/racetrack_client.egg-info/entry_points.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       82 2023-02-14 13:17:35.000000 racetrack-client-2.9.0/racetrack_client.egg-info/requires.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       17 2023-02-14 13:17:35.000000 racetrack-client-2.9.0/racetrack_client.egg-info/top_level.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2023-02-14 13:17:35.387178 racetrack-client-2.9.0/setup.cfg
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1126 2022-11-02 10:40:46.000000 racetrack-client-2.9.0/setup.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-20 09:17:37.275883 racetrack-client-2.9.1/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    10757 2023-01-27 12:44:20.000000 racetrack-client-2.9.1/LICENSE
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3606 2023-02-20 09:17:37.275883 racetrack-client-2.9.1/PKG-INFO
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3058 2023-02-14 12:08:04.000000 racetrack-client-2.9.1/README.md
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-20 09:17:37.091884 racetrack-client-2.9.1/racetrack_client/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       48 2023-02-20 09:14:06.000000 racetrack-client-2.9.1/racetrack_client/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       78 2022-08-04 14:52:29.000000 racetrack-client-2.9.1/racetrack_client/__main__.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-20 09:17:37.127884 racetrack-client-2.9.1/racetrack_client/client/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-08-04 14:52:29.000000 racetrack-client-2.9.1/racetrack_client/client/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     7793 2023-02-14 12:08:04.000000 racetrack-client-2.9.1/racetrack_client/client/deploy.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2353 2022-11-02 10:40:46.000000 racetrack-client-2.9.1/racetrack_client/client/env.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3345 2023-02-14 12:08:04.000000 racetrack-client-2.9.1/racetrack_client/client/logs.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     4720 2023-02-14 12:08:04.000000 racetrack-client-2.9.1/racetrack_client/client/manage.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1302 2023-02-14 12:08:04.000000 racetrack-client-2.9.1/racetrack_client/client/move.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     5397 2023-02-14 12:08:04.000000 racetrack-client-2.9.1/racetrack_client/client/run.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2429 2023-02-14 12:08:04.000000 racetrack-client-2.9.1/racetrack_client/client/socketio.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-20 09:17:37.155883 racetrack-client-2.9.1/racetrack_client/client_config/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-08-04 14:52:29.000000 racetrack-client-2.9.1/racetrack_client/client_config/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2019 2023-01-26 14:12:39.000000 racetrack-client-2.9.1/racetrack_client/client_config/alias.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2070 2023-01-26 14:12:39.000000 racetrack-client-2.9.1/racetrack_client/client_config/auth.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      638 2022-12-20 10:18:06.000000 racetrack-client-2.9.1/racetrack_client/client_config/client_config.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1392 2022-11-29 13:17:16.000000 racetrack-client-2.9.1/racetrack_client/client_config/io.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2120 2023-01-26 14:12:39.000000 racetrack-client-2.9.1/racetrack_client/client_config/update.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-20 09:17:37.175883 racetrack-client-2.9.1/racetrack_client/log/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-08-04 14:52:29.000000 racetrack-client-2.9.1/racetrack_client/log/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1214 2022-12-20 10:18:06.000000 racetrack-client-2.9.1/racetrack_client/log/context_error.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       91 2022-08-04 14:52:29.000000 racetrack-client-2.9.1/racetrack_client/log/errors.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2058 2022-08-04 14:52:29.000000 racetrack-client-2.9.1/racetrack_client/log/exception.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2360 2022-11-02 10:40:46.000000 racetrack-client-2.9.1/racetrack_client/log/logs.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    10571 2023-02-14 12:08:04.000000 racetrack-client-2.9.1/racetrack_client/main.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-20 09:17:37.199883 racetrack-client-2.9.1/racetrack_client/manifest/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       31 2022-08-04 14:52:29.000000 racetrack-client-2.9.1/racetrack_client/manifest/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2642 2023-02-14 12:08:04.000000 racetrack-client-2.9.1/racetrack_client/manifest/load.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3503 2023-02-14 12:08:04.000000 racetrack-client-2.9.1/racetrack_client/manifest/manifest.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1831 2023-01-26 14:12:39.000000 racetrack-client-2.9.1/racetrack_client/manifest/merge.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1769 2023-02-14 12:08:04.000000 racetrack-client-2.9.1/racetrack_client/manifest/validate.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-20 09:17:37.211883 racetrack-client-2.9.1/racetrack_client/plugin/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-11-02 10:40:46.000000 racetrack-client-2.9.1/racetrack_client/plugin/__init__.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-20 09:17:37.219883 racetrack-client-2.9.1/racetrack_client/plugin/bundler/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-11-02 10:40:46.000000 racetrack-client-2.9.1/racetrack_client/plugin/bundler/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2982 2023-01-26 14:12:39.000000 racetrack-client-2.9.1/racetrack_client/plugin/bundler/bundle.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3019 2022-11-02 10:40:46.000000 racetrack-client-2.9.1/racetrack_client/plugin/bundler/filename_matcher.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     7420 2023-02-03 12:28:08.000000 racetrack-client-2.9.1/racetrack_client/plugin/install.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      523 2022-12-20 10:18:06.000000 racetrack-client-2.9.1/racetrack_client/plugin/plugin_manifest.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-20 09:17:37.271883 racetrack-client-2.9.1/racetrack_client/utils/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-08-04 14:52:29.000000 racetrack-client-2.9.1/racetrack_client/utils/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1172 2023-01-27 11:45:30.000000 racetrack-client-2.9.1/racetrack_client/utils/auth.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1182 2022-11-02 10:40:46.000000 racetrack-client-2.9.1/racetrack_client/utils/config.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2892 2022-12-20 10:18:06.000000 racetrack-client-2.9.1/racetrack_client/utils/datamodel.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2655 2022-11-02 10:40:46.000000 racetrack-client-2.9.1/racetrack_client/utils/quantity.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    11450 2023-01-30 11:10:05.000000 racetrack-client-2.9.1/racetrack_client/utils/request.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     5339 2022-11-02 10:40:46.000000 racetrack-client-2.9.1/racetrack_client/utils/semver.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     5824 2023-02-10 13:41:58.000000 racetrack-client-2.9.1/racetrack_client/utils/shell.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      744 2023-01-26 14:12:39.000000 racetrack-client-2.9.1/racetrack_client/utils/table.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2414 2023-01-26 14:12:39.000000 racetrack-client-2.9.1/racetrack_client/utils/time.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      657 2022-11-02 10:40:46.000000 racetrack-client-2.9.1/racetrack_client/utils/url.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-02-20 09:17:37.095883 racetrack-client-2.9.1/racetrack_client.egg-info/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3606 2023-02-20 09:17:36.000000 racetrack-client-2.9.1/racetrack_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1827 2023-02-20 09:17:36.000000 racetrack-client-2.9.1/racetrack_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        1 2023-02-20 09:17:36.000000 racetrack-client-2.9.1/racetrack_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       57 2023-02-20 09:17:36.000000 racetrack-client-2.9.1/racetrack_client.egg-info/entry_points.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       82 2023-02-20 09:17:36.000000 racetrack-client-2.9.1/racetrack_client.egg-info/requires.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       17 2023-02-20 09:17:36.000000 racetrack-client-2.9.1/racetrack_client.egg-info/top_level.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2023-02-20 09:17:37.275883 racetrack-client-2.9.1/setup.cfg
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1126 2022-11-02 10:40:46.000000 racetrack-client-2.9.1/setup.py
```

### Comparing `racetrack-client-2.9.0/LICENSE` & `racetrack-client-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/PKG-INFO` & `racetrack-client-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: racetrack-client
-Version: 2.9.0
+Version: 2.9.1
 Summary: CLI client tool for deploying workloads to Racetrack
 Home-page: https://github.com/TheRacetrack/racetrack
 Author: ERST
 Author-email: noreply@erst.dk
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `racetrack-client-2.9.0/README.md` & `racetrack-client-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/client/deploy.py` & `racetrack-client-2.9.1/racetrack_client/client/deploy.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/client/env.py` & `racetrack-client-2.9.1/racetrack_client/client/env.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/client/logs.py` & `racetrack-client-2.9.1/racetrack_client/client/logs.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/client/manage.py` & `racetrack-client-2.9.1/racetrack_client/client/manage.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/client/move.py` & `racetrack-client-2.9.1/racetrack_client/client/move.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/client/run.py` & `racetrack-client-2.9.1/racetrack_client/client/run.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/client/socketio.py` & `racetrack-client-2.9.1/racetrack_client/client/socketio.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/client_config/alias.py` & `racetrack-client-2.9.1/racetrack_client/client_config/alias.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/client_config/auth.py` & `racetrack-client-2.9.1/racetrack_client/client_config/auth.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/client_config/client_config.py` & `racetrack-client-2.9.1/racetrack_client/client_config/client_config.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/client_config/io.py` & `racetrack-client-2.9.1/racetrack_client/client_config/io.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/client_config/update.py` & `racetrack-client-2.9.1/racetrack_client/client_config/update.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/log/context_error.py` & `racetrack-client-2.9.1/racetrack_client/log/context_error.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/log/exception.py` & `racetrack-client-2.9.1/racetrack_client/log/exception.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/log/logs.py` & `racetrack-client-2.9.1/racetrack_client/log/logs.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/main.py` & `racetrack-client-2.9.1/racetrack_client/main.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/manifest/load.py` & `racetrack-client-2.9.1/racetrack_client/manifest/load.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/manifest/manifest.py` & `racetrack-client-2.9.1/racetrack_client/manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/manifest/merge.py` & `racetrack-client-2.9.1/racetrack_client/manifest/merge.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/manifest/validate.py` & `racetrack-client-2.9.1/racetrack_client/manifest/validate.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/plugin/bundler/bundle.py` & `racetrack-client-2.9.1/racetrack_client/plugin/bundler/bundle.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/plugin/bundler/filename_matcher.py` & `racetrack-client-2.9.1/racetrack_client/plugin/bundler/filename_matcher.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/plugin/install.py` & `racetrack-client-2.9.1/racetrack_client/plugin/install.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/plugin/plugin_manifest.py` & `racetrack-client-2.9.1/racetrack_client/plugin/plugin_manifest.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/utils/auth.py` & `racetrack-client-2.9.1/racetrack_client/utils/auth.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/utils/config.py` & `racetrack-client-2.9.1/racetrack_client/utils/config.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/utils/datamodel.py` & `racetrack-client-2.9.1/racetrack_client/utils/datamodel.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/utils/quantity.py` & `racetrack-client-2.9.1/racetrack_client/utils/quantity.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/utils/request.py` & `racetrack-client-2.9.1/racetrack_client/utils/request.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/utils/semver.py` & `racetrack-client-2.9.1/racetrack_client/utils/semver.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/utils/shell.py` & `racetrack-client-2.9.1/racetrack_client/utils/shell.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/utils/table.py` & `racetrack-client-2.9.1/racetrack_client/utils/table.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/utils/time.py` & `racetrack-client-2.9.1/racetrack_client/utils/time.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client/utils/url.py` & `racetrack-client-2.9.1/racetrack_client/utils/url.py`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/racetrack_client.egg-info/PKG-INFO` & `racetrack-client-2.9.1/racetrack_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: racetrack-client
-Version: 2.9.0
+Version: 2.9.1
 Summary: CLI client tool for deploying workloads to Racetrack
 Home-page: https://github.com/TheRacetrack/racetrack
 Author: ERST
 Author-email: noreply@erst.dk
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `racetrack-client-2.9.0/racetrack_client.egg-info/SOURCES.txt` & `racetrack-client-2.9.1/racetrack_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `racetrack-client-2.9.0/setup.py` & `racetrack-client-2.9.1/setup.py`

 * *Files identical despite different names*

