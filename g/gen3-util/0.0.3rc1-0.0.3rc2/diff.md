# Comparing `tmp/gen3_util-0.0.3rc1.tar.gz` & `tmp/gen3_util-0.0.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_util-0.0.3rc1.tar", last modified: Mon Jul 10 18:40:18 2023, max compression
+gzip compressed data, was "gen3_util-0.0.3rc2.tar", last modified: Tue Jul 11 22:27:56 2023, max compression
```

## Comparing `gen3_util-0.0.3rc1.tar` & `gen3_util-0.0.3rc2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.511681 gen3_util-0.0.3rc1/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.3rc1/LICENSE
--rw-r--r--   0 walsbr   (320923486) 1971611142     8910 2023-07-10 18:40:18.511295 gen3_util-0.0.3rc1/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     8225 2023-07-10 18:37:56.000000 gen3_util-0.0.3rc1/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.469457 gen3_util-0.0.3rc1/gen3_util/
--rw-r--r--   0 walsbr   (320923486) 1971611142       71 2023-07-05 18:55:42.000000 gen3_util-0.0.3rc1/gen3_util/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.474230 gen3_util-0.0.3rc1/gen3_util/access/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2321 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/access/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4281 2023-07-07 00:45:48.000000 gen3_util-0.0.3rc1/gen3_util/access/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.474498 gen3_util-0.0.3rc1/gen3_util/access/policies/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/access/policies/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5679 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/access/requestor.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.490177 gen3_util-0.0.3rc1/gen3_util/buckets/
--rw-r--r--   0 walsbr   (320923486) 1971611142      803 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc1/gen3_util/buckets/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      629 2023-06-21 17:42:54.000000 gen3_util-0.0.3rc1/gen3_util/buckets/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      474 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc1/gen3_util/buckets/lister.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.491065 gen3_util-0.0.3rc1/gen3_util/cli/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4637 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/cli/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-06-21 17:42:54.000000 gen3_util-0.0.3rc1/gen3_util/cli/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.491494 gen3_util-0.0.3rc1/gen3_util/common/
--rw-r--r--   0 walsbr   (320923486) 1971611142     5262 2023-07-07 00:45:48.000000 gen3_util-0.0.3rc1/gen3_util/common/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.495969 gen3_util-0.0.3rc1/gen3_util/config/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2824 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/config/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      433 2023-06-28 20:29:46.000000 gen3_util-0.0.3rc1/gen3_util/config/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc1/gen3_util/config/config.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.498147 gen3_util-0.0.3rc1/gen3_util/files/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1285 2023-06-21 17:42:55.000000 gen3_util-0.0.3rc1/gen3_util/files/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2246 2023-06-21 17:42:55.000000 gen3_util-0.0.3rc1/gen3_util/files/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      938 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/files/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      192 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc1/gen3_util/files/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      202 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc1/gen3_util/files/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    12907 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/files/uploader.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.504241 gen3_util-0.0.3rc1/gen3_util/meta/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4101 2023-07-07 00:01:20.000000 gen3_util-0.0.3rc1/gen3_util/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2256 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      323 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/meta/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    11295 2023-07-10 18:31:58.000000 gen3_util-0.0.3rc1/gen3_util/meta/importer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      329 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/meta/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      201 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc1/gen3_util/meta/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3858 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/meta/uploader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3293 2023-07-07 00:01:20.000000 gen3_util-0.0.3rc1/gen3_util/meta/validator.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.505824 gen3_util-0.0.3rc1/gen3_util/projects/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2247 2023-06-21 17:42:55.000000 gen3_util-0.0.3rc1/gen3_util/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2769 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1901 2023-06-30 03:26:36.000000 gen3_util-0.0.3rc1/gen3_util/projects/creator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      793 2023-06-21 17:42:55.000000 gen3_util-0.0.3rc1/gen3_util/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1078 2023-06-28 20:29:46.000000 gen3_util-0.0.3rc1/gen3_util/projects/remover.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.472679 gen3_util-0.0.3rc1/gen3_util.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     8910 2023-07-10 18:40:18.000000 gen3_util-0.0.3rc1/gen3_util.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1687 2023-07-10 18:40:18.000000 gen3_util-0.0.3rc1/gen3_util.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-07-10 18:40:18.000000 gen3_util-0.0.3rc1/gen3_util.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       53 2023-07-10 18:40:18.000000 gen3_util-0.0.3rc1/gen3_util.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      128 2023-07-10 18:40:18.000000 gen3_util-0.0.3rc1/gen3_util.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       16 2023-07-10 18:40:18.000000 gen3_util-0.0.3rc1/gen3_util.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-07-10 18:40:18.511764 gen3_util-0.0.3rc1/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142     5579 2023-07-10 18:33:57.000000 gen3_util-0.0.3rc1/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.465045 gen3_util-0.0.3rc1/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.508037 gen3_util-0.0.3rc1/tests/integration/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.3rc1/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      270 2023-06-28 20:29:46.000000 gen3_util-0.0.3rc1/tests/integration/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4358 2023-07-07 00:45:48.000000 gen3_util-0.0.3rc1/tests/integration/test_access.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      454 2023-06-28 20:29:46.000000 gen3_util-0.0.3rc1/tests/integration/test_buckets.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      243 2023-06-28 20:29:46.000000 gen3_util-0.0.3rc1/tests/integration/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2089 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/tests/integration/test_files.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2443 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/tests/integration/test_meta.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1237 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/tests/integration/test_project.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.510307 gen3_util-0.0.3rc1/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.3rc1/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      322 2023-05-05 20:31:25.000000 gen3_util-0.0.3rc1/tests/unit/conftest.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.510561 gen3_util-0.0.3rc1/tests/unit/plugins/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:45:48.000000 gen3_util-0.0.3rc1/tests/unit/plugins/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.510794 gen3_util-0.0.3rc1/tests/unit/plugins/gen3_util_plugin_foo/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1450 2023-07-07 00:45:48.000000 gen3_util-0.0.3rc1/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3380 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/tests/unit/test_cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_util-0.0.3rc1/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      551 2023-05-05 20:31:25.000000 gen3_util-0.0.3rc1/tests/unit/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc1/tests/unit/test_files.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4616 2023-07-07 18:51:14.000000 gen3_util-0.0.3rc1/tests/unit/test_meta.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc1/tests/unit/test_validate_directory.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-11 22:27:56.448667 gen3_util-0.0.3rc2/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.3rc2/LICENSE
+-rw-r--r--   0 walsbr   (320923486) 1971611142     9566 2023-07-11 22:27:56.448147 gen3_util-0.0.3rc2/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     8881 2023-07-11 21:14:30.000000 gen3_util-0.0.3rc2/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-11 22:27:56.291139 gen3_util-0.0.3rc2/gen3_util/
+-rw-r--r--   0 walsbr   (320923486) 1971611142       71 2023-07-05 18:55:42.000000 gen3_util-0.0.3rc2/gen3_util/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-11 22:27:56.313512 gen3_util-0.0.3rc2/gen3_util/access/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2321 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc2/gen3_util/access/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4281 2023-07-07 00:45:48.000000 gen3_util-0.0.3rc2/gen3_util/access/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-11 22:27:56.314055 gen3_util-0.0.3rc2/gen3_util/access/policies/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc2/gen3_util/access/policies/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5679 2023-07-11 14:24:51.000000 gen3_util-0.0.3rc2/gen3_util/access/requestor.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-11 22:27:56.325103 gen3_util-0.0.3rc2/gen3_util/buckets/
+-rw-r--r--   0 walsbr   (320923486) 1971611142      803 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc2/gen3_util/buckets/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      629 2023-06-21 17:42:54.000000 gen3_util-0.0.3rc2/gen3_util/buckets/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      474 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc2/gen3_util/buckets/lister.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-11 22:27:56.327365 gen3_util-0.0.3rc2/gen3_util/cli/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4637 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc2/gen3_util/cli/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-06-21 17:42:54.000000 gen3_util-0.0.3rc2/gen3_util/cli/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-11 22:27:56.328279 gen3_util-0.0.3rc2/gen3_util/common/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5262 2023-07-07 00:45:48.000000 gen3_util-0.0.3rc2/gen3_util/common/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-11 22:27:56.363240 gen3_util-0.0.3rc2/gen3_util/config/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2824 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc2/gen3_util/config/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      433 2023-06-28 20:29:46.000000 gen3_util-0.0.3rc2/gen3_util/config/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc2/gen3_util/config/config.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-11 22:27:56.408918 gen3_util-0.0.3rc2/gen3_util/files/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1285 2023-06-21 17:42:55.000000 gen3_util-0.0.3rc2/gen3_util/files/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2246 2023-06-21 17:42:55.000000 gen3_util-0.0.3rc2/gen3_util/files/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      938 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc2/gen3_util/files/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      192 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc2/gen3_util/files/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      202 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc2/gen3_util/files/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    12907 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc2/gen3_util/files/uploader.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-11 22:27:56.416658 gen3_util-0.0.3rc2/gen3_util/meta/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4101 2023-07-07 00:01:20.000000 gen3_util-0.0.3rc2/gen3_util/meta/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2256 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc2/gen3_util/meta/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      323 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc2/gen3_util/meta/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    11295 2023-07-11 21:14:30.000000 gen3_util-0.0.3rc2/gen3_util/meta/importer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      329 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc2/gen3_util/meta/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      201 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc2/gen3_util/meta/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3858 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc2/gen3_util/meta/uploader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3299 2023-07-11 21:14:30.000000 gen3_util-0.0.3rc2/gen3_util/meta/validator.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-11 22:27:56.421153 gen3_util-0.0.3rc2/gen3_util/projects/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2247 2023-06-21 17:42:55.000000 gen3_util-0.0.3rc2/gen3_util/projects/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2769 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc2/gen3_util/projects/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1901 2023-06-30 03:26:36.000000 gen3_util-0.0.3rc2/gen3_util/projects/creator.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      793 2023-06-21 17:42:55.000000 gen3_util-0.0.3rc2/gen3_util/projects/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1078 2023-06-28 20:29:46.000000 gen3_util-0.0.3rc2/gen3_util/projects/remover.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-11 22:27:56.312033 gen3_util-0.0.3rc2/gen3_util.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     9566 2023-07-11 22:27:56.000000 gen3_util-0.0.3rc2/gen3_util.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1687 2023-07-11 22:27:56.000000 gen3_util-0.0.3rc2/gen3_util.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-07-11 22:27:56.000000 gen3_util-0.0.3rc2/gen3_util.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       53 2023-07-11 22:27:56.000000 gen3_util-0.0.3rc2/gen3_util.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      128 2023-07-11 22:27:56.000000 gen3_util-0.0.3rc2/gen3_util.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       16 2023-07-11 22:27:56.000000 gen3_util-0.0.3rc2/gen3_util.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-07-11 22:27:56.448741 gen3_util-0.0.3rc2/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5579 2023-07-11 22:27:31.000000 gen3_util-0.0.3rc2/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-11 22:27:56.278877 gen3_util-0.0.3rc2/tests/
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-11 22:27:56.439530 gen3_util-0.0.3rc2/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.3rc2/tests/integration/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      270 2023-06-28 20:29:46.000000 gen3_util-0.0.3rc2/tests/integration/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4358 2023-07-07 00:45:48.000000 gen3_util-0.0.3rc2/tests/integration/test_access.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      454 2023-06-28 20:29:46.000000 gen3_util-0.0.3rc2/tests/integration/test_buckets.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      243 2023-06-28 20:29:46.000000 gen3_util-0.0.3rc2/tests/integration/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2089 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc2/tests/integration/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4318 2023-07-11 21:14:30.000000 gen3_util-0.0.3rc2/tests/integration/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1237 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc2/tests/integration/test_project.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-11 22:27:56.445275 gen3_util-0.0.3rc2/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.3rc2/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      322 2023-05-05 20:31:25.000000 gen3_util-0.0.3rc2/tests/unit/conftest.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-11 22:27:56.445897 gen3_util-0.0.3rc2/tests/unit/plugins/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:45:48.000000 gen3_util-0.0.3rc2/tests/unit/plugins/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-11 22:27:56.446426 gen3_util-0.0.3rc2/tests/unit/plugins/gen3_util_plugin_foo/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1450 2023-07-07 00:45:48.000000 gen3_util-0.0.3rc2/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3380 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc2/tests/unit/test_cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_util-0.0.3rc2/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      551 2023-05-05 20:31:25.000000 gen3_util-0.0.3rc2/tests/unit/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc2/tests/unit/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4616 2023-07-07 18:51:14.000000 gen3_util-0.0.3rc2/tests/unit/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc2/tests/unit/test_validate_directory.py
```

### Comparing `gen3_util-0.0.3rc1/LICENSE` & `gen3_util-0.0.3rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/PKG-INFO` & `gen3_util-0.0.3rc2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3_util
-Version: 0.0.3rc1
+Version: 0.0.3rc2
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
@@ -233,14 +233,25 @@
 
 ```
 
 For more see [test_meta_plugin](./tests/unit/meta/test_plugins.py)
 
 
 
+> I need to upload those files to the instance
+
+```
+$ gen3_util files cp --ignore_state --project_id aced-MyExperiment tmp/foo/DocumentReference.ndjson  bucket://aced-development-ohsu-data-bucket
+100%|██████████████████████████████████████████████████████████████████████████████████████████████████████| 5.74M/5.74M [00:03<00:00, 1.71MB/s, elapsed=0:00:02.056022, file=6f8101]
+info:
+- Wrote state to ~/.gen3/gen3-util-state/state.ndjson
+msg: OK
+```
+
+
 > I need to upload the meta data about those files to the instance
 
 ```
 $gen3_util meta cp tmp/foo bucket://aced-development-ohsu-data-bucket --project_id aced-MyExperiment
 msg: Uploaded /var/folders/2c/hffqqtr94nv64tjy0xrl38r89k1sty/T/tmpacozhhoo/_aced-MyExperiment_meta.zip
 ```
```

### Comparing `gen3_util-0.0.3rc1/README.md` & `gen3_util-0.0.3rc2/gen3_util.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: gen3-util
+Version: 0.0.3rc2
+Summary: Commons utilities
+Home-page: https://github.com/ACED-IDP/gen3_util
+Author: Ellrott Lab
+License: UNKNOWN
+Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
+Project-URL: Source, https://github.com/ACED-IDP/gen3_util
+Keywords: gen3 bioinformatics
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 # Gen3 Utilities
 
 Utilities to manage Gen3 schemas, projects and submissions.
 
 ## Installation
 
@@ -213,14 +233,25 @@
 
 ```
 
 For more see [test_meta_plugin](./tests/unit/meta/test_plugins.py)
 
 
 
+> I need to upload those files to the instance
+
+```
+$ gen3_util files cp --ignore_state --project_id aced-MyExperiment tmp/foo/DocumentReference.ndjson  bucket://aced-development-ohsu-data-bucket
+100%|██████████████████████████████████████████████████████████████████████████████████████████████████████| 5.74M/5.74M [00:03<00:00, 1.71MB/s, elapsed=0:00:02.056022, file=6f8101]
+info:
+- Wrote state to ~/.gen3/gen3-util-state/state.ndjson
+msg: OK
+```
+
+
 > I need to upload the meta data about those files to the instance
 
 ```
 $gen3_util meta cp tmp/foo bucket://aced-development-ohsu-data-bucket --project_id aced-MyExperiment
 msg: Uploaded /var/folders/2c/hffqqtr94nv64tjy0xrl38r89k1sty/T/tmpacozhhoo/_aced-MyExperiment_meta.zip
 ```
 
@@ -328,7 +359,9 @@
 
 # this could be maintained as so: export $(cat .env | xargs)
 
 rm -r dist/
 python3  setup.py sdist bdist_wheel
 twine upload dist/*
 ```
+
+
```

### Comparing `gen3_util-0.0.3rc1/gen3_util/access/__init__.py` & `gen3_util-0.0.3rc2/gen3_util/access/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/access/cli.py` & `gen3_util-0.0.3rc2/gen3_util/access/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/access/requestor.py` & `gen3_util-0.0.3rc2/gen3_util/access/requestor.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/buckets/__init__.py` & `gen3_util-0.0.3rc2/gen3_util/buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/buckets/cli.py` & `gen3_util-0.0.3rc2/gen3_util/buckets/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/cli/__init__.py` & `gen3_util-0.0.3rc2/gen3_util/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/cli/cli.py` & `gen3_util-0.0.3rc2/gen3_util/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/common/__init__.py` & `gen3_util-0.0.3rc2/gen3_util/common/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/config/__init__.py` & `gen3_util-0.0.3rc2/gen3_util/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/files/__init__.py` & `gen3_util-0.0.3rc2/gen3_util/files/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/files/cli.py` & `gen3_util-0.0.3rc2/gen3_util/files/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/files/downloader.py` & `gen3_util-0.0.3rc2/gen3_util/files/downloader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/files/uploader.py` & `gen3_util-0.0.3rc2/gen3_util/files/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/meta/__init__.py` & `gen3_util-0.0.3rc2/gen3_util/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/meta/cli.py` & `gen3_util-0.0.3rc2/gen3_util/meta/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/meta/importer.py` & `gen3_util-0.0.3rc2/gen3_util/meta/importer.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/meta/uploader.py` & `gen3_util-0.0.3rc2/gen3_util/meta/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/meta/validator.py` & `gen3_util-0.0.3rc2/gen3_util/meta/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,17 @@
 
 def validate(config: Config, directory_path: pathlib.Path) -> ValidateDirectoryResult:
     """Check FHIR data, accumulate results."""
     exceptions = []
     resources = defaultdict(int)
     print("DIRECTORY PATH: ", directory_path)
     for parse_result in directory_reader(directory_path):
-        print('parse_result', parse_result)
 
         if parse_result.exception:
+            # print('parse_result', parse_result)
             exceptions.append(parse_result)
         else:
             resources[parse_result.resource.resource_type] += 1
     return ValidateDirectoryResult(resources={'summary': dict(resources)}, exceptions=exceptions)
 
 
 #
```

### Comparing `gen3_util-0.0.3rc1/gen3_util/projects/__init__.py` & `gen3_util-0.0.3rc2/gen3_util/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/projects/cli.py` & `gen3_util-0.0.3rc2/gen3_util/projects/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/projects/creator.py` & `gen3_util-0.0.3rc2/gen3_util/projects/creator.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/projects/lister.py` & `gen3_util-0.0.3rc2/gen3_util/projects/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util/projects/remover.py` & `gen3_util-0.0.3rc2/gen3_util/projects/remover.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/gen3_util.egg-info/PKG-INFO` & `gen3_util-0.0.3rc2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: gen3-util
-Version: 0.0.3rc1
-Summary: Commons utilities
-Home-page: https://github.com/ACED-IDP/gen3_util
-Author: Ellrott Lab
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
-Project-URL: Source, https://github.com/ACED-IDP/gen3_util
-Keywords: gen3 bioinformatics
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 # Gen3 Utilities
 
 Utilities to manage Gen3 schemas, projects and submissions.
 
 ## Installation
 
@@ -233,14 +213,25 @@
 
 ```
 
 For more see [test_meta_plugin](./tests/unit/meta/test_plugins.py)
 
 
 
+> I need to upload those files to the instance
+
+```
+$ gen3_util files cp --ignore_state --project_id aced-MyExperiment tmp/foo/DocumentReference.ndjson  bucket://aced-development-ohsu-data-bucket
+100%|██████████████████████████████████████████████████████████████████████████████████████████████████████| 5.74M/5.74M [00:03<00:00, 1.71MB/s, elapsed=0:00:02.056022, file=6f8101]
+info:
+- Wrote state to ~/.gen3/gen3-util-state/state.ndjson
+msg: OK
+```
+
+
 > I need to upload the meta data about those files to the instance
 
 ```
 $gen3_util meta cp tmp/foo bucket://aced-development-ohsu-data-bucket --project_id aced-MyExperiment
 msg: Uploaded /var/folders/2c/hffqqtr94nv64tjy0xrl38r89k1sty/T/tmpacozhhoo/_aced-MyExperiment_meta.zip
 ```
 
@@ -348,9 +339,7 @@
 
 # this could be maintained as so: export $(cat .env | xargs)
 
 rm -r dist/
 python3  setup.py sdist bdist_wheel
 twine upload dist/*
 ```
-
-
```

### Comparing `gen3_util-0.0.3rc1/gen3_util.egg-info/SOURCES.txt` & `gen3_util-0.0.3rc2/gen3_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/setup.py` & `gen3_util-0.0.3rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='gen3_util',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.3rc1',  # Required
+    version='0.0.3rc2',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Commons utilities',
     # Optional
```

### Comparing `gen3_util-0.0.3rc1/tests/integration/test_access.py` & `gen3_util-0.0.3rc2/tests/integration/test_access.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/tests/integration/test_files.py` & `gen3_util-0.0.3rc2/tests/integration/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/tests/integration/test_meta.py` & `gen3_util-0.0.3rc2/tests/unit/test_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,100 @@
-import json
-import pathlib
-
 from click.testing import CliRunner
-
 from gen3_util.cli.cli import cli
 
 
-def import_from_directory():
-    params = 'meta  import dir tests/fixtures/dir_to_study/ tmp/foo --project_id aced-foo'.split()
+def test_default_command(caplog):
+    """Ensure it prints version if no other command"""
     runner = CliRunner()
-    result = runner.invoke(cli, params)
-    print(result.output)
+    result = runner.invoke(cli)
     assert result.exit_code == 0
-    expected_strings = ['DocumentReference', "size: 6013814", 'ResearchStudy', "count: 1"]
-    for expected_string in expected_strings:
-        assert expected_string in result.output, f"{expected_string} not found in {result.output}"
+    expected = ['Version']
+    for _ in expected:
+        assert _ in result.output, f"Should have printed expected={_} actual={result.output}"
 
-    result = runner.invoke(cli, 'meta validate tmp/foo'.split())
-    print(result.output)
+
+def test_any_command(caplog):
+    """Ensure it does not print version if command provided"""
+    runner = CliRunner()
+    result = runner.invoke(cli, ['config'])
     assert result.exit_code == 0
-    expected_strings = ["msg: OK"]
-    for expected_string in expected_strings:
-        assert expected_string in result.output, f"{expected_string} not found in {result.output}"
+    un_expected_strings = ['Version']
+    for expected_string in un_expected_strings:
+        assert expected_string not in result.output, "only print version if nothing else to do"
 
 
-def ls():
-    params = '--format json meta ls'.split()
+def test_help(caplog):
+    """Ensure it prints command groups"""
     runner = CliRunner()
-    result = runner.invoke(cli, params)
-    print(result.output)
+    result = runner.invoke(cli, ['--help'])
     assert result.exit_code == 0
-    expected_strings = ['"msg": "OK"', "is_metadata", "file_name"]
+    print(result.output)
+    expected_strings = """
+        projects  Manage Gen3 projects.
+        buckets   Manage Gen3 buckets.
+        meta      Manage meta data.
+        files     Manage file transfers.
+        access    Manage access requests.
+        config    Configure this utility.
+        """.split()
     for expected_string in expected_strings:
-        assert expected_string in result.output, f"{expected_string} not found in {result.output}"
-    return json.loads(result.output)
+        assert expected_string in result.output, f"Should have printed {expected_string}"
 
 
-def cp_upload(data_bucket):
-    params = f'--format json meta cp tmp/foo/extractions bucket://{data_bucket} --project_id aced-foo --ignore_state'.split()
+def test_projects(caplog):
+    """Ensure it prints project"""
     runner = CliRunner()
-    result = runner.invoke(cli, params)
-    print(result.output)
+    result = runner.invoke(cli, ['projects', '--help'])
     assert result.exit_code == 0
-    expected_strings = ['Uploaded']
+    print(result.output)
+    expected_strings = """
+      ls     List all projects.
+      touch  Create a project
+      rm     Remove project.
+    """.split()
     for expected_string in expected_strings:
-        assert expected_string in result.output, f"{expected_string} not found in {result.output}"
+        assert expected_string in result.output, f"Should have printed {expected_string}"
 
 
-def cp_download(did):
-    params = f'--format json meta cp {did} tmp/foo/'.split()
+def test_meta(caplog):
+    """Ensure it prints meta"""
     runner = CliRunner()
-    result = runner.invoke(cli, params)
+    result = runner.invoke(cli, ['meta', '--help'])
+    assert result.exit_code == 0
     print(result.output)
+    expected_strings = """
+      cp        Copy meta to/from the project bucket.
+      ls        Query buckets from submitted metadata.
+      rm        Remove meta from a project.
+      import    Import study from directory listing.
+      validate  Validate FHIR data in DIRECTORY.
+    """.split()
+    for expected_string in expected_strings:
+        assert expected_string in result.output, f"Should have printed {expected_string}"
+
+
+def test_file(caplog):
+    """Ensure it prints file"""
+    runner = CliRunner()
+    result = runner.invoke(cli, ['files', '--help'])
     assert result.exit_code == 0
-    expected_strings = ['Downloaded']
+    print(result.output)
+    expected_strings = """
+      ls  List files in a project.
+      cp  Copy files to/from the project bucket.
+      rm  Remove files from a project.
+    """.split()
     for expected_string in expected_strings:
-        assert expected_string in result.output, f"{expected_string} not found in {result.output}"
+        assert expected_string in result.output, f"Should have printed {expected_string}"
 
 
-def test_workflow(data_bucket):
-    import_from_directory()
-    cp_upload(data_bucket)
-    records = ls()['records']
-    for _ in records:
-        cp_download(_['did'])
-        stat = pathlib.Path(f"tmp/foo/{_['file_name']}").stat()
-        assert stat.st_size == _['size']
+def test_config(caplog):
+    """Ensure it prints file"""
+    runner = CliRunner()
+    result = runner.invoke(cli, ['config', '--help'])
+    assert result.exit_code == 0
+    print(result.output)
+    expected_strings = """
+      ls  Show defaults.
+    """.split()
+    for expected_string in expected_strings:
+        assert expected_string in result.output, f"Should have printed {expected_string}"
```

### Comparing `gen3_util-0.0.3rc1/tests/integration/test_project.py` & `gen3_util-0.0.3rc2/tests/integration/test_project.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/tests/unit/plugins/gen3_util_plugin_foo/__init__.py` & `gen3_util-0.0.3rc2/tests/unit/plugins/gen3_util_plugin_foo/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/tests/unit/test_coding_conventions.py` & `gen3_util-0.0.3rc2/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/tests/unit/test_config.py` & `gen3_util-0.0.3rc2/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/tests/unit/test_files.py` & `gen3_util-0.0.3rc2/tests/unit/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/tests/unit/test_meta.py` & `gen3_util-0.0.3rc2/tests/unit/test_meta.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.3rc1/tests/unit/test_validate_directory.py` & `gen3_util-0.0.3rc2/tests/unit/test_validate_directory.py`

 * *Files identical despite different names*

