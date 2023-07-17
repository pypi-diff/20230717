# Comparing `tmp/mentpy-0.1.0a7.tar.gz` & `tmp/mentpy-0.1.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentpy-0.1.0a7.tar", last modified: Wed May 31 21:45:30 2023, max compression
+gzip compressed data, was "mentpy-0.1.0a8.tar", last modified: Mon Jul 17 00:07:07 2023, max compression
```

## Comparing `mentpy-0.1.0a7.tar` & `mentpy-0.1.0a8.tar`

### file list

```diff
@@ -1,68 +1,71 @@
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.806967 mentpy-0.1.0a7/
--rw-r--r--   0 luismantilla   (501) staff       (20)    35149 2023-03-17 11:11:29.000000 mentpy-0.1.0a7/LICENSE
--rw-r--r--   0 luismantilla   (501) staff       (20)     3336 2023-05-31 21:45:30.806688 mentpy-0.1.0a7/PKG-INFO
--rw-r--r--   0 luismantilla   (501) staff       (20)     3056 2023-05-08 04:08:41.000000 mentpy-0.1.0a7/README.md
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.784252 mentpy-0.1.0a7/mentpy/
--rw-r--r--   0 luismantilla   (501) staff       (20)      278 2023-05-23 00:36:24.000000 mentpy-0.1.0a7/mentpy/__init__.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.786621 mentpy-0.1.0a7/mentpy/calculator/
--rw-r--r--   0 luismantilla   (501) staff       (20)       46 2023-05-23 00:44:55.000000 mentpy-0.1.0a7/mentpy/calculator/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      137 2023-05-23 00:43:44.000000 mentpy-0.1.0a7/mentpy/calculator/borrows.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1128 2023-05-23 00:43:45.000000 mentpy-0.1.0a7/mentpy/calculator/linalg2.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.787394 mentpy-0.1.0a7/mentpy/gradients/
--rw-r--r--   0 luismantilla   (501) staff       (20)       33 2023-03-17 21:21:26.000000 mentpy-0.1.0a7/mentpy/gradients/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2014 2023-04-25 08:57:09.000000 mentpy-0.1.0a7/mentpy/gradients/finite_difference.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.790183 mentpy-0.1.0a7/mentpy/mbqc/
--rw-r--r--   0 luismantilla   (501) staff       (20)      343 2023-04-16 02:07:08.000000 mentpy-0.1.0a7/mentpy/mbqc/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    18653 2023-05-31 21:43:20.000000 mentpy-0.1.0a7/mentpy/mbqc/flow.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    29847 2023-05-31 21:43:20.000000 mentpy-0.1.0a7/mentpy/mbqc/mbqcircuit.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.791936 mentpy-0.1.0a7/mentpy/mbqc/states/
--rw-r--r--   0 luismantilla   (501) staff       (20)      149 2023-05-06 07:23:30.000000 mentpy-0.1.0a7/mentpy/mbqc/states/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      197 2023-05-06 07:23:09.000000 mentpy-0.1.0a7/mentpy/mbqc/states/aklt.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      229 2023-05-06 07:23:14.000000 mentpy-0.1.0a7/mentpy/mbqc/states/cluster.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2976 2023-04-16 05:41:03.000000 mentpy-0.1.0a7/mentpy/mbqc/states/graphstate.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     7594 2023-05-24 18:57:37.000000 mentpy-0.1.0a7/mentpy/mbqc/templates.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.792858 mentpy-0.1.0a7/mentpy/noise/
--rw-r--r--   0 luismantilla   (501) staff       (20)       34 2023-03-17 21:21:26.000000 mentpy-0.1.0a7/mentpy/noise/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      173 2023-03-17 21:21:26.000000 mentpy-0.1.0a7/mentpy/noise/base_noise.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.794157 mentpy-0.1.0a7/mentpy/operators/
--rw-r--r--   0 luismantilla   (501) staff       (20)      285 2023-05-10 00:16:14.000000 mentpy-0.1.0a7/mentpy/operators/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3364 2023-05-22 17:03:18.000000 mentpy-0.1.0a7/mentpy/operators/controlled_ment.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1599 2023-05-07 19:04:31.000000 mentpy-0.1.0a7/mentpy/operators/gates.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     8139 2023-05-16 20:00:06.000000 mentpy-0.1.0a7/mentpy/operators/ment.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     5675 2023-05-31 21:43:20.000000 mentpy-0.1.0a7/mentpy/operators/pauliop.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.797575 mentpy-0.1.0a7/mentpy/optimizers/
--rw-r--r--   0 luismantilla   (501) staff       (20)      245 2023-04-25 08:17:14.000000 mentpy-0.1.0a7/mentpy/optimizers/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3054 2023-03-22 20:56:41.000000 mentpy-0.1.0a7/mentpy/optimizers/adam.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      632 2023-03-17 21:21:26.000000 mentpy-0.1.0a7/mentpy/optimizers/base_optimizer.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      379 2023-03-17 21:21:26.000000 mentpy-0.1.0a7/mentpy/optimizers/bp_tools.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3101 2023-04-25 09:08:43.000000 mentpy-0.1.0a7/mentpy/optimizers/rcd.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2637 2023-04-15 23:00:30.000000 mentpy-0.1.0a7/mentpy/optimizers/sgd.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.801268 mentpy-0.1.0a7/mentpy/simulators/
--rw-r--r--   0 luismantilla   (501) staff       (20)      281 2023-04-16 02:18:15.000000 mentpy-0.1.0a7/mentpy/simulators/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2441 2023-05-07 19:04:31.000000 mentpy-0.1.0a7/mentpy/simulators/base_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1156 2023-04-18 08:22:14.000000 mentpy-0.1.0a7/mentpy/simulators/cirq_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    15594 2023-05-31 21:43:20.000000 mentpy-0.1.0a7/mentpy/simulators/np_simulator_dm.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    19270 2023-05-31 21:43:20.000000 mentpy-0.1.0a7/mentpy/simulators/np_simulator_sv.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2678 2023-05-18 06:35:37.000000 mentpy-0.1.0a7/mentpy/simulators/pattern_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     5677 2023-05-18 08:04:21.000000 mentpy-0.1.0a7/mentpy/simulators/pennylane_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1254 2023-04-25 08:57:09.000000 mentpy-0.1.0a7/mentpy/simulators/qiskit_simulators.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.802518 mentpy-0.1.0a7/mentpy/utils/
--rw-r--r--   0 luismantilla   (501) staff       (20)      140 2023-05-23 00:17:19.000000 mentpy-0.1.0a7/mentpy/utils/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     6673 2023-04-25 08:57:09.000000 mentpy-0.1.0a7/mentpy/utils/expressivity.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3183 2023-04-16 01:51:56.000000 mentpy-0.1.0a7/mentpy/utils/flow_space.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     4466 2023-04-16 01:44:39.000000 mentpy-0.1.0a7/mentpy/utils/generate_data.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    10395 2023-05-06 07:13:49.000000 mentpy-0.1.0a7/mentpy/utils/lc_equivalence.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     5383 2023-05-31 21:43:20.000000 mentpy-0.1.0a7/mentpy/utils/lie_algebra.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.785522 mentpy-0.1.0a7/mentpy.egg-info/
--rw-r--r--   0 luismantilla   (501) staff       (20)     3336 2023-05-31 21:45:30.000000 mentpy-0.1.0a7/mentpy.egg-info/PKG-INFO
--rw-r--r--   0 luismantilla   (501) staff       (20)     1497 2023-05-31 21:45:30.000000 mentpy-0.1.0a7/mentpy.egg-info/SOURCES.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)        1 2023-05-31 21:45:30.000000 mentpy-0.1.0a7/mentpy.egg-info/dependency_links.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)       49 2023-05-31 21:45:30.000000 mentpy-0.1.0a7/mentpy.egg-info/requires.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)        7 2023-05-31 21:45:30.000000 mentpy-0.1.0a7/mentpy.egg-info/top_level.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)       38 2023-05-31 21:45:30.807073 mentpy-0.1.0a7/setup.cfg
--rw-r--r--   0 luismantilla   (501) staff       (20)      553 2023-05-31 21:45:19.000000 mentpy-0.1.0a7/setup.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-05-31 21:45:30.806024 mentpy-0.1.0a7/tests/
--rw-r--r--   0 luismantilla   (501) staff       (20)       58 2023-04-16 01:51:49.000000 mentpy-0.1.0a7/tests/test_flow.py
--rw-r--r--   0 luismantilla   (501) staff       (20)       64 2023-04-16 01:52:08.000000 mentpy-0.1.0a7/tests/test_graph_state.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      579 2023-04-16 01:52:23.000000 mentpy-0.1.0a7/tests/test_mbqc_templates.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2110 2023-05-18 06:15:48.000000 mentpy-0.1.0a7/tests/test_simulators.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.416164 mentpy-0.1.0a8/
+-rw-r--r--   0 luismantilla   (501) staff       (20)    35149 2023-03-17 11:11:29.000000 mentpy-0.1.0a8/LICENSE
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3336 2023-07-17 00:07:07.415284 mentpy-0.1.0a8/PKG-INFO
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3056 2023-05-08 04:08:41.000000 mentpy-0.1.0a8/README.md
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.405648 mentpy-0.1.0a8/mentpy/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      278 2023-05-23 00:36:24.000000 mentpy-0.1.0a8/mentpy/__init__.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.407677 mentpy-0.1.0a8/mentpy/calculator/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       68 2023-07-07 03:46:01.000000 mentpy-0.1.0a8/mentpy/calculator/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      137 2023-05-23 00:43:44.000000 mentpy-0.1.0a8/mentpy/calculator/borrows.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1128 2023-05-23 00:43:45.000000 mentpy-0.1.0a8/mentpy/calculator/linalg2.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      137 2023-07-07 16:03:15.000000 mentpy-0.1.0a8/mentpy/calculator/states.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.408422 mentpy-0.1.0a8/mentpy/gradients/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       20 2023-06-10 07:26:23.000000 mentpy-0.1.0a8/mentpy/gradients/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2002 2023-06-10 07:30:42.000000 mentpy-0.1.0a8/mentpy/gradients/_finite_difference.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1599 2023-06-10 07:39:36.000000 mentpy-0.1.0a8/mentpy/gradients/_parameter_shift.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1934 2023-06-10 07:39:36.000000 mentpy-0.1.0a8/mentpy/gradients/grad.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.409194 mentpy-0.1.0a8/mentpy/mbqc/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      343 2023-04-16 02:07:08.000000 mentpy-0.1.0a8/mentpy/mbqc/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    18653 2023-05-31 21:43:20.000000 mentpy-0.1.0a8/mentpy/mbqc/flow.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    29788 2023-07-07 16:03:16.000000 mentpy-0.1.0a8/mentpy/mbqc/mbqcircuit.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.409823 mentpy-0.1.0a8/mentpy/mbqc/states/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      149 2023-05-06 07:23:30.000000 mentpy-0.1.0a8/mentpy/mbqc/states/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      197 2023-05-06 07:23:09.000000 mentpy-0.1.0a8/mentpy/mbqc/states/aklt.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      229 2023-05-06 07:23:14.000000 mentpy-0.1.0a8/mentpy/mbqc/states/cluster.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2976 2023-04-16 05:41:03.000000 mentpy-0.1.0a8/mentpy/mbqc/states/graphstate.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     7716 2023-06-21 22:34:00.000000 mentpy-0.1.0a8/mentpy/mbqc/templates.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.410152 mentpy-0.1.0a8/mentpy/noise/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       34 2023-03-17 21:21:26.000000 mentpy-0.1.0a8/mentpy/noise/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      173 2023-03-17 21:21:26.000000 mentpy-0.1.0a8/mentpy/noise/base_noise.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.410962 mentpy-0.1.0a8/mentpy/operators/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      285 2023-05-10 00:16:14.000000 mentpy-0.1.0a8/mentpy/operators/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3693 2023-06-28 21:20:40.000000 mentpy-0.1.0a8/mentpy/operators/controlled_ment.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1599 2023-05-07 19:04:31.000000 mentpy-0.1.0a8/mentpy/operators/gates.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     8449 2023-06-28 21:20:41.000000 mentpy-0.1.0a8/mentpy/operators/ment.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     5931 2023-05-31 23:51:54.000000 mentpy-0.1.0a8/mentpy/operators/pauliop.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.411880 mentpy-0.1.0a8/mentpy/optimizers/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      245 2023-04-25 08:17:14.000000 mentpy-0.1.0a8/mentpy/optimizers/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3277 2023-06-21 22:51:32.000000 mentpy-0.1.0a8/mentpy/optimizers/adam.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      707 2023-06-21 22:49:12.000000 mentpy-0.1.0a8/mentpy/optimizers/base_optimizer.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      366 2023-06-10 07:32:18.000000 mentpy-0.1.0a8/mentpy/optimizers/bp_tools.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3024 2023-06-21 22:52:45.000000 mentpy-0.1.0a8/mentpy/optimizers/rcd.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2814 2023-06-21 23:18:49.000000 mentpy-0.1.0a8/mentpy/optimizers/sgd.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.413530 mentpy-0.1.0a8/mentpy/simulators/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      281 2023-04-16 02:18:15.000000 mentpy-0.1.0a8/mentpy/simulators/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2441 2023-05-07 19:04:31.000000 mentpy-0.1.0a8/mentpy/simulators/base_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1156 2023-04-18 08:22:14.000000 mentpy-0.1.0a8/mentpy/simulators/cirq_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    19570 2023-07-16 02:01:47.000000 mentpy-0.1.0a8/mentpy/simulators/np_simulator_dm.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    19392 2023-06-02 22:34:53.000000 mentpy-0.1.0a8/mentpy/simulators/np_simulator_sv.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2678 2023-05-18 06:35:37.000000 mentpy-0.1.0a8/mentpy/simulators/pattern_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     5677 2023-05-18 08:04:21.000000 mentpy-0.1.0a8/mentpy/simulators/pennylane_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1254 2023-04-25 08:57:09.000000 mentpy-0.1.0a8/mentpy/simulators/qiskit_simulators.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.414510 mentpy-0.1.0a8/mentpy/utils/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      140 2023-05-23 00:17:19.000000 mentpy-0.1.0a8/mentpy/utils/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     6673 2023-04-25 08:57:09.000000 mentpy-0.1.0a8/mentpy/utils/expressivity.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3183 2023-04-16 01:51:56.000000 mentpy-0.1.0a8/mentpy/utils/flow_space.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     4466 2023-04-16 01:44:39.000000 mentpy-0.1.0a8/mentpy/utils/generate_data.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    10395 2023-05-06 07:13:49.000000 mentpy-0.1.0a8/mentpy/utils/lc_equivalence.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     5403 2023-06-28 16:40:04.000000 mentpy-0.1.0a8/mentpy/utils/lie_algebra.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.406856 mentpy-0.1.0a8/mentpy.egg-info/
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3336 2023-07-17 00:07:07.000000 mentpy-0.1.0a8/mentpy.egg-info/PKG-INFO
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1588 2023-07-17 00:07:07.000000 mentpy-0.1.0a8/mentpy.egg-info/SOURCES.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)        1 2023-07-17 00:07:07.000000 mentpy-0.1.0a8/mentpy.egg-info/dependency_links.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)       49 2023-07-17 00:07:07.000000 mentpy-0.1.0a8/mentpy.egg-info/requires.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)        7 2023-07-17 00:07:07.000000 mentpy-0.1.0a8/mentpy.egg-info/top_level.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)       38 2023-07-17 00:07:07.416229 mentpy-0.1.0a8/setup.cfg
+-rw-r--r--   0 luismantilla   (501) staff       (20)      553 2023-07-17 00:06:20.000000 mentpy-0.1.0a8/setup.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.415043 mentpy-0.1.0a8/tests/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       58 2023-04-16 01:51:49.000000 mentpy-0.1.0a8/tests/test_flow.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)       64 2023-04-16 01:52:08.000000 mentpy-0.1.0a8/tests/test_graph_state.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      579 2023-04-16 01:52:23.000000 mentpy-0.1.0a8/tests/test_mbqc_templates.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2110 2023-05-18 06:15:48.000000 mentpy-0.1.0a8/tests/test_simulators.py
```

### Comparing `mentpy-0.1.0a7/LICENSE` & `mentpy-0.1.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a7/PKG-INFO` & `mentpy-0.1.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentpy
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: A Python library for simulating MBQC circuits
 Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla
 Author-email: luismantilla99@outlook.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a7 Summary: A Python library
+Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a8 Summary: A Python library
 for simulating MBQC circuits Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla Author-email: luismantilla99@outlook.com Description-
 Content-Type: text/markdown License-File: LICENSE
           [MentPy: A Measurement-Based Quantum computing simulator.]
   [https://img.shields.io/pypi/v/mentpy]  [https://img.shields.io/pypi/wheel/
     mentpy] [Documentation_Status]  [https://img.shields.io/twitter/follow/
                  mentpy?label=mentpy&style=flat&logo=twitter]
```

### Comparing `mentpy-0.1.0a7/README.md` & `mentpy-0.1.0a8/README.md`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a7/mentpy/calculator/linalg2.py` & `mentpy-0.1.0a8/mentpy/calculator/linalg2.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a7/mentpy/gradients/finite_difference.py` & `mentpy-0.1.0a8/mentpy/gradients/_finite_difference.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
 
-def estimate_gradient(f, x, h=1e-5, type="central"):
+def fd_gradient(f, x, h=1e-5, type="central"):
     if type not in ["central", "forward", "backward"]:
         raise UserWarning(
             f"Expected type to be 'central', 'forward', or 'backward' but {type} was given"
         )
 
     grad = np.zeros(len(x))
     for i in range(len(x)):
@@ -16,15 +16,15 @@
         elif type == "forward":
             grad[i] = (f(x + h * np.eye(len(x))[i]) - f(x)) / h
         elif type == "backward":
             grad[i] = (f(x) - f(x - h * np.eye(len(x))[i])) / h
     return grad
 
 
-def estimate_hessian(f, x, h=1e-5, type="central"):
+def fd_hessian(f, x, h=1e-5, type="central"):
     if type not in ["central", "forward", "backward"]:
         raise UserWarning(
             f"Expected type to be 'central', 'forward', or 'backward' but {type} was given"
         )
 
     hess = np.zeros((len(x), len(x)))
     for i in range(len(x)):
```

### Comparing `mentpy-0.1.0a7/mentpy/mbqc/flow.py` & `mentpy-0.1.0a8/mentpy/mbqc/flow.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a7/mentpy/mbqc/mbqcircuit.py` & `mentpy-0.1.0a8/mentpy/mbqc/mbqcircuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,27 +133,15 @@
         self._flow, self._partial_order = None, None
         self._update_attributes()
 
         if (flow is None) or (partial_order is None):
             flow, partial_order, depth, layers = find_cflow(
                 graph, input_nodes, output_nodes
             )
-            self._layers = layers
-            self.gflow = Flow(
-                graph, input_nodes, output_nodes
-            )  # TODO: make this the standard flow in this class
-            # try:
-            #     flow, partial_order = find_flow(
-            #         graph, input_nodes, output_nodes
-            #     )  # TODO: FIX find_cflow!!!!
-            # except:
-            #     pass
-            # if flow is None:
-            #     flow, partial_order = find_cflow(graph, input_nodes, output_nodes)
-            # depth = None
+            self.gflow = Flow(graph, input_nodes, output_nodes)
 
         elif (flow is not None) and (partial_order is not None):
             check_if_flow(graph, input_nodes, output_nodes, flow, partial_order)
 
         self._flow = flow
         self._partial_order = partial_order
 
@@ -161,29 +149,34 @@
             measurement_order = self.calculate_order()
 
         # in case we measure an output node
         quantum_output_nodes = [
             node for node, i in self.measurements.items() if i is None
         ]
         self._quantum_output_nodes = quantum_output_nodes
-
-        self._depth = depth
         self._measurement_order = measurement_order
 
     def __repr__(self) -> str:
         """Return the representation of the current MBQC circuit state"""
         return f"MBQCircuit with {self.graph.number_of_nodes()} qubits."
 
     def __len__(self) -> int:
         """Return the number of nodes in the MBQCircuit"""
         return len(self.graph)
 
     # if an attribute is not found, look for it in the graph
     def __getattr__(self, name):
-        return getattr(self.graph, name)
+        # try getting the attribute in graph, if not there, look in gflow
+        try:
+            return getattr(self.graph, name)
+        except AttributeError:
+            try:
+                return getattr(self.gflow, name)
+            except AttributeError:
+                raise AttributeError(f"Attribute {name} not found in MBQCircuit.")
 
     def __setitem__(self, key, value):
         r"""Set the value of the measurement of the node with index key."""
         if key not in self.graph.nodes:
             raise ValueError(f"Node {key} is not in the graph.")
         if not isinstance(value, Ment):
             raise ValueError(f"Value {value} is not a Measurement object.")
@@ -287,15 +280,15 @@
     def partial_order(self) -> Callable:
         r"""Return the partial order function of the MBQC circuit."""
         return self._partial_order
 
     @property
     def depth(self) -> int:
         r"""Return the depth of the MBQC circuit."""
-        return self._depth
+        return self.gflow.depth
 
     @property
     def measurement_order(self) -> List[int]:
         r"""Return the measurement order of the MBQC circuit."""
         return self._measurement_order
 
     @measurement_order.setter
@@ -334,15 +327,15 @@
         quantum_outputs = []
         classical_outputs = []
         for nodei, menti in self._measurements.items():
             if menti is not None:
                 if isinstance(menti, ControlMent):
                     controlled_nodes.append(nodei)
 
-                if menti.angle is None:
+                if menti.is_trainable():
                     trainable_nodes.append(nodei)
 
                 planes[nodei] = menti.plane
                 self._measurements[nodei] = copy.deepcopy(menti)
                 self._measurements[nodei].node_id = nodei
                 if nodei in self._output_nodes:
                     classical_outputs.append(nodei)
@@ -651,15 +644,15 @@
 
     show_controls = options.pop("show_controls")
     show_flow = options.pop("show_flow")
     pauliop = options.pop("pauliop")
     edge_color_control = options.pop("edge_color_control")
     style = options.pop("style")
 
-    possible_styles = ("default", "black_and_white")
+    possible_styles = ("default", "black_and_white", "blue_inputs")
     assert style in possible_styles, f"Style must be one of {possible_styles}"
 
     if pauliop is not None:
         options["label"] = "pauliop"
 
     transp = options.pop("transparent")
     fig, ax = plt.subplots(figsize=options.pop("figsize"))
@@ -695,14 +688,18 @@
                 node_colors[i] = "#CCCCCC"
             else:
                 node_colors[i] = "#FFBD59"
 
         if style == "black_and_white":
             node_colors = {i: "#FFFFFF" for i in state.graph.nodes()}
 
+        if style == "blue_inputs":
+            for i in state.input_nodes:
+                node_colors[i] = "#ADD8E6"
+
         options["node_color"] = [node_colors[node] for node in state.graph.nodes()]
 
         fixed_nodes = state.input_nodes + state.output_nodes
         position_xy = {}
         for indx, p in enumerate(state.input_nodes):
             position_xy[p] = (0, -1 * indx)
```

### Comparing `mentpy-0.1.0a7/mentpy/mbqc/states/graphstate.py` & `mentpy-0.1.0a8/mentpy/mbqc/states/graphstate.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a7/mentpy/mbqc/templates.py` & `mentpy-0.1.0a8/mentpy/mbqc/templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,27 +170,31 @@
         mp.draw(g, figsize=(16,5))
 
     Group
     -----
     templates
     """
     options = {
-        "restrict-trainable": True,
+        "restrict_trainable": True,
+        "one_column": False,
     }
+    options.update(kwargs)
 
     SIZE_TRIANGLE = 5
 
     big_graph = None
     for wire in range(n_wires):
+        if options["one_column"] and wire != 0:
+            break
         g = many_wires([SIZE_TRIANGLE] * n_wires)
-        if options["restrict-trainable"]:
+        if options["restrict_trainable"]:
             g.trainable_nodes = list(
                 set(g.trainable_nodes) - set([i - 1 for i in g.output_nodes])
             )
-            # TODO! Make soemthing with this...
+            # TODO! Make something with this...
 
         for connect in range(n_wires):
             if connect != wire:
                 g.add_edge(SIZE_TRIANGLE * wire + 1, SIZE_TRIANGLE * connect)
                 g.add_edge(SIZE_TRIANGLE * wire + 1, SIZE_TRIANGLE * connect + 2)
 
         if big_graph is None:
```

### Comparing `mentpy-0.1.0a7/mentpy/operators/controlled_ment.py` & `mentpy-0.1.0a8/mentpy/operators/controlled_ment.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,16 @@
         condition: Optional[Union[bool, MentOutcome]] = None,
         true_angle: Optional[Union[int, float, tuple, str]] = None,
         true_plane: Optional[str] = "XY",
         false_angle: Optional[Union[int, float, tuple, str]] = 0,
         false_plane: Optional[str] = "X",
     ):
         """Controlled measurement operator."""
-        super().__init__(angle=false_angle, plane=false_plane)
         true_ment = Ment(angle=true_angle, plane=true_plane)
+        super().__init__(angle=false_angle, plane=false_plane)
         self._true_ment = true_ment
         self._condition = condition
 
     def __repr__(self) -> str:
         return (
             f"ControlMent(False: {super().__repr__()}, True: {repr(self._true_ment)})"
         )
@@ -37,15 +37,14 @@
     def condition(self, condition):
         if not isinstance(condition, (bool, MentOutcome)):
             raise TypeError(
                 f"Invalid argument type. Expected bool or MentOutcome but got {type(condition)}"
             )
         self._condition = condition
 
-    @property
     def angle(self, *args, **kwargs):
         if args == () and kwargs == {}:
             if isinstance(self._condition, bool):
                 if self._condition:
                     return self._true_ment.angle
                 else:
                     return super().angle
@@ -55,46 +54,53 @@
                 return super().angle
         else:
             if self.condition(*args, **kwargs):
                 return self._true_ment.angle
             else:
                 return super().angle
 
-    @property
     def plane(self, *args, **kwargs):
         if args == () and kwargs == {}:
             if self._true_ment.plane is None or super().plane is None:
                 return None
             else:
                 return super().plane
         else:
             if self.condition(*args, **kwargs):
                 return self._true_ment.plane
             else:
                 return super().plane
 
-    @property
     def is_trainable(self):
         return super().is_trainable() or self._true_ment.is_trainable()
 
     def copy(self):
         return ControlMent(
             self.condition,
             self._true_ment.angle,
             self._true_ment.plane,
-            self.angle,
-            self.plane,
+            self._angle,
+            self._plane,
         )
 
     def matrix(self, angle: float | None = None, *args, **kwargs):
         """Return the matrix of the controlled measurement operator."""
+        if (not self.is_trainable()) and (angle is not None):
+            raise ValueError("ControlledMent is not trainable, so angle must be None.")
+
         if self.condition(*args, **kwargs):
-            return self._true_ment.matrix(angle, *args, **kwargs)
+            if self._true_ment.is_trainable():
+                return self._true_ment.matrix(angle, *args, **kwargs)
+            else:
+                return self._true_ment.matrix()
         else:
-            return super().matrix(angle, *args, **kwargs)
+            if super().is_trainable():
+                return super().matrix(angle, *args, **kwargs)
+            else:
+                return super().matrix()
 
     def get_povm(self, angle: float | None = None, *args, **kwargs):
         if self.condition(*args, **kwargs):
             return self._true_ment.get_povm(angle, *args, **kwargs)
         else:
             return super().get_povm(angle, *args, **kwargs)
```

### Comparing `mentpy-0.1.0a7/mentpy/operators/gates.py` & `mentpy-0.1.0a8/mentpy/operators/gates.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a7/mentpy/operators/ment.py` & `mentpy-0.1.0a8/mentpy/operators/ment.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,27 @@
 from .gates import PauliX, PauliY, PauliZ
 
 
 class MentOutcome:
     """Measurement outcome class."""
 
     def __init__(self, outcome: Callable[..., bool], node_id=None, cond_nodes=None):
+        if isinstance(outcome, (bool, int)):
+            outcome_value = bool(outcome % 2)
+            outcome = lambda *args, **kwargs: outcome_value
         self._outcome = outcome
         self._node_id = node_id
-        self._cond_nodes = (
-            cond_nodes
-            if cond_nodes is not None
-            else (set([node_id]) if node_id is not None else set())
-        )
+        if isinstance(outcome, MentOutcome):
+            self._cond_nodes = outcome.cond_nodes
+        else:
+            self._cond_nodes = (
+                cond_nodes
+                if cond_nodes is not None
+                else (set([node_id]) if node_id is not None else set())
+            )
 
     @property
     def node_id(self):
         return self._node_id
 
     @node_id.setter
     def node_id(self, node_id):
@@ -37,25 +43,25 @@
             return self._outcome(*args, **kwargs)
         except:
             raise UserWarning("Could not evaluate callable at given")
 
     def _binary_operation(self, operation, other):
         if isinstance(other, (bool, int)):
             return MentOutcome(
-                lambda x: bool(operation(self._outcome(x), other)),
+                lambda x: bool(operation(self._outcome(x), other) % 2),
                 cond_nodes=self._cond_nodes,
             )
         elif isinstance(other, MentOutcome):
             return MentOutcome(
-                lambda x: bool(operation(self._outcome(x), other._outcome(x))),
+                lambda x: bool(operation(self._outcome(x), other._outcome(x)) % 2),
                 cond_nodes=self._cond_nodes | other._cond_nodes,
             )
         elif isinstance(other, Callable):
             return MentOutcome(
-                lambda x: bool(operation(self._outcome(x), other(x))),
+                lambda x: bool(operation(self._outcome(x), other(x)) % 2),
                 cond_nodes=self._cond_nodes,
             )
         else:
             raise TypeError(f"Invalid type {type(other)}")
 
     def __mul__(self, other):
         return self._binary_operation(lambda x, y: x * y, other)
@@ -158,21 +164,21 @@
 
         self._plane = plane
         self._angle = angle
         self._node_id = -1
         self._outcome = MentOutcome(lambda x: x[self._node_id])
 
     def __repr__(self):
-        theta = round(self.angle, 4) if isinstance(self.angle, (int, float)) else "θ"
+        theta = round(self._angle, 4) if isinstance(self._angle, (int, float)) else "θ"
         theta = (
-            (round(self.angle[0], 4), round(self.angle[1], 4))
-            if isinstance(self.angle, tuple)
+            (round(self._angle[0], 4), round(self._angle[1], 4))
+            if isinstance(self._angle, tuple)
             else theta
         )
-        return f"Ment({theta}, {self.plane})"
+        return f"Ment({theta}, {self._plane})"
 
     @property
     def plane(self):
         return self._plane
 
     @property
     def angle(self):
@@ -194,38 +200,38 @@
     def set_angle(self, angle):
         "Sets the angle of the measurement."
         self._angle = angle
         return self
 
     def copy(self):
         "Returns a copy of the measurement."
-        return Ment(self.angle, self.plane)
+        return Ment(self._angle, self._plane)
 
     def is_trainable(self):
         "Returns True if the measurement is trainable."
-        return self.angle is None and self.plane in ["XY", "XZ", "YZ", "XYZ"]
+        return self._angle is None and self._plane in ["XY", "XZ", "YZ", "XYZ"]
 
     def matrix(self, angle: Optional[float] = None, *args, **kwargs):
         "Returns the matrix representation of the measurement."
-        if self.angle is None and angle is None:
+        if self._angle is None and angle is None:
             raise ValueError("Measurement is trainable, please provide an angle.")
-        elif self.angle is not None and angle is not None:
-            if self.angle != angle:
+        elif self._angle is not None and angle is not None:
+            if self._angle != angle:
                 raise ValueError(
-                    f"Measurement has a fixed angle of {round(self.angle, 4)}"
+                    f"Measurement has a fixed angle of {round(self._angle, 4)}"
                 )
-        elif self.angle is not None:
-            angle = self.angle
+        elif self._angle is not None:
+            angle = self._angle
 
-        match self.plane:
+        match self._plane:
             case "XY":
                 matrix = np.cos(angle) * PauliX + np.sin(angle) * PauliY
             case "X" | "Y" | "Z":
                 matrices = {"X": PauliX, "Y": PauliY, "Z": PauliZ}
-                matrix = matrices[self.plane]
+                matrix = matrices[self._plane]
             case "XZ":
                 matrix = np.cos(angle) * PauliX + np.sin(angle) * PauliZ
             case "YZ":
                 matrix = np.cos(angle) * PauliY + np.sin(angle) * PauliZ
             case "XYZ":
                 if isinstance(angle, tuple):
                     angle1, angle2 = angle
```

### Comparing `mentpy-0.1.0a7/mentpy/operators/pauliop.py` & `mentpy-0.1.0a8/mentpy/operators/pauliop.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,19 @@
 
     def __getitem__(self, key):
         paulis = self._array[key]
         if isinstance(key, slice):
             return PauliOp(";".join([pauli.txt for pauli in paulis]))
         return paulis
 
+    def __mul__(self, other: "PauliOp"):
+        """Returns the product of two Pauli operators."""
+        new_matrix = GF(self.matrix) + GF(other.matrix)
+        return PauliOp(new_matrix)
+
     def __contains__(self, item: "PauliOp"):
         for row in item.matrix:
             if not np.any((self.matrix == row).all(axis=1)):
                 return False
         return True
 
     def __hash__(self):
@@ -141,14 +146,16 @@
                 elif char == "Y":
                     mat[i, j] = 1
                     mat[i, j + n_qubits] = 1
         return GF(mat)
 
     def commutator(self, other) -> "PauliOp":
         """Returns the commutator of two Pauli operators."""
+        if not self.symplectic_prod(other):
+            return 0
         new_matrix = GF(self.matrix) + GF(other.matrix)
         return PauliOp(new_matrix)
 
     def symplectic_prod(self, other):
         """Returns the symplectic product of two Pauli operators."""
         x1 = self.matrix[:, : self.matrix.shape[1] // 2]
         x2 = other.matrix[:, : other.matrix.shape[1] // 2]
```

### Comparing `mentpy-0.1.0a7/mentpy/optimizers/base_optimizer.py` & `mentpy-0.1.0a8/mentpy/optimizers/base_optimizer.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     optimizers
     """
 
     def __init__(self, *args, **kwargs):
         pass
 
     @abc.abstractmethod
+    def step(self, *args, **kwargs):
+        pass
+
+    @abc.abstractmethod
     def optimize(self, *args, **kwargs):
         pass
 
     @abc.abstractmethod
     def optimize_and_gradient_norm(self, *args, **kwargs):
         pass
```

### Comparing `mentpy-0.1.0a7/mentpy/optimizers/rcd.py` & `mentpy-0.1.0a8/mentpy/optimizers/rcd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from mentpy.optimizers.base_optimizer import BaseOptimizer
-from mentpy.gradients import estimate_gradient
 
 import numpy as np
 import random
 
 
 class RCDOptimizer(BaseOptimizer):
     """Class for the random coordinate descent optimizer.
@@ -30,37 +29,38 @@
     """
 
     def __init__(self, step_size=0.1, adaptive=False) -> None:
         """Initialize the random coordinate descent optimizer."""
         self.step_size = step_size
         self.adaptive = adaptive
 
+    def step(self, f, x, i, **kwargs):
+        """Take a step using the random coordinate descent optimizer."""
+        coord_idx = random.randint(0, len(x) - 1)
+        delta = np.zeros_like(x)
+        delta[coord_idx] = 1e-5
+        partial_gradient = (f(x + delta) - f(x - delta)) / (2 * delta[coord_idx])
+
+        current_step_size = self.step_size
+        if self.adaptive:
+            current_step_size /= np.sqrt(i + 1)
+
+        x[coord_idx] -= current_step_size * partial_gradient
+
+        return x
+
     def optimize(self, f, x0, num_iters=100, callback=None, verbose=False, **kwargs):
         """Optimize a function f using the random coordinate descent optimizer."""
         x = x0
-        coord_iters = np.zeros(len(x))
-
         for i in range(num_iters):
-            # Random coordinate descent optimizer
-            coord_idx = random.randint(0, len(x) - 1)
-            coord_iters[coord_idx] += 1
-            delta = np.zeros_like(x)
-            delta[coord_idx] = 1e-5
-            partial_gradient = (f(x + delta) - f(x - delta)) / (2 * delta[coord_idx])
-
-            current_step_size = self.step_size
-            if self.adaptive:
-                current_step_size /= np.sqrt(coord_iters[coord_idx])
-
-            x[coord_idx] -= current_step_size * partial_gradient
-
+            x = self.step(f, x, i, **kwargs)
             if callback is not None:
                 callback(x, i)
             if verbose:
-                print(f"Iteration {i+1} of {num_iters}: {x} with value {f(x)}")
+                print(f"Iteration {i+1}/{num_iters}")
         return x
 
     def update_step_size(self, x, i, factor=0.99):
         """Update the step size of the optimizer."""
         self.step_size = self.step_size * factor
 
     def optimize_and_gradient_norm(
```

### Comparing `mentpy-0.1.0a7/mentpy/optimizers/sgd.py` & `mentpy-0.1.0a8/mentpy/optimizers/sgd.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from mentpy.optimizers.base_optimizer import BaseOptimizer
-from mentpy.gradients import estimate_gradient
+from mentpy.gradients import get_gradient
 
 import numpy as np
 
 
 class SGDOptimizer(BaseOptimizer):
     """Class for the SGD optimizer.
 
@@ -35,32 +35,37 @@
     """
 
     def __init__(self, step_size=0.1, momentum=0.0, nesterov=False) -> None:
         """Initialize the SGD optimizer."""
         self.step_size = step_size
         self.momentum = momentum
         self.nesterov = nesterov
+        self.v = None
+
+    def step(self, f, x, i, **kwargs):
+        """Take a step of the SGD optimizer."""
+        g = get_gradient(f, x, **kwargs)
+        if self.v is None:
+            self.v = np.zeros(len(x))
+        self.v = self.momentum * self.v - self.step_size * g
+        if self.nesterov:
+            x = x + self.momentum * self.v - self.step_size * g
+        else:
+            x = x + self.v
+        return x
 
     def optimize(self, f, x0, num_iters=100, callback=None, verbose=False, **kwargs):
         """Optimize a function f using the SGD optimizer."""
-        v = np.zeros(len(x0))
         x = x0
-
         for i in range(num_iters):
-            # SGD Optimizer
-            g = estimate_gradient(f, x, **kwargs)
-            v = self.momentum * v - self.step_size * g
-            if self.nesterov:
-                x = x + self.momentum * v - self.step_size * g
-            else:
-                x = x + v
+            x = self.step(f, x, i, **kwargs)
             if callback is not None:
                 callback(x, i)
             if verbose:
-                print(f"Iteration {i+1} of {num_iters}: {x} with value {f(x)}")
+                print(f"Iteration {i+1}/{num_iters}")
         return x
 
     def update_step_size(self, x, i, factor=0.99):
         """Update the step size of the optimizer."""
         self.step_size = self.step_size * factor
 
     def optimize_and_gradient_norm(
@@ -68,22 +73,23 @@
     ):
         """Optimize a function f using the SGD optimizer."""
         v = np.zeros(len(x0))
         x = x0
         norm = []
         for i in range(num_iters):
             # SGD Optimizer
-            g = estimate_gradient(f, x, **kwargs)
+            g = get_gradient(f, x, **kwargs)
             norm.append(np.linalg.norm(g))
             v = self.momentum * v - self.step_size * g
             if self.nesterov:
                 x = x + self.momentum * v - self.step_size * g
             else:
                 x = x + v
             if callback is not None:
                 callback(x, i)
             if verbose:
                 print(f"Iteration {i+1} of {num_iters}: {x} with value {f(x)}")
         return x, norm
 
     def reset(self, *args, **kwargs):
-        pass
+        """Reset the optimizer."""
+        self.v = None
```

### Comparing `mentpy-0.1.0a7/mentpy/simulators/base_simulator.py` & `mentpy-0.1.0a8/mentpy/simulators/base_simulator.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a7/mentpy/simulators/cirq_simulator.py` & `mentpy-0.1.0a8/mentpy/simulators/cirq_simulator.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a7/mentpy/simulators/np_simulator_dm.py` & `mentpy-0.1.0a8/mentpy/simulators/np_simulator_dm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union, List, Tuple, Optional
 
 import numpy as np
 import math
 import networkx as nx
 
-from mentpy.operators import Ment
+from mentpy.operators import Ment, ControlledMent
 from mentpy.mbqc.mbqcircuit import MBQCircuit
 from mentpy.simulators.base_simulator import BaseSimulator
 
 # COMMON GATES
 H = np.array([[1, 1], [1, -1]]) / np.sqrt(2)
 S = np.array([[1, 0], [0, 1j]])
 Pi8 = np.array([[1, 0], [0, np.exp(1j * np.pi / 4)]])
@@ -28,22 +28,24 @@
         self, mbqcircuit: MBQCircuit, input_state: np.ndarray = None, **kwargs
     ) -> None:
         super().__init__(mbqcircuit, input_state)
 
         self.window_size = kwargs.pop("window_size", 1)
         self.schedule = kwargs.pop("schedule", None)
         self.force0 = kwargs.pop("force0", True)
+        self.dev_mode = kwargs.pop("dev_mode", False)
+        self.wires = kwargs.pop("wires", None)
 
         if not self.force0:
             raise NotImplementedError("Numpy simulator does not support force0=False.")
 
         # TODO: FIND SCHEDULE IF NOT PROVIDED
         if self.schedule is not None:
             self.schedule_measure = [
-                i for i in self.schedule if i not in mbqcircuit.measurements.values()
+                i for i in self.schedule if i not in mbqcircuit.quantum_output_nodes
             ]
         elif mbqcircuit.measurement_order is not None:
             # remove output nodes from the measurement order
             self.schedule_measure = [
                 i
                 for i in mbqcircuit.measurement_order
                 if i not in mbqcircuit.quantum_output_nodes
@@ -85,14 +87,17 @@
         # get subgraph of the first window_size nodes
         self.subgraph = self.mbqcircuit.graph.subgraph(
             self.schedule[: self.window_size]
         )
 
         self.initial_czs = np.eye(2**self.window_size)
 
+        if self.dev_mode:
+            self._current_simulated_nodes = self.schedule[0 : self.window_size]
+
         # apply cz gates to neighboring qubits
         for node in self.subgraph.nodes:
             for neighbour in self.subgraph.neighbors(node):
                 # avoid repeated application of cz gates
                 if node < neighbour:
                     indx = self.current_simulated_nodes().index(node)
                     indy = self.current_simulated_nodes().index(neighbour)
@@ -101,41 +106,93 @@
                     self.initial_czs = cz @ self.initial_czs
 
         self.qstate = self.initial_czs @ self.qstate @ np.conj(self.initial_czs).T
         self.outcomes = {}
 
     def current_simulated_nodes(self) -> List[int]:
         """Returns the nodes that are currently simulated."""
-        return self.schedule[
-            self.current_measurement : self.current_measurement + self.window_size
-        ]
+        if not self.dev_mode:
+            return self.schedule[
+                self.current_measurement : self.current_measurement + self.window_size
+            ]
+        elif self.dev_mode:
+            return self._current_simulated_nodes
 
     def current_number_simulated_nodes(self) -> int:
         """Returns the number of nodes that are currently simulated."""
         n = self.window_size
         return min(n, len(self.mbqcircuit) - self.current_measurement)
 
+    def node_in_which_wire(self, node: int) -> int:
+        """Returns the wire in which the node is."""
+        for i, wire in enumerate(self.wires):
+            if node in wire:
+                return i
+
+    def neighbors_in_wire(self, node: int) -> List[int]:
+        """Returns the neighbors of a node in the same wire."""
+        wire = self.wires[self.node_in_which_wire(node)]
+        # return nodes that have edges with node
+        return [n for n in wire if self.mbqcircuit.graph.has_edge(node, n)]
+
+    def future_neighbors_in_wire(self, node: int) -> List[int]:
+        neighs = self.neighbors_in_wire(node)
+        future_neighs = []
+        for neigh in neighs:
+            if neigh > node:
+                future_neighs.append(neigh)
+        return future_neighs
+
     def measure(self, angle: float, mode="sample") -> Tuple:
         if self.current_measurement >= len(self.schedule_measure):
             raise ValueError("No more measurements to be done.")
 
-        current_ment = self.mbqcircuit[
-            self.schedule_measure[self.current_measurement]
-        ].copy()
+        if not self.dev_mode:
+            current_ment = self.mbqcircuit[
+                self.schedule_measure[self.current_measurement]
+            ].copy()
+            indx = 0
+        elif self.dev_mode:
+            # if in dev mode, we measure the first node in the current_simulated_nodes
+            # only if a neighbor in the same wire is also in the current_simulated_nodes
+            for node in self.current_simulated_nodes():
+                cond = False
+                futnods = self.future_neighbors_in_wire(node)
+                if len(futnods) == 0:
+                    cond = True
+                else:
+                    cond = futnods[0] in self.current_simulated_nodes()
+                if cond:
+                    current_ment = self.mbqcircuit[node].copy()
+                    indx = self.current_simulated_nodes().index(node)
+                    break
+
         self.qstate, outcome = self.measure_ment(
-            current_ment, angle, 0, force0=self.force0, mode=mode
+            current_ment, angle, indx, force0=self.force0, mode=mode
         )
         # check if qstate has nan
         if np.isnan(self.qstate).any():
             raise ValueError(
                 "qstate has nan, you might want to increase the window size"
             )
         self.current_measurement += 1
 
-        self.qstate = self.partial_trace(self.qstate, [0])
+        self.qstate = self.partial_trace(self.qstate, [indx])
+
+        if self.dev_mode:
+            # remove qubit at indx from current_simulated_nodes
+            self._current_simulated_nodes = [
+                i for i in self._current_simulated_nodes if i != node
+            ]
+            if self.current_measurement + self.window_size <= len(
+                self.mbqcircuit.graph.nodes
+            ):
+                self._current_simulated_nodes.append(
+                    self.schedule[self.current_measurement + self.window_size - 1]
+                )
 
         if self.current_measurement + self.window_size <= len(
             self.mbqcircuit.graph.nodes
         ):
             self.qstate = np.kron(self.qstate, self.pure2density(qubit_plus))
             new_qubit = self.current_simulated_nodes()[-1]
 
@@ -148,30 +205,62 @@
                 if neighbour in self.current_simulated_nodes():
                     indxn = self.current_simulated_nodes().index(neighbour)
                     cz = self.controlled_z(indxn, indx_new, self.window_size)
                     self.qstate = cz @ self.qstate @ np.conj(cz.T)
 
         return self.qstate, outcome
 
-    def run(self, angles: List[float], mode="sample") -> Tuple[List[int], np.ndarray]:
+    def run(
+        self, angles: List[float], mode="sample", input_state=None
+    ) -> Tuple[List[int], np.ndarray]:
         """Measures the quantum state in the given pattern."""
+        if input_state is not None:
+            self.reset(input_state=input_state)
 
         if len(angles) != len(self.mbqcircuit.trainable_nodes):
             raise ValueError(
                 f"Number of angles ({len(angles)}) does not match number of trainable nodes ({len(self.mbqcircuit.trainable_nodes)})."
             )
 
-        for i in self.schedule_measure:
-            if i in self.mbqcircuit.trainable_nodes:
-                angle = angles[self.mbqcircuit.trainable_nodes.index(i)]
-            else:
-                angle = self.mbqcircuit[i].angle
+        if not self.dev_mode:
+            for i in self.schedule_measure:
+                if i in self.mbqcircuit.trainable_nodes:
+                    angle = angles[self.mbqcircuit.trainable_nodes.index(i)]
+                else:
+                    angle = self.mbqcircuit[i].angle
 
-            self.qstate, outcome = self.measure(angle, mode)
-            self.outcomes[i] = outcome
+                self.qstate, outcome = self.measure(angle, mode)
+                self.outcomes[i] = outcome
+
+        elif self.dev_mode:
+            while self.current_measurement < len(self.schedule_measure):
+                for node in self.current_simulated_nodes():
+                    cond = False
+                    futnods = self.future_neighbors_in_wire(node)
+                    if len(futnods) == 0:
+                        cond = True
+                    else:
+                        cond = futnods[0] in self.current_simulated_nodes()
+                    if cond:
+                        # current_ment = self.mbqcircuit[node].copy()
+                        # indx = self.current_simulated_nodes().index(node)
+                        break
+
+                if cond == False:
+                    raise ValueError("WTF")
+                if node in self.mbqcircuit.trainable_nodes:
+                    angle = angles[self.mbqcircuit.trainable_nodes.index(node)]
+                    if isinstance(self.mbqcircuit[node], ControlledMent):
+                        cond_angle = self.mbqcircuit[node].angle(self.outcomes) or angle
+                        angle = cond_angle
+                elif isinstance(self.mbqcircuit[node], Ment):
+                    angle = self.mbqcircuit[node].angle
+
+                self.qstate, outcome = self.measure(angle, mode)
+                self.outcomes[node] = outcome
 
         current_output_order = [
             i for i in self.schedule if i not in self.schedule_measure
         ]
         if self.mbqcircuit.quantum_output_nodes != current_output_order:
             self.qstate = self.reorder_qubits(
                 self.qstate, current_output_order, self.mbqcircuit.quantum_output_nodes
@@ -202,14 +291,17 @@
                 self.input_state = np.kron(self.input_state, qubit_plus)
 
         self.qstate = self.pure2density(self.input_state)
 
         self.qstate = self.initial_czs @ self.qstate @ np.conj(self.initial_czs).T
         self.outcomes = {}
 
+        if self.dev_mode:
+            self._current_simulated_nodes = self.schedule[0 : self.window_size]
+
     def arbitrary_qubit_gate(self, u, i, n):
         """
         Single qubit gate u acting on qubit i
         n is the number of qubits
         """
         op = 1
         for k in range(0, n):
@@ -279,14 +371,15 @@
             sigma = sigma + np.conjugate(ptrace.T) @ rho @ (ptrace)
         return sigma
 
     def measure_ment(self, ment: Ment, angle, i, force0=False, mode="sample"):
         """
         Measures a ment
         """
+
         op = ment.matrix(angle, self.outcomes)
         if op is None:
             raise ValueError(f"Ment has no matrix representation at qubit {i}")
 
         p0, p1 = ment.get_povm(angle, self.outcomes)
         p0_extended = self.arbitrary_qubit_gate(
             p0, i, self.current_number_simulated_nodes()
```

### Comparing `mentpy-0.1.0a7/mentpy/simulators/np_simulator_sv.py` & `mentpy-0.1.0a8/mentpy/simulators/np_simulator_sv.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,22 +209,24 @@
                     indxn = self.current_simulated_nodes().index(neighbour)
                     cz = self.controlled_z(indxn, indx_new, self.window_size)
                     self.qstate = cz @ self.qstate
 
         return self.qstate, outcome
 
     def run(
-        self, angles: List[float], output_form="dm"
+        self, angles: List[float], output_form="dm", **kwargs
     ) -> Tuple[List[int], np.ndarray]:
         """Measures the quantum state in the given pattern.
 
         Args:
             angles (List[float]): List of angles to be used for the measurements.
             output_form (str): Output form of the quantum state. Can be 'dm' for density matrix or 'sv' for statevector.
         """
+        if kwargs.get("input_state") is not None:
+            self.reset(input_state=kwargs.get("input_state"))
 
         if len(angles) != len(self.mbqcircuit.trainable_nodes):
             raise ValueError(
                 f"Number of angles ({len(angles)}) does not match number of trainable nodes ({len(self.mbqcircuit.trainable_nodes)})."
             )
 
         if not self.dev_mode:
```

### Comparing `mentpy-0.1.0a7/mentpy/simulators/pattern_simulator.py` & `mentpy-0.1.0a8/mentpy/simulators/pattern_simulator.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a7/mentpy/simulators/pennylane_simulator.py` & `mentpy-0.1.0a8/mentpy/simulators/pennylane_simulator.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a7/mentpy/simulators/qiskit_simulators.py` & `mentpy-0.1.0a8/mentpy/simulators/qiskit_simulators.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a7/mentpy/utils/expressivity.py` & `mentpy-0.1.0a8/mentpy/utils/expressivity.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a7/mentpy/utils/flow_space.py` & `mentpy-0.1.0a8/mentpy/utils/flow_space.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a7/mentpy/utils/generate_data.py` & `mentpy-0.1.0a8/mentpy/utils/generate_data.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a7/mentpy/utils/lc_equivalence.py` & `mentpy-0.1.0a8/mentpy/utils/lc_equivalence.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a7/mentpy/utils/lie_algebra.py` & `mentpy-0.1.0a8/mentpy/utils/lie_algebra.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,15 @@
     mapping = state.index_mapping()
     mo = [mapping[i] for i in mo]
     j = mapping[j]
 
     A = []
     b = []
     for k in mo:
-        indk = mo.index(k)
-        indj = mo.index(j)
-        if indk <= indj:
+        if (not state.partial_order(j, k)) or k == j:
             A.append(stabilizers[k].matrix[0, : len(mo)])
             b.append(np.zeros(1, dtype=int))
 
     for k in [mapping[i] for i in state.outputc]:
         A.append(stabilizers[k].matrix[0, len(mo) :])
         p = 0 if k != j else 1
         b.append(np.array([p]))
@@ -50,15 +48,15 @@
 
     if not _check_solution(A, b, sol):
         raise ValueError("Solution not found for j: " + str(j))
 
     op = PauliOp("I" * len(state.measurement_order))
     for i in range(len(sol)):
         if sol[i] == 1:
-            op = op.commutator(stabilizers[i])
+            op = op * stabilizers[i]
     return op
 
 
 def calculate_complete_gens_lie_algebra(state: MBQCircuit):
     """Calculates the Pauli operators for the Lie algebra of a given state"""
     graph_stabs = state.stabilizers()
 
@@ -128,17 +126,18 @@
     while iter < max_iter and queue:
         iter += 1
         x, y = queue.pop(0)
         if (x, y) not in already_commutated and (y, x) not in already_commutated:
             already_commutated.add((x, y))
             already_commutated.add((y, x))
             newOp = x.commutator(y)
-            if newOp not in lieAlg:
-                lieAlg.append(newOp)
-                queue.extend((newOp, k) for k in lieAlg if k != newOp)
+            if isinstance(newOp, PauliOp):
+                if newOp not in lieAlg:
+                    lieAlg.append(newOp)
+                    queue.extend((newOp, k) for k in lieAlg if k != newOp)
 
     if iter >= max_iter - 1 and queue:
         raise ValueError("Max iterations reached")
 
     # check IIII is in lieAlg
     identityPauli = PauliOp("I" * int(lieAlg[0].matrix.shape[1] // 2))
     if identityPauli not in lieAlg:
```

### Comparing `mentpy-0.1.0a7/mentpy.egg-info/PKG-INFO` & `mentpy-0.1.0a8/mentpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentpy
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: A Python library for simulating MBQC circuits
 Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla
 Author-email: luismantilla99@outlook.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a7 Summary: A Python library
+Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a8 Summary: A Python library
 for simulating MBQC circuits Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla Author-email: luismantilla99@outlook.com Description-
 Content-Type: text/markdown License-File: LICENSE
           [MentPy: A Measurement-Based Quantum computing simulator.]
   [https://img.shields.io/pypi/v/mentpy]  [https://img.shields.io/pypi/wheel/
     mentpy] [Documentation_Status]  [https://img.shields.io/twitter/follow/
                  mentpy?label=mentpy&style=flat&logo=twitter]
```

### Comparing `mentpy-0.1.0a7/mentpy.egg-info/SOURCES.txt` & `mentpy-0.1.0a8/mentpy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 mentpy.egg-info/SOURCES.txt
 mentpy.egg-info/dependency_links.txt
 mentpy.egg-info/requires.txt
 mentpy.egg-info/top_level.txt
 mentpy/calculator/__init__.py
 mentpy/calculator/borrows.py
 mentpy/calculator/linalg2.py
+mentpy/calculator/states.py
 mentpy/gradients/__init__.py
-mentpy/gradients/finite_difference.py
+mentpy/gradients/_finite_difference.py
+mentpy/gradients/_parameter_shift.py
+mentpy/gradients/grad.py
 mentpy/mbqc/__init__.py
 mentpy/mbqc/flow.py
 mentpy/mbqc/mbqcircuit.py
 mentpy/mbqc/templates.py
 mentpy/mbqc/states/__init__.py
 mentpy/mbqc/states/aklt.py
 mentpy/mbqc/states/cluster.py
```

### Comparing `mentpy-0.1.0a7/setup.py` & `mentpy-0.1.0a8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "0.1.0a7"
+version = "0.1.0a8"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="mentpy",
     version=version,
```

### Comparing `mentpy-0.1.0a7/tests/test_mbqc_templates.py` & `mentpy-0.1.0a8/tests/test_mbqc_templates.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a7/tests/test_simulators.py` & `mentpy-0.1.0a8/tests/test_simulators.py`

 * *Files identical despite different names*

