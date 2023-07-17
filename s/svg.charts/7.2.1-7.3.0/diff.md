# Comparing `tmp/svg.charts-7.2.1.tar.gz` & `tmp/svg.charts-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svg.charts-7.2.1.tar", last modified: Tue Jul 20 01:22:26 2021, max compression
+gzip compressed data, was "svg.charts-7.3.0.tar", last modified: Mon Jul 17 01:44:37 2023, max compression
```

## Comparing `svg.charts-7.2.1.tar` & `svg.charts-7.3.0.tar`

### file list

```diff
@@ -1,54 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 01:22:26.060401 svg.charts-7.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-07-20 01:22:05.000000 svg.charts-7.2.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-07-20 01:22:05.000000 svg.charts-7.2.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-07-20 01:22:05.000000 svg.charts-7.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 01:22:26.056401 svg.charts-7.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2021-07-20 01:22:05.000000 svg.charts-7.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 01:22:26.056401 svg.charts-7.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2021-07-20 01:22:05.000000 svg.charts-7.2.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-07-20 01:22:05.000000 svg.charts-7.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-07-20 01:22:05.000000 svg.charts-7.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     7182 2021-07-20 01:22:05.000000 svg.charts-7.2.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-07-20 01:22:05.000000 svg.charts-7.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2973 2021-07-20 01:22:26.060401 svg.charts-7.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2345 2021-07-20 01:22:05.000000 svg.charts-7.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 01:22:26.056401 svg.charts-7.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      790 2021-07-20 01:22:05.000000 svg.charts-7.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-07-20 01:22:05.000000 svg.charts-7.2.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      232 2021-07-20 01:22:05.000000 svg.charts-7.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2021-07-20 01:22:05.000000 svg.charts-7.2.1/docs/svg.charts.rst
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-07-20 01:22:05.000000 svg.charts-7.2.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-07-20 01:22:05.000000 svg.charts-7.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      416 2021-07-20 01:22:05.000000 svg.charts-7.2.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-07-20 01:22:26.064401 svg.charts-7.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-07-20 01:22:05.000000 svg.charts-7.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 01:22:26.056401 svg.charts-7.2.1/svg/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 01:22:26.060401 svg.charts-7.2.1/svg/charts/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2021-07-20 01:22:05.000000 svg.charts-7.2.1/svg/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2021-07-20 01:22:05.000000 svg.charts-7.2.1/svg/charts/bar.css
--rw-r--r--   0 runner    (1001) docker     (121)     8497 2021-07-20 01:22:05.000000 svg.charts-7.2.1/svg/charts/bar.py
--rw-r--r--   0 runner    (1001) docker     (121)     3149 2021-07-20 01:22:05.000000 svg.charts-7.2.1/svg/charts/css.py
--rw-r--r--   0 runner    (1001) docker     (121)     1623 2021-07-20 01:22:05.000000 svg.charts-7.2.1/svg/charts/graph.css
--rw-r--r--   0 runner    (1001) docker     (121)    25183 2021-07-20 01:22:05.000000 svg.charts-7.2.1/svg/charts/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     5952 2021-07-20 01:22:05.000000 svg.charts-7.2.1/svg/charts/line.py
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2021-07-20 01:22:05.000000 svg.charts-7.2.1/svg/charts/pie.css
--rw-r--r--   0 runner    (1001) docker     (121)     9386 2021-07-20 01:22:05.000000 svg.charts-7.2.1/svg/charts/pie.py
--rw-r--r--   0 runner    (1001) docker     (121)     2705 2021-07-20 01:22:05.000000 svg.charts-7.2.1/svg/charts/plot.css
--rw-r--r--   0 runner    (1001) docker     (121)    12702 2021-07-20 01:22:05.000000 svg.charts-7.2.1/svg/charts/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)    10080 2021-07-20 01:22:05.000000 svg.charts-7.2.1/svg/charts/schedule.py
--rw-r--r--   0 runner    (1001) docker     (121)     6283 2021-07-20 01:22:05.000000 svg.charts-7.2.1/svg/charts/time_series.py
--rw-r--r--   0 runner    (1001) docker     (121)      936 2021-07-20 01:22:05.000000 svg.charts-7.2.1/svg/charts/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 01:22:26.056401 svg.charts-7.2.1/svg.charts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2973 2021-07-20 01:22:25.000000 svg.charts-7.2.1/svg.charts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      856 2021-07-20 01:22:26.000000 svg.charts-7.2.1/svg.charts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-20 01:22:25.000000 svg.charts-7.2.1/svg.charts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      378 2021-07-20 01:22:25.000000 svg.charts-7.2.1/svg.charts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-07-20 01:22:25.000000 svg.charts-7.2.1/svg.charts.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 01:22:26.060401 svg.charts-7.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     6342 2021-07-20 01:22:05.000000 svg.charts-7.2.1/tests/samples.py
--rw-r--r--   0 runner    (1001) docker     (121)     2684 2021-07-20 01:22:05.000000 svg.charts-7.2.1/tests/source.csv
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-07-20 01:22:05.000000 svg.charts-7.2.1/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (121)     3572 2021-07-20 01:22:05.000000 svg.charts-7.2.1/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)      171 2021-07-20 01:22:05.000000 svg.charts-7.2.1/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (121)      567 2021-07-20 01:22:05.000000 svg.charts-7.2.1/tests/test_time_series.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2021-07-20 01:22:05.000000 svg.charts-7.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:44:37.190320 svg.charts-7.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-17 01:44:08.000000 svg.charts-7.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-17 01:44:08.000000 svg.charts-7.3.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:44:37.186320 svg.charts-7.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 01:44:08.000000 svg.charts-7.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:44:37.186320 svg.charts-7.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-17 01:44:08.000000 svg.charts-7.3.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-17 01:44:08.000000 svg.charts-7.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 01:44:08.000000 svg.charts-7.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-17 01:44:08.000000 svg.charts-7.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-07-17 01:44:08.000000 svg.charts-7.3.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-17 01:44:37.190320 svg.charts-7.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-17 01:44:08.000000 svg.charts-7.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:44:37.186320 svg.charts-7.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-17 01:44:08.000000 svg.charts-7.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 01:44:08.000000 svg.charts-7.3.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-17 01:44:08.000000 svg.charts-7.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-17 01:44:08.000000 svg.charts-7.3.0/docs/svg.charts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-17 01:44:08.000000 svg.charts-7.3.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-17 01:44:08.000000 svg.charts-7.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 01:44:08.000000 svg.charts-7.3.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-17 01:44:37.190320 svg.charts-7.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:44:37.182320 svg.charts-7.3.0/svg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:44:37.190320 svg.charts-7.3.0/svg/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 01:44:08.000000 svg.charts-7.3.0/svg/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-17 01:44:08.000000 svg.charts-7.3.0/svg/charts/bar.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-07-17 01:44:08.000000 svg.charts-7.3.0/svg/charts/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-17 01:44:08.000000 svg.charts-7.3.0/svg/charts/css.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-17 01:44:08.000000 svg.charts-7.3.0/svg/charts/graph.css
+-rw-r--r--   0 runner    (1001) docker     (123)    25183 2023-07-17 01:44:08.000000 svg.charts-7.3.0/svg/charts/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-07-17 01:44:08.000000 svg.charts-7.3.0/svg/charts/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-17 01:44:08.000000 svg.charts-7.3.0/svg/charts/pie.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-17 01:44:08.000000 svg.charts-7.3.0/svg/charts/pie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-17 01:44:08.000000 svg.charts-7.3.0/svg/charts/plot.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-07-17 01:44:08.000000 svg.charts-7.3.0/svg/charts/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-07-17 01:44:08.000000 svg.charts-7.3.0/svg/charts/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-17 01:44:08.000000 svg.charts-7.3.0/svg/charts/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-17 01:44:08.000000 svg.charts-7.3.0/svg/charts/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:44:37.186320 svg.charts-7.3.0/svg.charts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-17 01:44:37.000000 svg.charts-7.3.0/svg.charts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-17 01:44:37.000000 svg.charts-7.3.0/svg.charts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 01:44:37.000000 svg.charts-7.3.0/svg.charts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-17 01:44:37.000000 svg.charts-7.3.0/svg.charts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-17 01:44:37.000000 svg.charts-7.3.0/svg.charts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 01:44:37.190320 svg.charts-7.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-07-17 01:44:08.000000 svg.charts-7.3.0/tests/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-17 01:44:08.000000 svg.charts-7.3.0/tests/source.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-17 01:44:08.000000 svg.charts-7.3.0/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-17 01:44:08.000000 svg.charts-7.3.0/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-17 01:44:08.000000 svg.charts-7.3.0/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-17 01:44:08.000000 svg.charts-7.3.0/tests/test_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-17 01:44:08.000000 svg.charts-7.3.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-17 01:44:08.000000 svg.charts-7.3.0/tox.ini
```

### Comparing `svg.charts-7.2.1/CHANGES.rst` & `svg.charts-7.3.0/NEWS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v7.3.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
 v7.2.1
 ======
 
 Refreshed packaging.
 
 v7.2.0
 ======
```

### Comparing `svg.charts-7.2.1/LICENSE` & `svg.charts-7.3.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `svg.charts-7.2.1/PKG-INFO` & `svg.charts-7.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 Metadata-Version: 2.1
 Name: svg.charts
-Version: 7.2.1
+Version: 7.3.0
 Summary: Python SVG Charting Library
 Home-page: https://github.com/jaraco/svg.charts
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/svg.charts.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/svg.charts
 
 .. image:: https://img.shields.io/pypi/pyversions/svg.charts.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/svg.charts
 
 .. image:: https://github.com/jaraco/svg.charts/workflows/tests/badge.svg
    :target: https://github.com/jaraco/svg.charts/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/svgcharts/badge/?version=latest
+   :target: https://svgcharts.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2021-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 ``svg.charts`` is a pure-python library for generating charts
 and graphs using Scalable Vector Graphics.
 
 Acknowledgements
 ================
@@ -81,9 +80,7 @@
 
 This project is `hosted at Github
 <https://github.com/jaraco/svg.charts>`_.
 
 Please use that site for
 reporting bugs and requesting help. Patches and contributions
 of any kind are encouraged.
-
-
```

### Comparing `svg.charts-7.2.1/README.rst` & `svg.charts-7.3.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 .. image:: https://img.shields.io/pypi/v/svg.charts.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/svg.charts
 
 .. image:: https://img.shields.io/pypi/pyversions/svg.charts.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/svg.charts
 
 .. image:: https://github.com/jaraco/svg.charts/workflows/tests/badge.svg
    :target: https://github.com/jaraco/svg.charts/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/svgcharts/badge/?version=latest
+   :target: https://svgcharts.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2021-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 ``svg.charts`` is a pure-python library for generating charts
 and graphs using Scalable Vector Graphics.
 
 Acknowledgements
 ================
```

### Comparing `svg.charts-7.2.1/docs/svg.charts.rst` & `svg.charts-7.3.0/docs/svg.charts.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,87 +1,87 @@
 charts Package
 ==============
 
-:mod:`svg` Package
-------------------
+``svg`` Package
+---------------
 
 ``svg`` is a namespace package, meant to be shared with
 other libraries implementing svg functionality.
 
-:mod:`svg.charts` Package
--------------------------
+``svg.charts`` Package
+----------------------
 
 ``svg.charts`` is the package containing the various
 modules of this library.
 
-:mod:`bar` Module
------------------
+``bar`` Module
+--------------
 
 .. automodule:: svg.charts.bar
     :members:
     :undoc-members:
     :show-inheritance:
 
-:mod:`css` Module
------------------
+``css`` Module
+--------------
 
 .. automodule:: svg.charts.css
     :members:
     :undoc-members:
     :show-inheritance:
 
-:mod:`graph` Module
--------------------
+``graph`` Module
+----------------
 
 .. automodule:: svg.charts.graph
     :members:
     :undoc-members:
     :show-inheritance:
 
-:mod:`line` Module
-------------------
+``line`` Module
+---------------
 
 .. automodule:: svg.charts.line
     :members:
     :undoc-members:
     :show-inheritance:
 
-:mod:`pie` Module
------------------
+``pie`` Module
+--------------
 
 .. automodule:: svg.charts.pie
     :members:
     :undoc-members:
     :show-inheritance:
 
-:mod:`plot` Module
-------------------
+``plot`` Module
+---------------
 
 .. automodule:: svg.charts.plot
     :members:
     :undoc-members:
     :show-inheritance:
 
-:mod:`schedule` Module
-----------------------
+``schedule`` Module
+-------------------
 
 .. automodule:: svg.charts.schedule
     :members:
     :undoc-members:
     :show-inheritance:
 
-:mod:`time_series` Module
--------------------------
+``time_series`` Module
+----------------------
 
 .. automodule:: svg.charts.time_series
     :members:
     :undoc-members:
     :show-inheritance:
 
-:mod:`util` Module
-------------------
+``util`` Module
+---------------
 
 .. automodule:: svg.charts.util
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `svg.charts-7.2.1/setup.cfg` & `svg.charts-7.3.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = 
 	cssutils>=0.9.8a3
 	python-dateutil>=2.0
 	lxml>=2.0
 	more_itertools>=6
 	tempora>=1.3
 	importlib_resources; python_version < "3.7"
@@ -30,29 +30,31 @@
 	build*
 	dist*
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
-	pytest >= 4.6
+	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
-	pytest-mypy; \
+	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.0.1
+	pytest-enabler >= 2.2
+	pytest-ruff
 	
 	types-python-dateutil
 docs = 
-	sphinx
-	jaraco.packaging >= 8.2
+	sphinx >= 3.5
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
 
 [options.entry_points]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `svg.charts-7.2.1/svg/charts/bar.css` & `svg.charts-7.3.0/svg/charts/bar.css`

 * *Files identical despite different names*

### Comparing `svg.charts-7.2.1/svg/charts/bar.py` & `svg.charts-7.3.0/svg/charts/bar.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         return max(
             itertools.chain.from_iterable(map(lambda set: set['data'], self.data))
         )
         # above is same as
         # return max(map(lambda set: max(set['data']), self.data))
 
     def data_min(self):
-        if not getattr(self, 'min_scale_value') is None:
+        if getattr(self, 'min_scale_value') is not None:
             return self.min_scale_value
         min_value = min(
             itertools.chain.from_iterable(map(lambda set: set['data'], self.data))
         )
         min_value = min(min_value, 0)
         return min_value
```

### Comparing `svg.charts-7.2.1/svg/charts/css.py` & `svg.charts-7.3.0/svg/charts/css.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,18 +29,14 @@
     # Interactivity Properties
     'pointer-events': 'visiblePainted|visibleFill|visibleStroke|visible'
     '|painted|fill|stroke|all|none|inherit',
     # Color and Pointing Properties
     'color-interpolation': 'auto|sRGB|linearRGB|inherit',
     'color-interpolation-filters': 'auto|sRGB|linearRGB|inherit',
     'color-rendering': 'auto|optimizeSpeed|optimizeQuality|inherit',
-    'shape-rendering': 'auto|optimizeSpeed|crispEdges|geometricPrecision|inherit',
-    'text-rendering': (
-        'auto|optimizeSpeed|optimizeLegibility|geometricPrecision|inherit'
-    ),
     'fill': '{paint}',
     'fill-opacity': '{num}|inherit',
     'fill-rule': 'nonzero|evenodd|inherit',
     'image-rendering': 'auto|optimizeSpeed|optimizeQuality|inherit',
     'marker': 'none|inherit|{uri}',
     'marker-end': 'none|inherit|{uri}',
     'marker-mid': 'none|inherit|{uri}',
@@ -62,13 +58,16 @@
     'dominant-baseline': 'auto|use-script|no-change|reset-size|ideographic'
     '|alphabetic|hanging||mathematical|central|middle'
     '|text-after-edge|text-before-edge|inherit',
     'glyph-orientation-horizontal': '{angle}|inherit',
     'glyph-orientation-vertical': 'auto|{angle}|inherit',
     'kerning': 'auto|{length}|inherit',
     'text-anchor': 'start|middle|end|inherit',
+    'text-rendering': (
+        'auto|optimizeSpeed|optimizeLegibility|geometricPrecision|inherit'
+    ),
     'writing-mode': 'lr-tb|rl-tb|tb-rl|lr|rl|tb|inherit',
 }
 
 cssutils.profile.addProfile(SVG, properties, macros)
 
 cssutils.profile.defaultProfiles = [SVG, cssutils.profile.CSS_LEVEL_2]
```

### Comparing `svg.charts-7.2.1/svg/charts/graph.css` & `svg.charts-7.3.0/svg/charts/graph.css`

 * *Files identical despite different names*

### Comparing `svg.charts-7.2.1/svg/charts/graph.py` & `svg.charts-7.3.0/svg/charts/graph.py`

 * *Files identical despite different names*

### Comparing `svg.charts-7.2.1/svg/charts/line.py` & `svg.charts-7.3.0/svg/charts/line.py`

 * *Files identical despite different names*

### Comparing `svg.charts-7.2.1/svg/charts/pie.css` & `svg.charts-7.3.0/svg/charts/pie.css`

 * *Files identical despite different names*

### Comparing `svg.charts-7.2.1/svg/charts/pie.py` & `svg.charts-7.3.0/svg/charts/pie.py`

 * *Files identical despite different names*

### Comparing `svg.charts-7.2.1/svg/charts/plot.css` & `svg.charts-7.3.0/svg/charts/plot.css`

 * *Files identical despite different names*

### Comparing `svg.charts-7.2.1/svg/charts/plot.py` & `svg.charts-7.3.0/svg/charts/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         if len(series) % 2 != 0:
             tmpl = "Expecting x,y pairs for data points for %s."
             msg = tmpl % self.__class__.__name__
             raise ValueError(msg)
 
     def validate_data_pairs(self, series):
         # Should be pairs (or wider tuples).
-        for (i, p) in enumerate(series):
+        for i, p in enumerate(series):
             if len(p) < 2:
                 tmpl = "Expecting (x,y) pairs for data points for %s."
                 msg = tmpl % self.__class__.__name__
                 raise ValueError(msg)
 
     def process_data(self, data):
         series = data['data']
@@ -371,15 +371,15 @@
         x = (x - x_min) * x_step
         y = self.graph_height - (y - y_min) * y_step
         return x, y
 
     def draw_data_points(self, line, data_points, graph_points):
         if not self.show_data_points and not self.show_data_values:
             return
-        for (dp, (gx, gy)) in zip(data_points, graph_points):
+        for dp, (gx, gy) in zip(data_points, graph_points):
             dx = dp[0]
             dy = dp[1]
             if self.show_data_points:
                 doc = {
                     'cx': str(gx),
                     'cy': str(gy),
                     'r': '2.5',
```

### Comparing `svg.charts-7.2.1/svg/charts/schedule.py` & `svg.charts-7.3.0/svg/charts/schedule.py`

 * *Files identical despite different names*

### Comparing `svg.charts-7.2.1/svg/charts/time_series.py` & `svg.charts-7.3.0/svg/charts/time_series.py`

 * *Files identical despite different names*

### Comparing `svg.charts-7.2.1/svg/charts/util.py` & `svg.charts-7.3.0/svg/charts/util.py`

 * *Files identical despite different names*

### Comparing `svg.charts-7.2.1/svg.charts.egg-info/PKG-INFO` & `svg.charts-7.3.0/svg.charts.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 Metadata-Version: 2.1
 Name: svg.charts
-Version: 7.2.1
+Version: 7.3.0
 Summary: Python SVG Charting Library
 Home-page: https://github.com/jaraco/svg.charts
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/svg.charts.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/svg.charts
 
 .. image:: https://img.shields.io/pypi/pyversions/svg.charts.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/svg.charts
 
 .. image:: https://github.com/jaraco/svg.charts/workflows/tests/badge.svg
    :target: https://github.com/jaraco/svg.charts/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/svgcharts/badge/?version=latest
+   :target: https://svgcharts.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2021-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 ``svg.charts`` is a pure-python library for generating charts
 and graphs using Scalable Vector Graphics.
 
 Acknowledgements
 ================
@@ -81,9 +80,7 @@
 
 This project is `hosted at Github
 <https://github.com/jaraco/svg.charts>`_.
 
 Please use that site for
 reporting bugs and requesting help. Patches and contributions
 of any kind are encouraged.
-
-
```

### Comparing `svg.charts-7.2.1/svg.charts.egg-info/SOURCES.txt` & `svg.charts-7.3.0/svg.charts.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 .coveragerc
 .editorconfig
-.flake8
 .pre-commit-config.yaml
-.readthedocs.yml
-CHANGES.rst
+.readthedocs.yaml
 LICENSE
+NEWS.rst
 README.rst
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
-setup.py
+towncrier.toml
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
 docs/svg.charts.rst
```

### Comparing `svg.charts-7.2.1/tests/samples.py` & `svg.charts-7.3.0/tests/samples.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,14 @@
 
 
 class SampleBar:
     fields = ['Internet', 'TV', 'Newspaper', 'Magazine', 'Radio']
 
     @classmethod
     def vertical(cls):
-
         g = bar.VerticalBar(cls.fields)
 
         g.stack = 'side'
         g.scale_integers = True
         g.width, g.height = 640, 480
         g.graph_title = 'Question 7'
         g.show_graph_title = True
```

### Comparing `svg.charts-7.2.1/tests/source.csv` & `svg.charts-7.3.0/tests/source.csv`

 * *Files identical despite different names*

### Comparing `svg.charts-7.2.1/tests/test_plot.py` & `svg.charts-7.3.0/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `svg.charts-7.2.1/tests/test_time_series.py` & `svg.charts-7.3.0/tests/test_time_series.py`

 * *Files identical despite different names*

