# Comparing `tmp/activefires-pp-0.1.7.tar.gz` & `tmp/activefires-pp-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activefires-pp-0.1.7.tar", last modified: Wed Oct 26 12:21:40 2022, max compression
+gzip compressed data, was "activefires-pp-0.1.9.tar", last modified: Mon Jul 17 09:46:18 2023, max compression
```

## Comparing `activefires-pp-0.1.7.tar` & `activefires-pp-0.1.9.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 12:21:40.012298 activefires-pp-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/.git_archival.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 12:21:40.008298 activefires-pp-0.1.7/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 12:21:40.008298 activefires-pp-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2438 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/.github/workflows/deploy-sdist.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1844 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1780 2022-10-26 12:21:40.012298 activefires-pp-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/RELEASING.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 12:21:40.008298 activefires-pp-0.1.7/activefires_pp/
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1865 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/api_posting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    17249 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/fire_notifications.py
--rw-r--r--   0 runner    (1001) docker     (121)     2925 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/geojson_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3187 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/geometries_from_shapefiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)    26025 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/post_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)    22296 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/spatiotemporal_alarm_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 12:21:40.008298 activefires-pp-0.1.7/activefires_pp/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     9749 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/tests/test_api_posting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    12056 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/tests/test_fire_notifications.py
--rw-r--r--   0 runner    (1001) docker     (121)    16411 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/tests/test_fires_filtering.py
--rw-r--r--   0 runner    (1001) docker     (121)     7853 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/tests/test_geojson_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6396 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/tests/test_messaging.py
--rw-r--r--   0 runner    (1001) docker     (121)     4282 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/tests/test_shapefile_geometries.py
--rw-r--r--   0 runner    (1001) docker     (121)    29974 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/tests/test_spatiotemporal_alarm_filtering.py
--rw-r--r--   0 runner    (1001) docker     (121)     3380 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/activefires_pp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 12:21:40.008298 activefires-pp-0.1.7/activefires_pp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1780 2022-10-26 12:21:39.000000 activefires-pp-0.1.7/activefires_pp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-10-26 12:21:40.000000 activefires-pp-0.1.7/activefires_pp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 12:21:39.000000 activefires-pp-0.1.7/activefires_pp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 12:21:39.000000 activefires-pp-0.1.7/activefires_pp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-26 12:21:39.000000 activefires-pp-0.1.7/activefires_pp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-26 12:21:39.000000 activefires-pp-0.1.7/activefires_pp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 12:21:40.012298 activefires-pp-0.1.7/bin/
--rw-r--r--   0 runner    (1001) docker     (121)     4002 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/bin/active_fires_notifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     3187 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/bin/active_fires_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/bin/active_fires_spatiotemporal_alarm_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 12:21:40.012298 activefires-pp-0.1.7/continuous_integration/
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/continuous_integration/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 12:21:40.012298 activefires-pp-0.1.7/examples/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/examples/auth_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/examples/fire_notifier.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/examples/fire_notifier_regional.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/examples/fires_pp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/examples/log_config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/examples/spatio_temporal_alarm_filtering.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-10-26 12:21:40.012298 activefires-pp-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2737 2022-10-26 12:21:33.000000 activefires-pp-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.963641 activefires-pp-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/.git_archival.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.959641 activefires-pp-0.1.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.959641 activefires-pp-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/.github/workflows/deploy-sdist.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-17 09:46:18.963641 activefires-pp-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/RELEASING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.959641 activefires-pp-0.1.9/activefires_pp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/api_posting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/fire_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/geojson_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/geometries_from_shapefiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29911 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22296 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/spatiotemporal_alarm_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.963641 activefires-pp-0.1.9/activefires_pp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_api_posting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_fire_detection_id_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_fire_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21920 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_fires_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_geojson_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_messaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_shapefile_geometries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29974 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_spatiotemporal_alarm_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/activefires_pp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.959641 activefires-pp-0.1.9/activefires_pp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-17 09:46:18.000000 activefires-pp-0.1.9/activefires_pp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-17 09:46:18.000000 activefires-pp-0.1.9/activefires_pp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:46:18.000000 activefires-pp-0.1.9/activefires_pp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:46:18.000000 activefires-pp-0.1.9/activefires_pp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 09:46:18.000000 activefires-pp-0.1.9/activefires_pp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 09:46:18.000000 activefires-pp-0.1.9/activefires_pp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.963641 activefires-pp-0.1.9/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/bin/active_fires_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/bin/active_fires_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/bin/active_fires_spatiotemporal_alarm_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.963641 activefires-pp-0.1.9/continuous_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/continuous_integration/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:46:18.963641 activefires-pp-0.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/examples/auth_tokens.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/examples/fire_notifier.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/examples/fire_notifier_regional.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/examples/fires_pp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/examples/log_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/examples/spatio_temporal_alarm_filtering.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-17 09:46:18.963641 activefires-pp-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-17 09:46:14.000000 activefires-pp-0.1.9/setup.py
```

### Comparing `activefires-pp-0.1.7/.github/PULL_REQUEST_TEMPLATE.md` & `activefires-pp-0.1.9/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/.github/workflows/ci.yaml` & `activefires-pp-0.1.9/.github/workflows/ci.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -6,41 +6,57 @@
   test:
     runs-on: ${{ matrix.os }}
     continue-on-error: ${{ matrix.experimental }}
     strategy:
       fail-fast: true
       matrix:
         os: ["ubuntu-latest", "macos-latest"]
-        python-version: ["3.9", "3.10"]
+        python-version: ["3.9", "3.10", "3.11"]
         experimental: [false]
         include:
-          - python-version: "3.10"
+          - python-version: "3.11"
             os: "ubuntu-latest"
             experimental: true
 
     env:
       PYTHON_VERSION: ${{ matrix.python-version }}
       OS: ${{ matrix.os }}
       UNSTABLE: ${{ matrix.experimental }}
       ACTIONS_ALLOW_UNSECURE_COMMANDS: true
 
     steps:
       - name: Checkout source
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
 
       - name: Setup Conda Environment
         uses: conda-incubator/setup-miniconda@v2
         with:
-          miniconda-version: "latest"
+          miniforge-variant: Mambaforge
+          miniforge-version: latest
+          use-mamba: true
           python-version: ${{ matrix.python-version }}
-          mamba-version: "*"
-          channels: conda-forge,defaults
-          environment-file: continuous_integration/environment.yaml
           activate-environment: test-environment
 
+      - name: Set cache environment variables
+        shell: bash -l {0}
+        run: |
+          echo "DATE=$(date +'%Y%m%d')" >> $GITHUB_ENV
+          CONDA_PREFIX=$(python -c "import sys; print(sys.prefix)")
+          echo "CONDA_PREFIX=$CONDA_PREFIX" >> $GITHUB_ENV
+
+      - uses: actions/cache@v3
+        with:
+          path: ${{ env.CONDA_PREFIX }}
+          key: ${{ matrix.os }}-${{matrix.python-version}}-conda-${{ hashFiles('continuous_integration/environment.yaml') }}-${{ env.DATE }}-${{matrix.experimental}}-${{ env.CACHE_NUMBER }}
+        id: cache
+
+      - name: Update environment
+        run: mamba env update -n test-environment -f continuous_integration/environment.yaml
+        if: steps.cache.outputs.cache-hit != 'true'
+
       - name: Install unstable dependencies
         if: matrix.experimental == true
         shell: bash -l {0}
         run: |
           python -m pip install \
           --no-deps --pre --upgrade \
           matplotlib \
```

### Comparing `activefires-pp-0.1.7/.gitignore` & `activefires-pp-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/CHANGELOG.md` & `activefires-pp-0.1.9/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+## Version <v0.1.9> (2023/07/17)
+
+## Version <v0.1.8> (2023/07/14)
+
+
+### Pull Requests Merged
+
+#### Bugs fixed
+
+* [PR 14](https://github.com/adybbroe/activefires-pp/pull/14) - Bugfix multipolygon treatment and adapt to latest Shapely
+
+#### Features added
+
+* [PR 16](https://github.com/adybbroe/activefires-pp/pull/16) - Feature add unique detection
+* [PR 14](https://github.com/adybbroe/activefires-pp/pull/14) - Bugfix multipolygon treatment and adapt to latest Shapely
+
+In this release 3 pull requests were closed.
+
+
 ## Version <v0.1.7> (2022/10/24)
 
 
 ### Pull Requests Merged
 
 #### Features added
```

### Comparing `activefires-pp-0.1.7/LICENSE` & `activefires-pp-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/PKG-INFO` & `activefires-pp-0.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: activefires-pp
-Version: 0.1.7
+Version: 0.1.9
 Summary: Post-processing of and notifications on Satellite active fire detections
 Home-page: https://github.com/adybbroe/activefires-pp
 Author: Adam Dybroe
 Author-email: adam.dybroe@smhi.se
 License: GPLv3
-Description: activefires-pp
-        ==============
-        
-        [![Build status](https://github.com/adybbroe/activefires-pp/workflows/CI/badge.svg?branch=main)](https://github.com/adybbroe/activefires-pp/workflows/CI/badge.svg?branch=main)
-        [![Coverage Status](https://coveralls.io/repos/github/adybbroe/activefires-pp/badge.svg)](https://coveralls.io/github/adybbroe/activefires-pp)
-        
-        Post-processing (including regional filtering) of Satellite Active Fires and notify end-users
-        Supports reading and processing VIIRS Active Fires EDR. There is support for filtering out fire
-        detections using three different levels:
-        
-          * National filtering, where all detections outside boarders as given by a shapefile are left out
-        
-          * Filtering to exclude fire detections inside a set of polygons (meant to
-            define populated areas and local industries known to be heat sources that
-            can turn up as detections) from a shapefile
-        
-          * Regional filtering, where detections are localisized in regions and output
-            messages are treated accordingly.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
+License-File: LICENSE
+
+activefires-pp
+==============
+
+[![Build status](https://github.com/adybbroe/activefires-pp/workflows/CI/badge.svg?branch=main)](https://github.com/adybbroe/activefires-pp/workflows/CI/badge.svg?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/adybbroe/activefires-pp/badge.svg)](https://coveralls.io/github/adybbroe/activefires-pp)
+
+Post-processing (including regional filtering) of Satellite Active Fires and notify end-users
+Supports reading and processing VIIRS Active Fires EDR. There is support for filtering out fire
+detections using three different levels:
+
+  * National filtering, where all detections outside boarders as given by a shapefile are left out
+
+  * Filtering to exclude fire detections inside a set of polygons (meant to
+    define populated areas and local industries known to be heat sources that
+    can turn up as detections) from a shapefile
+
+  * Regional filtering, where detections are localisized in regions and output
+    messages are treated accordingly.
+
+
```

### Comparing `activefires-pp-0.1.7/README.md` & `activefires-pp-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/RELEASING.md` & `activefires-pp-0.1.9/RELEASING.md`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/activefires_pp/__init__.py` & `activefires-pp-0.1.9/activefires_pp/__init__.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/activefires_pp/api_posting.py` & `activefires-pp-0.1.9/activefires_pp/api_posting.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/activefires_pp/config.py` & `activefires-pp-0.1.9/activefires_pp/config.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/activefires_pp/fire_notifications.py` & `activefires-pp-0.1.9/activefires_pp/fire_notifications.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/activefires_pp/geojson_utils.py` & `activefires-pp-0.1.9/activefires_pp/geojson_utils.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/activefires_pp/geometries_from_shapefiles.py` & `activefires-pp-0.1.9/activefires_pp/geometries_from_shapefiles.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2021, 2022 Adam.Dybbroe
+# Copyright (c) 2021, 2022, 2023 Adam.Dybbroe
 
 # Author(s):
 
 #   Adam Dybbroe <Firstname.Lastname at smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -30,16 +30,16 @@
 
 class ShapeGeometry(object):
     """Geometry from a shape file."""
 
     def __init__(self, shapefilepath, globstr='*.shp'):
         """Initialize the ShapeGeometry class."""
         self.filepaths = _get_shapefile_paths(shapefilepath, globstr)
-        self.geometries = None
-        self.attributes = None
+        self.geometries = []
+        self.attributes = []
         self._get_proj()
 
     def load(self):
         """Load the geometries and the associated attributes."""
         records = []
         for filepath in self.filepaths:
             records = records + [r for r in shpreader.Reader(filepath).records()]
@@ -48,15 +48,15 @@
         self._load_member_from_records('geometries', 'geometry')
         self._load_member_from_records('attributes', 'attributes')
 
     def _get_proj(self):
         """Get and return the Proj.4 string."""
         self.proj4str = []
         for filepath in self.filepaths:
-            prj_filename = filepath.strip('.shp') + '.prj'
+            prj_filename = _get_proj_filename_from_shapefile(filepath)
             crs = pycrs.load.from_file(prj_filename)
             if crs.name == 'SWEREF99_TM' and crs.proj.name.proj4 == 'utm':
                 utm_zone_proj4 = ' +zone=33'
                 proj4str = crs.to_proj4() + utm_zone_proj4
             else:
                 proj4str = crs.to_proj4()
             self.proj4str.append(proj4str)
@@ -82,7 +82,11 @@
     if os.path.isfile(path):
         return [path]
 
     shapefile_paths = glob(os.path.join(path, globstr))
     if len(shapefile_paths) == 0:
         raise OSError('No matching shapefiles found on disk. Path = %s, glob-string = %s', path, globstr)
     return shapefile_paths
+
+
+def _get_proj_filename_from_shapefile(filepath):
+    return filepath.split('.shp')[0] + '.prj'
```

### Comparing `activefires-pp-0.1.7/activefires_pp/logger.py` & `activefires-pp-0.1.9/activefires_pp/logger.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/activefires_pp/post_processing.py` & `activefires-pp-0.1.9/activefires_pp/post_processing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2021 - 2022 Adam.Dybbro
+# Copyright (c) 2021 - 2023 Adam.Dybbro
 
 # Author(s):
 
 #   Adam Dybbroe <Firstname.Lastname@smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -65,14 +65,16 @@
 # column 4: Along-scan fire pixel resolution (km)
 # column 5: Along-track fire pixel resolution (km)
 # column 6: detection confidence ([7,8,9]->[lo,med,hi])
 # column 7: fire radiative power (MW)
 #
 COL_NAMES = ["latitude", "longitude", "tb", "along_scan_res", "along_track_res", "conf", "power"]
 
+NO_FIRES_TEXT = 'No fire detections for this granule'
+
 
 logger = logging.getLogger(__name__)
 logging.getLogger("fiona").setLevel(logging.WARNING)
 
 
 class ActiveFiresShapefileFiltering(object):
     """Reading, filtering and writing Active Fire detections.
@@ -152,18 +154,18 @@
         """
         detections = self._afdata
 
         lons = detections.longitude.values
         lats = detections.latitude.values
 
         toc = time.time()
-        insides = get_global_mask_from_shapefile(shapefile, (lons, lats), start_geometries_index)
+        points_inside = get_global_mask_from_shapefile(shapefile, (lons, lats), start_geometries_index)
         logger.debug("Time used checking inside polygon - mpl path method: %f", time.time() - toc)
 
-        self._afdata = detections[insides == inside]
+        self._afdata = detections[points_inside == inside]
 
         if len(self._afdata) == 0:
             logger.debug("No fires after filtering on Polygon...")
         else:
             logger.debug("Number of detections after filtering on Polygon: %d", len(self._afdata))
 
     def get_regional_filtermasks(self, shapefile, globstr):
@@ -247,16 +249,16 @@
         detections.to_csv(output_filename, index=False)
         return output_filename
     else:
         logger.debug("No detections to save!")
         return None
 
 
-def store_geojson(output_filename, detections, platform_name=None):
-    """Store the filtered AF detections in Geojson format on disk."""
+def geojson_feature_collection_from_detections(detections, platform_name=None):
+    """Create the Geojson feature collection from fire detection data."""
     if len(detections) == 0:
         logger.debug("No detections to save!")
         return None
 
     # Convert points to GeoJSON
     features = []
     for idx in range(len(detections)):
@@ -264,80 +266,76 @@
         endtime = detections.iloc[idx].endtime
         mean_granule_time = starttime.to_pydatetime() + (endtime.to_pydatetime() -
                                                          starttime.to_pydatetime()) / 2.
 
         prop = {'power': detections.iloc[idx].power,
                 'tb': detections.iloc[idx].tb,
                 'confidence': int(detections.iloc[idx].conf),
+                'id': detections.iloc[idx].detection_id,
                 'observation_time': json_serial(mean_granule_time)
                 }
         if platform_name:
             prop['platform_name'] = platform_name
         else:
             logger.debug("No platform name specified for output")
 
         feat = Feature(
             geometry=Point(map(float, [detections.iloc[idx].longitude, detections.iloc[idx].latitude])),
             properties=prop)
         features.append(feat)
 
-    feature_collection = FeatureCollection(features)
+    return FeatureCollection(features)
+
+
+def store_geojson(output_filename, feature_collection):
+    """Store the Geojson feature collection of fire detections on disk."""
     path = os.path.dirname(output_filename)
     if not os.path.exists(path):
         logger.info("Create directory: %s", path)
         os.makedirs(path)
 
     with open(output_filename, 'w') as fpt:
         dump(feature_collection, fpt)
 
-    return output_filename
 
-
-def get_mask_from_multipolygon(points, geometry):
+def get_mask_from_multipolygon(points, geometry, start_idx=1):
     """Get mask for points from a shapely Multipolygon."""
     shape = geometry.geoms[0]
     pth = Path(shape.exterior.coords)
     mask = pth.contains_points(points)
 
     if sum(mask) == len(points):
         return mask
 
-    for shape in geometry.geoms[1:]:
+    constituent_part = geometry.geoms[start_idx:]
+    for shape in constituent_part.geoms:
         pth = Path(shape.exterior.coords)
         mask = np.logical_or(mask, pth.contains_points(points))
         if sum(mask) == len(points):
             break
 
     return mask
 
 
 def get_global_mask_from_shapefile(shapefile, lonlats, start_geom_index=0):
     """Given geographical (lon,lat) points get a mask to apply when filtering."""
     lons, lats = lonlats
-
-    logger.debug("Getting the global mask from file: shapefile file path = %s" % str(shapefile))
+    logger.debug("Getting the global mask from file: shapefile file path = %s", str(shapefile))
     shape_geom = ShapeGeometry(shapefile)
     shape_geom.load()
 
     p__ = pyproj.Proj(shape_geom.proj4str)
 
     # There is only one geometry/multi-polygon!
     geometry = shape_geom.geometries[0]
 
     metersx, metersy = p__(lons, lats)
     points = np.vstack([metersx, metersy]).T
 
-    shape = geometry.geoms[0]
-    pth = Path(shape.exterior.coords)
-    mask = pth.contains_points(points)
-    for shape in geometry.geoms[start_geom_index:]:
-        pth = Path(shape.exterior.coords)
-        mask = np.logical_or(mask, pth.contains_points(points))
-
-    return mask
+    return get_mask_from_multipolygon(points, geometry, start_geom_index)
 
 
 class ActiveFiresPostprocessing(Thread):
     """The active fires post processor."""
 
     def __init__(self, configfile, shp_borders, shp_mask, regional_filtermask=None):
         """Initialize the active fires post processor class."""
@@ -349,27 +347,30 @@
         self.configfile = configfile
         self.options = {}
 
         config = read_config(self.configfile)
         self._set_options_from_config(config)
 
         self.host = socket.gethostname()
-
         self.timezone = self.options.get('timezone', 'GMT')
 
         self.input_topic = self.options['subscribe_topics'][0]
         self.output_topic = self.options['publish_topic']
         self.infile_pattern = self.options.get('af_pattern_ibands')
         self.outfile_pattern_national = self.options.get('geojson_file_pattern_national')
         self.outfile_pattern_regional = self.options.get('geojson_file_pattern_regional')
         self.output_dir = self.options.get('output_dir', '/tmp')
+        self.filepath_detection_id_cache = self.options.get('filepath_detection_id_cache')
 
         frmt = self.options['regional_shapefiles_format']
         self.regional_shapefiles_globstr = globify(frmt)
 
+        self._fire_detection_id = None
+        self._initialize_fire_detection_id()
+
         self.listener = None
         self.publisher = None
         self.loop = False
         self._setup_and_start_communication()
 
     def _setup_and_start_communication(self):
         """Set up the Posttroll communication and start the publisher."""
@@ -405,77 +406,110 @@
                     publish_topics.remove(item)
             self.options['publish_topics'] = publish_topics
 
     def signal_shutdown(self, *args, **kwargs):
         """Shutdown the Active Fires postprocessing."""
         self.close()
 
+    def check_incoming_message_and_get_filename(self, msg):
+        """Check the message content and return filename if okay."""
+        if msg.type not in ['file', 'collection', 'dataset']:
+            logger.debug("Message type not supported: %s", str(msg.type))
+            return None
+
+        filename = get_filename_from_uri(msg.data.get('uri'))
+        if not os.path.exists(filename):
+            logger.warning("File does not exist: %s", filename)
+            return None
+
+        file_ok = check_file_type_okay(msg.data.get('type'))
+        if not file_ok:
+            output_messages = self._generate_no_fires_messages(msg, NO_FIRES_TEXT)
+            for output_msg in output_messages:
+                logger.debug("Sending message: %s", str(output_msg))
+                self.publisher.send(str(output_msg))
+            return None
+
+        return filename
+
+    def do_postprocessing_on_message(self, msg, filename):
+        """Do the fires post processing on a message."""
+        platform_name = msg.data.get('platform_name')
+        af_shapeff = ActiveFiresShapefileFiltering(filename, platform_name=platform_name,
+                                                   timezone=self.timezone)
+        afdata = af_shapeff.get_af_data(self.infile_pattern)
+        if len(afdata) == 0:
+            output_messages = self._generate_no_fires_messages(msg, NO_FIRES_TEXT)
+            for output_msg in output_messages:
+                logger.debug("Sending message: %s", str(output_msg))
+                self.publisher.send(str(output_msg))
+            return
+
+        afdata = self.fires_filtering(msg, af_shapeff)
+        logger.debug("After fires_filtering...: Number of fire detections = %d", len(afdata))
+        if len(afdata) == 0:
+            logger.debug("No fires - so no regional filtering to be done!")
+            return
+
+        # It is here that we should add a uniue day-ID to each of the detections!
+        afdata = self.add_unique_day_id(afdata)
+        self.save_id_to_file()
+
+        # 1) Create geojson feature collection
+        # 2) Dump geojson data to disk
+        feature_collection = geojson_feature_collection_from_detections(afdata,
+                                                                        platform_name=af_shapeff.platform_name)
+
+        fmda = af_shapeff.metadata
+        pout = Parser(self.outfile_pattern_national)
+        out_filepath = os.path.join(self.output_dir, pout.compose(fmda))
+        logger.debug("Output file path = %s", out_filepath)
+
+        if feature_collection is None:
+            logger.info("No geojson file created, number of fires after filtering = %d", len(afdata))
+            output_messages = self._generate_no_fires_messages(msg,
+                                                               'No true fire detections inside National borders')  # noqa
+        else:
+            store_geojson(out_filepath, feature_collection)
+            output_messages = self.get_output_messages(out_filepath, msg, len(afdata))
+
+        for output_msg in output_messages:
+            if output_msg:
+                logger.debug("Sending message: %s", str(output_msg))
+                self.publisher.send(str(output_msg))
+
+        # Do the regional filtering now:
+        if not self.regional_filtermask:
+            logger.info("No regional filtering is attempted.")
+            return
+
+        # FIXME! If afdata is empty (len=0) then it seems all data are inside all regions!
+        af_shapeff = ActiveFiresShapefileFiltering(afdata=afdata, platform_name=platform_name,
+                                                   timezone=self.timezone)
+        regional_fmask = af_shapeff.get_regional_filtermasks(self.regional_filtermask,
+                                                             globstr=self.regional_shapefiles_globstr)
+        regional_messages = self.regional_fires_filtering_and_publishing(msg, regional_fmask, af_shapeff)
+        for region_msg in regional_messages:
+            logger.debug("Sending message: %s", str(region_msg))
+            self.publisher.send(str(region_msg))
+
     def run(self):
         """Run the AF post processing."""
         while self.loop:
             try:
                 msg = self.listener.output_queue.get(timeout=1)
                 logger.debug("Message: %s", str(msg.data))
             except Empty:
                 continue
             else:
-                if msg.type not in ['file', 'collection', 'dataset']:
-                    logger.debug("Message type not supported: %s", str(msg.type))
+                filename = self.check_incoming_message_and_get_filename(msg)
+                if not filename:
                     continue
 
-                platform_name = msg.data.get('platform_name')
-                filename = get_filename_from_uri(msg.data.get('uri'))
-                if not os.path.exists(filename):
-                    logger.warning("File does not exist!")
-                    continue
-
-                file_ok = check_file_type_okay(msg.data.get('type'))
-                no_fires_text = 'No fire detections for this granule'
-                output_messages = self._generate_no_fires_messages(msg, no_fires_text)
-                if not file_ok:
-                    for output_msg in output_messages:
-                        logger.debug("Sending message: %s", str(output_msg))
-                        self.publisher.send(str(output_msg))
-                    continue
-
-                af_shapeff = ActiveFiresShapefileFiltering(filename, platform_name=platform_name,
-                                                           timezone=self.timezone)
-                afdata = af_shapeff.get_af_data(self.infile_pattern)
-
-                if len(afdata) == 0:
-                    logger.debug("Sending message: %s", str(output_msg))
-                    self.publisher.send(str(output_msg))
-                    continue
-
-                output_messages, afdata = self.fires_filtering(msg, af_shapeff)
-                logger.debug("After fires_filtering...: Number of messages = %d", len(output_messages))
-
-                for output_msg in output_messages:
-                    if output_msg:
-                        logger.debug("Sending message: %s", str(output_msg))
-                        self.publisher.send(str(output_msg))
-
-                # Do the regional filtering now:
-                if not self.regional_filtermask:
-                    logger.info("No regional filtering is attempted.")
-                    continue
-
-                if len(afdata) == 0:
-                    logger.debug("No fires - so no regional filtering to be done!")
-                    continue
-
-                # FIXME! If afdata is empty (len=0) then it seems all data are inside all regions!
-                af_shapeff = ActiveFiresShapefileFiltering(afdata=afdata, platform_name=platform_name,
-                                                           timezone=self.timezone)
-                regional_fmask = af_shapeff.get_regional_filtermasks(self.regional_filtermask,
-                                                                     globstr=self.regional_shapefiles_globstr)
-                regional_messages = self.regional_fires_filtering_and_publishing(msg, regional_fmask, af_shapeff)
-                for region_msg in regional_messages:
-                    logger.debug("Sending message: %s", str(region_msg))
-                    self.publisher.send(str(region_msg))
+                self.do_postprocessing_on_message(msg, filename)
 
     def regional_fires_filtering_and_publishing(self, msg, regional_fmask, afsff_obj):
         """From the regional-fires-filter-mask and the fire detection data send regional messages."""
         logger.debug("Perform regional masking on VIIRS AF detections and publish accordingly.")
 
         afdata = afsff_obj.get_af_data()
         fmda = afsff_obj.metadata
@@ -492,21 +526,26 @@
 
             regions_with_detections = regions_with_detections + 1
             fmda['region_name'] = regional_fmask[region_name]['attributes']['Kod_omr']
 
             out_filepath = os.path.join(self.output_dir, pout.compose(fmda))
             logger.debug("Output file path = %s", out_filepath)
             data_in_region = afdata[regional_fmask[region_name]['mask']]
-            filepath = store_geojson(out_filepath, data_in_region, platform_name=fmda['platform'])
-            if not filepath:
+
+            # filepath = store_geojson(out_filepath, data_in_region, platform_name=fmda['platform'])
+            feature_collection = geojson_feature_collection_from_detections(data_in_region,
+                                                                            platform_name=fmda['platform'])
+            if feature_collection is None:
                 logger.warning("Something wrong happended storing regional " +
                                "data to Geojson - area: {name}".format(name=str(region_name)))
                 continue
 
-            outmsg = self._generate_output_message(filepath, msg, regional_fmask[region_name])
+            store_geojson(out_filepath, feature_collection)
+
+            outmsg = self._generate_output_message(out_filepath, msg, regional_fmask[region_name])
             output_messages.append(outmsg)
             logger.info("Geojson file created! Number of fires in region = %d", len(data_in_region))
 
         logger.debug("Regional masking done. Number of regions with fire " +
                      "detections on this granule: %s" % str(regions_with_detections))
         return output_messages
 
@@ -534,28 +573,20 @@
 
         if len(afdata_ff) > 0:
             logger.debug("Doing the fires filtering: shapefile-mask = %s", str(self.shp_filtermask))
             af_shapeff.fires_filtering(self.shp_filtermask, start_geometries_index=0, inside=False)
             afdata_ff = af_shapeff.get_af_data()
             logger.debug("After fires_filtering: Number of fire detections left: %d", len(afdata_ff))
 
-        filepath = store_geojson(out_filepath, afdata_ff, platform_name=af_shapeff.platform_name)
-        out_messages = self.get_output_messages(filepath, msg, len(afdata_ff))
-
-        return out_messages, afdata_ff
+        return afdata_ff
 
     def get_output_messages(self, filepath, msg, number_of_data):
         """Generate the adequate output message(s) depending on if an output file was created or not."""
-        if filepath:
-            logger.info("geojson file created! Number of fires after filtering = %d", number_of_data)
-            return [self._generate_output_message(filepath, msg)]
-        else:
-            logger.info("No geojson file created, number of fires after filtering = %d", number_of_data)
-            return self._generate_no_fires_messages(msg,
-                                                    'No true fire detections inside National borders')
+        logger.info("Geojson file created! Number of fires = %d", number_of_data)
+        return [self._generate_output_message(filepath, msg)]
 
     def _generate_output_message(self, filepath, input_msg, region=None):
         """Create the output message to publish."""
         output_topic = generate_posttroll_topic(self.output_topic, region)
         to_send = prepare_posttroll_message(input_msg, region)
         to_send['uri'] = ('ssh://%s/%s' % (self.host, filepath))
         to_send['uid'] = os.path.basename(filepath)
@@ -577,18 +608,78 @@
         return publish_messages
 
     def _check_borders_shapes_exists(self):
         """Check that the national borders shapefile exists on disk."""
         if not os.path.exists(self.shp_borders):
             raise OSError("Shape file does not exist! Filename = %s" % self.shp_borders)
 
+    def _initialize_fire_detection_id(self):
+        """Initialize the fire detection ID."""
+        if self.filepath_detection_id_cache and os.path.exists(self.filepath_detection_id_cache):
+            self._fire_detection_id = self.get_id_from_file()
+        else:
+            self._fire_detection_id = {'date': datetime.utcnow(), 'counter': 0}
+
+    def update_fire_detection_id(self):
+        """Update the fire detection ID registry."""
+        now = datetime.utcnow()
+        tdelta = now - self._fire_detection_id['date']
+        if tdelta.total_seconds() > 24*3600:
+            self._initialize_fire_detection_id()
+        elif tdelta.total_seconds() > 0 and self._fire_detection_id['date'].day != now.day:
+            self._initialize_fire_detection_id()
+
+        self._fire_detection_id['counter'] = self._fire_detection_id['counter'] + 1
+
+    def save_id_to_file(self):
+        """Save the (current) detection id on disk.
+
+        It is assumed that the user permissions are so that a file can actually
+        be written to disk here!
+        """
+        with open(self.filepath_detection_id_cache, 'w') as fpt:
+            id_ = self._create_id_string()
+            fpt.write(id_)
+
+    def get_id_from_file(self):
+        """Read the latest stored detection id string from disk and convert to internal format."""
+        with open(self.filepath_detection_id_cache, 'r') as fpt:
+            idstr = fpt.read()
+
+        return self._get_id_from_string(idstr)
+
+    def _get_id_from_string(self, idstr):
+        """Get the detection id from string."""
+        datestr, counter = idstr.split('-')
+        return {'date': datetime.strptime(datestr, '%Y%m%d'),
+                'counter': int(counter)}
+
+    def _create_id_string(self):
+        """From the internal fire detection id create the id string to be exposed to the user."""
+        return (self._fire_detection_id['date'].strftime('%Y%m%d') +
+                '-' + str(self._fire_detection_id['counter']))
+
+    def add_unique_day_id(self, afdata):
+        """Add a unique detection id - date + a running number for the day."""
+        # Add id's to the detections:
+        id_list = []
+        for _i in range(len(afdata)):
+            self.update_fire_detection_id()
+            id_ = self._create_id_string()
+            id_list.append(id_)
+
+        afdata['detection_id'] = id_list
+        return afdata
+
     def close(self):
         """Shutdown the Active Fires postprocessing."""
         logger.info('Terminating Active Fires post processing.')
         self.loop = False
+        logger.info('Dumping the latest detection id to disk: %s', str(self.filepath_detection_id_cache))
+        self.save_id_to_file()
         try:
             self.listener.stop()
         except Exception:
             logger.exception("Couldn't stop listener.")
         if self.publisher:
             try:
                 self.publisher.stop()
```

### Comparing `activefires-pp-0.1.7/activefires_pp/spatiotemporal_alarm_filtering.py` & `activefires-pp-0.1.9/activefires_pp/spatiotemporal_alarm_filtering.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/activefires_pp/tests/conftest.py` & `activefires-pp-0.1.9/activefires_pp/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/activefires_pp/tests/test_api_posting.py` & `activefires-pp-0.1.9/activefires_pp/tests/test_api_posting.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/activefires_pp/tests/test_config.py` & `activefires-pp-0.1.9/activefires_pp/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/activefires_pp/tests/test_fire_notifications.py` & `activefires-pp-0.1.9/activefires_pp/tests/test_fire_notifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2021, 2022 Adam Dybbroe
+# Copyright (c) 2021 - 2023 Adam Dybbroe
 
 # Author(s):
 
 #   Adam Dybbroe <Adam Dybbroe at smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -16,22 +16,21 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit testing the fire notifications.
-"""
+"""Unit testing the fire notifications."""
 
 import unittest
 from unittest.mock import patch
 import yaml
 import io
-from posttroll.message import Message
+# from posttroll.message import Message
 
 from activefires_pp.fire_notifications import EndUserNotifier
 from activefires_pp.fire_notifications import EndUserNotifierRegional
 from activefires_pp.fire_notifications import get_recipients_for_region
 
 TEST_CONFIG_FILE = "/home/a000680/usr/src/forks/activefires-pp/examples/fire_notifier.yaml"
 TEST_CONFIG_FILE_REGIONAL = "/home/a000680/usr/src/forks/activefires-pp/examples/fire_notifier_regional.yaml"
@@ -95,37 +94,40 @@
   - observation_time
 
 unsubscribe:
   address: unsubscribe@mydomain.xx
   text: 'Stop being bothered: Send a note to unsubscribe@mydomain.xx'
 """
 
-REGIONAL_TEST_MESSAGE = """pytroll://VIIRS/L2/Fires/PP/Regional/0114 file safusr.u@lxserv1043.smhi.se 2021-04-19T11:16:49.542021 v1.01 application/json {"start_time": "2021-04-16T12:29:53", "end_time": "2021-04-16T12:31:18", "orbit_number": 1, "platform_name": "NOAA-20", "sensor": "viirs", "data_processing_level": "2", "variant": "DR", "orig_orbit_number": 17666, "region_name": "Storstockholms brandf\u00f6rsvar", "region_code": "0114", "uri": "ssh://lxserv1043.smhi.se//san1/polar_out/direct_readout/viirs_active_fires/filtered/AFIMG_NOAA-20_d20210416_t122953_0114.geojson", "uid": "AFIMG_NOAA-20_d20210416_t122953_0114.geojson", "type": "GEOJSON-filtered", "format": "geojson", "product": "afimg"}"""
+REGIONAL_TEST_MESSAGE = """pytroll://VIIRS/L2/Fires/PP/Regional/0114 file safusr.u@lxserv1043.smhi.se 2021-04-19T11:16:49.542021 v1.01 application/json {"start_time": "2021-04-16T12:29:53", "end_time": "2021-04-16T12:31:18", "orbit_number": 1, "platform_name": "NOAA-20", "sensor": "viirs", "data_processing_level": "2", "variant": "DR", "orig_orbit_number": 17666, "region_name": "Storstockholms brandf\u00f6rsvar", "region_code": "0114", "uri": "ssh://lxserv1043.smhi.se//san1/polar_out/direct_readout/viirs_active_fires/filtered/AFIMG_NOAA-20_d20210416_t122953_0114.geojson", "uid": "AFIMG_NOAA-20_d20210416_t122953_0114.geojson", "type": "GEOJSON-filtered", "format": "geojson", "product": "afimg"}"""  # noqa
 
-NATIONAL_TEST_MESSAGE = """pytroll://VIIRS/L2/Fires/PP/National file safusr.u@lxserv1043.smhi.se 2021-04-19T11:16:49.519087 v1.01 application/json {"start_time": "2021-04-16T12:29:53", "end_time": "2021-04-16T12:31:18", "orbit_number": 1, "platform_name": "NOAA-20", "sensor": "viirs", "data_processing_level": "2", "variant": "DR", "orig_orbit_number": 17666, "uri": "ssh://lxserv1043.smhi.se//san1/polar_out/direct_readout/viirs_active_fires/filtered/AFIMG_j01_d20210416_t122953.geojson", "uid": "AFIMG_j01_d20210416_t122953.geojson", "type": "GEOJSON-filtered", "format": "geojson", "product": "afimg"}"""
+NATIONAL_TEST_MESSAGE = """pytroll://VIIRS/L2/Fires/PP/National file safusr.u@lxserv1043.smhi.se 2021-04-19T11:16:49.519087 v1.01 application/json {"start_time": "2021-04-16T12:29:53", "end_time": "2021-04-16T12:31:18", "orbit_number": 1, "platform_name": "NOAA-20", "sensor": "viirs", "data_processing_level": "2", "variant": "DR", "orig_orbit_number": 17666, "uri": "ssh://lxserv1043.smhi.se//san1/polar_out/direct_readout/viirs_active_fires/filtered/AFIMG_j01_d20210416_t122953.geojson", "uid": "AFIMG_j01_d20210416_t122953.geojson", "type": "GEOJSON-filtered", "format": "geojson", "product": "afimg"}"""  # noqa
 
 
 class MyNetrcMock(object):
+    """Mocking the handling of secrets via the .netrc file."""
 
     def __init__(self):
-
+        """Initialize the netrc mock class."""
         self.hosts = {'default': ('my_user', None, 'my_passwd')}
 
     def authenticators(self, host):
+        """Return authentication for host."""
         return self.hosts.get(host)
 
 
 class TestNotifyEndUsers(unittest.TestCase):
+    """Test notifications on National fires."""
 
     @patch('activefires_pp.fire_notifications.netrc')
     @patch('activefires_pp.fire_notifications.socket.gethostname')
     @patch('activefires_pp.fire_notifications.read_config')
     @patch('activefires_pp.fire_notifications.EndUserNotifier._setup_and_start_communication')
     def test_get_options_national_filtering(self, setup_comm, read_config, gethostname, netrc):
-
+        """Test get the config options for National fires filtering."""
         secrets = MyNetrcMock()
         netrc.return_value = secrets
         gethostname.return_value = 'default'
 
         myconfigfile = "/my/config/file/path"
         natstream = io.StringIO(NAT_CONFIG)
 
@@ -162,21 +164,22 @@
         self.assertListEqual(this.fire_data, ['power', 'observation_time'])
         assert this.unsubscribe_address == 'unsubscribe@mydomain.xx'
         assert this.input_topic == 'VIIRS/L2/Fires/PP/National'
         assert this.output_topic == 'VIIRS/L2/MSB/National'
 
 
 class TestNotifyEndUsersRegional(unittest.TestCase):
+    """Test the regional notifications."""
 
     @patch('activefires_pp.fire_notifications.netrc')
     @patch('activefires_pp.fire_notifications.socket.gethostname')
     @patch('activefires_pp.fire_notifications.read_config')
     @patch('activefires_pp.fire_notifications.EndUserNotifierRegional._setup_and_start_communication')
     def test_get_options_regional_filtering(self, setup_comm, read_config, gethostname, netrc):
-
+        """Test get the config options for regional filtering."""
         secrets = MyNetrcMock()
         netrc.return_value = secrets
         gethostname.return_value = 'default'
 
         myconfigfile = "/my/config/file/path"
         regstream = io.StringIO(REG_CONFIG)
 
@@ -224,29 +227,28 @@
         # assert this.subject is None
         # assert this.max_number_of_fires_in_sms == 3
         # self.assertListEqual(this.fire_data, ['power', 'observation_time'])
         # assert this.unsubscribe_address == 'unsubscribe@mydomain.xx'
         # assert this.input_topic == 'VIIRS/L2/Fires/PP/Regional'
         # assert this.output_topic == 'VIIRS/L2/MSB/Regional'
 
-        input_msg = Message.decode(rawstr=REGIONAL_TEST_MESSAGE)
+        # input_msg = Message.decode(rawstr=REGIONAL_TEST_MESSAGE)
         # this.notify_end_users(input_msg)
 
         # ffdata = {"features": [{"geometry": {"coordinates": [17.198933, 59.577972], "type": "Point"},
         #                        "properties": {"observation_time": "2021-04-16T14:30:35.900000",
         #                                       "platform_name": "NOAA-20", "power": 5.53501701, "tb": 367.0},
         #                        "type": "Feature"}], "type": "FeatureCollection"}
 
     @patch('activefires_pp.fire_notifications.netrc')
     @patch('activefires_pp.fire_notifications.socket.gethostname')
     @patch('activefires_pp.fire_notifications.read_config')
     @patch('activefires_pp.fire_notifications.EndUserNotifierRegional._setup_and_start_communication')
     def test_get_recipients_for_region(self, setup_comm, read_config, gethostname, netrc):
         """Test getting the recipients for a given region."""
-
         secrets = MyNetrcMock()
         netrc.return_value = secrets
         gethostname.return_value = 'default'
 
         myconfigfile = "/my/config/file/path"
         regstream = io.StringIO(REG_CONFIG)
```

### Comparing `activefires-pp-0.1.7/activefires_pp/tests/test_fires_filtering.py` & `activefires-pp-0.1.9/activefires_pp/tests/test_fires_filtering.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2021, 2022 Adam Dybbroe
+# Copyright (c) 2021 - 2023 Adam Dybbroe
 
 # Author(s):
 
 #   Adam Dybbroe <Firstname.Lastname at smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -20,25 +20,32 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Test the Fires filtering functionality."""
 
 import pytest
 from unittest.mock import patch
+from unittest import TestCase
+from freezegun import freeze_time
+
 import pandas as pd
+from geojson import FeatureCollection
 import numpy as np
 import io
 from datetime import datetime
 
 from activefires_pp.post_processing import ActiveFiresShapefileFiltering
 from activefires_pp.post_processing import ActiveFiresPostprocessing
 from activefires_pp.post_processing import COL_NAMES
 
+from activefires_pp.post_processing import geojson_feature_collection_from_detections
 
 TEST_ACTIVE_FIRES_FILEPATH = "./AFIMG_j01_d20210414_t1126439_e1128084_b17637_c20210414114130392094_cspp_dev.txt"
+TEST_ACTIVE_FIRES_FILEPATH2 = "./AFIMG_npp_d20230616_t1110054_e1111296_b60284_c20230616112418557033_cspp_dev.txt"
+
 
 TEST_ACTIVE_FIRES_FILE_DATA = """
 # Active Fires I-band EDR
 #
 # source: AFIMG_j01_d20210414_t1126439_e1128084_b17637_c20210414114130392094_cspp_dev.nc
 # version: CSPP Active Fires version: cspp-active-fire-noaa_1.1.0
 #
@@ -68,24 +75,49 @@
   60.13325882,   16.18420029,  329.47689819,  0.375,  0.375,    8,    5.32859230
   61.30901337,   21.98561668,  341.69180298,  0.375,  0.375,    8,    8.87900448
   58.29126740,    0.20132475,  331.47875977,  0.375,  0.375,    8,    3.64687872
   57.42922211,   -3.47403550,  336.02111816,  0.375,  0.375,    8,    8.39092922
   57.42747116,   -3.47912717,  353.80722046,  0.375,  0.375,    8,   12.13035393
 """
 
+# Here we have sorted out all detections not passing the filter mask!
+# So, 4 fire detections are left corresponding to what would end up in the geojson files:
+TEST_ACTIVE_FIRES_FILE_DATA2 = """
+# Active Fires I-band EDR
+#
+# source: AFIMG_npp_d20230616_t1110054_e1111296_b60284_c20230616112418557033_cspp_dev.nc
+# version: CSPP Active Fires version: cspp-active-fire-noaa_1.1.0
+#
+# column 1: latitude of fire pixel (degrees)
+# column 2: longitude of fire pixel (degrees)
+# column 3: I04 brightness temperature of fire pixel (K)
+# column 4: Along-scan fire pixel resolution (km)
+# column 5: Along-track fire pixel resolution (km)
+# column 6: detection confidence ([7,8,9]->[lo,med,hi])
+# column 7: fire radiative power (MW)
+#
+# number of fire pixels: 14
+#
+  62.65801239,   17.25905228,  339.66326904,  0.375,  0.375,    8,    2.51202917
+  64.21694183,   17.42074966,  329.65161133,  0.375,  0.375,    8,    3.39806151
+  64.56904602,   16.60095215,  346.52050781,  0.375,  0.375,    8,   20.59289360
+  64.57222748,   16.59840012,  348.72860718,  0.375,  0.375,    8,   20.59289360
+"""
+
 CONFIG_EXAMPLE = {'publish_topic': '/VIIRS/L2/Fires/PP',
                   'subscribe_topics': 'VIIRS/L2/AFI',
                   'af_pattern_ibands':
                   'AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S%f}_e{end_hour:%H%M%S%f}' +
                   '_b{orbit:s}_c{processing_time:%Y%m%d%H%M%S%f}_cspp_dev.txt',
                   'geojson_file_pattern_national': 'AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S}.geojson',
                   'geojson_file_pattern_regional': 'AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S}_' +
                   '{region_name:s}.geojson',
                   'regional_shapefiles_format': 'omr_{region_code:s}_Buffer.{ext:s}',
                   'output_dir': '/path/where/the/filtered/results/will/be/stored',
+                  'filepath_detection_id_cache': '/path/to/the/detection_id/cache',
                   'timezone': 'Europe/Stockholm'}
 
 OPEN_FSTREAM = io.StringIO(TEST_ACTIVE_FIRES_FILE_DATA)
 
 
 MY_FILE_PATTERN = ("AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S%f}_e{end_hour:%H%M%S%f}_" +
                    "b{orbit:s}_c{processing_time:%Y%m%d%H%M%S%f}_cspp_dev.txt")
@@ -121,16 +153,16 @@
 
 
 @patch('activefires_pp.post_processing._read_data')
 def test_add_start_and_end_time_to_active_fires_data_utc(readdata):
     """Test adding start and end times to the active fires data."""
     myfilepath = TEST_ACTIVE_FIRES_FILEPATH
 
-    fstream = io.StringIO(TEST_ACTIVE_FIRES_FILE_DATA)
-    afdata = pd.read_csv(fstream, index_col=None, header=None, comment='#', names=COL_NAMES)
+    # fstream = io.StringIO(TEST_ACTIVE_FIRES_FILE_DATA)
+    afdata = pd.read_csv(OPEN_FSTREAM, index_col=None, header=None, comment='#', names=COL_NAMES)
     readdata.return_value = afdata
 
     this = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='GMT')
     with patch('os.path.exists') as mypatch:
         mypatch.return_value = True
         this.get_af_data(filepattern=MY_FILE_PATTERN, localtime=False)
 
@@ -207,18 +239,27 @@
     gethostname.return_value = "my.host.name"
 
     myconfigfile = "/my/config/file/path"
     myborders_file = "/my/shape/file/with/country/borders"
     mymask_file = "/my/shape/file/with/polygons/to/filter/out"
 
     afpp = ActiveFiresPostprocessing(myconfigfile, myborders_file, mymask_file)
+    afpp._initialize_fire_detection_id()
 
     fstream = io.StringIO(TEST_ACTIVE_FIRES_FILE_DATA)
     afdata = pd.read_csv(fstream, index_col=None, header=None, comment='#', names=COL_NAMES)
 
+    starttime = datetime.fromisoformat('2021-04-14 11:26:43.900')
+    endtime = datetime.fromisoformat('2021-04-14 11:28:08')
+
+    afdata['starttime'] = np.repeat(starttime, len(afdata)).astype(np.datetime64)
+    afdata['endtime'] = np.repeat(endtime, len(afdata)).astype(np.datetime64)
+
+    afdata = afpp.add_unique_day_id(afdata)
+
     # Add metadata to the pandas dataframe:
     fake_metadata = {'platform': 'j01',
                      'start_time': datetime(2021, 4, 14, 11, 26, 43, 900000),
                      'end_hour': datetime(1900, 1, 1, 11, 28, 8, 400000),
                      'orbit': '17637',
                      'processing_time': datetime(2021, 4, 14, 11, 41, 30, 392094),
                      'end_time': datetime(2021, 4, 14, 11, 28, 8)}
@@ -226,15 +267,14 @@
 
     af_shapeff = ActiveFiresShapefileFiltering(afdata=afdata, platform_name='NOAA-20')
     regional_fmask = TEST_REGIONAL_MASK
 
     mymsg = "Fake message"
     with patch('activefires_pp.post_processing.store_geojson') as store_geojson:
         with patch('activefires_pp.post_processing.ActiveFiresPostprocessing._generate_output_message') as generate_msg:
-            store_geojson.return_value = "/some/output/path"
             generate_msg.return_value = "my fake output message"
             result = afpp.regional_fires_filtering_and_publishing(mymsg, regional_fmask, af_shapeff)
 
     store_geojson.assert_called_once()
     generate_msg.assert_called_once()
 
     assert len(result) == 1
@@ -268,30 +308,22 @@
                      'end_time': datetime(2021, 4, 14, 11, 28, 8)}
     afdata.attrs = fake_metadata
 
     af_shapeff = ActiveFiresShapefileFiltering(afdata=afdata, platform_name='NOAA-20')
     afdata = af_shapeff.get_af_data(MY_FILE_PATTERN)
 
     mymsg = "Fake message"
+    result = afpp.fires_filtering(mymsg, af_shapeff)
 
-    with patch('activefires_pp.post_processing.store_geojson') as store_geojson:
-        with patch('activefires_pp.post_processing.ActiveFiresPostprocessing.get_output_messages') as get_output_msg:
-            store_geojson.return_value = "/some/output/path"
-            get_output_msg.return_value = ["my fake output message"]
-            outmsg, result = afpp.fires_filtering(mymsg, af_shapeff)
-
-    store_geojson.assert_called_once()
-    get_output_msg.assert_called_once()
     assert get_global_mask.call_count == 2
 
     assert isinstance(result, pd.core.frame.DataFrame)
     assert len(result) == 1
     np.testing.assert_almost_equal(result.iloc[0]['latitude'], 59.52483368)
     np.testing.assert_almost_equal(result.iloc[0]['longitude'], 17.1681633)
-    assert outmsg == ["my fake output message"]
 
 
 @pytest.mark.usefixtures("fake_national_borders_shapefile")
 @pytest.mark.usefixtures("fake_yamlconfig_file_post_processing")
 @patch('socket.gethostname')
 @patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication')
 def test_checking_national_borders_shapefile_file_exists(setup_comm, gethostname,
@@ -323,7 +355,80 @@
 
     afpp = ActiveFiresPostprocessing(myconfigfile, myborders_file, mymask_file)
     with pytest.raises(OSError) as exec_info:
         afpp._check_borders_shapes_exists()
 
     expected = "Shape file does not exist! Filename = /my/shape/file/with/country/borders"
     assert str(exec_info.value) == expected
+
+
+@freeze_time('2023-06-16 11:24:00')
+@patch('socket.gethostname')
+@patch('activefires_pp.post_processing.read_config')
+@patch('activefires_pp.post_processing.ActiveFiresPostprocessing._setup_and_start_communication')
+@patch('activefires_pp.post_processing._read_data')
+def test_get_feature_collection_from_firedata(readdata, setup_comm,
+                                              get_config, gethostname):
+    """Test get the Geojson Feature Collection from fire detection."""
+    get_config.return_value = CONFIG_EXAMPLE
+    gethostname.return_value = "my.host.name"
+
+    myconfigfile = "/my/config/file/path"
+    myborders_file = "/my/shape/file/with/country/borders"
+    mymask_file = "/my/shape/file/with/polygons/to/filter/out"
+
+    afpp = ActiveFiresPostprocessing(myconfigfile, myborders_file, mymask_file)
+    afpp._initialize_fire_detection_id()
+
+    myfilepath = TEST_ACTIVE_FIRES_FILEPATH2
+
+    fstream = io.StringIO(TEST_ACTIVE_FIRES_FILE_DATA2)
+    afdata = pd.read_csv(fstream, index_col=None, header=None, comment='#', names=COL_NAMES)
+    readdata.return_value = afdata
+
+    this = ActiveFiresShapefileFiltering(filepath=myfilepath, timezone='GMT')
+    with patch('os.path.exists') as mypatch:
+        mypatch.return_value = True
+        afdata = this.get_af_data(filepattern=MY_FILE_PATTERN, localtime=False)
+
+    afdata = afpp.add_unique_day_id(afdata)
+
+    result = geojson_feature_collection_from_detections(afdata, platform_name='Suomi-NPP')
+
+    # NB! The time of the afdata is here still in UTC!
+    expected = FeatureCollection([{"geometry": {"coordinates": [17.259052, 62.658012],
+                                                "type": "Point"},
+                                   "properties": {"confidence": 8,
+                                                  "observation_time": "2023-06-16T11:10:47.200000",
+                                                  "platform_name": "Suomi-NPP",
+                                                  "id": '20230616-1',
+                                                  "power": 2.51202917, "tb": 339.66326904},
+                                   "type": "Feature"},
+                                  {"geometry": {"coordinates": [17.42075, 64.216942],
+                                                "type": "Point"},
+                                   "properties": {"confidence": 8,
+                                                  "observation_time": "2023-06-16T11:10:47.200000",
+                                                  "platform_name": "Suomi-NPP",
+                                                  "id": '20230616-2',
+                                                  "power": 3.39806151,
+                                                  "tb": 329.65161133},
+                                   "type": "Feature"},
+                                  {"geometry": {"coordinates": [16.600952, 64.569046],
+                                                "type": "Point"},
+                                   "properties": {"confidence": 8,
+                                                  "observation_time": "2023-06-16T11:10:47.200000",
+                                                  "platform_name": "Suomi-NPP",
+                                                  "id": '20230616-3',
+                                                  "power": 20.5928936,
+                                                  "tb": 346.52050781},
+                                   "type": "Feature"},
+                                  {"geometry": {"coordinates": [16.5984, 64.572227],
+                                                "type": "Point"},
+                                   "properties": {"confidence": 8,
+                                                  "observation_time": "2023-06-16T11:10:47.200000",
+                                                  "platform_name": "Suomi-NPP",
+                                                  "id": '20230616-4',
+                                                  "power": 20.5928936,
+                                                  "tb": 348.72860718},
+                                   "type": "Feature"}])
+
+    TestCase().assertDictEqual(result, expected)
```

### Comparing `activefires-pp-0.1.7/activefires_pp/tests/test_geojson_utils.py` & `activefires-pp-0.1.9/activefires_pp/tests/test_geojson_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2022 Adam Dybbroe
+# Copyright (c) 2022 - 2023 Adam Dybbroe
 
 # Author(s):
 
 #   Adam Dybbroe <Firstname.Lastname@smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
```

### Comparing `activefires-pp-0.1.7/activefires_pp/tests/test_spatiotemporal_alarm_filtering.py` & `activefires-pp-0.1.9/activefires_pp/tests/test_spatiotemporal_alarm_filtering.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/activefires_pp/tests/test_utils.py` & `activefires-pp-0.1.9/activefires_pp/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2021, 2022 Adam.Dybbroe
+# Copyright (c) 2021, 2022, 2023 Adam.Dybbroe
 
 # Author(s):
 
 #   Adam.Dybbroe <a000680@c21856.ad.smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -16,32 +16,30 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit testing the utility functions.
-"""
+"""Unit testing the utility functions."""
 
 import pytest
 from freezegun import freeze_time
 from datetime import datetime, timedelta
 from posttroll.message import Message
 
 from activefires_pp.utils import get_filename_from_posttroll_message
 from activefires_pp.utils import datetime_utc2local
 from activefires_pp.utils import json_serial
 
-NATIONAL_TEST_MESSAGE = """pytroll://VIIRS/L2/Fires/PP/National file safusr.u@lxserv1043.smhi.se 2021-04-19T11:16:49.519087 v1.01 application/json {"start_time": "2021-04-16T12:29:53", "end_time": "2021-04-16T12:31:18", "orbit_number": 1, "platform_name": "NOAA-20", "sensor": "viirs", "data_processing_level": "2", "variant": "DR", "orig_orbit_number": 17666, "uri": "ssh://lxserv1043.smhi.se//san1/polar_out/direct_readout/viirs_active_fires/filtered/AFIMG_j01_d20210416_t122953.geojson", "uid": "AFIMG_j01_d20210416_t122953.geojson", "type": "GEOJSON-filtered", "format": "geojson", "product": "afimg"}"""
+NATIONAL_TEST_MESSAGE = """pytroll://VIIRS/L2/Fires/PP/National file safusr.u@lxserv1043.smhi.se 2021-04-19T11:16:49.519087 v1.01 application/json {"start_time": "2021-04-16T12:29:53", "end_time": "2021-04-16T12:31:18", "orbit_number": 1, "platform_name": "NOAA-20", "sensor": "viirs", "data_processing_level": "2", "variant": "DR", "orig_orbit_number": 17666, "uri": "ssh://lxserv1043.smhi.se//san1/polar_out/direct_readout/viirs_active_fires/filtered/AFIMG_j01_d20210416_t122953.geojson", "uid": "AFIMG_j01_d20210416_t122953.geojson", "type": "GEOJSON-filtered", "format": "geojson", "product": "afimg"}"""  # noqa
 
 
 def test_json_serial():
     """Test the json_serial function."""
-
     dtime_obj = datetime(2021, 4, 7, 11, 58, 53, 200000)
     res = json_serial(dtime_obj)
 
     assert res == "2021-04-07T11:58:53.200000"
 
     with pytest.raises(TypeError) as exec_info:
         other_obj = 'not okay'
@@ -60,15 +58,14 @@
     assert filename.name == 'AFIMG_j01_d20210416_t122953.geojson'
     assert str(filename.parent) == '//san1/polar_out/direct_readout/viirs_active_fires/filtered'
 
 
 @freeze_time('2022-03-26 18:12:05')
 def test_utc2localtime_conversion():
     """Test converting utc time to local time."""
-
     atime1 = datetime.utcnow()
     dtobj = datetime_utc2local(atime1, 'Europe/Stockholm')
     assert dtobj.strftime('%Y%m%d-%H%M') == '20220326-1912'
 
     atime2 = atime1 + timedelta(days=1)
     dtobj = datetime_utc2local(atime2, 'Europe/Stockholm')
     assert dtobj.strftime('%Y%m%d-%H%M') == '20220327-2012'
```

### Comparing `activefires-pp-0.1.7/activefires_pp/utils.py` & `activefires-pp-0.1.9/activefires_pp/utils.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/activefires_pp.egg-info/PKG-INFO` & `activefires-pp-0.1.9/activefires_pp.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: activefires-pp
-Version: 0.1.7
+Version: 0.1.9
 Summary: Post-processing of and notifications on Satellite active fire detections
 Home-page: https://github.com/adybbroe/activefires-pp
 Author: Adam Dybroe
 Author-email: adam.dybroe@smhi.se
 License: GPLv3
-Description: activefires-pp
-        ==============
-        
-        [![Build status](https://github.com/adybbroe/activefires-pp/workflows/CI/badge.svg?branch=main)](https://github.com/adybbroe/activefires-pp/workflows/CI/badge.svg?branch=main)
-        [![Coverage Status](https://coveralls.io/repos/github/adybbroe/activefires-pp/badge.svg)](https://coveralls.io/github/adybbroe/activefires-pp)
-        
-        Post-processing (including regional filtering) of Satellite Active Fires and notify end-users
-        Supports reading and processing VIIRS Active Fires EDR. There is support for filtering out fire
-        detections using three different levels:
-        
-          * National filtering, where all detections outside boarders as given by a shapefile are left out
-        
-          * Filtering to exclude fire detections inside a set of polygons (meant to
-            define populated areas and local industries known to be heat sources that
-            can turn up as detections) from a shapefile
-        
-          * Regional filtering, where detections are localisized in regions and output
-            messages are treated accordingly.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
+License-File: LICENSE
+
+activefires-pp
+==============
+
+[![Build status](https://github.com/adybbroe/activefires-pp/workflows/CI/badge.svg?branch=main)](https://github.com/adybbroe/activefires-pp/workflows/CI/badge.svg?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/adybbroe/activefires-pp/badge.svg)](https://coveralls.io/github/adybbroe/activefires-pp)
+
+Post-processing (including regional filtering) of Satellite Active Fires and notify end-users
+Supports reading and processing VIIRS Active Fires EDR. There is support for filtering out fire
+detections using three different levels:
+
+  * National filtering, where all detections outside boarders as given by a shapefile are left out
+
+  * Filtering to exclude fire detections inside a set of polygons (meant to
+    define populated areas and local industries known to be heat sources that
+    can turn up as detections) from a shapefile
+
+  * Regional filtering, where detections are localisized in regions and output
+    messages are treated accordingly.
+
+
```

### Comparing `activefires-pp-0.1.7/activefires_pp.egg-info/SOURCES.txt` & `activefires-pp-0.1.9/activefires_pp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 activefires_pp.egg-info/dependency_links.txt
 activefires_pp.egg-info/not-zip-safe
 activefires_pp.egg-info/requires.txt
 activefires_pp.egg-info/top_level.txt
 activefires_pp/tests/conftest.py
 activefires_pp/tests/test_api_posting.py
 activefires_pp/tests/test_config.py
+activefires_pp/tests/test_fire_detection_id_handling.py
 activefires_pp/tests/test_fire_notifications.py
 activefires_pp/tests/test_fires_filtering.py
 activefires_pp/tests/test_geojson_utils.py
 activefires_pp/tests/test_messaging.py
 activefires_pp/tests/test_shapefile_geometries.py
 activefires_pp/tests/test_spatiotemporal_alarm_filtering.py
 activefires_pp/tests/test_utils.py
```

### Comparing `activefires-pp-0.1.7/bin/active_fires_notifier.py` & `activefires-pp-0.1.9/bin/active_fires_notifier.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/bin/active_fires_postprocessing.py` & `activefires-pp-0.1.9/bin/active_fires_postprocessing.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/bin/active_fires_spatiotemporal_alarm_filtering.py` & `activefires-pp-0.1.9/bin/active_fires_spatiotemporal_alarm_filtering.py`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/examples/fire_notifier.yaml` & `activefires-pp-0.1.9/examples/fire_notifier.yaml`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/examples/fire_notifier_regional.yaml` & `activefires-pp-0.1.9/examples/fire_notifier_regional.yaml`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/examples/fires_pp.yaml` & `activefires-pp-0.1.9/examples/fires_pp.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -7,9 +7,11 @@
 geojson_file_pattern_national: AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S}.geojson
 geojson_file_pattern_regional: AFIMG_{platform:s}_d{start_time:%Y%m%d_t%H%M%S}_{region_name:s}.geojson
 
 regional_shapefiles_format: omr_{region_code:s}_Buffer.{ext:s}
 
 output_dir: /path/where/the/filtered/results/will/be/stored
 
+filepath_detection_id_cache: /path/to/the/detection_id/cache
+
 timezone: Europe/Stockholm
 # pytz.all_timezones
```

### Comparing `activefires-pp-0.1.7/examples/log_config.yaml` & `activefires-pp-0.1.9/examples/log_config.yaml`

 * *Files identical despite different names*

### Comparing `activefires-pp-0.1.7/setup.py` & `activefires-pp-0.1.9/setup.py`

 * *Files identical despite different names*

