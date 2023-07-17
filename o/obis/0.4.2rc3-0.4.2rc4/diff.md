# Comparing `tmp/obis-0.4.2rc3.tar.gz` & `tmp/obis-0.4.2rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obis-0.4.2rc3.tar", last modified: Mon Jul 17 10:23:13 2023, max compression
+gzip compressed data, was "obis-0.4.2rc4.tar", last modified: Mon Jul 17 10:34:37 2023, max compression
```

## Comparing `obis-0.4.2rc3.tar` & `obis-0.4.2rc4.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:23:13.806892 obis-0.4.2rc3/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      773 2023-07-17 10:22:02.000000 obis-0.4.2rc3/CHANGELOG.md
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    11357 2023-02-20 13:30:53.000000 obis-0.4.2rc3/LICENSE
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      176 2023-02-20 13:30:53.000000 obis-0.4.2rc3/MANIFEST.in
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    30929 2023-07-17 10:23:13.806892 obis-0.4.2rc3/PKG-INFO
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    30367 2023-03-31 13:07:05.000000 obis-0.4.2rc3/README.md
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:23:13.782891 obis-0.4.2rc3/man/
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:23:13.790891 obis-0.4.2rc3/man/man1/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.2rc3/man/man1/obis-addref.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      879 2023-02-20 13:30:53.000000 obis-0.4.2rc3/man/man1/obis-clone.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      798 2023-02-20 13:30:53.000000 obis-0.4.2rc3/man/man1/obis-collection.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      825 2023-02-20 13:30:53.000000 obis-0.4.2rc3/man/man1/obis-commit.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-02-20 13:30:53.000000 obis-0.4.2rc3/man/man1/obis-config.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1027 2023-02-20 13:30:53.000000 obis-0.4.2rc3/man/man1/obis-data_set.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      893 2023-02-20 13:30:53.000000 obis-0.4.2rc3/man/man1/obis-download.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      757 2023-02-20 13:30:53.000000 obis-0.4.2rc3/man/man1/obis-init.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.2rc3/man/man1/obis-init_analysis.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.2rc3/man/man1/obis-move.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      762 2023-02-20 13:30:53.000000 obis-0.4.2rc3/man/man1/obis-object.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      617 2023-02-20 13:30:53.000000 obis-0.4.2rc3/man/man1/obis-removeref.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1221 2023-02-20 13:30:53.000000 obis-0.4.2rc3/man/man1/obis-repository.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      742 2023-02-20 13:30:53.000000 obis-0.4.2rc3/man/man1/obis-settings.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.2rc3/man/man1/obis-status.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      666 2023-02-20 13:30:53.000000 obis-0.4.2rc3/man/man1/obis-sync.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1684 2023-02-20 13:30:53.000000 obis-0.4.2rc3/man/man1/obis.1
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:23:13.790891 obis-0.4.2rc3/obis/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      757 2023-07-17 10:20:53.000000 obis-0.4.2rc3/obis/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:23:13.790891 obis-0.4.2rc3/obis/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      320 2023-07-07 07:51:46.000000 obis-0.4.2rc3/obis/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      563 2023-02-27 13:57:44.000000 obis-0.4.2rc3/obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      915 2023-02-21 12:05:41.000000 obis-0.4.2rc3/obis/conftest.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:23:13.794891 obis-0.4.2rc3/obis/dm/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      889 2023-02-21 12:05:41.000000 obis-0.4.2rc3/obis/dm/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:23:13.798891 obis-0.4.2rc3/obis/dm/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      411 2023-02-21 12:13:21.000000 obis-0.4.2rc3/obis/dm/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7402 2023-03-07 09:56:22.000000 obis-0.4.2rc3/obis/dm/__pycache__/checksum.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2407 2023-02-21 12:13:22.000000 obis-0.4.2rc3/obis/dm/__pycache__/command_log.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1839 2023-02-21 12:13:21.000000 obis-0.4.2rc3/obis/dm/__pycache__/command_result.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    15644 2023-02-21 12:13:21.000000 obis-0.4.2rc3/obis/dm/__pycache__/config.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    23132 2023-03-30 13:34:10.000000 obis-0.4.2rc3/obis/dm/__pycache__/data_mgmt.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    17466 2023-03-29 13:31:59.000000 obis-0.4.2rc3/obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7101 2023-03-30 10:33:16.000000 obis-0.4.2rc3/obis/dm/__pycache__/git.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1351 2023-02-21 12:17:13.000000 obis-0.4.2rc3/obis/dm/__pycache__/repository_utils.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3148 2023-03-30 10:51:56.000000 obis-0.4.2rc3/obis/dm/__pycache__/utils.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7820 2023-03-07 08:26:10.000000 obis-0.4.2rc3/obis/dm/checksum.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2674 2023-02-21 12:05:41.000000 obis-0.4.2rc3/obis/dm/command_log.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1981 2023-02-21 12:05:41.000000 obis-0.4.2rc3/obis/dm/command_result.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:23:13.798891 obis-0.4.2rc3/obis/dm/commands/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      634 2023-02-21 12:05:41.000000 obis-0.4.2rc3/obis/dm/commands/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:23:13.802892 obis-0.4.2rc3/obis/dm/commands/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      194 2023-02-21 12:13:21.000000 obis-0.4.2rc3/obis/dm/commands/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1867 2023-03-29 14:28:25.000000 obis-0.4.2rc3/obis/dm/commands/__pycache__/addref.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3935 2023-02-28 09:09:45.000000 obis-0.4.2rc3/obis/dm/commands/__pycache__/clone.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3041 2023-02-28 09:44:21.000000 obis-0.4.2rc3/obis/dm/commands/__pycache__/collection.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3046 2023-02-21 16:35:01.000000 obis-0.4.2rc3/obis/dm/commands/__pycache__/download.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3343 2023-03-03 14:34:14.000000 obis-0.4.2rc3/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2416 2023-02-21 12:17:13.000000 obis-0.4.2rc3/obis/dm/commands/__pycache__/move.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3263 2023-03-01 08:22:27.000000 obis-0.4.2rc3/obis/dm/commands/__pycache__/object.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    10941 2023-03-30 10:21:33.000000 obis-0.4.2rc3/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     6680 2023-02-21 12:17:13.000000 obis-0.4.2rc3/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3273 2023-02-21 12:17:13.000000 obis-0.4.2rc3/obis/dm/commands/__pycache__/removeref.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     8335 2023-07-17 10:14:41.000000 obis-0.4.2rc3/obis/dm/commands/__pycache__/search.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1589 2023-02-24 12:01:17.000000 obis-0.4.2rc3/obis/dm/commands/__pycache__/upload.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1897 2023-03-29 14:28:17.000000 obis-0.4.2rc3/obis/dm/commands/addref.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5292 2023-02-28 08:49:14.000000 obis-0.4.2rc3/obis/dm/commands/clone.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3657 2023-02-28 09:16:53.000000 obis-0.4.2rc3/obis/dm/commands/collection.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3920 2023-02-21 13:31:53.000000 obis-0.4.2rc3/obis/dm/commands/download.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4124 2023-03-03 14:31:58.000000 obis-0.4.2rc3/obis/dm/commands/download_physical.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2967 2023-02-21 12:05:41.000000 obis-0.4.2rc3/obis/dm/commands/move.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4373 2023-03-01 08:22:23.000000 obis-0.4.2rc3/obis/dm/commands/object.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    12135 2023-03-30 10:21:12.000000 obis-0.4.2rc3/obis/dm/commands/openbis_command.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1535 2023-02-21 12:05:41.000000 obis-0.4.2rc3/obis/dm/commands/openbis_command_test.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     9774 2023-02-21 12:05:41.000000 obis-0.4.2rc3/obis/dm/commands/openbis_sync.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3565 2023-02-21 12:05:41.000000 obis-0.4.2rc3/obis/dm/commands/removeref.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    12372 2023-07-17 10:12:16.000000 obis-0.4.2rc3/obis/dm/commands/search.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1801 2023-02-24 12:00:59.000000 obis-0.4.2rc3/obis/dm/commands/upload.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    16039 2023-02-21 12:05:42.000000 obis-0.4.2rc3/obis/dm/config.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2934 2023-02-21 12:05:41.000000 obis-0.4.2rc3/obis/dm/config_test.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    27953 2023-03-30 13:30:39.000000 obis-0.4.2rc3/obis/dm/data_mgmt.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    14376 2023-03-29 13:51:23.000000 obis-0.4.2rc3/obis/dm/data_mgmt_test.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      245 2023-02-20 13:30:53.000000 obis-0.4.2rc3/obis/dm/git-annex-attributes
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     8502 2023-03-30 10:32:13.000000 obis-0.4.2rc3/obis/dm/git.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1905 2023-02-21 12:05:41.000000 obis-0.4.2rc3/obis/dm/repository_utils.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3789 2023-03-30 10:51:34.000000 obis-0.4.2rc3/obis/dm/utils.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      980 2023-02-21 12:05:41.000000 obis-0.4.2rc3/obis/dm/utils_test.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:23:13.802892 obis-0.4.2rc3/obis/scripts/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      919 2023-02-21 12:05:41.000000 obis-0.4.2rc3/obis/scripts/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:23:13.802892 obis-0.4.2rc3/obis/scripts/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      431 2023-02-21 12:13:22.000000 obis-0.4.2rc3/obis/scripts/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    30930 2023-07-17 10:14:41.000000 obis-0.4.2rc3/obis/scripts/__pycache__/cli.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-02-21 12:13:22.000000 obis-0.4.2rc3/obis/scripts/__pycache__/click_util.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4351 2023-03-30 10:59:33.000000 obis-0.4.2rc3/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    39340 2023-07-17 10:13:46.000000 obis-0.4.2rc3/obis/scripts/cli.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1126 2023-02-21 12:05:41.000000 obis-0.4.2rc3/obis/scripts/click_util.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5701 2023-03-30 10:59:06.000000 obis-0.4.2rc3/obis/scripts/data_mgmt_runner.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:23:13.806892 obis-0.4.2rc3/obis/test-data/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)   160470 2023-02-20 13:30:53.000000 obis-0.4.2rc3/obis/test-data/snb-data.zip
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       43 2023-02-20 13:30:53.000000 obis-0.4.2rc3/obis/test-data/text-data-2.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       32 2023-02-20 13:30:53.000000 obis-0.4.2rc3/obis/test-data/text-data.txt
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:23:13.786891 obis-0.4.2rc3/obis/test-data/user_config/
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:23:13.806892 obis-0.4.2rc3/obis/test-data/user_config/.obis/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      167 2023-02-20 13:30:53.000000 obis-0.4.2rc3/obis/test-data/user_config/.obis/config.json
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:23:13.790891 obis-0.4.2rc3/obis.egg-info/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    30929 2023-07-17 10:23:13.000000 obis-0.4.2rc3/obis.egg-info/PKG-INFO
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3124 2023-07-17 10:23:13.000000 obis-0.4.2rc3/obis.egg-info/SOURCES.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-07-17 10:23:13.000000 obis-0.4.2rc3/obis.egg-info/dependency_links.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       47 2023-07-17 10:23:13.000000 obis-0.4.2rc3/obis.egg-info/entry_points.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-02-23 08:39:07.000000 obis-0.4.2rc3/obis.egg-info/not-zip-safe
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       37 2023-07-17 10:23:13.000000 obis-0.4.2rc3/obis.egg-info/requires.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        5 2023-07-17 10:23:13.000000 obis-0.4.2rc3/obis.egg-info/top_level.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       38 2023-07-17 10:23:13.806892 obis-0.4.2rc3/setup.cfg
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1985 2023-07-17 10:23:12.000000 obis-0.4.2rc3/setup.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.116191 obis-0.4.2rc4/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      773 2023-07-17 10:22:02.000000 obis-0.4.2rc4/CHANGELOG.md
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    11357 2023-02-20 13:30:53.000000 obis-0.4.2rc4/LICENSE
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      176 2023-02-20 13:30:53.000000 obis-0.4.2rc4/MANIFEST.in
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    32149 2023-07-17 10:34:37.116191 obis-0.4.2rc4/PKG-INFO
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    31587 2023-07-17 10:34:32.000000 obis-0.4.2rc4/README.md
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.096191 obis-0.4.2rc4/man/
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.100191 obis-0.4.2rc4/man/man1/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-addref.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      879 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-clone.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      798 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-collection.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      825 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-commit.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-config.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1027 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-data_set.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      893 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-download.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      757 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-init.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-init_analysis.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-move.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      762 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-object.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      617 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-removeref.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1221 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-repository.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      742 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-settings.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-status.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      666 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-sync.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1684 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis.1
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.100191 obis-0.4.2rc4/obis/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      757 2023-07-17 10:34:32.000000 obis-0.4.2rc4/obis/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.104191 obis-0.4.2rc4/obis/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      320 2023-07-17 10:26:50.000000 obis-0.4.2rc4/obis/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      563 2023-02-27 13:57:44.000000 obis-0.4.2rc4/obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      915 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/conftest.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.104191 obis-0.4.2rc4/obis/dm/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      889 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.108191 obis-0.4.2rc4/obis/dm/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      411 2023-02-21 12:13:21.000000 obis-0.4.2rc4/obis/dm/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7402 2023-03-07 09:56:22.000000 obis-0.4.2rc4/obis/dm/__pycache__/checksum.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2407 2023-02-21 12:13:22.000000 obis-0.4.2rc4/obis/dm/__pycache__/command_log.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1839 2023-02-21 12:13:21.000000 obis-0.4.2rc4/obis/dm/__pycache__/command_result.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    15644 2023-02-21 12:13:21.000000 obis-0.4.2rc4/obis/dm/__pycache__/config.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    23132 2023-03-30 13:34:10.000000 obis-0.4.2rc4/obis/dm/__pycache__/data_mgmt.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    17466 2023-03-29 13:31:59.000000 obis-0.4.2rc4/obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7101 2023-03-30 10:33:16.000000 obis-0.4.2rc4/obis/dm/__pycache__/git.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1351 2023-02-21 12:17:13.000000 obis-0.4.2rc4/obis/dm/__pycache__/repository_utils.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3148 2023-03-30 10:51:56.000000 obis-0.4.2rc4/obis/dm/__pycache__/utils.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7820 2023-03-07 08:26:10.000000 obis-0.4.2rc4/obis/dm/checksum.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2674 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/command_log.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1981 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/command_result.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.112191 obis-0.4.2rc4/obis/dm/commands/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      634 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/commands/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.112191 obis-0.4.2rc4/obis/dm/commands/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      194 2023-02-21 12:13:21.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1867 2023-03-29 14:28:25.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/addref.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3935 2023-02-28 09:09:45.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/clone.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3041 2023-02-28 09:44:21.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/collection.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3046 2023-02-21 16:35:01.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/download.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3343 2023-03-03 14:34:14.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2416 2023-02-21 12:17:13.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/move.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3263 2023-03-01 08:22:27.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/object.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    10941 2023-03-30 10:21:33.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     6680 2023-02-21 12:17:13.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3273 2023-02-21 12:17:13.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/removeref.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     8335 2023-07-17 10:14:41.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/search.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1589 2023-02-24 12:01:17.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/upload.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1897 2023-03-29 14:28:17.000000 obis-0.4.2rc4/obis/dm/commands/addref.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5292 2023-02-28 08:49:14.000000 obis-0.4.2rc4/obis/dm/commands/clone.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3657 2023-02-28 09:16:53.000000 obis-0.4.2rc4/obis/dm/commands/collection.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3920 2023-02-21 13:31:53.000000 obis-0.4.2rc4/obis/dm/commands/download.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4124 2023-03-03 14:31:58.000000 obis-0.4.2rc4/obis/dm/commands/download_physical.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2967 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/commands/move.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4373 2023-03-01 08:22:23.000000 obis-0.4.2rc4/obis/dm/commands/object.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    12135 2023-03-30 10:21:12.000000 obis-0.4.2rc4/obis/dm/commands/openbis_command.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1535 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/commands/openbis_command_test.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     9774 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/commands/openbis_sync.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3565 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/commands/removeref.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    12372 2023-07-17 10:12:16.000000 obis-0.4.2rc4/obis/dm/commands/search.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1801 2023-02-24 12:00:59.000000 obis-0.4.2rc4/obis/dm/commands/upload.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    16039 2023-02-21 12:05:42.000000 obis-0.4.2rc4/obis/dm/config.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2934 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/config_test.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    27953 2023-03-30 13:30:39.000000 obis-0.4.2rc4/obis/dm/data_mgmt.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    14376 2023-03-29 13:51:23.000000 obis-0.4.2rc4/obis/dm/data_mgmt_test.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      245 2023-02-20 13:30:53.000000 obis-0.4.2rc4/obis/dm/git-annex-attributes
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     8502 2023-03-30 10:32:13.000000 obis-0.4.2rc4/obis/dm/git.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1905 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/repository_utils.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3789 2023-03-30 10:51:34.000000 obis-0.4.2rc4/obis/dm/utils.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      980 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/utils_test.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.112191 obis-0.4.2rc4/obis/scripts/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      919 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/scripts/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.116191 obis-0.4.2rc4/obis/scripts/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      431 2023-02-21 12:13:22.000000 obis-0.4.2rc4/obis/scripts/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    30930 2023-07-17 10:14:41.000000 obis-0.4.2rc4/obis/scripts/__pycache__/cli.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-02-21 12:13:22.000000 obis-0.4.2rc4/obis/scripts/__pycache__/click_util.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4351 2023-03-30 10:59:33.000000 obis-0.4.2rc4/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    39340 2023-07-17 10:13:46.000000 obis-0.4.2rc4/obis/scripts/cli.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1126 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/scripts/click_util.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5701 2023-03-30 10:59:06.000000 obis-0.4.2rc4/obis/scripts/data_mgmt_runner.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.116191 obis-0.4.2rc4/obis/test-data/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)   160470 2023-02-20 13:30:53.000000 obis-0.4.2rc4/obis/test-data/snb-data.zip
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       43 2023-02-20 13:30:53.000000 obis-0.4.2rc4/obis/test-data/text-data-2.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       32 2023-02-20 13:30:53.000000 obis-0.4.2rc4/obis/test-data/text-data.txt
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.096191 obis-0.4.2rc4/obis/test-data/user_config/
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.116191 obis-0.4.2rc4/obis/test-data/user_config/.obis/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      167 2023-02-20 13:30:53.000000 obis-0.4.2rc4/obis/test-data/user_config/.obis/config.json
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.104191 obis-0.4.2rc4/obis.egg-info/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    32149 2023-07-17 10:34:36.000000 obis-0.4.2rc4/obis.egg-info/PKG-INFO
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3124 2023-07-17 10:34:36.000000 obis-0.4.2rc4/obis.egg-info/SOURCES.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-07-17 10:34:36.000000 obis-0.4.2rc4/obis.egg-info/dependency_links.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       47 2023-07-17 10:34:36.000000 obis-0.4.2rc4/obis.egg-info/entry_points.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-02-23 08:39:07.000000 obis-0.4.2rc4/obis.egg-info/not-zip-safe
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       37 2023-07-17 10:34:36.000000 obis-0.4.2rc4/obis.egg-info/requires.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        5 2023-07-17 10:34:36.000000 obis-0.4.2rc4/obis.egg-info/top_level.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       38 2023-07-17 10:34:37.116191 obis-0.4.2rc4/setup.cfg
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1985 2023-07-17 10:34:32.000000 obis-0.4.2rc4/setup.py
```

### Comparing `obis-0.4.2rc3/CHANGELOG.md` & `obis-0.4.2rc4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/LICENSE` & `obis-0.4.2rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/PKG-INFO` & `obis-0.4.2rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obis
-Version: 0.4.2rc3
+Version: 0.4.2rc4
 Summary: Local data management with assistance from OpenBIS.
 Home-page: https://sissource.ethz.ch/sispub/openbis/tree/master/app-openbis-command-line
 Author: ID SIS • ETH Zürich
 Author-email: openbis-support@id.ethz.ch
 License: Apache Software License Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -243,41 +243,66 @@
 
 **data_set**
 
 ```
 obis data_set search [OPTIONS]
 
 Options:
-  -object_type, --object_type TEXT              
-                                  Object type code to filter by
   -space, --space TEXT            Space code
-  -project, --project TEXT        Full project identification code
-  -experiment, --experiment TEXT  Full experiment code
-  -object, --object TEXT          Object identification information, it can be permId or identifier
-  -type, --type TEXT              Type code
+  -project, --project TEXT        Project identification code
+  -collection, --collection TEXT  Collection code
+  -id, --id TEXT                  Dataset identification information, it can
+                                  be permId or identifier
+  -type, --type TEXT              Dataset type code
+  -property TEXT                  Property code
+  -property-value TEXT            Property value
   -registration-date, --registration-date TEXT
                                   Registration date, it can be in the format
-                                  "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
   -modification-date, --modification-date TEXT
                                   Modification date, it can be in the format
-                                  "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
-  -property TEXT                  Property code
-  -property-value TEXT            Property value
-  -save, --save TEXT              Directory name to save results
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
+  -save, --save TEXT              Filename to save results
   -r, --recursive                 Search data recursively
+  
+Search by sample object parameters:  
+  -object-type, --object-type TEXT
+                                  Object type code to filter by
+  -object-space, --object-space TEXT
+                                  Object space code
+  -object-project, --object-project TEXT
+                                  Full object project identification code
+  -object-collection, --object-collection TEXT
+                                  Full object collection code
+  -object-id, --object-id TEXT    Object identification information, it can be
+                                  permId or identifier
+  -object-property TEXT           Object property code
+  -object-property-value TEXT     Object property value
+  -object-registration-date, --object-registration-date TEXT
+                                  Registration date, it can be in the format
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
+  -object-modification-date, --object-modification-date TEXT
+                                  Modification date, it can be in the format
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
+  --help                          Show this message and exit.
+
 ```
 
 With `data_set search` command, obis connects to a configured OpenBIS instance and searches for all
 data sets that fulfill given filtering criteria or by using object identification string.
 At least one search option must be specified. 
 
 Search results can be downloaded into a file by using `save` option.
 
 Recursive option enables searching for datasets of children samples or datasets
 
+-object* filtering parameters allows to search for datasets owned by objects specified by these params, 
+i.e. obis will find objects fitting these criterias (as if it was an `object search` command) and then it will extract 
+dataset data.
+
 *Note: Filtering by `-project` may not work when `Project Samples` are disabled in OpenBIS
 configuration.*
 
 **download**
 
 ```
 obis download [options] [data_set_id]
@@ -321,29 +346,31 @@
 
 **object search**
 
 ```
 obis object search [OPTIONS]
 
 Options:
-  -type, --type TEXT              Type code to filter by
   -space, --space TEXT            Space code
   -project, --project TEXT        Full project identification code
-  -experiment, --experiment TEXT  Full experiment 
-  -object, --object TEXT          Object identification information, it can be permId or identifier
+  -collection, --collection TEXT  Full collection code
+  -object, --object TEXT          Object identification information, it can be
+                                  permId or identifier
+  -type, --type TEXT              Type code
+  -property TEXT                  Property code
+  -property-value TEXT            Property value
   -registration-date, --registration-date TEXT
                                   Registration date, it can be in the format
-                                  "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
   -modification-date, --modification-date TEXT
                                   Modification date, it can be in the format
-                                  "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
-  -property TEXT                  Property code
-  -property-value TEXT            Property value
-  -save, --save TEXT              File name to save results in csv format
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
+  -save, --save TEXT              Filename to save results
   -r, --recursive                 Search data recursively
+
 ```
 
 With `object search` command, obis connects to a configured OpenBIS instance and searches for all
 objects/samples that fulfill given filtering criteria or by using object identification string.
 At least one search option must be specified. 
 
 Search results can be downloaded into a file by using `save` option.
```

### Comparing `obis-0.4.2rc3/README.md` & `obis-0.4.2rc4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -228,41 +228,66 @@
 
 **data_set**
 
 ```
 obis data_set search [OPTIONS]
 
 Options:
-  -object_type, --object_type TEXT              
-                                  Object type code to filter by
   -space, --space TEXT            Space code
-  -project, --project TEXT        Full project identification code
-  -experiment, --experiment TEXT  Full experiment code
-  -object, --object TEXT          Object identification information, it can be permId or identifier
-  -type, --type TEXT              Type code
+  -project, --project TEXT        Project identification code
+  -collection, --collection TEXT  Collection code
+  -id, --id TEXT                  Dataset identification information, it can
+                                  be permId or identifier
+  -type, --type TEXT              Dataset type code
+  -property TEXT                  Property code
+  -property-value TEXT            Property value
   -registration-date, --registration-date TEXT
                                   Registration date, it can be in the format
-                                  "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
   -modification-date, --modification-date TEXT
                                   Modification date, it can be in the format
-                                  "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
-  -property TEXT                  Property code
-  -property-value TEXT            Property value
-  -save, --save TEXT              Directory name to save results
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
+  -save, --save TEXT              Filename to save results
   -r, --recursive                 Search data recursively
+  
+Search by sample object parameters:  
+  -object-type, --object-type TEXT
+                                  Object type code to filter by
+  -object-space, --object-space TEXT
+                                  Object space code
+  -object-project, --object-project TEXT
+                                  Full object project identification code
+  -object-collection, --object-collection TEXT
+                                  Full object collection code
+  -object-id, --object-id TEXT    Object identification information, it can be
+                                  permId or identifier
+  -object-property TEXT           Object property code
+  -object-property-value TEXT     Object property value
+  -object-registration-date, --object-registration-date TEXT
+                                  Registration date, it can be in the format
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
+  -object-modification-date, --object-modification-date TEXT
+                                  Modification date, it can be in the format
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
+  --help                          Show this message and exit.
+
 ```
 
 With `data_set search` command, obis connects to a configured OpenBIS instance and searches for all
 data sets that fulfill given filtering criteria or by using object identification string.
 At least one search option must be specified. 
 
 Search results can be downloaded into a file by using `save` option.
 
 Recursive option enables searching for datasets of children samples or datasets
 
+-object* filtering parameters allows to search for datasets owned by objects specified by these params, 
+i.e. obis will find objects fitting these criterias (as if it was an `object search` command) and then it will extract 
+dataset data.
+
 *Note: Filtering by `-project` may not work when `Project Samples` are disabled in OpenBIS
 configuration.*
 
 **download**
 
 ```
 obis download [options] [data_set_id]
@@ -306,29 +331,31 @@
 
 **object search**
 
 ```
 obis object search [OPTIONS]
 
 Options:
-  -type, --type TEXT              Type code to filter by
   -space, --space TEXT            Space code
   -project, --project TEXT        Full project identification code
-  -experiment, --experiment TEXT  Full experiment 
-  -object, --object TEXT          Object identification information, it can be permId or identifier
+  -collection, --collection TEXT  Full collection code
+  -object, --object TEXT          Object identification information, it can be
+                                  permId or identifier
+  -type, --type TEXT              Type code
+  -property TEXT                  Property code
+  -property-value TEXT            Property value
   -registration-date, --registration-date TEXT
                                   Registration date, it can be in the format
-                                  "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
   -modification-date, --modification-date TEXT
                                   Modification date, it can be in the format
-                                  "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
-  -property TEXT                  Property code
-  -property-value TEXT            Property value
-  -save, --save TEXT              File name to save results in csv format
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
+  -save, --save TEXT              Filename to save results
   -r, --recursive                 Search data recursively
+
 ```
 
 With `object search` command, obis connects to a configured OpenBIS instance and searches for all
 objects/samples that fulfill given filtering criteria or by using object identification string.
 At least one search option must be specified. 
 
 Search results can be downloaded into a file by using `save` option.
```

### Comparing `obis-0.4.2rc3/man/man1/obis-addref.1` & `obis-0.4.2rc4/man/man1/obis-addref.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/man/man1/obis-clone.1` & `obis-0.4.2rc4/man/man1/obis-clone.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/man/man1/obis-collection.1` & `obis-0.4.2rc4/man/man1/obis-collection.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/man/man1/obis-commit.1` & `obis-0.4.2rc4/man/man1/obis-commit.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/man/man1/obis-config.1` & `obis-0.4.2rc4/man/man1/obis-config.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/man/man1/obis-data_set.1` & `obis-0.4.2rc4/man/man1/obis-data_set.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/man/man1/obis-download.1` & `obis-0.4.2rc4/man/man1/obis-download.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/man/man1/obis-init.1` & `obis-0.4.2rc4/man/man1/obis-init.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/man/man1/obis-init_analysis.1` & `obis-0.4.2rc4/man/man1/obis-init_analysis.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/man/man1/obis-move.1` & `obis-0.4.2rc4/man/man1/obis-move.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/man/man1/obis-object.1` & `obis-0.4.2rc4/man/man1/obis-object.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/man/man1/obis-removeref.1` & `obis-0.4.2rc4/man/man1/obis-removeref.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/man/man1/obis-repository.1` & `obis-0.4.2rc4/man/man1/obis-repository.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/man/man1/obis-settings.1` & `obis-0.4.2rc4/man/man1/obis-settings.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/man/man1/obis-status.1` & `obis-0.4.2rc4/man/man1/obis-status.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/man/man1/obis-sync.1` & `obis-0.4.2rc4/man/man1/obis-sync.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/man/man1/obis.1` & `obis-0.4.2rc4/man/man1/obis.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/__init__.py` & `obis-0.4.2rc4/obis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 __author__ = "ID SIS • ETH Zürich"
 __email__ = "openbis-support@id.ethz.ch"
-__version__ = "0.4.2rc3"
+__version__ = "0.4.2rc4"
 
 from .dm import *
```

### Comparing `obis-0.4.2rc3/obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc` & `obis-0.4.2rc4/obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/conftest.py` & `obis-0.4.2rc4/obis/conftest.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/__init__.py` & `obis-0.4.2rc4/obis/dm/__init__.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/__pycache__/checksum.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/__pycache__/checksum.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/__pycache__/command_log.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/__pycache__/command_log.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/__pycache__/command_result.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/__pycache__/command_result.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/__pycache__/config.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/__pycache__/data_mgmt.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/__pycache__/data_mgmt.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc` & `obis-0.4.2rc4/obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/__pycache__/git.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/__pycache__/git.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/__pycache__/repository_utils.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/__pycache__/repository_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/__pycache__/utils.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/checksum.py` & `obis-0.4.2rc4/obis/dm/checksum.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/command_log.py` & `obis-0.4.2rc4/obis/dm/command_log.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/command_result.py` & `obis-0.4.2rc4/obis/dm/command_result.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/__init__.py` & `obis-0.4.2rc4/obis/dm/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/__pycache__/addref.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/commands/__pycache__/addref.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/__pycache__/clone.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/commands/__pycache__/clone.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/__pycache__/collection.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/commands/__pycache__/collection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/__pycache__/download.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/commands/__pycache__/download.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/__pycache__/move.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/commands/__pycache__/move.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/__pycache__/object.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/commands/__pycache__/object.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/__pycache__/removeref.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/commands/__pycache__/removeref.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/__pycache__/search.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/commands/__pycache__/search.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/__pycache__/upload.cpython-310.pyc` & `obis-0.4.2rc4/obis/dm/commands/__pycache__/upload.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/addref.py` & `obis-0.4.2rc4/obis/dm/commands/addref.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/clone.py` & `obis-0.4.2rc4/obis/dm/commands/clone.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/collection.py` & `obis-0.4.2rc4/obis/dm/commands/collection.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/download.py` & `obis-0.4.2rc4/obis/dm/commands/download.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/download_physical.py` & `obis-0.4.2rc4/obis/dm/commands/download_physical.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/move.py` & `obis-0.4.2rc4/obis/dm/commands/move.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/object.py` & `obis-0.4.2rc4/obis/dm/commands/object.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/openbis_command.py` & `obis-0.4.2rc4/obis/dm/commands/openbis_command.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/openbis_command_test.py` & `obis-0.4.2rc4/obis/dm/commands/openbis_command_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/openbis_sync.py` & `obis-0.4.2rc4/obis/dm/commands/openbis_sync.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/removeref.py` & `obis-0.4.2rc4/obis/dm/commands/removeref.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/search.py` & `obis-0.4.2rc4/obis/dm/commands/search.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/commands/upload.py` & `obis-0.4.2rc4/obis/dm/commands/upload.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/config.py` & `obis-0.4.2rc4/obis/dm/config.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/config_test.py` & `obis-0.4.2rc4/obis/dm/config_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/data_mgmt.py` & `obis-0.4.2rc4/obis/dm/data_mgmt.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/data_mgmt_test.py` & `obis-0.4.2rc4/obis/dm/data_mgmt_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/git.py` & `obis-0.4.2rc4/obis/dm/git.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/repository_utils.py` & `obis-0.4.2rc4/obis/dm/repository_utils.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/utils.py` & `obis-0.4.2rc4/obis/dm/utils.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/dm/utils_test.py` & `obis-0.4.2rc4/obis/dm/utils_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/scripts/__init__.py` & `obis-0.4.2rc4/obis/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/scripts/__pycache__/cli.cpython-310.pyc` & `obis-0.4.2rc4/obis/scripts/__pycache__/cli.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/scripts/__pycache__/click_util.cpython-310.pyc` & `obis-0.4.2rc4/obis/scripts/__pycache__/click_util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc` & `obis-0.4.2rc4/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/scripts/cli.py` & `obis-0.4.2rc4/obis/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/scripts/click_util.py` & `obis-0.4.2rc4/obis/scripts/click_util.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/scripts/data_mgmt_runner.py` & `obis-0.4.2rc4/obis/scripts/data_mgmt_runner.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis/test-data/snb-data.zip` & `obis-0.4.2rc4/obis/test-data/snb-data.zip`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/obis.egg-info/PKG-INFO` & `obis-0.4.2rc4/obis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obis
-Version: 0.4.2rc3
+Version: 0.4.2rc4
 Summary: Local data management with assistance from OpenBIS.
 Home-page: https://sissource.ethz.ch/sispub/openbis/tree/master/app-openbis-command-line
 Author: ID SIS • ETH Zürich
 Author-email: openbis-support@id.ethz.ch
 License: Apache Software License Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -243,41 +243,66 @@
 
 **data_set**
 
 ```
 obis data_set search [OPTIONS]
 
 Options:
-  -object_type, --object_type TEXT              
-                                  Object type code to filter by
   -space, --space TEXT            Space code
-  -project, --project TEXT        Full project identification code
-  -experiment, --experiment TEXT  Full experiment code
-  -object, --object TEXT          Object identification information, it can be permId or identifier
-  -type, --type TEXT              Type code
+  -project, --project TEXT        Project identification code
+  -collection, --collection TEXT  Collection code
+  -id, --id TEXT                  Dataset identification information, it can
+                                  be permId or identifier
+  -type, --type TEXT              Dataset type code
+  -property TEXT                  Property code
+  -property-value TEXT            Property value
   -registration-date, --registration-date TEXT
                                   Registration date, it can be in the format
-                                  "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
   -modification-date, --modification-date TEXT
                                   Modification date, it can be in the format
-                                  "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
-  -property TEXT                  Property code
-  -property-value TEXT            Property value
-  -save, --save TEXT              Directory name to save results
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
+  -save, --save TEXT              Filename to save results
   -r, --recursive                 Search data recursively
+  
+Search by sample object parameters:  
+  -object-type, --object-type TEXT
+                                  Object type code to filter by
+  -object-space, --object-space TEXT
+                                  Object space code
+  -object-project, --object-project TEXT
+                                  Full object project identification code
+  -object-collection, --object-collection TEXT
+                                  Full object collection code
+  -object-id, --object-id TEXT    Object identification information, it can be
+                                  permId or identifier
+  -object-property TEXT           Object property code
+  -object-property-value TEXT     Object property value
+  -object-registration-date, --object-registration-date TEXT
+                                  Registration date, it can be in the format
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
+  -object-modification-date, --object-modification-date TEXT
+                                  Modification date, it can be in the format
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
+  --help                          Show this message and exit.
+
 ```
 
 With `data_set search` command, obis connects to a configured OpenBIS instance and searches for all
 data sets that fulfill given filtering criteria or by using object identification string.
 At least one search option must be specified. 
 
 Search results can be downloaded into a file by using `save` option.
 
 Recursive option enables searching for datasets of children samples or datasets
 
+-object* filtering parameters allows to search for datasets owned by objects specified by these params, 
+i.e. obis will find objects fitting these criterias (as if it was an `object search` command) and then it will extract 
+dataset data.
+
 *Note: Filtering by `-project` may not work when `Project Samples` are disabled in OpenBIS
 configuration.*
 
 **download**
 
 ```
 obis download [options] [data_set_id]
@@ -321,29 +346,31 @@
 
 **object search**
 
 ```
 obis object search [OPTIONS]
 
 Options:
-  -type, --type TEXT              Type code to filter by
   -space, --space TEXT            Space code
   -project, --project TEXT        Full project identification code
-  -experiment, --experiment TEXT  Full experiment 
-  -object, --object TEXT          Object identification information, it can be permId or identifier
+  -collection, --collection TEXT  Full collection code
+  -object, --object TEXT          Object identification information, it can be
+                                  permId or identifier
+  -type, --type TEXT              Type code
+  -property TEXT                  Property code
+  -property-value TEXT            Property value
   -registration-date, --registration-date TEXT
                                   Registration date, it can be in the format
-                                  "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
   -modification-date, --modification-date TEXT
                                   Modification date, it can be in the format
-                                  "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
-  -property TEXT                  Property code
-  -property-value TEXT            Property value
-  -save, --save TEXT              File name to save results in csv format
+                                  "oYYYY-MM-DD" (e.g. ">2023-01-01")
+  -save, --save TEXT              Filename to save results
   -r, --recursive                 Search data recursively
+
 ```
 
 With `object search` command, obis connects to a configured OpenBIS instance and searches for all
 objects/samples that fulfill given filtering criteria or by using object identification string.
 At least one search option must be specified. 
 
 Search results can be downloaded into a file by using `save` option.
```

### Comparing `obis-0.4.2rc3/obis.egg-info/SOURCES.txt` & `obis-0.4.2rc4/obis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc3/setup.py` & `obis-0.4.2rc4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 data_dir = os.path.join("man", "man1")
 data_files = [
     (d, [os.path.join(d, f) for f in files]) for d, folders, files in os.walk(data_dir)
 ]
 
 setup(
     name="obis",
-    version="0.4.2rc3",
+    version="0.4.2rc4",
     description="Local data management with assistance from OpenBIS.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://sissource.ethz.ch/sispub/openbis/tree/master/app-openbis-command-line",
     author="ID SIS • ETH Zürich",
     author_email="openbis-support@id.ethz.ch",
     license="Apache Software License Version 2.0",
```

