# Comparing `tmp/adafruit-circuitpython-nunchuk-1.1.8.tar.gz` & `tmp/adafruit-circuitpython-nunchuk-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-nunchuk-1.1.8.tar", last modified: Mon Jun 26 17:58:16 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-nunchuk-1.1.9.tar", last modified: Mon Jul 17 17:45:55 2023, max compression
```

## Comparing `adafruit-circuitpython-nunchuk-1.1.8.tar` & `adafruit-circuitpython-nunchuk-1.1.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.286054 adafruit-circuitpython-nunchuk-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.278053 adafruit-circuitpython-nunchuk-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.282054 adafruit-circuitpython-nunchuk-1.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.282054 adafruit-circuitpython-nunchuk-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.282054 adafruit-circuitpython-nunchuk-1.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-26 17:58:16.286054 adafruit-circuitpython-nunchuk-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.282054 adafruit-circuitpython-nunchuk-1.1.8/adafruit_circuitpython_nunchuk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-26 17:58:16.000000 adafruit-circuitpython-nunchuk-1.1.8/adafruit_circuitpython_nunchuk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-26 17:58:16.000000 adafruit-circuitpython-nunchuk-1.1.8/adafruit_circuitpython_nunchuk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:58:16.000000 adafruit-circuitpython-nunchuk-1.1.8/adafruit_circuitpython_nunchuk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 17:58:16.000000 adafruit-circuitpython-nunchuk-1.1.8/adafruit_circuitpython_nunchuk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 17:58:16.000000 adafruit-circuitpython-nunchuk-1.1.8/adafruit_circuitpython_nunchuk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-26 17:58:07.000000 adafruit-circuitpython-nunchuk-1.1.8/adafruit_nunchuk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.286054 adafruit-circuitpython-nunchuk-1.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.286054 adafruit-circuitpython-nunchuk-1.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.286054 adafruit-circuitpython-nunchuk-1.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-26 17:58:07.000000 adafruit-circuitpython-nunchuk-1.1.8/examples/nunchuk_accel_mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-26 17:58:07.000000 adafruit-circuitpython-nunchuk-1.1.8/examples/nunchuk_analog_mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-26 17:58:07.000000 adafruit-circuitpython-nunchuk-1.1.8/examples/nunchuk_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-26 17:58:07.000000 adafruit-circuitpython-nunchuk-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:58:16.286054 adafruit-circuitpython-nunchuk-1.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:45:55.739917 adafruit-circuitpython-nunchuk-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:45:55.731916 adafruit-circuitpython-nunchuk-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:45:55.731916 adafruit-circuitpython-nunchuk-1.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:45:55.735917 adafruit-circuitpython-nunchuk-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:45:55.735917 adafruit-circuitpython-nunchuk-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-17 17:45:55.739917 adafruit-circuitpython-nunchuk-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:45:55.735917 adafruit-circuitpython-nunchuk-1.1.9/adafruit_circuitpython_nunchuk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-17 17:45:55.000000 adafruit-circuitpython-nunchuk-1.1.9/adafruit_circuitpython_nunchuk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-17 17:45:55.000000 adafruit-circuitpython-nunchuk-1.1.9/adafruit_circuitpython_nunchuk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:45:55.000000 adafruit-circuitpython-nunchuk-1.1.9/adafruit_circuitpython_nunchuk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-17 17:45:55.000000 adafruit-circuitpython-nunchuk-1.1.9/adafruit_circuitpython_nunchuk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 17:45:55.000000 adafruit-circuitpython-nunchuk-1.1.9/adafruit_circuitpython_nunchuk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-07-17 17:45:46.000000 adafruit-circuitpython-nunchuk-1.1.9/adafruit_nunchuk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:45:55.735917 adafruit-circuitpython-nunchuk-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:45:55.735917 adafruit-circuitpython-nunchuk-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:45:55.739917 adafruit-circuitpython-nunchuk-1.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-17 17:45:46.000000 adafruit-circuitpython-nunchuk-1.1.9/examples/nunchuk_accel_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-17 17:45:46.000000 adafruit-circuitpython-nunchuk-1.1.9/examples/nunchuk_analog_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-17 17:45:46.000000 adafruit-circuitpython-nunchuk-1.1.9/examples/nunchuk_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-17 17:45:46.000000 adafruit-circuitpython-nunchuk-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-17 17:45:33.000000 adafruit-circuitpython-nunchuk-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 17:45:55.739917 adafruit-circuitpython-nunchuk-1.1.9/setup.cfg
```

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-nunchuk-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/.gitignore` & `adafruit-circuitpython-nunchuk-1.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-nunchuk-1.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/.pylintrc` & `adafruit-circuitpython-nunchuk-1.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-nunchuk-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/LICENSE` & `adafruit-circuitpython-nunchuk-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-nunchuk-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-nunchuk-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-nunchuk-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/PKG-INFO` & `adafruit-circuitpython-nunchuk-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-nunchuk
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython library for Nintendo Nunchuk controller
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Nunchuk.git
 Keywords: adafruit,blinka,circuitpython,micropython,nunchuk,nunchuck,nintendo,controller
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/README.rst` & `adafruit-circuitpython-nunchuk-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/adafruit_circuitpython_nunchuk.egg-info/PKG-INFO` & `adafruit-circuitpython-nunchuk-1.1.9/adafruit_circuitpython_nunchuk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-nunchuk
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython library for Nintendo Nunchuk controller
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Nunchuk.git
 Keywords: adafruit,blinka,circuitpython,micropython,nunchuk,nunchuck,nintendo,controller
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/adafruit_circuitpython_nunchuk.egg-info/SOURCES.txt` & `adafruit-circuitpython-nunchuk-1.1.9/adafruit_circuitpython_nunchuk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/adafruit_nunchuk.py` & `adafruit-circuitpython-nunchuk-1.1.9/adafruit_nunchuk.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 try:
     import typing  # pylint: disable=unused-import
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "1.1.8"
+__version__ = "1.1.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Nunchuk.git"
 
 _I2C_INIT_DELAY = 0.1
 
 
 class Nunchuk:
     """Class which provides interface to Nintendo Nunchuk controller.
```

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-nunchuk-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/docs/conf.py` & `adafruit-circuitpython-nunchuk-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/docs/index.rst` & `adafruit-circuitpython-nunchuk-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/examples/nunchuk_accel_mouse.py` & `adafruit-circuitpython-nunchuk-1.1.9/examples/nunchuk_analog_mouse.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,50 +3,46 @@
 
 import board
 import usb_hid
 from adafruit_hid.mouse import Mouse
 import adafruit_nunchuk
 
 m = Mouse(usb_hid.devices)
-nc = adafruit_nunchuk.Nunchuk(board.I2C())
+i2c = board.I2C()  # uses board.SCL and board.SDA
+# i2c = board.STEMMA_I2C()  # For using the built-in STEMMA QT connector on a microcontroller
+nc = adafruit_nunchuk.Nunchuk(i2c)
 
-centerX = 120
-centerY = 110
+centerX = 128
+centerY = 128
 
-scaleX = 0.4
-scaleY = 0.5
+scaleX = 0.3
+scaleY = 0.3
 
 cDown = False
 zDown = False
 
 # This is to allow double checking (only on left click - and it doesn't really work)
 CHECK_COUNT = 0
 
 
 # This is just to show that we're getting back data - uncomment it and hold down the buttons
 # while True:
 #    print((0 if nc.button_C else 1, 0 if nc.button_Z else 1))
 
 while True:
-    accel = nc.acceleration
-    #    print(accel)
-    #    x, y = nc.joystick
-    #    print((x,y))
-    x = accel[0] / 4
-    y = accel[1] / 4
-    print((x, y))
+    x, y = nc.joystick
     # Eliminate spurious reads
     if x == 255 or y == 255:
         continue
     relX = x - centerX
-    relY = y - centerY
+    relY = centerY - y
 
     m.move(int(scaleX * relX), int(scaleY * relY), 0)
-    buttons = nc.buttons
 
+    buttons = nc.buttons
     c = buttons.C
     z = buttons.Z
 
     if z and not zDown:
         stillDown = True
         for n in range(CHECK_COUNT):
             if nc.button_Z:
```

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/examples/nunchuk_analog_mouse.py` & `adafruit-circuitpython-nunchuk-1.1.9/examples/nunchuk_accel_mouse.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,44 +3,52 @@
 
 import board
 import usb_hid
 from adafruit_hid.mouse import Mouse
 import adafruit_nunchuk
 
 m = Mouse(usb_hid.devices)
-nc = adafruit_nunchuk.Nunchuk(board.I2C())
+i2c = board.I2C()  # uses board.SCL and board.SDA
+# i2c = board.STEMMA_I2C()  # For using the built-in STEMMA QT connector on a microcontroller
+nc = adafruit_nunchuk.Nunchuk(i2c)
 
-centerX = 128
-centerY = 128
+centerX = 120
+centerY = 110
 
-scaleX = 0.3
-scaleY = 0.3
+scaleX = 0.4
+scaleY = 0.5
 
 cDown = False
 zDown = False
 
 # This is to allow double checking (only on left click - and it doesn't really work)
 CHECK_COUNT = 0
 
 
 # This is just to show that we're getting back data - uncomment it and hold down the buttons
 # while True:
 #    print((0 if nc.button_C else 1, 0 if nc.button_Z else 1))
 
 while True:
-    x, y = nc.joystick
+    accel = nc.acceleration
+    #    print(accel)
+    #    x, y = nc.joystick
+    #    print((x,y))
+    x = accel[0] / 4
+    y = accel[1] / 4
+    print((x, y))
     # Eliminate spurious reads
     if x == 255 or y == 255:
         continue
     relX = x - centerX
-    relY = centerY - y
+    relY = y - centerY
 
     m.move(int(scaleX * relX), int(scaleY * relY), 0)
-
     buttons = nc.buttons
+
     c = buttons.C
     z = buttons.Z
 
     if z and not zDown:
         stillDown = True
         for n in range(CHECK_COUNT):
             if nc.button_Z:
```

### Comparing `adafruit-circuitpython-nunchuk-1.1.8/pyproject.toml` & `adafruit-circuitpython-nunchuk-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-nunchuk"
 description = "CircuitPython library for Nintendo Nunchuk controller"
-version = "1.1.8"
+version = "1.1.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Nunchuk.git"}
 keywords = [
     "adafruit",
```

