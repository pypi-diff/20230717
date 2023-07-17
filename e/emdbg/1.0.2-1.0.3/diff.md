# Comparing `tmp/emdbg-1.0.2.tar.gz` & `tmp/emdbg-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emdbg-1.0.2.tar", last modified: Thu Jul 13 14:17:56 2023, max compression
+gzip compressed data, was "emdbg-1.0.3.tar", last modified: Mon Jul 17 13:11:17 2023, max compression
```

## Comparing `emdbg-1.0.2.tar` & `emdbg-1.0.3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.509517 emdbg-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-13 14:17:38.000000 emdbg-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-13 14:17:56.509517 emdbg-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-07-13 14:17:38.000000 emdbg-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-13 14:17:38.000000 emdbg-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:17:56.509517 emdbg-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.489516 emdbg-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.489516 emdbg-1.0.2/src/emdbg/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.493516 emdbg-1.0.2/src/emdbg/analyze/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/analyze/backtrace.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/analyze/callgraph.md
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/analyze/callgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/analyze/calltrace.md
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/analyze/calltrace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/analyze/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/analyze/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.493516 emdbg-1.0.2/src/emdbg/bench/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.501516 emdbg-1.0.2/src/emdbg/bench/data/
--rw-r--r--   0 runner    (1001) docker     (123)  2501281 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/data/STM32F7x5.svd
--rw-r--r--   0 runner    (1001) docker     (123)  4087801 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/data/STM32H753x.svd
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/data/fmu.gdb
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/data/fmu_v5x.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/data/fmu_v6x.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/data/fmu_v6x.jlinkscript
--rw-r--r--   0 runner    (1001) docker     (123)    28207 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/data/orbuculum.gdb
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/fmu.md
--rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/fmu.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/skynode.md
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/bench/skynode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.505517 emdbg-1.0.2/src/emdbg/debug/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/crashdebug.md
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/crashdebug.py
--rw-r--r--   0 runner    (1001) docker     (123)    31384 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/gdb.md
--rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/gdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/jlink.md
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/jlink.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/openocd.md
--rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/openocd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.505517 emdbg-1.0.2/src/emdbg/debug/px4/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/pinout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/semaphore.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/system_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    13751 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/px4/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.505517 emdbg-1.0.2/src/emdbg/debug/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/remote/gdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/remote/gdb_api_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/remote/mi.py
--rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/remote/px4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/remote/rpyc.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/debug/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.505517 emdbg-1.0.2/src/emdbg/io/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/io/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/io/digilent.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.505517 emdbg-1.0.2/src/emdbg/patch/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.509517 emdbg-1.0.2/src/emdbg/patch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/data/disable_uavcan_v5x.patch
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/data/itm.h
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/data/itm_Make.defs
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/data/itm_nuttx_Makefile.patch
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/data/nuttx_tracing_itm.patch
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/data/sem_boostlog.c
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/data/semaphore_boostlog.h
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/data/semaphore_boostlog.patch
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/patch/set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.509517 emdbg-1.0.2/src/emdbg/power/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/power/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/power/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/power/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/power/yocto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.509517 emdbg-1.0.2/src/emdbg/serial/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/serial/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/serial/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/serial/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-13 14:17:38.000000 emdbg-1.0.2/src/emdbg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:17:56.493516 emdbg-1.0.2/src/emdbg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-13 14:17:56.000000 emdbg-1.0.2/src/emdbg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-13 14:17:56.000000 emdbg-1.0.2/src/emdbg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:17:56.000000 emdbg-1.0.2/src/emdbg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:17:56.000000 emdbg-1.0.2/src/emdbg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-13 14:17:56.000000 emdbg-1.0.2/src/emdbg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 14:17:56.000000 emdbg-1.0.2/src/emdbg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:11:17.757088 emdbg-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-17 13:10:56.000000 emdbg-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-17 13:11:17.757088 emdbg-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-07-17 13:10:56.000000 emdbg-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-17 13:10:56.000000 emdbg-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:11:17.757088 emdbg-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:11:17.733087 emdbg-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:11:17.733087 emdbg-1.0.3/src/emdbg/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:11:17.737087 emdbg-1.0.3/src/emdbg/analyze/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/analyze/backtrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/analyze/callgraph.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/analyze/callgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/analyze/calltrace.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/analyze/calltrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/analyze/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/analyze/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:11:17.737087 emdbg-1.0.3/src/emdbg/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/bench/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:11:17.749088 emdbg-1.0.3/src/emdbg/bench/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2501281 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/bench/data/STM32F7x5.svd
+-rw-r--r--   0 runner    (1001) docker     (123)  4087801 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/bench/data/STM32H753x.svd
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/bench/data/fmu.gdb
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/bench/data/fmu_v5x.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/bench/data/fmu_v6x.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/bench/data/fmu_v6x.jlinkscript
+-rw-r--r--   0 runner    (1001) docker     (123)    28207 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/bench/data/orbuculum.gdb
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/bench/fmu.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12725 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/bench/fmu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/bench/skynode.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/bench/skynode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:11:17.749088 emdbg-1.0.3/src/emdbg/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/crashdebug.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/crashdebug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31384 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/gdb.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/gdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/jlink.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9480 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/jlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/openocd.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/openocd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:11:17.753088 emdbg-1.0.3/src/emdbg/debug/px4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/px4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/px4/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12824 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/px4/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/px4/pinout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/px4/semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/px4/svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/px4/system_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/px4/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/px4/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:11:17.753088 emdbg-1.0.3/src/emdbg/debug/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/remote/gdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/remote/gdb_api_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/remote/mi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/remote/px4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/remote/rpyc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/debug/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:11:17.753088 emdbg-1.0.3/src/emdbg/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/io/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/io/digilent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:11:17.753088 emdbg-1.0.3/src/emdbg/patch/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/patch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/patch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/patch/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:11:17.757088 emdbg-1.0.3/src/emdbg/patch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/patch/data/disable_uavcan_v5x.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/patch/data/itm.h
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/patch/data/itm_Make.defs
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/patch/data/itm_nuttx_Makefile.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/patch/data/nuttx_tracing_itm.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/patch/data/sem_boostlog.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/patch/data/semaphore_boostlog.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/patch/data/semaphore_boostlog.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/patch/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/patch/set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:11:17.757088 emdbg-1.0.3/src/emdbg/power/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/power/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/power/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/power/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/power/yocto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:11:17.757088 emdbg-1.0.3/src/emdbg/serial/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/serial/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/serial/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/serial/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-17 13:10:56.000000 emdbg-1.0.3/src/emdbg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:11:17.737087 emdbg-1.0.3/src/emdbg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-17 13:11:17.000000 emdbg-1.0.3/src/emdbg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-17 13:11:17.000000 emdbg-1.0.3/src/emdbg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:11:17.000000 emdbg-1.0.3/src/emdbg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:11:17.000000 emdbg-1.0.3/src/emdbg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 13:11:17.000000 emdbg-1.0.3/src/emdbg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 13:11:17.000000 emdbg-1.0.3/src/emdbg.egg-info/top_level.txt
```

### Comparing `emdbg-1.0.2/LICENSE` & `emdbg-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/PKG-INFO` & `emdbg-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: emdbg
-Version: 1.0.2
+Version: 1.0.3
 Summary: Embedded Debug Tools
 Author-email: Auterion <success@auterion.com>
 License: BSD-3-Clause
-Project-URL: Homepage, https://github.com/auterion/embedded-debug-tools
+Project-URL: GitHub, https://github.com/auterion/embedded-debug-tools
+Project-URL: Changelog, https://github.com/auterion/embedded-debug-tools/blob/main/CHANGELOG.md
 Keywords: embedded,debug,gdb,stm32,px4
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Embedded Systems
```

### Comparing `emdbg-1.0.2/README.md` & `emdbg-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/pyproject.toml` & `emdbg-1.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 description = "Embedded Debug Tools"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["embedded", "debug", "gdb", "stm32", "px4"]
 license = {text = "BSD-3-Clause"}
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: Unix",
     "Programming Language :: Python :: 3.8",
     "Topic :: Software Development :: Debuggers",
     "Topic :: Software Development :: Embedded Systems",
@@ -35,15 +35,16 @@
     "pydwf",
     "yoctopuce",
     "rpyc",
 ]
 dynamic = ["version"]
 
 [project.urls]
-"Homepage" = "https://github.com/auterion/embedded-debug-tools"
+"GitHub" = "https://github.com/auterion/embedded-debug-tools"
+"Changelog" = "https://github.com/auterion/embedded-debug-tools/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 all = ["pdoc"]
 # Make our specific hardware drivers optional too?
 # digilent = ["pydwf"]
 # yocto = ["yoctopuce"]
 # rpyc = ["rpyc"]
```

### Comparing `emdbg-1.0.2/src/emdbg/__init__.py` & `emdbg-1.0.3/src/emdbg/__init__.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/analyze/backtrace.py` & `emdbg-1.0.3/src/emdbg/analyze/backtrace.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
+from __future__ import annotations
 import re
 from .priority import _BoostOperation
 
 class Frame:
     """
     Parses a GDB frame of a `backtrace` or `px4_backtrace` command.
     """
@@ -94,69 +95,69 @@
         OPENDIR = r"^opendir$",
         MOUNT = r"^mount$",
         MKDIR = r"^mkdir$",
         STAT = r"^stat$",
         IRQ = r"^stm32_sdmmc_interrupt$",
         INIT = r"^stm32_sdio_initialize$",
     )
-    COLORS = {"^fat_.*$": _fill("LightYellow"),
-              "^mmc?sd_.*$": _fill("LightCyan"),
-              "^stm32_.*$": _fill("DarkSeaGreen"),
-              "px4::logger::": _fill("Gold"),
-              "Navigator": _fill("GreenYellow"),
-              "can": _fill("LightSalmon"),
-              "^nsh_.*": _fill("LightSkyBlue"),
-              "^(param|bson)_.*": _fill("Bisque")} | \
-             {pattern: _bfill("Silver") for pattern in EDGES.values()}
+    COLORS = {**{"^fat_.*$": _fill("LightYellow"),
+                 "^mmc?sd_.*$": _fill("LightCyan"),
+                 "^stm32_.*$": _fill("DarkSeaGreen"),
+                 "px4::logger::": _fill("Gold"),
+                 "Navigator": _fill("GreenYellow"),
+                 "can": _fill("LightSalmon"),
+                 "^nsh_.*": _fill("LightSkyBlue"),
+                 "^(param|bson)_.*": _fill("Bisque")},
+              **{pattern: _bfill("Silver") for pattern in EDGES.values()}}
 
 
 class SpiBacktrace(Backtrace):
     EDGES = dict(
         READ = r"RegisterRead|FIFOReadCount",
         WRITE = r"RegisterWrite",
         PARAM = r"^param_main$",
         NSH = r"^nsh_initialize$",
     )
-    COLORS = {pattern: _bfill("Silver") for pattern in EDGES.values()} | \
-             {"^(ramtron|bch|bchlib)_.*$": _fill("LightYellow"),
-              "^spi_.*$": _fill("LightCyan"),
-              "^stm32_.*$": _fill("DarkSeaGreen"),
-              "ICM20602": _fill("Gold"),
-              "BMI088": _fill("GreenYellow"),
-              "ICM42688": _fill("LightSalmon"),
-              "^nsh_.*": _fill("LightSkyBlue"),
-              "^(param|bson)_.*": _fill("Bisque")}
+    COLORS = {**{pattern: _bfill("Silver") for pattern in EDGES.values()},
+              **{"^(ramtron|bch|bchlib)_.*$": _fill("LightYellow"),
+                 "^spi_.*$": _fill("LightCyan"),
+                 "^stm32_.*$": _fill("DarkSeaGreen"),
+                 "ICM20602": _fill("Gold"),
+                 "BMI088": _fill("GreenYellow"),
+                 "ICM42688": _fill("LightSalmon"),
+                 "^nsh_.*": _fill("LightSkyBlue"),
+                 "^(param|bson)_.*": _fill("Bisque")}}
 
 
 class I2cBacktrace(Backtrace):
     EDGES = dict(
         TRANSFER = r"stm32_i2c_transfer",
         NSH = r"^nsh_initialize$",
         IRQ = r"^stm32_i2c_isr$",
         INIT = r"^stm32_i2c_setclock$",
     )
-    COLORS = {"^stm32_.*$": _fill("DarkSeaGreen"),
-              "BMM150": _fill("Yellow"),
-              "IST8310": _fill("Cyan"),
-              "BMP388": _fill("Gold"),
-              "RGBLED": _fill("LightSkyBlue"),
-              "MCP23009": _fill("LightSalmon")} | \
-             {pattern: _bfill("Silver") for pattern in EDGES.values()}
+    COLORS = {**{"^stm32_.*$": _fill("DarkSeaGreen"),
+                 "BMM150": _fill("Yellow"),
+                 "IST8310": _fill("Cyan"),
+                 "BMP388": _fill("Gold"),
+                 "RGBLED": _fill("LightSkyBlue"),
+                 "MCP23009": _fill("LightSalmon")},
+              **{pattern: _bfill("Silver") for pattern in EDGES.values()}}
 
 
 class CanBacktrace(Backtrace):
     EDGES = dict(
         SEND = r"CanIface::send$",
         RECEIVE = r"CanIface::receive$",
         INIT = r"CanIface::init$",
         FRAME = r"TransferListener::handleFrame$",
     )
-    COLORS = {pattern: _bfill("Silver") for pattern in EDGES.values()} | \
-             {"^(ramtron|bch|bchlib)_.*$": _fill("LightYellow"),
-              "Publisher": _fill("DarkSeaGreen")}
+    COLORS = {**{pattern: _bfill("Silver") for pattern in EDGES.values()},
+              **{"^(ramtron|bch|bchlib)_.*$": _fill("LightYellow"),
+                 "Publisher": _fill("DarkSeaGreen")}}
 
 
 class UartBacktrace(Backtrace):
     EDGES = dict(
         READ = r"^read$",
         WRITE = r"^write$",
         FFLUSH = r"^fflush$",
@@ -164,23 +165,23 @@
         FPUTS = r"^fputs$",
         OPEN = r"^open$",
         SYSLOG = r"^syslog$",
         PRINTF = r"^printf$",
         IRQ = r"^irq_dispatch$",
         INIT = r"^arm_earlyserialinit$",
     )
-    COLORS = {"^I2CSPI": _fill("LightYellow"),
-              "^(up|uart)_.*$": _fill("LightCyan"),
-              "^stm32_.*$": _fill("DarkSeaGreen"),
-              "px4::logger": _fill("Gold"),
-              "[mM]avlink": _fill("GreenYellow"),
-              "can": _fill("LightSalmon"),
-              "^nsh_.*": _fill("LightSkyBlue"),
-              "^(param|bson)_.*": _fill("Bisque")} | \
-             {pattern: _bfill("Silver") for pattern in EDGES.values()}
+    COLORS = {**{"^I2CSPI": _fill("LightYellow"),
+                 "^(up|uart)_.*$": _fill("LightCyan"),
+                 "^stm32_.*$": _fill("DarkSeaGreen"),
+                 "px4::logger": _fill("Gold"),
+                 "[mM]avlink": _fill("GreenYellow"),
+                 "can": _fill("LightSalmon"),
+                 "^nsh_.*": _fill("LightSkyBlue"),
+                 "^(param|bson)_.*": _fill("Bisque")},
+              **{pattern: _bfill("Silver") for pattern in EDGES.values()}}
 
 
 class SemaphoreBacktrace(Backtrace):
     # EDGES = dict(
     #     RESTORE = r"^nxsem_restoreholderprio$",
     #     BOOST =  r"^nxsem_boostholderprio$",
     #     WAIT = r"^nxsem_wait$",
```

### Comparing `emdbg-1.0.2/src/emdbg/analyze/callgraph.md` & `emdbg-1.0.3/src/emdbg/analyze/callgraph.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/analyze/callgraph.py` & `emdbg-1.0.3/src/emdbg/analyze/callgraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
 """
 .. include:: callgraph.md
 """
 
+from __future__ import annotations
 import re, os
 import itertools
 import logging
 from pathlib import Path
 from collections import defaultdict
 from .backtrace import Backtrace
 from .utils import read_gdb_log
```

### Comparing `emdbg-1.0.2/src/emdbg/analyze/calltrace.md` & `emdbg-1.0.3/src/emdbg/analyze/calltrace.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/analyze/calltrace.py` & `emdbg-1.0.3/src/emdbg/analyze/calltrace.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/analyze/priority.py` & `emdbg-1.0.3/src/emdbg/analyze/priority.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 You can also generate a callgraph with boost operations:
 
 ```sh
 python3 -m emdbg.analyze.callgraph log_semaphore_boosts.txt --svg --type Semaphore
 ```
 """
 
+from __future__ import annotations
 import re
 from pathlib import Path
 import statistics
 import itertools
 from collections import defaultdict
 from ..debug.px4.utils import format_table
 from .utils import read_gdb_log
```

### Comparing `emdbg-1.0.2/src/emdbg/bench/data/STM32F7x5.svd` & `emdbg-1.0.3/src/emdbg/bench/data/STM32F7x5.svd`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/bench/data/STM32H753x.svd` & `emdbg-1.0.3/src/emdbg/bench/data/STM32H753x.svd`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/bench/data/fmu.gdb` & `emdbg-1.0.3/src/emdbg/bench/data/fmu.gdb`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/bench/data/fmu_v6x.jlinkscript` & `emdbg-1.0.3/src/emdbg/bench/data/fmu_v6x.jlinkscript`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/bench/data/orbuculum.gdb` & `emdbg-1.0.3/src/emdbg/bench/data/orbuculum.gdb`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/bench/fmu.md` & `emdbg-1.0.3/src/emdbg/bench/fmu.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/bench/fmu.py` & `emdbg-1.0.3/src/emdbg/bench/fmu.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
 """
 .. include:: fmu.md
 """
 
+from __future__ import annotations
 import time
 from pathlib import Path
 from contextlib import contextmanager, nullcontext
 import emdbg
 
 
 class Fmu:
     """
     FMU test bench with optional nsh, power, and logic analyzer attachements.
     """
-    DBGMCU_CONFIG = [
+    _DBGMCU_CONFIG = [
         "set *0xE0042008 = 0xffffffff",
         "set *0xE004200C = 0xffffffff"
     ]
-    MCU_MEMORIES = [
+    _MCU_MEMORIES = [
         (0x20000000, 0x00080000), # SRAM1-3
         (0x40010424, 4), # HRT uptime
     ]
 
     def __init__(self, elf: Path,
                  gdb: "emdbg.debug.remote.gdb.Interface",
                  nsh: "emdbg.serial.protocol.Nsh" = None,
                  power: "emdbg.power.base.Base" = None,
                  io: "emdbg.io.digilent.Digilent" = None):
-        self.elf = elf
-        self.gdb = gdb
+        self.elf: Path = elf
+        """The ELF file under debug"""
+        self.gdb: "emdbg.debug.remote.gdb.Interface" = gdb
         """The remote GDB access interface object"""
-        self.nsh = nsh
+        self.nsh: "emdbg.serial.protocol.Nsh" = nsh
         """The NSH protocol controller"""
-        self.power = power
+        self.power: "emdbg.power.base.Base" = power
         """The power relay controlling the FMU"""
-        self.io = io
+        self.io: "emdbg.io.digilent.Digilent" = io
         """The Digilent Scope"""
 
     def _init(self):
         self.gdb.interrupt_and_wait()
-        for cmd in self.DBGMCU_CONFIG:
+        for cmd in self._DBGMCU_CONFIG:
             self.gdb.execute(cmd)
         self.restart_system_load_monitor()
 
     def _deinit(self):
         self.gdb.interrupt_and_wait()
         self.gdb.execute("disconnect")
         self.gdb.interrupted = False
@@ -56,29 +58,29 @@
         """See `emdbg.debug.px4.system_load.restart_system_load_monitor`"""
         with self.gdb.interrupt_continue():
             if self.gdb.type == "mi":
                 self.gdb.execute("python px4.restart_system_load_monitor(gdb)")
             else:
                 emdbg.debug.px4.restart_system_load_monitor(self.gdb)
 
-    def coredump(self, filename: str = None):
+    def coredump(self, filename: Path = None):
         """
         Dumps the FMU core for later analysis with CrashDebug (see
         `emdbg.debug.crashdebug`).
 
         :param filename: Default `coredump_{datetime}.txt`.
         """
         with self.gdb.interrupt_continue():
             if False:
                 # Connection is remote, therefore we must use slower RPyC interface
-                emdbg.debug.px4.coredump(self.gdb, self.MCU_MEMORIES, filename)
+                emdbg.debug.px4.coredump(self.gdb, self._MCU_MEMORIES, filename)
             else:
                 # Executing directly on the GDB process is *significantly* faster!
                 if filename: filename = f"--file '{filename}'"
-                memories = [f"--memory {m[0]}:{m[1]}" for m in self.MCU_MEMORIES]
+                memories = [f"--memory {m[0]}:{m[1]}" for m in self._MCU_MEMORIES]
                 self.gdb.execute(f"px4_coredump {' '.join(memories)} {filename or ''}")
 
     def upload(self, source: Path = None):
         """
         Uploads the ELF file to the FMU, resets the device, clears the NSH
         :param source: optional path to ELF file, default is the ELF file passed
                        to the constructor.
@@ -131,16 +133,16 @@
         while(seconds > 0):
             seconds -= 1
             time.sleep(1)
             if func is not None:
                 func(seconds)
 
 
-def px4_config(px4_directory: Path, target: Path, commands: list[str] = None,
-               ui: str = None, speed: int = 16000, backend: str = None):
+def _px4_config(px4_directory: Path, target: Path, commands: list[str] = None,
+                ui: str = None, speed: int = 16000, backend: str = None) -> tuple:
     if "fmu-v5x" in target:
         device = "STM32F765II"
         svd = "STM32F7x5.svd"
         config = "fmu_v5x.cfg"
     elif "fmu-v6x" in target:
         device = "STM32H753II"
         svd = "STM32H753x.svd"
@@ -164,15 +166,15 @@
 
     svd = data_dir / svd
     elf = px4_dir / f"build/{target}_default/{target}_default.elf"
     cmds = [f"dir {px4_dir}", f"source {data_dir}/fmu.gdb",
             f"source {data_dir}/orbuculum.gdb",
             f"python px4._TARGET='{target.lower()}'"]
     if ui is not None:
-        cmds += Fmu.DBGMCU_CONFIG + ["python px4.restart_system_load_monitor(gdb)"]
+        cmds += Fmu._DBGMCU_CONFIG + ["python px4.restart_system_load_monitor(gdb)"]
     cmds += (commands or [])
 
     return backend, elf, svd, cmds
 
 
 # -----------------------------------------------------------------------------
 @contextmanager
@@ -202,20 +204,20 @@
     :param ui: If not `None`, then this launches the interactive debugger via
                `emdbg.debug.gdb.call` instead of the scripting API.
     :param commands: list of additional GDB commands to execute during launch.
     :param with_rpyc: Use the RPyC GDB interface implementation, rather than the
                       GDB/MI interface. See `emdbg.debug.remote`.
     :param keep_power_on: Do not shut off the Fmu after the context has closed.
     :param upload: Automatically upload the firmware after powering on the FMU.
-    :param backend: "openocd", "jlink", or "IP:PORT" for a GDB server on another machine.
+    :param backend: `openocd`, `jlink`, or `IP:PORT` for a GDB server on another machine.
 
     :return: A configured test bench with the latest firmware.
     """
-    backend, elf, svd, cmds = px4_config(px4_directory, target, commands, ui,
-                                         backend=backend or "openocd")
+    backend, elf, svd, cmds = _px4_config(px4_directory, target, commands, ui,
+                                          backend=backend or "openocd")
 
     with (nullcontext() if power is None else power) as pwr:
         try:
             if ui is not None:
                 # Manual mode that only connects the debugger (blocking)
                 if power: pwr.on()
                 yield emdbg.debug.gdb.call(backend, elf, commands=cmds, ui=ui, svd=svd)
```

### Comparing `emdbg-1.0.2/src/emdbg/bench/skynode.md` & `emdbg-1.0.3/src/emdbg/bench/skynode.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/bench/skynode.py` & `emdbg-1.0.3/src/emdbg/bench/skynode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
 """
 .. include:: skynode.md
 """
 
+from __future__ import annotations
 import time
 from pathlib import Path
 from .fmu import debug as fmu_debug, Fmu
 
 import emdbg
 
 class Skynode(Fmu):
```

### Comparing `emdbg-1.0.2/src/emdbg/debug/__init__.py` & `emdbg-1.0.3/src/emdbg/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/debug/backend.py` & `emdbg-1.0.3/src/emdbg/debug/backend.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) 2020-2022, Niklas Hauser
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
+from __future__ import annotations
 from pathlib import Path
 from contextlib import contextmanager
 
 
 class ProbeBackend:
     """
     Base class for starting and stopping debug probes and attaching GDB to them.
```

### Comparing `emdbg-1.0.2/src/emdbg/debug/crashdebug.md` & `emdbg-1.0.3/src/emdbg/debug/crashdebug.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/debug/crashdebug.py` & `emdbg-1.0.3/src/emdbg/debug/crashdebug.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
 """
 .. include:: crashdebug.md
 """
 
+from __future__ import annotations
 import os, platform
 from pathlib import Path
 from .backend import ProbeBackend
 
 class CrashProbeBackend(ProbeBackend):
     """
     CrashDebug specific debug backend implementation. Note that this
```

### Comparing `emdbg-1.0.2/src/emdbg/debug/gdb.md` & `emdbg-1.0.3/src/emdbg/debug/gdb.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/debug/gdb.py` & `emdbg-1.0.3/src/emdbg/debug/gdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """
 .. include:: gdb.md
 
 ## Python API
 """
 
-
+from __future__ import annotations
 import os
 import sys
 import subprocess
 import signal
 import tempfile
 import shlex
 import time
```

### Comparing `emdbg-1.0.2/src/emdbg/debug/jlink.md` & `emdbg-1.0.3/src/emdbg/debug/jlink.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/debug/jlink.py` & `emdbg-1.0.3/src/emdbg/debug/jlink.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
 """
 .. include:: jlink.md
 """
 
+from __future__ import annotations
 import os
 import time
 import signal
 import platform
 import subprocess
 import logging
 import tempfile
```

### Comparing `emdbg-1.0.2/src/emdbg/debug/openocd.md` & `emdbg-1.0.3/src/emdbg/debug/openocd.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/debug/openocd.py` & `emdbg-1.0.3/src/emdbg/debug/openocd.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
 """
 .. include:: openocd.md
 """
 
+from __future__ import annotations
 import os
 import time
 import signal
 import logging
 import tempfile
 import platform
 import telnetlib
```

### Comparing `emdbg-1.0.2/src/emdbg/debug/px4/__init__.py` & `emdbg-1.0.3/src/emdbg/debug/px4/__init__.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/debug/px4/base.py` & `emdbg-1.0.3/src/emdbg/debug/px4/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
+from __future__ import annotations
 import re
 from . import utils
 from functools import cached_property
 
 class Base:
     """
     This base class provides basic abstractions to simplify usage of the GDB
```

### Comparing `emdbg-1.0.2/src/emdbg/debug/px4/device.py` & `emdbg-1.0.3/src/emdbg/debug/px4/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
+from __future__ import annotations
 from . import utils
 from dataclasses import dataclass
 from .base import Base
 from functools import cached_property
 from pathlib import Path
 import re, time
```

### Comparing `emdbg-1.0.2/src/emdbg/debug/px4/pinout.py` & `emdbg-1.0.3/src/emdbg/debug/px4/pinout.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/debug/px4/semaphore.py` & `emdbg-1.0.3/src/emdbg/debug/px4/semaphore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
+from __future__ import annotations
 from functools import cached_property
 from dataclasses import dataclass
 from . import utils
 from .base import Base
 
 
 class Semaphore(Base):
```

### Comparing `emdbg-1.0.2/src/emdbg/debug/px4/svd.py` & `emdbg-1.0.3/src/emdbg/debug/px4/svd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
+from __future__ import annotations
 import io
 from pathlib import Path
 from collections import defaultdict
 from contextlib import redirect_stdout
 
 from . import utils
 from .base import Base
```

### Comparing `emdbg-1.0.2/src/emdbg/debug/px4/system_load.py` & `emdbg-1.0.3/src/emdbg/debug/px4/system_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
+from __future__ import annotations
 from functools import cached_property
 from . import utils
 from .base import Base
 from .device import Device
 import logging
 LOGGER = logging.getLogger(__name__)
```

### Comparing `emdbg-1.0.2/src/emdbg/debug/px4/task.py` & `emdbg-1.0.3/src/emdbg/debug/px4/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
-from functools import cached_property, cache
+from __future__ import annotations
+from functools import cached_property
 from . import utils
 from .system_load import SystemLoad
 from .device import Device
 from .base import Base
 from dataclasses import dataclass
 
 # The mapping from register name to position on the thread stack
```

### Comparing `emdbg-1.0.2/src/emdbg/debug/px4/utils.py` & `emdbg-1.0.3/src/emdbg/debug/px4/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
+from __future__ import annotations
 import re
 import math
 
 from datetime import datetime
 from itertools import zip_longest
 from pathlib import Path
```

### Comparing `emdbg-1.0.2/src/emdbg/debug/remote/__init__.py` & `emdbg-1.0.3/src/emdbg/debug/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/debug/remote/gdb.py` & `emdbg-1.0.3/src/emdbg/debug/remote/gdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
+from __future__ import annotations
 from contextlib import contextmanager
 import time
 
 
 class Interface:
     """
     The interface of all GDB remote access implementations.
```

### Comparing `emdbg-1.0.2/src/emdbg/debug/remote/gdb_api_bridge.py` & `emdbg-1.0.3/src/emdbg/debug/remote/gdb_api_bridge.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/debug/remote/mi.py` & `emdbg-1.0.3/src/emdbg/debug/remote/mi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
+from __future__ import annotations
 from contextlib import contextmanager
 import time
 import os
 import threading
 import signal
 import logging
 from .gdb import Interface
@@ -41,25 +42,22 @@
         self._response_thread.start()
 
     def _handle_responses(self):
         while self._run_thread:
             responses = self.mi.io_manager.get_gdb_response(timeout_sec=0, raise_error_on_timeout=False)
             for response in responses:
                 # print(response)
-                match (response["type"], response["message"]):
-                    # Previous command has done executing
-                    case "result", "done" | "running":
-                        self._command_is_done = True
-                    # Console is logging out messages
-                    case "console", _:
-                        if payload := response["payload"].encode("latin-1").decode('unicode_escape'):
-                            payload = payload.replace("\\e", "\033")
-                            self._payloads.append(payload)
-                            if "#" not in payload or VERBOSITY >= 3:
-                                LOGGER.debug(payload)
+                if response["type"] == "result" and response["message"] in ["done", "running"]:
+                    self._command_is_done = True
+                elif response["type"] == "console":
+                    if payload := response["payload"].encode("latin-1").decode('unicode_escape'):
+                        payload = payload.replace("\\e", "\033")
+                        self._payloads.append(payload)
+                        if "#" not in payload or VERBOSITY >= 3:
+                            LOGGER.debug(payload)
             time.sleep(0.01)
 
     def read(self, clear=True):
         p = self._payloads
         if clear: self._payloads = []
         return p
```

### Comparing `emdbg-1.0.2/src/emdbg/debug/remote/px4.py` & `emdbg-1.0.3/src/emdbg/debug/remote/px4.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/debug/remote/rpyc.py` & `emdbg-1.0.3/src/emdbg/debug/remote/rpyc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) 2015, Gallopsled et al.
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: MIT
 # Adapted from https://github.com/Gallopsled/pwntools
 
+from __future__ import annotations
 from threading import Event
 from contextlib import contextmanager
 import time
 from .gdb import Interface
 import logging
 LOGGER = logging.getLogger(__name__)
 from ...logger import VERBOSITY
```

### Comparing `emdbg-1.0.2/src/emdbg/debug/utils.py` & `emdbg-1.0.3/src/emdbg/debug/utils.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/io/digilent.py` & `emdbg-1.0.3/src/emdbg/io/digilent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
+from __future__ import annotations
 from pydwf import DwfLibrary
 from pydwf.utilities import openDwfDevice
 from contextlib import contextmanager
-from functools import cache
+from functools import lru_cache
 import enum
 import logging
 
 LOGGER = logging.getLogger("io:dwf")
 _DWF = None
 
 @contextmanager
@@ -160,15 +161,15 @@
     """
     def __init__(self, device):
         """
         :param device: DWF device
         """
         self.dwf = device
 
-    @cache
+    @lru_cache(100)
     def gpio(self, position: int) -> DigilentPin:
         """
         Creates a pin abstraction.
         :param position: Pin number
         """
         return DigilentPin(self.dwf.digitalIO, 1 << position)
```

### Comparing `emdbg-1.0.2/src/emdbg/logger.py` & `emdbg-1.0.3/src/emdbg/logger.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/patch/README.md` & `emdbg-1.0.3/src/emdbg/patch/README.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/patch/__main__.py` & `emdbg-1.0.3/src/emdbg/patch/__main__.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/patch/data/disable_uavcan_v5x.patch` & `emdbg-1.0.3/src/emdbg/patch/data/disable_uavcan_v5x.patch`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/patch/data/itm.h` & `emdbg-1.0.3/src/emdbg/patch/data/itm.h`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/patch/data/itm_nuttx_Makefile.patch` & `emdbg-1.0.3/src/emdbg/patch/data/itm_nuttx_Makefile.patch`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/patch/data/nuttx_tracing_itm.patch` & `emdbg-1.0.3/src/emdbg/patch/data/nuttx_tracing_itm.patch`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/patch/data/sem_boostlog.c` & `emdbg-1.0.3/src/emdbg/patch/data/sem_boostlog.c`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/patch/data/semaphore_boostlog.h` & `emdbg-1.0.3/src/emdbg/patch/data/semaphore_boostlog.h`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/patch/data/semaphore_boostlog.patch` & `emdbg-1.0.3/src/emdbg/patch/data/semaphore_boostlog.patch`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/patch/operation.py` & `emdbg-1.0.3/src/emdbg/patch/operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
+from __future__ import annotations
 import os
 import shutil
 import subprocess
 import hashlib
 from pathlib import Path
 from contextlib import contextmanager
 import logging
```

### Comparing `emdbg-1.0.2/src/emdbg/patch/set.py` & `emdbg-1.0.3/src/emdbg/patch/set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
+from __future__ import annotations
 from pathlib import Path
 from .operation import CopyOperation, PatchOperation, PatchManager
 
 def _data(file: str) -> Path:
     return Path(__file__).parent / "data" / file
```

### Comparing `emdbg-1.0.2/src/emdbg/power/README.md` & `emdbg-1.0.3/src/emdbg/power/README.md`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/power/base.py` & `emdbg-1.0.3/src/emdbg/power/base.py`

 * *Files identical despite different names*

### Comparing `emdbg-1.0.2/src/emdbg/power/yocto.py` & `emdbg-1.0.3/src/emdbg/power/yocto.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,13 @@
         dest="verbosity",
         action="count",
         help="Verbosity level.")
     args = parser.parse_args()
     emdbg.logger.configure(args.verbosity)
 
     with relay(args.channel, args.inverted, args.location) as pwr:
-        match args.command:
-            case "on":
-                pwr.on(args.time)
-            case "off":
-                pwr.off(args.time)
-            case "cycle":
-                pwr.cycle(args.time, args.time)
+        if args.command == "on":
+            pwr.on(args.time)
+        elif args.command == "off":
+            pwr.off(args.time)
+        elif args.command == "cycle":
+            pwr.cycle(args.time, args.time)
```

### Comparing `emdbg-1.0.2/src/emdbg/serial/protocol.py` & `emdbg-1.0.3/src/emdbg/serial/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
+from __future__ import annotations
 import re
 import time
 import logging
 from contextlib import contextmanager
 from pathlib import Path
 from serial import Serial
 from serial.threaded import ReaderThread, Protocol
```

### Comparing `emdbg-1.0.2/src/emdbg/serial/utils.py` & `emdbg-1.0.3/src/emdbg/serial/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) 2023, Auterion AG
 # SPDX-License-Identifier: BSD-3-Clause
 
+from __future__ import annotations
 from serial.tools import list_ports
 import logging
 LOGGER = logging.getLogger("serial")
 
 
 class SerialException(Exception):
     """Exception for all serial port related errors."""
```

### Comparing `emdbg-1.0.2/src/emdbg.egg-info/PKG-INFO` & `emdbg-1.0.3/src/emdbg.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: emdbg
-Version: 1.0.2
+Version: 1.0.3
 Summary: Embedded Debug Tools
 Author-email: Auterion <success@auterion.com>
 License: BSD-3-Clause
-Project-URL: Homepage, https://github.com/auterion/embedded-debug-tools
+Project-URL: GitHub, https://github.com/auterion/embedded-debug-tools
+Project-URL: Changelog, https://github.com/auterion/embedded-debug-tools/blob/main/CHANGELOG.md
 Keywords: embedded,debug,gdb,stm32,px4
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Embedded Systems
```

### Comparing `emdbg-1.0.2/src/emdbg.egg-info/SOURCES.txt` & `emdbg-1.0.3/src/emdbg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

