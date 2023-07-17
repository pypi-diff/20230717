# Comparing `tmp/renderg-sdk-0.1.5.tar.gz` & `tmp/renderg-sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\renderg-sdk-0.1.5.tar", last modified: Wed Jul 12 07:53:13 2023, max compression
+gzip compressed data, was "dist\renderg-sdk-0.1.6.tar", last modified: Mon Jul 17 09:38:02 2023, max compression
```

## Comparing `renderg-sdk-0.1.5.tar` & `renderg-sdk-0.1.6.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/
--rw-rw-rw-   0        0        0     3341 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2960 2023-07-12 07:52:09.000000 renderg-sdk-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/analyze_houdini/
--rw-rw-rw-   0        0        0       52 2023-06-20 02:05:27.000000 renderg-sdk-0.1.5/analyze_houdini/__init__.py
--rw-rw-rw-   0        0        0     4084 2023-07-12 07:52:09.000000 renderg-sdk-0.1.5/analyze_houdini/analyze.py
-drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/analyze_houdini/houdini/
--rw-rw-rw-   0        0        0   942080 2023-05-22 08:30:57.000000 renderg-sdk-0.1.5/analyze_houdini/houdini/HoudiniAnalyze.pyd
--rw-rw-rw-   0        0        0  1128448 2023-05-22 08:30:57.000000 renderg-sdk-0.1.5/analyze_houdini/houdini/HoudiniAnalyze_py37.pyd
--rw-rw-rw-   0        0        0   820224 2023-05-22 08:30:57.000000 renderg-sdk-0.1.5/analyze_houdini/houdini/HoudiniAnalyze_py39.pyd
--rw-rw-rw-   0        0        0      708 2023-05-26 09:16:22.000000 renderg-sdk-0.1.5/analyze_houdini/houdini/run.py
-drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/ascp/
--rw-rw-rw-   0        0        0        0 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/ascp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/ascp/bin/
--rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-file-l1-2-0.dll
--rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-file-l2-1-0.dll
--rw-rw-rw-   0        0        0    25176 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-localization-l1-2-0.dll
--rw-rw-rw-   0        0        0    23120 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-processthreads-l1-1-1.dll
--rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-synch-l1-2-0.dll
--rw-rw-rw-   0        0        0    22616 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-timezone-l1-1-0.dll
--rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-xstate-l2-1-0.dll
--rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-conio-l1-1-0.dll
--rw-rw-rw-   0        0        0    26704 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-convert-l1-1-0.dll
--rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-environment-l1-1-0.dll
--rw-rw-rw-   0        0        0    24656 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-filesystem-l1-1-0.dll
--rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-heap-l1-1-0.dll
--rw-rw-rw-   0        0        0    23120 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-locale-l1-1-0.dll
--rw-rw-rw-   0        0        0    33360 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-math-l1-1-0.dll
--rw-rw-rw-   0        0        0    30800 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-multibyte-l1-1-0.dll
--rw-rw-rw-   0        0        0    75344 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-private-l1-1-0.dll
--rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-process-l1-1-0.dll
--rw-rw-rw-   0        0        0    27216 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-runtime-l1-1-0.dll
--rw-rw-rw-   0        0        0    28752 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-stdio-l1-1-0.dll
--rw-rw-rw-   0        0        0    28752 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-string-l1-1-0.dll
--rw-rw-rw-   0        0        0    25168 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-time-l1-1-0.dll
--rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-utility-l1-1-0.dll
--rw-rw-rw-   0        0        0    22616 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/api-ms-win-eventing-provider-l1-1-0.dll
--rwxrwxrwx   0        0        0  3075664 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/ascp.exe
--rwxrwxrwx   0        0        0  2299472 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/ascp4.exe
--rw-rw-rw-   0        0        0   870103 2023-06-20 02:06:37.000000 renderg-sdk-0.1.5/ascp/bin/aspera-scp-transfer.0.log
--rw-rw-rw-   0        0        0    58519 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/aspera-scp-transfer.log
--rwxrwxrwx   0        0        0  8328272 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/aspera.exe
--rw-rw-rw-   0        0        0   246864 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/concrt140.dll
--rw-rw-rw-   0        0        0  1444944 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/fasp3_shared.dll
--rw-rw-rw-   0        0        0  1292880 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/libeay32.dll
--rw-rw-rw-   0        0        0   434768 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/msvcp100.dll
--rw-rw-rw-   0        0        0   442968 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/msvcp140.dll
--rw-rw-rw-   0        0        0   783952 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/msvcr100.dll
--rw-rw-rw-   0        0        0   293976 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/ssleay32.dll
--rw-rw-rw-   0        0        0   886872 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/ucrtbase.dll
--rw-rw-rw-   0        0        0   270928 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/vccorlib140.dll
--rw-rw-rw-   0        0        0    88664 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/bin/vcruntime140.dll
-drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/ascp/etc/
--rw-rw-rw-   0        0        0     1622 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/etc/aspera-license
--rw-rw-rw-   0        0        0      121 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/etc/aspera.conf
--rw-rw-rw-   0        0        0     3380 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/etc/aspera_tokenauth_id_rsa
--rw-rw-rw-   0        0        0      680 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/etc/asperaweb_id_dsa.openssh
--rw-rw-rw-   0        0        0      806 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/etc/asperaweb_id_dsa.putty
--rw-rw-rw-   0        0        0   218894 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/ascp/etc/curl-ca-bundle.crt
-drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_api/
--rw-rw-rw-   0        0        0       39 2023-06-15 06:53:33.000000 renderg-sdk-0.1.5/renderg_api/__init__.py
--rw-rw-rw-   0        0        0     2249 2023-06-16 01:07:50.000000 renderg-sdk-0.1.5/renderg_api/connect.py
--rw-rw-rw-   0        0        0      518 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/renderg_api/constants.py
--rw-rw-rw-   0        0        0     1183 2023-06-15 06:53:33.000000 renderg-sdk-0.1.5/renderg_api/core.py
--rw-rw-rw-   0        0        0      393 2023-06-15 01:37:04.000000 renderg-sdk-0.1.5/renderg_api/exception.py
-drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_api/operators/
--rw-rw-rw-   0        0        0      328 2023-06-15 02:47:54.000000 renderg-sdk-0.1.5/renderg_api/operators/__init__.py
--rw-rw-rw-   0        0        0      989 2023-06-15 08:50:33.000000 renderg-sdk-0.1.5/renderg_api/operators/env.py
--rw-rw-rw-   0        0        0     2496 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/renderg_api/operators/job.py
--rw-rw-rw-   0        0        0      103 2023-06-15 02:27:45.000000 renderg-sdk-0.1.5/renderg_api/operators/project.py
--rw-rw-rw-   0        0        0      100 2023-06-15 02:27:45.000000 renderg-sdk-0.1.5/renderg_api/operators/task.py
--rw-rw-rw-   0        0        0     1059 2023-06-15 08:52:48.000000 renderg-sdk-0.1.5/renderg_api/operators/transfer.py
--rw-rw-rw-   0        0        0      100 2023-06-15 02:27:45.000000 renderg-sdk-0.1.5/renderg_api/operators/user.py
-drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_api/param_check/
--rw-rw-rw-   0        0        0       61 2023-06-15 06:14:24.000000 renderg-sdk-0.1.5/renderg_api/param_check/__init__.py
--rw-rw-rw-   0        0        0     3195 2023-07-12 07:52:09.000000 renderg-sdk-0.1.5/renderg_api/param_check/check.py
--rw-rw-rw-   0        0        0      728 2023-06-16 01:12:35.000000 renderg-sdk-0.1.5/renderg_api/urls.py
-drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_sdk.egg-info/
--rw-rw-rw-   0        0        0     3341 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2652 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       62 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_sdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_upload/
--rw-rw-rw-   0        0        0        0 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/renderg_upload/__init__.py
--rw-rw-rw-   0        0        0      159 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/renderg_upload/asperaTransfer.py
--rw-rw-rw-   0        0        0     1474 2023-06-16 07:10:02.000000 renderg-sdk-0.1.5/renderg_upload/asperaTransferHelper.py
--rw-rw-rw-   0        0        0     3920 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/renderg_upload/assetsPathHelper.py
--rw-rw-rw-   0        0        0     2309 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/renderg_upload/rgUpload.py
-drwxrwxrwx   0        0        0        0 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/renderg_utils/
--rw-rw-rw-   0        0        0      113 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/renderg_utils/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/renderg_utils/constants.py
--rw-rw-rw-   0        0        0     1131 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/renderg_utils/exception.py
--rw-rw-rw-   0        0        0     2655 2023-07-12 07:50:32.000000 renderg-sdk-0.1.5/renderg_utils/utils.py
--rw-rw-rw-   0        0        0       42 2023-07-12 07:53:13.000000 renderg-sdk-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      980 2023-07-12 07:52:09.000000 renderg-sdk-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:38:02.000000 renderg-sdk-0.1.6/
+-rw-rw-rw-   0        0        0     3341 2023-07-17 09:38:02.000000 renderg-sdk-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2960 2023-07-17 03:00:02.000000 renderg-sdk-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 09:37:57.000000 renderg-sdk-0.1.6/analyze_houdini/
+-rw-rw-rw-   0        0        0       52 2023-06-20 02:05:27.000000 renderg-sdk-0.1.6/analyze_houdini/__init__.py
+-rw-rw-rw-   0        0        0     4084 2023-07-12 07:52:09.000000 renderg-sdk-0.1.6/analyze_houdini/analyze.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:37:57.000000 renderg-sdk-0.1.6/analyze_houdini/houdini/
+-rw-rw-rw-   0        0        0   942080 2023-05-22 08:30:57.000000 renderg-sdk-0.1.6/analyze_houdini/houdini/HoudiniAnalyze.pyd
+-rw-rw-rw-   0        0        0  1128448 2023-05-22 08:30:57.000000 renderg-sdk-0.1.6/analyze_houdini/houdini/HoudiniAnalyze_py37.pyd
+-rw-rw-rw-   0        0        0   820224 2023-05-22 08:30:57.000000 renderg-sdk-0.1.6/analyze_houdini/houdini/HoudiniAnalyze_py39.pyd
+-rw-rw-rw-   0        0        0      708 2023-05-26 09:16:22.000000 renderg-sdk-0.1.6/analyze_houdini/houdini/run.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:37:57.000000 renderg-sdk-0.1.6/ascp/
+-rw-rw-rw-   0        0        0        0 2023-07-12 07:50:32.000000 renderg-sdk-0.1.6/ascp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:38:02.000000 renderg-sdk-0.1.6/ascp/bin/
+-rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-core-file-l1-2-0.dll
+-rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-core-file-l2-1-0.dll
+-rw-rw-rw-   0        0        0    25176 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-core-localization-l1-2-0.dll
+-rw-rw-rw-   0        0        0    23120 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-core-processthreads-l1-1-1.dll
+-rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-core-synch-l1-2-0.dll
+-rw-rw-rw-   0        0        0    22616 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-core-timezone-l1-1-0.dll
+-rw-rw-rw-   0        0        0    22608 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-core-xstate-l2-1-0.dll
+-rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-conio-l1-1-0.dll
+-rw-rw-rw-   0        0        0    26704 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-convert-l1-1-0.dll
+-rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-environment-l1-1-0.dll
+-rw-rw-rw-   0        0        0    24656 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-filesystem-l1-1-0.dll
+-rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-heap-l1-1-0.dll
+-rw-rw-rw-   0        0        0    23120 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-locale-l1-1-0.dll
+-rw-rw-rw-   0        0        0    33360 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-math-l1-1-0.dll
+-rw-rw-rw-   0        0        0    30800 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-multibyte-l1-1-0.dll
+-rw-rw-rw-   0        0        0    75344 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-private-l1-1-0.dll
+-rw-rw-rw-   0        0        0    23632 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-process-l1-1-0.dll
+-rw-rw-rw-   0        0        0    27216 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-runtime-l1-1-0.dll
+-rw-rw-rw-   0        0        0    28752 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-stdio-l1-1-0.dll
+-rw-rw-rw-   0        0        0    28752 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-string-l1-1-0.dll
+-rw-rw-rw-   0        0        0    25168 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-time-l1-1-0.dll
+-rw-rw-rw-   0        0        0    23128 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-utility-l1-1-0.dll
+-rw-rw-rw-   0        0        0    22616 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/api-ms-win-eventing-provider-l1-1-0.dll
+-rwxrwxrwx   0        0        0  3075664 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/ascp.exe
+-rwxrwxrwx   0        0        0  2299472 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/ascp4.exe
+-rw-rw-rw-   0        0        0   870103 2023-06-20 02:06:37.000000 renderg-sdk-0.1.6/ascp/bin/aspera-scp-transfer.0.log
+-rw-rw-rw-   0        0        0    58519 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/aspera-scp-transfer.log
+-rwxrwxrwx   0        0        0  8328272 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/aspera.exe
+-rw-rw-rw-   0        0        0   246864 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/concrt140.dll
+-rw-rw-rw-   0        0        0  1444944 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/fasp3_shared.dll
+-rw-rw-rw-   0        0        0  1292880 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/libeay32.dll
+-rw-rw-rw-   0        0        0   434768 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/msvcp100.dll
+-rw-rw-rw-   0        0        0   442968 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/msvcp140.dll
+-rw-rw-rw-   0        0        0   783952 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/msvcr100.dll
+-rw-rw-rw-   0        0        0   293976 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/ssleay32.dll
+-rw-rw-rw-   0        0        0   886872 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/ucrtbase.dll
+-rw-rw-rw-   0        0        0   270928 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/vccorlib140.dll
+-rw-rw-rw-   0        0        0    88664 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/bin/vcruntime140.dll
+drwxrwxrwx   0        0        0        0 2023-07-17 09:38:02.000000 renderg-sdk-0.1.6/ascp/etc/
+-rw-rw-rw-   0        0        0     1622 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/etc/aspera-license
+-rw-rw-rw-   0        0        0      121 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/etc/aspera.conf
+-rw-rw-rw-   0        0        0     3380 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/etc/aspera_tokenauth_id_rsa
+-rw-rw-rw-   0        0        0      680 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/etc/asperaweb_id_dsa.openssh
+-rw-rw-rw-   0        0        0      806 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/etc/asperaweb_id_dsa.putty
+-rw-rw-rw-   0        0        0   218894 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/ascp/etc/curl-ca-bundle.crt
+drwxrwxrwx   0        0        0        0 2023-07-17 09:38:02.000000 renderg-sdk-0.1.6/renderg_api/
+-rw-rw-rw-   0        0        0       39 2023-06-15 06:53:33.000000 renderg-sdk-0.1.6/renderg_api/__init__.py
+-rw-rw-rw-   0        0        0     2345 2023-07-17 05:31:35.000000 renderg-sdk-0.1.6/renderg_api/connect.py
+-rw-rw-rw-   0        0        0      518 2023-07-12 07:50:32.000000 renderg-sdk-0.1.6/renderg_api/constants.py
+-rw-rw-rw-   0        0        0     1183 2023-07-17 03:00:02.000000 renderg-sdk-0.1.6/renderg_api/core.py
+-rw-rw-rw-   0        0        0      393 2023-06-15 01:37:04.000000 renderg-sdk-0.1.6/renderg_api/exception.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:38:02.000000 renderg-sdk-0.1.6/renderg_api/operators/
+-rw-rw-rw-   0        0        0      328 2023-06-15 02:47:54.000000 renderg-sdk-0.1.6/renderg_api/operators/__init__.py
+-rw-rw-rw-   0        0        0      989 2023-06-15 08:50:33.000000 renderg-sdk-0.1.6/renderg_api/operators/env.py
+-rw-rw-rw-   0        0        0     2496 2023-07-17 03:00:02.000000 renderg-sdk-0.1.6/renderg_api/operators/job.py
+-rw-rw-rw-   0        0        0      103 2023-06-15 02:27:45.000000 renderg-sdk-0.1.6/renderg_api/operators/project.py
+-rw-rw-rw-   0        0        0      100 2023-06-15 02:27:45.000000 renderg-sdk-0.1.6/renderg_api/operators/task.py
+-rw-rw-rw-   0        0        0     1059 2023-07-17 03:00:02.000000 renderg-sdk-0.1.6/renderg_api/operators/transfer.py
+-rw-rw-rw-   0        0        0      382 2023-07-17 03:25:49.000000 renderg-sdk-0.1.6/renderg_api/operators/user.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:38:02.000000 renderg-sdk-0.1.6/renderg_api/param_check/
+-rw-rw-rw-   0        0        0       61 2023-06-15 06:14:24.000000 renderg-sdk-0.1.6/renderg_api/param_check/__init__.py
+-rw-rw-rw-   0        0        0     3195 2023-07-12 07:52:09.000000 renderg-sdk-0.1.6/renderg_api/param_check/check.py
+-rw-rw-rw-   0        0        0      829 2023-07-17 03:25:27.000000 renderg-sdk-0.1.6/renderg_api/urls.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:38:02.000000 renderg-sdk-0.1.6/renderg_sdk.egg-info/
+-rw-rw-rw-   0        0        0     3341 2023-07-17 09:37:57.000000 renderg-sdk-0.1.6/renderg_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2652 2023-07-17 09:37:57.000000 renderg-sdk-0.1.6/renderg_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 09:37:57.000000 renderg-sdk-0.1.6/renderg_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-17 09:37:57.000000 renderg-sdk-0.1.6/renderg_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       62 2023-07-17 09:37:57.000000 renderg-sdk-0.1.6/renderg_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 09:38:02.000000 renderg-sdk-0.1.6/renderg_upload/
+-rw-rw-rw-   0        0        0        0 2023-07-17 03:00:02.000000 renderg-sdk-0.1.6/renderg_upload/__init__.py
+-rw-rw-rw-   0        0        0      159 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/renderg_upload/asperaTransfer.py
+-rw-rw-rw-   0        0        0     1474 2023-06-16 07:10:02.000000 renderg-sdk-0.1.6/renderg_upload/asperaTransferHelper.py
+-rw-rw-rw-   0        0        0     3920 2023-07-12 07:50:32.000000 renderg-sdk-0.1.6/renderg_upload/assetsPathHelper.py
+-rw-rw-rw-   0        0        0     2309 2023-07-17 03:00:02.000000 renderg-sdk-0.1.6/renderg_upload/rgUpload.py
+drwxrwxrwx   0        0        0        0 2023-07-17 09:38:02.000000 renderg-sdk-0.1.6/renderg_utils/
+-rw-rw-rw-   0        0        0      113 2023-07-12 07:50:32.000000 renderg-sdk-0.1.6/renderg_utils/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 07:50:32.000000 renderg-sdk-0.1.6/renderg_utils/constants.py
+-rw-rw-rw-   0        0        0     1131 2023-07-12 07:50:32.000000 renderg-sdk-0.1.6/renderg_utils/exception.py
+-rw-rw-rw-   0        0        0     2655 2023-07-12 07:50:32.000000 renderg-sdk-0.1.6/renderg_utils/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-17 09:38:02.000000 renderg-sdk-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      980 2023-07-17 09:37:55.000000 renderg-sdk-0.1.6/setup.py
```

### Comparing `renderg-sdk-0.1.5/PKG-INFO` & `renderg-sdk-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renderg-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: www.renderg.com
 Home-page: https://github.com/renderg-repo/renderg-sdk.git
 Author: RenderG
 Author-email: support@renderg.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `renderg-sdk-0.1.5/README.md` & `renderg-sdk-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/analyze_houdini/analyze.py` & `renderg-sdk-0.1.6/analyze_houdini/analyze.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/analyze_houdini/houdini/run.py` & `renderg-sdk-0.1.6/analyze_houdini/houdini/run.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-file-l1-2-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-core-file-l1-2-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-file-l2-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-core-file-l2-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-localization-l1-2-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-core-localization-l1-2-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-processthreads-l1-1-1.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-core-processthreads-l1-1-1.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-synch-l1-2-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-core-synch-l1-2-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-timezone-l1-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-core-timezone-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-core-xstate-l2-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-core-xstate-l2-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-conio-l1-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-conio-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-convert-l1-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-convert-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-environment-l1-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-environment-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-filesystem-l1-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-filesystem-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-heap-l1-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-heap-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-locale-l1-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-locale-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-math-l1-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-math-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-multibyte-l1-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-multibyte-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-private-l1-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-private-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-process-l1-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-process-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-runtime-l1-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-runtime-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-stdio-l1-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-stdio-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-string-l1-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-string-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-time-l1-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-time-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-crt-utility-l1-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-crt-utility-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/api-ms-win-eventing-provider-l1-1-0.dll` & `renderg-sdk-0.1.6/ascp/bin/api-ms-win-eventing-provider-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/ascp.exe` & `renderg-sdk-0.1.6/ascp/bin/ascp.exe`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/ascp4.exe` & `renderg-sdk-0.1.6/ascp/bin/ascp4.exe`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/aspera-scp-transfer.0.log` & `renderg-sdk-0.1.6/ascp/bin/aspera-scp-transfer.0.log`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/aspera-scp-transfer.log` & `renderg-sdk-0.1.6/ascp/bin/aspera-scp-transfer.log`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/aspera.exe` & `renderg-sdk-0.1.6/ascp/bin/aspera.exe`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/concrt140.dll` & `renderg-sdk-0.1.6/ascp/bin/concrt140.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/fasp3_shared.dll` & `renderg-sdk-0.1.6/ascp/bin/fasp3_shared.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/libeay32.dll` & `renderg-sdk-0.1.6/ascp/bin/libeay32.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/msvcp100.dll` & `renderg-sdk-0.1.6/ascp/bin/msvcp100.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/msvcp140.dll` & `renderg-sdk-0.1.6/ascp/bin/msvcp140.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/msvcr100.dll` & `renderg-sdk-0.1.6/ascp/bin/msvcr100.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/ssleay32.dll` & `renderg-sdk-0.1.6/ascp/bin/ssleay32.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/ucrtbase.dll` & `renderg-sdk-0.1.6/ascp/bin/ucrtbase.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/vccorlib140.dll` & `renderg-sdk-0.1.6/ascp/bin/vccorlib140.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/bin/vcruntime140.dll` & `renderg-sdk-0.1.6/ascp/bin/vcruntime140.dll`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/etc/aspera-license` & `renderg-sdk-0.1.6/ascp/etc/aspera-license`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/etc/aspera_tokenauth_id_rsa` & `renderg-sdk-0.1.6/ascp/etc/aspera_tokenauth_id_rsa`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/etc/asperaweb_id_dsa.openssh` & `renderg-sdk-0.1.6/ascp/etc/asperaweb_id_dsa.openssh`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/etc/asperaweb_id_dsa.putty` & `renderg-sdk-0.1.6/ascp/etc/asperaweb_id_dsa.putty`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/ascp/etc/curl-ca-bundle.crt` & `renderg-sdk-0.1.6/ascp/etc/curl-ca-bundle.crt`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/renderg_api/connect.py` & `renderg-sdk-0.1.6/renderg_api/connect.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,45 +28,48 @@
 
     @property
     def headers(self):
         return self._headers
 
     @retry(reraise=True, stop=stop_after_attempt(5),
            wait=wait_random(min=1, max=2))
-    def post(self, api_url, data=None, validator=True):
+    def post(self, api_url, data=None, params=None, validator=True):
         if not data:
             data = {}
 
         if validator:
             # todo data validator
             pass
 
         request_url = assemble_api_url(self.domain, api_url, self._protocol)
         data = json.dumps(data)
 
-        response = self._session.post(request_url, data, headers=self._headers)
+        response = self._session.post(request_url, data=data, headers=self._headers, params=params)
         response_json = response.json()
+
         if not response.ok:
             response_code = response_json.get('error_code')
             raise RenderGAPIError(response_code, response_json.get("msg", ""), response.url)
 
         return response_json
 
     @retry(reraise=True, stop=stop_after_attempt(5),
            wait=wait_random(min=1, max=2))
-    def get(self, api_url, data=None, validator=True):
+    def get(self, api_url, data=None, params=None, validator=True):
         if not data:
             data = {}
 
         if validator:
             # todo data validator
             pass
 
         request_url = assemble_api_url(self.domain, api_url, self._protocol)
+        data = json.dumps(data)
 
-        response = self._session.get(request_url, params=data, headers=self._headers)
+        response = self._session.get(request_url, data=data, headers=self._headers, params=params)
         response_json = response.json()
+
         if not response.ok:
             response_code = response_json.get('error_code')
             raise RenderGAPIError(response_code, response_json.get("msg", ""), response.url)
 
         return response_json
```

### Comparing `renderg-sdk-0.1.5/renderg_api/constants.py` & `renderg-sdk-0.1.6/renderg_api/constants.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/renderg_api/core.py` & `renderg-sdk-0.1.6/renderg_api/core.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/renderg_api/operators/env.py` & `renderg-sdk-0.1.6/renderg_api/operators/env.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/renderg_api/operators/job.py` & `renderg-sdk-0.1.6/renderg_api/operators/job.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/renderg_api/operators/transfer.py` & `renderg-sdk-0.1.6/renderg_api/operators/transfer.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/renderg_api/param_check/check.py` & `renderg-sdk-0.1.6/renderg_api/param_check/check.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/renderg_api/urls.py` & `renderg-sdk-0.1.6/renderg_api/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,11 +12,14 @@
     NewJob = "/api/v1/front/job/add"
     UpdateJobStatus = "/api/v1/front/job/status"
     ControlJob = "/api/v1/front/job/control"
     SubmitJob = "/api/v1/front/job/submit"
     DelJob = "/api/v1/front/job/del"
     SetJobConfig = "/api/v1/front/job/cluster_id"
 
+    GetClusterList = "/api/v1/front/cluster/current"
+    GetZoneList = "/api/v1/front/zone/list"
+
     GetEnvList = "/api/v1/front/environment/list"
 
     GetTransferLine = "/api/v1/front/transfer/lines"
     GetTransferConfig = "/api/v1/front/job/transfer_plus"
```

### Comparing `renderg-sdk-0.1.5/renderg_sdk.egg-info/PKG-INFO` & `renderg-sdk-0.1.6/renderg_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renderg-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: www.renderg.com
 Home-page: https://github.com/renderg-repo/renderg-sdk.git
 Author: RenderG
 Author-email: support@renderg.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `renderg-sdk-0.1.5/renderg_sdk.egg-info/SOURCES.txt` & `renderg-sdk-0.1.6/renderg_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/renderg_upload/asperaTransferHelper.py` & `renderg-sdk-0.1.6/renderg_upload/asperaTransferHelper.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/renderg_upload/assetsPathHelper.py` & `renderg-sdk-0.1.6/renderg_upload/assetsPathHelper.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/renderg_upload/rgUpload.py` & `renderg-sdk-0.1.6/renderg_upload/rgUpload.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/renderg_utils/exception.py` & `renderg-sdk-0.1.6/renderg_utils/exception.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/renderg_utils/utils.py` & `renderg-sdk-0.1.6/renderg_utils/utils.py`

 * *Files identical despite different names*

### Comparing `renderg-sdk-0.1.5/setup.py` & `renderg-sdk-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
         long_description = f.read()
     return long_description
 
 
 setup(
     name='renderg-sdk',
-    version='0.1.5',
+    version='0.1.6',
     url='https://github.com/renderg-repo/renderg-sdk.git',
     author='RenderG',
     author_email='support@renderg.com',
     description='www.renderg.com',
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

