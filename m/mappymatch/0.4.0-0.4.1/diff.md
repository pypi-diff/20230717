# Comparing `tmp/mappymatch-0.4.0.tar.gz` & `tmp/mappymatch-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mappymatch-0.4.0.tar", last modified: Tue Jul 11 21:44:36 2023, max compression
+gzip compressed data, was "mappymatch-0.4.1.tar", last modified: Mon Jul 17 20:18:38 2023, max compression
```

## Comparing `mappymatch-0.4.0.tar` & `mappymatch-0.4.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.526218 mappymatch-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-11 21:44:24.000000 mappymatch-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 21:44:24.000000 mappymatch-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-11 21:44:36.526218 mappymatch-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-11 21:44:24.000000 mappymatch-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.506217 mappymatch-0.4.0/mappymatch/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.510217 mappymatch-0.4.0/mappymatch/constructs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/constructs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/constructs/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/constructs/geofence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/constructs/match.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/constructs/road.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/constructs/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.510217 mappymatch-0.4.0/mappymatch/maps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/maps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.510217 mappymatch-0.4.0/mappymatch/maps/igraph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/maps/igraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/maps/igraph/igraph_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/maps/map_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.514217 mappymatch-0.4.0/mappymatch/maps/nx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/maps/nx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/maps/nx/nx_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.514217 mappymatch-0.4.0/mappymatch/maps/nx/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/maps/nx/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/maps/nx/readers/osm_readers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.514217 mappymatch-0.4.0/mappymatch/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.518217 mappymatch-0.4.0/mappymatch/matchers/lcss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/lcss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/lcss/constructs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/lcss/lcss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/lcss/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/lcss/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/line_snap.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/match_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/matcher_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/osrm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/matchers/valhalla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.518217 mappymatch-0.4.0/mappymatch/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.518217 mappymatch-0.4.0/mappymatch/resources/traces/
--rw-r--r--   0 runner    (1001) docker     (123)    22920 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/resources/traces/sample_trace_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/resources/traces/sample_trace_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    31962 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/resources/traces/sample_trace_3.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.522217 mappymatch-0.4.0/mappymatch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/utils/crs.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/utils/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/utils/process_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-11 21:44:24.000000 mappymatch-0.4.0/mappymatch/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.510217 mappymatch-0.4.0/mappymatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-11 21:44:36.000000 mappymatch-0.4.0/mappymatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-11 21:44:36.000000 mappymatch-0.4.0/mappymatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 21:44:36.000000 mappymatch-0.4.0/mappymatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-11 21:44:36.000000 mappymatch-0.4.0/mappymatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 21:44:36.000000 mappymatch-0.4.0/mappymatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-11 21:44:24.000000 mappymatch-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 21:44:36.526218 mappymatch-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 21:44:24.000000 mappymatch-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:44:36.526218 mappymatch-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_geofence.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_lcss_add_match_for_stationary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_lcss_compress.py
--rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_lcss_drop_stationary_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_lcss_find_stationary_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_lcss_forward_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_lcss_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_lcss_reverse_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_lcss_same_trajectory_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_match_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_osm.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_process_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-11 21:44:24.000000 mappymatch-0.4.0/tests/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.068137 mappymatch-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-17 20:18:22.000000 mappymatch-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 20:18:22.000000 mappymatch-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-17 20:18:38.068137 mappymatch-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-17 20:18:22.000000 mappymatch-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.052136 mappymatch-0.4.1/mappymatch/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.052136 mappymatch-0.4.1/mappymatch/constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/constructs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/constructs/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/constructs/geofence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/constructs/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/constructs/road.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/constructs/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.052136 mappymatch-0.4.1/mappymatch/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/maps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.056136 mappymatch-0.4.1/mappymatch/maps/igraph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/maps/igraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13041 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/maps/igraph/igraph_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/maps/map_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.056136 mappymatch-0.4.1/mappymatch/maps/nx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/maps/nx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11890 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/maps/nx/nx_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.056136 mappymatch-0.4.1/mappymatch/maps/nx/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/maps/nx/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/maps/nx/readers/osm_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.056136 mappymatch-0.4.1/mappymatch/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.060136 mappymatch-0.4.1/mappymatch/matchers/lcss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/lcss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/lcss/constructs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/lcss/lcss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/lcss/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/lcss/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/line_snap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/match_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/matcher_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/osrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/matchers/valhalla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.060136 mappymatch-0.4.1/mappymatch/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.060136 mappymatch-0.4.1/mappymatch/resources/traces/
+-rw-r--r--   0 runner    (1001) docker     (123)    22920 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/resources/traces/sample_trace_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/resources/traces/sample_trace_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    31962 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/resources/traces/sample_trace_3.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.064137 mappymatch-0.4.1/mappymatch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/utils/crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/utils/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/utils/process_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-17 20:18:22.000000 mappymatch-0.4.1/mappymatch/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.052136 mappymatch-0.4.1/mappymatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-17 20:18:38.000000 mappymatch-0.4.1/mappymatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-17 20:18:38.000000 mappymatch-0.4.1/mappymatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:18:38.000000 mappymatch-0.4.1/mappymatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-17 20:18:38.000000 mappymatch-0.4.1/mappymatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 20:18:38.000000 mappymatch-0.4.1/mappymatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-17 20:18:22.000000 mappymatch-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:18:38.068137 mappymatch-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:18:22.000000 mappymatch-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:18:38.068137 mappymatch-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_geofence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_lcss_add_match_for_stationary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_lcss_compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_lcss_drop_stationary_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_lcss_find_stationary_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_lcss_forward_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_lcss_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_lcss_reverse_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_lcss_same_trajectory_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_match_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_osm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_process_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-17 20:18:22.000000 mappymatch-0.4.1/tests/test_trace.py
```

### Comparing `mappymatch-0.4.0/LICENSE` & `mappymatch-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/PKG-INFO` & `mappymatch-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mappymatch
-Version: 0.4.0
+Version: 0.4.1
 Summary: Package for mapmatching.
 Author: National Renewable Energy Laboratory
 License: BSD 3-Clause License Copyright (c) 2022, Alliance for Sustainable Energy, LLC
 Project-URL: Homepage, https://github.com/NREL/mappymatch
 Keywords: GPS,map,match
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mappymatch-0.4.0/README.md` & `mappymatch-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/constructs/coordinate.py` & `mappymatch-0.4.1/mappymatch/constructs/coordinate.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/constructs/geofence.py` & `mappymatch-0.4.1/mappymatch/constructs/geofence.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/constructs/match.py` & `mappymatch-0.4.1/mappymatch/constructs/match.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/constructs/road.py` & `mappymatch-0.4.1/mappymatch/constructs/road.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/constructs/trace.py` & `mappymatch-0.4.1/mappymatch/constructs/trace.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/maps/igraph/igraph_map.py` & `mappymatch-0.4.1/mappymatch/maps/igraph/igraph_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Set, Union
 
 import igraph as ig
 import networkx as nx
 import numpy as np
 import rtree as rt
 from shapely.geometry import Point
 
@@ -98,14 +98,17 @@
         self._time_weight = time_weight
         self._geom_key = geom_key
         self._metadata_key = metadata_key
         self._crs_key = crs_key
         self._node_id_name = node_id_name
         self._edge_id_name = edge_id_name
 
+        # store the names of any additional added attributes
+        self._additional_attribute_names: Set[str] = set()
+
         self._build_rtree()
 
         # build mapping from mappymatch road id to igraph edge id
         self.road_mapping = {}
         for e in self.g.es:
             source_node_id = e.source_vertex[self._node_id_name]
             target_node_id = e.target_vertex[self._node_id_name]
@@ -135,14 +138,17 @@
             metadata = {}
         else:
             metadata = metadata.copy()
 
         metadata[self._dist_weight] = edge_data.get(self._dist_weight)
         metadata[self._time_weight] = edge_data.get(self._time_weight)
 
+        for attr in self._additional_attribute_names:
+            metadata[attr] = edge_data.get(attr)
+
         road = Road(
             RoadId(source_node_id, target_node_id, road_key),
             edge_data[self._geom_key],
             metadata=metadata,
         )
 
         return road
@@ -204,14 +210,15 @@
         """
         geom_updated = False
         for road_id, attrs in attributes.items():
             edge_id = self.road_mapping.get(road_id)
             if edge_id is None:
                 raise ValueError(f"Road id {road_id} not found in graph")
             for attr, val in attrs.items():
+                self._additional_attribute_names.add(attr)
                 if attr == self._geom_key:
                     geom_updated = True
                 self.g.es[edge_id][attr] = val
 
         if geom_updated:
             self._build_rtree()
```

### Comparing `mappymatch-0.4.0/mappymatch/maps/map_interface.py` & `mappymatch-0.4.1/mappymatch/maps/map_interface.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/maps/nx/nx_map.py` & `mappymatch-0.4.1/mappymatch/maps/nx/nx_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import json
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Set, Union
 
 import networkx as nx
 import numpy as np
 import rtree as rt
 import shapely.wkt as wkt
 from shapely.geometry import Point
 
@@ -68,14 +68,16 @@
 
         self._dist_weight = dist_weight
         self._time_weight = time_weight
         self._geom_key = geom_key
         self._metadata_key = metadata_key
         self._crs_key = crs_key
 
+        self._addtional_attribute_names: Set[str] = set()
+
         self._build_rtree()
 
     def _has_road_id(self, road_id: RoadId) -> bool:
         return self.g.has_edge(*road_id)
 
     def _build_road(
         self,
@@ -94,24 +96,26 @@
             metadata = {}
         else:
             metadata = metadata.copy()
 
         metadata[self._dist_weight] = edge_data.get(self._dist_weight)
         metadata[self._time_weight] = edge_data.get(self._time_weight)
 
+        for attr_name in self._addtional_attribute_names:
+            metadata[attr_name] = edge_data.get(attr_name)
+
         road = Road(
             road_id,
             edge_data[self._geom_key],
             metadata=metadata,
         )
 
         return road
 
     def _build_rtree(self):
-
         idx = rt.index.Index()
         for i, gtuple in enumerate(self.g.edges(data=True, keys=True)):
             u, v, k, d = gtuple
             road_id = RoadId(u, v, k)
             # road = self._build_road(u, v, k, d)
             geom = d[self._geom_key]
             box = geom.bounds
@@ -163,14 +167,18 @@
 
         Args:
             attributes: A dictionary mapping road ids to dictionaries of attributes
 
         Returns:
             None
         """
+        for attrs in attributes.values():
+            for attr_name in attrs.keys():
+                self._addtional_attribute_names.add(attr_name)
+
         nx.set_edge_attributes(self.g, attributes)
         self._build_rtree()
 
     @property
     def roads(self) -> List[Road]:
         roads = [
             self._build_road(RoadId(u, v, k))
```

### Comparing `mappymatch-0.4.0/mappymatch/maps/nx/readers/osm_readers.py` & `mappymatch-0.4.1/mappymatch/maps/nx/readers/osm_readers.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/matchers/lcss/constructs.py` & `mappymatch-0.4.1/mappymatch/matchers/lcss/constructs.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/matchers/lcss/lcss.py` & `mappymatch-0.4.1/mappymatch/matchers/lcss/lcss.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/matchers/lcss/ops.py` & `mappymatch-0.4.1/mappymatch/matchers/lcss/ops.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/matchers/lcss/utils.py` & `mappymatch-0.4.1/mappymatch/matchers/lcss/utils.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/matchers/line_snap.py` & `mappymatch-0.4.1/mappymatch/matchers/line_snap.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/matchers/match_result.py` & `mappymatch-0.4.1/mappymatch/matchers/match_result.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/matchers/matcher_interface.py` & `mappymatch-0.4.1/mappymatch/matchers/matcher_interface.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/matchers/osrm.py` & `mappymatch-0.4.1/mappymatch/matchers/osrm.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/matchers/valhalla.py` & `mappymatch-0.4.1/mappymatch/matchers/valhalla.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/resources/traces/sample_trace_1.csv` & `mappymatch-0.4.1/mappymatch/resources/traces/sample_trace_1.csv`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/resources/traces/sample_trace_2.csv` & `mappymatch-0.4.1/mappymatch/resources/traces/sample_trace_2.csv`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/resources/traces/sample_trace_3.csv` & `mappymatch-0.4.1/mappymatch/resources/traces/sample_trace_3.csv`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/utils/geo.py` & `mappymatch-0.4.1/mappymatch/utils/geo.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/utils/plot.py` & `mappymatch-0.4.1/mappymatch/utils/plot.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch/utils/process_trace.py` & `mappymatch-0.4.1/mappymatch/utils/process_trace.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/mappymatch.egg-info/PKG-INFO` & `mappymatch-0.4.1/mappymatch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mappymatch
-Version: 0.4.0
+Version: 0.4.1
 Summary: Package for mapmatching.
 Author: National Renewable Energy Laboratory
 License: BSD 3-Clause License Copyright (c) 2022, Alliance for Sustainable Energy, LLC
 Project-URL: Homepage, https://github.com/NREL/mappymatch
 Keywords: GPS,map,match
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mappymatch-0.4.0/mappymatch.egg-info/SOURCES.txt` & `mappymatch-0.4.1/mappymatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/pyproject.toml` & `mappymatch-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mappymatch"
-version = "0.4.0"
+version = "0.4.1"
 description = "Package for mapmatching."
 readme = "README.md"
 authors = [{ name = "National Renewable Energy Laboratory" }]
 license = { text = "BSD 3-Clause License Copyright (c) 2022, Alliance for Sustainable Energy, LLC" }
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Science/Research",
@@ -105,15 +105,15 @@
 
 [tool.tbump]
 # Uncomment  this if your project is hosted on GitHub:
 # github_url = "https://github.com/<user or organization>/<project>/"
 
 [tool.tbump.version]
 # Make sure this matches current_version before using tbump
-current = "0.4.0"
+current = "0.4.1"
 # Example of a semver regexp.
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `mappymatch-0.4.0/tests/test_coordinate.py` & `mappymatch-0.4.1/tests/test_coordinate.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/tests/test_lcss_add_match_for_stationary.py` & `mappymatch-0.4.1/tests/test_lcss_add_match_for_stationary.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/tests/test_lcss_compress.py` & `mappymatch-0.4.1/tests/test_lcss_compress.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/tests/test_lcss_drop_stationary_points.py` & `mappymatch-0.4.1/tests/test_lcss_drop_stationary_points.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/tests/test_lcss_find_stationary_points.py` & `mappymatch-0.4.1/tests/test_lcss_find_stationary_points.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/tests/test_lcss_forward_merge.py` & `mappymatch-0.4.1/tests/test_lcss_forward_merge.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/tests/test_lcss_merge.py` & `mappymatch-0.4.1/tests/test_lcss_merge.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/tests/test_lcss_reverse_merge.py` & `mappymatch-0.4.1/tests/test_lcss_reverse_merge.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/tests/test_lcss_same_trajectory_scheme.py` & `mappymatch-0.4.1/tests/test_lcss_same_trajectory_scheme.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/tests/test_match_result.py` & `mappymatch-0.4.1/tests/test_match_result.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/tests/test_osm.py` & `mappymatch-0.4.1/tests/test_osm.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/tests/test_process_trace.py` & `mappymatch-0.4.1/tests/test_process_trace.py`

 * *Files identical despite different names*

### Comparing `mappymatch-0.4.0/tests/test_trace.py` & `mappymatch-0.4.1/tests/test_trace.py`

 * *Files identical despite different names*

