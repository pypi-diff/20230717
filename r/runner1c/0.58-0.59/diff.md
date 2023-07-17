# Comparing `tmp/runner1c-0.58.tar.gz` & `tmp/runner1c-0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runner1c-0.58.tar", last modified: Thu Jul 13 12:43:01 2023, max compression
+gzip compressed data, was "runner1c-0.59.tar", last modified: Mon Jul 17 13:06:06 2023, max compression
```

## Comparing `runner1c-0.58.tar` & `runner1c-0.59.tar`

### file list

```diff
@@ -1,106 +1,103 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.364266 runner1c-0.58/
--rw-rw-rw-   0        0        0     1363 2018-06-06 07:24:58.000000 runner1c-0.58/LICENSE
--rw-rw-rw-   0        0        0      248 2019-02-21 11:18:58.000000 runner1c-0.58/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-13 12:43:01.364266 runner1c-0.58/PKG-INFO
--rw-rw-rw-   0        0        0      708 2023-03-06 10:43:08.000000 runner1c-0.58/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.270517 runner1c-0.58/runner1c/
--rw-rw-rw-   0        0        0       94 2023-07-13 12:41:40.000000 runner1c-0.58/runner1c/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.270517 runner1c-0.58/runner1c/build/
--rw-rw-rw-   0        0        0       68 2017-11-30 07:27:08.000000 runner1c-0.58/runner1c/build/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/build/tests/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/build/tests/repo/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.270517 runner1c-0.58/runner1c/build/tests/repo/epf/
--rw-rw-rw-   0        0        0     5563 2022-11-29 12:38:31.000000 runner1c-0.58/runner1c/build/tests/repo/epf/CheckConfig.epf
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/build/tools/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.286140 runner1c-0.58/runner1c/build/tools/epf/
--rw-rw-rw-   0        0        0     5669 2022-11-29 12:38:33.000000 runner1c-0.58/runner1c/build/tools/epf/ChangeSafeModeForExtension.epf
--rw-rw-rw-   0        0        0     9691 2022-11-29 12:38:35.000000 runner1c-0.58/runner1c/build/tools/epf/CloseAfterUpdate.epf
--rw-rw-rw-   0        0        0     7837 2022-11-29 12:38:36.000000 runner1c-0.58/runner1c/build/tools/epf/FileCompareMxl.epf
--rw-rw-rw-   0        0        0    11501 2023-02-27 08:40:08.000000 runner1c-0.58/runner1c/build/tools/epf/Runner1C.epf
--rw-rw-rw-   0        0        0    18974 2023-03-06 11:18:23.000000 runner1c-0.58/runner1c/command.py
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.317389 runner1c-0.58/runner1c/commands/
--rw-rw-rw-   0        0        0        0 2018-01-31 10:55:59.000000 runner1c-0.58/runner1c/commands/__init__.py
--rw-rw-rw-   0        0        0     9674 2023-03-13 11:07:31.000000 runner1c-0.58/runner1c/commands/base_for_test.py
--rw-rw-rw-   0        0        0      417 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/create_base.py
--rw-rw-rw-   0        0        0     1164 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/create_epf.py
--rw-rw-rw-   0        0        0     1700 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/diff_mxl.py
--rw-rw-rw-   0        0        0     7716 2023-03-06 11:18:23.000000 runner1c-0.58/runner1c/commands/dump_config.py
--rw-rw-rw-   0        0        0     2612 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/dump_epf.py
--rw-rw-rw-   0        0        0     1334 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/dump_extensions.py
--rw-rw-rw-   0        0        0      895 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/file.py
--rw-rw-rw-   0        0        0     2127 2022-12-23 07:28:15.000000 runner1c-0.58/runner1c/commands/load_config.py
--rw-rw-rw-   0        0        0     6045 2023-02-27 10:03:54.000000 runner1c-0.58/runner1c/commands/load_extension.py
--rw-rw-rw-   0        0        0     5233 2023-07-13 12:10:01.000000 runner1c-0.58/runner1c/commands/platform_check.py
--rw-rw-rw-   0        0        0      956 2022-01-27 09:51:20.000000 runner1c-0.58/runner1c/commands/reg_server.py
--rw-rw-rw-   0        0        0     1749 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/start.py
--rw-rw-rw-   0        0        0      821 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/start_agent.py
--rw-rw-rw-   0        0        0     9397 2022-12-23 07:28:15.000000 runner1c-0.58/runner1c/commands/sync.py
--rw-rw-rw-   0        0        0      442 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/version.py
--rw-rw-rw-   0        0        0     1114 2022-01-26 08:04:08.000000 runner1c-0.58/runner1c/commands/webinst.py
--rw-rw-rw-   0        0        0     2889 2022-12-23 07:28:15.000000 runner1c-0.58/runner1c/common.py
--rw-rw-rw-   0        0        0     2406 2022-11-30 15:41:24.000000 runner1c-0.58/runner1c/core.py
--rw-rw-rw-   0        0        0      208 2022-01-26 07:47:39.000000 runner1c-0.58/runner1c/exit_code.py
--rw-rw-rw-   0        0        0     2851 2023-02-14 07:03:32.000000 runner1c-0.58/runner1c/parser.py
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.333020 runner1c-0.58/runner1c/tests/
--rw-rw-rw-   0        0        0        0 2018-01-31 10:55:59.000000 runner1c-0.58/runner1c/tests/__init__.py
--rw-rw-rw-   0        0        0      432 2022-01-26 07:47:39.000000 runner1c-0.58/runner1c/tests/conftest.py
--rw-rw-rw-   0        0        0      599 2022-01-26 07:47:39.000000 runner1c-0.58/runner1c/tests/test_diff_mxl.py
--rw-rw-rw-   0        0        0      632 2022-01-26 07:47:39.000000 runner1c-0.58/runner1c/tests/test_sync_without_base.py
--rw-rw-rw-   0        0        0     1082 2022-01-26 07:47:39.000000 runner1c-0.58/runner1c/tests/test_version.py
--rw-rw-rw-   0        0        0     5803 2023-07-13 08:47:16.000000 runner1c-0.58/runner1c/tests/test_with_base.py
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.333020 runner1c-0.58/runner1c/tools/
--rw-rw-rw-   0        0        0     6716 2023-02-27 10:04:24.000000 runner1c-0.58/runner1c/tools/create_base_for_test.py
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.333020 runner1c-0.58/runner1c/tools/epf/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.333020 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.333020 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.333020 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form/
--rw-rw-rw-   0        0        0     1050 2022-07-15 07:16:21.000000 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form/Module.bsl
--rw-rw-rw-   0        0        0     1340 2022-07-15 07:16:21.000000 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form.xml
--rw-rw-rw-   0        0        0     1513 2022-07-15 07:16:21.000000 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form.xml
--rw-rw-rw-   0        0        0     1921 2022-07-15 07:16:21.000000 runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension.xml
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.333020 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Ext/
--rw-rw-rw-   0        0        0     2001 2022-07-15 07:40:45.000000 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Ext/ObjectModule.bsl
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.348642 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.348642 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.348642 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form/
--rw-rw-rw-   0        0        0     2983 2022-07-15 12:08:24.000000 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form/Module.bsl
--rw-rw-rw-   0        0        0     2170 2022-07-15 07:40:45.000000 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form.xml
--rw-rw-rw-   0        0        0     1519 2022-07-15 07:40:45.000000 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed.xml
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.348642 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.348642 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form/
--rw-rw-rw-   0        0        0     1720 2022-07-15 07:40:45.000000 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form/Module.bsl
--rw-rw-rw-   0        0        0     5911 2022-07-15 07:51:27.000000 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form.bin
--rw-rw-rw-   0        0        0     1522 2022-07-15 07:40:45.000000 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary.xml
--rw-rw-rw-   0        0        0     2035 2022-07-15 07:40:45.000000 runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate.xml
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/FileCompareMxl/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.348642 runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.348642 runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.364266 runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form/
--rw-rw-rw-   0        0        0    10183 2022-07-15 12:08:24.000000 runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form/Module.bsl
--rw-rw-rw-   0        0        0    19173 2022-07-15 12:08:24.000000 runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form.bin
--rw-rw-rw-   0        0        0     1514 2022-07-15 07:40:46.000000 runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form.xml
--rw-rw-rw-   0        0        0     1871 2022-07-15 07:40:46.000000 runner1c-0.58/runner1c/tools/epf/FileCompareMxl.xml
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/Runner1C/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.364266 runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.239282 runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.364266 runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form/Ext/
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.364266 runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form/
--rw-rw-rw-   0        0        0    29395 2023-02-27 08:40:18.000000 runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form/Module.bsl
--rw-rw-rw-   0        0        0    10896 2023-02-27 08:40:18.000000 runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form.xml
--rw-rw-rw-   0        0        0     1513 2023-02-27 08:40:18.000000 runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form.xml
--rw-rw-rw-   0        0        0     1845 2023-02-27 08:40:18.000000 runner1c-0.58/runner1c/tools/epf/Runner1C.xml
-drwxrwxrwx   0        0        0        0 2023-07-13 12:43:01.270517 runner1c-0.58/runner1c.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-13 12:43:01.000000 runner1c-0.58/runner1c.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2530 2023-07-13 12:43:01.000000 runner1c-0.58/runner1c.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 12:43:01.000000 runner1c-0.58/runner1c.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-13 12:43:01.000000 runner1c-0.58/runner1c.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-07-13 12:43:01.000000 runner1c-0.58/runner1c.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-13 12:43:01.000000 runner1c-0.58/runner1c.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 12:43:01.364266 runner1c-0.58/setup.cfg
--rw-rw-rw-   0        0        0      684 2023-02-14 07:03:32.000000 runner1c-0.58/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.748206 runner1c-0.59/
+-rw-rw-rw-   0        0        0     1363 2018-06-06 07:24:58.000000 runner1c-0.59/LICENSE
+-rw-rw-rw-   0        0        0      248 2019-02-21 11:18:58.000000 runner1c-0.59/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-17 13:06:06.748206 runner1c-0.59/PKG-INFO
+-rw-rw-rw-   0        0        0      708 2023-07-13 12:53:16.000000 runner1c-0.59/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.660764 runner1c-0.59/runner1c/
+-rw-rw-rw-   0        0        0       94 2023-07-17 13:04:51.000000 runner1c-0.59/runner1c/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.670274 runner1c-0.59/runner1c/build/
+-rw-rw-rw-   0        0        0       68 2017-11-30 07:27:08.000000 runner1c-0.59/runner1c/build/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.622991 runner1c-0.59/runner1c/build/tools/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.670274 runner1c-0.59/runner1c/build/tools/epf/
+-rw-rw-rw-   0        0        0     5669 2023-07-17 11:17:41.000000 runner1c-0.59/runner1c/build/tools/epf/ChangeSafeModeForExtension.epf
+-rw-rw-rw-   0        0        0     9688 2023-07-17 11:17:42.000000 runner1c-0.59/runner1c/build/tools/epf/CloseAfterUpdate.epf
+-rw-rw-rw-   0        0        0     7837 2023-07-17 11:17:43.000000 runner1c-0.59/runner1c/build/tools/epf/FileCompareMxl.epf
+-rw-rw-rw-   0        0        0    11398 2023-07-17 11:17:45.000000 runner1c-0.59/runner1c/build/tools/epf/Runner1C.epf
+-rw-rw-rw-   0        0        0    18643 2023-07-17 11:15:27.000000 runner1c-0.59/runner1c/command.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.701421 runner1c-0.59/runner1c/commands/
+-rw-rw-rw-   0        0        0        0 2018-01-31 10:55:59.000000 runner1c-0.59/runner1c/commands/__init__.py
+-rw-rw-rw-   0        0        0     9303 2023-07-17 12:31:31.000000 runner1c-0.59/runner1c/commands/base_for_test.py
+-rw-rw-rw-   0        0        0      417 2022-01-26 08:04:08.000000 runner1c-0.59/runner1c/commands/create_base.py
+-rw-rw-rw-   0        0        0     1164 2022-01-26 08:04:08.000000 runner1c-0.59/runner1c/commands/create_epf.py
+-rw-rw-rw-   0        0        0     1713 2023-07-17 09:45:57.000000 runner1c-0.59/runner1c/commands/diff_mxl.py
+-rw-rw-rw-   0        0        0     7716 2023-03-06 11:18:23.000000 runner1c-0.59/runner1c/commands/dump_config.py
+-rw-rw-rw-   0        0        0     2612 2022-01-26 08:04:08.000000 runner1c-0.59/runner1c/commands/dump_epf.py
+-rw-rw-rw-   0        0        0     1334 2022-01-26 08:04:08.000000 runner1c-0.59/runner1c/commands/dump_extensions.py
+-rw-rw-rw-   0        0        0      895 2022-01-26 08:04:08.000000 runner1c-0.59/runner1c/commands/file.py
+-rw-rw-rw-   0        0        0     2127 2023-07-13 12:53:16.000000 runner1c-0.59/runner1c/commands/load_config.py
+-rw-rw-rw-   0        0        0     6071 2023-07-17 09:45:32.000000 runner1c-0.59/runner1c/commands/load_extension.py
+-rw-rw-rw-   0        0        0     5233 2023-07-13 12:53:16.000000 runner1c-0.59/runner1c/commands/platform_check.py
+-rw-rw-rw-   0        0        0      956 2022-01-27 09:51:20.000000 runner1c-0.59/runner1c/commands/reg_server.py
+-rw-rw-rw-   0        0        0     1749 2022-01-26 08:04:08.000000 runner1c-0.59/runner1c/commands/start.py
+-rw-rw-rw-   0        0        0      821 2022-01-26 08:04:08.000000 runner1c-0.59/runner1c/commands/start_agent.py
+-rw-rw-rw-   0        0        0     9410 2023-07-17 09:45:09.000000 runner1c-0.59/runner1c/commands/sync.py
+-rw-rw-rw-   0        0        0      442 2023-07-17 11:51:46.000000 runner1c-0.59/runner1c/commands/version.py
+-rw-rw-rw-   0        0        0     1114 2022-01-26 08:04:08.000000 runner1c-0.59/runner1c/commands/webinst.py
+-rw-rw-rw-   0        0        0     3373 2023-07-17 11:39:15.000000 runner1c-0.59/runner1c/common.py
+-rw-rw-rw-   0        0        0     2294 2023-07-17 07:00:13.000000 runner1c-0.59/runner1c/core.py
+-rw-rw-rw-   0        0        0      208 2022-01-26 07:47:39.000000 runner1c-0.59/runner1c/exit_code.py
+-rw-rw-rw-   0        0        0     1061 2023-07-17 11:20:28.000000 runner1c-0.59/runner1c/logger.py
+-rw-rw-rw-   0        0        0     2851 2023-07-13 12:53:16.000000 runner1c-0.59/runner1c/parser.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.701421 runner1c-0.59/runner1c/tests/
+-rw-rw-rw-   0        0        0        0 2018-01-31 10:55:59.000000 runner1c-0.59/runner1c/tests/__init__.py
+-rw-rw-rw-   0        0        0      432 2022-01-26 07:47:39.000000 runner1c-0.59/runner1c/tests/conftest.py
+-rw-rw-rw-   0        0        0      546 2023-07-17 12:54:01.000000 runner1c-0.59/runner1c/tests/test_diff_mxl.py
+-rw-rw-rw-   0        0        0      563 2023-07-17 12:54:01.000000 runner1c-0.59/runner1c/tests/test_sync_without_base.py
+-rw-rw-rw-   0        0        0      976 2023-07-17 12:40:08.000000 runner1c-0.59/runner1c/tests/test_version.py
+-rw-rw-rw-   0        0        0     5362 2023-07-17 12:54:17.000000 runner1c-0.59/runner1c/tests/test_with_base.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.717059 runner1c-0.59/runner1c/tools/
+-rw-rw-rw-   0        0        0     6716 2023-07-13 12:53:16.000000 runner1c-0.59/runner1c/tools/create_base_for_test.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.717059 runner1c-0.59/runner1c/tools/epf/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.622991 runner1c-0.59/runner1c/tools/epf/ChangeSafeModeForExtension/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.717059 runner1c-0.59/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.622991 runner1c-0.59/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.717059 runner1c-0.59/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.717059 runner1c-0.59/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form/
+-rw-rw-rw-   0        0        0     1050 2022-07-15 07:16:21.000000 runner1c-0.59/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form/Module.bsl
+-rw-rw-rw-   0        0        0     1340 2022-07-15 07:16:21.000000 runner1c-0.59/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form.xml
+-rw-rw-rw-   0        0        0     1513 2022-07-15 07:16:21.000000 runner1c-0.59/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form.xml
+-rw-rw-rw-   0        0        0     1921 2022-07-15 07:16:21.000000 runner1c-0.59/runner1c/tools/epf/ChangeSafeModeForExtension.xml
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.638616 runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.717059 runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Ext/
+-rw-rw-rw-   0        0        0     2001 2022-07-15 07:40:45.000000 runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Ext/ObjectModule.bsl
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.732571 runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.638616 runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.732571 runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.732571 runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form/
+-rw-rw-rw-   0        0        0     2983 2022-07-15 12:08:24.000000 runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form/Module.bsl
+-rw-rw-rw-   0        0        0     2170 2022-07-15 07:40:45.000000 runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form.xml
+-rw-rw-rw-   0        0        0     1519 2022-07-15 07:40:45.000000 runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed.xml
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.638616 runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.732571 runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.732571 runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form/
+-rw-rw-rw-   0        0        0     1720 2022-07-15 07:40:45.000000 runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form/Module.bsl
+-rw-rw-rw-   0        0        0     5911 2022-07-15 07:51:27.000000 runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form.bin
+-rw-rw-rw-   0        0        0     1522 2022-07-15 07:40:45.000000 runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary.xml
+-rw-rw-rw-   0        0        0     2035 2022-07-15 07:40:45.000000 runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate.xml
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.638616 runner1c-0.59/runner1c/tools/epf/FileCompareMxl/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.732571 runner1c-0.59/runner1c/tools/epf/FileCompareMxl/Forms/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.638616 runner1c-0.59/runner1c/tools/epf/FileCompareMxl/Forms/Form/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.732571 runner1c-0.59/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.732571 runner1c-0.59/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form/
+-rw-rw-rw-   0        0        0    10183 2022-07-15 12:08:24.000000 runner1c-0.59/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form/Module.bsl
+-rw-rw-rw-   0        0        0    19173 2022-07-15 12:08:24.000000 runner1c-0.59/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form.bin
+-rw-rw-rw-   0        0        0     1514 2022-07-15 07:40:46.000000 runner1c-0.59/runner1c/tools/epf/FileCompareMxl/Forms/Form.xml
+-rw-rw-rw-   0        0        0     1871 2022-07-15 07:40:46.000000 runner1c-0.59/runner1c/tools/epf/FileCompareMxl.xml
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.638616 runner1c-0.59/runner1c/tools/epf/Runner1C/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.748206 runner1c-0.59/runner1c/tools/epf/Runner1C/Forms/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.638616 runner1c-0.59/runner1c/tools/epf/Runner1C/Forms/Form/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.748206 runner1c-0.59/runner1c/tools/epf/Runner1C/Forms/Form/Ext/
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.748206 runner1c-0.59/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form/
+-rw-rw-rw-   0        0        0    28804 2023-07-13 12:53:16.000000 runner1c-0.59/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form/Module.bsl
+-rw-rw-rw-   0        0        0    10612 2023-07-13 12:53:16.000000 runner1c-0.59/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form.xml
+-rw-rw-rw-   0        0        0     1513 2023-02-27 08:40:18.000000 runner1c-0.59/runner1c/tools/epf/Runner1C/Forms/Form.xml
+-rw-rw-rw-   0        0        0     1845 2023-02-27 08:40:18.000000 runner1c-0.59/runner1c/tools/epf/Runner1C.xml
+drwxrwxrwx   0        0        0        0 2023-07-17 13:06:06.660764 runner1c-0.59/runner1c.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-17 13:06:06.000000 runner1c-0.59/runner1c.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2503 2023-07-17 13:06:06.000000 runner1c-0.59/runner1c.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 13:06:06.000000 runner1c-0.59/runner1c.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-17 13:06:06.000000 runner1c-0.59/runner1c.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-07-17 13:06:06.000000 runner1c-0.59/runner1c.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 13:06:06.000000 runner1c-0.59/runner1c.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 13:06:06.748206 runner1c-0.59/setup.cfg
+-rw-rw-rw-   0        0        0      684 2023-07-13 12:53:16.000000 runner1c-0.59/setup.py
```

### Comparing `runner1c-0.58/LICENSE` & `runner1c-0.59/LICENSE`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/README.md` & `runner1c-0.59/README.md`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/build/tests/repo/epf/CheckConfig.epf` & `runner1c-0.59/runner1c/build/tools/epf/ChangeSafeModeForExtension.epf`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: ffff ff7f 0002 0000 0700 0000 0000 0000  ................
 00000010: 0d0a 3030 3030 3030 3534 2030 3030 3030  ..00000054 00000
 00000020: 3230 3020 3766 6666 6666 6666 200d 0a2f  200 7fffffff ../
-00000030: 0200 00ae 0200 00ff ffff 7fcd 0400 0050  ...............P
-00000040: 0500 00ff ffff 7f8f 0900 00d6 0900 00ff  ................
-00000050: ffff 7ff5 0b00 0074 0c00 00ff ffff 7f93  .......t........
-00000060: 0e00 00d2 0e00 00ff ffff 7ff1 1000 0036  ...............6
-00000070: 1100 00ff ffff 7f55 1300 009c 1300 00ff  .......U........
+00000030: 0200 00ae 0200 00ff ffff 7fcd 0400 004c  ...............L
+00000040: 0500 00ff ffff 7f6b 0700 00ee 0700 00ff  .......k........
+00000050: ffff 7f97 0c00 00de 0c00 00ff ffff 7ffd  ................
+00000060: 0e00 003c 0f00 00ff ffff 7f5b 1100 00a0  ...<.......[....
+00000070: 1100 00ff ffff 7fbf 1300 0006 1400 00ff  ................
 00000080: ffff 7f00 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -30,227 +30,227 @@
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 000d  ................
 00000230: 0a30 3030 3030 3036 3020 3030 3030 3030  .00000060 000000
-00000240: 3630 2037 6666 6666 6666 6620 0d0a 7059  60 7fffffff ..pY
-00000250: 4b60 4e44 0200 7059 4b60 4e44 0200 0000  K`ND..pYK`ND....
-00000260: 0000 3700 6400 6200 3800 3300 6100 3300  ..7.d.b.8.3.a.3.
-00000270: 6100 2d00 3300 3000 3500 6300 2d00 3400  a.-.3.0.5.c.-.4.
-00000280: 3400 3400 3400 2d00 6100 3200 3200 3000  4.4.4.-.a.2.2.0.
-00000290: 2d00 6500 6600 6300 3100 3100 3000 3100  -.e.f.c.1.1.0.1.
-000002a0: 3500 3700 3000 3400 3700 0000 0000 0d0a  5.7.0.4.7.......
-000002b0: 3030 3030 3030 3965 2030 3030 3030 3230  0000009e 0000020
-000002c0: 3020 3766 6666 6666 6666 200d 0a95 4f4b  0 7fffffff ...OK
-000002d0: 0a02 310c dd0f cc25 eab6 81a4 1fd3 5ec0  ..1....%......^.
-000002e0: 7b24 9dce 4e84 0157 d293 b9f0 485e c1da  {$..N..W....H^..
-000002f0: 5170 6b08 e125 79ef 913c ef8f 1bd9 79da  Qpk..%y..<....y.
-00000300: 0b0e e47e 7ab4 bc68 f2e2 053c c602 a107  ...~z..h...<....
-00000310: 8873 0875 2d44 4891 3170 b3e6 74d9 ce66  .s.u-DH.1p..t..f
-00000320: 179a ed6a 3e83 be30 dd83 ac77 1513 8b02  ...j>..0...w....
-00000330: 854c 10b2 1e41 5418 828f 4c1a 488a 53eb  .L...AT...L.H.S.
-00000340: dbe0 7693 7182 3918 4b8c 695d 44a0 68a9  ..v.q.9.K.i]D.h.
-00000350: 105c caa0 9e3d 204b 140e 5a6b 264b ed2f  .\...= K..Zk&K./
-00000360: ba6b f3f4 cef1 e117 637b 0100 0000 0000  .k......c{......
-00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000240: 3630 2037 6666 6666 6666 6620 0d0a 50dc  60 7fffffff ..P.
+00000250: 09a2 7c44 0200 50dc 09a2 7c44 0200 0000  ..|D..P...|D....
+00000260: 0000 3800 3900 6600 3600 3200 6200 6300  ..8.9.f.6.2.b.c.
+00000270: 3100 2d00 3900 6600 6500 3900 2d00 3400  1.-.9.f.e.9.-.4.
+00000280: 6600 3800 3900 2d00 6200 3600 3900 3100  f.8.9.-.b.6.9.1.
+00000290: 2d00 3800 3100 6200 6200 3200 3000 3300  -.8.1.b.b.2.0.3.
+000002a0: 3700 3400 3300 6300 6600 0000 0000 0d0a  7.4.3.c.f.......
+000002b0: 3030 3030 3031 3637 2030 3030 3030 3230  00000167 0000020
+000002c0: 3020 3766 6666 6666 6666 200d 0a8d 913d  0 7fffffff ....=
+000002d0: 8e94 310c 86fb 95f6 0ea3 affe 2c39 7f8e  ..1.........,9..
+000002e0: 5d23 e8a8 3881 93d8 40c1 8c34 0b12 d26a  ]#..8...@..4...j
+000002f0: 4e46 c191 b802 9e99 ddad 28b0 a228 c5a3  NF........(..(..
+00000300: d7f6 933f bf7e 3fa7 fdf1 e199 c529 8f99  ...?.~?......)..
+00000310: 40dc 04aa b3c0 2049 c069 8c8c a5d7 32fd  @..... I.i....2.
+00000320: b2df d059 b824 9b0c 8b57 0b54 0ab0 e60c  ...Y.$...W.T....
+00000330: 2ec3 d5b0 97dc fdca dde0 badb d28a 1a79  ...............y
+00000340: 3c5a 814a d641 3b25 e89a 5da9 28b2 fb8e  <Z.J.A;%..].(...
+00000350: 8269 522e b07a 21a8 ad54 6021 879c 6d78  .iR..z!..T`!..mx
+00000360: 25e5 c9f9 1a87 6fc1 b8e3 de6a a998 7941  %.....o....j..yA
+00000370: 5fb6 a05a 2360 e709 581b 1159 4ed5 db65  _..Z#`..X..YN..e
+00000380: dfde 7dd1 e367 fba4 6e1f 4fcb 3e9c ceef  ..}..g..n.O.>...
+00000390: 7f7e b7e3 d3d7 d371 bbc7 6de7 1fdb 2b76  .~.....q..m...+v
+000003a0: 780a eef0 2dc0 839f ce07 7b43 2368 8b9e  x...-.....{C#h..
+000003b0: 7879 7cb8 ecaa c265 2142 6eb5 43d5 aea0  xy|....e!Bn.C...
+000003c0: 312a d892 29a5 3b6b 1937 fea5 e01f d76b  1*..).;k.7.....k
+000003d0: 5df6 7a1d 23ec 9be3 4a80 c209 525a 0443  ].z.#...J...RZ.C
+000003e0: 0607 da70 8457 95b6 a2fb 152d 4b4d 3111  ...p.W.....-KM1.
+000003f0: 908c e86e ab82 8433 48b9 4b4a a567 377a  ...n...3H.KJ.g7z
+00000400: 4157 1b68 2dec e446 a128 2c83 cc50 ec54  AW.h-..F.(,..P.T
+00000410: 70aa 2f56 caf1 adff b3cf 2dcf 268d d1ac  p./V......-.&...
+00000420: c1e8 ca50 578f 974d 016a 9cb0 2b89 4cbf  ...PW..M.j..+.L.
+00000430: 3bba 9fbf 0000 0000 0000 0000 0000 0000  ;...............
 00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004c0: 0000 0000 0000 0000 0000 0000 000d 0a30  ...............0
-000004d0: 3030 3030 3036 3420 3030 3030 3030 3634  0000064 00000064
-000004e0: 2037 6666 6666 6666 6620 0d0a 7059 4b60   7fffffff ..pYK`
-000004f0: 4e44 0200 7059 4b60 4e44 0200 0000 0000  ND..pYK`ND......
-00000500: 3700 6400 6200 3800 3300 6100 3300 6100  7.d.b.8.3.a.3.a.
-00000510: 2d00 3300 3000 3500 6300 2d00 3400 3400  -.3.0.5.c.-.4.4.
-00000520: 3400 3400 2d00 6100 3200 3200 3000 2d00  4.4.-.a.2.2.0.-.
-00000530: 6500 6600 6300 3100 3100 3000 3100 3500  e.f.c.1.1.0.1.5.
-00000540: 3700 3000 3400 3700 2e00 3000 0000 0000  7.0.4.7...0.....
-00000550: 0d0a 3030 3030 3034 3230 2030 3030 3030  ..00000420 00000
-00000560: 3432 3020 3766 6666 6666 6666 200d 0a8d  420 7fffffff ...
-00000570: 93eb 6e1a 4714 c73f 0789 7740 1ba9 c212  ..n.G..?..w@....
-00000580: 9bce eeec 2e6c a3a8 8a13 1bb0 166c 01e6  .....l.......l..
-00000590: f66d 6f18 30c6 560c 6bd8 c892 0352 5bd5  .mo.0.V.k....R[.
-000005a0: 96fa a9aa d4aa 4913 f501 c885 d689 13f2  ......I.........
-000005b0: 0a33 4fd2 57e8 99d9 b5c1 8e13 07cc cefa  .3O.W...........
-000005c0: cc99 df39 e77f cefc 77f6 f131 4e44 238f  ...9....w..1ND#.
-000005d0: 153d 81c2 af14 ace1 47bc e671 fe01 5738  .=......G..q..W8
-000005e0: 0afe 87e1 4189 1f66 3f6e c7b6 6d6b 2a72  ....A..f?n..mk*r
-000005f0: c586 8625 51b1 4d57 4cb9 188b d835 4d5b  ...%Q.MWL....5M[
-00000600: 9390 a536 f484 409e d123 724a 9ed2 1179  ...6..@..#rJ...y
-00000610: 478f e831 aca7 e454 e098 af22 40c4 4316  G..1...T..."@.C.
-00000620: 10d2 e009 c932 7b8a 705e 4632 d670 524c  .....2{.p^F2.pRL
-00000630: a6b4 94a8 986a 434c a949 4d4c 61d5 4c6a  .....jCL.IMLa.Lj
-00000640: 2eb2 75cb 3c0c ab66 89fc 4d66 90ca 7b32  ..u.<..f..Mf..{2
-00000650: 21bf 9319 5f3f 9037 f09b d05f c833 fedf  !..._?.7..._.3..
-00000660: 949c d113 e1a2 ea79 f5a1 6809 39c1 83e3  .......y..h.9...
-00000670: 8412 6414 8d70 af64 0207 02a1 e014 770e  ..d..p.d......w.
-00000680: d345 4101 7306 66ce cc20 08ec 8f6d f065  .EA.s.f.. ...m.e
-00000690: fee5 1e81 e608 85aa a340 75d6 481e 5588  .........@u.H.U.
-000006a0: 46be 217f f25a ce40 d029 f900 c24e a311  F.!..Z.@.)...N..
-000006b0: 2ef7 8cfe 0096 3774 0cef 93d8 f51d 8807  ......7t........
-000006c0: 0620 fcbb 148d dc82 3ff2 2b7d c260 31e0  . ......?.+}.`1.
-000006d0: 4ed9 a931 7d02 2e4c 9ee7 74c4 b0cc 3dce  N..1}..L..t...=.
-000006e0: b462 5c50 70ca cdbf c1fb 47e6 ccb6 9762  .b\Pp.....G....b
-000006f0: e405 38be 0665 27c0 64dc 5b81 0739 05dc  ..8..e'.d.[..9..
-00000700: 0974 6142 de42 9849 ec1e 0b34 23af e831  .taB.B.I...4#..1
-00000710: 791b bbe4 f302 b27f 1704 bf29 dcdd cf07  y..........)....
-00000720: b833 3703 6204 5b17 65d0 71fc fbf8 a274  .37.b.[.e.q....t
-00000730: 9c36 83f7 40ab 3378 ff87 edb0 fd3b 90c2  .6..@.3x.....;..
-00000740: 0c26 634c 7f04 16e3 30ee 6b66 63e9 335e  .&cL....0.kfc.3^
-00000750: 7c09 aa11 8492 bbdf 8bd9 bbdd 466b 0b5a  |...........Fk.Z
-00000760: 1a43 8998 b474 7386 6153 e849 3cf0 bdf0  .C...ts.aS.I<...
-00000770: 7f05 151f d19f c2a0 7f81 e525 b476 44c7  ...........%.vD.
-00000780: e439 2741 c3c9 7b7a 1c27 7fb0 74e9 c9c5  .9'A..{z.'..t...
-00000790: 713e e030 ce30 0661 4fef f216 2fd8 af8c  q>.0.0.aO.../...
-000007a0: 093d 8e46 f8e0 2bc1 d4ea 7cf8 f994 92a7  .=.F..+...|.....
-000007b0: e425 fd99 7764 74e9 6e08 1b66 afe7 3eea  .%..wdt.n..f..>.
-000007c0: 72a3 705b 4868 0d53 9724 b8c4 6612 2eb1  r.p[Hh.S.$..f...
-000007d0: d2c0 aea8 2753 4834 1b52 03db 9285 3527  ....'SH4.R....5'
-000007e0: 797e 65d0 c543 5816 f805 f99a 1d34 5f17  y~e..CX......4_.
-000007f0: 2ec5 a29d b986 e6db 96b9 ef6a ca77 c964  ...........j.w.d
-00000800: ffdb 8d87 ba62 550e b69c 9df2 d096 3b9e  .....bU.......;.
-00000810: d546 ad5c 5139 c8b6 963b d64e deab a73b  .F.\Q9...;.N...;
-00000820: fdba 8f5a e572 216d 94b6 5a1b be92 7fd0  ...Z.r!m..Z.....
-00000830: 1e94 ead5 028a 4623 6645 edda c365 400c  ......F#fE...e@.
-00000840: fa36 b899 9902 b21f ee7a 06ae 2946 7bb5  .6.......z..)F{.
-00000850: 6d74 d724 c3df eae7 8afa 76ad 5a68 1a95  mt.$......v.Zh..
-00000860: bc67 5597 3d08 85cc 8ade 0784 51cd ab36  .gU.=.......Q..6
-00000870: 2e74 aca2 ee33 6a80 cc6e b969 69df eae6  .t...3j..n.ii...
-00000880: b47a 3aef d764 7db8 515c db75 3285 83f5  .z:..d}.Q\.u2...
-00000890: 56ca 73da 80ac e4fa 7677 d303 c4fa 0365  V.s.....vw.....e
-000008a0: 60c8 85a6 935e e981 6bcf 4eeb be59 2dec  `....^..k.N..Y-.
-000008b0: 59b2 d2b3 71c7 77d2 e59e 21e7 3d7b 67b3  Y...q.w...!.={g.
-000008c0: 95cd 347b 565a f5d7 bb79 e456 061d 8605  ..4{VZ...y.V....
-000008d0: c475 e405 ace7 54b6 3dc8 52b5 d297 10ea  .u....T.=.R.....
-000008e0: 79d1 80f8 62dd b8bc 67c8 75cf ea16 7c03  y...b...g.u...|.
-000008f0: 9f17 3c2f 12c2 ea80 c8ee 3491 93b9 af19  ..</......4.....
-00000900: 435d 66d1 6b43 75e8 1453 805c 814e aca2  C]f.kCu..S.\.N..
-00000910: 5a51 6f5b 78ad 03dd 0925 df93 d733 e5bd  ZQo[x....%...3..
-00000920: 736d 9816 5f2e 6221 79a7 536b 7fda 31d6  sm.._.b!y.Sk..1.
-00000930: 916b 9387 c6a5 f5a1 3dd4 71bd 925d c4ec  .k......=.q..]..
-00000940: 5957 300c f159 0de6 1868 f4b6 851d 7fa1  YW0..Y...h......
-00000950: 18e5 1339 1dec 0c55 9c1b aad0 3cdb cbb5  ...9...U....<...
-00000960: ef1f 00ae 56da 1c94 6a72 b363 5556 1632  ....V...jr.cUV.2
-00000970: 69fa 6669 9e09 cbe2 e6e3 3dc8 02e6 63b5  i.fi......=...c.
-00000980: 5f93 375b 86af dcbb f64e 5d5d d9e3 7f0d  _.7[.....N]]....
-00000990: 0a30 3030 3030 3032 3820 3030 3030 3030  .00000028 000000
-000009a0: 3238 2037 6666 6666 6666 6620 0d0a 7059  28 7fffffff ..pY
-000009b0: 4b60 4e44 0200 7059 4b60 4e44 0200 0000  K`ND..pYK`ND....
-000009c0: 0000 6300 6f00 7000 7900 6900 6e00 6600  ..c.o.p.y.i.n.f.
-000009d0: 6f00 0000 0000 0d0a 3030 3030 3030 6362  o.......000000cb
-000009e0: 2030 3030 3030 3230 3020 3766 6666 6666   00000200 7fffff
-000009f0: 6666 200d 0a8d 903d 6a03 410c 857b 832f  ff ....=j.A..{./
-00000a00: b1f5 08a4 d1fc a936 e41e 1acd 2809 2131  .......6....(.!1
-00000a10: a435 3e59 8a1c 2957 c8ee c6e9 57c5 1308  .5>Y..)W....W...
-00000a20: bdc7 27fd 7c7d df52 389f 6e71 1717 d1c4  ..'.|}.R8.nq....
-00000a30: 0984 3041 32ce d0a8 0c30 9739 7b67 979c  ..0A2....0.9{g..
-00000a40: c3a1 25da e28c 1bd3 b406 a38d 0cc9 85a1  ..%.............
-00000a50: 698c e0d2 5d27 568e d5c3 7279 99f6 76b9  i...]'V...ry..v.
-00000a60: 7ef8 ebf3 723f 9fee 9bb3 8ede 5859 8131  ~...r?......XY.1
-00000a70: 1ba4 b560 3522 4c37 22a4 5c31 d570 6869  ...`5"L7".\1.phi
-00000a80: 0719 b9e3 cc73 40cc 2b68 4232 10e3 025e  .....s@.+hB2...^
-00000a90: 184d 7d34 2d31 2c4f d7cf f79d e001 b15b  .M}4-1,O.......[
-00000aa0: 8bab 10e9 04ad cceb 0d3c 416a 4350 2767  .........<AjCP'g
-00000ab0: a3ce 65d4 632f c1ff 5cfc d3f0 e8db f817  ..e.c/..\.......
-00000ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000bf0: 0000 0000 000d 0a30 3030 3030 3036 3020  .......00000060 
-00000c00: 3030 3030 3030 3630 2037 6666 6666 6666  00000060 7ffffff
-00000c10: 6620 0d0a 7059 4b60 4e44 0200 7059 4b60  f ..pYK`ND..pYK`
-00000c20: 4e44 0200 0000 0000 6600 3500 3000 6100  ND......f.5.0.a.
-00000c30: 6400 6200 6400 3700 2d00 3900 6300 3400  d.b.d.7.-.9.c.4.
-00000c40: 3400 2d00 3400 6100 6600 3900 2d00 6200  4.-.4.a.f.9.-.b.
-00000c50: 3400 3400 3100 2d00 3800 3300 3800 6500  4.4.1.-.8.3.8.e.
-00000c60: 6100 3400 6100 3700 3600 3700 3200 3400  a.4.a.7.6.7.2.4.
-00000c70: 0000 0000 0d0a 3030 3030 3031 3463 2030  ......0000014c 0
-00000c80: 3030 3030 3230 3020 3766 6666 6666 6666  0000200 7fffffff
-00000c90: 200d 0a8d 914d 6a5d 310c 85e7 81ec a1bc   ....Mj]1.......
-00000ca0: f115 4896 6d59 e3ac 44b2 a5b6 145a 2874  ..H.mY..D....Z(t
-00000cb0: 14ee ca32 e892 ba85 f8fd a4a3 0e2a 8c31  ...2.........*.1
-00000cc0: f6a7 231f e9cf dbef 573a 9e9f 5eb3 a12d  ..#.....W:..^..-
-00000cd0: 5f02 3a6b 856a a9e0 b512 0c1e 61d5 a44b  _.:k.j......a..K
-00000ce0: a9e7 7143 270f a698 03d6 580d 6a2a c3b0  ..qC'.....X.j*..
-00000cf0: 5220 d5d3 0285 8be4 95bb c1f5 e869 4a64  R ...........iJd
-00000d00: 0126 cc1b e700 9581 6049 c993 9cfb 9243  .&......`I.....C
-00000d10: 46d7 e94e d025 03ea 5403 5f49 c0ad e728  F..N.%..T._I...(
-00000d20: 85bb 0dbd cae1 5f61 3cf0 28a9 6a95 2b28  ......_a<.(.j.+(
-00000d30: e1fe f4e4 0683 fa82 991a e1ce a9ad 9dc7  ................
-00000d40: e5e5 4bcc 6f2f 3fbe e7d7 cf97 7bfe e5e7  ..K.o/?.....{...
-00000d50: afcb e3fe d3bc 3f6c eeb2 25f1 7c7e 3a0f  ......?l..%.|~:.
-00000d60: 593e d8d8 80b1 4da8 3b60 3b44 889c 4448  Y>....M.;`;D..DH
-00000d70: 4db0 ca8d 7f04 fc63 fb88 f3a8 d7a2 c567  M......c.......g
-00000d80: 242e 02d4 4140 b43a b8fa d868 43df 6d33  $...A@.:...hC.m3
-00000d90: 6d6b 57bf a2bc 2c0c a943 5717 a8b1 b6c1  mkW...,..CW.....
-00000da0: da18 a8c8 ee24 4bc9 e80f 7435 c768 b1a0  .....$K...t5.h..
-00000db0: b4ed bb22 cd3d 40ee 909d 715a ae61 bdec  ...".=@...qZ.a..
-00000dc0: a9fd 8f9f 9b5e ccee dea2 818b 0da8 4bf6  .....^........K.
-00000dd0: 29a6 426f 8350 acab cebc f7e8 bede 0100  ).Bo.P..........
+000004d0: 3030 3030 3036 3020 3030 3030 3030 3630  0000060 00000060
+000004e0: 2037 6666 6666 6666 6620 0d0a 50dc 09a2   7fffffff ..P...
+000004f0: 7c44 0200 50dc 09a2 7c44 0200 0000 0000  |D..P...|D......
+00000500: 6100 6100 3900 3800 3300 6400 3000 3000  a.a.9.8.3.d.0.0.
+00000510: 2d00 3200 3500 3400 3700 2d00 3400 6100  -.2.5.4.7.-.4.a.
+00000520: 3700 6100 2d00 6100 3200 6500 6200 2d00  7.a.-.a.2.e.b.-.
+00000530: 6500 6400 3900 6300 3900 3300 3700 6600  e.d.9.c.9.3.7.f.
+00000540: 3800 6100 3300 6200 0000 0000 0d0a 3030  8.a.3.b.......00
+00000550: 3030 3030 3966 2030 3030 3030 3230 3020  00009f 00000200 
+00000560: 3766 6666 6666 6666 200d 0a95 8f41 0a02  7fffffff ....A..
+00000570: 310c 45f7 0373 89ba 6d20 693a a6bd 80f7  1.E..s..m i:....
+00000580: 4866 3a3b 1106 5c49 4fe6 c223 7905 6b47  Hf:;..\IO..#y.kG
+00000590: c1ad 10c2 4ff2 f348 9ef7 c78d fc38 ec09  ....O..H.....8..
+000005a0: bb0a 3f35 7ad5 9c78 4184 3045 81a8 a2a0  ..?5z..xA.0E....
+000005b0: a118 9425 cf99 654d ca56 bd3b 5db6 b3db  ...%..eM.V.;]...
+000005c0: 17dd 7675 9f46 1bb8 c620 cfa1 6012 35a0  ..vu.F... ..`.5.
+000005d0: 9809 62b6 23a8 69e3 f124 6491 740e e6b9  ..b.#.i..$d.t...
+000005e0: 766f 83f4 13dc c179 124c eba2 0ab3 cd05  vo.....y.L......
+000005f0: 6248 198c 8501 4527 9568 a564 f254 ffb2  bH....E'.h.d.T..
+00000600: 873a 0eef e81f 7e35 d617 0000 0000 0000  .:....~5........
+00000610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000760: 0000 0000 0000 0000 0000 000d 0a30 3030  .............000
+00000770: 3030 3036 3420 3030 3030 3030 3634 2037  00064 00000064 7
+00000780: 6666 6666 6666 6620 0d0a 50dc 09a2 7c44  fffffff ..P...|D
+00000790: 0200 50dc 09a2 7c44 0200 0000 0000 6100  ..P...|D......a.
+000007a0: 6100 3900 3800 3300 6400 3000 3000 2d00  a.9.8.3.d.0.0.-.
+000007b0: 3200 3500 3400 3700 2d00 3400 6100 3700  2.5.4.7.-.4.a.7.
+000007c0: 6100 2d00 6100 3200 6500 6200 2d00 6500  a.-.a.2.e.b.-.e.
+000007d0: 6400 3900 6300 3900 3300 3700 6600 3800  d.9.c.9.3.7.f.8.
+000007e0: 6100 3300 6200 2e00 3000 0000 0000 0d0a  a.3.b...0.......
+000007f0: 3030 3030 3034 3861 2030 3030 3030 3438  0000048a 0000048
+00000800: 6120 3766 6666 6666 6666 200d 0ab5 546d  a 7fffffff ...Tm
+00000810: 6fda 5614 fe1c 24fe 0372 a429 9170 77f1  o.V...$..r.).pw.
+00000820: b50d 5ed4 0f4d 9b40 2243 2220 10f8 e637  ..^..M.@"C" ...7
+00000830: 0284 50d4 8213 5c45 ca92 a99b 9668 d5a4  ..P...\E.....h..
+00000840: 4d9b 36ad 4db6 6a9f e91a 1a16 1af2 17ae  M.6.M.j.........
+00000850: 7fc9 fec2 cebd 3681 2634 ab56 15b0 0de7  ......6.&4.V....
+00000860: 9ef3 9ce7 79ce e5fe d3bf 7c82 c3c1 c013  ....y.....|.....
+00000870: 5109 23ff 1df1 9efe 8b9f 701b be20 154a  Q.#.......p.. .J
+00000880: 217f d72f 8cb0 627a b138 360c 4396 90c5  !../..bz.86.C...
+00000890: 9764 1ce1 4543 b3f8 9885 318f 2d4d 33e4  .d..EC....1.-M3.
+000008a0: 08d2 a592 12e6 c80b 778f f4c8 7377 9f9c  ........w...sw..
+000008b0: bb7b ee21 3c7b a4c7 3198 0f42 808e bbb4  .{.!<{..1..B....
+000008c0: 21d0 6084 0481 de79 a817 9080 651c e5a3  !.`....y....e...
+000008d0: 3139 c68b 9a54 e263 5254 e663 58d2 a2b2  19...T.cRT.cX...
+000008e0: 850c 45d7 767d d594 c84b 3200 2a6f 4987  ..E.v}...K2.*oI.
+000008f0: fc42 06ec 7941 4ee1 eab8 cfc8 0bf6 ab4b  .B..yAN........K
+00000900: faee 1177 a57a a4de 372d 2c84 5973 1c16  ...w.z..7-,.Ys..
+00000910: 3d46 c100 cb8a 86b1 6710 f2aa 58b2 4fd7  =F......g...X.O.
+00000920: ff3e c2c0 3499 0638 8e7e e802 7b8c de2c  .>..4..8.~..{..,
+00000930: c3f3 1c21 df75 e4b9 4e07 c9ba 72c1 c034  ...!.u..N...r..4
+00000940: 794e 5e91 3ef0 ffd2 dd77 8f42 f427 08ec  yN^.>....w.B.'..
+00000950: 4070 0081 afc1 e773 b84e 40ec 2bdf f7bf  @p.....s.N@.+...
+00000960: 8726 b887 c140 30f0 19f9 8db9 d187 a52e  .&...@0.........
+00000970: b980 946e 30c0 0636 709f 42e4 d43d a080  ...n0..6p.B..=..
+00000980: a1c9 339c f102 8070 361b 0c4c c187 fce1  ..3....p6..L....
+00000990: 31a0 74c8 f700 7006 bd2f 2941 003f 84ee  1.t...p../)A.?..
+000009a0: c710 7b03 b56f c1f0 0198 7f0e 867f 074c  ..{..o.........L
+000009b0: a139 e9c1 188e 9998 6fe0 fbde 3036 333b  .9......o...063;
+000009c0: 4791 7f82 367f 912e 74a7 ab14 fff8 4ae9  G...6...t.....J.
+000009d0: 0168 ec51 13a0 0694 cd90 5f01 fc8d 7bc4  .h.Q......_...{.
+000009e0: 2a41 101d 370c 1724 5d93 e6b9 303d 9630  *A..7..$]...0=.0
+000009f0: e628 e979 8bd7 4c3e 01ca 0720 a20b 612a  .(.y..L>... ..a*
+00000a00: aa7b 1394 fc4c 5e42 ce05 98f5 941a 35b2  .{...L^B......5.
+00000a10: fa84 2af0 7440 bae7 106b ceb8 9fb3 b69d  ..*.t@...k......
+00000a20: c923 f824 d6fa 63fb 0172 9f85 8049 0720  .#.$..c..r...I. 
+00000a30: 4ea1 fc35 1984 6e56 906e 08a4 9d4d 5801  N..5..nV.n...MX.
+00000a40: 7c4f c657 90f5 daa3 ec69 bfc3 e880 6574  |O.W.....i....et
+00000a50: 3f52 f233 b321 f227 db9a 7d68 4ddb 4f91  ?R.3.!.'..}hM.O.
+00000a60: 1f41 05ec c110 78d4 9dd8 f7ce ed92 43e4  .A....x.......C.
+00000a70: 7746 fa94 9a37 0580 cc3f a6a4 4f33 68df  wF...7...?..O3h.
+00000a80: 39d6 6934 69bf e7dc 1589 ffd1 f66e 68b8  9.i4i........nh.
+00000a90: d5e6 de0f 4177 ee25 dd9f def0 bcfd cc6c  ....Aw.%.......l
+00000aa0: 1f91 f10d 219d 8fde b1ec f412 bda3 4761  ....!.........Ga
+00000ab0: 2718 3b6a d8d9 f02d db63 fbef 1c70 dcaa  '.;j...-.c...p..
+00000ac0: d66c 5a8f ea2c c84d 7361 cbd4 44a4 c514  .lZ..,.Msa..D...
+00000ad0: 3ea6 4b98 1765 2bca c369 1ae1 a39a 50d2  >.K..e+..i....P.
+00000ae0: 64ac a158 a934 3cf7 d0d5 8d9b e7e8 318d  d..X.4<.......1.
+00000af0: 3e64 058d 9e63 27db 789c a6fa e169 5d7b  >d...c'.x....i]{
+00000b00: 6cc9 e217 d168 ebf3 d507 8aa8 e7b7 37cc  l....h........7.
+00000b10: ad5c db10 6ab6 5e45 9564 46dc 5eaa ccd7  .\..j.^E.dF.^...
+00000b20: f4ad 945d 8cd7 5a45 0755 72b9 745c cd6e  ...]..ZE.Ur.t\.n
+00000b30: 5456 1d31 75bf ba93 2dae a751 3018 d0f2  TV.1u...-..Q0...
+00000b40: 52dd 68cf 03c4 4ecb 8034 2d91 46c6 8387  R.h...N..4-.F...
+00000b50: b68a 0ba2 5a5d acaa f5e5 88ea 6cb4 9219  ....Z]......l...
+00000b60: 65b3 b09e 2eab f994 adaf cfdb d00a 6979  e.............iy
+00000b70: a505 10ea 7a4a 3270 baa6 6714 87a2 7a90  ....zJ2p..g...z.
+00000b80: 4b1b 563c f258 af27 e562 3ce5 1404 a5bd  K.V<.X.'.b<.....
+00000b90: 9a59 7e68 26d2 db2b 9598 6d56 0132 9f6c  .Y~h&..+..mV.2.l
+00000ba0: 19f5 351b 2056 ee8b 3baa 902e 9bf1 8526  ..5. V..;......&
+00000bb0: a436 8db8 e268 ebe9 862e 884d 03d7 1c33  .6...h.....M...3
+00000bc0: 9e6b aa42 ca36 b6d6 2a4b 8972 538f 4bce  .k.B.6..*K.rS.K.
+00000bd0: 4a3d 85ac fc4e 8dc2 02c4 24e4 3158 dbcc  J=...N....$.1X..
+00000be0: 6fda c052 d2e3 ef40 4843 d100 71ab 6e9c  o..R...@HC..q.n.
+00000bf0: 6ba8 42d1 d6eb 6947 c543 c123 91d0 5601  k.B...iG.C.#..V.
+00000c00: 88a5 ad32 3213 f764 b5ad 08b4 7ba1 2db5  ...22..d....{.-.
+00000c10: cd4c 0c20 1760 128b a890 51aa 3a5e aec1  .L. .`....Q.:^..
+00000c20: 747c cb1b c24a 22d7 187a 43bd b85d c418  t|...J"..zC..]..
+00000c30: 79b3 56a8 de9c 189d c844 f230 b8b8 d236  y.V......D.0...6
+00000c40: da0a 2ee6 97c6 611a fa35 180a f15e 0f46  ......a..5...^.F
+00000c50: 3030 e84d 1d9b ce98 18f1 869d 2636 db12  00.M........&6..
+00000c60: 4eb6 2518 9e61 27ab f7b6 01ae 905d dbc9  N.%..a'......]..
+00000c70: 1684 724d cf2f 8c31 293b 5a76 c484 b2f8  ..rM./.1);Zv....
+00000c80: eff2 26b0 80fd b1d8 2a08 6b15 d511 ef4e  ..&.....*.k....N
+00000c90: fc4f 5d7f d2db bf0d 0a30 3030 3030 3032  .O]......0000002
+00000ca0: 3820 3030 3030 3030 3238 2037 6666 6666  8 00000028 7ffff
+00000cb0: 6666 6620 0d0a 50dc 09a2 7c44 0200 50dc  fff ..P...|D..P.
+00000cc0: 09a2 7c44 0200 0000 0000 6300 6f00 7000  ..|D......c.o.p.
+00000cd0: 7900 6900 6e00 6600 6f00 0000 0000 0d0a  y.i.n.f.o.......
+00000ce0: 3030 3030 3030 6463 2030 3030 3030 3230  000000dc 0000020
+00000cf0: 3020 3766 6666 6666 6666 200d 0a8d 9031  0 7fffffff ....1
+00000d00: 4e04 310c 45fb 95f6 1253 c792 2776 12a7  N.1.E....S..'v..
+00000d10: 46d0 5171 024f 6203 053b d242 81b4 da93  F.Qq.Ob..;.B....
+00000d20: 5170 24ae c0cc b0f4 d37c 4bd6 f7d7 fbfe  Qp$......|K.....
+00000d30: f9fa be70 381e 2e71 95c4 c418 a543 e9d6  ...p8..q.....C..
+00000d40: 812d 6510 9706 c829 e76c 7164 4f61 9769  .-e....).lqdOa.i
+00000d50: 5ce3 1a09 8dd6 04ba f404 ec95 4034 46f0  \...........@4F.
+00000d60: 3ab9 1a16 8ac5 c370 f7a2 a767 7b52 b7c7  :......p...g{R..
+00000d70: b9db c37c beff fcb0 d3fb eb7c 1aae c7c3  ...|.......|....
+00000d80: 750d 52ad 421d 1162 e202 ac45 41a3 4d60  u.R.B..b...EA.M`
+00000d90: bdb6 4ac5 4569 0abb 4c1b 574f 135a 5ae0  ..J.Ei..L.WO.ZZ.
+00000da0: 63ca 4b03 1c1b d446 193c 1336 f52e 9a63  c.K....F.<.6...c
+00000db0: 1816 92b7 8de0 06b1 9d5a 5746 950a 3225  .........ZWF..2%
+00000dc0: 02ce 5640 4b1e a168 74cd a428 eefb 3e84  ..V@K..ht..(..>.
+00000dd0: ffb9 f8a7 e136 d7f5 2f00 0000 0000 0000  .....6../.......
 00000de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000e90: 0000 000d 0a30 3030 3030 3032 3020 3030  .....00000020 00
-00000ea0: 3030 3030 3230 2037 6666 6666 6666 6620  000020 7fffffff 
-00000eb0: 0d0a 7059 4b60 4e44 0200 7059 4b60 4e44  ..pYK`ND..pYK`ND
-00000ec0: 0200 0000 0000 7200 6f00 6f00 7400 0000  ......r.o.o.t...
-00000ed0: 0000 0d0a 3030 3030 3030 3265 2030 3030  ....0000002e 000
-00000ee0: 3030 3230 3020 3766 6666 6666 6666 200d  00200 7fffffff .
-00000ef0: 0a7b bf7b 7fb5 914e 9aa9 4162 4a52 8ab9  .{.{...N..AbJR..
-00000f00: ae65 b289 89ae 4962 9aa5 6e92 8989 a1ae  .e....Ib..n.....
-00000f10: 85b1 456a a249 a2b9 99b9 9189 4e2d 0000  ..Ej.I......N-..
-00000f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000ef0: 0000 0000 0000 0000 0000 0000 000d 0a30  ...............0
+00000f00: 3030 3030 3032 3020 3030 3030 3030 3230  0000020 00000020
+00000f10: 2037 6666 6666 6666 6620 0d0a 50dc 09a2   7fffffff ..P...
+00000f20: 7c44 0200 50dc 09a2 7c44 0200 0000 0000  |D..P...|D......
+00000f30: 7200 6f00 6f00 7400 0000 0000 0d0a 3030  r.o.o.t.......00
+00000f40: 3030 3030 3265 2030 3030 3030 3230 3020  00002e 00000200 
+00000f50: 3766 6666 6666 6666 200d 0a7b bf7b 7fb5  7fffffff ..{.{..
+00000f60: 918e 8565 9a99 5152 b2a1 ae65 5aaa a5ae  ...e..QR...eZ...
+00000f70: 499a 85a5 6e92 99a5 a1ae 8561 5292 9181  I...n......aR...
+00000f80: b1b9 8971 729a 4e2d 0000 0000 0000 0000  ...qr.N-........
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -265,29 +265,29 @@
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000010f0: 000d 0a30 3030 3030 3032 3620 3030 3030  ...00000026 0000
-00001100: 3030 3236 2037 6666 6666 6666 6620 0d0a  0026 7fffffff ..
-00001110: 7059 4b60 4e44 0200 7059 4b60 4e44 0200  pYK`ND..pYK`ND..
-00001120: 0000 0000 7600 6500 7200 7300 6900 6f00  ....v.e.r.s.i.o.
-00001130: 6e00 0000 0000 0d0a 3030 3030 3030 3163  n.......0000001c
-00001140: 2030 3030 3030 3230 3020 3766 6666 6666   00000200 7fffff
-00001150: 6666 200d 0a7b bf7b 7f35 2f57 b591 a199  ff ..{.{.5/W....
-00001160: 8e81 0e90 6161 606c 68a4 6350 cbcb 0542  ....aa`lh.cP...B
-00001170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000011a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000011b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000011c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000011d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000010f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001150: 0000 0000 0000 0000 0000 000d 0a30 3030  .............000
+00001160: 3030 3032 3620 3030 3030 3030 3236 2037  00026 00000026 7
+00001170: 6666 6666 6666 6620 0d0a 50dc 09a2 7c44  fffffff ..P...|D
+00001180: 0200 50dc 09a2 7c44 0200 0000 0000 7600  ..P...|D......v.
+00001190: 6500 7200 7300 6900 6f00 6e00 0000 0000  e.r.s.i.o.n.....
+000011a0: 0d0a 3030 3030 3030 3163 2030 3030 3030  ..0000001c 00000
+000011b0: 3230 3020 3766 6666 6666 6666 200d 0a7b  200 7fffffff ..{
+000011c0: bf7b 7f35 2f57 b591 a199 8e81 0e90 6161  .{.5/W........aa
+000011d0: 606c 68a4 6350 cbcb 0542 0000 0000 0000  `lh.cP...B......
 000011e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000011f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -303,46 +303,53 @@
 000012e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000012f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001350: 0000 0000 000d 0a30 3030 3030 3032 3820  .......00000028 
-00001360: 3030 3030 3030 3238 2037 6666 6666 6666  00000028 7ffffff
-00001370: 6620 0d0a 7059 4b60 4e44 0200 7059 4b60  f ..pYK`ND..pYK`
-00001380: 4e44 0200 0000 0000 7600 6500 7200 7300  ND......v.e.r.s.
-00001390: 6900 6f00 6e00 7300 0000 0000 0d0a 3030  i.o.n.s.......00
-000013a0: 3030 3031 3165 2030 3030 3030 3230 3020  00011e 00000200 
-000013b0: 3766 6666 6666 6666 200d 0a8d 9141 6e5d  7fffffff ....An]
-000013c0: 210c 45f7 c218 47d8 180c cbc1 184b 7ff2  !.E...G......K..
-000013d0: 5ff5 5355 aaa2 ac2c 832e a95b a8df a4e3  _.SU...,...[....
-000013e0: 30e5 fa70 7df8 fbf5 e703 f3c8 2965 652f  0..p}.......)ee/
-000013f0: 6513 c199 6d02 db40 98de 1aec 4613 abe9  e...m..@....F...
-00001400: 428f 9c98 8eba ea82 5ada 068e 038b a8c0  B.......Z.......
-00001410: f18d 58b0 4961 4979 199f e5cd 61cd 1aac  ..X.IaIy....a...
-00001420: d319 86cd 03db cda4 9c53 3bef efb1 de4a  .........S;....J
-00001430: cab3 da58 051d 76e7 063c a706 4d10 9a93  ...X..v..<..M...
-00001440: 56f1 2e86 9cd3 be7e fc7e 3cfd 4a19 7d11  V......~.~<.J.}.
-00001450: 6b47 90a6 083c ca80 b979 c433 627e af42  kG...<...y.3b~.B
-00001460: 4439 792b cbd4 e4be 63e0 e513 9419 61d4  D9y+....c.....a.
-00001470: 7116 2fe9 429c 32f3 3e87 4e0c 4b2c c13c  q./.B.2.>.N.K,.<
-00001480: 0dd4 6c02 194e 2429 54b5 e5f4 baae 9f29  ..l..N$)T......)
-00001490: 9fc3 382a 2e68 8186 5b67 b043 6859 5ce4  ..8*.h..[g.ChY\.
-000014a0: 489b 2ad1 f3d7 79bd 3fae 67ca dbef 3e2c  H.*...y.?.g...>,
-000014b0: 6022 35e2 e32e 400c b207 b38a 8917 fb1f  `"5...@.........
-000014c0: 7f0f 0d63 8a5a fc0d f51d bab4 f6d0 a0e1  ...c.Z..........
-000014d0: 4cbd 9776 4219 ebe7 3f00 0000 0000 0000  L..vB...?.......
-000014e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000014f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000013a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000013b0: 0000 0000 0000 0000 0000 0000 0000 000d  ................
+000013c0: 0a30 3030 3030 3032 3820 3030 3030 3030  .00000028 000000
+000013d0: 3238 2037 6666 6666 6666 6620 0d0a 50dc  28 7fffffff ..P.
+000013e0: 09a2 7c44 0200 50dc 09a2 7c44 0200 0000  ..|D..P...|D....
+000013f0: 0000 7600 6500 7200 7300 6900 6f00 6e00  ..v.e.r.s.i.o.n.
+00001400: 7300 0000 0000 0d0a 3030 3030 3031 3164  s.......0000011d
+00001410: 2030 3030 3030 3230 3020 3766 6666 6666   00000200 7fffff
+00001420: 6666 200d 0a8d 9131 6e98 3108 46ef e2d9  ff ....1n.1.F...
+00001430: 54d8 c606 8e03 064b 59f2 5749 55a9 aa7a  T......KY.WIU..z
+00001440: b20c 3d52 af50 67e9 dc15 7df0 1ef0 e7e3  ..=R.Pg...}.....
+00001450: f7cf 56a5 9652 e974 5174 84d9 8280 4426  ..V..R.tQt....D&
+00001460: 2893 80b5 a9b9 5578 4eab 45f4 acee bb81  (.....UxN.E.....
+00001470: 9e54 a023 0abe b481 34f7 8e83 69ec 536a  .T.#....4...i.Sj
+00001480: a29f a9d1 60ef 1540 da0d 8442 2187 da58  ....`..@...B!..X
+00001490: 3372 6dad c54c 6504 22f4 490c 646c 603d  3rm..Le.".I.dl`=
+000014a0: 1d32 74eb e023 36bc 5423 ea84 bd41 b209  .2t..#6.T#...A..
+000014b0: d06a 04c2 b601 939d d035 82ec ff66 7dc1  .j.......5...f}.
+000014c0: 5277 ac61 9b03 46f3 0e44 dbc1 3305 d2b3  Rw.a..F..D..3...
+000014d0: 296f ca19 5ecb 7ebe fe78 793d cfa5 ef35  )o..^.~..xy=...5
+000014e0: 5058 413b d9cd 3b81 5b5f b79d a2a1 e05c  PXA;..;.[_.....\
+000014f0: 346a 797b 9e6f a52e 67e5 d92f 74f2 35c5  4jy{.o..g../t.5.
+00001500: 754d b133 a498 f51e 33d8 b096 eff9 f6fe  uM.3....3.......
+00001510: f2bc 963a e632 6325 d8d6 1c68 b60b f9f4  ...:.2c%...h....
+00001520: 3e7d c55d 6e70 f6f8 177f 2f95 e9b3 dc0c  >}.]np..../.....
+00001530: a2e5 5537 bcbf 9974 8f1a 93ce c2b1 1ad3  ..U7...t........
+00001540: afbf 0000 0000 0000 0000 0000 0000 0000  ................
 00001550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000015b0: 0000 0000 0000 0000 0000 00              ...........
+000015b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001620: 0000 0000 00                             .....
```

### Comparing `runner1c-0.58/runner1c/build/tools/epf/CloseAfterUpdate.epf` & `runner1c-0.59/runner1c/build/tools/epf/CloseAfterUpdate.epf`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 00000000: ffff ff7f 0002 0000 0a00 0000 0000 0000  ................
 00000010: 0d0a 3030 3030 3030 3738 2030 3030 3030  ..00000078 00000
 00000020: 3230 3020 3766 6666 6666 6666 200d 0a2f  200 7fffffff ../
-00000030: 0200 00b2 0200 00ff ffff 7fd8 0500 0057  ...............W
-00000040: 0600 00ff ffff 7f76 0800 00f9 0800 00ff  .......v........
-00000050: ffff 7f1d 0f00 009c 0f00 00ff ffff 7fbb  ................
-00000060: 1100 003e 1200 00ff ffff 7faf 1900 002e  ...>............
-00000070: 1a00 00ff ffff 7f4d 1c00 0094 1c00 00ff  .......M........
-00000080: ffff 7fb3 1e00 00f2 1e00 00ff ffff 7f11  ................
-00000090: 2100 0056 2100 00ff ffff 7f75 2300 00bc  !..V!......u#...
+00000030: 0200 00b2 0200 00ff ffff 7fd5 0500 0054  ...............T
+00000040: 0600 00ff ffff 7f73 0800 00f6 0800 00ff  .......s........
+00000050: ffff 7f1a 0f00 0099 0f00 00ff ffff 7fb8  ................
+00000060: 1100 003b 1200 00ff ffff 7fac 1900 002b  ...;...........+
+00000070: 1a00 00ff ffff 7f4a 1c00 0091 1c00 00ff  .......J........
+00000080: ffff 7fb0 1e00 00ef 1e00 00ff ffff 7f0e  ................
+00000090: 2100 0053 2100 00ff ffff 7f72 2300 00b9  !..S!......r#...
 000000a0: 2300 00ff ffff 7f00 0000 0000 0000 0000  #...............
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -30,92 +30,92 @@
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 000d  ................
 00000230: 0a30 3030 3030 3036 3420 3030 3030 3030  .00000064 000000
-00000240: 3634 2037 6666 6666 6666 6620 0d0a b0f5  64 7fffffff ....
-00000250: 4b60 4e44 0200 b0f5 4b60 4e44 0200 0000  K`ND....K`ND....
+00000240: 3634 2037 6666 6666 6666 6620 0d0a 6003  64 7fffffff ..`.
+00000250: 0aa2 7c44 0200 6003 0aa2 7c44 0200 0000  ..|D..`...|D....
 00000260: 0000 3500 3100 6100 3000 3400 3000 6400  ..5.1.a.0.4.0.d.
 00000270: 3400 2d00 6200 6100 3800 3500 2d00 3400  4.-.b.a.8.5.-.4.
 00000280: 3800 3600 3900 2d00 3800 3700 3200 3100  8.6.9.-.8.7.2.1.
 00000290: 2d00 3000 3400 3700 6600 3500 3400 6200  -.0.4.7.f.5.4.b.
 000002a0: 6500 3000 6400 6400 3700 2e00 3000 0000  e.0.d.d.7...0...
-000002b0: 0000 0d0a 3030 3030 3033 3037 2030 3030  ....00000307 000
-000002c0: 3030 3330 3720 3766 6666 6666 6666 200d  00307 7fffffff .
-000002d0: 0aed 55bd 6ed3 5014 36dd b0e4 77b8 4a97  ..U.n.P.6...w.J.
-000002e0: 4484 36a5 4311 850d 8901 8967 6080 482c  D.6.C......g`.H,
-000002f0: b030 2021 449c 9496 2a15 552b 1055 a5b6  .0 !D...*.U+.U..
-00000300: a4e2 6742 7253 4cd2 8638 af70 ee3b b033  ..gBrSL..8.p.;.3
-00000310: 3187 ef9c ebeb 3876 aa54 6504 2771 aecf  1.....8v.Te.'q..
-00000320: ff77 fe3c 1c0e 5f3a 338e 73c9 3197 e756  .w.<.._:3.s.1..V
-00000330: e45a b8ae 92c3 52d5 5cca 73ef 4064 15bf  .Z....R.\.s.@d..
-00000340: 21d4 3e41 ede7 8c39 5bb5 6b15 951c 526a  !.>A...9[.k...Rj
-00000350: c1ef bbf7 efdd 9e71 ec3f 5f8f 9cc7 4ed5  .......q.?_...N.
-00000360: 7932 e6b5 5255 b1f6 98fa afde e0f9 6279  y2..RU........by
-00000370: a15c 2917 0ae5 ca0b fa81 4f5f 37e9 8476  .\).......O_7..v
-00000380: f05f a750 d7f4 0a85 74a2 7dcf f5dc f979  ._.P....t.}....y
-00000390: 4507 ba46 915e a32e d881 aeeb 0da5 7d8a  E..F.^........}.
-000003a0: e848 3741 e852 a8a8 4301 b545 f535 54fb  .H7A.R..C..E.5T.
-000003b0: 90dc 542c 8163 0446 cf12 e7c4 a0b1 ba0d  ..T,.c.F........
-000003c0: 5687 dab0 1de8 75e8 8708 2432 c6fa 20ad  V.....u...$2.. .
-000003d0: 191d 0a6f 88b8 a22d dd10 436d 8ad4 5545  ...o...-..Cm..UE
-000003e0: 3bda 17ef 902d 2bb8 f6c1 ec4e 703a 29bc  ;....-+....Np:).
-000003f0: 48e2 f05c fa08 9b7d 3ad5 ab26 e21c 506a  H..\...}:..&..Pj
-00000400: a571 d2fb 3c4c dacf a32c 9614 7d85 559f  .q..<L...,..}.U.
-00000410: 0630 57d3 75cf bd8c 2f7d 8040 8751 e80d  .0W.u.../}.@.Q..
-00000420: e340 dd1a c3b1 1ccb 1dc0 dc40 9c9e 5200  .@.........@..R.
-00000430: c264 4d45 7b8c 6d1b 821c b1e0 e798 8b85  .dME{.m.........
-00000440: 7c4c b873 7557 10ce 05ba eba9 f3d0 7986  |L.suW........y.
-00000450: 7baa bb96 1e2c a8e4 30de 5d9e 3b4b ef6c  {....,..0.].;K.l
-00000460: 395a 9c2d 9333 4035 b443 44d6 63d4 d275  9Z.-.3@5.CD.c..u
-00000470: bb4c e428 016c 5f72 bd26 b187 528d 2eb8  .L.(.l_r.&..R...
-00000480: 117d 1f95 32b6 b18d e710 55c0 1d9f 96c8  .}..2.....U.....
-00000490: 7f93 2c26 92ec e618 c480 db78 5672 d243  ..,&.......xVr.C
-000004a0: ea7c 6960 536a 3ae6 eefb 3f02 ffd8 08d4  .|i`Sj:...?.....
-000004b0: 90e6 8001 83df 17a9 13da 02ae 8e6e ceb1  .............n..
-000004c0: 4501 fc0a 77ee 28ae c805 8d15 4b85 1203  E...w.(.....K...
-000004d0: 6280 c0d1 d36f 4625 65f2 aea8 8450 4ec3  b....oF%e....PN.
-000004e0: edda 1ca4 bba3 aef2 0930 7229 2ba9 5252  .........0r)+.RR
-000004f0: d776 6ed2 d288 3ea0 9e12 4f5c 639f 82bf  .vn...>...O\c...
-00000500: e9c5 2f71 c2a5 1333 328a 8b99 f61a bbca  ../q...32.......
-00000510: b75b 263a 643a 096e 520b 6572 b2b8 3c1d  .[&:d:.nR.er..<.
-00000520: 7f7e 7261 2f88 e73e 04a1 a69b 663c 06ba  .~ra/..>....f<..
-00000530: 2175 b2b1 8a76 56d4 c26f f123 3c43 9c13  !u...vV..o.#<C..
-00000540: 9079 6cc7 edc3 59d9 54b2 732c 7782 ab0b  .yl...Y.T.s,w...
-00000550: 5620 e7b3 79a6 d773 0f7b 0eaf 0c7c 126e  V ..y..s.{...|.n
-00000560: 31ed 747a 7dd2 d253 4a35 9b62 a656 b565  1.tz}..SJ5.b.V.e
-00000570: 66b6 770b 53d0 90d7 c291 6cee 3086 b2ca  f.w.S.....l.0...
-00000580: af01 04cb 81ef e49d 64a5 b81c 8cb8 c145  ........d......E
-00000590: 2962 8fd4 38e9 7ab3 6427 d012 26ad 3dde  )b..8.z.d'..&.=.
-000005a0: 5c87 7838 85a5 75ce 38bd 65d0 d2b8 57d4  \.x8..u.8.e...W.
-000005b0: 4877 d9ee 33a9 fe59 1a37 d514 6ff4 1928  Hw..3..Y.7..o..(
-000005c0: b044 c617 474c b48b 33bd 52b2 0939 4796  .D..GL..3.R..9G.
-000005d0: 47cc f805 eeb9 7f00 0d0a 3030 3030 3030  G.........000000
-000005e0: 3630 2030 3030 3030 3036 3020 3766 6666  60 00000060 7fff
-000005f0: 6666 6666 200d 0ab0 f54b 604e 4402 00b0  ffff ....K`ND...
-00000600: f54b 604e 4402 0000 0000 0036 0032 0031  .K`ND......6.2.1
-00000610: 0037 0036 0062 0062 0038 002d 0036 0038  .7.6.b.b.8.-.6.8
-00000620: 0063 0066 002d 0034 0037 0066 0033 002d  .c.f.-.4.7.f.3.-
-00000630: 0038 0063 0039 0030 002d 0035 0065 0035  .8.c.9.0.-.5.e.5
-00000640: 0039 0032 0038 0039 0065 0064 0036 0032  .9.2.8.9.e.d.6.2
-00000650: 0064 0000 0000 000d 0a30 3030 3030 3061  .d.......000000a
-00000660: 3520 3030 3030 3032 3030 2037 6666 6666  5 00000200 7ffff
-00000670: 6666 6620 0d0a 954f 3b0a c330 0cdd 0bb9  fff ...O;..0....
-00000680: 84bb 5a60 f927 fb14 3d83 643b d0a5 43a0  ..Z`.'..=.d;..C.
-00000690: 4329 3e59 871e a957 a893 50c8 5a10 e23d  C)>Y...W..P.Z..=
-000006a0: f1f4 9ef4 79bd 9fa8 a7d3 decc 86ec 811b  ....y...........
-000006b0: 1d2d 5214 4910 5399 c1d3 ec20 956c 20b4  .-R.I.S.... .l .
-000006c0: 906d caad 465b bb56 97a5 5e6f bc3c d4be  .m..F[.V..^o.<..
-000006d0: ac96 bb3a 0c87 400d 2fd4 ce36 9388 05d0  ...:..@./..6....
-000006e0: 6704 9f25 020b 1378 1708 c523 172b da75  g..%...x...#.+.u
-000006f0: bd26 0fa3 ed14 7556 1ac9 a4b9 3243 91d2  .&....uV....2C..
-00000700: c08f 6010 470e 0c71 60f2 d25a 468d fd2f  ..`.G..q`..ZF../
-00000710: b9ed d369 aded d31f 36fd 0b00 0000 0000  ...i....6.......
+000002b0: 0000 0d0a 3030 3030 3033 3034 2030 3030  ....00000304 000
+000002c0: 3030 3330 3420 3766 6666 6666 6666 200d  00304 7fffffff .
+000002d0: 0aed 55bd 6ed3 5014 3665 c292 dfe1 2a59  ..U.n.P.6e....*Y
+000002e0: 1211 da94 0e45 1436 245e 8301 2ab1 c0c2  .....E.6$^..*...
+000002f0: 8004 8838 2929 552a aa56 20aa 4ab4 a4e2  ...8))U*.V .J...
+00000300: 6742 7253 4cd2 8638 af70 ee3b b0f3 08e1  gBrSL..8.p.;....
+00000310: 3bc7 bece 8d9d 2a55 19c1 499c ebf3 ff9d  ;.....*U..I.....
+00000320: 3f8f 46a3 97ce 9ce3 5c72 e2cb 73ab 722d  ?.F.....\r..s.r-
+00000330: de50 e961 7935 be94 e7de 8548 13bf 11d4  .P.ay5.....H....
+00000340: 3e43 edd7 5c7c 366a d7ab 2a3d 586a f72e  >C..\|6j..*=Xj..
+00000350: bb87 cfef cc39 e69f af87 ce23 67d5 793c  .....9.....#g.y<
+00000360: e1b5 baaa 12ed 09f5 dffd e1b3 a5ca 62a5  ..............b.
+00000370: 5a29 142a d517 f413 9f81 6ed1 09ed e2bf  Z).*......n.....
+00000380: 4ea1 aee9 350a e944 fb9e ebb9 0b0b 8a0e  N...5..D........
+00000390: 748d 22bd 4e3d b003 5dd7 9b4a fb14 d191  t.".N=..]..J....
+000003a0: 6e81 d0a3 5051 9702 ea88 ea6b a80e 20b9  n...PQ.....k.. .
+000003b0: a558 02c7 088c be21 ce8b c1d8 ea0e 585d  .X.....!......X]
+000003c0: eac0 76a0 37a0 1f22 9028 3636 0069 3dd6  ..v.7..".(66.i=.
+000003d0: a1f0 a688 2bda d60d 31d4 a148 5d53 b4ab  ....+...1..H]S..
+000003e0: 7df1 0ed9 8a82 6b1f ccde 14a7 d3c2 8b24  }.....k........$
+000003f0: 0ecf a54f b039 a053 dd8c 23ce 01a5 b68d  ...O.9.S..#.....
+00000400: 93de e761 d27e 1e65 a9ac e81b acfa 3484  ...a.~.e......4.
+00000410: b99a ae7b ee15 7ce9 2304 ba8c 426f c60e  ...{..|.#...Bo..
+00000420: d4ed 091c 2b89 dc01 cc0d c5e9 2905 204c  ....+.......). L
+00000430: d754 f481 b1ed 4090 2316 fc1c 73a9 908f  .T....@.#...s...
+00000440: 0977 aeee 1ac2 b940 773d 711e 384f 71b7  .w.....@w=q.8Oq.
+00000450: ba6b f9fe a24a 0f93 dde5 b945 7a67 cad1  .k...J.....Ezg..
+00000460: e66c c539 03d4 9876 88c8 fa8c 5aba 6e8f  .l.9...v....Z.n.
+00000470: 891c 2580 ed4b aed7 25f6 50aa d103 37a2  ..%..K..%.P...7.
+00000480: 1fe3 5226 3676 f01c a20a b8e3 d316 f9ef  ..R&6v..........
+00000490: 92c5 5492 dd1c 8318 701b 1725 277d a4ce  ..T.....p..%'}..
+000004a0: 9706 8e4b 4dc7 dc7d ff47 e01f 1b81 1ad2  ...KM..}.G......
+000004b0: 1c30 60f0 0722 7542 dbc0 d5d5 ad79 b628  .0`.."uB.....y.(
+000004c0: 805f e1ce 1dc5 15b9 a0b1 52b9 5066 400c  ._........R.Pf@.
+000004d0: 1038 fafa cdb8 a44c de13 9510 ca36 dc9e  .8.....L.....6..
+000004e0: c981 dd1d 7595 4f40 2c67 59b1 4a49 3dd3  ....u.O@,gY.JI=.
+000004f0: b969 4b23 fa80 fa4a 3c71 8d7d 0afe a617  .iK#...J<q.}....
+00000500: bf26 0997 4ecc c828 2ea6 ed35 7195 6fb7  .&..N..(...5q.o.
+00000510: 4c74 c874 1adc b416 cae4 6469 6536 fefc  Lt.t......die6..
+00000520: e4c2 5e90 cc7d 0842 4db7 e2f1 18ea 86d4  ..^..}.BM.......
+00000530: c9c4 2ada 5951 03bf cd8f f00c 714e 40e6  ..*.YQ......qN@.
+00000540: b193 b40f 6765 4bc9 ce31 dc29 ae2e 5881  ....geK..1.)..X.
+00000550: 9ccf d699 5ecf 3dec 39bc 32f0 69b8 25db  ....^.=.9.2.i.%.
+00000560: e9ec fad8 d233 4a55 b498 d6aa 36cc ccf6  .....3JU....6...
+00000570: 6e63 0a1a f25a 3892 cd1d 2650 9afc 1a40  nc...Z8...&P...@
+00000580: b01c f86e de49 568a cbc1 881b 5c94 12f6  ...n.IV.....\...
+00000590: 488d 93ae b7ca 6602 0d61 dada e3cd 7588  H.....f..a....u.
+000005a0: 8753 58da e08c d35b 062d 8d7b 558d 7557  .SX....[.-.{U.uW
+000005b0: cc3e 93ea 9fa5 714b cdf0 465f 8002 4b64  .>....qK..F_..Kd
+000005c0: 7271 2444 b338 ed95 924d c839 b23c 6626  rq$D.8...M.9.<f&
+000005d0: 2f70 cffd 030d 0a30 3030 3030 3036 3020  /p.....00000060 
+000005e0: 3030 3030 3030 3630 2037 6666 6666 6666  00000060 7ffffff
+000005f0: 6620 0d0a 6003 0aa2 7c44 0200 6003 0aa2  f ..`...|D..`...
+00000600: 7c44 0200 0000 0000 3600 3200 3100 3700  |D......6.2.1.7.
+00000610: 3600 6200 6200 3800 2d00 3600 3800 6300  6.b.b.8.-.6.8.c.
+00000620: 6600 2d00 3400 3700 6600 3300 2d00 3800  f.-.4.7.f.3.-.8.
+00000630: 6300 3900 3000 2d00 3500 6500 3500 3900  c.9.0.-.5.e.5.9.
+00000640: 3200 3800 3900 6500 6400 3600 3200 6400  2.8.9.e.d.6.2.d.
+00000650: 0000 0000 0d0a 3030 3030 3030 6135 2030  ......000000a5 0
+00000660: 3030 3030 3230 3020 3766 6666 6666 6666  0000200 7fffffff
+00000670: 200d 0a95 4f3b 0ac3 300c dd0b b984 bb5a   ...O;..0......Z
+00000680: 60f9 27fb 143d 8364 3bd0 a543 a043 293e  `.'..=.d;..C.C)>
+00000690: 5987 1ea9 57a8 9350 c85a 10e2 3df1 f49e  Y...W..P.Z..=...
+000006a0: f479 bd9f a8a7 d3de cc86 ec81 1b1d 2d52  .y............-R
+000006b0: 1449 1053 99c1 d3ec 2095 6c20 b490 6dca  .I.S.... .l ..m.
+000006c0: ad46 5bbb 5697 a55e 6fbc 3cd4 beac 96bb  .F[.V..^o.<.....
+000006d0: 3a0c 8740 0d2f d4ce 3693 8805 d067 049f  :..@./..6....g..
+000006e0: 2502 0b13 7817 08c5 2317 2bda 75bd 260f  %...x...#.+.u.&.
+000006f0: a3ed 1475 561a c9a4 b932 4391 d2c0 8f60  ...uV....2C....`
+00000700: 1047 0e0c 7160 f2d2 5a46 8dfd 2fb9 edd3  .G..q`..ZF../...
+00000710: 69ad edd3 1f36 fd0b 0000 0000 0000 0000  i....6..........
 00000720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -129,141 +129,141 @@
 00000800: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000870: 0000 0000 0000 0d0a 3030 3030 3030 3634  ........00000064
-00000880: 2030 3030 3030 3036 3420 3766 6666 6666   00000064 7fffff
-00000890: 6666 200d 0ab0 f54b 604e 4402 00b0 f54b  ff ....K`ND....K
-000008a0: 604e 4402 0000 0000 0036 0032 0031 0037  `ND......6.2.1.7
-000008b0: 0036 0062 0062 0038 002d 0036 0038 0063  .6.b.b.8.-.6.8.c
-000008c0: 0066 002d 0034 0037 0066 0033 002d 0038  .f.-.4.7.f.3.-.8
-000008d0: 0063 0039 0030 002d 0035 0065 0035 0039  .c.9.0.-.5.e.5.9
-000008e0: 0032 0038 0039 0065 0064 0036 0032 0064  .2.8.9.e.d.6.2.d
-000008f0: 002e 0030 0000 0000 000d 0a30 3030 3030  ...0.......00000
-00000900: 3630 3520 3030 3030 3036 3035 2037 6666  605 00000605 7ff
-00000910: 6666 6666 6620 0d0a ed58 4b8f 1b45 10b6  fffff ...XK..E..
-00000920: 728b 25ff 87d1 e4b2 8ba6 43bf e645 8438  r.%.......C..E.8
-00000930: f007 9010 176e e399 f189 0414 25a7 c862  .....n......%..b
-00000940: 1f68 1391 8895 2250 5010 5916 459c 9dcd  .h...."PP.Y.E...
-00000950: 3a31 f13e fe42 0f7f 849f b054 57f7 8cdb  :1.>.B.....TW...
-00000960: 8fd8 219b 0424 187b 77ba 6baa abbe aafe  ..!..$.{w.k.....
-00000970: aa7a 76cf cece be6e 5d68 e92f 5e9d 36c5  .zv....n]h./^.6.
-00000980: 8b25 1ede 39a5 5edc 3397 d769 bf0f 7a77  .%..9.^.3..i..zw
-00000990: 2eb6 5a67 b0ec 1a8c 9f5c 30e3 d6ff d77f  ..Zg.....\0.....
-000009a0: e2aa e9c1 a9d7 0c1c 7a0c 3ebf f9d1 1f1f  ........z.>.....
-000009b0: 5f68 d577 7df5 5a5f b6ae b7ae 4e2f 975e  _h.w}.Z_....N/.^
-000009c0: 3358 b1fc 2a2c 2f5a 375b 5fb4 4ad7 44d4  3X..*,/Z7[_.J.D.
-000009d0: b504 d503 c7c4 9fe3 d34e fb92 7aa4 9ea8  .........N..z...
-000009e0: b11a 549b d556 75cf d3d3 6a43 0d40 7802  ..T..Vu...jC.@x.
-000009f0: 82db 6aa4 5ec0 cfbe 3a01 f9dd 6a0b c6bf  ..j.^...:...j...
-00000a00: abc7 f06c 431d 5577 3bed 4e5b edc1 f8a4  ...lC.Uw;.N[....
-00000a10: da51 4375 586d ebb5 1e8a 46ea 11a8 bfa8  .QCuXm....F.....
-00000a20: 36ec b2d1 da7a a77d 11be ea87 6a13 3c8e  6....z.}....j.<.
-00000a30: 3cf5 b31a 6add 6ded 1b10 ecaa 7d70 09c6  <...j.m.....}p..
-00000a40: c0e5 604d ed81 4823 3952 4314 3f80 f1a9  ..`M..H#9RC.?...
-00000a50: 56d6 8fd7 3df5 2b28 3e55 876a 0036 2f4e  V...=.+(>U.j.6/N
-00000a60: e386 9510 ccac 85ea eeb4 8d55 2eae 68b0  ...........U..h.
-00000a70: 0fc1 cb31 3cde a961 5fb1 51ec c183 43d0  ...1<..a_.Q...C.
-00000a80: 1b57 dfe9 34a1 c345 c97b a49e c11d 6082  .W..4..E.{....`.
-00000a90: 9951 b5bb e69b 84a9 0330 baa1 fda8 fb00  .Q.......0......
-00000aa0: ec14 2463 ed08 7e8e 61f5 26e6 4cef cd31  ..$c..~.a.&.L..1
-00000ab0: ea8e f109 acf7 034f fda8 8ee1 b15e 7e00  .......O.....^~.
-00000ac0: cbc7 a076 8a7b b009 31ad af1b 800e f099  ...v.{..1.......
-00000ad0: 0d32 db76 c951 7028 a046 e6e1 0c2b f621  .2.v.Qp(.F...+.!
-00000ae0: cc6d 0864 a801 01dc e1bc 5140 f518 748e  .m.d......Q@..t.
-00000af0: 61cb 77f4 762f e3c6 6b47 ff52 0e69 37b8  a.w.v/..kG.R.i7.
-00000b00: 0b76 eb5d c20e 715f d163 75a7 b6b4 d8fa  .v.]..q_.cu.....
-00000b10: 2cab eec3 ecb9 3ad0 c8ab ade5 7c78 5556  ,.....:.....|xUV
-00000b20: c303 0df0 e10c 6375 2a8e e659 3d29 a159  ......cu*..Y=).Y
-00000b30: 7a81 7c7b 6d05 47dd b80d 437f 69d8 b90d  z.|{m.G...C.i...
-00000b40: 391a 21c6 a12e e535 f513 5879 56dd 7b45  9.!....5..XyV.{E
-00000b50: fe2c dada d7aa c107 e065 50dd f6dc 34ad  .,.......eP...4.
-00000b60: 6381 2dcb 94f7 e1a2 5d5f e9cc f571 e535  c.-.....]_...q.5
-00000b70: 835c b525 36f7 df43 c9ec 7ae0 6100 7573  .\.%6..C..z.a.us
-00000b80: 88bb 7ae2 41eb 1c40 031d eb1a 7eae a902  ..z.A..@....~...
-00000b90: 33e4 a895 eb7d 581a 77e0 f9ef 5d2e bfea  3....}X.w...]...
-00000ba0: 611b b075 728c edf0 37ec 3663 a48d 6dd0  a..ur...7.6c..m.
-00000bb0: 0017 d274 1f23 bca3 290e 71cc da1c 5dc6  ...t.#..).q...].
-00000bc0: 4e06 e5dd 74b1 babd 6faf d5b0 ac0e d6cb  N...t...o.......
-00000bd0: 10a0 1f55 bb48 13c7 d3e5 e9c4 cc31 d3c2  ...U.H.......1..
-00000be0: 5383 37d0 9ef0 342b 627b b0ea c1f4 b176  S.7...4+b{.....v
-00000bf0: 8bc7 41a7 7d8b 25fa b71e 044c 8ffc eb37  ..A.}.%....L...7
-00000c00: fdc0 474a 3438 3da6 f63d dd7f b070 a070  ..GJ48=..=...p.p
-00000c10: 4fe6 db82 07c0 014b f50d 84f0 d4d0 c0b4  O......K........
-00000c20: 38bf df69 f783 3090 3c95 6914 f334 ec6b  8..i..0.<.i..4.k
-00000c30: 3f34 cdf3 228f 6352 662c 2332 8b0a 9275  ?4..".cRf,#2...u
-00000c40: 594e 8414 6199 1519 9742 20be 1a5e 64f0  YN..a....B ..^d.
-00000c50: 8940 e272 b4ba 601e 0722 a0a0 ca28 edc3  .@.r..`.."...(..
-00000c60: 0035 d010 e1fc 656b e6e7 6645 3c2b e06c  .5....ek..fE<+.l
-00000c70: 22a1 6609 dcf5 4726 82f1 9ca6 8487 718f  ".f...G&......q.
-00000c80: c82e 4f49 9727 94f0 4416 4592 96bd 9c95  ..OI.'..D.E.....
-00000c90: 7d13 8f5d 0300 f5bd 1ff0 c8da c0f8 28a4  }..]..........(.
-00000ca0: 4a18 0d98 2546 281b 6fbe 1f10 a6bf 6007  J...%F(.o.....`.
-00000cb0: 26fd 733d b510 0c22 164c 4820 9db1 2584  &.s=...".LH ..%.
-00000cc0: 690a e67c de51 03e6 d799 488c fdb7 0891  i..|.Q....H.....
-00000cd0: 1b88 2865 8ba0 ac66 86f9 06c6 2e8a 7990  ..(e...f......y.
-00000ce0: 04cc 0a6c 0eac 54a7 82cf 4845 98a2 ae40  ...l..T...HE...@
-00000cf0: 69d2 c8a1 86b4 ba9c 88a9 4374 d8ca 48d6  i.........Ct..H.
-00000d00: 2474 c069 e530 6ecc 3788 39ce 7a79 5c72  $t.i.0n.7.9.zy\r
-00000d10: 5a90 1e97 8cc8 88e6 a45b f424 09b3 2249  Z........[.$.."I
-00000d20: ca50 c632 0b8d 31f1 064a 6355 21fc 9385  .P.2..1..JcU!...
-00000d30: c15c 4a5a 1ace 757b 0f8e 0d3c 439e bb87  .\JZ..u{...<C...
-00000d40: d807 be4d 74bd bd58 5996 e9b5 33f6 6ee8  ...Mt..XY...3.n.
-00000d50: 6bfd ca9a 520e b1e8 a488 f487 09a6 1965  k...R..........e
-00000d60: fb00 1202 6c45 0ddb ecc4 aeb1 1ada 2e4b  ....lE.........K
-00000d70: 9769 bc8a 0d1e 302e ce67 e465 1a36 1c19  .i....0..g.e.6..
-00000d80: b0a6 cde8 99e8 3be9 604d 4a98 845d d647  ......;.`MJ..].G
-00000d90: fe21 1c38 fad5 6bee f501 46f8 da30 fdda  .!.8..k...F..0..
-00000da0: e2bb 75b7 20c3 2261 6511 7149 52ce 6222  ..u. ."ae.qIR.b"
-00000db0: cb48 9024 2cba 2497 b9c8 bb49 5c64 5909  .H.$,.$....I\dY.
-00000dc0: f50a 9a29 d2ed 93ec c68d f2fa 351f 279f  ...)........5.'.
-00000dd0: 36dd ee5f 5971 8885 b0a4 ef04 3e55 4e38  6.._Yq......>UN8
-00000de0: 114e aaa7 125f 4b2c 8ffd cf0c adf1 0e8c  .N..._K,........
-00000df0: 7697 9ca7 1666 0bd1 05e9 008a e238 e62c  v....f.......8.,
-00000e00: 0c9a f830 ba34 8b23 290a 4e58 5aa6 4486  ...0.4.#).NXZ.D.
-00000e10: 2527 4992 0a68 23b4 9ba7 2c0d b334 6e4e  %'I..h#...,..4nN
-00000e20: aea9 08a8 89a1 3e06 9ae6 c49c 4e40 6d11  ......>.....N@m.
-00000e30: 3211 4119 ea66 ffb7 cb30 7c03 6548 616f  2.A..f...0|.eHao
-00000e40: 49f2 56ab 3034 55e8 1280 4fd7 deb9 abcd  I.V.04U...O.....
-00000e50: e659 44c0 fed0 124c c227 a4b5 2c8d ea5a  .YD....L.'..,..Z
-00000e60: 0230 a239 f9cc dc80 5a84 434b be85 f7cd  .0.9....Z.CK....
-00000e70: 17d5 963f 5fa3 97fc a080 b326 e351 4958  ...?_......&.QIX
-00000e80: 1e75 8964 9c93 b42c 04e9 757b b148 ba51  .u.d...,..u{.H.Q
-00000e90: c64c d54c 6a99 f72d 407f f95f 140b fc99  .L.Lj..-@.._....
-00000ea0: 9e30 b186 090e 9b11 9f3c b50a 615a 4439  .0.......<..aZD9
-00000eb0: e731 4963 c024 a35e 4412 9951 1226 320f  .1Ic.$.^D..Q.&2.
-00000ec0: 3320 725c dab3 8e37 7552 d375 ba18 62fd  3 r\...7uR.u..b.
-00000ed0: 0fd5 a064 51ca f39c 9388 8610 6d28 42a2  ...dQ.......m(B.
-00000ee0: cf54 7db2 4aca 4512 cb28 37fd c15f fcbf  .T}.J.E..(7.._..
-00000ef0: 26df 185c fed4 3d7c 51cf b37f c44d 1427  &..\..=|Q....M.'
-00000f00: d8de 96f2 f29e 439d f26e 5ef4 e4d4 d1df  ......C..n^.....
-00000f10: 9ffc 7e67 077e fd16 090f fb7f 010d 0a30  ..~g.~.........0
-00000f20: 3030 3030 3036 3020 3030 3030 3030 3630  0000060 00000060
-00000f30: 2037 6666 6666 6666 6620 0d0a b0f5 4b60   7fffffff ....K`
-00000f40: 4e44 0200 b0f5 4b60 4e44 0200 0000 0000  ND....K`ND......
-00000f50: 3600 3400 3000 6300 6100 6300 3200 3300  6.4.0.c.a.c.2.3.
-00000f60: 2d00 3500 6200 3800 3600 2d00 3400 3900  -.5.b.8.6.-.4.9.
-00000f70: 3700 6500 2d00 3800 6600 3000 6300 2d00  7.e.-.8.f.0.c.-.
-00000f80: 6500 3800 3200 3800 6200 6200 6500 3300  e.8.2.8.b.b.e.3.
-00000f90: 6500 6100 6100 3300 0000 0000 0d0a 3030  e.a.a.3.......00
-00000fa0: 3030 3030 6131 2030 3030 3030 3230 3020  0000a1 00000200 
-00000fb0: 3766 6666 6666 6666 200d 0a95 8f3b 0ec2  7fffffff ....;..
-00000fc0: 300c 8677 a45e 22ac b164 2769 9d1c 8243  0..w.^"..d'i...C
-00000fd0: d8a9 cbc6 80c4 8472 3206 8ec4 1548 5b21  .......r2....H[!
-00000fe0: 5891 2ceb f7eb b3fd 7a3c efe4 87c3 ee70  X.,.....z<.....p
-00000ff0: 53e1 2746 3f25 ac52 4384 51f3 04a9 b041  S.'F?%.RC.Q....A
-00001000: 5eb0 82e5 9055 2d9a 486c de9d e422 679b  ^....U-.Hl..."g.
-00001010: dd3e ebae 37f7 cdf5 b2eb 24f2 3118 6616  .>..7.....$.1.f.
-00001020: 054a 853a 4b27 1015 8614 4726 4dd4 f7a8  .J.:K'....G&M...
-00001030: efb4 b5b7 73b6 43dc d179 62cc cb2c 0255  ....s.C..yb..,.U
-00001040: ab41 0ab9 8046 8e80 2ca3 7052 b342 9eda  .A...F..,.pR.B..
-00001050: 5fed a10d 87d5 b63f 3f1a db1b 0000 0000  _......??.......
+00000870: 0000 000d 0a30 3030 3030 3036 3420 3030  .....00000064 00
+00000880: 3030 3030 3634 2037 6666 6666 6666 6620  000064 7fffffff 
+00000890: 0d0a 6003 0aa2 7c44 0200 6003 0aa2 7c44  ..`...|D..`...|D
+000008a0: 0200 0000 0000 3600 3200 3100 3700 3600  ......6.2.1.7.6.
+000008b0: 6200 6200 3800 2d00 3600 3800 6300 6600  b.b.8.-.6.8.c.f.
+000008c0: 2d00 3400 3700 6600 3300 2d00 3800 6300  -.4.7.f.3.-.8.c.
+000008d0: 3900 3000 2d00 3500 6500 3500 3900 3200  9.0.-.5.e.5.9.2.
+000008e0: 3800 3900 6500 6400 3600 3200 6400 2e00  8.9.e.d.6.2.d...
+000008f0: 3000 0000 0000 0d0a 3030 3030 3036 3035  0.......00000605
+00000900: 2030 3030 3030 3630 3520 3766 6666 6666   00000605 7fffff
+00000910: 6666 200d 0aed 584b 8f1b 4510 b672 8b25  ff ...XK..E..r.%
+00000920: ff87 d1e4 b28b a643 bfe6 4584 38f0 0790  .......C..E.8...
+00000930: 1017 6ee3 99f1 8904 1425 a7c8 621f 6813  ..n......%..b.h.
+00000940: 9188 9522 5050 1059 1645 9c9d cd3a 31f1  ..."PP.Y.E...:1.
+00000950: 3efe 420f 7f84 9fb0 5457 f78c db8f d821  >.B.....TW.....!
+00000960: 9b04 2418 7b77 ba6b aaab beaa feaa 7a76  ..$.{w.k......zv
+00000970: cfce cebe 6e5d 68e9 2f5e 9d36 c58b 251e  ....n]h./^.6..%.
+00000980: de39 a55e dc33 97d7 69bf 0f7a 772e b65a  .9.^.3..i..zw..Z
+00000990: 67b0 ec1a 8c9f 5c30 e3d6 ffd7 7fe2 aae9  g.....\0........
+000009a0: c1a9 d70c 1c7a 0c3e bff9 d11f 1f5f 68d5  .....z.>....._h.
+000009b0: 777d f55a 5fb6 aeb7 ae4e 2f97 5e33 58b1  w}.Z_....N/.^3X.
+000009c0: fc2a 2c2f 5a37 5b5f b44a d744 d4b5 04d5  .*,/Z7[_.J.D....
+000009d0: 03c7 c49f e3d3 4efb 927a a49e a8b1 1a54  ......N..z.....T
+000009e0: 9bd5 5675 cfd3 d36a 430d 4078 0282 db6a  ..Vu...jC.@x...j
+000009f0: a45e c0cf be3a 01f9 dd6a 0bc6 bfab c7f0  .^...:...j......
+00000a00: 6c43 1d55 773b ed4e 5bed c1f8 a4da 5143  lC.Uw;.N[.....QC
+00000a10: 7558 6deb b51e 8a46 ea11 a8bf a836 ecb2  uXm....F.....6..
+00000a20: d1da 7aa7 7d11 beea 876a 133c 8e3c f5b3  ..z.}....j.<.<..
+00000a30: 1a6a dd6d ed1b 10ec aa7d 7009 c6c0 e560  .j.m.....}p....`
+00000a40: 4ded 8148 2339 5243 143f 80f1 a956 d68f  M..H#9RC.?...V..
+00000a50: d73d f52b 283e 5587 6a00 362f 4ee3 8695  .=.+(>U.j.6/N...
+00000a60: 10cc ac85 eaee b48d 552e ae68 b00f c1cb  ........U..h....
+00000a70: 313c dea9 615f b151 ecc1 8343 d01b 57df  1<..a_.Q...C..W.
+00000a80: e934 a1c3 45c9 7ba4 9ec1 1d60 8299 51b5  .4..E.{....`..Q.
+00000a90: bbe6 9b84 a903 30ba a1fd a8fb 00ec 1424  ......0........$
+00000aa0: 63ed 087e 8e61 f526 e64c efcd 31ea 8ef1  c..~.a.&.L..1...
+00000ab0: 09ac f703 4ffd a88e e1b1 5e7e 00cb c7a0  ....O.....^~....
+00000ac0: 768a 7bb0 0931 adaf 1b80 0ef0 990d 32db  v.{..1........2.
+00000ad0: 76c9 5170 28a0 46e6 e10c 2bf6 21cc 6d08  v.Qp(.F...+.!.m.
+00000ae0: 64a8 0101 dce1 bc51 40f5 1874 8e61 cb77  d......Q@..t.a.w
+00000af0: f476 2fe3 c66b 47ff 520e 6937 b80b 76eb  .v/..kG.R.i7..v.
+00000b00: 5dc2 0e71 5fd1 6375 a7b6 b4d8 fa2c abee  ]..q_.cu.....,..
+00000b10: c3ec b93a d0c8 abad e57c 7855 56c3 030d  ...:.....|xUV...
+00000b20: f0e1 0c63 752a 8ee6 593d 29a1 597a 817c  ...cu*..Y=).Yz.|
+00000b30: 7b6d 0547 ddb8 0d43 7f69 d8b9 0d39 1a21  {m.G...C.i...9.!
+00000b40: c6a1 2ee5 35f5 1358 7956 dd7b 45fe 2cda  ....5..XyV.{E.,.
+00000b50: dad7 aac1 07e0 6550 ddf6 dc34 ad63 812d  ......eP...4.c.-
+00000b60: cb94 f7e1 a25d 5fe9 ccf5 71e5 3583 5cb5  .....]_...q.5.\.
+00000b70: 2536 f7df 43c9 ec7a e061 0075 7388 bb7a  %6..C..z.a.us..z
+00000b80: e241 eb1c 4003 1deb 1a7e aea9 0233 e4a8  .A..@....~...3..
+00000b90: 95eb 7d58 1a77 e0f9 ef5d 2ebf ea61 1bb0  ..}X.w...]...a..
+00000ba0: 7572 8ced f037 ec36 63a4 8d6d d000 17d2  ur...7.6c..m....
+00000bb0: 741f 23bc a329 0e71 ccda 1c5d c64e 06e5  t.#..).q...].N..
+00000bc0: dd74 b1ba bd6f afd5 b0ac 0ed6 cb10 a01f  .t...o..........
+00000bd0: 55bb 4813 c7d3 e5e9 c4cc 31d3 c253 8337  U.H.......1..S.7
+00000be0: d09e f034 2b62 7bb0 eac1 f4b1 768b c741  ...4+b{.....v..A
+00000bf0: a77d 8b25 fab7 1e04 4c8f fceb 37fd c047  .}.%....L...7..G
+00000c00: 4a34 383d a6f6 3ddd 7fb0 70a0 704f e6db  J48=..=...p.pO..
+00000c10: 8207 c001 4bf5 0d84 f0d4 d0c0 b438 bfdf  ....K........8..
+00000c20: 69f7 8330 903c 9569 14f3 34ec 6b3f 34cd  i..0.<.i..4.k?4.
+00000c30: f322 8f63 5266 2c23 328b 0a92 7559 4e84  .".cRf,#2...uYN.
+00000c40: 1461 9915 1997 4220 be1a 5e64 f089 40e2  .a....B ..^d..@.
+00000c50: 72b4 ba60 1e07 22a0 a0ca 28ed c300 35d0  r..`.."...(...5.
+00000c60: 10e1 fc65 6be6 e766 453c 2be0 6c22 a166  ...ek..fE<+.l".f
+00000c70: 09dc f547 2682 f19c a684 8771 8fc8 2e4f  ...G&......q...O
+00000c80: 4997 2794 f044 1645 9296 bd9c 957d 138f  I.'..D.E.....}..
+00000c90: 5d03 00f5 bd1f f0c8 dac0 f828 a44a 180d  ]..........(.J..
+00000ca0: 9825 4628 1b6f be1f 10a6 bf60 0726 fd73  .%F(.o.....`.&.s
+00000cb0: 3db5 100c 2216 4c48 209d b125 8469 0ae6  =...".LH ..%.i..
+00000cc0: 7cde 5103 e6d7 9948 8cfd b708 911b 8828  |.Q....H.......(
+00000cd0: 658b a0ac 6686 f906 c62e 8a79 9004 cc0a  e...f......y....
+00000ce0: 6c0e ac54 a782 cf48 4598 a2ae 4069 d2c8  l..T...HE...@i..
+00000cf0: a186 b4ba 9c88 a943 74d8 ca48 d624 74c0  .......Ct..H.$t.
+00000d00: 69e5 306e cc37 8839 ce7a 795c 725a 901e  i.0n.7.9.zy\rZ..
+00000d10: 978c c888 e6a4 5bf4 2409 b322 49ca 50c6  ......[.$.."I.P.
+00000d20: 320b 8d31 f106 4a63 5521 fc93 85c1 5c4a  2..1..JcU!....\J
+00000d30: 5a1a ce75 7b0f 8e0d 3c43 9ebb 87d8 07be  Z..u{...<C......
+00000d40: 4d74 bdbd 5859 96e9 b533 f66e e86b fdca  Mt..XY...3.n.k..
+00000d50: 9a52 0eb1 e8a4 88f4 8709 a619 65fb 0012  .R..........e...
+00000d60: 026c 450d dbec c4ae b11a da2e 4b97 69bc  .lE.........K.i.
+00000d70: 8a0d 1e30 2ece 67e4 651a 361c 19b0 a6cd  ...0..g.e.6.....
+00000d80: e899 e83b e960 4d4a 9884 5dd6 47fe 211c  ...;.`MJ..].G.!.
+00000d90: 38fa d56b eef5 0146 f8da 30fd dae2 bb75  8..k...F..0....u
+00000da0: b720 c322 6165 1171 4952 ce62 22cb 4890  . ."ae.qIR.b".H.
+00000db0: 242c ba24 97b9 c8bb 495c 6459 09f5 0a9a  $,.$....I\dY....
+00000dc0: 29d2 ed93 ecc6 8df2 fa35 1f27 9f36 ddee  )........5.'.6..
+00000dd0: 5f59 7188 85b0 a4ef 043e 554e 3811 4eaa  _Yq......>UN8.N.
+00000de0: a712 5f4b 2c8f fdcf 0cad f10e 8c76 979c  .._K,........v..
+00000df0: a716 660b d105 e900 8ae2 38e6 2c0c 9af8  ..f.......8.,...
+00000e00: 30ba 348b 2329 0a4e 585a a644 8625 2749  0.4.#).NXZ.D.%'I
+00000e10: 920a 6823 b49b a72c 0db3 346e 4eae a908  ..h#...,..4nN...
+00000e20: a889 a13e 069a e6c4 9c4e 406d 1132 1141  ...>.....N@m.2.A
+00000e30: 19ea 66ff b7cb 307c 0365 4861 6f49 f256  ..f...0|.eHaoI.V
+00000e40: ab30 3455 e812 804f d7de b9ab cde6 5944  .04U...O......YD
+00000e50: c0fe d012 4cc2 27a4 b52c 8dea 5a02 30a2  ....L.'..,..Z.0.
+00000e60: 39f9 ccdc 805a 8443 4bbe 85f7 cd17 d596  9....Z.CK.......
+00000e70: 3f5f a397 fca0 80b3 26e3 5149 581e 7589  ?_......&.QIX.u.
+00000e80: 649c 93b4 2c04 e975 7bb1 48ba 51c6 4cd5  d...,..u{.H.Q.L.
+00000e90: 4c6a 99f7 2d40 7ff9 5f14 0bfc 999e 30b1  Lj..-@.._.....0.
+00000ea0: 8609 0e9b 119f 3cb5 0a61 5a44 39e7 3149  ......<..aZD9.1I
+00000eb0: 63c0 24a3 5e44 1299 5112 2632 0f33 2072  c.$.^D..Q.&2.3 r
+00000ec0: 5cda b38e 3775 52d3 75ba 1862 fd0f d5a0  \...7uR.u..b....
+00000ed0: 6451 caf3 9c93 8886 106d 2842 a2cf 547d  dQ.......m(B..T}
+00000ee0: b24a ca45 12cb 2837 fdc1 5ffc bf26 df18  .J.E..(7.._..&..
+00000ef0: 5cfe d43d 7c51 cfb3 7fc4 4d14 27d8 de96  \..=|Q....M.'...
+00000f00: f2f2 9e43 9df2 6e5e f4e4 d4d1 df9f fc7e  ...C..n^.......~
+00000f10: 6707 7efd 1609 0ffb 7f01 0d0a 3030 3030  g.~.........0000
+00000f20: 3030 3630 2030 3030 3030 3036 3020 3766  0060 00000060 7f
+00000f30: 6666 6666 6666 200d 0a60 030a a27c 4402  ffffff ..`...|D.
+00000f40: 0060 030a a27c 4402 0000 0000 0036 0034  .`...|D......6.4
+00000f50: 0030 0063 0061 0063 0032 0033 002d 0035  .0.c.a.c.2.3.-.5
+00000f60: 0062 0038 0036 002d 0034 0039 0037 0065  .b.8.6.-.4.9.7.e
+00000f70: 002d 0038 0066 0030 0063 002d 0065 0038  .-.8.f.0.c.-.e.8
+00000f80: 0032 0038 0062 0062 0065 0033 0065 0061  .2.8.b.b.e.3.e.a
+00000f90: 0061 0033 0000 0000 000d 0a30 3030 3030  .a.3.......00000
+00000fa0: 3061 3120 3030 3030 3032 3030 2037 6666  0a1 00000200 7ff
+00000fb0: 6666 6666 6620 0d0a 958f 3b0e c230 0c86  fffff ....;..0..
+00000fc0: 77a4 5e22 acb1 6427 699d 1c82 43d8 a9cb  w.^"..d'i...C...
+00000fd0: c680 c484 7232 068e c415 485b 2158 912c  ....r2....H[!X.,
+00000fe0: ebf7 ebb3 fd7a 3cef e487 c3ee 7053 e127  .....z<.....pS.'
+00000ff0: 463f 25ac 5243 8451 f304 a9b0 415e b082  F?%.RC.Q....A^..
+00001000: e590 552d 9a48 6cde 9de4 2267 9bdd 3eeb  ..U-.Hl..."g..>.
+00001010: ae37 f7cd f5b2 eb24 f231 1866 1605 4a85  .7.....$.1.f..J.
+00001020: 3a4b 2710 1586 1447 264d d4f7 a8ef b4b5  :K'....G&M......
+00001030: b773 b643 dcd1 7962 cccb 2c02 55ab 410a  .s.C..yb..,.U.A.
+00001040: b980 468e 802c a370 52b3 429e da5f eda1  ..F..,.pR.B.._..
+00001050: 0d87 d5b6 3f3f 1adb 1b00 0000 0000 0000  ....??..........
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000010c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -277,206 +277,206 @@
 00001140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000011a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000011b0: 0000 0000 0000 0000 0000 000d 0a30 3030  .............000
-000011c0: 3030 3036 3420 3030 3030 3030 3634 2037  00064 00000064 7
-000011d0: 6666 6666 6666 6620 0d0a b0f5 4b60 4e44  fffffff ....K`ND
-000011e0: 0200 b0f5 4b60 4e44 0200 0000 0000 3600  ....K`ND......6.
-000011f0: 3400 3000 6300 6100 6300 3200 3300 2d00  4.0.c.a.c.2.3.-.
-00001200: 3500 6200 3800 3600 2d00 3400 3900 3700  5.b.8.6.-.4.9.7.
-00001210: 6500 2d00 3800 6600 3000 6300 2d00 6500  e.-.8.f.0.c.-.e.
-00001220: 3800 3200 3800 6200 6200 6500 3300 6500  8.2.8.b.b.e.3.e.
-00001230: 6100 6100 3300 2e00 3000 0000 0000 0d0a  a.a.3...0.......
-00001240: 3030 3030 3037 3532 2030 3030 3030 3735  00000752 0000075
-00001250: 3220 3766 6666 6666 6666 200d 0abd 586d  2 7fffffff ...Xm
-00001260: 6f13 4710 fe4c 24ff 07eb a256 49e5 4bef  o.G..L$....VI.K.
-00001270: f6ee 6c5f 233e 9002 4e90 1390 f3e2 38df  ..l_#>..N.....8.
-00001280: 7c77 765e 7042 0489 898d 2211 2201 2a88  |wv^pB....".".*.
-00001290: b4a8 1588 b640 2a54 f5a3 a131 3198 84bf  .....@*T...11...
-000012a0: b0f7 4bfa 173a 3bbb 679f 9d8b ed84 b471  ..K..:;.g......q
-000012b0: eed6 b73b 3b3b f3cc 33b3 b7fe a7fe f98e  ...;;;..3.......
-000012c0: 1609 f5dd d1cd 8822 3e2a 6fc5 9f1c 70f3  .......">*o...p.
-000012d0: fe40 14a6 82fc a698 a8e2 6476 61bf 66db  .@........dva.f.
-000012e0: 76d4 5072 723e aaa9 b26e 6773 723c a769  v.Prr>...ngsr<.i
-000012f0: b296 cb66 eda8 aa58 46de 8c48 f495 7b97  ...f...XF..H..{.
-00001300: d6e8 4bf7 1efd e8de 751f 415b a335 09d5  ..K.....u.A[.5..
-00001310: f4a4 0156 dc64 0b82 1968 1021 ec2e c37c  ...V.d...h.!...|
-00001320: a210 2daa c5e4 583c 1a97 f5ac 9197 e346  ..-...X<.......F
-00001330: 2c2a c735 231b 8be6 14db b4b2 9bc2 6b66  ,*.5#.........kf
-00001340: c81b 7a08 a67c a215 fa82 1e62 7b40 f7e0  ..z..|.....b{@..
-00001350: aab8 3bf4 153e 5569 dd7d 2c35 bc6e 7a2f  ..;..>Ui.},5.nz/
-00001360: 408b 9008 2eae 4574 6e51 a80f a562 118d  @.....EtnQ...b..
-00001370: 03a4 f059 282c cc15 df9b 3a34 26cc 0663  ...Y(,....:4&..c
-00001380: b17c deb6 8929 c7f2 c491 7542 34d9 2224  .|...)....uB4."$
-00001390: 2fab 6634 1acd c588 a158 595c 4d17 969c  /.f4.....XY\M...
-000013a0: c05f 02fe bea4 6fc1 df0a 7d0b 7e03 f8f0  ._....o...}.~...
-000013b0: ed67 f06f 873e 836f 9fdd 6d77 8bf5 49cd  .g.o.>.o..mw..I.
-000013c0: 78fa 3cc6 9661 ed79 8806 aba0 56e1 08b4  x.<..a.y....V...
-000013d0: 4873 5e68 78a9 d832 caf1 0686 2529 02d1  Hs^hx..2....%)..
-000013e0: 92b9 9424 6d76 1fed 866f fb78 b7e7 4ef1  ...$mv...o.x..N.
-000013f0: d144 4405 cb59 8455 bcb7 7e40 469a e6d6  .DD..Y.U..~@F...
-00001400: 610b 6677 7393 abd3 7acb 35d0 6128 8a1e  a.fws...z.5.a(..
-00001410: 6918 b819 0034 f182 255d cbae ade5 6eae  i....4..%]....n.
-00001420: 480d 9279 725f 048d 2aa0 e060 3457 55f0  H..yr_..*..`4WU.
-00001430: 52fd f5c3 ffd9 f499 e04b 5172 22c6 c67b  R........KQr"..{
-00001440: 652c 66ef 018c 57a1 a06c 417b 00cf 55fa  e,f...W..lA{..U.
-00001450: 1b5c 07ee 9333 ce5e 9515 9f80 dc6d 8d41  .\...3.^.....m.A
-00001460: eb13 1041 9204 2938 624c 9187 ed09 2051  ...A..)8bL.... Q
-00001470: 7a86 e435 14b1 2df7 21ad 812c c0d0 286a  z..5..-.!..,..(j
-00001480: 8774 4f48 ecf3 643f 9aba a704 c610 7828  .tOH..d?......x(
-00001490: 27a5 9fd2 4086 adad c735 95d8 8a29 1323  '...@....5...).#
-000014a0: 9697 750b aaa1 45e2 8a4c e2ba e3c4 cd5c  ..u...E..L.....\
-000014b0: de56 7338 57c1 acf4 ea12 0fac 07af 7717  .Vs8W.........w.
-000014c0: d111 0d0f 031b c1a6 f9c1 713e 4951 44f1  ..........q>IQD.
-000014d0: 5244 36c3 7683 cb49 a1be 7e86 3dad 23b2  RD6.v..I..~.=.#.
-000014e0: f7dc c7e1 d650 b80f 601b fb08 d72e 80fc  .....P..`.......
-000014f0: 566c 6b1f bc3d c67d 14ea 0bf5 7d4d 7f47  Vlk..=.}....}M.G
-00001500: bad6 61a8 ca29 1bea c3fd f0d0 bd0f 3d7b  ..a..)........={
-00001510: 103f 5018 0ede 2207 7807 8bdd 60a8 ef1c  .?P...".x...`...
-00001520: fcd3 5f20 98a0 2c0c 7aab 6cd6 36f2 9f85  .._ ..,.z.l.6...
-00001530: 7a17 2c02 b54c 7c80 6d66 68e8 275a c5ee  z.,..L|.mfh.'Z..
-00001540: 16ae 0c86 e91f 20f8 376c 7d15 d079 ae8d  ...... .7l}..y..
-00001550: 6115 e66b bb06 f751 ab8e 6e4b 0c33 6331  a..k...Q..nK.3c1
-00001560: 4d61 f8be 67f6 b0f0 0269 0972 75f7 0943  Ma..g....i.ru..C
-00001570: 1117 0cc2 f625 7d0f ed1e eecc 3577 6740  .....%}.....5wg@
-00001580: e2ef 1287 f41d 68bd 8bc8 3c05 cb3e 434f  ......h...<..>CO
-00001590: 1d37 6fc6 fb43 84a4 86b1 3b40 d93a 8e80  .7o..C....;@.:..
-000015a0: 02a0 4198 3ee7 7180 f9ef 607e 1de4 3e63  ..A.>.q...`~..>c
-000015b0: 3cb6 c0ab c141 6ea2 cff4 b660 f1b8 f6fb  <....An....`....
-000015c0: 047c 1ca1 353e d846 9b5d 7074 1b5c a932  .|..5>.F.]pt.\.2
-000015d0: 8bc0 deea 51a5 60d5 1b90 3980 f0df 67a1  ....Q.`...9...g.
-000015e0: 3f31 794e 8dc9 c071 d462 cb60 7004 23fc  ?1yN...q.b.`p.#.
-000015f0: 34af 62b8 7145 a839 4253 b0f6 76b2 3d85  4.b.qE.9BS..v.=.
-00001600: a77d fa8e 59ee deeb 4c93 5ec9 0e03 ccc0  .}..Y...L.^.....
-00001610: 1701 a5f2 d351 b237 73ac 9d75 d0bf 3dd0  .....Q.7s..u..=.
-00001620: 85ba 7ebf 3971 5f37 48bb 0d18 d5d0 c62a  ..~.9q_7H......*
-00001630: 2b00 03f4 57d0 f2de 7ddc 23a9 78bc 7705  +...W...}.#.x.w.
-00001640: 35d9 9dc5 db47 0b77 e70c e3c2 9c69 8945  5....G.w.....i.E
-00001650: 183c 810d 15a4 6ad0 c9f4 374a 1908 3ec3  .<....j...7J..>.
-00001660: 1de5 019f 4fab 2c15 1976 3fe0 1e7c 4f92  ....O.,..v?..|O.
-00001670: 0687 cece b4e1 16ac 8ec9 8b2e 3875 ccf2  ............8u..
-00001680: b3f7 bde3 723d f9d3 439e 9faa 4e0b e3c3  ....r=..C...N...
-00001690: 5d0a 3696 e54e 8914 3e1f 44be 2fdf 26fe  ].6..N..>.D./.&.
-000016a0: a3ac e81d 175f 2df9 5f92 a2ab 657e 83ce  ....._-._...e~..
-000016b0: 8c3a ddaa 9e28 6ff8 6a19 068d 15d8 aff6  .:...(o.j.......
-000016c0: b070 1e86 c1e7 0abc d9d4 5956 ed87 71c9  .p........YV..q.
-000016d0: 0f98 d3a2 9f95 ba8e dc89 8425 e99b a1dc  ...........%....
-000016e0: 6a9e 6fc0 6233 3ac0 5791 3f71 a7af b3da  j.o.b3:.W.?q....
-000016f0: 8cf5 f947 301a 62ec 6e01 e124 f81b 6e8c  ...G0.b.n..$..n.
-00001700: bcc2 337b 95cf c6c5 c4fa 03cd 4991 86b1  ..3{........I...
-00001710: 4328 5f17 6783 e710 b19d 4818 86fd 35f9  C(_.g.....H...5.
-00001720: 1cef 476a 07bc 923c 45d8 1fb2 4385 fb24  ..Gj...<E...C..$
-00001730: 00b4 e6b2 834d 2b5b 91f6 d8b2 ed85 f52f  .....M+[......./
-00001740: d450 6721 6574 692e b1c3 ab61 2b74 435f  .Pg!eti....a+tC_
-00001750: a943 cd5f 2d7c 5fc5 9b0c 183f d858 db47  .C._-|_....?.X.G
-00001760: 1401 2aad 9c7a e7a1 3fc1 b57f e4a4 5509  ..*..z..?.....U.
-00001770: c8bd d320 d7c8 be26 8401 b9d7 5083 f46e  ... ...&....P..n
-00001780: 47a7 3614 b476 5b54 3a65 4f87 b738 899f  G.6..v[T:eO..8..
-00001790: ecf1 bc61 e279 63b3 7118 f3d2 db7f 946a  ...a.yc.q......j
-000017a0: 1cfe f0a1 5f8a 3870 acc9 9268 4e56 eda8  ...._.8p...hNV..
-000017b0: 25eb 2a21 b299 7334 396f e563 5adc 8a66  %.*!..s49o.cZ..f
-000017c0: 55a2 367e 5a69 dca4 1109 8f9b bd8c f87e  U.6~Zi.........~
-000017d0: 27f0 9d5f fcfd 42d4 e4bf e3a0 fd1d d354  '.._..B........T
-000017e0: 78c4 cfb6 37d7 a5a6 7c98 7e0c e35e de3e  x...7...|.~..^.>
-000017f0: c35b a3d5 ff49 e9cc 5c53 8e77 4d74 f75b  .[...I..\S.wMt.[
-00001800: d95b b9a8 fe5d 2cb6 feed b58b a66e a56f  .[...],......n.o
-00001810: cf3b cb33 259b 148a d692 b238 3ea9 df1e  .;.3%......8>...
-00001820: 5b1c 2958 cb13 c5b9 4461 7dae ac2c cecc  [.)X....Da}..,..
-00001830: a412 c9a9 f9c5 6b65 7de2 fba5 8da9 b9d9  ......ke}.......
-00001840: 9412 0af5 65d3 c68a 5d1a 0115 1beb 3688  ....e...].....6.
-00001850: 6547 538a 7df1 4631 a965 f4e4 d2e5 a5e4  eGS.}.F1.e......
-00001860: ca15 3559 9e5f 1f9f 34af 6766 530b c9f4  ..5Y._..4.gfS...
-00001870: 44d1 9a1d 29c2 524a 366d ae83 8ae4 ec84  D...).RJ6m......
-00001880: 616b a982 3569 9699 56ae 726c 3e97 506f  ak..5i..V.rl>.Po
-00001890: 592b e3d1 b9c4 4439 43cc d2b5 c92b 379c  Y+....D9C....+7.
-000018a0: d1d4 edab 8bf1 a2b3 042a d3e3 ebf6 ca74  .........*.....t
-000018b0: 1154 5cfd 5edf 4892 d482 93b8 b406 a26b  .T\.^.H........k
-000018c0: 76c2 2c67 6753 ab16 d1d7 6cad 5076 1233  v.,ggS....l.Pv.3
-000018d0: 6b49 3251 b497 a717 c746 17d6 ac84 51be  kI2Q.....F....Q.
-000018e0: ba32 a1e4 d21b 05a6 1654 0469 f6a9 2d3a  .2.......T.i..-:
-000018f0: e9eb 45b0 d2b0 122d 2a0c cf69 50d1 d16f  ..E....-*..iP..o
-00001900: 6d66 3549 e68a d64a aa9c d43c 879b 4ec2  mf5I...J...<..N.
-00001910: b226 a818 5b5e 509c d10b d164 c924 6cf5  .&..[^P....d.$l.
-00001920: 4cc9 2839 9371 5079 0922 7159 c94c 9a4b  L.(9.qPy."qY.L.K
-00001930: 9676 a500 d111 90af 92ab a333 ab1e 360c  .v.........3..6.
-00001940: 8bce 4ef8 8c77 0a99 a5a3 1163 1109 341e  ..N..w.....c..4.
-00001950: 0297 304b 76c9 d4e6 d263 7e35 ab56 9b1a  ..0Kv....c~5.V..
-00001960: a6e2 580c 9a6a 20d0 d72d cd29 fb9c d18f  ..X..j ..-.)....
-00001970: c0e9 684e c9d0 c64b 0604 cf2e 8e2f 5db8  ..hN...K...../].
-00001980: 0dea 3253 d31b 5319 b250 b0d2 977c 962c  ..2S..S..P...|.,
-00001990: 94b3 534d 4b98 15dd a7af 8115 c08f cbeb  ..SMK...........
-000019a0: 1932 bd98 2ceb e703 732a 20c7 36ff 050d  .2..,...s* .6...
-000019b0: 0a30 3030 3030 3036 3020 3030 3030 3030  .00000060 000000
-000019c0: 3630 2037 6666 6666 6666 6620 0d0a b0f5  60 7fffffff ....
-000019d0: 4b60 4e44 0200 b0f5 4b60 4e44 0200 0000  K`ND....K`ND....
-000019e0: 0000 6200 3900 3000 6400 3800 3500 3800  ..b.9.0.d.8.5.8.
-000019f0: 3600 2d00 6100 3100 3200 6500 2d00 3400  6.-.a.1.2.e.-.4.
-00001a00: 3500 6600 3600 2d00 6100 3100 3800 3200  5.f.6.-.a.1.8.2.
-00001a10: 2d00 3400 6500 3500 6100 3000 3800 3700  -.4.e.5.a.0.8.7.
-00001a20: 6200 3100 6400 3200 3800 0000 0000 0d0a  b.1.d.2.8.......
-00001a30: 3030 3030 3031 6164 2030 3030 3030 3230  000001ad 0000020
-00001a40: 3020 3766 6666 6666 6666 200d 0a8d 5249  0 7fffffff ...RI
-00001a50: 6a5c 3110 dd1b 7c87 e6af 5550 9a4a a565  j\1...|...UP.J.e
-00001a60: c819 7200 0da5 5520 c171 56a6 c119 c826  ..r...U .qV....&
-00001a70: 812c b3ce 0d9c 8440 6363 fb0a fa27 c915  .,.....@cc...'..
-00001a80: 52bf 1bbc 3608 f124 1ef5 06e9 dfdd e395  R...6..$........
-00001a90: 35e7 6757 3563 e7c8 04c5 3a81 10c7 86d8  5.gW5c....:.....
-00001aa0: 4190 5890 53b5 ddf1 de1c a9cd b3b7 d218  A.X.S...........
-00001ab0: 3af7 0861 640f 5c9c 8391 eb28 82c9 bb34  :..ad.\....(...4
-00001ac0: 36de 911c 4c57 7671 2460 1b55 0856 9959  6...LWvq$`.U.V.Y
-00001ad0: ba87 5147 f25c 4905 ad61 c111 5288 5052  ..QG.\I..a..R.PR
-00001ae0: 1b10 7cf5 906b 65a8 96c9 47c2 e884 b671  ..|..ke...G....q
-00001af0: f834 180d 9a68 0b06 ec01 6a61 75c2 9481  .4...h....jau...
-00001b00: 93b3 8021 8d18 aa60 ef69 6f96 97af dfbc  ...!...`.io.....
-00001b10: 9317 e352 2e5e bded e552 96d3 90e5 e2fd  ...R.^...R......
-00001b20: 6296 f963 decc dbf5 7afd ba7e 5cbf edec  b..c....z..~\...
-00001b30: fcb9 9b8f f361 fd30 efe6 dfdd 7c98 bfe6  .....a.0....|...
-00001b40: bdee bfb7 a3a2 c3fa 7d37 6ff5 e27e fd3c  ........}7o..~.<
-00001b50: 0ff3 cffa 69bd 9e37 eb17 c587 45b5 16b5  ....i..7....E...
-00001b60: 85fb f3b3 bd21 6713 6d19 88b7 4869 684d  .....!g.m...HihM
-00001b70: 2d23 4489 d9b1 5640 ae6f 7c0a d84a 731e  -#D...V@.o|..Js.
-00001b80: 62d5 fa43 4e02 3cb0 81b0 e35a c54b 297e  b..CN.<....Z.K)~
-00001b90: 6fc2 e6d9 d526 03bb 06cc 6cc1 da4e 50b3  o....&....l..NP.
-00001ba0: 2a20 46ac 5a7d c9b1 abfa 46f5 bd48 414b  * F.Z}....F..HAK
-00001bb0: 40b9 267d 452d 2987 e8c1 ba94 adf5 c90d  @.&}E-).........
-00001bc0: 2df4 44ed b1a2 44e9 e022 7508 681b e4e6  -.D...D.."u.h...
-00001bd0: 0906 7975 363a 1772 c63d cbe7 b342 1f45  ..yu6:.r.=...B.E
-00001be0: 453f 43d5 5ba8 a930 849e 1449 cb40 912d  E?C.[..0...I.@.-
-00001bf0: a642 39b7 712a f2b4 fe03 0000 0000 0000  .B9.q*..........
+000011b0: 0000 0000 0000 0000 0d0a 3030 3030 3030  ..........000000
+000011c0: 3634 2030 3030 3030 3036 3420 3766 6666  64 00000064 7fff
+000011d0: 6666 6666 200d 0a60 030a a27c 4402 0060  ffff ..`...|D..`
+000011e0: 030a a27c 4402 0000 0000 0036 0034 0030  ...|D......6.4.0
+000011f0: 0063 0061 0063 0032 0033 002d 0035 0062  .c.a.c.2.3.-.5.b
+00001200: 0038 0036 002d 0034 0039 0037 0065 002d  .8.6.-.4.9.7.e.-
+00001210: 0038 0066 0030 0063 002d 0065 0038 0032  .8.f.0.c.-.e.8.2
+00001220: 0038 0062 0062 0065 0033 0065 0061 0061  .8.b.b.e.3.e.a.a
+00001230: 0033 002e 0030 0000 0000 000d 0a30 3030  .3...0.......000
+00001240: 3030 3735 3220 3030 3030 3037 3532 2037  00752 00000752 7
+00001250: 6666 6666 6666 6620 0d0a bd58 6d6f 1347  fffffff ...Xmo.G
+00001260: 10fe 4c24 ff07 eba2 5649 e54b eff6 ee6c  ..L$....VI.K...l
+00001270: 5f23 3e90 024e 9013 90f3 e238 df7c 7776  _#>..N.....8.|wv
+00001280: 5e70 4204 8989 8d22 1122 012a 88b4 a815  ^pB....".".*....
+00001290: 88b6 402a 54f5 a3a1 3131 9884 bfb0 f74b  ..@*T...11.....K
+000012a0: fa17 3a3b bb67 9f9d 8bed 84b4 71ee d6b7  ..:;.g......q...
+000012b0: 3b3b 3bf3 cc33 b3b7 fea7 fef9 8e16 09f5  ;;;..3..........
+000012c0: ddd1 cd88 223e 2a6f c59f 1c70 f3fe 4014  ....">*o...p..@.
+000012d0: a682 fca6 98a8 e264 7661 bf66 db76 d450  .......dva.f.v.P
+000012e0: 7272 3eaa a9b2 6e67 7372 3ca7 69b2 96cb  rr>...ngsr<.i...
+000012f0: 66ed a8aa 5846 de8c 48f4 957b 97d6 e84b  f...XF..H..{...K
+00001300: f71e fde8 de75 1f41 5ba3 3509 d5f4 a401  .....u.A[.5.....
+00001310: 56dc 640b 8219 6810 21ec 2ec3 7ca2 102d  V.d...h.!...|..-
+00001320: aac5 e458 3c1a 97f5 ac91 97e3 462c 2ac7  ...X<.......F,*.
+00001330: 3523 1b8b e614 dbb4 b29b c26b 66c8 1b7a  5#.........kf..z
+00001340: 08a6 7ca2 15fa 821e 627b 40f7 e0aa b83b  ..|.....b{@....;
+00001350: f415 3e55 69dd 7d2c 35bc 6e7a 2f40 8b90  ..>Ui.},5.nz/@..
+00001360: 082e ae45 746e 51a8 0fa5 6211 8d03 a4f0  ...EtnQ...b.....
+00001370: 5928 2ccc 15df 9b3a 3426 cc06 63b1 7cde  Y(,....:4&..c.|.
+00001380: b689 29c7 f2c4 9175 4234 d922 242f ab66  ..)....uB4."$/.f
+00001390: 341a cdc5 88a1 5859 5c4d 1796 9cc0 5f02  4.....XY\M...._.
+000013a0: febe a46f c1df 0a7d 0b7e 03f8 f0ed 67f0  ...o...}.~....g.
+000013b0: 6f87 3e83 6f9f dd6d 778b f549 cd78 fa3c  o.>.o..mw..I.x.<
+000013c0: c696 61ed 7988 06ab a056 e108 b448 735e  ..a.y....V...Hs^
+000013d0: 6878 a9d8 32ca f106 8625 2902 d192 b994  hx..2....%).....
+000013e0: 246d 761f ed86 6ffb 78b7 e74e f1d1 4444  $mv...o.x..N..DD
+000013f0: 05cb 5984 55bc b77e 4046 9ae6 d661 0b66  ..Y.U..~@F...a.f
+00001400: 7773 93ab d37a cb35 d061 288a 1e69 18b8  ws...z.5.a(..i..
+00001410: 1900 34f1 8225 5dcb aead e56e ae48 0d92  ..4..%]....n.H..
+00001420: 7972 5f04 8d2a a0e0 6034 5755 f052 fdf5  yr_..*..`4WU.R..
+00001430: c3ff d9f4 99e0 4b51 7222 c6c6 7b65 2c66  ......KQr"..{e,f
+00001440: ef01 8c57 a1a0 6c41 7b00 cf55 fa1b 5c07  ...W..lA{..U..\.
+00001450: ee93 33ce 5e95 159f 80dc 6d8d 41eb 1310  ..3.^.....m.A...
+00001460: 4192 0429 3862 4c91 87ed 0920 517a 86e4  A..)8bL.... Qz..
+00001470: 3514 b12d f721 ad81 2cc0 d028 6a87 744f  5..-.!..,..(j.tO
+00001480: 48ec f364 3f9a baa7 04c6 1078 2827 a59f  H..d?......x('..
+00001490: d240 86ad adc7 3595 d88a 2913 2396 9775  .@....5...).#..u
+000014a0: 0baa a145 e28a 4ce2 bae3 c4cd 5cde 5673  ...E..L.....\.Vs
+000014b0: 3857 c1ac f4ea 120f ac07 af77 17d1 110d  8W.........w....
+000014c0: 0f03 1bc1 a6f9 c171 3e49 5144 f152 4436  .......q>IQD.RD6
+000014d0: c376 83cb 49a1 be7e 863d ad23 b2f7 dcc7  .v..I..~.=.#....
+000014e0: e1d6 50b8 0f60 1bfb 08d7 2e80 fc56 6c6b  ..P..`.......Vlk
+000014f0: 1fbc 3dc6 7d14 ea0b f57d 4d7f 47ba d661  ..=.}....}M.G..a
+00001500: a8ca 291b eac3 fdf0 d0bd 0f3d 7b10 3f50  ..)........={.?P
+00001510: 180e de22 0778 078b dd60 a8ef 1cfc d35f  ...".x...`....._
+00001520: 2098 a02c 0c7a ab6c d636 f29f 857a 172c   ..,.z.l.6...z.,
+00001530: 02b5 4c7c 806d 6668 e827 5ac5 ee16 ae0c  ..L|.mfh.'Z.....
+00001540: 86e9 1f20 f837 6c7d 15d0 79ae 8d61 15e6  ... .7l}..y..a..
+00001550: 6bbb 06f7 51ab 8e6e 4b0c 3363 314d 61f8  k...Q..nK.3c1Ma.
+00001560: be67 f6b0 f002 6909 7275 f709 4311 170c  .g....i.ru..C...
+00001570: c2f6 257d 0fed 1eee cc35 7767 40e2 ef12  ..%}.....5wg@...
+00001580: 87f4 1d68 bd8b c83c 05cb 3e43 4f1d 376f  ...h...<..>CO.7o
+00001590: c6fb 4384 a486 b13b 40d9 3a8e 8002 a041  ..C....;@.:....A
+000015a0: 983e e771 80f9 ef60 7e1d e43e 633c b6c0  .>.q...`~..>c<..
+000015b0: abc1 416e a2cf f4b6 60f1 b8f6 fb04 7c1c  ..An....`.....|.
+000015c0: a135 3ed8 469b 5d70 741b 5ca9 328b c0de  .5>.F.]pt.\.2...
+000015d0: ea51 a560 d51b 9039 80f0 df67 a13f 3179  .Q.`...9...g.?1y
+000015e0: 4e8d c9c0 71d4 62cb 6070 0423 fc34 af62  N...q.b.`p.#.4.b
+000015f0: b871 45a8 3942 53b0 f676 b23d 85a7 7dfa  .qE.9BS..v.=..}.
+00001600: 8e59 eede eb4c 935e c90e 03cc c017 01a5  .Y...L.^........
+00001610: f2d3 51b2 3773 ac9d 75d0 bf3d d085 ba7e  ..Q.7s..u..=...~
+00001620: bf39 715f 3748 bb0d 18d5 d0c6 2a2b 0003  .9q_7H......*+..
+00001630: f457 d0f2 de7d dc23 a978 bc77 0535 d99d  .W...}.#.x.w.5..
+00001640: c5db 470b 77e7 0ce3 c29c 6989 4518 3c81  ..G.w.....i.E.<.
+00001650: 0d15 a46a d0c9 f437 4a19 083e c31d e501  ...j...7J..>....
+00001660: 9f4f ab2c 1519 763f e01e 7c4f 9206 87ce  .O.,..v?..|O....
+00001670: ceb4 e116 ac8e c98b 2e38 75cc f2b3 f7bd  .........8u.....
+00001680: e372 3df9 d343 9e9f aa4e 0be3 c35d 0a36  .r=..C...N...].6
+00001690: 96e5 4e89 143e 1f44 be2f df26 fea3 ace8  ..N..>.D./.&....
+000016a0: 1d17 5f2d f95f 92a2 ab65 7e83 ce8c 3add  .._-._...e~...:.
+000016b0: aa9e 286f f86a 1906 8d15 d8af f6b0 701e  ..(o.j........p.
+000016c0: 86c1 e70a bcd9 d459 56ed 8771 c90f 98d3  .......YV..q....
+000016d0: a29f 95ba 8edc 8984 25e9 9ba1 dc6a 9e6f  ........%....j.o
+000016e0: c062 333a c057 913f 71a7 afb3 da8c f5f9  .b3:.W.?q.......
+000016f0: 4730 1a62 ec6e 01e1 24f8 1b6e 8cbc c233  G0.b.n..$..n...3
+00001700: 7b95 cfc6 c5c4 fa03 cd49 9186 b143 285f  {........I...C(_
+00001710: 1767 83e7 10b1 9d48 1886 fd35 f91c ef47  .g.....H...5...G
+00001720: 6a07 bc92 3c45 d81f b243 85fb 2400 b4e6  j...<E...C..$...
+00001730: b283 4d2b 5b91 f6d8 b2ed 85f5 2fd4 5067  ..M+[......./.Pg
+00001740: 2165 7469 2eb1 c3ab 612b 7443 5fa9 43cd  !eti....a+tC_.C.
+00001750: 5f2d 7c5f c59b 0c18 3fd8 58db 4714 012a  _-|_....?.X.G..*
+00001760: ad9c 7ae7 a13f c1b5 7fe4 a455 09c8 bdd3  ..z..?.....U....
+00001770: 20d7 c8be 2684 01b9 d750 83f4 6e47 a736   ...&....P..nG.6
+00001780: 14b4 765b 543a 654f 87b7 3889 9fec f1bc  ..v[T:eO..8.....
+00001790: 61e2 7963 b371 18f3 d2db 7f94 6a1c fef0  a.yc.q......j...
+000017a0: a15f 8a38 70ac c992 684e 56ed a825 eb2a  ._.8p...hNV..%.*
+000017b0: 21b2 9973 3439 6fe5 635a dc8a 6655 a236  !..s49o.cZ..fU.6
+000017c0: 7e5a 69dc a411 098f 9bbd 8cf8 7e27 f09d  ~Zi.........~'..
+000017d0: 5ffc fd42 d4e4 bfe3 a0fd 1dd3 5478 c4cf  _..B........Tx..
+000017e0: b637 d7a5 a67c 987e 0ce3 5ede 3ec3 5ba3  .7...|.~..^.>.[.
+000017f0: d5ff 49e9 cc5c 538e 774d 74f7 5bd9 5bb9  ..I..\S.wMt.[.[.
+00001800: a8fe 5d2c b6fe edb5 8ba6 6ea5 6fcf 3bcb  ..],......n.o.;.
+00001810: 3325 9b14 8ad6 92b2 383e a9df 1e5b 1c29  3%......8>...[.)
+00001820: 58cb 13c5 b944 617d aeac 2cce cca4 12c9  X....Da}..,.....
+00001830: a9f9 c56b 657d e2fb a58d a9b9 d994 120a  ...ke}..........
+00001840: f565 d3c6 8a5d 1a01 151b eb36 8865 4753  .e...].....6.eGS
+00001850: 8a7d f146 31a9 65f4 e4d2 e5a5 e4ca 1535  .}.F1.e........5
+00001860: 599e 5f1f 9f34 af67 6653 0bc9 f444 d19a  Y._..4.gfS...D..
+00001870: 1d29 c252 4a36 6dae 838a e4ec 8461 6ba9  .).RJ6m......ak.
+00001880: 8235 6996 9956 ae72 6c3e 9750 6f59 2be3  .5i..V.rl>.PoY+.
+00001890: d1b9 c444 3943 ccd2 b5c9 2b37 9cd1 d4ed  ...D9C....+7....
+000018a0: ab8b f1a2 b304 2ad3 e3eb f6ca 7411 545c  ......*.....t.T\
+000018b0: fd5e df48 92d4 8293 b8b4 06a2 6b76 c22c  .^.H........kv.,
+000018c0: 6767 53ab 16d1 d76c ad50 7612 336b 4932  ggS....l.Pv.3kI2
+000018d0: 51b4 97a7 17c7 4617 d6ac 8451 beba 32a1  Q.....F....Q..2.
+000018e0: e4d2 1b05 a616 5404 69f6 a92d 3ae9 eb45  ......T.i..-:..E
+000018f0: b0d2 b012 2d2a 0ccf 6950 d1d1 6f6d 6635  ....-*..iP..omf5
+00001900: 49e6 8ad6 4aaa 9cd4 3c87 9b4e c2b2 26a8  I...J...<..N..&.
+00001910: 185b 5e50 9cd1 0bd1 64c9 246c f54c c928  .[^P....d.$l.L.(
+00001920: 3993 7150 7909 2271 59c9 4c9a 4b96 76a5  9.qPy."qY.L.K.v.
+00001930: 00d1 1190 af92 aba3 33ab 1e36 0c8b ce4e  ........3..6...N
+00001940: f88c 770a 99a5 a311 6311 0934 1e02 9730  ..w.....c..4...0
+00001950: 4b76 c9d4 e6d2 637e 35ab 569b 1aa6 e258  Kv....c~5.V....X
+00001960: 0c9a 6a20 d0d7 2dcd 29fb 9cd1 8fc0 e968  ..j ..-.)......h
+00001970: 4ec9 d0c6 4b06 04cf 2e8e 2f5d b80d ea32  N...K...../]...2
+00001980: 53d3 1b53 19b2 50b0 d297 7c96 2c94 b353  S..S..P...|.,..S
+00001990: 4d4b 9815 dda7 af81 15c0 8fcb eb19 32bd  MK............2.
+000019a0: 982c ebe7 0373 2a20 c736 ff05 0d0a 3030  .,...s* .6....00
+000019b0: 3030 3030 3630 2030 3030 3030 3036 3020  000060 00000060 
+000019c0: 3766 6666 6666 6666 200d 0a60 030a a27c  7fffffff ..`...|
+000019d0: 4402 0060 030a a27c 4402 0000 0000 0062  D..`...|D......b
+000019e0: 0039 0030 0064 0038 0035 0038 0036 002d  .9.0.d.8.5.8.6.-
+000019f0: 0061 0031 0032 0065 002d 0034 0035 0066  .a.1.2.e.-.4.5.f
+00001a00: 0036 002d 0061 0031 0038 0032 002d 0034  .6.-.a.1.8.2.-.4
+00001a10: 0065 0035 0061 0030 0038 0037 0062 0031  .e.5.a.0.8.7.b.1
+00001a20: 0064 0032 0038 0000 0000 000d 0a30 3030  .d.2.8.......000
+00001a30: 3030 3161 6420 3030 3030 3032 3030 2037  001ad 00000200 7
+00001a40: 6666 6666 6666 6620 0d0a 8d52 496a 5c31  fffffff ...RIj\1
+00001a50: 10dd 1b7c 87e6 af55 509a 4aa5 65c8 1972  ...|...UP.J.e..r
+00001a60: 000d a555 20c1 7156 a6c1 19c8 2681 2cb3  ...U .qV....&.,.
+00001a70: ce0d 9c84 4063 63fb 0afa 27c9 1552 bf1b  ....@cc...'..R..
+00001a80: bc36 08f1 241e f506 e9df dde3 9535 e767  .6..$........5.g
+00001a90: 5735 63e7 c804 c53a 8110 c786 d841 9058  W5c....:.....A.X
+00001aa0: 9053 b5dd f1de 1ca9 cdb3 b7d2 183a f708  .S...........:..
+00001ab0: 6164 0f5c 9c83 91eb 2882 c9bb 3436 de91  ad.\....(...46..
+00001ac0: 1c4c 5776 7124 601b 5508 5699 59ba 8751  .LWvq$`.U.V.Y..Q
+00001ad0: 47f2 5c49 05ad 61c1 1152 8850 521b 107c  G.\I..a..R.PR..|
+00001ae0: f590 6b65 a896 c947 c2e8 84b6 71f8 3418  ..ke...G....q.4.
+00001af0: 0d9a 680b 06ec 016a 6175 c294 8193 b380  ..h....jau......
+00001b00: 218d 18aa 60ef 696f 9697 afdf bc93 17e3  !...`.io........
+00001b10: 522e 5ebd ede5 5296 d390 e5e2 fd62 96f9  R.^...R......b..
+00001b20: 63de ccdb f57a fdba 7e5c bfed ecfc b99b  c....z..~\......
+00001b30: 8ff3 61fd 30ef e6df dd7c 98bf e6bd eebf  ..a.0....|......
+00001b40: b7a3 a2c3 fa7d 376f f5e2 7efd 3c0f f3cf  .....}7o..~.<...
+00001b50: fa69 bd9e 37eb 17c5 8745 b516 b585 fbf3  .i..7....E......
+00001b60: b3bd 2167 136d 1988 b748 6968 4d2d 2344  ..!g.m...HihM-#D
+00001b70: 89d9 b156 40ae 6f7c 0ad8 4a73 1e62 d5fa  ...V@.o|..Js.b..
+00001b80: 434e 023c b081 b0e3 5ac5 4b29 7e6f c2e6  CN.<....Z.K)~o..
+00001b90: d9d5 2603 bb06 cc6c c1da 4e50 b32a 2046  ..&....l..NP.* F
+00001ba0: ac5a 7dc9 b1ab fa46 f5bd 4841 4b40 b926  .Z}....F..HAK@.&
+00001bb0: 7d45 2d29 87e8 c1ba 94ad f5c9 0d2d f444  }E-).........-.D
+00001bc0: edb1 a244 e9e0 2275 0868 1be4 e609 0679  ...D.."u.h.....y
+00001bd0: 7536 3a17 72c6 3dcb e7b3 421f 4545 3f43  u6:.r.=...B.EE?C
+00001be0: d55b a8a9 3084 9e14 49cb 4091 2da6 4239  .[..0...I.@.-.B9
+00001bf0: b771 2af2 b4fe 0300 0000 0000 0000 0000  .q*.............
 00001c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c40: 0000 0000 0000 0000 0000 0000 000d 0a30  ...............0
-00001c50: 3030 3030 3032 3820 3030 3030 3030 3238  0000028 00000028
-00001c60: 2037 6666 6666 6666 6620 0d0a b0f5 4b60   7fffffff ....K`
-00001c70: 4e44 0200 b0f5 4b60 4e44 0200 0000 0000  ND....K`ND......
-00001c80: 6300 6f00 7000 7900 6900 6e00 6600 6f00  c.o.p.y.i.n.f.o.
-00001c90: 0000 0000 0d0a 3030 3030 3030 6639 2030  ......000000f9 0
-00001ca0: 3030 3030 3230 3020 3766 6666 6666 6666  0000200 7fffffff
-00001cb0: 200d 0a95 9131 4e83 310c 85f7 4abd 44e7   ....1N.1...J.D.
-00001cc0: 584a 9cc4 7146 c48c 9838 8013 3b08 0901  XJ..qF...8..;...
-00001cd0: 2a5d 50d5 9331 7024 ae40 feb6 88f5 67b1  *]P..1p$.@....g.
-00001ce0: 25e7 bda7 cfce f7e7 d731 b9ed e618 9792  %........1......
-00001cf0: 83f8 e435 4113 ce90 982a 70c1 003e 9591  ...5A....*p..>..
-00001d00: 5333 af5a dc2a 5158 e27a e418 ac33 28eb  S3.Z.*QX.z...3(.
-00001d10: 548e 1a81 0511 466d 43cc 9788 65b8 dded  T.....FmC...e...
-00001d20: f3eb bbdd 8c83 ed1f de54 0eb6 3b6d 37a7  .........T..;m7.
-00001d30: c54e 180a b5c6 40dc 07cc f469 efd5 43b6  .N....@....i..C.
-00001d40: 5c91 ab29 a1ba 55a2 338d e6e6 2d9b 0266  \..)..U.3...-..f
-00001d50: 5248 3e74 a83d 120c 8abe cb50 1642 b7bb  RH>t.=.....P.B..
-00001d60: dfeb d38b ec3f fe28 d27c ed18 2137 2648  .....?.(.|..!7&H
-00001d70: b518 f0f0 1d8c 915b b368 22d1 ad12 fd83  .......[.h".....
-00001d80: e24e 5ee4 d1f4 0c71 e5b8 b8e7 4105 c920  .N^....q....A.. 
-00001d90: 746a 90c2 3ce6 5c31 c268 a344 6e24 01c3  tj..<.\1.h.Dn$..
-00001da0: ba0f f2bf b9fe 52dd b52f e31f 0000 0000  ......R../......
+00001c40: 0000 0000 0000 0000 0000 0d0a 3030 3030  ............0000
+00001c50: 3030 3238 2030 3030 3030 3032 3820 3766  0028 00000028 7f
+00001c60: 6666 6666 6666 200d 0a60 030a a27c 4402  ffffff ..`...|D.
+00001c70: 0060 030a a27c 4402 0000 0000 0063 006f  .`...|D......c.o
+00001c80: 0070 0079 0069 006e 0066 006f 0000 0000  .p.y.i.n.f.o....
+00001c90: 000d 0a30 3030 3030 3066 3920 3030 3030  ...000000f9 0000
+00001ca0: 3032 3030 2037 6666 6666 6666 6620 0d0a  0200 7fffffff ..
+00001cb0: 9591 314e 8331 0c85 f74a bd44 e758 4a9c  ..1N.1...J.D.XJ.
+00001cc0: c471 46c4 8c98 3880 133b 0809 012a 5d50  .qF...8..;...*]P
+00001cd0: d593 3170 24ae 40fe b688 f567 b125 e7bd  ..1p$.@....g.%..
+00001ce0: a7cf cef7 e7d7 31b9 ede6 1897 9283 f8e4  ......1.........
+00001cf0: 3541 13ce 9098 2a70 c100 3e95 9153 33af  5A....*p..>..S3.
+00001d00: 5adc 2a51 58e2 7ae4 18ac 3328 eb54 8e1a  Z.*QX.z...3(.T..
+00001d10: 8105 1146 6d43 cc97 8865 b8dd edf3 ebbb  ...FmC...e......
+00001d20: dd8c 83ed 1fde 540e b63b 6d37 a7c5 4e18  ......T..;m7..N.
+00001d30: 0ab5 c640 dc07 ccf4 69ef d543 b65c 91ab  ...@....i..C.\..
+00001d40: 29a1 ba55 a233 8de6 e62d 9b02 6652 483e  )..U.3...-..fRH>
+00001d50: 74a8 3d12 0c8a becb 5016 42b7 bbdf ebd3  t.=.....P.B.....
+00001d60: 8bec 3ffe 28d2 7ced 1821 3726 48b5 18f0  ..?.(.|..!7&H...
+00001d70: f01d 8c91 5bb3 6822 d1ad 12fd 83e2 4e5e  ....[.h"......N^
+00001d80: e4d1 f40c 71e5 b8b8 e741 05c9 2074 6a90  ....q....A.. tj.
+00001d90: c23c e65c 31c2 68a3 446e 2401 c3ba 0ff2  .<.\1.h.Dn$.....
+00001da0: bfb9 fe52 ddb5 2fe3 1f00 0000 0000 0000  ...R../.........
 00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -485,23 +485,23 @@
 00001e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001eb0: 0000 000d 0a30 3030 3030 3032 3020 3030  .....00000020 00
-00001ec0: 3030 3030 3230 2037 6666 6666 6666 6620  000020 7fffffff 
-00001ed0: 0d0a b0f5 4b60 4e44 0200 b0f5 4b60 4e44  ....K`ND....K`ND
-00001ee0: 0200 0000 0000 7200 6f00 6f00 7400 0000  ......r.o.o.t...
-00001ef0: 0000 0d0a 3030 3030 3030 3263 2030 3030  ....0000002c 000
-00001f00: 3030 3230 3020 3766 6666 6666 6666 200d  00200 7fffffff .
-00001f10: 0a7b bf7b 7fb5 914e 92a5 418a 85a9 8599  .{.{...N..A.....
-00001f20: 6ea2 a151 aaae 8969 1a88 6561 a46b 926a  n..Q...i..ea.k.j
-00001f30: 9a68 6061 9e64 9862 64a1 530b 0000 0000  .h`a.d.bd.S.....
+00001eb0: 0d0a 3030 3030 3030 3230 2030 3030 3030  ..00000020 00000
+00001ec0: 3032 3020 3766 6666 6666 6666 200d 0a60  020 7fffffff ..`
+00001ed0: 030a a27c 4402 0060 030a a27c 4402 0000  ...|D..`...|D...
+00001ee0: 0000 0072 006f 006f 0074 0000 0000 000d  ...r.o.o.t......
+00001ef0: 0a30 3030 3030 3032 6320 3030 3030 3032  .0000002c 000002
+00001f00: 3030 2037 6666 6666 6666 6620 0d0a 7bbf  00 7fffffff ..{.
+00001f10: 7b7f b591 4e92 a541 8a85 a985 996e a2a1  {...N..A.....n..
+00001f20: 51aa ae89 691a 8865 61a4 6b92 6a9a 6860  Q...i..ea.k.j.h`
+00001f30: 619e 6498 6264 a153 0b00 0000 0000 0000  a.d.bd.S........
 00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -522,23 +522,23 @@
 00002090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000020f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002110: 000d 0a30 3030 3030 3032 3620 3030 3030  ...00000026 0000
-00002120: 3030 3236 2037 6666 6666 6666 6620 0d0a  0026 7fffffff ..
-00002130: b0f5 4b60 4e44 0200 b0f5 4b60 4e44 0200  ..K`ND....K`ND..
-00002140: 0000 0000 7600 6500 7200 7300 6900 6f00  ....v.e.r.s.i.o.
-00002150: 6e00 0000 0000 0d0a 3030 3030 3030 3163  n.......0000001c
-00002160: 2030 3030 3030 3230 3020 3766 6666 6666   00000200 7fffff
-00002170: 6666 200d 0a7b bf7b 7f35 2f57 b591 a199  ff ..{.{.5/W....
-00002180: 8e81 0e90 6161 606c 68a4 6350 cbcb 0542  ....aa`lh.cP...B
+00002100: 0000 0000 0000 0000 0000 0000 0000 0d0a  ................
+00002110: 3030 3030 3030 3236 2030 3030 3030 3032  00000026 0000002
+00002120: 3620 3766 6666 6666 6666 200d 0a60 030a  6 7fffffff ..`..
+00002130: a27c 4402 0060 030a a27c 4402 0000 0000  .|D..`...|D.....
+00002140: 0076 0065 0072 0073 0069 006f 006e 0000  .v.e.r.s.i.o.n..
+00002150: 0000 000d 0a30 3030 3030 3031 6320 3030  .....0000001c 00
+00002160: 3030 3032 3030 2037 6666 6666 6666 6620  000200 7fffffff 
+00002170: 0d0a 7bbf 7b7f 352f 57b5 91a1 998e 810e  ..{.{.5/W.......
+00002180: 9061 6160 6c68 a463 50cb cb05 4200 0000  .aa`lh.cP...B...
 00002190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000021a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000021b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000021c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000021d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000021e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000021f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -561,46 +561,46 @@
 00002300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002370: 0000 0000 000d 0a30 3030 3030 3032 3820  .......00000028 
-00002380: 3030 3030 3030 3238 2037 6666 6666 6666  00000028 7ffffff
-00002390: 6620 0d0a b0f5 4b60 4e44 0200 b0f5 4b60  f ....K`ND....K`
-000023a0: 4e44 0200 0000 0000 7600 6500 7200 7300  ND......v.e.r.s.
-000023b0: 6900 6f00 6e00 7300 0000 0000 0d0a 3030  i.o.n.s.......00
-000023c0: 3030 3031 3863 2030 3030 3030 3230 3020  00018c 00000200 
-000023d0: 3766 6666 6666 6666 200d 0a8d 9141 6e5e  7fffffff ....An^
-000023e0: 3108 84ef f2d6 8f08 30d8 701c 6363 299b  1.......0.p.cc).
-000023f0: fc55 5255 aaaa 9eac 8b1e a957 28ff 26eb  .URU.......W(.&.
-00002400: ec90 187d cc0c fffe fcfd 4537 d17d 5df7  ...}......E7.}].
-00002410: 645c a6cd 61b5 6820 a3a6 c943 2130 6210  d\..a.h ...C!0b.
-00002420: bb0d 5af7 a534 5170 0bc4 3405 b1ee 6083  ..Z..4Qp..4...`.
-00002430: 0950 c651 89c4 bdc7 0b5e f7a6 cd39 6c81  .P.Q.....^...9l.
-00002440: a13b 084a c2cc d361 3796 43d4 7c62 dc57  .;.J...a7.C.|b.W
-00002450: 671a 3dc2 a0db 3a75 f334 b0e5 089a ea6c  g.=...:u.4.....l
-00002460: 9ebb f3be 6e3b ec31 a7c0 3009 9013 01ee  ....n;.1..0.....
-00002470: cfeb 23e6 3ec6 c14c 5f63 3d9d ad3e c789  ..#.>..L_c=..>..
-00002480: d1a1 3155 ce45 0216 7440 d754 b5ce a622  ..1U.E..t@.T..."
-00002490: 4513 5c73 7103 0deb 203e 12ec e082 34b6  E.\sq... >....4.
-000024a0: 886c 3967 2b67 b631 5b35 d5f9 7993 7580  .l9g+g.1[5..y.u.
-000024b0: 6d9f 809c 41b4 f7ac 82be c67a 3ad3 6dea  m...A......z:.m.
-000024c0: 031b 9023 8168 990f e77a c374 ef16 56e6  ...#.h...z.t..V.
-000024d0: 2a67 3896 ae40 9338 4b75 9e93 3148 ea44  *g8..@.8Ku..1H.D
-000024e0: 1b51 c5db 750f 666d d1b1 58a3 76db 8a55  .Q..u.fm..X.v..U
-000024f0: 3bc8 73b4 11c5 e9aa f7b5 1edf 7ebe be9d  ;.s.........~...
-00002500: c775 7ba5 e89d 07d0 99d5 f1d0 a856 42e1  .u{..........VB.
-00002510: 9067 1252 f65d 49de 1f8f efc5 debd 1ddd  .g.R.]I.........
-00002520: 4fd8 1ed5 2033 cc95 0ea8 bcd7 da22 d44a  O... 3.......".J
-00002530: fb23 df3f 5e1f 6fd7 1d23 5b67 61d0 73a4  .#.?^.o..#[ga.s.
-00002540: e267 8263 6fd0 b035 f685 96c7 3ee5 1fa5  .g.co..5....>...
-00002550: f7c5 58cd 41ea da15 ab7e 13b2 0f98 af91  ..X.A....~......
-00002560: 9377 88cc dfff 0100 0000 0000 0000 0000  .w..............
+00002370: 0000 0d0a 3030 3030 3030 3238 2030 3030  ....00000028 000
+00002380: 3030 3032 3820 3766 6666 6666 6666 200d  00028 7fffffff .
+00002390: 0a60 030a a27c 4402 0060 030a a27c 4402  .`...|D..`...|D.
+000023a0: 0000 0000 0076 0065 0072 0073 0069 006f  .....v.e.r.s.i.o
+000023b0: 006e 0073 0000 0000 000d 0a30 3030 3030  .n.s.......00000
+000023c0: 3138 6220 3030 3030 3032 3030 2037 6666  18b 00000200 7ff
+000023d0: 6666 6666 6620 0d0a 8d92 3b6e 5d31 0c05  fffff ....;n]1..
+000023e0: f772 eb4b 43a2 f85d 8e28 4a80 1bbf c00e  .r.KC..].(J.....
+000023f0: 0204 4156 9622 4bca 16c2 d7b8 76a7 e2e8  ..AV."K.....v...
+00002400: 7046 d4bf 3f7f 7ff5 bbf7 fbba eeb9 28c6  pF..?.........(.
+00002410: 680a 6aaa 405d 1882 86c1 382e e6ec bce6  h.j.@]....8.....
+00002420: ba2f eeb3 514b 8298 c640 260e a6d8 a191  ./..QK...@&.....
+00002430: 1ea6 d82d 535f 5ab5 998d c522 70f4 38d0  ...-S_Z...."p.8.
+00002440: 2181 8931 2163 f4d8 6b0c a49a 2ad8 5522  !..1!c..k...*.U"
+00002450: 0cc4 d681 aa18 60cb 1bf0 6647 f39d 8279  ......`...fG...y
+00002460: dded 0c8d a501 baa6 d54c 0a70 1784 1872  .........L.p...r
+00002470: 94ac 0dde f6b5 ae27 d91a b21d 8f00 1227  .......'.......'
+00002480: d08e 0351 d430 b549 e2d8 8839 ab8d 5af9  ...Q.0.I...9..Z.
+00002490: e200 0e13 20d7 0d76 da82 6d68 117b ec39  .... ..v..mh.{.9
+000024a0: 4791 0dec 6d79 c24a 5940 b118 66af 7719  G...my.JY@..f.w.
+000024b0: 278e bb62 06fa d7ba 9e64 6351 f6de 1324  '..b.....dcQ...$
+000024c0: a997 a721 585d 8145 139d 829b 36bc aff0  ...!X].E....6...
+000024d0: 96c6 5534 3b6e 203e cf53 4569 f36c a6d1  ..U4;n >.SEi.l..
+000024e0: 13ed ba35 b393 ea82 e854 9639 0e38 a680  ...5.....T.9.8..
+000024f0: b4c6 54d8 7938 ee6b 3dbe fd7c 7d3b 8f32  ..T.y8.k=..|};.2
+00002500: 69ec 0d77 c0a9 a597 0997 c999 f8dc b012  i..w............
+00002510: 8fe6 467a 5fef 8fc7 f7eb dea8 9e9a 5ecb  ..Fz_.........^.
+00002520: ecc5 39cc c0cc 36f8 f120 e6dc c8f5 537e  ..9...6.. ....S~
+00002530: ecf7 8fd7 c75b c5a7 8bc4 3980 d2a8 8077  .....[....9....w
+00002540: 2569 056c ac4b 9c62 47ed 33fe 5128 a593  %i.l.K.bG.3.Q(..
+00002550: 920a b9bd 5064 7698 3b17 b8f1 4047 dfd2  ....Pdv.;...@G..
+00002560: f2f7 7f00 0000 0000 0000 0000 0000 0000  ................
 00002570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000025a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000025b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000025c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000025d0: 0000 0000 0000 0000 0000 00              ...........
+000025d0: 0000 0000 0000 0000                      ........
```

### Comparing `runner1c-0.58/runner1c/build/tools/epf/FileCompareMxl.epf` & `runner1c-0.59/runner1c/build/tools/epf/FileCompareMxl.epf`

 * *Files 21% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 000d  ................
 00000230: 0a30 3030 3030 3036 3020 3030 3030 3030  .00000060 000000
-00000240: 3630 2037 6666 6666 6666 6620 0d0a c01c  60 7fffffff ....
-00000250: 4c60 4e44 0200 c01c 4c60 4e44 0200 0000  L`ND....L`ND....
+00000240: 3630 2037 6666 6666 6666 6620 0d0a 702a  60 7fffffff ..p*
+00000250: 0aa2 7c44 0200 702a 0aa2 7c44 0200 0000  ..|D..p*..|D....
 00000260: 0000 3100 3900 6600 3500 6500 3700 3900  ..1.9.f.5.e.7.9.
 00000270: 3500 2d00 3900 6200 6600 3900 2d00 3400  5.-.9.b.f.9.-.4.
 00000280: 6600 3700 6500 2d00 3900 3600 3300 6300  f.7.e.-.9.6.3.c.
 00000290: 2d00 3500 3800 3700 3500 3900 6200 6100  -.5.8.7.5.9.b.a.
 000002a0: 3900 3600 3600 3100 3500 0000 0000 0d0a  9.6.6.1.5.......
 000002b0: 3030 3030 3031 3531 2030 3030 3030 3230  00000151 0000020
 000002c0: 3020 3766 6666 6666 6666 200d 0a8d 914b  0 7fffffff ....K
@@ -72,16 +72,16 @@
 00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004c0: 0000 0000 0000 0000 0000 0000 000d 0a30  ...............0
 000004d0: 3030 3030 3036 3020 3030 3030 3030 3630  0000060 00000060
-000004e0: 2037 6666 6666 6666 6620 0d0a c01c 4c60   7fffffff ....L`
-000004f0: 4e44 0200 c01c 4c60 4e44 0200 0000 0000  ND....L`ND......
+000004e0: 2037 6666 6666 6666 6620 0d0a 702a 0aa2   7fffffff ..p*..
+000004f0: 7c44 0200 702a 0aa2 7c44 0200 0000 0000  |D..p*..|D......
 00000500: 3900 3300 3500 3300 3300 6300 6100 3800  9.3.5.3.3.c.a.8.
 00000510: 2d00 3300 3600 6300 3400 2d00 3400 3400  -.3.6.c.4.-.4.4.
 00000520: 3200 3300 2d00 3900 3400 3100 3900 2d00  2.3.-.9.4.1.9.-.
 00000530: 3200 3600 3000 3600 3000 3900 3000 3400  2.6.0.6.0.9.0.4.
 00000540: 3400 3600 3200 3400 0000 0000 0d0a 3030  4.6.2.4.......00
 00000550: 3030 3030 3965 2030 3030 3030 3230 3020  00009e 00000200 
 00000560: 3766 6666 6666 6666 200d 0a95 4f49 0a02  7fffffff ...OI..
@@ -114,16 +114,16 @@
 00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000760: 0000 0000 0000 0000 0000 000d 0a30 3030  .............000
 00000770: 3030 3036 3420 3030 3030 3030 3634 2037  00064 00000064 7
-00000780: 6666 6666 6666 6620 0d0a c01c 4c60 4e44  fffffff ....L`ND
-00000790: 0200 c01c 4c60 4e44 0200 0000 0000 3900  ....L`ND......9.
+00000780: 6666 6666 6666 6620 0d0a 702a 0aa2 7c44  fffffff ..p*..|D
+00000790: 0200 702a 0aa2 7c44 0200 0000 0000 3900  ..p*..|D......9.
 000007a0: 3300 3500 3300 3300 6300 6100 3800 2d00  3.5.3.3.c.a.8.-.
 000007b0: 3300 3600 6300 3400 2d00 3400 3400 3200  3.6.c.4.-.4.4.2.
 000007c0: 3300 2d00 3900 3400 3100 3900 2d00 3200  3.-.9.4.1.9.-.2.
 000007d0: 3600 3000 3600 3000 3900 3000 3400 3400  6.0.6.0.9.0.4.4.
 000007e0: 3600 3200 3400 2e00 3000 0000 0000 0d0a  6.2.4...0.......
 000007f0: 3030 3030 3064 3032 2030 3030 3030 6430  00000d02 00000d0
 00000800: 3220 3766 6666 6666 6666 200d 0aed 5c5b  2 7fffffff ...\[
@@ -332,16 +332,16 @@
 000014b0: 8174 c917 ad61 6325 0992 349c 1112 41ec  .t...ac%..4...A.
 000014c0: 4bc1 52e1 3c84 3579 e2d8 41ec cf82 0984  K.R.<.5y..A.....
 000014d0: 8f28 e361 8188 7d0a 9f62 6533 12e1 0ddb  .(.a..}..be3....
 000014e0: 7155 c842 f33f c754 f5c6 8eab b57a 1ef6  qU.B.?.T.....z..
 000014f0: 3318 36a4 8e2d c5bf 13ec 3c3a 9547 f8cb  3.6..-....<:.G..
 00001500: c598 cdea fb3b 2bc1 9437 03d1 a5ff 0f0d  .....;+..7......
 00001510: 0a30 3030 3030 3032 3820 3030 3030 3030  .00000028 000000
-00001520: 3238 2037 6666 6666 6666 6620 0d0a c01c  28 7fffffff ....
-00001530: 4c60 4e44 0200 c01c 4c60 4e44 0200 0000  L`ND....L`ND....
+00001520: 3238 2037 6666 6666 6666 6620 0d0a 702a  28 7fffffff ..p*
+00001530: 0aa2 7c44 0200 702a 0aa2 7c44 0200 0000  ..|D..p*..|D....
 00001540: 0000 6300 6f00 7000 7900 6900 6e00 6600  ..c.o.p.y.i.n.f.
 00001550: 6f00 0000 0000 0d0a 3030 3030 3030 6365  o.......000000ce
 00001560: 2030 3030 3030 3230 3020 3766 6666 6666   00000200 7fffff
 00001570: 6666 200d 0a8d 8f3d 8a03 310c 46fb 402e  ff ....=..1.F.@.
 00001580: 91da 0259 7f63 d781 747b 085b b661 2121  ...Y.c..t{.[.a!!
 00001590: 4baa 8590 936d b147 ca15 7666 92ed a7f9  K....m.G..vf....
 000015a0: 04e2 d3e3 e9f9 f37b 97b0 dfdd 6989 ccca  .......{....i...
@@ -371,16 +371,16 @@
 00001720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001770: 0000 0000 000d 0a30 3030 3030 3032 3020  .......00000020 
 00001780: 3030 3030 3030 3230 2037 6666 6666 6666  00000020 7ffffff
-00001790: 6620 0d0a c01c 4c60 4e44 0200 c01c 4c60  f ....L`ND....L`
-000017a0: 4e44 0200 0000 0000 7200 6f00 6f00 7400  ND......r.o.o.t.
+00001790: 6620 0d0a 702a 0aa2 7c44 0200 702a 0aa2  f ..p*..|D..p*..
+000017a0: 7c44 0200 0000 0000 7200 6f00 6f00 7400  |D......r.o.o.t.
 000017b0: 0000 0000 0d0a 3030 3030 3030 3265 2030  ......0000002e 0
 000017c0: 3030 3030 3230 3020 3766 6666 6666 6666  0000200 7fffffff
 000017d0: 200d 0a7b bf7b 7fb5 918e a165 9a69 aab9   ..{.{.....e.i..
 000017e0: a5a9 ae65 529a a5ae 499a 79aa aea5 9971  ...eR...I.y....q
 000017f0: b2ae a985 b9a9 6552 a2a5 9999 a1a9 4e2d  ......eR......N-
 00001800: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -409,15 +409,15 @@
 00001980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019d0: 0000 000d 0a30 3030 3030 3032 3620 3030  .....00000026 00
 000019e0: 3030 3030 3236 2037 6666 6666 6666 6620  000026 7fffffff 
-000019f0: 0d0a c01c 4c60 4e44 0200 c01c 4c60 4e44  ....L`ND....L`ND
+000019f0: 0d0a 702a 0aa2 7c44 0200 702a 0aa2 7c44  ..p*..|D..p*..|D
 00001a00: 0200 0000 0000 7600 6500 7200 7300 6900  ......v.e.r.s.i.
 00001a10: 6f00 6e00 0000 0000 0d0a 3030 3030 3030  o.n.......000000
 00001a20: 3163 2030 3030 3030 3230 3020 3766 6666  1c 00000200 7fff
 00001a30: 6666 6666 200d 0a7b bf7b 7f35 2f57 b591  ffff ..{.{.5/W..
 00001a40: a199 8e81 0e90 6161 606c 68a4 6350 cbcb  ......aa`lh.cP..
 00001a50: 0542 0000 0000 0000 0000 0000 0000 0000  .B..............
 00001a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -447,37 +447,37 @@
 00001be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c30: 0000 0000 0000 000d 0a30 3030 3030 3032  .........0000002
 00001c40: 3820 3030 3030 3030 3238 2037 6666 6666  8 00000028 7ffff
-00001c50: 6666 6620 0d0a c01c 4c60 4e44 0200 c01c  fff ....L`ND....
-00001c60: 4c60 4e44 0200 0000 0000 7600 6500 7200  L`ND......v.e.r.
+00001c50: 6666 6620 0d0a 702a 0aa2 7c44 0200 702a  fff ..p*..|D..p*
+00001c60: 0aa2 7c44 0200 0000 0000 7600 6500 7200  ..|D......v.e.r.
 00001c70: 7300 6900 6f00 6e00 7300 0000 0000 0d0a  s.i.o.n.s.......
-00001c80: 3030 3030 3031 3163 2030 3030 3030 3230  0000011c 0000020
-00001c90: 3020 3766 6666 6666 6666 200d 0a8d 904b  0 7fffffff ....K
-00001ca0: 6e50 310c 45f7 9271 8cec f813 7b39 713e  nP1.E..q....{9q>
-00001cb0: 5227 7da8 4548 08b1 3206 2c89 2d90 4e3a  R'}.EH..2.,.-.N:
-00001cc0: 666e 9f7b eff9 fbfb cf4f aa5e 4ba9 3b31  fn.{.....O.^K.;1
-00001cd0: 8677 07ec 6e20 2213 86ce 017b 8f3e 0871  .w..n "....{.>.q
-00001ce0: e59a b550 1cdd 3d14 224f 809c be21 8c27  ...P..=."O...!.'
-00001cf0: a877 8d1c 6146 5aea f023 2e97 7524 1c24  .w..aFZ..#..u$.$
-00001d00: e3b2 1a13 0c5c 819e c1c2 544b b032 cfe1  .....\....TK.2..
-00001d10: c036 e526 3686 100a 6886 8681 22d6 a454  .6.&6...h..."..T
-00001d20: 6d31 f58c 0e19 ed26 2a19 8c35 1832 795d  m1.....&*..5.2y]
-00001d30: ba8d eced ff58 5fb0 d4a5 b769 ac06 e871  .....X_....i...q
-00001d40: 57f6 9310 6b6d 681c 9626 4bc4 2f6d 3e5f  W...kmh..&K./m>_
-00001d50: 7fbc bc9e a7d4 e446 a363 8261 7eec 4502  .......F.c.a~.E.
-00001d60: 8ffb c99b 8e20 db38 78ad bc3d cfb7 525b  ..... .8x..=..R[
-00001d70: e8da 1e09 53b7 5e36 250c cb03 11aa 3ad8  ....S.^6%.....:.
-00001d80: 6cc7 aee5 fb7e 7b7f 795e 4b0d 4e15 a20d  l....~{.y^K.N...
-00001d90: 9b8c 41f6 c63b cc14 d6ea ce76 dca6 c7e7  ..A..;.....v....
-00001da0: f97b a9e7 ec7d 2811 92ae 4f41 3dd7 2775  .{...}(...OA=.'u
-00001db0: 7041 5ad7 8378 e6af 7f00 0000 0000 0000  pAZ..x..........
+00001c80: 3030 3030 3031 3166 2030 3030 3030 3230  0000011f 0000020
+00001c90: 3020 3766 6666 6666 6666 200d 0a8d 9131  0 7fffffff ....1
+00001ca0: 6e98 3108 85ef e2d9 54b6 c160 8e83 0d48  n.1.....T..`...H
+00001cb0: 59f2 5749 55a9 aa7a b20e 3d52 af50 67c9  Y.WIU..z..=R.Pg.
+00001cc0: 5cb1 30c0 c77b 8fbf bfff fcec 75d5 526a  \.0..{......u.Rj
+00001cd0: 2072 982e 38e8 0768 f504 5bd8 81d3 74e2   r..8..h..[...t.
+00001ce0: a2b4 396b e99a 3344 27e8 4e05 4a09 50c6  ..9k..3D'.N.J.P.
+00001cf0: 0373 c9d4 6dca dc67 a9c4 2cd3 4561 f062  .s..m..g..,.Ea.b
+00001d00: 20f3 8025 be20 51b3 1fda d993 6b51 9c88   ..%. Q.....kQ..
+00001d10: c716 201f 02a2 81a0 d43f 961a 376d 443c  .. ......?..7mD<
+00001d20: e8b2 e270 7824 9c8d 0224 1a60 b81d aca5  ...px$...$.`....
+00001d30: bb9e 3ece 58ff c7fa d24a 65db dbdc 1c86  ..>.X....Je.....
+00001d40: b50d 74fb abdf 1d5a c366 4c2e 285e cb79  ..t....Z.fL.(^.y
+00001d50: befe 7879 cda7 54d4 c522 b2c1 1d0d a84b  ..xy..T..".....K
+00001d60: 83ad d400 7b46 deeb fb8c 9bca dbf3 7c2b  ....{F........|+
+00001d70: 75b5 46a7 f304 51cc eb7a 5e76 5840 1363  u.F...Q..z^vX@.c
+00001d80: 5f9d 2f9a 6af9 1e6f ef2f cf6b a9ad e7e2  _./.j..o./.k....
+00001d90: cd0d 2ce6 95a2 71c7 375f 77ae 19ec d46f  ..,...q.7_w....o
+00001da0: 7d8e bfdf 2096 8f71 5990 deaf 94b1 1376  }... ..qY......v
+00001db0: 9c01 a6f7 596b 9f99 437e fd03 0000 0000  ....Yk..C~......
 00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `runner1c-0.58/runner1c/command.py` & `runner1c-0.59/runner1c/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,92 +3,86 @@
 при переопределении декоратор теряется, поэтому нельзя переопределять run
 run вызывается, если нужна пред обработка или пост обработка, причем для этого переопределяем execute
 execute используется как точка входа плагина
 """
 
 import abc
 import copy
-import logging
 import os
 import socket
 import subprocess
 import tempfile
 import time
 from enum import Enum
 
 import paramiko
 
 import runner1c.common as common
 import runner1c.exit_code
+import runner1c.logger
 
 
 def create_base_if_necessary(func):
     def wrapper(self):
         if not self.need_connection or getattr(self.arguments, 'connection', False):
             return func(self)
         else:
             temp_folder = tempfile.mkdtemp()
             connection = 'File={}'.format(temp_folder)
 
             p_create_base = runner1c.command.EmptyParameters(self.arguments)
             setattr(p_create_base, 'connection', connection)
-            # todo нужно копирование logger handler при multiprocessing
-            command = CreateBase(arguments=p_create_base)
+            command = CreateBase(arguments=p_create_base, parent=self)
             return_code = command.execute()
 
             if runner1c.exit_code.success_result(return_code):
                 setattr(self.arguments, 'connection', connection)
                 return_code = self.execute()
 
             common.clear_folder(temp_folder)
 
             return return_code
 
     return wrapper
 
 
-class Command(abc.ABC):
+class Command(runner1c.logger.Logger, abc.ABC):
     def __init__(self, **kwargs):
-        self._logger = kwargs.get('logger', None)
-        if self._logger is None:
-            self._logger = logging.getLogger(self.name)
-
+        super().__init__(**kwargs)
         self.arguments = copy.copy(kwargs['arguments'])
+        self._init_agent_mode(kwargs)
+        self._program_1c_arguments = []
+        self._program_1c = ''
+        self._version_1c = ''
+        self._init_mode(kwargs)
+        self._set_path_1c()
+
+    def _init_mode(self, kwargs):
         self._mode = kwargs.get('mode', None)
+        if self._mode == Mode.DESIGNER:
+            self._set_designer()
+        elif self._mode == Mode.ENTERPRISE:
+            self._set_enterprise()
+        elif self._mode == Mode.CREATE:
+            self._set_create_base()
 
+    def _init_agent_mode(self, kwargs):
         self._client = None
         self._channel = None
         self._connect_to_agent = False
         self._need_close_agent = False
         agent_channel = kwargs.get('agent_channel', None)
         if agent_channel is not None:
             self._client, self._channel = agent_channel
             self._connect_to_agent = True
         self._agent_port = kwargs.get('agent_port', None)
         self._agent_folder = ''
         self._agent_process = None
         self._agent_server = '127.0.0.1'
 
-        self._program_1c_arguments = []
-        self._program_1c = ''
-        self._version_1c = ''
-
-        if self._mode == Mode.DESIGNER:
-            self._set_designer()
-        elif self._mode == Mode.ENTERPRISE:
-            self._set_enterprise()
-        elif self._mode == Mode.CREATE:
-            self._set_create_base()
-
-        self._set_path_1c()
-
-    @property
-    def name(self):
-        return self.__class__.__name__
-
     @property
     def default_result(self):
         return runner1c.exit_code.EXIT_CODE.error
 
     @property
     def need_connection(self):
         return True
@@ -101,36 +95,29 @@
         return self._start()
 
     def get_module_ordinary_form(self, dir_for_scan):
         for folder in dir_for_scan:
             for bin_form in self._find_bin_forms(folder):
                 self._parse_module_from_bin(bin_form)
 
-    def debug(self, msg, *args):
-        self._logger.debug(msg, *args)
-
-    def error(self, msg, *args):
-        self._logger.error(msg, *args)
-
-    def start_agent(self, logger=None):
+    def start_agent(self):
         if self._connect_to_agent:
             return
 
         self._need_close_agent = True
 
         self._agent_port = self._get_port_for_agent()
         self._agent_folder = os.path.split(self.arguments.folder)[0]
 
         # запуск конфигуратора в режиме агента
         p_agent = runner1c.command.EmptyParameters(self.arguments)
         setattr(p_agent, 'connection', self.arguments.connection)
         setattr(p_agent, 'folder', self._agent_folder)
         setattr(p_agent, 'port', self._agent_port)
-        # todo нужно копирование logger handler при multiprocessing
-        agent = StartAgent(arguments=p_agent, logger=logger)
+        agent = StartAgent(arguments=p_agent, parent=self)
         return_code = agent.execute()
         if not runner1c.exit_code.success_result(return_code):
             raise Exception('Failed start agent')
 
         self._agent_process = agent.process
         del agent
```

### Comparing `runner1c-0.58/runner1c/commands/base_for_test.py` & `runner1c-0.59/runner1c/commands/base_for_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import multiprocessing
 import os
-import tempfile
 from logging.handlers import QueueHandler
 from logging.handlers import QueueListener
 
 import runner1c
 import runner1c.commands.load_config as load_config
 import runner1c.commands.load_extension as load_extension
 import runner1c.commands.start as start
@@ -47,18 +46,18 @@
 
 class BaseForTest(runner1c.command.Command):
     def execute(self):
         fixtures_src = os.path.join('spec', 'fixtures')
         lib_src = 'lib'
 
         config_path = {'config_src': os.path.join(self.arguments.folder, 'cf'),
-                       'epf_src': ','.join([os.path.join(self.arguments.folder, fixtures_src),
-                                            os.path.join(self.arguments.folder, lib_src)]),
+                       'lib_src': os.path.join(self.arguments.folder, lib_src),
                        'ext_src': os.path.join(self.arguments.folder, lib_src, 'ext'),
-                       'path_to_fixtures': os.path.join(self.arguments.folder, 'build', fixtures_src)}
+                       'fixtures_src': os.path.join(self.arguments.folder, fixtures_src),
+                       'fixtures_epf': os.path.join(self.arguments.folder, 'build', fixtures_src)}
 
         self.start_agent()
         agent_port = self.get_agent_port()
         stream_handler = logging.StreamHandler()
         if self.arguments.debug:
             stream_handler.setLevel(logging.DEBUG)
         queue = multiprocessing.Queue(-1)
@@ -85,86 +84,71 @@
         queue_listener.stop()
         self.close_agent()
 
         # todo нужен анализ результата запуска процессов
         return runner1c.exit_code.EXIT_CODE.done
 
 
-def _get_logger(arguments, name, queue):
-    logger = logging.getLogger(name)
-    if arguments.debug:
-        logger.setLevel(logging.DEBUG)
-    if queue:
-        handler = QueueHandler(queue)
-        handler.setFormatter(logging.Formatter(common.get_formatter_string()))
-        logger.addHandler(handler)
-    return logger
-
-
 def _create_test(arguments, config_path, queue):
-    temp_folder = tempfile.mkdtemp()
-    p_create = runner1c.command.EmptyParameters(arguments)
-    setattr(p_create, 'connection', 'File={}'.format(temp_folder))
-    logger = _get_logger(arguments, "CreateBase_create_test", queue)
-    command_create = runner1c.command.CreateBase(arguments=p_create, logger=logger)
-    return_code = command_create.execute()
-    if not exit_code.success_result(return_code):
-        raise _ProcessError(logger.name, return_code)
-
     p_test = runner1c.command.EmptyParameters(arguments)
-    setattr(p_test, 'connection', p_create.connection)
     setattr(p_test, 'folder', arguments.folder)
     setattr(p_test, 'create', True)
-    setattr(p_test, 'exclude', config_path['epf_src'])
-    logger = _get_logger(arguments, "Sync_create_test", queue)
-    command = sync.Sync(arguments=p_test, logger=logger)
-    logger_agent = _get_logger(arguments, "Agent_create_test", queue)
-    command.start_agent(logger_agent)
-    command.connect_to_agent()
+    setattr(p_test, 'exclude', ','.join([config_path['lib_src'], config_path['fixtures_src']]))
+    command = sync.Sync(arguments=p_test, logger_handlers=[QueueHandler(queue)])
     return_code = command.execute()
-    if exit_code.success_result(return_code):
-        common.clear_folder(temp_folder)
-    else:
-        raise _ProcessError(logger.name, return_code)
+    if not exit_code.success_result(return_code):
+        raise _ProcessError(command.get_logger_name(), return_code)
 
 
-def _create_base(arguments, config_path, agent_port, queue=None):
+def _create_base(arguments, config_path, agent_port, queue):
     p_create = runner1c.command.EmptyParameters(arguments)
     setattr(p_create, 'connection', arguments.connection)
-    logger = _get_logger(arguments, "CreateBase_create_base", queue)
-    command_create = runner1c.command.CreateBase(arguments=p_create, logger=logger)
+    command_create = runner1c.command.CreateBase(arguments=p_create, logger_handlers=[QueueHandler(queue)])
     return_code = command_create.execute()
     if not exit_code.success_result(return_code):
-        raise _ProcessError(logger.name, return_code)
+        raise _ProcessError(command_create.get_logger_name(), return_code)
 
     p_load_config = runner1c.command.EmptyParameters(arguments)
     setattr(p_load_config, 'connection', arguments.connection)
     setattr(p_load_config, 'folder', config_path['config_src'])
     setattr(p_load_config, 'agent', True)
     setattr(p_load_config, 'update', True)
-    logger = _get_logger(arguments, "LoadConfig_create_base", queue)
-    command_load_cf = load_config.LoadConfig(arguments=p_load_config, agent_port=agent_port, logger=logger)
+    command_load_cf = load_config.LoadConfig(arguments=p_load_config,
+                                             agent_port=agent_port,
+                                             logger_handlers=[QueueHandler(queue)])
     command_load_cf.connect_to_agent()
     return_code = command_load_cf.execute()
     if not exit_code.success_result(return_code):
-        raise _ProcessError(logger.name, return_code)
+        raise _ProcessError(command_load_cf.get_logger_name(), return_code)
 
     if getattr(arguments, 'create_cfe', False):
         p_extensions = runner1c.command.EmptyParameters(arguments)
         setattr(p_extensions, 'connection', arguments.connection)
         setattr(p_extensions, 'folder', config_path['ext_src'])
         setattr(p_extensions, 'agent', True)
         setattr(p_extensions, 'update', True)
-        logger = _get_logger(arguments, "LoadExtension_create_base", queue)
         command_load_ext = load_extension.LoadExtension(arguments=p_extensions,
                                                         agent_channel=command_load_cf.get_agent_channel(),
-                                                        logger=logger)
+                                                        logger_handlers=[QueueHandler(queue)])
         return_code = command_load_ext.execute()
         if not exit_code.success_result(return_code):
-            raise _ProcessError(logger.name, return_code)
+            raise _ProcessError(command_load_ext.get_logger_name(), return_code)
+
+    if getattr(arguments, 'create_epf', False):
+        p_sync = runner1c.command.EmptyParameters(arguments)
+        setattr(p_sync, 'connection', arguments.connection)
+        setattr(p_sync, 'folder', arguments.folder)
+        setattr(p_sync, 'create', True)
+        setattr(p_sync, 'include', config_path['fixtures_src'])
+        command_create_epf = sync.Sync(arguments=p_sync,
+                                        agent_channel=command_load_cf.get_agent_channel(),
+                                        logger_handlers=[QueueHandler(queue)])
+        return_code = command_create_epf.execute()
+        if not exit_code.success_result(return_code):
+            raise _ProcessError(command_create_epf.get_logger_name(), return_code)
 
     command_load_cf.disconnect_from_agent()
     if getattr(arguments, 'create_epf', False):
         command_load_cf.debug('start child multiprocessing')
 
         args = (arguments, config_path, queue)
         proc_enterprise = multiprocessing.Process(name='start_enterprise',
@@ -182,38 +166,36 @@
         proc_create_epf.join()
 
         command_load_cf.debug('stop child multiprocessing')
     else:
         _start_enterprise(arguments, config_path, queue)
 
 
-def _start_enterprise(arguments, config_path, queue=None):
+def _start_enterprise(arguments, config_path, queue):
     p_start = runner1c.command.EmptyParameters(arguments)
     setattr(p_start, 'connection', arguments.connection)
     setattr(p_start, 'thick', arguments.thick)
     setattr(p_start, 'epf', common.get_path_to_project(os.path.join('runner1c',
                                                                     'build',
                                                                     'tools',
                                                                     'epf',
                                                                     'CloseAfterUpdate.epf')))
-    if os.path.exists(config_path['path_to_fixtures']):
-        setattr(p_start, 'options', config_path['path_to_fixtures'])
-    logger = _get_logger(arguments, "Start_start_enterprise", queue)
-    command = runner1c.commands.start.Start(arguments=p_start, logger=logger)
+    if os.path.exists(config_path['fixtures_epf']):
+        setattr(p_start, 'options', config_path['fixtures_epf'])
+    command = runner1c.commands.start.Start(arguments=p_start, logger_handlers=[QueueHandler(queue)])
     return_code = command.execute()
     if not exit_code.success_result(return_code):
-        raise _ProcessError(logger.name, return_code)
+        raise _ProcessError(command.get_logger_name(), return_code)
 
 
 def _create_epf(arguments, agent_port, config_path, queue):
     p_sync = runner1c.command.EmptyParameters(arguments)
     setattr(p_sync, 'connection', arguments.connection)
     setattr(p_sync, 'folder', arguments.folder)
     setattr(p_sync, 'create', True)
-    setattr(p_sync, 'include', config_path['epf_src'])
-    logger = _get_logger(arguments, "Sync_create_epf", queue)
-    command = sync.Sync(arguments=p_sync, agent_port=agent_port, logger=logger)
+    setattr(p_sync, 'include', config_path['lib_src'])
+    command = sync.Sync(arguments=p_sync, agent_port=agent_port, logger_handlers=[QueueHandler(queue)])
     command.connect_to_agent()
     return_code = command.execute()
     command.disconnect_from_agent()
     if not exit_code.success_result(return_code):
-        raise _ProcessError(logger.name, return_code)
+        raise _ProcessError(command.get_logger_name(), return_code)
```

### Comparing `runner1c-0.58/runner1c/commands/create_epf.py` & `runner1c-0.59/runner1c/commands/create_epf.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/commands/diff_mxl.py` & `runner1c-0.59/runner1c/commands/diff_mxl.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,8 +34,8 @@
         setattr(p_start, 'epf', common.get_path_to_project(os.path.join('runner1c',
                                                                         'build',
                                                                         'tools',
                                                                         'epf',
                                                                         'FileCompareMxl.epf')))
         setattr(p_start, 'options', options)
 
-        return runner1c.commands.start.Start(arguments=p_start).execute()
+        return runner1c.commands.start.Start(arguments=p_start, parent=self).execute()
```

### Comparing `runner1c-0.58/runner1c/commands/dump_config.py` & `runner1c-0.59/runner1c/commands/dump_config.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/commands/dump_epf.py` & `runner1c-0.59/runner1c/commands/dump_epf.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/commands/dump_extensions.py` & `runner1c-0.59/runner1c/commands/dump_extensions.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/commands/file.py` & `runner1c-0.59/runner1c/commands/file.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/commands/load_config.py` & `runner1c-0.59/runner1c/commands/load_config.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/commands/load_extension.py` & `runner1c-0.59/runner1c/commands/load_extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             if getattr(self.arguments, 'name', False) and len(extensions_name) > 1:
                 error_in_loop = False
                 for name in extensions_name:
                     p_extensions = runner1c.command.EmptyParameters(self.arguments)
                     setattr(p_extensions, 'connection', self.arguments.connection)
                     setattr(p_extensions, 'folder', self.arguments.folder)
                     setattr(p_extensions, 'name', name)
-                    return_code = LoadExtension(arguments=p_extensions).execute()
+                    return_code = LoadExtension(arguments=p_extensions, parent=self).execute()
                     if not runner1c.exit_code.success_result(return_code):
                         error_in_loop = True
                         break
                 if error_in_loop:
                     return error_code
                 else:
                     return self.default_result
@@ -119,15 +119,15 @@
                 p_start = runner1c.command.EmptyParameters(self.arguments)
                 setattr(p_start, 'connection', self.arguments.connection)
                 setattr(p_start, 'epf', common.get_path_to_project(os.path.join('runner1c',
                                                                                 'build',
                                                                                 'tools',
                                                                                 'epf',
                                                                                 'ChangeSafeModeForExtension.epf')))
-                return_code = runner1c.commands.start.Start(arguments=p_start).execute()
+                return_code = runner1c.commands.start.Start(arguments=p_start, parent=self).execute()
 
             return return_code
 
     def _get_extensions_name(self):
         if os.path.exists(self.arguments.folder):
             result = os.listdir(self.arguments.folder)
         else:
```

### Comparing `runner1c-0.58/runner1c/commands/platform_check.py` & `runner1c-0.59/runner1c/commands/platform_check.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/commands/reg_server.py` & `runner1c-0.59/runner1c/commands/reg_server.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/commands/start.py` & `runner1c-0.59/runner1c/commands/start.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/commands/start_agent.py` & `runner1c-0.59/runner1c/commands/start_agent.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/commands/sync.py` & `runner1c-0.59/runner1c/commands/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                     p_dump_epf = runner1c.command.EmptyParameters(self.arguments)
                     setattr(p_dump_epf, 'connection', self.arguments.connection)
                     setattr(p_dump_epf, 'folder', os.path.dirname(path_source))
                     setattr(p_dump_epf, 'file', path_binary)
                     setattr(p_dump_epf, 'access', self.arguments.access)
                     setattr(p_dump_epf, 'login', self.arguments.login)
                     setattr(p_dump_epf, 'password', self.arguments.password)
-                    return_code = runner1c.commands.dump_epf.DumpEpf(arguments=p_dump_epf).execute()
+                    return_code = runner1c.commands.dump_epf.DumpEpf(arguments=p_dump_epf, parent=self).execute()
                     if not runner1c.exit_code.success_result(return_code):
                         error_in_loop = True
                         break
 
         if error_in_loop:
             result_code = runner1c.exit_code.EXIT_CODE.error
```

### Comparing `runner1c-0.58/runner1c/commands/webinst.py` & `runner1c-0.59/runner1c/commands/webinst.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/common.py` & `runner1c-0.59/runner1c/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import logging
 import os
 import shutil
+import sys
 import tempfile
 from functools import partial
 
 get_path_to_project = partial(os.path.join, os.path.dirname(os.path.abspath(os.path.dirname(__file__))))
 get_path_to_script = partial(os.path.join, os.path.abspath(os.path.dirname(__file__)))
 MAXIMUM_BYTES_READ = 99999999
 
@@ -89,9 +91,23 @@
     with open(new_file, mode='bw') as new_file_stream, open(file_name, mode='br') as old_file_stream:
         new_file_stream.write(old_file_stream.read().decode('cp1251').encode('utf-8'))
     new_file_stream.close()
     old_file_stream.close()
     shutil.move(new_file, file_name)
 
 
-def get_formatter_string():
-    return '%(asctime)s - %(levelname)s - %(name)19s (%(process)5d) - %(message)s'
+def get_logger(name, debug, handlers = None):
+    logger_handlers = []
+    if handlers is None:
+        logger_handlers.append(logging.StreamHandler(sys.stdout))
+    else:
+        logger_handlers = handlers
+    logger = logging.getLogger(name)
+    if debug:
+        logger.setLevel(logging.DEBUG)
+    for element in logger_handlers:
+        if debug:
+            element.setLevel(logging.DEBUG)
+        element.setFormatter(logging.Formatter('%(asctime)s - %(levelname)s - %(name)25s (%(process)5d) - %(message)s'))
+        logger.addHandler(element)
+
+    return logger
```

### Comparing `runner1c-0.58/runner1c/core.py` & `runner1c-0.59/runner1c/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import argparse
 import inspect
-import logging
 import os
 import sys
 
 import runner1c.common as common
 from runner1c.parser import Parser
 
 
@@ -58,25 +57,20 @@
         list_argument = sys.argv[1:]
         logger_name = 'Core'
     else:
         list_argument = arg
         logger_name = 'File'
 
     arguments = parser.parse_args(list_argument)
+    logger = common.get_logger(logger_name, arguments.debug)
 
-    if arguments.debug:
-        logging.basicConfig(level=logging.DEBUG, format=common.get_formatter_string())
-
-    logger = logging.getLogger(logger_name)
     logger.debug('start')
-
     handler = commands[arguments.command].create_handler(arguments=arguments)
     _check_override_methods(handler)
     return_code = handler.execute()
-
     logger.debug('exit code = %s', return_code)
 
     return return_code
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `runner1c-0.58/runner1c/parser.py` & `runner1c-0.59/runner1c/parser.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tests/test_diff_mxl.py` & `runner1c-0.59/runner1c/tests/test_diff_mxl.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,16 +7,15 @@
     with open(file, mode='r', encoding='utf-8') as file_stream:
         count = len(file_stream.readlines())
     file_stream.close()
 
     return count
 
 
-@pytest.mark.usefixtures("set_log_level")
 def test_diff_same_mxl(runner, tmpdir, repo_folder):
     first = os.path.join(repo_folder, 'Test.mxl')
     second = first
     result = str(tmpdir.join("result.txt"))
-    argument = ['--debug', 'diff_mxl', '--first', first, '--second', second, '--equal_files', result]
+    argument = ['diff_mxl', '--first', first, '--second', second, '--equal_files', result]
     assert runner(argument) == 0
 
     assert count_lines_in_file(result) == 1
```

### Comparing `runner1c-0.58/runner1c/tests/test_sync_without_base.py` & `runner1c-0.59/runner1c/tests/test_sync_without_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import os
 
 import pytest
 
 
-@pytest.mark.usefixtures("set_log_level")
 def test_sync_without_base(runner):
     test_dir = os.path.dirname(__file__)
     repo_folder = os.path.join(test_dir, 'repo')
 
     epf = os.path.join(repo_folder, 'build', 'epf', 'CheckConfig.epf')
     if os.path.exists(epf):
         os.remove(epf)
     # обработки нет
     assert not os.path.exists(epf)
 
-    argument = ['--debug',
-                'sync',
+    argument = ['sync',
                 '--folder',
                 repo_folder,
                 '--create']
     assert runner(argument) == 0
 
     # обработка создалась
     assert os.path.exists(epf)
```

### Comparing `runner1c-0.58/runner1c/tests/test_version.py` & `runner1c-0.59/runner1c/tests/test_version.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,31 +11,29 @@
                             stdout=subprocess.PIPE,
                             stderr=subprocess.PIPE,
                             )
     out, err = proc.communicate()
     return out, err, proc.returncode
 
 
-@pytest.mark.usefixtures("set_log_level")
 def test_version_main(capsys, runner):
-    argument = ['--debug', 'version']
+    argument = ['version']
     assert runner(argument) == 0
 
     captured = capsys.readouterr()
     assert captured.out == runner1c.__version__ + '\n'
 
 
 def test_version_cli():
     command = ["runner1c", "version"]
     out, err, exitcode = capture(command)
     assert exitcode == 0
     assert out.decode() == runner1c.__version__ + '\r\n'
 
 
-@pytest.mark.usefixtures("set_log_level")
 def test_version_file(capsys, runner, repo_folder):
     file = os.path.join(repo_folder, 'file.json')
-    argument = ['--debug', 'file', '--params', file]
+    argument = ['file', '--params', file]
     assert runner(argument) == 0
 
     captured = capsys.readouterr()
     assert captured.out == runner1c.__version__ + '\n'
```

### Comparing `runner1c-0.58/runner1c/tests/test_with_base.py` & `runner1c-0.59/runner1c/tests/test_with_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,141 +18,128 @@
         count = len(file_stream.readlines())
     file_stream.close()
 
     return count
 
 
 @pytest.mark.dependency()
-@pytest.mark.usefixtures("set_log_level")
 def test_base_for_test(tmpdir, runner, base_dir):
     test_dir = os.path.dirname(__file__)
     repo_folder = os.path.join(test_dir, 'repo')
     epf = os.path.join(repo_folder, 'build', 'epf', 'CheckConfig.epf')
     result = str(tmpdir.join("result.txt"))
 
-    argument = ['--debug',
-                'base_for_test',
+    argument = ['base_for_test',
                 '--connection',
                 'File={}'.format(base_dir),
                 '--folder',
                 repo_folder,
                 '--create_epf']
     assert runner(argument) == 0
 
     # обработка создалась
     assert os.path.exists(epf)
 
     # проверка базы
-    argument = ['--debug',
-                'start',
+    argument = ['start',
                 '--connection',
                 'File={}'.format(base_dir),
                 '--result',
                 result,
                 '--epf',
                 epf,
                 '--option',
                 result]
     assert runner(argument) == 0
 
 
 @pytest.mark.dependency(depends=["test_base_for_test"])
-@pytest.mark.usefixtures("set_log_level")
 def test_sync(tmpdir, runner, repo_folder):
     new_repo = str(tmpdir.join("repo"))
     old_build = os.path.join(repo_folder, 'build')
     new_build = os.path.join(new_repo, 'build')
     copy_tree.copy_tree(old_build, new_build)
 
-    argument = ['--debug',
-                'sync',
+    argument = ['sync',
                 '--folder',
                 new_repo]
     assert runner(argument) == 0
 
     assert os.path.exists(os.path.join(repo_folder, 'epf', 'CheckConfig.xml'))
     assert os.path.exists(os.path.join(repo_folder, 'feature', 'Example.data'))
 
 
 @pytest.mark.dependency(depends=["test_base_for_test"])
-@pytest.mark.usefixtures("set_log_level")
 def test_platform_check_skip_modality(tmpdir, runner, base_dir):
     skip_file = str(tmpdir.join("skip.txt"))
     with open(skip_file, mode='w', encoding='utf-8') as file:
         file.write('Справочник.Catalog1.Форма.Form.Форма')
     file.close()
 
     log = str(tmpdir.join("log.html"))
-    argument = ['--debug',
-                'platform_check',
+    argument = ['platform_check',
                 '--connection',
                 'File={}'.format(base_dir),
                 '--log',
                 log,
                 '--options',
                 '"{}"'.format(options_for_platform_check()),
                 '--skip_modality',
                 skip_file]
     assert runner(argument) == 0
     assert count_lines_in_file(log) == 0
 
 
 @pytest.mark.dependency(depends=["test_base_for_test"])
-@pytest.mark.usefixtures("set_log_level")
 def test_platform_check_skip_object(tmpdir, runner, base_dir):
     skip_file = str(tmpdir.join("skip.txt"))
     with open(skip_file, mode='w', encoding='utf-8') as file:
         file.write('Справочник.Catalog1')
     file.close()
 
     log = str(tmpdir.join("log.html"))
-    argument = ['--debug',
-                'platform_check',
+    argument = ['platform_check',
                 '--connection',
                 'File={}'.format(base_dir),
                 '--log',
                 log,
                 '--options',
                 '"{}"'.format(options_for_platform_check()),
                 '--skip_object',
                 skip_file]
     assert runner(argument) == 0
     assert count_lines_in_file(log) == 0
 
 
 @pytest.mark.dependency(depends=["test_base_for_test"])
-@pytest.mark.usefixtures("set_log_level")
 def test_platform_check_skip_error(tmpdir, runner, base_dir):
     skip_file = str(tmpdir.join("skip.txt"))
     with open(skip_file, mode='w', encoding='utf-8') as file:
         file.write('Справочник.Catalog1.Форма.Form.Форма '
                    'Использование модального вызова: "Предупреждение"\n')
     file.close()
 
     log = str(tmpdir.join("log.html"))
-    argument = ['--debug',
-                'platform_check',
+    argument = ['platform_check',
                 '--connection',
                 'File={}'.format(base_dir),
                 '--log',
                 log,
                 '--options',
                 '"{}"'.format(options_for_platform_check()),
                 '--skip_error',
                 skip_file]
     assert runner(argument) == 0
     assert count_lines_in_file(log) == 0
 
 
 @pytest.mark.dependency(depends=["test_base_for_test"])
-@pytest.mark.usefixtures("set_log_level")
 def test_platform_dump_config(tmpdir, runner, base_dir):
     folder = str(tmpdir.join("cf"))
-    argument = ['--debug',
-                'dump_config',
+    argument = ['dump_config',
                 '--connection',
                 'File={}'.format(base_dir),
                 '--folder',
                 folder]
 
     assert runner(argument) == 0
```

### Comparing `runner1c-0.58/runner1c/tools/create_base_for_test.py` & `runner1c-0.59/runner1c/tools/create_base_for_test.py`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form/Module.bsl` & `runner1c-0.59/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form/Module.bsl`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form.xml` & `runner1c-0.59/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form/Ext/Form.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form.xml` & `runner1c-0.59/runner1c/tools/epf/ChangeSafeModeForExtension/Forms/Form.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/ChangeSafeModeForExtension.xml` & `runner1c-0.59/runner1c/tools/epf/ChangeSafeModeForExtension.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Ext/ObjectModule.bsl` & `runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Ext/ObjectModule.bsl`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form/Module.bsl` & `runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form/Module.bsl`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form.xml` & `runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed/Ext/Form.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed.xml` & `runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Managed.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form/Module.bsl` & `runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form/Module.bsl`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form.bin` & `runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary/Ext/Form.bin`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary.xml` & `runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate/Forms/Ordinary.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/CloseAfterUpdate.xml` & `runner1c-0.59/runner1c/tools/epf/CloseAfterUpdate.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form/Module.bsl` & `runner1c-0.59/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form/Module.bsl`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form.bin` & `runner1c-0.59/runner1c/tools/epf/FileCompareMxl/Forms/Form/Ext/Form.bin`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/FileCompareMxl/Forms/Form.xml` & `runner1c-0.59/runner1c/tools/epf/FileCompareMxl/Forms/Form.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/FileCompareMxl.xml` & `runner1c-0.59/runner1c/tools/epf/FileCompareMxl.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form/Module.bsl` & `runner1c-0.59/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form/Module.bsl`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,591 +1,591 @@
-﻿
-// работает в режим совместимости "Версия 8.2.16".
-// отсутствуют все методы на Стр*.
-
-#Область ОписаниеПеременных
-
-&НаКлиенте
-Перем Операции; // Название выполняемой операции.
-
-&НаКлиенте
-Перем ТекстовыйДокумент; // Кэш для показа ошибок.
-
-#КонецОбласти
-
-#Область ОбработчикиСобытий
-
-&НаКлиенте
-Процедура ПриОткрытии(Отказ)
-	
-	ПутьКПлатформе = ПутьКПлатформе();
-	СтрокаПодключенияКБазе = СтрокаСоединенияИнформационнойБазы();
-	Логин = ИмяПользователяНаСервере();
-
-	ЗаполнитьСписокВыбораТипаОперации();
-	ПрочитатьПутьКРепозиторию();
-	
-	Если ПустаяСтрока(ТипОперации) Тогда
-		ТипОперации = Операции.ПолнаяВыгрузкаCF;
-	КонецЕсли;
-	
-	УстановитьВидимостьЭлементов();
-	ВывестиВерсиюПакета();
-	
-КонецПроцедуры
-
-&НаСервере
-Процедура ОбработкаПроверкиЗаполненияНаСервере(Отказ, ПроверяемыеРеквизиты)
-	
-	Если Не ПустаяСтрока(Логин) Тогда
-		ПроверяемыеРеквизиты.Добавить("Пароль");
-	КонецЕсли;
-	
-КонецПроцедуры
-
-#КонецОбласти
-
-#Область ОбработчикиКомандФормы
-
-&НаКлиенте
-Процедура Сделать(Команда)
-	
-	Если Не ПроверитьЗаполнение() Тогда
-		Возврат;
-	КонецЕсли;
-	
-	Оповещение = Новый ОписаниеОповещения("ВыполнитьОперациюСВопросомЗавершение", ЭтаФорма);
-	
-	Если ТипОперации = Операции.СоздатьEPF Тогда
-		ПоказатьВопрос(Новый ОписаниеОповещения("РезультатВопросаПередОперациейСозданияEpf", ЭтаФорма, Оповещение),
-		               "Будут заново созданы файлы. Продолжить?",
-		               РежимДиалогаВопрос.ДаНет,
-		               60,
-		               КодВозвратаДиалога.Нет,
-		               "Внимание",
-		               КодВозвратаДиалога.Нет);
-	Иначе
-		ВыполнитьОбработкуОповещения(Оповещение, Истина);
-	КонецЕсли;
-	
-КонецПроцедуры
-
-#КонецОбласти
-
-#Область ОбработчикиСобытийЭлементовШапкиФормы
-
-&НаКлиенте
-Процедура ПутьКПлатформеНачалоВыбора(Элемент, ДанныеВыбора, СтандартнаяОбработка)
-	НачалоВыбораФайла(Элемент, СтандартнаяОбработка);
-КонецПроцедуры
-
-&НаКлиенте
-Процедура ПапкаВыгрузкиНачалоВыбора(Элемент, ДанныеВыбора, СтандартнаяОбработка)
-	НачалоВыбораФайла(Элемент, СтандартнаяОбработка);
-КонецПроцедуры
-
-&НаКлиенте
-Процедура ТипОперацииПриИзменении(Элемент)
-	УстановитьВидимостьЭлементов();
-КонецПроцедуры
-
-#КонецОбласти
-
-#Область СлужебныйПрограммныйИнтерфейс
-
-&НаКлиенте
-Процедура УстановитьПапкуВыгрузкиПоПутиВФайле(Знач Существует, Знач ДополнительныеПараметры) Экспорт
-	
-	Если Не Существует Тогда
-		Возврат;
-	КонецЕсли;
-	
-	ЧтениеJSON = Новый ЧтениеJSON();
-	ЧтениеJSON.ОткрытьФайл(ДополнительныеПараметры.ИмяФайла);
-	ПараметрыИзФайла = ПрочитатьJSON(ЧтениеJSON);
-	ЧтениеJSON.Закрыть();
-	
-	ПапкаВыгрузки = ПараметрыИзФайла.repo;
-	
-КонецПроцедуры
-
-&НаКлиенте
-Процедура УстановитьВыбранныйПуть(Знач ВыбранныеФайлы, Знач ДополнительныеПараметры) Экспорт
-	
-	Если ВыбранныеФайлы = Неопределено Тогда
-		Возврат;
-	КонецЕсли;
-	
-	ЭтаФорма[ДополнительныеПараметры.ИмяЭлемента] = ВыбранныеФайлы[0];
-	
-КонецПроцедуры
-
-&НаКлиенте
-Процедура РезультатВопросаПередОперациейСозданияEpf(Знач РезультатВопроса, Знач ДополнительныеПараметры) Экспорт
-	ВыполнитьОбработкуОповещения(ДополнительныеПараметры, РезультатВопроса = КодВозвратаДиалога.Да);
-КонецПроцедуры
-
-&НаКлиенте
-Процедура ВыполнитьОперациюСВопросомЗавершение(Знач Результат, Знач ДополнительныеПараметры) Экспорт
-	
-	Если Не Результат Тогда
-		Возврат;
-	КонецЕсли;
-	
-	Для Каждого Этап Из ПолучитьЭтапы(ТипОперации) Цикл
-		ПараметрыКоманднойСтроки = РеквизитыФормыВСтруктуру();
-		ПараметрыКоманднойСтроки.Вставить("Команда", Этап.Команда);
-		ЗапуститьКоманду(Этап.СтрокаДляЗапуска, ПараметрыКоманднойСтроки);
-	КонецЦикла;
-	
-КонецПроцедуры
-
-&НаКлиенте
-Процедура ЧтениеЛогаЗавершение(Знач ДополнительныеПараметры) Экспорт
-	ТекстовыйДокумент.Показать("Ошибка при выполнении операции");
-	НачатьУдалениеФайлов(Неопределено, ДополнительныеПараметры.Лог);
-КонецПроцедуры
-
-&НаКлиенте
-Процедура ЗапуститьКомандуЗавершение(Знач КодВозврата, Знач ДополнительныеПараметры) Экспорт
-	
-	Если КодВозврата = 0 Тогда
-		Возврат;
-	КонецЕсли;
-	
-	Файл = Новый Файл(ДополнительныеПараметры.Лог);
-	Файл.НачатьПроверкуСуществования(Новый ОписаниеОповещения("ПроверкаСуществованияЛога",
-	                                                          ЭтаФорма,
-	                                                          ДополнительныеПараметры));
-	
-КонецПроцедуры
-
-&НаКлиенте
-Процедура ПроверкаСуществованияЛога(Знач Существует, Знач ДополнительныеПараметры) Экспорт
-	
-	Если Не Существует Тогда
-		ПоказатьПредупреждение( , "Команда не выполнилась. Лог не найден");
-		Возврат;
-	КонецЕсли;
-	
-	ТекстовыйДокумент = Новый ТекстовыйДокумент;
-	ТекстовыйДокумент.НачатьЧтение(Новый ОписаниеОповещения("ЧтениеЛогаЗавершение",
-	                                                        ЭтаФорма,
-	                                                        Новый Структура("Лог", ДополнительныеПараметры.Лог)),
-	                               ДополнительныеПараметры.Лог,
-	                               КодировкаТекста.UTF8);
-	
-КонецПроцедуры
-
-#КонецОбласти
-
-#Область СлужебныеПроцедурыИФункции
-
-&НаКлиенте
-Функция ПутьКПлатформе()
-	// для linux нужно по другому
-	Возврат СтрЗаменить(КаталогПрограммы(), "\bin\", "");
-КонецФункции
-
-&НаКлиенте
-Процедура ЗапуститьКоманду(Знач СтрокаДляЗапуска, Знач ПараметрыКоманднойСтроки)
-	
-	Команда = ПодставитьПараметрыВСтроку(СтрокаЗапускаСкрипта(Истина, Отладка) + " " + СтрокаДляЗапуска, ПараметрыКоманднойСтроки);
-	
-	Если Отладка Тогда
-		Сообщение(Команда);
-	Иначе
-		Описание = Новый ОписаниеОповещения("ЗапуститьКомандуЗавершение",
-											ЭтаФорма,
-											Новый Структура("Лог", ПараметрыКоманднойСтроки.Лог));
-		НачатьЗапускПриложения(Описание,
-								Команда,
-								,
-								Истина);
-	КонецЕсли;
-	
-КонецПроцедуры
-
-&НаКлиенте
-Функция РеквизитыФормыВСтруктуру()
-	
-	ПапкаВыгрузкиБезСлеша = УбратьСКонцаРазделительПути(ПапкаВыгрузки);
-	ПлатформаБезСлеша = УбратьСКонцаРазделительПути(ПутьКПлатформе);
-	
-	НастройкиВыгрузкиРасширений = Новый Структура("ПапкаВыгрузки, ИмяПапки", ПапкаВыгрузкиБезСлеша, ?(Не ВыгружатьРасширенияВSpec, "lib", "spec"));
-	
-	Структура = Новый Структура;
-	Структура.Вставить("КодРазблокировки",          ?(ПустаяСтрока(КодРазблокировки), "None", КодРазблокировки));
-	Структура.Вставить("Логин",                     Логин);
-	Структура.Вставить("ПапкаВыгрузки",             ПапкаВыгрузкиБезСлеша);
-	Структура.Вставить("ПапкаВыгрузкиКонфигурации", СоединитьПути(ПапкаВыгрузкиБезСлеша, "cf"));
-	Структура.Вставить("ПапкаВыгрузкиРасширений",   ПодставитьПараметрыВСтроку(СоединитьПути("%ПапкаВыгрузки%", "%ИмяПапки%", "ext"), НастройкиВыгрузкиРасширений));
-	Структура.Вставить("Пароль",                    Пароль);
-	Структура.Вставить("ПутьКПлатформе",            ПлатформаБезСлеша);
-	Структура.Вставить("СтрокаПодключенияКБазе",    СтрокаПодключенияКБазе);
-	Структура.Вставить("Лог",                       ПолучитьИмяВременногоФайла("txt"));
-	
-	Возврат Структура;
-	
-КонецФункции
-
-&НаСервереБезКонтекста
-Функция ИмяПользователяНаСервере()
-	Возврат ИмяПользователя();
-КонецФункции
-
-&НаКлиенте
-Процедура ЗаполнитьСписокВыбораТипаОперации()
-	
-	Для Каждого ТипОперции Из Операции Цикл
-		Элементы.ТипОперации.СписокВыбора.Добавить(ТипОперции.Значение);
-	КонецЦикла;
-
-КонецПроцедуры
-
-&НаКлиенте
-Процедура ПрочитатьПутьКРепозиторию()
-	
-	Если Не ИнформационнаяБазаФайловая(СтрокаПодключенияКБазе) Тогда
-		Возврат;
-	КонецЕсли;
-	
-	Структура = ПараметрыИзСтроки(СтрокаПодключенияКБазе);
-	
-	ПутьКФайлуСПараметрамиБазы = СоединитьПути(Структура.File, "parameters.txt");
-	
-	Файл = Новый Файл(ПутьКФайлуСПараметрамиБазы);
-	Файл.НачатьПроверкуСуществования(Новый ОписаниеОповещения("УстановитьПапкуВыгрузкиПоПутиВФайле",
-	                                                          ЭтаФорма,
-	                                                          Новый Структура("ИмяФайла", ПутьКФайлуСПараметрамиБазы)));
-	
-КонецПроцедуры
-
-&НаКлиенте
-Процедура НачалоВыбораФайла(Знач Элемент, СтандартнаяОбработка)
-	
-	СтандартнаяОбработка = Ложь;
-	
-	ДиалогВыбораФайла = Новый ДиалогВыбораФайла(РежимДиалогаВыбораФайла.ВыборКаталога);
-		
-	Если ЗначениеЗаполнено(Элемент.ТекстРедактирования) Тогда
-		
-		Файл = Новый Файл(Элемент.ТекстРедактирования);
-		ДиалогВыбораФайла.Каталог = Файл.Путь;
-		
-	КонецЕсли;
-	
-	ДиалогВыбораФайла.Показать(Новый ОписаниеОповещения("УстановитьВыбранныйПуть",
-	                                                    ЭтаФорма,
-	                                                    Новый Структура("ИмяЭлемента", Элемент.Имя)));
-	
-КонецПроцедуры
-
-&НаСервереБезКонтекста
-Функция КонфигурацияСОшибкамиВыгрузки()
-	
-	Результат = Ложь;
-	
-	Если Метаданные.РегистрыСведений.Найти("ВерсииПодсистем") <> Неопределено 
-		Или (Метаданные.Имя = "УправлениеТорговлей" И Лев(Метаданные.Версия, 4) = "10.3") Тогда
-		Результат = Истина;
-	КонецЕсли;
-	
-	Возврат Результат;
-	
-КонецФункции
-
-&НаКлиенте
-Функция СтрокаЗапускаСкрипта(Знач ТекущаяБаза = Истина, Знач Отладка = Ложь)
-	
-	Если ПодменитьПутьRunner Тогда
-		ВызватьИсключение "Не реализовано";
-	Иначе
-		Шаблон = "runner1c";
-	КонецЕсли;
-	
-	Если Отладка Тогда
-		Шаблон = Шаблон + " --debug";
-	КонецЕсли;
-	Шаблон = Шаблон + " %Команда%";
-	
-	ПараметрыДляДобавления = Новый Массив;
-	
-	Если ТекущаяБаза Тогда
-		
-		ПараметрыДляДобавления.Добавить(" --log ""%Лог%""");
-		ПараметрыДляДобавления.Добавить("silent");
-		ПараметрыДляДобавления.Добавить("path ""%ПутьКПлатформе%""");
-	
-		Если Не ПустаяСтрока(КодРазблокировки) Тогда
-			ПараметрыДляДобавления.Добавить("access %КодРазблокировки%");
-		КонецЕсли;
-		
-		Если Не ПустаяСтрока(Логин) Тогда
-			ПараметрыДляДобавления.Добавить("login ""%Логин%""");
-			ПараметрыДляДобавления.Добавить("password ""%Пароль%""");
-		КонецЕсли;
-		
-		ПараметрыДляДобавления.Добавить("connection ""%СтрокаПодключенияКБазе%""");
-		
-	КонецЕсли;
-	
-	Возврат Шаблон + СобратьСтрокуИзПодстрок(ПараметрыДляДобавления, " --");
-	
-КонецФункции
-
-&НаКлиенте
-Функция ИнформационнаяБазаФайловая(Знач СтрокаСоединенияИнформационнойБазы = "")
-			
-	Если ПустаяСтрока(СтрокаСоединенияИнформационнойБазы) Тогда
-		СтрокаСоединенияИнформационнойБазы =  СтрокаСоединенияИнформационнойБазы();
-	КонецЕсли;
-	Возврат Найти(Врег(СтрокаСоединенияИнформационнойБазы), "FILE=") = 1;
-	
-КонецФункции
-
-&НаКлиенте
-Функция ПараметрыИзСтроки(Знач СтрокаПараметров)
-	
-	Результат = Новый Структура;
-	
-	СимволДвойныеКавычки = Символ(34); // (")
-	
-	МассивПодстрок = РазложитьСтрокуВМассивПодстрок(СтрокаПараметров, ";");
-	
-	Для Каждого СтрокаПараметра Из МассивПодстрок Цикл
-		
-		ПозицияПервогоЗнакаРавенства = Найти(СтрокаПараметра, "=");
-		
-		// Получаем имя параметра
-		ИмяПараметра = СокрЛП(Лев(СтрокаПараметра, ПозицияПервогоЗнакаРавенства - 1));
-		
-		// Получаем значение параметра.
-		ЗначениеПараметра = СокрЛП(Сред(СтрокаПараметра, ПозицияПервогоЗнакаРавенства + 1));
-		
-		Если  Лев(ЗначениеПараметра, 1) = СимволДвойныеКавычки
-			И Прав(ЗначениеПараметра, 1) = СимволДвойныеКавычки Тогда
-			
-			ЗначениеПараметра = Сред(ЗначениеПараметра, 2, СтрДлина(ЗначениеПараметра) - 2);
-			
-		КонецЕсли;
-		
-		Если Не ПустаяСтрока(ИмяПараметра) Тогда
-			
-			Результат.Вставить(ИмяПараметра, ЗначениеПараметра);
-			
-		КонецЕсли;
-		
-	КонецЦикла;
-	
-	Возврат Результат;
-КонецФункции
-
-&НаКлиенте
-Функция ПодставитьПараметрыВСтроку(Шаблон, Знач ПарметрыСтроки)
-	
-	Строка = Шаблон;
-	Для Каждого Элемент Из ПарметрыСтроки Цикл
-		Строка = СтрЗаменить(Строка, "%" + Элемент.Ключ + "%", Элемент.Значение);
-	КонецЦикла;
-		
-	Возврат Строка;
-	
-КонецФункции
-
-&НаКлиентеНаСервереБезКонтекста
-Процедура Сообщение(Знач Текст)
-	
-	СообщениеПользователю = Новый СообщениеПользователю;
-	СообщениеПользователю.Текст = Текст;
-	СообщениеПользователю.Сообщить();
-	
-КонецПроцедуры
-
-&НаКлиенте
-Функция РазложитьСтрокуВМассивПодстрок(Знач Стр, Разделитель = ",")
-	
-	МассивСтрок = Новый Массив();
-	Если Разделитель = " " Тогда
-		Стр = СокрЛП(Стр);
-		Пока Истина Цикл
-			Поз = Найти(Стр, Разделитель);
-			Если Поз = 0 Тогда
-				МассивСтрок.Добавить(Стр);
-				Возврат МассивСтрок;
-			КонецЕсли;
-			МассивСтрок.Добавить(Лев(Стр, Поз - 1));
-			Стр = СокрЛ(Сред(Стр, Поз));
-		КонецЦикла;
-	Иначе
-		ДлинаРазделителя = СтрДлина(Разделитель);
-		Пока Истина Цикл
-			Поз = Найти(Стр, Разделитель);
-			Если Поз = 0 Тогда
-				МассивСтрок.Добавить(Стр);
-				Возврат МассивСтрок;
-			КонецЕсли;
-			МассивСтрок.Добавить(Лев(Стр, Поз - 1));
-			Стр = Сред(Стр, Поз + ДлинаРазделителя);
-		КонецЦикла;
-	КонецЕсли;
-	
-КонецФункции
-
-&НаКлиенте
-Функция СобратьСтрокуИзПодстрок(Знач Строки, Знач Разделитель)
-	
-	Результат = "";
-	
-	Для Каждого Строка Из Строки Цикл
-		Результат = Результат + ?(ПустаяСтрока(Результат), "", Разделитель) + Строка;
-	КонецЦикла;
-	
-	Возврат Результат;
-	
-КонецФункции
-
-&НаКлиенте
-Процедура УстановитьВидимостьЭлементов()
-	Элементы.ВыгружатьРасширенияВSpec.Видимость = (ТипОперации = Операции.ВыгрузкаCFE);
-КонецПроцедуры
-
-&НаСервере
-Функция ИмяФайлаОбработки()
-	Возврат РеквизитФормыВЗначение("Объект").ИспользуемоеИмяФайла;
-КонецФункции
-
-&НаКлиенте
-Процедура ВывестиВерсиюПакета()
-	
-	ЧтениеТекста = Новый ЧтениеТекста(ПутьДоRunner() + РазделительПути() + "__init__.py");
-	СтрокаВерсии = ЧтениеТекста.ПрочитатьСтроку();
-	ЧтениеТекста.Закрыть();
-	
-	ПараметрыВерсии = РазложитьСтрокуВМассивПодстрок(СтрокаВерсии, "=");
-	Версия = СокрЛП(ПараметрыВерсии[1]);
-	
-	Заголовок = Версия;
-	
-КонецПроцедуры
-
-&НаКлиенте
-Функция РазделительПути()
-	Возврат "\";
-КонецФункции
-
-&НаКлиенте
-Функция СоединитьПути(Знач ПутьКаталога, Знач Элемент1, Знач Элемент2 = "")
-	
-	Массив = Новый Массив;
-	Массив.Добавить(ПутьКаталога);
-	Массив.Добавить(Элемент1);
-	Если Не ПустаяСтрока(Элемент2) Тогда
-		Массив.Добавить(Элемент2);
-	КонецЕсли;
-	
-	Возврат СобратьСтрокуИзПодстрок(Массив, РазделительПути());
-	
-КонецФункции
-
-&НаКлиенте
-Функция УбратьСКонцаРазделительПути(Знач Путь)
-	
-	Результат = Путь;
-	Если Прав(Путь, 1) = РазделительПути() Тогда
-		Результат = Лев(Результат, СтрДлина(Результат) - 1);
-	КонецЕсли;
-	
-	Возврат Результат;
-	
-КонецФункции
-
-&НаКлиенте
-Функция ПолучитьЭтапы(Знач ВыбраннаяОперация)
-	
-	Массив = Новый Массив();
-	
-	СтрокаДляЗапуска = "";
-	
-	Если ВыбраннаяОперация = Операции.ПолнаяВыгрузкаCF Или ВыбраннаяОперация = Операции.ЧастичнаяВыгрузкаCF Тогда
-		
-		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузкиКонфигурации%""";
-		Если КонфигурацияСОшибкамиВыгрузки() Тогда
-			СтрокаДляЗапуска = СтрокаДляЗапуска + " --repair";
-		КонецЕсли;
-		Если ВыбраннаяОперация = Операции.ЧастичнаяВыгрузкаCF Тогда
-			СтрокаДляЗапуска = СтрокаДляЗапуска + " --update";
-		КонецЕсли;
-		
-		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "dump_config"));
-		
-	ИначеЕсли ВыбраннаяОперация = Операции.ВыгрузкаCFE Тогда
-		
-		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузкиРасширений%""";
-		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "dump_extensions"));
-		
-	ИначеЕсли ВыбраннаяОперация = Операции.ПолнаяВыгрузкаEPF Или ВыбраннаяОперация = Операции.ЧастичнаяВыгрузкаEPF Тогда
-		
-		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузки%""";
-		Если ВыбраннаяОперация = Операции.ПолнаяВыгрузкаEPF Тогда
-			СтрокаДляЗапуска = СтрокаДляЗапуска + " --clear_hash";
-		КонецЕсли;
-		
-		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "sync"));
-		
-	ИначеЕсли ВыбраннаяОперация = Операции.СоздатьEPF Тогда
-		
-		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузки%"" --create";
-		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "sync"));
-		
-	ИначеЕсли ВыбраннаяОперация = Операции.ЗагрузитьCF Тогда
-		
-		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузкиКонфигурации%""";
-		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "load_config"));
-		
-		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузкиРасширений%""";
-		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "load_extension"));
-		
-	Иначе
-		ВызватьИсключение "операция не определена";
-	КонецЕсли;
-	
-	Возврат Массив;
-	
-КонецФункции
-
-&НаКлиенте
-Функция ПутьДоRunner()
-	
-	Разделитель = РазделительПути();
-	
-	ПутьОбработки = РазложитьСтрокуВМассивПодстрок(ИмяФайлаОбработки(), Разделитель);
-	ПутьОбработки.Удалить(ПутьОбработки.Количество() - 1);
-	ПутьОбработки.Удалить(ПутьОбработки.Количество() - 1);
-	ПутьОбработки.Удалить(ПутьОбработки.Количество() - 1);
-	ПутьОбработки.Удалить(ПутьОбработки.Количество() - 1);
-	
-	ПутьВерсии = СобратьСтрокуИзПодстрок(ПутьОбработки, Разделитель);
-	
-	Возврат ПутьВерсии;
-	
-КонецФункции
-
-&НаКлиенте
-Функция СоздатьЭтап(Знач СтрокаДляЗапуска, Знач Команда)
-	Возврат Новый Структура("СтрокаДляЗапуска, Команда", СтрокаДляЗапуска, Команда);
-КонецФункции
-
-#КонецОбласти
-
-#Область Инициализация
-
-Операции = Новый Структура;
-Операции.Вставить("ПолнаяВыгрузкаCF", "CF Полная Выгрузка");
-Операции.Вставить("ЧастичнаяВыгрузкаCF", "CF Частичная Выгрузка");
-Операции.Вставить("ПолнаяВыгрузкаEPF", "EPF Полная Выгрузка");
-Операции.Вставить("ЧастичнаяВыгрузкаEPF", "EPF Частичная Выгрузка");
-Операции.Вставить("СоздатьEPF", "EPF Создать");
-Операции.Вставить("ВыгрузкаCFE", "CFE Выгрузка");
-Операции.Вставить("ЗагрузитьCF", "Загрузить конфигурацию");
-
-#КонецОбласти
+﻿
+// работает в режим совместимости "Версия 8.2.16".
+// отсутствуют все методы на Стр*.
+
+#Область ОписаниеПеременных
+
+&НаКлиенте
+Перем Операции; // Название выполняемой операции.
+
+&НаКлиенте
+Перем ТекстовыйДокумент; // Кэш для показа ошибок.
+
+#КонецОбласти
+
+#Область ОбработчикиСобытий
+
+&НаКлиенте
+Процедура ПриОткрытии(Отказ)
+	
+	ПутьКПлатформе = ПутьКПлатформе();
+	СтрокаПодключенияКБазе = СтрокаСоединенияИнформационнойБазы();
+	Логин = ИмяПользователяНаСервере();
+
+	ЗаполнитьСписокВыбораТипаОперации();
+	ПрочитатьПутьКРепозиторию();
+	
+	Если ПустаяСтрока(ТипОперации) Тогда
+		ТипОперации = Операции.ПолнаяВыгрузкаCF;
+	КонецЕсли;
+	
+	УстановитьВидимостьЭлементов();
+	ВывестиВерсиюПакета();
+	
+КонецПроцедуры
+
+&НаСервере
+Процедура ОбработкаПроверкиЗаполненияНаСервере(Отказ, ПроверяемыеРеквизиты)
+	
+	Если Не ПустаяСтрока(Логин) Тогда
+		ПроверяемыеРеквизиты.Добавить("Пароль");
+	КонецЕсли;
+	
+КонецПроцедуры
+
+#КонецОбласти
+
+#Область ОбработчикиКомандФормы
+
+&НаКлиенте
+Процедура Сделать(Команда)
+	
+	Если Не ПроверитьЗаполнение() Тогда
+		Возврат;
+	КонецЕсли;
+	
+	Оповещение = Новый ОписаниеОповещения("ВыполнитьОперациюСВопросомЗавершение", ЭтаФорма);
+	
+	Если ТипОперации = Операции.СоздатьEPF Тогда
+		ПоказатьВопрос(Новый ОписаниеОповещения("РезультатВопросаПередОперациейСозданияEpf", ЭтаФорма, Оповещение),
+		               "Будут заново созданы файлы. Продолжить?",
+		               РежимДиалогаВопрос.ДаНет,
+		               60,
+		               КодВозвратаДиалога.Нет,
+		               "Внимание",
+		               КодВозвратаДиалога.Нет);
+	Иначе
+		ВыполнитьОбработкуОповещения(Оповещение, Истина);
+	КонецЕсли;
+	
+КонецПроцедуры
+
+#КонецОбласти
+
+#Область ОбработчикиСобытийЭлементовШапкиФормы
+
+&НаКлиенте
+Процедура ПутьКПлатформеНачалоВыбора(Элемент, ДанныеВыбора, СтандартнаяОбработка)
+	НачалоВыбораФайла(Элемент, СтандартнаяОбработка);
+КонецПроцедуры
+
+&НаКлиенте
+Процедура ПапкаВыгрузкиНачалоВыбора(Элемент, ДанныеВыбора, СтандартнаяОбработка)
+	НачалоВыбораФайла(Элемент, СтандартнаяОбработка);
+КонецПроцедуры
+
+&НаКлиенте
+Процедура ТипОперацииПриИзменении(Элемент)
+	УстановитьВидимостьЭлементов();
+КонецПроцедуры
+
+#КонецОбласти
+
+#Область СлужебныйПрограммныйИнтерфейс
+
+&НаКлиенте
+Процедура УстановитьПапкуВыгрузкиПоПутиВФайле(Знач Существует, Знач ДополнительныеПараметры) Экспорт
+	
+	Если Не Существует Тогда
+		Возврат;
+	КонецЕсли;
+	
+	ЧтениеJSON = Новый ЧтениеJSON();
+	ЧтениеJSON.ОткрытьФайл(ДополнительныеПараметры.ИмяФайла);
+	ПараметрыИзФайла = ПрочитатьJSON(ЧтениеJSON);
+	ЧтениеJSON.Закрыть();
+	
+	ПапкаВыгрузки = ПараметрыИзФайла.repo;
+	
+КонецПроцедуры
+
+&НаКлиенте
+Процедура УстановитьВыбранныйПуть(Знач ВыбранныеФайлы, Знач ДополнительныеПараметры) Экспорт
+	
+	Если ВыбранныеФайлы = Неопределено Тогда
+		Возврат;
+	КонецЕсли;
+	
+	ЭтаФорма[ДополнительныеПараметры.ИмяЭлемента] = ВыбранныеФайлы[0];
+	
+КонецПроцедуры
+
+&НаКлиенте
+Процедура РезультатВопросаПередОперациейСозданияEpf(Знач РезультатВопроса, Знач ДополнительныеПараметры) Экспорт
+	ВыполнитьОбработкуОповещения(ДополнительныеПараметры, РезультатВопроса = КодВозвратаДиалога.Да);
+КонецПроцедуры
+
+&НаКлиенте
+Процедура ВыполнитьОперациюСВопросомЗавершение(Знач Результат, Знач ДополнительныеПараметры) Экспорт
+	
+	Если Не Результат Тогда
+		Возврат;
+	КонецЕсли;
+	
+	Для Каждого Этап Из ПолучитьЭтапы(ТипОперации) Цикл
+		ПараметрыКоманднойСтроки = РеквизитыФормыВСтруктуру();
+		ПараметрыКоманднойСтроки.Вставить("Команда", Этап.Команда);
+		ЗапуститьКоманду(Этап.СтрокаДляЗапуска, ПараметрыКоманднойСтроки);
+	КонецЦикла;
+	
+КонецПроцедуры
+
+&НаКлиенте
+Процедура ЧтениеЛогаЗавершение(Знач ДополнительныеПараметры) Экспорт
+	ТекстовыйДокумент.Показать("Ошибка при выполнении операции");
+	НачатьУдалениеФайлов(Неопределено, ДополнительныеПараметры.Лог);
+КонецПроцедуры
+
+&НаКлиенте
+Процедура ЗапуститьКомандуЗавершение(Знач КодВозврата, Знач ДополнительныеПараметры) Экспорт
+	
+	Если КодВозврата = 0 Тогда
+		Возврат;
+	КонецЕсли;
+	
+	Файл = Новый Файл(ДополнительныеПараметры.Лог);
+	Файл.НачатьПроверкуСуществования(Новый ОписаниеОповещения("ПроверкаСуществованияЛога",
+	                                                          ЭтаФорма,
+	                                                          ДополнительныеПараметры));
+	
+КонецПроцедуры
+
+&НаКлиенте
+Процедура ПроверкаСуществованияЛога(Знач Существует, Знач ДополнительныеПараметры) Экспорт
+	
+	Если Не Существует Тогда
+		ПоказатьПредупреждение( , "Команда не выполнилась. Лог не найден");
+		Возврат;
+	КонецЕсли;
+	
+	ТекстовыйДокумент = Новый ТекстовыйДокумент;
+	ТекстовыйДокумент.НачатьЧтение(Новый ОписаниеОповещения("ЧтениеЛогаЗавершение",
+	                                                        ЭтаФорма,
+	                                                        Новый Структура("Лог", ДополнительныеПараметры.Лог)),
+	                               ДополнительныеПараметры.Лог,
+	                               КодировкаТекста.UTF8);
+	
+КонецПроцедуры
+
+#КонецОбласти
+
+#Область СлужебныеПроцедурыИФункции
+
+&НаКлиенте
+Функция ПутьКПлатформе()
+	// для linux нужно по другому
+	Возврат СтрЗаменить(КаталогПрограммы(), "\bin\", "");
+КонецФункции
+
+&НаКлиенте
+Процедура ЗапуститьКоманду(Знач СтрокаДляЗапуска, Знач ПараметрыКоманднойСтроки)
+	
+	Команда = ПодставитьПараметрыВСтроку(СтрокаЗапускаСкрипта(Истина, Отладка) + " " + СтрокаДляЗапуска, ПараметрыКоманднойСтроки);
+	
+	Если Отладка Тогда
+		Сообщение(Команда);
+	Иначе
+		Описание = Новый ОписаниеОповещения("ЗапуститьКомандуЗавершение",
+											ЭтаФорма,
+											Новый Структура("Лог", ПараметрыКоманднойСтроки.Лог));
+		НачатьЗапускПриложения(Описание,
+								Команда,
+								,
+								Истина);
+	КонецЕсли;
+	
+КонецПроцедуры
+
+&НаКлиенте
+Функция РеквизитыФормыВСтруктуру()
+	
+	ПапкаВыгрузкиБезСлеша = УбратьСКонцаРазделительПути(ПапкаВыгрузки);
+	ПлатформаБезСлеша = УбратьСКонцаРазделительПути(ПутьКПлатформе);
+	
+	НастройкиВыгрузкиРасширений = Новый Структура("ПапкаВыгрузки, ИмяПапки", ПапкаВыгрузкиБезСлеша, ?(Не ВыгружатьРасширенияВSpec, "lib", "spec"));
+	
+	Структура = Новый Структура;
+	Структура.Вставить("КодРазблокировки",          ?(ПустаяСтрока(КодРазблокировки), "None", КодРазблокировки));
+	Структура.Вставить("Логин",                     Логин);
+	Структура.Вставить("ПапкаВыгрузки",             ПапкаВыгрузкиБезСлеша);
+	Структура.Вставить("ПапкаВыгрузкиКонфигурации", СоединитьПути(ПапкаВыгрузкиБезСлеша, "cf"));
+	Структура.Вставить("ПапкаВыгрузкиРасширений",   ПодставитьПараметрыВСтроку(СоединитьПути("%ПапкаВыгрузки%", "%ИмяПапки%", "ext"), НастройкиВыгрузкиРасширений));
+	Структура.Вставить("Пароль",                    Пароль);
+	Структура.Вставить("ПутьКПлатформе",            ПлатформаБезСлеша);
+	Структура.Вставить("СтрокаПодключенияКБазе",    СтрокаПодключенияКБазе);
+	Структура.Вставить("Лог",                       ПолучитьИмяВременногоФайла("txt"));
+	
+	Возврат Структура;
+	
+КонецФункции
+
+&НаСервереБезКонтекста
+Функция ИмяПользователяНаСервере()
+	Возврат ИмяПользователя();
+КонецФункции
+
+&НаКлиенте
+Процедура ЗаполнитьСписокВыбораТипаОперации()
+	
+	Для Каждого ТипОперции Из Операции Цикл
+		Элементы.ТипОперации.СписокВыбора.Добавить(ТипОперции.Значение);
+	КонецЦикла;
+
+КонецПроцедуры
+
+&НаКлиенте
+Процедура ПрочитатьПутьКРепозиторию()
+	
+	Если Не ИнформационнаяБазаФайловая(СтрокаПодключенияКБазе) Тогда
+		Возврат;
+	КонецЕсли;
+	
+	Структура = ПараметрыИзСтроки(СтрокаПодключенияКБазе);
+	
+	ПутьКФайлуСПараметрамиБазы = СоединитьПути(Структура.File, "parameters.txt");
+	
+	Файл = Новый Файл(ПутьКФайлуСПараметрамиБазы);
+	Файл.НачатьПроверкуСуществования(Новый ОписаниеОповещения("УстановитьПапкуВыгрузкиПоПутиВФайле",
+	                                                          ЭтаФорма,
+	                                                          Новый Структура("ИмяФайла", ПутьКФайлуСПараметрамиБазы)));
+	
+КонецПроцедуры
+
+&НаКлиенте
+Процедура НачалоВыбораФайла(Знач Элемент, СтандартнаяОбработка)
+	
+	СтандартнаяОбработка = Ложь;
+	
+	ДиалогВыбораФайла = Новый ДиалогВыбораФайла(РежимДиалогаВыбораФайла.ВыборКаталога);
+		
+	Если ЗначениеЗаполнено(Элемент.ТекстРедактирования) Тогда
+		
+		Файл = Новый Файл(Элемент.ТекстРедактирования);
+		ДиалогВыбораФайла.Каталог = Файл.Путь;
+		
+	КонецЕсли;
+	
+	ДиалогВыбораФайла.Показать(Новый ОписаниеОповещения("УстановитьВыбранныйПуть",
+	                                                    ЭтаФорма,
+	                                                    Новый Структура("ИмяЭлемента", Элемент.Имя)));
+	
+КонецПроцедуры
+
+&НаСервереБезКонтекста
+Функция КонфигурацияСОшибкамиВыгрузки()
+	
+	Результат = Ложь;
+	
+	Если Метаданные.РегистрыСведений.Найти("ВерсииПодсистем") <> Неопределено 
+		Или (Метаданные.Имя = "УправлениеТорговлей" И Лев(Метаданные.Версия, 4) = "10.3") Тогда
+		Результат = Истина;
+	КонецЕсли;
+	
+	Возврат Результат;
+	
+КонецФункции
+
+&НаКлиенте
+Функция СтрокаЗапускаСкрипта(Знач ТекущаяБаза = Истина, Знач Отладка = Ложь)
+	
+	Если ПодменитьПутьRunner Тогда
+		ВызватьИсключение "Не реализовано";
+	Иначе
+		Шаблон = "runner1c";
+	КонецЕсли;
+	
+	Если Отладка Тогда
+		Шаблон = Шаблон + " --debug";
+	КонецЕсли;
+	Шаблон = Шаблон + " %Команда%";
+	
+	ПараметрыДляДобавления = Новый Массив;
+	
+	Если ТекущаяБаза Тогда
+		
+		ПараметрыДляДобавления.Добавить(" --log ""%Лог%""");
+		ПараметрыДляДобавления.Добавить("silent");
+		ПараметрыДляДобавления.Добавить("path ""%ПутьКПлатформе%""");
+	
+		Если Не ПустаяСтрока(КодРазблокировки) Тогда
+			ПараметрыДляДобавления.Добавить("access %КодРазблокировки%");
+		КонецЕсли;
+		
+		Если Не ПустаяСтрока(Логин) Тогда
+			ПараметрыДляДобавления.Добавить("login ""%Логин%""");
+			ПараметрыДляДобавления.Добавить("password ""%Пароль%""");
+		КонецЕсли;
+		
+		ПараметрыДляДобавления.Добавить("connection ""%СтрокаПодключенияКБазе%""");
+		
+	КонецЕсли;
+	
+	Возврат Шаблон + СобратьСтрокуИзПодстрок(ПараметрыДляДобавления, " --");
+	
+КонецФункции
+
+&НаКлиенте
+Функция ИнформационнаяБазаФайловая(Знач СтрокаСоединенияИнформационнойБазы = "")
+			
+	Если ПустаяСтрока(СтрокаСоединенияИнформационнойБазы) Тогда
+		СтрокаСоединенияИнформационнойБазы =  СтрокаСоединенияИнформационнойБазы();
+	КонецЕсли;
+	Возврат Найти(Врег(СтрокаСоединенияИнформационнойБазы), "FILE=") = 1;
+	
+КонецФункции
+
+&НаКлиенте
+Функция ПараметрыИзСтроки(Знач СтрокаПараметров)
+	
+	Результат = Новый Структура;
+	
+	СимволДвойныеКавычки = Символ(34); // (")
+	
+	МассивПодстрок = РазложитьСтрокуВМассивПодстрок(СтрокаПараметров, ";");
+	
+	Для Каждого СтрокаПараметра Из МассивПодстрок Цикл
+		
+		ПозицияПервогоЗнакаРавенства = Найти(СтрокаПараметра, "=");
+		
+		// Получаем имя параметра
+		ИмяПараметра = СокрЛП(Лев(СтрокаПараметра, ПозицияПервогоЗнакаРавенства - 1));
+		
+		// Получаем значение параметра.
+		ЗначениеПараметра = СокрЛП(Сред(СтрокаПараметра, ПозицияПервогоЗнакаРавенства + 1));
+		
+		Если  Лев(ЗначениеПараметра, 1) = СимволДвойныеКавычки
+			И Прав(ЗначениеПараметра, 1) = СимволДвойныеКавычки Тогда
+			
+			ЗначениеПараметра = Сред(ЗначениеПараметра, 2, СтрДлина(ЗначениеПараметра) - 2);
+			
+		КонецЕсли;
+		
+		Если Не ПустаяСтрока(ИмяПараметра) Тогда
+			
+			Результат.Вставить(ИмяПараметра, ЗначениеПараметра);
+			
+		КонецЕсли;
+		
+	КонецЦикла;
+	
+	Возврат Результат;
+КонецФункции
+
+&НаКлиенте
+Функция ПодставитьПараметрыВСтроку(Шаблон, Знач ПарметрыСтроки)
+	
+	Строка = Шаблон;
+	Для Каждого Элемент Из ПарметрыСтроки Цикл
+		Строка = СтрЗаменить(Строка, "%" + Элемент.Ключ + "%", Элемент.Значение);
+	КонецЦикла;
+		
+	Возврат Строка;
+	
+КонецФункции
+
+&НаКлиентеНаСервереБезКонтекста
+Процедура Сообщение(Знач Текст)
+	
+	СообщениеПользователю = Новый СообщениеПользователю;
+	СообщениеПользователю.Текст = Текст;
+	СообщениеПользователю.Сообщить();
+	
+КонецПроцедуры
+
+&НаКлиенте
+Функция РазложитьСтрокуВМассивПодстрок(Знач Стр, Разделитель = ",")
+	
+	МассивСтрок = Новый Массив();
+	Если Разделитель = " " Тогда
+		Стр = СокрЛП(Стр);
+		Пока Истина Цикл
+			Поз = Найти(Стр, Разделитель);
+			Если Поз = 0 Тогда
+				МассивСтрок.Добавить(Стр);
+				Возврат МассивСтрок;
+			КонецЕсли;
+			МассивСтрок.Добавить(Лев(Стр, Поз - 1));
+			Стр = СокрЛ(Сред(Стр, Поз));
+		КонецЦикла;
+	Иначе
+		ДлинаРазделителя = СтрДлина(Разделитель);
+		Пока Истина Цикл
+			Поз = Найти(Стр, Разделитель);
+			Если Поз = 0 Тогда
+				МассивСтрок.Добавить(Стр);
+				Возврат МассивСтрок;
+			КонецЕсли;
+			МассивСтрок.Добавить(Лев(Стр, Поз - 1));
+			Стр = Сред(Стр, Поз + ДлинаРазделителя);
+		КонецЦикла;
+	КонецЕсли;
+	
+КонецФункции
+
+&НаКлиенте
+Функция СобратьСтрокуИзПодстрок(Знач Строки, Знач Разделитель)
+	
+	Результат = "";
+	
+	Для Каждого Строка Из Строки Цикл
+		Результат = Результат + ?(ПустаяСтрока(Результат), "", Разделитель) + Строка;
+	КонецЦикла;
+	
+	Возврат Результат;
+	
+КонецФункции
+
+&НаКлиенте
+Процедура УстановитьВидимостьЭлементов()
+	Элементы.ВыгружатьРасширенияВSpec.Видимость = (ТипОперации = Операции.ВыгрузкаCFE);
+КонецПроцедуры
+
+&НаСервере
+Функция ИмяФайлаОбработки()
+	Возврат РеквизитФормыВЗначение("Объект").ИспользуемоеИмяФайла;
+КонецФункции
+
+&НаКлиенте
+Процедура ВывестиВерсиюПакета()
+	
+	ЧтениеТекста = Новый ЧтениеТекста(ПутьДоRunner() + РазделительПути() + "__init__.py");
+	СтрокаВерсии = ЧтениеТекста.ПрочитатьСтроку();
+	ЧтениеТекста.Закрыть();
+	
+	ПараметрыВерсии = РазложитьСтрокуВМассивПодстрок(СтрокаВерсии, "=");
+	Версия = СокрЛП(ПараметрыВерсии[1]);
+	
+	Заголовок = Версия;
+	
+КонецПроцедуры
+
+&НаКлиенте
+Функция РазделительПути()
+	Возврат "\";
+КонецФункции
+
+&НаКлиенте
+Функция СоединитьПути(Знач ПутьКаталога, Знач Элемент1, Знач Элемент2 = "")
+	
+	Массив = Новый Массив;
+	Массив.Добавить(ПутьКаталога);
+	Массив.Добавить(Элемент1);
+	Если Не ПустаяСтрока(Элемент2) Тогда
+		Массив.Добавить(Элемент2);
+	КонецЕсли;
+	
+	Возврат СобратьСтрокуИзПодстрок(Массив, РазделительПути());
+	
+КонецФункции
+
+&НаКлиенте
+Функция УбратьСКонцаРазделительПути(Знач Путь)
+	
+	Результат = Путь;
+	Если Прав(Путь, 1) = РазделительПути() Тогда
+		Результат = Лев(Результат, СтрДлина(Результат) - 1);
+	КонецЕсли;
+	
+	Возврат Результат;
+	
+КонецФункции
+
+&НаКлиенте
+Функция ПолучитьЭтапы(Знач ВыбраннаяОперация)
+	
+	Массив = Новый Массив();
+	
+	СтрокаДляЗапуска = "";
+	
+	Если ВыбраннаяОперация = Операции.ПолнаяВыгрузкаCF Или ВыбраннаяОперация = Операции.ЧастичнаяВыгрузкаCF Тогда
+		
+		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузкиКонфигурации%""";
+		Если КонфигурацияСОшибкамиВыгрузки() Тогда
+			СтрокаДляЗапуска = СтрокаДляЗапуска + " --repair";
+		КонецЕсли;
+		Если ВыбраннаяОперация = Операции.ЧастичнаяВыгрузкаCF Тогда
+			СтрокаДляЗапуска = СтрокаДляЗапуска + " --update";
+		КонецЕсли;
+		
+		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "dump_config"));
+		
+	ИначеЕсли ВыбраннаяОперация = Операции.ВыгрузкаCFE Тогда
+		
+		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузкиРасширений%""";
+		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "dump_extensions"));
+		
+	ИначеЕсли ВыбраннаяОперация = Операции.ПолнаяВыгрузкаEPF Или ВыбраннаяОперация = Операции.ЧастичнаяВыгрузкаEPF Тогда
+		
+		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузки%""";
+		Если ВыбраннаяОперация = Операции.ПолнаяВыгрузкаEPF Тогда
+			СтрокаДляЗапуска = СтрокаДляЗапуска + " --clear_hash";
+		КонецЕсли;
+		
+		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "sync"));
+		
+	ИначеЕсли ВыбраннаяОперация = Операции.СоздатьEPF Тогда
+		
+		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузки%"" --create";
+		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "sync"));
+		
+	ИначеЕсли ВыбраннаяОперация = Операции.ЗагрузитьCF Тогда
+		
+		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузкиКонфигурации%""";
+		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "load_config"));
+		
+		СтрокаДляЗапуска = "--folder ""%ПапкаВыгрузкиРасширений%""";
+		Массив.Добавить(СоздатьЭтап(СтрокаДляЗапуска, "load_extension"));
+		
+	Иначе
+		ВызватьИсключение "операция не определена";
+	КонецЕсли;
+	
+	Возврат Массив;
+	
+КонецФункции
+
+&НаКлиенте
+Функция ПутьДоRunner()
+	
+	Разделитель = РазделительПути();
+	
+	ПутьОбработки = РазложитьСтрокуВМассивПодстрок(ИмяФайлаОбработки(), Разделитель);
+	ПутьОбработки.Удалить(ПутьОбработки.Количество() - 1);
+	ПутьОбработки.Удалить(ПутьОбработки.Количество() - 1);
+	ПутьОбработки.Удалить(ПутьОбработки.Количество() - 1);
+	ПутьОбработки.Удалить(ПутьОбработки.Количество() - 1);
+	
+	ПутьВерсии = СобратьСтрокуИзПодстрок(ПутьОбработки, Разделитель);
+	
+	Возврат ПутьВерсии;
+	
+КонецФункции
+
+&НаКлиенте
+Функция СоздатьЭтап(Знач СтрокаДляЗапуска, Знач Команда)
+	Возврат Новый Структура("СтрокаДляЗапуска, Команда", СтрокаДляЗапуска, Команда);
+КонецФункции
+
+#КонецОбласти
+
+#Область Инициализация
+
+Операции = Новый Структура;
+Операции.Вставить("ПолнаяВыгрузкаCF", "CF Полная Выгрузка");
+Операции.Вставить("ЧастичнаяВыгрузкаCF", "CF Частичная Выгрузка");
+Операции.Вставить("ПолнаяВыгрузкаEPF", "EPF Полная Выгрузка");
+Операции.Вставить("ЧастичнаяВыгрузкаEPF", "EPF Частичная Выгрузка");
+Операции.Вставить("СоздатьEPF", "EPF Создать");
+Операции.Вставить("ВыгрузкаCFE", "CFE Выгрузка");
+Операции.Вставить("ЗагрузитьCF", "Загрузить конфигурацию");
+
+#КонецОбласти
```

### Comparing `runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form.xml` & `runner1c-0.59/runner1c/tools/epf/Runner1C/Forms/Form/Ext/Form.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, Unicode text, UTF-8 (with BOM) text, with very long lines (850), with CRLF line terminators*

 * *Files 22% similar despite different names*

```diff
@@ -1,681 +1,664 @@
 00000000: efbb bf3c 3f78 6d6c 2076 6572 7369 6f6e  ...<?xml version
 00000010: 3d22 312e 3022 2065 6e63 6f64 696e 673d  ="1.0" encoding=
-00000020: 2255 5446 2d38 223f 3e0d 0a3c 466f 726d  "UTF-8"?>..<Form
-00000030: 2078 6d6c 6e73 3d22 6874 7470 3a2f 2f76   xmlns="http://v
-00000040: 382e 3163 2e72 752f 382e 332f 7863 662f  8.1c.ru/8.3/xcf/
-00000050: 6c6f 6766 6f72 6d22 2078 6d6c 6e73 3a61  logform" xmlns:a
-00000060: 7070 3d22 6874 7470 3a2f 2f76 382e 3163  pp="http://v8.1c
-00000070: 2e72 752f 382e 322f 6d61 6e61 6765 642d  .ru/8.2/managed-
-00000080: 6170 706c 6963 6174 696f 6e2f 636f 7265  application/core
-00000090: 2220 786d 6c6e 733a 6366 673d 2268 7474  " xmlns:cfg="htt
-000000a0: 703a 2f2f 7638 2e31 632e 7275 2f38 2e31  p://v8.1c.ru/8.1
-000000b0: 2f64 6174 612f 656e 7465 7270 7269 7365  /data/enterprise
-000000c0: 2f63 7572 7265 6e74 2d63 6f6e 6669 6722  /current-config"
-000000d0: 2078 6d6c 6e73 3a64 6373 636f 723d 2268   xmlns:dcscor="h
-000000e0: 7474 703a 2f2f 7638 2e31 632e 7275 2f38  ttp://v8.1c.ru/8
-000000f0: 2e31 2f64 6174 612d 636f 6d70 6f73 6974  .1/data-composit
-00000100: 696f 6e2d 7379 7374 656d 2f63 6f72 6522  ion-system/core"
-00000110: 2078 6d6c 6e73 3a64 6373 7365 743d 2268   xmlns:dcsset="h
-00000120: 7474 703a 2f2f 7638 2e31 632e 7275 2f38  ttp://v8.1c.ru/8
-00000130: 2e31 2f64 6174 612d 636f 6d70 6f73 6974  .1/data-composit
-00000140: 696f 6e2d 7379 7374 656d 2f73 6574 7469  ion-system/setti
-00000150: 6e67 7322 2078 6d6c 6e73 3a65 6e74 3d22  ngs" xmlns:ent="
-00000160: 6874 7470 3a2f 2f76 382e 3163 2e72 752f  http://v8.1c.ru/
-00000170: 382e 312f 6461 7461 2f65 6e74 6572 7072  8.1/data/enterpr
-00000180: 6973 6522 2078 6d6c 6e73 3a6c 663d 2268  ise" xmlns:lf="h
-00000190: 7474 703a 2f2f 7638 2e31 632e 7275 2f38  ttp://v8.1c.ru/8
-000001a0: 2e32 2f6d 616e 6167 6564 2d61 7070 6c69  .2/managed-appli
-000001b0: 6361 7469 6f6e 2f6c 6f67 666f 726d 2220  cation/logform" 
-000001c0: 786d 6c6e 733a 7374 796c 653d 2268 7474  xmlns:style="htt
-000001d0: 703a 2f2f 7638 2e31 632e 7275 2f38 2e31  p://v8.1c.ru/8.1
-000001e0: 2f64 6174 612f 7569 2f73 7479 6c65 2220  /data/ui/style" 
-000001f0: 786d 6c6e 733a 7379 733d 2268 7474 703a  xmlns:sys="http:
-00000200: 2f2f 7638 2e31 632e 7275 2f38 2e31 2f64  //v8.1c.ru/8.1/d
-00000210: 6174 612f 7569 2f66 6f6e 7473 2f73 7973  ata/ui/fonts/sys
-00000220: 7465 6d22 2078 6d6c 6e73 3a76 383d 2268  tem" xmlns:v8="h
-00000230: 7474 703a 2f2f 7638 2e31 632e 7275 2f38  ttp://v8.1c.ru/8
-00000240: 2e31 2f64 6174 612f 636f 7265 2220 786d  .1/data/core" xm
-00000250: 6c6e 733a 7638 7569 3d22 6874 7470 3a2f  lns:v8ui="http:/
-00000260: 2f76 382e 3163 2e72 752f 382e 312f 6461  /v8.1c.ru/8.1/da
-00000270: 7461 2f75 6922 2078 6d6c 6e73 3a77 6562  ta/ui" xmlns:web
-00000280: 3d22 6874 7470 3a2f 2f76 382e 3163 2e72  ="http://v8.1c.r
-00000290: 752f 382e 312f 6461 7461 2f75 692f 636f  u/8.1/data/ui/co
-000002a0: 6c6f 7273 2f77 6562 2220 786d 6c6e 733a  lors/web" xmlns:
-000002b0: 7769 6e3d 2268 7474 703a 2f2f 7638 2e31  win="http://v8.1
-000002c0: 632e 7275 2f38 2e31 2f64 6174 612f 7569  c.ru/8.1/data/ui
-000002d0: 2f63 6f6c 6f72 732f 7769 6e64 6f77 7322  /colors/windows"
-000002e0: 2078 6d6c 6e73 3a78 723d 2268 7474 703a   xmlns:xr="http:
-000002f0: 2f2f 7638 2e31 632e 7275 2f38 2e33 2f78  //v8.1c.ru/8.3/x
-00000300: 6366 2f72 6561 6461 626c 6522 2078 6d6c  cf/readable" xml
-00000310: 6e73 3a78 733d 2268 7474 703a 2f2f 7777  ns:xs="http://ww
-00000320: 772e 7733 2e6f 7267 2f32 3030 312f 584d  w.w3.org/2001/XM
-00000330: 4c53 6368 656d 6122 2078 6d6c 6e73 3a78  LSchema" xmlns:x
-00000340: 7369 3d22 6874 7470 3a2f 2f77 7777 2e77  si="http://www.w
-00000350: 332e 6f72 672f 3230 3031 2f58 4d4c 5363  3.org/2001/XMLSc
-00000360: 6865 6d61 2d69 6e73 7461 6e63 6522 2076  hema-instance" v
-00000370: 6572 7369 6f6e 3d22 322e 3622 3e0d 0a09  ersion="2.6">...
-00000380: 3c41 7574 6f53 6176 6544 6174 6149 6e53  <AutoSaveDataInS
-00000390: 6574 7469 6e67 733e 5573 653c 2f41 7574  ettings>Use</Aut
-000003a0: 6f53 6176 6544 6174 6149 6e53 6574 7469  oSaveDataInSetti
-000003b0: 6e67 733e 0d0a 093c 5665 7274 6963 616c  ngs>...<Vertical
-000003c0: 5363 726f 6c6c 3e75 7365 4966 4e65 6365  Scroll>useIfNece
-000003d0: 7373 6172 793c 2f56 6572 7469 6361 6c53  ssary</VerticalS
-000003e0: 6372 6f6c 6c3e 0d0a 093c 4175 746f 436f  croll>...<AutoCo
-000003f0: 6d6d 616e 6442 6172 206e 616d 653d 22d0  mmandBar name=".
-00000400: a4d0 bed1 80d0 bcd0 b0d0 9ad0 bed0 bcd0  ................
-00000410: b0d0 bdd0 b4d0 bdd0 b0d1 8fd0 9fd0 b0d0  ................
-00000420: bdd0 b5d0 bbd1 8c22 2069 643d 222d 3122  ......." id="-1"
-00000430: 3e0d 0a09 093c 4175 746f 6669 6c6c 3e66  >....<Autofill>f
-00000440: 616c 7365 3c2f 4175 746f 6669 6c6c 3e0d  alse</Autofill>.
-00000450: 0a09 3c2f 4175 746f 436f 6d6d 616e 6442  ..</AutoCommandB
-00000460: 6172 3e0d 0a09 3c45 7665 6e74 733e 0d0a  ar>...<Events>..
-00000470: 0909 3c45 7665 6e74 206e 616d 653d 224f  ..<Event name="O
-00000480: 6e4f 7065 6e22 3ed0 9fd1 80d0 b8d0 9ed1  nOpen">.........
-00000490: 82d0 bad1 80d1 8bd1 82d0 b8d0 b83c 2f45  .............</E
-000004a0: 7665 6e74 3e0d 0a09 093c 4576 656e 7420  vent>....<Event 
-000004b0: 6e61 6d65 3d22 4669 6c6c 4368 6563 6b50  name="FillCheckP
-000004c0: 726f 6365 7373 696e 6741 7453 6572 7665  rocessingAtServe
-000004d0: 7222 3ed0 9ed0 b1d1 80d0 b0d0 b1d0 bed1  r">.............
-000004e0: 82d0 bad0 b0d0 9fd1 80d0 bed0 b2d0 b5d1  ................
-000004f0: 80d0 bad0 b8d0 97d0 b0d0 bfd0 bed0 bbd0  ................
-00000500: bdd0 b5d0 bdd0 b8d1 8fd0 9dd0 b0d0 a1d0  ................
-00000510: b5d1 80d0 b2d0 b5d1 80d0 b53c 2f45 7665  ...........</Eve
-00000520: 6e74 3e0d 0a09 3c2f 4576 656e 7473 3e0d  nt>...</Events>.
-00000530: 0a09 3c43 6869 6c64 4974 656d 733e 0d0a  ..<ChildItems>..
-00000540: 0909 3c49 6e70 7574 4669 656c 6420 6e61  ..<InputField na
-00000550: 6d65 3d22 d0a2 d0b8 d0bf d09e d0bf d0b5  me="............
-00000560: d180 d0b0 d186 d0b8 d0b8 2220 6964 3d22  .........." id="
-00000570: 3132 223e 0d0a 0909 093c 4461 7461 5061  12">.....<DataPa
-00000580: 7468 3ed0 a2d0 b8d0 bfd0 9ed0 bfd0 b5d1  th>.............
-00000590: 80d0 b0d1 86d0 b8d0 b83c 2f44 6174 6150  .........</DataP
-000005a0: 6174 683e 0d0a 0909 093c 4c69 7374 4368  ath>.....<ListCh
-000005b0: 6f69 6365 4d6f 6465 3e74 7275 653c 2f4c  oiceMode>true</L
-000005c0: 6973 7443 686f 6963 654d 6f64 653e 0d0a  istChoiceMode>..
-000005d0: 0909 093c 436f 6e74 6578 744d 656e 7520  ...<ContextMenu 
-000005e0: 6e61 6d65 3d22 d0a2 d0b8 d0bf d09e d0bf  name="..........
-000005f0: d0b5 d180 d0b0 d186 d0b8 d0b8 d09a d0be  ................
-00000600: d0bd d182 d0b5 d0ba d181 d182 d0bd d0be  ................
-00000610: d0b5 d09c d0b5 d0bd d18e 2220 6964 3d22  .........." id="
-00000620: 3133 222f 3e0d 0a09 0909 3c45 7874 656e  13"/>.....<Exten
-00000630: 6465 6454 6f6f 6c74 6970 206e 616d 653d  dedTooltip name=
-00000640: 22d0 a2d0 b8d0 bfd0 9ed0 bfd0 b5d1 80d0  "...............
-00000650: b0d1 86d0 b8d0 b8d0 a0d0 b0d1 81d1 88d0  ................
-00000660: b8d1 80d0 b5d0 bdd0 bdd0 b0d1 8fd0 9fd0  ................
-00000670: bed0 b4d1 81d0 bad0 b0d0 b7d0 bad0 b022  ..............."
-00000680: 2069 643d 2232 3722 2f3e 0d0a 0909 093c   id="27"/>.....<
-00000690: 4576 656e 7473 3e0d 0a09 0909 093c 4576  Events>......<Ev
-000006a0: 656e 7420 6e61 6d65 3d22 4f6e 4368 616e  ent name="OnChan
-000006b0: 6765 223e d0a2 d0b8 d0bf d09e d0bf d0b5  ge">............
-000006c0: d180 d0b0 d186 d0b8 d0b8 d09f d180 d0b8  ................
-000006d0: d098 d0b7 d0bc d0b5 d0bd d0b5 d0bd d0b8  ................
-000006e0: d0b8 3c2f 4576 656e 743e 0d0a 0909 093c  ..</Event>.....<
-000006f0: 2f45 7665 6e74 733e 0d0a 0909 3c2f 496e  /Events>....</In
-00000700: 7075 7446 6965 6c64 3e0d 0a09 093c 4368  putField>....<Ch
-00000710: 6563 6b42 6f78 4669 656c 6420 6e61 6d65  eckBoxField name
-00000720: 3d22 d092 d18b d0b3 d180 d183 d0b6 d0b0  ="..............
-00000730: d182 d18c d0a0 d0b0 d181 d188 d0b8 d180  ................
-00000740: d0b5 d0bd d0b8 d18f d092 5370 6563 2220  ..........Spec" 
-00000750: 6964 3d22 3338 223e 0d0a 0909 093c 4461  id="38">.....<Da
-00000760: 7461 5061 7468 3ed0 92d1 8bd0 b3d1 80d1  taPath>.........
-00000770: 83d0 b6d0 b0d1 82d1 8cd0 a0d0 b0d1 81d1  ................
-00000780: 88d0 b8d1 80d0 b5d0 bdd0 b8d1 8fd0 9253  ...............S
-00000790: 7065 633c 2f44 6174 6150 6174 683e 0d0a  pec</DataPath>..
-000007a0: 0909 093c 5469 746c 653e 0d0a 0909 0909  ...<Title>......
-000007b0: 3c76 383a 6974 656d 3e0d 0a09 0909 0909  <v8:item>.......
-000007c0: 3c76 383a 6c61 6e67 3e72 753c 2f76 383a  <v8:lang>ru</v8:
-000007d0: 6c61 6e67 3e0d 0a09 0909 0909 3c76 383a  lang>.......<v8:
-000007e0: 636f 6e74 656e 743e d092 d18b d0b3 d180  content>........
-000007f0: d183 d0b6 d0b0 d182 d18c 20d0 b220 7370  .......... .. sp
-00000800: 6563 3c2f 7638 3a63 6f6e 7465 6e74 3e0d  ec</v8:content>.
-00000810: 0a09 0909 093c 2f76 383a 6974 656d 3e0d  .....</v8:item>.
-00000820: 0a09 0909 3c2f 5469 746c 653e 0d0a 0909  ....</Title>....
-00000830: 093c 4368 6563 6b42 6f78 5479 7065 3e41  .<CheckBoxType>A
-00000840: 7574 6f3c 2f43 6865 636b 426f 7854 7970  uto</CheckBoxTyp
-00000850: 653e 0d0a 0909 093c 436f 6e74 6578 744d  e>.....<ContextM
-00000860: 656e 7520 6e61 6d65 3d22 d092 d18b d0b3  enu name="......
-00000870: d180 d183 d0b6 d0b0 d182 d18c d0a0 d0b0  ................
-00000880: d181 d188 d0b8 d180 d0b5 d0bd d0b8 d18f  ................
-00000890: d092 5370 6563 d09a d0be d0bd d182 d0b5  ..Spec..........
-000008a0: d0ba d181 d182 d0bd d0be d0b5 d09c d0b5  ................
-000008b0: d0bd d18e 2220 6964 3d22 3339 222f 3e0d  ...." id="39"/>.
-000008c0: 0a09 0909 3c45 7874 656e 6465 6454 6f6f  ....<ExtendedToo
-000008d0: 6c74 6970 206e 616d 653d 22d0 92d1 8bd0  ltip name=".....
-000008e0: b3d1 80d1 83d0 b6d0 b0d1 82d1 8cd0 a0d0  ................
-000008f0: b0d1 81d1 88d0 b8d1 80d0 b5d0 bdd0 b8d1  ................
-00000900: 8fd0 9253 7065 63d0 a0d0 b0d1 81d1 88d0  ...Spec.........
-00000910: b8d1 80d0 b5d0 bdd0 bdd0 b0d1 8fd0 9fd0  ................
-00000920: bed0 b4d1 81d0 bad0 b0d0 b7d0 bad0 b022  ..............."
-00000930: 2069 643d 2234 3022 2f3e 0d0a 0909 3c2f   id="40"/>....</
-00000940: 4368 6563 6b42 6f78 4669 656c 643e 0d0a  CheckBoxField>..
-00000950: 0909 3c49 6e70 7574 4669 656c 6420 6e61  ..<InputField na
-00000960: 6d65 3d22 d09f d0b0 d0bf d0ba d0b0 d092  me="............
-00000970: d18b d0b3 d180 d183 d0b7 d0ba d0b8 2220  .............." 
-00000980: 6964 3d22 3722 3e0d 0a09 0909 3c44 6174  id="7">.....<Dat
-00000990: 6150 6174 683e d09f d0b0 d0bf d0ba d0b0  aPath>..........
-000009a0: d092 d18b d0b3 d180 d183 d0b7 d0ba d0b8  ................
-000009b0: 3c2f 4461 7461 5061 7468 3e0d 0a09 0909  </DataPath>.....
-000009c0: 3c54 6974 6c65 3e0d 0a09 0909 093c 7638  <Title>......<v8
-000009d0: 3a69 7465 6d3e 0d0a 0909 0909 093c 7638  :item>.......<v8
-000009e0: 3a6c 616e 673e 7275 3c2f 7638 3a6c 616e  :lang>ru</v8:lan
-000009f0: 673e 0d0a 0909 0909 093c 7638 3a63 6f6e  g>.......<v8:con
-00000a00: 7465 6e74 3ed0 9ad0 bed1 80d0 b5d0 bdd1  tent>...........
-00000a10: 8c20 d180 d0b5 d0bf d0be d0b7 d0b8 d182  . ..............
-00000a20: d0be d180 d0b8 d18f 3c2f 7638 3a63 6f6e  ........</v8:con
-00000a30: 7465 6e74 3e0d 0a09 0909 093c 2f76 383a  tent>......</v8:
-00000a40: 6974 656d 3e0d 0a09 0909 3c2f 5469 746c  item>.....</Titl
-00000a50: 653e 0d0a 0909 093c 4368 6f69 6365 4275  e>.....<ChoiceBu
-00000a60: 7474 6f6e 3e74 7275 653c 2f43 686f 6963  tton>true</Choic
-00000a70: 6542 7574 746f 6e3e 0d0a 0909 093c 436f  eButton>.....<Co
-00000a80: 6e74 6578 744d 656e 7520 6e61 6d65 3d22  ntextMenu name="
-00000a90: d09f d0b0 d0bf d0ba d0b0 d092 d18b d0b3  ................
-00000aa0: d180 d183 d0b7 d0ba d0b8 d09a d0be d0bd  ................
-00000ab0: d182 d0b5 d0ba d181 d182 d0bd d0be d0b5  ................
-00000ac0: d09c d0b5 d0bd d18e 2220 6964 3d22 3822  ........" id="8"
-00000ad0: 2f3e 0d0a 0909 093c 4578 7465 6e64 6564  />.....<Extended
-00000ae0: 546f 6f6c 7469 7020 6e61 6d65 3d22 d09f  Tooltip name="..
-00000af0: d0b0 d0bf d0ba d0b0 d092 d18b d0b3 d180  ................
-00000b00: d183 d0b7 d0ba d0b8 d0a0 d0b0 d181 d188  ................
-00000b10: d0b8 d180 d0b5 d0bd d0bd d0b0 d18f d09f  ................
-00000b20: d0be d0b4 d181 d0ba d0b0 d0b7 d0ba d0b0  ................
-00000b30: 2220 6964 3d22 3331 222f 3e0d 0a09 0909  " id="31"/>.....
-00000b40: 3c45 7665 6e74 733e 0d0a 0909 0909 3c45  <Events>......<E
-00000b50: 7665 6e74 206e 616d 653d 2253 7461 7274  vent name="Start
-00000b60: 4368 6f69 6365 223e d09f d0b0 d0bf d0ba  Choice">........
-00000b70: d0b0 d092 d18b d0b3 d180 d183 d0b7 d0ba  ................
-00000b80: d0b8 d09d d0b0 d187 d0b0 d0bb d0be d092  ................
-00000b90: d18b d0b1 d0be d180 d0b0 3c2f 4576 656e  ..........</Even
-00000ba0: 743e 0d0a 0909 093c 2f45 7665 6e74 733e  t>.....</Events>
-00000bb0: 0d0a 0909 3c2f 496e 7075 7446 6965 6c64  ....</InputField
-00000bc0: 3e0d 0a09 093c 496e 7075 7446 6965 6c64  >....<InputField
-00000bd0: 206e 616d 653d 22d0 9fd1 83d1 82d1 8cd0   name=".........
-00000be0: 9ad0 9fd0 bbd0 b0d1 82d1 84d0 bed1 80d0  ................
-00000bf0: bcd0 b522 2069 643d 2231 223e 0d0a 0909  ..." id="1">....
-00000c00: 093c 4461 7461 5061 7468 3ed0 9fd1 83d1  .<DataPath>.....
-00000c10: 82d1 8cd0 9ad0 9fd0 bbd0 b0d1 82d1 84d0  ................
-00000c20: bed1 80d0 bcd0 b53c 2f44 6174 6150 6174  .......</DataPat
-00000c30: 683e 0d0a 0909 093c 4368 6f69 6365 4275  h>.....<ChoiceBu
-00000c40: 7474 6f6e 3e74 7275 653c 2f43 686f 6963  tton>true</Choic
-00000c50: 6542 7574 746f 6e3e 0d0a 0909 093c 436f  eButton>.....<Co
-00000c60: 6e74 6578 744d 656e 7520 6e61 6d65 3d22  ntextMenu name="
-00000c70: d09f d183 d182 d18c d09a d09f d0bb d0b0  ................
-00000c80: d182 d184 d0be d180 d0bc d0b5 d09a d0be  ................
-00000c90: d0bd d182 d0b5 d0ba d181 d182 d0bd d0be  ................
-00000ca0: d0b5 d09c d0b5 d0bd d18e 2220 6964 3d22  .........." id="
-00000cb0: 3222 2f3e 0d0a 0909 093c 4578 7465 6e64  2"/>.....<Extend
-00000cc0: 6564 546f 6f6c 7469 7020 6e61 6d65 3d22  edTooltip name="
-00000cd0: d09f d183 d182 d18c d09a d09f d0bb d0b0  ................
-00000ce0: d182 d184 d0be d180 d0bc d0b5 d0a0 d0b0  ................
-00000cf0: d181 d188 d0b8 d180 d0b5 d0bd d0bd d0b0  ................
-00000d00: d18f d09f d0be d0b4 d181 d0ba d0b0 d0b7  ................
-00000d10: d0ba d0b0 2220 6964 3d22 3236 222f 3e0d  ...." id="26"/>.
-00000d20: 0a09 0909 3c45 7665 6e74 733e 0d0a 0909  ....<Events>....
-00000d30: 0909 3c45 7665 6e74 206e 616d 653d 2253  ..<Event name="S
-00000d40: 7461 7274 4368 6f69 6365 223e d09f d183  tartChoice">....
-00000d50: d182 d18c d09a d09f d0bb d0b0 d182 d184  ................
-00000d60: d0be d180 d0bc d0b5 d09d d0b0 d187 d0b0  ................
-00000d70: d0bb d0be d092 d18b d0b1 d0be d180 d0b0  ................
-00000d80: 3c2f 4576 656e 743e 0d0a 0909 093c 2f45  </Event>.....</E
-00000d90: 7665 6e74 733e 0d0a 0909 3c2f 496e 7075  vents>....</Inpu
-00000da0: 7446 6965 6c64 3e0d 0a09 093c 496e 7075  tField>....<Inpu
-00000db0: 7446 6965 6c64 206e 616d 653d 22d0 a1d1  tField name="...
-00000dc0: 82d1 80d0 bed0 bad0 b0d0 9fd0 bed0 b4d0  ................
-00000dd0: bad0 bbd1 8ed1 87d0 b5d0 bdd0 b8d1 8fd0  ................
-00000de0: 9ad0 91d0 b0d0 b7d0 b522 2069 643d 2234  ........." id="4
-00000df0: 223e 0d0a 0909 093c 4461 7461 5061 7468  ">.....<DataPath
-00000e00: 3ed0 a1d1 82d1 80d0 bed0 bad0 b0d0 9fd0  >...............
-00000e10: bed0 b4d0 bad0 bbd1 8ed1 87d0 b5d0 bdd0  ................
-00000e20: b8d1 8fd0 9ad0 91d0 b0d0 b7d0 b53c 2f44  .............</D
-00000e30: 6174 6150 6174 683e 0d0a 0909 093c 436f  ataPath>.....<Co
-00000e40: 6e74 6578 744d 656e 7520 6e61 6d65 3d22  ntextMenu name="
-00000e50: d0a1 d182 d180 d0be d0ba d0b0 d09f d0be  ................
-00000e60: d0b4 d0ba d0bb d18e d187 d0b5 d0bd d0b8  ................
-00000e70: d18f d09a d091 d0b0 d0b7 d0b5 d09a d0be  ................
-00000e80: d0bd d182 d0b5 d0ba d181 d182 d0bd d0be  ................
-00000e90: d0b5 d09c d0b5 d0bd d18e 2220 6964 3d22  .........." id="
-00000ea0: 3522 2f3e 0d0a 0909 093c 4578 7465 6e64  5"/>.....<Extend
-00000eb0: 6564 546f 6f6c 7469 7020 6e61 6d65 3d22  edTooltip name="
-00000ec0: d0a1 d182 d180 d0be d0ba d0b0 d09f d0be  ................
-00000ed0: d0b4 d0ba d0bb d18e d187 d0b5 d0bd d0b8  ................
-00000ee0: d18f d09a d091 d0b0 d0b7 d0b5 d0a0 d0b0  ................
-00000ef0: d181 d188 d0b8 d180 d0b5 d0bd d0bd d0b0  ................
-00000f00: d18f d09f d0be d0b4 d181 d0ba d0b0 d0b7  ................
-00000f10: d0ba d0b0 2220 6964 3d22 3238 222f 3e0d  ...." id="28"/>.
-00000f20: 0a09 0909 3c45 7665 6e74 733e 0d0a 0909  ....<Events>....
-00000f30: 0909 3c45 7665 6e74 206e 616d 653d 2253  ..<Event name="S
-00000f40: 7461 7274 4368 6f69 6365 223e d0a1 d182  tartChoice">....
-00000f50: d180 d0be d0ba d0b0 d09f d0be d0b4 d0ba  ................
-00000f60: d0bb d18e d187 d0b5 d0bd d0b8 d18f d09a  ................
-00000f70: d091 d0b0 d0b7 d0b5 d09d d0b0 d187 d0b0  ................
-00000f80: d0bb d0be d092 d18b d0b1 d0be d180 d0b0  ................
-00000f90: 3c2f 4576 656e 743e 0d0a 0909 093c 2f45  </Event>.....</E
-00000fa0: 7665 6e74 733e 0d0a 0909 3c2f 496e 7075  vents>....</Inpu
-00000fb0: 7446 6965 6c64 3e0d 0a09 093c 496e 7075  tField>....<Inpu
-00000fc0: 7446 6965 6c64 206e 616d 653d 22d0 9bd0  tField name="...
-00000fd0: bed0 b3d0 b8d0 bd22 2069 643d 2231 3822  ......." id="18"
-00000fe0: 3e0d 0a09 0909 3c44 6174 6150 6174 683e  >.....<DataPath>
-00000ff0: d09b d0be d0b3 d0b8 d0bd 3c2f 4461 7461  ..........</Data
-00001000: 5061 7468 3e0d 0a09 0909 3c43 6f6e 7465  Path>.....<Conte
-00001010: 7874 4d65 6e75 206e 616d 653d 22d0 9bd0  xtMenu name="...
-00001020: bed0 b3d0 b8d0 bdd0 9ad0 bed0 bdd1 82d0  ................
-00001030: b5d0 bad1 81d1 82d0 bdd0 bed0 b5d0 9cd0  ................
-00001040: b5d0 bdd1 8e22 2069 643d 2231 3922 2f3e  ....." id="19"/>
-00001050: 0d0a 0909 093c 4578 7465 6e64 6564 546f  .....<ExtendedTo
-00001060: 6f6c 7469 7020 6e61 6d65 3d22 d09b d0be  oltip name="....
-00001070: d0b3 d0b8 d0bd d0a0 d0b0 d181 d188 d0b8  ................
-00001080: d180 d0b5 d0bd d0bd d0b0 d18f d09f d0be  ................
-00001090: d0b4 d181 d0ba d0b0 d0b7 d0ba d0b0 2220  .............." 
-000010a0: 6964 3d22 3239 222f 3e0d 0a09 093c 2f49  id="29"/>....</I
-000010b0: 6e70 7574 4669 656c 643e 0d0a 0909 3c49  nputField>....<I
-000010c0: 6e70 7574 4669 656c 6420 6e61 6d65 3d22  nputField name="
-000010d0: d09f d0b0 d180 d0be d0bb d18c 2220 6964  ............" id
-000010e0: 3d22 3231 223e 0d0a 0909 093c 4461 7461  ="21">.....<Data
-000010f0: 5061 7468 3ed0 9fd0 b0d1 80d0 bed0 bbd1  Path>...........
-00001100: 8c3c 2f44 6174 6150 6174 683e 0d0a 0909  .</DataPath>....
-00001110: 093c 5061 7373 776f 7264 4d6f 6465 3e74  .<PasswordMode>t
-00001120: 7275 653c 2f50 6173 7377 6f72 644d 6f64  rue</PasswordMod
-00001130: 653e 0d0a 0909 093c 436f 6e74 6578 744d  e>.....<ContextM
-00001140: 656e 7520 6e61 6d65 3d22 d09f d0b0 d180  enu name="......
-00001150: d0be d0bb d18c d09a d0be d0bd d182 d0b5  ................
-00001160: d0ba d181 d182 d0bd d0be d0b5 d09c d0b5  ................
-00001170: d0bd d18e 2220 6964 3d22 3232 222f 3e0d  ...." id="22"/>.
-00001180: 0a09 0909 3c45 7874 656e 6465 6454 6f6f  ....<ExtendedToo
-00001190: 6c74 6970 206e 616d 653d 22d0 9fd0 b0d1  ltip name=".....
-000011a0: 80d0 bed0 bbd1 8cd0 a0d0 b0d1 81d1 88d0  ................
-000011b0: b8d1 80d0 b5d0 bdd0 bdd0 b0d1 8fd0 9fd0  ................
-000011c0: bed0 b4d1 81d0 bad0 b0d0 b7d0 bad0 b022  ..............."
-000011d0: 2069 643d 2233 3022 2f3e 0d0a 0909 3c2f   id="30"/>....</
-000011e0: 496e 7075 7446 6965 6c64 3e0d 0a09 093c  InputField>....<
-000011f0: 496e 7075 7446 6965 6c64 206e 616d 653d  InputField name=
-00001200: 22d0 9ad0 bed0 b4d0 a0d0 b0d0 b7d0 b1d0  "...............
-00001210: bbd0 bed0 bad0 b8d1 80d0 bed0 b2d0 bad0  ................
-00001220: b822 2069 643d 2233 3522 3e0d 0a09 0909  ." id="35">.....
-00001230: 3c44 6174 6150 6174 683e d09a d0be d0b4  <DataPath>......
-00001240: d0a0 d0b0 d0b7 d0b1 d0bb d0be d0ba d0b8  ................
-00001250: d180 d0be d0b2 d0ba d0b8 3c2f 4461 7461  ..........</Data
-00001260: 5061 7468 3e0d 0a09 0909 3c43 6f6e 7465  Path>.....<Conte
-00001270: 7874 4d65 6e75 206e 616d 653d 22d0 9ad0  xtMenu name="...
-00001280: bed0 b4d0 a0d0 b0d0 b7d0 b1d0 bbd0 bed0  ................
-00001290: bad0 b8d1 80d0 bed0 b2d0 bad0 b8d0 9ad0  ................
-000012a0: bed0 bdd1 82d0 b5d0 bad1 81d1 82d0 bdd0  ................
-000012b0: bed0 b5d0 9cd0 b5d0 bdd1 8e22 2069 643d  ..........." id=
-000012c0: 2233 3622 2f3e 0d0a 0909 093c 4578 7465  "36"/>.....<Exte
-000012d0: 6e64 6564 546f 6f6c 7469 7020 6e61 6d65  ndedTooltip name
-000012e0: 3d22 d09a d0be d0b4 d0a0 d0b0 d0b7 d0b1  ="..............
-000012f0: d0bb d0be d0ba d0b8 d180 d0be d0b2 d0ba  ................
-00001300: d0b8 d0a0 d0b0 d181 d188 d0b8 d180 d0b5  ................
-00001310: d0bd d0bd d0b0 d18f d09f d0be d0b4 d181  ................
-00001320: d0ba d0b0 d0b7 d0ba d0b0 2220 6964 3d22  .........." id="
-00001330: 3337 222f 3e0d 0a09 093c 2f49 6e70 7574  37"/>....</Input
-00001340: 4669 656c 643e 0d0a 0909 3c55 7375 616c  Field>....<Usual
-00001350: 4772 6f75 7020 6e61 6d65 3d22 d093 d180  Group name="....
-00001360: d183 d0bf d0bf d0b0 2220 6964 3d22 3434  ........" id="44
-00001370: 223e 0d0a 0909 093c 5265 7072 6573 656e  ">.....<Represen
-00001380: 7461 7469 6f6e 3e4e 6f6e 653c 2f52 6570  tation>None</Rep
-00001390: 7265 7365 6e74 6174 696f 6e3e 0d0a 0909  resentation>....
-000013a0: 093c 5368 6f77 5469 746c 653e 6661 6c73  .<ShowTitle>fals
-000013b0: 653c 2f53 686f 7754 6974 6c65 3e0d 0a09  e</ShowTitle>...
-000013c0: 0909 3c45 7874 656e 6465 6454 6f6f 6c74  ..<ExtendedToolt
-000013d0: 6970 206e 616d 653d 22d0 93d1 80d1 83d0  ip name=".......
-000013e0: bfd0 bfd0 b0d0 a0d0 b0d1 81d1 88d0 b8d1  ................
-000013f0: 80d0 b5d0 bdd0 bdd0 b0d1 8fd0 9fd0 bed0  ................
-00001400: b4d1 81d0 bad0 b0d0 b7d0 bad0 b022 2069  ............." i
-00001410: 643d 2234 3522 2f3e 0d0a 0909 093c 4368  d="45"/>.....<Ch
-00001420: 696c 6449 7465 6d73 3e0d 0a09 0909 093c  ildItems>......<
-00001430: 4368 6563 6b42 6f78 4669 656c 6420 6e61  CheckBoxField na
-00001440: 6d65 3d22 d09f d0be d0b4 d0bc d0b5 d0bd  me="............
-00001450: d0b8 d182 d18c d09f d183 d182 d18c 5275  ..............Ru
-00001460: 6e6e 6572 2220 6964 3d22 3431 223e 0d0a  nner" id="41">..
-00001470: 0909 0909 093c 4461 7461 5061 7468 3ed0  .....<DataPath>.
-00001480: 9fd0 bed0 b4d0 bcd0 b5d0 bdd0 b8d1 82d1  ................
-00001490: 8cd0 9fd1 83d1 82d1 8c52 756e 6e65 723c  .........Runner<
-000014a0: 2f44 6174 6150 6174 683e 0d0a 0909 0909  /DataPath>......
-000014b0: 093c 456e 6162 6c65 643e 6661 6c73 653c  .<Enabled>false<
-000014c0: 2f45 6e61 626c 6564 3e0d 0a09 0909 0909  /Enabled>.......
-000014d0: 3c43 6865 636b 426f 7854 7970 653e 4175  <CheckBoxType>Au
-000014e0: 746f 3c2f 4368 6563 6b42 6f78 5479 7065  to</CheckBoxType
-000014f0: 3e0d 0a09 0909 0909 3c43 6f6e 7465 7874  >.......<Context
-00001500: 4d65 6e75 206e 616d 653d 22d0 9fd0 bed0  Menu name=".....
-00001510: b4d0 bcd0 b5d0 bdd0 b8d1 82d1 8cd0 9fd1  ................
-00001520: 83d1 82d1 8c52 756e 6e65 72d0 9ad0 bed0  .....Runner.....
-00001530: bdd1 82d0 b5d0 bad1 81d1 82d0 bdd0 bed0  ................
-00001540: b5d0 9cd0 b5d0 bdd1 8e22 2069 643d 2234  ........." id="4
-00001550: 3222 2f3e 0d0a 0909 0909 093c 4578 7465  2"/>.......<Exte
-00001560: 6e64 6564 546f 6f6c 7469 7020 6e61 6d65  ndedTooltip name
-00001570: 3d22 d09f d0be d0b4 d0bc d0b5 d0bd d0b8  ="..............
-00001580: d182 d18c d09f d183 d182 d18c 5275 6e6e  ............Runn
-00001590: 6572 d0a0 d0b0 d181 d188 d0b8 d180 d0b5  er..............
-000015a0: d0bd d0bd d0b0 d18f d09f d0be d0b4 d181  ................
-000015b0: d0ba d0b0 d0b7 d0ba d0b0 2220 6964 3d22  .........." id="
-000015c0: 3433 222f 3e0d 0a09 0909 093c 2f43 6865  43"/>......</Che
-000015d0: 636b 426f 7846 6965 6c64 3e0d 0a09 0909  ckBoxField>.....
-000015e0: 093c 4368 6563 6b42 6f78 4669 656c 6420  .<CheckBoxField 
-000015f0: 6e61 6d65 3d22 d09e d182 d0bb d0b0 d0b4  name="..........
-00001600: d0ba d0b0 2220 6964 3d22 3135 223e 0d0a  ...." id="15">..
-00001610: 0909 0909 093c 4461 7461 5061 7468 3ed0  .....<DataPath>.
-00001620: 9ed1 82d0 bbd0 b0d0 b4d0 bad0 b03c 2f44  .............</D
-00001630: 6174 6150 6174 683e 0d0a 0909 0909 093c  ataPath>.......<
-00001640: 4368 6563 6b42 6f78 5479 7065 3e41 7574  CheckBoxType>Aut
-00001650: 6f3c 2f43 6865 636b 426f 7854 7970 653e  o</CheckBoxType>
-00001660: 0d0a 0909 0909 093c 436f 6e74 6578 744d  .......<ContextM
-00001670: 656e 7520 6e61 6d65 3d22 d09e d182 d0bb  enu name="......
-00001680: d0b0 d0b4 d0ba d0b0 d09a d0be d0bd d182  ................
-00001690: d0b5 d0ba d181 d182 d0bd d0be d0b5 d09c  ................
-000016a0: d0b5 d0bd d18e 2220 6964 3d22 3136 222f  ......" id="16"/
-000016b0: 3e0d 0a09 0909 0909 3c45 7874 656e 6465  >.......<Extende
-000016c0: 6454 6f6f 6c74 6970 206e 616d 653d 22d0  dTooltip name=".
-000016d0: 9ed1 82d0 bbd0 b0d0 b4d0 bad0 b0d0 a0d0  ................
-000016e0: b0d1 81d1 88d0 b8d1 80d0 b5d0 bdd0 bdd0  ................
-000016f0: b0d1 8fd0 9fd0 bed0 b4d1 81d0 bad0 b0d0  ................
-00001700: b7d0 bad0 b022 2069 643d 2233 3322 2f3e  ....." id="33"/>
-00001710: 0d0a 0909 0909 3c2f 4368 6563 6b42 6f78  ......</CheckBox
-00001720: 4669 656c 643e 0d0a 0909 093c 2f43 6869  Field>.....</Chi
-00001730: 6c64 4974 656d 733e 0d0a 0909 3c2f 5573  ldItems>....</Us
-00001740: 7561 6c47 726f 7570 3e0d 0a09 093c 4275  ualGroup>....<Bu
-00001750: 7474 6f6e 206e 616d 653d 22d0 a1d0 b4d0  tton name=".....
-00001760: b5d0 bbd0 b0d1 82d1 8c22 2069 643d 2231  ........." id="1
-00001770: 3022 3e0d 0a09 0909 3c54 7970 653e 5573  0">.....<Type>Us
-00001780: 7561 6c42 7574 746f 6e3c 2f54 7970 653e  ualButton</Type>
-00001790: 0d0a 0909 093c 436f 6d6d 616e 644e 616d  .....<CommandNam
-000017a0: 653e 466f 726d 2e43 6f6d 6d61 6e64 2ed0  e>Form.Command..
-000017b0: a1d0 b4d0 b5d0 bbd0 b0d1 82d1 8c3c 2f43  .............</C
-000017c0: 6f6d 6d61 6e64 4e61 6d65 3e0d 0a09 0909  ommandName>.....
-000017d0: 3c45 7874 656e 6465 6454 6f6f 6c74 6970  <ExtendedTooltip
-000017e0: 206e 616d 653d 22d0 a1d0 b4d0 b5d0 bbd0   name=".........
-000017f0: b0d1 82d1 8cd0 a0d0 b0d1 81d1 88d0 b8d1  ................
-00001800: 80d0 b5d0 bdd0 bdd0 b0d1 8fd0 9fd0 bed0  ................
-00001810: b4d1 81d0 bad0 b0d0 b7d0 bad0 b022 2069  ............." i
-00001820: 643d 2233 3422 2f3e 0d0a 0909 3c2f 4275  d="34"/>....</Bu
-00001830: 7474 6f6e 3e0d 0a09 3c2f 4368 696c 6449  tton>...</ChildI
-00001840: 7465 6d73 3e0d 0a09 3c41 7474 7269 6275  tems>...<Attribu
-00001850: 7465 733e 0d0a 0909 3c41 7474 7269 6275  tes>....<Attribu
-00001860: 7465 206e 616d 653d 22d0 9ed0 b1d1 8ad0  te name=".......
-00001870: b5d0 bad1 8222 2069 643d 2231 223e 0d0a  ....." id="1">..
-00001880: 0909 093c 5479 7065 3e0d 0a09 0909 093c  ...<Type>......<
-00001890: 7638 3a54 7970 653e 6366 673a 4578 7465  v8:Type>cfg:Exte
-000018a0: 726e 616c 4461 7461 5072 6f63 6573 736f  rnalDataProcesso
-000018b0: 724f 626a 6563 742e 5275 6e6e 6572 3143  rObject.Runner1C
-000018c0: 3c2f 7638 3a54 7970 653e 0d0a 0909 093c  </v8:Type>.....<
-000018d0: 2f54 7970 653e 0d0a 0909 093c 4d61 696e  /Type>.....<Main
-000018e0: 4174 7472 6962 7574 653e 7472 7565 3c2f  Attribute>true</
-000018f0: 4d61 696e 4174 7472 6962 7574 653e 0d0a  MainAttribute>..
-00001900: 0909 3c2f 4174 7472 6962 7574 653e 0d0a  ..</Attribute>..
-00001910: 0909 3c41 7474 7269 6275 7465 206e 616d  ..<Attribute nam
-00001920: 653d 22d0 9fd1 83d1 82d1 8cd0 9ad0 9fd0  e=".............
-00001930: bbd0 b0d1 82d1 84d0 bed1 80d0 bcd0 b522  ..............."
-00001940: 2069 643d 2232 223e 0d0a 0909 093c 5469   id="2">.....<Ti
-00001950: 746c 653e 0d0a 0909 0909 3c76 383a 6974  tle>......<v8:it
-00001960: 656d 3e0d 0a09 0909 0909 3c76 383a 6c61  em>.......<v8:la
-00001970: 6e67 3e72 753c 2f76 383a 6c61 6e67 3e0d  ng>ru</v8:lang>.
-00001980: 0a09 0909 0909 3c76 383a 636f 6e74 656e  ......<v8:conten
-00001990: 743e d09f d183 d182 d18c 20d0 ba20 d0bf  t>........ .. ..
-000019a0: d0bb d0b0 d182 d184 d0be d180 d0bc d0b5  ................
-000019b0: 3c2f 7638 3a63 6f6e 7465 6e74 3e0d 0a09  </v8:content>...
-000019c0: 0909 093c 2f76 383a 6974 656d 3e0d 0a09  ...</v8:item>...
-000019d0: 0909 3c2f 5469 746c 653e 0d0a 0909 093c  ..</Title>.....<
-000019e0: 5479 7065 3e0d 0a09 0909 093c 7638 3a54  Type>......<v8:T
-000019f0: 7970 653e 7873 3a73 7472 696e 673c 2f76  ype>xs:string</v
-00001a00: 383a 5479 7065 3e0d 0a09 0909 093c 7638  8:Type>......<v8
-00001a10: 3a53 7472 696e 6751 7561 6c69 6669 6572  :StringQualifier
-00001a20: 733e 0d0a 0909 0909 093c 7638 3a4c 656e  s>.......<v8:Len
-00001a30: 6774 683e 303c 2f76 383a 4c65 6e67 7468  gth>0</v8:Length
-00001a40: 3e0d 0a09 0909 0909 3c76 383a 416c 6c6f  >.......<v8:Allo
-00001a50: 7765 644c 656e 6774 683e 5661 7269 6162  wedLength>Variab
-00001a60: 6c65 3c2f 7638 3a41 6c6c 6f77 6564 4c65  le</v8:AllowedLe
-00001a70: 6e67 7468 3e0d 0a09 0909 093c 2f76 383a  ngth>......</v8:
-00001a80: 5374 7269 6e67 5175 616c 6966 6965 7273  StringQualifiers
-00001a90: 3e0d 0a09 0909 3c2f 5479 7065 3e0d 0a09  >.....</Type>...
-00001aa0: 0909 3c46 696c 6c43 6865 636b 3e53 686f  ..<FillCheck>Sho
-00001ab0: 7745 7272 6f72 3c2f 4669 6c6c 4368 6563  wError</FillChec
-00001ac0: 6b3e 0d0a 0909 3c2f 4174 7472 6962 7574  k>....</Attribut
-00001ad0: 653e 0d0a 0909 3c41 7474 7269 6275 7465  e>....<Attribute
-00001ae0: 206e 616d 653d 22d0 a1d1 82d1 80d0 bed0   name=".........
-00001af0: bad0 b0d0 9fd0 bed0 b4d0 bad0 bbd1 8ed1  ................
-00001b00: 87d0 b5d0 bdd0 b8d1 8fd0 9ad0 91d0 b0d0  ................
-00001b10: b7d0 b522 2069 643d 2233 223e 0d0a 0909  ..." id="3">....
-00001b20: 093c 5469 746c 653e 0d0a 0909 0909 3c76  .<Title>......<v
-00001b30: 383a 6974 656d 3e0d 0a09 0909 0909 3c76  8:item>.......<v
-00001b40: 383a 6c61 6e67 3e72 753c 2f76 383a 6c61  8:lang>ru</v8:la
-00001b50: 6e67 3e0d 0a09 0909 0909 3c76 383a 636f  ng>.......<v8:co
-00001b60: 6e74 656e 743e d0a1 d182 d180 d0be d0ba  ntent>..........
-00001b70: d0b0 20d0 bfd0 bed0 b4d0 bad0 bbd1 8ed1  .. .............
-00001b80: 87d0 b5d0 bdd0 b8d1 8f3c 2f76 383a 636f  .........</v8:co
-00001b90: 6e74 656e 743e 0d0a 0909 0909 3c2f 7638  ntent>......</v8
-00001ba0: 3a69 7465 6d3e 0d0a 0909 093c 2f54 6974  :item>.....</Tit
-00001bb0: 6c65 3e0d 0a09 0909 3c54 7970 653e 0d0a  le>.....<Type>..
-00001bc0: 0909 0909 3c76 383a 5479 7065 3e78 733a  ....<v8:Type>xs:
-00001bd0: 7374 7269 6e67 3c2f 7638 3a54 7970 653e  string</v8:Type>
-00001be0: 0d0a 0909 0909 3c76 383a 5374 7269 6e67  ......<v8:String
-00001bf0: 5175 616c 6966 6965 7273 3e0d 0a09 0909  Qualifiers>.....
-00001c00: 0909 3c76 383a 4c65 6e67 7468 3e30 3c2f  ..<v8:Length>0</
-00001c10: 7638 3a4c 656e 6774 683e 0d0a 0909 0909  v8:Length>......
-00001c20: 093c 7638 3a41 6c6c 6f77 6564 4c65 6e67  .<v8:AllowedLeng
-00001c30: 7468 3e56 6172 6961 626c 653c 2f76 383a  th>Variable</v8:
-00001c40: 416c 6c6f 7765 644c 656e 6774 683e 0d0a  AllowedLength>..
-00001c50: 0909 0909 3c2f 7638 3a53 7472 696e 6751  ....</v8:StringQ
-00001c60: 7561 6c69 6669 6572 733e 0d0a 0909 093c  ualifiers>.....<
-00001c70: 2f54 7970 653e 0d0a 0909 093c 4669 6c6c  /Type>.....<Fill
-00001c80: 4368 6563 6b3e 5368 6f77 4572 726f 723c  Check>ShowError<
-00001c90: 2f46 696c 6c43 6865 636b 3e0d 0a09 093c  /FillCheck>....<
-00001ca0: 2f41 7474 7269 6275 7465 3e0d 0a09 093c  /Attribute>....<
-00001cb0: 4174 7472 6962 7574 6520 6e61 6d65 3d22  Attribute name="
-00001cc0: d09f d0b0 d0bf d0ba d0b0 d092 d18b d0b3  ................
-00001cd0: d180 d183 d0b7 d0ba d0b8 2220 6964 3d22  .........." id="
-00001ce0: 3422 3e0d 0a09 0909 3c54 6974 6c65 3e0d  4">.....<Title>.
-00001cf0: 0a09 0909 093c 7638 3a69 7465 6d3e 0d0a  .....<v8:item>..
-00001d00: 0909 0909 093c 7638 3a6c 616e 673e 7275  .....<v8:lang>ru
-00001d10: 3c2f 7638 3a6c 616e 673e 0d0a 0909 0909  </v8:lang>......
-00001d20: 093c 7638 3a63 6f6e 7465 6e74 3ed0 9fd0  .<v8:content>...
-00001d30: b0d0 bfd0 bad0 b020 d0b2 d18b d0b3 d180  ....... ........
-00001d40: d183 d0b7 d0ba d0b8 3c2f 7638 3a63 6f6e  ........</v8:con
-00001d50: 7465 6e74 3e0d 0a09 0909 093c 2f76 383a  tent>......</v8:
-00001d60: 6974 656d 3e0d 0a09 0909 3c2f 5469 746c  item>.....</Titl
-00001d70: 653e 0d0a 0909 093c 5479 7065 3e0d 0a09  e>.....<Type>...
-00001d80: 0909 093c 7638 3a54 7970 653e 7873 3a73  ...<v8:Type>xs:s
-00001d90: 7472 696e 673c 2f76 383a 5479 7065 3e0d  tring</v8:Type>.
-00001da0: 0a09 0909 093c 7638 3a53 7472 696e 6751  .....<v8:StringQ
-00001db0: 7561 6c69 6669 6572 733e 0d0a 0909 0909  ualifiers>......
-00001dc0: 093c 7638 3a4c 656e 6774 683e 303c 2f76  .<v8:Length>0</v
-00001dd0: 383a 4c65 6e67 7468 3e0d 0a09 0909 0909  8:Length>.......
-00001de0: 3c76 383a 416c 6c6f 7765 644c 656e 6774  <v8:AllowedLengt
-00001df0: 683e 5661 7269 6162 6c65 3c2f 7638 3a41  h>Variable</v8:A
-00001e00: 6c6c 6f77 6564 4c65 6e67 7468 3e0d 0a09  llowedLength>...
-00001e10: 0909 093c 2f76 383a 5374 7269 6e67 5175  ...</v8:StringQu
-00001e20: 616c 6966 6965 7273 3e0d 0a09 0909 3c2f  alifiers>.....</
-00001e30: 5479 7065 3e0d 0a09 0909 3c46 696c 6c43  Type>.....<FillC
-00001e40: 6865 636b 3e53 686f 7745 7272 6f72 3c2f  heck>ShowError</
-00001e50: 4669 6c6c 4368 6563 6b3e 0d0a 0909 093c  FillCheck>.....<
-00001e60: 5361 7665 3e0d 0a09 0909 093c 4669 656c  Save>......<Fiel
-00001e70: 643e d09f d0b0 d0bf d0ba d0b0 d092 d18b  d>..............
-00001e80: d0b3 d180 d183 d0b7 d0ba d0b8 3c2f 4669  ............</Fi
-00001e90: 656c 643e 0d0a 0909 093c 2f53 6176 653e  eld>.....</Save>
-00001ea0: 0d0a 0909 3c2f 4174 7472 6962 7574 653e  ....</Attribute>
-00001eb0: 0d0a 0909 3c41 7474 7269 6275 7465 206e  ....<Attribute n
-00001ec0: 616d 653d 22d0 a2d0 b8d0 bfd0 9ed0 bfd0  ame="...........
-00001ed0: b5d1 80d0 b0d1 86d0 b8d0 b822 2069 643d  ..........." id=
-00001ee0: 2235 223e 0d0a 0909 093c 5469 746c 653e  "5">.....<Title>
-00001ef0: 0d0a 0909 0909 3c76 383a 6974 656d 3e0d  ......<v8:item>.
-00001f00: 0a09 0909 0909 3c76 383a 6c61 6e67 3e72  ......<v8:lang>r
-00001f10: 753c 2f76 383a 6c61 6e67 3e0d 0a09 0909  u</v8:lang>.....
-00001f20: 0909 3c76 383a 636f 6e74 656e 743e d0a2  ..<v8:content>..
-00001f30: d0b8 d0bf 20d0 bed0 bfd0 b5d1 80d0 b0d1  .... ...........
-00001f40: 86d0 b8d0 b83c 2f76 383a 636f 6e74 656e  .....</v8:conten
-00001f50: 743e 0d0a 0909 0909 3c2f 7638 3a69 7465  t>......</v8:ite
-00001f60: 6d3e 0d0a 0909 093c 2f54 6974 6c65 3e0d  m>.....</Title>.
-00001f70: 0a09 0909 3c54 7970 653e 0d0a 0909 0909  ....<Type>......
-00001f80: 3c76 383a 5479 7065 3e78 733a 7374 7269  <v8:Type>xs:stri
-00001f90: 6e67 3c2f 7638 3a54 7970 653e 0d0a 0909  ng</v8:Type>....
-00001fa0: 0909 3c76 383a 5374 7269 6e67 5175 616c  ..<v8:StringQual
-00001fb0: 6966 6965 7273 3e0d 0a09 0909 0909 3c76  ifiers>.......<v
-00001fc0: 383a 4c65 6e67 7468 3e30 3c2f 7638 3a4c  8:Length>0</v8:L
-00001fd0: 656e 6774 683e 0d0a 0909 0909 093c 7638  ength>.......<v8
-00001fe0: 3a41 6c6c 6f77 6564 4c65 6e67 7468 3e56  :AllowedLength>V
-00001ff0: 6172 6961 626c 653c 2f76 383a 416c 6c6f  ariable</v8:Allo
-00002000: 7765 644c 656e 6774 683e 0d0a 0909 0909  wedLength>......
-00002010: 3c2f 7638 3a53 7472 696e 6751 7561 6c69  </v8:StringQuali
-00002020: 6669 6572 733e 0d0a 0909 093c 2f54 7970  fiers>.....</Typ
-00002030: 653e 0d0a 0909 093c 4669 6c6c 4368 6563  e>.....<FillChec
-00002040: 6b3e 5368 6f77 4572 726f 723c 2f46 696c  k>ShowError</Fil
-00002050: 6c43 6865 636b 3e0d 0a09 0909 3c53 6176  lCheck>.....<Sav
-00002060: 653e 0d0a 0909 0909 3c46 6965 6c64 3ed0  e>......<Field>.
-00002070: a2d0 b8d0 bfd0 9ed0 bfd0 b5d1 80d0 b0d1  ................
-00002080: 86d0 b8d0 b83c 2f46 6965 6c64 3e0d 0a09  .....</Field>...
-00002090: 0909 3c2f 5361 7665 3e0d 0a09 093c 2f41  ..</Save>....</A
-000020a0: 7474 7269 6275 7465 3e0d 0a09 093c 4174  ttribute>....<At
-000020b0: 7472 6962 7574 6520 6e61 6d65 3d22 d09e  tribute name="..
-000020c0: d182 d0bb d0b0 d0b4 d0ba d0b0 2220 6964  ............" id
-000020d0: 3d22 3722 3e0d 0a09 0909 3c54 6974 6c65  ="7">.....<Title
-000020e0: 3e0d 0a09 0909 093c 7638 3a69 7465 6d3e  >......<v8:item>
-000020f0: 0d0a 0909 0909 093c 7638 3a6c 616e 673e  .......<v8:lang>
-00002100: 7275 3c2f 7638 3a6c 616e 673e 0d0a 0909  ru</v8:lang>....
-00002110: 0909 093c 7638 3a63 6f6e 7465 6e74 3ed0  ...<v8:content>.
-00002120: 9ed1 82d0 bbd0 b0d0 b4d0 bad0 b03c 2f76  .............</v
-00002130: 383a 636f 6e74 656e 743e 0d0a 0909 0909  8:content>......
-00002140: 3c2f 7638 3a69 7465 6d3e 0d0a 0909 093c  </v8:item>.....<
-00002150: 2f54 6974 6c65 3e0d 0a09 0909 3c54 7970  /Title>.....<Typ
-00002160: 653e 0d0a 0909 0909 3c76 383a 5479 7065  e>......<v8:Type
-00002170: 3e78 733a 626f 6f6c 6561 6e3c 2f76 383a  >xs:boolean</v8:
-00002180: 5479 7065 3e0d 0a09 0909 3c2f 5479 7065  Type>.....</Type
-00002190: 3e0d 0a09 093c 2f41 7474 7269 6275 7465  >....</Attribute
-000021a0: 3e0d 0a09 093c 4174 7472 6962 7574 6520  >....<Attribute 
-000021b0: 6e61 6d65 3d22 d09b d0be d0b3 d0b8 d0bd  name="..........
-000021c0: 2220 6964 3d22 3822 3e0d 0a09 0909 3c54  " id="8">.....<T
-000021d0: 6974 6c65 3e0d 0a09 0909 093c 7638 3a69  itle>......<v8:i
-000021e0: 7465 6d3e 0d0a 0909 0909 093c 7638 3a6c  tem>.......<v8:l
-000021f0: 616e 673e 7275 3c2f 7638 3a6c 616e 673e  ang>ru</v8:lang>
-00002200: 0d0a 0909 0909 093c 7638 3a63 6f6e 7465  .......<v8:conte
-00002210: 6e74 3ed0 9bd0 bed0 b3d0 b8d0 bd3c 2f76  nt>..........</v
-00002220: 383a 636f 6e74 656e 743e 0d0a 0909 0909  8:content>......
-00002230: 3c2f 7638 3a69 7465 6d3e 0d0a 0909 093c  </v8:item>.....<
-00002240: 2f54 6974 6c65 3e0d 0a09 0909 3c54 7970  /Title>.....<Typ
-00002250: 653e 0d0a 0909 0909 3c76 383a 5479 7065  e>......<v8:Type
-00002260: 3e78 733a 7374 7269 6e67 3c2f 7638 3a54  >xs:string</v8:T
-00002270: 7970 653e 0d0a 0909 0909 3c76 383a 5374  ype>......<v8:St
-00002280: 7269 6e67 5175 616c 6966 6965 7273 3e0d  ringQualifiers>.
-00002290: 0a09 0909 0909 3c76 383a 4c65 6e67 7468  ......<v8:Length
-000022a0: 3e30 3c2f 7638 3a4c 656e 6774 683e 0d0a  >0</v8:Length>..
-000022b0: 0909 0909 093c 7638 3a41 6c6c 6f77 6564  .....<v8:Allowed
-000022c0: 4c65 6e67 7468 3e56 6172 6961 626c 653c  Length>Variable<
-000022d0: 2f76 383a 416c 6c6f 7765 644c 656e 6774  /v8:AllowedLengt
-000022e0: 683e 0d0a 0909 0909 3c2f 7638 3a53 7472  h>......</v8:Str
-000022f0: 696e 6751 7561 6c69 6669 6572 733e 0d0a  ingQualifiers>..
-00002300: 0909 093c 2f54 7970 653e 0d0a 0909 3c2f  ...</Type>....</
-00002310: 4174 7472 6962 7574 653e 0d0a 0909 3c41  Attribute>....<A
-00002320: 7474 7269 6275 7465 206e 616d 653d 22d0  ttribute name=".
-00002330: 9fd0 b0d1 80d0 bed0 bbd1 8c22 2069 643d  ..........." id=
-00002340: 2239 223e 0d0a 0909 093c 5469 746c 653e  "9">.....<Title>
-00002350: 0d0a 0909 0909 3c76 383a 6974 656d 3e0d  ......<v8:item>.
-00002360: 0a09 0909 0909 3c76 383a 6c61 6e67 3e72  ......<v8:lang>r
-00002370: 753c 2f76 383a 6c61 6e67 3e0d 0a09 0909  u</v8:lang>.....
-00002380: 0909 3c76 383a 636f 6e74 656e 743e d09f  ..<v8:content>..
-00002390: d0b0 d180 d0be d0bb d18c 3c2f 7638 3a63  ..........</v8:c
-000023a0: 6f6e 7465 6e74 3e0d 0a09 0909 093c 2f76  ontent>......</v
-000023b0: 383a 6974 656d 3e0d 0a09 0909 3c2f 5469  8:item>.....</Ti
-000023c0: 746c 653e 0d0a 0909 093c 5479 7065 3e0d  tle>.....<Type>.
-000023d0: 0a09 0909 093c 7638 3a54 7970 653e 7873  .....<v8:Type>xs
-000023e0: 3a73 7472 696e 673c 2f76 383a 5479 7065  :string</v8:Type
-000023f0: 3e0d 0a09 0909 093c 7638 3a53 7472 696e  >......<v8:Strin
-00002400: 6751 7561 6c69 6669 6572 733e 0d0a 0909  gQualifiers>....
-00002410: 0909 093c 7638 3a4c 656e 6774 683e 303c  ...<v8:Length>0<
-00002420: 2f76 383a 4c65 6e67 7468 3e0d 0a09 0909  /v8:Length>.....
-00002430: 0909 3c76 383a 416c 6c6f 7765 644c 656e  ..<v8:AllowedLen
-00002440: 6774 683e 5661 7269 6162 6c65 3c2f 7638  gth>Variable</v8
-00002450: 3a41 6c6c 6f77 6564 4c65 6e67 7468 3e0d  :AllowedLength>.
-00002460: 0a09 0909 093c 2f76 383a 5374 7269 6e67  .....</v8:String
-00002470: 5175 616c 6966 6965 7273 3e0d 0a09 0909  Qualifiers>.....
-00002480: 3c2f 5479 7065 3e0d 0a09 0909 3c53 6176  </Type>.....<Sav
-00002490: 653e 0d0a 0909 0909 3c46 6965 6c64 3ed0  e>......<Field>.
-000024a0: 9fd0 b0d1 80d0 bed0 bbd1 8c3c 2f46 6965  ...........</Fie
-000024b0: 6c64 3e0d 0a09 0909 3c2f 5361 7665 3e0d  ld>.....</Save>.
-000024c0: 0a09 093c 2f41 7474 7269 6275 7465 3e0d  ...</Attribute>.
-000024d0: 0a09 093c 4174 7472 6962 7574 6520 6e61  ...<Attribute na
-000024e0: 6d65 3d22 d09a d0be d0b4 d0a0 d0b0 d0b7  me="............
-000024f0: d0b1 d0bb d0be d0ba d0b8 d180 d0be d0b2  ................
-00002500: d0ba d0b8 2220 6964 3d22 3130 223e 0d0a  ...." id="10">..
-00002510: 0909 093c 5469 746c 653e 0d0a 0909 0909  ...<Title>......
-00002520: 3c76 383a 6974 656d 3e0d 0a09 0909 0909  <v8:item>.......
-00002530: 3c76 383a 6c61 6e67 3e72 753c 2f76 383a  <v8:lang>ru</v8:
-00002540: 6c61 6e67 3e0d 0a09 0909 0909 3c76 383a  lang>.......<v8:
-00002550: 636f 6e74 656e 743e d09a d0be d0b4 20d1  content>...... .
-00002560: 80d0 b0d0 b7d0 b1d0 bbd0 bed0 bad0 b8d1  ................
-00002570: 80d0 bed0 b2d0 bad0 b83c 2f76 383a 636f  .........</v8:co
-00002580: 6e74 656e 743e 0d0a 0909 0909 3c2f 7638  ntent>......</v8
-00002590: 3a69 7465 6d3e 0d0a 0909 093c 2f54 6974  :item>.....</Tit
-000025a0: 6c65 3e0d 0a09 0909 3c54 7970 653e 0d0a  le>.....<Type>..
-000025b0: 0909 0909 3c76 383a 5479 7065 3e78 733a  ....<v8:Type>xs:
-000025c0: 7374 7269 6e67 3c2f 7638 3a54 7970 653e  string</v8:Type>
-000025d0: 0d0a 0909 0909 3c76 383a 5374 7269 6e67  ......<v8:String
-000025e0: 5175 616c 6966 6965 7273 3e0d 0a09 0909  Qualifiers>.....
-000025f0: 0909 3c76 383a 4c65 6e67 7468 3e31 303c  ..<v8:Length>10<
-00002600: 2f76 383a 4c65 6e67 7468 3e0d 0a09 0909  /v8:Length>.....
-00002610: 0909 3c76 383a 416c 6c6f 7765 644c 656e  ..<v8:AllowedLen
-00002620: 6774 683e 5661 7269 6162 6c65 3c2f 7638  gth>Variable</v8
-00002630: 3a41 6c6c 6f77 6564 4c65 6e67 7468 3e0d  :AllowedLength>.
-00002640: 0a09 0909 093c 2f76 383a 5374 7269 6e67  .....</v8:String
-00002650: 5175 616c 6966 6965 7273 3e0d 0a09 0909  Qualifiers>.....
-00002660: 3c2f 5479 7065 3e0d 0a09 093c 2f41 7474  </Type>....</Att
-00002670: 7269 6275 7465 3e0d 0a09 093c 4174 7472  ribute>....<Attr
-00002680: 6962 7574 6520 6e61 6d65 3d22 d092 d18b  ibute name="....
-00002690: d0b3 d180 d183 d0b6 d0b0 d182 d18c d0a0  ................
-000026a0: d0b0 d181 d188 d0b8 d180 d0b5 d0bd d0b8  ................
-000026b0: d18f d092 5370 6563 2220 6964 3d22 3131  ....Spec" id="11
-000026c0: 223e 0d0a 0909 093c 5469 746c 653e 0d0a  ">.....<Title>..
-000026d0: 0909 0909 3c76 383a 6974 656d 3e0d 0a09  ....<v8:item>...
-000026e0: 0909 0909 3c76 383a 6c61 6e67 3e72 753c  ....<v8:lang>ru<
-000026f0: 2f76 383a 6c61 6e67 3e0d 0a09 0909 0909  /v8:lang>.......
-00002700: 3c76 383a 636f 6e74 656e 743e d092 d18b  <v8:content>....
-00002710: d0b3 d180 d183 d0b6 d0b0 d182 d18c 20d1  .............. .
-00002720: 80d0 b0d1 81d1 88d0 b8d1 80d0 b5d0 bdd0  ................
-00002730: b8d1 8f20 d0b2 2073 7065 633c 2f76 383a  ... .. spec</v8:
-00002740: 636f 6e74 656e 743e 0d0a 0909 0909 3c2f  content>......</
-00002750: 7638 3a69 7465 6d3e 0d0a 0909 093c 2f54  v8:item>.....</T
-00002760: 6974 6c65 3e0d 0a09 0909 3c54 7970 653e  itle>.....<Type>
-00002770: 0d0a 0909 0909 3c76 383a 5479 7065 3e78  ......<v8:Type>x
-00002780: 733a 626f 6f6c 6561 6e3c 2f76 383a 5479  s:boolean</v8:Ty
-00002790: 7065 3e0d 0a09 0909 3c2f 5479 7065 3e0d  pe>.....</Type>.
-000027a0: 0a09 093c 2f41 7474 7269 6275 7465 3e0d  ...</Attribute>.
-000027b0: 0a09 093c 4174 7472 6962 7574 6520 6e61  ...<Attribute na
-000027c0: 6d65 3d22 d09f d0be d0b4 d0bc d0b5 d0bd  me="............
-000027d0: d0b8 d182 d18c d09f d183 d182 d18c 5275  ..............Ru
-000027e0: 6e6e 6572 2220 6964 3d22 3622 3e0d 0a09  nner" id="6">...
-000027f0: 0909 3c54 6974 6c65 3e0d 0a09 0909 093c  ..<Title>......<
-00002800: 7638 3a69 7465 6d3e 0d0a 0909 0909 093c  v8:item>.......<
-00002810: 7638 3a6c 616e 673e 7275 3c2f 7638 3a6c  v8:lang>ru</v8:l
-00002820: 616e 673e 0d0a 0909 0909 093c 7638 3a63  ang>.......<v8:c
-00002830: 6f6e 7465 6e74 3ed0 9fd0 bed0 b4d0 bcd0  ontent>.........
-00002840: b5d0 bdd0 b8d1 82d1 8c20 d0bf d183 d182  ......... ......
-00002850: d18c 2072 756e 6e65 723c 2f76 383a 636f  .. runner</v8:co
-00002860: 6e74 656e 743e 0d0a 0909 0909 3c2f 7638  ntent>......</v8
-00002870: 3a69 7465 6d3e 0d0a 0909 093c 2f54 6974  :item>.....</Tit
-00002880: 6c65 3e0d 0a09 0909 3c54 7970 653e 0d0a  le>.....<Type>..
-00002890: 0909 0909 3c76 383a 5479 7065 3e78 733a  ....<v8:Type>xs:
-000028a0: 626f 6f6c 6561 6e3c 2f76 383a 5479 7065  boolean</v8:Type
-000028b0: 3e0d 0a09 0909 3c2f 5479 7065 3e0d 0a09  >.....</Type>...
-000028c0: 093c 2f41 7474 7269 6275 7465 3e0d 0a09  .</Attribute>...
-000028d0: 3c2f 4174 7472 6962 7574 6573 3e0d 0a09  </Attributes>...
-000028e0: 3c43 6f6d 6d61 6e64 733e 0d0a 0909 3c43  <Commands>....<C
-000028f0: 6f6d 6d61 6e64 206e 616d 653d 22d0 a1d0  ommand name="...
-00002900: b4d0 b5d0 bbd0 b0d1 82d1 8c22 2069 643d  ..........." id=
-00002910: 2231 223e 0d0a 0909 093c 5469 746c 653e  "1">.....<Title>
-00002920: 0d0a 0909 0909 3c76 383a 6974 656d 3e0d  ......<v8:item>.
-00002930: 0a09 0909 0909 3c76 383a 6c61 6e67 3e72  ......<v8:lang>r
-00002940: 753c 2f76 383a 6c61 6e67 3e0d 0a09 0909  u</v8:lang>.....
-00002950: 0909 3c76 383a 636f 6e74 656e 743e d0a1  ..<v8:content>..
-00002960: d0b4 d0b5 d0bb d0b0 d182 d18c 3c2f 7638  ............</v8
-00002970: 3a63 6f6e 7465 6e74 3e0d 0a09 0909 093c  :content>......<
-00002980: 2f76 383a 6974 656d 3e0d 0a09 0909 3c2f  /v8:item>.....</
-00002990: 5469 746c 653e 0d0a 0909 093c 546f 6f6c  Title>.....<Tool
-000029a0: 5469 703e 0d0a 0909 0909 3c76 383a 6974  Tip>......<v8:it
-000029b0: 656d 3e0d 0a09 0909 0909 3c76 383a 6c61  em>.......<v8:la
-000029c0: 6e67 3e72 753c 2f76 383a 6c61 6e67 3e0d  ng>ru</v8:lang>.
-000029d0: 0a09 0909 0909 3c76 383a 636f 6e74 656e  ......<v8:conten
-000029e0: 743e d0a1 d0b4 d0b5 d0bb d0b0 d182 d18c  t>..............
-000029f0: 3c2f 7638 3a63 6f6e 7465 6e74 3e0d 0a09  </v8:content>...
-00002a00: 0909 093c 2f76 383a 6974 656d 3e0d 0a09  ...</v8:item>...
-00002a10: 0909 3c2f 546f 6f6c 5469 703e 0d0a 0909  ..</ToolTip>....
-00002a20: 093c 4163 7469 6f6e 3ed0 a1d0 b4d0 b5d0  .<Action>.......
-00002a30: bbd0 b0d1 82d1 8c3c 2f41 6374 696f 6e3e  .......</Action>
-00002a40: 0d0a 0909 093c 4375 7272 656e 7452 6f77  .....<CurrentRow
-00002a50: 5573 653e 446f 6e74 5573 653c 2f43 7572  Use>DontUse</Cur
-00002a60: 7265 6e74 526f 7755 7365 3e0d 0a09 093c  rentRowUse>....<
-00002a70: 2f43 6f6d 6d61 6e64 3e0d 0a09 3c2f 436f  /Command>...</Co
-00002a80: 6d6d 616e 6473 3e0d 0a3c 2f46 6f72 6d3e  mmands>..</Form>
+00000020: 2255 5446 2d38 223f 3e0a 3c46 6f72 6d20  "UTF-8"?>.<Form 
+00000030: 786d 6c6e 733d 2268 7474 703a 2f2f 7638  xmlns="http://v8
+00000040: 2e31 632e 7275 2f38 2e33 2f78 6366 2f6c  .1c.ru/8.3/xcf/l
+00000050: 6f67 666f 726d 2220 786d 6c6e 733a 6170  ogform" xmlns:ap
+00000060: 703d 2268 7474 703a 2f2f 7638 2e31 632e  p="http://v8.1c.
+00000070: 7275 2f38 2e32 2f6d 616e 6167 6564 2d61  ru/8.2/managed-a
+00000080: 7070 6c69 6361 7469 6f6e 2f63 6f72 6522  pplication/core"
+00000090: 2078 6d6c 6e73 3a63 6667 3d22 6874 7470   xmlns:cfg="http
+000000a0: 3a2f 2f76 382e 3163 2e72 752f 382e 312f  ://v8.1c.ru/8.1/
+000000b0: 6461 7461 2f65 6e74 6572 7072 6973 652f  data/enterprise/
+000000c0: 6375 7272 656e 742d 636f 6e66 6967 2220  current-config" 
+000000d0: 786d 6c6e 733a 6463 7363 6f72 3d22 6874  xmlns:dcscor="ht
+000000e0: 7470 3a2f 2f76 382e 3163 2e72 752f 382e  tp://v8.1c.ru/8.
+000000f0: 312f 6461 7461 2d63 6f6d 706f 7369 7469  1/data-compositi
+00000100: 6f6e 2d73 7973 7465 6d2f 636f 7265 2220  on-system/core" 
+00000110: 786d 6c6e 733a 6463 7373 6574 3d22 6874  xmlns:dcsset="ht
+00000120: 7470 3a2f 2f76 382e 3163 2e72 752f 382e  tp://v8.1c.ru/8.
+00000130: 312f 6461 7461 2d63 6f6d 706f 7369 7469  1/data-compositi
+00000140: 6f6e 2d73 7973 7465 6d2f 7365 7474 696e  on-system/settin
+00000150: 6773 2220 786d 6c6e 733a 656e 743d 2268  gs" xmlns:ent="h
+00000160: 7474 703a 2f2f 7638 2e31 632e 7275 2f38  ttp://v8.1c.ru/8
+00000170: 2e31 2f64 6174 612f 656e 7465 7270 7269  .1/data/enterpri
+00000180: 7365 2220 786d 6c6e 733a 6c66 3d22 6874  se" xmlns:lf="ht
+00000190: 7470 3a2f 2f76 382e 3163 2e72 752f 382e  tp://v8.1c.ru/8.
+000001a0: 322f 6d61 6e61 6765 642d 6170 706c 6963  2/managed-applic
+000001b0: 6174 696f 6e2f 6c6f 6766 6f72 6d22 2078  ation/logform" x
+000001c0: 6d6c 6e73 3a73 7479 6c65 3d22 6874 7470  mlns:style="http
+000001d0: 3a2f 2f76 382e 3163 2e72 752f 382e 312f  ://v8.1c.ru/8.1/
+000001e0: 6461 7461 2f75 692f 7374 796c 6522 2078  data/ui/style" x
+000001f0: 6d6c 6e73 3a73 7973 3d22 6874 7470 3a2f  mlns:sys="http:/
+00000200: 2f76 382e 3163 2e72 752f 382e 312f 6461  /v8.1c.ru/8.1/da
+00000210: 7461 2f75 692f 666f 6e74 732f 7379 7374  ta/ui/fonts/syst
+00000220: 656d 2220 786d 6c6e 733a 7638 3d22 6874  em" xmlns:v8="ht
+00000230: 7470 3a2f 2f76 382e 3163 2e72 752f 382e  tp://v8.1c.ru/8.
+00000240: 312f 6461 7461 2f63 6f72 6522 2078 6d6c  1/data/core" xml
+00000250: 6e73 3a76 3875 693d 2268 7474 703a 2f2f  ns:v8ui="http://
+00000260: 7638 2e31 632e 7275 2f38 2e31 2f64 6174  v8.1c.ru/8.1/dat
+00000270: 612f 7569 2220 786d 6c6e 733a 7765 623d  a/ui" xmlns:web=
+00000280: 2268 7474 703a 2f2f 7638 2e31 632e 7275  "http://v8.1c.ru
+00000290: 2f38 2e31 2f64 6174 612f 7569 2f63 6f6c  /8.1/data/ui/col
+000002a0: 6f72 732f 7765 6222 2078 6d6c 6e73 3a77  ors/web" xmlns:w
+000002b0: 696e 3d22 6874 7470 3a2f 2f76 382e 3163  in="http://v8.1c
+000002c0: 2e72 752f 382e 312f 6461 7461 2f75 692f  .ru/8.1/data/ui/
+000002d0: 636f 6c6f 7273 2f77 696e 646f 7773 2220  colors/windows" 
+000002e0: 786d 6c6e 733a 7872 3d22 6874 7470 3a2f  xmlns:xr="http:/
+000002f0: 2f76 382e 3163 2e72 752f 382e 332f 7863  /v8.1c.ru/8.3/xc
+00000300: 662f 7265 6164 6162 6c65 2220 786d 6c6e  f/readable" xmln
+00000310: 733a 7873 3d22 6874 7470 3a2f 2f77 7777  s:xs="http://www
+00000320: 2e77 332e 6f72 672f 3230 3031 2f58 4d4c  .w3.org/2001/XML
+00000330: 5363 6865 6d61 2220 786d 6c6e 733a 7873  Schema" xmlns:xs
+00000340: 693d 2268 7474 703a 2f2f 7777 772e 7733  i="http://www.w3
+00000350: 2e6f 7267 2f32 3030 312f 584d 4c53 6368  .org/2001/XMLSch
+00000360: 656d 612d 696e 7374 616e 6365 2220 7665  ema-instance" ve
+00000370: 7273 696f 6e3d 2232 2e36 223e 0a09 3c41  rsion="2.6">..<A
+00000380: 7574 6f53 6176 6544 6174 6149 6e53 6574  utoSaveDataInSet
+00000390: 7469 6e67 733e 5573 653c 2f41 7574 6f53  tings>Use</AutoS
+000003a0: 6176 6544 6174 6149 6e53 6574 7469 6e67  aveDataInSetting
+000003b0: 733e 0a09 3c56 6572 7469 6361 6c53 6372  s>..<VerticalScr
+000003c0: 6f6c 6c3e 7573 6549 664e 6563 6573 7361  oll>useIfNecessa
+000003d0: 7279 3c2f 5665 7274 6963 616c 5363 726f  ry</VerticalScro
+000003e0: 6c6c 3e0a 093c 4175 746f 436f 6d6d 616e  ll>..<AutoComman
+000003f0: 6442 6172 206e 616d 653d 22d0 a4d0 bed1  dBar name=".....
+00000400: 80d0 bcd0 b0d0 9ad0 bed0 bcd0 b0d0 bdd0  ................
+00000410: b4d0 bdd0 b0d1 8fd0 9fd0 b0d0 bdd0 b5d0  ................
+00000420: bbd1 8c22 2069 643d 222d 3122 3e0a 0909  ..." id="-1">...
+00000430: 3c41 7574 6f66 696c 6c3e 6661 6c73 653c  <Autofill>false<
+00000440: 2f41 7574 6f66 696c 6c3e 0a09 3c2f 4175  /Autofill>..</Au
+00000450: 746f 436f 6d6d 616e 6442 6172 3e0a 093c  toCommandBar>..<
+00000460: 4576 656e 7473 3e0a 0909 3c45 7665 6e74  Events>...<Event
+00000470: 206e 616d 653d 224f 6e4f 7065 6e22 3ed0   name="OnOpen">.
+00000480: 9fd1 80d0 b8d0 9ed1 82d0 bad1 80d1 8bd1  ................
+00000490: 82d0 b8d0 b83c 2f45 7665 6e74 3e0a 0909  .....</Event>...
+000004a0: 3c45 7665 6e74 206e 616d 653d 2246 696c  <Event name="Fil
+000004b0: 6c43 6865 636b 5072 6f63 6573 7369 6e67  lCheckProcessing
+000004c0: 4174 5365 7276 6572 223e d09e d0b1 d180  AtServer">......
+000004d0: d0b0 d0b1 d0be d182 d0ba d0b0 d09f d180  ................
+000004e0: d0be d0b2 d0b5 d180 d0ba d0b8 d097 d0b0  ................
+000004f0: d0bf d0be d0bb d0bd d0b5 d0bd d0b8 d18f  ................
+00000500: d09d d0b0 d0a1 d0b5 d180 d0b2 d0b5 d180  ................
+00000510: d0b5 3c2f 4576 656e 743e 0a09 3c2f 4576  ..</Event>..</Ev
+00000520: 656e 7473 3e0a 093c 4368 696c 6449 7465  ents>..<ChildIte
+00000530: 6d73 3e0a 0909 3c49 6e70 7574 4669 656c  ms>...<InputFiel
+00000540: 6420 6e61 6d65 3d22 d0a2 d0b8 d0bf d09e  d name="........
+00000550: d0bf d0b5 d180 d0b0 d186 d0b8 d0b8 2220  .............." 
+00000560: 6964 3d22 3132 223e 0a09 0909 3c44 6174  id="12">....<Dat
+00000570: 6150 6174 683e d0a2 d0b8 d0bf d09e d0bf  aPath>..........
+00000580: d0b5 d180 d0b0 d186 d0b8 d0b8 3c2f 4461  ............</Da
+00000590: 7461 5061 7468 3e0a 0909 093c 4c69 7374  taPath>....<List
+000005a0: 4368 6f69 6365 4d6f 6465 3e74 7275 653c  ChoiceMode>true<
+000005b0: 2f4c 6973 7443 686f 6963 654d 6f64 653e  /ListChoiceMode>
+000005c0: 0a09 0909 3c43 6f6e 7465 7874 4d65 6e75  ....<ContextMenu
+000005d0: 206e 616d 653d 22d0 a2d0 b8d0 bfd0 9ed0   name=".........
+000005e0: bfd0 b5d1 80d0 b0d1 86d0 b8d0 b8d0 9ad0  ................
+000005f0: bed0 bdd1 82d0 b5d0 bad1 81d1 82d0 bdd0  ................
+00000600: bed0 b5d0 9cd0 b5d0 bdd1 8e22 2069 643d  ..........." id=
+00000610: 2231 3322 2f3e 0a09 0909 3c45 7874 656e  "13"/>....<Exten
+00000620: 6465 6454 6f6f 6c74 6970 206e 616d 653d  dedTooltip name=
+00000630: 22d0 a2d0 b8d0 bfd0 9ed0 bfd0 b5d1 80d0  "...............
+00000640: b0d1 86d0 b8d0 b8d0 a0d0 b0d1 81d1 88d0  ................
+00000650: b8d1 80d0 b5d0 bdd0 bdd0 b0d1 8fd0 9fd0  ................
+00000660: bed0 b4d1 81d0 bad0 b0d0 b7d0 bad0 b022  ..............."
+00000670: 2069 643d 2232 3722 2f3e 0a09 0909 3c45   id="27"/>....<E
+00000680: 7665 6e74 733e 0a09 0909 093c 4576 656e  vents>.....<Even
+00000690: 7420 6e61 6d65 3d22 4f6e 4368 616e 6765  t name="OnChange
+000006a0: 223e d0a2 d0b8 d0bf d09e d0bf d0b5 d180  ">..............
+000006b0: d0b0 d186 d0b8 d0b8 d09f d180 d0b8 d098  ................
+000006c0: d0b7 d0bc d0b5 d0bd d0b5 d0bd d0b8 d0b8  ................
+000006d0: 3c2f 4576 656e 743e 0a09 0909 3c2f 4576  </Event>....</Ev
+000006e0: 656e 7473 3e0a 0909 3c2f 496e 7075 7446  ents>...</InputF
+000006f0: 6965 6c64 3e0a 0909 3c43 6865 636b 426f  ield>...<CheckBo
+00000700: 7846 6965 6c64 206e 616d 653d 22d0 92d1  xField name="...
+00000710: 8bd0 b3d1 80d1 83d0 b6d0 b0d1 82d1 8cd0  ................
+00000720: a0d0 b0d1 81d1 88d0 b8d1 80d0 b5d0 bdd0  ................
+00000730: b8d1 8fd0 9253 7065 6322 2069 643d 2233  .....Spec" id="3
+00000740: 3822 3e0a 0909 093c 4461 7461 5061 7468  8">....<DataPath
+00000750: 3ed0 92d1 8bd0 b3d1 80d1 83d0 b6d0 b0d1  >...............
+00000760: 82d1 8cd0 a0d0 b0d1 81d1 88d0 b8d1 80d0  ................
+00000770: b5d0 bdd0 b8d1 8fd0 9253 7065 633c 2f44  .........Spec</D
+00000780: 6174 6150 6174 683e 0a09 0909 3c54 6974  ataPath>....<Tit
+00000790: 6c65 3e0a 0909 0909 3c76 383a 6974 656d  le>.....<v8:item
+000007a0: 3e0a 0909 0909 093c 7638 3a6c 616e 673e  >......<v8:lang>
+000007b0: 7275 3c2f 7638 3a6c 616e 673e 0a09 0909  ru</v8:lang>....
+000007c0: 0909 3c76 383a 636f 6e74 656e 743e d092  ..<v8:content>..
+000007d0: d18b d0b3 d180 d183 d0b6 d0b0 d182 d18c  ................
+000007e0: 20d0 b220 7370 6563 3c2f 7638 3a63 6f6e   .. spec</v8:con
+000007f0: 7465 6e74 3e0a 0909 0909 3c2f 7638 3a69  tent>.....</v8:i
+00000800: 7465 6d3e 0a09 0909 3c2f 5469 746c 653e  tem>....</Title>
+00000810: 0a09 0909 3c43 6865 636b 426f 7854 7970  ....<CheckBoxTyp
+00000820: 653e 4175 746f 3c2f 4368 6563 6b42 6f78  e>Auto</CheckBox
+00000830: 5479 7065 3e0a 0909 093c 436f 6e74 6578  Type>....<Contex
+00000840: 744d 656e 7520 6e61 6d65 3d22 d092 d18b  tMenu name="....
+00000850: d0b3 d180 d183 d0b6 d0b0 d182 d18c d0a0  ................
+00000860: d0b0 d181 d188 d0b8 d180 d0b5 d0bd d0b8  ................
+00000870: d18f d092 5370 6563 d09a d0be d0bd d182  ....Spec........
+00000880: d0b5 d0ba d181 d182 d0bd d0be d0b5 d09c  ................
+00000890: d0b5 d0bd d18e 2220 6964 3d22 3339 222f  ......" id="39"/
+000008a0: 3e0a 0909 093c 4578 7465 6e64 6564 546f  >....<ExtendedTo
+000008b0: 6f6c 7469 7020 6e61 6d65 3d22 d092 d18b  oltip name="....
+000008c0: d0b3 d180 d183 d0b6 d0b0 d182 d18c d0a0  ................
+000008d0: d0b0 d181 d188 d0b8 d180 d0b5 d0bd d0b8  ................
+000008e0: d18f d092 5370 6563 d0a0 d0b0 d181 d188  ....Spec........
+000008f0: d0b8 d180 d0b5 d0bd d0bd d0b0 d18f d09f  ................
+00000900: d0be d0b4 d181 d0ba d0b0 d0b7 d0ba d0b0  ................
+00000910: 2220 6964 3d22 3430 222f 3e0a 0909 3c2f  " id="40"/>...</
+00000920: 4368 6563 6b42 6f78 4669 656c 643e 0a09  CheckBoxField>..
+00000930: 093c 496e 7075 7446 6965 6c64 206e 616d  .<InputField nam
+00000940: 653d 22d0 9fd0 b0d0 bfd0 bad0 b0d0 92d1  e=".............
+00000950: 8bd0 b3d1 80d1 83d0 b7d0 bad0 b822 2069  ............." i
+00000960: 643d 2237 223e 0a09 0909 3c44 6174 6150  d="7">....<DataP
+00000970: 6174 683e d09f d0b0 d0bf d0ba d0b0 d092  ath>............
+00000980: d18b d0b3 d180 d183 d0b7 d0ba d0b8 3c2f  ..............</
+00000990: 4461 7461 5061 7468 3e0a 0909 093c 5469  DataPath>....<Ti
+000009a0: 746c 653e 0a09 0909 093c 7638 3a69 7465  tle>.....<v8:ite
+000009b0: 6d3e 0a09 0909 0909 3c76 383a 6c61 6e67  m>......<v8:lang
+000009c0: 3e72 753c 2f76 383a 6c61 6e67 3e0a 0909  >ru</v8:lang>...
+000009d0: 0909 093c 7638 3a63 6f6e 7465 6e74 3ed0  ...<v8:content>.
+000009e0: 9ad0 bed1 80d0 b5d0 bdd1 8c20 d180 d0b5  ........... ....
+000009f0: d0bf d0be d0b7 d0b8 d182 d0be d180 d0b8  ................
+00000a00: d18f 3c2f 7638 3a63 6f6e 7465 6e74 3e0a  ..</v8:content>.
+00000a10: 0909 0909 3c2f 7638 3a69 7465 6d3e 0a09  ....</v8:item>..
+00000a20: 0909 3c2f 5469 746c 653e 0a09 0909 3c43  ..</Title>....<C
+00000a30: 686f 6963 6542 7574 746f 6e3e 7472 7565  hoiceButton>true
+00000a40: 3c2f 4368 6f69 6365 4275 7474 6f6e 3e0a  </ChoiceButton>.
+00000a50: 0909 093c 436f 6e74 6578 744d 656e 7520  ...<ContextMenu 
+00000a60: 6e61 6d65 3d22 d09f d0b0 d0bf d0ba d0b0  name="..........
+00000a70: d092 d18b d0b3 d180 d183 d0b7 d0ba d0b8  ................
+00000a80: d09a d0be d0bd d182 d0b5 d0ba d181 d182  ................
+00000a90: d0bd d0be d0b5 d09c d0b5 d0bd d18e 2220  .............." 
+00000aa0: 6964 3d22 3822 2f3e 0a09 0909 3c45 7874  id="8"/>....<Ext
+00000ab0: 656e 6465 6454 6f6f 6c74 6970 206e 616d  endedTooltip nam
+00000ac0: 653d 22d0 9fd0 b0d0 bfd0 bad0 b0d0 92d1  e=".............
+00000ad0: 8bd0 b3d1 80d1 83d0 b7d0 bad0 b8d0 a0d0  ................
+00000ae0: b0d1 81d1 88d0 b8d1 80d0 b5d0 bdd0 bdd0  ................
+00000af0: b0d1 8fd0 9fd0 bed0 b4d1 81d0 bad0 b0d0  ................
+00000b00: b7d0 bad0 b022 2069 643d 2233 3122 2f3e  ....." id="31"/>
+00000b10: 0a09 0909 3c45 7665 6e74 733e 0a09 0909  ....<Events>....
+00000b20: 093c 4576 656e 7420 6e61 6d65 3d22 5374  .<Event name="St
+00000b30: 6172 7443 686f 6963 6522 3ed0 9fd0 b0d0  artChoice">.....
+00000b40: bfd0 bad0 b0d0 92d1 8bd0 b3d1 80d1 83d0  ................
+00000b50: b7d0 bad0 b8d0 9dd0 b0d1 87d0 b0d0 bbd0  ................
+00000b60: bed0 92d1 8bd0 b1d0 bed1 80d0 b03c 2f45  .............</E
+00000b70: 7665 6e74 3e0a 0909 093c 2f45 7665 6e74  vent>....</Event
+00000b80: 733e 0a09 093c 2f49 6e70 7574 4669 656c  s>...</InputFiel
+00000b90: 643e 0a09 093c 496e 7075 7446 6965 6c64  d>...<InputField
+00000ba0: 206e 616d 653d 22d0 9fd1 83d1 82d1 8cd0   name=".........
+00000bb0: 9ad0 9fd0 bbd0 b0d1 82d1 84d0 bed1 80d0  ................
+00000bc0: bcd0 b522 2069 643d 2231 223e 0a09 0909  ..." id="1">....
+00000bd0: 3c44 6174 6150 6174 683e d09f d183 d182  <DataPath>......
+00000be0: d18c d09a d09f d0bb d0b0 d182 d184 d0be  ................
+00000bf0: d180 d0bc d0b5 3c2f 4461 7461 5061 7468  ......</DataPath
+00000c00: 3e0a 0909 093c 4368 6f69 6365 4275 7474  >....<ChoiceButt
+00000c10: 6f6e 3e74 7275 653c 2f43 686f 6963 6542  on>true</ChoiceB
+00000c20: 7574 746f 6e3e 0a09 0909 3c43 6f6e 7465  utton>....<Conte
+00000c30: 7874 4d65 6e75 206e 616d 653d 22d0 9fd1  xtMenu name="...
+00000c40: 83d1 82d1 8cd0 9ad0 9fd0 bbd0 b0d1 82d1  ................
+00000c50: 84d0 bed1 80d0 bcd0 b5d0 9ad0 bed0 bdd1  ................
+00000c60: 82d0 b5d0 bad1 81d1 82d0 bdd0 bed0 b5d0  ................
+00000c70: 9cd0 b5d0 bdd1 8e22 2069 643d 2232 222f  ......." id="2"/
+00000c80: 3e0a 0909 093c 4578 7465 6e64 6564 546f  >....<ExtendedTo
+00000c90: 6f6c 7469 7020 6e61 6d65 3d22 d09f d183  oltip name="....
+00000ca0: d182 d18c d09a d09f d0bb d0b0 d182 d184  ................
+00000cb0: d0be d180 d0bc d0b5 d0a0 d0b0 d181 d188  ................
+00000cc0: d0b8 d180 d0b5 d0bd d0bd d0b0 d18f d09f  ................
+00000cd0: d0be d0b4 d181 d0ba d0b0 d0b7 d0ba d0b0  ................
+00000ce0: 2220 6964 3d22 3236 222f 3e0a 0909 093c  " id="26"/>....<
+00000cf0: 4576 656e 7473 3e0a 0909 0909 3c45 7665  Events>.....<Eve
+00000d00: 6e74 206e 616d 653d 2253 7461 7274 4368  nt name="StartCh
+00000d10: 6f69 6365 223e d09f d183 d182 d18c d09a  oice">..........
+00000d20: d09f d0bb d0b0 d182 d184 d0be d180 d0bc  ................
+00000d30: d0b5 d09d d0b0 d187 d0b0 d0bb d0be d092  ................
+00000d40: d18b d0b1 d0be d180 d0b0 3c2f 4576 656e  ..........</Even
+00000d50: 743e 0a09 0909 3c2f 4576 656e 7473 3e0a  t>....</Events>.
+00000d60: 0909 3c2f 496e 7075 7446 6965 6c64 3e0a  ..</InputField>.
+00000d70: 0909 3c49 6e70 7574 4669 656c 6420 6e61  ..<InputField na
+00000d80: 6d65 3d22 d0a1 d182 d180 d0be d0ba d0b0  me="............
+00000d90: d09f d0be d0b4 d0ba d0bb d18e d187 d0b5  ................
+00000da0: d0bd d0b8 d18f d09a d091 d0b0 d0b7 d0b5  ................
+00000db0: 2220 6964 3d22 3422 3e0a 0909 093c 4461  " id="4">....<Da
+00000dc0: 7461 5061 7468 3ed0 a1d1 82d1 80d0 bed0  taPath>.........
+00000dd0: bad0 b0d0 9fd0 bed0 b4d0 bad0 bbd1 8ed1  ................
+00000de0: 87d0 b5d0 bdd0 b8d1 8fd0 9ad0 91d0 b0d0  ................
+00000df0: b7d0 b53c 2f44 6174 6150 6174 683e 0a09  ...</DataPath>..
+00000e00: 0909 3c43 6f6e 7465 7874 4d65 6e75 206e  ..<ContextMenu n
+00000e10: 616d 653d 22d0 a1d1 82d1 80d0 bed0 bad0  ame="...........
+00000e20: b0d0 9fd0 bed0 b4d0 bad0 bbd1 8ed1 87d0  ................
+00000e30: b5d0 bdd0 b8d1 8fd0 9ad0 91d0 b0d0 b7d0  ................
+00000e40: b5d0 9ad0 bed0 bdd1 82d0 b5d0 bad1 81d1  ................
+00000e50: 82d0 bdd0 bed0 b5d0 9cd0 b5d0 bdd1 8e22  ..............."
+00000e60: 2069 643d 2235 222f 3e0a 0909 093c 4578   id="5"/>....<Ex
+00000e70: 7465 6e64 6564 546f 6f6c 7469 7020 6e61  tendedTooltip na
+00000e80: 6d65 3d22 d0a1 d182 d180 d0be d0ba d0b0  me="............
+00000e90: d09f d0be d0b4 d0ba d0bb d18e d187 d0b5  ................
+00000ea0: d0bd d0b8 d18f d09a d091 d0b0 d0b7 d0b5  ................
+00000eb0: d0a0 d0b0 d181 d188 d0b8 d180 d0b5 d0bd  ................
+00000ec0: d0bd d0b0 d18f d09f d0be d0b4 d181 d0ba  ................
+00000ed0: d0b0 d0b7 d0ba d0b0 2220 6964 3d22 3238  ........" id="28
+00000ee0: 222f 3e0a 0909 093c 4576 656e 7473 3e0a  "/>....<Events>.
+00000ef0: 0909 0909 3c45 7665 6e74 206e 616d 653d  ....<Event name=
+00000f00: 2253 7461 7274 4368 6f69 6365 223e d0a1  "StartChoice">..
+00000f10: d182 d180 d0be d0ba d0b0 d09f d0be d0b4  ................
+00000f20: d0ba d0bb d18e d187 d0b5 d0bd d0b8 d18f  ................
+00000f30: d09a d091 d0b0 d0b7 d0b5 d09d d0b0 d187  ................
+00000f40: d0b0 d0bb d0be d092 d18b d0b1 d0be d180  ................
+00000f50: d0b0 3c2f 4576 656e 743e 0a09 0909 3c2f  ..</Event>....</
+00000f60: 4576 656e 7473 3e0a 0909 3c2f 496e 7075  Events>...</Inpu
+00000f70: 7446 6965 6c64 3e0a 0909 3c49 6e70 7574  tField>...<Input
+00000f80: 4669 656c 6420 6e61 6d65 3d22 d09b d0be  Field name="....
+00000f90: d0b3 d0b8 d0bd 2220 6964 3d22 3138 223e  ......" id="18">
+00000fa0: 0a09 0909 3c44 6174 6150 6174 683e d09b  ....<DataPath>..
+00000fb0: d0be d0b3 d0b8 d0bd 3c2f 4461 7461 5061  ........</DataPa
+00000fc0: 7468 3e0a 0909 093c 436f 6e74 6578 744d  th>....<ContextM
+00000fd0: 656e 7520 6e61 6d65 3d22 d09b d0be d0b3  enu name="......
+00000fe0: d0b8 d0bd d09a d0be d0bd d182 d0b5 d0ba  ................
+00000ff0: d181 d182 d0bd d0be d0b5 d09c d0b5 d0bd  ................
+00001000: d18e 2220 6964 3d22 3139 222f 3e0a 0909  .." id="19"/>...
+00001010: 093c 4578 7465 6e64 6564 546f 6f6c 7469  .<ExtendedToolti
+00001020: 7020 6e61 6d65 3d22 d09b d0be d0b3 d0b8  p name="........
+00001030: d0bd d0a0 d0b0 d181 d188 d0b8 d180 d0b5  ................
+00001040: d0bd d0bd d0b0 d18f d09f d0be d0b4 d181  ................
+00001050: d0ba d0b0 d0b7 d0ba d0b0 2220 6964 3d22  .........." id="
+00001060: 3239 222f 3e0a 0909 3c2f 496e 7075 7446  29"/>...</InputF
+00001070: 6965 6c64 3e0a 0909 3c49 6e70 7574 4669  ield>...<InputFi
+00001080: 656c 6420 6e61 6d65 3d22 d09f d0b0 d180  eld name="......
+00001090: d0be d0bb d18c 2220 6964 3d22 3231 223e  ......" id="21">
+000010a0: 0a09 0909 3c44 6174 6150 6174 683e d09f  ....<DataPath>..
+000010b0: d0b0 d180 d0be d0bb d18c 3c2f 4461 7461  ..........</Data
+000010c0: 5061 7468 3e0a 0909 093c 5061 7373 776f  Path>....<Passwo
+000010d0: 7264 4d6f 6465 3e74 7275 653c 2f50 6173  rdMode>true</Pas
+000010e0: 7377 6f72 644d 6f64 653e 0a09 0909 3c43  swordMode>....<C
+000010f0: 6f6e 7465 7874 4d65 6e75 206e 616d 653d  ontextMenu name=
+00001100: 22d0 9fd0 b0d1 80d0 bed0 bbd1 8cd0 9ad0  "...............
+00001110: bed0 bdd1 82d0 b5d0 bad1 81d1 82d0 bdd0  ................
+00001120: bed0 b5d0 9cd0 b5d0 bdd1 8e22 2069 643d  ..........." id=
+00001130: 2232 3222 2f3e 0a09 0909 3c45 7874 656e  "22"/>....<Exten
+00001140: 6465 6454 6f6f 6c74 6970 206e 616d 653d  dedTooltip name=
+00001150: 22d0 9fd0 b0d1 80d0 bed0 bbd1 8cd0 a0d0  "...............
+00001160: b0d1 81d1 88d0 b8d1 80d0 b5d0 bdd0 bdd0  ................
+00001170: b0d1 8fd0 9fd0 bed0 b4d1 81d0 bad0 b0d0  ................
+00001180: b7d0 bad0 b022 2069 643d 2233 3022 2f3e  ....." id="30"/>
+00001190: 0a09 093c 2f49 6e70 7574 4669 656c 643e  ...</InputField>
+000011a0: 0a09 093c 496e 7075 7446 6965 6c64 206e  ...<InputField n
+000011b0: 616d 653d 22d0 9ad0 bed0 b4d0 a0d0 b0d0  ame="...........
+000011c0: b7d0 b1d0 bbd0 bed0 bad0 b8d1 80d0 bed0  ................
+000011d0: b2d0 bad0 b822 2069 643d 2233 3522 3e0a  ....." id="35">.
+000011e0: 0909 093c 4461 7461 5061 7468 3ed0 9ad0  ...<DataPath>...
+000011f0: bed0 b4d0 a0d0 b0d0 b7d0 b1d0 bbd0 bed0  ................
+00001200: bad0 b8d1 80d0 bed0 b2d0 bad0 b83c 2f44  .............</D
+00001210: 6174 6150 6174 683e 0a09 0909 3c43 6f6e  ataPath>....<Con
+00001220: 7465 7874 4d65 6e75 206e 616d 653d 22d0  textMenu name=".
+00001230: 9ad0 bed0 b4d0 a0d0 b0d0 b7d0 b1d0 bbd0  ................
+00001240: bed0 bad0 b8d1 80d0 bed0 b2d0 bad0 b8d0  ................
+00001250: 9ad0 bed0 bdd1 82d0 b5d0 bad1 81d1 82d0  ................
+00001260: bdd0 bed0 b5d0 9cd0 b5d0 bdd1 8e22 2069  ............." i
+00001270: 643d 2233 3622 2f3e 0a09 0909 3c45 7874  d="36"/>....<Ext
+00001280: 656e 6465 6454 6f6f 6c74 6970 206e 616d  endedTooltip nam
+00001290: 653d 22d0 9ad0 bed0 b4d0 a0d0 b0d0 b7d0  e=".............
+000012a0: b1d0 bbd0 bed0 bad0 b8d1 80d0 bed0 b2d0  ................
+000012b0: bad0 b8d0 a0d0 b0d1 81d1 88d0 b8d1 80d0  ................
+000012c0: b5d0 bdd0 bdd0 b0d1 8fd0 9fd0 bed0 b4d1  ................
+000012d0: 81d0 bad0 b0d0 b7d0 bad0 b022 2069 643d  ..........." id=
+000012e0: 2233 3722 2f3e 0a09 093c 2f49 6e70 7574  "37"/>...</Input
+000012f0: 4669 656c 643e 0a09 093c 5573 7561 6c47  Field>...<UsualG
+00001300: 726f 7570 206e 616d 653d 22d0 93d1 80d1  roup name=".....
+00001310: 83d0 bfd0 bfd0 b022 2069 643d 2234 3422  ......." id="44"
+00001320: 3e0a 0909 093c 5265 7072 6573 656e 7461  >....<Representa
+00001330: 7469 6f6e 3e4e 6f6e 653c 2f52 6570 7265  tion>None</Repre
+00001340: 7365 6e74 6174 696f 6e3e 0a09 0909 3c53  sentation>....<S
+00001350: 686f 7754 6974 6c65 3e66 616c 7365 3c2f  howTitle>false</
+00001360: 5368 6f77 5469 746c 653e 0a09 0909 3c45  ShowTitle>....<E
+00001370: 7874 656e 6465 6454 6f6f 6c74 6970 206e  xtendedTooltip n
+00001380: 616d 653d 22d0 93d1 80d1 83d0 bfd0 bfd0  ame="...........
+00001390: b0d0 a0d0 b0d1 81d1 88d0 b8d1 80d0 b5d0  ................
+000013a0: bdd0 bdd0 b0d1 8fd0 9fd0 bed0 b4d1 81d0  ................
+000013b0: bad0 b0d0 b7d0 bad0 b022 2069 643d 2234  ........." id="4
+000013c0: 3522 2f3e 0a09 0909 3c43 6869 6c64 4974  5"/>....<ChildIt
+000013d0: 656d 733e 0a09 0909 093c 4368 6563 6b42  ems>.....<CheckB
+000013e0: 6f78 4669 656c 6420 6e61 6d65 3d22 d09f  oxField name="..
+000013f0: d0be d0b4 d0bc d0b5 d0bd d0b8 d182 d18c  ................
+00001400: d09f d183 d182 d18c 5275 6e6e 6572 2220  ........Runner" 
+00001410: 6964 3d22 3431 223e 0a09 0909 0909 3c44  id="41">......<D
+00001420: 6174 6150 6174 683e d09f d0be d0b4 d0bc  ataPath>........
+00001430: d0b5 d0bd d0b8 d182 d18c d09f d183 d182  ................
+00001440: d18c 5275 6e6e 6572 3c2f 4461 7461 5061  ..Runner</DataPa
+00001450: 7468 3e0a 0909 0909 093c 456e 6162 6c65  th>......<Enable
+00001460: 643e 6661 6c73 653c 2f45 6e61 626c 6564  d>false</Enabled
+00001470: 3e0a 0909 0909 093c 4368 6563 6b42 6f78  >......<CheckBox
+00001480: 5479 7065 3e41 7574 6f3c 2f43 6865 636b  Type>Auto</Check
+00001490: 426f 7854 7970 653e 0a09 0909 0909 3c43  BoxType>......<C
+000014a0: 6f6e 7465 7874 4d65 6e75 206e 616d 653d  ontextMenu name=
+000014b0: 22d0 9fd0 bed0 b4d0 bcd0 b5d0 bdd0 b8d1  "...............
+000014c0: 82d1 8cd0 9fd1 83d1 82d1 8c52 756e 6e65  ...........Runne
+000014d0: 72d0 9ad0 bed0 bdd1 82d0 b5d0 bad1 81d1  r...............
+000014e0: 82d0 bdd0 bed0 b5d0 9cd0 b5d0 bdd1 8e22  ..............."
+000014f0: 2069 643d 2234 3222 2f3e 0a09 0909 0909   id="42"/>......
+00001500: 3c45 7874 656e 6465 6454 6f6f 6c74 6970  <ExtendedTooltip
+00001510: 206e 616d 653d 22d0 9fd0 bed0 b4d0 bcd0   name=".........
+00001520: b5d0 bdd0 b8d1 82d1 8cd0 9fd1 83d1 82d1  ................
+00001530: 8c52 756e 6e65 72d0 a0d0 b0d1 81d1 88d0  .Runner.........
+00001540: b8d1 80d0 b5d0 bdd0 bdd0 b0d1 8fd0 9fd0  ................
+00001550: bed0 b4d1 81d0 bad0 b0d0 b7d0 bad0 b022  ..............."
+00001560: 2069 643d 2234 3322 2f3e 0a09 0909 093c   id="43"/>.....<
+00001570: 2f43 6865 636b 426f 7846 6965 6c64 3e0a  /CheckBoxField>.
+00001580: 0909 0909 3c43 6865 636b 426f 7846 6965  ....<CheckBoxFie
+00001590: 6c64 206e 616d 653d 22d0 9ed1 82d0 bbd0  ld name=".......
+000015a0: b0d0 b4d0 bad0 b022 2069 643d 2231 3522  ......." id="15"
+000015b0: 3e0a 0909 0909 093c 4461 7461 5061 7468  >......<DataPath
+000015c0: 3ed0 9ed1 82d0 bbd0 b0d0 b4d0 bad0 b03c  >..............<
+000015d0: 2f44 6174 6150 6174 683e 0a09 0909 0909  /DataPath>......
+000015e0: 3c43 6865 636b 426f 7854 7970 653e 4175  <CheckBoxType>Au
+000015f0: 746f 3c2f 4368 6563 6b42 6f78 5479 7065  to</CheckBoxType
+00001600: 3e0a 0909 0909 093c 436f 6e74 6578 744d  >......<ContextM
+00001610: 656e 7520 6e61 6d65 3d22 d09e d182 d0bb  enu name="......
+00001620: d0b0 d0b4 d0ba d0b0 d09a d0be d0bd d182  ................
+00001630: d0b5 d0ba d181 d182 d0bd d0be d0b5 d09c  ................
+00001640: d0b5 d0bd d18e 2220 6964 3d22 3136 222f  ......" id="16"/
+00001650: 3e0a 0909 0909 093c 4578 7465 6e64 6564  >......<Extended
+00001660: 546f 6f6c 7469 7020 6e61 6d65 3d22 d09e  Tooltip name="..
+00001670: d182 d0bb d0b0 d0b4 d0ba d0b0 d0a0 d0b0  ................
+00001680: d181 d188 d0b8 d180 d0b5 d0bd d0bd d0b0  ................
+00001690: d18f d09f d0be d0b4 d181 d0ba d0b0 d0b7  ................
+000016a0: d0ba d0b0 2220 6964 3d22 3333 222f 3e0a  ...." id="33"/>.
+000016b0: 0909 0909 3c2f 4368 6563 6b42 6f78 4669  ....</CheckBoxFi
+000016c0: 656c 643e 0a09 0909 3c2f 4368 696c 6449  eld>....</ChildI
+000016d0: 7465 6d73 3e0a 0909 3c2f 5573 7561 6c47  tems>...</UsualG
+000016e0: 726f 7570 3e0a 0909 3c42 7574 746f 6e20  roup>...<Button 
+000016f0: 6e61 6d65 3d22 d0a1 d0b4 d0b5 d0bb d0b0  name="..........
+00001700: d182 d18c 2220 6964 3d22 3130 223e 0a09  ...." id="10">..
+00001710: 0909 3c54 7970 653e 5573 7561 6c42 7574  ..<Type>UsualBut
+00001720: 746f 6e3c 2f54 7970 653e 0a09 0909 3c43  ton</Type>....<C
+00001730: 6f6d 6d61 6e64 4e61 6d65 3e46 6f72 6d2e  ommandName>Form.
+00001740: 436f 6d6d 616e 642e d0a1 d0b4 d0b5 d0bb  Command.........
+00001750: d0b0 d182 d18c 3c2f 436f 6d6d 616e 644e  ......</CommandN
+00001760: 616d 653e 0a09 0909 3c45 7874 656e 6465  ame>....<Extende
+00001770: 6454 6f6f 6c74 6970 206e 616d 653d 22d0  dTooltip name=".
+00001780: a1d0 b4d0 b5d0 bbd0 b0d1 82d1 8cd0 a0d0  ................
+00001790: b0d1 81d1 88d0 b8d1 80d0 b5d0 bdd0 bdd0  ................
+000017a0: b0d1 8fd0 9fd0 bed0 b4d1 81d0 bad0 b0d0  ................
+000017b0: b7d0 bad0 b022 2069 643d 2233 3422 2f3e  ....." id="34"/>
+000017c0: 0a09 093c 2f42 7574 746f 6e3e 0a09 3c2f  ...</Button>..</
+000017d0: 4368 696c 6449 7465 6d73 3e0a 093c 4174  ChildItems>..<At
+000017e0: 7472 6962 7574 6573 3e0a 0909 3c41 7474  tributes>...<Att
+000017f0: 7269 6275 7465 206e 616d 653d 22d0 9ed0  ribute name="...
+00001800: b1d1 8ad0 b5d0 bad1 8222 2069 643d 2231  ........." id="1
+00001810: 223e 0a09 0909 3c54 7970 653e 0a09 0909  ">....<Type>....
+00001820: 093c 7638 3a54 7970 653e 6366 673a 4578  .<v8:Type>cfg:Ex
+00001830: 7465 726e 616c 4461 7461 5072 6f63 6573  ternalDataProces
+00001840: 736f 724f 626a 6563 742e 5275 6e6e 6572  sorObject.Runner
+00001850: 3143 3c2f 7638 3a54 7970 653e 0a09 0909  1C</v8:Type>....
+00001860: 3c2f 5479 7065 3e0a 0909 093c 4d61 696e  </Type>....<Main
+00001870: 4174 7472 6962 7574 653e 7472 7565 3c2f  Attribute>true</
+00001880: 4d61 696e 4174 7472 6962 7574 653e 0a09  MainAttribute>..
+00001890: 093c 2f41 7474 7269 6275 7465 3e0a 0909  .</Attribute>...
+000018a0: 3c41 7474 7269 6275 7465 206e 616d 653d  <Attribute name=
+000018b0: 22d0 9fd1 83d1 82d1 8cd0 9ad0 9fd0 bbd0  "...............
+000018c0: b0d1 82d1 84d0 bed1 80d0 bcd0 b522 2069  ............." i
+000018d0: 643d 2232 223e 0a09 0909 3c54 6974 6c65  d="2">....<Title
+000018e0: 3e0a 0909 0909 3c76 383a 6974 656d 3e0a  >.....<v8:item>.
+000018f0: 0909 0909 093c 7638 3a6c 616e 673e 7275  .....<v8:lang>ru
+00001900: 3c2f 7638 3a6c 616e 673e 0a09 0909 0909  </v8:lang>......
+00001910: 3c76 383a 636f 6e74 656e 743e d09f d183  <v8:content>....
+00001920: d182 d18c 20d0 ba20 d0bf d0bb d0b0 d182  .... .. ........
+00001930: d184 d0be d180 d0bc d0b5 3c2f 7638 3a63  ..........</v8:c
+00001940: 6f6e 7465 6e74 3e0a 0909 0909 3c2f 7638  ontent>.....</v8
+00001950: 3a69 7465 6d3e 0a09 0909 3c2f 5469 746c  :item>....</Titl
+00001960: 653e 0a09 0909 3c54 7970 653e 0a09 0909  e>....<Type>....
+00001970: 093c 7638 3a54 7970 653e 7873 3a73 7472  .<v8:Type>xs:str
+00001980: 696e 673c 2f76 383a 5479 7065 3e0a 0909  ing</v8:Type>...
+00001990: 0909 3c76 383a 5374 7269 6e67 5175 616c  ..<v8:StringQual
+000019a0: 6966 6965 7273 3e0a 0909 0909 093c 7638  ifiers>......<v8
+000019b0: 3a4c 656e 6774 683e 303c 2f76 383a 4c65  :Length>0</v8:Le
+000019c0: 6e67 7468 3e0a 0909 0909 093c 7638 3a41  ngth>......<v8:A
+000019d0: 6c6c 6f77 6564 4c65 6e67 7468 3e56 6172  llowedLength>Var
+000019e0: 6961 626c 653c 2f76 383a 416c 6c6f 7765  iable</v8:Allowe
+000019f0: 644c 656e 6774 683e 0a09 0909 093c 2f76  dLength>.....</v
+00001a00: 383a 5374 7269 6e67 5175 616c 6966 6965  8:StringQualifie
+00001a10: 7273 3e0a 0909 093c 2f54 7970 653e 0a09  rs>....</Type>..
+00001a20: 0909 3c46 696c 6c43 6865 636b 3e53 686f  ..<FillCheck>Sho
+00001a30: 7745 7272 6f72 3c2f 4669 6c6c 4368 6563  wError</FillChec
+00001a40: 6b3e 0a09 093c 2f41 7474 7269 6275 7465  k>...</Attribute
+00001a50: 3e0a 0909 3c41 7474 7269 6275 7465 206e  >...<Attribute n
+00001a60: 616d 653d 22d0 a1d1 82d1 80d0 bed0 bad0  ame="...........
+00001a70: b0d0 9fd0 bed0 b4d0 bad0 bbd1 8ed1 87d0  ................
+00001a80: b5d0 bdd0 b8d1 8fd0 9ad0 91d0 b0d0 b7d0  ................
+00001a90: b522 2069 643d 2233 223e 0a09 0909 3c54  ." id="3">....<T
+00001aa0: 6974 6c65 3e0a 0909 0909 3c76 383a 6974  itle>.....<v8:it
+00001ab0: 656d 3e0a 0909 0909 093c 7638 3a6c 616e  em>......<v8:lan
+00001ac0: 673e 7275 3c2f 7638 3a6c 616e 673e 0a09  g>ru</v8:lang>..
+00001ad0: 0909 0909 3c76 383a 636f 6e74 656e 743e  ....<v8:content>
+00001ae0: d0a1 d182 d180 d0be d0ba d0b0 20d0 bfd0  ............ ...
+00001af0: bed0 b4d0 bad0 bbd1 8ed1 87d0 b5d0 bdd0  ................
+00001b00: b8d1 8f3c 2f76 383a 636f 6e74 656e 743e  ...</v8:content>
+00001b10: 0a09 0909 093c 2f76 383a 6974 656d 3e0a  .....</v8:item>.
+00001b20: 0909 093c 2f54 6974 6c65 3e0a 0909 093c  ...</Title>....<
+00001b30: 5479 7065 3e0a 0909 0909 3c76 383a 5479  Type>.....<v8:Ty
+00001b40: 7065 3e78 733a 7374 7269 6e67 3c2f 7638  pe>xs:string</v8
+00001b50: 3a54 7970 653e 0a09 0909 093c 7638 3a53  :Type>.....<v8:S
+00001b60: 7472 696e 6751 7561 6c69 6669 6572 733e  tringQualifiers>
+00001b70: 0a09 0909 0909 3c76 383a 4c65 6e67 7468  ......<v8:Length
+00001b80: 3e30 3c2f 7638 3a4c 656e 6774 683e 0a09  >0</v8:Length>..
+00001b90: 0909 0909 3c76 383a 416c 6c6f 7765 644c  ....<v8:AllowedL
+00001ba0: 656e 6774 683e 5661 7269 6162 6c65 3c2f  ength>Variable</
+00001bb0: 7638 3a41 6c6c 6f77 6564 4c65 6e67 7468  v8:AllowedLength
+00001bc0: 3e0a 0909 0909 3c2f 7638 3a53 7472 696e  >.....</v8:Strin
+00001bd0: 6751 7561 6c69 6669 6572 733e 0a09 0909  gQualifiers>....
+00001be0: 3c2f 5479 7065 3e0a 0909 093c 4669 6c6c  </Type>....<Fill
+00001bf0: 4368 6563 6b3e 5368 6f77 4572 726f 723c  Check>ShowError<
+00001c00: 2f46 696c 6c43 6865 636b 3e0a 0909 3c2f  /FillCheck>...</
+00001c10: 4174 7472 6962 7574 653e 0a09 093c 4174  Attribute>...<At
+00001c20: 7472 6962 7574 6520 6e61 6d65 3d22 d09f  tribute name="..
+00001c30: d0b0 d0bf d0ba d0b0 d092 d18b d0b3 d180  ................
+00001c40: d183 d0b7 d0ba d0b8 2220 6964 3d22 3422  ........" id="4"
+00001c50: 3e0a 0909 093c 5469 746c 653e 0a09 0909  >....<Title>....
+00001c60: 093c 7638 3a69 7465 6d3e 0a09 0909 0909  .<v8:item>......
+00001c70: 3c76 383a 6c61 6e67 3e72 753c 2f76 383a  <v8:lang>ru</v8:
+00001c80: 6c61 6e67 3e0a 0909 0909 093c 7638 3a63  lang>......<v8:c
+00001c90: 6f6e 7465 6e74 3ed0 9fd0 b0d0 bfd0 bad0  ontent>.........
+00001ca0: b020 d0b2 d18b d0b3 d180 d183 d0b7 d0ba  . ..............
+00001cb0: d0b8 3c2f 7638 3a63 6f6e 7465 6e74 3e0a  ..</v8:content>.
+00001cc0: 0909 0909 3c2f 7638 3a69 7465 6d3e 0a09  ....</v8:item>..
+00001cd0: 0909 3c2f 5469 746c 653e 0a09 0909 3c54  ..</Title>....<T
+00001ce0: 7970 653e 0a09 0909 093c 7638 3a54 7970  ype>.....<v8:Typ
+00001cf0: 653e 7873 3a73 7472 696e 673c 2f76 383a  e>xs:string</v8:
+00001d00: 5479 7065 3e0a 0909 0909 3c76 383a 5374  Type>.....<v8:St
+00001d10: 7269 6e67 5175 616c 6966 6965 7273 3e0a  ringQualifiers>.
+00001d20: 0909 0909 093c 7638 3a4c 656e 6774 683e  .....<v8:Length>
+00001d30: 303c 2f76 383a 4c65 6e67 7468 3e0a 0909  0</v8:Length>...
+00001d40: 0909 093c 7638 3a41 6c6c 6f77 6564 4c65  ...<v8:AllowedLe
+00001d50: 6e67 7468 3e56 6172 6961 626c 653c 2f76  ngth>Variable</v
+00001d60: 383a 416c 6c6f 7765 644c 656e 6774 683e  8:AllowedLength>
+00001d70: 0a09 0909 093c 2f76 383a 5374 7269 6e67  .....</v8:String
+00001d80: 5175 616c 6966 6965 7273 3e0a 0909 093c  Qualifiers>....<
+00001d90: 2f54 7970 653e 0a09 0909 3c46 696c 6c43  /Type>....<FillC
+00001da0: 6865 636b 3e53 686f 7745 7272 6f72 3c2f  heck>ShowError</
+00001db0: 4669 6c6c 4368 6563 6b3e 0a09 0909 3c53  FillCheck>....<S
+00001dc0: 6176 653e 0a09 0909 093c 4669 656c 643e  ave>.....<Field>
+00001dd0: d09f d0b0 d0bf d0ba d0b0 d092 d18b d0b3  ................
+00001de0: d180 d183 d0b7 d0ba d0b8 3c2f 4669 656c  ..........</Fiel
+00001df0: 643e 0a09 0909 3c2f 5361 7665 3e0a 0909  d>....</Save>...
+00001e00: 3c2f 4174 7472 6962 7574 653e 0a09 093c  </Attribute>...<
+00001e10: 4174 7472 6962 7574 6520 6e61 6d65 3d22  Attribute name="
+00001e20: d0a2 d0b8 d0bf d09e d0bf d0b5 d180 d0b0  ................
+00001e30: d186 d0b8 d0b8 2220 6964 3d22 3522 3e0a  ......" id="5">.
+00001e40: 0909 093c 5469 746c 653e 0a09 0909 093c  ...<Title>.....<
+00001e50: 7638 3a69 7465 6d3e 0a09 0909 0909 3c76  v8:item>......<v
+00001e60: 383a 6c61 6e67 3e72 753c 2f76 383a 6c61  8:lang>ru</v8:la
+00001e70: 6e67 3e0a 0909 0909 093c 7638 3a63 6f6e  ng>......<v8:con
+00001e80: 7465 6e74 3ed0 a2d0 b8d0 bf20 d0be d0bf  tent>...... ....
+00001e90: d0b5 d180 d0b0 d186 d0b8 d0b8 3c2f 7638  ............</v8
+00001ea0: 3a63 6f6e 7465 6e74 3e0a 0909 0909 3c2f  :content>.....</
+00001eb0: 7638 3a69 7465 6d3e 0a09 0909 3c2f 5469  v8:item>....</Ti
+00001ec0: 746c 653e 0a09 0909 3c54 7970 653e 0a09  tle>....<Type>..
+00001ed0: 0909 093c 7638 3a54 7970 653e 7873 3a73  ...<v8:Type>xs:s
+00001ee0: 7472 696e 673c 2f76 383a 5479 7065 3e0a  tring</v8:Type>.
+00001ef0: 0909 0909 3c76 383a 5374 7269 6e67 5175  ....<v8:StringQu
+00001f00: 616c 6966 6965 7273 3e0a 0909 0909 093c  alifiers>......<
+00001f10: 7638 3a4c 656e 6774 683e 303c 2f76 383a  v8:Length>0</v8:
+00001f20: 4c65 6e67 7468 3e0a 0909 0909 093c 7638  Length>......<v8
+00001f30: 3a41 6c6c 6f77 6564 4c65 6e67 7468 3e56  :AllowedLength>V
+00001f40: 6172 6961 626c 653c 2f76 383a 416c 6c6f  ariable</v8:Allo
+00001f50: 7765 644c 656e 6774 683e 0a09 0909 093c  wedLength>.....<
+00001f60: 2f76 383a 5374 7269 6e67 5175 616c 6966  /v8:StringQualif
+00001f70: 6965 7273 3e0a 0909 093c 2f54 7970 653e  iers>....</Type>
+00001f80: 0a09 0909 3c46 696c 6c43 6865 636b 3e53  ....<FillCheck>S
+00001f90: 686f 7745 7272 6f72 3c2f 4669 6c6c 4368  howError</FillCh
+00001fa0: 6563 6b3e 0a09 0909 3c53 6176 653e 0a09  eck>....<Save>..
+00001fb0: 0909 093c 4669 656c 643e d0a2 d0b8 d0bf  ...<Field>......
+00001fc0: d09e d0bf d0b5 d180 d0b0 d186 d0b8 d0b8  ................
+00001fd0: 3c2f 4669 656c 643e 0a09 0909 3c2f 5361  </Field>....</Sa
+00001fe0: 7665 3e0a 0909 3c2f 4174 7472 6962 7574  ve>...</Attribut
+00001ff0: 653e 0a09 093c 4174 7472 6962 7574 6520  e>...<Attribute 
+00002000: 6e61 6d65 3d22 d09e d182 d0bb d0b0 d0b4  name="..........
+00002010: d0ba d0b0 2220 6964 3d22 3722 3e0a 0909  ...." id="7">...
+00002020: 093c 5469 746c 653e 0a09 0909 093c 7638  .<Title>.....<v8
+00002030: 3a69 7465 6d3e 0a09 0909 0909 3c76 383a  :item>......<v8:
+00002040: 6c61 6e67 3e72 753c 2f76 383a 6c61 6e67  lang>ru</v8:lang
+00002050: 3e0a 0909 0909 093c 7638 3a63 6f6e 7465  >......<v8:conte
+00002060: 6e74 3ed0 9ed1 82d0 bbd0 b0d0 b4d0 bad0  nt>.............
+00002070: b03c 2f76 383a 636f 6e74 656e 743e 0a09  .</v8:content>..
+00002080: 0909 093c 2f76 383a 6974 656d 3e0a 0909  ...</v8:item>...
+00002090: 093c 2f54 6974 6c65 3e0a 0909 093c 5479  .</Title>....<Ty
+000020a0: 7065 3e0a 0909 0909 3c76 383a 5479 7065  pe>.....<v8:Type
+000020b0: 3e78 733a 626f 6f6c 6561 6e3c 2f76 383a  >xs:boolean</v8:
+000020c0: 5479 7065 3e0a 0909 093c 2f54 7970 653e  Type>....</Type>
+000020d0: 0a09 093c 2f41 7474 7269 6275 7465 3e0a  ...</Attribute>.
+000020e0: 0909 3c41 7474 7269 6275 7465 206e 616d  ..<Attribute nam
+000020f0: 653d 22d0 9bd0 bed0 b3d0 b8d0 bd22 2069  e=".........." i
+00002100: 643d 2238 223e 0a09 0909 3c54 6974 6c65  d="8">....<Title
+00002110: 3e0a 0909 0909 3c76 383a 6974 656d 3e0a  >.....<v8:item>.
+00002120: 0909 0909 093c 7638 3a6c 616e 673e 7275  .....<v8:lang>ru
+00002130: 3c2f 7638 3a6c 616e 673e 0a09 0909 0909  </v8:lang>......
+00002140: 3c76 383a 636f 6e74 656e 743e d09b d0be  <v8:content>....
+00002150: d0b3 d0b8 d0bd 3c2f 7638 3a63 6f6e 7465  ......</v8:conte
+00002160: 6e74 3e0a 0909 0909 3c2f 7638 3a69 7465  nt>.....</v8:ite
+00002170: 6d3e 0a09 0909 3c2f 5469 746c 653e 0a09  m>....</Title>..
+00002180: 0909 3c54 7970 653e 0a09 0909 093c 7638  ..<Type>.....<v8
+00002190: 3a54 7970 653e 7873 3a73 7472 696e 673c  :Type>xs:string<
+000021a0: 2f76 383a 5479 7065 3e0a 0909 0909 3c76  /v8:Type>.....<v
+000021b0: 383a 5374 7269 6e67 5175 616c 6966 6965  8:StringQualifie
+000021c0: 7273 3e0a 0909 0909 093c 7638 3a4c 656e  rs>......<v8:Len
+000021d0: 6774 683e 303c 2f76 383a 4c65 6e67 7468  gth>0</v8:Length
+000021e0: 3e0a 0909 0909 093c 7638 3a41 6c6c 6f77  >......<v8:Allow
+000021f0: 6564 4c65 6e67 7468 3e56 6172 6961 626c  edLength>Variabl
+00002200: 653c 2f76 383a 416c 6c6f 7765 644c 656e  e</v8:AllowedLen
+00002210: 6774 683e 0a09 0909 093c 2f76 383a 5374  gth>.....</v8:St
+00002220: 7269 6e67 5175 616c 6966 6965 7273 3e0a  ringQualifiers>.
+00002230: 0909 093c 2f54 7970 653e 0a09 093c 2f41  ...</Type>...</A
+00002240: 7474 7269 6275 7465 3e0a 0909 3c41 7474  ttribute>...<Att
+00002250: 7269 6275 7465 206e 616d 653d 22d0 9fd0  ribute name="...
+00002260: b0d1 80d0 bed0 bbd1 8c22 2069 643d 2239  ........." id="9
+00002270: 223e 0a09 0909 3c54 6974 6c65 3e0a 0909  ">....<Title>...
+00002280: 0909 3c76 383a 6974 656d 3e0a 0909 0909  ..<v8:item>.....
+00002290: 093c 7638 3a6c 616e 673e 7275 3c2f 7638  .<v8:lang>ru</v8
+000022a0: 3a6c 616e 673e 0a09 0909 0909 3c76 383a  :lang>......<v8:
+000022b0: 636f 6e74 656e 743e d09f d0b0 d180 d0be  content>........
+000022c0: d0bb d18c 3c2f 7638 3a63 6f6e 7465 6e74  ....</v8:content
+000022d0: 3e0a 0909 0909 3c2f 7638 3a69 7465 6d3e  >.....</v8:item>
+000022e0: 0a09 0909 3c2f 5469 746c 653e 0a09 0909  ....</Title>....
+000022f0: 3c54 7970 653e 0a09 0909 093c 7638 3a54  <Type>.....<v8:T
+00002300: 7970 653e 7873 3a73 7472 696e 673c 2f76  ype>xs:string</v
+00002310: 383a 5479 7065 3e0a 0909 0909 3c76 383a  8:Type>.....<v8:
+00002320: 5374 7269 6e67 5175 616c 6966 6965 7273  StringQualifiers
+00002330: 3e0a 0909 0909 093c 7638 3a4c 656e 6774  >......<v8:Lengt
+00002340: 683e 303c 2f76 383a 4c65 6e67 7468 3e0a  h>0</v8:Length>.
+00002350: 0909 0909 093c 7638 3a41 6c6c 6f77 6564  .....<v8:Allowed
+00002360: 4c65 6e67 7468 3e56 6172 6961 626c 653c  Length>Variable<
+00002370: 2f76 383a 416c 6c6f 7765 644c 656e 6774  /v8:AllowedLengt
+00002380: 683e 0a09 0909 093c 2f76 383a 5374 7269  h>.....</v8:Stri
+00002390: 6e67 5175 616c 6966 6965 7273 3e0a 0909  ngQualifiers>...
+000023a0: 093c 2f54 7970 653e 0a09 0909 3c53 6176  .</Type>....<Sav
+000023b0: 653e 0a09 0909 093c 4669 656c 643e d09f  e>.....<Field>..
+000023c0: d0b0 d180 d0be d0bb d18c 3c2f 4669 656c  ..........</Fiel
+000023d0: 643e 0a09 0909 3c2f 5361 7665 3e0a 0909  d>....</Save>...
+000023e0: 3c2f 4174 7472 6962 7574 653e 0a09 093c  </Attribute>...<
+000023f0: 4174 7472 6962 7574 6520 6e61 6d65 3d22  Attribute name="
+00002400: d09a d0be d0b4 d0a0 d0b0 d0b7 d0b1 d0bb  ................
+00002410: d0be d0ba d0b8 d180 d0be d0b2 d0ba d0b8  ................
+00002420: 2220 6964 3d22 3130 223e 0a09 0909 3c54  " id="10">....<T
+00002430: 6974 6c65 3e0a 0909 0909 3c76 383a 6974  itle>.....<v8:it
+00002440: 656d 3e0a 0909 0909 093c 7638 3a6c 616e  em>......<v8:lan
+00002450: 673e 7275 3c2f 7638 3a6c 616e 673e 0a09  g>ru</v8:lang>..
+00002460: 0909 0909 3c76 383a 636f 6e74 656e 743e  ....<v8:content>
+00002470: d09a d0be d0b4 20d1 80d0 b0d0 b7d0 b1d0  ...... .........
+00002480: bbd0 bed0 bad0 b8d1 80d0 bed0 b2d0 bad0  ................
+00002490: b83c 2f76 383a 636f 6e74 656e 743e 0a09  .</v8:content>..
+000024a0: 0909 093c 2f76 383a 6974 656d 3e0a 0909  ...</v8:item>...
+000024b0: 093c 2f54 6974 6c65 3e0a 0909 093c 5479  .</Title>....<Ty
+000024c0: 7065 3e0a 0909 0909 3c76 383a 5479 7065  pe>.....<v8:Type
+000024d0: 3e78 733a 7374 7269 6e67 3c2f 7638 3a54  >xs:string</v8:T
+000024e0: 7970 653e 0a09 0909 093c 7638 3a53 7472  ype>.....<v8:Str
+000024f0: 696e 6751 7561 6c69 6669 6572 733e 0a09  ingQualifiers>..
+00002500: 0909 0909 3c76 383a 4c65 6e67 7468 3e31  ....<v8:Length>1
+00002510: 303c 2f76 383a 4c65 6e67 7468 3e0a 0909  0</v8:Length>...
+00002520: 0909 093c 7638 3a41 6c6c 6f77 6564 4c65  ...<v8:AllowedLe
+00002530: 6e67 7468 3e56 6172 6961 626c 653c 2f76  ngth>Variable</v
+00002540: 383a 416c 6c6f 7765 644c 656e 6774 683e  8:AllowedLength>
+00002550: 0a09 0909 093c 2f76 383a 5374 7269 6e67  .....</v8:String
+00002560: 5175 616c 6966 6965 7273 3e0a 0909 093c  Qualifiers>....<
+00002570: 2f54 7970 653e 0a09 093c 2f41 7474 7269  /Type>...</Attri
+00002580: 6275 7465 3e0a 0909 3c41 7474 7269 6275  bute>...<Attribu
+00002590: 7465 206e 616d 653d 22d0 92d1 8bd0 b3d1  te name=".......
+000025a0: 80d1 83d0 b6d0 b0d1 82d1 8cd0 a0d0 b0d1  ................
+000025b0: 81d1 88d0 b8d1 80d0 b5d0 bdd0 b8d1 8fd0  ................
+000025c0: 9253 7065 6322 2069 643d 2231 3122 3e0a  .Spec" id="11">.
+000025d0: 0909 093c 5469 746c 653e 0a09 0909 093c  ...<Title>.....<
+000025e0: 7638 3a69 7465 6d3e 0a09 0909 0909 3c76  v8:item>......<v
+000025f0: 383a 6c61 6e67 3e72 753c 2f76 383a 6c61  8:lang>ru</v8:la
+00002600: 6e67 3e0a 0909 0909 093c 7638 3a63 6f6e  ng>......<v8:con
+00002610: 7465 6e74 3ed0 92d1 8bd0 b3d1 80d1 83d0  tent>...........
+00002620: b6d0 b0d1 82d1 8c20 d180 d0b0 d181 d188  ....... ........
+00002630: d0b8 d180 d0b5 d0bd d0b8 d18f 20d0 b220  ............ .. 
+00002640: 7370 6563 3c2f 7638 3a63 6f6e 7465 6e74  spec</v8:content
+00002650: 3e0a 0909 0909 3c2f 7638 3a69 7465 6d3e  >.....</v8:item>
+00002660: 0a09 0909 3c2f 5469 746c 653e 0a09 0909  ....</Title>....
+00002670: 3c54 7970 653e 0a09 0909 093c 7638 3a54  <Type>.....<v8:T
+00002680: 7970 653e 7873 3a62 6f6f 6c65 616e 3c2f  ype>xs:boolean</
+00002690: 7638 3a54 7970 653e 0a09 0909 3c2f 5479  v8:Type>....</Ty
+000026a0: 7065 3e0a 0909 3c2f 4174 7472 6962 7574  pe>...</Attribut
+000026b0: 653e 0a09 093c 4174 7472 6962 7574 6520  e>...<Attribute 
+000026c0: 6e61 6d65 3d22 d09f d0be d0b4 d0bc d0b5  name="..........
+000026d0: d0bd d0b8 d182 d18c d09f d183 d182 d18c  ................
+000026e0: 5275 6e6e 6572 2220 6964 3d22 3622 3e0a  Runner" id="6">.
+000026f0: 0909 093c 5469 746c 653e 0a09 0909 093c  ...<Title>.....<
+00002700: 7638 3a69 7465 6d3e 0a09 0909 0909 3c76  v8:item>......<v
+00002710: 383a 6c61 6e67 3e72 753c 2f76 383a 6c61  8:lang>ru</v8:la
+00002720: 6e67 3e0a 0909 0909 093c 7638 3a63 6f6e  ng>......<v8:con
+00002730: 7465 6e74 3ed0 9fd0 bed0 b4d0 bcd0 b5d0  tent>...........
+00002740: bdd0 b8d1 82d1 8c20 d0bf d183 d182 d18c  ....... ........
+00002750: 2072 756e 6e65 723c 2f76 383a 636f 6e74   runner</v8:cont
+00002760: 656e 743e 0a09 0909 093c 2f76 383a 6974  ent>.....</v8:it
+00002770: 656d 3e0a 0909 093c 2f54 6974 6c65 3e0a  em>....</Title>.
+00002780: 0909 093c 5479 7065 3e0a 0909 0909 3c76  ...<Type>.....<v
+00002790: 383a 5479 7065 3e78 733a 626f 6f6c 6561  8:Type>xs:boolea
+000027a0: 6e3c 2f76 383a 5479 7065 3e0a 0909 093c  n</v8:Type>....<
+000027b0: 2f54 7970 653e 0a09 093c 2f41 7474 7269  /Type>...</Attri
+000027c0: 6275 7465 3e0a 093c 2f41 7474 7269 6275  bute>..</Attribu
+000027d0: 7465 733e 0a09 3c43 6f6d 6d61 6e64 733e  tes>..<Commands>
+000027e0: 0a09 093c 436f 6d6d 616e 6420 6e61 6d65  ...<Command name
+000027f0: 3d22 d0a1 d0b4 d0b5 d0bb d0b0 d182 d18c  ="..............
+00002800: 2220 6964 3d22 3122 3e0a 0909 093c 5469  " id="1">....<Ti
+00002810: 746c 653e 0a09 0909 093c 7638 3a69 7465  tle>.....<v8:ite
+00002820: 6d3e 0a09 0909 0909 3c76 383a 6c61 6e67  m>......<v8:lang
+00002830: 3e72 753c 2f76 383a 6c61 6e67 3e0a 0909  >ru</v8:lang>...
+00002840: 0909 093c 7638 3a63 6f6e 7465 6e74 3ed0  ...<v8:content>.
+00002850: a1d0 b4d0 b5d0 bbd0 b0d1 82d1 8c3c 2f76  .............</v
+00002860: 383a 636f 6e74 656e 743e 0a09 0909 093c  8:content>.....<
+00002870: 2f76 383a 6974 656d 3e0a 0909 093c 2f54  /v8:item>....</T
+00002880: 6974 6c65 3e0a 0909 093c 546f 6f6c 5469  itle>....<ToolTi
+00002890: 703e 0a09 0909 093c 7638 3a69 7465 6d3e  p>.....<v8:item>
+000028a0: 0a09 0909 0909 3c76 383a 6c61 6e67 3e72  ......<v8:lang>r
+000028b0: 753c 2f76 383a 6c61 6e67 3e0a 0909 0909  u</v8:lang>.....
+000028c0: 093c 7638 3a63 6f6e 7465 6e74 3ed0 a1d0  .<v8:content>...
+000028d0: b4d0 b5d0 bbd0 b0d1 82d1 8c3c 2f76 383a  ...........</v8:
+000028e0: 636f 6e74 656e 743e 0a09 0909 093c 2f76  content>.....</v
+000028f0: 383a 6974 656d 3e0a 0909 093c 2f54 6f6f  8:item>....</Too
+00002900: 6c54 6970 3e0a 0909 093c 4163 7469 6f6e  lTip>....<Action
+00002910: 3ed0 a1d0 b4d0 b5d0 bbd0 b0d1 82d1 8c3c  >..............<
+00002920: 2f41 6374 696f 6e3e 0a09 0909 3c43 7572  /Action>....<Cur
+00002930: 7265 6e74 526f 7755 7365 3e44 6f6e 7455  rentRowUse>DontU
+00002940: 7365 3c2f 4375 7272 656e 7452 6f77 5573  se</CurrentRowUs
+00002950: 653e 0a09 093c 2f43 6f6d 6d61 6e64 3e0a  e>...</Command>.
+00002960: 093c 2f43 6f6d 6d61 6e64 733e 0a3c 2f46  .</Commands>.</F
+00002970: 6f72 6d3e                                orm>
```

### Comparing `runner1c-0.58/runner1c/tools/epf/Runner1C/Forms/Form.xml` & `runner1c-0.59/runner1c/tools/epf/Runner1C/Forms/Form.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c/tools/epf/Runner1C.xml` & `runner1c-0.59/runner1c/tools/epf/Runner1C.xml`

 * *Files identical despite different names*

### Comparing `runner1c-0.58/runner1c.egg-info/SOURCES.txt` & `runner1c-0.59/runner1c.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 README.md
 setup.py
 runner1c/__init__.py
 runner1c/command.py
 runner1c/common.py
 runner1c/core.py
 runner1c/exit_code.py
+runner1c/logger.py
 runner1c/parser.py
 runner1c.egg-info/PKG-INFO
 runner1c.egg-info/SOURCES.txt
 runner1c.egg-info/dependency_links.txt
 runner1c.egg-info/entry_points.txt
 runner1c.egg-info/requires.txt
 runner1c.egg-info/top_level.txt
 runner1c/build/README.md
-runner1c/build/tests/repo/epf/CheckConfig.epf
 runner1c/build/tools/epf/ChangeSafeModeForExtension.epf
 runner1c/build/tools/epf/CloseAfterUpdate.epf
 runner1c/build/tools/epf/FileCompareMxl.epf
 runner1c/build/tools/epf/Runner1C.epf
 runner1c/commands/__init__.py
 runner1c/commands/base_for_test.py
 runner1c/commands/create_base.py
```

### Comparing `runner1c-0.58/setup.py` & `runner1c-0.59/setup.py`

 * *Files identical despite different names*

