# Comparing `tmp/adafruit-circuitpython-sgp40-1.3.8.tar.gz` & `tmp/adafruit-circuitpython-sgp40-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-sgp40-1.3.8.tar", last modified: Fri Aug 26 02:29:34 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-sgp40-1.3.9.tar", last modified: Mon Oct  3 04:56:16 2022, max compression
```

## Comparing `adafruit-circuitpython-sgp40-1.3.8.tar` & `adafruit-circuitpython-sgp40-1.3.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:34.253192 adafruit-circuitpython-sgp40-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:34.249192 adafruit-circuitpython-sgp40-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:34.249192 adafruit-circuitpython-sgp40-1.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:34.249192 adafruit-circuitpython-sgp40-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:34.249192 adafruit-circuitpython-sgp40-1.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4798 2022-08-26 02:29:34.253192 adafruit-circuitpython-sgp40-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3997 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:34.249192 adafruit-circuitpython-sgp40-1.3.8/adafruit_circuitpython_sgp40.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4798 2022-08-26 02:29:34.000000 adafruit-circuitpython-sgp40-1.3.8/adafruit_circuitpython_sgp40.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-08-26 02:29:34.000000 adafruit-circuitpython-sgp40-1.3.8/adafruit_circuitpython_sgp40.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:29:34.000000 adafruit-circuitpython-sgp40-1.3.8/adafruit_circuitpython_sgp40.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 02:29:34.000000 adafruit-circuitpython-sgp40-1.3.8/adafruit_circuitpython_sgp40.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-26 02:29:34.000000 adafruit-circuitpython-sgp40-1.3.8/adafruit_circuitpython_sgp40.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:34.249192 adafruit-circuitpython-sgp40-1.3.8/adafruit_sgp40/
--rw-r--r--   0 runner    (1001) docker     (121)    12008 2022-08-26 02:29:26.000000 adafruit-circuitpython-sgp40-1.3.8/adafruit_sgp40/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31648 2022-08-26 02:29:26.000000 adafruit-circuitpython-sgp40-1.3.8/adafruit_sgp40/voc_algorithm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:34.253192 adafruit-circuitpython-sgp40-1.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:34.253192 adafruit-circuitpython-sgp40-1.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5859 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:34.253192 adafruit-circuitpython-sgp40-1.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-08-26 02:29:26.000000 adafruit-circuitpython-sgp40-1.3.8/examples/sgp40_indextest.py
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-08-26 02:29:26.000000 adafruit-circuitpython-sgp40-1.3.8/examples/sgp40_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-08-26 02:29:26.000000 adafruit-circuitpython-sgp40-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-26 02:29:19.000000 adafruit-circuitpython-sgp40-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:29:34.253192 adafruit-circuitpython-sgp40-1.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 04:56:16.676737 adafruit-circuitpython-sgp40-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 04:56:16.672737 adafruit-circuitpython-sgp40-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 04:56:16.676737 adafruit-circuitpython-sgp40-1.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 04:56:16.676737 adafruit-circuitpython-sgp40-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 04:56:16.676737 adafruit-circuitpython-sgp40-1.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4804 2022-10-03 04:56:16.676737 adafruit-circuitpython-sgp40-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4003 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 04:56:16.676737 adafruit-circuitpython-sgp40-1.3.9/adafruit_circuitpython_sgp40.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4804 2022-10-03 04:56:16.000000 adafruit-circuitpython-sgp40-1.3.9/adafruit_circuitpython_sgp40.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2022-10-03 04:56:16.000000 adafruit-circuitpython-sgp40-1.3.9/adafruit_circuitpython_sgp40.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 04:56:16.000000 adafruit-circuitpython-sgp40-1.3.9/adafruit_circuitpython_sgp40.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-10-03 04:56:16.000000 adafruit-circuitpython-sgp40-1.3.9/adafruit_circuitpython_sgp40.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-03 04:56:16.000000 adafruit-circuitpython-sgp40-1.3.9/adafruit_circuitpython_sgp40.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 04:56:16.676737 adafruit-circuitpython-sgp40-1.3.9/adafruit_sgp40/
+-rw-r--r--   0 runner    (1001) docker     (121)    12008 2022-10-03 04:56:09.000000 adafruit-circuitpython-sgp40-1.3.9/adafruit_sgp40/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31648 2022-10-03 04:56:09.000000 adafruit-circuitpython-sgp40-1.3.9/adafruit_sgp40/voc_algorithm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 04:56:16.676737 adafruit-circuitpython-sgp40-1.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 04:56:16.676737 adafruit-circuitpython-sgp40-1.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5859 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 04:56:16.676737 adafruit-circuitpython-sgp40-1.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-10-03 04:56:09.000000 adafruit-circuitpython-sgp40-1.3.9/examples/sgp40_indextest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      782 2022-10-03 04:56:09.000000 adafruit-circuitpython-sgp40-1.3.9/examples/sgp40_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-10-03 04:56:09.000000 adafruit-circuitpython-sgp40-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-10-03 04:56:01.000000 adafruit-circuitpython-sgp40-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-03 04:56:16.676737 adafruit-circuitpython-sgp40-1.3.9/setup.cfg
```

### Comparing `adafruit-circuitpython-sgp40-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-sgp40-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-sgp40-1.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-sgp40-1.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/.gitignore` & `adafruit-circuitpython-sgp40-1.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-sgp40-1.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/.pylintrc` & `adafruit-circuitpython-sgp40-1.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-sgp40-1.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/LICENSE` & `adafruit-circuitpython-sgp40-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-sgp40-1.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-sgp40-1.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-sgp40-1.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/PKG-INFO` & `adafruit-circuitpython-sgp40-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-sgp40
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython library for the Adafruit SGP40 Air Quality Sensor / VOC Index Sensor Breakouts
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SGP40
 Keywords: adafruit,blinka,circuitpython,micropython,sgp40,IAQ,Air Quality,VOC,MOX,Gas
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -81,15 +81,15 @@
 .. code-block:: python3
 
     import time
     import board
     import adafruit_sgp40
 
     i2c = board.I2C()  # uses board.SCL and board.SDA
-    sgp = adafruit_sgp40(i2c)
+    sgp = adafruit_sgp40.SGP40(i2c)
 
     while True:
         print("Measurement: ", sgp.raw)
         print("")
         sleep(1)
 
 For humidity compensated raw gas and voc index readings, we'll need a secondary sensor such as the bme280
```

### Comparing `adafruit-circuitpython-sgp40-1.3.8/README.rst` & `adafruit-circuitpython-sgp40-1.3.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 .. code-block:: python3
 
     import time
     import board
     import adafruit_sgp40
 
     i2c = board.I2C()  # uses board.SCL and board.SDA
-    sgp = adafruit_sgp40(i2c)
+    sgp = adafruit_sgp40.SGP40(i2c)
 
     while True:
         print("Measurement: ", sgp.raw)
         print("")
         sleep(1)
 
 For humidity compensated raw gas and voc index readings, we'll need a secondary sensor such as the bme280
```

### Comparing `adafruit-circuitpython-sgp40-1.3.8/adafruit_circuitpython_sgp40.egg-info/PKG-INFO` & `adafruit-circuitpython-sgp40-1.3.9/adafruit_circuitpython_sgp40.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-sgp40
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython library for the Adafruit SGP40 Air Quality Sensor / VOC Index Sensor Breakouts
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SGP40
 Keywords: adafruit,blinka,circuitpython,micropython,sgp40,IAQ,Air Quality,VOC,MOX,Gas
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -81,15 +81,15 @@
 .. code-block:: python3
 
     import time
     import board
     import adafruit_sgp40
 
     i2c = board.I2C()  # uses board.SCL and board.SDA
-    sgp = adafruit_sgp40(i2c)
+    sgp = adafruit_sgp40.SGP40(i2c)
 
     while True:
         print("Measurement: ", sgp.raw)
         print("")
         sleep(1)
 
 For humidity compensated raw gas and voc index readings, we'll need a secondary sensor such as the bme280
```

### Comparing `adafruit-circuitpython-sgp40-1.3.8/adafruit_circuitpython_sgp40.egg-info/SOURCES.txt` & `adafruit-circuitpython-sgp40-1.3.9/adafruit_circuitpython_sgp40.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/adafruit_sgp40/__init__.py` & `adafruit-circuitpython-sgp40-1.3.9/adafruit_sgp40/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
  * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 
 """
 from time import sleep
 from struct import unpack_from
 from adafruit_bus_device import i2c_device
 
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SGP40.git"
 
 _WORD_LEN = 2
 
 # no point in generating this each time
 # Generated from temp 25c, humidity 50%
 _READ_CMD = b"\x26\x0F\x80\x00\xA2\x66\x66\x93"
```

### Comparing `adafruit-circuitpython-sgp40-1.3.8/adafruit_sgp40/voc_algorithm.py` & `adafruit-circuitpython-sgp40-1.3.9/adafruit_sgp40/voc_algorithm.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-sgp40-1.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/docs/conf.py` & `adafruit-circuitpython-sgp40-1.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/docs/index.rst` & `adafruit-circuitpython-sgp40-1.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/examples/sgp40_indextest.py` & `adafruit-circuitpython-sgp40-1.3.9/examples/sgp40_indextest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/examples/sgp40_simpletest.py` & `adafruit-circuitpython-sgp40-1.3.9/examples/sgp40_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sgp40-1.3.8/pyproject.toml` & `adafruit-circuitpython-sgp40-1.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-sgp40"
 description = "CircuitPython library for the Adafruit SGP40 Air Quality Sensor / VOC Index Sensor Breakouts"
-version = "1.3.8"
+version = "1.3.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SGP40"}
 keywords = [
     "adafruit",
```

