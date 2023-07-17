# Comparing `tmp/walrus-0.9.2.tar.gz` & `tmp/walrus-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/walrus-0.9.2.tar", last modified: Thu Jun 30 16:39:39 2022, max compression
+gzip compressed data, was "dist/walrus-0.9.3.tar", last modified: Mon Jul 17 13:39:40 2023, max compression
```

## Comparing `walrus-0.9.2.tar` & `walrus-0.9.3.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-06-30 16:39:39.000000 walrus-0.9.2/
--rw-r--r--   0 charles   (1000) charles   (1000)       68 2018-08-16 18:40:47.000000 walrus-0.9.2/MANIFEST.in
--rw-r--r--   0 charles   (1000) charles   (1000)     4165 2022-06-30 16:39:39.000000 walrus-0.9.2/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)     3035 2021-01-28 14:57:18.000000 walrus-0.9.2/README.md
--rw-r--r--   0 charles   (1000) charles   (1000)       38 2022-06-30 16:39:39.000000 walrus-0.9.2/setup.cfg
--rw-r--r--   0 charles   (1000) charles   (1000)     1300 2019-01-02 19:05:44.000000 walrus-0.9.2/setup.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-06-30 16:39:39.000000 walrus-0.9.2/walrus/
--rw-r--r--   0 charles   (1000) charles   (1000)     1488 2022-06-30 16:39:34.000000 walrus-0.9.2/walrus/__init__.py
--rw-r--r--   0 charles   (1000) charles   (1000)    12532 2021-03-27 17:30:46.000000 walrus-0.9.2/walrus/autocomplete.py
--rw-r--r--   0 charles   (1000) charles   (1000)    10030 2022-02-18 00:41:10.000000 walrus-0.9.2/walrus/cache.py
--rw-r--r--   0 charles   (1000) charles   (1000)    59972 2022-03-21 12:29:45.000000 walrus-0.9.2/walrus/containers.py
--rw-r--r--   0 charles   (1000) charles   (1000)     1105 2018-08-16 18:40:47.000000 walrus-0.9.2/walrus/counter.py
--rw-r--r--   0 charles   (1000) charles   (1000)    15164 2021-03-03 03:30:03.000000 walrus-0.9.2/walrus/database.py
--rw-r--r--   0 charles   (1000) charles   (1000)     5868 2020-07-09 18:24:17.000000 walrus-0.9.2/walrus/fts.py
--rw-r--r--   0 charles   (1000) charles   (1000)     7869 2019-01-31 00:15:19.000000 walrus-0.9.2/walrus/graph.py
--rw-r--r--   0 charles   (1000) charles   (1000)     4217 2019-12-30 20:15:01.000000 walrus-0.9.2/walrus/lock.py
--rw-r--r--   0 charles   (1000) charles   (1000)    27707 2020-07-07 18:28:45.000000 walrus-0.9.2/walrus/models.py
--rw-r--r--   0 charles   (1000) charles   (1000)     9874 2019-02-14 04:14:39.000000 walrus-0.9.2/walrus/query.py
--rw-r--r--   0 charles   (1000) charles   (1000)     3591 2021-07-01 13:07:48.000000 walrus-0.9.2/walrus/rate_limit.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-06-30 16:39:39.000000 walrus-0.9.2/walrus/scripts/
--rw-r--r--   0 charles   (1000) charles   (1000)      122 2018-08-16 18:40:47.000000 walrus-0.9.2/walrus/scripts/array_append.lua
--rw-r--r--   0 charles   (1000) charles   (1000)      189 2018-08-16 18:40:47.000000 walrus-0.9.2/walrus/scripts/array_extend.lua
--rw-r--r--   0 charles   (1000) charles   (1000)      219 2018-08-16 18:40:47.000000 walrus-0.9.2/walrus/scripts/array_get.lua
--rw-r--r--   0 charles   (1000) charles   (1000)      198 2018-08-16 18:40:47.000000 walrus-0.9.2/walrus/scripts/array_pop.lua
--rw-r--r--   0 charles   (1000) charles   (1000)      434 2018-08-16 18:40:47.000000 walrus-0.9.2/walrus/scripts/array_remove.lua
--rw-r--r--   0 charles   (1000) charles   (1000)      221 2018-08-16 18:40:47.000000 walrus-0.9.2/walrus/scripts/array_set.lua
--rw-r--r--   0 charles   (1000) charles   (1000)      313 2018-09-19 01:59:10.000000 walrus-0.9.2/walrus/scripts/cas.lua
--rw-r--r--   0 charles   (1000) charles   (1000)      198 2019-12-30 20:10:47.000000 walrus-0.9.2/walrus/scripts/lock_acquire.lua
--rw-r--r--   0 charles   (1000) charles   (1000)      271 2018-08-16 18:40:47.000000 walrus-0.9.2/walrus/scripts/lock_release.lua
--rw-r--r--   0 charles   (1000) charles   (1000)      289 2018-08-16 18:40:47.000000 walrus-0.9.2/walrus/scripts/zset_score_filter.lua
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-06-30 16:39:39.000000 walrus-0.9.2/walrus/search/
--rw-r--r--   0 charles   (1000) charles   (1000)     3294 2018-08-16 18:40:47.000000 walrus-0.9.2/walrus/search/__init__.py
--rwxr-xr-x   0 charles   (1000) charles   (1000)    19437 2021-07-01 13:07:55.000000 walrus-0.9.2/walrus/search/metaphone.py
--rw-r--r--   0 charles   (1000) charles   (1000)    12745 2018-08-16 18:40:47.000000 walrus-0.9.2/walrus/search/porter.py
--rw-r--r--   0 charles   (1000) charles   (1000)     3801 2021-03-19 17:59:08.000000 walrus-0.9.2/walrus/stopwords.txt
--rw-r--r--   0 charles   (1000) charles   (1000)     7383 2022-03-21 12:29:43.000000 walrus-0.9.2/walrus/streams.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-06-30 16:39:39.000000 walrus-0.9.2/walrus/tests/
--rw-r--r--   0 charles   (1000) charles   (1000)      734 2018-10-07 19:55:13.000000 walrus-0.9.2/walrus/tests/__init__.py
--rw-r--r--   0 charles   (1000) charles   (1000)    11243 2021-03-27 17:30:46.000000 walrus-0.9.2/walrus/tests/autocomplete.py
--rw-r--r--   0 charles   (1000) charles   (1000)     1551 2018-10-29 19:28:32.000000 walrus-0.9.2/walrus/tests/base.py
--rw-r--r--   0 charles   (1000) charles   (1000)     2808 2022-02-18 00:41:10.000000 walrus-0.9.2/walrus/tests/cache.py
--rw-r--r--   0 charles   (1000) charles   (1000)    35303 2021-11-17 15:04:39.000000 walrus-0.9.2/walrus/tests/containers.py
--rw-r--r--   0 charles   (1000) charles   (1000)      707 2018-10-01 02:58:28.000000 walrus-0.9.2/walrus/tests/counter.py
--rw-r--r--   0 charles   (1000) charles   (1000)     3762 2020-04-03 13:41:38.000000 walrus-0.9.2/walrus/tests/database.py
--rw-r--r--   0 charles   (1000) charles   (1000)     6156 2020-07-09 18:25:13.000000 walrus-0.9.2/walrus/tests/fts.py
--rw-r--r--   0 charles   (1000) charles   (1000)     5140 2018-10-01 03:00:04.000000 walrus-0.9.2/walrus/tests/graph.py
--rw-r--r--   0 charles   (1000) charles   (1000)     2366 2022-05-17 16:14:37.000000 walrus-0.9.2/walrus/tests/lock.py
--rw-r--r--   0 charles   (1000) charles   (1000)    25312 2020-01-06 15:01:01.000000 walrus-0.9.2/walrus/tests/models.py
--rw-r--r--   0 charles   (1000) charles   (1000)     2612 2018-10-01 02:58:18.000000 walrus-0.9.2/walrus/tests/rate_limit.py
--rw-r--r--   0 charles   (1000) charles   (1000)     8387 2021-11-17 15:04:40.000000 walrus-0.9.2/walrus/tests/streams.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-06-30 16:39:39.000000 walrus-0.9.2/walrus/tusks/
--rw-r--r--   0 charles   (1000) charles   (1000)        0 2018-08-16 18:40:47.000000 walrus-0.9.2/walrus/tusks/__init__.py
--rw-r--r--   0 charles   (1000) charles   (1000)     7037 2018-08-16 18:40:47.000000 walrus-0.9.2/walrus/tusks/helpers.py
--rw-r--r--   0 charles   (1000) charles   (1000)    10933 2018-08-16 18:40:47.000000 walrus-0.9.2/walrus/tusks/ledisdb.py
--rw-r--r--   0 charles   (1000) charles   (1000)     3035 2018-08-16 18:40:47.000000 walrus-0.9.2/walrus/tusks/rlite.py
--rw-r--r--   0 charles   (1000) charles   (1000)     6274 2018-11-16 16:25:23.000000 walrus-0.9.2/walrus/tusks/vedisdb.py
--rw-r--r--   0 charles   (1000) charles   (1000)     1634 2020-03-04 20:42:57.000000 walrus-0.9.2/walrus/utils.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-06-30 16:39:39.000000 walrus-0.9.2/walrus.egg-info/
--rw-r--r--   0 charles   (1000) charles   (1000)     4165 2022-06-30 16:39:39.000000 walrus-0.9.2/walrus.egg-info/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)     1262 2022-06-30 16:39:39.000000 walrus-0.9.2/walrus.egg-info/SOURCES.txt
--rw-r--r--   0 charles   (1000) charles   (1000)        1 2022-06-30 16:39:39.000000 walrus-0.9.2/walrus.egg-info/dependency_links.txt
--rw-r--r--   0 charles   (1000) charles   (1000)       13 2022-06-30 16:39:39.000000 walrus-0.9.2/walrus.egg-info/requires.txt
--rw-r--r--   0 charles   (1000) charles   (1000)        7 2022-06-30 16:39:39.000000 walrus-0.9.2/walrus.egg-info/top_level.txt
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 13:39:40.000000 walrus-0.9.3/
+-rw-rw-r--   0 charles   (1000) charles   (1000)       68 2018-08-16 18:40:47.000000 walrus-0.9.3/MANIFEST.in
+-rw-r--r--   0 charles   (1000) charles   (1000)     4165 2023-07-17 13:39:40.000000 walrus-0.9.3/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)     3035 2021-01-28 14:57:18.000000 walrus-0.9.3/README.md
+-rw-r--r--   0 charles   (1000) charles   (1000)       38 2023-07-17 13:39:40.000000 walrus-0.9.3/setup.cfg
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1300 2019-01-02 19:05:44.000000 walrus-0.9.3/setup.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 13:39:40.000000 walrus-0.9.3/walrus/
+-rw-r--r--   0 charles   (1000) charles   (1000)     1488 2023-07-17 13:39:21.000000 walrus-0.9.3/walrus/__init__.py
+-rw-r--r--   0 charles   (1000) charles   (1000)    12532 2021-03-27 17:30:46.000000 walrus-0.9.3/walrus/autocomplete.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    10030 2022-02-17 15:25:25.000000 walrus-0.9.3/walrus/cache.py
+-rw-r--r--   0 charles   (1000) charles   (1000)    59898 2023-07-17 13:38:14.000000 walrus-0.9.3/walrus/containers.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1105 2018-08-16 18:40:47.000000 walrus-0.9.3/walrus/counter.py
+-rw-r--r--   0 charles   (1000) charles   (1000)    15502 2023-07-17 13:37:56.000000 walrus-0.9.3/walrus/database.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     5868 2020-07-09 18:24:17.000000 walrus-0.9.3/walrus/fts.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     7864 2022-10-07 13:24:31.000000 walrus-0.9.3/walrus/graph.py
+-rw-r--r--   0 charles   (1000) charles   (1000)     4525 2022-11-06 21:27:32.000000 walrus-0.9.3/walrus/lock.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    27697 2023-05-08 13:03:26.000000 walrus-0.9.3/walrus/models.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     9874 2019-02-14 04:14:39.000000 walrus-0.9.3/walrus/query.py
+-rw-r--r--   0 charles   (1000) charles   (1000)     4083 2022-11-27 14:23:35.000000 walrus-0.9.3/walrus/rate_limit.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 13:39:40.000000 walrus-0.9.3/walrus/scripts/
+-rw-rw-r--   0 charles   (1000) charles   (1000)      122 2018-08-16 18:40:47.000000 walrus-0.9.3/walrus/scripts/array_append.lua
+-rw-rw-r--   0 charles   (1000) charles   (1000)      189 2018-08-16 18:40:47.000000 walrus-0.9.3/walrus/scripts/array_extend.lua
+-rw-rw-r--   0 charles   (1000) charles   (1000)      219 2018-08-16 18:40:47.000000 walrus-0.9.3/walrus/scripts/array_get.lua
+-rw-rw-r--   0 charles   (1000) charles   (1000)      198 2018-08-16 18:40:47.000000 walrus-0.9.3/walrus/scripts/array_pop.lua
+-rw-rw-r--   0 charles   (1000) charles   (1000)      434 2018-08-16 18:40:47.000000 walrus-0.9.3/walrus/scripts/array_remove.lua
+-rw-rw-r--   0 charles   (1000) charles   (1000)      221 2018-08-16 18:40:47.000000 walrus-0.9.3/walrus/scripts/array_set.lua
+-rw-rw-r--   0 charles   (1000) charles   (1000)      313 2018-09-19 01:59:10.000000 walrus-0.9.3/walrus/scripts/cas.lua
+-rw-rw-r--   0 charles   (1000) charles   (1000)      198 2022-05-10 21:11:12.000000 walrus-0.9.3/walrus/scripts/lock_acquire.lua
+-rw-rw-r--   0 charles   (1000) charles   (1000)      271 2022-05-10 21:11:11.000000 walrus-0.9.3/walrus/scripts/lock_release.lua
+-rw-r--r--   0 charles   (1000) charles   (1000)      599 2022-11-27 14:23:35.000000 walrus-0.9.3/walrus/scripts/rate_limit.lua
+-rw-rw-r--   0 charles   (1000) charles   (1000)      289 2018-08-16 18:40:47.000000 walrus-0.9.3/walrus/scripts/zset_score_filter.lua
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 13:39:40.000000 walrus-0.9.3/walrus/search/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     3294 2018-08-16 18:40:47.000000 walrus-0.9.3/walrus/search/__init__.py
+-rwxrwxr-x   0 charles   (1000) charles   (1000)    19437 2021-07-01 13:07:55.000000 walrus-0.9.3/walrus/search/metaphone.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    12745 2018-08-16 18:40:47.000000 walrus-0.9.3/walrus/search/porter.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     3801 2021-03-19 17:59:08.000000 walrus-0.9.3/walrus/stopwords.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)     7383 2022-03-21 12:36:45.000000 walrus-0.9.3/walrus/streams.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 13:39:40.000000 walrus-0.9.3/walrus/tests/
+-rw-rw-r--   0 charles   (1000) charles   (1000)      734 2018-10-07 19:55:13.000000 walrus-0.9.3/walrus/tests/__init__.py
+-rw-r--r--   0 charles   (1000) charles   (1000)    11243 2021-03-27 17:30:46.000000 walrus-0.9.3/walrus/tests/autocomplete.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1551 2018-10-29 19:28:32.000000 walrus-0.9.3/walrus/tests/base.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     2808 2022-02-17 15:28:09.000000 walrus-0.9.3/walrus/tests/cache.py
+-rw-r--r--   0 charles   (1000) charles   (1000)    35303 2021-11-17 15:04:39.000000 walrus-0.9.3/walrus/tests/containers.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      707 2018-10-01 02:58:28.000000 walrus-0.9.3/walrus/tests/counter.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     3762 2020-04-03 13:41:38.000000 walrus-0.9.3/walrus/tests/database.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     6156 2020-07-09 18:25:13.000000 walrus-0.9.3/walrus/tests/fts.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     5879 2022-10-07 13:24:14.000000 walrus-0.9.3/walrus/tests/graph.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     2366 2022-05-10 21:10:56.000000 walrus-0.9.3/walrus/tests/lock.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    25312 2020-01-06 15:01:01.000000 walrus-0.9.3/walrus/tests/models.py
+-rw-r--r--   0 charles   (1000) charles   (1000)     2862 2022-11-27 14:23:35.000000 walrus-0.9.3/walrus/tests/rate_limit.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     8387 2021-11-17 15:04:40.000000 walrus-0.9.3/walrus/tests/streams.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 13:39:40.000000 walrus-0.9.3/walrus/tusks/
+-rw-rw-r--   0 charles   (1000) charles   (1000)        0 2018-08-16 18:40:47.000000 walrus-0.9.3/walrus/tusks/__init__.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     7037 2018-08-16 18:40:47.000000 walrus-0.9.3/walrus/tusks/helpers.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    10933 2018-08-16 18:40:47.000000 walrus-0.9.3/walrus/tusks/ledisdb.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     3035 2018-08-16 18:40:47.000000 walrus-0.9.3/walrus/tusks/rlite.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     6274 2018-11-16 16:25:23.000000 walrus-0.9.3/walrus/tusks/vedisdb.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1634 2020-03-04 20:42:57.000000 walrus-0.9.3/walrus/utils.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-07-17 13:39:40.000000 walrus-0.9.3/walrus.egg-info/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     4165 2023-07-17 13:39:40.000000 walrus-0.9.3/walrus.egg-info/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1292 2023-07-17 13:39:40.000000 walrus-0.9.3/walrus.egg-info/SOURCES.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        1 2023-07-17 13:39:40.000000 walrus-0.9.3/walrus.egg-info/dependency_links.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)       13 2023-07-17 13:39:40.000000 walrus-0.9.3/walrus.egg-info/requires.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        7 2023-07-17 13:39:40.000000 walrus-0.9.3/walrus.egg-info/top_level.txt
```

### Comparing `walrus-0.9.2/PKG-INFO` & `walrus-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: walrus
-Version: 0.9.2
+Version: 0.9.3
 Summary: walrus
 Home-page: http://github.com/coleifer/walrus/
 Author: Charles Leifer
 Author-email: coleifer@gmail.com
 License: UNKNOWN
 Description: ## Walrus
```

### Comparing `walrus-0.9.2/README.md` & `walrus-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/setup.py` & `walrus-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/__init__.py` & `walrus-0.9.3/walrus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Lightweight Python utilities for working with Redis.
 """
 
 __author__ = 'Charles Leifer'
 __license__ = 'MIT'
-__version__ = '0.9.2'
+__version__ = '0.9.3'
 
 #               ___
 #            .-9 9 `\
 #          =(:(::)=  ;
 #            ||||     \
 #            ||||      `-.
 #           ,\|\|         `,
```

### Comparing `walrus-0.9.2/walrus/autocomplete.py` & `walrus-0.9.3/walrus/autocomplete.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/cache.py` & `walrus-0.9.3/walrus/cache.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/containers.py` & `walrus-0.9.3/walrus/containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 import struct
 try:
     from functools import reduce
 except ImportError:
     pass
 from functools import wraps
 try:
-    from redis.client import zset_score_pairs
     from redis.exceptions import ResponseError
 except ImportError:
     ResponseError = Exception
-    zset_score_pairs = None
 
 from walrus.utils import basestring_type
 from walrus.utils import decode as _decode
 from walrus.utils import decode_dict
 from walrus.utils import encode
 from walrus.utils import exception_message
 from walrus.utils import make_python_attr
```

### Comparing `walrus-0.9.2/walrus/counter.py` & `walrus-0.9.3/walrus/counter.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/database.py` & `walrus-0.9.3/walrus/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,18 @@
 import os
 import sys
 import threading
 import uuid
 
 try:
     from redis import Redis
-    from redis.client import pairs_to_dict
-    from redis.client import zset_score_pairs
     from redis.exceptions import ConnectionError
     from redis.exceptions import TimeoutError
 except ImportError:
     Redis = object
-    zset_score_pairs = None
     ConnectionError = TimeoutError = Exception
 
 from walrus.autocomplete import Autocomplete
 from walrus.cache import Cache
 from walrus.containers import Array
 from walrus.containers import BitField
 from walrus.containers import BloomFilter
@@ -29,14 +26,15 @@
 from walrus.containers import Stream
 from walrus.containers import ZSet
 from walrus.counter import Counter
 from walrus.fts import Index
 from walrus.graph import Graph
 from walrus.lock import Lock
 from walrus.rate_limit import RateLimit
+from walrus.rate_limit import RateLimitLua
 from walrus.streams import TimeSeries
 
 
 class TransactionLocal(threading.local):
     def __init__(self, **kwargs):
         super(TransactionLocal, self).__init__(**kwargs)
         self.pipes = []
@@ -76,14 +74,17 @@
             b'zset': self.ZSet,
             b'hash': self.Hash}
         self._transaction_local = TransactionLocal()
         self._transaction_lock = threading.RLock()
         if script_dir is not False:
             self.init_scripts(script_dir=script_dir)
 
+    def __bool__(self):
+        return True  # Avoid falling back to __len__().
+
     def xsetid(self, name, id):
         """
         Set the last ID of the given stream.
 
         :param name: stream identifier
         :param id: new value for last ID
         """
@@ -255,14 +256,23 @@
         Rate limit implementation. Allows up to `limit` of events every `per`
         seconds.
 
         See :ref:`rate-limit` for more information.
         """
         return RateLimit(self, name, limit, per, debug)
 
+    def rate_limit_lua(self, name, limit=5, per=60, debug=False):
+        """
+        Rate limit implementation. Allows up to `limit` of events every `per`
+        seconds. Uses a Lua script for atomicity.
+
+        See :ref:`rate-limit` for more information.
+        """
+        return RateLimitLua(self, name, limit, per, debug)
+
     def Index(self, name, **options):
         """
         Create a :py:class:`Index` full-text search index with the given
         name and options.
         """
         return Index(self, name, **options)
```

### Comparing `walrus-0.9.2/walrus/fts.py` & `walrus-0.9.3/walrus/fts.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/graph.py` & `walrus-0.9.3/walrus/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,16 @@
             parts.extend(('pos', p, o))
         elif s:
             parts.extend(('spo', s))
         elif p:
             parts.extend(('pos', p))
         elif o:
             parts.extend(('osp', o))
+        else:
+            parts.extend(('spo',))
         return key(parts + ['']), key(parts + ['\xff'])
 
     def query(self, s=None, p=None, o=None):
         """
         Return all triples that satisfy the given expression. You may specify
         all or none of the fields (s, p, and o). For instance, if I wanted
         to query for all the people who live in Kansas, I might write:
@@ -143,16 +145,14 @@
             for triple in graph.query(p='lives', o='Kansas'):
                 print triple['s'], 'lives in Kansas!'
         """
         start, end = self.keys_for_query(s, p, o)
         if end is None:
             if start in self._z:
                 yield {'s': s, 'p': p, 'o': o}
-            else:
-                raise StopIteration
         else:
             for key in self._z.range_by_lex('[' + start, '[' + end):
                 keys, p1, p2, p3 = decode(key).split('::')
                 yield dict(zip(keys, (p1, p2, p3)))
 
     def v(self, name):
         """
```

### Comparing `walrus-0.9.2/walrus/lock.py` & `walrus-0.9.3/walrus/lock.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 
     Unlike the redis-py lock implementation, this Lock does not
     use a spin-loop when blocking to acquire the lock. Instead,
     it performs a blocking pop on a list. When a lock is released,
     a value is pushed into this list, signalling that the lock is
     available.
 
+    .. warning::
+        The event list for each lock persists
+        indefinitely unless removed using :py:meth:`Lock.clear` or
+        otherwise manually in the Redis database. For this reason,
+        be cautious when creating locks dynamically, or your
+        keyspace might grow in an unbounded way.
+
     The lock uses Lua scripts to ensure the atomicity of its
     operations.
 
     You can set a TTL on a lock to reduce the potential for deadlocks
     in the event of a crash. If a lock is not released before it
     exceeds its TTL, and threads that are blocked waiting for the
     lock could potentially re-acquire it.
```

### Comparing `walrus-0.9.2/walrus/models.py` & `walrus-0.9.3/walrus/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,15 +387,15 @@
         self.field = field
         self.__database__ = self.field.model_class.__database__
         self.query_helper = self.field.model_class._query
 
     def field_value(self, instance):
         return self.field.db_value(getattr(instance, self.field.name))
 
-    def get_key(self, instance, value):
+    def get_key(self, value):
         raise NotImplementedError
 
     def store_instance(self, key, instance, value):
         raise NotImplementedError
 
     def delete_instance(self, key, instance, value):
         raise NotImplementedError
```

### Comparing `walrus-0.9.2/walrus/query.py` & `walrus-0.9.3/walrus/query.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/rate_limit.py` & `walrus-0.9.3/walrus/rate_limit.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 
         counter = self.database.List(self.name + ':' + key)
         n = len(counter)
         is_limited = False
         if n < self._limit:
             counter.prepend(str(time.time()))
         else:
-            oldest = float(counter[-1])
-            if time.time() - oldest < self._per:
+            oldest = counter[-1]
+            if (oldest is not None) and (time.time() - float(oldest) < self._per):
                 is_limited = True
             else:
                 counter.prepend(str(time.time()))
             del counter[:self._limit]
         counter.pexpire(int(self._per * 2000))
         return is_limited
 
@@ -91,7 +91,23 @@
                 if self.limit(key):
                     raise RateLimitException(
                         'Call to %s exceeded %s events in %s seconds.' % (
                             fn.__name__, self._limit, self._per))
                 return fn(*args, **kwargs)
             return inner
         return decorator
+
+
+class RateLimitLua(RateLimit):
+    """
+    Rate limit implementation. Allows up to "limit" number of events every per
+    the given number of seconds. Uses a Lua script to ensure atomicity.
+    """
+    def limit(self, key):
+        if self._debug:
+            return False
+
+        key = self.name + ':' + key
+        return bool(self.database.run_script(
+            'rate_limit',
+            keys=[key],
+            args=[self._limit, self._per, time.time()]))
```

### Comparing `walrus-0.9.2/walrus/search/__init__.py` & `walrus-0.9.3/walrus/search/__init__.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/search/metaphone.py` & `walrus-0.9.3/walrus/search/metaphone.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/search/porter.py` & `walrus-0.9.3/walrus/search/porter.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/stopwords.txt` & `walrus-0.9.3/walrus/stopwords.txt`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/streams.py` & `walrus-0.9.3/walrus/streams.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/tests/__init__.py` & `walrus-0.9.3/walrus/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/tests/autocomplete.py` & `walrus-0.9.3/walrus/tests/autocomplete.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/tests/base.py` & `walrus-0.9.3/walrus/tests/base.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/tests/cache.py` & `walrus-0.9.3/walrus/tests/cache.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/tests/containers.py` & `walrus-0.9.3/walrus/tests/containers.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/tests/counter.py` & `walrus-0.9.3/walrus/tests/counter.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/tests/database.py` & `walrus-0.9.3/walrus/tests/database.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/tests/fts.py` & `walrus-0.9.3/walrus/tests/fts.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/tests/graph.py` & `walrus-0.9.3/walrus/tests/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,30 @@
         self.assertEqual(len(result), len(expected))
         for i1, i2 in zip(result, expected):
             self.assertEqual(
                 (i1['s'], i1['p'], i1['o']), i2)
 
     def test_query(self):
         self.create_graph_data()
+        res = self.g.query()
+        self.assertTriples(res, (
+            ('charlie', 'is', 'human'),
+            ('charlie', 'likes', 'huey'),
+            ('charlie', 'likes', 'mickey'),
+            ('charlie', 'likes', 'zaizee'),
+            ('connor', 'likes', 'huey'),
+            ('connor', 'likes', 'mickey'),
+            ('huey', 'eats', 'catfood'),
+            ('huey', 'is', 'cat'),
+            ('mickey', 'eats', 'anything'),
+            ('mickey', 'is', 'dog'),
+            ('zaizee', 'eats', 'catfood'),
+            ('zaizee', 'is', 'cat'),
+        ))
+
         res = self.g.query('charlie', 'likes')
         self.assertTriples(res, (
             ('charlie', 'likes', 'huey'),
             ('charlie', 'likes', 'mickey'),
             ('charlie', 'likes', 'zaizee'),
         ))
 
@@ -106,14 +122,20 @@
 
         res = self.g.query(o='huey')
         self.assertTriples(res, (
             ('charlie', 'likes', 'huey'),
             ('connor', 'likes', 'huey'),
         ))
 
+        res = self.g.query(s='does-not-exist')
+        self.assertTriples(res, [])
+
+        res = self.g.query(s='huey', p='is', o='x')
+        self.assertTriples(res, [])
+
     def test_search(self):
         self.create_graph_data()
         X = self.g.v('x')
         result = self.g.search(
             {'s': 'charlie', 'p': 'likes', 'o': X},
             {'s': X, 'p': 'eats', 'o': 'catfood'},
             {'s': X, 'p': 'is', 'o': 'cat'})
```

### Comparing `walrus-0.9.2/walrus/tests/lock.py` & `walrus-0.9.3/walrus/tests/lock.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/tests/models.py` & `walrus-0.9.3/walrus/tests/models.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/tests/rate_limit.py` & `walrus-0.9.3/walrus/tests/rate_limit.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,30 @@
 from walrus.tests.base import db
 
 
 class TestRateLimit(WalrusTestCase):
     def setUp(self):
         super(TestRateLimit, self).setUp()
         # Limit to 5 events per second.
-        self.rl = db.rate_limit('test-rl', 5, 1)
+        self.rl = self.get_rate_limit('test-rl', 5, 1)
+
+    def get_rate_limit(self, key, limit, per):
+        return db.rate_limit(key, limit, per)
 
     def test_rate_limit(self):
         for i in range(5):
             self.assertFalse(self.rl.limit('k1'))
 
         for i in range(3):
             self.assertTrue(self.rl.limit('k1'))
 
         self.assertFalse(self.rl.limit('k2'))
 
     def test_rate_limit_rollover(self):
-        rl = db.rate_limit('test-rl2', 3, 100)
+        rl = self.get_rate_limit('test-rl2', 3, 100)
         container = db.List('test-rl2:k1')
 
         now = time.time()
         past = now - 101
 
         # Simulate two events.
         container.extend([now, now])
@@ -62,15 +65,15 @@
         container[-1] = past
 
         self.assertFalse(rl.limit('k1'))
         self.assertFalse(rl.limit('k1'))
         self.assertTrue(rl.limit('k1'))
 
     def test_decorator(self):
-        rl = db.rate_limit('test-rl2', 3, 100)
+        rl = self.get_rate_limit('test-rl2', 3, 100)
         container = db.List('test-rl2:fake-key')
 
         def key_fn(*args, **kwargs):
             return 'fake-key'
 
         @rl.rate_limited(key_function=key_fn)
         def do_test():
@@ -84,7 +87,12 @@
 
         container.popright()
         container[-1] = now - 101
 
         self.assertEqual(do_test(), 'OK')
         self.assertEqual(do_test(), 'OK')
         self.assertRaises(RateLimitException, do_test)
+
+
+class TestRateLimitLua(TestRateLimit):
+    def get_rate_limit(self, key, limit, per):
+        return db.rate_limit_lua(key, limit, per)
```

### Comparing `walrus-0.9.2/walrus/tests/streams.py` & `walrus-0.9.3/walrus/tests/streams.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/tusks/helpers.py` & `walrus-0.9.3/walrus/tusks/helpers.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/tusks/ledisdb.py` & `walrus-0.9.3/walrus/tusks/ledisdb.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/tusks/rlite.py` & `walrus-0.9.3/walrus/tusks/rlite.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/tusks/vedisdb.py` & `walrus-0.9.3/walrus/tusks/vedisdb.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus/utils.py` & `walrus-0.9.3/walrus/utils.py`

 * *Files identical despite different names*

### Comparing `walrus-0.9.2/walrus.egg-info/PKG-INFO` & `walrus-0.9.3/walrus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: walrus
-Version: 0.9.2
+Version: 0.9.3
 Summary: walrus
 Home-page: http://github.com/coleifer/walrus/
 Author: Charles Leifer
 Author-email: coleifer@gmail.com
 License: UNKNOWN
 Description: ## Walrus
```

### Comparing `walrus-0.9.2/walrus.egg-info/SOURCES.txt` & `walrus-0.9.3/walrus.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 walrus/scripts/array_get.lua
 walrus/scripts/array_pop.lua
 walrus/scripts/array_remove.lua
 walrus/scripts/array_set.lua
 walrus/scripts/cas.lua
 walrus/scripts/lock_acquire.lua
 walrus/scripts/lock_release.lua
+walrus/scripts/rate_limit.lua
 walrus/scripts/zset_score_filter.lua
 walrus/search/__init__.py
 walrus/search/metaphone.py
 walrus/search/porter.py
 walrus/tests/__init__.py
 walrus/tests/autocomplete.py
 walrus/tests/base.py
```

