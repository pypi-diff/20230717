# Comparing `tmp/obis-0.4.2rc4.tar.gz` & `tmp/obis-0.4.2rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obis-0.4.2rc4.tar", last modified: Mon Jul 17 10:34:37 2023, max compression
+gzip compressed data, was "obis-0.4.2rc5.tar", last modified: Mon Jul 17 15:17:19 2023, max compression
```

## Comparing `obis-0.4.2rc4.tar` & `obis-0.4.2rc5.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.116191 obis-0.4.2rc4/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      773 2023-07-17 10:22:02.000000 obis-0.4.2rc4/CHANGELOG.md
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    11357 2023-02-20 13:30:53.000000 obis-0.4.2rc4/LICENSE
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      176 2023-02-20 13:30:53.000000 obis-0.4.2rc4/MANIFEST.in
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    32149 2023-07-17 10:34:37.116191 obis-0.4.2rc4/PKG-INFO
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    31587 2023-07-17 10:34:32.000000 obis-0.4.2rc4/README.md
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.096191 obis-0.4.2rc4/man/
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.100191 obis-0.4.2rc4/man/man1/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-addref.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      879 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-clone.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      798 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-collection.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      825 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-commit.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-config.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1027 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-data_set.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      893 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-download.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      757 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-init.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-init_analysis.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-move.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      762 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-object.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      617 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-removeref.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1221 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-repository.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      742 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-settings.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-status.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      666 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis-sync.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1684 2023-02-20 13:30:53.000000 obis-0.4.2rc4/man/man1/obis.1
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.100191 obis-0.4.2rc4/obis/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      757 2023-07-17 10:34:32.000000 obis-0.4.2rc4/obis/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.104191 obis-0.4.2rc4/obis/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      320 2023-07-17 10:26:50.000000 obis-0.4.2rc4/obis/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      563 2023-02-27 13:57:44.000000 obis-0.4.2rc4/obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      915 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/conftest.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.104191 obis-0.4.2rc4/obis/dm/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      889 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.108191 obis-0.4.2rc4/obis/dm/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      411 2023-02-21 12:13:21.000000 obis-0.4.2rc4/obis/dm/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7402 2023-03-07 09:56:22.000000 obis-0.4.2rc4/obis/dm/__pycache__/checksum.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2407 2023-02-21 12:13:22.000000 obis-0.4.2rc4/obis/dm/__pycache__/command_log.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1839 2023-02-21 12:13:21.000000 obis-0.4.2rc4/obis/dm/__pycache__/command_result.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    15644 2023-02-21 12:13:21.000000 obis-0.4.2rc4/obis/dm/__pycache__/config.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    23132 2023-03-30 13:34:10.000000 obis-0.4.2rc4/obis/dm/__pycache__/data_mgmt.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    17466 2023-03-29 13:31:59.000000 obis-0.4.2rc4/obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7101 2023-03-30 10:33:16.000000 obis-0.4.2rc4/obis/dm/__pycache__/git.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1351 2023-02-21 12:17:13.000000 obis-0.4.2rc4/obis/dm/__pycache__/repository_utils.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3148 2023-03-30 10:51:56.000000 obis-0.4.2rc4/obis/dm/__pycache__/utils.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7820 2023-03-07 08:26:10.000000 obis-0.4.2rc4/obis/dm/checksum.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2674 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/command_log.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1981 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/command_result.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.112191 obis-0.4.2rc4/obis/dm/commands/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      634 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/commands/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.112191 obis-0.4.2rc4/obis/dm/commands/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      194 2023-02-21 12:13:21.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1867 2023-03-29 14:28:25.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/addref.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3935 2023-02-28 09:09:45.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/clone.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3041 2023-02-28 09:44:21.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/collection.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3046 2023-02-21 16:35:01.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/download.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3343 2023-03-03 14:34:14.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2416 2023-02-21 12:17:13.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/move.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3263 2023-03-01 08:22:27.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/object.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    10941 2023-03-30 10:21:33.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     6680 2023-02-21 12:17:13.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3273 2023-02-21 12:17:13.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/removeref.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     8335 2023-07-17 10:14:41.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/search.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1589 2023-02-24 12:01:17.000000 obis-0.4.2rc4/obis/dm/commands/__pycache__/upload.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1897 2023-03-29 14:28:17.000000 obis-0.4.2rc4/obis/dm/commands/addref.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5292 2023-02-28 08:49:14.000000 obis-0.4.2rc4/obis/dm/commands/clone.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3657 2023-02-28 09:16:53.000000 obis-0.4.2rc4/obis/dm/commands/collection.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3920 2023-02-21 13:31:53.000000 obis-0.4.2rc4/obis/dm/commands/download.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4124 2023-03-03 14:31:58.000000 obis-0.4.2rc4/obis/dm/commands/download_physical.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2967 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/commands/move.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4373 2023-03-01 08:22:23.000000 obis-0.4.2rc4/obis/dm/commands/object.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    12135 2023-03-30 10:21:12.000000 obis-0.4.2rc4/obis/dm/commands/openbis_command.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1535 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/commands/openbis_command_test.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     9774 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/commands/openbis_sync.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3565 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/commands/removeref.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    12372 2023-07-17 10:12:16.000000 obis-0.4.2rc4/obis/dm/commands/search.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1801 2023-02-24 12:00:59.000000 obis-0.4.2rc4/obis/dm/commands/upload.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    16039 2023-02-21 12:05:42.000000 obis-0.4.2rc4/obis/dm/config.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2934 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/config_test.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    27953 2023-03-30 13:30:39.000000 obis-0.4.2rc4/obis/dm/data_mgmt.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    14376 2023-03-29 13:51:23.000000 obis-0.4.2rc4/obis/dm/data_mgmt_test.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      245 2023-02-20 13:30:53.000000 obis-0.4.2rc4/obis/dm/git-annex-attributes
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     8502 2023-03-30 10:32:13.000000 obis-0.4.2rc4/obis/dm/git.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1905 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/repository_utils.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3789 2023-03-30 10:51:34.000000 obis-0.4.2rc4/obis/dm/utils.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      980 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/dm/utils_test.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.112191 obis-0.4.2rc4/obis/scripts/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      919 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/scripts/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.116191 obis-0.4.2rc4/obis/scripts/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      431 2023-02-21 12:13:22.000000 obis-0.4.2rc4/obis/scripts/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    30930 2023-07-17 10:14:41.000000 obis-0.4.2rc4/obis/scripts/__pycache__/cli.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-02-21 12:13:22.000000 obis-0.4.2rc4/obis/scripts/__pycache__/click_util.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4351 2023-03-30 10:59:33.000000 obis-0.4.2rc4/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    39340 2023-07-17 10:13:46.000000 obis-0.4.2rc4/obis/scripts/cli.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1126 2023-02-21 12:05:41.000000 obis-0.4.2rc4/obis/scripts/click_util.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5701 2023-03-30 10:59:06.000000 obis-0.4.2rc4/obis/scripts/data_mgmt_runner.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.116191 obis-0.4.2rc4/obis/test-data/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)   160470 2023-02-20 13:30:53.000000 obis-0.4.2rc4/obis/test-data/snb-data.zip
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       43 2023-02-20 13:30:53.000000 obis-0.4.2rc4/obis/test-data/text-data-2.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       32 2023-02-20 13:30:53.000000 obis-0.4.2rc4/obis/test-data/text-data.txt
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.096191 obis-0.4.2rc4/obis/test-data/user_config/
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.116191 obis-0.4.2rc4/obis/test-data/user_config/.obis/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      167 2023-02-20 13:30:53.000000 obis-0.4.2rc4/obis/test-data/user_config/.obis/config.json
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 10:34:37.104191 obis-0.4.2rc4/obis.egg-info/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    32149 2023-07-17 10:34:36.000000 obis-0.4.2rc4/obis.egg-info/PKG-INFO
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3124 2023-07-17 10:34:36.000000 obis-0.4.2rc4/obis.egg-info/SOURCES.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-07-17 10:34:36.000000 obis-0.4.2rc4/obis.egg-info/dependency_links.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       47 2023-07-17 10:34:36.000000 obis-0.4.2rc4/obis.egg-info/entry_points.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-02-23 08:39:07.000000 obis-0.4.2rc4/obis.egg-info/not-zip-safe
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       37 2023-07-17 10:34:36.000000 obis-0.4.2rc4/obis.egg-info/requires.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        5 2023-07-17 10:34:36.000000 obis-0.4.2rc4/obis.egg-info/top_level.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       38 2023-07-17 10:34:37.116191 obis-0.4.2rc4/setup.cfg
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1985 2023-07-17 10:34:32.000000 obis-0.4.2rc4/setup.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 15:17:19.467440 obis-0.4.2rc5/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      774 2023-07-17 15:13:38.000000 obis-0.4.2rc5/CHANGELOG.md
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    11357 2023-02-20 13:30:53.000000 obis-0.4.2rc5/LICENSE
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      176 2023-02-20 13:30:53.000000 obis-0.4.2rc5/MANIFEST.in
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    32149 2023-07-17 15:17:19.467440 obis-0.4.2rc5/PKG-INFO
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    31587 2023-07-17 10:34:32.000000 obis-0.4.2rc5/README.md
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 15:17:19.451439 obis-0.4.2rc5/man/
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 15:17:19.455439 obis-0.4.2rc5/man/man1/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.2rc5/man/man1/obis-addref.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      879 2023-02-20 13:30:53.000000 obis-0.4.2rc5/man/man1/obis-clone.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      798 2023-02-20 13:30:53.000000 obis-0.4.2rc5/man/man1/obis-collection.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      825 2023-02-20 13:30:53.000000 obis-0.4.2rc5/man/man1/obis-commit.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-02-20 13:30:53.000000 obis-0.4.2rc5/man/man1/obis-config.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1027 2023-02-20 13:30:53.000000 obis-0.4.2rc5/man/man1/obis-data_set.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      893 2023-02-20 13:30:53.000000 obis-0.4.2rc5/man/man1/obis-download.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      757 2023-02-20 13:30:53.000000 obis-0.4.2rc5/man/man1/obis-init.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.2rc5/man/man1/obis-init_analysis.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.2rc5/man/man1/obis-move.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      762 2023-02-20 13:30:53.000000 obis-0.4.2rc5/man/man1/obis-object.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      617 2023-02-20 13:30:53.000000 obis-0.4.2rc5/man/man1/obis-removeref.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1221 2023-02-20 13:30:53.000000 obis-0.4.2rc5/man/man1/obis-repository.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      742 2023-02-20 13:30:53.000000 obis-0.4.2rc5/man/man1/obis-settings.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.2rc5/man/man1/obis-status.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      666 2023-02-20 13:30:53.000000 obis-0.4.2rc5/man/man1/obis-sync.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1684 2023-02-20 13:30:53.000000 obis-0.4.2rc5/man/man1/obis.1
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 15:17:19.455439 obis-0.4.2rc5/obis/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      757 2023-07-17 15:15:50.000000 obis-0.4.2rc5/obis/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 15:17:19.459440 obis-0.4.2rc5/obis/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      320 2023-07-17 14:48:24.000000 obis-0.4.2rc5/obis/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      563 2023-02-27 13:57:44.000000 obis-0.4.2rc5/obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      915 2023-02-21 12:05:41.000000 obis-0.4.2rc5/obis/conftest.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 15:17:19.459440 obis-0.4.2rc5/obis/dm/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      889 2023-02-21 12:05:41.000000 obis-0.4.2rc5/obis/dm/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 15:17:19.459440 obis-0.4.2rc5/obis/dm/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      411 2023-02-21 12:13:21.000000 obis-0.4.2rc5/obis/dm/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7402 2023-03-07 09:56:22.000000 obis-0.4.2rc5/obis/dm/__pycache__/checksum.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2407 2023-02-21 12:13:22.000000 obis-0.4.2rc5/obis/dm/__pycache__/command_log.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1839 2023-02-21 12:13:21.000000 obis-0.4.2rc5/obis/dm/__pycache__/command_result.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    15644 2023-02-21 12:13:21.000000 obis-0.4.2rc5/obis/dm/__pycache__/config.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    23132 2023-03-30 13:34:10.000000 obis-0.4.2rc5/obis/dm/__pycache__/data_mgmt.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    17466 2023-07-17 14:48:25.000000 obis-0.4.2rc5/obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7101 2023-03-30 10:33:16.000000 obis-0.4.2rc5/obis/dm/__pycache__/git.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1351 2023-02-21 12:17:13.000000 obis-0.4.2rc5/obis/dm/__pycache__/repository_utils.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3148 2023-03-30 10:51:56.000000 obis-0.4.2rc5/obis/dm/__pycache__/utils.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7820 2023-03-07 08:26:10.000000 obis-0.4.2rc5/obis/dm/checksum.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2674 2023-02-21 12:05:41.000000 obis-0.4.2rc5/obis/dm/command_log.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1981 2023-02-21 12:05:41.000000 obis-0.4.2rc5/obis/dm/command_result.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 15:17:19.463440 obis-0.4.2rc5/obis/dm/commands/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      634 2023-02-21 12:05:41.000000 obis-0.4.2rc5/obis/dm/commands/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 15:17:19.463440 obis-0.4.2rc5/obis/dm/commands/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      194 2023-02-21 12:13:21.000000 obis-0.4.2rc5/obis/dm/commands/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1867 2023-03-29 14:28:25.000000 obis-0.4.2rc5/obis/dm/commands/__pycache__/addref.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3935 2023-02-28 09:09:45.000000 obis-0.4.2rc5/obis/dm/commands/__pycache__/clone.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3041 2023-02-28 09:44:21.000000 obis-0.4.2rc5/obis/dm/commands/__pycache__/collection.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3046 2023-02-21 16:35:01.000000 obis-0.4.2rc5/obis/dm/commands/__pycache__/download.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3343 2023-03-03 14:34:14.000000 obis-0.4.2rc5/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2416 2023-02-21 12:17:13.000000 obis-0.4.2rc5/obis/dm/commands/__pycache__/move.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3263 2023-03-01 08:22:27.000000 obis-0.4.2rc5/obis/dm/commands/__pycache__/object.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    10941 2023-03-30 10:21:33.000000 obis-0.4.2rc5/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     6680 2023-02-21 12:17:13.000000 obis-0.4.2rc5/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3273 2023-02-21 12:17:13.000000 obis-0.4.2rc5/obis/dm/commands/__pycache__/removeref.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     8335 2023-07-17 10:14:41.000000 obis-0.4.2rc5/obis/dm/commands/__pycache__/search.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1589 2023-02-24 12:01:17.000000 obis-0.4.2rc5/obis/dm/commands/__pycache__/upload.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1897 2023-03-29 14:28:17.000000 obis-0.4.2rc5/obis/dm/commands/addref.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5292 2023-02-28 08:49:14.000000 obis-0.4.2rc5/obis/dm/commands/clone.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3657 2023-02-28 09:16:53.000000 obis-0.4.2rc5/obis/dm/commands/collection.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3920 2023-02-21 13:31:53.000000 obis-0.4.2rc5/obis/dm/commands/download.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4124 2023-03-03 14:31:58.000000 obis-0.4.2rc5/obis/dm/commands/download_physical.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2967 2023-02-21 12:05:41.000000 obis-0.4.2rc5/obis/dm/commands/move.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4373 2023-03-01 08:22:23.000000 obis-0.4.2rc5/obis/dm/commands/object.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    12135 2023-03-30 10:21:12.000000 obis-0.4.2rc5/obis/dm/commands/openbis_command.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1535 2023-02-21 12:05:41.000000 obis-0.4.2rc5/obis/dm/commands/openbis_command_test.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     9774 2023-02-21 12:05:41.000000 obis-0.4.2rc5/obis/dm/commands/openbis_sync.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3565 2023-02-21 12:05:41.000000 obis-0.4.2rc5/obis/dm/commands/removeref.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    12372 2023-07-17 10:12:16.000000 obis-0.4.2rc5/obis/dm/commands/search.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1801 2023-02-24 12:00:59.000000 obis-0.4.2rc5/obis/dm/commands/upload.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    16039 2023-02-21 12:05:42.000000 obis-0.4.2rc5/obis/dm/config.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2934 2023-02-21 12:05:41.000000 obis-0.4.2rc5/obis/dm/config_test.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    27953 2023-03-30 13:30:39.000000 obis-0.4.2rc5/obis/dm/data_mgmt.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    14376 2023-03-29 13:51:23.000000 obis-0.4.2rc5/obis/dm/data_mgmt_test.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      245 2023-02-20 13:30:53.000000 obis-0.4.2rc5/obis/dm/git-annex-attributes
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     8502 2023-03-30 10:32:13.000000 obis-0.4.2rc5/obis/dm/git.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1905 2023-02-21 12:05:41.000000 obis-0.4.2rc5/obis/dm/repository_utils.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3789 2023-03-30 10:51:34.000000 obis-0.4.2rc5/obis/dm/utils.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      980 2023-02-21 12:05:41.000000 obis-0.4.2rc5/obis/dm/utils_test.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 15:17:19.463440 obis-0.4.2rc5/obis/scripts/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      919 2023-02-21 12:05:41.000000 obis-0.4.2rc5/obis/scripts/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 15:17:19.467440 obis-0.4.2rc5/obis/scripts/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      431 2023-02-21 12:13:22.000000 obis-0.4.2rc5/obis/scripts/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    30930 2023-07-17 10:14:41.000000 obis-0.4.2rc5/obis/scripts/__pycache__/cli.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-02-21 12:13:22.000000 obis-0.4.2rc5/obis/scripts/__pycache__/click_util.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4351 2023-03-30 10:59:33.000000 obis-0.4.2rc5/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    39340 2023-07-17 10:13:46.000000 obis-0.4.2rc5/obis/scripts/cli.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1126 2023-02-21 12:05:41.000000 obis-0.4.2rc5/obis/scripts/click_util.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5701 2023-03-30 10:59:06.000000 obis-0.4.2rc5/obis/scripts/data_mgmt_runner.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 15:17:19.467440 obis-0.4.2rc5/obis/test-data/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)   160470 2023-02-20 13:30:53.000000 obis-0.4.2rc5/obis/test-data/snb-data.zip
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       43 2023-02-20 13:30:53.000000 obis-0.4.2rc5/obis/test-data/text-data-2.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       32 2023-02-20 13:30:53.000000 obis-0.4.2rc5/obis/test-data/text-data.txt
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 15:17:19.451439 obis-0.4.2rc5/obis/test-data/user_config/
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 15:17:19.467440 obis-0.4.2rc5/obis/test-data/user_config/.obis/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      167 2023-02-20 13:30:53.000000 obis-0.4.2rc5/obis/test-data/user_config/.obis/config.json
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-07-17 15:17:19.455439 obis-0.4.2rc5/obis.egg-info/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    32149 2023-07-17 15:17:19.000000 obis-0.4.2rc5/obis.egg-info/PKG-INFO
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3124 2023-07-17 15:17:19.000000 obis-0.4.2rc5/obis.egg-info/SOURCES.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-07-17 15:17:19.000000 obis-0.4.2rc5/obis.egg-info/dependency_links.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       47 2023-07-17 15:17:19.000000 obis-0.4.2rc5/obis.egg-info/entry_points.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-02-23 08:39:07.000000 obis-0.4.2rc5/obis.egg-info/not-zip-safe
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       38 2023-07-17 15:17:19.000000 obis-0.4.2rc5/obis.egg-info/requires.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        5 2023-07-17 15:17:19.000000 obis-0.4.2rc5/obis.egg-info/top_level.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       38 2023-07-17 15:17:19.467440 obis-0.4.2rc5/setup.cfg
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1986 2023-07-17 15:13:38.000000 obis-0.4.2rc5/setup.py
```

### Comparing `obis-0.4.2rc4/CHANGELOG.md` & `obis-0.4.2rc5/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # New in version 0.4.2
 
 * Added filtering by object in object and data_set search commands
 * Added recursive search to object and data_set search commands
 * Updated documentation regarding authentication
 * Added dataset ids to sample search results
-* changed pybis dependency to version == 1.35.9
+* changed pybis dependency to version == 1.35.10
 
 # New in version 0.4.1
 
 * Fixed parameters for determine_hostname method in addref functionality 
 
 # New in version 0.4.0.1
```

### Comparing `obis-0.4.2rc4/LICENSE` & `obis-0.4.2rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/PKG-INFO` & `obis-0.4.2rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obis
-Version: 0.4.2rc4
+Version: 0.4.2rc5
 Summary: Local data management with assistance from OpenBIS.
 Home-page: https://sissource.ethz.ch/sispub/openbis/tree/master/app-openbis-command-line
 Author: ID SIS • ETH Zürich
 Author-email: openbis-support@id.ethz.ch
 License: Apache Software License Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `obis-0.4.2rc4/README.md` & `obis-0.4.2rc5/README.md`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/man/man1/obis-addref.1` & `obis-0.4.2rc5/man/man1/obis-addref.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/man/man1/obis-clone.1` & `obis-0.4.2rc5/man/man1/obis-clone.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/man/man1/obis-collection.1` & `obis-0.4.2rc5/man/man1/obis-collection.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/man/man1/obis-commit.1` & `obis-0.4.2rc5/man/man1/obis-commit.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/man/man1/obis-config.1` & `obis-0.4.2rc5/man/man1/obis-config.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/man/man1/obis-data_set.1` & `obis-0.4.2rc5/man/man1/obis-data_set.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/man/man1/obis-download.1` & `obis-0.4.2rc5/man/man1/obis-download.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/man/man1/obis-init.1` & `obis-0.4.2rc5/man/man1/obis-init.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/man/man1/obis-init_analysis.1` & `obis-0.4.2rc5/man/man1/obis-init_analysis.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/man/man1/obis-move.1` & `obis-0.4.2rc5/man/man1/obis-move.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/man/man1/obis-object.1` & `obis-0.4.2rc5/man/man1/obis-object.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/man/man1/obis-removeref.1` & `obis-0.4.2rc5/man/man1/obis-removeref.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/man/man1/obis-repository.1` & `obis-0.4.2rc5/man/man1/obis-repository.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/man/man1/obis-settings.1` & `obis-0.4.2rc5/man/man1/obis-settings.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/man/man1/obis-status.1` & `obis-0.4.2rc5/man/man1/obis-status.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/man/man1/obis-sync.1` & `obis-0.4.2rc5/man/man1/obis-sync.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/man/man1/obis.1` & `obis-0.4.2rc5/man/man1/obis.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/__init__.py` & `obis-0.4.2rc5/obis/__init__.py`

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
-__version__ = "0.4.2rc4"
+__version__ = "0.4.2rc5"
 
 from .dm import *
```

### Comparing `obis-0.4.2rc4/obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc` & `obis-0.4.2rc5/obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/conftest.py` & `obis-0.4.2rc5/obis/conftest.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/__init__.py` & `obis-0.4.2rc5/obis/dm/__init__.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/__pycache__/checksum.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/__pycache__/checksum.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/__pycache__/command_log.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/__pycache__/command_log.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/__pycache__/command_result.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/__pycache__/command_result.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/__pycache__/config.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/__pycache__/data_mgmt.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/__pycache__/data_mgmt.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc` & `obis-0.4.2rc5/obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Mar 29 13:31:41 2023 UTC, .py size: 14376 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 bd3d 2464 2838 0000  o........=$d(8..
+00000000: 6f0d 0d0a 0000 0000 5b42 2464 2838 0000  o.......[B$d(8..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5201 0000 6400  .....@...sR...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 0200 0100 6d05 5a06 0100 6401 6402  m.....m.Z...d.d.
 00000050: 6c07 5a07 6401 6402 6c08 5a08 6401 6402  l.Z.d.d.l.Z.d.d.
 00000060: 6c09 5a09 6401 6402 6c0a 5a0a 6401 6402  l.Z.d.d.l.Z.d.d.
 00000070: 6c0b 5a0b 6401 6402 6c0c 5a0c 6401 6403  l.Z.d.d.l.Z.d.d.
@@ -608,57 +608,57 @@
 000025f0: 0000 4300 0000 73c2 0200 0074 007c 0083  ..C...s....t.|..
 00002600: 017d 0174 01a0 027c 01a1 0190 018f 4c01  .}.t...|......L.
 00002610: 0074 037c 0183 017d 0274 047c 0283 0101  .t.|...}.t.|....
 00002620: 0074 01a0 057c 02a1 017d 0374 067c 0283  .t...|...}.t.|..
 00002630: 0101 007c 03a0 07a1 007d 0474 08a0 09a1  ...|.....}.t....
 00002640: 007d 057c 03a0 0aa1 007d 067c 036a 0ba0  .}.|.....}.|.j..
 00002650: 0ca1 007d 077c 076a 0d7d 087c 0883 007d  ...}.|.j.}.|...}
-00002660: 0964 017d 0a7c 097c 0a6b 027d 0b7c 0b73  .d.}.|.|.k.}.|.s
+00002660: 0964 017d 0a7c 097c 0a75 007d 0b7c 0b73  .d.}.|.|.u.}.|.s
 00002670: 7374 0ea0 0f64 027c 0b66 0164 037c 097c  st...d.|.f.d.|.|
 00002680: 0a66 02a1 0464 0474 10a0 11a1 0076 0073  .f...d.t.....v.s
 00002690: 5074 0ea0 127c 07a1 0172 5574 0ea0 137c  Pt...|...rUt...|
 000026a0: 07a1 016e 0164 0474 0ea0 137c 08a1 0174  ...n.d.t...|...t
 000026b0: 0ea0 137c 09a1 0174 0ea0 137c 0aa1 0164  ...|...t...|...d
 000026c0: 059c 0416 007d 0c64 0664 077c 0c69 0116  .....}.d.d.|.i..
 000026d0: 007d 0d74 1474 0ea0 157c 0da1 0183 0182  .}.t.t...|......
 000026e0: 0164 0004 007d 0804 007d 0904 007d 0b7d  .d...}...}...}.}
 000026f0: 0a7c 036a 0ba0 16a1 007d 077c 076a 0d7d  .|.j.....}.|.j.}
-00002700: 087c 0883 007d 0964 017d 0a7c 097c 0a6b  .|...}.d.}.|.|.k
-00002710: 027d 0b7c 0b73 c674 0ea0 0f64 027c 0b66  .}.|.s.t...d.|.f
+00002700: 087c 0883 007d 0964 017d 0a7c 097c 0a75  .|...}.d.}.|.|.u
+00002710: 007d 0b7c 0b73 c674 0ea0 0f64 027c 0b66  .}.|.s.t...d.|.f
 00002720: 0164 037c 097c 0a66 02a1 0464 0474 10a0  .d.|.|.f...d.t..
 00002730: 11a1 0076 0073 a374 0ea0 127c 07a1 0172  ...v.s.t...|...r
 00002740: a874 0ea0 137c 07a1 016e 0164 0474 0ea0  .t...|...n.d.t..
 00002750: 137c 08a1 0174 0ea0 137c 09a1 0174 0ea0  .|...t...|...t..
 00002760: 137c 0aa1 0164 059c 0416 007d 0c64 0664  .|...d.....}.d.d
 00002770: 077c 0c69 0116 007d 0d74 1474 0ea0 157c  .|.i...}.t.t...|
 00002780: 0da1 0183 0182 0164 0004 007d 0804 007d  .......d...}...}
 00002790: 0904 007d 0b7d 0a74 176a 18a0 197c 076a  ...}.}.t.j...|.j
 000027a0: 1aa1 015c 027d 0e7d 0f74 1ba0 1c7c 0ea0  ...\.}.}.t...|..
 000027b0: 1d64 08a1 01a1 01a0 1ea1 0064 0964 0a85  .d.........d.d..
 000027c0: 0219 007d 107c 0664 0075 0072 f264 0ba0  ...}.|.d.u.r.d..
 000027d0: 1f7c 047c 057c 10a1 03a0 20a1 007d 067c  .|.|.|.... ..}.|
 000027e0: 03a0 21a1 007d 077c 076a 0d7d 087c 0883  ..!..}.|.j.}.|..
-000027f0: 007d 0964 017d 0a7c 097c 0a6b 027d 0b7c  .}.d.}.|.|.k.}.|
+000027f0: 007d 0964 017d 0a7c 097c 0a75 007d 0b7c  .}.d.}.|.|.u.}.|
 00002800: 0b90 0173 3f74 0ea0 0f64 027c 0b66 0164  ...s?t...d.|.f.d
 00002810: 037c 097c 0a66 02a1 0464 0474 10a0 11a1  .|.|.f...d.t....
 00002820: 0076 0090 0173 1c74 0ea0 127c 07a1 0190  .v...s.t...|....
 00002830: 0172 2174 0ea0 137c 07a1 016e 0164 0474  .r!t...|...n.d.t
 00002840: 0ea0 137c 08a1 0174 0ea0 137c 09a1 0174  ...|...t...|...t
 00002850: 0ea0 137c 0aa1 0164 059c 0416 007d 0c64  ...|...d.....}.d
 00002860: 0664 077c 0c69 0116 007d 0d74 1474 0ea0  .d.|.i...}.t.t..
 00002870: 157c 0da1 0183 0182 0164 0004 007d 0804  .|.......d...}..
 00002880: 007d 0904 007d 0b7d 0a7c 026a 226a 23a0  .}...}.}.|.j"j#.
 00002890: 247c 06a1 0101 0057 0064 0004 0004 0083  $|.....W.d......
 000028a0: 0301 0064 0053 0031 0090 0173 5a77 0101  ...d.S.1...sZw..
 000028b0: 0001 0001 0059 0001 0064 0053 0029 0c4e  .....Y...d.S.).N
-000028c0: 4672 6200 0000 2901 7a46 2528 7079 3429  Frb...).zF%(py4)
+000028c0: 4672 5d00 0000 2901 7a46 2528 7079 3429  Fr]...).zF%(py4)
 000028d0: 730a 7b25 2870 7934 2973 203d 2025 2870  s.{%(py4)s = %(p
 000028e0: 7932 2973 0a7b 2528 7079 3229 7320 3d20  y2)s.{%(py2)s = 
 000028f0: 2528 7079 3029 732e 6661 696c 7572 650a  %(py0)s.failure.
-00002900: 7d28 290a 7d20 3d3d 2025 2870 7937 2973  }().} == %(py7)s
+00002900: 7d28 290a 7d20 6973 2025 2870 7937 2973  }().} is %(py7)s
 00002910: 726b 0000 0029 0472 4200 0000 7243 0000  rk...).rB...rC..
 00002920: 0072 4400 0000 726e 0000 007a 0e61 7373  .rD...rn...z.ass
 00002930: 6572 7420 2528 7079 3929 7372 4600 0000  ert %(py9)srF...
 00002940: 7a05 7574 662d 3872 0100 0000 e908 0000  z.utf-8r........
 00002950: 007a 087b 7d2d 7b7d 2d7b 7d29 2572 8100  .z.{}-{}-{})%r..
 00002960: 0000 720b 0000 0072 8300 0000 7224 0000  ..r....r....r$..
 00002970: 0072 8700 0000 da0b 4f70 656e 6269 7353  .r......OpenbisS
```

### Comparing `obis-0.4.2rc4/obis/dm/__pycache__/git.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/__pycache__/git.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/__pycache__/repository_utils.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/__pycache__/repository_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/__pycache__/utils.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/checksum.py` & `obis-0.4.2rc5/obis/dm/checksum.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/command_log.py` & `obis-0.4.2rc5/obis/dm/command_log.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/command_result.py` & `obis-0.4.2rc5/obis/dm/command_result.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/__init__.py` & `obis-0.4.2rc5/obis/dm/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/__pycache__/addref.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/commands/__pycache__/addref.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/__pycache__/clone.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/commands/__pycache__/clone.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/__pycache__/collection.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/commands/__pycache__/collection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/__pycache__/download.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/commands/__pycache__/download.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/__pycache__/move.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/commands/__pycache__/move.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/__pycache__/object.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/commands/__pycache__/object.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/__pycache__/removeref.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/commands/__pycache__/removeref.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/__pycache__/search.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/commands/__pycache__/search.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/__pycache__/upload.cpython-310.pyc` & `obis-0.4.2rc5/obis/dm/commands/__pycache__/upload.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/addref.py` & `obis-0.4.2rc5/obis/dm/commands/addref.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/clone.py` & `obis-0.4.2rc5/obis/dm/commands/clone.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/collection.py` & `obis-0.4.2rc5/obis/dm/commands/collection.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/download.py` & `obis-0.4.2rc5/obis/dm/commands/download.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/download_physical.py` & `obis-0.4.2rc5/obis/dm/commands/download_physical.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/move.py` & `obis-0.4.2rc5/obis/dm/commands/move.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/object.py` & `obis-0.4.2rc5/obis/dm/commands/object.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/openbis_command.py` & `obis-0.4.2rc5/obis/dm/commands/openbis_command.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/openbis_command_test.py` & `obis-0.4.2rc5/obis/dm/commands/openbis_command_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/openbis_sync.py` & `obis-0.4.2rc5/obis/dm/commands/openbis_sync.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/removeref.py` & `obis-0.4.2rc5/obis/dm/commands/removeref.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/search.py` & `obis-0.4.2rc5/obis/dm/commands/search.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/commands/upload.py` & `obis-0.4.2rc5/obis/dm/commands/upload.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/config.py` & `obis-0.4.2rc5/obis/dm/config.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/config_test.py` & `obis-0.4.2rc5/obis/dm/config_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/data_mgmt.py` & `obis-0.4.2rc5/obis/dm/data_mgmt.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/data_mgmt_test.py` & `obis-0.4.2rc5/obis/dm/data_mgmt_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/git.py` & `obis-0.4.2rc5/obis/dm/git.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/repository_utils.py` & `obis-0.4.2rc5/obis/dm/repository_utils.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/utils.py` & `obis-0.4.2rc5/obis/dm/utils.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/dm/utils_test.py` & `obis-0.4.2rc5/obis/dm/utils_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/scripts/__init__.py` & `obis-0.4.2rc5/obis/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/scripts/__pycache__/cli.cpython-310.pyc` & `obis-0.4.2rc5/obis/scripts/__pycache__/cli.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/scripts/__pycache__/click_util.cpython-310.pyc` & `obis-0.4.2rc5/obis/scripts/__pycache__/click_util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc` & `obis-0.4.2rc5/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/scripts/cli.py` & `obis-0.4.2rc5/obis/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/scripts/click_util.py` & `obis-0.4.2rc5/obis/scripts/click_util.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/scripts/data_mgmt_runner.py` & `obis-0.4.2rc5/obis/scripts/data_mgmt_runner.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis/test-data/snb-data.zip` & `obis-0.4.2rc5/obis/test-data/snb-data.zip`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/obis.egg-info/PKG-INFO` & `obis-0.4.2rc5/obis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obis
-Version: 0.4.2rc4
+Version: 0.4.2rc5
 Summary: Local data management with assistance from OpenBIS.
 Home-page: https://sissource.ethz.ch/sispub/openbis/tree/master/app-openbis-command-line
 Author: ID SIS • ETH Zürich
 Author-email: openbis-support@id.ethz.ch
 License: Apache Software License Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `obis-0.4.2rc4/obis.egg-info/SOURCES.txt` & `obis-0.4.2rc5/obis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `obis-0.4.2rc4/setup.py` & `obis-0.4.2rc5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 data_dir = os.path.join("man", "man1")
 data_files = [
     (d, [os.path.join(d, f) for f in files]) for d, folders, files in os.walk(data_dir)
 ]
 
 setup(
     name="obis",
-    version="0.4.2rc4",
+    version="0.4.2rc5",
     description="Local data management with assistance from OpenBIS.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://sissource.ethz.ch/sispub/openbis/tree/master/app-openbis-command-line",
     author="ID SIS • ETH Zürich",
     author_email="openbis-support@id.ethz.ch",
     license="Apache Software License Version 2.0",
     packages=["obis", "obis.dm", "obis.dm.commands", "obis.scripts"],
     data_files=data_files,
     package_data={"obis": ["dm/git-annex-attributes"]},
-    install_requires=["pyOpenSSL", "pytest", "pybis==1.35.9", "click"],
+    install_requires=["pyOpenSSL", "pytest", "pybis==1.35.10", "click"],
     entry_points={"console_scripts": ["obis=obis.scripts.cli:main"]},
     zip_safe=False,
     python_requires=">=3.3",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
```

