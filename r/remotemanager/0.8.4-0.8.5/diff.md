# Comparing `tmp/remotemanager-0.8.4.tar.gz` & `tmp/remotemanager-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.8.4.tar", last modified: Thu Jul 13 07:25:54 2023, max compression
+gzip compressed data, was "remotemanager-0.8.5.tar", last modified: Mon Jul 17 10:02:38 2023, max compression
```

## Comparing `remotemanager-0.8.4.tar` & `remotemanager-0.8.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.880416 remotemanager-0.8.4/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.8.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-13 07:25:54.880416 remotemanager-0.8.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.8.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-12 12:21:16.000000 remotemanager-0.8.4/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.868415 remotemanager-0.8.4/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-12 12:21:16.000000 remotemanager-0.8.4/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.872415 remotemanager-0.8.4/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.8.4/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.872415 remotemanager-0.8.4/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:11.000000 remotemanager-0.8.4/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.8.4/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.8.4/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.8.4/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.8.4/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    25712 2023-07-04 13:31:41.000000 remotemanager-0.8.4/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.872415 remotemanager-0.8.4/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    50081 2023-07-13 05:57:57.000000 remotemanager-0.8.4/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     4895 2023-07-12 13:38:06.000000 remotemanager-0.8.4/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-12 13:38:06.000000 remotemanager-0.8.4/remotemanager/dataset/lazy_append.py
--rw-rw-rw-   0 root         (0) root         (0)    26112 2023-07-13 05:57:57.000000 remotemanager-0.8.4/remotemanager/dataset/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.872415 remotemanager-0.8.4/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.8.4/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4922 2023-07-13 05:57:57.000000 remotemanager-0.8.4/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.876415 remotemanager-0.8.4/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.8.4/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.8.4/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.8.4/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.8.4/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.876415 remotemanager-0.8.4/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.8.4/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.8.4/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.8.4/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.876415 remotemanager-0.8.4/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.8.4/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.8.4/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-07-13 05:57:57.000000 remotemanager-0.8.4/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.876415 remotemanager-0.8.4/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.8.4/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.8.4/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)     9435 2023-07-13 05:57:57.000000 remotemanager-0.8.4/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.876415 remotemanager-0.8.4/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     4596 2023-07-13 05:57:57.000000 remotemanager-0.8.4/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.8.4/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 07:25:54.872415 remotemanager-0.8.4/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-13 07:25:54.000000 remotemanager-0.8.4/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1825 2023-07-13 07:25:54.000000 remotemanager-0.8.4/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 07:25:54.000000 remotemanager-0.8.4/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-07-13 07:25:54.000000 remotemanager-0.8.4/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-13 07:25:54.000000 remotemanager-0.8.4/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 07:25:54.880416 remotemanager-0.8.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.8.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:02:38.434273 remotemanager-0.8.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.8.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-17 10:02:38.434273 remotemanager-0.8.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.8.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-17 06:40:51.000000 remotemanager-0.8.5/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:02:38.426272 remotemanager-0.8.5/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-17 06:40:51.000000 remotemanager-0.8.5/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:02:38.430272 remotemanager-0.8.5/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.8.5/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.8.5/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:02:38.430272 remotemanager-0.8.5/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.8.5/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:11.000000 remotemanager-0.8.5/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.8.5/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.8.5/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.8.5/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.8.5/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.8.5/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    25712 2023-07-04 13:31:41.000000 remotemanager-0.8.5/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:02:38.430272 remotemanager-0.8.5/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.8.5/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    52101 2023-07-17 06:40:51.000000 remotemanager-0.8.5/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     5819 2023-07-17 06:40:51.000000 remotemanager-0.8.5/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-12 13:38:06.000000 remotemanager-0.8.5/remotemanager/dataset/lazy_append.py
+-rw-rw-rw-   0 root         (0) root         (0)    26112 2023-07-17 06:40:51.000000 remotemanager-0.8.5/remotemanager/dataset/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:02:38.430272 remotemanager-0.8.5/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.8.5/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4922 2023-07-17 06:40:51.000000 remotemanager-0.8.5/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:02:38.434273 remotemanager-0.8.5/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.8.5/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.8.5/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.8.5/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.8.5/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.8.5/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:02:38.434273 remotemanager-0.8.5/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.8.5/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.8.5/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.8.5/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.8.5/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.8.5/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.8.5/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:02:38.434273 remotemanager-0.8.5/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.8.5/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.8.5/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.8.5/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.8.5/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.8.5/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-07-17 06:40:51.000000 remotemanager-0.8.5/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:02:38.434273 remotemanager-0.8.5/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.8.5/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.8.5/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.8.5/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.8.5/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)     9435 2023-07-17 06:40:51.000000 remotemanager-0.8.5/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:02:38.434273 remotemanager-0.8.5/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     4596 2023-07-17 06:40:51.000000 remotemanager-0.8.5/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.8.5/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.8.5/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.8.5/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:02:38.430272 remotemanager-0.8.5/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-17 10:02:38.000000 remotemanager-0.8.5/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-07-17 10:02:38.000000 remotemanager-0.8.5/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 10:02:38.000000 remotemanager-0.8.5/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-17 10:02:38.000000 remotemanager-0.8.5/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-17 10:02:38.000000 remotemanager-0.8.5/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 10:02:38.434273 remotemanager-0.8.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.8.5/setup.py
```

### Comparing `remotemanager-0.8.4/LICENSE` & `remotemanager-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/PKG-INFO` & `remotemanager-0.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.8.4
+Version: 0.8.5
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.8.4/README.md` & `remotemanager-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/pyproject.toml` & `remotemanager-0.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.8.4"
+current_version = "0.8.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.8.4/remotemanager/connection/cmd.py` & `remotemanager-0.8.5/remotemanager/connection/cmd.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/connection/computers/base.py` & `remotemanager-0.8.5/remotemanager/connection/computers/base.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/connection/computers/example.py` & `remotemanager-0.8.5/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/connection/computers/options.py` & `remotemanager-0.8.5/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/connection/computers/parsers.py` & `remotemanager-0.8.5/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/connection/testing_object.py` & `remotemanager-0.8.5/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/connection/url.py` & `remotemanager-0.8.5/remotemanager/connection/url.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/dataset/dataset.py` & `remotemanager-0.8.5/remotemanager/dataset/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -542,27 +542,32 @@
 
     def finish_append(self):
         self.database.update(self.pack())
 
     def lazy_append(self):
         return LazyAppend(self)
 
-    def remove_run(self, id: any) -> bool:
+    def remove_run(self, id: any, dependency_call: bool = False) -> bool:
         """
         Remove a runner with the given identifier. Search methods are identical
         get_runner(id)
 
         Args:
             id:
                 identifier
+            dependency_call (bool):
+                used by any dependencies that exist, prevents recursion
 
         Returns:
             (bool): True if succeeded
         """
-        runner = self.get_runner(id)
+        if not dependency_call and self.dependency is not None:
+            return self.dependency.remove_run(id)
+
+        runner = self.get_runner(id, dependency_call)
 
         if runner is None:
             self._logger.info(f"could not find runner to remove")
             return False
 
         del self._runs[runner.id]
         self._uuids.remove(runner.uuid)
@@ -571,26 +576,29 @@
 
         # need to override attribute first, as updating can only add
         self.database._storage[self.uuid]["_runs"] = {}
         self.database.update(self.pack())
 
         return True
 
-    def get_runner(self, id) -> [Runner, None]:
+    def get_runner(self, id, dependency_call: bool = False) -> [Runner, None]:
         """
         Collect a runner with the given identifier. Depending on the type of
         arg passed, there are different search methods:
 
         - int: the runners[id] of the runner to remove
         - str: searches for a runner with the matching uuid
         - dict: attempts to find a runner with matching args
 
         Args:
             id:
                 identifier
+            dependency_call (bool):
+                used by the dependencies, runners cannot be removed via uuid in this
+                case, as the uuids will not match between datasets
 
         Returns:
             (Runner): collected Runner, None if not available
         """
 
         def get_by_id(id):
             self._logger.info(f"getting runner by id {id}")
@@ -602,14 +610,18 @@
 
         def get_by_str(id):
             self._logger.info(f'getting runner by string "{id}"')
 
             if id.lower() in self.runner_dict:
                 return self.runner_dict[id.lower()]
 
+            if dependency_call:
+                raise RuntimeError(
+                    "runners within a dependency cannot be removed by uuid"
+                )
             for r_id, r in self.runner_dict.items():
                 if len(id) == 64 and r.uuid == id:
                     self._logger.info(f"full uuid")
                     return r
                 elif len(id) == 8 and r.short_uuid == id:
                     self._logger.info(f"short uuid")
                     return r
@@ -620,35 +632,49 @@
                 if format_iterable(r.args) == format_iterable(id):
                     return r
 
         dispatch = {int: get_by_id, str: get_by_str, dict: get_by_dict}
 
         return dispatch.get(type(id))(id)
 
-    def clear_runs(self) -> None:
+    def clear_runs(self, dependency_call: bool = False) -> None:
         """
-        Wipes all runners
+        Removes all runners
+
+        Args:
+            dependency_call (bool):
+                used by any dependencies that exist, prevents recursion
         """
+        if not dependency_call and self.dependency is not None:
+            return self.dependency.clear_runs()
+
         self._logger.info("wiping all runners and updating the db")
 
         self._uuids = []
         self._runs = {}
 
         self.database._storage[self.uuid]["_runs"] = {}
         self.database.update(self.pack())
 
-    def clear_results(self) -> None:
+    def clear_results(self, dependency_call: bool = False) -> None:
         """
         Remove any results from the stored runners and attempt to delete their
         result files.
 
         .. warning::
             This is a potentially destructive action, be careful with this
             method
+
+        Args:
+            dependency_call (bool):
+                used by any dependencies that exist, prevents recursion
         """
+        if not dependency_call and self.dependency is not None:
+            return self.dependency.clear_results()
+
         for runner in self.runners:
             runner.clear_result()
 
     def _collect_files(self, attribute: str) -> list:
         """
         Collects attribute `attribute` from both Dataset and each runner,
         returning a list.
@@ -670,26 +696,33 @@
             tmp = []
         for runner in self.runners:
             file = getattr(runner, attribute)
             if file not in tmp:
                 tmp.append(file)
         return tmp
 
-    def wipe_local(self, files_only: bool = False) -> None:
+    def wipe_local(
+        self, files_only: bool = False, dependency_call: bool = False
+    ) -> None:
         """
         Clear out the local directory
 
         Args:
             files_only (bool):
                 delete individual files instead of whole folders (preserves
                 extra files)
+            dependency_call (bool):
+                used by any dependencies that exist, prevents recursion
 
         Returns:
             None
         """
+        if not dependency_call and self.dependency is not None:
+            return self.dependency.wipe_local(files_only)
+
         if not check_dir_is_child:
             raise RuntimeError(
                 f"local dir {self.local_dir} is not a child directory, "
                 f"deleting could have catastrophic effects"
             )
 
         if not files_only:
@@ -710,26 +743,33 @@
                 local += [f.local for f in self._collect_files(attr)]
             for file in local:
                 try:
                     os.remove(file)
                 except FileNotFoundError:
                     pass
 
-    def wipe_remote(self, files_only: bool = False) -> None:
+    def wipe_remote(
+        self, files_only: bool = False, dependency_call: bool = False
+    ) -> None:
         """
         Clear out the remote directory (including run dir)
 
         Args:
             files_only (bool):
                 delete individual files instead of whole folders (preserves
                 extra files)
+            dependency_call (bool):
+                used by any dependencies that exist, prevents recursion
 
         Returns:
             None
         """
+        if not dependency_call and self.dependency is not None:
+            return self.dependency.wipe_remote(files_only)
+
         if not files_only:
             remotes = self._collect_files("remote_dir")
         else:
             remotes = [s.remote for s in self._master_scripts]
             remotes += [r.remote for r in self._repo_files]
             attrs = ["runfile", "resultfile", "jobscript"]
             for attr in attrs:
@@ -740,26 +780,33 @@
         if len(remotes) > 1:
             remotestring = ",".join(remotes)
             self._logger.info(f"removing several remotes with string {remotestring}")
             self.url.cmd(f"rm -r {{{remotestring}}}", raise_errors=False)
         else:
             self.url.cmd(f"rm -r {remotes[0]}", raise_errors=False)
 
-    def hard_reset(self, files_only: bool = False) -> None:
+    def hard_reset(
+        self, files_only: bool = False, dependency_call: bool = False
+    ) -> None:
         """
         Hard reset the dataset, including wiping local and remote folders
 
         Args:
             files_only (bool):
                 delete individual files instead of whole folders (preserves
                 extra files)
+            dependency_call (bool):
+                used by any dependencies that exist, prevents recursion
 
         Returns:
             None
         """
+        if not dependency_call and self.dependency is not None:
+            return self.dependency.hard_reset(files_only)
+
         self.wipe_local(files_only)
         self.wipe_remote(files_only)
         self.clear_runs()
 
         try:
             os.remove(self.dbfile)
         except FileNotFoundError:
```

### Comparing `remotemanager-0.8.4/remotemanager/dataset/dependency.py` & `remotemanager-0.8.5/remotemanager/dataset/dependency.py`

 * *Files 18% similar despite different names*

```diff
@@ -56,14 +56,41 @@
         for pair in self.network:
             for ds in pair:
                 if ds not in datasets:
                     datasets.append(ds)
 
         return datasets
 
+    def remove_run(self, id: bool = False) -> bool:
+        out = []
+        for ds in self.ds_list:
+            out.append(ds.remove_run(id=id, dependency_call=True))
+
+        return all(out)
+
+    def clear_runs(self) -> None:
+        for ds in self.ds_list:
+            ds.clear_runs(dependency_call=True)
+
+    def clear_results(self) -> None:
+        for ds in self.ds_list:
+            ds.clear_results(dependency_call=True)
+
+    def wipe_local(self, files_only: bool = False) -> None:
+        for ds in self.ds_list:
+            ds.wipe_local(files_only=files_only, dependency_call=True)
+
+    def wipe_remote(self, files_only: bool = False) -> None:
+        for ds in self.ds_list:
+            ds.wipe_remote(files_only=files_only, dependency_call=True)
+
+    def hard_reset(self, files_only: bool = False) -> None:
+        for ds in self.ds_list:
+            ds.hard_reset(files_only=files_only, dependency_call=True)
+
     def append_run(self, caller, chain_run_args, run_args, *args, **kwargs):
         """
         Appends runs with the same args to all datasets
 
         Args:
             caller:
                 (Dataset): The dataset which defers to the dependency
```

### Comparing `remotemanager-0.8.4/remotemanager/dataset/lazy_append.py` & `remotemanager-0.8.5/remotemanager/dataset/lazy_append.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/dataset/runner.py` & `remotemanager-0.8.5/remotemanager/dataset/runner.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/jupyter/magic.py` & `remotemanager-0.8.5/remotemanager/jupyter/magic.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/logging/__init__.py` & `remotemanager-0.8.5/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/logging/log.py` & `remotemanager-0.8.5/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/logging/utils.py` & `remotemanager-0.8.5/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/logging/verbosity.py` & `remotemanager-0.8.5/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/serialisation/__init__.py` & `remotemanager-0.8.5/remotemanager/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/serialisation/serial.py` & `remotemanager-0.8.5/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.8.5/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.8.5/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/storage/database.py` & `remotemanager-0.8.5/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/storage/function.py` & `remotemanager-0.8.5/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/storage/remotefunction.py` & `remotemanager-0.8.5/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/storage/sendablemixin.py` & `remotemanager-0.8.5/remotemanager/storage/sendablemixin.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/storage/trackedfile.py` & `remotemanager-0.8.5/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/transport/cp.py` & `remotemanager-0.8.5/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/transport/rsync.py` & `remotemanager-0.8.5/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/transport/scp.py` & `remotemanager-0.8.5/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/transport/transport.py` & `remotemanager-0.8.5/remotemanager/transport/transport.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/utils/__init__.py` & `remotemanager-0.8.5/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/utils/flags.py` & `remotemanager-0.8.5/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager/utils/version.py` & `remotemanager-0.8.5/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.4/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.8.5/remotemanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.8.4
+Version: 0.8.5
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.8.4/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.8.5/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

