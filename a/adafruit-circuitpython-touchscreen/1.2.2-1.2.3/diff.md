# Comparing `tmp/adafruit-circuitpython-touchscreen-1.2.2.tar.gz` & `tmp/adafruit-circuitpython-touchscreen-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-touchscreen-1.2.2.tar", last modified: Fri May 26 16:25:50 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-touchscreen-1.2.3.tar", last modified: Mon Jul 17 16:05:03 2023, max compression
```

## Comparing `adafruit-circuitpython-touchscreen-1.2.2.tar` & `adafruit-circuitpython-touchscreen-1.2.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.270369 adafruit-circuitpython-touchscreen-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.262369 adafruit-circuitpython-touchscreen-1.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.266369 adafruit-circuitpython-touchscreen-1.2.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.266369 adafruit-circuitpython-touchscreen-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.266369 adafruit-circuitpython-touchscreen-1.2.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-26 16:25:50.270369 adafruit-circuitpython-touchscreen-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.266369 adafruit-circuitpython-touchscreen-1.2.2/adafruit_circuitpython_touchscreen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-26 16:25:50.000000 adafruit-circuitpython-touchscreen-1.2.2/adafruit_circuitpython_touchscreen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-26 16:25:50.000000 adafruit-circuitpython-touchscreen-1.2.2/adafruit_circuitpython_touchscreen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:25:50.000000 adafruit-circuitpython-touchscreen-1.2.2/adafruit_circuitpython_touchscreen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 16:25:50.000000 adafruit-circuitpython-touchscreen-1.2.2/adafruit_circuitpython_touchscreen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 16:25:50.000000 adafruit-circuitpython-touchscreen-1.2.2/adafruit_circuitpython_touchscreen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-26 16:25:43.000000 adafruit-circuitpython-touchscreen-1.2.2/adafruit_touchscreen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.266369 adafruit-circuitpython-touchscreen-1.2.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.266369 adafruit-circuitpython-touchscreen-1.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.270369 adafruit-circuitpython-touchscreen-1.2.2/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6146 2023-05-26 16:25:43.000000 adafruit-circuitpython-touchscreen-1.2.2/examples/touchscreen_calibrator_built_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-26 16:25:43.000000 adafruit-circuitpython-touchscreen-1.2.2/examples/touchscreen_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-26 16:25:43.000000 adafruit-circuitpython-touchscreen-1.2.2/examples/touchscreen_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-26 16:25:43.000000 adafruit-circuitpython-touchscreen-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:25:50.270369 adafruit-circuitpython-touchscreen-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:05:03.035852 adafruit-circuitpython-touchscreen-1.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:05:03.027852 adafruit-circuitpython-touchscreen-1.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:05:03.027852 adafruit-circuitpython-touchscreen-1.2.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:05:03.031852 adafruit-circuitpython-touchscreen-1.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:05:03.031852 adafruit-circuitpython-touchscreen-1.2.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-17 16:05:03.031852 adafruit-circuitpython-touchscreen-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:05:03.031852 adafruit-circuitpython-touchscreen-1.2.3/adafruit_circuitpython_touchscreen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-17 16:05:03.000000 adafruit-circuitpython-touchscreen-1.2.3/adafruit_circuitpython_touchscreen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-17 16:05:03.000000 adafruit-circuitpython-touchscreen-1.2.3/adafruit_circuitpython_touchscreen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:05:03.000000 adafruit-circuitpython-touchscreen-1.2.3/adafruit_circuitpython_touchscreen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 16:05:03.000000 adafruit-circuitpython-touchscreen-1.2.3/adafruit_circuitpython_touchscreen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 16:05:03.000000 adafruit-circuitpython-touchscreen-1.2.3/adafruit_circuitpython_touchscreen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-07-17 16:04:55.000000 adafruit-circuitpython-touchscreen-1.2.3/adafruit_touchscreen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:05:03.031852 adafruit-circuitpython-touchscreen-1.2.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:05:03.031852 adafruit-circuitpython-touchscreen-1.2.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:05:03.031852 adafruit-circuitpython-touchscreen-1.2.3/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6146 2023-07-17 16:04:55.000000 adafruit-circuitpython-touchscreen-1.2.3/examples/touchscreen_calibrator_built_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-17 16:04:55.000000 adafruit-circuitpython-touchscreen-1.2.3/examples/touchscreen_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-17 16:04:55.000000 adafruit-circuitpython-touchscreen-1.2.3/examples/touchscreen_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-17 16:04:55.000000 adafruit-circuitpython-touchscreen-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-17 16:04:46.000000 adafruit-circuitpython-touchscreen-1.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 16:05:03.035852 adafruit-circuitpython-touchscreen-1.2.3/setup.cfg
```

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-touchscreen-1.2.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/.gitignore` & `adafruit-circuitpython-touchscreen-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/.pre-commit-config.yaml` & `adafruit-circuitpython-touchscreen-1.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/.pylintrc` & `adafruit-circuitpython-touchscreen-1.2.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-touchscreen-1.2.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/LICENSE` & `adafruit-circuitpython-touchscreen-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-touchscreen-1.2.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/LICENSES/MIT.txt` & `adafruit-circuitpython-touchscreen-1.2.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-touchscreen-1.2.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/PKG-INFO` & `adafruit-circuitpython-touchscreen-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-touchscreen
-Version: 1.2.2
+Version: 1.2.3
 Summary: CircuitPython library for 4-wire resistive touchscreens
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Touchscreen
 Keywords: adafruit,blinka,circuitpython,micropython,touchscreen,resistive
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/README.rst` & `adafruit-circuitpython-touchscreen-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/adafruit_circuitpython_touchscreen.egg-info/PKG-INFO` & `adafruit-circuitpython-touchscreen-1.2.3/adafruit_circuitpython_touchscreen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-touchscreen
-Version: 1.2.2
+Version: 1.2.3
 Summary: CircuitPython library for 4-wire resistive touchscreens
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Touchscreen
 Keywords: adafruit,blinka,circuitpython,micropython,touchscreen,resistive
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/adafruit_circuitpython_touchscreen.egg-info/SOURCES.txt` & `adafruit-circuitpython-touchscreen-1.2.3/adafruit_circuitpython_touchscreen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/adafruit_touchscreen.py` & `adafruit-circuitpython-touchscreen-1.2.3/adafruit_touchscreen.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
 """
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Touchscreen.git"
 
 from digitalio import DigitalInOut
 from analogio import AnalogIn
 
 try:
     from typing import Optional, Tuple
```

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/docs/_static/favicon.ico` & `adafruit-circuitpython-touchscreen-1.2.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/docs/conf.py` & `adafruit-circuitpython-touchscreen-1.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/docs/index.rst` & `adafruit-circuitpython-touchscreen-1.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/examples/touchscreen_calibrator_built_in.py` & `adafruit-circuitpython-touchscreen-1.2.3/examples/touchscreen_calibrator_built_in.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/examples/touchscreen_orientation.py` & `adafruit-circuitpython-touchscreen-1.2.3/examples/touchscreen_orientation.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/examples/touchscreen_simpletest.py` & `adafruit-circuitpython-touchscreen-1.2.3/examples/touchscreen_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.2/pyproject.toml` & `adafruit-circuitpython-touchscreen-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-touchscreen"
 description = "CircuitPython library for 4-wire resistive touchscreens"
-version = "1.2.2"
+version = "1.2.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Touchscreen"}
 keywords = [
     "adafruit",
```

