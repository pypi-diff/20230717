# Comparing `tmp/adafruit-circuitpython-focaltouch-1.4.8.tar.gz` & `tmp/adafruit-circuitpython-focaltouch-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-focaltouch-1.4.8.tar", last modified: Fri May 26 16:16:51 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-focaltouch-1.4.9.tar", last modified: Mon Jul 17 16:29:54 2023, max compression
```

## Comparing `adafruit-circuitpython-focaltouch-1.4.8.tar` & `adafruit-circuitpython-focaltouch-1.4.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.331114 adafruit-circuitpython-focaltouch-1.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.331114 adafruit-circuitpython-focaltouch-1.4.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/adafruit_circuitpython_focaltouch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-26 16:16:51.000000 adafruit-circuitpython-focaltouch-1.4.8/adafruit_circuitpython_focaltouch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-26 16:16:51.000000 adafruit-circuitpython-focaltouch-1.4.8/adafruit_circuitpython_focaltouch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:16:51.000000 adafruit-circuitpython-focaltouch-1.4.8/adafruit_circuitpython_focaltouch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 16:16:51.000000 adafruit-circuitpython-focaltouch-1.4.8/adafruit_circuitpython_focaltouch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 16:16:51.000000 adafruit-circuitpython-focaltouch-1.4.8/adafruit_circuitpython_focaltouch.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     5629 2023-05-26 16:16:44.000000 adafruit-circuitpython-focaltouch-1.4.8/adafruit_focaltouch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-26 16:16:44.000000 adafruit-circuitpython-focaltouch-1.4.8/examples/focaltouch_paint_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-26 16:16:44.000000 adafruit-circuitpython-focaltouch-1.4.8/examples/focaltouch_print_touches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-26 16:16:44.000000 adafruit-circuitpython-focaltouch-1.4.8/examples/focaltouch_print_touches_with_irq.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-26 16:16:44.000000 adafruit-circuitpython-focaltouch-1.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:29:54.710730 adafruit-circuitpython-focaltouch-1.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:29:54.706730 adafruit-circuitpython-focaltouch-1.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:29:54.706730 adafruit-circuitpython-focaltouch-1.4.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:29:54.706730 adafruit-circuitpython-focaltouch-1.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:29:54.706730 adafruit-circuitpython-focaltouch-1.4.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-17 16:29:54.710730 adafruit-circuitpython-focaltouch-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:29:54.706730 adafruit-circuitpython-focaltouch-1.4.9/adafruit_circuitpython_focaltouch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-17 16:29:54.000000 adafruit-circuitpython-focaltouch-1.4.9/adafruit_circuitpython_focaltouch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-17 16:29:54.000000 adafruit-circuitpython-focaltouch-1.4.9/adafruit_circuitpython_focaltouch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:29:54.000000 adafruit-circuitpython-focaltouch-1.4.9/adafruit_circuitpython_focaltouch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-17 16:29:54.000000 adafruit-circuitpython-focaltouch-1.4.9/adafruit_circuitpython_focaltouch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 16:29:54.000000 adafruit-circuitpython-focaltouch-1.4.9/adafruit_circuitpython_focaltouch.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5629 2023-07-17 16:29:47.000000 adafruit-circuitpython-focaltouch-1.4.9/adafruit_focaltouch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:29:54.710730 adafruit-circuitpython-focaltouch-1.4.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:29:54.710730 adafruit-circuitpython-focaltouch-1.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:29:54.710730 adafruit-circuitpython-focaltouch-1.4.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-17 16:29:47.000000 adafruit-circuitpython-focaltouch-1.4.9/examples/focaltouch_paint_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-17 16:29:47.000000 adafruit-circuitpython-focaltouch-1.4.9/examples/focaltouch_print_touches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-17 16:29:47.000000 adafruit-circuitpython-focaltouch-1.4.9/examples/focaltouch_print_touches_with_irq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-17 16:29:47.000000 adafruit-circuitpython-focaltouch-1.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-17 16:29:37.000000 adafruit-circuitpython-focaltouch-1.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 16:29:54.710730 adafruit-circuitpython-focaltouch-1.4.9/setup.cfg
```

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-focaltouch-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/.gitignore` & `adafruit-circuitpython-focaltouch-1.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/.pre-commit-config.yaml` & `adafruit-circuitpython-focaltouch-1.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/.pylintrc` & `adafruit-circuitpython-focaltouch-1.4.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-focaltouch-1.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/LICENSE` & `adafruit-circuitpython-focaltouch-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-focaltouch-1.4.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/LICENSES/MIT.txt` & `adafruit-circuitpython-focaltouch-1.4.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-focaltouch-1.4.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/PKG-INFO` & `adafruit-circuitpython-focaltouch-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-focaltouch
-Version: 1.4.8
+Version: 1.4.9
 Summary: CircuitPython Focaltouch library for capacitive touch displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Focaltouch
 Keywords: adafruit,focaltouch,capacitive,touch,screen,display,touchscreenhardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/README.rst` & `adafruit-circuitpython-focaltouch-1.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/adafruit_circuitpython_focaltouch.egg-info/PKG-INFO` & `adafruit-circuitpython-focaltouch-1.4.9/adafruit_circuitpython_focaltouch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-focaltouch
-Version: 1.4.8
+Version: 1.4.9
 Summary: CircuitPython Focaltouch library for capacitive touch displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Focaltouch
 Keywords: adafruit,focaltouch,capacitive,touch,screen,display,touchscreenhardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/adafruit_circuitpython_focaltouch.egg-info/SOURCES.txt` & `adafruit-circuitpython-focaltouch-1.4.9/adafruit_circuitpython_focaltouch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/adafruit_focaltouch.py` & `adafruit-circuitpython-focaltouch-1.4.9/adafruit_focaltouch.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   https://github.com/adafruit/circuitpython/releases
 * Adafruit's Bus Device library (when using I2C/SPI):
   https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 """
 
 # imports
 
-__version__ = "1.4.8"
+__version__ = "1.4.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FocalTouch.git"
 
 import struct
 
 from adafruit_bus_device.i2c_device import I2CDevice
 
 from micropython import const
```

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/docs/_static/favicon.ico` & `adafruit-circuitpython-focaltouch-1.4.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/docs/conf.py` & `adafruit-circuitpython-focaltouch-1.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/docs/index.rst` & `adafruit-circuitpython-focaltouch-1.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/examples/focaltouch_paint_simpletest.py` & `adafruit-circuitpython-focaltouch-1.4.9/examples/focaltouch_paint_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/examples/focaltouch_print_touches.py` & `adafruit-circuitpython-focaltouch-1.4.9/examples/focaltouch_print_touches.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.8/pyproject.toml` & `adafruit-circuitpython-focaltouch-1.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-focaltouch"
 description = "CircuitPython Focaltouch library for capacitive touch displays."
-version = "1.4.8"
+version = "1.4.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Focaltouch"}
 keywords = [
     "adafruit",
```

