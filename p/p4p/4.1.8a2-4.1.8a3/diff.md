# Comparing `tmp/p4p-4.1.8a2.tar.gz` & `tmp/p4p-4.1.8a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p4p-4.1.8a2.tar", last modified: Mon Jul  3 00:24:09 2023, max compression
+gzip compressed data, was "p4p-4.1.8a3.tar", last modified: Thu Jul  6 02:21:15 2023, max compression
```

## Comparing `p4p-4.1.8a2.tar` & `p4p-4.1.8a3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.315979 p4p-4.1.8a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-03 00:23:12.000000 p4p-4.1.8a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-03 00:23:12.000000 p4p-4.1.8a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-03 00:24:09.315979 p4p-4.1.8a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-03 00:23:12.000000 p4p-4.1.8a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-03 00:23:12.000000 p4p-4.1.8a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 00:24:09.315979 p4p-4.1.8a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4846 2023-07-03 00:23:12.000000 p4p-4.1.8a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.303979 p4p-4.1.8a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.303979 p4p-4.1.8a2/src/p4p/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/_gw.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/_p4p.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    27326 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/_p4p.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.307978 p4p-4.1.8a2/src/p4p/asLib/
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/asLib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/asLib/lex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/asLib/pvlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/asLib/yacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.307978 p4p-4.1.8a2/src/p4p/client/
--rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/client/Qt.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/client/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/client/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/client/cothread.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/client/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    15778 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/client/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/disect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/example.conf
--rw-r--r--   0 runner    (1001) docker     (123)    28038 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/gw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.307978 p4p-4.1.8a2/src/p4p/nt/
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/nt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/nt/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/nt/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/nt/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/nt/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvagw@.service
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.311978 p4p-4.1.8a2/src/p4p/pvxs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/client.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/data.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/log.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/nt.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/server.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/sharedArray.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/sharedpv.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/source.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/pvxs/version.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.311978 p4p-4.1.8a2/src/p4p/server/
--rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/server/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/server/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/server/cothread.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/server/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/server/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/set.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.315979 p4p-4.1.8a2/src/p4p/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/asynciotest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/cothreadtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/qttest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_asLib.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_client_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_client_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_cothread.py
--rw-r--r--   0 runner    (1001) docker     (123)    20146 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_gw.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_nt.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_sharedpv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/test_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:24:09.307978 p4p-4.1.8a2/src/p4p.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-03 00:24:09.000000 p4p-4.1.8a2/src/p4p.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-03 00:24:09.000000 p4p-4.1.8a2/src/p4p.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 00:24:09.000000 p4p-4.1.8a2/src/p4p.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-03 00:24:09.000000 p4p-4.1.8a2/src/p4p.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 00:24:09.000000 p4p-4.1.8a2/src/p4p.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-03 00:24:09.000000 p4p-4.1.8a2/src/p4p.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-03 00:24:09.000000 p4p-4.1.8a2/src/p4p.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/p4p.h
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/pvxs_client.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    30817 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/pvxs_gw.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/pvxs_gw.h
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/pvxs_odometer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/pvxs_sharedpv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/pvxs_source.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/pvxs_type.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-07-03 00:23:12.000000 p4p-4.1.8a2/src/pvxs_value.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:15.022584 p4p-4.1.8a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-06 02:20:26.000000 p4p-4.1.8a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-06 02:20:26.000000 p4p-4.1.8a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-06 02:21:15.022584 p4p-4.1.8a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-06 02:20:26.000000 p4p-4.1.8a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-06 02:20:26.000000 p4p-4.1.8a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 02:21:15.022584 p4p-4.1.8a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4846 2023-07-06 02:20:26.000000 p4p-4.1.8a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:15.010583 p4p-4.1.8a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:15.010583 p4p-4.1.8a3/src/p4p/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/_gw.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/_p4p.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    27326 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/_p4p.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:15.014584 p4p-4.1.8a3/src/p4p/asLib/
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/asLib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/asLib/lex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/asLib/pvlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/asLib/yacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:15.014584 p4p-4.1.8a3/src/p4p/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/client/Qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/client/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/client/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/client/cothread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/client/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15778 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/client/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/disect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/example.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    28038 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/gw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:15.014584 p4p-4.1.8a3/src/p4p/nt/
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/nt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/nt/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/nt/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/nt/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/nt/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/pvagw@.service
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:15.018584 p4p-4.1.8a3/src/p4p/pvxs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/pvxs/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/pvxs/client.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/pvxs/data.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/pvxs/log.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/pvxs/nt.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/pvxs/server.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/pvxs/sharedArray.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/pvxs/sharedpv.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/pvxs/source.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/pvxs/util.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/pvxs/version.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:15.018584 p4p-4.1.8a3/src/p4p/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/server/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/server/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/server/cothread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/server/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/server/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/set.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:15.022584 p4p-4.1.8a3/src/p4p/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/asynciotest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/cothreadtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/qttest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/test_asLib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/test_client_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/test_client_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/test_cothread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/test_gw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/test_nt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/test_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12614 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/test_sharedpv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/test_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:21:15.010583 p4p-4.1.8a3/src/p4p.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-06 02:21:14.000000 p4p-4.1.8a3/src/p4p.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-06 02:21:14.000000 p4p-4.1.8a3/src/p4p.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 02:21:14.000000 p4p-4.1.8a3/src/p4p.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 02:21:14.000000 p4p-4.1.8a3/src/p4p.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 02:21:14.000000 p4p-4.1.8a3/src/p4p.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-06 02:21:14.000000 p4p-4.1.8a3/src/p4p.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 02:21:14.000000 p4p-4.1.8a3/src/p4p.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/p4p.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/pvxs_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32737 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/pvxs_gw.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/pvxs_gw.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/pvxs_odometer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/pvxs_sharedpv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/pvxs_source.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/pvxs_type.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-07-06 02:20:26.000000 p4p-4.1.8a3/src/pvxs_value.cpp
```

### Comparing `p4p-4.1.8a2/LICENSE` & `p4p-4.1.8a3/LICENSE`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/PKG-INFO` & `p4p-4.1.8a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p4p
-Version: 4.1.8a2
+Version: 4.1.8a3
 Summary: Python interface to PVAccess protocol client
 Home-page: https://mdavidsaver.github.io/p4p
 Author: Michael Davidsaver
 Author-email: mdavidsaver@gmail.com
 License: BSD
 Keywords: epics scada
 Platform: UNKNOWN
```

### Comparing `p4p-4.1.8a2/setup.py` & `p4p-4.1.8a3/setup.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/__init__.py` & `p4p-4.1.8a3/src/p4p/__init__.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/_gw.pyx` & `p4p-4.1.8a3/src/p4p/_gw.pyx`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/_p4p.pyx` & `p4p-4.1.8a3/src/p4p/_p4p.pyx`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/asLib/__init__.py` & `p4p-4.1.8a3/src/p4p/asLib/__init__.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/asLib/lex.py` & `p4p-4.1.8a3/src/p4p/asLib/lex.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/asLib/pvlist.py` & `p4p-4.1.8a3/src/p4p/asLib/pvlist.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/asLib/yacc.py` & `p4p-4.1.8a3/src/p4p/asLib/yacc.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/client/Qt.py` & `p4p-4.1.8a3/src/p4p/client/Qt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from math import ceil
 
 from qtpy.QtCore import QObject, QCoreApplication, Signal, QEvent
 
 from . import raw
 from .raw import Disconnected, RemoteError, Cancelled, Finished
 from ..wrapper import Value, Type
 from .._p4p import ClientProvider
@@ -43,15 +44,15 @@
     _op = None
     _result = None
     # receives a Value or an Exception
     result = Signal(object)
 
     def __init__(self, parent, timeout):
         QObject.__init__(self, parent)
-        self._active = self.startTimer(timeout*1000)
+        self._active = self.startTimer(ceil(timeout*1000))
 
     def close(self):
         self._op.close()
 
     @exceptionGuard
     def timerEvent(self, evt):
         if self._result is None:
@@ -91,15 +92,15 @@
         # Rate limiting for multiple consumers is hard.
         # We throttle to the highest consumer rate (shortest holdoff).
         if self._holdoff is None or self._holdoff > holdoff:
             self._holdoff = holdoff
             if self._active is not None:
                 # restart timer
                 self.killTimer(self._active)
-                self._active = self.startTimer(self._holdoff)
+                self._active = self.startTimer(ceil(self._holdoff))
 
         # TODO: re-adjust on slot disconnect?
 
         # schedule to receive initial update later (avoids recursion)
         QCoreApplication.postEvent(self, CBEvent(slot))
 
     def _event(self):
@@ -116,15 +117,15 @@
         #   None - FIFO not empty (call pop())
         #   RemoteError
         #   Disconnected
         #   some method, adding new subscriber
 
         if E is None:
             if self._active is None:
-                self._active = self.startTimer(self._holdoff)
+                self._active = self.startTimer(ceil(self._holdoff))
                 _log.debug('Start timer with %s', self._holdoff)
             return
 
         else:
             E(self._last)
             self.update.connect(E)
```

### Comparing `p4p-4.1.8a2/src/p4p/client/asyncio.py` & `p4p-4.1.8a3/src/p4p/client/asyncio.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/client/cli.py` & `p4p-4.1.8a3/src/p4p/client/cli.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/client/cothread.py` & `p4p-4.1.8a3/src/p4p/client/cothread.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/client/raw.py` & `p4p-4.1.8a3/src/p4p/client/raw.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/client/thread.py` & `p4p-4.1.8a3/src/p4p/client/thread.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/disect.py` & `p4p-4.1.8a3/src/p4p/disect.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/example.conf` & `p4p-4.1.8a3/src/p4p/example.conf`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/gw.py` & `p4p-4.1.8a3/src/p4p/gw.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/nt/__init__.py` & `p4p-4.1.8a3/src/p4p/nt/__init__.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/nt/common.py` & `p4p-4.1.8a3/src/p4p/nt/common.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/nt/enum.py` & `p4p-4.1.8a3/src/p4p/nt/enum.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/nt/ndarray.py` & `p4p-4.1.8a3/src/p4p/nt/ndarray.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/nt/scalar.py` & `p4p-4.1.8a3/src/p4p/nt/scalar.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/pvagw@.service` & `p4p-4.1.8a3/src/p4p/pvagw@.service`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/pvxs/client.pxd` & `p4p-4.1.8a3/src/p4p/pvxs/client.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/pvxs/data.pxd` & `p4p-4.1.8a3/src/p4p/pvxs/data.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/pvxs/server.pxd` & `p4p-4.1.8a3/src/p4p/pvxs/server.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/pvxs/sharedArray.pxd` & `p4p-4.1.8a3/src/p4p/pvxs/sharedArray.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/pvxs/sharedpv.pxd` & `p4p-4.1.8a3/src/p4p/pvxs/sharedpv.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/pvxs/source.pxd` & `p4p-4.1.8a3/src/p4p/pvxs/source.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/rpc.py` & `p4p-4.1.8a3/src/p4p/rpc.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/server/__init__.py` & `p4p-4.1.8a3/src/p4p/server/__init__.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/server/asyncio.py` & `p4p-4.1.8a3/src/p4p/server/asyncio.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/server/cli.py` & `p4p-4.1.8a3/src/p4p/server/cli.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/server/cothread.py` & `p4p-4.1.8a3/src/p4p/server/cothread.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/server/raw.py` & `p4p-4.1.8a3/src/p4p/server/raw.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/server/thread.py` & `p4p-4.1.8a3/src/p4p/server/thread.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/set.pxd` & `p4p-4.1.8a3/src/p4p/set.pxd`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/test/asynciotest.py` & `p4p-4.1.8a3/src/p4p/test/asynciotest.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/test/cothreadtest.py` & `p4p-4.1.8a3/src/p4p/test/cothreadtest.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         with Server(providers=[self.provider], isolate=True) as S:
             with Context('pva', conf=S.conf(), useenv=False) as C:
 
                 args = NTURI([
                     ('oops', '?'),
                 ])
 
-                with self.assertRaisesRegexp(RemoteError, 'oops'):
+                with self.assertRaisesRegex(RemoteError, 'oops'):
                     ret = C.rpc('foo', args.wrap('foo', kws={'oops':True}))
 
 class TestFirstLast(RefTestCase):
     maxDiff = 1000
     timeout = 1.0
     mode = 'Mask'
```

### Comparing `p4p-4.1.8a2/src/p4p/test/qttest.py` & `p4p-4.1.8a3/src/p4p/test/qttest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import unittest
 from functools import wraps
+from math import ceil
 
 from qtpy.QtCore import QObject, QCoreApplication
 
 from ..client.Qt import exceptionGuard, Disconnected, TimeoutError, Context
 
 from ..server import Server, StaticProvider
 from ..server.thread import SharedPV, _defaultWorkQueue
@@ -45,15 +46,15 @@
         _log.debug('signalled %s', args)
         self._args = args
         QCoreApplication.instance().quit()
         self.close()
 
     def wait(self, timeout=5.0):
         assert self._T is None, self._T
-        self._T = self.startTimer(timeout*1000)
+        self._T = self.startTimer(ceil(timeout*1000))
         try:
             self._args = None
             QCoreApplication.instance().exec_()
             if self._args is not None:
                 return self._args
 
             else:
```

### Comparing `p4p-4.1.8a2/src/p4p/test/test_asLib.py` & `p4p-4.1.8a3/src/p4p/test/test_asLib.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/test/test_client_raw.py` & `p4p-4.1.8a3/src/p4p/test/test_client_raw.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/test/test_client_thread.py` & `p4p-4.1.8a3/src/p4p/test/test_client_thread.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/test/test_gw.py` & `p4p-4.1.8a3/src/p4p/test/test_gw.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,26 +35,26 @@
             try:
                 main(['--example-config', F.name])
             except SystemExit as e:
                 self.assertEqual(e.code, 0)
 
             F.seek(0)
             content = F.read()
-            self.assertRegexpMatches(content, '"statusprefix"')
+            self.assertRegex(content, '"statusprefix"')
 
     def test_systemd(self):
         with NamedTemporaryFile() as F:
             try:
                 main(['--example-systemd', F.name])
             except SystemExit as e:
                 self.assertEqual(e.code, 0)
 
             F.seek(0)
             content = F.read()
-            self.assertRegexpMatches(content, 'multi-user.target')
+            self.assertRegex(content, 'multi-user.target')
 
 class TestGC(RefTestCase):
     def test_empty(self):
         class Dummy(object):
             pass
         H = Dummy()
         CLI = raw.Context(conf={'EPICS_PVA_BROADCAST_PORT': '0',
@@ -214,14 +214,27 @@
             self.assertIsInstance(Q1.get(timeout=self.timeout), Disconnected)
             self.assertEqual(42, Q1.get(timeout=self.timeout))
 
             with self._ds_client.monitor('pv:rw', Q2.put, notify_disconnect=True):
                 self.assertIsInstance(Q2.get(timeout=self.timeout), Disconnected)
                 self.assertEqual(42, Q2.get(timeout=self.timeout))
 
+                # check stats now that we have an active connection
+                S = self.gw.report(1.0)
+                self.assertEqual(len(S), 1, S)
+                self.assertEqual(S[0][0], "pv:name")
+
+                S = _gw.Server_report(self._ds_server._S, 1.0)
+                self.assertEqual(len(S), 2, S)
+                self.assertEqual(S[0][0], "pv:name")
+                self.assertEqual(S[1][0], "pv:name")
+                # TODO: is order stable?
+                self.assertEqual(S[0][1], "pv:ro")
+                self.assertEqual(S[1][1], "pv:rw")
+
                 # no activity on first subscription
                 with self.assertRaises(Empty):
                     Q2.get(timeout=0.01)
 
 class TestApp(App):
     def __init__(self, args):
         super(TestApp, self).__init__(args)
@@ -353,25 +366,25 @@
 
     def test_get_mask(self):
         val = self._ds_client.get('pv:name', timeout=self.timeout, request='timeStamp')
         self.assertEqual(val, 0) # not requested at default
         self.assertFalse(val.raw.changed('value'))
 
     def test_get_bad_mask(self):
-        with self.assertRaisesRegexp(RemoteError, ".*Empty field selection"):
+        with self.assertRaisesRegex(RemoteError, ".*Empty field selection"):
             val = self._ds_client.get('pv:name', timeout=self.timeout, request='nonexistant')
 
     def test_put(self):
         self._ds_client.put('pv:name', 41, timeout=self.timeout)
 
         val = self._ds_client.get('pv:name', timeout=self.timeout)
         self.assertEqual(val, 41)
 
     def test_put_bad_mask(self):
-        with self.assertRaisesRegexp(RemoteError, ".*Empty field selection"):
+        with self.assertRaisesRegex(RemoteError, ".*Empty field selection"):
             self._ds_client.put('pv:name', 41, request='nonexistant', timeout=self.timeout)
 
     def test_mon(self):
         """Setup a monitor through the GW
         """
         Q = Queue(maxsize=4)
         with self._ds_client.monitor('pv:name', Q.put, notify_disconnect=True):
```

### Comparing `p4p-4.1.8a2/src/p4p/test/test_nt.py` & `p4p-4.1.8a3/src/p4p/test/test_nt.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/test/test_rpc.py` & `p4p-4.1.8a3/src/p4p/test/test_rpc.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/test/test_server.py` & `p4p-4.1.8a3/src/p4p/test/test_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,13 +95,13 @@
             self.assertIsNone(p())
         finally:
             removeProvider("foo")
 
 class TestServerConf(RefTestCase):
     def test_bad_iface(self):
         P = StaticProvider('x')
-        with self.assertRaisesRegexp(RuntimeError, "invalid"):
+        with self.assertRaisesRegex(RuntimeError, "invalid"):
             S = Server(providers=[P], useenv=False, conf={
                 'EPICS_PVAS_INTF_ADDR_LIST':'invalid.host.name.',
                 'EPICS_PVAS_BROADCAST_PORT':'0',
                 'EPICS_PVAS_SERVER_PORT':'0',
             })
```

### Comparing `p4p-4.1.8a2/src/p4p/test/test_sharedpv.py` & `p4p-4.1.8a3/src/p4p/test/test_sharedpv.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         with Server(providers=[self.provider], isolate=True) as S:
             with Context('pva', conf=S.conf(), useenv=False) as C:
 
                 args = NTURI([
                     ('oops', '?'),
                 ])
 
-                with self.assertRaisesRegexp(RemoteError, 'oops'):
+                with self.assertRaisesRegex(RemoteError, 'oops'):
                     ret = C.rpc('foo', args.wrap('foo', kws={'oops':True}))
 
 class TestRPC2(TestRPC):
     openclose = True
 
 class TestPVRequestMask(RefTestCase):
     maxDiff = 1000
```

### Comparing `p4p-4.1.8a2/src/p4p/test/test_type.py` & `p4p-4.1.8a3/src/p4p/test/test_type.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/test/test_value.py` & `p4p-4.1.8a3/src/p4p/test/test_value.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/test/utils.py` & `p4p-4.1.8a3/src/p4p/test/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 from .. import listRefs
 from .._p4p import _forceLazy
 
 _log = logging.getLogger(__name__)
 
 _forceLazy()
 
+if not hasattr(unittest.TestCase, 'assertRegex'):
+    unittest.TestCase.assertRegex = unittest.TestCase.assertRegexpMatches
+
+if not hasattr(unittest.TestCase, 'assertRaisesRegex'):
+    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
+
 class RefTestMixin(object):
 
     """Ensure that each test does not result in a net change in extension object counts
     """
     # set to list of names to compare.  Set to None to disable
     ref_check = ('*',)
```

### Comparing `p4p-4.1.8a2/src/p4p/util.py` & `p4p-4.1.8a3/src/p4p/util.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p/version.py` & `p4p-4.1.8a3/src/p4p/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,8 +63,8 @@
     def __eq__(self, o):
         return self._cmp(o)==0
     def __ge__(self, o):
         return self._cmp(o)>=0
     def __gt__(self, o):
         return self._cmp(o)>0
 
-version = Version('4.1.8a2')
+version = Version('4.1.8a3')
```

### Comparing `p4p-4.1.8a2/src/p4p/wrapper.py` & `p4p-4.1.8a3/src/p4p/wrapper.py`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p.egg-info/PKG-INFO` & `p4p-4.1.8a3/src/p4p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p4p
-Version: 4.1.8a2
+Version: 4.1.8a3
 Summary: Python interface to PVAccess protocol client
 Home-page: https://mdavidsaver.github.io/p4p
 Author: Michael Davidsaver
 Author-email: mdavidsaver@gmail.com
 License: BSD
 Keywords: epics scada
 Platform: UNKNOWN
```

### Comparing `p4p-4.1.8a2/src/p4p.egg-info/SOURCES.txt` & `p4p-4.1.8a3/src/p4p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/p4p.h` & `p4p-4.1.8a3/src/p4p.h`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/pvxs_client.cpp` & `p4p-4.1.8a3/src/pvxs_client.cpp`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/pvxs_gw.cpp` & `p4p-4.1.8a3/src/pvxs_gw.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -101,27 +101,35 @@
                .onConnect([this](){
                     log_debug_printf(_log, "%p upstream connect '%s'\n", &this->src, this->usname.c_str());
                 })
                .onDisconnect([this]()
                 {
                     // on client worker
                     log_debug_printf(_log, "%p upstream disconnect '%s'\n", &this->src, this->usname.c_str());
-                    Guard G(dschans_lock);
-                    for(auto& chan : dschans) {
+                    decltype (dschans) chans;
+                    {
+                        Guard G(dschans_lock);
+                        chans = dschans; // copy...
+                    }
+                    for(auto& chan : chans) {
                         chan->close();
                     }
                 })
                .exec())
 {}
 
 GWUpstream::~GWUpstream()
 {
     log_debug_printf(_log, "upstream shutdown %s\n", usname.c_str());
-    Guard G(dschans_lock);
-    for(auto& chan : dschans) {
+    decltype (dschans) chans;
+    {
+        Guard G(dschans_lock);
+        chans = std::move(dschans);
+    }
+    for(auto& chan : chans) {
         chan->close();
     }
 }
 
 GWChan::GWChan(const std::string& usname,
                const std::string& dsname,
                const std::shared_ptr<GWUpstream>& upstream,
@@ -216,17 +224,17 @@
 
 static
 void onGetCached(const std::shared_ptr<GWChan>& pv, const std::shared_ptr<server::ConnectOp>& ctrl)
 {
     // on server worker
     // 1. downstream creating GET operation, maybe with holdoff
 
-    auto us(pv->us);
+    const auto& us(pv->us);
 
-    Guard G(us->lock);
+    // getop and get->upstream are only used within this function (and thread)
     auto get(us->getop.lock());
     auto cliop(get ? get->upstream.lock() : nullptr);
 
     if(!get || !cliop) {
         us->getop = get = std::make_shared<GWGet>();
         get->upstream = cliop = us->upstream.get(us->usname)
                 .autoExec(false)
@@ -286,23 +294,34 @@
                             setup->error(e.what());
                         }
                     }
                 })
                 .exec();
     }
 
-    switch(get->state) {
+    decltype (get->state) state;
+    Value prototype;
+    {
+        Guard G(us->lock);
+        state = get->state;
+        prototype = get->prototype;
+        if(state==GWGet::Connecting) {
+            log_debug_printf(_logget, "'%s' GET init conn\n", ctrl->name().c_str());
+            get->setups.push_back(ctrl);
+        }
+    }
+
+    switch(state) {
     case GWGet::Connecting:
-        log_debug_printf(_logget, "'%s' GET init conn\n", ctrl->name().c_str());
-        get->setups.push_back(ctrl);
+        // handled above under lock
         break;
     case GWGet::Idle:
     case GWGet::Exec:
         log_debug_printf(_logget, "'%s' GET init typed\n", ctrl->name().c_str());
-        ctrl->connect(get->prototype);
+        ctrl->connect(prototype);
         break;
     case GWGet::Error:
         ctrl->error(get->error);
         return;
     }
 
     ctrl->onGet([get, us, cliop](std::unique_ptr<server::ExecOp>&& sop){
@@ -554,45 +573,47 @@
         ctrl->error(SB()<<"p4p.gw unsupported operation "<<ctrl->op());
     }
 }
 
 static
 void onSubEvent(const std::shared_ptr<GWSubscription>& sub, const std::shared_ptr<GWChan>& pv)
 {
-    // on workQworker
+    auto& us(pv->us);
+
+    // on client worker or workQ worker
     auto cli(sub->upstream.lock());
     if(!cli)
         return;
 
     log_debug_printf(_logmon, "'%s' MONITOR wakeup\n", cli->name().c_str());
 
     for(unsigned i=0; i<4u; i++) {
         try {
             auto val(cli->pop());
             if(!val)
                 return; // queue emptied
 
             log_debug_printf(_logmon, "'%s' MONITOR event\n", cli->name().c_str());
 
-            Guard G(pv->us->lock);
+            Guard G(us->lock);
             sub->current.assign(val); // accumulate deltas
             sub->state = GWSubscription::Running;
 
             for(auto& ctrl : sub->controls)
-                ctrl->post(val);
+                ctrl->post(val); // dispatch() under lock is safe
 
          } catch(client::Finished&) {
             log_debug_printf(_logmon, "'%s' MONITOR finish\n", cli->name().c_str());
 
-            decltype (pv->us->subscription) trash;
+            decltype (us->subscription) trash;
             decltype (sub->setups) setups;
             decltype (sub->controls) controls;
             {
-                Guard G(pv->us->lock);
-                trash = std::move(pv->us->subscription);
+                Guard G(us->lock);
+                trash = std::move(us->subscription);
                 setups = std::move(sub->setups);
                 controls = std::move(sub->controls);
             }
             for(auto& ctrl : setups)
                 ctrl->error("Shared monitor finished before starting");
             for(auto& ctrl : controls)
                 ctrl->finish();
@@ -602,15 +623,15 @@
                             cli->name().c_str(), e.what());
          }
     }
 
     log_debug_printf(_logmon, "'%s' MONITOR resched\n", cli->name().c_str());
 
     // queue not empty, reschedule for later to give other subscriptions a chance
-    pv->us->workQ->push([sub, pv](){ onSubEvent(sub, pv); });
+    us->workQ->push([sub, pv](){ onSubEvent(sub, pv); });
 }
 
 void GWChan::onSubscribe(const std::shared_ptr<GWChan>& pv, std::unique_ptr<server::MonitorSetupOp>&& sop)
 {
     // on server worker
 
     std::shared_ptr<server::MonitorSetupOp> op(std::move(sop));
@@ -620,120 +641,138 @@
     pvReq["record._options.cache"].as(docache);
 
     if(!docache && !pv->allow_uncached) {
         op->error("Gateway disallows uncachable monitor");
         return;
     }
 
-    Guard G(pv->us->lock);
+    std::shared_ptr<GWSubscription> sub;
+    std::shared_ptr<client::Subscription> cli;
+    if(docache) {
+        // check for subscription to re-use
+        Guard G(pv->us->lock);
 
-    auto sub(pv->us->subscription.lock());
-    auto cli(sub ? sub->upstream.lock() : nullptr);
-    if(sub && cli) {
-        // re-use
-        switch(sub->state) {
-        case GWSubscription::Connecting:
-            log_debug_printf(_logmon, "'%s' MONITOR init conn\n", op->name().c_str());
-            sub->setups.push_back(op);
-            goto done;
-
-        case GWSubscription::Connected:
-        case GWSubscription::Running: {
-            log_debug_printf(_logmon, "'%s' MONITOR init run\n", op->name().c_str());
-            auto ctrl(op->connect(sub->current));
-            if(sub->state == GWSubscription::Running)
-                ctrl->post(sub->current); // post current as initial for new subscriber
-            sub->controls.emplace_back(std::move(ctrl));
-            goto done;
-        }
-
-        case GWSubscription::Error:
-            break;
+        sub = pv->us->subscription.lock();
+        if(sub) {
+            cli = sub->upstream.lock();
         }
     }
 
-    log_debug_printf(_logmon, "'%s' MONITOR new\n", op->name().c_str());
+    const bool create = !sub || !cli;
+    if(create) {
+        log_debug_printf(_logmon, "'%s' MONITOR new\n", op->name().c_str());
+
+        // start new subscription
+        sub = std::make_shared<GWSubscription>();
 
-    // start new subscription
-    sub = std::make_shared<GWSubscription>();
-    sub->setups.push_back(op);
-    {
         auto req = pv->us->upstream.monitor(pv->us->usname)
                 .syncCancel(false)
                 .maskConnected(true) // upstream should already be connected
                 .maskDisconnected(true); // handled by the client Connect op
 
         if(!docache)
             req.rawRequest(op->pvRequest()); // when not cached, pass through upstream client request verbatim.
 
-        sub->upstream = cli = req
-                .event([sub, pv](client::Subscription& cli)
-        {
-            // on client worker
+        cli = req.event([sub, pv](client::Subscription& cli)
+                {
+                    // on client worker
 
-            // only invoked if there is an early error.
-            // replaced below for starting
+                    // only invoked if there is an early error.
+                    // replaced below for starting
 
-            try {
-                cli.pop(); // expected to throw
-                throw std::runtime_error("not error??");
-            }catch(std::exception& e){
-                log_warn_printf(_logmon, "'%s' MONITOR setup error: %s\n", cli.name().c_str(), e.what());
+                    try {
+                        cli.pop(); // expected to throw
+                        throw std::runtime_error("not error??");
+                    }catch(std::exception& e){
+                        log_warn_printf(_logmon, "'%s' MONITOR setup error: %s\n", cli.name().c_str(), e.what());
 
-                decltype (pv->us->subscription) trash;
-                decltype (sub->setups) setups;
+                        decltype (pv->us->subscription) trash;
+                        decltype (sub->setups) setups;
+                        {
+                            Guard G(pv->us->lock);
+                            trash = std::move(pv->us->subscription);
+                            setups = std::move(sub->setups);
+                        }
+                        for(auto& op : setups)
+                            op->error(e.what());
+                    }
+                })
+                        .onInit([sub, pv](client::Subscription& cli, const Value& prototype)
                 {
-                    Guard G(pv->us->lock);
-                    trash = std::move(pv->us->subscription);
-                    setups = std::move(sub->setups);
-                }
-                for(auto& op : setups)
-                    op->error(e.what());
-            }
-        })
-                .onInit([sub, pv](client::Subscription& cli, const Value& prototype)
-        {
-            // on client worker
+                    // on client worker
 
-            log_debug_printf(_logmon, "'%s' MONITOR typed\n", cli.name().c_str());
+                    log_debug_printf(_logmon, "'%s' MONITOR typed\n", cli.name().c_str());
 
-            //auto clisub(cli.shared_from_this());
+                    //auto clisub(cli.shared_from_this());
 
-            cli.onEvent([sub, pv](client::Subscription& cli) { // replace earlier .event(...)
-                // on client worker
+                    cli.onEvent([sub, pv](client::Subscription& cli) { // replace earlier .event(...)
+                        // on client worker
 
-                log_debug_printf(_logmon, "'%s' MONITOR wakeup\n", cli.name().c_str());
+                        log_debug_printf(_logmon, "'%s' MONITOR wakeup\n", cli.name().c_str());
 
-                pv->us->workQ->push([sub, pv]() { onSubEvent(sub, pv); });
-            });
+                        pv->us->workQ->push([sub, pv]() { onSubEvent(sub, pv); });
+                    });
 
-            // syncs client worker with server worker
-            {
-                Guard G(pv->us->lock);
-                sub->state = GWSubscription::Connected;
-                sub->current = prototype.clone();
-                auto setups(std::move(sub->setups));
-                for(auto& setup : setups) {
-                    sub->controls.push_back(setup->connect(sub->current));
-                }
-            }
-        })
-                .exec();
+                    decltype (sub->setups) setups;
+                    decltype (sub->controls) controls;
+                    {
+                        Guard G(pv->us->lock);
+                        sub->state = GWSubscription::Connected;
+                        sub->current = prototype.clone();
+                        setups = std::move(sub->setups);
+                    }
+                    // unlock to call() into server worker.
+                    // since we are on the client worker, no further client events are delivered.
+                    // however, server events may.  So controls[] may not be empty after re-lock
+                    for(auto& setup : setups) {
+                        controls.push_back(setup->connect(sub->current));
+                    }
+                    {
+                        Guard G(pv->us->lock);
+                        for(auto&& ctrl : controls)
+                            sub->controls.push_back(std::move(ctrl));
+                    }
+                })
+                        .exec();
     }
 
-    if(docache)
-        pv->us->subscription = sub;
-
-    // BUG: need to unlock before onClose()
-done:
     // tie client subscription lifetime (and by extension GWSubscription) to server op.
     // Reference to CLI stored in internal server OP struct, so no ref. loop
     op->onClose([cli](const std::string&) {
         log_debug_printf(_log, "sub close '%s'\n", cli->name().c_str());
     });
+
+    {
+        Guard G(pv->us->lock);
+
+        if(create) {
+            sub->upstream = cli;
+
+            if(docache)
+                pv->us->subscription = sub;
+        }
+
+        switch(sub->state) {
+        case GWSubscription::Connecting:
+            log_debug_printf(_logmon, "'%s' MONITOR init conn\n", op->name().c_str());
+            sub->setups.push_back(op);
+            break;
+
+        case GWSubscription::Connected:
+        case GWSubscription::Running: {
+            log_debug_printf(_logmon, "'%s' MONITOR init run\n", op->name().c_str());
+            // post()ing to server worker from server worker will recurse instead of blocking.
+            auto ctrl(op->connect(sub->current));
+            if(sub->state == GWSubscription::Running)
+                ctrl->post(sub->current); // post current as initial for new subscriber
+            sub->controls.emplace_back(std::move(ctrl));
+            break;
+        }
+        }
+    }
 }
 
 void GWSource::onCreate(std::unique_ptr<server::ChannelControl> &&op)
 {
     // on server worker
 
     // Server worker may make synchronous calls to client worker.
@@ -782,35 +821,40 @@
     }); // onSubscribe
 
     log_debug_printf(_log, "%p onCreate '%s' as '%s' success\n", this, pv->dsname.c_str(), pv->us->usname.c_str());
 }
 
 GWSearchResult GWSource::test(const std::string &usname)
 {
+    std::shared_ptr<GWUpstream> newchan; // if !pair.second, must unlock before dtor of discarded chan
     Guard G(mutex);
 
     auto it(channels.find(usname));
+    bool miss = it==channels.end();
 
     log_debug_printf(_log, "%p '%s' channel cache %s\n", this, usname.c_str(),
-                     (it==channels.end()) ? "miss" : "hit");
-    if(it==channels.end()) {
-
-        auto chan(std::make_shared<GWUpstream>(usname, *this));
+                     miss ? "miss" : "hit");
+    if(miss) {
+        {
+            UnGuard U(G);
+            newchan = std::make_shared<GWUpstream>(usname, *this);
+        }
 
-        auto pair = channels.insert(std::make_pair(usname, chan));
-        assert(pair.second); // we already checked
+        auto pair = channels.emplace(usname, newchan);
+        // pair.second true if actually inserted, false if collision.
+        // in either case, use what is in the channels map.
         it = pair.first;
 
         log_debug_printf(_log, "%p new upstream channel '%s'\n", this, usname.c_str());
     }
 
     if(it->second->gcmark) {
         log_debug_printf(_log, "%p unmark '%s'\n", this, usname.c_str());
+        it->second->gcmark = false;
     }
-    it->second->gcmark = false;
     auto usconn = it->second->connector->connected();
 
     log_debug_printf(_log, "%p test '%s' -> %c\n", this, usname.c_str(), usconn ? '!' : '_');
 
     return usconn ? GWSearchClaim : GWSearchIgnore;
 }
 
@@ -833,40 +877,43 @@
     log_debug_printf(_log, "%p connect '%s' as '%s' -> %c\n", this, usname.c_str(), dsname.c_str(), ret ? '!' : '_');
 
     return ret;
 }
 
 void GWSource::sweep()
 {
+    // py worker thread
     log_debug_printf(_log, "%p sweeps\n", this);
 
     std::vector<std::shared_ptr<GWUpstream>> trash;
     // garbage disposal after unlock
-    Guard G(mutex);
 
     {
+        Guard G(mutex);
         auto it(channels.begin()), end(channels.end());
         while(it!=end) {
             auto cur(it++);
 
             if(cur->second.use_count() > 1u) {
                 // no-op
 
             } else if(!cur->second->gcmark) {
                 log_debug_printf(_log, "%p marked '%s'\n", this, cur->first.c_str());
                 cur->second->gcmark = true;
 
             } else { // one for GWSource::channels map
                 log_debug_printf(_log, "%p swept '%s'\n", this, cur->first.c_str());
                 trash.emplace_back(std::move(cur->second));
-                upstream.cacheClear(cur->first);
                 channels.erase(cur);
             }
         }
     }
+
+    for(auto& tr : trash)
+        upstream.cacheClear(tr->usname);
 }
 
 void GWSource::disconnect(const std::string& usname) {}
 void GWSource::forceBan(const std::string& host, const std::string& usname) {}
 void GWSource::clearBan() {}
 
 void GWSource::cachePeek(std::set<std::string> &names) const {}
```

### Comparing `p4p-4.1.8a2/src/pvxs_gw.h` & `p4p-4.1.8a3/src/pvxs_gw.h`

 * *Files 4% similar despite different names*

```diff
@@ -27,74 +27,76 @@
     GWSearchClaim,
     GWSearchBanHost,
     GWSearchBanPV,
     GWSearchBanHostPV,
 };
 
 struct GWSubscription {
-    //const std::shared_ptr<GWUpstream> chan;
-
     // should only be lock()'d from server worker
     std::weak_ptr<client::Subscription> upstream;
 
     Value current;
 
     enum state_t {
         Connecting, // waiting for onInit()
         Connected,  // waiting for first event
         Running,
-        Error,
     } state = Connecting;
 
     std::vector<std::shared_ptr<server::MonitorSetupOp>> setups;
     std::vector<std::shared_ptr<server::MonitorControlOp>> controls;
 };
 
 struct GWGet {
+    // only access from server worker
     std::weak_ptr<client::Operation> upstream;
 
+    // guarded by GWUpstream::lock
+
     Value prototype;
     epicsTime lastget;
     Timer delay;
     std::string error;
 
-    enum state_t {
-        Connecting, // waiting for onInit()
-        Idle,
-        Exec,
-        Error,
+    enum state_t {  // downstream/server close() at any time...
+        Connecting, // waiting for onInit() from upstream/client
+        Idle,       // waiting for onGet() from downstream/server
+        Exec,       // waiting for reExecGet() from upstream/client
+        Error,      // abnormal completion from upstream/client
     } state = Connecting;
 
     bool firstget = true;
 
     std::vector<std::shared_ptr<server::ConnectOp>> setups;
     std::vector<std::shared_ptr<server::ExecOp>> ops;
 };
 
 struct GWUpstream {
     const std::string usname;
-    client::Context upstream;
+    client::Context upstream; //const after ctor
     GWSource& src;
 
+    const std::shared_ptr<MPMCFIFO<std::function<void()>>> workQ;
+
+    // only access from server worker
+    std::weak_ptr<GWGet> getop;
+
     mutable epicsMutex dschans_lock;
     std::set<std::shared_ptr<server::ChannelControl>> dschans;
 
-    // time in msec
-    std::atomic<unsigned> get_holdoff{};
-
     epicsMutex lock;
 
     std::weak_ptr<GWSubscription> subscription;
 
-    std::weak_ptr<GWGet> getop;
-
     bool gcmark = false;
 
-    const std::shared_ptr<MPMCFIFO<std::function<void()>>> workQ;
+    // time in msec
+    std::atomic<unsigned> get_holdoff{};
 
+    // must be last (cf. ctor body)
     const std::shared_ptr<client::Connect> connector;
 
     explicit GWUpstream(const std::string& usname, GWSource &src);
     ~GWUpstream();
 };
 
 struct GWChanInfo : public server::ReportInfo {
```

### Comparing `p4p-4.1.8a2/src/pvxs_odometer.cpp` & `p4p-4.1.8a3/src/pvxs_odometer.cpp`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/pvxs_sharedpv.cpp` & `p4p-4.1.8a3/src/pvxs_sharedpv.cpp`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/pvxs_source.cpp` & `p4p-4.1.8a3/src/pvxs_source.cpp`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/pvxs_type.cpp` & `p4p-4.1.8a3/src/pvxs_type.cpp`

 * *Files identical despite different names*

### Comparing `p4p-4.1.8a2/src/pvxs_value.cpp` & `p4p-4.1.8a3/src/pvxs_value.cpp`

 * *Files identical despite different names*

