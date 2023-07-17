# Comparing `tmp/metarace-2.1.2.tar.gz` & `tmp/metarace-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metarace-2.1.2.tar", last modified: Wed Jun 28 13:21:45 2023, max compression
+gzip compressed data, was "metarace-2.1.3.tar", last modified: Mon Jul 17 05:28:52 2023, max compression
```

## Comparing `metarace-2.1.2.tar` & `metarace-2.1.3.tar`

### file list

```diff
@@ -1,46 +1,44 @@
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-28 13:21:45.296258 metarace-2.1.2/
--rw-------   0 ndf       (1000) ndf       (1000)     1092 2022-01-22 06:38:57.000000 metarace-2.1.2/LICENSE
--rw-r--r--   0 ndf       (1000) ndf       (1000)       28 2022-05-31 01:20:37.000000 metarace-2.1.2/MANIFEST.in
--rw-r--r--   0 ndf       (1000) ndf       (1000)     4762 2023-06-28 13:21:45.296258 metarace-2.1.2/PKG-INFO
--rw-------   0 ndf       (1000) ndf       (1000)     4243 2023-06-28 01:33:45.000000 metarace-2.1.2/README.md
--rw-r--r--   0 ndf       (1000) ndf       (1000)      753 2023-06-28 13:21:14.000000 metarace-2.1.2/pyproject.toml
--rw-r--r--   0 ndf       (1000) ndf       (1000)       38 2023-06-28 13:21:45.296258 metarace-2.1.2/setup.cfg
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-28 13:21:45.284257 metarace-2.1.2/src/
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-28 13:21:45.292257 metarace-2.1.2/src/metarace/
--rw-r--r--   0 ndf       (1000) ndf       (1000)     9466 2023-06-28 13:21:28.000000 metarace-2.1.2/src/metarace/__init__.py
--rw-------   0 ndf       (1000) ndf       (1000)     4268 2023-06-25 00:11:43.000000 metarace-2.1.2/src/metarace/countback.py
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-28 13:21:45.292257 metarace-2.1.2/src/metarace/data/
--rw-------   0 ndf       (1000) ndf       (1000)     3067 2022-01-22 22:18:40.000000 metarace-2.1.2/src/metarace/data/IOC_Codes.csv
--rw-r--r--   0 ndf       (1000) ndf       (1000)        0 2023-06-28 11:57:11.000000 metarace-2.1.2/src/metarace/data/__init__.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.2/src/metarace/data/bg_armfin.svg
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.2/src/metarace/data/bg_armint.svg
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.2/src/metarace/data/bg_armstart.svg
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.2/src/metarace/data/bg_idle.svg
--rw-r--r--   0 ndf       (1000) ndf       (1000)     2369 2022-01-22 22:18:40.000000 metarace-2.1.2/src/metarace/data/bg_src.svg
--rw-------   0 ndf       (1000) ndf       (1000)      520 2023-06-05 02:11:31.000000 metarace-2.1.2/src/metarace/data/metarace.json
--rw-------   0 ndf       (1000) ndf       (1000)     8729 2022-01-22 22:18:40.000000 metarace-2.1.2/src/metarace/data/metarace_icon.svg
--rw-------   0 ndf       (1000) ndf       (1000)     2048 2023-06-05 01:23:26.000000 metarace-2.1.2/src/metarace/data/pdf_template.json
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-28 13:21:45.296258 metarace-2.1.2/src/metarace/decoder/
--rw-r--r--   0 ndf       (1000) ndf       (1000)     5730 2023-05-31 00:29:16.000000 metarace-2.1.2/src/metarace/decoder/__init__.py
--rw-------   0 ndf       (1000) ndf       (1000)    15284 2023-06-27 08:32:43.000000 metarace-2.1.2/src/metarace/decoder/rrs.py
--rw-------   0 ndf       (1000) ndf       (1000)    27311 2023-06-27 08:32:09.000000 metarace-2.1.2/src/metarace/decoder/rru.py
--rw-------   0 ndf       (1000) ndf       (1000)    18916 2023-06-27 13:14:15.000000 metarace-2.1.2/src/metarace/decoder/thbc.py
--rw-------   0 ndf       (1000) ndf       (1000)    11424 2023-06-25 00:11:28.000000 metarace-2.1.2/src/metarace/eventdb.py
--rw-------   0 ndf       (1000) ndf       (1000)     3733 2023-05-31 00:53:46.000000 metarace-2.1.2/src/metarace/export.py
--rw-------   0 ndf       (1000) ndf       (1000)     8787 2023-06-25 00:11:12.000000 metarace-2.1.2/src/metarace/gemini.py
--rw-------   0 ndf       (1000) ndf       (1000)     5970 2023-06-28 00:17:21.000000 metarace-2.1.2/src/metarace/htlib.py
--rw-------   0 ndf       (1000) ndf       (1000)     5636 2023-06-25 00:10:49.000000 metarace-2.1.2/src/metarace/jsonconfig.py
--rw-------   0 ndf       (1000) ndf       (1000)   199422 2023-06-28 00:18:10.000000 metarace-2.1.2/src/metarace/report.py
--rw-------   0 ndf       (1000) ndf       (1000)    24615 2023-06-24 14:16:56.000000 metarace-2.1.2/src/metarace/riderdb.py
--rw-------   0 ndf       (1000) ndf       (1000)    10274 2023-06-25 00:10:28.000000 metarace-2.1.2/src/metarace/sender.py
--rw-------   0 ndf       (1000) ndf       (1000)    17918 2023-06-25 00:09:45.000000 metarace-2.1.2/src/metarace/strops.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)    13652 2022-11-14 06:21:05.000000 metarace-2.1.2/src/metarace/telegraph.py
--rw-------   0 ndf       (1000) ndf       (1000)    15088 2023-06-04 10:37:01.000000 metarace-2.1.2/src/metarace/timy.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)    20914 2023-06-25 00:08:46.000000 metarace-2.1.2/src/metarace/tod.py
--rw-------   0 ndf       (1000) ndf       (1000)     4485 2023-06-25 00:09:26.000000 metarace-2.1.2/src/metarace/unt4.py
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-06-28 13:21:45.292257 metarace-2.1.2/src/metarace.egg-info/
--rw-r--r--   0 ndf       (1000) ndf       (1000)     4762 2023-06-28 13:21:45.000000 metarace-2.1.2/src/metarace.egg-info/PKG-INFO
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1015 2023-06-28 13:21:45.000000 metarace-2.1.2/src/metarace.egg-info/SOURCES.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)        1 2023-06-28 13:21:45.000000 metarace-2.1.2/src/metarace.egg-info/dependency_links.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)       67 2023-06-28 13:21:45.000000 metarace-2.1.2/src/metarace.egg-info/requires.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)        9 2023-06-28 13:21:45.000000 metarace-2.1.2/src/metarace.egg-info/top_level.txt
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-17 05:28:52.642412 metarace-2.1.3/
+-rw-------   0 ndf       (1000) ndf       (1000)     1092 2023-07-11 12:51:50.000000 metarace-2.1.3/LICENSE
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       28 2022-05-31 01:20:37.000000 metarace-2.1.3/MANIFEST.in
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     4490 2023-07-17 05:28:52.638412 metarace-2.1.3/PKG-INFO
+-rw-------   0 ndf       (1000) ndf       (1000)     3921 2023-07-11 12:41:25.000000 metarace-2.1.3/README.md
+-rw-r--r--   0 ndf       (1000) ndf       (1000)      798 2023-07-17 05:27:44.000000 metarace-2.1.3/pyproject.toml
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       38 2023-07-17 05:28:52.642412 metarace-2.1.3/setup.cfg
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-17 05:28:52.630412 metarace-2.1.3/src/
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-17 05:28:52.634412 metarace-2.1.3/src/metarace/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     9422 2023-07-17 03:19:05.000000 metarace-2.1.3/src/metarace/__init__.py
+-rw-------   0 ndf       (1000) ndf       (1000)     4268 2023-06-25 00:11:43.000000 metarace-2.1.3/src/metarace/countback.py
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-17 05:28:52.638412 metarace-2.1.3/src/metarace/data/
+-rw-------   0 ndf       (1000) ndf       (1000)     3067 2022-01-22 22:18:40.000000 metarace-2.1.3/src/metarace/data/IOC_Codes.csv
+-rw-r--r--   0 ndf       (1000) ndf       (1000)        0 2023-06-28 11:57:11.000000 metarace-2.1.3/src/metarace/data/__init__.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.3/src/metarace/data/bg_armfin.svg
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.3/src/metarace/data/bg_armint.svg
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.3/src/metarace/data/bg_armstart.svg
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.3/src/metarace/data/bg_idle.svg
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     2369 2022-01-22 22:18:40.000000 metarace-2.1.3/src/metarace/data/bg_src.svg
+-rw-------   0 ndf       (1000) ndf       (1000)        4 2023-07-11 12:42:36.000000 metarace-2.1.3/src/metarace/data/metarace.json
+-rw-------   0 ndf       (1000) ndf       (1000)     8729 2022-01-22 22:18:40.000000 metarace-2.1.3/src/metarace/data/metarace_icon.svg
+-rw-------   0 ndf       (1000) ndf       (1000)     2048 2023-06-05 01:23:26.000000 metarace-2.1.3/src/metarace/data/pdf_template.json
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-17 05:28:52.638412 metarace-2.1.3/src/metarace/decoder/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     5721 2023-07-13 12:30:30.000000 metarace-2.1.3/src/metarace/decoder/__init__.py
+-rw-------   0 ndf       (1000) ndf       (1000)    16233 2023-07-13 12:30:42.000000 metarace-2.1.3/src/metarace/decoder/rrs.py
+-rw-------   0 ndf       (1000) ndf       (1000)    32727 2023-07-13 12:35:31.000000 metarace-2.1.3/src/metarace/decoder/rru.py
+-rw-------   0 ndf       (1000) ndf       (1000)    25107 2023-07-17 04:57:46.000000 metarace-2.1.3/src/metarace/decoder/thbc.py
+-rw-------   0 ndf       (1000) ndf       (1000)    11415 2023-07-13 12:29:27.000000 metarace-2.1.3/src/metarace/eventdb.py
+-rw-------   0 ndf       (1000) ndf       (1000)     6290 2023-07-13 12:29:44.000000 metarace-2.1.3/src/metarace/export.py
+-rw-------   0 ndf       (1000) ndf       (1000)     5970 2023-06-28 00:17:21.000000 metarace-2.1.3/src/metarace/htlib.py
+-rw-------   0 ndf       (1000) ndf       (1000)    12251 2023-07-13 12:30:06.000000 metarace-2.1.3/src/metarace/jsonconfig.py
+-rw-------   0 ndf       (1000) ndf       (1000)   204351 2023-07-13 12:29:15.000000 metarace-2.1.3/src/metarace/report.py
+-rw-------   0 ndf       (1000) ndf       (1000)    25632 2023-07-16 01:35:36.000000 metarace-2.1.3/src/metarace/riderdb.py
+-rw-------   0 ndf       (1000) ndf       (1000)    17918 2023-06-25 00:09:45.000000 metarace-2.1.3/src/metarace/strops.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    14783 2023-07-13 12:28:46.000000 metarace-2.1.3/src/metarace/telegraph.py
+-rw-------   0 ndf       (1000) ndf       (1000)    16903 2023-07-15 05:11:51.000000 metarace-2.1.3/src/metarace/timy.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    20994 2023-07-13 12:27:42.000000 metarace-2.1.3/src/metarace/tod.py
+-rw-------   0 ndf       (1000) ndf       (1000)     4485 2023-06-25 00:09:26.000000 metarace-2.1.3/src/metarace/unt4.py
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-17 05:28:52.638412 metarace-2.1.3/src/metarace.egg-info/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     4490 2023-07-17 05:28:52.000000 metarace-2.1.3/src/metarace.egg-info/PKG-INFO
+-rw-r--r--   0 ndf       (1000) ndf       (1000)      969 2023-07-17 05:28:52.000000 metarace-2.1.3/src/metarace.egg-info/SOURCES.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)        1 2023-07-17 05:28:52.000000 metarace-2.1.3/src/metarace.egg-info/dependency_links.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       67 2023-07-17 05:28:52.000000 metarace-2.1.3/src/metarace.egg-info/requires.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)        9 2023-07-17 05:28:52.000000 metarace-2.1.3/src/metarace.egg-info/top_level.txt
```

### Comparing `metarace-2.1.2/LICENSE` & `metarace-2.1.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019-2022 Nathan Fraser and contributors
+Copyright (c) 2019-2023 Nathan Fraser and contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `metarace-2.1.2/PKG-INFO` & `metarace-2.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: metarace
-Version: 2.1.2
+Version: 2.1.3
 Summary: Cyclesport results and timing toolkit
 Author-email: Nathan Fraser <ndf-zz@6-v.org>
 License: MIT
 Project-URL: homepage, https://github.com/ndf-zz/metarace
 Keywords: cyclesport,results,timing
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Other/Nonlisted Topic
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # metarace
 
 A collection of Python modules to assist with cycle race timekeeping
@@ -31,33 +32,34 @@
    - [ttstart](https://github.com/ndf-zz/metarace-ttstart) : Time
      Trial starter console.
 
 
 ## Work in Progress
 
    - include grapheme support in strops
-   - update pango text layouts to align vertically by text baseline
-   - re-write report library for better sectioning and dynamic updates
+   - re-write report library for better sectioning
+   - overhaul PDF text rendering
+   - replace xls export with xlsx
    - module documentation
    - sample scripts
 
 
 ## Module Overview
 
 ### metarace: Base Library
 
    - shared configuration, default files and resources
    - tempfile-backed file writer
    - meet folder locking
 
 
-### jsonconfig: Configuration File Wrapper
+### jsonconfig: Configuration Options
 
-A thin wrapper on a dictionary-based configuration
-with JSON export and import.
+Schema defined dictionary-like
+configuration with JSON export and import.
 
 
 ### riderdb: CSV-backed Competitor Information
 
 Store details for competitors, teams, and categories.
 
 
@@ -96,28 +98,14 @@
 
 ### unt4: Legacy Timing Protocol
 
 Swiss Timing UNT4 protocol wrapper, for legacy devices
 and DHI communications.
 
 
-### sender: Legacy DHI Scoreboard Interface
-
-Thread object for drawing text on a
-[Caprica](https://github.com/ndf-zz/caprica)
-or Galactica DHI scoreboard over TCP,
-UDP and serial connections.
-
-
-### gemini: Numeric LED Scoreboard Interface
-
-Thread object for writing to a pair of Swiss Timing Gemini
-numeric LED boards, and lap count displays.
-
-
 ### countback: Accumulate and Compare Count of Places
 
 Represent a countback of places and allow for simple
 placing comparisons.
 
 
 ### htlib: HTML Generation
@@ -128,69 +116,68 @@
 ### report: Report Generation
 
 Create sectioned reports and save to PDF, HTML, XLS and JSON.
 
 
 ### export: Result Export and Mirroring
 
-Execute a process on the host system to
-mirror result files to a remote server,
-or to run a script.
+Mirror export files to a remote host using rsync over ssh,
+rsync TCP daemon or by running a local script.
 
 
 ### eventdb: CSV Event List
 
-Store details for events within a meet.
+Store details for multple events within a meet.
 
 
 ## Requirements
 
 System requirements:
 
    - Python >= 3.9
    - Cairo
    - Pango
    - Rsvg
    - Python gi
    - Python gi-cairo
    - tex-gyre (optional, recommended)
    - evince (optional, recommended)
+   - fonts-noto (optional)
    - mosquitto (optional)
    - libreoffice (optional)
 
 Python packages:
 
    - pyserial: Serial port interface
    - python-dateutil: Generic date/time string parser
    - xlwt: XLS file writer
    - paho-mqtt: MQTT interface
    - grapheme: Unicode grapheme support
 
 
 ## Installation
 
-Check that your python
-version is at least 3.9 before installing. This library will
-not work with python versions less than 3.9.
+Check that your python version is at least 3.9 before installing.
+This library will not work with python versions less than 3.9.
 
 
 ### Debian 11+
 
 Install system requirements with apt:
 
 	$ sudo apt install python3-venv python3-pip python3-cairo python3-gi python3-gi-cairo
 	$ sudo apt install gir1.2-rsvg-2.0 gir1.2-pango-1.0
 	$ sudo apt install python3-serial python3-paho-mqtt python3-dateutil python3-xlwt
 
 Optionally add fonts, PDF viewer and MQTT broker:
 
-	$ sudo apt install tex-gyre evince mosquitto
+	$ sudo apt install tex-gyre fonts-noto evince mosquitto
 
 Create a virtualenv for metarace and associated packages:
 
-	$ python3 -m venv --system-site-packages mrv
+	$ python3 -m venv --system-site-packages venv
 
 Activate the virtualenv and install packages with pip:
 
-	$ source ./mrv/bin/activate
-	(mrv) $ pip3 install metarace
+	$ source ./venv/bin/activate
+	(venv) $ pip3 install metarace
```

### Comparing `metarace-2.1.2/README.md` & `metarace-2.1.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -15,33 +15,34 @@
    - [ttstart](https://github.com/ndf-zz/metarace-ttstart) : Time
      Trial starter console.
 
 
 ## Work in Progress
 
    - include grapheme support in strops
-   - update pango text layouts to align vertically by text baseline
-   - re-write report library for better sectioning and dynamic updates
+   - re-write report library for better sectioning
+   - overhaul PDF text rendering
+   - replace xls export with xlsx
    - module documentation
    - sample scripts
 
 
 ## Module Overview
 
 ### metarace: Base Library
 
    - shared configuration, default files and resources
    - tempfile-backed file writer
    - meet folder locking
 
 
-### jsonconfig: Configuration File Wrapper
+### jsonconfig: Configuration Options
 
-A thin wrapper on a dictionary-based configuration
-with JSON export and import.
+Schema defined dictionary-like
+configuration with JSON export and import.
 
 
 ### riderdb: CSV-backed Competitor Information
 
 Store details for competitors, teams, and categories.
 
 
@@ -80,28 +81,14 @@
 
 ### unt4: Legacy Timing Protocol
 
 Swiss Timing UNT4 protocol wrapper, for legacy devices
 and DHI communications.
 
 
-### sender: Legacy DHI Scoreboard Interface
-
-Thread object for drawing text on a
-[Caprica](https://github.com/ndf-zz/caprica)
-or Galactica DHI scoreboard over TCP,
-UDP and serial connections.
-
-
-### gemini: Numeric LED Scoreboard Interface
-
-Thread object for writing to a pair of Swiss Timing Gemini
-numeric LED boards, and lap count displays.
-
-
 ### countback: Accumulate and Compare Count of Places
 
 Represent a countback of places and allow for simple
 placing comparisons.
 
 
 ### htlib: HTML Generation
@@ -112,69 +99,68 @@
 ### report: Report Generation
 
 Create sectioned reports and save to PDF, HTML, XLS and JSON.
 
 
 ### export: Result Export and Mirroring
 
-Execute a process on the host system to
-mirror result files to a remote server,
-or to run a script.
+Mirror export files to a remote host using rsync over ssh,
+rsync TCP daemon or by running a local script.
 
 
 ### eventdb: CSV Event List
 
-Store details for events within a meet.
+Store details for multple events within a meet.
 
 
 ## Requirements
 
 System requirements:
 
    - Python >= 3.9
    - Cairo
    - Pango
    - Rsvg
    - Python gi
    - Python gi-cairo
    - tex-gyre (optional, recommended)
    - evince (optional, recommended)
+   - fonts-noto (optional)
    - mosquitto (optional)
    - libreoffice (optional)
 
 Python packages:
 
    - pyserial: Serial port interface
    - python-dateutil: Generic date/time string parser
    - xlwt: XLS file writer
    - paho-mqtt: MQTT interface
    - grapheme: Unicode grapheme support
 
 
 ## Installation
 
-Check that your python
-version is at least 3.9 before installing. This library will
-not work with python versions less than 3.9.
+Check that your python version is at least 3.9 before installing.
+This library will not work with python versions less than 3.9.
 
 
 ### Debian 11+
 
 Install system requirements with apt:
 
 	$ sudo apt install python3-venv python3-pip python3-cairo python3-gi python3-gi-cairo
 	$ sudo apt install gir1.2-rsvg-2.0 gir1.2-pango-1.0
 	$ sudo apt install python3-serial python3-paho-mqtt python3-dateutil python3-xlwt
 
 Optionally add fonts, PDF viewer and MQTT broker:
 
-	$ sudo apt install tex-gyre evince mosquitto
+	$ sudo apt install tex-gyre fonts-noto evince mosquitto
 
 Create a virtualenv for metarace and associated packages:
 
-	$ python3 -m venv --system-site-packages mrv
+	$ python3 -m venv --system-site-packages venv
 
 Activate the virtualenv and install packages with pip:
 
-	$ source ./mrv/bin/activate
-	(mrv) $ pip3 install metarace
+	$ source ./venv/bin/activate
+	(venv) $ pip3 install metarace
```

### Comparing `metarace-2.1.2/pyproject.toml` & `metarace-2.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metarace"
-version = "2.1.2"
+version = "2.1.3"
 description = "Cyclesport results and timing toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT"}
 keywords = ["cyclesport", "results", "timing"]
 authors = [
     {email = "ndf-zz@6-v.org", name = "Nathan Fraser"}
 ]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Topic :: Other/Nonlisted Topic",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
     "pyserial",
     "python-dateutil",
     "pycairo",
     "PyGObject",
     "paho-mqtt",
```

### Comparing `metarace-2.1.2/src/metarace/__init__.py` & `metarace-2.1.3/src/metarace/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 from shutil import copyfile
 from metarace import jsonconfig
 try:
     from importlib.resources import files, as_file
 except ImportError:
     print('Python >= 3.9 is required to use this module')
 
-VERSION = '2.1.2'
+VERSION = '2.1.3'
 DATA_PATH = os.path.realpath(
     os.path.expanduser(os.path.join('~', 'Documents', 'metarace')))
 DEFAULTS_PATH = os.path.join(DATA_PATH, 'default')
 RESOURCE_PKG = 'metarace.data'
 LOGO = 'metarace_icon.svg'
 SYSCONF = 'metarace.json'
 PDF_TEMPLATE = 'pdf_template.json'
 LOGFILEFORMAT = '%(asctime)s %(levelname)s:%(name)s: %(message)s'
-LOGFORMAT = '%(levelname)s:%(name)s: %(message)s'
+LOGFORMAT = '%(levelname)s %(name)s: %(message)s'
 LOGLEVEL = logging.DEBUG  # default console log level
 sysconf = jsonconfig.config()  # system-defaults, populated by init() method
 _log = logging.getLogger('metarace')
 _log.setLevel(logging.DEBUG)
 
 
 def init():
@@ -53,15 +53,15 @@
             copyconf = True
     except Exception as e:
         _log.error('%s reading system config: %s', e.__class__.__name__, e)
 
     # if required, create new system default file
     if copyconf:
         _log.info('Creating default system config %s', SYSCONF)
-        with savefile(os.path.join(DEFAULTS_PATH, SYSCONF)) as f:
+        with savefile(os.path.join(DEFAULTS_PATH, SYSCONF), perm=0o600) as f:
             sysconf.write(f)
 
 
 def mk_data_path():
     """Create a shared data path if it does not yet exist."""
     ret = False
     if not os.path.exists(DATA_PATH):
@@ -128,25 +128,25 @@
         pass
     else:
         try:
             check = os.path.join(DEFAULTS_PATH, basefile)
             os.stat(check)
             ret = check
         except Exception as e:
-            _log.debug('%s: %s', e.__class__.__name__, e)
+            # ignore file not found and path errors
+            pass
     return ret
 
 
 def resource_text(name=''):
     """Return a string from the contents of the named resource."""
     basefile = os.path.basename(name)
     if basefile in ['..', '.', '', None]:
         raise FileNotFoundError('Invalid resource name: ' + repr(name))
     t = files(RESOURCE_PKG).joinpath(basefile)
-    _log.debug('Fetching %r from resource %r', basefile, t)
     if t is not None and t.is_file():
         return t.read_text(encoding='utf-8')
     else:
         raise FileNotFoundError('Named resource not found: ' + repr(name))
 
 
 def resource_file(name=''):
@@ -160,15 +160,14 @@
               Gtk.Image.new_from_file(r)
     """
 
     basefile = os.path.basename(name)
     if basefile in ['..', '.', '', None]:
         raise FileNotFoundError('Invalid resource name: ' + repr(name))
     t = files(RESOURCE_PKG).joinpath(basefile)
-    _log.debug('Fetching %r from resource %r', basefile, t)
     if t is not None and t.is_file():
         return as_file(t)
     else:
         raise FileNotFoundError('Named resource not found: ' + repr(name))
 
 
 class savefile:
@@ -180,17 +179,23 @@
        On close, the temp file is atomically moved to the provided
        filename (if possible).
 
        Note: This function will log a warning if the file could not be
        moved atomically.
     """
 
-    def __init__(self, filename, mode='t', encoding='utf-8', tempdir='.'):
+    def __init__(self,
+                 filename,
+                 mode='t',
+                 encoding='utf-8',
+                 tempdir='.',
+                 perm=0o644):
         self.__sfile = filename
         self.__path = tempdir
+        self.__perm = perm
         if mode == 'b':
             encoding = None
         self.__tfile = NamedTemporaryFile(mode='w' + mode,
                                           suffix='.tmp',
                                           prefix='sav_',
                                           dir=self.__path,
                                           encoding=encoding,
@@ -200,18 +205,17 @@
         return self.__tfile
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.__tfile.close()
         if exc_type is not None:
             return False  # raise exception
         # otherwise, file is saved ok in temp file
-        os.chmod(self.__tfile.name, 0o644)
+        os.chmod(self.__tfile.name, self.__perm)
         try:
             os.rename(self.__tfile.name, self.__sfile)
-            #_log.debug('os.rename: %r,%r', self.__tfile.name, self.__sfile)
         except OSError as e:
             _log.debug('os.rename failed: %s', e)
             copyfile(self.__tfile.name, self.__sfile)
             _log.warn('Un-safely moved file: %r', self.__sfile)
             os.unlink(self.__tfile.name)
         return True
```

### Comparing `metarace-2.1.2/src/metarace/countback.py` & `metarace-2.1.3/src/metarace/countback.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.2/src/metarace/data/IOC_Codes.csv` & `metarace-2.1.3/src/metarace/data/IOC_Codes.csv`

 * *Files identical despite different names*

### Comparing `metarace-2.1.2/src/metarace/data/bg_armfin.svg` & `metarace-2.1.3/src/metarace/data/bg_armfin.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.2/src/metarace/data/bg_armint.svg` & `metarace-2.1.3/src/metarace/data/bg_armint.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.2/src/metarace/data/bg_armstart.svg` & `metarace-2.1.3/src/metarace/data/bg_armstart.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.2/src/metarace/data/bg_idle.svg` & `metarace-2.1.3/src/metarace/data/bg_idle.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.2/src/metarace/data/bg_src.svg` & `metarace-2.1.3/src/metarace/data/bg_src.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.2/src/metarace/data/metarace_icon.svg` & `metarace-2.1.3/src/metarace/data/metarace_icon.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.2/src/metarace/data/pdf_template.json` & `metarace-2.1.3/src/metarace/data/pdf_template.json`

 * *Files identical despite different names*

### Comparing `metarace-2.1.2/src/metarace/decoder/__init__.py` & `metarace-2.1.3/src/metarace/decoder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import threading
 import queue
 import logging
 
 from metarace import tod
 
-_log = logging.getLogger('metarace.decoder')
+_log = logging.getLogger('decoder')
 _log.setLevel(logging.DEBUG)
 DECODER_LOG_LEVEL = 15
 logging.addLevelName(DECODER_LOG_LEVEL, 'DECODER')
 _PHOTOTHRESH = tod.tod('0.03')
 
 
 class decoder(threading.Thread):
```

### Comparing `metarace-2.1.2/src/metarace/decoder/rrs.py` & `metarace-2.1.3/src/metarace/decoder/rrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import socket
 import datetime
 
 from . import (decoder, DECODER_LOG_LEVEL)
 from metarace import sysconf
 from metarace import tod
 
-_log = logging.getLogger('metarace.decoder.rrs')
+_log = logging.getLogger('decoder.rrs')
 _log.setLevel(logging.DEBUG)
 
 # desired target protocol level
 _RRS_PROTOCOL = '3.2'
 # decoder port
 _RRS_TCP_PORT = 3601
 # passing record length
@@ -37,29 +37,63 @@
     32: 'Active loop limit',
     64: 'Active connection lost',
     256: 'GPS time sync error',
     512: 'GPS communication error warning',
     1024: 'Active time sync error'
 }
 
+_CONFIG_SCHEMA = {
+    'ttype': {
+        'prompt': 'Race Result System/Active Extension',
+        'control': 'section'
+    },
+    'allowstored': {
+        'type': 'bool',
+        'attr': 'allowstored',
+        'subtext': 'Report stored passings?',
+        'prompt': 'Allow Stored:',
+        'hint': 'Stored passings will be reported as normal passings',
+        'control': 'check',
+        'default': True,
+    },
+    'passiveloop': {
+        'type': 'chan',
+        'attr': 'passiveloop',
+        'prompt': 'Passive Loop:',
+        'hint': 'Assign loop ID to passive passings',
+        'control': 'choice',
+        'options': {
+            '1': '1 (Base)',
+            '2': '2',
+            '3': '3',
+            '4': '4',
+            '5': '5',
+            '6': '6',
+            '7': '7',
+            '8': '8'
+        },
+        'default': 1
+    }
+}
+
 
 class rrs(decoder):
     """RRS thread object class."""
 
     def __init__(self):
         decoder.__init__(self)
         self._io = None
         self._rdbuf = b''
         self._curfile = None
         self._lastpassing = None
         self._dorefetch = True
         self._fetchpending = False
         self._pending_command = None
-        self._allowstored = False
-        self._passiveloop = 'C1'
+        self._allowstored = True
+        self._passiveloop = 1
         self._curport = None
 
     # API overrides
     def sync(self, data=None):
         self.stop_session(data)
         self._cqueue.put_nowait(('_sync', data))
         self.start_session(data)
@@ -190,18 +224,23 @@
                 if eventid == '0':
                     eventid = ''
             except Exception as e:
                 _log.debug('%s reading isactive: %s', e.__class__.__name__, e)
 
             if not loopid:
                 loopid = self._passiveloop
-            try:
-                loopid = 'C' + str(int(loopid))
-            except Exception as e:
-                _log.debug('%s reading loop id: %s', e.__class__.__name__, e)
+            if loopid is not None:
+                try:
+                    loopid = 'C' + str(int(loopid))
+                except Exception as e:
+                    _log.debug('%s reading loop id: %s', e.__class__.__name__,
+                               e)
+            else:
+                # Assume passive without loop set
+                loopid = 'PSV'
             activestore = False
             if active and adata:
                 activestore = (int(adata) & 0x40) == 0x40
             if not active and tagid and eventid:
                 tagid = '-'.join((eventid, tagid))
             if tagid == _RRS_MARKER:
                 tagid = ''
@@ -391,20 +430,19 @@
                 self._dorefetch = False
                 cmd = '{:d}:32'.format(self._lastpassing + 1)
                 self.write(cmd)
 
     def run(self):
         """Decoder main loop."""
         _log.debug('Starting')
-        if sysconf.has_option('rrs', 'allowstored'):
-            self._allowstored = sysconf.get_bool('rrs', 'allowstored')
-            _log.debug('Allow stored passings: %r', self._allowstored)
-        if sysconf.has_option('rrs', 'passiveloop'):
-            self._passiveloop = sysconf.get_str('rrs', 'passiveloop', '1')
-            _log.info('Passive loop id set to: %r', self._passiveloop)
+        sysconf.add_section('rrs', _CONFIG_SCHEMA)
+        self._allowstored = sysconf.get_value('rrs', 'allowstored')
+        self._passiveloop = sysconf.get_value('rrs', 'passiveloop')
+        _log.debug('Allow stored passings: %r', self._allowstored)
+        _log.debug('Passive loop id set to: %r', self._passiveloop)
         self._running = True
         while self._running:
             try:
                 c = None
                 if self._io is not None:
                     # Read responses until response complete or timeout
                     try:
```

### Comparing `metarace-2.1.2/src/metarace/decoder/rru.py` & `metarace-2.1.3/src/metarace/decoder/rru.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from time import sleep
 
 from . import (decoder, DECODER_LOG_LEVEL)
 from metarace import tod
 from metarace import sysconf
 from metarace import strops
 
-_log = logging.getLogger('metarace.decoder.rru')
+_log = logging.getLogger('decoder.rru')
 _log.setLevel(logging.DEBUG)
 
 _RRU_BAUD = 19200
 _RRU_PASSLEN = 12
 _RRU_BEACONLEN = 17
 _RRU_LOWBATT = 2.3  # Warn if battery voltage is below this many volts
 _RRU_REFCHECK = 1800  # check ref after this many timeouts
@@ -39,16 +39,18 @@
     'EPOCHREFSET',
     'EPOCHREFADJ1D',
     'PASSINGGET',
     'PASSINGINFOGET',
     'BEACONGET',
     'PREWARN',
 ]
-# Documented configuration parameter. If default is not None, the
-# value will be set in _sane().
+# Internal Decoder configuration parameters,
+# Some of these may be accessed through the
+# sysconf/jsonconfig schema below.
+# Values are sent to decoder in _sane().
 _CONFINFO = {
     '01': {
         'label': 'Push Pre-Warn',
         'default': None,
         '00': 'disabled',
         '01': 'enabled'
     },
@@ -71,14 +73,15 @@
         '00': 'disabled',
         '01': 'enabled'
     },
     '05': {
         'label': 'Operation Mode',
         # assume usb-timing is required unless explicity configured otherwise
         'default': '06',
+        '00': 'active extension',
         '05': 'usb-kiosk',
         '06': 'usb-timing',
         '07': 'usb-store&copy'
     },
     '06': {
         'label': 'Channel ID',
         'default': None,
@@ -201,14 +204,138 @@
 _LOOP_STATES = {
     '00': 'OK',
     '01': 'Fault',
     '02': 'Limit',
     '03': 'Overvoltage Error'
 }
 
+_CONFIG_SCHEMA = {
+    'ttype': {
+        'prompt': 'Race Result USB Active Decoder',
+        'control': 'section'
+    },
+    'allowstored': {
+        'type': 'bool',
+        'subtext': 'Report stored passings?',
+        'prompt': 'Allow Stored:',
+        'hint': 'Stored passings will be reported as normal passings',
+        'control': 'check',
+        'default': True
+    },
+    'loopid': {
+        'attr': '07',
+        'prompt': 'Loop ID:',
+        'hint': 'Active loop ID',
+        'control': 'choice',
+        'options': {
+            '00': '1 (Base)',
+            '01': '2',
+            '02': '3',
+            '03': '4',
+            '04': '5',
+            '05': '6',
+            '06': '7',
+            '07': '8'
+        },
+        'default': '00'
+    },
+    'looppower': {
+        'attr': '08',
+        'prompt': 'Loop Power:',
+        'hint': 'Loop activation power',
+        'type': 'float',
+        'control': 'short',
+        'subtext': '%',
+        'default': 30.0,
+    },
+    'channel': {
+        'attr': '06',
+        'prompt': 'Channel ID:',
+        'hint': 'Race Result wireless channel ID',
+        'control': 'choice',
+        'options': {
+            '00': '1',
+            '01': '2',
+            '02': '3',
+            '03': '4',
+            '04': '5',
+            '05': '6',
+            '06': '7',
+            '07': '8',
+            'auto': 'Auto (Site Survey)',
+        },
+    },
+    'hwopts': {
+        'control': 'section',
+        'prompt': 'Hardware Setup',
+    },
+    'impulse': {
+        'prompt': 'Option Jack:',
+        'control': 'choice',
+        'attr': '03',
+        'hint': 'Use the option jack for impulse in or beep output',
+        'options': {
+            '00': 'Impulse Input',
+            '01': 'Beep Output'
+        },
+        'default': '00',
+    },
+    'mode': {
+        'attr': '05',
+        'control': 'choice',
+        'prompt': 'Mode:',
+        'hint': 'Specify extension timing mode',
+        'default': '06',
+        'options': {
+            '00': 'Active Extension RS-232',
+            '06': 'USB TIming Box',
+            '05': 'USB Kiosk',
+            '07': 'USB Store & Copy',
+        },
+    },
+    'usedtr': {
+        'attr': '0b',
+        'type': 'bool',
+        'subtext': 'Use DTR line?',
+        'prompt': 'DTR Sync:',
+        'hint': 'Use DTR signal to synchronise decoder with host computer',
+        'control': 'check',
+        'default': True
+    },
+    'charge': {
+        'attr': '0a',
+        'type': 'bool',
+        'subtext': 'Charge via USB connection?',
+        'prompt': 'Charge:',
+        'hint': 'Charger decoder internal battery using USB power',
+        'control': 'check',
+        'default': True
+    },
+    'shutdown': {
+        'attr': '04',
+        'type': 'bool',
+        'subtext': 'Shutdown on power loss?',
+        'prompt': 'Shutdown:',
+        'hint': 'Automatically shutdown decoder on power loss',
+        'control': 'check',
+        'default': False
+    },
+    'chanswitch': {
+        'attr': '0c',
+        'prompt': 'Channel Switch:',
+        'hint': 'Alternate channel switching',
+        'control': 'choice',
+        'options': {
+            '00': 'Disabled (V1)',
+            '01': 'Automatic',
+            '02': 'Forced (V2 Only)'
+        },
+    },
+}
+
 
 class rru(decoder):
     """Race Result USB Active Decoder"""
 
     def __init__(self):
         decoder.__init__(self)
         self._sitenoise = {
@@ -227,15 +354,15 @@
         self._rruht = None
         self._error = False
         self._io = None
         self._rdbuf = b''
         self._curreply = None  # current multi-line response mode
         self._lastpassing = 0
         self._lastrequest = None
-        self._request_pending = False
+        self._request_pending = 1
         self._allowstored = False
         self._autochannelid = None
         self._refcount = 0
         self._curport = None
 
     # API overrides
     def status(self):
@@ -246,57 +373,77 @@
             self.write(''.join(['INFOGET;', c]))
         self.write('BEACONGET')
         self.write('PASSINGINFOGET')
         self.write('TIMESTAMPGET')
 
     def connected(self):
         """Return true if decoder is connected"""
-        return self._boxname is not None and self._io is not None
+        return self._boxname is not None and self._io is not None and self._request_pending < 10
 
     # Device-specific functions
     def _close(self):
         self._boxname = None
         if self._io is not None:
             _log.debug('Close connection')
             cp = self._io
             self._io = None
             cp.close()
 
     def _port(self, port):
         """Re-establish connection to supplied device port."""
-        self._request_pending = False
+        self._request_pending = 1
         self._rrustamp = None
         self._rruht = None
         self._close()
         if port is None and self._curport is not None:
             port = self._curport
         if port is None:
             _log.debug('Re-connect cancelled: port is None')
             return
         self._rdbuf = b''
         _log.debug('Connecting to %r', port)
         s = serial.Serial(baudrate=_RRU_BAUD,
                           rtscts=False,
                           timeout=_RRU_IOTIMEOUT)
-        s.dtr = 0  # This must be set _before_ open()
+        s.dtr = 0
         s.port = port
         s.open()
         self._io = s
         self._sane()
+        self._cqueue.put(('_pendclr', ''))
 
     def _sane(self, data=None):
         """Load system config and then check decoder is properly configured"""
+        sysconf.add_section('rru', _CONFIG_SCHEMA)
+        self._allowstored = sysconf.get_value('rru', 'allowstored')
+        _log.debug('Allow stored passings: %r', self._allowstored)
         setconfs = {}
-        if sysconf.has_option('rru', 'allowstored'):
-            self._allowstored = strops.confopt_bool(
-                sysconf.get('rru', 'allowstored'))
-            _log.info('Allow stored passings: %r', self._allowstored)
-        if sysconf.has_option('rru', 'decoderconfig'):
-            setconfs = sysconf.get('rru', 'decoderconfig')
-            _log.debug('Loaded %r config options from sysconf', len(setconfs))
+        for opt in ('loopid', 'channel', 'impulse', 'chanswitch', 'mode'):
+            nv = sysconf.get_value('rru', opt)
+            if nv is not None:
+                lbl = _CONFINFO[_CONFIG_SCHEMA[opt]['attr']]['label']
+                setconfs[lbl] = nv
+                _log.debug('Read value: %r = %r from sysconf', lbl, nv)
+        for opt in ('usedtr', 'charge', 'shutdown'):
+            if sysconf.has_value('rru', opt):
+                nv = '00'
+                if sysconf.get_value('rru', opt):
+                    nv = '01'
+                lbl = _CONFINFO[_CONFIG_SCHEMA[opt]['attr']]['label']
+                setconfs[lbl] = nv
+                _log.debug('Read value: %r = %r from sysconf', lbl, nv)
+        if sysconf.has_value('rru', 'looppower'):
+            # WTF Race Result? 0x0-0x64
+            nv = round(sysconf.get_value('rru', 'looppower'))
+            nv = '%02x' % ((min(100, max(0, nv))))
+            lbl = _CONFINFO[_CONFIG_SCHEMA['looppower']['attr']]['label']
+            setconfs[lbl] = nv
+            _log.debug('Read value: %r = %r from sysconf', lbl, nv)
+
+        # re-build internal configuration
         self._config = {}
         for opt in _CONFINFO:
             ko = _CONFINFO[opt]
             kn = ko['label']
             if kn in setconfs and setconfs[kn] is not None:
                 self._config[opt] = setconfs[kn]
                 sv = setconfs[kn]
@@ -306,14 +453,17 @@
             elif ko['default'] is not None:
                 self._config[opt] = ko['default']
 
         # if channel id set already by site survey, keep it
         if self._autochannelid is not None:
             self._config['06'] = self._autochannelid
 
+        # Clear any messages in queue
+        self._dump_queue()
+
         # Set protocol
         self.write('ASCII')
         # Fetch decoder ID
         self.write('INFOGET;01')
         # Set options, ordering ensures Box mode is set before impulse in
         for opt in [
                 '05', '01', '02', '04', '07', '08', '09', '0a', '0b', '0c',
@@ -328,16 +478,14 @@
                 self.write('SITESURVEY')
             else:
                 self.write(';'.join(['CONFSET', '06', self._config['06']]))
         # Request current epoch ref setting
         self.write('EPOCHREFGET')
         # Request current number of ticks
         self.write('TIMESTAMPGET')
-        # Request loop ID
-        self.write('CONFGET;07')
         # Request current memory status
         self.write('PASSINGINFOGET')
 
     def _sync(self, data=None):
         _log.debug('Performing blocking DTR sync')
         # for the purpose of sync, the "epoch" is considered to be
         # midnight localtime of the current day
@@ -364,14 +512,15 @@
             nt = tod.now()
             diff = ett - nt
         _log.debug('Set DTR')
         self._io.dtr = 1
         sleep(0.2)
         _log.debug('Clear DTR')
         self._io.dtr = 0
+        self._cqueue.put(('_pendclr', ''))
 
     def _start_session(self, data=None):
         """Reset decoder to start a new session"""
         # On USB decoder, session is always active, this
         # method performs a hard reset/clear/sync
         self._clear(data)
         _log.info('Start session')
@@ -381,35 +530,47 @@
         # USB decoder will continue collecting passings, but
         # they are not received by handler - the passings can
         # be fetched by restarting connection without reset
         self._rrustamp = None
         _log.info('Stop session')
 
     def _clear(self, data=None):
-        _log.debug('Performing box reset')
+        _log.info('Requesting new session')
+        self._rrustamp = None
         self._boxname = None
         self._write('RESET')
         while True:
             m = self._readline()
             #_log.debug('RECV: %r', m)
             if m == 'AUTOBOOT':
+                sleep(1.0)
                 break
-        self._rrustamp = None
         self._lastrequest = 0
         self._lastpassing = 0
-        # Queue 'sane' config options before sync request
         self._sane()
-        self.sync()
+
+    def _dump_queue(self):
+        try:
+            while not self._cqueue.empty():
+                m = self._cqueue.get_nowait()
+                _log.debug('Dumping command: %r', m)
+                self._cqueue.task_done()
+        except Exception as e:
+            _log.debug('$s emptying queue: %s', e.__class__.__name__, e)
 
     def _write(self, msg):
         if self._io is not None:
             ob = (msg + _RRU_EOL)
             self._io.write(ob.encode(_RRU_ENCODING))
             #_log.debug('SEND: %r', ob)
 
+    def _pendclr(self, msg):
+        _log.debug('Enable passing request')
+        self._request_pending = 0
+
     def _tstotod(self, ts):
         """Convert a race result timestamp to time of day."""
         ret = None
         try:
             ti = int(ts, 16) - self._rrustamp
             tsec = decimal.Decimal(ti // 256) + decimal.Decimal(ti % 256) / 256
             nsec = (self._rruht.timeval + tsec) % 86400
@@ -491,39 +652,45 @@
 
     def _refgetmsg(self, epoch, stime):
         """Collect the epoch ref and system tick message."""
         self._rruht = tod.mkagg(int(epoch, 16))
         self._rrustamp = int(stime, 16)
         _log.debug('Reference ticks: %r @ %r', self._rrustamp,
                    self._rruht.rawtime())
+        if self._rrustamp == 0:
+            _log.info('Decoder time is not set, requesting sync')
+            self.sync()
 
     def _timestampchk(self, ticks):
         """Receive the number of ticks on the decoder."""
         tcnt = int(ticks, 16)
-        _log.info('Box tick count: %r', tcnt)
+        _log.debug('Box tick count: %r', tcnt)
         if tcnt > _RRU_REFTHRESH:
-            _log.info('Tick threshold exceeded, adjusting ref')
+            _log.info('Box tick threshold exceeded, adjusting ref')
             self.write('EPOCHREFADJ1D')
 
     def _passinginfomsg(self, mv):
         """Receive info about internal passing memory."""
         if len(mv) == 5:
             pcount = int(mv[0], 16)
             if pcount > 0:
                 pfirst = int(mv[1], 16)
                 pftime = self._tstotod(mv[2])
                 plast = int(mv[3], 16)
                 pltime = self._tstotod(mv[4])
                 _log.info('Info %r Passings, %r@%s - %r@%s', pcount, pfirst,
                           pftime.rawtime(2), plast, pltime.rawtime(2))
-                if plast + 1 < self._lastpassing:
-                    _log.warning(
-                        'Decoder memory/ID mismatch last=%r, req=%r, clear/sync required.',
-                        plast, self._lastpassing)
+                if self._lastrequest is None:
                     self._lastpassing = plast + 1
+                else:
+                    if plast + 1 < self._lastpassing:
+                        _log.warning(
+                            'Decoder memory/ID mismatch last=%r, req=%r, clear/sync required.',
+                            plast, self._lastpassing)
+                        self._lastpassing = plast + 1
             else:
                 _log.info('Info No Passings')
         else:
             _log.debug('Non-passinginfo message: %r', mv)
 
     def _passingmsg(self, mv):
         """Receive a passing from the decoder."""
@@ -589,15 +756,15 @@
                 else:
                     pass
             self._lastpassing += 1
         elif len(mv) == 2:
             resp = int(mv[0], 16)
             rcount = int(mv[1], 16)
             if resp != self._lastrequest:
-                _log.error('Sequence mismatch request: %r, response: %r',
+                _log.debug('Sequence mismatch request: %r, response: %r',
                            self._lastrequest, resp)
                 self._lastpassing = 0
             elif rcount > 0:
                 _log.debug('Receiving %r passings', rcount)
         else:
             _log.debug('Non-passing message: %r', mv)
 
@@ -651,15 +818,15 @@
             nv = self._sitenoise[c]
             lv.append('{}:{:d}%'.format(c, nv))
             if nv < cv:
                 ch = c
                 cv = nv
         _log.debug('Site survey: %s', ' '.join(lv))
         if ch is not None:
-            _log.info('Selected channel %r (%d%%)', ch, cv)
+            _log.info('Auto-selected channel %r, Noise: %d%%', ch, cv)
             sv = '{0:02x}'.format(ch - 1)
             self._autochannelid = sv
             m = 'CONFSET;06;{}'.format(sv)
             self.write(m)
         else:
             _log.warning('Unable to find a suitable channel')
 
@@ -699,28 +866,37 @@
             if mv[0] == '#P':
                 # pushed passing overrides cmd/reply logic
                 self._passingmsg(mv[1:])
             elif mv[0] == 'PREWARN':
                 self._curreply = mv[0]
             elif mv[0] == 'EOR':
                 if self._curreply in ['PASSINGGET', 'PASSINGIDERROR']:
-                    self._request_pending = False
+                    self._request_pending = 0
                 if self._curreply == 'SITESURVEY':
                     self._chansurf()
                 self._curreply = None
             elif mv[0] in _REPLIES:
                 if self._curreply is not None:
                     _log.debug('Protocol error: %r not terminated',
                                self._curreply)
                 self._curreply = mv[0]
                 if mv[1] != '00':
                     if self._curreply == 'PASSINGGET' and mv[1] == '10':
                         self._curreply = 'PASSINGIDERROR'
                     else:
                         _log.debug('%r error: %r', self._curreply, mv[1])
+            elif mv[0] == 'AUTOBOOT':
+                _log.warning('Re-connecting restarted decoder')
+                self._request_pending = 1
+                self._sane()
+            elif 'rrActive' in mv[0]:
+                _log.warning('Decoder reset - waiting for AUTOBOOT')
+                self._request_pending = 1
+                sleep(3.0)
+                self._dump_queue()
             else:
                 if self._curreply is not None:
                     self._handlereply(mv)
 
     def _readline(self):
         """Read from the decoder until end of line or timeout condition."""
         ret = None
@@ -739,22 +915,24 @@
             ch = self._io.read(1)
         return ret
 
     def _request_next(self):
         """Queue a passingget request if the reftime is set."""
         if self._rrustamp is not None:
             if not self._request_pending:
-                self._request_pending = True
+                self._request_pending = 1
                 es = 'PASSINGGET;{0:08x}'.format(self._lastpassing)
                 self._lastrequest = self._lastpassing
                 self.write(es)
                 self._refcount += 1
                 if self._refcount > _RRU_REFCHECK:
                     self.write('TIMESTAMPGET')
                     self._refcount = 0
+            else:
+                self._request_pending += 1
 
     def run(self):
         """Decoder main loop."""
         _log.debug('Starting')
         self._running = True
         while self._running:
             try:
```

### Comparing `metarace-2.1.2/src/metarace/decoder/thbc.py` & `metarace-2.1.3/src/metarace/timy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,560 +1,531 @@
 # SPDX-License-Identifier: MIT
-"""Tag Heuer/Chronelec Decoder Interface."""
+"""Alge Timy Interface
 
-# For connections to multiple decoders, use thbchub
+ Interface an Alge Timy chronoprinter via serial port.
 
+ Example:
+
+	import metarace
+	from metarace import timy
+	metarace.init()
+
+	def timercb(impulse):
+	    print(impulse)
+
+	t = timy.timy()
+	t.setport('/dev/ttyS0')
+	t.setcb(timercb)
+	t.start()
+	t.sane()
+	t.arm('C0')
+	t.armlock()
+	...
+
+ Configuration is read from metarace system config (metarace.json),
+ under section 'timy':
+
+  key: (type) Description [default]
+  --
+  baudrate: (int) serial port speed [38400]
+  ctsrts: (bool) if True, use hardware flow control [False]
+  delayN: (tod) channel N delay time in seconds [None]
+
+ Notes:
+
+	- Callback function is only called for impulses received
+	  while channel is armed.
+
+	- ALL timing impulses correctly read from an attached
+	  Timy will be logged by the command thread with the log
+	  label 'TIMER', even when the channel is not armed.
+
+	- It is assumed that messages are received over the serial
+	  connection in the same order as they are measured by
+	  the Timy.
+
+	- Channel delay config compensates for wireless impulse
+	  or relay sytems with a fixed processing time. To adjust
+	  channel blocking delay times, instead use method timy.delaytime()
+
+"""
+
+import threading
 import queue
-import logging
 import serial
-import socket
-import time
+import logging
 
-from . import (decoder, DECODER_LOG_LEVEL)
 from metarace import sysconf
 from metarace import tod
+from metarace.strops import chan2id, id2chan
+
+# Configuration defaults
+_DEFBAUD = 38400
+_DEFCTSRTS = False
+
+# Internal constants
+_ENCODING = 'cp437'
+_CHAN_UNKNOWN = -1
+_CR = b'\x0d'
+_TCMDS = ('EXIT', 'PORT', 'MSG', 'TRIG', 'RCLR')
 
-_log = logging.getLogger('metarace.decoder.thbc')
+# Logging
+_log = logging.getLogger('timy')
 _log.setLevel(logging.DEBUG)
+_TIMER_LOG_LEVEL = 15
+logging.addLevelName(_TIMER_LOG_LEVEL, 'TIMER')
 
-THBC_BAUD = 19200
-THBC_UDP_PORT = 2008
-THBC_ENCODING = 'iso8859-1'
-
-# THbC protocol messages
-ESCAPE = b'\x1b'
-HELOCMD = b'MR1'
-STOPCMD = ESCAPE + b'\x13\x5c'
-REPEATCMD = ESCAPE + b'\x12'
-ACKCMD = ESCAPE + b'\x11'
-
-STATCMD = ESCAPE + b'\x05'  # fetch status
-CHKCMD = ESCAPE + b'\x06'  # UNKNOWN
-STARTCMD = ESCAPE + b'\x07'  # start decoder
-SETCMD = ESCAPE + b'\x08'  # set configuration
-IPCMD = ESCAPE + b'\x09'  # set IP configuration
-QUECMD = ESCAPE + b'\x10'  # fetch configuration
-
-STALVL = ESCAPE + b'\x1e'
-BOXLVL = ESCAPE + b'\x1f'
-
-NACK = b'\x07'
-CR = b'\x0d'
-LF = b'\x0a'
-SETTIME = ESCAPE + b'\x48'
-STATSTART = b'['
-PASSSTART = b'<'
-
-# decoder config consts
-IPCONFIG_LEN = 16
-CONFIG_LEN = 27
-CONFIG_TOD = 0
-CONFIG_GPS = 1
-CONFIG_TZ_HOUR = 2
-CONFIG_TZ_MIN = 3
-CONFIG_485 = 4
-CONFIG_FIBRE = 5
-CONFIG_PRINT = 6
-CONFIG_MAX = 7
-CONFIG_PROT = 8
-CONFIG_PULSE = 9
-CONFIG_PULSEINT = 10
-CONFIG_CELLSYNC = 11
-CONFIG_CELLTOD_HOUR = 12
-CONFIG_CELLTOD_MIN = 13
-CONFIG_TONE_STA = 15
-CONFIG_TONE_BOX = 17
-CONFIG_TONE_MAN = 19
-CONFIG_TONE_CEL = 21
-CONFIG_TONE_BXX = 23
-CONFIG_ACTIVE_LOOP = 14
-CONFIG_SPARE = 25
-CONFIG_FLAGS = {
-    CONFIG_TOD: 'Time of Day',
-    CONFIG_GPS: 'GPS Sync',
-    CONFIG_TZ_HOUR: 'Timezone Hour',
-    CONFIG_TZ_MIN: 'Timezone Min',
-    CONFIG_485: 'Distant rs485',
-    CONFIG_FIBRE: 'Distant Fibre',
-    CONFIG_PRINT: 'Serial Print',
-    CONFIG_MAX: 'Detect Max',
-    CONFIG_PROT: 'Protocol',
-    CONFIG_PULSE: 'Sync Pulse',
-    CONFIG_PULSEINT: 'Sync Interval',
-    CONFIG_CELLSYNC: 'CELL Sync',
-    CONFIG_CELLTOD_HOUR: 'CELL Sync Hour',
-    CONFIG_CELLTOD_MIN: 'CELL Sync Min',
-    CONFIG_TONE_STA: 'STA Tone',
-    CONFIG_TONE_BOX: 'BOX Tone',
-    CONFIG_TONE_MAN: 'MAN Tone',
-    CONFIG_TONE_CEL: 'CEL Tone',
-    CONFIG_TONE_BXX: 'BXX Tone',
-    CONFIG_ACTIVE_LOOP: 'Active Loop',
-    CONFIG_SPARE: '[spare]'
-}
-DEFAULT_IPCFG = {
-    'IP': '192.168.0.10',
-    'Netmask': '255.255.255.0',
-    'Gateway': '0.0.0.0',
-    'Host': '192.168.0.255'
+_CONFIG_SCHEMA = {
+    'ttype': {
+        'prompt': 'Alge Timy RS-232 Options',
+        'control': 'section',
+    },
+    'baudrate': {
+        'prompt': 'Baudrate:',
+        'attr': 'baudrate',
+        'hint': 'Serial line speed in bps',
+        'control': 'choice',
+        'type': 'int',
+        'options': {
+            '9600': '9600 (Timy)',
+            '19200': '19200',
+            '38400': '38400 (Timy 2/3)'
+        },
+        'default': _DEFBAUD,
+    },
+    'ctsrts': {
+        'prompt': 'Handshake:',
+        'attr': 'cstrts',
+        'hint': 'Enable RTS-CTS handshake on serial line',
+        'subtext': 'With RTS-CTS?',
+        'control': 'check',
+        'type': 'bool',
+        'default': _DEFCTSRTS,
+    },
+    'dsec': {
+        'prompt': 'Channel Delays',
+        'control': 'section',
+    },
+    'delay0': {
+        'prompt': 'C0:',
+        'control': 'short',
+        'subtext': '(Start)',
+        'type': 'tod',
+        'places': '4',
+    },
+    'delay1': {
+        'prompt': 'C1:',
+        'control': 'short',
+        'subtext': '(Finish)',
+        'type': 'tod',
+        'places': '4',
+    },
+    'delay2': {
+        'prompt': 'C2:',
+        'control': 'short',
+        'subtext': '(Cell/Pursuit A)',
+        'type': 'tod',
+        'places': '4',
+    },
+    'delay3': {
+        'prompt': 'C3:',
+        'control': 'short',
+        'subtext': '(Plunger/Pursuit B)',
+        'type': 'tod',
+        'places': '4',
+    },
+    'delay4': {
+        'prompt': 'C4:',
+        'control': 'short',
+        'subtext': '(Aux Start/200m Start)',
+        'type': 'tod',
+        'places': '4',
+    },
+    'delay5': {
+        'prompt': 'C5:',
+        'control': 'short',
+        'subtext': '(100m Split)',
+        'type': 'tod',
+        'places': '4',
+    },
+    'delay6': {
+        'prompt': 'C6:',
+        'control': 'short',
+        'type': 'tod',
+        'places': '4',
+    },
+    'delay7': {
+        'prompt': 'C7:',
+        'control': 'short',
+        'type': 'tod',
+        'places': '4',
+    },
+    'delay8': {
+        'prompt': 'C8:',
+        'control': 'short',
+        'type': 'tod',
+        'places': '4',
+    },
 }
-DEFPORT = '/dev/ttyS0'
-
-
-def reflect(dat, width):
-    """Reverse bit order of byte"""
-    out = dat & 0x01
-    for i in range(width - 1):
-        dat >>= 1
-        out = (out << 1) | (dat & 0x01)
-    return out
-
-
-# Build a lookup table for the MCRF4XX CRC
-# Source: pycrc https://pycrc.org/
-_MCRF4XXTBL = [0] * 256
-for i in range(256):
-    r = i
-    r = reflect(r, 8) << 8
-    for j in range(8):
-        if r & 0x8000 != 0:
-            r = (r << 1) ^ 0x1021
-        else:
-            r = (r << 1)
-    r = reflect(r, 16)
-    _MCRF4XXTBL[i] = r & 0xffff
-
-
-def mcrf4xx(msgstr=b''):
-    """Return MCRF4XX CRC for provided byte string."""
-    r = 0xffff  # reflect(0xffff,16) == 0xffff
-    for b in msgstr:
-        i = (r ^ b) & 0xff
-        r = ((r >> 8) ^ _MCRF4XXTBL[i]) & 0xffff
-    return r & 0xffff  # collapse two reflects, mask and ^0
 
 
-def thbc_sum(msgstr=b''):
-    """Return sum of character values as decimal string."""
+def _timy_checksum(msg):
+    """Return a checksum for the Timy message string."""
     ret = 0
-    for ch in msgstr:
-        ret = ret + ch
-    return '{0:04d}'.format(ret).encode('ascii', 'ignore')
+    for ch in msg:
+        ret = ret + ord(ch)
+    return ret & 0xff
 
 
-def val2hexval(val):
-    """Convert int to decimal digit equivalent hex byte."""
-    ret = 0x00
-    ret |= ((val // 10) & 0x0f) << 4  # msd	97 -> 0x90
-    ret |= (val % 10) & 0x0f  # lsd   97 -> 0x07
+def _timy_getsum(chkstr):
+    """Convert Timy checksum string to an integer."""
+    ret = -1
+    try:
+        ms = (ord(chkstr[0]) - 0x30) & 0xf
+        ls = (ord(chkstr[1]) - 0x30) & 0xf
+        ret = ms << 4 | ls
+    except Exception as e:
+        _log.debug('error collecting timy checksum: %s', e)
     return ret
 
 
-def hexval2val(hexval):
-    """Unconvert a decimal digit equivalent hex byte to int."""
-    ret = 10 * (hexval >> 4)  # tens 0x97 -> 90
-    ret += hexval & 0x0f  # ones 0x97 ->  7
-    return ret
+def _defcallback(impulse=None):
+    """Default impulse callback."""
+    _log.debug('Unhandled impulse: %r', impulse)
 
 
-class thbc(decoder):
-    """Tag Heuer / Chronelec thread object class."""
+class timy(threading.Thread):
+    """Timy thread object class."""
 
     def __init__(self):
-        decoder.__init__(self)
-        self._boxname = None
-        self._version = ''
-        self._decoderconfig = {}
-        self._decoderipconfig = {}
-        self._io = None
-        self._cksumerr = 0
-        self._rdbuf = b''  # bytestring read buffer
-        self._curport = None
-
-    # API overrides
-    def status(self):
-        """Request status message from decoder."""
-        self.write(STATCMD)
+        """Construct Timy thread object."""
+        threading.Thread.__init__(self, daemon=True)
+        self.__port = None
+        self.__cqueue = queue.Queue()  # command queue
+        self.__rdbuf = b''
+        self.__arms = [
+            False, False, False, False, False, False, False, False, False,
+            False
+        ]
+        self.__clearing = False
+        self.__armlocked = False
+        self.__chandelay = {}
+        self.__cb = _defcallback
+        self.__name = 'timy'
+        self.error = False
+
+        sysconf.add_section('timy', _CONFIG_SCHEMA)
+        self.__baudrate = sysconf.get_value('timy', 'baudrate')
+        self.__ctsrts = sysconf.get_value('timy', 'ctsrts')
+        _log.debug('Set serial baudrate to: %d', self.__baudrate)
+        _log.debug('Set serial CTSRTS to: %s', self.__ctsrts)
+        for c in range(0, 8):
+            cd = sysconf.get_value('timy', 'delay' + str(c))
+            if cd is not None:
+                self.__chandelay[c] = cd
+                _log.debug('Set channel delay %s: %s', c, cd.rawtime(4))
+
+    def setcb(self, func=None):
+        """Set or clear impulse callback function."""
+        if func is not None:
+            self.__cb = func
+        else:
+            self.__cb = _defcallback
 
-    def connected(self):
-        return self._io is not None and self._boxname is not None
+    def printline(self, msg=''):
+        """Print msg to Timy printer, stripped and truncated."""
+        lmsg = msg[0:32]
+        _log.log(_TIMER_LOG_LEVEL, lmsg)
+        self.__cqueue.put_nowait(('MSG', 'DTP' + lmsg + '\r'))
+
+    def linefeed(self):
+        """Advance Timy printer by one line."""
+        self.__cqueue.put_nowait(('MSG', 'PRILF\r'))
+
+    def clrmem(self):
+        """Clear memory in attached Timy."""
+        self.__cqueue.put_nowait(('MSG', 'CLR\r'))
 
-    def stop_session(self):
-        """Send a stop command to decoder."""
-        self.write(STOPCMD)
-
-    def start_session(self):
-        """Send a depart command to decoder."""
-        self.write(STARTCMD)
-
-    def clear(self):
-        """Start a new session and request time sync."""
-        self.stop_session()
-        self.start_session()
-        self.sync()
-
-    def get_config(self):
-        """Request decoder configuration."""
-        self.write(QUECMD)
-
-    def ipconfig(self):
-        """Request sanity check in decoder thread."""
-        self._cqueue.put_nowait(('_ipcfg', None))
-
-    # Device-specific functions
-    def _close(self):
-        if self._io is not None:
-            _log.debug('Close connection')
-            cp = self._io
-            self._io = None
-            try:
-                cp.close()
-            except Exception as e:
-                _log.debug('%s closing io: %s', e.__class__.__name__, e)
-
-    def _port(self, port):
-        """Re-establish connection to supplied device port."""
-        self._close()
-        if port is None and self._curport is not None:
-            port = self._curport
-        if port is None:
-            _log.debug('Re-connect cancelled: port is None')
-            return
-        s = None
-        self._rdbuf = b''
-        if '/' not in port and '.' in port:
-            _log.debug('Attempting UDP on %r', port)
-            s = dgram(port, THBC_UDP_PORT)
-        else:
-            # assume device file
-            s = serial.Serial(port, THBC_BAUD, rtscts=False, timeout=0.2)
-        self._boxname = None
-        self._io = s
-        self._write(QUECMD)
-        # queue sane through command loop
-        time.sleep(0.2)
-        self.sane()
-        self._curport = port
-
-    def _sync(self, data=None):
-        _log.debug('Performing blocking sync')
-        acceptval = tod.tod('0.001')
-        nt = tod.now()
-        diff = nt - nt.truncate(0)
-        while diff > acceptval and diff < tod.ONE:
-            time.sleep(0.0005)
-            nt = tod.now()
-            diff = nt - nt.truncate(0)
-        self._write(self._set_time_cmd(nt))
-        _log.debug('Set time: %r', nt.meridiem())
-
-    def _ipcfg(self, data=None):
-        """Alter the attached decoder's IP address."""
-        ipcfg = sysconf.get('thbc', 'ipconfig')
-        cmd = b'\x09\x09'
-        for i in ['IP', 'Netmask', 'Gateway', 'Host']:
-            if i not in ipcfg:
-                ipcfg[i] = DEFAULT_IPCFG[i]
-            cmd += socket.inet_aton(socket.gethostbyname(ipcfg[i]))
-        _log.info('Attempting IP config update')
-        self._v3_cmd(cmd)
-
-    def _sane(self, data=None):
-        """Check decoder config against system settings."""
-        doconf = False
-        if self._boxname is not None:
-            if sysconf.has_option('thbc', 'decoderconfig'):
-                oconf = sysconf.get('thbc', 'decoderconfig')
-                for flag in self._decoderconfig:
-                    key = CONFIG_FLAGS[flag]
-                    if key in oconf:
-                        if oconf[key] != self._decoderconfig[flag]:
-                            _log.info('Key mismatch: %r', key)
-                            self._decoderconfig[flag] = oconf[key]
-                            doconf = True
+    def status(self):
+        """Request status and current program from Timy."""
+        self.__cqueue.put_nowait(('MSG', 'NSF?\r'))
+        self.__cqueue.put_nowait(('MSG', 'PROG?\r'))
+
+    def dumpall(self):
+        """Request a dump of all recorded impulses to host."""
+        self.__cqueue.put_nowait(('MSG', 'RSM\r'))
+
+    def delaytime(self, newdelay='2.0'):
+        """Update blocking delay time for all channels."""
+        dt = tod.mktod(newdelay)
+        if dt is not None:
+            if dt > tod.ZERO and dt < tod.tod('99.99'):
+                nt = dt.rawtime(2, zeros=True)[6:]
+                self.__cqueue.put_nowait(('MSG', 'DTS' + nt + '\r'))
+                self.__cqueue.put_nowait(('MSG', 'DTF' + nt + '\r'))
+            else:
+                _log.info('Ignoring invalid delay time: %s', dt.rawtime())
         else:
-            _log.info('Decoder not connected')
+            _log.info('Ignoring invalid delay time')
 
-        # re-write config if required
-        if doconf:
-            _log.info('Re-configuring %r', self._boxname)
-            self._set_config()
-
-        # force decoder levels
-        if sysconf.has_option('thbc', 'levels'):
-            lvl = sysconf.get('thbc', 'levels')
-            self._setlvl(box=lvl[0], sta=lvl[1])
-
-    def _v3_cmd(self, cmdstr=b''):
-        """Pack and send a v3 command directly to port."""
-        crc = mcrf4xx(cmdstr)
-        crcstr = bytes([(crc >> 8) & 0xff, crc & 0xff])
-        self._write(ESCAPE + cmdstr + crcstr + b'>')
-
-    def _serialise_config(self):
-        """Convert current decoder setting into a config string"""
-        obuf = bytearray(CONFIG_LEN)
-        # fill in level bytes
-        obuf[CONFIG_SPARE] = 0x13  # will be fixed by subsequent levelset
-        obuf[CONFIG_SPARE + 1] = 0x15
-
-        # fill in tone values
-        for opt in [
-                CONFIG_TONE_STA, CONFIG_TONE_BOX, CONFIG_TONE_MAN,
-                CONFIG_TONE_CEL, CONFIG_TONE_BXX
-        ]:
-            if opt in self._decoderconfig:
-                obuf[opt] = val2hexval(self._decoderconfig[opt] // 100)  # xx00
-                obuf[opt + 1] = val2hexval(self._decoderconfig[opt] %
-                                           100)  # 00xx
-
-        # fill in single byte values
-        for opt in [
-                CONFIG_TZ_HOUR, CONFIG_TZ_MIN, CONFIG_PROT, CONFIG_PULSEINT,
-                CONFIG_CELLTOD_HOUR, CONFIG_CELLTOD_MIN
+    def printer(self, enable=False):
+        """Enable or disable Timy printer."""
+        cmd = '0'
+        if enable:
+            cmd = '1'
+        self.__cqueue.put_nowait(('MSG', 'PRINTER' + cmd + '\r'))
+
+    def printimp(self, doprint=True):
+        """Enable or disable automatic printing of timing impulses."""
+        cmd = '1'
+        if doprint:
+            cmd = '0'
+        self.__cqueue.put_nowait(('MSG', 'PRIIGN' + cmd + '\r'))
+
+    def keylock(self, setlock=True):
+        """Set or clear Timy keypad lock function."""
+        cmd = '1'
+        if not setlock:
+            cmd = '0'
+        self.__cqueue.put_nowait(('MSG', 'KL' + cmd + '\r'))
+
+    def write(self, msg=None):
+        """Queue a raw command string to attached Timy."""
+        self.__cqueue.put_nowait(('MSG', msg.rstrip() + '\r'))
+
+    def exit(self, msg=None):
+        """Request thread termination."""
+        self.running = False
+        self.__cqueue.put_nowait(('EXIT', msg))
+
+    def setport(self, device=None):
+        """Request (re)opening serial port as specified.
+
+        Call setport with None or an empty string to close an open port
+        or to run the Timy thread with no external device.
+
+        """
+        self.__cqueue.put_nowait(('PORT', device))
+
+    def arm(self, channel=0):
+        """Arm channel 0 - 8 for timing impulses."""
+        chan = chan2id(channel)
+        _log.debug('Arming channel %s', id2chan(chan))
+        self.__arms[chan] = True
+
+    def dearm(self, channel=0):
+        """Disarm channel 0 - 8."""
+        chan = chan2id(channel)
+        _log.debug('De-arm channel %s', id2chan(chan))
+        self.__arms[chan] = False
+
+    def armlock(self, lock=True):
+        """Set or clear the arming lock."""
+        self.__armlocked = bool(lock)
+        _log.debug('Armlock is now %s', self.__armlocked)
+
+    def sane(self):
+        """Initialise Timy to 'sane' values.
+
+        Values set by sane():
+
+            TIMIYINIT		- initialise
+            KL0			- keylock off
+	    CHK1		- enable "checksum"
+	    PRE4		- 10,000th sec precision
+	    RR0			- Round by 'cut'
+	    BE1			- Beep on
+	    DTS02.00		- Start delay 2.0
+	    DTF02.00		- Finish & intermediate delay 2.0
+	    EMU0		- Running time off
+	    PRINTER0		- Printer off
+	    PRIIGN1		- Don't print all impulses to receipt
+            SL0			- Logo off
+	    PRILF		- Linefeed
+	
+        All commands are queued individually to the command thread
+        so it may be necessary to use wait() to suspend the calling
+        thread until all the commands are sent:
+
+            t.start()
+	    t.sane()
+	    t.wait()
+    
+        Note: "sane" here comes from use at track meets with the
+              trackmeet program. It may not always make sense eg, to
+              have all channel delays set to 2 seconds, or to have
+              the internal impulse print off by default.
+
+        """
+        for msg in [
+                'TIMYINIT', 'NSF?', 'PROG?', 'KL0', 'CHK1', 'PRE4', 'RR0',
+                'BE1', 'DTS02.00', 'DTF02.00', 'EMU0', 'PRINTER0', 'PRIIGN1',
+                'SL0', 'PRILF'
         ]:
-            if opt in self._decoderconfig:
-                obuf[opt] = val2hexval(self._decoderconfig[opt] % 100)  # ??
+            self.write(msg)
 
-        # fill in flags
-        for opt in [
-                CONFIG_TOD, CONFIG_GPS, CONFIG_485, CONFIG_FIBRE, CONFIG_PRINT,
-                CONFIG_MAX, CONFIG_PULSE, CONFIG_CELLSYNC, CONFIG_ACTIVE_LOOP
-        ]:
-            if opt in self._decoderconfig:
-                if self._decoderconfig[opt]:
-                    obuf[opt] = 0x01
-        return bytes(obuf)
-
-    def _set_config(self):
-        """Write current configuration to decoder."""
-        cmd = b'\x08\x08' + self._serialise_config()
-        self._v3_cmd(cmd)
-        self._write(QUECMD)
-
-    def _set_date(self, timestruct=None):
-        """Set the date on the decoder."""
-        if timestruct is None:
-            timestruct = time.localtime()
-        _log.debug('Set date on decoder: %s',
-                   time.strftime('%Y-%m-%d', timestruct))
-        cmd = bytearray(5)
-        cmd[0] = 0x0a
-        cmd[1] = 0x0a
-        cmd[2] = 0xff & timestruct[2]  # day
-        cmd[3] = 0xff & timestruct[1]  # month
-        cmd[4] = 0xff & (timestruct[0] - 2000)  # year, after 2000
-        self._v3_cmd(bytes(cmd))
-
-    def _setlvl(self, box='10', sta='10'):
-        """Set the read level on box and sta channels."""
-        # TODO: verify opts
-        self.write(BOXLVL + box.encode(THBC_ENCODING))
-        self.write(STALVL + sta.encode(THBC_ENCODING))
-
-    def _set_time_cmd(self, t):
-        """Return a set time command string for the provided time of day."""
-        body = bytearray(4)
-        s = int(t.timeval)
-        body[0] = s // 3600  # hours
-        body[1] = (s // 60) % 60  # minutes
-        body[2] = s % 60  # seconds
-        body[3] = 0x74
-        return SETTIME + bytes(body)
-
-    def _parse_config(self, msg):
-        # decoder configuration message.
-        ibuf = bytearray(msg)
-        self._decoderconfig = {}
-        for flag in sorted(CONFIG_FLAGS):  # import all
-            # tone values
-            if flag in [
-                    CONFIG_TONE_STA, CONFIG_TONE_BOX, CONFIG_TONE_MAN,
-                    CONFIG_TONE_CEL, CONFIG_TONE_BXX
-            ]:
-                self._decoderconfig[flag] = 100 * hexval2val(ibuf[flag])
-                self._decoderconfig[flag] += hexval2val(ibuf[flag + 1])
-
-            # single byte values
-            elif flag in [
-                    CONFIG_TZ_HOUR, CONFIG_TZ_MIN, CONFIG_PROT,
-                    CONFIG_PULSEINT, CONFIG_CELLTOD_HOUR, CONFIG_CELLTOD_MIN
-            ]:
-                self._decoderconfig[flag] = hexval2val(ibuf[flag])
-
-            # 'booleans'
-            elif flag in [
-                    CONFIG_TOD, CONFIG_GPS, CONFIG_485, CONFIG_FIBRE,
-                    CONFIG_PRINT, CONFIG_MAX, CONFIG_PULSE, CONFIG_CELLSYNC,
-                    CONFIG_ACTIVE_LOOP
-            ]:
-                self._decoderconfig[flag] = bool(ibuf[flag])
-
-        self._boxname = ''
-        for c in msg[43:47]:
-            self._boxname += chr(c + ord('0'))
-        self._version = str(hexval2val(ibuf[47]))
-        stalvl = hexval2val(msg[25])
-        boxlvl = hexval2val(msg[26])
-        _log.info('Info Decoder ID: %s', self._boxname)
-        _log.debug('Info Firmware Version: %r', self._version)
-        _log.debug('Levels: STA=%r, BOX=%r', stalvl, boxlvl)
-        self._decoderipconfig['IP'] = socket.inet_ntoa(msg[27:31])
-        self._decoderipconfig['Mask'] = socket.inet_ntoa(msg[31:35])
-        self._decoderipconfig['Gateway'] = socket.inet_ntoa(msg[35:39])
-        self._decoderipconfig['Host'] = socket.inet_ntoa(msg[39:43])
-        for key in ['IP', 'Mask', 'Gateway', 'Host']:
-            _log.debug('%r: %r', key, self._decoderipconfig[key])
+    def wait(self):
+        """Wait for Timy thread to finish processing any queued commands."""
+        self.__cqueue.join()
 
-    def _parse_message(self, msg, ack=True):
+    def __parse_message(self, msg):
         """Return tod object from timing msg or None."""
         ret = None
-        if len(msg) > 4:
-            if msg[0] == PASSSTART[0]:  # RFID message
-                idx = msg.find(b'>')
-                if idx == 37:  # Valid length
-                    data = msg[1:33]
-                    msum = msg[33:37]
-                    tsum = thbc_sum(data)
-                    if tsum == msum:  # Valid 'sum'
-                        pvec = data.decode(THBC_ENCODING).split()
-                        istr = pvec[3] + ':' + pvec[5]
-                        rstr = pvec[1].lstrip('0')
-                        cstr = 'C1'
-                        if pvec[0] == 'BOX':
-                            cstr = 'C2'
-                        elif pvec[0] == 'MAN':
-                            cstr = 'C0'
-                        if pvec[5] == '3':  # LOW BATTERY ALERT
-                            _log.warning('Low battery on %r', rstr)
-                        ret = tod.tod(pvec[2],
-                                      index=istr,
-                                      chan=cstr,
-                                      refid=rstr,
-                                      source=self._boxname)
-                        # Log a hardware-specific passing
-                        _log.log(DECODER_LOG_LEVEL, msg.strip())
-                        if ack:
-                            self._write(ACKCMD)  # Acknowledge if ok
-                        self._cksumerr = 0
+        msg = msg.rstrip()  # remove cr/lf if present
+        tsum = 0
+        csum = 0
+
+        if msg == 'CLR':
+            self.__cqueue.put_nowait(('RCLR', ''))
+            _log.debug('RCLR Ack')
+        elif msg.startswith('HW_SN'):
+            _log.info('%r connected', msg.split()[-1])
+        elif msg.startswith('NSF'):
+            _log.info('Version: %r', msg.replace('NSF', ''))
+        elif msg.startswith('PROG:'):
+            _log.debug('Program: %r', msg.split()[-1])
+        elif msg.startswith('PULSE HOLD:'):
+            _log.warning('Pulse hold: %s', msg.split('][')[1])
+        else:
+            if len(msg) == 28:
+                # assume checksum present, grab it and truncate msg
+                tsum = _timy_getsum(msg[26:28])
+                msg = msg[0:26]
+                csum = _timy_checksum(msg)
+            if len(msg) == 26:
+                # assume now msg is a timing impulse
+                if tsum == csum:
+                    e = msg.split()
+                    if len(e) == 4:
+                        cid = chan2id(e[1])
+                        ret = tod.mktod(e[2])
+                        if ret is not None:
+                            if cid in self.__chandelay:
+                                # note: ret might wrap over 24hr boundary
+                                ret = ret - self.__chandelay[cid]
+                            ret.index = e[0]
+                            ret.chan = e[1]
+                            ret.refid = ''
+                            ret.source = self.__name
+                        else:
+                            _log.error('Invalid message: %s', msg)
                     else:
-                        _log.warning('Invalid checksum: %r != %r: %r', tsum,
-                                     msum, msg)
-                        self._cksumerr += 1
-                        if self._cksumerr > 3:
-                            # assume error on decoder, so acknowledge and
-                            # continue with log
-                            # NOTE: This path is triggered when serial comms
-                            # fail and a tag read happens before a manual trig
-                            _log.error('Erroneous message from decoder')
-                            if ack:
-                                self._write(ACKCMD)
-                else:
-                    _log.debug('Invalid message: %r', msg)
-            elif msg[0] == STATSTART:  # Status message
-                data = msg[1:22]
-                pvec = data.decode(THBC_ENCODING).split()
-                if len(pvec) == 5:
-                    _log.info('%r@%s Noise:%s/%s Levels:%s/%s', self._boxname,
-                              pvec[0], pvec[1], pvec[2], pvec[3], pvec[4])
+                        _log.error('Invalid message: %s', msg)
                 else:
-                    _log.info('Invalid status: %r', msg)
-            elif b'+++' == msg[0:3] and len(msg) > 53:
-                self._parse_config(msg[3:])
-            else:
-                pass
-        else:
-            _log.debug('Short message: %r', msg)
+                    _log.warning('Corrupt message: %s', msg)
+                    _log.debug('Checksum fail: 0x%02X != 0x%02X', tsum, csum)
         return ret
 
-    def _ipcompletion(self):
-        """Blocking wait for ipconfig completion - horrible."""
-        _log.info('IP Config')
-        time.sleep(10)
-        self.write(QUECMD)
-
-    def _read(self):
-        """Read messages from the decoder until a timeout condition."""
-        ch = self._io.read(1)
+    def __proc_impulse(self, st):
+        """Process a parsed tod impulse from the Timy.
+
+        On reception of a timing channel message, the channel is
+        compared against the list of armed channels. If the channel
+        is armed, the callback is run.
+
+        If arm lock is not set, the channel is then de-armed.
+        """
+        _log.log(_TIMER_LOG_LEVEL, st)
+        channo = chan2id(st.chan)
+        if channo != _CHAN_UNKNOWN:
+            if self.__arms[channo]:
+                self.__cb(st)
+                if not self.__armlocked:
+                    self.__arms[channo] = False
+            if st.index.isdigit():
+                index = int(st.index)
+                if index > 2000 and not self.__clearing:
+                    self.__clearing = True
+                    self.clrmem()
+                    _log.debug('Auto clear memory')
+        else:
+            pass
+        return False
+
+    def __read(self):
+        """Read messages from timy until a timeout condition."""
+        ch = self.__port.read(1)
+        mcnt = 0
         while ch != b'':
-            if ch == LF and len(self._rdbuf) > 0 and self._rdbuf[-1] == CR[0]:
-                # Return ends the current 'message', if preceeded by return
-                self._rdbuf += ch  # include trailing newline
-                #_log.debug('RECV: %r', self._rdbuf)
-                t = self._parse_message(self._rdbuf.lstrip(b'\0'))
+            if ch == _CR:
+                # Return ends the current 'message'
+                self.__rdbuf += ch  # include trailing <cr>
+                msg = self.__rdbuf.decode(_ENCODING, 'ignore')
+                #_log.debug('RECV: %r', msg)
+                t = self.__parse_message(msg)
                 if t is not None:
-                    self._trig(t)
-                self._rdbuf = b''
-            elif len(self._rdbuf) > 40 and b'\x1e\x86\x98' in self._rdbuf:
-                # Assume acknowledge from IP Command
-                #_log.debug('RECV: %r', self._rdbuf)
-                self._rdbuf = b''
-                self._ipcompletion()
+                    self.__proc_impulse(t)
+                self.__rdbuf = b''
+                mcnt += 1
+                if mcnt > 4:  # break to allow write back
+                    return
             else:
-                self._rdbuf += ch
-            ch = self._io.read(1)
-
-    def _write(self, msg):
-        if self._io is not None:
-            self._io.write(msg)
-            #_log.debug('SEND: %r', msg)
+                self.__rdbuf += ch
+            ch = self.__port.read(1)
 
     def run(self):
-        """Decoder main loop."""
+        """Run the Timy thread.
+
+           Called by invoking thread method: timy.start()
+        """
+        running = True
         _log.debug('Starting')
-        self._running = True
-        while self._running:
+        while running:
             try:
-                c = None
-                if self._io is not None:
-                    # Read responses until response complete or timeout
-                    try:
-                        self._read()
-                    except socket.timeout:
+                # Read phase
+                if self.__port is not None:
+                    self.__read()
+                    m = self.__cqueue.get_nowait()
+                else:
+                    m = self.__cqueue.get()
+                self.__cqueue.task_done()
+
+                # Write phase
+                if isinstance(m, tuple) and m[0] in _TCMDS:
+                    if m[0] == 'MSG':
+                        if self.__port is not None and not self.error:
+                            #_log.debug('SEND: %r', m[1])
+                            self.__port.write(m[1].encode(_ENCODING, 'ignore'))
+                    elif m[0] == 'TRIG':
+                        if isinstance(m[1], tod.tod):
+                            self.__proc_impulse(m[1])
+                    elif m[0] == 'RCLR':
+                        self.__clearing = False
+                    elif m[0] == 'EXIT':
+                        _log.debug('Request to close: %s', m[1])
+                        running = False
+                    elif m[0] == 'PORT':
+                        if self.__port is not None:
+                            self.__port.close()
+                            self.__port = None
+                        if m[1] is not None and m[1] not in [
+                                '', 'NULL', 'None'
+                        ]:
+                            _log.debug('Re-Connect port: %s @ %d', m[1],
+                                       self.__baudrate)
+                            self.__port = serial.Serial(m[1],
+                                                        self.__baudrate,
+                                                        rtscts=self.__ctsrts,
+                                                        timeout=0.2)
+                            self.error = False
+                        else:
+                            _log.debug('Not connected')
+                            self.error = True
+                    else:
                         pass
-                    c = self._cqueue.get_nowait()
                 else:
-                    c = self._cqueue.get()
-                self._cqueue.task_done()
-                self._proccmd(c)
+                    _log.warning('Unknown message: %r', m)
             except queue.Empty:
                 pass
-            except (serial.SerialException, socket.error) as e:
-                self._close()
-                self._boxname = None
-                _log.error('%s: %s', e.__class__.__name__, e)
+            except serial.SerialException as e:
+                if self.__port is not None:
+                    self.__port.close()
+                    self.__port = None
+                self.error = True
+                _log.error('Serial error: %s', e)
             except Exception as e:
-                _log.critical('%s: %s', e.__class__.__name__, e)
-                self._boxname = None
-                self._running = False
-        self.setcb()
-        _log.debug('Exiting')
-
-
-class dgram:
-    """Serial-like UDP port object."""
-
-    def __init__(self, host, port):
-        self._host = host
-        self._port = port
-        self._s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        self._s.settimeout(0.2)
-        self._s.bind(('', self._port))
-        self._buf = b''
-
-    def read(self, sz=1):
-        ret = b''
-        if len(self._buf) == 0:
-            nb, addr = self._s.recvfrom(4096)  # timeout raises exception
-            if addr[0] == self._host:
-                self._buf += nb
-        if len(self._buf) > 0:
-            # make sure ret is bytes
-            ret = self._buf[0:1]
-            self._buf = self._buf[1:]
-        return ret
-
-    def write(self, buf=b''):
-        return self._s.sendto(buf, (self._host, self._port))
-
-    def close(self):
-        self._s.close()
+                _log.error('%s: %s', e.__class__.__name__, e)
+                self.error = True
+        if self.__port is not None:
+            self.__port.close()
+            self.__port = None
+        _log.info('Exiting')
```

### Comparing `metarace-2.1.2/src/metarace/eventdb.py` & `metarace-2.1.3/src/metarace/eventdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 import os
 import csv
 
 import metarace
 from metarace import strops
 
-_log = logging.getLogger('metarace.eventdb')
+_log = logging.getLogger('eventdb')
 _log.setLevel(logging.DEBUG)
 
 # Note: These are for the trackmeet module, roadmeet re-defines race types
 defracetypes = [
     'sprint',
     'keirin',
     'flying 200',
```

### Comparing `metarace-2.1.2/src/metarace/htlib.py` & `metarace-2.1.3/src/metarace/htlib.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.2/src/metarace/report.py` & `metarace-2.1.3/src/metarace/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import logging
 import metarace
 from metarace import tod
 from metarace import strops
 from metarace import htlib
 from metarace import jsonconfig
 
-_log = logging.getLogger('metarace.report')
+_log = logging.getLogger('report')
 _log.setLevel(logging.DEBUG)
 
 # JSON report API versioning
 APIVERSION = '1.2.0'
 
 # xls cell styles
 XS_LEFT = xlwt.easyxf()
@@ -76,15 +76,20 @@
 
 
 def pt2pt(pt=1):
     """Dummy conversion."""
     return pt
 
 
-# raw defaults
+# Transitional baseline position - to be replaced with font metrics
+_CELL_BASELINE = 0.715
+
+# defaults
+PANGO_SCALE = float(Pango.SCALE)
+PANGO_INVSCALE = 1.0 / float(Pango.SCALE)
 FEPSILON = 0.0001  # float epsilon
 BODYFONT = 'serif 7.0'  # body text
 BODYOBLIQUE = 'serif italic 7.0'  # body text oblique
 BODYBOLDFONT = 'serif bold 7.0'  # bold body text
 BODYSMALL = 'serif 6.0'  # small body text
 MONOSPACEFONT = 'monospace Bold 7.0'  # monospaced text
 SECTIONFONT = 'sans-serif Bold 7.0'  # section headings
@@ -3686,15 +3691,14 @@
         self.fill = fill
         self.width = width
         self.colour = colour
         self.dash = dash
 
     def draw(self, c, p):
         c.save()
-        #c.move_to(self.cx, self.cy)
         c.new_sub_path()
         c.arc(self.cx, self.cy, self.r, self.a1, self.a2)
         outline = False
         if self.width is not None:
             outline = True
             c.set_line_width(self.width)
         if self.fill is not None:
@@ -4856,22 +4860,29 @@
         if zebra:
             self.drawbox(self.body_left - mm2pt(1), h,
                          self.body_right + mm2pt(1), h + self.line_height,
                          0.07)
         omap = vecmap(rvec, 9)
         strikeright = self.col_oft_rank
         if omap[0]:
-            if not omap[8]:  # Photo-finish
+            if omap[8]:  # Photo-finish
+                font = self.fonts['bodysmall']
+                self.text_left(self.col_oft_rank, h, '\U0001f4f7', font)
+            elif omap[0] == '____':
+                font = self.fonts['body']
+                self.text_left(self.col_oft_rank,
+                               h,
+                               '\u3000' * 2,
+                               font,
+                               underline=True)
+            else:
                 font = self.fonts['body']
                 if not omap[7]:  # Placed
                     font = self.fonts['bodyoblique']
                 self.text_left(self.col_oft_rank, h, omap[0], font)
-            else:
-                font = self.fonts['bodysmall']
-                self.text_left(self.col_oft_rank, h, '\U0001f4f7', font)
         if omap[1]:
             self.text_right(self.col_oft_no, h, omap[1], self.fonts['body'])
             strikeright = self.col_oft_rank
         if omap[2]:
             maxnamew = (self.col_oft_cat - mm2pt(35.0)) - self.col_oft_name
             (tw, th) = self.fit_text(self.col_oft_name,
                                      h,
@@ -4920,15 +4931,15 @@
                            fonts['key'])
         if data is not None:
             if data['name']:
                 self.fit_text(x + 0.4 * width,
                               h + (0.05 * height),
                               data['name'],
                               0.55 * width,
-                              align=1.0,
+                              right=True,
                               font=fonts['text'])
             if data['gcline']:
                 self.text_right(x + width - mm2pt(1.0), h + (0.30 * height),
                                 data['gcline'], fonts['gcline'])
             if data['ltext']:
                 self.text_left(x + mm2pt(0.5), h + (0.66 * height),
                                data['ltext'], fonts['text'])
@@ -5188,33 +5199,14 @@
             doline = False
         if doline:
             self.drawline(w + mm2pt(8.0), baseline, w + mm2pt(60), baseline)
         if len(rvec) > 3 and rvec[3]:  # cat/hcap/draw/etc
             self.text_left(w + mm2pt(62.0), h, rvec[3],
                            self.fonts['bodyoblique'])
 
-    def text_right(self,
-                   w,
-                   h,
-                   msg,
-                   font=None,
-                   strikethrough=False,
-                   maxwidth=None):
-        l = Pango.Layout.new(self.p)
-        l.set_alignment(Pango.Alignment.RIGHT)
-        if font is not None:
-            l.set_font_description(font)
-        l.set_text(msg, -1)
-        (tw, th) = l.get_pixel_size()
-        self.c.move_to(w - tw, h)
-        PangoCairo.update_context(self.c, self.p)
-        l.context_changed()
-        PangoCairo.show_layout(self.c, l)
-        return (tw, th)
-
     def drawbox(self, x1, y1, x2, y2, alpha=0.1):
         self.c.save()
         self.c.set_source_rgba(0.0, 0.0, 0.0, alpha)
         self.c.move_to(x1, y1)
         self.c.line_to(x2, y1)
         self.c.line_to(x2, y2)
         self.c.line_to(x1, y2)
@@ -5231,109 +5223,234 @@
         self.c.restore()
 
     def fit_text(self,
                  w,
                  h,
                  msg,
                  maxwidth,
-                 align=0,
+                 right=False,
                  font=None,
-                 strikethrough=False):
-        if msg is not None:
-            self.c.save()
+                 strikethrough=False,
+                 underline=False):
+        tw = 0
+        th = self.line_height
+        if msg:
+            baseline = _CELL_BASELINE * self.line_height
             l = Pango.Layout.new(self.p)
-            l.set_alignment(Pango.Alignment.LEFT)
+            if right:
+                l.set_alignment(Pango.Alignment.RIGHT)
+                l.set_ellipsize(Pango.EllipsizeMode.START)
+            else:
+                l.set_alignment(Pango.Alignment.LEFT)
+                l.set_ellipsize(Pango.EllipsizeMode.END)
             if font is not None:
                 l.set_font_description(font)
+
+            l.set_wrap(Pango.WrapMode.WORD_CHAR)
             l.set_text(msg, -1)
-            (tw, th) = l.get_pixel_size()
-            oft = 0.0
-            if align != 0 and tw < maxwidth:
-                oft = align * (maxwidth - tw)  # else squish
-            self.c.move_to(w + oft,
-                           h)  # move before applying conditional scale
-            if tw > maxwidth:
-                self.c.scale(float(maxwidth) / float(tw), 1.0)
-                tw = maxwidth
+            l.set_width(int(maxwidth * PANGO_SCALE))
+            l.set_height(0)
+            intr, logr = l.get_extents()
+            fnbaseline = l.get_baseline() * PANGO_INVSCALE
+            thof = logr.y * PANGO_INVSCALE
+            twof = logr.x * PANGO_INVSCALE
+            tw = logr.width * PANGO_INVSCALE
+            th = logr.height * PANGO_INVSCALE
+            oft = w + twof
+            if right:
+                oft = w - (tw + twof)
+            self.c.move_to(oft, h + (baseline - fnbaseline) + thof)
             PangoCairo.update_context(self.c, self.p)
             l.context_changed()
             PangoCairo.show_layout(self.c, l)
+
+            metrics = None
+            if strikethrough or underline:
+                metrics = l.get_context().get_metrics(font)
             if strikethrough:
-                self.drawline(w, h + (0.85 * th), w + tw, h + (0.15 * th))
-            self.c.restore()
-            return (tw, th)
+                strikethick = metrics.get_strikethrough_thickness(
+                ) * PANGO_INVSCALE
+                strikeoft = baseline - metrics.get_strikethrough_position(
+                ) * PANGO_INVSCALE
+                sth = h + strikeoft - 0.5 * strikethick
+                self.drawline(oft, sth, oft + tw, sth, strikethick)
+            if underline:
+                underthick = metrics.get_underline_thickness() * PANGO_INVSCALE
+                underoft = baseline - metrics.get_underline_position(
+                ) * PANGO_INVSCALE
+                uth = h + underoft - 0.5 * underthick
+                self.drawline(oft, uth, oft + tw, uth, underthick)
+        return (tw, th)
+
+    def placemark(self, w, h):
+        """Draw a crosshair mark at w,h"""
+        self.drawline(w, h - 2.5, w, h + 2.5, 0.10)
+        self.drawline(w - 2.5, h, w + 2.5, h, 0.10)
+        self.c.save()
+        self.c.set_line_width(0.10)
+        self.c.new_sub_path()
+        self.c.arc(w, h, 1.0, 0.0, 2.0 * math.pi)
+        self.c.stroke()
+        self.c.restore()
+
+    def text_right(self,
+                   w,
+                   h,
+                   msg,
+                   font=None,
+                   strikethrough=False,
+                   maxwidth=None,
+                   underline=False):
+        # TODO: replace with text_cell
+        tw = 0
+        th = self.line_height
+        if msg:
+            baseline = _CELL_BASELINE * self.line_height
+
+            l = Pango.Layout.new(self.p)
+            l.set_alignment(Pango.Alignment.RIGHT)
+            if font is not None:
+                l.set_font_description(font)
+            l.set_text(msg, -1)
+            intr, logr = l.get_extents()
+            fnbaseline = l.get_baseline() * PANGO_INVSCALE
+            thof = logr.y * PANGO_INVSCALE
+            twof = logr.x * PANGO_INVSCALE
+            tw = logr.width * PANGO_INVSCALE
+            th = logr.height * PANGO_INVSCALE
+            oft = w - (tw + twof)
+            self.c.move_to(oft, h + (baseline - fnbaseline) + thof)
+            PangoCairo.update_context(self.c, self.p)
+            l.context_changed()
+            PangoCairo.show_layout(self.c, l)
+
+            metrics = None
+            if underline or strikethrough:
+                metrics = l.get_context().get_metrics(font)
+            if strikethrough:
+                strikethick = metrics.get_strikethrough_thickness(
+                ) * PANGO_INVSCALE
+                strikeoft = baseline - metrics.get_strikethrough_position(
+                ) * PANGO_INVSCALE
+                sth = h + strikeoft - 0.5 * strikethick
+                self.drawline(oft, sth, oft + tw, sth, strikethick)
+            if underline:
+                underthick = metrics.get_underline_thickness() * PANGO_INVSCALE
+                underoft = baseline - metrics.get_underline_position(
+                ) * PANGO_INVSCALE
+                uth = h + underoft - 0.5 * underthick
+                self.drawline(oft, uth, oft + tw, uth, underthick)
+        return (tw, th)
 
     def text_left(self,
                   w,
                   h,
                   msg,
                   font=None,
                   strikethrough=False,
-                  maxwidth=None):
-        l = Pango.Layout.new(self.p)
-        l.set_alignment(Pango.Alignment.LEFT)
-        if font is not None:
-            l.set_font_description(font)
-        l.set_text(msg, -1)
-        (tw, th) = l.get_pixel_size()
-        self.c.move_to(w, h)
-        PangoCairo.update_context(self.c, self.p)
-        l.context_changed()
-        PangoCairo.show_layout(self.c, l)
-        if strikethrough:
-            self.drawline(w, h + (th / 2), w + tw, h + (th / 2))
+                  maxwidth=None,
+                  underline=False):
+        # TODO: replace with text_cell
+        tw = 0
+        th = self.line_height
+        if msg:
+            baseline = _CELL_BASELINE * self.line_height
+
+            l = Pango.Layout.new(self.p)
+            l.set_alignment(Pango.Alignment.LEFT)
+            if font is not None:
+                l.set_font_description(font)
+            l.set_text(msg, -1)
+            intr, logr = l.get_extents()
+            fnbaseline = l.get_baseline() * PANGO_INVSCALE
+            thof = logr.y * PANGO_INVSCALE
+            twof = logr.x * PANGO_INVSCALE
+            tw = logr.width * PANGO_INVSCALE
+            th = logr.height * PANGO_INVSCALE
+            oft = w + twof
+            self.c.move_to(oft, h + (baseline - fnbaseline) + thof)
+            PangoCairo.update_context(self.c, self.p)
+            l.context_changed()
+            PangoCairo.show_layout(self.c, l)
+
+            metrics = None
+            if underline or strikethrough:
+                metrics = l.get_context().get_metrics(font)
+            if strikethrough:
+                strikethick = metrics.get_strikethrough_thickness(
+                ) * PANGO_INVSCALE
+                strikeoft = baseline - metrics.get_strikethrough_position(
+                ) * PANGO_INVSCALE
+                sth = h + strikeoft - 0.5 * strikethick
+                self.drawline(oft, sth, oft + tw, sth, strikethick)
+            if underline:
+                underthick = metrics.get_underline_thickness() * PANGO_INVSCALE
+                underoft = baseline - metrics.get_underline_position(
+                ) * PANGO_INVSCALE
+                uth = h + underoft - 0.5 * underthick
+                self.drawline(oft, uth, oft + tw, uth, underthick)
         return (tw, th)
 
     def text_para(self,
                   w,
                   h,
                   text,
                   font=None,
                   width=None,
                   halign=Pango.Alignment.LEFT):
-        if width is None:
-            width = self.body_width
-        l = Pango.Layout.new(self.p)
-        if font is not None:
-            l.set_font_description(font)
-        l.set_width(int(Pango.SCALE * width + 1))
-        l.set_wrap(Pango.WrapMode.WORD_CHAR)
-        l.set_alignment(halign)
-        l.set_text(text, -1)
-        (tw, th) = l.get_pixel_size()
-        self.c.move_to(w, h)
-        PangoCairo.update_context(self.c, self.p)
-        l.context_changed()
-        PangoCairo.show_layout(self.c, l)
+        tw = 0
+        th = self.line_height
+        if text:
+            if width is None:
+                width = self.body_width
+            l = Pango.Layout.new(self.p)
+            if font is not None:
+                l.set_font_description(font)
+            l.set_width(int(Pango.SCALE * width + 1))
+            l.set_wrap(Pango.WrapMode.WORD_CHAR)
+            l.set_alignment(halign)
+            l.set_text(text, -1)
+            (tw, th) = l.get_pixel_size()
+            self.c.move_to(w, h)
+            PangoCairo.update_context(self.c, self.p)
+            l.context_changed()
+            PangoCairo.show_layout(self.c, l)
         return (tw, th)
 
     def text_cent(self, w, h, msg, font=None, halign=Pango.Alignment.CENTER):
-        l = Pango.Layout.new(self.p)
-        l.set_alignment(halign)
-        if font is not None:
-            l.set_font_description(font)
-        l.set_text(msg, -1)
-        (tw, th) = l.get_pixel_size()
-        self.c.move_to(w - (0.5 * tw), h)
-        PangoCairo.update_context(self.c, self.p)
-        l.context_changed()
-        PangoCairo.show_layout(self.c, l)
+        # TODO: Replace with text_box
+        tw = 0
+        th = self.line_height
+        if msg:
+            l = Pango.Layout.new(self.p)
+            l.set_alignment(halign)
+            if font is not None:
+                l.set_font_description(font)
+            l.set_text(msg, -1)
+            (tw, th) = l.get_pixel_size()
+            self.c.move_to(w - (0.5 * tw), h)
+            PangoCairo.update_context(self.c, self.p)
+            l.context_changed()
+            PangoCairo.show_layout(self.c, l)
         return (tw, th)
 
     def text_path(self, w, h, msg, font=None):
-        l = Pango.Layout.new(self.p)
-        if font is not None:
-            l.set_font_description(font)
-        l.set_text(msg, -1)
-        (tw, th) = l.get_pixel_size()
-        self.c.move_to(w - (0.5 * tw), h)
-        PangoCairo.update_context(self.c, self.p)
-        l.context_changed()
-        PangoCairo.layout_path(self.c, l)
-        self.c.fill()
+        tw = 0
+        th = self.line_height
+        if msg:
+            l = Pango.Layout.new(self.p)
+            if font is not None:
+                l.set_font_description(font)
+            l.set_text(msg, -1)
+            (tw, th) = l.get_pixel_size()
+            self.c.move_to(w - (0.5 * tw), h)
+            PangoCairo.update_context(self.c, self.p)
+            l.context_changed()
+            PangoCairo.layout_path(self.c, l)
+            self.c.fill()
         return (tw, th)
 
     def draw_provisional(self):
         self.c.save()
         self.c.set_source_rgb(1.0, 1.0, 1.0)
         self.text_cent(self.midpagew, self.body_top - mm2pt(5), 'PROVISIONAL',
                        self.fonts['body'])
```

### Comparing `metarace-2.1.2/src/metarace/riderdb.py` & `metarace-2.1.3/src/metarace/riderdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import csv
 from unicodedata import normalize
 import grapheme
 
 import metarace
 from metarace import strops
 
-_log = logging.getLogger('metarace.riderdb')
+_log = logging.getLogger('riderdb')
 _log.setLevel(logging.DEBUG)
 
 # default values when columns omitted
 _RIDER_DEFAULTS = {}
 
 # Rider column headings
 _RIDER_COLUMNS = {
@@ -55,84 +55,96 @@
         'control': 'section',
     },
     'no': {
         'prompt': 'Rider No:',
         'control': 'short',
         'attr': 'no',
         'defer': True,
+        'default': '',
     },
     'series': {
         'prompt': 'Series:',
         'control': 'short',
         'attr': 'series',
         'defer': True,
+        'default': '',
     },
     'first': {
         'prompt': 'First Name:',
         'attr': 'first',
         'defer': True,
+        'default': '',
     },
     'last': {
         'prompt': 'Last Name:',
         'attr': 'last',
         'defer': True,
+        'default': '',
     },
     'org': {
         'prompt': 'Organisation:',
         'attr': 'org',
         'defer': True,
         'hint': 'Club or team affiliation',
+        'default': '',
     },
     'cat': {
         'prompt': 'Categories:',
         'attr': 'cat',
         'defer': True,
         'hint': 'Space separated list of categories',
+        'default': '',
     },
     'nat': {
         'prompt': 'Nationality:',
         'attr': 'nat',
         'defer': True,
         'hint': '3 letter IOC country code eg: AUS, GBR, JPN',
         'control': 'short',
+        'default': '',
     },
     'ref': {
         'prompt': 'Transponder:',
         'attr': 'ref',
         'defer': True,
         'control': 'short',
+        'default': '',
     },
     'uci': {
         'prompt': 'UCI ID:',
         'attr': 'uci',
         'defer': True,
         'control': 'short',
         'hint': '11 digit UCI ID',
+        'default': '',
     },
     'dob': {
         'prompt': 'Date of Birth:',
         'attr': 'dob',
         'control': 'short',
         'defer': True,
         'subtext': '(YYYY-MM-DD)',
         'hint': 'ISO8601 Date of birth eg: 2012-01-25',
+        'default': '',
     },
     'sex': {
         'prompt': 'Sex:',
         'control': 'short',
         'subtext': '(Male|Female)',
         'defer': True,
         'hint': 'Sex of participant',
         'attr': 'sex',
+        'default': '',
     },
     'note': {
         'prompt': 'Notes:',
         'attr': 'note',
         'defer': True,
         'hint': 'Supplementary rider notes',
+        'default': '',
     },
 }
 
 # Config schema for a category
 _CATEGORY_SCHEMA = {
     'rtype': {
         'prompt': 'Category',
@@ -140,140 +152,158 @@
     },
     'no': {
         'prompt': 'ID:',
         'control': 'short',
         'attr': 'no',
         'hint': 'Category ID or handicap group',
         'defer': True,
+        'default': '',
     },
     'series': {
         'prompt': 'Series:',
         'control': 'short',
         'readonly': True,
         'attr': 'series',
         'defer': True,
+        'default': '',
     },
     'first': {
         'prompt': 'Title:',
         'attr': 'first',
         'hint': 'Category title',
         'defer': True,
+        'default': '',
     },
     'last': {
         'prompt': 'Subtitle:',
         'attr': 'last',
         'hint': 'Category subtitle',
         'defer': True,
+        'default': '',
     },
     'note': {
         'prompt': 'Footer:',
         'attr': 'note',
         'defer': True,
         'hint': 'Supplementary footer text for reports',
+        'default': '',
     },
     'uci': {
         'prompt': 'Start Offset:',
         'attr': 'uci',
         'defer': True,
         'control': 'short',
         'hint': 'Start time offset from event start',
+        'default': '',
     },
     'cat': {
         'prompt': 'Target:',
         'attr': 'cat',
         'control': 'short',
         'subtext': 'laps',
         'defer': True,
         'hint': 'Target number of laps for this category',
+        'default': '',
     },
     'ref': {
         'prompt': 'Distance:',
         'attr': 'ref',
         'defer': True,
         'control': 'short',
         'subtext': 'km',
         'hint': 'Category distance override',
+        'default': '',
     },
     'org': {
         'prompt': 'Lap Prefix:',
         'attr': 'org',
         'control': 'short',
         'defer': True,
         'hint': 'Optional category lap prefix',
+        'default': '',
     },
 }
 
 # Config schema for a team
 _TEAM_SCHEMA = {
     'rtype': {
         'prompt': 'Team',
         'control': 'section',
     },
     'no': {
         'prompt': 'Team Code:',
         'control': 'short',
         'attr': 'no',
         'defer': True,
+        'default': '',
     },
     'series': {
         'prompt': 'Series:',
         'control': 'short',
         'readonly': True,
         'attr': 'series',
         'defer': True,
+        'default': '',
     },
     'first': {
         'prompt': 'Name:',
         'attr': 'first',
         'hint': 'Team name',
         'defer': True,
+        'default': '',
     },
     'last': {
         'prompt': 'Short Name:',
         'attr': 'last',
         'control': 'short',
         'subtext': '(~12 characters)',
         'hint': 'Abbreviated team name for reports',
         'defer': True,
+        'default': '',
     },
     'nat': {
         'prompt': 'Nationality:',
         'attr': 'nat',
         'defer': True,
         'hint': '3 letter IOC country code eg: AUS, GBR, JPN',
         'control': 'short',
+        'default': '',
     },
     'uci': {
         'prompt': 'UCI ID:',
         'attr': 'uci',
         'defer': True,
         'control': 'short',
         'hint': 'Team UCI ID',
+        'default': '',
     },
     'sex': {
         'prompt': 'Division:',
         'control': 'short',
         'subtext': '',
         'defer': True,
         'hint': 'UCI division of team eg: WTT WTW PRT',
         'attr': 'sex',
+        'default': '',
     },
     'ref': {
         'prompt': 'Start Time:',
         'attr': 'ref',
         'defer': True,
         'control': 'short',
         'subtext': '(Team TT)',
         'hint': 'Team TT Start Time',
+        'default': '',
     },
     'note': {
         'prompt': 'Notes:',
         'attr': 'note',
         'defer': True,
         'hint': 'Supplementary team notes',
+        'default': '',
     },
 }
 
 # reserved series
 _RESERVED_SERIES = ('spare', 'cat', 'team', 'ds')
 
 # legacy csv file ordering
@@ -437,14 +467,25 @@
         for k in colset:
             if self[k]:
                 iv.append('%s: %s' % (colset[k], self[k]))
             ret = ', '.join(iv)
 
         return ret
 
+    def name_bib(self):
+        """Return rider name with bib and without org."""
+        ret = None
+        nkey = 'nb'
+        if nkey not in self.__strcache:
+            ret = self.get_bibstr() + ' ' + self.fitname(48)
+            self.__strcache[nkey] = ret
+        else:
+            ret = self.__strcache[nkey]
+        return ret
+
     def resname_bib(self):
         """Return rider name formatted for results with bib."""
         ret = None
         nkey = 'rnb'
         if nkey not in self.__strcache:
             ret = self.get_bibstr() + ' ' + self.listname(48)
             self.__strcache[nkey] = ret
```

### Comparing `metarace-2.1.2/src/metarace/strops.py` & `metarace-2.1.3/src/metarace/strops.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.2/src/metarace/telegraph.py` & `metarace-2.1.3/src/metarace/telegraph.py`

 * *Files 27% similar despite different names*

```diff
@@ -31,22 +31,22 @@
  Configuration is via metarace system config (metarace.json), under
  section 'telegraph':
 
   key: (type) Description [default]
   --
   host : (string) MQTT broker, None to disable ['localhost']
   port: (int) MQTT port [1883/8883]
-  usetls : (bool) if True, connect to server over TLS [False]
-  debug : (bool) if True, enable logging in MQTT library [False]
   username : (string) username [None]
   password : (string) password [None]
-  deftopic : (string) a default publish topic [None]
+  usetls : (bool) if True, connect to server over TLS [False]
   persist : (bool) if true, open a persistent connection to broker [False]
   clientid : (string) provide an explicit client id [None]
   qos : (int) default QOS to use for subscribe and publish [0]
+  debug : (bool) if True, enable logging in MQTT library [False]
+  deftopic : (string) a default publish topic [None]
 
 
 """
 
 import threading
 import queue
 import logging
@@ -54,17 +54,91 @@
 import paho.mqtt.client as mqtt
 from uuid import uuid4
 import metarace
 
 QUEUE_TIMEOUT = 2
 
 # module logger
-_log = logging.getLogger('metarace.telegraph')
+_log = logging.getLogger('telegraph')
 _log.setLevel(logging.DEBUG)
 
+_CONFIG_SCHEMA = {
+    'ttype': {
+        'prompt': 'MQTT Broker Details',
+        'control': 'section'
+    },
+    'host': {
+        'prompt': 'Host:',
+        'hint': 'Hostname or IP of MQTT broker',
+        'default': 'localhost',
+    },
+    'port': {
+        'prompt': 'Port:',
+        'control': 'short',
+        'hint': 'TCP port number of MQTT broker',
+        'type': 'int',
+    },
+    'usetls': {
+        'prompt': 'Security:',
+        'subtext': 'Use TLS?',
+        'type': 'bool',
+        'control': 'check',
+        'hint': 'Connect to MQTT broker using TLS',
+        'default': False
+    },
+    'username': {
+        'prompt': 'Username:',
+        'hint': 'Username on MQTT broker if required'
+    },
+    'password': {
+        'prompt': 'Password:',
+        'hint': 'Password on MQTT broker if required'
+    },
+    'debug': {
+        'prompt': 'Log:',
+        'control': 'check',
+        'type': 'bool',
+        'subtext': 'Debug MQTT connection?',
+        'hint': 'Log detailed information on connection to MQTT broken',
+        'default': False,
+    },
+    'ssec': {
+        'prompt': 'Session Options',
+        'control': 'section',
+    },
+    'clientid': {
+        'prompt': 'Client ID:',
+        'hint': 'Specify client id for MQTT connection'
+    },
+    'persist': {
+        'prompt': 'Session:',
+        'subtext': 'Persistent?',
+        'type': 'bool',
+        'control': 'check',
+        'hint': 'Request persistent session on broker',
+        'default': True,
+    },
+    'qos': {
+        'prompt': 'QoS:',
+        'control': 'choice',
+        'hint': 'Default message QOS',
+        'type': 'int',
+        'options': {
+            '0': '0 - At most once',
+            '1': '1 - At least once',
+            '2': '2 - Exactly once'
+        },
+        'default': 0,
+    },
+    'deftopic': {
+        'prompt': 'Default Topic:',
+        'hint': 'Default topic for messages published without one',
+    },
+}
+
 
 def from_json(payload=None):
     """Return message payload decoded from json, or None."""
     ret = None
     try:
         ret = json.loads(payload)
     except Exception as e:
@@ -173,73 +247,62 @@
 
     def __init__(self):
         """Constructor."""
         threading.Thread.__init__(self, daemon=True)
         self.__queue = queue.Queue()
         self.__cb = defcallback
         self.__subscriptions = {}
-        self.__deftopic = None
         self.__connected = False
         self.__connect_pending = False
-        self.__host = 'localhost'
-        self.__port = 1883
         self.__cid = None
-        self.__persist = False
         self.__resub = True
-        self.__qos = 0
         self.__doreconnect = False
 
-        # check system config for overrides
-        if metarace.sysconf.has_option('telegraph', 'host'):
-            self.__host = metarace.sysconf.get_str('telegraph', 'host')
-        if metarace.sysconf.has_option('telegraph', 'deftopic'):
-            # note: this may be overidden by application
-            self.__deftopic = metarace.sysconf.get_str('telegraph', 'deftopic')
-        if metarace.sysconf.has_option('telegraph', 'qos'):
-            self.__qos = metarace.sysconf.get_posint('telegraph', 'qos', 0)
-            if self.__qos > 2:
-                _log.info('Invalid QOS %r set to %r', self.__qos, 2)
-                self.__qos = 2
-        if metarace.sysconf.has_option('telegraph', 'clientid'):
-            self.__cid = metarace.sysconf.get_str('telegraph', 'clientid')
+        metarace.sysconf.add_section('telegraph', _CONFIG_SCHEMA)
+        self.__host = metarace.sysconf.get_value('telegraph', 'host')
+        self.__port = metarace.sysconf.get_value('telegraph', 'port')
+        if self.__port is None:
+            self.__port = 1883
+        self.__deftopic = metarace.sysconf.get_value('telegraph', 'deftopic')
+        self.__qos = metarace.sysconf.get_value('telegraph', 'qos')
+        self.__persist = metarace.sysconf.get_value('telegraph', 'persist')
+        self.__cid = metarace.sysconf.get_value('telegraph', 'clientid')
+
+        # check values
+        if self.__qos > 2:
+            _log.info('Invalid QOS %r set to %r', self.__qos, 2)
+            self.__qos = 2
         if not self.__cid:
             self.__cid = str(uuid4())
+        _log.debug('Using QoS: %r', self.__qos)
         _log.debug('Using client id: %r', self.__cid)
-        if metarace.sysconf.has_option('telegraph', 'persist'):
-            self.__persist = metarace.sysconf.get_bool('telegraph', 'persist')
         _log.debug('Persistent connection: %r', self.__persist)
 
         # create mqtt client
         self.__client = mqtt.Client(client_id=self.__cid,
                                     clean_session=not self.__persist)
-        if metarace.sysconf.has_option('telegraph', 'debug'):
-            if metarace.sysconf.get_bool('telegraph', 'debug'):
-                _log.debug('Enabling mqtt/paho debug')
-                mqlog = logging.getLogger('metarace.telegraph.mqtt')
-                mqlog.setLevel(logging.DEBUG)
-                self.__client.enable_logger(mqlog)
-        if metarace.sysconf.has_option('telegraph', 'usetls'):
-            if metarace.sysconf.get_bool('telegraph', 'usetls'):
-                _log.debug('Enabling TLS connection')
+
+        if metarace.sysconf.get_value('telegraph', 'debug'):
+            _log.debug('Enabling mqtt/paho debug')
+            mqlog = logging.getLogger('telegraph.mqtt')
+            mqlog.setLevel(logging.DEBUG)
+            self.__client.enable_logger(mqlog)
+
+        if metarace.sysconf.get_value('telegraph', 'usetls'):
+            _log.debug('Enabling TLS connection')
+            if not metarace.sysconf.has_value('telegraph', 'port'):
+                # Update port for TLS if not exlicitly set
                 self.__port = 8883
-                self.__client.tls_set()
-        username = None
-        password = None
-        if metarace.sysconf.has_option('telegraph', 'username'):
-            username = metarace.sysconf.get_str('telegraph', 'username')
-        if metarace.sysconf.has_option('telegraph', 'password'):
-            password = metarace.sysconf.get_str('telegraph', 'password')
+                _log.debug('Set port to %r', self.__port)
+            self.__client.tls_set()
+        username = metarace.sysconf.get_value('telegraph', 'username')
+        password = metarace.sysconf.get_value('telegraph', 'password')
         if username and password:
             self.__client.username_pw_set(username, password)
-        # override automatic port selection if provided
-        if metarace.sysconf.has_option('telegraph', 'port'):
-            np = metarace.sysconf.get_posint('telegraph', 'port')
-            if np is not None:
-                self.__port = np
-                _log.debug('Set port to %r', self.__port)
+
         self.__client.reconnect_delay_set(2, 16)
         self.__client.on_message = self.__on_message
         self.__client.on_connect = self.__on_connect
         self.__client.on_disconnect = self.__on_disconnect
         if self.__host:
             self.__doreconnect = True
         self.__running = False
```

### Comparing `metarace-2.1.2/src/metarace/tod.py` & `metarace-2.1.3/src/metarace/tod.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,17 +31,18 @@
 """
 
 import decimal
 import re
 import logging
 from datetime import datetime
 from dateutil.parser import isoparse, parse as dateparse
+from bisect import bisect_left as _bisect
 
 # module log object
-_log = logging.getLogger('metarace.tod')
+_log = logging.getLogger('tod')
 _log.setLevel(logging.DEBUG)
 
 # Formatting and truncation constants
 QUANT_6PLACES = decimal.Decimal('0.000001')
 QUANT_5PLACES = decimal.Decimal('0.00001')
 QUANT_4PLACES = decimal.Decimal('0.0001')
 QUANT_3PLACES = decimal.Decimal('0.001')
@@ -56,21 +57,40 @@
 QUANT_TWID = [8, 10, 11, 12, 13, 14, 15]
 QUANT_PAD = ['     ', '   ', '  ', ' ', '', '', '']
 QUANT_OPAD = ['    ', '  ', ' ', '', '', '', '']
 MILL = decimal.Decimal(1000000)
 
 # default rounding is toward zero
 ROUNDING = decimal.ROUND_DOWN
+TRUNCATE = decimal.ROUND_DOWN
+ROUND = decimal.ROUND_HALF_EVEN
 
 
-def now(index='', chan='CLK', refid='', source='host'):
+def now(index='', chan='CLK', refid='', source=''):
     """Return a tod set to the current local time."""
     return tod(_now2dec(), index, chan, refid, source)
 
 
+def fromobj(obj):
+    """Create tod from serialized object"""
+    ret = None
+    try:
+        timeval = obj['timeval']
+        if '__agg__' in obj:
+            ret = agg(timeval)
+        else:
+            ret = tod(timeval)
+        for attr in ('index', 'chan', 'refid', 'source'):
+            if attr in obj:
+                setattr(ret, attr, obj[attr])
+    except Exception as e:
+        _log.warning('%s deserializing tod: %s', e.__class__.__name__, e)
+    return ret
+
+
 def fromdate(timestr=''):
     """Try to parse the provided str as a local datetime"""
     rd = None
     rt = None
     try:
         # retrieve date and time for the current timezone
         d = dateparse(timestr).astimezone()
@@ -265,20 +285,15 @@
         ret = decimal.Decimal(timeval)
     return ret
 
 
 class tod:
     """A class for representing time of day, net time and RFID events."""
 
-    def __init__(self,
-                 timeval=0,
-                 index='',
-                 chan='TOD',
-                 refid='',
-                 source='host'):
+    def __init__(self, timeval=0, index='', chan='', refid='', source=''):
         self.index = index
         self.chan = chan
         self.refid = refid
         self.source = source
         self.timeval = _tv2dec(timeval)
         if self.timeval < 0 or self.timeval >= 86400:
             raise ValueError('Time of day value not in range [0, 86400)')
@@ -298,19 +313,35 @@
         return "{5}({0}, {1}, {2}, {3}, {4})".format(repr(self.timeval),
                                                      repr(self.index),
                                                      repr(self.chan),
                                                      repr(self.refid),
                                                      repr(self.source),
                                                      self.__class__.__name__)
 
+    def serialize(self):
+        """Return serialized object for JSON export"""
+        obj = {'__tod__': 1, 'timeval': str(self.timeval)}
+        for attr in ('index', 'chan', 'refid', 'source'):
+            val = getattr(self, attr)
+            if val:
+                obj[attr] = val
+        return obj
+
+    def round(self, places=4):
+        """Return a new rounded time value."""
+        return self.places(places, ROUND, 'ROUND')
+
     def truncate(self, places=4):
         """Return a new truncated time value."""
+        return self.places(places, TRUNCATE, 'TRUNC')
+
+    def places(self, places=4, rounding=ROUNDING, flag='PLACES'):
         return self.__class__(timeval=self.timeval.quantize(QUANT[places],
-                                                            rounding=ROUNDING),
-                              chan='TRUNC')
+                                                            rounding=rounding),
+                              chan=flag)
 
     def as_hours(self, places=0):
         """Return decimal value in hours, truncated to the desired places."""
         return (self.timeval / 3600).quantize(QUANT[places], rounding=ROUNDING)
 
     def as_minutes(self, places=0):
         """Return decimal value in minutes, truncated to the desired places."""
@@ -450,26 +481,30 @@
         """Unary absolute value."""
         return self.__class__(self.timeval.copy_abs(), chan='ABS')
 
 
 class agg(tod):
     """Aggregate time type."""
 
-    def __init__(self,
-                 timeval=0,
-                 index='',
-                 chan='AGG',
-                 refid='',
-                 source='host'):
+    def __init__(self, timeval=0, index='', chan='', refid='', source=''):
         self.index = index
         self.chan = chan
         self.refid = refid
         self.source = source
         self.timeval = _tv2dec(timeval)
 
+    def serialize(self):
+        """Return serialized object for JSON export"""
+        obj = {'__agg__': 1, 'timeval': str(self.timeval)}
+        for attr in ('index', 'chan', 'refid', 'source'):
+            val = getattr(self, attr)
+            if val:
+                obj[attr] = val
+        return obj
+
     def __add__(self, other):
         """Compute addition and return aggregate."""
         if isinstance(other, tod):
             return agg(timeval=self.timeval + other.timeval, chan='AGG')
         elif isinstance(other, (int, decimal.Decimal)):
             return agg(timeval=self.timeval + other, chan='AGG')
         else:
@@ -487,15 +522,15 @@
     def __neg__(self):
         """Unary - operation."""
         return self.__class__(self.timeval.copy_negate(), chan='AGG')
 
 
 # TOD 'constants'
 ZERO = tod()
-ONE = tod('1.0')
+ONE = tod(1)
 MINUTE = tod('1:00')
 MAX = tod('23h59:59.999990')  # largest val possible for tod
 MAXELAP = tod('23h30:00')  # max displayed elapsed time
 
 # Fake times for special cases
 # these are unused tods that sort correctly when compared
 FAKETIMES = {
@@ -550,31 +585,17 @@
             if lt[0].refid == bib and lt[0].index == series:
                 ret = i
                 break
             lpri = lt[0]
             lsec = lt[1]
             count += 1
         return ret
-        """Return current 0-based rank for given bib."""
-        ret = None
-        i = 0
-        r = 0
-        last = None
-        for lt in self.__store:
-            if last is not None:
-                if lt != last:
-                    r = i
-            i += 1
-            if lt.refid == bib and lt.index == series:
-                ret = r
-                break
-            last = lt
-        return ret
 
     def clear(self):
+        """Clear list"""
         self.__store = []
         return 0
 
     def remove(self, bib, series='', once=False):
         i = 0
         while i < len(self.__store):
             if (self.__store[i][0].refid == bib
@@ -582,43 +603,23 @@
                 del self.__store[i]
                 if once:
                     break
             else:
                 i += 1
         return i
 
-    def insert(self, pri=None, sec=None, bib=None, series='', prec=3):
+    def insert(self, pri=None, sec=None, bib=None, series=''):
         """Insert primary tod and secondary tod into ordered list."""
         ret = None
-        trunc = True
         if isinstance(pri, str) and pri in FAKETIMES:
             pri = FAKETIMES[pri]
-            trunc = False  # retain precision for primary comparison
 
         if isinstance(pri, tod):
             if bib is None:
                 bib = pri.index
             if sec is None:
                 sec = ZERO
-            if trunc:
-                pri = pri.truncate(prec)
-                sec = sec.truncate(prec)
             rt0 = tod(pri, chan=self.__label, refid=bib, index=series)
             rt1 = tod(sec, chan=self.__label, refid=bib, index=series)
-            last = None
-            i = 0
-            found = False
-            for lt in self.__store:
-                if rt0 < lt[0]:  # primary time is faster, insert ok
-                    self.__store.insert(i, [rt0, rt1])
-                    found = True
-                    break
-                elif rt0 == lt[0]:  # primary same, compare on secondary
-                    if rt1 < lt[1]:  # secondary time faster - insert ok
-                        self.__store.insert(i, [rt0, rt1])
-                        found = True
-                        break
-                i += 1
-            if not found:
-                self.__store.append([rt0, rt1])
-            ret = i
+            ret = _bisect(self.__store, (rt0, rt1))
+            self.__store.insert(ret, (rt0, rt1))
         return ret
```

### Comparing `metarace-2.1.2/src/metarace/unt4.py` & `metarace-2.1.3/src/metarace/unt4.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.2/src/metarace.egg-info/PKG-INFO` & `metarace-2.1.3/src/metarace.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: metarace
-Version: 2.1.2
+Version: 2.1.3
 Summary: Cyclesport results and timing toolkit
 Author-email: Nathan Fraser <ndf-zz@6-v.org>
 License: MIT
 Project-URL: homepage, https://github.com/ndf-zz/metarace
 Keywords: cyclesport,results,timing
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Other/Nonlisted Topic
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # metarace
 
 A collection of Python modules to assist with cycle race timekeeping
@@ -31,33 +32,34 @@
    - [ttstart](https://github.com/ndf-zz/metarace-ttstart) : Time
      Trial starter console.
 
 
 ## Work in Progress
 
    - include grapheme support in strops
-   - update pango text layouts to align vertically by text baseline
-   - re-write report library for better sectioning and dynamic updates
+   - re-write report library for better sectioning
+   - overhaul PDF text rendering
+   - replace xls export with xlsx
    - module documentation
    - sample scripts
 
 
 ## Module Overview
 
 ### metarace: Base Library
 
    - shared configuration, default files and resources
    - tempfile-backed file writer
    - meet folder locking
 
 
-### jsonconfig: Configuration File Wrapper
+### jsonconfig: Configuration Options
 
-A thin wrapper on a dictionary-based configuration
-with JSON export and import.
+Schema defined dictionary-like
+configuration with JSON export and import.
 
 
 ### riderdb: CSV-backed Competitor Information
 
 Store details for competitors, teams, and categories.
 
 
@@ -96,28 +98,14 @@
 
 ### unt4: Legacy Timing Protocol
 
 Swiss Timing UNT4 protocol wrapper, for legacy devices
 and DHI communications.
 
 
-### sender: Legacy DHI Scoreboard Interface
-
-Thread object for drawing text on a
-[Caprica](https://github.com/ndf-zz/caprica)
-or Galactica DHI scoreboard over TCP,
-UDP and serial connections.
-
-
-### gemini: Numeric LED Scoreboard Interface
-
-Thread object for writing to a pair of Swiss Timing Gemini
-numeric LED boards, and lap count displays.
-
-
 ### countback: Accumulate and Compare Count of Places
 
 Represent a countback of places and allow for simple
 placing comparisons.
 
 
 ### htlib: HTML Generation
@@ -128,69 +116,68 @@
 ### report: Report Generation
 
 Create sectioned reports and save to PDF, HTML, XLS and JSON.
 
 
 ### export: Result Export and Mirroring
 
-Execute a process on the host system to
-mirror result files to a remote server,
-or to run a script.
+Mirror export files to a remote host using rsync over ssh,
+rsync TCP daemon or by running a local script.
 
 
 ### eventdb: CSV Event List
 
-Store details for events within a meet.
+Store details for multple events within a meet.
 
 
 ## Requirements
 
 System requirements:
 
    - Python >= 3.9
    - Cairo
    - Pango
    - Rsvg
    - Python gi
    - Python gi-cairo
    - tex-gyre (optional, recommended)
    - evince (optional, recommended)
+   - fonts-noto (optional)
    - mosquitto (optional)
    - libreoffice (optional)
 
 Python packages:
 
    - pyserial: Serial port interface
    - python-dateutil: Generic date/time string parser
    - xlwt: XLS file writer
    - paho-mqtt: MQTT interface
    - grapheme: Unicode grapheme support
 
 
 ## Installation
 
-Check that your python
-version is at least 3.9 before installing. This library will
-not work with python versions less than 3.9.
+Check that your python version is at least 3.9 before installing.
+This library will not work with python versions less than 3.9.
 
 
 ### Debian 11+
 
 Install system requirements with apt:
 
 	$ sudo apt install python3-venv python3-pip python3-cairo python3-gi python3-gi-cairo
 	$ sudo apt install gir1.2-rsvg-2.0 gir1.2-pango-1.0
 	$ sudo apt install python3-serial python3-paho-mqtt python3-dateutil python3-xlwt
 
 Optionally add fonts, PDF viewer and MQTT broker:
 
-	$ sudo apt install tex-gyre evince mosquitto
+	$ sudo apt install tex-gyre fonts-noto evince mosquitto
 
 Create a virtualenv for metarace and associated packages:
 
-	$ python3 -m venv --system-site-packages mrv
+	$ python3 -m venv --system-site-packages venv
 
 Activate the virtualenv and install packages with pip:
 
-	$ source ./mrv/bin/activate
-	(mrv) $ pip3 install metarace
+	$ source ./venv/bin/activate
+	(venv) $ pip3 install metarace
```

### Comparing `metarace-2.1.2/src/metarace.egg-info/SOURCES.txt` & `metarace-2.1.3/src/metarace.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 MANIFEST.in
 README.md
 pyproject.toml
 src/metarace/__init__.py
 src/metarace/countback.py
 src/metarace/eventdb.py
 src/metarace/export.py
-src/metarace/gemini.py
 src/metarace/htlib.py
 src/metarace/jsonconfig.py
 src/metarace/report.py
 src/metarace/riderdb.py
-src/metarace/sender.py
 src/metarace/strops.py
 src/metarace/telegraph.py
 src/metarace/timy.py
 src/metarace/tod.py
 src/metarace/unt4.py
 src/metarace.egg-info/PKG-INFO
 src/metarace.egg-info/SOURCES.txt
```

