# Comparing `tmp/riccati-1.1.0.tar.gz` & `tmp/riccati-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riccati-1.1.0.tar", last modified: Fri Jun  2 15:34:10 2023, max compression
+gzip compressed data, was "riccati-1.1.1.tar", last modified: Mon Jul 17 17:21:31 2023, max compression
```

## Comparing `riccati-1.1.0.tar` & `riccati-1.1.1.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.364724 riccati-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 15:33:57.000000 riccati-1.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 15:33:57.000000 riccati-1.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.360724 riccati-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.360724 riccati-1.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-02 15:33:57.000000 riccati-1.1.0/.github/ISSUE_TEMPLATE/issue-name.md
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-02 15:33:57.000000 riccati-1.1.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.360724 riccati-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-02 15:33:57.000000 riccati-1.1.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-02 15:33:57.000000 riccati-1.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 15:33:57.000000 riccati-1.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-02 15:33:57.000000 riccati-1.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-02 15:33:57.000000 riccati-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-02 15:34:10.364724 riccati-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-02 15:33:57.000000 riccati-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.360724 riccati-1.1.0/benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.360724 riccati-1.1.0/benchmarks/data/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-02 15:33:57.000000 riccati-1.1.0/benchmarks/data/eq237.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-06-02 15:33:57.000000 riccati-1.1.0/benchmarks/fig1.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-02 15:33:57.000000 riccati-1.1.0/benchmarks/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.360724 riccati-1.1.0/binder/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-02 15:33:57.000000 riccati-1.1.0/binder/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.364724 riccati-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)  1062708 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    81767 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.364724 riccati-1.1.0/joss-paper/
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-02 15:33:57.000000 riccati-1.1.0/joss-paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-06-02 15:33:57.000000 riccati-1.1.0/joss-paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)   322295 2023-06-02 15:33:57.000000 riccati-1.1.0/joss-paper/timing-fig.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    24397 2023-06-02 15:33:57.000000 riccati-1.1.0/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-02 15:33:57.000000 riccati-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-02 15:33:57.000000 riccati-1.1.0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 15:33:57.000000 riccati-1.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.364724 riccati-1.1.0/riccati/
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-02 15:33:57.000000 riccati-1.1.0/riccati/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-02 15:34:10.364724 riccati-1.1.0/riccati/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-06-02 15:33:57.000000 riccati-1.1.0/riccati/chebutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13782 2023-06-02 15:33:57.000000 riccati-1.1.0/riccati/evolve.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-02 15:33:57.000000 riccati-1.1.0/riccati/solversetup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-06-02 15:33:57.000000 riccati-1.1.0/riccati/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-02 15:33:57.000000 riccati-1.1.0/riccati/stepsize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.364724 riccati-1.1.0/riccati/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 15:33:57.000000 riccati-1.1.0/riccati/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-06-02 15:33:57.000000 riccati-1.1.0/riccati/tests/test_riccati.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.364724 riccati-1.1.0/riccati.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-02 15:34:10.000000 riccati-1.1.0/riccati.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-02 15:34:10.000000 riccati-1.1.0/riccati.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:34:10.000000 riccati-1.1.0/riccati.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-02 15:34:10.000000 riccati-1.1.0/riccati.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 15:34:10.000000 riccati-1.1.0/riccati.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 15:34:10.364724 riccati-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-02 15:33:57.000000 riccati-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:21:31.229423 riccati-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 17:21:17.000000 riccati-1.1.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 17:21:17.000000 riccati-1.1.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:21:31.221423 riccati-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:21:31.221423 riccati-1.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-17 17:21:17.000000 riccati-1.1.1/.github/ISSUE_TEMPLATE/issue-name.md
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-17 17:21:17.000000 riccati-1.1.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:21:31.221423 riccati-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-17 17:21:17.000000 riccati-1.1.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 17:21:17.000000 riccati-1.1.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 17:21:17.000000 riccati-1.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-17 17:21:17.000000 riccati-1.1.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-17 17:21:17.000000 riccati-1.1.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-17 17:21:17.000000 riccati-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-17 17:21:31.229423 riccati-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-17 17:21:17.000000 riccati-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:21:31.221423 riccati-1.1.1/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:21:31.221423 riccati-1.1.1/benchmarks/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-17 17:21:17.000000 riccati-1.1.1/benchmarks/data/eq237.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-07-17 17:21:17.000000 riccati-1.1.1/benchmarks/fig1.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-17 17:21:17.000000 riccati-1.1.1/benchmarks/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:21:31.221423 riccati-1.1.1/binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-17 17:21:17.000000 riccati-1.1.1/binder/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:21:31.225423 riccati-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-17 17:21:17.000000 riccati-1.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-17 17:21:17.000000 riccati-1.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-17 17:21:17.000000 riccati-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1062708 2023-07-17 17:21:17.000000 riccati-1.1.1/docs/examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-17 17:21:17.000000 riccati-1.1.1/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-17 17:21:17.000000 riccati-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-17 17:21:17.000000 riccati-1.1.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    81767 2023-07-17 17:21:17.000000 riccati-1.1.1/docs/quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-17 17:21:17.000000 riccati-1.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:21:31.225423 riccati-1.1.1/joss-paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-17 17:21:17.000000 riccati-1.1.1/joss-paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-07-17 17:21:17.000000 riccati-1.1.1/joss-paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)   322295 2023-07-17 17:21:17.000000 riccati-1.1.1/joss-paper/timing-fig.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    24397 2023-07-17 17:21:17.000000 riccati-1.1.1/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-17 17:21:17.000000 riccati-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-17 17:21:17.000000 riccati-1.1.1/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-17 17:21:17.000000 riccati-1.1.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:21:31.225423 riccati-1.1.1/riccati/
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-17 17:21:17.000000 riccati-1.1.1/riccati/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-17 17:21:31.229423 riccati-1.1.1/riccati/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-07-17 17:21:17.000000 riccati-1.1.1/riccati/chebutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-07-17 17:21:17.000000 riccati-1.1.1/riccati/evolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-07-17 17:21:17.000000 riccati-1.1.1/riccati/solversetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-17 17:21:17.000000 riccati-1.1.1/riccati/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-17 17:21:17.000000 riccati-1.1.1/riccati/stepsize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:21:31.229423 riccati-1.1.1/riccati/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:21:17.000000 riccati-1.1.1/riccati/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-07-17 17:21:17.000000 riccati-1.1.1/riccati/tests/test_riccati.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:21:31.229423 riccati-1.1.1/riccati.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-17 17:21:31.000000 riccati-1.1.1/riccati.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-17 17:21:31.000000 riccati-1.1.1/riccati.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:21:31.000000 riccati-1.1.1/riccati.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-17 17:21:31.000000 riccati-1.1.1/riccati.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 17:21:31.000000 riccati-1.1.1/riccati.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 17:21:31.229423 riccati-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-17 17:21:17.000000 riccati-1.1.1/setup.py
```

### Comparing `riccati-1.1.0/.github/ISSUE_TEMPLATE/issue-name.md` & `riccati-1.1.1/.github/ISSUE_TEMPLATE/issue-name.md`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/.github/workflows/tests.yml` & `riccati-1.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/CONTRIBUTING.md` & `riccati-1.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/LICENSE` & `riccati-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/PKG-INFO` & `riccati-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riccati
-Version: 1.1.0
+Version: 1.1.1
 Summary: adaptive Riccati defect correction solver
 Home-page: 
 Author: Fruzsina J Agocs and Alex H Barnett
 Author-email: 
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: all
@@ -16,15 +16,15 @@
 ![Riccati logo](https://github.com/fruzsinaagocs/riccati/blob/master/logo.png?raw=true)
 
 
 # riccati
 
 **A package implementing the adaptive Riccati defect correction (ARDC) method**
 
-
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05430/status.svg)](https://doi.org/10.21105/joss.05430)
 [![Documentation Status](https://readthedocs.org/projects/riccati/badge/?version=latest)](https://riccati.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/fruzsinaagocs/riccati/branch/master/graph/badge.svg?token=XA47G7P1XM)](https://codecov.io/gh/fruzsinaagocs/riccati)
 
 ## About
 
 `riccati` is a `Python` package for solving ODEs of the form
```

### Comparing `riccati-1.1.0/README.md` & `riccati-1.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![Riccati logo](https://github.com/fruzsinaagocs/riccati/blob/master/logo.png?raw=true)
 
 
 # riccati
 
 **A package implementing the adaptive Riccati defect correction (ARDC) method**
 
-
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05430/status.svg)](https://doi.org/10.21105/joss.05430)
 [![Documentation Status](https://readthedocs.org/projects/riccati/badge/?version=latest)](https://riccati.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/fruzsinaagocs/riccati/branch/master/graph/badge.svg?token=XA47G7P1XM)](https://codecov.io/gh/fruzsinaagocs/riccati)
 
 ## About
 
 `riccati` is a `Python` package for solving ODEs of the form
```

### Comparing `riccati-1.1.0/benchmarks/fig1.py` & `riccati-1.1.1/benchmarks/fig1.py`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/docs/Makefile` & `riccati-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/docs/api.rst` & `riccati-1.1.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/docs/conf.py` & `riccati-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/docs/examples.ipynb` & `riccati-1.1.1/docs/examples.ipynb`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/docs/favicon.ico` & `riccati-1.1.1/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/docs/index.rst` & `riccati-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/docs/installation.rst` & `riccati-1.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/docs/quickstart.ipynb` & `riccati-1.1.1/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/joss-paper/paper.bib` & `riccati-1.1.1/joss-paper/paper.bib`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 @misc{ardc,
 author = {Agocs, F J and Barnett, A H},
 keywords = {Numerical Analysis (math.NA), FOS: Mathematics, FOS: Mathematics},
-title = {An adaptive spectral method for oscillatory second-order linear ODEs with frequency-independent cost},
+title = {An adaptive spectral method for oscillatory second-order linear {ODEs} with frequency-independent cost},
 publisher = {arXiv},
 year = {2022},
 doi = {10.48550/arxiv.2212.06924}
 }
 
 @article{oscode-joss,
 year = {2020}, 
 publisher = {The Open Journal}, 
 volume = {5}, 
 number = {56},
 pages = {2830}, 
 author = {Agocs, F J}, 
-title = {{(py)oscode: fast solutions of oscillatory ODEs}}, 
+title = {{(py)}oscode: fast solutions of oscillatory {ODEs}}, 
 journal = {Journal of Open Source Software},
 doi = {10.21105/joss.02830}
 }
 
 @article{oscode-theory,
 title={Efficient method for solving highly oscillatory ordinary differential equations with applications to physical systems},
 author={Agocs, F J and Handley, W J and Lasenby, A N and Hobson, M P},
@@ -59,26 +59,26 @@
 pages={437--483},
 year={1997},
 publisher={Cambridge University Press},
 doi={10.1017/S0962492900002750}
 }
 
 @article{wkbmarching1,
-title={{WKB-based scheme with adaptive step size control for the Schr{\"o}dinger equation in the highly oscillatory regime}},
+title={{WKB}-based scheme with adaptive step size control for the {S}chr{\"o}dinger equation in the highly oscillatory regime},
 author={K{\"o}rner, Jannis and Arnold, Anton and D{\"o}pfner, Kirian},
 journal={Journal of Computational and Applied Mathematics},
 volume={404},
 pages={113905},
 year={2022},
 publisher={Elsevier},
 doi = {10.1016/j.cam.2021.113905}
 }
 
 @article{wkbmarching2,
-title={{WKB-based schemes for the oscillatory 1D Schr{\"o}dinger equation in the semiclassical limit}},
+title={WKB-based schemes for the oscillatory 1{D} {S}chr{\"o}dinger equation in the semiclassical limit},
 author={Arnold, Anton and Abdallah, Naoufel Ben and Negulescu, Claudia},
 journal={SIAM journal on numerical analysis},
 volume={49},
 number={4},
 pages={1436--1460},
 year={2011},
 publisher={SIAM},
@@ -95,25 +95,25 @@
           Kern, Robert and Larson, Eric and Carey, C J and
           Polat, {\.I}lhan and Feng, Yu and Moore, Eric W. and
           {VanderPlas}, Jake and Laxalde, Denis and Perktold, Josef and
           Cimrman, Robert and Henriksen, Ian and Quintero, E. A. and
           Harris, Charles R. and Archibald, Anne M. and
           Ribeiro, Ant{\^o}nio H. and Pedregosa, Fabian and
           {van Mulbregt}, Paul and {SciPy 1.0 Contributors}},
-title   = {{{SciPy} 1.0: Fundamental Algorithms for Scientific
-          Computing in Python}},
+title   = {{SciPy} 1.0: Fundamental Algorithms for Scientific
+          Computing in Python},
 journal = {Nature Methods},
 year    = {2020},
 volume  = {17},
 pages   = {261--272},
 doi     = {10.1038/s41592-019-0686-2},
 }
 
 @article{dop853,
-title={A family of embedded Runge-Kutta formulae},
+title={A family of embedded {R}unge-{K}utta formulae},
 author={Dormand, John R and Prince, Peter J},
 journal={Journal of computational and applied mathematics},
 volume={6},
 number={1},
 pages={19--26},
 year={1980},
 publisher={Elsevier},
```

### Comparing `riccati-1.1.0/joss-paper/paper.md` & `riccati-1.1.1/joss-paper/paper.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
 ---
 
 # Summary
 
 Highly oscillatory ordinary differential equations (ODEs) pose a computational
 challenge for standard solvers available in scientific computing libraries. 
-These conventional methods are typically based on a polynomial approximation
-resulting in several timesteps per oscillation period, and hence runtimes
+These conventional methods are typically based on a polynomial approximation,
+resulting in there being several timesteps per oscillation period, which leads to runtimes
 scaling as $\mathcal{O}(\omega)$, with $\omega$ being the oscillation
-frequency. This can get prohibitively slow.
+frequency. This can become prohibitively slow.
 
 The `riccati`
 (Python) package implements the efficient numerical method described in @ardc
 (dubbed ARDC for adaptive Riccati defect correction) for solving ODEs of the
 form
 \begin{equation}\label{eq:ode}
 u''(t) + 2\gamma(t)u'(t) + \omega^2(t) u(t) = 0, \quad t \in [t_0, t_1],
@@ -39,15 +39,15 @@
 and friction $\gamma(t)$ terms are given smooth real-valued functions (passed in as callables). The
 solution $u(t)$ may vary between highly oscillatory and slowly-changing over the
 integration range, in which case `riccati` will switch between using nonoscillatory
 (spectral Chebyshev) and a specialised oscillatory solver (Riccati defect
 correction) to achieve an $\mathcal{O}(1)$
 (frequency-independent) runtime. It automatically adapts its stepsize to
 attempt to reach a user-requested relative error tolerance. The solver is
-capable of producing _dense output_, i.e. can return a numerical
+capable of producing _dense output_, i.e., it can return a numerical
 solution estimate at a user-selected set of $t$-values, at the cost of a few
 arithmetic operations per $t$-point.
 
 # Statement of need
 
 Specialised numerical methods exist to solve \autoref{eq:ode} in
 the high-frequency ($\omega \gg 1$) regime, but of those that have software implementations,
@@ -65,27 +65,27 @@
 coefficients $\omega(t)$, $\gamma(t)$ (in the oscillatory regime), and that of
 the solution $u(t)$ (in the nonoscillatory regime) allows. 
 `oscode` [@oscode-joss; @oscode-theory] and the WKB-marching method[^1]
 [@wkbmarching1; @wkbmarching2] are examples of low-order adaptive oscillatory
 solvers, efficient when no more than about 6 digits of accuracy are required or $\omega(t)$ is near-constant.
 A high-order alternative is the Kummer's phase function-based method 
 [@kummerphase; @phasefntp], whose current implementation supports solving
-\autoref{eq:ode} in the highly oscillatory regime when $\gamma \equiv 0$. Other existing numerical methods are
-reviewed in e.g. @petzoldrev. \autoref{fig:solver-comparison} compares the
+\autoref{eq:ode} in the highly oscillatory regime when $\gamma \equiv 0$. Other existing numerical methods have been
+reviewed, e.g., in @petzoldrev. \autoref{fig:solver-comparison} compares the
 performance of the above specialised solvers and one of SciPy's [@scipy] built-in methods [@dop853]
 by plotting their runtime against the frequency parameter $\lambda$ while
 solving
 \begin{equation}\label{eq:runtime-ode}
 u'' + \omega^2(t) u = 0, \quad \text{where} \quad \omega^2(t) = \lambda^2(1 - t^2\cos 3t ),
 \end{equation}
 on the interval $t \in [-1, 1]$, subject to the initial conditions $u(-1) = 0$,
 $u'(-1) = \lambda$. The runtimes were measured at two settings of the required
 relative tolerance $\varepsilon$, $10^{-6}$ and $10^{-12}$. The figure
 demonstrates the advantage `riccati`'s adaptivity provides at low tolerances.
-`riccati` avoids the runtime-increase `oscode` and the WKB marching method exhibit
+`riccati` avoids the runtime increase `oscode` and the WKB marching method exhibit
 at low-to-intermediate frequencies, and its runtime is virtually
 independent of the oscillation frequency. 
 
 ![Left: Numerical solution of \autoref{eq:runtime-ode} with $\lambda = 10^2$. Right: performance comparison of `riccati` (labelled ARDC) against state-of-the-art oscillatory solvers. `oscode`, the WKB marching method, Kummer's phase function method, and a high-order Runge--Kutta method (RK78) [@dop853] on \autoref{eq:runtime-ode} with a varying frequency parameter $\lambda$. Solid and dashed lines denote runs with a relative tolerance settings of $\varepsilon = 10^{-12}$ and $10^{-6}$, respectively. \label{fig:solver-comparison}](timing-fig.pdf)
 
 
 [^1]: Available from [https://github.com/JannisKoerner/adaptive-WKB-marching-method](https://github.com/JannisKoerner/adaptive-WKB-marching-method).
```

### Comparing `riccati-1.1.0/joss-paper/timing-fig.pdf` & `riccati-1.1.1/joss-paper/timing-fig.pdf`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/logo.png` & `riccati-1.1.1/logo.png`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/riccati/__init__.py` & `riccati-1.1.1/riccati/__init__.py`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/riccati/chebutils.py` & `riccati-1.1.1/riccati/chebutils.py`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/riccati/evolve.py` & `riccati-1.1.1/riccati/evolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,24 +170,24 @@
         Objects containing differentiation matrices, etc.
     xi, xf: float
         Solution range.
     yi, dyi: complex
         Initial conditions, value of the dependent variable and its derivative at `xi`.
     eps: float
         Relative tolerance for the local error of both Riccati and Chebyshev type steps.
-    epsh: float
+    epsh: float 
         Relative tolerance for choosing the stepsize of Riccati steps.
-    xeval: list
+    xeval: list 
         List of x-values where the solution is to be interpolated (dense output) and returned.
-    hard_stop: bool
+    hard_stop: bool 
         Whether to force the solver to have a potentially smaller last
         stepsize, in order to stop exactly at `xf` (rather than allowing the
         solver to step over it and get the value of the solution by
         interpolation).
-    warn: bool
+    warn: bool 
         Whether to display warnings, e.g. RuntimeWarnings, during a run. Due to
         the high level of adaptivity in this algorithm, it may throw several
         RuntimeWarnings even in a standard setup as it chooses the type of
         step, stepsize, and other parameters. For this reason, all warnings are
         silenced by default (`warn = False`). Set to `True` if you wish to see
         the warnings.
 
@@ -199,14 +199,18 @@
         Values of the dependent variable and its derivative at the internal steps of the solver.
     successes: list [int]
         Has elements 1 and 0: 1 denoting each successful step, 0 denoting unsuccessful steps. 
     phases:  list [complex]
         Complex phase of the solution accumulated during each successful Riccati step.
     steptypes: list [int]
         Types of successful steps taken: 1 for Riccati and 0 for Chebyshev. 
+    yeval: numpy.array [complex]
+        Dense output, i.e. values of the solution at the requested
+        independent-variable values specified in `xeval`. If `xeval` was not
+        given, then it is an empty numpy array of shape (0,).
     """
     if warn == False:
         warnings.simplefilter("ignore")
     else:
         warnings.simplefilter("default")
 
     w = info.w
@@ -220,14 +224,16 @@
     # Is there dense output?
     info.denseout = False
     denselen = len(xeval)
     if denselen > 0:
         info.denseout = True
         info.intmat = integrationm(n+1)
         yeval = np.zeros(denselen, dtype = complex)
+    else:
+        yeval = np.empty(0)
     
     # Check if stepsize sign is consistent with direction of integration
     if (xf - xi)*hi < 0:
         warnings.warn("Direction of itegration does not match stepsize sign,\
                 adjusting it so that integration happens from xi to xf.")
         hi *= -1
 
@@ -308,15 +314,15 @@
         # Log step
         if steptype == 1:
             h = hosc
         else:
             h = hslo
         # If there were dense output points, check where:
         if info.denseout:
-            positions = np.logical_or(np.logical_and(intdir*xeval >= intdir*xcurrent, intdir*xeval < intdir*(xcurrent+h)), xeval == xf)
+            positions = np.logical_or(np.logical_and(intdir*xeval >= intdir*xcurrent, intdir*xeval < intdir*(xcurrent+h)), np.logical_and(xeval == xf, xeval == xcurrent + h))
             xdense = xeval[positions] 
             if steptype == 1:
                 #xscaled = xcurrent + h/2 + h/2*info.xn
                 xscaled = 2/h*(xdense - xcurrent) - 1
                 Linterp = interp(info.xn, xscaled)
                 udense = Linterp @ info.un
                 fdense = np.exp(udense)
@@ -351,12 +357,9 @@
                     hosc_ini = xf - xcurrent
                 if intdir*(xcurrent + hslo_ini) > intdir*xf:
                     hslo_ini = xf - xcurrent
             hosc = choose_osc_stepsize(info, xcurrent, hosc_ini, epsh = epsh)  
             hslo = choose_nonosc_stepsize(info, xcurrent, hslo_ini)
             yprev = y
             dyprev = dy
-    if info.denseout:
-        return xs, ys, dys, successes, phases, steptypes, yeval
-    else:
-        return xs, ys, dys, successes, phases, steptypes
+    return xs, ys, dys, successes, phases, steptypes, yeval
```

### Comparing `riccati-1.1.0/riccati/solversetup.py` & `riccati-1.1.1/riccati/solversetup.py`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/riccati/step.py` & `riccati-1.1.1/riccati/step.py`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/riccati/stepsize.py` & `riccati-1.1.1/riccati/stepsize.py`

 * *Files identical despite different names*

### Comparing `riccati-1.1.0/riccati/tests/test_riccati.py` & `riccati-1.1.1/riccati/tests/test_riccati.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     Neval = int(1e2)
     xeval = np.linspace(xi, xf, Neval) 
     xs, ys, dys, ss, ps, stypes, yeval = solve(info, xi, xf, yi, dyi,\
                                                        xeval = xeval,\
                                                        eps = eps, epsh = epsh)
     ytrue = np.array([mpmath.airyai(-x) + 1j*mpmath.airybi(-x) for x in xeval])
     yerr = np.abs((ytrue - yeval)/ytrue)
+    print(yeval, ytrue)
     maxerr = max(yerr)
     assert maxerr < 1e-6
 
 def test_denseoutput_xbac():
     w = lambda x: np.sqrt(x)
     g = lambda x: np.zeros_like(x)
     info = solversetup(w, g, n = 32, p = 32)
@@ -142,15 +143,15 @@
     info = solversetup(w, g, n = 32, p = 32)
     xi = 1e0
     xf = 1e6
     eps = 1e-12
     epsh = 1e-13
     yi = sp.airy(-xi)[0] + 1j*sp.airy(-xi)[2]
     dyi = -sp.airy(-xi)[1] - 1j*sp.airy(-xi)[3]
-    xs, ys, dys, ss, ps, stypes = solve(info, xi, xf, yi, dyi, eps = eps, epsh = epsh)
+    xs, ys, dys, ss, ps, stypes, yeval = solve(info, xi, xf, yi, dyi, eps = eps, epsh = epsh)
     xs = np.array(xs)
     ys = np.array(ys)
     ytrue = np.array([mpmath.airyai(-x) + 1j*mpmath.airybi(-x) for x in xs])
     yerr = np.abs((ytrue - ys)/ytrue)
     maxerr = max(yerr)
     print(maxerr)
     assert maxerr < 1e-6
@@ -161,15 +162,15 @@
     info = solversetup(w, g, n = 32, p = 32)
     xi = 1e6
     xf = 1e0
     eps = 1e-12
     epsh = 1e-13
     yi = sp.airy(-xi)[0] + 1j*sp.airy(-xi)[2]
     dyi = -sp.airy(-xi)[1] - 1j*sp.airy(-xi)[3]
-    xs, ys, dys, ss, ps, stypes = solve(info, xi, xf, yi, dyi,\
+    xs, ys, dys, ss, ps, stypes, yeval = solve(info, xi, xf, yi, dyi,\
                                                 eps = eps, epsh = epsh,\
                                                 hard_stop = True)
     xs = np.array(xs)
     ys = np.array(ys)
     ytrue = np.array([mpmath.airyai(-x) + 1j*mpmath.airybi(-x) for x in xs])
     yerr = np.abs((ytrue - ys)/ytrue)
     maxerr = max(yerr)
@@ -230,15 +231,15 @@
     xi = -m
     xf = m
     yi = bursty(xi)
     dyi = burstdy(xi)
     eps = 1e-10
     epsh = 1e-12
     info = solversetup(w, g, n = 32, p = 32)
-    xs, ys, dys, ss, ps, types = solve(info, xi, xf, yi, dyi, eps = eps, epsh = epsh)
+    xs, ys, dys, ss, ps, types, yeval = solve(info, xi, xf, yi, dyi, eps = eps, epsh = epsh)
     xs = np.array(xs)
     ys = np.array(ys)
     ytrue = bursty(xs)
     yerr = np.abs((ytrue - ys))/np.abs(ytrue)
     maxerr = max(yerr)
     assert maxerr < 2e-7
```

### Comparing `riccati-1.1.0/riccati.egg-info/PKG-INFO` & `riccati-1.1.1/riccati.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riccati
-Version: 1.1.0
+Version: 1.1.1
 Summary: adaptive Riccati defect correction solver
 Home-page: 
 Author: Fruzsina J Agocs and Alex H Barnett
 Author-email: 
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: all
@@ -16,15 +16,15 @@
 ![Riccati logo](https://github.com/fruzsinaagocs/riccati/blob/master/logo.png?raw=true)
 
 
 # riccati
 
 **A package implementing the adaptive Riccati defect correction (ARDC) method**
 
-
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05430/status.svg)](https://doi.org/10.21105/joss.05430)
 [![Documentation Status](https://readthedocs.org/projects/riccati/badge/?version=latest)](https://riccati.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/fruzsinaagocs/riccati/branch/master/graph/badge.svg?token=XA47G7P1XM)](https://codecov.io/gh/fruzsinaagocs/riccati)
 
 ## About
 
 `riccati` is a `Python` package for solving ODEs of the form
```

### Comparing `riccati-1.1.0/riccati.egg-info/SOURCES.txt` & `riccati-1.1.1/riccati.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .coveragerc
 .gitattributes
 .gitmodules
 CHANGELOG.rst
+CITATION.cff
 CONTRIBUTING.md
 LICENSE
 README.md
 logo.png
 pyproject.toml
 readthedocs.yml
 requirements.txt
```

### Comparing `riccati-1.1.0/setup.py` & `riccati-1.1.1/setup.py`

 * *Files identical despite different names*

