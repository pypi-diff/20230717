# Comparing `tmp/sbn-12.tar.gz` & `tmp/sbn-20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbn-12.tar", last modified: Fri Jun 23 14:27:51 2023, max compression
+gzip compressed data, was "sbn-20.tar", last modified: Mon Jul 17 05:57:45 2023, max compression
```

## Comparing `sbn-12.tar` & `sbn-20.tar`

### file list

```diff
@@ -1,76 +1,65 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-23 14:27:51.657055 sbn-12/
--rw-r--r--   0 bart      (1000) bart      (1000)     2958 2023-06-23 14:27:51.657055 sbn-12/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     2396 2023-06-20 12:31:49.000000 sbn-12/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-23 14:27:51.645054 sbn-12/files/
--rw-r--r--   0 bart      (1000) bart      (1000)   180711 2023-06-22 12:55:52.000000 sbn-12/files/ECHAabilify.png
--rw-r--r--   0 bart      (1000) bart      (1000)   193757 2023-06-22 12:55:52.000000 sbn-12/files/ECHAclozapine.png
--rw-r--r--   0 bart      (1000) bart      (1000)   197697 2023-06-22 12:55:52.000000 sbn-12/files/ECHAhaldol.png
--rw-r--r--   0 bart      (1000) bart      (1000)   232313 2023-06-22 12:55:52.000000 sbn-12/files/ECHAzyprexa.png
--rw-r--r--   0 bart      (1000) bart      (1000)  1685507 2023-06-22 11:04:43.000000 sbn-12/files/bevestigd.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)    69979 2023-06-22 12:56:01.000000 sbn-12/files/informed.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   287102 2023-06-20 11:29:34.000000 sbn-12/files/skull3.png
--rw-r--r--   0 bart      (1000) bart      (1000)   234877 2023-06-20 11:35:00.000000 sbn-12/files/verbatim2.png
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-23 14:27:51.653054 sbn-12/pdf/
--rw-r--r--   0 bart      (1000) bart      (1000)   238330 2023-06-22 10:55:52.000000 sbn-12/pdf/EM_T04_OTP-CR-117_19.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   236671 2023-06-22 10:55:52.000000 sbn-12/pdf/EM_T07_OTP-CR-117_19_001.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   257079 2023-06-22 10:55:52.000000 sbn-12/pdf/Elements-of-Crimes.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)    41559 2023-06-22 10:55:52.000000 sbn-12/pdf/Kamer.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   323490 2023-06-22 10:55:52.000000 sbn-12/pdf/Rome-Statute.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   571580 2023-06-22 10:55:52.000000 sbn-12/pdf/Rules-of-Procedure-and-Evidence.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)    50044 2023-06-22 10:55:52.000000 sbn-12/pdf/bevestigd.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)     1580 2023-06-22 13:08:51.000000 sbn-12/pyproject.toml
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-23 14:27:51.657055 sbn-12/sbn/
--rw-r--r--   0 bart      (1000) bart      (1000)     3213 2023-06-21 12:03:14.000000 sbn-12/sbn/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2521 2023-06-23 12:19:48.000000 sbn-12/sbn/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      600 2023-06-19 11:01:18.000000 sbn-12/sbn/clients.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1110 2023-06-19 11:01:18.000000 sbn-12/sbn/clocked.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2094 2023-06-22 10:49:46.000000 sbn-12/sbn/command.py
--rw-r--r--   0 bart      (1000) bart      (1000)      180 2023-06-19 11:01:18.000000 sbn-12/sbn/configs.py
--rw-r--r--   0 bart      (1000) bart      (1000)      817 2023-06-19 11:01:18.000000 sbn-12/sbn/decoder.py
--rw-r--r--   0 bart      (1000) bart      (1000)      399 2023-06-19 11:01:18.000000 sbn-12/sbn/default.py
--rw-r--r--   0 bart      (1000) bart      (1000)      302 2023-06-19 11:01:18.000000 sbn-12/sbn/defines.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1344 2023-06-19 11:01:18.000000 sbn-12/sbn/encoder.py
--rw-r--r--   0 bart      (1000) bart      (1000)      381 2023-06-19 11:01:18.000000 sbn-12/sbn/errored.py
--rw-r--r--   0 bart      (1000) bart      (1000)      956 2023-06-19 11:01:18.000000 sbn-12/sbn/evented.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1974 2023-06-19 11:01:18.000000 sbn-12/sbn/handler.py
--rw-r--r--   0 bart      (1000) bart      (1000)      954 2023-06-19 11:01:18.000000 sbn-12/sbn/listens.py
--rw-r--r--   0 bart      (1000) bart      (1000)      466 2023-06-19 11:01:18.000000 sbn-12/sbn/logging.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-23 14:27:51.657055 sbn-12/sbn/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      577 2023-06-21 14:58:57.000000 sbn-12/sbn/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      596 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/cfg.py
--rw-r--r--   0 bart      (1000) bart      (1000)      234 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      730 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      439 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      979 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    20870 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      725 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3615 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17837 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/mdl.py
--rw-r--r--   0 bart      (1000) bart      (1000)      208 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2355 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)      830 2023-06-22 10:51:45.000000 sbn-12/sbn/modules/rld.py
--rw-r--r--   0 bart      (1000) bart      (1000)     7741 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)      377 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/sts.py
--rw-r--r--   0 bart      (1000) bart      (1000)      964 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1014 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2448 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/udp.py
--rw-r--r--   0 bart      (1000) bart      (1000)      236 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/upt.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5769 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/wsd.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2033 2023-06-19 11:01:18.000000 sbn-12/sbn/objects.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2181 2023-06-19 11:01:18.000000 sbn-12/sbn/objfunc.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1839 2023-06-19 11:01:18.000000 sbn-12/sbn/parsers.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4739 2023-06-19 11:01:18.000000 sbn-12/sbn/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)      380 2023-06-19 11:01:18.000000 sbn-12/sbn/repeats.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2671 2023-06-21 14:02:53.000000 sbn-12/sbn/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1000)      928 2023-06-19 11:01:18.000000 sbn-12/sbn/threads.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2949 2023-06-19 11:01:18.000000 sbn-12/sbn/utility.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-23 14:27:51.657055 sbn-12/sbn.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     2958 2023-06-23 14:27:51.000000 sbn-12/sbn.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1299 2023-06-23 14:27:51.000000 sbn-12/sbn.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-06-23 14:27:51.000000 sbn-12/sbn.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       42 2023-06-23 14:27:51.000000 sbn-12/sbn.egg-info/entry_points.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        7 2023-06-23 14:27:51.000000 sbn-12/sbn.egg-info/requires.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        4 2023-06-23 14:27:51.000000 sbn-12/sbn.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-06-23 14:27:51.000000 sbn-12/sbn.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-06-23 14:27:51.657055 sbn-12/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      101 2023-06-19 11:01:18.000000 sbn-12/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:57:45.864786 sbn-20/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2958 2023-07-17 05:57:45.864786 sbn-20/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     2396 2023-07-16 19:32:30.000000 sbn-20/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:57:45.844786 sbn-20/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     1987 2023-07-17 04:53:14.000000 sbn-20/bin/sbn
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:57:45.852786 sbn-20/files/
+-rw-r--r--   0 bart      (1000) bart      (1000)   180711 2023-07-16 19:32:30.000000 sbn-20/files/ECHAabilify.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   193757 2023-07-16 19:32:30.000000 sbn-20/files/ECHAclozapine.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   197697 2023-07-16 19:32:30.000000 sbn-20/files/ECHAhaldol.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   232313 2023-07-16 19:32:30.000000 sbn-20/files/ECHAzyprexa.png
+-rw-r--r--   0 bart      (1000) bart      (1000)  1685507 2023-07-16 19:32:30.000000 sbn-20/files/bevestigd.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)    69979 2023-07-16 19:32:30.000000 sbn-20/files/informed.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   287102 2023-07-16 19:32:30.000000 sbn-20/files/skull3.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   234877 2023-07-16 19:32:30.000000 sbn-20/files/verbatim2.png
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:57:45.860786 sbn-20/pdf/
+-rw-r--r--   0 bart      (1000) bart      (1000)   238330 2023-07-16 19:32:30.000000 sbn-20/pdf/EM_T04_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   236671 2023-07-16 19:32:30.000000 sbn-20/pdf/EM_T07_OTP-CR-117_19_001.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   257079 2023-07-16 19:32:30.000000 sbn-20/pdf/Elements-of-Crimes.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)    41559 2023-07-16 19:32:30.000000 sbn-20/pdf/Kamer.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   323490 2023-07-16 19:32:30.000000 sbn-20/pdf/Rome-Statute.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   571580 2023-07-16 19:32:30.000000 sbn-20/pdf/Rules-of-Procedure-and-Evidence.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)    50044 2023-07-16 19:32:30.000000 sbn-20/pdf/bevestigd.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)     1562 2023-07-16 19:32:30.000000 sbn-20/pyproject.toml
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:57:45.860786 sbn-20/sbn/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1725 2023-07-16 20:27:57.000000 sbn-20/sbn/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1021 2023-07-16 19:33:37.000000 sbn-20/sbn/brokers.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1952 2023-07-16 19:33:37.000000 sbn-20/sbn/command.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      284 2023-07-16 19:39:53.000000 sbn-20/sbn/configs.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      938 2023-07-16 19:33:37.000000 sbn-20/sbn/decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1558 2023-07-16 19:33:37.000000 sbn-20/sbn/encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1248 2023-07-16 19:33:37.000000 sbn-20/sbn/errored.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1158 2023-07-16 19:33:37.000000 sbn-20/sbn/evented.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      353 2023-07-16 19:33:37.000000 sbn-20/sbn/locking.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      802 2023-07-16 19:33:37.000000 sbn-20/sbn/loggers.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:57:45.864786 sbn-20/sbn/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      380 2023-07-16 19:33:48.000000 sbn-20/sbn/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3528 2023-07-16 19:42:02.000000 sbn-20/sbn/modules/bsc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    19192 2023-07-16 19:36:10.000000 sbn-20/sbn/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      829 2023-07-16 19:36:26.000000 sbn-20/sbn/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4057 2023-07-16 19:41:06.000000 sbn-20/sbn/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17641 2023-07-16 19:40:40.000000 sbn-20/sbn/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2401 2023-07-16 19:33:48.000000 sbn-20/sbn/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     7441 2023-07-16 19:36:42.000000 sbn-20/sbn/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1036 2023-07-16 19:36:54.000000 sbn-20/sbn/modules/shp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      998 2023-07-16 19:37:11.000000 sbn-20/sbn/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2664 2023-07-16 19:40:10.000000 sbn-20/sbn/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5754 2023-07-16 19:33:48.000000 sbn-20/sbn/modules/wsd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1009 2023-07-16 19:37:25.000000 sbn-20/sbn/modules/wsh.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5069 2023-07-16 19:33:37.000000 sbn-20/sbn/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1297 2023-07-16 19:33:37.000000 sbn-20/sbn/parsers.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4332 2023-07-16 19:33:37.000000 sbn-20/sbn/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2174 2023-07-16 19:33:37.000000 sbn-20/sbn/reactor.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      928 2023-07-16 19:33:37.000000 sbn-20/sbn/recurse.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1246 2023-07-16 19:33:37.000000 sbn-20/sbn/repeats.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1873 2023-07-16 19:33:37.000000 sbn-20/sbn/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2153 2023-07-16 19:33:37.000000 sbn-20/sbn/utility.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:57:45.860786 sbn-20/sbn.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2958 2023-07-17 05:57:45.000000 sbn-20/sbn.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1068 2023-07-17 05:57:45.000000 sbn-20/sbn.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-07-17 05:57:45.000000 sbn-20/sbn.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        7 2023-07-17 05:57:45.000000 sbn-20/sbn.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        4 2023-07-17 05:57:45.000000 sbn-20/sbn.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-07-17 05:57:45.000000 sbn-20/sbn.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-07-17 05:57:45.864786 sbn-20/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      101 2023-07-16 19:32:30.000000 sbn-20/setup.py
```

### Comparing `sbn-12/PKG-INFO` & `sbn-20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbn
-Version: 12
+Version: 20
 Summary: Skull, Bones and Number (OTP-CR-117/19)
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/sbn
 Project-URL: bugs, https://github.com/bthate/sbn/issues
 Project-URL: source, https://github.com/bthate/sbn
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sbn-12/README.rst` & `sbn-20/README.rst`

 * *Files identical despite different names*

### Comparing `sbn-12/files/ECHAabilify.png` & `sbn-20/files/ECHAabilify.png`

 * *Files identical despite different names*

### Comparing `sbn-12/files/ECHAclozapine.png` & `sbn-20/files/ECHAclozapine.png`

 * *Files identical despite different names*

### Comparing `sbn-12/files/ECHAhaldol.png` & `sbn-20/files/ECHAhaldol.png`

 * *Files identical despite different names*

### Comparing `sbn-12/files/ECHAzyprexa.png` & `sbn-20/files/ECHAzyprexa.png`

 * *Files identical despite different names*

### Comparing `sbn-12/files/bevestigd.jpg` & `sbn-20/files/bevestigd.jpg`

 * *Files identical despite different names*

### Comparing `sbn-12/files/informed.jpg` & `sbn-20/files/informed.jpg`

 * *Files identical despite different names*

### Comparing `sbn-12/files/skull3.png` & `sbn-20/files/skull3.png`

 * *Files identical despite different names*

### Comparing `sbn-12/files/verbatim2.png` & `sbn-20/files/verbatim2.png`

 * *Files identical despite different names*

### Comparing `sbn-12/pdf/EM_T04_OTP-CR-117_19.pdf` & `sbn-20/pdf/EM_T04_OTP-CR-117_19.pdf`

 * *Files identical despite different names*

### Comparing `sbn-12/pdf/EM_T07_OTP-CR-117_19_001.pdf` & `sbn-20/pdf/EM_T07_OTP-CR-117_19_001.pdf`

 * *Files identical despite different names*

### Comparing `sbn-12/pdf/Elements-of-Crimes.pdf` & `sbn-20/pdf/Elements-of-Crimes.pdf`

 * *Files identical despite different names*

### Comparing `sbn-12/pdf/Kamer.pdf` & `sbn-20/pdf/Kamer.pdf`

 * *Files identical despite different names*

### Comparing `sbn-12/pdf/Rome-Statute.pdf` & `sbn-20/pdf/Rome-Statute.pdf`

 * *Files identical despite different names*

### Comparing `sbn-12/pdf/Rules-of-Procedure-and-Evidence.pdf` & `sbn-20/pdf/Rules-of-Procedure-and-Evidence.pdf`

 * *Files identical despite different names*

### Comparing `sbn-12/pdf/bevestigd.pdf` & `sbn-20/pdf/bevestigd.pdf`

 * *Files identical despite different names*

### Comparing `sbn-12/pyproject.toml` & `sbn-20/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "sbn"
 description = "Skull, Bones and Number (OTP-CR-117/19)"
-version = "12"
+version = "20"
 authors = [
     {name = "Bart Thate", email = "bthate@dds.nl" },
 ]
 readme = "README.rst"
 license = { text="Public Domain"}
 classifiers=[
              'Development Status :: 3 - Alpha',
@@ -23,27 +23,24 @@
 
 [project.urls]
 "home" = "https://pypi.org/project/sbn"
 "bugs" = "https://github.com/bthate/sbn/issues"
 "source" = "https://github.com/bthate/sbn"
 
 
-[project.scripts]
-sbn = "sbn.__main__:main"
-
-
 [project.optional-dependencies]
 dev = []
 
 [tool.setuptools]
 packages = [
             "sbn",
             "sbn.modules"
            ]
 zip-safe = true
+script-files = ["bin/sbn",]
 
 
 [tool.setuptools.data-files]
 "share/doc/sbn" = [
           "files/ECHAabilify.png",
           "files/ECHAclozapine.png",
           "files/ECHAhaldol.png",
```

### Comparing `sbn-12/sbn/clocked.py` & `sbn-20/sbn/repeats.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C0114,C0115,C0116
-
-
-"execute at a time"
+# pylint: disable=C,I,R,E0402
 
 
 import threading
 import time
 
 
 from .objects import Object
-from .runtime import launch
+from .threads import launch
 
 
 def __dir__():
     return (
-            'Timer',
+            'Repeater',
+            'Timer'
            )
 
 
+__all__ = __dir__()
+
+
 class Timer:
 
     def __init__(self, sleep, func, *args, thrname=None):
         super().__init__()
         self.args = args
         self.func = func
         self.sleep = sleep
@@ -46,7 +47,15 @@
         timer.func = self.func
         timer.start()
         self.timer = timer
 
     def stop(self) -> None:
         if self.timer:
             self.timer.cancel()
+
+
+class Repeater(Timer):
+
+    def run(self):
+        thr = launch(self.start)
+        super().run()
+        return thr
```

### Comparing `sbn-12/sbn/decoder.py` & `sbn-20/sbn/decoder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C0114,C0115,C0116
+# pylint: disable=C,I,R,E0402
 
 
-"json to object"
+"deconding objects"
+
+
+__author__ = "Bart Thate <programmingobject@gmail.com>"
 
 
 import json
 
 
-from .objects import Object, copy
+from .objects import Object
 
 
 def __dir__():
     return (
             'ObjectDecoder',
             'load',
-            'loads'
+            'loads',
            )
 
 
+__all__ = __dir__()
+
+
+
 class ObjectDecoder(json.JSONDecoder):
 
-    def decode(self, s, _w=None) -> Object:
+    def __init__(self, *args, **kwargs):
+        ""
+        json.JSONDecoder.__init__(self, *args, **kwargs)
+
+    def decode(self, s, _w=None):
+        ""
         val = json.JSONDecoder.decode(self, s)
         if not val:
             val = {}
-        obj = Object()
-        copy(obj, val)
-        return obj
+        return Object(val)
 
-    def raw_decode(self, s, idx=0) -> (int, Object):
+    def raw_decode(self, s, idx=0):
+        ""
         return json.JSONDecoder.raw_decode(self, s, idx)
 
 
-def load(fpt, *args, **kw) -> Object:
+def load(fpt, *args, **kw) :
     return json.load(fpt, *args, cls=ObjectDecoder, **kw)
 
 
-def loads(string, *args, **kw) -> Object:
+def loads(string, *args, **kw):
     return json.loads(string, *args, cls=ObjectDecoder, **kw)
```

### Comparing `sbn-12/sbn/encoder.py` & `sbn-20/sbn/encoder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C0114,C0115,C0116
+# pylint: disable=C,I,R
 
 
-"object to json"
+"encoding objects"
+
+
+__author__ = "Bart Thate <programmingobject@gmail.com>"
 
 
 import json
 
 
 from .objects import Object
 
 
 def __dir__():
     return (
             'ObjectEncoder',
             'dump',
-            'dumps'
+            'dumps',
            )
 
 
+__all__ = __dir__()
+
+
 class ObjectEncoder(json.JSONEncoder):
 
+    def __init__(self, *args, **kwargs):
+        ""
+        json.JSONEncoder.__init__(self, *args, **kwargs)
+
     def default(self, o) -> str:
+        ""
         if isinstance(o, dict):
             return o.items()
         if isinstance(o, Object):
             return vars(o)
         if isinstance(o, list):
             return iter(o)
         if isinstance(
@@ -42,17 +53,19 @@
             return str(o)
         try:
             return json.JSONEncoder.default(self, o)
         except TypeError:
             return str(o)
 
     def encode(self, o) -> str:
+        ""
         return json.JSONEncoder.encode(self, o)
 
     def iterencode(self, o, _one_shot=False) -> str:
+        ""
         return json.JSONEncoder.iterencode(self, o, _one_shot)
 
 
 def dump(*args, **kw) -> None:
     kw["cls"] = ObjectEncoder
     return json.dump(*args, **kw)
```

### Comparing `sbn-12/sbn/handler.py` & `sbn-20/sbn/reactor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,92 +1,106 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=R,C0114,C0115,C0116,W0613,W0212,W0703
+# pylint: disable=C,I,R,W0212,W0718
 
 
-"teh handler"
+"reacting"
+
+
+__author__ = "Bart Thate <programmingobject@gmail.com>"
 
 
 import queue
 import ssl
 import threading
 
 
 from .errored import Errors
 from .evented import Event
 from .objects import Object
-from .runtime import Cfg, launch
+from .threads import launch
 
 
 def __dir__():
     return (
-            'Handler',
+            'Reactor',
+            "dispatch"
            )
 
 
-class Handler(Object):
+__all__ = __dir__()
+
+
+class Reactor(Object):
 
     def __init__(self):
         Object.__init__(self)
         self.cbs = Object()
         self.queue = queue.Queue()
         self.stopped = threading.Event()
-        self.threaded = True
+
+    def announce(self, txt) -> None:
+        self.raw(txt)
 
     def event(self, txt) -> Event:
         msg = Event()
-        msg.type = 'command'
+        msg.type = 'event'
         msg.orig = repr(self)
-        msg.parse(txt)
+        msg.txt = txt
         return msg
 
     def handle(self, evt) -> Event:
         func = getattr(self.cbs, evt.type, None)
         if func:
-            if "t" in Cfg.opts:
-                evt._thr = launch(dispatch, func, evt, name=evt.cmd)
-            else:
-                dispatch(func, evt)
+            evt._thr = launch(dispatch, func, evt, name=evt.cmd)
+            evt._thr.join()
         return evt
 
     def loop(self) -> None:
         while not self.stopped.is_set():
             try:
                 self.handle(self.poll())
-            except (ssl.SSLError, EOFError, KeyboardInterrupt) as ex:
+            except (ssl.SSLError, EOFError) as ex:
                 Errors.handle(ex)
                 self.restart()
 
     def one(self, txt) -> Event:
         return self.handle(self.event(txt))
 
     def poll(self) -> Event:
         return self.queue.get()
 
     def put(self, evt) -> None:
         self.queue.put_nowait(evt)
 
-    def register(self, cmd, func) -> None:
-        setattr(self.cbs, cmd, func)
+    def raw(self, txt) -> None:
+        pass
+
+    def say(self, channel, txt) -> None:
+        if channel:
+            self.raw(txt)
+
+    def register(self, typ, func) -> None:
+        self.cbs[typ] = func
 
     def restart(self) -> None:
         self.stop()
         self.start()
 
     def start(self) -> None:
         launch(self.loop)
 
     def stop(self) -> None:
         self.stopped.set()
         self.queue.put_nowait(None)
 
 
-# HANDLERS
-
-
 def dispatch(func, evt) -> None:
     try:
         func(evt)
     except Exception as ex:
         exc = ex.with_traceback(ex.__traceback__)
         Errors.errors.append(exc)
-        evt.ready()
+        try:
+            evt.ready()
+        except AttributeError:
+            pass
```

### Comparing `sbn-12/sbn/modules/fnd.py` & `sbn-20/sbn/modules/wsh.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C0116
+# pylint: disable=C,I,R,W0401,W0614
 
 
-"locate objects"
+"wish list"
+
+
+__author__ = "Bart Thate <programmingobject@gmail.com>"
 
 
 import time
 
 
-from ..objects import keys
-from ..objfunc import prt
-from ..persist import Persist
-from ..utility import elapsed, fntime
+from .. import Object
+from .. import find, fntime, laps, write
+
+
+class Wish(Object):
 
+    def __init__(self):
+        Object.__init__(self)
+        self.txt = ''
 
-def fnd(event):
+    def gettxt(self):
+        return self.txt
+
+    def settxt(self, txt):
+        self.txt = txt
+
+
+def ful(event):
     if not event.args:
-        res = sorted([x.split('.')[-1].lower() for x in Persist.files()])
-        if res:
-            event.reply(",".join(res))
-        else:
-            event.reply('no types yet.')
         return
-    otype = event.args[0]
-    nmr = 0
-    keyz = None
-    if event.gets:
-        keyz = ','.join(keys(event.gets))
-    if len(event.args) > 1:
-        keyz += ',' + ','.join(event.args[1:])
-    for obj in Persist.find(otype, event.gets):
-        if not keyz:
-            keyz = ',' + ','.join(keys(obj))
-        prnt = prt(obj, keyz)
-        lap = elapsed(time.time()-fntime(obj.__oid__))
-        event.reply(f'{nmr} {prnt} {lap}')
-        nmr += 1
-    if not nmr:
-        event.reply(f'no result ({event.txt})')
+    selector = {'txt': event.args[0]}
+    for obj in find('wish', selector):
+        obj.__deleted__ = True
+        write(obj)
+        event.reply('done')
+
+
+def wsh(event):
+    if not event.rest:
+        nmr = 0
+        for obj in find('wish'):
+            lap = laps(time.time()-fntime(obj.__oid__))
+            event.reply(f'{nmr} {obj.txt} {lap}')
+            nmr += 1
+        if not nmr:
+            event.reply("no wishes")
+        return
+    obj = Wish()
+    obj.txt = event.rest
+    write(obj)
+    event.reply('ok')
```

### Comparing `sbn-12/sbn/modules/irc.py` & `sbn-20/sbn/modules/irc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,100 +1,87 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=E0012,R,C0114,C0115,C0116,C0209,W0613,E1101
-# flake8:
-# pylama: ignore=C901
+# pylint: disable=C,I,R,W0401
 
 
 "internet relay chat"
 
 
+__author__ = "Bart Thate <programmingobject@gmail.com>"
+
+
 import base64
 import os
 import queue
 import random
 import socket
 import ssl
 import time
 import textwrap
 import threading
-import _thread
 
 
-from ..clients import Client
-from ..command import Commands
-from ..default import Default
-from ..errored import Errors
-from ..evented import Event
-from ..listens import Listens
-from ..logging import Logging
-from ..objects import Object, copy, keys, update
-from ..objfunc import edit, prt
-from ..persist import Persist, last, write
-from ..runtime import NAME, launch
-from ..utility import elapsed, fntime
+from .. import Broker, Cfg, Command, Errors, Event, Logging, Object, Reactor
+from .. import edit, find, fntime, keys, laps, last, prt, write
+from .. import launch, parse, update
 
 
-saylock = _thread.allocate_lock()
+from ..locking import saylock
 
 
 def start():
     irc = IRC()
-    irc.start()
-    irc.joined.wait()
+    launch(irc.start)
+    irc.events.joined.wait()
     return irc
 
 
-class NoUser(Exception):
+def stop():
+    for bot in Broker.objs:
+        if "IRC" in str(type(bot)):
+            bot.stop()
 
-    pass
 
+class NoUser(Exception):
 
-# CONFIG
+    pass
 
 
-class Config(Default):
+class Config(Object):
 
-    channel = '#%s' % NAME
+    channel = f'#{Cfg.name}'
     control = '!'
-    nick = NAME
-    nocommands = True
+    edited = time.time()
+    nick = Cfg.name
+    nocommands = False
     password = ''
     port = 6667
-    realname = NAME
+    realname = Cfg.name
     sasl = False
     server = 'localhost'
     servermodes = ''
     sleep = 60
-    username = NAME
+    username = Cfg.name
     users = False
     verbose = False
 
     def __init__(self):
-        Default.__init__(self)
-        self.control = Config.control
+        Object.__init__(self)
         self.channel = Config.channel
         self.nick = Config.nick
-        self.nocommands = Config.nocommands
-        self.password = Config.password
         self.port = Config.port
         self.realname = Config.realname
-        self.sasl = Config.sasl
         self.server = Config.server
-        self.servermodes = Config.servermodes
-        self.sleep = Config.sleep
         self.username = Config.username
-        self.users = Config.users
-        self.verbose = Config.verbose
 
+    def __edited__(self):
+        return Config.edited
 
-Persist.add(Config)
-
-
-# OUTPUT
+    def __size__(self):
+        return len(Config)
 
 
 class TextWrap(textwrap.TextWrapper):
 
     def __init__(self):
         super().__init__()
         self.break_long_words = False
@@ -109,16 +96,14 @@
 
     cache = Object()
 
     def __init__(self):
         Object.__init__(self)
         self.oqueue = queue.Queue()
         self.dostop = threading.Event()
-        self.state = Default()
-        self.state.starttime = time.time()
 
     def dosay(self, channel, txt):
         raise NotImplementedError
 
     def extend(self, channel, txtlist):
         if channel not in self.cache:
             setattr(self.cache, channel, [])
@@ -149,17 +134,18 @@
             wrapper = TextWrap()
             try:
                 txtlist = wrapper.wrap(txt)
             except AttributeError:
                 continue
             if len(txtlist) > 3:
                 self.extend(channel, txtlist)
+                length = len(txtlist)
                 self.dosay(
                            channel,
-                           'use !mre to show more (+%s)' % len(txtlist)
+                           f"use !mre to show more (+{length})"
                           )
                 continue
             _nr = -1
             for txt in txtlist:
                 _nr += 1
                 self.dosay(channel, txt)
 
@@ -174,140 +160,105 @@
         return self
 
     def stop(self):
         self.dostop.set()
         self.oqueue.put_nowait((None, None))
 
 
-# IRC
-
-
-class IRC(Client, Output):
+class IRC(Reactor, Output):
 
     def __init__(self):
-        Client.__init__(self)
+        Reactor.__init__(self)
         Output.__init__(self)
         self.buffer = []
         self.cfg = Config()
-        self.authed = threading.Event()
-        self.connected = threading.Event()
+        self.events = Object()
+        self.events.authed = threading.Event()
+        self.events.connected = threading.Event()
+        self.events.joined = threading.Event()
         self.channels = []
-        self.joined = threading.Event()
-        self.keeprunning = False
-        self.outqueue = queue.Queue()
         self.sock = None
-        self.speed = 'slow'
         self.state = Object()
-        self.state.needconnect = False
-        self.state.errors = []
-        self.state.last = 0
-        self.state.lastline = ''
+        self.state.keeprunning = False
         self.state.nrconnect = 0
-        self.state.nrerror = 0
         self.state.nrsend = 0
-        self.state.pongcheck = False
-        self.state.starttime = time.time()
-        self.threaded = False
         self.zelf = ''
-        self.register('903', self.h903)
-        self.register('904', self.h903)
-        self.register('AUTHENTICATE', self.auth)
-        self.register('CAP', self.cap)
-        self.register('ERROR', self.error)
-        self.register('LOG', self.log)
-        self.register('NOTICE', self.notice)
-        self.register('PRIVMSG', self.privmsg)
-        self.register('QUIT', self.quit)
-        self.register("command", self.docommand)
-        self.target = 'type'
+        self.register('903', cb_h903)
+        self.register('904', cb_h903)
+        self.register('AUTHENTICATE', cb_auth)
+        self.register('CAP', cb_cap)
+        self.register('ERROR', cb_error)
+        self.register('LOG', cb_log)
+        self.register('NOTICE', cb_notice)
+        self.register('PRIVMSG', cb_privmsg)
+        self.register('QUIT', cb_quit)
+        Broker.add(self)
 
     def announce(self, txt):
         for channel in self.channels:
             self.say(channel, txt)
 
-    def auth(self, event):
-        assert self.cfg.password
-        self.direct('AUTHENTICATE %s' % self.cfg.password)
-
-    def cap(self, event):
-        if self.cfg.password and 'ACK' in event.arguments:
-            self.direct('AUTHENTICATE PLAIN')
-        else:
-            self.direct('CAP REQ :sasl')
-
     def command(self, cmd, *args):
         with saylock:
             if not args:
                 self.raw(cmd)
             elif len(args) == 1:
-                self.raw('%s %s' % (cmd.upper(), args[0]))
+                self.raw(f'{cmd.upper()} {args[0]}')
             elif len(args) == 2:
-                self.raw(
-                         '%s %s :%s' % (
-                                        cmd.upper(),
-                                        args[0],
-                                        ' '.join(args[1:])
-                                       )
-                        )
+                txt = ' '.join(args[1:])
+                self.raw(f'{cmd.upper()} {args[0]} :{txt}')
             elif len(args) >= 3:
-                self.raw(
-                         '%s %s %s :%s' % (
-                                           cmd.upper(),
-                                           args[0],
-                                           args[1],
-                                           ' '.join(args[2:])
-                                           )
-                        )
+                txt = ' '.join(args[2:])
+                self.raw("{cmd.upper()} {args[0]} {args[1]} :{txt}")
             if (time.time() - self.state.last) < 5.0:
                 time.sleep(5.0)
             self.state.last = time.time()
 
     def connect(self, server, port=6667):
         self.state.nrconnect += 1
-        self.connected.clear()
+        self.events.connected.clear()
         Logging.debug(f"connecting to {server}:{port}")
         if self.cfg.password:
             Logging.debug("using SASL")
             self.cfg.sasl = True
+            self.cfg.port = "6697"
             ctx = ssl.SSLContext(ssl.PROTOCOL_TLS)
             ctx.check_hostname = False
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock = ctx.wrap_socket(sock)
             self.sock.connect((server, port))
+            time.sleep(1.0)
             self.command('CAP LS 302')
         else:
             addr = socket.getaddrinfo(server, port, socket.AF_INET)[-1][-1]
             self.sock = socket.create_connection(addr)
-            self.authed.set()
+            self.events.authed.set()
         if self.sock:
-            os.set_inheritable(self.fileno(), os.O_RDWR)
+            os.set_inheritable(self.sock.fileno(), os.O_RDWR)
             self.sock.setblocking(True)
             self.sock.settimeout(180.0)
-            self.connected.set()
+            self.events.connected.set()
             return True
         return False
 
     def direct(self, txt):
+        time.sleep(1.0)
         Logging.debug(txt)
         self.sock.send(bytes(txt.rstrip()+'\r\n', 'utf-8'))
 
     def disconnect(self):
         try:
             self.sock.shutdown(2)
         except (
                 ssl.SSLError,
                 OSError,
                 BrokenPipeError
                ) as ex:
             Errors.errors.append(ex)
 
-    def docommand(self, evt):
-        evt.orig = repr(self)
-        Commands.handle(evt)
-
     def doconnect(self, server, nck, port=6667):
         while 1:
             try:
                 if self.connect(server, port):
                     break
             except (
                     ssl.SSLError,
@@ -317,112 +268,72 @@
                 self.state.errors = str(ex)
                 Logging.debug(str(ex))
             Logging.debug(f"sleeping {self.cfg.sleep} seconds")
             time.sleep(self.cfg.sleep)
         self.logon(server, nck)
 
     def dosay(self, channel, txt):
-        self.joined.wait()
+        self.events.joined.wait()
         txt = str(txt).replace('\n', '')
         txt = txt.replace('  ', ' ')
         self.command('PRIVMSG', channel, txt)
 
-    def error(self, event):
-        self.state.nrerror += 1
-        self.state.errors.append(event.txt)
-        Logging.debug(event.txt)
-
     def event(self, txt):
         evt = self.parsing(txt)
         cmd = evt.command
         if cmd == 'PING':
             self.state.pongcheck = True
             self.command('PONG', evt.txt or '')
         elif cmd == 'PONG':
             self.state.pongcheck = False
         if cmd == '001':
             self.state.needconnect = False
             if self.cfg.servermodes:
-                self.command(
-                             'MODE %s %s' % (
-                                             self.cfg.nick,
-                                             self.cfg.servermodes
-                                            )
-                            )
+                self.command(f'MODE {self.cfg.nick} {self.cfg.servermodes}')
             self.zelf = evt.args[-1]
             self.joinall()
         elif cmd == '002':
             self.state.host = evt.args[2][:-1]
         elif cmd == '366':
             self.state.errors = []
-            self.joined.set()
+            self.events.joined.set()
         elif cmd == '433':
             self.state.errors = txt
             nck = self.cfg.nick + '_' + str(random.randint(1, 10))
             self.command('NICK', nck)
         return evt
 
-    def fileno(self):
-        return self.sock.fileno()
-
-    def h903(self, event):
-        self.command('CAP END')
-        self.authed.set()
-
-    def h904(self, event):
-        self.command('CAP END')
-        self.authed.set()
-
     def joinall(self):
         for channel in self.channels:
             self.command('JOIN', channel)
 
     def keep(self):
         while 1:
-            self.connected.wait()
-            self.keeprunning = True
+            self.events.connected.wait()
+            self.events.authed.wait()
+            self.state.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
             self.command('PING', self.cfg.server)
             if self.state.pongcheck:
                 Logging.debug("failed pongcheck, restarting")
                 self.state.pongcheck = False
-                self.keeprunning = False
-                self.connected.clear()
+                self.state.keeprunning = False
+                self.events.connected.clear()
                 self.stop()
                 start()
                 break
 
     def logon(self, server, nck):
-        self.connected.wait()
-        self.authed.wait()
-        self.direct('NICK %s' % nck)
-        self.direct(
-                    'USER %s %s %s :%s' % (
-                                           self.cfg.username or nck,
-                                           server,
-                                           server,
-                                           self.cfg.realname or nck
-                                          )
-                   )
+        self.events.connected.wait()
+        self.events.authed.wait()
+        nck = self.cfg.username
+        self.command(f'NICK {nck}')
+        self.command(f'USER {nck} {server} {server} {nck}')
 
-    def kill(self, event):
-        pass
-
-    def log(self, event):
-        pass
-
-    def notice(self, event):
-        if event.txt.startswith('VERSION'):
-            txt = '\001VERSION %s %s - %s\001' % (
-                'op',
-                self.cfg.version,
-                self.cfg.username,
-            )
-            self.command('NOTICE', event.channel, txt)
 
     def parsing(self, txt):
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
         Logging.debug(txt)
         obj = Event()
@@ -475,15 +386,15 @@
             obj.args = spl[1:]
         obj.orig = repr(self)
         obj.txt = obj.txt.strip()
         obj.type = obj.command
         return obj
 
     def poll(self):
-        self.connected.wait()
+        self.events.connected.wait()
         if not self.buffer:
             try:
                 self.some()
             except BlockingIOError as ex:
                 time.sleep(1.0)
                 return self.event(str(ex))
             except (
@@ -493,44 +404,21 @@
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
                 Errors.errors.append(ex)
                 self.stop()
                 Logging.debug("handler stopped")
+                return self.event(str(ex))
         try:
             txt = self.buffer.pop(0)
         except IndexError:
             txt = ""
         return self.event(txt)
 
-    def privmsg(self, event):
-        if self.cfg.nocommands:
-            return
-        if event.txt:
-            if event.txt[0] in [self.cfg.control, '!']:
-                event.txt = event.txt[1:]
-            elif event.txt.startswith('%s:' % self.cfg.nick):
-                event.txt = event.txt[len(self.cfg.nick)+1:]
-            else:
-                return
-            if self.cfg.users and not Users.allowed(event.origin, 'USER'):
-                return
-            Logging.debug(f"command from {event.origin}: {event.txt}")
-            msg = Event()
-            copy(msg, event)
-            msg.type = 'command'
-            msg.parse(event.txt)
-            self.handle(msg)
-
-    def quit(self, event):
-        Logging.debug(f"quit from {self.cfg.server}")
-        if event.orig and event.orig in self.zelf:
-            self.stop()
-
     def raw(self, txt):
         txt = txt.rstrip()
         Logging.debug(txt)
         if not txt.endswith('\r\n'):
             txt += '\r\n'
         txt = txt[:512]
         txt += '\n'
@@ -553,23 +441,23 @@
 
     def reconnect(self):
         Logging.debug(f"reconnecting to {self.cfg.server}")
         try:
             self.disconnect()
         except (ssl.SSLError, OSError):
             pass
-        self.connected.clear()
-        self.joined.clear()
+        self.events.connected.clear()
+        self.events.joined.clear()
         self.doconnect(self.cfg.server, self.cfg.nick, int(self.cfg.port))
 
     def say(self, channel, txt):
         self.oput(channel, txt)
 
     def some(self):
-        self.connected.wait()
+        self.events.connected.wait()
         if not self.sock:
             return
         inbytes = self.sock.recv(512)
         txt = str(inbytes, 'utf-8')
         if txt == '':
             raise ConnectionResetError
         self.state.lastline += txt
@@ -578,48 +466,128 @@
             self.buffer.append(line)
         self.state.lastline = splitted[-1]
 
     def start(self):
         last(self.cfg)
         if self.cfg.channel not in self.channels:
             self.channels.append(self.cfg.channel)
-        self.connected.clear()
-        self.joined.clear()
-        launch(Client.start, self)
+        self.events.connected.clear()
+        self.events.joined.clear()
+        launch(Reactor.start, self)
         launch(Output.start, self)
         launch(
                self.doconnect,
                self.cfg.server or "localhost",
                self.cfg.nick,
                int(self.cfg.port or '6667')
               )
-        if not self.keeprunning:
+        if not self.state.keeprunning:
             launch(self.keep)
 
     def stop(self):
-        Listens.remove(self)
-        Client.stop(self)
+        Broker.remove(self)
+        Reactor.stop(self)
         Output.stop(self)
         self.disconnect()
 
 
-# USERS
+def cb_auth(evt):
+    bot = evt.bot()
+    assert evt
+    assert bot.cfg.password
+    bot.direct(f'AUTHENTICATE {bot.cfg.password}')
+
+
+def cb_cap(evt):
+    bot = evt.bot()
+    if bot.cfg.password and 'ACK' in evt.arguments:
+        bot.direct('AUTHENTICATE PLAIN')
+    else:
+        bot.direct('CAP REQ :sasl')
+
+
+def cb_command(evt):
+    Command.handle(evt)
+
+
+def cb_error(evt):
+    bot = evt.bot()
+    bot.state.nrerror += 1
+    bot.state.errors.append(evt.txt)
+    Logging.debug(evt.txt)
+
+
+def cb_h903(evt):
+    assert evt
+    bot = evt.bot()
+    bot.direct('CAP END')
+    bot.events.authed.set()
+
+
+def cb_h904(evt):
+    assert evt
+    bot = evt.bot()
+    bot.direct('CAP END')
+    bot.events.authed.set()
+
+
+def cb_kill(evt):
+    pass
+
+
+def cb_log(evt):
+    pass
+
+
+def cb_notice(evt):
+    bot = evt.bot()
+    if evt.txt.startswith('VERSION'):
+        txt = f'\001VERSION {Cfg.name.upper()} 140 - {bot.cfg.username}\001'
+        bot.command('NOTICE', evt.channel, txt)
+
+
+def cb_privmsg(evt):
+    bot = evt.bot()
+    if bot.cfg.nocommands:
+        return
+    if evt.txt:
+        if evt.txt[0] in ['!',]:
+            evt.txt = evt.txt[1:]
+        elif evt.txt.startswith(f'{bot.cfg.nick}:'):
+            evt.txt = evt.txt[len(bot.cfg.nick)+1:]
+        else:
+            return
+        if bot.cfg.users and not Users.allowed(evt.origin, 'USER'):
+            return
+        Logging.debug(f"command from {evt.origin}: {evt.txt}")
+        parse(evt, evt.txt)
+        Command.handle(evt)
+
+
+def cb_quit(evt):
+    bot = evt.bot()
+    Logging.debug(f"quit from {bot.cfg.server}")
+    if evt.orig and evt.orig in bot.zelf:
+        bot.stop()
 
 
 class User(Object):
 
     def __init__(self, val=None):
         Object.__init__(self)
         self.user = ''
         self.perms = []
         if val:
             update(self, val)
 
+    def isok(self):
+        return True
 
-Persist.add(User)
+    def isthere(self):
+        return True
 
 
 class Users(Object):
 
     @staticmethod
     def allowed(origin, perm):
         perm = perm.upper()
@@ -640,15 +608,15 @@
             except ValueError:
                 pass
         return res
 
     @staticmethod
     def get_users(origin=''):
         selector = {'user': origin}
-        return Persist.find('user', selector)
+        return find('user', selector)
 
     @staticmethod
     def get_user(origin):
         users = list(Users.get_users(origin))
         res = None
         if len(users) > 0:
             res = users[-1]
@@ -661,17 +629,14 @@
             raise NoUser(origin)
         if permission.upper() not in user.perms:
             user.perms.append(permission.upper())
             write(user)
         return user
 
 
-# COMMANDS
-
-
 def cfg(event):
     config = Config()
     last(config)
     if not event.sets:
         event.reply(
                     prt(
                         config,
@@ -686,26 +651,26 @@
 
 
 def dlt(event):
     if not event.args:
         event.reply('dlt <username>')
         return
     selector = {'user': event.args[0]}
-    for obj in Persist.find('user', selector):
+    for obj in find('user', selector):
         obj.__deleted__ = True
         write(obj)
         event.reply('ok')
         break
 
 
 def met(event):
     if not event.args:
         nmr = 0
-        for obj in Persist.find('user'):
-            lap = elapsed(time.time() - fntime(obj.__fnm__))
+        for obj in find('user'):
+            lap = laps(time.time() - fntime(obj.__fnm__))
             event.reply(f'{nmr} {obj.user} {obj.perms} {lap}s')
             nmr += 1
         if not nmr:
             event.reply('no user')
         return
     user = User()
     user.user = event.rest
@@ -719,26 +684,28 @@
         event.reply('channel is not set.')
         return
     bot = event.bot()
     if 'cache' not in dir(bot):
         event.reply('bot is missing cache')
         return
     if event.channel not in bot.cache:
-        event.reply('no output in %s cache.' % event.channel)
+        event.reply(f'no output in {event.channel} cache.')
         return
     for _x in range(3):
         txt = bot.gettxt(event.channel)
         if txt:
             bot.say(event.channel, txt)
     size = bot.size(event.channel)
-    event.reply('%s more in cache' % size)
+    event.reply(f'{size} more in cache')
 
 
 def pwd(event):
     if len(event.args) != 2:
         event.reply('pwd <nick> <password>')
         return
-    txt = '\x00%s\x00%s' % (event.args[0], event.args[1])
+    arg1 = event.args[0]
+    arg2 = event.args[1]
+    txt = f'\x00{arg1}\x00{arg2}'
     enc = txt.encode('ascii')
     base = base64.b64encode(enc)
     dcd = base.decode('ascii')
     event.reply(dcd)
```

### Comparing `sbn-12/sbn/modules/log.py` & `sbn-20/sbn/modules/log.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=R,C0114,C0115,C0116
+# pylint: disable=C,I,R
 
 
-"log some text"
+"log text"
+
+
+__author__ = "Bart Thate <programmingobject@gmail.com>"
 
 
 import time
 
 
-from ..objects import Object
-from ..persist import Persist, write
-from ..utility import elapsed, fntime
+from .. import Object
+from .. import find, fntime, laps, write
 
 
 class Log(Object):
 
     def __init__(self):
         super().__init__()
+        self.createtime = time.time()
         self.txt = ''
 
+    def __size__(self):
+        return len(self.txt)
 
-Persist.add(Log)
-
-
-# COMMANDS
+    def __since__(self):
+        return self.createtime
 
 
 def log(event):
     if not event.rest:
         nmr = 0
-        for obj in Persist.find('log'):
-            lap = elapsed(time.time() - fntime(obj.__oid__))
+        for obj in find('log'):
+            lap = laps(time.time() - fntime(obj.__oid__))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
             event.reply('no log')
         return
     obj = Log()
     obj.txt = event.rest
```

### Comparing `sbn-12/sbn/modules/mbx.py` & `sbn-20/sbn/modules/mbx.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,70 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C0103,C0209,C0301,C0115,C0116,W0212,R0903
+# pylint: disable=C,I,R,W0212,W0401
 
 
 "mailbox"
 
 
+__author__ = "Bart Thate <programmingobject@gmail.com>"
+
+
 import mailbox
 import os
 import time
 
 
-from ..objects import Object, update
-from ..objfunc import prt
-from ..persist import Persist, write
-from ..utility import elapsed, fntime
-
+from .. import Object
+from .. import find, fntime, laps, prt, update, write
 
-bdmonths = ['Bo', 'Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
 
+bdmonths = [
+            'Bo',
+            'Jan',
+            'Feb',
+            'Mar',
+            'Apr',
+            'May',
+            'Jun',
+            'Jul',
+            'Aug',
+            'Sep',
+            'Oct',
+            'Nov',
+            'Dec'
+           ]
 
 monthint = {
-    'Jan': 1,
-    'Feb': 2,
-    'Mar': 3,
-    'Apr': 4,
-    'May': 5,
-    'Jun': 6,
-    'Jul': 7,
-    'Aug': 8,
-    'Sep': 9,
-    'Oct': 10,
-    'Nov': 11,
-    'Dec': 12
-}
+            'Jan': 1,
+            'Feb': 2,
+            'Mar': 3,
+            'Apr': 4,
+            'May': 5,
+            'Jun': 6,
+            'Jul': 7,
+            'Aug': 8,
+            'Sep': 9,
+            'Oct': 10,
+            'Nov': 11,
+            'Dec': 12
+           }
 
 
 class Email(Object):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.text = ""
 
+    def len(self):
+        return len(self.__dict__)
 
-Persist.add(Email)
+    def size(self):
+        return len(self.__dict__)
 
 
 def to_date(date):
     date = date.replace("_", ":")
     res = date.split()
     ddd = ""
     try:
@@ -82,59 +99,61 @@
     return ddd
 
 
 def cor(event):
     if not event.args:
         event.reply("cor <email>")
         return
-    nr = -1
-    for _fn, email in Persist.find("email", {"From": event.args[0]}):
-        nr += 1
+    nrs = -1
+    for email in find("email", {"From": event.args[0]}):
+        nrs += 1
         txt = ""
         if len(event.args) > 1:
             txt = ",".join(event.args[1:])
         else:
             txt = "From,Subject"
-        event.reply("%s %s %s" % (nr, prt(email, txt, plain=True), elapsed(time.time() - fntime(email.__stp__))))
-
+        lsp = laps(time.time() - fntime(email.__oid__))
+        txt = prt(email, txt, plain=True)
+        event.reply(f"{nrs} {txt} {lsp}")
 
 
 def eml(event):
     if not event.args:
         event.reply("eml <searchtxtinemail>")
         return
-    nr = -1
-    for fn, o in Persist.find("email"):
-        if event.rest in o.text:
-            nr += 1
-            event.reply("%s %s %s" % (nr, prt(o, "From,Subject"), elapsed(time.time() - fntime(fn))))
-
+    nrs = -1
+    for email in find("email"):
+        if event.rest in email.text:
+            nrs += 1
+            txt = prt(email, "From,Subject")
+            lsp = laps(time.time() - fntime(email.__oid__))
+            event.reply(f"{nrs} {txt} {lsp}")
 
 
 def mbx(event):
     if not event.args:
         return
-    fn = os.path.expanduser(event.args[0])
-    event.reply("reading from %s" % fn)
-    nr = 0
-    if os.path.isdir(fn):
-        thing = mailbox.Maildir(fn, create=False)
-    elif os.path.isfile(fn):
-        thing = mailbox.mbox(fn, create=False)
+    path = os.path.expanduser(event.args[0])
+    event.reply("reading from {path}")
+    nrs = 0
+    if os.path.isdir(path):
+        thing = mailbox.Maildir(path, create=False)
+    elif os.path.isfile(path):
+        thing = mailbox.mbox(path, create=False)
     else:
         return
     try:
         thing.lock()
     except FileNotFoundError:
         pass
-    for m in thing:
-        o = Email()
-        update(o, m._headers)
-        o.text = ""
-        for payload in m.walk():
+    for mail in thing:
+        email = Email()
+        update(email, mail._headers)
+        email.text = ""
+        for payload in mail.walk():
             if payload.get_content_type() == 'text/plain':
-                o.text += payload.get_payload()
-        o.text = o.text.replace("\\n", "\n")
-        write(o)
-        nr += 1
-    if nr:
-        event.reply("ok %s" % nr)
+                email.text += payload.get_payload()
+        email.text = email.text.replace("\\n", "\n")
+        write(email)
+        nrs += 1
+    if nrs:
+        event.reply("ok {nrs}")
```

### Comparing `sbn-12/sbn/modules/mdl.py` & `sbn-20/sbn/modules/mdl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,29 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,I,R,,W0613,E1101,E0402
+# pylint: disable=C,I,R,W0613,E1101,E0402,W0401
 # pylama: ignore=E225,E501
 
 
-"genocide model for here in the netherlands"
+"genocide model of the netherlands"
 
 
-import datetime
-import time
+__author__ = "Bart Thate <programmingobject@gmail.com>"
 
 
-from ..evented import Event
-from ..listens import Listens
-from ..objects import Object, copy, keys
-from ..repeats import Repeater
-from ..runtime import launch
-from ..utility import elapsed
+import datetime
+import time
 
 
-def __dir__():
-    return (
-        'mdl',
-        'now',
-        'start'
-    )
+from .. import Broker, Event, Object, Repeater
+from .. import laps, launch, keys
 
 
 def start():
+    time.sleep(60.0)
     for key in keys(oorzaken):
         val = getattr(oorzaken, key, None)
         if val and int(val) > 10000:
             evt = Event()
             evt.txt = ""
             evt.rest = key
             sec = seconds(val)
@@ -42,15 +34,14 @@
 
 DAY=24*60*60
 YEAR = 365*DAY
 SOURCE = "https://github.com/bthate/genocide"
 STARTDATE = "2020-01-01 00:00:00"
 STARTTIME = time.mktime(time.strptime(STARTDATE, "%Y-%m-%d %H:%M:%S"))
 
-
 oor = """"Totaal onderliggende doodsoorzaken (aantal)";
          "1 Infectieuze en parasitaire ziekten/Totaal infectieuze en parasitaire zktn (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.1 Tuberculose (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.2 Meningokokkeninfecties (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.3 Virale hepatitis (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.4 AIDS (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.5 Ov. infectieuze en parasitaire zktn (aantal)";
@@ -139,15 +130,14 @@
          "17 Uitwendige doodsoorzaken/17.3 Moord en doodslag (aantal)";
          "17 Uitwendige doodsoorzaken/17.4 Gebeurtenissen opzet onbekend (aantal)";
          "17 Uitwendige doodsoorzaken/17.5 Overige uitwendige doodsoorzaken (aantal)";
          "18 COVID-19 (Coronavirus ziekte 19)/18 Totaal COVID-19 (Coronavirus 19) (aantal)";
          "18 COVID-19 (Coronavirus ziekte 19)/18.1 Vastgestelde COVID-19 (aantal)";
          "18 COVID-19 (Coronavirus ziekte 19)/18.2 Vermoedelijke COVID-19 (aantal)""".split(";")
 
-
 aantal = """
           168678;
           2974;
           32;
           1;
           34;
           23;
@@ -238,19 +228,14 @@
           28;
           639;
           20173;
           17495;
           2678
          """.split(";")
 
-
-oorzaak = Object()
-copy(oorzaak, zip(oor,aantal))
-
-
 #oorzaak.Suicide = 1859
 
 
 aliases = {}
 aliases["Nieuwvormingen"] = "cancer"
 aliases["Hart en vaatstelsel"] = "hart disease"
 aliases["Psychische en gedragsstoornissen"] = "mental illness"
@@ -266,20 +251,14 @@
 aliases["Bloed, bloedvormende organen"] = "blood disease"
 aliases["Aangeboren afwijkingen"] = "birth defect"
 aliases["Huid en subcutis"] = "skin disease"
 aliases["Zwangerschap"] = "pregnancy"
 aliases["Suicide"] = "suicide"
 
 
-def getalias(txt):
-    for key, value in aliases.items():
-        if txt.lower() in key.lower():
-            return value
-
-
 demo = Object()
 demo.gehandicapten = 2000000
 demo.ggz = 800000
 demo.population = 17440000
 demo.part = 7000000000 / demo.population
 
 
@@ -287,14 +266,15 @@
 jaar["WvGGZ"] = 14206
 jaar["Pvp"] = 20088
 jaar["Wzd"] = 25000
 jaar["Wfz"] = 23820
 jaar["totaal"] = 168678
 
 
+oorzaak = Object(zip(oor, aantal))
 oorzaken = Object()
 
 
 def boot():
     _nr = -1
     for key in keys(oorzaak):
         _nr += 1
@@ -323,32 +303,38 @@
         nms = nms.strip()
         setattr(oorzaken, nms, aantal[_nr])
 
 
 def daily():
     time.sleep(10.0)
     while 1:
-        event = Event()
-        cbnow(event)
+        evt = Event()
+        cbnow(evt)
         time.sleep(24*60*60)
 
 
 def hourly():
     while 1:
         time.sleep(60*60)
-        event = Event()
-        cbnow(event)
+        evt = Event()
+        cbnow(evt)
 
 
 def seconds(nrs):
     if not nrs:
         return nrs
     return 60*60*24*365 / float(nrs)
 
 
+def getalias(txt):
+    for key, value in aliases.items():
+        if txt.lower() in key.lower():
+            return value
+
+
 def getday():
     day = datetime.datetime.now()
     day = day.replace(hour=0, minute=0, second=0, microsecond=0)
     return day.timestamp()
 
 
 def getnr(name):
@@ -363,50 +349,49 @@
         if word in k:
             return True
     return False
 
 
 def cbnow(evt):
     delta = time.time() - STARTTIME
-    txt = elapsed(delta) + " "
+    txt = laps(delta) + " "
     for name in sorted(keys(oorzaken), key=lambda x: seconds(getnr(x))):
         needed = seconds(getnr(name))
         if needed > 60*60:
             continue
         nrtimes = int(delta/needed)
         txt += "%s: %s " % (getalias(name), nrtimes)
     txt += " http://genocide.rtfd.io"
-    Listens.announce(txt)
+    Broker.announce(txt)
 
 
 def cbstats(evt):
     name = evt.rest or "Psych"
     needed = seconds(getnr(name))
     if needed:
         delta = time.time() - STARTTIME
         nrtimes = int(delta/needed)
         nryear = int(YEAR/needed)
         nrday = int(DAY/needed)
         delta2 = time.time() - getday()
         thisday = int(delta2/needed)
-        #onday = (24*60*60/needed)
         txt = "patient #%s died from %s (%s/%s) every %s (%s/year)" % (
                                                                nrtimes,
                                                                getalias(name),
                                                                thisday,
                                                                nrday,
-                                                               elapsed(needed),
+                                                               laps(needed),
                                                                nryear,
                                                               )
-        Listens.announce(txt)
+        Broker.announce(txt)
 
 
 def now(event):
     delta = time.time() - STARTTIME
-    txt = elapsed(delta) + " "
+    txt = laps(delta) + " "
     for name in sorted(keys(oorzaken), key=lambda x: seconds(getnr(x))):
         needed = seconds(getnr(name))
         if needed > 60*60:
             continue
         nrtimes = int(delta/needed)
         txt += "%s: %s " % (getalias(name), nrtimes)
     txt += " http://genocide.rtfd.io"
@@ -424,29 +409,29 @@
         thisday = int(DAY % needed)
         txt = "patient #%s died from %s (%s/%s/%s) every %s" % (
                                                                nrtimes,
                                                                getalias(name),
                                                                thisday,
                                                                nrday,
                                                                nryear,
-                                                               elapsed(needed)
+                                                               laps(needed)
                                                               )
         event.reply(txt)
 
 
 def tpc(event):
-    txt = "%ss " % elapsed(time.time() - STARTTIME)
+    txt = "%ss " % laps(time.time() - STARTTIME)
     for name in sorted(oorzaken, key=lambda x: seconds(getnr(x))):
         needed = seconds(getnr(name))
         delta = time.time() - STARTTIME
         nrtimes = int(delta/needed)
         if needed > 60*60:
             continue
         txt += "%s %s " % (getalias(name), nrtimes)
-    for bot in Listens.objs:
+    for bot in Broker.objs:
         try:
             for channel in bot.channels:
                 bot.topic(channel, txt)
         except AttributeError:
             pass
```

### Comparing `sbn-12/sbn/modules/req.py` & `sbn-20/sbn/modules/req.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C0114,C0115,C0116
+# pylint: disable=C,I,R
 
 
 """| **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
@@ -75,9 +75,12 @@
 
 
 (1) provided are the confirmation letters of both the chamber and the king.
 (2) your reference: OTP-CR-117/19
 """
 
 
+__author__ = "Bart Thate <programmingobject@gmail.com>"
+
+
 def req(event):
     event.reply(__doc__)
```

### Comparing `sbn-12/sbn/modules/rss.py` & `sbn-20/sbn/modules/rss.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=E0012,R,C0114,C0115,C0116,C0209,W0613,E1101
+# pylint: disable=C,I,R,W0401
 
 
-"rich site syndicate"
+"rich site syndicte"
+
+
+__author__ = "Bart Thate <programmingobject@gmail.com>"
 
 
 import html.parser
 import re
 import threading
 import time
 import urllib
@@ -15,71 +18,75 @@
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 from urllib.request import Request, urlopen
 
 
-from ..listens import Listens
-from ..objects import Object, update
-from ..objfunc import prt
-from ..persist import Persist, last, write
-from ..repeats import Repeater
-from ..runtime import Cfg, launch, threaded
-from ..utility import elapsed, fntime, spl
+from .. import Broker, Cfg, Object, Repeater
+from .. import find, fntime, laps, prt, update, write
+from .. import launch, last, spl
 
 
 def start():
+    time.sleep(15.0)
     fetcher = Fetcher()
     fetcher.start()
     return fetcher
 
 
 fetchlock = _thread.allocate_lock()
 
 
 class Feed(Object):
 
-    pass
+    def len(self):
+        return len(self.__dict__)
+
+    def size(self):
+        return len(self.__dict__)
 
 
 class Rss(Object):
 
     def __init__(self):
         super().__init__()
         self.display_list = 'title,link,author'
         self.name = ''
         self.rss = ''
 
+    def len(self):
+        return len(self.__dict__)
 
-Persist.add(Rss)
+    def size(self):
+        return len(self.__dict__)
 
 
 class Seen(Object):
 
     def __init__(self):
         super().__init__()
         self.urls = []
 
+    def len(self):
+        return len(self.__dict__)
 
-Persist.add(Seen)
+    def size(self):
+        return len(self.__dict__)
 
 
 class Fetcher(Object):
 
     dosave = False
     seen = Seen()
 
     def __init__(self):
         super().__init__()
         self.connected = threading.Event()
 
-    def clone(self, other):
-        pass
-
     @staticmethod
     def display(obj):
         result = ''
         displaylist = []
         try:
             displaylist = obj.display_list or 'title,link'
         except AttributeError:
@@ -104,42 +111,38 @@
             for obj in reversed(list(getfeed(feed.rss, feed.display_list))):
                 fed = Feed()
                 update(fed, obj)
                 update(fed, feed)
                 if 'link' in fed:
                     url = urllib.parse.urlparse(fed.link)
                     if url.path and not url.path == '/':
-                        uurl = '%s://%s/%s' % (
-                                               url.scheme,
-                                               url.netloc,
-                                               url.path
-                                              )
+                        uurl = f'{url.scheme}://{url.netloc}/{url.path}'
                     else:
                         uurl = fed.link
                     if uurl in Fetcher.seen.urls:
                         continue
                     Fetcher.seen.urls.append(uurl)
                 counter += 1
                 if self.dosave:
                     write(fed)
                 objs.append(fed)
         if objs:
             write(Fetcher.seen)
         txt = ''
         feedname = getattr(feed, 'name')
         if feedname:
-            txt = '[%s] ' % feedname
+            txt = f'[{feedname}] '
         for obj in objs:
             txt2 = txt + self.display(obj)
-            Listens.announce(txt2.rstrip())
+            Broker.announce(txt2.rstrip())
         return counter
 
     def run(self):
         thrs = []
-        for feed in Persist.find('rss'):
+        for feed in find('rss'):
             thrs.append(launch(self.fetch, feed))
         return thrs
 
     def start(self, repeat=True):
         last(Fetcher.seen)
         if repeat:
             repeater = Repeater(300.0, self.run)
@@ -148,16 +151,16 @@
 
 class Parser(Object):
 
     @staticmethod
     def getitem(line, item):
         lne = ''
         try:
-            index1 = line.index('<%s>' % item) + len(item) + 2
-            index2 = line.index('</%s>' % item)
+            index1 = line.index(f'<{item}>') + len(item) + 2
+            index2 = line.index(f'</{item}>')
             lne = line[index1:index2]
             if 'CDATA' in lne:
                 lne = lne.replace('![CDATA[', '')
                 lne = lne.replace(']]', '')
                 lne = lne[1:-1]
         except ValueError:
             lne = None
@@ -171,17 +174,14 @@
             obj = Object()
             for itm in spl(item):
                 setattr(obj, itm, Parser.getitem(line, itm))
             res.append(obj)
         return res
 
 
-# UTILITIES
-
-
 def getfeed(url, item):
     if Cfg.debug:
         return [Object(), Object()]
     try:
         result = geturl(url)
     except (ValueError, HTTPError, URLError):
         return [Object(), Object()]
@@ -227,30 +227,26 @@
     return html.unescape(txt)
 
 
 def useragent(txt):
     return 'Mozilla/5.0 (X11; Linux x86_64) ' + txt
 
 
-# COMMANDS
-
-
 def dpl(event):
     if len(event.args) < 2:
         event.reply('dpl <stringinurl> <item1,item2>')
         return
     setter = {'display_list': event.args[1]}
-    for feed in Persist.find('rss', {'rss': event.args[0]}):
+    for feed in find('rss', {'rss': event.args[0]}):
         if feed:
             update(feed, setter)
             write(feed)
     event.reply('ok')
 
 
-@threaded
 def ftc(event):
     res = []
     thrs = []
     fetcher = Fetcher()
     fetcher.start(False)
     thrs = fetcher.run()
     for thr in thrs:
@@ -261,53 +257,49 @@
 
 
 def nme(event):
     if len(event.args) != 2:
         event.reply('name <stringinurl> <name>')
         return
     selector = {'rss': event.args[0]}
-    for feed in Persist.find('rss', selector):
+    for feed in find('rss', selector):
         if feed:
             feed.name = event.args[1]
             write(feed)
     event.reply('ok')
 
 
 def rem(event):
     if len(event.args) != 1:
         event.reply('rem <stringinurl>')
         return
     selector = {'rss': event.args[0]}
-    for feed in Persist.find('rss', selector):
+    for feed in find('rss', selector):
         if feed:
             feed.__deleted__ = True
             write(feed)
     event.reply('ok')
 
 
 def rss(event):
     if not event.rest:
         nrs = 0
-        for feed in Persist.find('rss'):
-            event.reply(
-                        '%s %s %s' % (
-                                      nrs,
-                                      prt(feed),
-                                      elapsed(time.time()-fntime(feed.__oid__))
-                                     )
-                       )
+        for feed in find('rss'):
+            elp = laps(time.time()-fntime(feed.__oid__))
+            txt = prt(feed)
+            event.reply(f'{nrs} {txt} {elp}')
             nrs += 1
         if not nrs:
             event.reply('no rss feed found.')
         return
     url = event.args[0]
     if 'http' not in url:
         event.reply('i need an url')
         return
-    for res in Persist.find('rss', {'rss': url}):
+    for res in find('rss', {'rss': url}):
         if res:
-            event.reply('already got %s' % url)
+            event.reply(f'already got {url}')
             return
     feed = Rss()
     feed.rss = event.args[0]
     write(feed)
     event.reply('ok')
```

### Comparing `sbn-12/sbn/modules/tdo.py` & `sbn-20/sbn/modules/shp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=R,C0114,C0115,C0116
+# pylint: disable=C,I,R
 
 
-"maintain todo list"
+"shopping list"
+
+
+__author__ = "Bart Thate <programmingobject@gmail.com>"
 
 
 import time
 
 
-from ..objects import Object
-from ..persist import Persist, write
-from ..utility import elapsed, fntime
+from .. import Cfg, Object 
+from .. import find, fntime, laps, write
 
 
-class Todo(Object):
+class Shop(Object):
 
     def __init__(self):
         super().__init__()
         self.txt = ''
 
+    def size(self):
+        return len(self.__dict__)
 
-Persist.add(Todo)
-
-
-# COMMANDS
+    def length(self):
+        return len(self.__dict__)
 
 
-def dne(event):
+def got(event):
     if not event.args:
         return
     selector = {'txt': event.args[0]}
-    for obj in Persist.find('todo', selector):
+    for obj in find('shop', selector):
         obj.__deleted__ = True
         write(obj)
-        event.reply('ok')
-        break
+        event.reply('ok') # okdan
 
 
-def tdo(event):
+def shp(event):
     if not event.rest:
         nmr = 0
-        for obj in Persist.find('todo'):
-            lap = elapsed(time.time()-fntime(obj.__oid__))
+        for obj in find(Cfg.workdir, 'shop'):
+            lap = laps(time.time()-fntime(obj.__oid__))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
-            event.reply("no todo")
+            event.reply("no shops")
         return
-    obj = Todo()
+    obj = Shop()
     obj.txt = event.rest
     write(obj)
     event.reply('ok')
```

### Comparing `sbn-12/sbn/modules/udp.py` & `sbn-20/sbn/modules/udp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,65 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C0103,C0115,C0116,W0613,R0903
+# pylint: disable=C,I,R
 
 
 "udp to irc relay"
 
 
+__author__ = "Bart Thate <programmingobject@gmail.com>"
+
+
 import select
 import socket
 import sys
 import time
 
 
-from ..listens import Listens
-from ..objects import Object
-from ..persist import Persist, last
-from ..runtime import launch
+from .. import Broker, Object
+from .. import last, launch
 
 
 def start():
-    u = UDP()
-    u.start()
-    return u
+    udpd = UDP()
+    udpd.start()
+    return udpd
 
 
 class Cfg(Object):
 
     def __init__(self):
         super().__init__()
         self.host = "localhost"
         self.port = 5500
 
+    def len(self):
+        return self.server
 
-Persist.add(Cfg)
+    def size(self):
+        return self.port
 
 
 class UDP(Object):
 
     def __init__(self):
         super().__init__()
         self.stopped = False
         self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
         self._sock.setblocking(1)
         self._starttime = time.time()
         self.cfg = Cfg()
+        self.cfg.addr = ""
 
-    def output(self, txt, addr):
-        Listens.announce(txt.replace("\00", ""))
+    def output(self, txt, addr=None):
+        if addr:
+            self.cfg.addr = addr
+        Broker.announce(txt.replace("\00", ""))
 
     def server(self):
         try:
             self._sock.bind((self.cfg.host, self.cfg.port))
         except socket.gaierror:
             return
         while not self.stopped:
@@ -84,23 +91,26 @@
     last(cfg)
     if len(sys.argv) > 2:
         txt = " ".join(sys.argv[2:])
         toudp(cfg.host, cfg.port, txt)
         return
     if not select.select([sys.stdin, ], [], [], 0.0)[0]:
         return
+    size = 0
     while 1:
         try:
-            (i, _o, e) = select.select([sys.stdin,], [], [sys.stderr,])
+            (inp, _out, err) = select.select([sys.stdin,], [], [sys.stderr,])
         except KeyboardInterrupt:
             return
-        if e:
+        if err:
             break
         stop = False
-        for sock in i:
+        for sock in inp:
             txt = sock.readline()
             if not txt:
                 stop = True
                 break
+            size += len(txt)
             toudp(cfg.host, cfg.port, txt)
         if stop:
             break
+    event.reply(f"send {size}")
```

### Comparing `sbn-12/sbn/modules/wsd.py` & `sbn-20/sbn/modules/wsd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,I,R,E0401
+# pylint: disable=C,I,R
 
 
 """| wijsheid, wijs !
 
 | OVERDRACHT
 | ==========
 
@@ -182,16 +182,15 @@
 | twee eieren (gemeente huis en buiging naar west)
 | vreedevernoeming
 | duiding
 | coding
 """
 
 
-__author__ = "B.H.J. Thate <thatebhj@gmail.com>"
-__version__ = 1
+__author__ = "Bart Thate <programmingobject@gmail.com>"
 
 
 import random
 
 
 def wsd(event):
     event.reply(random.choice(__doc__.split("\n")).strip()[2:])
```

### Comparing `sbn-12/sbn/objects.py` & `sbn-20/sbn/utility.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,101 +1,99 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=E0012,R,C0114,C0115,C0116,C0209,W0613,E1101
+# pylint: disable=C,I,R
 
 
-"clean namespace"
+"utilities"
 
 
-import datetime
-import os
-import uuid
-
-
-def __dir__():
-    return (
-            'Object',
-            'copy',
-            'dumprec',
-            'ident',
-            'items',
-            'keys',
-            'kind',
-            'update',
-            'values'
-           )
-
-
-class Object:
-
-    __slots__ = ('__dict__', '__oid__')
-
-    def __init__(self):
-        self.__oid__ = ident(self)
-
-    def __iter__(self):
-        return iter(self.__dict__)
-
-    def __len__(self):
-        return len(self.__dict__)
-
-    def __str__(self):
-        return dumprec(self)
-
-
-def copy(obj, val) -> None:
-    if isinstance(val, list):
-        update(obj, dict(val))
-    elif isinstance(val, zip):
-        update(obj, dict(val))
-    elif isinstance(val, dict):
-        update(obj, val)
-    elif isinstance(val, Object):
-        update(obj, vars(val))
-    return obj
+__author__ = "Bart Thate <programmingobject@gmail.com>"
 
 
-def dumprec(obj, ooo="{"):
-    for key, value in items(obj):
-        if issubclass(type(value), Object):
-            ooo += "'%s': %s" % (str(key), dumprec(value, ooo))
-            continue
-        else:
-            ooo += "'%s': '%s'" % (str(key), str(value))
-    ooo += "}"
-    return ooo
-
-
-def ident(obj) -> str:
-    return os.path.join(
-                        kind(obj),
-                        str(uuid.uuid4().hex),
-                        os.sep.join(str(datetime.datetime.now()).split())
-                       )
-
-
-def items(obj) -> []:
-    if isinstance(obj, type({})):
-        return obj.items()
-    return obj.__dict__.items()
-
-
-def keys(obj) -> []:
-    return obj.__dict__.keys()
-
-
-def kind(obj) -> str:
-    kin = str(type(obj)).split()[-1][1:-2]
-    if kin == "type":
-        kin = obj.__name__
-    return kin
-
-
-def update(obj, data, empty=True) -> None:
-    for key, value in items(data):
-        if not empty and not value:
-            continue
-        setattr(obj, key, value)
+import os
+import pathlib
+import time
+import types
+
+
+def banner(names, version):
+    times = time.ctime(time.time())
+    return f"{names.upper()} {version} {times}"
+
+
+def cdir(pth) -> None:
+    if not pth.endswith(os.sep):
+        pth = os.path.dirname(pth)
+    pth = pathlib.Path(pth)
+    os.makedirs(pth, exist_ok=True)
+
+
+def laps(seconds, short=True) -> str:
+    txt = ""
+    nsec = float(seconds)
+    if nsec < 1:
+        return f"{nsec:.2f}s"
+    year = 365*24*60*60
+    week = 7*24*60*60
+    nday = 24*60*60
+    hour = 60*60
+    minute = 60
+    years = int(nsec/year)
+    nsec -= years*year
+    weeks = int(nsec/week)
+    nsec -= weeks*week
+    nrdays = int(nsec/nday)
+    nsec -= nrdays*nday
+    hours = int(nsec/hour)
+    nsec -= hours*hour
+    minutes = int(nsec/minute)
+    nsec -= int(minute*minutes)
+    sec = int(nsec)
+    if years:
+        txt += f"{years}y"
+    if weeks:
+        nrdays += weeks * 7
+    if nrdays:
+        txt += f"{nrdays}d"
+    if years and short and txt:
+        return txt.strip()
+    if hours:
+        txt += f"{hours}h"
+    if minutes:
+        txt += f"{minutes}m"
+    if sec:
+        txt += f"{sec}s"
+    txt = txt.strip()
+    return txt
+
+
+def name(obj) -> str:
+    typ = type(obj)
+    if isinstance(typ, types.ModuleType):
+        return obj.__name__
+    if '__self__' in dir(obj):
+        clz = obj.__self__.__class__.__name__
+        nme = obj.__name__
+        return f'{clz}.{nme}'
+    if '__class__' in dir(obj) and '__name__' in dir(obj):
+        clz = obj.__class__.__name__
+        nme = obj.__name__
+        return f'{clz}.{nme}'
+    if '__class__' in dir(obj):
+        return obj.__class__.__name__
+    if '__name__' in dir(obj):
+        clz = obj.__class__.__name__
+        nme = obj.__name__
+        return f'{clz}.{nme}'
+    return None
+
+
+def spl(txt) -> []:
+    try:
+        res = txt.split(',')
+    except (TypeError, ValueError):
+        res = txt
+    return [x for x in res if x]
 
 
-def values(obj) -> []:
-    return obj.__dict__.values()
+def strip(path) -> str:
+    return os.sep.join(path.split(os.sep)[-4:])
```

### Comparing `sbn-12/sbn/parsers.py` & `sbn-20/sbn/parsers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,56 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=R,C0114,C0116
-# pylama: ignore=C901
+# pylint: disable=C,I,R
 
 
-"parse text for command"
+"parse events"
 
 
-from .default import Default
-from .utility import spl
+__author__ = "Bart Thate <programmingobject@gmail.com>"
 
 
 def __dir__():
     return (
-            'parse',
+            "parse",
            )
 
 
+__all__ = __dir__()
+
+
 def parse(obj, txt):
-    obj.otxt = txt
-    splitted = obj.otxt.split()
-    args = []
-    _nr = -1
-    for word in splitted:
-        if word.startswith('-'):
-            if not obj.index:
-                obj.index = 0
+    obj.cmd = obj.cmd or ""
+    obj.args = obj.args or []
+    obj.gets = obj.gets or {}
+    obj.mod = obj.mod or ""
+    obj.opts = obj.opts or ""
+    obj.otxt = txt or ""
+    obj.rest = obj.rest or ""
+    obj.sets = obj.sets or {}
+    for spli in txt.split():
+        if spli.startswith("-"):
             try:
-                obj.index = int(word[1:])
+                obj.index = int(spli[1:])
             except ValueError:
-                if not obj.opts:
-                    obj.opts = ""
-                obj.opts = obj.opts + word[1:]
+                obj.opts += spli[1:]
             continue
-        try:
-            key, value = word.split('==')
-            if not obj.skip:
-                obj.skip = Default()
-            if value.endswith('-'):
-                value = value[:-1]
-                setattr(obj.skip, value, '')
-            if not obj.gets:
-                obj.gets = Default()
-            setattr(obj.gets, key, value)
-            continue
-        except ValueError:
-            pass
-        try:
-            key, value = word.split('=')
+        if "=" in spli:
+            key, value = spli.split("=", maxsplit=1)
             if key == "mod":
-                if not obj.mod:
-                    obj.mod = ""
-                for val in spl(value):
-                    if val not in obj.mods:
-                        obj.mods += f",{val}"
+                obj.mod += "," + value
                 continue
-            if not obj.sets:
-                obj.sets = Default()
-            setattr(obj.sets, key, value)
+            obj.sets[key] = value
+            continue
+        if "==" in spli:
+            key, value = spli.split("==", maxsplit=1)
+            obj.gets[key] = value
             continue
-        except ValueError:
-            pass
-        _nr += 1
-        if _nr == 0:
-            obj.cmd = word
+        if not obj.cmd:
+            obj.cmd = spli
             continue
-        args.append(word)
-    if args:
-        obj.args = args
-        obj.rest = ' '.join(args)
-        obj.txt = obj.cmd + ' ' + obj.rest
-    else:
-        obj.txt = obj.cmd
+        obj.args.append(spli)
+    obj.txt = obj.cmd
+    if obj.args:
+        obj.rest = str(" ".join(obj.args))
+        if obj.rest:
+            obj.txt += " " + obj.rest
```

### Comparing `sbn-12/sbn.egg-info/PKG-INFO` & `sbn-20/sbn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbn
-Version: 12
+Version: 20
 Summary: Skull, Bones and Number (OTP-CR-117/19)
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/sbn
 Project-URL: bugs, https://github.com/bthate/sbn/issues
 Project-URL: source, https://github.com/bthate/sbn
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sbn-12/sbn.egg-info/SOURCES.txt` & `sbn-20/sbn.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.rst
 pyproject.toml
 setup.py
+bin/sbn
 files/ECHAabilify.png
 files/ECHAclozapine.png
 files/ECHAhaldol.png
 files/ECHAzyprexa.png
 files/bevestigd.jpg
 files/informed.jpg
 files/skull3.png
@@ -13,56 +14,43 @@
 pdf/EM_T07_OTP-CR-117_19_001.pdf
 pdf/Elements-of-Crimes.pdf
 pdf/Kamer.pdf
 pdf/Rome-Statute.pdf
 pdf/Rules-of-Procedure-and-Evidence.pdf
 pdf/bevestigd.pdf
 sbn/__init__.py
-sbn/__main__.py
-sbn/clients.py
-sbn/clocked.py
+sbn/brokers.py
 sbn/command.py
 sbn/configs.py
 sbn/decoder.py
-sbn/default.py
-sbn/defines.py
 sbn/encoder.py
 sbn/errored.py
 sbn/evented.py
-sbn/handler.py
-sbn/listens.py
-sbn/logging.py
+sbn/locking.py
+sbn/loggers.py
 sbn/objects.py
-sbn/objfunc.py
 sbn/parsers.py
 sbn/persist.py
+sbn/reactor.py
+sbn/recurse.py
 sbn/repeats.py
-sbn/runtime.py
 sbn/threads.py
 sbn/utility.py
 sbn.egg-info/PKG-INFO
 sbn.egg-info/SOURCES.txt
 sbn.egg-info/dependency_links.txt
-sbn.egg-info/entry_points.txt
 sbn.egg-info/requires.txt
 sbn.egg-info/top_level.txt
 sbn.egg-info/zip-safe
 sbn/modules/__init__.py
-sbn/modules/cfg.py
-sbn/modules/cmd.py
-sbn/modules/err.py
-sbn/modules/flt.py
-sbn/modules/fnd.py
+sbn/modules/bsc.py
 sbn/modules/irc.py
 sbn/modules/log.py
 sbn/modules/mbx.py
 sbn/modules/mdl.py
-sbn/modules/mod.py
 sbn/modules/req.py
-sbn/modules/rld.py
 sbn/modules/rss.py
-sbn/modules/sts.py
+sbn/modules/shp.py
 sbn/modules/tdo.py
-sbn/modules/thr.py
 sbn/modules/udp.py
-sbn/modules/upt.py
-sbn/modules/wsd.py
+sbn/modules/wsd.py
+sbn/modules/wsh.py
```

