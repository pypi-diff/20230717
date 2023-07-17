# Comparing `tmp/coba-6.5.0.tar.gz` & `tmp/coba-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\coba-6.5.0.tar", last modified: Sun May 28 19:12:44 2023, max compression
+gzip compressed data, was "C:\Users\Mark\Projects\coba\dist\.tmp-b59ppplj\coba-7.0.0.tar", last modified: Mon Jul 17 05:11:17 2023, max compression
```

## Comparing `coba-6.5.0.tar` & `coba-7.0.0.tar`

### file list

```diff
@@ -1,74 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/
--rw-rw-rw-   0        0        0       40 2023-05-11 00:41:22.000000 coba-6.5.0/AUTHORS
--rw-rw-rw-   0        0        0     1593 2023-05-11 00:41:22.000000 coba-6.5.0/LICENSE
--rw-rw-rw-   0        0        0     7933 2023-05-28 19:12:44.000000 coba-6.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     7336 2023-05-11 00:41:22.000000 coba-6.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba/
--rw-rw-rw-   0        0        0     2406 2023-05-24 18:06:29.000000 coba-6.5.0/coba/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba/backports/
--rw-rw-rw-   0        0        0      222 2023-05-11 00:41:22.000000 coba-6.5.0/coba/backports/__init__.py
--rw-rw-rw-   0        0        0      473 2023-05-11 00:41:22.000000 coba-6.5.0/coba/backports/metadata.py
--rw-rw-rw-   0        0        0      143 2023-05-11 00:41:22.000000 coba-6.5.0/coba/backports/typing.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba/contexts/
--rw-rw-rw-   0        0        0     1035 2023-05-11 00:41:22.000000 coba-6.5.0/coba/contexts/__init__.py
--rw-rw-rw-   0        0        0     9727 2023-05-11 00:41:22.000000 coba-6.5.0/coba/contexts/cachers.py
--rw-rw-rw-   0        0        0     9263 2023-05-11 00:41:22.000000 coba-6.5.0/coba/contexts/core.py
--rw-rw-rw-   0        0        0     9726 2023-05-11 00:41:22.000000 coba-6.5.0/coba/contexts/loggers.py
--rw-rw-rw-   0        0        0    15634 2023-05-11 00:41:22.000000 coba-6.5.0/coba/encodings.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba/environments/
--rw-rw-rw-   0        0        0     2317 2023-05-11 00:41:22.000000 coba-6.5.0/coba/environments/__init__.py
--rw-rw-rw-   0        0        0    22278 2023-05-15 01:59:07.000000 coba-6.5.0/coba/environments/core.py
--rw-rw-rw-   0        0        0    50314 2023-05-28 18:39:49.000000 coba-6.5.0/coba/environments/filters.py
--rw-rw-rw-   0        0        0    14343 2023-05-11 00:41:22.000000 coba-6.5.0/coba/environments/openml.py
--rw-rw-rw-   0        0        0     7792 2023-05-11 00:41:22.000000 coba-6.5.0/coba/environments/primitives.py
--rw-rw-rw-   0        0        0     3014 2023-05-11 00:41:22.000000 coba-6.5.0/coba/environments/serialized.py
--rw-rw-rw-   0        0        0     9630 2023-05-18 00:29:59.000000 coba-6.5.0/coba/environments/supervised.py
--rw-rw-rw-   0        0        0    24199 2023-05-11 00:41:22.000000 coba-6.5.0/coba/environments/synthetics.py
--rw-rw-rw-   0        0        0     6179 2023-05-11 00:41:22.000000 coba-6.5.0/coba/environments/templates.py
--rw-rw-rw-   0        0        0     1126 2023-05-11 00:41:22.000000 coba-6.5.0/coba/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba/experiments/
--rw-rw-rw-   0        0        0     1050 2023-05-14 20:33:18.000000 coba-6.5.0/coba/experiments/__init__.py
--rw-rw-rw-   0        0        0     9556 2023-05-12 13:18:19.000000 coba-6.5.0/coba/experiments/core.py
--rw-rw-rw-   0        0        0     9312 2023-05-11 00:41:22.000000 coba-6.5.0/coba/experiments/process.py
--rw-rw-rw-   0        0        0    52540 2023-05-19 22:26:08.000000 coba-6.5.0/coba/experiments/results.py
--rw-rw-rw-   0        0        0    39708 2023-05-28 18:57:52.000000 coba-6.5.0/coba/experiments/tasks.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba/learners/
--rw-rw-rw-   0        0        0     1155 2023-05-24 18:07:17.000000 coba-6.5.0/coba/learners/__init__.py
--rw-rw-rw-   0        0        0     7907 2023-05-11 00:41:22.000000 coba-6.5.0/coba/learners/bandit.py
--rw-rw-rw-   0        0        0     8055 2023-05-24 19:10:26.000000 coba-6.5.0/coba/learners/corral.py
--rw-rw-rw-   0        0        0     5010 2023-05-11 00:41:22.000000 coba-6.5.0/coba/learners/linucb.py
--rw-rw-rw-   0        0        0     4376 2023-05-27 01:06:49.000000 coba-6.5.0/coba/learners/primitives.py
--rw-rw-rw-   0        0        0     9021 2023-05-26 14:25:09.000000 coba-6.5.0/coba/learners/safety.py
--rw-rw-rw-   0        0        0    30752 2023-05-28 18:41:36.000000 coba-6.5.0/coba/learners/vowpal.py
--rw-rw-rw-   0        0        0     4288 2023-05-11 00:41:22.000000 coba-6.5.0/coba/multiprocessing.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba/pipes/
--rw-rw-rw-   0        0        0     2378 2023-05-11 00:41:22.000000 coba-6.5.0/coba/pipes/__init__.py
--rw-rw-rw-   0        0        0     1890 2023-05-15 13:57:18.000000 coba-6.5.0/coba/pipes/core.py
--rw-rw-rw-   0        0        0    15589 2023-05-11 00:41:22.000000 coba-6.5.0/coba/pipes/filters.py
--rw-rw-rw-   0        0        0    15095 2023-05-11 00:41:22.000000 coba-6.5.0/coba/pipes/multiprocessing.py
--rw-rw-rw-   0        0        0     6622 2023-05-11 00:41:22.000000 coba-6.5.0/coba/pipes/primitives.py
--rw-rw-rw-   0        0        0    13003 2023-05-18 00:30:21.000000 coba-6.5.0/coba/pipes/readers.py
--rw-rw-rw-   0        0        0    18327 2023-05-18 00:32:45.000000 coba-6.5.0/coba/pipes/rows.py
--rw-rw-rw-   0        0        0     3734 2023-05-11 00:41:22.000000 coba-6.5.0/coba/pipes/sinks.py
--rw-rw-rw-   0        0        0     6115 2023-05-12 03:29:30.000000 coba-6.5.0/coba/pipes/sources.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba/primitives/
--rw-rw-rw-   0        0        0      928 2023-05-11 00:41:22.000000 coba-6.5.0/coba/primitives/__init__.py
--rw-rw-rw-   0        0        0      942 2023-05-11 00:41:22.000000 coba-6.5.0/coba/primitives/feedbacks.py
--rw-rw-rw-   0        0        0     6745 2023-05-26 03:19:33.000000 coba-6.5.0/coba/primitives/rewards.py
--rw-rw-rw-   0        0        0     4425 2023-05-11 00:41:22.000000 coba-6.5.0/coba/primitives/rows.py
--rw-rw-rw-   0        0        0      234 2023-05-11 00:41:22.000000 coba-6.5.0/coba/primitives/semantic.py
--rw-rw-rw-   0        0        0      657 2023-05-16 05:30:40.000000 coba-6.5.0/coba/primitives/types.py
--rw-rw-rw-   0        0        0    11036 2023-05-13 00:19:56.000000 coba-6.5.0/coba/random.py
--rw-rw-rw-   0        0        0     1405 2023-05-11 00:41:22.000000 coba-6.5.0/coba/register.py
--rw-rw-rw-   0        0        0    10657 2023-05-11 00:41:22.000000 coba-6.5.0/coba/registry.py
--rw-rw-rw-   0        0        0     8417 2023-05-11 00:41:22.000000 coba-6.5.0/coba/statistics.py
--rw-rw-rw-   0        0        0     4594 2023-05-11 00:41:22.000000 coba-6.5.0/coba/utilities.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:12:44.000000 coba-6.5.0/coba.egg-info/
--rw-rw-rw-   0        0        0     7933 2023-05-28 19:12:44.000000 coba-6.5.0/coba.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1490 2023-05-28 19:12:44.000000 coba-6.5.0/coba.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 19:12:44.000000 coba-6.5.0/coba.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-28 19:12:44.000000 coba-6.5.0/coba.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       91 2023-05-28 19:12:44.000000 coba-6.5.0/coba.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-28 19:12:44.000000 coba-6.5.0/coba.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 19:12:44.000000 coba-6.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1273 2023-05-28 19:09:21.000000 coba-6.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/
+-rw-rw-rw-   0        0        0       40 2023-05-11 00:41:22.000000 coba-7.0.0/AUTHORS
+-rw-rw-rw-   0        0        0     1593 2023-05-11 00:41:22.000000 coba-7.0.0/LICENSE
+-rw-rw-rw-   0        0        0     7942 2023-07-17 05:11:17.000000 coba-7.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7327 2023-06-16 06:32:50.000000 coba-7.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/
+-rw-rw-rw-   0        0        0     1378 2023-07-17 05:09:07.000000 coba-7.0.0/coba/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/backports/
+-rw-rw-rw-   0        0        0       93 2023-06-18 23:59:19.000000 coba-7.0.0/coba/backports/__init__.py
+-rw-rw-rw-   0        0        0      363 2023-06-18 23:59:52.000000 coba-7.0.0/coba/backports/metadata.py
+-rw-rw-rw-   0        0        0      159 2023-06-14 06:26:06.000000 coba-7.0.0/coba/backports/typing.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/contexts/
+-rw-rw-rw-   0        0        0      703 2023-06-19 00:00:10.000000 coba-7.0.0/coba/contexts/__init__.py
+-rw-rw-rw-   0        0        0     9727 2023-05-11 00:41:22.000000 coba-7.0.0/coba/contexts/cachers.py
+-rw-rw-rw-   0        0        0     9263 2023-06-18 23:38:55.000000 coba-7.0.0/coba/contexts/core.py
+-rw-rw-rw-   0        0        0     9726 2023-05-11 00:41:22.000000 coba-7.0.0/coba/contexts/loggers.py
+-rw-rw-rw-   0        0        0    15634 2023-05-11 00:41:22.000000 coba-7.0.0/coba/encodings.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/environments/
+-rw-rw-rw-   0        0        0     1448 2023-07-04 19:28:10.000000 coba-7.0.0/coba/environments/__init__.py
+-rw-rw-rw-   0        0        0    22778 2023-07-17 04:57:59.000000 coba-7.0.0/coba/environments/core.py
+-rw-rw-rw-   0        0        0    52607 2023-07-13 04:00:27.000000 coba-7.0.0/coba/environments/filters.py
+-rw-rw-rw-   0        0        0    14347 2023-07-02 16:51:02.000000 coba-7.0.0/coba/environments/openml.py
+-rw-rw-rw-   0        0        0     7646 2023-06-30 15:24:01.000000 coba-7.0.0/coba/environments/primitives.py
+-rw-rw-rw-   0        0        0     2966 2023-07-04 17:42:06.000000 coba-7.0.0/coba/environments/serialized.py
+-rw-rw-rw-   0        0        0     9551 2023-06-30 15:23:55.000000 coba-7.0.0/coba/environments/supervised.py
+-rw-rw-rw-   0        0        0    24201 2023-06-25 05:50:30.000000 coba-7.0.0/coba/environments/synthetics.py
+-rw-rw-rw-   0        0        0     6179 2023-05-11 00:41:22.000000 coba-7.0.0/coba/environments/templates.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/evaluators/
+-rw-rw-rw-   0        0        0      217 2023-06-20 04:16:24.000000 coba-7.0.0/coba/evaluators/__init__.py
+-rw-rw-rw-   0        0        0    15064 2023-06-18 22:54:36.000000 coba-7.0.0/coba/evaluators/offline.py
+-rw-rw-rw-   0        0        0    22185 2023-07-13 05:34:25.000000 coba-7.0.0/coba/evaluators/online.py
+-rw-rw-rw-   0        0        0     2095 2023-06-25 05:45:51.000000 coba-7.0.0/coba/evaluators/primitives.py
+-rw-rw-rw-   0        0        0     1126 2023-05-11 00:41:22.000000 coba-7.0.0/coba/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/experiments/
+-rw-rw-rw-   0        0        0      379 2023-06-19 00:00:43.000000 coba-7.0.0/coba/experiments/__init__.py
+-rw-rw-rw-   0        0        0    10512 2023-07-09 16:24:44.000000 coba-7.0.0/coba/experiments/core.py
+-rw-rw-rw-   0        0        0     7686 2023-07-04 17:08:08.000000 coba-7.0.0/coba/experiments/process.py
+-rw-rw-rw-   0        0        0    65268 2023-07-14 04:53:15.000000 coba-7.0.0/coba/experiments/results.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/learners/
+-rw-rw-rw-   0        0        0      761 2023-06-25 04:18:42.000000 coba-7.0.0/coba/learners/__init__.py
+-rw-rw-rw-   0        0        0     7907 2023-05-11 00:41:22.000000 coba-7.0.0/coba/learners/bandit.py
+-rw-rw-rw-   0        0        0     8055 2023-05-24 19:10:26.000000 coba-7.0.0/coba/learners/corral.py
+-rw-rw-rw-   0        0        0     4947 2023-07-17 04:57:59.000000 coba-7.0.0/coba/learners/linucb.py
+-rw-rw-rw-   0        0        0      958 2023-07-03 04:52:50.000000 coba-7.0.0/coba/learners/misguided.py
+-rw-rw-rw-   0        0        0     4376 2023-05-27 01:06:49.000000 coba-7.0.0/coba/learners/primitives.py
+-rw-rw-rw-   0        0        0     8927 2023-07-09 04:29:49.000000 coba-7.0.0/coba/learners/safety.py
+-rw-rw-rw-   0        0        0    31011 2023-06-25 05:22:07.000000 coba-7.0.0/coba/learners/vowpal.py
+-rw-rw-rw-   0        0        0     4139 2023-07-04 16:30:02.000000 coba-7.0.0/coba/multiprocessing.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/pipes/
+-rw-rw-rw-   0        0        0     1456 2023-07-04 23:11:40.000000 coba-7.0.0/coba/pipes/__init__.py
+-rw-rw-rw-   0        0        0     1890 2023-05-15 13:57:18.000000 coba-7.0.0/coba/pipes/core.py
+-rw-rw-rw-   0        0        0    16751 2023-07-03 07:12:05.000000 coba-7.0.0/coba/pipes/filters.py
+-rw-rw-rw-   0        0        0    14968 2023-07-04 17:01:11.000000 coba-7.0.0/coba/pipes/multiprocessing.py
+-rw-rw-rw-   0        0        0     6622 2023-07-04 16:53:56.000000 coba-7.0.0/coba/pipes/primitives.py
+-rw-rw-rw-   0        0        0    13003 2023-05-18 00:30:21.000000 coba-7.0.0/coba/pipes/readers.py
+-rw-rw-rw-   0        0        0    19485 2023-07-05 00:06:18.000000 coba-7.0.0/coba/pipes/rows.py
+-rw-rw-rw-   0        0        0     4474 2023-07-02 17:30:52.000000 coba-7.0.0/coba/pipes/sinks.py
+-rw-rw-rw-   0        0        0     6510 2023-06-04 18:59:11.000000 coba-7.0.0/coba/pipes/sources.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba/primitives/
+-rw-rw-rw-   0        0        0      477 2023-06-19 00:01:57.000000 coba-7.0.0/coba/primitives/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-06-16 03:47:25.000000 coba-7.0.0/coba/primitives/feedbacks.py
+-rw-rw-rw-   0        0        0     4494 2023-06-16 05:48:36.000000 coba-7.0.0/coba/primitives/rewards.py
+-rw-rw-rw-   0        0        0     4421 2023-07-05 00:02:17.000000 coba-7.0.0/coba/primitives/rows.py
+-rw-rw-rw-   0        0        0      219 2023-06-16 03:47:51.000000 coba-7.0.0/coba/primitives/semantic.py
+-rw-rw-rw-   0        0        0      657 2023-05-16 05:30:40.000000 coba-7.0.0/coba/primitives/types.py
+-rw-rw-rw-   0        0        0    11151 2023-07-17 04:57:59.000000 coba-7.0.0/coba/random.py
+-rw-rw-rw-   0        0        0     1479 2023-07-03 01:30:21.000000 coba-7.0.0/coba/register.py
+-rw-rw-rw-   0        0        0    10657 2023-05-11 00:41:22.000000 coba-7.0.0/coba/registry.py
+-rw-rw-rw-   0        0        0     9049 2023-07-13 05:09:41.000000 coba-7.0.0/coba/statistics.py
+-rw-rw-rw-   0        0        0     5212 2023-06-05 02:30:05.000000 coba-7.0.0/coba/utilities.py
+drwxrwxrwx   0        0        0        0 2023-07-17 05:11:17.000000 coba-7.0.0/coba.egg-info/
+-rw-rw-rw-   0        0        0     7942 2023-07-17 05:11:16.000000 coba-7.0.0/coba.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1608 2023-07-17 05:11:16.000000 coba-7.0.0/coba.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 05:11:16.000000 coba-7.0.0/coba.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-17 05:11:16.000000 coba-7.0.0/coba.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      155 2023-07-17 05:11:16.000000 coba-7.0.0/coba.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-17 05:11:16.000000 coba-7.0.0/coba.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1283 2023-06-18 23:54:01.000000 coba-7.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 05:11:17.000000 coba-7.0.0/setup.cfg
```

### Comparing `coba-6.5.0/LICENSE` & `coba-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coba-6.5.0/PKG-INFO` & `coba-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: coba
-Version: 6.5.0
-Summary: A contextual bandit research package.
-Home-page: https://github.com/VowpalWabbit/coba
-Author: Mark Rucker
-Author-email: rucker.mark@gmail.com
-License: BSD 3-Clause License
+Version: 7.0.0
+Summary: A contextual bandit research package
+Author-email: Mark Rucker <rucker.mark@gmail.com>
+License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/vowpalwabbit/coba
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: full
 License-File: LICENSE
 License-File: AUTHORS
 
 [![codecov](https://codecov.io/gh/VowpalWabbit/coba/branch/master/graph/badge.svg?token=885XLZJ2D4)](https://codecov.io/gh/VowpalWabbit/coba)
 [![badge](https://img.shields.io/badge/launch%20example-binder-579ACA.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAB8lBMVEX///9XmsrmZYH1olJXmsr1olJXmsrmZYH1olJXmsr1olJXmsrmZYH1olL1olJXmsr1olJXmsrmZYH1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olJXmsrmZYH1olL1olL0nFf1olJXmsrmZYH1olJXmsq8dZb1olJXmsrmZYH1olJXmspXmspXmsr1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olLeaIVXmsrmZYH1olL1olL1olJXmsrmZYH1olLna31Xmsr1olJXmsr1olJXmsrmZYH1olLqoVr1olJXmsr1olJXmsrmZYH1olL1olKkfaPobXvviGabgadXmsqThKuofKHmZ4Dobnr1olJXmsr1olJXmspXmsr1olJXmsrfZ4TuhWn1olL1olJXmsqBi7X1olJXmspZmslbmMhbmsdemsVfl8ZgmsNim8Jpk8F0m7R4m7F5nLB6jbh7jbiDirOEibOGnKaMhq+PnaCVg6qWg6qegKaff6WhnpKofKGtnomxeZy3noG6dZi+n3vCcpPDcpPGn3bLb4/Mb47UbIrVa4rYoGjdaIbeaIXhoWHmZYHobXvpcHjqdHXreHLroVrsfG/uhGnuh2bwj2Hxk17yl1vzmljzm1j0nlX1olL3AJXWAAAAbXRSTlMAEBAQHx8gICAuLjAwMDw9PUBAQEpQUFBXV1hgYGBkcHBwcXl8gICAgoiIkJCQlJicnJ2goKCmqK+wsLC4usDAwMjP0NDQ1NbW3Nzg4ODi5+3v8PDw8/T09PX29vb39/f5+fr7+/z8/Pz9/v7+zczCxgAABC5JREFUeAHN1ul3k0UUBvCb1CTVpmpaitAGSLSpSuKCLWpbTKNJFGlcSMAFF63iUmRccNG6gLbuxkXU66JAUef/9LSpmXnyLr3T5AO/rzl5zj137p136BISy44fKJXuGN/d19PUfYeO67Znqtf2KH33Id1psXoFdW30sPZ1sMvs2D060AHqws4FHeJojLZqnw53cmfvg+XR8mC0OEjuxrXEkX5ydeVJLVIlV0e10PXk5k7dYeHu7Cj1j+49uKg7uLU61tGLw1lq27ugQYlclHC4bgv7VQ+TAyj5Zc/UjsPvs1sd5cWryWObtvWT2EPa4rtnWW3JkpjggEpbOsPr7F7EyNewtpBIslA7p43HCsnwooXTEc3UmPmCNn5lrqTJxy6nRmcavGZVt/3Da2pD5NHvsOHJCrdc1G2r3DITpU7yic7w/7Rxnjc0kt5GC4djiv2Sz3Fb2iEZg41/ddsFDoyuYrIkmFehz0HR2thPgQqMyQYb2OtB0WxsZ3BeG3+wpRb1vzl2UYBog8FfGhttFKjtAclnZYrRo9ryG9uG/FZQU4AEg8ZE9LjGMzTmqKXPLnlWVnIlQQTvxJf8ip7VgjZjyVPrjw1te5otM7RmP7xm+sK2Gv9I8Gi++BRbEkR9EBw8zRUcKxwp73xkaLiqQb+kGduJTNHG72zcW9LoJgqQxpP3/Tj//c3yB0tqzaml05/+orHLksVO+95kX7/7qgJvnjlrfr2Ggsyx0eoy9uPzN5SPd86aXggOsEKW2Prz7du3VID3/tzs/sSRs2w7ovVHKtjrX2pd7ZMlTxAYfBAL9jiDwfLkq55Tm7ifhMlTGPyCAs7RFRhn47JnlcB9RM5T97ASuZXIcVNuUDIndpDbdsfrqsOppeXl5Y+XVKdjFCTh+zGaVuj0d9zy05PPK3QzBamxdwtTCrzyg/2Rvf2EstUjordGwa/kx9mSJLr8mLLtCW8HHGJc2R5hS219IiF6PnTusOqcMl57gm0Z8kanKMAQg0qSyuZfn7zItsbGyO9QlnxY0eCuD1XL2ys/MsrQhltE7Ug0uFOzufJFE2PxBo/YAx8XPPdDwWN0MrDRYIZF0mSMKCNHgaIVFoBbNoLJ7tEQDKxGF0kcLQimojCZopv0OkNOyWCCg9XMVAi7ARJzQdM2QUh0gmBozjc3Skg6dSBRqDGYSUOu66Zg+I2fNZs/M3/f/Grl/XnyF1Gw3VKCez0PN5IUfFLqvgUN4C0qNqYs5YhPL+aVZYDE4IpUk57oSFnJm4FyCqqOE0jhY2SMyLFoo56zyo6becOS5UVDdj7Vih0zp+tcMhwRpBeLyqtIjlJKAIZSbI8SGSF3k0pA3mR5tHuwPFoa7N7reoq2bqCsAk1HqCu5uvI1n6JuRXI+S1Mco54YmYTwcn6Aeic+kssXi8XpXC4V3t7/ADuTNKaQJdScAAAAAElFTkSuQmCC)](https://mybinder.org/v2/gh/VowpalWabbit/Coba/HEAD?filepath=examples/notebooks)
 
 # Coba
@@ -61,15 +61,15 @@
 
  Learners are algorithms which are able to improve their action selection through interactions with environments.
 
  A number of algorithms are provided natively with Coba for quick comparsions. These include:
 
  * All contextual bandit learners in VowpalWabbit
  * UCB1-Tuned Bandit Learner by Auer et al. 2002
- * LinUCB by Chu et al. 2011
+ * LinUCB by Li and Chu et al. 2010
  * Corral by Agarwal et al. 2017
 
  ## Environments
 
  Environments are the core unit of evaluation in Coba. They are nothing more than a sequence of interactions with contexts, actions and rewards. A number of tools have been built into Coba to make simulation creation easier. All these tools are defined in the `coba.environments` module. We describe a few of these tools here.
 
  ### Creating Environments From Classification Data Sets
@@ -83,15 +83,15 @@
 
  ### Creating Environments From Generative Functions
 
  Sometimes we have well defined models that an agent has to make decisions within but no data. To support evaluation in these domains one can use `LambdaSimulation` to define generative functions to create an Environment.
 
  ### Creating Environments From Scratch
 
- If more customization is needed beyond what is offered above then you can easily create your own simulation by implementing Coba's simple `SimulatedEnvironment` interface.
+ If more customization is needed beyond what is offered above then you can easily create your own simulation by implementing Coba's `Environment` interface.
 
  ## Experiments
 
  Experiments are combinations of Learners and Environments. The Experiment class orchestrates the complex tasks of evaluating learners on environments in a resource efficient, repeatable, and robust manner. Experiments can be run on any number of processes (we often run on 96 core machines) and writes all results to file as it runs so that it can be restarted if it ever stops.
 
  ## Results
```

### Comparing `coba-6.5.0/README.md` & `coba-7.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
  Learners are algorithms which are able to improve their action selection through interactions with environments.
 
  A number of algorithms are provided natively with Coba for quick comparsions. These include:
 
  * All contextual bandit learners in VowpalWabbit
  * UCB1-Tuned Bandit Learner by Auer et al. 2002
- * LinUCB by Chu et al. 2011
+ * LinUCB by Li and Chu et al. 2010
  * Corral by Agarwal et al. 2017
 
  ## Environments
 
  Environments are the core unit of evaluation in Coba. They are nothing more than a sequence of interactions with contexts, actions and rewards. A number of tools have been built into Coba to make simulation creation easier. All these tools are defined in the `coba.environments` module. We describe a few of these tools here.
 
  ### Creating Environments From Classification Data Sets
@@ -65,15 +65,15 @@
 
  ### Creating Environments From Generative Functions
 
  Sometimes we have well defined models that an agent has to make decisions within but no data. To support evaluation in these domains one can use `LambdaSimulation` to define generative functions to create an Environment.
 
  ### Creating Environments From Scratch
 
- If more customization is needed beyond what is offered above then you can easily create your own simulation by implementing Coba's simple `SimulatedEnvironment` interface.
+ If more customization is needed beyond what is offered above then you can easily create your own simulation by implementing Coba's `Environment` interface.
 
  ## Experiments
 
  Experiments are combinations of Learners and Environments. The Experiment class orchestrates the complex tasks of evaluating learners on environments in a resource efficient, repeatable, and robust manner. Experiments can be run on any number of processes (we often run on 96 core machines) and writes all results to file as it runs so that it can be restarted if it ever stops.
 
  ## Results
```

### Comparing `coba-6.5.0/coba/contexts/cachers.py` & `coba-7.0.0/coba/contexts/cachers.py`

 * *Files identical despite different names*

### Comparing `coba-6.5.0/coba/contexts/core.py` & `coba-7.0.0/coba/contexts/core.py`

 * *Files identical despite different names*

### Comparing `coba-6.5.0/coba/contexts/loggers.py` & `coba-7.0.0/coba/contexts/loggers.py`

 * *Files identical despite different names*

### Comparing `coba-6.5.0/coba/encodings.py` & `coba-7.0.0/coba/encodings.py`

 * *Files identical despite different names*

### Comparing `coba-6.5.0/coba/environments/core.py` & `coba-7.0.0/coba/environments/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 from coba.environments.templates  import EnvironmentsTemplateV1, EnvironmentsTemplateV2
 from coba.environments.openml     import OpenmlSimulation
 from coba.environments.synthetics import LinearSyntheticSimulation, NeighborsSyntheticSimulation
 from coba.environments.synthetics import KernelSyntheticSimulation, MLPSyntheticSimulation, LambdaSimulation
 from coba.environments.supervised import SupervisedSimulation
 
 from coba.environments.filters   import EnvironmentFilter, Repr, Batch, Chunk, Logged, Finalize, BatchSafe
-from coba.environments.filters   import Binary, Shuffle, Take, Sparse, Reservoir, Cycle, Scale, Unbatch, Slice
-from coba.environments.filters   import Impute, Where, Noise, Riffle, Sort, Flatten, Cache, Params, Grounded
+from coba.environments.filters   import Binary, Shuffle, Take, Sparsify, Densify, Reservoir, Cycle, Scale, Unbatch
+from coba.environments.filters   import Slice, Impute, Where, Noise, Riffle, Sort, Flatten, Cache, Params, Grounded
 from coba.environments.filters   import MappingToInteraction, OpeRewards
 
 from coba.environments.serialized import EnvironmentFromObjects, EnvironmentsToObjects, ZipMemberToObjects, ObjectsToZipMember
 
 class Environments(collections.abc.Sequence, Sequence[Environment]):
     """A friendly wrapper around commonly used environment functionality."""
 
@@ -264,16 +264,21 @@
                 self._environments.append(env)
 
     def binary(self) -> 'Environments':
         """Binarize all rewards to either 1 (max rewards) or 0 (all others)."""
         return self.filter(Binary())
 
     def sparse(self, context:bool = True, action:bool = False) -> 'Environments':
-        """Convert an environment from a dense representation to sparse. This has little utility beyond debugging."""
-        return self.filter(Sparse(context,action))
+        """Convert all environments to a sparse representation."""
+        return self.filter(Sparsify(context,action))
+
+    def dense(self, n_feats:int, method:Literal['lookup','hashing'], context:bool = True, action:bool = False) -> 'Environments':
+        """Convert all environments to a dense representation."""
+        make_dense = lambda: Densify(n_feats=n_feats, method=method, context=context, action=action)
+        return Environments([Pipes.join(env, make_dense()) for env in self])
 
     @overload
     def shuffle(self, seed: int = 1) -> 'Environments':
         ...
 
     @overload
     def shuffle(self, seeds: Iterable[int]) -> 'Environments':
@@ -310,32 +315,33 @@
 
     def riffle(self, spacing: int, seed: int = 1) -> 'Environments':
         """Riffle shuffle by evenly spacing interactions at the end of an environment into the beginning."""
         return self.filter(Riffle(spacing, seed))
 
     def cycle(self, after: int) -> 'Environments':
         """Cycle all rewards associated with actions by one place."""
-        return self.filter(Cycle(after))
+        if isinstance(after,(int,float)): after = [after]
+        return self.filter([Cycle(a) for a in after])
 
     def params(self, params: Mapping[str,Any]) -> 'Environments':
         """Add params to the environments."""
         return self.filter(Params(params))
 
     def take(self, n_interactions: int) -> 'Environments':
         """Take a fixed number of interactions from the Environments."""
         return self.filter(Take(n_interactions))
-    
+
     def slice(self, start: Optional[int], stop: Optional[int]=None, step:int = 1) -> 'Environments':
         """Take a slice of interactions from an Environment."""
         return self.filter(Slice(start,stop,step))
 
     def reservoir(self, n_interactions: int, seeds: Union[int,Sequence[int]]=1) -> 'Environments':
         """Take a random fixed number of interactions from the Environments."""
         if isinstance(seeds,int): seeds = [seeds]
-        return self.filter([Reservoir(n_interactions,seed) for seed in seeds])
+        return self.filter([Reservoir(n_interactions,seed=seed) for seed in seeds])
 
     def scale(self,
         shift: Union[float,Literal["min","mean","med"]] = "min",
         scale: Union[float,Literal["minmax","std","iqr","maxabs"]] = "minmax",
         targets: Union[Literal["context","ope_rewards","argmax"], Sequence[Literal["context","ope_rewards","argmax"]]] = "context",
         using: Optional[int] = None) -> 'Environments':
         """Apply an affine shift and scaling factor to precondition environments."""
@@ -359,41 +365,41 @@
 
     def noise(self,
         context: Callable[[float,CobaRandom], float] = None,
         action : Callable[[float,CobaRandom], float] = None,
         reward : Callable[[float,CobaRandom], float] = None,
         seed   : int = 1) -> 'Environments':
         """Add noise to an environment's context, actions and rewards."""
-        return Environments(*self).filter(Noise(context,action,reward,seed))
+        return self.filter(Noise(context,action,reward,seed))
 
     def flat(self) -> 'Environments':
         """Flatten environment's context and actions."""
         return self.filter(Flatten())
 
     def materialize(self) -> 'Environments':
         """Materialize the environments in memory. Ideal for stateful environments such as Jupyter Notebook."""
-        #we use pipes.cache directly because the environment cache will copy 
+        #we use pipes.cache directly because the environment cache will copy
         #which we don't need when we materialize an environment in memory
         envs = Environments([Pipes.join(env, Finalize(apply_repr=False), pipes.Cache(25,True)) for env in self])
-        
+
         for env in envs: list(env.read()) #force read to pre-load cache
-            
+
         for env in envs:
             for i in range(len(env)-1):
                 pipe = env[i]
                 if isinstance(pipe, pipes.Cache) and not pipe._protected:
                     pipe._cache = None
 
         return envs
 
     def grounded(self, n_users: int, n_normal:int, n_words:int, n_good:int, seed:int=1) -> 'Environments':
         """Convert from simulated environments to interaction grounded environments."""
         return self.filter(Grounded(n_users, n_normal, n_words, n_good, seed))
 
-    def repr(self, 
+    def repr(self,
         cat_context:Literal["onehot","onehot_tuple","string"] = "onehot",
         cat_actions:Literal["onehot","onehot_tuple","string"] = "onehot") -> 'Environments':
         """Determine how certain types of data is represented."""
         return self.filter(Repr(cat_context,cat_actions))
 
     def batch(self, batch_size:int) -> 'Environments':
         """Batch interactions for learning and evaluation."""
@@ -409,22 +415,22 @@
         if not isinstance(learners, collections.abc.Sequence): learners = [learners]
         return self.filter(BatchSafe(Finalize())).filter([Logged(learner, seed) for learner in learners ])
 
     def unbatch(self):
         """Unbatch interactions in the environments."""
         return self.filter(Unbatch())
 
-    def ope_rewards(self, rewards_type:Literal['IPS','DM','DR','NO'] = None):
+    def ope_rewards(self, rewards_type:Literal['IPS','DM','DR'] = None):
         """Reward estimates for off-policy evaluation."""
-        return self.filter(OpeRewards(rewards_type))
+        if isinstance(rewards_type,str): rewards_type = [rewards_type]
+        return self.filter([OpeRewards(r) for r in rewards_type])
 
     def save(self, path: str, processes:int=1, overwrite:bool=False) -> 'Environments':
-
+        """Save the environments to disk."""
         self_envs = list(self)
-
         if Path(path).exists():
             try:
                 path_envs   = Environments.from_save(path)
                 path_params = [e.params for e in path_envs]
                 self_params = [e.params for e in self_envs]
 
                 try:
```

### Comparing `coba-6.5.0/coba/environments/filters.py` & `coba-7.0.0/coba/environments/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,33 +2,34 @@
 import pickle
 import warnings
 import copy
 
 from math import isnan
 from statistics import median, stdev, mode
 from numbers import Number
+from zlib import crc32
 from operator import eq, getitem, methodcaller, itemgetter
-from collections import defaultdict, deque
+from collections import defaultdict
 from functools import lru_cache
 from itertools import islice, chain, tee, compress, repeat
 from typing import Optional, Sequence, Union, Iterable, Any, Tuple, Callable, Mapping
 from coba.backports import Literal
 
 from coba            import pipes, primitives
 from coba.random     import CobaRandom
 from coba.exceptions import CobaException
 from coba.statistics import iqr
 from coba.utilities  import peek_first, PackageChecker
-from coba.primitives import ScaleReward, BinaryReward, SequenceReward, BatchReward
+from coba.primitives import BinaryReward, SequenceReward, BatchReward, argmax
 from coba.primitives import IPSReward, SequenceFeedback, MappingReward, MulticlassReward
 from coba.primitives import Feedback, BatchFeedback
 from coba.learners   import Learner, SafeLearner
-from coba.pipes      import Filter
+from coba.pipes      import Filter, SparseDense
 
-from coba.environments.primitives import EnvironmentFilter, Interaction
+from coba.environments.primitives import Interaction, EnvironmentFilter, SimpleEnvironment
 
 class Identity(pipes.Identity, EnvironmentFilter):
     """Return whatever interactions are given to the filter."""
     pass
 
 class Take(pipes.Take, EnvironmentFilter):
     """Take a fixed number of interactions from an Environment."""
@@ -83,15 +84,15 @@
 
 class Scale(EnvironmentFilter):
     """Shift and scale features to precondition them before learning."""
 
     def __init__(self,
         shift: Union[Number,Literal["min","mean","med"]] = 0,
         scale: Union[Number,Literal["minmax","std","iqr","maxabs"]] = "minmax",
-        target: Literal["context","rewards","argmax"] = "context",
+        target: Literal["context"] = "context",
         using: Optional[int] = None):
         """Instantiate a Scale filter.
 
         Args:
             shift: The statistic to use to shift each context feature.
             scale: The statistic to use to scale each context feature.
             target: The target data we wish to scale in the environment.
@@ -128,115 +129,80 @@
 
         first_context = first['context']
         first_actions = first.get('actions')
 
         if isinstance(first_context, primitives.Sparse) and self._target=="context" and self._shift != 0:
             raise CobaException("Shift is required to be 0 for sparse environments. Otherwise the environment will become dense.")
 
-        is_discrete       = first_actions and len(first_actions) > 0
         is_dense_context  = isinstance(first_context, primitives.Dense)
         is_sparse_context = isinstance(first_context, primitives.Sparse)
         is_value_context  = not (is_dense_context or is_sparse_context)
 
         #get the values we wish to scale
-        start = time.time()
-        if self._target == "context" and is_dense_context:
-            potential_cols = [i for i,v in enumerate(first['context']) if isinstance(v,(int,float))]
-            if len(potential_cols) == 0:
-                unscaled = []
-            elif len(potential_cols) == 1:
-                unscaled = [ tuple(map(itemgetter(*potential_cols),map(getitem,fitting_interactions,repeat("context")))) ]
-            else:
-                unscaled = list(zip(*map(itemgetter(*potential_cols),map(getitem,fitting_interactions,repeat("context")))))
-
-        elif self._target == "context" and is_sparse_context:
-            unscalable_cols = {k for k,v in first['context'].items() if not isinstance(v,(int,float))}
-            unscaled = defaultdict(list)
-            for interaction in fitting_interactions:
-                context = interaction['context']
-                for k in context.keys()-unscalable_cols:
-                    unscaled[k].append(context[k])
-
-        elif self._target == "context" and is_value_context:
-            unscaled = [interaction['context'] for interaction in fitting_interactions]
-
-        elif self._target == "rewards" and is_discrete:
-            rwd_vals = lambda i: list(map(i['rewards'].eval,i['actions']))
-            unscaled = sum(list(map(rwd_vals,fitting_interactions)),[])
-
-        elif self._target == "rewards" and not is_discrete:
-            unscaled = []
-
-        elif self._target == "argmax":
-            unscaled = [interaction['rewards'].argmax() for interaction in fitting_interactions]
-        self._times[1] += time.time()-start
+        if self._target == "context" :
+            if is_dense_context:
+                potential_cols = [i for i,v in enumerate(first['context']) if isinstance(v,(int,float))]
+                if len(potential_cols) == 0:
+                    unscaled = []
+                elif len(potential_cols) == 1:
+                    unscaled = [ tuple(map(itemgetter(*potential_cols),map(getitem,fitting_interactions,repeat("context")))) ]
+                else:
+                    unscaled = list(zip(*map(itemgetter(*potential_cols),map(getitem,fitting_interactions,repeat("context")))))
+            elif is_sparse_context:
+                unscalable_cols = {k for k,v in first['context'].items() if not isinstance(v,(int,float))}
+                unscaled = defaultdict(list)
+                for interaction in fitting_interactions:
+                    context = interaction['context']
+                    for k in context.keys()-unscalable_cols:
+                        unscaled[k].append(context[k])
+            elif is_value_context:
+                unscaled = [interaction['context'] for interaction in fitting_interactions]
 
-        start = time.time()
         #determine the scale and shift values
-        if self._target == "context" and is_dense_context:
-            shifts_scales = []
-            for i,col in zip(potential_cols,unscaled):
-                shift_scale = self._get_shift_and_scale(col)
-                if shift_scale is not None:
-                    shifts_scales.append((i,)+shift_scale)
-
-        elif self._target == "context" and is_sparse_context:
-            shifts_scales = {}
-            for k,col in unscaled.items():
-                vals = col + [0]*(len(fitting_interactions)-len(col))
-                shift_scale = self._get_shift_and_scale(vals)
-                if shift_scale is not None:
-                    shifts_scales[k] = shift_scale
+        if self._target == "context":
+            if is_dense_context:
+                shifts_scales = []
+                for i,col in zip(potential_cols,unscaled):
+                    shift_scale = self._get_shift_and_scale(col)
+                    if shift_scale is not None:
+                        shifts_scales.append((i,)+shift_scale)
+            elif is_sparse_context:
+                shifts_scales = {}
+                for k,col in unscaled.items():
+                    vals = col + [0]*(len(fitting_interactions)-len(col))
+                    shift_scale = self._get_shift_and_scale(vals)
+                    if shift_scale is not None:
+                        shifts_scales[k] = shift_scale
+            elif is_value_context:
+                shifts_scales = self._get_shift_and_scale(unscaled)
 
-        elif self._target in ['context','rewards','argmax']:
-            shifts_scales = self._get_shift_and_scale(unscaled)
-        self._times[2] += time.time()-start
-
-        start = time.time()
+        #now scale
         if not shifts_scales:
             yield from chain(fitting_interactions, remaining_interactions)
-
-        #now scale return
-        elif self._target == "context" and is_dense_context:
-            for interaction in chain(fitting_interactions, remaining_interactions):
-                context = interaction['context']
-                for i,shift,scale in shifts_scales:
-                     context[i] = (context[i]+shift)*scale
-                yield interaction
-
-        elif self._target == "context" and is_sparse_context:
-            for interaction in chain(fitting_interactions, remaining_interactions):
-                new = interaction # Mutable copies
-                context = new['context']
-                for k in shifts_scales.keys() & context.keys():
-                    (shift,scale) = shifts_scales[k]
-                    context[k] = (context[k]+shift)*scale
-                yield new
-
-        elif self._target == "context" and is_value_context:
-            (shift,scale) = shifts_scales
-            for interaction in chain(fitting_interactions, remaining_interactions):
-                new = interaction.copy()
-                new['context'] = (new['context']+shift)*scale
-                yield new
-
-        elif self._target == "rewards":
-            (shift,scale) = shifts_scales
-            for interaction in chain(fitting_interactions, remaining_interactions):
-                new = interaction.copy()
-                new['rewards'] = ScaleReward(new['rewards'], shift, scale, 'value')
-                yield new
-
-        elif self._target == "argmax":
-            (shift,scale) = shifts_scales
-            for interaction in chain(fitting_interactions, remaining_interactions):
-                new = interaction.copy()
-                new['rewards'] = ScaleReward(new['rewards'], shift, scale, 'argmax')
-                yield new
-        self._times[3] += time.time()-start
+        elif self._target == "context":
+            if is_dense_context:
+                for interaction in chain(fitting_interactions, remaining_interactions):
+                    context = interaction['context']
+                    for i,shift,scale in shifts_scales:
+                        context[i] = (context[i]+shift)*scale
+                    yield interaction
+            elif is_sparse_context:
+                for interaction in chain(fitting_interactions, remaining_interactions):
+                    new = interaction # Mutable copies
+                    context = new['context']
+                    for k in shifts_scales.keys() & context.keys():
+                        (shift,scale) = shifts_scales[k]
+                        context[k] = (context[k]+shift)*scale
+                    yield new
+            elif is_value_context:
+                (shift,scale) = shifts_scales
+                for interaction in chain(fitting_interactions, remaining_interactions):
+                    new = interaction.copy()
+                    new['context'] = (new['context']+shift)*scale
+                    yield new
 
     def _get_shift_and_scale(self,values) -> Tuple[float,float]:
         try:
             shift = self._shift_value(values)
             scale = self._scale_value(values,shift)
 
             if isnan(shift):
@@ -395,17 +361,17 @@
         for interaction in chain(using_interactions,other_interactions):
 
             context = interaction['context']
 
             if is_dense:
                 is_missing = [0]*len(impute_binary)
                 for k,v in enumerate(context):
-                    if v is None and k in imputations: 
+                    if v is None and k in imputations:
                         context[k] = imputations[k]
-                        if k in impute_binary: 
+                        if k in impute_binary:
                             is_missing[impute_binary[k]] = 1
                 context += is_missing
 
             elif is_sparse:
 
                 is_missing = binary_template.copy()
                 for k,v in context.items():
@@ -436,34 +402,31 @@
             if self._stat == "median":
                 return median(values)
             if self._stat == "mode":
                 return mode(values)
         except:
             return None
 
-class Sparse(EnvironmentFilter):
-    """Sparsify an environment's feature representation.
-
-    This has little utility beyond debugging.
-    """
+class Sparsify(EnvironmentFilter):
+    """Sparsify an environment's feature representation."""
 
     def __init__(self, context:bool = True, action:bool = False):
-        """Instantiate a Sparse filter.
+        """Instantiate a Sparsify filter.
 
         Args:
             context: If True then contexts should be made sparse otherwise leave them alone.
             action: If True then actions should be made sparse otherwise leave them alone.
         """
 
         self._context = context
         self._action  = action
 
     @property
     def params(self) -> Mapping[str, Any]:
-        return { "sparse_C": self._context, "sparse_A": self._action }
+        return { "sparse_c": self._context, "sparse_a": self._action }
 
     def filter(self, interactions: Iterable[Interaction]) -> Iterable[Interaction]:
 
         first,interactions = peek_first(interactions)
 
         context_has_headers = 'context' in first and hasattr(first['context']   ,'headers')
         actions_has_headers = 'actions' in first and hasattr(first['actions'][0],'headers')
@@ -476,28 +439,137 @@
             if self._context:
                 new['context'] = self._make_sparse(new['context'], context_has_headers, 'context')
 
             if self._action and 'actions' in new:
                 new['actions'] = list(map(self._make_sparse,new['actions'],repeat(actions_has_headers),repeat('action')))
 
             if self._action and 'action' in new:
-                new['action'] = self._make_sparse(new['action'],action_has_headers, 'action')
+                new['action'] = self._make_sparse(new['action'],action_has_headers,'action')
 
             yield new
 
     def _make_sparse(self, value, has_headers:bool, default_header:str) -> Optional[dict]:
         if value is None:
             return value
+
         if isinstance(value,primitives.Dense):
-            value_list = list(value)
-            return {k:value_list[i] for k,i in value.headers.items() if i < len(value_list) and value_list[i] != 0} if has_headers else {k:v for k,v in enumerate(value) if v != 0 }
+            if has_headers:
+                value_list = list(value)
+                return {k:value_list[i] for k,i in value.headers.items() if i < len(value_list) and value_list[i] != 0}
+            else:
+                return {str(k):v for k,v in enumerate(value) if v != 0 }
+
         if isinstance(value,primitives.Sparse):
             return value
+
         return {default_header:value}
 
+class Densify(EnvironmentFilter):
+    """Densify an environment's feature representation."""
+
+    def __init__(self,
+        n_feats: int = 400,
+        method : Literal['lookup','hashing'] = 'lookup',
+        context: bool = True,
+        action : bool = False):
+        """Instantiate a Densify filter.
+
+        Args:
+            n_feats: The number of features to use when densifying a sparse entry.
+            method: The method used to convert sparse representation to dense representation.
+            The "lookup" method produces a more efficient feature representation but its memory
+            usage expand to the cardinality of the sparse features. The "hashing" method utilizes
+            a less efficient feature representation but does not use any memory beyond the features.
+            When using the 'hashing' method `n_feats` should be set to a large number such as 2**18.
+            context: If True then contexts should be made sparse otherwise leave them alone.
+            action: If True then actions should be made sparse otherwise leave them alone.
+        """
+
+        self._n_feats = n_feats
+        self._context = context
+        self._action  = action
+        self._method  = method
+
+        def generator():
+            rng = CobaRandom(seed=1)
+            while True:
+                for i in rng.shuffle(range(n_feats)):
+                    yield i
+
+        def factory(g=generator()):
+            return next(g)
+
+        self._lookup  = defaultdict(factory)
+
+    @property
+    def params(self) -> Mapping[str, Any]:
+        return { "dense_m": self._method, "dense_n": self._n_feats, "dense_c": self._context, "dense_a": self._action }
+
+    def filter(self, interactions: Iterable[Interaction]) -> Iterable[Interaction]:
+
+        for interaction in interactions:
+
+            new = interaction.copy()
+
+            if self._context:
+                new['context'] = self._make_dense(new['context'])
+
+            if self._action and 'actions' in new:
+                new['actions'] = list(map(self._make_dense,new['actions']))
+
+            if self._action and 'action' in new:
+                new['action'] = self._make_dense(new['action'])
+
+            yield new
+
+    def _make_dense(self, value) -> Optional[dict]:
+
+        #For this conversion we use the hashing trick. Based on many tests we go with crc32:
+        #   > It is fast
+        #   > It has few collisions
+        #   > It is deterministic between runs
+
+        # Hashing Algorithms We Tested:
+        #   from hashlib import md5, sha1, sha256, sha3_128, sha3_256, shake_128, shake_256, blake2b
+        #   from zlib import adler32, crc32
+        #   from mmh3 import hash as mmh3_hash #(aka, MurmurHash3, requires pip install mmh3)
+        #   from builtins import hash
+
+        # Performance Findings:
+            # hashlib algorithms took between 0.5 to 0.75 seconds to produce 1 million hashes
+            # zlib and mmh3 algorithms took about .16 seconds to produce 1 million hashes
+            # builtin hash algorithm took about .09 seconds to produce 1 million hashes
+
+        # Collision Findings:
+            # we used the code below to count collisions for 1,000,000 randomly generated strings:
+                #random_strings = lambda n: (''.join(map(str,[r*1,r*2,r*3,r*4,r*5])) for r in cb.random.randoms(n))
+                #hashed_values  = [<hash-algo>(s.encode('ascii')) for s in random_strings(1_000_000)]
+                #Counter(Counter(hashed_values).values())
+
+            # hashlib and the builtin hash had 0 collisions
+            # mmh3 and crc32 had ~130 collisions (i.e., 0.013%)
+            # adler32 had ~250k collisions (i.e., 24.00%)
+
+        #Final decisions:
+            # crc32:
+            #   > It is considerably faster than the hashlib algorithms
+            #   > It has equal performance and collisions to MurmurHash3
+            #   > It is deterministic across runs
+
+        if not isinstance(value,primitives.Sparse):
+            return value
+
+        else:
+            if self._method == 'lookup':
+                values = { self._lookup[k]:v for k,v in value.items() }
+            else:
+                values = { crc32(k.encode('ascii')) % self._n_feats: v for k,v in value.items() }
+
+            return SparseDense(values, self._n_feats)
+
 class Cycle(EnvironmentFilter):
     """Cycle all rewards associated with actions by one place.
 
     This filter is useful for testing an algorithms response to a non-stationary shock.
     """
 
     def __init__(self, after:int = 0):
@@ -510,46 +582,45 @@
 
     @property
     def params(self) -> Mapping[str, Any]:
         return { "cycle_after": self._after }
 
     def filter(self, interactions: Iterable[Interaction]) -> Iterable[Interaction]:
 
-        underlying_iterable     = iter(interactions)
-        sans_cycle_interactions = islice(underlying_iterable, self._after)
-        with_cycle_interactions = underlying_iterable
+        first, interactions = peek_first(interactions)
 
-        yield from sans_cycle_interactions
+        has_actions = first and 'actions' in first
+        has_rewards = first and 'rewards' in first
 
-        first, with_cycle_interactions = peek_first(with_cycle_interactions)
+        one_hot = lambda n,N: tuple([0]*n+[1]+[0]*(N-n-1))
+        rotate  = lambda l: l[-1%n_actions:] + l[:-1%n_actions]
 
-        if with_cycle_interactions:
+        n_actions      = len(first['actions']) if has_actions else 0
+        is_discrete    = 0 < n_actions and n_actions < float('inf')
+        onehot_actions = set(map(one_hot,range(n_actions),repeat(n_actions)))
+        is_onehot      = has_actions and set(first['actions']) == onehot_actions
+        is_categorical = has_actions and all(map(isinstance,first['actions'],repeat(str)))
 
-            action_set = set(first['actions'])
-            n_actions  = len(action_set)
+        is_cyclable = has_actions and has_rewards and is_discrete and (is_onehot or is_categorical)
 
-            onehot_actions  = {tuple([0]*n+[1]+[0]*(n_actions-n-1)) for n in range(n_actions)}
-            is_discrete     = 0 < n_actions and n_actions < float('inf')
-            is_onehots      = action_set == onehot_actions
-            is_categoricals = all([isinstance(a,str) for a in action_set])
+        if not is_cyclable:
+            warnings.warn("Cycle only works for discrete environments without action features. It will be ignored in this case.")
+            yield from interactions
 
-            is_cyclable = is_discrete and (is_onehots or is_categoricals)
+        else:
+            for i,interaction in enumerate(interactions):
 
-            if not is_cyclable:
-                warnings.warn("Cycle only works for discrete environments without action features. It will be ignored in this case.")
-                yield from with_cycle_interactions
-            else:
-                for interaction in with_cycle_interactions:
-                    rewards = deque(map(interaction['rewards'].eval,interaction['actions']))
-                    rewards.rotate(1)
+                new = interaction.copy()
 
-                    new = interaction.copy()
-                    new['rewards'] = SequenceReward(interaction['actions'],list(rewards))
+                if i >= self._after:
+                    actions = interaction['actions']
+                    rewards = interaction['rewards']
+                    new['rewards'] = SequenceReward(actions,rotate(list(map(rewards.eval,actions))))
 
-                    yield new
+                yield new
 
 class Flatten(EnvironmentFilter):
     """Flatten the context and action features for interactions."""
 
     def __init__(self):
         self._flattener = pipes.Flatten()
 
@@ -575,18 +646,26 @@
     """Binarize all rewards to either 1 (max rewards) or 0 (all others)."""
 
     @property
     def params(self) -> Mapping[str, Any]:
         return { "binary": True }
 
     def filter(self, interactions: Iterable[Interaction]) -> Iterable[Interaction]:
-        for interaction in interactions:
-            new = interaction.copy()
-            new['rewards'] = BinaryReward(interaction['rewards'].argmax())
-            yield new
+
+        first, interactions = peek_first(interactions)
+        is_discrete = 'actions' in first and 0 < len(first['actions']) and len(first['actions']) < float('inf')
+
+        if not is_discrete:
+            warnings.warn("Only discrete action rewards can be made binary. ")
+            yield from interactions
+        else:
+            for interaction in interactions:
+                new = interaction.copy()
+                new['rewards'] = BinaryReward(argmax(interaction['actions'], interaction['rewards']))
+                yield new
 
 class Sort(EnvironmentFilter):
     """Sort a sequence of Interactions in an Environment."""
 
     def __init__(self, *keys: Union[str,int,Sequence[Union[str,int]]]) -> None:
         """Instantiate a Sort filter.
 
@@ -855,25 +934,25 @@
 
         goods = [(g,) for g in self.goodwords]
         bads  = [(b,) for b in self.badwords ]
 
         for seed, interaction in enumerate(interactions, self._seed):
 
             userid,normal = rng.choice(userid_isnormal)
-            argmax        = interaction['rewards'].argmax()
+            maxarg        = argmax(interaction['actions'],interaction['rewards'])
 
             new = interaction.copy()
 
             if not is_binary_rwd:
-                new['rewards'] = BinaryReward(argmax)
+                new['rewards'] = BinaryReward(maxarg)
 
             if normal:
-                new['feedbacks'] = Grounded.GroundedFeedback(goods,bads,argmax,seed)
+                new['feedbacks'] = Grounded.GroundedFeedback(goods,bads,maxarg,seed)
             else:
-                new['feedbacks'] = Grounded.GroundedFeedback(bads,goods,argmax,seed)
+                new['feedbacks'] = Grounded.GroundedFeedback(bads,goods,maxarg,seed)
 
             if is_sparse:
                 new['context'] = dict(userid=userid,**new['context'])
             elif is_dense:
                 new['context'] = (userid,)+tuple(new['context'])
             else:
                 new['context'] = (userid, new['context'])
@@ -885,15 +964,15 @@
 
     def _cast_int(self, value:Union[float,int], value_name:str) -> int:
         if isinstance(value, int): return value
         if isinstance(value, float) and value.is_integer(): return int(value)
         raise CobaException(f"{value_name} must be a whole number and not {value}.")
 
 class Repr(EnvironmentFilter):
-    def __init__(self, 
+    def __init__(self,
         categorical_context:Literal["onehot","onehot_tuple","string"] = None,
         categorical_actions:Literal["onehot","onehot_tuple","string"] = None) -> None:
         self._cat_context = categorical_context
         self._cat_actions = categorical_actions
 
     @property
     def params(self) -> Mapping[str, Any]:
@@ -934,18 +1013,19 @@
                 old_actions = new['actions']
 
                 if new_actions != old_actions or type(new_actions[0]) != type(old_actions[0]):
                     new['actions'] = new_actions
 
                 if new_actions != old_actions:
                     if has_rewards:
-                        if isinstance(new['rewards'],MulticlassReward):
-                            new['rewards'] = MulticlassReward(new_actions[old_actions.index(new['rewards'].argmax())])
+                        old_rewards = new['rewards']
+                        if isinstance(old_rewards,MulticlassReward):
+                            new['rewards'] = MulticlassReward(new_actions[old_actions.index(argmax(old_actions,old_rewards))])
                         else:
-                            new['rewards'] = SequenceReward(new_actions,list(map(new['rewards'].eval,old_actions)))
+                            new['rewards'] = SequenceReward(new_actions,list(map(old_rewards.eval,old_actions)))
                     if has_feedbacks:
                         new['feedbacks'] = SequenceFeedback(new_actions,list(map(new['feedbacks'].eval,old_actions)))
 
             yield new
 
 class Batch(EnvironmentFilter):
     def __init__(self, batch_size: int) -> None:
@@ -1093,22 +1173,26 @@
 
         if not interactions: return []
 
         if 'context' not in first or 'actions' not in first or 'rewards' not in first:
             raise CobaException("We were unable to create a logged representation of the interaction.")
 
         #Avoid circular dependency
-        from coba.experiments.tasks import OnPolicyEvaluation
+        from coba.evaluators import OnPolicyEvaluator
 
         seed = self._seed if self._seed is not None else CobaRandom().random()
 
         I1,I2 = tee(interactions,2)
-        flat_int = Unbatch().filter(I1)
-        eval_log = OnPolicyEvaluation(record=['action','reward','probability'],seed=seed).process(copy.deepcopy(self._learner),I2)
-        for interaction, log in zip(flat_int,eval_log):
+        interactions = Unbatch().filter(I1)
+
+        env = SimpleEnvironment(I2)
+        lrn = copy.deepcopy(self._learner)
+        evaluator = OnPolicyEvaluator(record=['action','reward','probability'],seed=seed)
+
+        for interaction, log in zip(interactions,evaluator.evaluate(env,lrn)):
             out = interaction.copy()
             out.update(log)
             yield out
 
 class Mutable(EnvironmentFilter):
 
     def filter(self, interactions: Iterable[Interaction]) -> Iterable[Interaction]:
@@ -1116,15 +1200,15 @@
         first, interactions = peek_first(interactions)
 
         if not interactions: return []
 
         first_is_dense   = isinstance(first['context'], primitives.Dense)
         first_is_sparse  = isinstance(first['context'], primitives.Sparse)
         first_is_value   = not (first_is_dense or first_is_sparse)
-        first_is_mutable = isinstance(first['context'], (list,dict))
+        first_is_mutable = isinstance(first['context'], (list,dict,SparseDense))
 
         if first_is_mutable:
             for interaction in interactions:
                 new = interaction.copy()
                 new['context'] = new['context'].copy()
                 yield new
 
@@ -1146,40 +1230,36 @@
 
 class MappingToInteraction(Filter[Iterable[Mapping], Iterable[Interaction]]):
     def filter(self, items: Iterable[Mapping]) -> Iterable[Interaction]:
         yield from map(Interaction.from_dict,items)
 
 class OpeRewards(EnvironmentFilter):
 
-    def __init__(self, rwds_type:Literal['IPS','DM','DR','NO']=None):
-        if rwds_type in ['DM','DR']:
+    def __init__(self, rwd_type:Literal['IPS','DM','DR']=None):
+        if rwd_type in ['DM','DR']:
             PackageChecker.vowpalwabbit("Rewards.__init__")
-        self._rwds_type = rwds_type
+        self._rwd_type = rwd_type
 
     @property
     def params(self) -> Mapping[str, Any]:
-        return {'rewards_type': self._rwds_type} if self._rwds_type else {}
+        return {'ope_reward': self._rwd_type or 'None'}
 
     def filter(self, interactions: Iterable[Interaction]) -> Iterable[Interaction]:
-        if self._rwds_type is None:
-            yield from interactions
+        rwd_type = self._rwd_type
 
-        elif self._rwds_type == "NO":
-            for log in interactions:
-                log = log.copy()
-                log.pop('rewards',None)
-                yield log
+        if rwd_type is None:
+            yield from interactions
 
-        elif self._rwds_type == "IPS":
+        elif rwd_type == "IPS":
             for log in interactions:
                 log = log.copy()
                 log['rewards'] = IPSReward(log['reward'], log['action'], log.get('probability'))
                 yield log
 
-        elif self._rwds_type in ["DM","DR"]:
+        elif rwd_type in ["DM","DR"]:
             from coba.learners.vowpal import VowpalMediator
 
             rng = CobaRandom(1)
             vw = VowpalMediator()
 
             # When using cb_adf to estimate rewards for actions instead of the
             # regression we would receive rewards far outside of the expected boundaries.
@@ -1194,53 +1274,31 @@
 
                 #Batch Shuffling reduces the correlation between
                 #the reward functions learned by this VW learner
                 #and potential downstream VW learners. If this
                 #correlation is strong, we will over estimate
                 #the downstream VW learner's performance.
                 L = list(islice(interactions,4000))
-                R = [ [] for _ in range(len(L)) ]
-                X = []
 
                 if not L: break
 
-                for log, rewards in rng.shuffle(list(zip(L,R)), inplace=True):
-                    log_context = log['context']
-                    log_action  = log['action']
-                    log_reward  = log['reward']
-                    log_prob    = log['probability']
-
-                    #type-4
-                    #labels            = [None]*len(log_actions)
-                    #labels[log_index] = f"{log_index+1}:{log_reward}:{log_prob}"
-                    #vw.learn(vw.make_examples({"x":log_context}, [{"a":a} for a in log_actions], labels))
-
-                    #type-1
-                    vw.learn(vw.make_example({"x":log_context, "a": log_action}, f"{log_reward} {1/log_prob}"))
-
-                for log, rewards in rng.shuffle(list(zip(L,R)), inplace=True):
-                    log_context = log['context']
-                    log_actions = log['actions']
-                    log_action  = log['action']
-                    log_reward  = log['reward']
-                    log_prob    = log['probability']
-                    log_index   = log_actions.index(log_action)
-
-                    #type-4
-                    #examples = vw.make_examples({"x":log_context}, [{"a":a} for a in log_actions])
-                    #rewards.extend(vw.predict(examples))
-
-                    #type-1
-                    examples = vw.make_examples({"x":log_context}, [{"a":a} for a in log_actions])
-                    rewards.extend(vw.predict(e) for e in examples)
-
-                    if self._rwds_type=="DR":
-                        rewards[log_index] += (log_reward-rewards[log_index])/log_prob
+                for log in rng.shuffle(L):
+                    features = {"x": log['context'], "a": log['action']}
+                    label    = f"{log['reward']} {1/(log['probability'] or 1)}"
+                    vw.learn(vw.make_example(features,label))
+
+                for log in L:
+
+                    examples = vw.make_examples({"x":log['context']}, [{"a":a} for a in log['actions']])
+                    rewards = list(map(vw.predict,examples))
+
+                    if rwd_type=="DR":
+                        log_index = log['actions'].index(log['action'])
+                        rewards[log_index] += (log['reward']-rewards[log_index])/(log['probability'] or 1)
 
-                for log,rewards in zip(L,R):
                     log = log.copy()
 
                     try:
                         log['rewards'] = MappingReward(dict(zip(log['actions'],rewards)))
                     except:
                         log['rewards'] = SequenceReward(log['actions'],rewards)
```

### Comparing `coba-6.5.0/coba/environments/openml.py` & `coba-7.0.0/coba/environments/openml.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
     def __init__(self, *args, **kwargs) -> None:
         """Instantiate an OpenmlSimulation."""
         kwargs.update(zip(['data_id','drop_missing','take'], args))
         super().__init__(OpenmlSource(**kwargs), None, kwargs.get('label_type',None), kwargs.get('take',None))
 
     @property
     def params(self) -> Dict[str, Any]:
-        return {**super().params, "type": "OpenmlSimulation" }
+        return {**super().params, "env_type": "OpenmlSimulation" }
 
     def __str__(self) -> str:
 
         params = [
             f"data={self.params['openml_data']}" if self.params.get('openml_data') else f"task={self.params['openml_task']}",
             f"target={self.params['openml_target']}" if self.params.get('openml_target') else "",
         ]
```

### Comparing `coba-6.5.0/coba/environments/primitives.py` & `coba-7.0.0/coba/environments/primitives.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,25 @@
 from abc import abstractmethod, ABC
 from typing import Any, Union, Iterable, Sequence, Mapping, overload
 
 from coba.primitives import Context, Action, Actions
-from coba.primitives import Reward, SequenceReward, Feedback, SequenceFeedback, IPSReward
+from coba.primitives import Reward, SequenceReward, Feedback, SequenceFeedback
 from coba.pipes import Source, SourceFilters, Filter
-from coba.exceptions import CobaException
 
 class Interaction(dict):
     """An individual interaction that occurs in an Environment."""
     __slots__=()
     keywords = {}
 
-    @property
-    def extra(self) -> Mapping[str,Any]:
-        return { k:self[k] for k in self.keys()-self.keywords}
-
     @staticmethod
     def from_dict(kwargs_dict: Mapping[str, Any]) -> 'Interaction':
-        if 'feedbacks' in kwargs_dict:
-            sub_class =  GroundedInteraction
-        elif 'rewards' in kwargs_dict:
-            sub_class = SimulatedInteraction
-        else:
-            sub_class =  LoggedInteraction
-
-        return sub_class(**kwargs_dict)
+        if 'feedbacks' in kwargs_dict: return GroundedInteraction(**kwargs_dict)
+        if 'rewards' in kwargs_dict: return SimulatedInteraction(**kwargs_dict)
+        if 'reward' in kwargs_dict: return LoggedInteraction(**kwargs_dict)
+        return kwargs_dict
 
 class SimulatedInteraction(Interaction):
     """Simulated data that provides rewards for every possible action."""
     __slots__=()
     keywords = {'type', 'context', 'actions', 'rewards'}
 
     def __init__(self,
@@ -68,17 +59,17 @@
             context: Features describing the interaction's context.
             actions: Features describing available actions during the interaction.
             rewards: The reward for each action in the interaction.
             feedbacks: The feedback for each action in the interaction.
             **kwargs: Additional information that should be recorded in the interactions table of an experiment result.
         """
 
-        self['context'] = context
-        self['actions'] = actions
-        self['rewards'] = SequenceReward(actions,rewards) if isinstance(rewards,(list,tuple)) else rewards
+        self['context']   = context
+        self['actions']   = actions
+        self['rewards']   = SequenceReward(actions,rewards) if isinstance(rewards,(list,tuple)) else rewards
         self['feedbacks'] = SequenceFeedback(actions,feedbacks) if isinstance(feedbacks,(list,tuple)) else feedbacks
 
         if kwargs: self.update(kwargs)
 
 class LoggedInteraction(Interaction):
     """A logged interaction with an action, reward and optional probability."""
     __slots__ = ()
@@ -106,15 +97,15 @@
         Args
             context: Features describing the logged context.
             action: Features describing the action taken by the logging policy.
             reward: The reward that was revealed when the logged action was taken.
             probability: The probability that the logged action was taken. That is P(action|context,actions,logging policy).
             actions: All actions that were availble to be taken when the logged action was taken. Necessary for OPE.
             rewards: The rewards to use for off policy evaluation. These rewards will not be shown to any learners. They will
-                only be recorded in experimental results. If probability and actions is provided and rewards is None then 
+                only be recorded in experimental results. If probability and actions is provided and rewards is None then
                 rewards will be initialized using the IPS estimator.
             **kwargs : Any additional information.
         """
 
         if isinstance(kwargs.get('rewards'),(list,tuple)):
             self['rewards'] = SequenceReward(kwargs['actions'],kwargs.pop('rewards'))
 
@@ -132,15 +123,15 @@
         """Apply a filter to an Environment's interactions."""
         ...
 
 class Environment(Source[Iterable[Interaction]], ABC):
     """An Environment that produces Contextual Bandit data"""
 
     @property
-    def params(self) -> Mapping[str,Any]: # pragma: no cover
+    def params(self) -> Mapping[str,Any]: #pragma: no cover
         """Paramaters describing the simulation.
 
         Remarks:
             These will become columns in the environments table of experiment results.
         """
         return {}
 
@@ -152,58 +143,59 @@
             This function should always be "re-iterable".
         """
         ...
 
     def __str__(self) -> str:
         return str(self.params) if self.params else self.__class__.__name__
 
-class SimulatedEnvironment(Environment):
-    """An environment made from SimulatedInteractions."""
-
-    @abstractmethod
-    def read(self) -> Iterable[SimulatedInteraction]:
-        """The sequence of interactions in the environment.
-
-        Remarks:
-            This function should always be "re-iterable".
-        """
-        ...
-
 class SafeEnvironment(Environment):
     """A wrapper for environment-likes that guarantees interface consistency."""
 
     def __init__(self, environment: Environment) -> None:
         """Instantiate a SafeEnvironment.
 
         Args:
             environment: The environment we wish to make sure has the expected interface
         """
 
-        self._environment = environment if not isinstance(environment, SafeEnvironment) else environment._environment
+        self.environment = environment if not isinstance(environment, SafeEnvironment) else environment.environment
 
     @property
     def params(self) -> Mapping[str, Any]:
         try:
-            params = self._environment.params
+            params = self.environment.params
         except AttributeError:
             params = {}
 
-        if "type" not in params:
+        if "env_type" not in params:
 
-            if isinstance(self._environment, SourceFilters):
-                params["type"] = self._environment._source.__class__.__name__
+            if isinstance(self.environment, SourceFilters):
+                params["env_type"] = self.environment._source.__class__.__name__
             else:
-                params["type"] = self._environment.__class__.__name__
+                params["env_type"] = self.environment.__class__.__name__
 
         return params
 
     def read(self) -> Iterable[Interaction]:
-        return self._environment.read()
+        return self.environment.read()
 
     def __str__(self) -> str:
         params = dict(self.params)
-        tipe   = params.pop("type")
+        tipe   = params.pop("env_type")
 
         if len(params) > 0:
             return f"{tipe}({','.join(f'{k}={v}' for k,v in params.items())})"
         else:
             return tipe
+
+class SimpleEnvironment(Environment):
+
+    def __init__(self, interactions: Sequence[Interaction]=(), params: Mapping[str,Any]={}) -> None:
+        self._interactions = interactions
+        self._params = params
+
+    @property
+    def params(self):
+        return self._params
+
+    def read(self) -> Iterable[Interaction]:
+        return self._interactions
```

### Comparing `coba-6.5.0/coba/environments/serialized.py` & `coba-7.0.0/coba/environments/serialized.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from pathlib import Path
 from collections import abc
 from zipfile import ZipFile, ZIP_DEFLATED
 from itertools import islice, repeat, chain
 from typing import Union, Sequence, Mapping, Iterable, Any
 
 from coba.contexts import CobaContext
-from coba.backports import version
 from coba.pipes import Source, Sink, Filter
 from coba.environments.primitives import Environment, Interaction
 
 class ObjectsToZipMember(Sink[Iterable[Sequence[object]]]):
     def __init__(self, zip:str):
         self._zip = zip
         self._start = 0
@@ -43,22 +42,21 @@
             with ZipFile(self._zip) as z:
                 with z.open(self._member) as m:
                     yield from map(pickle.load, repeat(m))
         except EOFError:
             pass
 
 class EnvironmentsToObjects(Filter[Environment, Iterable]):
-    def filter(self, envs: Union[Environment,Sequence[Environment]]) -> Iterable[Iterable[object]]:
-        if not isinstance(envs,(abc.Iterable)): envs = [envs]
-        for env in envs:
-            with CobaContext.logger.time("Materializing environment..."):
-                yield list(self._env_to_objects(env))
+    def filter(self, env: Union[Environment,Sequence[Environment]]) -> Iterable[Iterable[object]]:        
+        with CobaContext.logger.time("Materializing environment..."):
+            yield list(self._env_to_objects(env))
 
     def _env_to_objects(self,env):
-        yield {"version":2,"coba_version":version("coba")}
+        from coba import __version__ #imported here to avoid circular dependency
+        yield {"version":2,"coba_version":__version__}
         yield env.params
         I = iter(env.read())
         batch = list(islice(I,1000))
         while batch: 
             yield batch
             batch = list(islice(I,1000))
```

### Comparing `coba-6.5.0/coba/environments/supervised.py` & `coba-7.0.0/coba/environments/supervised.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from coba.pipes import Pipes, Source, IterableSource, LabelRows, Reservoir, UrlSource, CsvReader
 from coba.pipes import CsvReader, ArffReader, LibsvmReader, ManikReader
 
 from coba.utilities import peek_first
 from coba.primitives import Categorical, L1Reward, MulticlassReward, HammingReward
 
-from coba.environments.primitives import SimulatedEnvironment, SimulatedInteraction
+from coba.environments.primitives import Environment, SimulatedInteraction
 
 class CsvSource(Source[Iterable[MutableSequence]]):
     """Load a source (either local or remote) in CSV format.
 
     This is primarily used by SupervisedSimulation to create Environments for Experiments.
     """
 
@@ -116,15 +116,15 @@
     def params(self) -> Dict[str, Any]:
         """Parameters describing the manik source."""
         return self._source.params
 
     def __str__(self) -> str:
         return str(self._source)
 
-class SupervisedSimulation(SimulatedEnvironment):
+class SupervisedSimulation(Environment):
     """Create a contextual bandit simulation using an existing supervised regression or classification dataset."""
 
     @overload
     def __init__(self,
         source: Source = None,
         label_col: Union[int,str] = None,
         label_type: Literal["c","r","m"] = None,
@@ -173,15 +173,15 @@
             Y          = args[1]
             label_type = args[2] if len(args) > 2 else kwargs.get("label_type", None)
             params     = {"source": "[X,Y]"}
             source     = IterableSource(zip(X,Y))
 
         self._label_type = label_type
         self._source     = source
-        self._params     = {**params, "label_type": self._label_type, "type": "SupervisedSimulation" }
+        self._params     = {**params, "label_type": self._label_type, "env_type": "SupervisedSimulation" }
 
     @property
     def params(self) -> Dict[str,Any]:
         return self._params
 
     def read(self) -> Iterable[SimulatedInteraction]:
 
@@ -195,20 +195,19 @@
 
         if first_label_type is None:
             label_type = self._label_type or ("r" if isinstance(first_label, (int,float)) else "c")
         else:
             label_type = self._label_type or first_label_type
 
         label_type = label_type.lower()
-        self._params['label_type'] = label_type.upper()
 
         if label_type == "r":
             actions = []
             reward  = L1Reward
-        
+
         elif label_type == "c" and isinstance(first_label, Categorical):
             #Handling the categoricals separately allows for a performance optimization
             #since we can use the Categorical's as_int property rather than action_indexes
             actions = [ Categorical(l,first_label.levels) for l in first_label.levels ]
             reward  = MulticlassReward
         else:
             #we need to know all labels in the dataset to determine actions
```

### Comparing `coba-6.5.0/coba/environments/synthetics.py` & `coba-7.0.0/coba/environments/synthetics.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from typing import Sequence, Dict, Tuple, Any, Callable, Optional, overload, Iterable
 from coba.backports import Literal
 
 from coba.exceptions import CobaException
 from coba.random import CobaRandom
 from coba.encodings import InteractionsEncoder, OneHotEncoder
 
-from coba.environments.primitives import Context, Action, SimulatedEnvironment, SimulatedInteraction, SequenceReward
+from coba.environments.primitives import Context, Action, Environment, SimulatedInteraction, SequenceReward
 
-class LambdaSimulation(SimulatedEnvironment):
+class LambdaSimulation(Environment):
     """A simulation created from generative lambda functions."""
 
     @overload
     def __init__(self,
         n_interactions: Optional[int],
         context       : Callable[[int               ],Context         ],
         actions       : Callable[[int,Context       ],Sequence[Action]],
@@ -54,15 +54,15 @@
         self._actions        = actions
         self._reward         = reward
         self._make_rng       = seed is not None
         if seed is not None: self._seed = seed
 
     @property
     def params(self) -> Dict[str, Any]:
-        params = { "type": "LambdaSimulation" }
+        params = { "env_type": "LambdaSimulation" }
 
         if hasattr(self, '_seed'):
             params["seed"] = self._seed
 
         return params
 
     def read(self) -> Iterable[SimulatedInteraction]:
@@ -177,15 +177,15 @@
         def reward(index:int, context:Tuple[float,...], action:Tuple[int,...]):
             return context_action_rewards[(context,action)]
 
         return super().__init__(self._n_interactions, context, actions, reward)
 
     @property
     def params(self) -> Dict[str, Any]:
-        return {**super().params, "type": "NeighborsSynthetic", "n_neighborhoods": self._n_neighborhoods }
+        return {**super().params, "env_type": "NeighborsSynthetic", "n_neighborhoods": self._n_neighborhoods }
 
     def __str__(self) -> str:
         return f"NeighborsSynth(A={self._n_actions},c={self._n_context_feats},a={self._n_action_feats},N={self._n_neighborhoods},seed={self._seed})"
 
     def __reduce__(self) -> Tuple[object, ...]:
         return (NeighborsSyntheticSimulation, self._args)
 
@@ -269,15 +269,15 @@
             self._weights[i] = [w/scale for w in self._weights[i]]
             self._biases[i]  = 0.5-mean(part_rewards)/scale
 
         super().__init__(n_interactions, context, actions, reward, seed=self._seed)
 
     @property
     def params(self) -> Dict[str, Any]:
-        return {**super().params, "type":"LinearSynthetic", "reward_features": self._reward_features }
+        return {**super().params, "env_type":"LinearSynthetic", "reward_features": self._reward_features }
 
     def __reduce__(self) -> Tuple[object, ...]:
         return (LinearSyntheticSimulation, self._args)
 
     def __str__(self) -> str:
         return f"LinearSynth(A={self._n_actions},c={self._n_context_features},a={self._n_action_features},R={self._reward_features},seed={self._seed})"
 
@@ -381,15 +381,15 @@
             self._weights[i] = [w/scale for w in self._weights[i]]
             self._biases[i]  = 0.5-mean(part_rewards)/scale
 
         super().__init__(n_interactions, context, actions, reward, self._seed)
 
     @property
     def params(self) -> Dict[str, Any]:
-        params = {**super().params, "type": "KernelSynthetic", "n_exemplars": self._n_exemplars, 'kernel': self._kernel}
+        params = {**super().params, "env_type": "KernelSynthetic", "n_exemplars": self._n_exemplars, 'kernel': self._kernel}
 
         if self._kernel == "polynomial":
             params['degree'] = self._degree
 
         if self._kernel in ["exponential","gaussian"]:
             params['gamma'] = self._gamma
 
@@ -500,14 +500,14 @@
         self._bias = 0.5-m/s
         self._output_weights = [ w/s for w in self._output_weights ]
 
         super().__init__(n_interactions, context, actions, reward, self._seed)
 
     @property
     def params(self) -> Dict[str, Any]:
-        return {**super().params, "type": "MLPSynthetic" }
+        return {**super().params, "env_type": "MLPSynthetic" }
 
     def __reduce__(self) -> Tuple[object, ...]:
         return (MLPSyntheticSimulation, self._args)
 
     def __str__(self) -> str:
         return f"MLPSynth(A={self._n_actions},c={self._n_context_features},a={self._n_action_features},seed={self._seed})"
```

### Comparing `coba-6.5.0/coba/environments/templates.py` & `coba-7.0.0/coba/environments/templates.py`

 * *Files identical despite different names*

### Comparing `coba-6.5.0/coba/exceptions.py` & `coba-7.0.0/coba/exceptions.py`

 * *Files identical despite different names*

### Comparing `coba-6.5.0/coba/experiments/core.py` & `coba-7.0.0/coba/experiments/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,78 @@
+
+from collections import abc
 from pathlib import Path
 from itertools import product
 from typing import Sequence, Optional, Union, overload, Tuple
 
-from coba.pipes import Pipes
-from coba.learners import Learner
 from coba.environments import Environment
-from coba.multiprocessing import CobaMultiprocessor
+from coba.learners     import Learner
+from coba.evaluators   import Evaluator, OnPolicyEvaluator
+
+from coba.pipes import Pipes, DiskSink, ListSink, DiskSource, ListSource, Identity, Insert
 from coba.contexts import CobaContext, ExceptLog, StampLog, NameLog, DecoratedLogger, ExceptionLogger
 from coba.exceptions import CobaException
+from coba.multiprocessing import CobaMultiprocessor
 
-from coba.experiments.process import CreateWorkItems,  RemoveFinished, ChunkByChunk, MaxChunkSize, ProcessWorkItems
-from coba.experiments.tasks   import EnvironmentTask, EvaluationTask, LearnerTask
-from coba.experiments.tasks   import SimpleLearnerInfo, SimpleEnvironmentInfo, SimpleEvaluation, LambdaEvaluation
-from coba.experiments.results import Result, TransactionIO
+from coba.experiments.process import MakeTasks, ChunkTasks, ProcessTasks
+from coba.experiments.results import Result, TransactionDecode, TransactionEncode, TransactionResult
 
 class Experiment:
     """An Experiment using a collection of environments and learners."""
 
     @overload
     def __init__(self,
-        environments    : Union[Environment, Sequence[Environment]],
-        learners        : Union[Learner,Sequence[Learner]],
-        *,
-        description     : str             = None,
-        learner_task    : LearnerTask     = SimpleLearnerInfo(),
-        environment_task: EnvironmentTask = SimpleEnvironmentInfo(),
-        evaluation_task : EvaluationTask  = SimpleEvaluation()) -> None:
+        environments : Union[Environment, Sequence[Environment]],
+        learners     : Union[Learner,Sequence[Learner]],
+        evaluator    : Union[Evaluator,Sequence[Evaluator]] = OnPolicyEvaluator(),
+        description  : str = None) -> None:
         """Instantiate an Experiment.
 
         Args:
             environments: The collection of environments to use in the experiment.
             learners: The collection of learners to use in the experiment.
+            evaluator: The evaluation task we wish to perform on learners and environments.
             description: A description of the experiment for documentaiton purposes.
-            learner_task: A task which describes a learner.
-            environment_task: A task which describes an environment.
-            evaluation_task: A task which evaluates a learner on an environment.
         """
 
     @overload
     def __init__(self,
-        eval_pairs      : Sequence[Tuple[Learner,Environment]],
-        *,
-        description     : str             = None,
-        learner_task    : LearnerTask     = SimpleLearnerInfo(),
-        environment_task: EnvironmentTask = SimpleEnvironmentInfo(),
-        evaluation_task : EvaluationTask  = SimpleEvaluation()) -> None:
+        eval_tuples: Sequence[Tuple[Learner,Environment,Evaluator]],
+        description: str = None) -> None:
         ...
         """Instantiate an Experiment.
 
         Args:
-            eval_pairs: The collection of learners with their evaluation environments.
-            learner_task: A task which describes a learner.
-            environment_task: A task which describes an environment.
-            evaluation_task: A task which evaluates a learner on an environment.
+            eval_tuples: The learner-environment-evaluator triples we wish to evaluate.
+            description: A description of the experiment for documentaiton purposes.
         """
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args,**kwargs) -> None:
         """Instantiate an Experiment."""
 
-        # TODO kwargs from other constructors aren't properly processed
-        if len(args) == 2:
-            envs = [args[0]] if hasattr(args[0],'read') else args[0]
-            lrns = [args[1]] if hasattr(args[1],'predict') else args[1]
-            args = [list(zip(*reversed(list(zip(*product(envs,lrns))))))]
-
-        self._pairs            = args[0]
-        self._description      = kwargs.get('description',None)
-        self._learner_task     = kwargs.get('learner_task', SimpleLearnerInfo())
-        self._environment_task = kwargs.get('environment_task', SimpleEnvironmentInfo())
-        self._evaluation_task  = kwargs.get('evaluation_task', SimpleEvaluation())
+        if 'evaluation_task' in kwargs:
+            raise CobaException(
+                "The `evaluation_task` argument has been deprecated. Instead of `Experiment(x,y,evaluation_task=t)` "
+                "you should call `Experiment(x,y,t)`. Additionally if you are using a custom evaluator then the "
+                "main evaluation method should be `def evaluate(self, learner, environment)` rather than "
+                "`def process(self,learner,interactions)`."
+            )
+
+        args = list(args)
+        if len(args) > 0 and not isinstance(args[0],(abc.Sequence,abc.Iterable)): args[0] = [args[0]]
+
+        triples,description = self._parse_init_args(*args,**kwargs)
 
-        if callable(self._evaluation_task):
-            self._evaluation_task = LambdaEvaluation(self._evaluation_task)
+        self._triples     = triples
+        self._description = description
 
-        if any([lrn is None for lrn,_ in self._pairs]):
+        if any([lrn is None for _,lrn,_ in self._triples]):
             raise CobaException("A Learner was given whose value was None, which can't be processed.")
 
-        if any([env is None for _,env in self._pairs]):
+        if any([env is None for env,_,_ in self._triples]):
             raise CobaException("An Environment was given whose value was None, which can't be processed.")
 
         self._processes        : Optional[int] = None
         self._maxchunksperchild: Optional[int] = None
         self._maxtasksperchunk : Optional[int] = None
 
     def config(self,
@@ -89,17 +81,17 @@
         maxtasksperchunk: Optional[int] = None) -> 'Experiment':
         """Configure how the experiment will be executed.
 
         A value of `None` for any item means the CobaContext.experiment will be used.
 
         Args:
             processes: The number of processes to create for evaluating the experiment.
-            maxchunksperchild: The number of chunks each process evaluate before being restarted. A 
+            maxchunksperchild: The number of chunks each process evaluate before being restarted. A
                 value of 0 means that all processes will survive until the end of the experiment.
-            maxtasksperchunk: The maximum number of tasks a chunk can have. If a chunk has too many 
+            maxtasksperchunk: The maximum number of tasks a chunk can have. If a chunk has too many
                 tasks it will be split into smaller chunks. A value of 0 means that chunks are never
                 broken down into smaller chunks.
         """
 
         assert processes is None or processes > 0, "The given number of processes is invalid. Must be greater than 0."
         assert maxchunksperchild is None or maxchunksperchild >= 0, "The given number of chunks per child is invalid. Must be greater than or equal to 0 (0 for infinite)."
         assert maxtasksperchunk is None or maxtasksperchunk >= 0, "The given number of tasks per chunk is invalid. Must be greater than or equal to 0 (0 for infinite)."
@@ -142,50 +134,80 @@
         old_logger = CobaContext.logger
 
         if quiet:
             CobaContext.logger = DecoratedLogger([], ExceptionLogger(CobaContext.logger.sink), [NameLog(),StampLog()] if is_multiproc else [StampLog()])
         else:
             CobaContext.logger = DecoratedLogger([ExceptLog()], CobaContext.logger, [NameLog(),StampLog()] if is_multiproc else [StampLog()])
 
+        CobaContext.logger.log("Experiment Started")
+
         if result_file and Path(result_file).exists():
-            CobaContext.logger.log("Restoring existing experiment logs...")
+            CobaContext.logger.log("Restoring Results")
             restored = Result.from_file(result_file)
         else:
             restored = None
 
-        n_given_learners     = len(set([l for l,_ in self._pairs]))
-        n_given_environments = len(set([e for _,e in self._pairs]))
+        n_given_lrns = len(set([l for _,l,_ in self._triples]))
+        n_given_envs = len(set([e for e,_,_ in self._triples]))
 
-        if restored:
-            assert n_given_learners     == restored.experiment.get('n_learners',n_given_learners)        , "The current experiment doesn't match the given transaction log."
-            assert n_given_environments == restored.experiment.get('n_environments',n_given_environments), "The current experiment doesn't match the given transaction log."
-
-        workitems  = CreateWorkItems(self._pairs, self._learner_task, self._environment_task, self._evaluation_task)
-        unfinished = RemoveFinished(restored)
-        chunk      = ChunkByChunk(mp)
-        max_chunk  = MaxChunkSize(mt)
-        sink       = TransactionIO(result_file)
-        process    = CobaMultiprocessor(ProcessWorkItems(), mp, mc, False)
+        meta = {'n_learners':n_given_lrns,'n_environments':n_given_envs,'description':self._description,'seed':seed}
 
-        try:
-            if not restored: sink.write([["T0", {'n_learners':n_given_learners, 'n_environments':n_given_environments, 'description':self._description, 'seed':seed }]])
-            Pipes.join(workitems, unfinished, chunk, max_chunk, process, sink).run()
-
-        except KeyboardInterrupt: # pragma: no cover
-            CobaContext.logger.log("Experiment execution was manually aborted via Ctrl-C")
+        workitems = MakeTasks(self._triples,restored)
+        chunker   = ChunkTasks(mt)
+        process   = CobaMultiprocessor(ProcessTasks(), mp, mc, False)
+        encode    = TransactionEncode()
+        sink      = DiskSink(result_file,batch=1) if result_file else ListSink(foreach=True)
+        source    = DiskSource(result_file) if result_file else ListSource(sink.items)
+        decode    = TransactionDecode()
+        result    = TransactionResult()
+        preamble  = Identity() if restored else Insert([["T0",meta]])
 
-        except Exception as ex: # pragma: no cover
+        try:
+            lrn_mismatch = restored and n_given_lrns != restored.experiment.get('n_learners',n_given_lrns)
+            env_mismatch = restored and n_given_envs != restored.experiment.get('n_environments',n_given_envs)
+            if lrn_mismatch or env_mismatch: raise CobaException("The experiment does not match the given logs")
+            Pipes.join(workitems, chunker, process, preamble, encode, sink).run()
+        except KeyboardInterrupt: #pragma: no cover
+            CobaContext.logger.log("Experiment Aborted (aborted via Ctrl-C)")
+        except Exception as ex: #pragma: no cover
             CobaContext.logger.log(ex)
+            CobaContext.logger.log("Experiment Failed")
+        else:
+            CobaContext.logger.log("Experiment Finished")
 
         CobaContext.logger = old_logger
         del CobaContext.store['experiment_seed']
 
-        return sink.read()
+        return Pipes.join(source,decode,result).read()
 
     def evaluate(self, result_file:str = None) -> Result:
         """Evaluate the experiment and return the results (this is a backwards compatible proxy for the run method).
 
         Args:
             result_file: The file for writing and restoring results .
         """
 
         return self.run(result_file=result_file)
+
+    def _parse_init_args(self,*args,**kwargs) -> Tuple[Sequence[Tuple[Environment,Learner]], Evaluator, Optional[str]]:
+        #we know this with 100% certainty
+        definite_triples = ({'eval_tuples'} & kwargs.keys()            ) or \
+                           (len(args) == 1 and 'learners' not in kwargs) or \
+                           (len(args) == 2 and isinstance(args[1],str) )
+        try:
+            if definite_triples:
+                triples = args[0] if len(args) > 0 else kwargs['eval_tuples']
+                descr   = args[1] if len(args) > 1 else kwargs.get('description',None)
+                return list(triples), descr
+
+            else:
+                envs  = args[0] if len(args) > 0 else kwargs['environments']
+                lrns  = args[1] if len(args) > 1 else kwargs['learners']
+                vals  = args[2] if len(args) > 2 else kwargs.get('evaluator',OnPolicyEvaluator())
+                descr = args[3] if len(args) > 3 else kwargs.get('description',None)
+                if not isinstance(envs,abc.Sequence): envs = [envs]
+                if not isinstance(lrns,abc.Sequence): lrns = [lrns]
+                if not isinstance(vals,abc.Sequence): vals = [vals]
+
+                return list(product(envs,lrns,vals)), descr
+        except KeyError as e:
+            raise TypeError(f'Experiment.__init__ missing required arguments')
```

### Comparing `coba-6.5.0/coba/experiments/results.py` & `coba-7.0.0/coba/experiments/results.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,84 +1,68 @@
 import re
 import collections
 import collections.abc
 
 from bisect import bisect_left, bisect_right
 from pathlib import Path
 from numbers import Number
-from operator import truediv, sub, itemgetter, gt
+from operator import truediv, sub, itemgetter
+from functools import cmp_to_key
 from abc import abstractmethod
-from itertools import chain, repeat, accumulate, groupby, count, compress
-from typing import Any, Mapping, Tuple, Optional, Sequence, Iterable, Iterator, Union, Callable, NamedTuple
+from dataclasses import dataclass, astuple, field, replace
+from itertools import chain, repeat, accumulate, groupby, count, compress, groupby
+from typing import Mapping, Tuple, Optional, Sequence, Iterable, Iterator, Union, Callable, List, Any, overload
 from coba.backports import Literal
 
 from coba.primitives import Batch
 from coba.environments import Environment
-from coba.statistics import mean, stdev, StandardErrorOfMean, BootstrapConfidenceInterval, BinomialConfidenceInterval, PointAndInterval
+from coba.statistics import mean, StdDevCI, StdErrCI, BootstrapCI, BinomialCI, PointAndInterval
 from coba.contexts import CobaContext
 from coba.exceptions import CobaException
 from coba.utilities import PackageChecker, peek_first
-from coba.pipes import Pipes, Sink, Source, JsonEncode, JsonDecode, DiskSource, DiskSink, IterableSource, ListSink, Foreach
+from coba.pipes import Pipes, JsonEncode, JsonDecode, DiskSource
 
-def exponential_moving_average(values:Sequence[float], span:int=None) -> Iterable[float]:
-    #exponential moving average identical to Pandas df.ewm(span=span).mean()
-    alpha = 2/(1+span)
-    cumwindow  = list(accumulate(values          , lambda a,v: v + (1-alpha)*a))
-    cumdivisor = list(accumulate([1.]*len(values), lambda a,v: v + (1-alpha)*a))
-    return map(truediv, cumwindow, cumdivisor)
+def moving_average(values:Sequence[float], span:int=None, exponential:bool=False) -> Iterable[float]:
 
-def moving_average(values:Sequence[float], span:int=None) -> Iterable[float]:
-    if span == 1:
-        return values
-
-    if span is None or span >= len(values):
-        return tuple(map(truediv, accumulate(values),count(1)))
-
-    window_sums  = accumulate(map(sub, values, chain(repeat(0,span),values)))
-    window_sizes = chain(range(1,span), repeat(span))
-
-    return map(truediv,window_sums,window_sizes)
-
-def old_to_new(
-    env_rows: Mapping[int           ,Mapping[str,Any]] = {},
-    lrn_rows: Mapping[int           ,Mapping[str,Any]] = {},
-    int_rows: Mapping[Tuple[int,int],Mapping[str,Any]] = {}) -> Tuple[Sequence,Sequence,Sequence]:
-
-    rwd_col = ['reward'] if any('reward' in v.keys() for v in int_rows.values()) else []
-
-    env_table = Table(columns=['environment_id'                     ]          )
-    lrn_table = Table(columns=[                 'learner_id'        ]          )
-    int_table = Table(columns=['environment_id','learner_id','index'] + rwd_col)
-
-    env_table.insert([{"environment_id":e,                **v} for e,v in env_rows.items()])
-    lrn_table.insert([{                   "learner_id":l, **v} for l,v in lrn_rows.items()])
-
-    for (env_id, lrn_id), results in int_rows.items():
-        if results.get('_packed'):
+    if exponential:
+        #exponential moving average identical to Pandas' df.ewm(span=span).mean()
+        alpha = 2/(1+span)
+        cumwindow  = list(accumulate(values          , lambda a,v: v + (1-alpha)*a))
+        cumdivisor = list(accumulate([1.]*len(values), lambda a,v: v + (1-alpha)*a))
+        return map(truediv, cumwindow, cumdivisor)
 
-            packed = results['_packed']
-            N = len(packed[next(iter(packed))])
-
-            packed['environment_id'] = repeat(env_id,N)
-            packed['learner_id'    ] = repeat(lrn_id,N)
-            packed['index'         ] = range(1,N+1)
-
-            int_table.insert(packed)
-
-    return env_table, lrn_table, int_table
+    elif span == 1:
+        return values
 
-def env_len_and_cnt(interactions: 'Table') -> Tuple[Mapping[int,int],Mapping[int,int]]:
-    env_len = {}
-    env_cnt = {}
-    for table in interactions.groupby(2):
-        env_id = table['environment_id'][0]
-        env_len[env_id] = len(table)
-        env_cnt[env_id] = env_cnt.get(env_id,0)+1
+    elif span is None or span >= len(values):
+        return map(truediv, accumulate(values), count(1))
 
-    return env_len, env_cnt
+    else:
+        window_sums  = accumulate(map(sub, values, chain(repeat(0,span),values)))
+        window_sizes = chain(range(1,span), repeat(span))
+
+        return map(truediv,window_sums,window_sizes)
+
+def comparer(item1,item2):
+    try:
+        if item1[:-1]<item2[:-1]:
+            return -1
+        if item1[:-1]>item2[:-1]:
+            return 1
+        return 0
+    except TypeError as e:
+        if 'NoneType' in str(e):
+            return -1 if str(e).endswith("'NoneType'") else 1
+        if 'str' in str(e):
+            return -1 if str(e).endswith("'str'") else 1
+
+#this adds one more check on average but avoids the worst case
+#scenario, which can be common for certain types of experiments.
+def my_bisect_left(c,a,l,h): return l if c[l  ]==a else bisect_left(c,a,l,h)
+def my_bisect_right(c,a,l,h): return h if c[h-1]==a else bisect_right(c,a,l,h)
 
 class View:
 
     class ListView:
         def __init__(self, seq:Sequence, sel:Sequence):
             self._seq = seq
             self._sel = sel
@@ -91,44 +75,89 @@
                 return View.ListView(self._seq,self._sel[key])
             else:
                 return self._seq[self._sel[key]]
 
         def __iter__(self):
             return iter(map(self._seq.__getitem__,self._sel))
 
-    def __init__(self, data: Mapping[str,Sequence], selection: Union[Sequence[int],slice]) -> None:
-        self._data = data
-        self._selection = selection
+    class SliceView:
+        def __init__(self, seq:Sequence, sel:slice):
+            self._seq = seq
+            self._sel = sel
+
+        def __len__(self):
+            return (self._sel.stop or len(self._seq)) - (self._sel.start or 0)
+
+        def __getitem__(self,key):
+            if isinstance(key,slice):
+                key_start = key.start or 0
+                key_stop  = key.stop or len(self)
+                new_start = (self._sel.start or 0) + key_start
+                new_stop  = new_start + key_stop - key_start
+                return self._seq[slice(new_start,new_stop)]
+            else:
+                return self._seq[(self._sel.start or 0)+key]
+
+        def __iter__(self):
+            #this isn't a true iter, this makes a copy, but
+            #this runs about 3x faster than doing a true iter.
+            return iter(self._seq[self._sel])
+
+    def __init__(self, data: Union[Mapping[str,Sequence],'View'], select: Union[Sequence[int],slice]) -> None:
+        if isinstance(data,collections.abc.Mapping):
+            self._data = data
+            self._select = self._try_slice(select)
+        else:
+            self._data = data._data
+
+            given_slice = isinstance(select,slice)
+            have_slice  = isinstance(data._select,slice)
+
+            if given_slice and have_slice:
+                self._select = slice(data._select.start+select.start,data._select.start+select.stop)
+            if given_slice and not have_slice:
+                self._select = self._try_slice(data._select[select])
+            if not given_slice and have_slice:
+                self._select = self._try_slice([data._select.start + i for i in select])
+            if not given_slice and not have_slice:
+                self._select = self._try_slice([data._select[i] for i in select])
+
+    def _try_slice(self, select: Sequence[int]):
+        if select and not isinstance(select,slice) and (select[-1]-select[0]+1) == len(select):
+            return slice(select[0], select[-1]+1)
+        else:
+            return select
 
     def keys(self):
         return self._data.keys()
 
     def values(self):
         return [self[k] for k in self]
 
     def __iter__(self):
         return iter(self._data)
 
     def __getitem__(self,key):
-        if isinstance(self._selection,slice):
-            return self._data[key][self._selection]
+        if isinstance(self._select,slice):
+            return View.SliceView(self._data[key],self._select)
         else:
-            return View.ListView(self._data[key], self._selection)
+            return View.ListView(self._data[key],self._select)
 
     def __setitem__(self,key,value):
         raise CobaException("A view of the data cannot be modified.")
 
     def __contains__(self,key) -> bool:
         return key in self._data
 
 class Table:
     """A container class for storing tabular data."""
     #Potentially overkill, however, by having our own "simple" table implementation we can provide
     #several useful pieces of functionality out of the box. Additionally, when working with
     #very large experiments pandas can become quite slow while our Table works acceptably.
+
     def __init__(self, data:Union[Mapping, Sequence[Mapping], Sequence[Sequence]] = (), columns: Sequence[str] = (), indexes: Sequence[str]= ()):
 
         self._columns = tuple(columns)
         self._data    = {c:[] for c in columns}
         self.insert(data)
         self._indexes = tuple(indexes)
         self._lohis   = self._calc_lohis()
@@ -138,31 +167,31 @@
         return self._columns
 
     @property
     def indexes(self) -> Sequence[str]:
         return self._indexes
 
     def insert(self, data:Union[Mapping, Sequence[Mapping], Sequence[Sequence]]=()) -> 'Table':
-        data_is_empty              = not data
-        data_is_where_clause_view  = data and isinstance(data,View)
-        data_is_sequence_of_dicts  = data and isinstance(data,collections.abc.Sequence) and isinstance(data[0],collections.abc.Mapping)
-        data_is_mapping_of_columns = data and isinstance(data,collections.abc.Mapping)
+        data_is_empty             = not data
+        data_is_where_clause_view = data and isinstance(data,View)
+        data_is_mapping_of_cols   = data and isinstance(data,collections.abc.Mapping)
+        data_is_sequence_of_dicts = data and isinstance(data,collections.abc.Sequence) and isinstance(data[0],collections.abc.Mapping)
 
         if data_is_empty:
             return self
 
         if data_is_where_clause_view:
             self._data = data
             return self
 
         if data_is_sequence_of_dicts:
             data = {k:[d.get(k) for d in data] for k in set().union(*(d.keys() for d in data))}
-            data_is_mapping_of_columns = True
+            data_is_mapping_of_cols = True
 
-        if data_is_mapping_of_columns:
+        if data_is_mapping_of_cols:
             old,new = set(self._columns), set(data.keys())
             old_len = len(self)
             new_len = 0
 
             for hdr in new-old:
                 self._data[hdr] = list(chain(repeat(None, old_len), data[hdr]))
                 new_len = len(self._data[hdr])
@@ -175,15 +204,15 @@
                 self._data[hdr].extend(repeat(None,new_len-old_len))
 
             self._columns += tuple(sorted(new-old))
 
         else: #data_is_list_of_rows
             assert len(data[0]) == len(self._columns), "The given data rows don't align with the table's headers."
             for hdr,col in zip(self._columns,zip(*data)):
-                self._data[hdr].extend(col)  
+                self._data[hdr].extend(col)
 
         self._indexes = ()
         self._lohis = {}
 
         return self
 
     def index(self, *indx) -> 'Table':
@@ -206,15 +235,15 @@
             self._data[col][:] = map(self._data[col].__getitem__,indexes)
 
         self._indexes = tuple(indx)
         self._lohis = self._calc_lohis()
 
         return self
 
-    def where(self, row_pred:Callable[[Sequence],bool] = None, comparison:Literal['=','<=','<','>','>=','match','in'] = None, **kwargs) -> 'Table':
+    def where(self, row_pred:Callable[[Sequence],bool] = None, comparison:Literal['=','!=','<=','<','>','>=','match','in'] = None, **kwargs) -> 'Table':
         """Filter to specific rows.
 
         Args:
             pred: A predicate that accepts rows and returns true for rows that should be kept.
             kwargs: key value pairs where the key is the column and the value indicates what
                 value a row should have in that column to be kept. Keeping logic depends on
                 the row value type and the kwargs value type. If kwarg value == row value keep
@@ -223,36 +252,41 @@
                 If kwarg value is a string apply a regular expression match to the row value.
         """
 
         if not row_pred and not kwargs:
             return self
 
         if row_pred:
-            selection = list(compress(count(),map(row_pred,self[:])))
-            return Table(View(self._data,selection), self._columns, self._indexes) 
- 
+            selection = list(compress(count(),map(row_pred,self)))
+            return Table(View(self._data,selection), self._columns, self._indexes)
+
         if kwargs:
             selection = []
             for kw,arg in kwargs.items():
                 if kw in self._indexes and comparison != "match" and not callable(kwargs[kw]):
                     for lo,hi in self._lohis[kw]:
                         for l,h in self._compare(lo,hi,self._data[kw],arg,comparison,"bisect"):
                             selection.extend(range(l,h))
                 else:
                     selection.extend(self._compare(0,len(self),self._data[kw],arg,comparison,"foreach"))
 
-            selection=sorted(set(selection))
+            if len(kwargs) > 1: selection=sorted(set(selection))
+
             return Table(View(self._data,selection), self._columns, self._indexes)
 
-    def groupby(self, level:int) -> Iterable['Table']:
+    def groupby(self, level:int) -> Iterable[Tuple[Tuple,'Table']]:
         for l,h in self._lohis[self._indexes[level]]:
-            yield Table(View(self._data, slice(l,h)), self._columns, self._indexes)
+            group = tuple(self._data[hdr][l] for hdr in self._indexes[:level])
+            table = Table(View(self._data, slice(l,h)), self._columns, self._indexes)
+            yield group, table
 
     def copy(self) -> 'Table':
-        return Table(dict(self._data), tuple(self._columns), tuple(self._indexes))
+        #views are immutable so we don't really need to copy them...
+        data_copy = self._data.copy() if isinstance(self._data,dict) else self._data
+        return Table(data_copy, tuple(self._columns), tuple(self._indexes))
 
     def to_pandas(self):
         """Turn the Table into a Pandas data frame."""
 
         PackageChecker.pandas("Table.to_pandas")
         import pandas as pd
 
@@ -267,24 +301,24 @@
             yield {c:self._data[c][i] for c in self._columns}
 
     def __getitem__(self,idx1):
 
         if isinstance(idx1,str):
             return self._data[idx1]
 
-        if isinstance(idx1,slice) and idx1.start is None and idx1.stop is None and idx1.step is None:
-            idx1 = self.columns
+        if isinstance(idx1,slice):
+            return [self._data[col] for col in self._columns[idx1]]
 
         if isinstance(idx1,collections.abc.Collection):
-            return list(zip(*(self._data[col] for col in idx1)))
+            return [self._data[col] for col in idx1]
 
         raise KeyError(idx1)
 
     def __iter__(self) -> Iterator[Sequence[Any]]:
-        return iter(self[:])
+        return iter(zip(*self[:]))
 
     def __str__(self) -> str:
         return str({"Columns": self.columns, "Rows": len(self)})
 
     def __len__(self) -> int:
         return len(self._data[next(iter(self._data))]) if self._data else 0
 
@@ -305,248 +339,205 @@
             indexcol = self._data[k]
             lohis.append([lh for lo,hi in lohis[-1] for lh in self._sub_lohis(lo,hi,indexcol)])
 
         return dict(zip(self._indexes,lohis))
 
     def _sub_lohis(self,lo,hi,col):
         while lo != hi:
-            new_hi = bisect_right(col,col[lo],lo,hi)
+            new_hi = my_bisect_right(col,col[lo],lo,hi)
             yield (lo,new_hi)
             lo = new_hi
 
     def _compare(self,lo,hi,col,arg,comparison,method):
 
-        if method != "bisect" or callable(arg): 
+        if isinstance(arg,dict) and len(arg) == 1:
+            key,value = list(arg.items())[0]
+            if key in ['=','!=','<=','<','>','>=','match','in']:
+                comparison,arg = key,value
+
+        if method != "bisect" or callable(arg):
             col = col[lo:hi]
 
         if callable(arg):
             return list(compress(count(lo),map(arg,col)))
 
         if comparison == "in" or (comparison is None and isinstance(arg,collections.abc.Iterable) and not isinstance(arg,str)):
             if method == "bisect":
-                return [ (bisect_left(col,v,lo,hi),bisect_right(col,v,lo,hi)) for v in arg ]
+                return [ (my_bisect_left(col,v,lo,hi),my_bisect_right(col,v,lo,hi)) for v in sorted(arg) ]
             else:
                 return [ i for i,c in enumerate(col,lo) if c in arg ]
 
         if comparison == "=" or (comparison is None and (not isinstance(arg,collections.abc.Iterable) or isinstance(arg,str))):
             if method == "bisect":
-                return [ (bisect_left(col,arg,lo,hi),bisect_right(col,arg,lo,hi)) ]
+                return [ (my_bisect_left(col,arg,lo,hi),my_bisect_right(col,arg,lo,hi)) ]
             else:
                 return [ i for i,c in enumerate(col,lo) if c == arg ]
 
+        if comparison == "!=":
+            if method == "bisect":
+                return [ (lo,my_bisect_left(col,arg,lo,hi)), (my_bisect_right(col,arg,lo,hi), hi) ]
+            else:
+                return [ i for i,c in enumerate(col,lo) if c != arg ]
+
         if comparison == "<":
             if method == "bisect":
-                return [ (lo,bisect_left(col,arg,lo,hi)) ]
+                return [ (lo,my_bisect_left(col,arg,lo,hi)) ]
             else:
                 return [ i for i,c in enumerate(col,lo) if c < arg ]
 
         if comparison == "<=":
             if method == "bisect":
-                return [ (lo,bisect_right(col,arg,lo,hi)) ]
+                return [ (lo,my_bisect_right(col,arg,lo,hi)) ]
             else:
                 return [ i for i,c in enumerate(col,lo) if c <= arg ]
 
         if comparison == ">=":
             if method == "bisect":
-                return [ (bisect_left(col,arg,lo,hi), hi) ]
+                return [ (my_bisect_left(col,arg,lo,hi), hi) ]
             else:
                 return [ i for i,c in enumerate(col,lo) if c >= arg ]
 
         if comparison == ">":
             if method == "bisect":
-                return [ (bisect_right(col,arg,lo,hi), hi) ]
+                return [ (my_bisect_right(col,arg,lo,hi), hi) ]
             else:
                 return [ i for i,c in enumerate(col,lo) if c > arg ]
 
         if comparison == "match":
             if isinstance(arg,Number) and col and isinstance(col[0],Number):
                 return [ i for i,c in enumerate(col,lo) if c == arg ]
             elif isinstance(arg,Number) and isinstance(col[0],str):
                 _re = re.compile(f'(\D|^){arg}(\D|$)')
                 return [ i for i,c in enumerate(col,lo) if _re.search(c) ]
             elif isinstance(arg,str) and isinstance(col[0],str):
                 _re = re.compile(arg)
                 return [ i for i,c in enumerate(col,lo) if _re.search(c) ]
 
-class TransactionIO_V3(Source['Result'], Sink[Any]):
+class TransactionDecode:
+    def filter(self, transactions:Iterable[str]) -> Iterable[Any]:
 
-    def __init__(self, log_file: Optional[str] = None, minify:bool = True) -> None:
+        transactions = iter(transactions)
+        ver_row = JsonDecode().filter(next(transactions))
 
-        self._log_file = log_file
-        self._minify   = minify
-        self._source   = DiskSource(log_file) if log_file else IterableSource()
-        self._sink     = DiskSink(log_file) if log_file else ListSink(self._source.iterable)
-
-    def write(self, item: Any) -> None:
-        if isinstance(self._sink, ListSink):
-            self._sink.write(self._encode(item))
-        else:
-            if not Path(self._sink._filename).exists():self._sink.write('["version",3]')
-            self._sink.write(JsonEncode(self._minify).filter(self._encode(item)))
+        if ver_row[1] == 4:
+            yield ver_row
+            yield from map(JsonDecode().filter,transactions)
 
-    def read(self) -> 'Result':
-        n_lrns   = None
-        n_envs   = None
-        lrn_rows = {}
-        env_rows = {}
-        int_rows = {}
+class TransactionEncode:
+    def filter(self, transactions: Iterable[Any]) -> Iterable[str]:
 
-        if isinstance(self._source, IterableSource):
-            decoded_source = self._source
-        else:
-            decoded_source = Pipes.join(self._source, Foreach(JsonDecode()))
+        yield JsonEncode().filter(["version",4])
 
-        for trx in decoded_source.read():
+        encoder = JsonEncode()
 
-            if not trx: continue
+        for item in transactions:
+            if item[0] == "T0":
+                yield encoder.filter(['experiment', item[1]])
 
-            if trx[0] == "benchmark":
-                n_lrns = trx[1]["n_learners"]
-                n_envs = trx[1]["n_simulations"]
+            elif item[0] == "T1":
+                yield encoder.filter(["E", item[1], item[2]])
 
-            if trx[0] == "S":
-                env_rows[trx[1]] = trx[2]
+            elif item[0] == "T2":
+                yield encoder.filter(["L", item[1], item[2]])
 
-            if trx[0] == "L":
-                lrn_rows[trx[1]] = trx[2]
+            elif item[0] == "T3":
+                yield encoder.filter(["V", item[1], item[2]])
 
-            if trx[0] == "I":
-                int_rows[tuple(trx[1])] = trx[2]
+            elif item[0] == "T4":
+                rows_T = collections.defaultdict(list)
 
-        return Result(*old_to_new(env_rows, lrn_rows, int_rows), {"n_learners":n_lrns,"n_environments":n_envs})
+                keys = sorted(set().union(*[r.keys() for r in item[2]]))
 
-    def _encode(self,item):
-        if item[0] == "T0":
-            return ['benchmark', {"n_learners":item[1], "n_simulations":item[2]}]
+                for row in item[2]:
+                    for key in keys:
+                        rows_T[key].append(row.get(key,None))
 
-        if item[0] == "T1":
-            return ["L", item[1], item[2]]
+                yield encoder.filter(["I", item[1], { "_packed": rows_T }])
 
-        if item[0] == "T2":
-            return ["S", item[1], item[2]]
+class TransactionResult:
 
-        if item[0] == "T3":
-            rows_T = collections.defaultdict(list)
-
-            for row in item[2]:
-                for col,val in row.items():
-                    rows_T[col].append(val)
-
-            return ["I", item[1], { "_packed": rows_T }]
-
-        return None
-
-class TransactionIO_V4(Source['Result'], Sink[Any]):
-
-    def __init__(self, log_file: Optional[str] = None, minify:bool=True) -> None:
-
-        self._log_file = log_file
-        self._minify   = minify
-        self._source   = DiskSource(log_file) if log_file else IterableSource()
-        self._sink     = DiskSink(log_file)   if log_file else ListSink(self._source.iterable)
-
-    def write(self, item: Any) -> None:
-        if isinstance(self._sink, ListSink):
-            self._sink.write(self._encode(item))
-        else:
-            if not Path(self._sink._filename).exists():self._sink.write('["version",4]')
-            self._sink.write(JsonEncode(self._minify).filter(self._encode(item)))
+    def filter(self, transactions:Iterable[Any]) -> 'Result':
+        env_rows = collections.defaultdict(dict)
+        lrn_rows = collections.defaultdict(dict)
+        val_rows = collections.defaultdict(dict)
+        int_rows = {}
+        exp_dict = {}
 
-    def read(self) -> 'Result':
+        transactions = iter(transactions)
+        version      = next(transactions)[1]
 
-        exp_dict = {}
-        lrn_rows = {}
-        env_rows = {}
-        int_rows = {}
+        if version == 3:
+            raise CobaException("Deprecated transaction format. Please revert to an older version of Coba to read it.")
 
-        if isinstance(self._source, IterableSource):
-            decoded_source = self._source
-        else:
-            decoded_source = Pipes.join(self._source, Foreach(JsonDecode()))
+        if version != 4:
+            raise CobaException(f"Unrecognized transaction format: version equals {version}.")
 
-        for trx in decoded_source.read():
+        for trx in transactions:
 
             if not trx: continue
 
             if trx[0] == "experiment":
                 exp_dict = trx[1]
 
             if trx[0] == "E":
-                env_rows[trx[1]] = trx[2]
+                env_rows[trx[1]].update(trx[2])
 
             if trx[0] == "L":
-                lrn_rows[trx[1]] = trx[2]
+                lrn_rows[trx[1]].update(trx[2])
+
+            if trx[0] == "V":
+                val_rows[trx[1]].update(trx[2])
 
             if trx[0] == "I":
+                if len(trx[1]) ==2: trx[1] = [*trx[1],0]
                 int_rows[tuple(trx[1])] = trx[2]
 
-        return Result(*old_to_new(env_rows, lrn_rows, int_rows), exp_dict)
-
-    def _encode(self,item):
-        if item[0] == "T0":
-            return ['experiment', {"n_learners":item[1], "n_environments":item[2], "description":None} if len(item)==3 else item[1] ]
-
-        if item[0] == "T1":
-            return ["L", item[1], item[2]]
-
-        if item[0] == "T2":
-            return ["E", item[1], item[2]]
-
-        if item[0] == "T3":
-            rows_T = collections.defaultdict(list)
-
-            keys = set().union(*[r.keys() for r in item[2]])
-
-            for row in item[2]:
-                for key in keys:
-                    rows_T[key].append(row.get(key,None))
-
-            return ["I", item[1], { "_packed": rows_T }]
-
-        return None
-
-class TransactionIO(Source['Result'], Sink[Any]):
-
-    def __init__(self, transaction_log: Optional[str] = None) -> None:
+        rwd_col = ['reward'] if any('reward' in v.keys() for v in int_rows.values()) else []
 
-        if not transaction_log or not Path(transaction_log).exists():
-            version = None
-        else:
-            version = JsonDecode().filter(next(DiskSource(transaction_log).read()))[1]
-
-        if version == 3:
-            self._transactionIO = TransactionIO_V3(transaction_log)
-
-        elif version == 4:
-            self._transactionIO = TransactionIO_V4(transaction_log)
-
-        elif version is None:
-            self._transactionIO = TransactionIO_V4(transaction_log)
-
-        else:
-            raise CobaException("We were unable to determine the appropriate Transaction reader for the file.")
-
-    def write(self, transactions: Iterable[Any]) -> None:
-        for transaction in transactions:
-            self._transactionIO.write(transaction)
-
-    def read(self) -> 'Result':
-        return self._transactionIO.read()
-
-class Points(NamedTuple):
-    X    : Sequence[Any]
-    Y    : Sequence[float]
-    XE   : Sequence[float]  = None
-    YE   : Sequence[float]  = None
+        env_table = Table(columns=['environment_id'                                    ]          )
+        lrn_table = Table(columns=[                 'learner_id'                       ]          )
+        val_table = Table(columns=[                              'evaluator_id'        ]          )
+        int_table = Table(columns=['environment_id','learner_id','evaluator_id','index'] + rwd_col)
+
+        env_table.insert([{"environment_id":e,                                 **r} for e,r in env_rows.items()])
+        lrn_table.insert([{                   "learner_id":l,                  **r} for l,r in lrn_rows.items()])
+        val_table.insert([{                                  "evaluator_id":v, **r} for v,r in val_rows.items()])
+
+        for (env_id, lrn_id, val_id), results in int_rows.items():
+            if '_packed' in results and results['_packed']:
+
+                packed = results['_packed']
+                N = len(packed[next(iter(packed))])
+
+                packed['environment_id'] = repeat(env_id,N)
+                packed['learner_id'    ] = repeat(lrn_id,N)
+                packed['evaluator_id'  ] = repeat(val_id,N)
+                packed['index'         ] = range(1,N+1)
+
+                int_table.insert(packed)
+
+        return Result(env_table, lrn_table, val_table, int_table, exp_dict)
+
+@dataclass
+class Points:
+    X    : List[Any]        = field(default_factory=list)
+    Y    : List[float]      = field(default_factory=list)
+    XE   : List[float]      = field(default_factory=list)
+    YE   : List[float]      = field(default_factory=list)
     color: Union[str,int]   = None
     alpha: float            = 1
     label: Optional[str]    = None
     style: Literal['-','.'] = "-"
     zorder:int              = 1
 
+    def add(self, x, y, ye):
+        self.X.append(x)
+        self.Y.append(y)
+        self.YE.append(ye)
+
 class Plotter:
     @abstractmethod
     def plot(self,
         ax,
         lines: Sequence[Points],
         title: str,
         xlabel: str,
@@ -556,15 +547,15 @@
         xticks: bool,
         yticks: bool,
         xrotation: Optional[float],
         yrotation: Optional[float],
         out: Union[None,Literal['screen'],str]) -> None:
         pass
 
-class MatplotlibPlotter(Plotter):
+class MatplotPlotter(Plotter):
 
     def plot(self,
         ax,
         lines: Sequence[Points],
         title: str,
         xlabel: str,
         ylabel: str,
@@ -576,15 +567,15 @@
         yrotation: Optional[float],
         out: Union[None,Literal['screen'],str]
     ) -> None:
 
         xlim = xlim or [None,None]
         ylim = ylim or [None,None]
 
-        PackageChecker.matplotlib('Result.plot_learners')
+        PackageChecker.matplotlib('MatplotPlotter')
         import matplotlib.pyplot as plt
 
         color_cycle = plt.rcParams['axes.prop_cycle'].by_key()['color']
 
         ax: plt.Axes
 
         bad_xlim  = xlim and xlim[0] is not None and xlim[1] is not None and xlim[0] >= xlim[1]
@@ -608,39 +599,39 @@
                     ax = plt.subplot(111) if not isinstance(ax,int) else plt.subplot(ax)
 
             in_lim = lambda v,lim: lim is None or ((lim[0] or -float('inf')) <= v and v <= (lim[1] or float('inf')))
 
             any_label = False
             num_coalesce = lambda x1,x2: x1 if isinstance(x1,(int,float)) else x2
 
-            for X, Y, XE, YE, c, a, l, fmt,z in lines:
+            for X, Y, XE, YE, c, a, l, fmt,z in map(astuple,lines):
 
                 if l: any_label = True
 
                 # we remove values outside of the given lims because matplotlib won't correctly scale otherwise
                 if not YE:
                     XY = [(x,y) for i,x,y in zip(count(),X,Y) if in_lim(num_coalesce(x,i),xlim) and in_lim(num_coalesce(y,i),ylim)]
                     X,Y = map(list,zip(*XY)) if XY else ([],[])
                 else:
                     XYE = [(x,y,e) for i,x,y,e in zip(count(),X,Y,YE) if in_lim(num_coalesce(x,i),xlim) and in_lim(num_coalesce(y,i),ylim)]
                     X,Y,YE = map(list,zip(*XYE)) if XYE else ([],[],[])
 
                 if isinstance(c,int): c = color_cycle[c%len(color_cycle)]
 
-                not_err_bar = lambda E: not E or all([e is None for e in E])
+                not_err_bar = lambda E: not E or all(not e for e in E)
 
                 if X and Y:
                     if all(map(not_err_bar,[XE,YE])):
                         ax.plot(X, Y, fmt,  color=c, alpha=a, label=l,zorder=z)
                     else:
                         XE = None if not_err_bar(XE) else list(zip(*XE)) if isinstance(XE[0],tuple) else XE
                         YE = None if not_err_bar(YE) else list(zip(*YE)) if isinstance(YE[0],tuple) else YE
-                        error_every = max(int(len(X)*0.05),1) if fmt == "-" else 1
+                        errorevery = 1 if fmt == "-" else 1
                         elinewidth = 0.5 if 'elinewidth' not in CobaContext.store else CobaContext.store['elinewidth']
-                        ax.errorbar(X, Y, YE, XE, fmt, elinewidth=elinewidth, errorevery=error_every, color=c, alpha=a, label=l,zorder=z)
+                        ax.errorbar(X, Y, YE, XE, fmt, elinewidth=elinewidth, errorevery=errorevery, color=c, alpha=a, label=l,zorder=z)
 
             if xrotation is not None:
                 plt.xticks(rotation=xrotation)
 
             if yrotation is not None:
                 plt.yticks(rotation=yrotation)
 
@@ -681,142 +672,41 @@
                 plt.show()
                 plt.close()
 
             if out=="screen":
                 plt.show()
                 plt.close()
 
-class FilterPlottingData:
-
-    def filter(self, unfinished:'Result', x:Sequence[str], y:str) -> Table:
-
-        if len(unfinished.interactions) == 0: raise CobaException("This result doesn't contain any evaluation data to plot.")
-        if y not in unfinished.interactions.columns: raise CobaException(f"{y} is not available in the environment. Plotting has been stopped.")
-
-        finished = unfinished.filter_fin('min' if x == ['index'] else None)
-
-        if len(finished.learners) == 0:
-            raise CobaException("This result does not contain an environment that has been finished for every learner. Plotting has been stopped.")
-
-        if len(finished.environments) != len(unfinished.environments):
-            CobaContext.logger.log("Environments not present for all learners have been excluded. To supress this call filter_fin() before plotting.")
-
-        if len(set(map(len,unfinished.interactions.groupby(2)))) > 1 and x == ['index']:
-            CobaContext.logger.log("This result contains environments of different lengths. The plot only includes interactions up to the shortest environment. To supress this warning in the future call <result>.filter_fin(n_interactions) before plotting.")
-
-        return finished.interactions
-
-class SmoothPlottingData:
-
-    def filter(self, interactions:Table, y:str, span:Optional[int]) -> Sequence[Mapping[str,Any]]:
-
-        try:
-            out = []
-            for table in interactions.groupby(2):
-                out.append({"environment_id":table['environment_id'][0], "learner_id":table['learner_id'][0], y:moving_average(table[y],span)})
-            return out
-        except:#pragma: no cover
-            out = []
-            for g, Y in groupby(interactions[["environment_id","learner_id", y]], itemgetter(slice(2))):
-                out.append({"environment_id":g[0], "learner_id":g[1], y:moving_average(list(Y),span)})
-            return out
-
-class ContrastPlottingData:
-
-    def filter(self, rows:Sequence[Mapping[str,Any]], y:str, mode:Union[Literal["diff","prob",'scat'],Callable[[float,float],float]], learner_id1:int) -> Sequence[Mapping[str,Any]]:
-
-        sort_key  = lambda row: (row['environment_id'], 0 if row['learner_id']==learner_id1 else 1)
-        group_key = lambda row: row['environment_id']
-
-        if mode == "prob":
-            contraster = lambda Y1,Y2: list(map(int,map(gt,Y1,Y2)))
-        elif mode == "diff":
-            contraster = lambda Y1,Y2: list(map(sub,Y1,Y2))
-        elif mode =="scat":
-            contraster = lambda Y1,Y2: list(zip(Y1,Y2))
-        else:
-            contraster = lambda Y1,Y2: list(map(mode,Y1,Y2))
-
-        contrast = lambda env_id, pair: {'environment_id': env_id, y: contraster(pair[0][y],pair[1][y]) }
-
-        return [ contrast(env_id,list(pair)) for env_id, pair in groupby(sorted(rows,key=sort_key),key=group_key) ]
-
-class TransformToXYE:
-
-    def filter(self,
-        rows: Sequence[Mapping[str,Any]],
-        envs: Mapping[int,Mapping[str,Any]],
-        x:Sequence[str],
-        y:str,
-        err:Union[str,None,PointAndInterval]) -> Sequence[Tuple[Any,float,Union[None,float,Tuple[float,float]]]]:
-
-        if err == 'sd':
-            YE = lambda z: (mean(z), stdev(z))
-        elif err == 'se':
-            YE = StandardErrorOfMean(1.96).calculate #z-score for .975 area to the left and right
-        elif err == "bs":
-            YE = BootstrapConfidenceInterval(.95, mean).calculate
-        elif err == "bi":
-            YE = BinomialConfidenceInterval('wilson').calculate
-        elif isinstance(err,PointAndInterval):
-            YE = err.calculate
-        else:
-            YE = lambda z: (mean(z) if len(z) > 1 else z[0], None)
-
-        iters = [ iter(row[y]) for row in rows ]
-        first_val = next(iters[0])
-        iters[0] = chain([first_val],iters[0])
-
-        is_scatter = isinstance(first_val,(list,tuple))
-
-        if x == ['index']:
-            Z = zip(*iters)
-            X = count(1)
-
-            if not is_scatter:
-                points = [(x,None)+YE(z) for x,z in zip(X,Z) ]
-            else:
-                points = [YE(z1)+YE(z2) for _,z in zip(X,Z) for z1,z2 in [tuple(zip(*z))]]
-        else:
-            XZ = collections.defaultdict(list)
-
-            make_x = lambda eid: eid if list(x) == ['environment_id'] else envs[eid].get(x[0]) if len(x) == 1 else tuple(envs[eid].get(k) for k in x)
-            for row,I in zip(rows,iters):
-                XZ[str(make_x(row["environment_id"]))].append(list(I)[-1])
-
-            if not is_scatter:
-                points = [(x,None)+YE(z) for x,z in XZ.items()]
-            else:
-                points = [YE(z1)+YE(z2) for _,z in XZ.items() for z1,z2 in [tuple(zip(*z))]]
-
-        return [ (x,y,xe,ye) for x,xe,y,ye in points ]
-
 class Result:
     """A class representing the result of an Experiment."""
 
     @staticmethod
-    def from_file(filename: str) -> 'Result':
+    def from_save(filename: str) -> 'Result':
         """Create a Result from a transaction file."""
-
         if not Path(filename).exists():
             raise CobaException("We were unable to find the given Result file.")
 
-        return TransactionIO(filename).read()
+        return Pipes.join(DiskSource(filename),TransactionDecode(),TransactionResult()).read()
 
     @staticmethod
-    def from_logged_envs(environments: Iterable[Environment],include_probability:bool=False):
+    def from_file(filename: str) -> 'Result':
+        """Create a Result from a transaction file."""
+        return Result.from_save(filename)
 
-        env_param_list = []
-        lrn_param_list = []
-        env_param_dict = {}
-        lrn_param_dict = {}
+    @staticmethod
+    def from_logged_envs(environments: Iterable[Environment], include_prob:bool=False):
 
-        env_rows = {}
-        lrn_rows = {}
-        int_rows = {}
+        seen_env = set()
+        seen_lrn = set()
+        seen_val = set()
+
+        env_table = Table(columns=['environment_id'                                             ])
+        lrn_table = Table(columns=[                 'learner_id'                                ])
+        val_table = Table(columns=[                              'evaluator_id'                 ])
+        int_table = Table(columns=['environment_id','learner_id','evaluator_id','index','reward'])
 
         def determine_id(param,param_list,param_dict):
             try:
                 key = frozenset(param.items())
                 if key not in param_dict:
                     param_dict[key] = len(param_list)
                     param_list.append(param)
@@ -824,73 +714,128 @@
             except:
                 try:
                     return param_list.index(param)
                 except:
                     param_list.append(param)
                     return len(param_list)-1
 
+        def determine_env_id(env_param,env_param_list=[],env_param_dict={}):
+            return determine_id(env_param,env_param_list,env_param_dict)
+
+        def determine_lrn_id(lrn_param,lrn_param_list=[],lrn_param_dict={}):
+            return determine_id(lrn_param,lrn_param_list,lrn_param_dict)
+
+        def determine_val_id(val_param,val_param_list=[],val_param_dict={}):
+            return determine_id(val_param,val_param_list,val_param_dict)
+
         my_mean = lambda x: sum(x)/len(x)
 
         for env in environments:
 
             first, interactions = peek_first(env.read())
 
             if not env.params.get('logged'): continue
             if not interactions: continue
 
             is_batched = isinstance(first['reward'],(Batch,list,tuple))
+
             env_param = dict(env.params)
             lrn_param = env_param.pop('learner')
+            val_param = env_param.pop('evaluator',{'eval_type':'unknown'})
 
-            env_id = determine_id(env_param,env_param_list,env_param_dict)
-            lrn_id = determine_id(lrn_param,lrn_param_list,lrn_param_dict)
-
-            if env_id not in env_rows: env_rows[env_id] = env_param
-            if lrn_id not in lrn_rows: lrn_rows[lrn_id] = lrn_param
+            env_id = determine_env_id(env_param)
+            lrn_id = determine_lrn_id(lrn_param)
+            val_id = determine_val_id(val_param)
+
+            if env_id not in seen_env:
+                seen_env.add(env_id)
+                env_table.insert([{'environment_id':env_id, **env_param}])
+
+            if lrn_id not in seen_lrn:
+                seen_lrn.add(lrn_id)
+                lrn_table.insert([{'learner_id':lrn_id, **lrn_param}])
+
+            if val_id not in seen_val:
+                seen_val.add(val_id)
+                val_table.insert([{'evaluator_id':val_id, **val_param}])
 
             keys = first.keys() - {'context', 'actions', 'rewards'}
-            if not include_probability: keys -= {'probability'}
-
-            _packed = {k:[] for k in keys}
-            results = {"_packed": _packed}
-
-            if is_batched:
-                for interaction in interactions:
-                    for k in keys:
-                        _packed[k].append(my_mean(interaction[k]))
-            else:
-                for interaction in interactions:
-                    for k in keys:
-                        _packed[k].append(interaction[k])
-
-            int_rows[(env_id,lrn_id)]= results
+            if not include_prob: keys -= {'probability'}
 
-        return Result(*old_to_new(env_rows,lrn_rows,int_rows))
+            int_cols = [[] for _ in keys]
+            for interaction in interactions:
+                for k,c in zip(keys,int_cols):
+                    c.append(my_mean(interaction[k]) if is_batched else interaction[k])
+
+            int_count = len(int_cols[0])
+            int_maps = {
+                'environment_id': [env_id]*int_count,
+                'learner_id'    : [lrn_id]*int_count,
+                'evaluator_id'  : [val_id]*int_count,
+                'index'         : list(range(1,int_count+1))
+            }
+            int_maps.update(zip(keys,int_cols))
+            int_table.insert(int_maps)
+
+        return Result(env_table, lrn_table, val_table, int_table, {})
+
+    @overload
+    def __init__(self) -> None:
+        ...
 
+    @overload
     def __init__(self,
-        env_rows: Union[Sequence,Table] = Table(),
-        lrn_rows: Union[Sequence,Table] = Table(),
-        int_rows: Union[Sequence,Table] = Table(),
-        exp_dict: Mapping  = {}) -> None:
+        env_rows: Union[Sequence,Table,None],
+        lrn_rows: Union[Sequence,Table,None],
+        val_rows: Union[Sequence,Table,None],
+        int_rows: Union[Sequence,Table,None],
+        exp_dict: Mapping = {}) -> None:
+        ...
+
+    def __init__(self,*args) -> None:
         """Instantiate a Result class.
 
         This constructor should never be called directly. Instead a Result file should be created
         from an Experiment and the result file should be loaded via Result.from_file(filename).
         """
-        self.experiment = exp_dict
+        if len(args) > 0:
+            env_rows,lrn_rows,val_rows,int_rows = args[:4]
+        else:
+            env_rows,lrn_rows,val_rows,int_rows = tuple([None]*4)
+
+        env_rows = env_rows if env_rows is not None else Table(columns=['environment_id'                                    ])
+        lrn_rows = lrn_rows if lrn_rows is not None else Table(columns=[                 'learner_id'                       ])
+        val_rows = val_rows if val_rows is not None else Table(columns=[                              'evaluator_id'        ])
+        int_rows = int_rows if int_rows is not None else Table(columns=['environment_id','learner_id','evaluator_id','index'])
+
+        self.experiment = args[4] if len(args) == 5 else {}
 
         self._environments = env_rows if isinstance(env_rows,Table) else Table(columns=env_rows[0]).insert(env_rows[1:])
         self._learners     = lrn_rows if isinstance(lrn_rows,Table) else Table(columns=lrn_rows[0]).insert(lrn_rows[1:])
+        self._evaluators   = val_rows if isinstance(val_rows,Table) else Table(columns=val_rows[0]).insert(val_rows[1:])
         self._interactions = int_rows if isinstance(int_rows,Table) else Table(columns=int_rows[0]).insert(int_rows[1:])
 
-        self._environments.index('environment_id'                     )
-        self._learners    .index(                 'learner_id'        )
-        self._interactions.index('environment_id','learner_id','index')
+        self._environments.index('environment_id'                                    )
+        self._learners    .index(                 'learner_id'                       )
+        self._evaluators  .index(                              'evaluator_id'        )
+        self._interactions.index('environment_id','learner_id','evaluator_id','index')
+
+        self._env_cache = {d['environment_id']:d for d in self._environments.to_dicts()}
+        self._lrn_cache = {d['learner_id'    ]:d for d in self._learners    .to_dicts()}
+        self._val_cache = {d['evaluator_id'  ]:d for d in self._evaluators  .to_dicts()}
+
+        for value in self._lrn_cache.values():
+            lrn_id = value['learner_id']
+            family = value.get('family',lrn_id)
+            params = [f'{k}={v}' for k,v in value.items() if k and k not in ['family','learner_id'] and v is not None ]
+            params = f"({','.join(params)})" if params else ''
+            value['full_name'] = f"{lrn_id}. {family}{params}"
+            value['full_name_sans_lrn_id'] = f"{family}{params}"
 
-        self._plotter = MatplotlibPlotter()
+        self._plotter = MatplotPlotter()
 
     @property
     def learners(self) -> Table:
         """The collection of learners used in the Experiment.
 
         The primary key of this table is learner_id.
         """
@@ -901,339 +846,661 @@
         """The collection of environments used in the Experiment.
 
         The primary key of this table is environment_id.
         """
         return self._environments
 
     @property
+    def evaluators(self) -> Table:
+        """The collection of evaluators used in the Experiment.
+
+        The primary key of this table is evaluator_id.
+        """
+        return self._evaluators
+
+    @property
     def interactions(self) -> Table:
-        """The collection of interactions that learners chose actions for in the Experiment.
+        """The collection of interactions evaluated by evaluators in the Experiment.
 
-        The primary key of this Table is (index, environment_id, learner_id). It should be noted that the InteractionTable
-        has an additional property, to_progressive_pandas() which calculates the expanding moving average or exponential
-        moving average for interactions ordered by index and grouped by environment_id and learner_id.
+        The primary key of this Table is (environment_id, learner_id, evaluator_id, index).
         """
         return self._interactions
 
     def set_plotter(self, plotter: Plotter) -> None:
         """Manually set the underlying plotting tool. By default matplotlib is used though this can be changed."""
         self._plotter = plotter
 
     def copy(self) -> 'Result':
         """Create a copy of Result."""
-        return Result(self.environments.copy(), self.learners.copy(), self.interactions.copy(), dict(self.experiment))
+        return Result(self.environments.copy(), self.learners.copy(), self.evaluators.copy(), self.interactions.copy(), dict(self.experiment))
 
-    def filter_fin(self, n_interactions: Union[int,Literal['min']] = None) -> 'Result':
-        """Filter the result to only contain data about environments with all learners and interactions.
+    def filter_fin(self,
+        n: Union[int,Literal['min']] = None,
+        l: Union[str, Sequence[str]] = None,
+        p: Union[str, Sequence[str]] = None) -> 'Result':
+        """Filter the results down to even outcomes so that plotted results will be meaningful.
 
         Args:
-            n_interactions: The number of interactions at which an environment is considered complete.
+            n: The number of interactions a specific evaluation must have (None indicates no constraint).
+            l: The level at which we wish to compare evalation outcomes.
+            p: The pairs that must exist across all comparison levels in order to be included.
         """
-        interactions = self.interactions
-        learners     = self.learners
-        environments = self.environments
-
-        env_lens, env_cnts = env_len_and_cnt(interactions)
-        n_interactions = min(env_lens.values()) if n_interactions == "min" else n_interactions
-
-        def has_all(env_id):
-            return env_cnts.get(env_id,-1) == len(learners)
 
-        def has_min(env_id):
-            return n_interactions == None or env_lens.get(env_id,-1) >= n_interactions
+        result = self._filter_fin(n,l,p)
 
-        complete_ids = set([env_id for env_id in environments["environment_id"] if has_all(env_id) and has_min(env_id)])
-
-        if complete_ids != set(env_lens.keys()):
-            environments = environments.where(environment_id=complete_ids)
-            interactions = interactions.where(environment_id=complete_ids)
-
-        if n_interactions and {n_interactions} != set(env_lens.values()):
-            interactions = interactions.where(index=n_interactions,comparison="<=")
-
-        if len(environments) == 0:
-            learners = learners.where(lambda _:False)
-            CobaContext.logger.log(f"There was no environment which was finished for every learner.")
+        if len(result.interactions) == 0:
+            CobaContext.logger.log(f"There was no {p} which was finished for every {l}.")
 
-        return Result(environments, learners, interactions, self.experiment)
+        return result
 
     def filter_env(self, pred:Callable[[Mapping[str,Any]],bool] = None, **kwargs: Any) -> 'Result':
         """Filter the result to only contain data about specific environments.
 
         Args:
             pred: A predicate that returns true for learner dictionaries that should be kept.
             **kwargs: key-value pairs to filter on. To see filtering options see Table.filter.
         """
 
         if len(self.environments) == 0: return self
 
         environments = self.environments.where(pred, **kwargs)
         learners     = self.learners
+        evaluators   = self.evaluators
         interactions = self.interactions
 
-        if len(environments) != len(self.environments):
-            interactions = interactions.where(environment_id=set(environments["environment_id"]))
-            learners     = learners    .where(learner_id    =set(interactions["learner_id"]))
+        if len(environments) == len(self.environments):
+            return self
 
         if len(environments) == 0:
             CobaContext.logger.log(f"No environments matched the given filter.")
 
-        return Result(environments,learners,interactions,self.experiment)
+        interactions = interactions.where(environment_id=set(environments["environment_id"]))
+        learners     = learners    .where(learner_id    =set(interactions["learner_id"]))
+        evaluators   = evaluators  .where(evaluator_id  =set(interactions["evaluator_id"]))
+
+        return Result(environments,learners,evaluators,interactions,self.experiment)
 
     def filter_lrn(self, pred:Callable[[Mapping[str,Any]],bool] = None, **kwargs: Any) -> 'Result':
         """Filter the result to only contain data about specific learners.
 
         Args:
             pred: A predicate that returns true for learner dictionaries that should be kept.
             **kwargs: key-value pairs to filter on. To see filtering options see Table.filter.
         """
         if len(self.learners) == 0: return self
 
         environments = self.environments
         learners     = self.learners.where(pred, **kwargs)
+        evaluators   = self.evaluators
         interactions = self.interactions
 
-        if len(learners) != len(self.learners):
-            interactions = self.interactions.where(learner_id    =set(learners["learner_id"]))
-            environments = self.environments.where(environment_id=set(interactions["environment_id"]))
+        if len(learners) == len(self.learners):
+            return self
 
         if len(learners) == 0:
             CobaContext.logger.log(f"No learners matched the given filter.")
 
-        return Result(environments,learners,interactions)
+        interactions = interactions.where(learner_id    =set(learners["learner_id"]))
+        environments = environments.where(environment_id=set(interactions["environment_id"]))
+        evaluators   = evaluators  .where(evaluator_id  =set(interactions["evaluator_id"]))
 
-    def plot_contrast(self,
-        learner_id1: int,
-        learner_id2: int,
-        x          : Union[str, Sequence[str]] = "environment_id",
-        y          : str = "reward",
-        mode       : Union[Literal["diff","prob",'scat'],Callable[[float,float],float]] = "diff",
-        span       : int = None,
-        err        : Union[Literal['se','sd','bs'], None, PointAndInterval] = None,
-        labels     : Sequence[str] = None,
-        colors     : Sequence[str] = None,
-        xlim       : Tuple[Optional[Number],Optional[Number]] = None,
-        ylim       : Tuple[Optional[Number],Optional[Number]] = None,
-        xticks     : bool = True,
-        yticks     : bool = True,
-        reverse    : bool = False,
-        out        : Union[None,Literal['screen'],str] = 'screen',
+        return Result(environments,learners,evaluators,interactions)
+
+    def filter_val(self, pred:Callable[[Mapping[str,Any]],bool] = None, **kwargs: Any) -> 'Result':
+        """Filter the result to only contain data about specific evaluators.
+
+        Args:
+            pred: A predicate that returns true for learner dictionaries that should be kept.
+            **kwargs: key-value pairs to filter on. To see filtering options see Table.filter.
+        """
+        if len(self.learners) == 0: return self
+
+        environments = self.environments
+        learners     = self.learners
+        evaluators   = self.evaluators.where(pred, **kwargs)
+        interactions = self.interactions
+
+        if len(evaluators) == len(self.evaluators):
+            return self
+
+        if len(evaluators) == 0:
+            CobaContext.logger.log(f"No evaluators matched the given filter.")
+
+        interactions = interactions.where(evaluator_id  =set(evaluators['evaluator_id']))
+        environments = environments.where(environment_id=set(interactions["environment_id"]))
+        learners     = learners    .where(learner_id    =set(interactions["learner_id"]))
+
+        return Result(environments,learners,evaluators,interactions)
+
+    def where(self, **kwargs) -> 'Result':
+
+        env_kwargs = {}
+        lrn_kwargs = {}
+        val_kwargs = {}
+
+        for key,arg in kwargs.items():
+            if key in self.environments.columns:
+                env_kwargs[key] = arg
+            elif key in self.learners.columns:
+                lrn_kwargs[key] = arg
+            else:
+                val_kwargs[key] = arg
+
+        out = self
+
+        if env_kwargs: out = out.filter_env(**env_kwargs)
+        if lrn_kwargs: out = out.filter_lrn(**lrn_kwargs)
+        if val_kwargs: out = out.filter_val(**val_kwargs)
+
+        return out
+
+    def plot_learners(self,
+        x       : Union[str, Sequence[str]] = 'index',
+        y       : str = "reward",
+        l       : Union[str, Sequence[str]] = 'full_name',
+        p       : Union[str, Sequence[str]] = 'environment_id',
+        span    : int = None,
+        err     : Union[Literal['se','sd','bs','bi'], None, PointAndInterval] = None,
+        errevery: int = None,
+        labels  : Sequence[str] = None,
+        colors  : Union[int,Sequence[Union[str,int]]] = None,
+        xlim    : Tuple[Optional[Number],Optional[Number]] = None,
+        ylim    : Tuple[Optional[Number],Optional[Number]] = None,
+        xticks  : bool = True,
+        yticks  : bool = True,
+        top_n   : int = None,
+        out     : Union[None,Literal['screen'],str] = 'screen',
         ax = None) -> None:
-        """Plot a direct contrast of the performance for two learners.
+        """Plot the performance of multiple learners on multiple environments. It gives a sense of the expected
+        performance for different learners across independent environments. This plot is valuable in gaining
+        insight into how various learners perform in comparison to one another.
 
         Args:
-            learner_id1: The first learner to plot in the contrast.
-            learner_id2: The second learner to plot in the contrast.
-            x: The value to plot on the x-axis. This can either be index or environment columns to group by.
+            x: The values to plot on the x-axis.
             y: The value to plot on the y-axis.
-            mode: The kind of contrast plot to make: diff plots the pairwise difference, prob plots the the probability
-                of learner_id1 beating learner_id2, and scatter plots learner_id1 on x-axis and learner_id2 on y axis.
+            l: The values to plot in the legend.
+            p: The pairs that must exist across all items in the legend in order to be included.
             span: The number of y values to smooth together when reporting y. If this is None then the average of all y
                 values up to current is shown otherwise a moving average with window size of span (the window will be
                 smaller than span initially).
             err: This determines what kind of error bars to plot (if any). If `None` then no bars are plotted, if 'se'
                 the standard error is shown, and if 'sd' the standard deviation is shown.
+            errevery: This determines the frequency of errorbars. If `None` they appear 5% of the time.
             labels: The legend labels to use in the plot. These should be in order of the actual legend labels.
             colors: The colors used to plot the learners plot.
             xlim: Define the x-axis limits to plot. If `None` the x-axis limits will be inferred.
             ylim: Define the y-axis limits to plot. If `None` the y-axis limits will be inferred.
             xticks: Whether the x-axis labels should be drawn.
             yticks: Whether the y-axis labels should be drawn.
-            reverse: Whether to reverse order when counting winners and losers.
+            top_n: Only plot the top_n learners. If `None` all learners will be plotted. If negative the bottom will be plotted.
             out: Indicate where the plot should be sent to after plotting is finished.
             ax: Provide an optional axes that the plot will be drawn to. If not provided a new figure/axes is created.
         """
         try:
             xlim = xlim or [None,None]
             ylim = ylim or [None,None]
 
-            x = [x] if isinstance(x,str) else list(x)
-            self._validate_parameters(x)
-
-            if x == ['index']:
-                raise CobaException("plot_contrast does not currently support contrasting by `index`.")
-
-            rows = FilterPlottingData().filter(self.filter_lrn(learner_id=[learner_id1, learner_id2]), x, y)
-            rows = SmoothPlottingData().filter(rows, y, span)
-            rows = ContrastPlottingData().filter(rows, y, mode, learner_id1)
-
-            envs = self.environments
-            XYE = TransformToXYE().filter(rows, { row[0]:dict(zip(envs.columns,row)) for row in envs }, x, y, err)
-
-            if x != ['index']:
-                XYE = sorted(XYE, key=lambda xye: xye[1], reverse=reverse)
-
-            bound = .5 if mode == "prob" else 0
-
-            win,tie,loss = [],[],[]
-            for _x,_y,_xe,_ye in XYE:
-                o = 1 if not reverse else -1
-
-                xl,xu = (0,0) if _xe is None else (_xe,_xe) if isinstance(_xe,Number) else _xe
-                yl,yu = (0,0) if _ye is None else (_ye,_ye) if isinstance(_ye,Number) else _ye
-
-                if mode != 'scat':
-                    (win if _y-yl > o*bound else loss if _y+yu < o*bound else tie).append((_x,_y,_xe,_ye))
-                else:
-                    (win if _x-xl>o*(_y+yu) else loss if _y-yl> o*(_x+xu) else tie).append((_x,_y,_xe,_ye))
+            if isinstance(labels,str): labels = [labels]
 
-            colors = (colors or []) + [0,1,2]
-            labels = (labels or []) + [self._full_name(learner_id1), self._full_name(learner_id2)]
+            plottable = self._plottable(x,y,l,p)
+            n_interactions = len(next(plottable.interactions.groupby(3))[1])
 
-            fmt = "-" if x == ['index'] else "."
+            errevery = errevery or max(int(n_interactions*0.05),1) if x == 'index' else 1
+            style    = "-" if x == 'index' else "."
+            err      = plottable._confidence(err, errevery)
+            x_prep   = str if x != 'index' else (lambda _x: _x)
+
+            lines: List[Points] = []
+            for _l, group in groupby(plottable._indexed_ys(l,x,y=y,span=span),key=itemgetter(0)):
+
+                color = plottable._get_color(colors,   len(lines))
+                label = plottable._get_label(labels,_l,len(lines))
+                group = map(itemgetter(slice(1,None)),group)
+                lines.append(Points(style=style,color=color,label=label))
+
+                for _xi, (_x, group) in enumerate(groupby(group, key=itemgetter(0))):
+                    Y = [g[-1] for g in group]
+                    lines[-1].add(x_prep(_x), *err(Y, _xi))
+
+            lines  = sorted(lines, key=lambda line: line.Y[-1], reverse=True)
+            labels = [l.label or str(l.label) for l in lines]
+            colors = [l.color                 for l in lines]
+            xlabel = "Interaction" if x=='index' else x[0] if len(x) == 1 else x
+            ylabel = y.capitalize().replace("_pct"," Percent")
 
-            plots = []
+            y_location = "Total" if x != 'index' else ""
+            y_avg_type = ("Instant" if span == 1 else f"Span {span}" if span else "Progressive")
+            y_samples  = f"({len(Y)} Environments)"
+            title      = ' '.join(filter(None,[y_location, y_avg_type, ylabel, y_samples]))
 
-            if not reverse:
-                if loss: plots.append(Points(*zip(*loss), colors[0], 1, labels[1] + " " + f"({len(loss)})", fmt))
-                if tie : plots.append(Points(*zip(*tie) , colors[1], 1, 'Tie'     + " " + f"({len(tie )})", fmt))
-                if win : plots.append(Points(*zip(*win) , colors[2], 1, labels[0] + " " + f"({len(win )})", fmt))
-            else:
-                if win : plots.append(Points(*zip(*win) , colors[2], 1, labels[0] + " " + f"({len(win )})", fmt))
-                if tie : plots.append(Points(*zip(*tie) , colors[1], 1, 'Tie'     + " " + f"({len(tie )})", fmt))
-                if loss: plots.append(Points(*zip(*loss), colors[0], 1, labels[1] + " " + f"({len(loss)})", fmt))
-
-            if mode != 'scat':
-                leftmost_x  = (loss+tie+win)[ 0][0] if not reverse else (win+tie+loss)[ 0][0]
-                rightmost_x = (loss+tie+win)[-1][0] if not reverse else (win+tie+loss)[-1][0]
-                plots.append(Points((leftmost_x,rightmost_x),(bound,bound), None, None , "#888", 1, None, '-',.5))
-            else:
-                m = max([p[0] for p in (loss+tie+win)]+[p[1] for p in (loss+tie+win)]+[1])
-                plots.append(Points((0,m),(0,m), None, None , "#888", 1, None, '-',.5))
-
-            xrotation = 90 if x != ['index'] and len(XYE)>5 else 0
+            xrotation = 90 if x != 'index' and len(lines[0].X)>5 else 0
             yrotation = 0
 
-            if mode != "scat":
-                xlabel = "Interaction" if x==['index'] else x[0] if len(x) == 1 else x
-                ylabel = f"{labels[0]} - {labels[1]}" if mode=="diff" else f"P({labels[0]} > {labels[1]})"
-            else:
-                xlabel = y
-                ylabel = y
+            if top_n:
+                if abs(top_n) > len(lines): top_n = len(lines)*abs(top_n)/top_n
+                if top_n > 0: lines = [replace(l,color=plottable._get_color(colors,i),label=plottable._get_label(labels,l.label,i)) for i,l in enumerate(lines[:top_n],0    ) ]
+                if top_n < 0: lines = [replace(l,color=plottable._get_color(colors,i),label=plottable._get_label(labels,l.label,i)) for i,l in enumerate(lines[top_n:],top_n) ]
 
-            title = f"{ylabel} ({len(rows) if x==['index'] else len(XYE)} Environments)"
+            self._plotter.plot(ax, lines, title, xlabel, ylabel, xlim, ylim, xticks, yticks, xrotation, yrotation, out)
 
-            self._plotter.plot(ax, plots, title, xlabel, ylabel, xlim, ylim, xticks, yticks, xrotation, yrotation, out)
         except CobaException as e:
             CobaContext.logger.log(str(e))
 
-    def plot_learners(self,
-        x     : Union[str,Sequence[str]] = "index",
-        y     : str = "reward",
-        span  : int = None,
-        err   : Union[Literal['se','sd','bs'], None, PointAndInterval] = None,
-        labels: Sequence[str] = None,
-        colors: Union[int,Sequence[Union[str,int]]] = None,
-        xlim  : Tuple[Optional[Number],Optional[Number]] = None,
-        ylim  : Tuple[Optional[Number],Optional[Number]] = None,
-        xticks: bool = True,
-        yticks: bool = True,
-        top_n: int = None,
-        out   : Union[None,Literal['screen'],str] = 'screen',
+    def plot_contrast(self,
+        l1      : Any,
+        l2      : Any,
+        x       : Union[str, Sequence[str]] = "environment_id",
+        y       : str = "reward",
+        l       : Union[str, Sequence[str]] = 'learner_id',
+        p       : Union[str, Sequence[str]] = 'environment_id',
+        mode    : Union[Literal["diff","prob"], Callable[[float,float],float]] = "diff",
+        span    : int = None,
+        err     : Union[Literal['se','sd','bs','bi'], None, PointAndInterval] = None,
+        errevery: int = None,
+        labels  : Sequence[str] = None,
+        colors  : Sequence[str] = None,
+        xlim    : Tuple[Optional[Number],Optional[Number]] = None,
+        ylim    : Tuple[Optional[Number],Optional[Number]] = None,
+        xticks  : bool = True,
+        yticks  : bool = True,
+        boundary: bool = True,
+        legend  : bool = True,
+        out     : Union[None,Literal['screen'],str] = 'screen',
         ax = None) -> None:
-        """Plot the performance of multiple learners on multiple environments. It gives a sense of the expected
-            performance for different learners across independent environments. This plot is valuable in gaining
-            insight into how various learners perform in comparison to one another.
+        """Plot a direct contrast of the performance for two learners.
 
         Args:
+            l1: The first set of parameter values we want to contrast.
+            l2: The second set of parameter values we want to contrast.
             x: The value to plot on the x-axis. This can either be index or environment columns to group by.
             y: The value to plot on the y-axis.
+            l: The level at which we want to contrast.
+            p: The pairs that must exist across all comparison levels in order to be included.
+            mode: The kind of contrast plot to make: diff plots the pairwise difference, prob plots the the probability
+                of learner_id1 beating learner_id2, and scatter plots learner_id1 on x-axis and learner_id2 on y axis.
             span: The number of y values to smooth together when reporting y. If this is None then the average of all y
                 values up to current is shown otherwise a moving average with window size of span (the window will be
                 smaller than span initially).
             err: This determines what kind of error bars to plot (if any). If `None` then no bars are plotted, if 'se'
                 the standard error is shown, and if 'sd' the standard deviation is shown.
+            errevery: This determines the frequency of errorbars. If `None` they appear 5% of the time.
             labels: The legend labels to use in the plot. These should be in order of the actual legend labels.
             colors: The colors used to plot the learners plot.
             xlim: Define the x-axis limits to plot. If `None` the x-axis limits will be inferred.
             ylim: Define the y-axis limits to plot. If `None` the y-axis limits will be inferred.
             xticks: Whether the x-axis labels should be drawn.
             yticks: Whether the y-axis labels should be drawn.
-            top_n: Only plot the top_n learners. If `None` all learners will be plotted. If negative the bottom will be plotted.
+            boundary: Whether we want to plot the boundary line between which set is the best performing.
             out: Indicate where the plot should be sent to after plotting is finished.
             ax: Provide an optional axes that the plot will be drawn to. If not provided a new figure/axes is created.
         """
+
         try:
             xlim = xlim or [None,None]
             ylim = ylim or [None,None]
 
-            if isinstance(labels,str): labels = [labels]
-            if isinstance(x,str): x = [x]
-
-            self._validate_parameters(x)
-
-            rows = FilterPlottingData().filter(self, x, y)
-            rows = SmoothPlottingData().filter(rows, y, span)
-
-            envs     = self.environments
-            env_rows = { row[0]:dict(zip(envs.columns,row)) for row in envs }
-            get_key  = lambda row: row['learner_id']
-            lines    = []
+            og_l = (l1,l2)
 
-            style = "-" if x == ['index'] else "."
+            if not isinstance(l1,(list,tuple)): l1     = [l1]
+            if not isinstance(l2,(list,tuple)): l2     = [l2]
+            if     isinstance(labels,str)     : labels = [labels]
+
+            if any(_l1 in l2 for _l1 in l1):
+                raise CobaException("A value cannot be in both `l1` and `l2`. Please make a change and run it again.")
+
+            contraster = (lambda x,y: y-x) if mode == 'diff' else (lambda x,y: int(y-x>0)) if mode=='prob' else mode
+            _boundary  = 0 if mode == 'diff' else .5
+
+            plottable = self._plottable(x,y,l,p)
+            eid       = 'environment_id'
+            lid       = 'learner_id'
+
+            n_interactions = len(next(plottable.interactions.groupby(3))[1])
+
+            errevery = errevery or max(int(n_interactions*0.05),1) if x == 'index' else 1
+            style    = "-" if x == 'index' else "."
+            err      = plottable._confidence(err, errevery)
+
+            if x != 'index':
+                #this implementation is considerably slower but always gives the correct results
+                L1,L2 = [],[]
+                for _l, group in groupby(plottable._indexed_ys(l,eid,lid,x,y=y,span=span),key=itemgetter(0)):
+
+                    if _l in l1:
+                        L1.extend(map(itemgetter(slice(1,None)),group))
+                    if _l in l2:
+                        L2.extend(map(itemgetter(slice(1,None)),group))
+
+                X_Y_YE = []
+                for _xi, (_x, group) in enumerate(groupby(sorted(plottable._pairings(p,L1,L2),key=cmp_to_key(comparer)),key=itemgetter(0))):
+                    _x = f"{_x[0]}" if _x[0] == _x[1] else f"{_x[1]}-{_x[0]}"
+                    _Y = [contraster(*pair) for _,pair in group]
+                    if _Y: X_Y_YE.append((_x,) + err(_Y,_xi))
 
-            def get_color(colors:Union[None,Sequence[Union[str,int]]], i:int):
-                try:
-                    return colors[i] if colors else i
-                except IndexError:
-                    return i+max(colors) if isinstance(colors[0],(int,float)) else i
-                except TypeError:
-                    return i+colors
-
-            def get_label(labels:Sequence[str], i:int, lrn_id:int=None):
-                try:
-                    return labels[i] if labels else self._full_name(lrn_id)
-                except:
-                    return self._full_name(lrn_id)
+            else:
+                #this implementation is considerably faster but only gives correct results under certain conditions
+                X_Y_YE = []
+                for _xi, (_x, _group) in enumerate(groupby(plottable._indexed_ys(x,l,eid,lid,x,y=y,span=span),key=itemgetter(0))):
+
+                    _group = list(map(itemgetter(slice(1,None)),_group))
+                    _L1    = [g[1:] for g in _group if g[0] in l1]
+                    _L2    = [g[1:] for g in _group if g[0] in l2]
+                    _Y     = [contraster(*pair) for _,pair in plottable._pairings(p,_L1,_L2)]
+
+                    if _Y: X_Y_YE.append((str(_x) if x != 'index' else _x,) + err(_Y,_xi))
+
+            if not X_Y_YE:
+                raise CobaException(f"We were unable to create any pairings to contrast. Make sure l1={og_l[0]} and l2={og_l[1]} is correct.")
+
+            if x == 'index':
+                X,Y,YE = zip(*X_Y_YE)
+                color  = plottable._get_color(colors,        0)
+                label  = plottable._get_label(labels,'l2-l1',0)
+                label  = f"{label}" if legend else None
+                lines  = [Points(X,Y,None,YE, style=style, label=label, color=color)]
+
+            elif x == l:
+                if len(l1) > 1 and len(l2) == 1:
+                    #Sort by l1. We assume _x is "{l2}-{l1}."
+                    l2_len = len(str(l2[0]))
+                    l1 = list(map(str,l1))
+                    X_Y_YE = sorted(X_Y_YE, key=lambda items: l1.index(items[0][l2_len+1:]))
+                elif len(l2) > 1 and len(l1) == 1:
+                    #Sort by l2. We assume _x is "{l2}-{l1}."
+                    l1_len = len(str(l1[0]))
+                    l2 = list(map(str,l2))
+                    X_Y_YE = sorted(X_Y_YE, key=lambda items: l2.index(items[0][:-(l1_len+1)]))
+                else:
+                    X_Y_YE = sorted(X_Y_YE)
 
-            for i, (lrn_id, lrn_rows) in enumerate(groupby(sorted(rows, key=get_key),key=get_key)):
-                lrn_rows = list(lrn_rows)
-                XYE      = TransformToXYE().filter(lrn_rows, env_rows, x, y, err)
-                color    = get_color(colors,i)
-                label    = get_label(labels,i,lrn_id)
-                lines.append(Points(*zip(*XYE), color, 1, label, style))
-
-            lines  = sorted(lines, key=lambda line: line[1][-1], reverse=True)
-            labels = [l.label for l in lines]
-            colors = [l.color for l in lines]
-            xlabel = "Interaction" if x==['index'] else x[0] if len(x) == 1 else x
-            ylabel = y.capitalize().replace("_pct"," Percent")
+                X,Y,YE = zip(*X_Y_YE)
+                color  = plottable._get_color(colors, 0)
+                lines  = [Points(X,Y,None,YE, style=style, label=None, color=color)]
 
-            title = ("Instantaneous" if span == 1 else f"Span {span}" if span else "Progressive") + f" {ylabel}"
-            title = title + f" ({len(lrn_rows) if x==['index'] else len(XYE)} Environments)"
+            else:
+                upper = lambda y,ye: y+ye[1] if isinstance(ye,(list,tuple)) else y+ye
+                lower = lambda y,ye: y-ye[0] if isinstance(ye,(list,tuple)) else y-ye
 
-            if x != ['index']: title = f"Final {title}"
+                #split into win,tie,loss
+                l1_win = [(x,y,ye) for x,y,ye in X_Y_YE if upper(y,ye) <  _boundary                             ]
+                no_win = [(x,y,ye) for x,y,ye in X_Y_YE if lower(y,ye) <= _boundary and _boundary <= upper(y,ye)]
+                l2_win = [(x,y,ye) for x,y,ye in X_Y_YE if                              _boundary <  lower(y,ye)]
+
+                #sort by order of magnitude
+                l1_win = sorted(l1_win,key=itemgetter(1))
+                no_win = sorted(no_win,key=itemgetter(1))
+                l2_win = sorted(l2_win,key=itemgetter(1))
+
+                lines = []
+
+                if l1_win:
+                    X,Y,YE = zip(*l1_win)
+                    color  = plottable._get_color(colors,     0)
+                    label  = plottable._get_label(labels,'l1',0)
+                    label  = f"{label} ({len(X)})" if legend else None
+                    lines.append(Points(X,Y,None,YE, style=style, label=label, color=color))
+
+                if no_win:
+                    X,Y,YE = zip(*no_win)
+                    color  = plottable._get_color(colors, 1)
+                    label  = 'Tie'
+                    label  = f"{label} ({len(X)})" if legend else None
+                    lines.append(Points(X,Y,None,YE, style=style, label=label, color=color))
+
+                if l2_win:
+                    X,Y,YE = zip(*l2_win)
+                    color  = plottable._get_color(colors,     2)
+                    label  = plottable._get_label(labels,'l2',1)
+                    label  = f"{label} ({len(X)})" if legend else None
+                    lines.append(Points(X,Y,None,YE, style=style, label=label, color=color))
+
+            if boundary:
+                leftmost_x  = lines[0 ].X[0 ]
+                rightmost_x = lines[-1].X[-1]
+                lines.append(Points((leftmost_x,rightmost_x),(_boundary,_boundary), None, None , "#888", 1, None, '-',.5))
 
-            xrotation = 90 if x != ['index'] and len(XYE)>5 else 0
+            xrotation = 90 if x != 'index' and len(X_Y_YE)>5 else 0
             yrotation = 0
 
-            if top_n:
-                if abs(top_n) > len(lines): top_n = len(lines)*abs(top_n)/top_n
-                if top_n > 0: lines = [l._replace(color=get_color(colors,i),label=get_label(labels,i)) for i,l in enumerate(lines[:top_n],0    ) ]
-                if top_n < 0: lines = [l._replace(color=get_color(colors,i),label=get_label(labels,i)) for i,l in enumerate(lines[top_n:],top_n) ]
+            xlabel = "Interaction" if x=='index' else x[0] if len(x) == 1 else x
+            ylabel = f"$\Delta$ {y}" if mode=="diff" else f"P($\Delta$ {y} > 0)"
+            title  = f"{ylabel} ({len(_Y)} Environments)"
 
             self._plotter.plot(ax, lines, title, xlabel, ylabel, xlim, ylim, xticks, yticks, xrotation, yrotation, out)
+
         except CobaException as e:
             CobaContext.logger.log(str(e))
 
-    def _full_name(self,lrn_id:int) -> str:
-        """A user-friendly name created from a learner's params for reporting purposes."""
-
-        cols = self.learners.columns
-        vals = self.learners.where(learner_id=lrn_id)[:][0]
-
-        values = dict((k,v) for k,v in zip(cols,vals) if v is not None)
-        family = values.get('family',values['learner_id'])
-        params = f"({','.join(f'{k}={v}' for k,v in values.items() if k not in ['family','learner_id'])})"
-
-        return family if params == '()' else family+params
-
     def __str__(self) -> str:
         return str({"Learners": len(self._learners), "Environments": len(self._environments), "Interactions": len(self._interactions) })
 
+    def __eq__(self, o: object) -> bool:
+        return isinstance(o,Result) \
+           and o.environments == self.environments \
+           and o.learners == self.learners \
+           and o.evaluators == self.evaluators
+
     def _ipython_display_(self):
         #pretty print in jupyter notebook (https://ipython.readthedocs.io/en/stable/config/integrating.html)
         print(str(self))
 
-    def _validate_parameters(self, x:Sequence[str]):
-        if 'index' in x and len(x) > 1:
-            raise CobaException('The x-axis cannot contain both interaction index and environment features. Please choose one or the other.')
+    def _get_color(self, colors:Union[None,Sequence[Union[str,int]]], i:int) -> Union[str,int]:
+        try:
+            return colors[i] if colors else i
+        except IndexError:
+            return i+max(colors) if isinstance(colors[0],(int,float)) else i
+        except TypeError:
+            return i+colors
+
+    def _get_label(self, labels:Sequence[str], label:str, i:int) -> str:
+        try:
+            label = labels[i] if labels else label
+        except:
+            pass
+
+        return 'None' if label is None else label
+
+    def _pairings(self, p:Sequence[str], L1: Sequence[Tuple[int,int,float]], L2: Sequence[Tuple[int,int,float]]) -> Iterable[Tuple[float,float]]:
+
+        if isinstance(p,str): p = [p]
+
+        env_eq_cols = list(set(p) & set(self.environments.columns))
+        lrn_eq_cols = list(set(p) & set(self.learners.columns))
+
+        env_eq_vals = { row[0]:row[1:] for row in zip(*self.environments[['environment_id']+env_eq_cols]) }
+        lrn_eq_vals = { row[0]:row[1:] for row in zip(*self.learners    [['learner_id'    ]+lrn_eq_cols]) }
+
+        #could this be made faster? I could think of special cases but not a general solution to speed it up.
+        for e1,l1,x1,y1 in L1:
+            for e2,l2,x2,y2 in L2:
+                if env_eq_vals[e1] == env_eq_vals[e2] and lrn_eq_vals[l1] == lrn_eq_vals[l2]:
+                    yield ((x1,x2),(y1,y2))
+
+    def _plottable(self, x:Sequence[str], y:str, l: Sequence[str], p: Sequence[str]) -> 'Result':
+
+        if not isinstance(x,str) and 'index' in x and len(x) > 1:
+            raise CobaException('The x-axis cannot contain both indexes and parameters.')
+
+        if len(self.interactions) == 0:
+            raise CobaException("This result does not contain any data to plot.")
+
+        if y not in self.interactions.columns:
+            raise CobaException(f"This result does not contain column '{y}' in interactions.")
+
+        only_finished = self._filter_fin('min' if x == 'index' else None, l, p)
+
+        if len(only_finished.learners) == 0:
+            raise CobaException(f"This result does not contain a {p} that has been finished for every {l}.")
+
+        if len(only_finished.environments) != len(self.environments):
+            CobaContext.logger.log(f"Every {p} not present for all {l} has been excluded.")
+
+        if len(only_finished.interactions) != len(self.interactions):
+            CobaContext.logger.log(f"Interactions beyond the shortest {p} have been excluded.")
+
+        return only_finished
+
+    def _confidence(self, err: Union[str,PointAndInterval], errevery:int = 1):
+
+        if err == 'se':
+            ci = StdErrCI(1.96)
+        elif err == 'bs':
+            ci = BootstrapCI(.95, mean)
+        elif err == 'bi':
+            ci = BinomialCI('wilson')
+        elif err == 'sd':
+            ci = StdDevCI()
+        elif err is None or isinstance(err,str):
+            ci = None
+        else:
+            ci = err
+
+        def calc_ci(Z:Sequence[float],i:int = -1):
+            if ci is None:
+                return (mean(Z),0)
+            else:
+                skip_err = (i+1)%errevery
+                return (ci.point(Z), (0,0)) if skip_err else ci.point_interval(Z)
+
+        return calc_ci
+
+    def _indexed_tables(self,*indexes) -> Iterable[Tuple[Any]]:
+        indexed_tables = []
+
+        for (env_id,lrn_id,val_id), table in self.interactions.groupby(3):
+            e = self._env_cache.get(env_id,{})
+            l = self._lrn_cache.get(lrn_id,{})
+            v = self._val_cache.get(val_id,{})
+
+            indexed_table = []
+            for K in indexes:
+                if isinstance(K,str):
+                    indexed_table.append(e.get(K,l.get(K,v.get(K,None))))
+                if isinstance(K,(list,tuple)):
+                    indexed_table.append(tuple(e.get(k,l.get(k,v.get(k,None))) for k in K))
+
+            indexed_table.append(table)
+            indexed_tables.append(indexed_table)
+
+        return sorted(map(tuple,indexed_tables),key=cmp_to_key(comparer))
+
+    def _indexed_ys(self,*indexes,y,span) -> Iterable[Tuple[Any]]:
+
+        coords = [ i for i,I in enumerate(indexes) if I == 'index' ]
+
+        indexed_values = []
+        for indexed_table in self._indexed_tables(*indexes):
+            _table    = indexed_table[ -1]
+            _indexes = [repeat(i) for i in indexed_table[:-1]]
+            for i in coords: _indexes[i] = iter(_table['index'])
+            _y_values = [mean(_table[y])] if not coords else iter(moving_average(_table[y],span))
+            indexed_values.append( (indexed_table[:-1], iter(zip(*_indexes,_y_values))) )
+
+        first_index = coords[0] if coords else -1
+        upto_index  = itemgetter(slice(0,first_index))
+
+        for _,group in groupby(indexed_values,key=upto_index):
+            try:
+                group = list(group)
+                while True:
+                    for _,_indexed_ys in group:
+                        Y = next(_indexed_ys)
+                        yield Y
+            except StopIteration:
+                #we assume all environments are of equal length due to `_plottable`
+                pass
+
+    def _global_n(self, n: Union[int,Literal['min']]):
+
+        environments = self.environments
+        learners     = self.learners
+        evaluators   = self.evaluators
+        interactions = self.interactions
+
+        min_N = float('inf')
+
+        to_remove = []
+        for indexed_table in self._indexed_tables(['environment_id','learner_id','evaluator_id']):
+            table = indexed_table[1]
+            min_N = min(min_N,len(table))
+            if n!='min' and len(table) != n:
+                to_remove.append(indexed_table[0])
+
+        if to_remove:
+            select = self._remove(to_remove,n)
+            interactions = Table(View(interactions._data,select), interactions.columns, interactions.indexes)
+
+        if n == 'min':
+            interactions = interactions.where(index={'<=':min_N})
+
+        if len(interactions) != len(self.interactions):
+            environments = environments.where(environment_id=set(interactions['environment_id']))
+            learners     = learners    .where(learner_id    =set(interactions['learner_id'    ]))
+            evaluators   = evaluators  .where(evaluator_id  =set(interactions['evaluator_id'  ]))
+
+        return Result(environments, learners, evaluators, interactions, self.experiment)
+
+    def _group_p(self, l:Union[str, Sequence[str]], p:Union[str, Sequence[str]]):
+
+        environments = self.environments
+        learners     = self.learners
+        evaluators   = self.evaluators
+        interactions = self.interactions
+
+        n_levels = len(set(it[0] for it in self._indexed_tables(l)))
+
+        to_remove = []
+        for _, group in groupby(self._indexed_tables(p,['environment_id','learner_id','evaluator_id']),key=itemgetter(0)):
+            group = list(group)
+            if (len(group) < n_levels):
+                to_remove.extend(g[1] for g in group)
+
+        if to_remove:
+            select = self._remove(to_remove)
+            interactions = Table(View(interactions._data,select), interactions.columns, interactions.indexes)
+
+        if len(interactions) != len(self.interactions):
+            environments = environments.where(environment_id=set(interactions['environment_id']))
+            learners     = learners    .where(learner_id    =set(interactions['learner_id'    ]))
+            evaluators   = evaluators  .where(evaluator_id  =set(interactions['evaluator_id'  ]))
+
+        return Result(environments, learners, evaluators, interactions, self.experiment)
+
+    def _filter_fin(self,
+        n: Union[int,Literal['min'], None],
+        l: Union[str, Sequence[str], None],
+        p: Union[str, Sequence[str], None]) -> 'Result':
+        """Filter the results down to even outcomes so that plotted results will be meaningful.
+
+        Args:
+            n: The number of interactions a specific evaluation must have (None indicates no constraint).
+            l: The level at which we wish to compare evalation outcomes.
+            p: The pairs that must exist across all comparison levels in order to be included.
+        """
+
+        result = self.copy()
+
+        if n     : result = result._global_n(n)
+        if l or p: result = result._group_p(l,p)
+
+        return result
+
+    def _remove(self, ids: Sequence[Tuple[int,int,int]], n=0) -> Sequence[int]:
+        #this is much faster than any built in Table methods
+        loc          = 0
+        select       = []
+        interactions = self.interactions
+        for e,l,v in sorted(ids):
+            lo1 = my_bisect_left(interactions['environment_id'],e,loc,len(interactions))
+            hi1 = my_bisect_right(interactions['environment_id'],e,loc,len(interactions))
+            lo2 = my_bisect_left(interactions['learner_id'],l,lo1,hi1)
+            hi2 = my_bisect_right(interactions['learner_id'],l,lo1,hi1)
+            lo3 = my_bisect_left(interactions['evaluator_id'],v,lo2,hi2)
+            hi3 = my_bisect_right(interactions['evaluator_id'],v,lo2,hi2)
+
+            k = n if hi3-lo3>n else 0
+            select.extend(range(loc,lo3+k))
+            loc = hi3
+
+        select.extend(range(loc,len(interactions)))
+
+        return select
```

### Comparing `coba-6.5.0/coba/learners/__init__.py` & `coba-7.0.0/coba/learners/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,11 @@
 """This module contains all public learners and learner interfaces."""
 
 from coba.learners.primitives import Learner, PMF, ActionProb
 from coba.learners.safety     import SafeLearner
 from coba.learners.bandit     import EpsilonBanditLearner, UcbBanditLearner, FixedLearner, RandomLearner
 from coba.learners.corral     import CorralLearner
 from coba.learners.vowpal     import VowpalMediator
-from coba.learners.vowpal     import VowpalLearner, VowpalEpsilonLearner, VowpalSoftmaxLearner, VowpalBagLearner
+from coba.learners.vowpal     import VowpalLearner, VowpalEpsilonLearner, VowpalSoftmaxLearner, VowpalBagLearner, VowpalRndLearner
 from coba.learners.vowpal     import VowpalCoverLearner, VowpalRegcbLearner, VowpalSquarecbLearner, VowpalOffPolicyLearner
 from coba.learners.linucb     import LinUCBLearner
-
-__all__ = [
-    'PMF',
-    'ActionProb',
-    'Learner',
-    'SafeLearner',
-    'RandomLearner',
-    'FixedLearner',
-    'EpsilonBanditLearner',
-    'UcbBanditLearner',
-    'CorralLearner',
-    'LinUCBLearner',
-    'VowpalLearner',
-    'VowpalEpsilonLearner',
-    'VowpalSoftmaxLearner',
-    'VowpalBagLearner',
-    'VowpalCoverLearner',
-    'VowpalRegcbLearner',
-    'VowpalSquarecbLearner',
-    'VowpalOffPolicyLearner',
-    'VowpalMediator',
-]
+from coba.learners.misguided  import MisguidedLearner
```

### Comparing `coba-6.5.0/coba/learners/bandit.py` & `coba-7.0.0/coba/learners/bandit.py`

 * *Files identical despite different names*

### Comparing `coba-6.5.0/coba/learners/corral.py` & `coba-7.0.0/coba/learners/corral.py`

 * *Files identical despite different names*

### Comparing `coba-6.5.0/coba/learners/primitives.py` & `coba-7.0.0/coba/learners/primitives.py`

 * *Files identical despite different names*

### Comparing `coba-6.5.0/coba/learners/safety.py` & `coba-7.0.0/coba/learners/safety.py`

 * *Files 9% similar despite different names*

```diff
@@ -101,26 +101,20 @@
     def __init__(self, learner: Learner, seed:int=1) -> None:
         """Instantiate a SafeLearner.
 
         Args:
             learner: The learner we wish to make sure has the expected interface
         """
 
-        #is learn   batch safe
-        #is request batch safe
-        #is predict batch safe
-
-        # what is the prediction format being returned by predict?
-
-        self._learner     = learner if not isinstance(learner, SafeLearner) else learner._learner
-        self._rng         = CobaRandom(seed)
-        self._method      = {}
+        self.learner = learner if not isinstance(learner, SafeLearner) else learner.learner
+        self._rng    = CobaRandom(seed)
+        self._method = {}
 
-        self._pred_kwargs  = None
-        self._pred_batch = None
+        self._pred_kwargs = None
+        self._pred_batch  = None
         self._pred_format = None
 
     @property
     def full_name(self) -> str:
         """A user-friendly name created from a learner's params for reporting purposes."""
 
         params = dict(self.params)
@@ -130,21 +124,22 @@
             return f"{family}({','.join(f'{k}={v}' for k,v in params.items())})"
         else:
             return family
 
     @property
     def params(self) -> Mapping[str, Any]:
         try:
-            params = self._learner.params
-            params = params if isinstance(params,dict) else params()
+            params = self.learner.params
+            params = params if not callable(params) else params()               
+            params = params if isinstance(params,dict) else {'params':str(params)}
         except AttributeError:
             params = {}
 
         if "family" not in params:
-            params["family"] = self._learner.__class__.__name__
+            params["family"] = self.learner.__class__.__name__
 
         return params
 
     def _safe_call(self, key, method, args, kwargs = {}):
 
         if key in self._method:
             prev_method = self._method[key]
@@ -165,26 +160,26 @@
             except:
                 del self._method[key]
             raise
 
     def request(self, context: Context, actions: Actions, request: Actions) -> Sequence[Prob]:
 
         try:
-            return self._safe_call('request', self._learner.request, (context,actions,request))
+            return self._safe_call('request', self.learner.request, (context,actions,request))
         except AttributeError as ex:
             if "'request'" in str(ex):
                 raise CobaException(("The `request` method is not implemented for this learner."))
             raise
 
     def predict(self, context: Context, actions: Actions) -> Tuple[Action,Prob,kwargs]:
 
-        pred = self._safe_call('predict', self._learner.predict, (context,actions))
+        pred = self._safe_call('predict', self.learner.predict, (context,actions))
 
         if self._pred_batch is None: # first call only
-            predictor = lambda X,A: self._safe_call('predict', self._learner.predict, (X,A))
+            predictor = lambda X,A: self._safe_call('predict', self.learner.predict, (X,A))
 
             self._pred_batch  = batch_order(predictor,pred,context,actions)
             self._pred_kwargs = isinstance(pred[-1] if self._pred_batch != 'row' else pred[0][-1],abc.Mapping)
             self._pred_format = pred_format(pred, self._pred_batch, self._pred_kwargs, actions)
 
         if self._pred_batch == 'not':
             kwargs = pred[-1] if self._pred_kwargs else {}
@@ -230,15 +225,15 @@
                 P = pred[1]
 
             return A,P,kwargs
 
     def learn(self, context, actions, action, reward, probability, **kwargs) -> None:
 
         try:
-            self._safe_call('learn', self._learner.learn, (context,actions,action,reward,probability), kwargs)
+            self._safe_call('learn', self.learner.learn, (context,actions,action,reward,probability), kwargs)
         except TypeError as ex:
             if 'got an unexpected' in str(ex):
                 raise CobaException("It appears that learner.predict returned kwargs but learner.learn did not accept them.") from ex
             if 'learn() missing' in str(ex):
                 raise CobaException("It appears that learner.predict expected kwargs but learner.predict did not provide any.") from ex
             raise
```

### Comparing `coba-6.5.0/coba/learners/vowpal.py` & `coba-7.0.0/coba/learners/vowpal.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from itertools import repeat, compress
 from sys import platform
 from typing import Any, Dict, Union, Sequence, Mapping, Optional, Tuple
 
 from coba.backports import Literal
 from coba.exceptions import CobaException
 from coba.learners.primitives import Learner, PMF, Prob
-from coba.primitives import Sparse, Context, Action, Actions
+from coba.primitives import Sparse, Context, Action, Actions, Batch
 from coba.utilities import PackageChecker
 
 Feature       = Union[str,int,float]
 Features      = Union[Feature, Sequence[Feature], Dict[str,Union[int,float]]]
 Namespaces    = Dict[str,Features]
 VW_Features   = Sequence[Union[str,int,Tuple[Union[str,int],Union[int,float]],Dict[str,Union[int,float]]]]
 VW_Namespaces = Dict[str,VW_Features]
@@ -18,17 +18,17 @@
 DEFAULT_NAMESPACE_INTERACTIONS = (1, 'a', 'ax', 'axx')
 
 class VowpalMediator:
     """A class to handle all communication between Coba and VW."""
 
     def __init__(self) -> None:
         self._vw = None
-        self._namespace_keys = []
-        self._namespace_keys_index: Dict[str,int] = {}
         self._args = ""
+        self._ns_keys = {}
+        self._ns_keys_cnt = 0
  
         PackageChecker.vowpalwabbit('VowpalMediator.__init__')
 
     @property
     def is_initialized(self) -> bool:
         """Indicate whether init_learner has been called previously."""
         return self._vw is not None
@@ -135,29 +135,29 @@
 
         if self._version < [9,2] or (self._version == [9,2,0] and "linux" in platform): #pragma: no cover
             #the strange type checks below were faster than traditional methods when performance testing
             for ns, feats in namespaces.items():
                 if not feats and feats != 0 and feats != "":
                     continue
                 elif feats.__class__ is str:
-                    yield (ns, [f"{self._get_namespace_keys(ns,1)[0]}={feats}"])
+                    yield (ns, [f"{self._get_ns_keys(ns,0)}={feats}"])
                 elif feats.__class__ is int or feats.__class__ is float:
-                    yield (ns, [(self._get_namespace_keys(ns,1)[0], feats)])
+                    yield (ns, [(self._get_ns_keys(ns,0), feats)])
                 else:
-                    feats = feats.items() if isinstance(feats, Sparse) else zip(self._get_namespace_keys(ns,len(feats)),feats)
+                    feats = feats.items() if isinstance(feats, Sparse) else zip(self._get_ns_keys(ns,len(feats)),feats)
                     yield (ns, [f"{k}={v}" if v.__class__ is str else (k, v) for k,v in feats if v!= 0])
         else: #pragma: no cover
             #the strange type checks below were faster than traditional methods when performance testing
             for ns, feats in namespaces.items():
                 if not feats and feats != 0 and feats != "":
                     continue
                 elif feats.__class__ is str:
-                    yield (ns, [f"{self._get_namespace_keys(ns,1)[0]}={feats}"])
+                    yield (ns, {f"{self._get_ns_keys(ns,0)}={feats}":1})
                 elif feats.__class__ is int or feats.__class__ is float:
-                    yield (ns, [(self._get_namespace_keys(ns,1)[0], feats)])
+                    yield (ns, {self._get_ns_keys(ns,0): feats})
                 elif isinstance(feats,Sparse):
                     no_str = not any(map(isinstance,feats.values(),repeat(str))) # most-performant (still 2x slower than no check)
                     #no_str = str not in set(map(attrgetter("__class__"),feats.values()))
                     #no_str = not any(map(is_,map(attrgetter("__class__"),feats.values()),repeat(str)))
                     #no_str = True
                     if no_str:
                         yield (ns, feats.copy())
@@ -165,40 +165,42 @@
                         new = feats.copy()
                         for k,v in feats.items():
                             if isinstance(v,str):
                                 new[f"{k}={v}"] = 1
                                 del new[k]
                         yield (ns,new)
                 else:
-                    d={}
+                    no_str = not any(map(isinstance,compress(feats,feats),repeat(str)))
 
-                    K = self._get_namespace_keys(ns,len(feats))
+                    K = self._get_ns_keys(ns,len(feats))
                     V = feats
 
-                    for k,v in compress(zip(K,V),V):
-                        if v.__class__ is str:
-                            d[f"{k}={v}"] = 1
-                        else:
-                            d[k] = v
+                    if no_str:
+                        d = dict(compress(zip(K,V),V))
+                    else:
+                        d={}
+                        for k,v in compress(zip(K,V),V):
+                            if v.__class__ is str:
+                                d[f"{k}={v}"] = 1
+                            else:
+                                d[k] = v
 
                     yield (ns, d)
 
-    def _get_namespace_keys(self, namespace:str, length:int) -> Sequence[str]:
+    def _get_ns_keys(self, ns:str, length: int) -> Union[str,Sequence[str]]:
 
-        if namespace in self._namespace_keys_index:
-            index = self._namespace_keys_index[namespace]
-            keys  = self._namespace_keys[index:index+length]
-        else:
-            index = len(self._namespace_keys)
-            keys  = list(map(str,range(index,index+length)))
+        if ns not in self._ns_keys:
+            if not length:
+                self._ns_keys[ns] = str(self._ns_keys_cnt)
+                self._ns_keys_cnt += 1
+            else:
+                self._ns_keys[ns] = list(map(str,range(self._ns_keys_cnt,self._ns_keys_cnt+length)))
+                self._ns_keys_cnt += length
 
-            self._namespace_keys_index[namespace] = index
-            self._namespace_keys += keys
-
-        return keys
+        return self._ns_keys[ns]
 
     def __str__(self) -> str:
         return self._args
 
 class VowpalLearner(Learner):
     """A friendly wrapper around Vowpal Wabbit's python interface to support CB learning.
 
@@ -284,14 +286,17 @@
 
     def request(self, context: Context, actions: Actions, request: Actions) -> Sequence[Prob]:
         probs = self.predict(context,actions)
         return probs if actions == request else list(map(probs.__getitem__,map(actions.index,request)))
 
     def predict(self, context: Context, actions: Sequence[Action]) -> PMF:
 
+        if not self._vw.is_initialized and isinstance(context,Batch):#pragma: no cover
+            raise CobaException("VW learner does not support batched calls.")
+
         if not self._vw.is_initialized and self._adf:
             self._vw.init_learner(self._args, 4)
 
         if not self._vw.is_initialized and not self._adf and self._n_actions:
             self._vw.init_learner(self._args, 4)
 
         if not self._vw.is_initialized and not self._adf and not self._n_actions:
```

### Comparing `coba-6.5.0/coba/multiprocessing.py` & `coba-7.0.0/coba/multiprocessing.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,28 +63,26 @@
                 logger = CobaContext.logger
                 cacher = ConcurrentCacher(CobaContext.cacher,array,lock)
                 store  = { "openml_semaphore": spawn_context.Semaphore(3), **CobaContext.store }
 
                 filter = CobaMultiprocessor.ProcessFilter(self._filter, logger, cacher, store, write_stdlog)
 
             try:
-                yield from Multiprocessor(filter, self._processes, self._maxtasksperchild, self._chunked).filter(items)
+                yield from Multiprocessor(filter, self._processes, self._maxtasksperchild).filter(items)
 
             except Exception as e:
                 # If the error was due to an uncaught exception in the given filter it could be the case that the user 
                 # is expecting it therefore we don't want to supress it. On the other hand, if the error is due to the
                 # act of multiprocessing then we know the user is not expecting it and we log it in a friendly way.
-                if self._user_error(e): raise
-                CobaContext.logger.log(e)
+
+                #I have since changed my mind. We should raise it regardless.
+                raise
 
             finally:
                  if self._maxtasksperchild != 0 or self._processes > 1:
                     write_stdlog.write(None) #attempt to shutdown the logging process gracefully by sending the poison pill
                     stdlog_writer.join()
                     stdlog.close()
 
         except RuntimeError as e: #pragma: no cover
             #This happens when importing main causes this code to run again
             coba_exit(str(e))
-
-    def _user_error(self, exception: Exception) -> bool:
-        return 'pickle' not in str(exception) and 'unable to find' not in str(exception)
```

### Comparing `coba-6.5.0/coba/pipes/core.py` & `coba-7.0.0/coba/pipes/core.py`

 * *Files identical despite different names*

### Comparing `coba-6.5.0/coba/pipes/filters.py` & `coba-7.0.0/coba/pipes/filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,30 +44,34 @@
     @property
     def params(self) -> Mapping[str, Any]:
         return { "shuffle": self._seed }
 
 class Take(Filter[Iterable[Any], Sequence[Any]]):
     """Take a fixed number of items from an iterable."""
 
-    def __init__(self, count: Optional[int] ) -> None:
+    def __init__(self, count: Optional[int], strict:bool = False) -> None:
         """Instantiate a Take filter.
 
         Args:
             count: The number of items we wish to take from an iterable.
+            strict: Whether we want to take anything up to count or only count exactly.
         """
 
         is_valid_count = (count is None) or (isinstance(count,int) and count >= 0)
 
         if not is_valid_count:
             raise ValueError(f"Invalid value for Take: {count}. A positive integer or None was expected.")
 
         self._count = count
+        self._strict = strict
 
     def filter(self, items: Iterable[Any]) -> Iterable[Any]:
-        return islice(items, self._count)
+        out = islice(items, self._count)
+        if self._strict: out = list(out)
+        return [] if self._strict and len(out) < self._count else out
 
     @property
     def params(self) -> Mapping[str, Any]:
         return { "take": self._count }
 
 class Slice(Filter[Iterable[Any], Sequence[Any]]):
     """Take a slice of items from an iterable."""
@@ -107,59 +111,75 @@
         We use Algorithm L as described by Kim-Hung Li. (1994) to take a random count of items.
 
     References:
         Kim-Hung Li. 1994. Reservoir-sampling algorithms of time complexity O(n(1 + log(N/n))).
         ACM Trans. Math. Softw. 20, 4 (Dec. 1994), 481–493. DOI:https://doi.org/10.1145/198429.198435
     """
 
-    def __init__(self, count: Optional[int], seed: float = 1) -> None:
+    def __init__(self, count: Optional[int], strict: bool = False, seed: float = 1) -> None:
         """Instantiate a Reservoir filter.
 
         Args:
             count: The number of items we wish to sample from an iterable (expressed as either an exact value or range).
+            strict: Whether we want to take anything up to count or only count exactly.
             seed : The seed which determines which random items to take.
         """
 
         is_valid_count = (count is None) or (isinstance(count,int) and count >= 0)
 
         if not is_valid_count:
             raise ValueError(f"Invalid value for Reservoir: {count}. A positive integer or None was expected.")
 
-        self._count = count
-        self._seed  = seed
+        self._count  = count
+        self._seed   = seed
+        self._strict = strict
 
     @property
     def params(self) -> Mapping[str, Any]:
         return { "reservoir_count": self._count, "reservoir_seed": self._seed }
 
     def filter(self, items: Iterable[Any]) -> Sequence[Any]:
 
         rng = CobaRandom(self._seed)
 
         if self._count == 0:
             yield from []
 
         elif self._count is None:
             yield from rng.shuffle(items)
-        
+
         else:
             W         = 1
             items     = iter(items)
             reservoir = rng.shuffle(list(islice(items,self._count)))
 
-            try:
-                while True:
-                    [r1,r2,r3] = rng.randoms(3)
-                    W = W * math.exp(math.log(r1)/ (self._count or 1) )
-                    S = math.floor(math.log(r2)/math.log(1-W))
-                    reservoir[int(r3*self._count-.001)] = next(islice(items,S,S+1))
-            except StopIteration:
-                pass
+            if len(reservoir) < self._count:
+                yield from ([] if self._strict else reservoir)
+
+            else:
+                count = self._count or 1
+                log   = math.log
+                floor = math.floor
+                x     = 1/count
+
+                def batched_randoms_forever(batch_size):
+                    while True:
+                        randoms = rng.randoms(3*batch_size)
+                        for i in range(0,3*batch_size,3):
+                            yield randoms[i:i+3]
+
+                try:
+                    for r1,r2,r3 in batched_randoms_forever(20):
+                        W = W*r1**x
+                        S = floor(log(r2,1-W))
+                        reservoir[int(r3*count)] = next(islice(items,S,S+1))
+                except StopIteration:
+                    pass
 
-            yield from reservoir
+                yield from reservoir
 
 class JsonEncode(Filter[Any, str]):
     """A filter which turn a Python object into JSON strings."""
 
     def _min(self, obj):
         #WARNING: This method doesn't handle primitive types such int, float, or str. We handle this shortcoming
         #WARNING: by making sure no primitive type is passed to this method in filter. Accepting the shortcoming
@@ -243,15 +263,15 @@
             any_flattable = bool(flattable)
         else:
             flattable = []
             any_flattable = False
 
         def flatter_list(row):
             for f,r in zip(flattable,row):
-                if f: yield from r 
+                if f: yield from r
                 else: yield r
 
         if not any_flattable or first_type is None:
             yield from data
         elif first_type == "list":
             yield from (list(flatter_list(row)) for row in data)
         elif first_type == "tuple":
@@ -416,7 +436,15 @@
             items = iter(items)
             current = list(islice(items,n_slice))
             while current:
                 temp_cache.extend(current)
                 yield from current
                 current = list(islice(items,n_slice))
             self._cache = temp_cache
+
+class Insert(Filter[Iterable[Any], Iterable[Any]]):
+    def __init__(self, insert_items: Sequence[Any]) -> None:
+        self._insert_items = insert_items
+
+    def filter(self, items: Iterable[Any]) -> Iterable[Any]:
+        yield from self._insert_items
+        yield from items
```

### Comparing `coba-6.5.0/coba/pipes/multiprocessing.py` & `coba-7.0.0/coba/pipes/multiprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pickle
 import threading as mt
 import multiprocessing as mp
 
+from collections.abc import Iterator
 from queue import Empty
 from traceback import format_tb
 from typing import Iterable, Mapping, Callable, Optional, Union, Sequence, Any
 from coba.backports import Literal
 
 from coba.utilities import peek_first
 from coba.exceptions import CobaException
@@ -160,15 +161,15 @@
 
     @property
     def poisoned(self) -> bool:
         return self._poisoned
 
 class AsyncableLine(SourceSink):
 
-    def run_async(self, 
+    def run_async(self,
         callback:Callable[['AsyncableLine',Optional[Exception],Optional[str]],None]=None,
         mode:Literal['process','thread']='process') -> Union[ThreadLine,ProcessLine]:
         """Run the pipeline asynchronously."""
 
         mode = mode.lower()
 
         if mode == "process":
@@ -177,20 +178,23 @@
             worker = ThreadLine(line=self, callback=callback)
         else:
             raise CobaException(f"Unrecognized pipe async mode {mode}. Valid values are 'process' and 'thread'.")
 
         worker.start()
         return worker
 
-class Unchunker:
-    def __init__(self, chunked: bool) -> None:
-        self._chunked = chunked
+class Foreach:
+    def __init__(self,pipe:Filter) -> None:
+        self._pipe = pipe
+
     def filter(self, items: Iterable[Any]) -> Iterable[Any]:
-        if not self._chunked: items = [items]
-        for item in items: yield from item
+        for item in items:
+            out = self._pipe.filter(item)
+            out = out if isinstance(out,Iterator) else [out]
+            yield from out
 
 class Pickler:
 
     def filter(self, items) -> Iterable[bytes]:
         try:
             yield from map(pickle.dumps,items)
         except Exception as e:
@@ -232,65 +236,62 @@
 
 class Multiprocessor(Filter[Iterable[Any], Iterable[Any]]):
     """Create multiple processes to filter given items."""
 
     def __init__(self,
             filter: Filter[Iterable[Any], Iterable[Any]],
             n_processes: int = 1,
-            maxtasksperchild: int = 0,
-            chunked: bool = False,) -> None:
+            maxtasksperchild: int = 0) -> None:
         """Instantiate a Multiprocessor.
 
         Args:
             filter: The inner pipe that will be executed on multiple processes.
             n_processes: The number of processes that should be created to filter items.
             maxtasksperchild: The number of items/chunks a process should filter before restarting.
-            chunked: Indicates that the given items have been chunked.
         """
         self._filter           = filter
-        self._chunked          = chunked
         self._max_processes    = n_processes
         self._maxtasksperchild = maxtasksperchild or None
 
     @property
     def params(self) -> Mapping[str,Any]:
         return self._filter.params
 
     def filter(self, items: Iterable[Any]) -> Iterable[Any]:
 
         items = peek_first(items)[1]
         if not items: return []
 
         if self._max_processes == 1 and self._maxtasksperchild is None:
-            yield from self._filter.filter(Unchunker(self._chunked).filter(items))
+            yield from Foreach(self._filter).filter(items)
+
         else:
             event = spawn_context.Event()
 
             #for some reason if this mp queue get too big we can't keyboradinterrupt
             #therefore, we slightly limit its size and then empty it before closing.
             in_queue  = spawn_context.Queue(maxsize=self._max_processes*2)
             out_queue = spawn_context.Queue()
             in_put    = QueueSink(in_queue,foreach=True)
             in_get    = QueueSource(in_queue)
             out_put   = QueueSink(out_queue,foreach=True)
             out_get   = QueueSource(out_queue)
             pickler   = Pickler()
-            unpickler = Unpickler() 
+            unpickler = Unpickler()
             get_max   = Slice(None,self._maxtasksperchild)
-            unchunk   = Unchunker(self._chunked)
             setter    = EventSetter(event)
 
             self._n_procs      = self._max_processes
             self._exceptions   = []
             self._poison       = None
             self._main_err     = False
             self._load_stopper = Stopper() #this works because the loader is a thread which means we have shared memory
 
             load_line   = SourceSink(IterableSource(items), self._load_stopper, pickler, in_put)
-            filter_line = SourceSink(in_get, setter, unpickler, get_max, unchunk, self._filter, out_put)
+            filter_line = SourceSink(in_get, setter, unpickler, get_max, Foreach(self._filter), out_put)
 
             def loader_finished_or_failed(worker: Union[ThreadLine,ProcessLine]):
                 if worker.exception: self._exceptions.append(worker.exception)
                 in_put.write(self._load_stopper.filter([self._poison]*self._n_procs))
 
             def filter_finished_or_failed(worker: Union[ThreadLine,ProcessLine]):
                 if worker.exception: self._exceptions.append(worker.exception)
@@ -301,15 +302,15 @@
                 if worker.exitcode != 0: #pragma: no cover
                     #exitcode -15 is keyboard interrupt...
                     if worker.exitcode != -15:
                         print(worker.exitcode)
                     self._main_err = True
                     event.set()
 
-                #we have to stop on exception because depending on where the exception occurred
+                #we have to stop on exception since, depending on where the exception occurred,
                 #we may not have actually read anything from the input queue. If we didn't then
                 #the input queue will never empty and we'll be stuck starting processes forever.
                 if not worker.poisoned and not self._exceptions and worker.exitcode == 0:
                     ProcessLine(worker.pipeline,callback=filter_finished_or_failed).start()
                 else:
                     self._n_procs -= 1
                     if self._n_procs == 0:
@@ -340,15 +341,15 @@
                 #empty the input queue and then close it
                 #if we don't empty first then we can easily
                 #lock during a keyboard interrupt
                 try:
                     while True: in_queue.get_nowait()
                 except Empty:
                     pass
-                    #closing can cause exceptions 
+                    #closing can cause exceptions
                     #and doesn't seem to help anything
                     #in_queue.close()
 
                 #empty the input queue and then close it
                 #if we don't empty first then we can easily
                 #lock during a keyboard interrupt
                 try:
```

### Comparing `coba-6.5.0/coba/pipes/primitives.py` & `coba-7.0.0/coba/pipes/primitives.py`

 * *Files identical despite different names*

### Comparing `coba-6.5.0/coba/pipes/readers.py` & `coba-7.0.0/coba/pipes/readers.py`

 * *Files identical despite different names*

### Comparing `coba-6.5.0/coba/pipes/rows.py` & `coba-7.0.0/coba/pipes/rows.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import abc
 from itertools import count, compress, chain, filterfalse, islice, repeat
-from typing import Any, Union, Callable, Iterator, Sequence, Mapping, Iterable, Tuple
+from typing import Dict, Any, Union, Callable, Iterator, Sequence, Mapping, Iterable, Tuple
 from coba.backports import Literal
 
 from coba.primitives import Sparse, Dense, Categorical
 from coba.primitives.rows import Dense_, Sparse_
 from coba.utilities import peek_first
 from coba.pipes.primitives import Filter
 from coba.pipes.filters import Flatten
@@ -54,15 +54,15 @@
         #but is a bit of a conflation of functionality.
         #In theory this error checking logic with None
         #should be in an ARFF specific implementation.
         for e,v in zip(self._enc, self._load_or_get()):
             try:
                 yield e(v)
             except:
-                if v in ['?','']: 
+                if v in ['?','']:
                     yield None
                 else:
                     raise
 
 class LazySparse(Sparse_):
     __slots__=('_row','_enc','_nsp','_fwd','_inv','missing')
 
@@ -117,15 +117,15 @@
 
         if enc:
             return tuple(self._enc_items())
         elif inv:
             return tuple((inv.get(k,k), v) for k,v in row.items())
         else:
             return tuple(row.items())
-        
+
     def _enc_items(self)->Iterator:
         enc   = self._enc
         inv   = self._inv
         raw   = self._load_or_get()
         items = chain(raw.items(), zip(self._nsp-raw.keys(), repeat("0")))
 
         for k,v in items:
@@ -133,14 +133,55 @@
                 v = enc.get(k,lambda x:x)(v)
             except:
                 if v in ['?','']: v = None
                 else: raise
 
             yield (inv.get(k,k) if inv else k,v)
 
+class SparseDense(Dense_):
+    __slots__=('_values','_length')
+
+    def __init__(self, values: Dict[int,Any], length:int) -> None:
+        self._values = values
+        self._length = length
+
+    def copy(self) -> 'SparseDense':
+        return SparseDense(self._values.copy(), self._length)
+
+    def __setitem__(self, key:int, value:Any):
+        key = key if key >= 0 else key+self._length
+
+        if key < 0 or key >= self._length:
+            raise IndexError("list index out of range")
+
+        self._values[key] = value
+
+    def __getitem__(self, key: int):
+        key = key if key >= 0 else key+self._length
+
+        if key < 0 or key >= self._length:
+            raise IndexError("list index out of range")
+
+        return self._values.get(key,0)
+
+    def __iter__(self) -> Iterator:
+        sort = sorted(self._values.items())
+
+        yield from repeat(0,sort[0][0])
+        yield sort[0][1]
+
+        for p,n in zip(sort,sort[1:]):
+            yield from repeat(0,n[0]-p[0]-1)
+            yield n[1]
+
+        yield from repeat(0,self._length-sort[-1][0]-1)
+
+    def __len__(self) -> int:
+        return self._length
+
 class HeadDense(Dense_):
     __slots__=('_row','headers')
 
     def __init__(self, row: Dense, headers: Mapping[str,int] = None) -> None:
         self._row    = row
         self.headers = headers
 
@@ -168,19 +209,19 @@
     def __iter__(self) -> Iterator:
         return iter(self.keys())
 
     def __len__(self) -> int:
         return len(self._row)
 
     def keys(self) -> abc.KeysView:
-        head_map_inv_get = self._inv.__getitem__ 
+        head_map_inv_get = self._inv.__getitem__
         return set(map(head_map_inv_get, self._row.keys()))
 
     def items(self) -> Sequence:
-        head_map_inv_get = self._inv.__getitem__ 
+        head_map_inv_get = self._inv.__getitem__
         return tuple((head_map_inv_get(k),v) for k,v in self._row.items())
 
 class HeadRows(Filter[Iterable[Union[Dense,Sparse]],Iterable[Union[Dense,Sparse]]]):
 
     def __init__(self, headers: Union[Sequence,Mapping]) -> None:
         if isinstance(headers, abc.Mapping):
             self._mapping = headers
@@ -305,15 +346,15 @@
         return iter(compress(self._row, self._sel))
 
     def __len__(self) -> int:
         return self._len
 
 class DropSparse(Sparse_):
     __slots__=('_row','_drop_set')
-    
+
     def __init__(self, row: Sparse, drop_set: set = None) -> None:
         self._row      = row
         self._drop_set = drop_set
 
     def _key_check(self,key):
         if key not in self._drop_set:
             return key
@@ -329,15 +370,15 @@
         return len(self.keys())
 
     def keys(self) -> abc.KeysView:
         return self._row.keys() - self._drop_set
 
     def items(self) -> Sequence:
         drop = self._drop_set
-        yield from (item for item in self._row.items() if item[0] not in drop) 
+        yield from (item for item in self._row.items() if item[0] not in drop)
 
 class DropRows(Filter[Iterable[Union[Dense,Sparse]], Iterable[Union[Dense,Sparse]]]):
     """A filter which drops rows and columns from in table shaped data."""
 
     def __init__(self,
         drop_cols: Sequence[Union[str,int]] = [],
         drop_row: Callable[[Union[Sequence,Mapping]], bool] = None) -> None:
@@ -362,15 +403,15 @@
                 selects = [ i not in drop_cols for i in range(len(first)) ]
                 headers = []
                 indexes = list(compress(range(len(first)), selects))
 
             mapping = {k:v for k,v in chain(enumerate(indexes),headers)}
             length  = len(indexes)
 
-            if headers: 
+            if headers:
                 external_indexes = dict(zip(indexes,count()))
                 external_headers = { h: external_indexes[i] for h,i in headers if i in external_indexes }
             else:
                 external_headers = None
 
             return mapping, selects, length, external_headers
         else:
```

### Comparing `coba-6.5.0/coba/pipes/sinks.py` & `coba-7.0.0/coba/pipes/sinks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 import gzip
 
 from queue import Queue
 from collections.abc import Iterator
-from typing import Callable, Any, List
+from itertools import islice
+from typing import Callable, Any, List, Union, Sequence, Iterable
 
 from coba.pipes.primitives import Sink
 
 class NullSink(Sink[Any]):
     """A sink which does nothing with written items."""
     def write(self, item: Any) -> None:
         pass
 
 class ConsoleSink(Sink[Any]):
     """A sink which prints written items to console."""
 
     def write(self, item: Any) -> None:
         print(item)
 
-class DiskSink(Sink[str]):
+class DiskSink(Sink[Union[str,Sequence[str]]]):
     """A sink which writes to a file on disk.
 
     This sink supports writing in either plain text or as a gz compressed file.
     In order to make this distinction gzip files must end with a gz extension.
     """
 
-    def __init__(self, filename:str, mode:str='a+') -> None:
+    def __init__(self, filename:str, mode:str='a+', batch:int=None) -> None:
         """Instantiate a DiskSink.
 
         Args:
             filename: The path to the file to write.
             mode: The mode with which the file should be written.
+            batch: The number of lines to write before closing and reopening the file.
         """
 
-        #If you are using the gzip functionality of disk sink
-        #then you should note that this implementation isn't optimal
-        #in terms of compression since it compresses one line at a time.
+        #Gzip compression performance is relative to batch size
         #see https://stackoverflow.com/a/18109797/1066291 for more info.
 
         self._filename = filename
         self._count    = 0
         self._file     = None
         self._mode     = mode
+        self._batch    = batch
 
     def __enter__(self) -> 'DiskSink':
         self._count += 1
 
         if self._file is None:
             if ".gz" in self._filename:
                 self._file = gzip.open(self._filename, f"{self._mode}b", compresslevel=6)
@@ -55,18 +56,37 @@
 
     def __exit__(self, exc_type, exc_value, traceback):
         self._count -= 1
         if self._count == 0 and self._file is not None:
             self._file.close()
             self._file = None
 
-    def write(self, item: str) -> None:
-        with self:
-            self._file.write((item + '\n').encode('utf-8'))
-            self._file.flush()
+    def write(self, lines: Union[str,Iterable[str]]) -> None:
+        if isinstance(lines,str): 
+            lines = [lines]
+
+        lines = iter(lines)
+        batch = None
+
+        while self._unfinished(batch):
+            batch = self._get_batch(lines)
+            with self:
+                for line in batch:
+                    self._file.write((line + '\n').encode('utf-8'))
+                    self._file.flush()
+
+    def _get_batch(self, lines: Iterable[str]) -> Iterable[str]:
+        batch = islice(lines,self._batch)
+        if self._batch: batch = list(batch)
+        return batch
+
+    def _unfinished(self, batch:Any) -> bool:
+        not_started  = batch is None
+        not_finished = isinstance(batch,list) and len(batch) == self._batch
+        return not_started or not_finished
 
 class ListSink(Sink[Any]):
     """A sink which appends written items to a list."""
 
     def __init__(self, items: List[Any] = None, foreach: bool=False) -> None:
         """Instantiate a ListSink.
```

### Comparing `coba-6.5.0/coba/pipes/sources.py` & `coba-7.0.0/coba/pipes/sources.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import requests
 import gzip
 
 from queue import Queue
-from typing import Callable, Iterable, Any, Union, Mapping
+from typing import Any, Callable, Iterable, Union, Mapping, Sequence
 from coba.backports import Literal
 
 from coba.exceptions import CobaException
 from coba.pipes.primitives import Source
 
 class NullSource(Source[Any]):
     """A source which always returns an empty list."""
 
     def read(self) -> Iterable[Any]:
         return []
 
 class IdentitySource(Source[Any]):
-    """A source which reads from an iterable."""
+    """A source that reads from an iterable."""
 
     def __init__(self, item: Any, params: Mapping[str,Any] = None):
         """Instantiate an IterableSource.
 
         Args:
             item: The item to return from read.
             params: Teh params descirbing the source.
@@ -31,15 +31,15 @@
     def params(self) -> Mapping[str, Any]:
         return self._params
 
     def read(self) -> Iterable[Any]:
         return self._item
 
 class DiskSource(Source[Iterable[str]]):
-    """A source which reads a file from disk.
+    """A source that reads a file from disk.
 
     This source supports reading both plain text files as well gz compressed file.
     In order to make this distinction gzip files must end with a gz extension.
     """
 
     def __init__(self, filename:str, mode:str='r+'):
         """Instantiate a DiskSource.
@@ -73,15 +73,15 @@
 
     def read(self) -> Iterable[str]:
         with self:
             for line in self._file:
                 yield line.rstrip('\r\n')
 
 class QueueSource(Source[Iterable[Any]]):
-    """A source which reads from a queue."""
+    """A source that reads from a queue."""
 
     def __init__(self, queue:Queue, block:bool=True, poison:Any=None) -> None:
         """Instantiate a QueueSource.
 
         Args:
             queue: The queue that should be read.
             block: Indicates if the queue should block when it is empty.
@@ -102,15 +102,15 @@
                     break
 
                 yield item
         except (EOFError,BrokenPipeError,TypeError):
             pass
 
 class HttpSource(Source[Union[requests.Response, Iterable[str]]]):
-    """A source which reads from a web URL."""
+    """A source that reads from a web URL."""
 
     def __init__(self, url: str, mode: Literal["response","lines"] = "response") -> None:
         """Instantiate an HttpSource.
 
         Args:
             url: url that we should request an HTTP response from.
             mode: Return the response object if mode=`response` otherwise just return the response's lines.
@@ -119,43 +119,57 @@
         self._mode = mode
 
     def read(self) -> Union[requests.Response, Iterable[str]]:
         response = requests.get(self._url, stream=True) #by default this includes the header accept-encoding gzip and deflate
         return response if self._mode == "response" else response.iter_lines(decode_unicode=True)
 
 class IterableSource(Source[Iterable[Any]]):
-    """A source which reads from an iterable."""
+    """A source that reads from an iterable."""
 
     def __init__(self, iterable: Iterable[Any]=None):
         """Instantiate an IterableSource.
 
         Args:
             iterable: The iterable we should read from.
         """
         self.iterable = [] if iterable is None else iterable
 
     def read(self) -> Iterable[Any]:
         return self.iterable
 
+class ListSource(Source[Sequence[Any]]):
+    """A source that reads from a list."""
+
+    def __init__(self, sequence: Sequence[Any]=None):
+        """Instantiate a ListSource.
+
+        Args:
+            list: The sequence we should read from.
+        """
+        self.items = [] if sequence is None else sequence
+
+    def read(self) -> Iterable[Any]:
+        return self.items
+
 class LambdaSource(Source[Any]):
-    """A source which reads from a callable method."""
+    """A source that reads from a callable method."""
 
     def __init__(self, read: Callable[[],Any]):
         """Instantiate a LambdaSource.
 
         Args:
             read: A function to call for a return value when reading.
         """
         self._read = read
 
     def read(self) -> Iterable[Any]:
         return self._read()
 
 class UrlSource(Source[Iterable[str]]):
-    """A source which reads from a url.
+    """A source that reads from a url.
 
     If the given url uses a file scheme or is a local path then 
     a DiskSource is used internally.If the given url uses an http 
     or https scheme then an HttpSource is used internally.
     """
 
     def __init__(self, url:str) -> None:
```

### Comparing `coba-6.5.0/coba/primitives/feedbacks.py` & `coba-7.0.0/coba/primitives/feedbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
-from typing import Union, Sequence, Any
+from typing import Sequence, Any
 
-from coba.primitives.semantic import Action, AIndex, Batch
+from coba.primitives.semantic import Action, Batch
 
 class Feedback(ABC):
     @abstractmethod
-    def eval(self, arg: Union[Action,AIndex]) -> Any:
+    def eval(self, arg: Action) -> Any:
         ...
 
 class SequenceFeedback(Feedback):
     __slots__ = ('_actions','_feedbacks')
 
     def __init__(self, actions:Sequence[Action], feedbacks: Sequence[Any]) -> None:
         self._actions = actions
```

### Comparing `coba-6.5.0/coba/primitives/rows.py` & `coba-7.0.0/coba/primitives/rows.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from operator import eq
 from collections import abc
 from abc import ABC, abstractmethod
 from typing import Sequence, Iterator, Iterable, Any
 
 class Dense(ABC):
     __slots__=()
-    
+
     @abstractmethod
     def __getitem__(self, key) -> Any:
         ...
 
     @abstractmethod
     def __len__(self) -> int:
         ...
```

### Comparing `coba-6.5.0/coba/primitives/types.py` & `coba-7.0.0/coba/primitives/types.py`

 * *Files identical despite different names*

### Comparing `coba-6.5.0/coba/random.py` & `coba-7.0.0/coba/random.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,18 +305,19 @@
     Args:
         seq: The sequence to pick randomly from.
         weights: The proportion by which seq is selected from.
     """
 
     return _random.choice(seq, weights)
 
-def shuffle(array_like: Sequence[Any]) -> Sequence[Any]:
+def shuffle(array_like: Sequence[Any], inplace:bool=False) -> Sequence[Any]:
     """Shuffle the order of items in a sequence.
 
     Args:
         sequence: The sequence of items that are to be shuffled.
+        inplace: The sequence of items should be shuffled within the given sequence.
 
     Returns:
         A new sequence with the order of items shuffled.
     """
 
-    return _random.shuffle(array_like)
+    return _random.shuffle(array_like, inplace)
```

### Comparing `coba-6.5.0/coba/register.py` & `coba-7.0.0/coba/register.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from coba.registry     import CobaRegistry
 from coba.pipes        import NullSink, ConsoleSink, DiskSink, HttpSource
 from coba.environments import OpenmlSimulation, SupervisedSimulation
-from coba.environments import Sort, Scale, Cycle, Shuffle, Take, Identity, Where, Repr
+from coba.environments import Sort, Scale, Cycle, Shuffle, Take, Identity, Where, Repr, Reservoir
 from coba.contexts     import DiskCacher, NullCacher, IndentLogger, NullLogger, BasicLogger
 
 CobaRegistry.register("range" , range)
 CobaRegistry.register("zip"   , zip  )
 
 CobaRegistry.register("Null"   , NullSink   )
 CobaRegistry.register("Disk"   , DiskSink   )
@@ -18,15 +18,16 @@
 
 CobaRegistry.register("DiskCacher", DiskCacher)
 CobaRegistry.register("NullCacher", NullCacher)
 
 CobaRegistry.register("OpenmlSimulation"    , OpenmlSimulation    )
 CobaRegistry.register("SupervisedSimulation", SupervisedSimulation)
 
-CobaRegistry.register("Identity", Identity)
-CobaRegistry.register("Take"    , Take    )
-CobaRegistry.register("Shuffle" , Shuffle )
-CobaRegistry.register("Sort"    , Sort    )
-CobaRegistry.register("Scale"   , Scale   )
-CobaRegistry.register("Cycle"   , Cycle   )
-CobaRegistry.register("Where"   , Where   )
-CobaRegistry.register("Repr"    , Repr    )
+CobaRegistry.register("Identity" , Identity )
+CobaRegistry.register("Take"     , Take     )
+CobaRegistry.register("Reservoir", Reservoir)
+CobaRegistry.register("Shuffle"  , Shuffle  )
+CobaRegistry.register("Sort"     , Sort     )
+CobaRegistry.register("Scale"    , Scale    )
+CobaRegistry.register("Cycle"    , Cycle    )
+CobaRegistry.register("Where"    , Where    )
+CobaRegistry.register("Repr"     , Repr     )
```

### Comparing `coba-6.5.0/coba/registry.py` & `coba-7.0.0/coba/registry.py`

 * *Files identical despite different names*

### Comparing `coba-6.5.0/coba/statistics.py` & `coba-7.0.0/coba/statistics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,188 +1,211 @@
-from math import hypot, isnan, erf, sqrt
+from math import hypot, isnan, erf, sqrt, fsum
 from sys import version_info
 from operator import mul, sub
-from bisect import bisect_left 
-from itertools import repeat, accumulate
+from bisect import bisect_left
+from itertools import repeat, accumulate, compress, chain
 from abc import abstractmethod, ABC
-from typing import Sequence, Tuple, Union, Callable
+from typing import Sequence, Tuple, Union, Callable, Optional
 from coba.backports import Literal
 
 from coba.exceptions import CobaException
-from coba.random import CobaRandom
 from coba.utilities import PackageChecker
 
 def iqr(values: Sequence[float]) -> float:
 
     if len(values) <= 1: return 0.
 
     values = sorted(values)
 
     p25,p75 = percentile(values, [0.25,0.75])
 
     return p75-p25
 
-def weighted_percentile(values: Sequence[float], weights: Sequence[float], percentiles: Union[float,Sequence[float]], sort: bool = True) -> Union[float, Tuple[float,...]]:
+def percentile(values: Sequence[float], percentiles: Union[float,Sequence[float]], weights: Sequence[float] = None, sort: bool = True) -> Union[float, Tuple[float,...]]:
+
+    if len(values) == 1:
+        if isinstance(percentiles,(int,float)):
+            return values[0]
+        else:
+            return list(values)*len(percentiles)
+
+    def _percentile(values: Sequence[float], weights:Optional[Sequence[float]], percentile: float) -> float:
 
-    def _percentile(values: Sequence[float], weights:Sequence[float], percentile: float) -> float:
         assert 0 <= percentile and percentile <= 1, "Percentile must be between 0 and 1 inclusive."
 
         if percentile == 0:
             return values[0]
-        
+
         if percentile == 1:
             return values[-1]
 
-        R = bisect_left(weights,percentile)
-        L = R-1
-        LP = (weights[R]-percentile)/(weights[R]-weights[L])
+        if weights:
+            R = bisect_left(weights,percentile)
+            L = R-1
+            LP = (weights[R]-percentile)/(weights[R]-weights[L])
 
-        return LP*values[L] + (1-LP)*values[R]
+            return LP*values[L] + (1-LP)*values[R]
+        else:
+            i = percentile*(len(values)-1)
+            I = int(i)
+            
+            if i == I:
+                return values[I]
+            else:
+                w = (i-I)
+                return (1-w)*values[I] + w*values[I+1]
 
     if sort:
-        values, weights = zip(*sorted(zip(values,weights)))
-    
-    weights = (0,)+weights[1:]
-    weight_sum = sum(weights)
-    weights    = [w/weight_sum for w in accumulate(weights) ] 
-
-    if isinstance(percentiles,(float,int)):
-        return _percentile(values, weights, percentiles)
-    else:
-        return tuple([_percentile(values, weights, p) for p in percentiles ])
-
-def percentile(values: Sequence[float], percentiles: Union[float,Sequence[float]], sort: bool = True) -> Union[float, Tuple[float,...]]:
-
-    def _percentile(values: Sequence[float], percentile: float) -> float:
-        assert 0 <= percentile and percentile <= 1, "Percentile must be between 0 and 1 inclusive."
-
-        i = percentile*(len(values)-1)
-        I = int(i)
-        
-        if i == I:
-            return values[I]
+        if weights:
+            values, weights = zip(*sorted(zip(values,weights)))
         else:
-            w = (i-I)
-            return (1-w)*values[I] + w*values[I+1]
+            values = sorted(values)
 
-    if sort:
-        values = sorted(values)
+    if weights:
+        if any(not w for w in weights):
+            values = list(compress(values,weights))
+        weight_sum = sum(weights[1:])
+        weights    = [w/weight_sum for w in accumulate(chain([0],compress(weights[1:],weights)))]
 
     if isinstance(percentiles,(float,int)):
-        return _percentile(values, percentiles)
+        return _percentile(values, weights, percentiles)
     else:
-        return tuple([_percentile(values, p) for p in percentiles ])
+        return tuple([_percentile(values, weights, p) for p in percentiles ])
 
 def phi(x: float) -> float:
     'Cumulative distribution function for the standard normal distribution'
     return (1.0 + erf(x / sqrt(2.0))) / 2.0
 
 def mean(sample: Sequence[float]) -> float:
-    #If precision is needed use a true statistics package  
-    return sum(sample)/len(sample)
+    #If precision is needed use a true statistics package
+    return fsum(sample)/len(sample)
 
 def var(sample: Sequence[float]) -> float:
     n = len(sample)
 
     if n == 1: return float('nan')
 
     if version_info >= (3,8): #pragma: no cover
         #In Python 3.8 hypot was extended to support any number of items
         #this provides a fast/safe way to calculate the sum of squares
         #and so we revert to the one-pass method and trust in hypot
         E_s2 = hypot(*sample)**2
         E_s = sum(sample)
         return (E_s2-E_s*E_s/n)/(n-1)
-    else:
+    else: #pragma: no cover
         #using the corrected two pass algo as recommended by
         #https://cpsc.yale.edu/sites/default/files/files/tr222.pdf
         #I've optimized this as much as I think is possible in python
         diffs = tuple(map(sub,sample,repeat(sum(sample)/n)))
         return sum(map(mul,diffs,diffs))/(n-1)
 
 def stdev(sample: Sequence[float]) -> float:
     return var(sample)**(1/2)
 
 class PointAndInterval(ABC):
 
     @abstractmethod
-    def calculate(self, sample: Sequence[float]) -> Tuple[float, Tuple[float, float]]:
+    def point(self, sample: Sequence[float]) -> float:
+        ...
+
+    @abstractmethod
+    def point_interval(self, sample: Sequence[float]) -> Tuple[float, Tuple[float, float]]:
         ...
 
-class StandardErrorOfMean(PointAndInterval):
+class StdDevCI(PointAndInterval):
+    def point(self,sample: Sequence[float]) -> float:
+        return mean(sample)
+    def point_interval(self, sample: Sequence[float]) -> Tuple[float, Tuple[float, float]]:
+        mu = mean(sample)
+        sd = round(0 if len(sample) == 1 else stdev(sample),5)
+        return (mu, (sd,sd))
+
+class StdErrCI(PointAndInterval):
 
     def __init__(self, z_score:float=1.96) -> None:
-        self._z_score = z_score 
+        self._z_score = z_score
+        self._inner   = StdDevCI()
 
-    def calculate(self, sample: Sequence[float]) -> Tuple[float, Tuple[float, float]]:
-        mu = mean(sample)
-        se = 0 if len(sample) == 1 else stdev(sample)/(len(sample)**(.5))
-        
-        return (mu, (self._z_score*se,self._z_score*se))
+    def point(self,sample: Sequence[float]) -> float:
+        return self._inner.point(sample)
+
+    def point_interval(self, sample: Sequence[float]) -> Tuple[float, Tuple[float, float]]:
+        (mu,(sd,sd)) = self._inner.point_interval(sample)
+        sqrtn = len(sample)**.5
+        se    = round(sd/sqrtn,5)
+        ci    = self._z_score*se
+        return (mu, (ci,ci))
 
-class BootstrapConfidenceInterval(PointAndInterval):
+class BootstrapCI(PointAndInterval):
 
     def __init__(self, confidence:float, statistic:Callable[[Sequence[float]], float]) -> None:
+        PackageChecker.scipy('BootstrapConfidenceInterval.__init__')
         self._conf = confidence
         self._stat = statistic
+        self._args = dict(method='basic', vectorized=False, n_resamples=1000, random_state=1)
 
-    def calculate(self, sample: Sequence[float]) -> Tuple[float, Tuple[float, float]]:
-        rng = CobaRandom(1)
-        n = len(sample)
+    def point(self,sample: Sequence[float]) -> float:
+        return self._stat(sample)
 
-        sample_stats = [ self._stat([sample[i] for i in rng.randints(n, 0, n-1)]) for _ in range(50) ]
+    def point_interval(self, sample: Sequence[float]) -> Tuple[float, Tuple[float, float]]:
+        from scipy.stats import bootstrap
 
-        lower_conf = (1-self._conf)/2
-        upper_conf = (1+self._conf)/2
+        p   = self._stat(sample)
 
-        point_stat = self._stat(sample)
-        lower_stat,upper_stat = percentile(sample_stats,[lower_conf,upper_conf])
+        if len(sample) < 3:
+            l,h = p,p
+        else:
+            l,h = bootstrap([sample], self._stat, **self._args).confidence_interval
 
-        return (point_stat, (point_stat-lower_stat,upper_stat-point_stat))
+        return (p, (p-l,h-p))
 
-class BinomialConfidenceInterval(PointAndInterval):
+class BinomialCI(PointAndInterval):
 
     def __init__(self, method:Literal['wilson', 'clopper-pearson']):
         self._method = method
 
-    def calculate(self, sample: Sequence[float]) -> Tuple[float, Tuple[float, float]]:
+    def point(self,sample: Sequence[float]) -> float:
+        return sum(sample)/len(sample)
+
+    def point_interval(self, sample: Sequence[float]) -> Tuple[float, Tuple[float, float]]:
         if set(sample) - set([0,1]):
             raise CobaException("A binomial confidence interval can only be calculated on values of 0 and 1.")
 
         if self._method == "wilson":
             z_975 = 1.96 #z-score for .975 area to the left
             p_hat = sum(sample)/len(sample)
             n     = len(sample)
             Q     = z_975**2/(2*n)
 
             #https://www.itl.nist.gov/div898/handbook/prc/section2/prc241.htm
             interval_num = z_975*((p_hat*(1-p_hat))/n + Q/(2*n))**(.5)
             location_num = (p_hat+Q)
-            
+
             interval_den = (1+2*Q)
             location_den = (1+2*Q)
 
             interval = interval_num/interval_den
             location = location_num/location_den
 
             return (p_hat, (p_hat-(location-interval), (location+interval)-p_hat))
-        
+
         else:
-            PackageChecker.sklearn("BinomialConfidenceInterval")
+            PackageChecker.scipy("BinomialConfidenceInterval")
             from scipy.stats import beta
+
             lo = beta.ppf(.05/2, sum(sample), len(sample) - sum(sample) + 1)
             hi = beta.ppf(1-.05/2, sum(sample) + 1, len(sample) - sum(sample))
             p_hat = sum(sample)/len(sample)
 
             lo = 0.0 if isnan(lo) else lo
             hi = 1.0 if isnan(hi) else hi
 
             return (p_hat, (p_hat-lo,hi-p_hat))
 
-class OnlineVariance():
+class OnlineVariance:
     """Calculate sample variance in an online fashion.
 
     Remarks:
         This algorithm is known as Welford's algorithm and the implementation below
         is a modified version of the Python algorithm created by Wikepedia contributors (2020).
 
     References:
@@ -215,15 +238,15 @@
         M2     += delta * delta2
 
         (self._count, self._mean, self._M2) = (count, mean, M2)
 
         if count > 1:
             self._variance = M2 / (count - 1)
 
-class OnlineMean():
+class OnlineMean:
     """Calculate mean in an online fashion."""
 
     def __init__(self):
         self._n = 0
         self._mean = float('nan')
 
     @property
```

### Comparing `coba-6.5.0/coba/utilities.py` & `coba-7.0.0/coba/utilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -81,14 +81,31 @@
         """
         try:
             importlib.import_module('numpy')
         except ImportError:
             PackageChecker._handle_import_error(caller_name, "numpy")
 
     @staticmethod
+    def scipy(caller_name: str) -> None:
+        """Raise ImportError with detailed error message if scipy is not installed.
+
+        Functionality requiring scipy should call this helper and then lazily import.
+
+        Args:
+            caller_name: The name of the caller that requires scipy.
+
+        Remarks:
+            This pattern was inspired by sklearn (see `PackageChecker.scipy` for more information).
+        """
+        try:
+            importlib.import_module('scipy')
+        except ImportError:
+            PackageChecker._handle_import_error(caller_name, "scipy")
+
+    @staticmethod
     def sklearn(caller_name: str) -> None:
         """Raise ImportError with detailed error message if sklearn is not installed.
 
         Functionality requiring sklearn should call this helper and then lazily import.
 
         Args:
             caller_name: The name of the caller that requires sklearn.
```

### Comparing `coba-6.5.0/coba.egg-info/PKG-INFO` & `coba-7.0.0/coba.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: coba
-Version: 6.5.0
-Summary: A contextual bandit research package.
-Home-page: https://github.com/VowpalWabbit/coba
-Author: Mark Rucker
-Author-email: rucker.mark@gmail.com
-License: BSD 3-Clause License
+Version: 7.0.0
+Summary: A contextual bandit research package
+Author-email: Mark Rucker <rucker.mark@gmail.com>
+License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/vowpalwabbit/coba
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: full
 License-File: LICENSE
 License-File: AUTHORS
 
 [![codecov](https://codecov.io/gh/VowpalWabbit/coba/branch/master/graph/badge.svg?token=885XLZJ2D4)](https://codecov.io/gh/VowpalWabbit/coba)
 [![badge](https://img.shields.io/badge/launch%20example-binder-579ACA.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAB8lBMVEX///9XmsrmZYH1olJXmsr1olJXmsrmZYH1olJXmsr1olJXmsrmZYH1olL1olJXmsr1olJXmsrmZYH1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olJXmsrmZYH1olL1olL0nFf1olJXmsrmZYH1olJXmsq8dZb1olJXmsrmZYH1olJXmspXmspXmsr1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olLeaIVXmsrmZYH1olL1olL1olJXmsrmZYH1olLna31Xmsr1olJXmsr1olJXmsrmZYH1olLqoVr1olJXmsr1olJXmsrmZYH1olL1olKkfaPobXvviGabgadXmsqThKuofKHmZ4Dobnr1olJXmsr1olJXmspXmsr1olJXmsrfZ4TuhWn1olL1olJXmsqBi7X1olJXmspZmslbmMhbmsdemsVfl8ZgmsNim8Jpk8F0m7R4m7F5nLB6jbh7jbiDirOEibOGnKaMhq+PnaCVg6qWg6qegKaff6WhnpKofKGtnomxeZy3noG6dZi+n3vCcpPDcpPGn3bLb4/Mb47UbIrVa4rYoGjdaIbeaIXhoWHmZYHobXvpcHjqdHXreHLroVrsfG/uhGnuh2bwj2Hxk17yl1vzmljzm1j0nlX1olL3AJXWAAAAbXRSTlMAEBAQHx8gICAuLjAwMDw9PUBAQEpQUFBXV1hgYGBkcHBwcXl8gICAgoiIkJCQlJicnJ2goKCmqK+wsLC4usDAwMjP0NDQ1NbW3Nzg4ODi5+3v8PDw8/T09PX29vb39/f5+fr7+/z8/Pz9/v7+zczCxgAABC5JREFUeAHN1ul3k0UUBvCb1CTVpmpaitAGSLSpSuKCLWpbTKNJFGlcSMAFF63iUmRccNG6gLbuxkXU66JAUef/9LSpmXnyLr3T5AO/rzl5zj137p136BISy44fKJXuGN/d19PUfYeO67Znqtf2KH33Id1psXoFdW30sPZ1sMvs2D060AHqws4FHeJojLZqnw53cmfvg+XR8mC0OEjuxrXEkX5ydeVJLVIlV0e10PXk5k7dYeHu7Cj1j+49uKg7uLU61tGLw1lq27ugQYlclHC4bgv7VQ+TAyj5Zc/UjsPvs1sd5cWryWObtvWT2EPa4rtnWW3JkpjggEpbOsPr7F7EyNewtpBIslA7p43HCsnwooXTEc3UmPmCNn5lrqTJxy6nRmcavGZVt/3Da2pD5NHvsOHJCrdc1G2r3DITpU7yic7w/7Rxnjc0kt5GC4djiv2Sz3Fb2iEZg41/ddsFDoyuYrIkmFehz0HR2thPgQqMyQYb2OtB0WxsZ3BeG3+wpRb1vzl2UYBog8FfGhttFKjtAclnZYrRo9ryG9uG/FZQU4AEg8ZE9LjGMzTmqKXPLnlWVnIlQQTvxJf8ip7VgjZjyVPrjw1te5otM7RmP7xm+sK2Gv9I8Gi++BRbEkR9EBw8zRUcKxwp73xkaLiqQb+kGduJTNHG72zcW9LoJgqQxpP3/Tj//c3yB0tqzaml05/+orHLksVO+95kX7/7qgJvnjlrfr2Ggsyx0eoy9uPzN5SPd86aXggOsEKW2Prz7du3VID3/tzs/sSRs2w7ovVHKtjrX2pd7ZMlTxAYfBAL9jiDwfLkq55Tm7ifhMlTGPyCAs7RFRhn47JnlcB9RM5T97ASuZXIcVNuUDIndpDbdsfrqsOppeXl5Y+XVKdjFCTh+zGaVuj0d9zy05PPK3QzBamxdwtTCrzyg/2Rvf2EstUjordGwa/kx9mSJLr8mLLtCW8HHGJc2R5hS219IiF6PnTusOqcMl57gm0Z8kanKMAQg0qSyuZfn7zItsbGyO9QlnxY0eCuD1XL2ys/MsrQhltE7Ug0uFOzufJFE2PxBo/YAx8XPPdDwWN0MrDRYIZF0mSMKCNHgaIVFoBbNoLJ7tEQDKxGF0kcLQimojCZopv0OkNOyWCCg9XMVAi7ARJzQdM2QUh0gmBozjc3Skg6dSBRqDGYSUOu66Zg+I2fNZs/M3/f/Grl/XnyF1Gw3VKCez0PN5IUfFLqvgUN4C0qNqYs5YhPL+aVZYDE4IpUk57oSFnJm4FyCqqOE0jhY2SMyLFoo56zyo6becOS5UVDdj7Vih0zp+tcMhwRpBeLyqtIjlJKAIZSbI8SGSF3k0pA3mR5tHuwPFoa7N7reoq2bqCsAk1HqCu5uvI1n6JuRXI+S1Mco54YmYTwcn6Aeic+kssXi8XpXC4V3t7/ADuTNKaQJdScAAAAAElFTkSuQmCC)](https://mybinder.org/v2/gh/VowpalWabbit/Coba/HEAD?filepath=examples/notebooks)
 
 # Coba
@@ -61,15 +61,15 @@
 
  Learners are algorithms which are able to improve their action selection through interactions with environments.
 
  A number of algorithms are provided natively with Coba for quick comparsions. These include:
 
  * All contextual bandit learners in VowpalWabbit
  * UCB1-Tuned Bandit Learner by Auer et al. 2002
- * LinUCB by Chu et al. 2011
+ * LinUCB by Li and Chu et al. 2010
  * Corral by Agarwal et al. 2017
 
  ## Environments
 
  Environments are the core unit of evaluation in Coba. They are nothing more than a sequence of interactions with contexts, actions and rewards. A number of tools have been built into Coba to make simulation creation easier. All these tools are defined in the `coba.environments` module. We describe a few of these tools here.
 
  ### Creating Environments From Classification Data Sets
@@ -83,15 +83,15 @@
 
  ### Creating Environments From Generative Functions
 
  Sometimes we have well defined models that an agent has to make decisions within but no data. To support evaluation in these domains one can use `LambdaSimulation` to define generative functions to create an Environment.
 
  ### Creating Environments From Scratch
 
- If more customization is needed beyond what is offered above then you can easily create your own simulation by implementing Coba's simple `SimulatedEnvironment` interface.
+ If more customization is needed beyond what is offered above then you can easily create your own simulation by implementing Coba's `Environment` interface.
 
  ## Experiments
 
  Experiments are combinations of Learners and Environments. The Experiment class orchestrates the complex tasks of evaluating learners on environments in a resource efficient, repeatable, and robust manner. Experiments can be run on any number of processes (we often run on 96 core machines) and writes all results to file as it runs so that it can be restarted if it ever stops.
 
  ## Results
```

### Comparing `coba-6.5.0/coba.egg-info/SOURCES.txt` & `coba-7.0.0/coba.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 AUTHORS
 LICENSE
 README.md
-setup.py
+pyproject.toml
 coba/__init__.py
 coba/encodings.py
 coba/exceptions.py
 coba/multiprocessing.py
 coba/random.py
 coba/register.py
 coba/registry.py
@@ -29,23 +29,27 @@
 coba/environments/filters.py
 coba/environments/openml.py
 coba/environments/primitives.py
 coba/environments/serialized.py
 coba/environments/supervised.py
 coba/environments/synthetics.py
 coba/environments/templates.py
+coba/evaluators/__init__.py
+coba/evaluators/offline.py
+coba/evaluators/online.py
+coba/evaluators/primitives.py
 coba/experiments/__init__.py
 coba/experiments/core.py
 coba/experiments/process.py
 coba/experiments/results.py
-coba/experiments/tasks.py
 coba/learners/__init__.py
 coba/learners/bandit.py
 coba/learners/corral.py
 coba/learners/linucb.py
+coba/learners/misguided.py
 coba/learners/primitives.py
 coba/learners/safety.py
 coba/learners/vowpal.py
 coba/pipes/__init__.py
 coba/pipes/core.py
 coba/pipes/filters.py
 coba/pipes/multiprocessing.py
```

### Comparing `coba-6.5.0/setup.py` & `coba-7.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,48 @@
-import setuptools
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
 
-MAJOR               = 6
-MINOR               = 5
-MICRO               = 0
-VERSION             = f"{MAJOR}.{MINOR}.{MICRO}"
-
-with open("README.md", "r") as f:
-    long_description = f.read()
-
-setuptools.setup(
-    name="coba",
-    version=VERSION,
-    author="Mark Rucker",
-    author_email="rucker.mark@gmail.com",
-    description="A contextual bandit research package.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/VowpalWabbit/coba",
-    license="BSD 3-Clause License",
-    packages=["coba", "coba.environments", "coba.learners", "coba.experiments", "coba.pipes", "coba.contexts", "coba.backports", "coba.primitives"],
-    entry_points={ "coba.register": ["coba = coba.register"]},
-    classifiers=[
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: BSD License",
-        "Programming Language :: Python :: 3.7",
-        "Operating System :: OS Independent",
-        "Topic :: Scientific/Engineering"
-    ],
-    install_requires = [
-        'requests>=2',
-        'importlib-metadata>=1.0;python_version<"3.8"',
-        'typing-extensions>=4.1,<4.2;python_version<"3.8"'
-    ],
-    python_requires=">=3.7",
-)
+[tool.setuptools]
+packages = ["coba", "coba.environments", "coba.learners", "coba.evaluators", "coba.experiments", "coba.pipes", "coba.contexts", "coba.backports", "coba.primitives"]
+
+[tool.setuptools.dynamic]
+version = {attr = "coba.__version__"}
+
+[project]
+name = "coba"
+dynamic = ["version"]
+authors = [
+    {name = "Mark Rucker", email = "rucker.mark@gmail.com"},
+]
+description = "A contextual bandit research package"
+readme = "README.md"
+requires-python = ">=3.7"
+license = {text = "BSD-3-Clause"}
+classifiers = [
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: BSD License",
+    "Programming Language :: Python :: 3.7",
+    "Operating System :: OS Independent",
+    "Topic :: Scientific/Engineering"
+]
+dependencies = [
+    'requests>=2',
+    'importlib-metadata>=1.0;python_version<"3.8"',
+    'typing-extensions>=4.1,<4.2;python_version<"3.8"'
+]
+
+[project.urls]
+Homepage = "https://github.com/vowpalwabbit/coba"
+
+[project.entry-points."coba.register"]
+coba = "coba.register"
+
+[project.optional-dependencies]
+full = [
+    "vowpalwabbit",
+    "scikit-learn",
+    "pandas",
+    "matplotlib",
+    "numpy",
+    "scipy"
+]
```

