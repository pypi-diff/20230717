# Comparing `tmp/adafruit-circuitpython-asyncio-0.5.8.tar.gz` & `tmp/adafruit-circuitpython-asyncio-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-asyncio-0.5.8.tar", last modified: Tue Mar 22 17:36:40 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-asyncio-0.5.9.tar", last modified: Tue Jun  7 16:42:27 2022, max compression
```

## Comparing `adafruit-circuitpython-asyncio-0.5.8.tar` & `adafruit-circuitpython-asyncio-0.5.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-22 17:36:40.496053 adafruit-circuitpython-asyncio-0.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-22 17:36:40.492053 adafruit-circuitpython-asyncio-0.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-22 17:36:40.492053 adafruit-circuitpython-asyncio-0.5.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-22 17:36:40.492053 adafruit-circuitpython-asyncio-0.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2677 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2939 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16271 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6753 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-22 17:36:40.492053 adafruit-circuitpython-asyncio-0.5.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3448 2022-03-22 17:36:40.496053 adafruit-circuitpython-asyncio-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2735 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-22 17:36:40.492053 adafruit-circuitpython-asyncio-0.5.8/adafruit_circuitpython_asyncio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3448 2022-03-22 17:36:40.000000 adafruit-circuitpython-asyncio-0.5.8/adafruit_circuitpython_asyncio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-03-22 17:36:40.000000 adafruit-circuitpython-asyncio-0.5.8/adafruit_circuitpython_asyncio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-22 17:36:40.000000 adafruit-circuitpython-asyncio-0.5.8/adafruit_circuitpython_asyncio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-03-22 17:36:40.000000 adafruit-circuitpython-asyncio-0.5.8/adafruit_circuitpython_asyncio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-03-22 17:36:40.000000 adafruit-circuitpython-asyncio-0.5.8/adafruit_circuitpython_asyncio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-22 17:36:40.492053 adafruit-circuitpython-asyncio-0.5.8/asyncio/
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-03-22 17:36:37.000000 adafruit-circuitpython-asyncio-0.5.8/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9756 2022-03-22 17:36:37.000000 adafruit-circuitpython-asyncio-0.5.8/asyncio/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-03-22 17:36:37.000000 adafruit-circuitpython-asyncio-0.5.8/asyncio/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     2498 2022-03-22 17:36:37.000000 adafruit-circuitpython-asyncio-0.5.8/asyncio/funcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-03-22 17:36:37.000000 adafruit-circuitpython-asyncio-0.5.8/asyncio/lock.py
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-03-22 17:36:37.000000 adafruit-circuitpython-asyncio-0.5.8/asyncio/manifest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-03-22 17:36:37.000000 adafruit-circuitpython-asyncio-0.5.8/asyncio/stream.py
--rw-r--r--   0 runner    (1001) docker     (121)     5749 2022-03-22 17:36:37.000000 adafruit-circuitpython-asyncio-0.5.8/asyncio/task.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-22 17:36:40.496053 adafruit-circuitpython-asyncio-0.5.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-22 17:36:40.496053 adafruit-circuitpython-asyncio-0.5.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5678 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-22 17:36:40.496053 adafruit-circuitpython-asyncio-0.5.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)    10645 2022-03-22 17:36:37.000000 adafruit-circuitpython-asyncio-0.5.8/examples/asyncio_displayio_button.py
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-03-22 17:36:37.000000 adafruit-circuitpython-asyncio-0.5.8/examples/asyncio_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-03-22 17:36:28.000000 adafruit-circuitpython-asyncio-0.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-22 17:36:40.496053 adafruit-circuitpython-asyncio-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2086 2022-03-22 17:36:37.000000 adafruit-circuitpython-asyncio-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:42:27.486328 adafruit-circuitpython-asyncio-0.5.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:42:27.482328 adafruit-circuitpython-asyncio-0.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:42:27.482328 adafruit-circuitpython-asyncio-0.5.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:42:27.482328 adafruit-circuitpython-asyncio-0.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2677 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2939 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16271 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6753 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:42:27.482328 adafruit-circuitpython-asyncio-0.5.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3500 2022-06-07 16:42:27.486328 adafruit-circuitpython-asyncio-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2787 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:42:27.482328 adafruit-circuitpython-asyncio-0.5.9/adafruit_circuitpython_asyncio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3500 2022-06-07 16:42:27.000000 adafruit-circuitpython-asyncio-0.5.9/adafruit_circuitpython_asyncio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-06-07 16:42:27.000000 adafruit-circuitpython-asyncio-0.5.9/adafruit_circuitpython_asyncio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 16:42:27.000000 adafruit-circuitpython-asyncio-0.5.9/adafruit_circuitpython_asyncio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-07 16:42:27.000000 adafruit-circuitpython-asyncio-0.5.9/adafruit_circuitpython_asyncio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-07 16:42:27.000000 adafruit-circuitpython-asyncio-0.5.9/adafruit_circuitpython_asyncio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:42:27.482328 adafruit-circuitpython-asyncio-0.5.9/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-06-07 16:42:23.000000 adafruit-circuitpython-asyncio-0.5.9/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9756 2022-06-07 16:42:23.000000 adafruit-circuitpython-asyncio-0.5.9/asyncio/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-06-07 16:42:23.000000 adafruit-circuitpython-asyncio-0.5.9/asyncio/event.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2498 2022-06-07 16:42:23.000000 adafruit-circuitpython-asyncio-0.5.9/asyncio/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-06-07 16:42:23.000000 adafruit-circuitpython-asyncio-0.5.9/asyncio/lock.py
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-06-07 16:42:23.000000 adafruit-circuitpython-asyncio-0.5.9/asyncio/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-06-07 16:42:23.000000 adafruit-circuitpython-asyncio-0.5.9/asyncio/stream.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5749 2022-06-07 16:42:23.000000 adafruit-circuitpython-asyncio-0.5.9/asyncio/task.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:42:27.486328 adafruit-circuitpython-asyncio-0.5.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:42:27.486328 adafruit-circuitpython-asyncio-0.5.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5678 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:42:27.486328 adafruit-circuitpython-asyncio-0.5.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)    10645 2022-06-07 16:42:23.000000 adafruit-circuitpython-asyncio-0.5.9/examples/asyncio_displayio_button.py
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-06-07 16:42:23.000000 adafruit-circuitpython-asyncio-0.5.9/examples/asyncio_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2022-06-07 16:42:15.000000 adafruit-circuitpython-asyncio-0.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 16:42:27.486328 adafruit-circuitpython-asyncio-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2086 2022-06-07 16:42:23.000000 adafruit-circuitpython-asyncio-0.5.9/setup.py
```

### Comparing `adafruit-circuitpython-asyncio-0.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-asyncio-0.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/.github/workflows/build.yml` & `adafruit-circuitpython-asyncio-0.5.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/.github/workflows/release.yml` & `adafruit-circuitpython-asyncio-0.5.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/.pre-commit-config.yaml` & `adafruit-circuitpython-asyncio-0.5.9/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
--   repo: https://github.com/python/black
-    rev: 20.8b1
+  - repo: https://github.com/python/black
+    rev: 22.3.0
     hooks:
-    - id: black
--   repo: https://github.com/fsfe/reuse-tool
-    rev: v0.12.1
+      - id: black
+  - repo: https://github.com/fsfe/reuse-tool
+    rev: v0.14.0
     hooks:
-    - id: reuse
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v2.3.0
+      - id: reuse
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.2.0
     hooks:
-    -   id: check-yaml
-    -   id: end-of-file-fixer
-    -   id: trailing-whitespace
--   repo: https://github.com/pycqa/pylint
-    rev: pylint-2.7.1
+      - id: check-yaml
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+  - repo: https://github.com/pycqa/pylint
+    rev: v2.11.1
     hooks:
-    -   id: pylint
+      - id: pylint
         name: pylint (library code)
         types: [python]
+        args:
+          - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
--   repo: local
-    hooks:
-    -   id: pylint_examples
-        name: pylint (examples code)
+      - id: pylint
+        name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
-        entry: /usr/bin/env bash -c
-        args: ['([[ ! -d "examples" ]] || for example in $(find . -path "./examples/*.py"); do pylint --disable=missing-docstring,invalid-name,consider-using-f-string $example; done)']
-        language: system
-    -   id: pylint_tests
-        name: pylint (tests code)
+        types: [python]
+        files: "^examples/"
+        args:
+          - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+      - id: pylint
+        name: pylint (test code)
         description: Run pylint rules on "tests/*.py" files
-        entry: /usr/bin/env bash -c
-        args: ['([[ ! -d "tests" ]] || for test in $(find . -path "./tests/*.py"); do pylint --disable=missing-docstring $test; done)']
-        language: system
+        types: [python]
+        files: "^tests/"
+        args:
+          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `adafruit-circuitpython-asyncio-0.5.8/.pylintrc` & `adafruit-circuitpython-asyncio-0.5.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-asyncio-0.5.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/LICENSE` & `adafruit-circuitpython-asyncio-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-asyncio-0.5.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/LICENSES/MIT.txt` & `adafruit-circuitpython-asyncio-0.5.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-asyncio-0.5.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/PKG-INFO` & `adafruit-circuitpython-asyncio-0.5.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-asyncio
-Version: 0.5.8
+Version: 0.5.9
 Summary: Cooperative multitasking and asynchronous I/O
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_asyncio.git
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython asyncio async
 Platform: UNKNOWN
@@ -22,15 +22,15 @@
 
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-asyncio/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/asyncio/en/latest/
     :alt: Documentation Status
 
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_asyncio/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_asyncio/actions
     :alt: Build Status
```

### Comparing `adafruit-circuitpython-asyncio-0.5.8/README.rst` & `adafruit-circuitpython-asyncio-0.5.9/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-asyncio/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/asyncio/en/latest/
     :alt: Documentation Status
 
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_asyncio/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_asyncio/actions
     :alt: Build Status
```

### Comparing `adafruit-circuitpython-asyncio-0.5.8/adafruit_circuitpython_asyncio.egg-info/PKG-INFO` & `adafruit-circuitpython-asyncio-0.5.9/adafruit_circuitpython_asyncio.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-asyncio
-Version: 0.5.8
+Version: 0.5.9
 Summary: Cooperative multitasking and asynchronous I/O
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_asyncio.git
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython asyncio async
 Platform: UNKNOWN
@@ -22,15 +22,15 @@
 
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-asyncio/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/asyncio/en/latest/
     :alt: Documentation Status
 
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_asyncio/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_asyncio/actions
     :alt: Build Status
```

### Comparing `adafruit-circuitpython-asyncio-0.5.8/adafruit_circuitpython_asyncio.egg-info/SOURCES.txt` & `adafruit-circuitpython-asyncio-0.5.9/adafruit_circuitpython_asyncio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/asyncio/__init__.py` & `adafruit-circuitpython-asyncio-0.5.9/asyncio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Altering these files significantly would make merging difficult, so we will not use
 # pylint or black.
 # pylint: skip-file
 # fmt: off
 
 from .core import *
 
-__version__ = "0.5.8"
+__version__ = "0.5.9"
 __repo__ = "https://github.com/Adafruit/Adafruit_CircuitPython_asyncio.git"
 
 _attrs = {
     "wait_for": "funcs",
     "wait_for_ms": "funcs",
     "gather": "funcs",
     "Event": "event",
```

### Comparing `adafruit-circuitpython-asyncio-0.5.8/asyncio/core.py` & `adafruit-circuitpython-asyncio-0.5.9/asyncio/core.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/asyncio/event.py` & `adafruit-circuitpython-asyncio-0.5.9/asyncio/event.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/asyncio/funcs.py` & `adafruit-circuitpython-asyncio-0.5.9/asyncio/funcs.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/asyncio/lock.py` & `adafruit-circuitpython-asyncio-0.5.9/asyncio/lock.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/asyncio/manifest.py` & `adafruit-circuitpython-asyncio-0.5.9/asyncio/manifest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/asyncio/stream.py` & `adafruit-circuitpython-asyncio-0.5.9/asyncio/stream.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/asyncio/task.py` & `adafruit-circuitpython-asyncio-0.5.9/asyncio/task.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/docs/_static/favicon.ico` & `adafruit-circuitpython-asyncio-0.5.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/docs/conf.py` & `adafruit-circuitpython-asyncio-0.5.9/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = [
     "_build",
     "Thumbs.db",
```

### Comparing `adafruit-circuitpython-asyncio-0.5.8/docs/index.rst` & `adafruit-circuitpython-asyncio-0.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/examples/asyncio_displayio_button.py` & `adafruit-circuitpython-asyncio-0.5.9/examples/asyncio_displayio_button.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-asyncio-0.5.8/setup.py` & `adafruit-circuitpython-asyncio-0.5.9/setup.py`

 * *Files identical despite different names*

