# Comparing `tmp/PyLTSpice-4.0.5.tar.gz` & `tmp/PyLTSpice-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\sandbox\PySpice\dist\.tmp-84jaqpyk\PyLTSpice-4.0.5.tar", last modified: Fri Jun 16 14:16:18 2023, max compression
+gzip compressed data, was "C:\sandbox\PyLTSpice\dist\.tmp-chpp5bb4\PyLTSpice-4.0.6.tar", last modified: Mon Jul 17 17:45:07 2023, max compression
```

## Comparing `PyLTSpice-4.0.5.tar` & `PyLTSpice-4.0.6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 14:16:18.026907 PyLTSpice-4.0.5/
--rw-rw-rw-   0        0        0    35823 2022-12-04 12:18:59.000000 PyLTSpice-4.0.5/LICENSE
--rw-rw-rw-   0        0        0    58334 2023-06-16 14:16:18.025910 PyLTSpice-4.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-16 14:16:17.915878 PyLTSpice-4.0.5/PyLTSpice/
--rw-rw-rw-   0        0        0     9679 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/Histogram.py
--rw-rw-rw-   0        0        0      362 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/LTSpiceBatch.py
--rw-rw-rw-   0        0        0      333 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/LTSpice_RawRead.py
--rw-rw-rw-   0        0        0      332 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/LTSpice_RawWrite.py
--rw-rw-rw-   0        0        0     6743 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/LTSteps.py
--rw-rw-rw-   0        0        0     1692 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 14:16:17.944826 PyLTSpice-4.0.5/PyLTSpice/client_server/
--rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/client_server/__init__.py
--rw-rw-rw-   0        0        0     8488 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/client_server/sim_client.py
--rw-rw-rw-   0        0        0     5570 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/client_server/sim_server.py
--rw-rw-rw-   0        0        0     4865 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/client_server/srv_sim_runner.py
-drwxrwxrwx   0        0        0        0 2023-06-16 14:16:17.953334 PyLTSpice-4.0.5/PyLTSpice/log/
--rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/log/__init__.py
--rw-rw-rw-   0        0        0    29997 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/log/ltsteps.py
--rw-rw-rw-   0        0        0     6047 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/log/semi_dev_op_reader.py
-drwxrwxrwx   0        0        0        0 2023-06-16 14:16:17.966506 PyLTSpice-4.0.5/PyLTSpice/raw/
--rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/raw/__init__.py
--rw-rw-rw-   0        0        0    14667 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/raw/raw_classes.py
--rw-rw-rw-   0        0        0     5609 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/raw/raw_convert.py
--rw-rw-rw-   0        0        0    36151 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/raw/raw_read.py
--rw-rw-rw-   0        0        0    16752 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/raw/raw_write.py
--rw-rw-rw-   0        0        0     4014 2023-05-14 19:17:53.000000 PyLTSpice-4.0.5/PyLTSpice/rawplot.py
-drwxrwxrwx   0        0        0        0 2023-06-16 14:16:18.000035 PyLTSpice-4.0.5/PyLTSpice/sim/
--rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/sim/__init__.py
--rw-rw-rw-   0        0        0     9342 2023-06-16 12:17:42.000000 PyLTSpice-4.0.5/PyLTSpice/sim/ltspice_simulator.py
--rw-rw-rw-   0        0        0     4738 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/sim/ngspice_simulator.py
--rw-rw-rw-   0        0        0     1505 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/sim/process_callback.py
--rw-rw-rw-   0        0        0     7179 2023-06-04 10:41:26.000000 PyLTSpice-4.0.5/PyLTSpice/sim/run_task.py
--rw-rw-rw-   0        0        0     4809 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/sim/sim_analysis.py
--rw-rw-rw-   0        0        0    10823 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/sim/sim_batch.py
--rw-rw-rw-   0        0        0    23309 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/sim/sim_runner.py
--rw-rw-rw-   0        0        0     9298 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/sim/sim_stepping.py
--rw-rw-rw-   0        0        0     4652 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/sim/simulator.py
--rw-rw-rw-   0        0        0    46624 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/sim/spice_editor.py
--rw-rw-rw-   0        0        0     7456 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/sim/xyce_simulator.py
--rw-rw-rw-   0        0        0    21638 2023-06-02 14:46:46.000000 PyLTSpice-4.0.5/PyLTSpice/sim_batch.py
-drwxrwxrwx   0        0        0        0 2023-06-16 14:16:18.006939 PyLTSpice-4.0.5/PyLTSpice/utils/
--rw-rw-rw-   0        0        0     2935 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/utils/detect_encoding.py
--rw-rw-rw-   0        0        0    11563 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/PyLTSpice/utils/sweep_iterators.py
-drwxrwxrwx   0        0        0        0 2023-06-16 14:16:17.933827 PyLTSpice-4.0.5/PyLTSpice.egg-info/
--rw-rw-rw-   0        0        0    58334 2023-06-16 14:16:17.000000 PyLTSpice-4.0.5/PyLTSpice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1361 2023-06-16 14:16:17.000000 PyLTSpice-4.0.5/PyLTSpice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 14:16:17.000000 PyLTSpice-4.0.5/PyLTSpice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      165 2023-06-16 14:16:17.000000 PyLTSpice-4.0.5/PyLTSpice.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-06-16 14:16:17.000000 PyLTSpice-4.0.5/PyLTSpice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-06-16 14:16:17.000000 PyLTSpice-4.0.5/PyLTSpice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    16553 2023-06-16 12:20:56.000000 PyLTSpice-4.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 14:16:18.009950 PyLTSpice-4.0.5/doc/
--rw-rw-rw-   0        0        0     2448 2023-05-14 19:17:07.000000 PyLTSpice-4.0.5/doc/conf.py
--rw-rw-rw-   0        0        0     1193 2023-06-16 12:20:56.000000 PyLTSpice-4.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 14:16:18.027904 PyLTSpice-4.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 14:16:18.012944 PyLTSpice-4.0.5/tests/
--rw-rw-rw-   0        0        0      801 2023-05-14 19:17:08.000000 PyLTSpice-4.0.5/tests/test_ltsteps.py
-drwxrwxrwx   0        0        0        0 2023-06-16 14:16:18.017931 PyLTSpice-4.0.5/tests/unittest/
-drwxrwxrwx   0        0        0        0 2023-06-16 14:16:18.020923 PyLTSpice-4.0.5/tests/unittest/sweep_iterators/
--rw-rw-rw-   0        0        0     6014 2023-05-14 19:17:08.000000 PyLTSpice-4.0.5/tests/unittest/sweep_iterators/sweep_iterators_unittest.py
--rw-rw-rw-   0        0        0    19227 2023-05-14 19:17:08.000000 PyLTSpice-4.0.5/tests/unittest/test_pyltspice.py
+drwxrwxrwx   0        0        0        0 2023-07-17 17:45:07.824167 PyLTSpice-4.0.6/
+-rw-rw-rw-   0        0        0    35823 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/LICENSE
+-rw-rw-rw-   0        0        0    58563 2023-07-17 17:45:07.823170 PyLTSpice-4.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-17 17:45:07.752657 PyLTSpice-4.0.6/PyLTSpice/
+-rw-rw-rw-   0        0        0     9679 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/Histogram.py
+-rw-rw-rw-   0        0        0      362 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/LTSpiceBatch.py
+-rw-rw-rw-   0        0        0      333 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/LTSpice_RawRead.py
+-rw-rw-rw-   0        0        0      332 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/LTSpice_RawWrite.py
+-rw-rw-rw-   0        0        0     6743 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/LTSteps.py
+-rw-rw-rw-   0        0        0     1692 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 17:45:07.773602 PyLTSpice-4.0.6/PyLTSpice/client_server/
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/client_server/__init__.py
+-rw-rw-rw-   0        0        0     8488 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/client_server/sim_client.py
+-rw-rw-rw-   0        0        0     5570 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/client_server/sim_server.py
+-rw-rw-rw-   0        0        0     4865 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/client_server/srv_sim_runner.py
+drwxrwxrwx   0        0        0        0 2023-07-17 17:45:07.779587 PyLTSpice-4.0.6/PyLTSpice/log/
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/log/__init__.py
+-rw-rw-rw-   0        0        0    29997 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/log/ltsteps.py
+-rw-rw-rw-   0        0        0     6047 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/log/semi_dev_op_reader.py
+drwxrwxrwx   0        0        0        0 2023-07-17 17:45:07.787563 PyLTSpice-4.0.6/PyLTSpice/raw/
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/raw/__init__.py
+-rw-rw-rw-   0        0        0    14667 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/raw/raw_classes.py
+-rw-rw-rw-   0        0        0     5609 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/raw/raw_convert.py
+-rw-rw-rw-   0        0        0    36151 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/raw/raw_read.py
+-rw-rw-rw-   0        0        0    16752 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/raw/raw_write.py
+-rw-rw-rw-   0        0        0     4014 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/rawplot.py
+drwxrwxrwx   0        0        0        0 2023-07-17 17:45:07.809207 PyLTSpice-4.0.6/PyLTSpice/sim/
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/sim/__init__.py
+-rw-rw-rw-   0        0        0     9342 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/sim/ltspice_simulator.py
+-rw-rw-rw-   0        0        0     4738 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/sim/ngspice_simulator.py
+-rw-rw-rw-   0        0        0     1505 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/sim/process_callback.py
+-rw-rw-rw-   0        0        0     7179 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/sim/run_task.py
+-rw-rw-rw-   0        0        0     4809 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/sim/sim_analysis.py
+-rw-rw-rw-   0        0        0    10823 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/sim/sim_batch.py
+-rw-rw-rw-   0        0        0    23309 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/sim/sim_runner.py
+-rw-rw-rw-   0        0        0     9298 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/sim/sim_stepping.py
+-rw-rw-rw-   0        0        0     4652 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/sim/simulator.py
+-rw-rw-rw-   0        0        0    46677 2023-07-17 16:43:53.000000 PyLTSpice-4.0.6/PyLTSpice/sim/spice_editor.py
+-rw-rw-rw-   0        0        0     7456 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/sim/xyce_simulator.py
+-rw-rw-rw-   0        0        0    21638 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/sim_batch.py
+drwxrwxrwx   0        0        0        0 2023-07-17 17:45:07.813196 PyLTSpice-4.0.6/PyLTSpice/utils/
+-rw-rw-rw-   0        0        0     2935 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/utils/detect_encoding.py
+-rw-rw-rw-   0        0        0    11563 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/PyLTSpice/utils/sweep_iterators.py
+drwxrwxrwx   0        0        0        0 2023-07-17 17:45:07.765625 PyLTSpice-4.0.6/PyLTSpice.egg-info/
+-rw-rw-rw-   0        0        0    58563 2023-07-17 17:45:07.000000 PyLTSpice-4.0.6/PyLTSpice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1361 2023-07-17 17:45:07.000000 PyLTSpice-4.0.6/PyLTSpice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 17:45:07.000000 PyLTSpice-4.0.6/PyLTSpice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      165 2023-07-17 17:45:07.000000 PyLTSpice-4.0.6/PyLTSpice.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-07-17 17:45:07.000000 PyLTSpice-4.0.6/PyLTSpice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-07-17 17:45:07.000000 PyLTSpice-4.0.6/PyLTSpice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    16782 2023-07-17 16:46:33.000000 PyLTSpice-4.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 17:45:07.815191 PyLTSpice-4.0.6/doc/
+-rw-rw-rw-   0        0        0     2448 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/doc/conf.py
+-rw-rw-rw-   0        0        0     1193 2023-07-17 16:46:40.000000 PyLTSpice-4.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 17:45:07.824167 PyLTSpice-4.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 17:45:07.817186 PyLTSpice-4.0.6/tests/
+-rw-rw-rw-   0        0        0      801 2023-07-17 16:33:51.000000 PyLTSpice-4.0.6/tests/test_ltsteps.py
+drwxrwxrwx   0        0        0        0 2023-07-17 17:45:07.819180 PyLTSpice-4.0.6/tests/unittest/
+drwxrwxrwx   0        0        0        0 2023-07-17 17:45:07.821174 PyLTSpice-4.0.6/tests/unittest/sweep_iterators/
+-rw-rw-rw-   0        0        0     6014 2023-05-14 19:17:08.000000 PyLTSpice-4.0.6/tests/unittest/sweep_iterators/sweep_iterators_unittest.py
+-rw-rw-rw-   0        0        0    19227 2023-05-14 19:17:08.000000 PyLTSpice-4.0.6/tests/unittest/test_pyltspice.py
```

### Comparing `PyLTSpice-4.0.5/LICENSE` & `PyLTSpice-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PKG-INFO` & `PyLTSpice-4.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLTSpice
-Version: 4.0.5
+Version: 4.0.6
 Summary: A set of tools to Automate LTSpice simulations
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -975,14 +975,18 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 4.0.6\
+  Fixing issue with the write_netlist() function when receiving a string instead of a pathlib.Path object.\
+  Changing the regular expression for the resistor in order to accept the R= prefix on the values.
+
 * Version 4.0.5\
   Accepting fixes from aanas-sayed@GitHub that fixes issues with running the LTSpice in Linux.
 
 * Version 4.0.4\
   Improved usage of the logging library. (Thanks TSprech@GitHub)\
   Included RunTask number in the log messages.\ 
   Included milliseconds in the time elapsed calculation.
```

### Comparing `PyLTSpice-4.0.5/PyLTSpice/Histogram.py` & `PyLTSpice-4.0.6/PyLTSpice/Histogram.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/LTSteps.py` & `PyLTSpice-4.0.6/PyLTSpice/LTSteps.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/__init__.py` & `PyLTSpice-4.0.6/PyLTSpice/__init__.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/client_server/sim_client.py` & `PyLTSpice-4.0.6/PyLTSpice/client_server/sim_client.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/client_server/sim_server.py` & `PyLTSpice-4.0.6/PyLTSpice/client_server/sim_server.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/client_server/srv_sim_runner.py` & `PyLTSpice-4.0.6/PyLTSpice/client_server/srv_sim_runner.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/log/ltsteps.py` & `PyLTSpice-4.0.6/PyLTSpice/log/ltsteps.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/log/semi_dev_op_reader.py` & `PyLTSpice-4.0.6/PyLTSpice/log/semi_dev_op_reader.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/raw/raw_classes.py` & `PyLTSpice-4.0.6/PyLTSpice/raw/raw_classes.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/raw/raw_convert.py` & `PyLTSpice-4.0.6/PyLTSpice/raw/raw_convert.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/raw/raw_read.py` & `PyLTSpice-4.0.6/PyLTSpice/raw/raw_read.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/raw/raw_write.py` & `PyLTSpice-4.0.6/PyLTSpice/raw/raw_write.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/rawplot.py` & `PyLTSpice-4.0.6/PyLTSpice/rawplot.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/sim/ltspice_simulator.py` & `PyLTSpice-4.0.6/PyLTSpice/sim/ltspice_simulator.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/sim/ngspice_simulator.py` & `PyLTSpice-4.0.6/PyLTSpice/sim/ngspice_simulator.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/sim/process_callback.py` & `PyLTSpice-4.0.6/PyLTSpice/sim/process_callback.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/sim/run_task.py` & `PyLTSpice-4.0.6/PyLTSpice/sim/run_task.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/sim/sim_analysis.py` & `PyLTSpice-4.0.6/PyLTSpice/sim/sim_analysis.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/sim/sim_batch.py` & `PyLTSpice-4.0.6/PyLTSpice/sim/sim_batch.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/sim/sim_runner.py` & `PyLTSpice-4.0.6/PyLTSpice/sim/sim_runner.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/sim/sim_stepping.py` & `PyLTSpice-4.0.6/PyLTSpice/sim/sim_stepping.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/sim/simulator.py` & `PyLTSpice-4.0.6/PyLTSpice/sim/simulator.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/sim/spice_editor.py` & `PyLTSpice-4.0.6/PyLTSpice/sim/spice_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
                                                         # This implementation replaces everything after the 2 first nets
     'J': r"^(?P<designator>J§?\w+)(?P<nodes>(\s+\S+){3})\s+(?P<value>\w+).*$",  # JFET
     'K': r"^(?P<designator>K§?\w+)(?P<nodes>(\s+\S+){2,4})\s+(?P<value>[\+\-]?[0-9\.E+-]+[kmuµnpf]?).*$",  # Mutual Inductance
     'L': r"^(?P<designator>L§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>({)?(?(5).*}|([0-9\.E+-]+(Meg|[kmuµnpf])?H?))).*$",  # Inductance
     'M': r"^(?P<designator>M§?\w+)(?P<nodes>(\s+\S+){3,4})\s+(?P<value>\w+).*$",  # MOSFET TODO: Parameters substitution not supported
     'O': r"^(?P<designator>O§?\w+)(?P<nodes>(\s+\S+){4})\s+(?P<value>\w+).*$",  # Lossy Transmission Line TODO: Parameters substitution not supported
     'Q': r"^(?P<designator>Q§?\w+)(?P<nodes>(\s+\S+){3,4})\s+(?P<value>\w+).*$",  # Bipolar TODO: Parameters substitution not supported
-    'R': r"^(?P<designator>R§?\w+)(?P<nodes>(\s+\S+){2})(?P<model>\s+\w+)?\s+(?P<value>({)?(?(6).*}|([0-9\.E+-]+(Meg|[kmuµnpf])?R?)\d*)).*$", # Resistors
+    'R': r"^(?P<designator>R§?\w+)(?P<nodes>(\s+\S+){2})(?P<model>\s+\w+)?\s+(?P<value>(R=)?({)?(?(7).*}|([0-9\.E+-]+(Meg|[kmuµnpf])?R?)\d*)).*$", # Resistors
     'S': r"^(?P<designator>S§?\w+)(?P<nodes>(\s+\S+){4})\s+(?P<value>.*)$",  # Voltage Controlled Switch
     'T': r"^(?P<designator>T§?\w+)(?P<nodes>(\s+\S+){4})\s+(?P<value>.*)$",  # Lossless Transmission
     'U': r"^(?P<designator>U§?\w+)(?P<nodes>(\s+\S+){3})\s+(?P<value>.*)$",  # Uniform RC-line
     'V': r"^(?P<designator>V§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>.*)$",  # Voltage Source
                                                         # This implementation replaces everything after the 2 first nets
     'W': r"^(?P<designator>W§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>.*)$",  # Current Controlled Switch
                                                         # This implementation replaces everything after the 2 first nets
@@ -370,17 +370,18 @@
         line_no = 0
         reg_subckt = re.compile(SUBCKT_CLAUSE_FIND + subcircuit_name, re.IGNORECASE)
 
         libs_list = []
         sub_circuit = None
         while line_no < len(self.netlist):
             line = self.netlist[line_no]
-            if isinstance(line, SpiceCircuit) and line.name() == subcircuit_name:
-                sub_circuit = line # The circuit was already found
-                break
+            if isinstance(line, SpiceCircuit):
+                if line.name() == subcircuit_name:
+                    sub_circuit = line  # The circuit was already found
+                    break
             else:
                 m = lib_inc_regex.match(line)
                 if m:     # For compatibility issues not using the walruss operator here
                     libs_list.append( m.group(2) )
             line_no += 1
         if sub_circuit is None:
             # If we reached here is because the subciruit was not found. Search for it in declared libraries
@@ -848,15 +849,15 @@
             component_split = component.split(SUBCIRCUIT_DIVIDER)
             modified_path = SUBCIRCUIT_DIVIDER.join(component_split[:-1])  # excludes last component
             component = component_split[-1] # This is the last component to modify
 
             if modified_path in self.modified_subcircuits:  # See if this was already a modified subcircuit instance
                 sub_circuit = self.modified_subcircuits[modified_path]
             else:
-                sub_circuit_original = self._get_subcircuit(modified_path)  # If not will look of it.
+                sub_circuit_original = self._get_subcircuit(modified_path)  # If not will look for it.
                 if sub_circuit_original:
                     new_name = sub_circuit_original.name() + '_' + '_'.join(component_split[:-1])  # Creates a new name with the path appended
                     sub_circuit = sub_circuit_original.clone(new_name=new_name)
                     # Memorize that the copy is relative to that particular instance
                     self.modified_subcircuits[modified_path] = sub_circuit
                     # Change the call to the subcircuit
                     self._set_model_and_value(modified_path, new_name)
@@ -941,23 +942,23 @@
         # Because the netlist is stored containing the end of line terminations and because they are added when they
         # they are added to the netlist.
         if not instruction.endswith(END_LINE_TERM):
             instruction += END_LINE_TERM
 
         self.netlist.remove(instruction)
 
-    def write_netlist(self, run_netlist_file: 'Path') -> None:
+    def write_netlist(self, run_netlist_file: Union[str, 'Path']) -> None:
         """
         Writes the netlist will all the requested updates into a file named <run_netlist_file>.
 
         :param run_netlist_file: File name of the netlist file.
-        :type run_netlist_file: Path
+        :type run_netlist_file: Path or str
         :returns: Nothing
         """
-        with run_netlist_file.open('w', encoding=self.encoding) as f:
+        with open(run_netlist_file, 'w', encoding=self.encoding) as f:
             lines = iter(self.netlist)
             for line in lines:
                 if isinstance(line, SpiceCircuit):
                     line._write_lines(f)
                 else:
                     # Writes the modified subcircuits at the end just before the .END clause
                     if line.upper().startswith(".END"):
@@ -971,15 +972,15 @@
         Removes all previous edits done to the netlist, i.e. resets it to the original state.
 
         :returns: Nothing
         """
         self.netlist.clear()
         self.modified_subcircuits.clear()
         if self.netlist_file.exists():
-            with self.netlist_file.open('r', encoding=self.encoding, errors='replace') as f:
+            with open(self.netlist_file, 'r', encoding=self.encoding, errors='replace') as f:
                 lines = iter(f)  # Creates an iterator object to consume the file
                 finished = self._add_lines(lines)
                 if not finished:
                     raise SyntaxError("Netlist with missing .END or .ENDS statements")
                 # else:
                 #     for _ in lines:  # Consuming the rest of the file.
                 #         pass  # print("Ignoring %s" % _)
```

### Comparing `PyLTSpice-4.0.5/PyLTSpice/sim/xyce_simulator.py` & `PyLTSpice-4.0.6/PyLTSpice/sim/xyce_simulator.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/sim_batch.py` & `PyLTSpice-4.0.6/PyLTSpice/sim_batch.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/utils/detect_encoding.py` & `PyLTSpice-4.0.6/PyLTSpice/utils/detect_encoding.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice/utils/sweep_iterators.py` & `PyLTSpice-4.0.6/PyLTSpice/utils/sweep_iterators.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/PyLTSpice.egg-info/PKG-INFO` & `PyLTSpice-4.0.6/PyLTSpice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLTSpice
-Version: 4.0.5
+Version: 4.0.6
 Summary: A set of tools to Automate LTSpice simulations
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -975,14 +975,18 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 4.0.6\
+  Fixing issue with the write_netlist() function when receiving a string instead of a pathlib.Path object.\
+  Changing the regular expression for the resistor in order to accept the R= prefix on the values.
+
 * Version 4.0.5\
   Accepting fixes from aanas-sayed@GitHub that fixes issues with running the LTSpice in Linux.
 
 * Version 4.0.4\
   Improved usage of the logging library. (Thanks TSprech@GitHub)\
   Included RunTask number in the log messages.\ 
   Included milliseconds in the time elapsed calculation.
```

### Comparing `PyLTSpice-4.0.5/PyLTSpice.egg-info/SOURCES.txt` & `PyLTSpice-4.0.6/PyLTSpice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/README.md` & `PyLTSpice-4.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -286,14 +286,18 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 4.0.6\
+  Fixing issue with the write_netlist() function when receiving a string instead of a pathlib.Path object.\
+  Changing the regular expression for the resistor in order to accept the R= prefix on the values.
+
 * Version 4.0.5\
   Accepting fixes from aanas-sayed@GitHub that fixes issues with running the LTSpice in Linux.
 
 * Version 4.0.4\
   Improved usage of the logging library. (Thanks TSprech@GitHub)\
   Included RunTask number in the log messages.\ 
   Included milliseconds in the time elapsed calculation.
```

### Comparing `PyLTSpice-4.0.5/doc/conf.py` & `PyLTSpice-4.0.6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/pyproject.toml` & `PyLTSpice-4.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "PyLTSpice"
-version = "4.0.5"
+version = "4.0.6"
 authors = [
   { name="Nuno Brum", email="me@nunobrum.com" },
 ]
 description = "A set of tools to Automate LTSpice simulations"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `PyLTSpice-4.0.5/tests/test_ltsteps.py` & `PyLTSpice-4.0.6/tests/test_ltsteps.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/tests/unittest/sweep_iterators/sweep_iterators_unittest.py` & `PyLTSpice-4.0.6/tests/unittest/sweep_iterators/sweep_iterators_unittest.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.5/tests/unittest/test_pyltspice.py` & `PyLTSpice-4.0.6/tests/unittest/test_pyltspice.py`

 * *Files identical despite different names*

