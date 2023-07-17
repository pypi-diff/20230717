# Comparing `tmp/circuitpython-uplot-0.9.3.tar.gz` & `tmp/circuitpython-uplot-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-uplot-0.9.3.tar", last modified: Fri Mar 10 14:34:55 2023, max compression
+gzip compressed data, was "circuitpython-uplot-0.9.4.tar", last modified: Fri Mar 10 14:44:13 2023, max compression
```

## Comparing `circuitpython-uplot-0.9.3.tar` & `circuitpython-uplot-0.9.4.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:34:55.594005 circuitpython-uplot-0.9.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:34:55.582005 circuitpython-uplot-0.9.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:34:55.586005 circuitpython-uplot-0.9.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:34:55.586005 circuitpython-uplot-0.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:34:55.586005 circuitpython-uplot-0.9.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-10 14:34:55.594005 circuitpython-uplot-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:34:55.586005 circuitpython-uplot-0.9.3/circuitpython_uplot/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/circuitpython_uplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/circuitpython_uplot/ubar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/circuitpython_uplot/ucartesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/circuitpython_uplot/ufillbetween.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/circuitpython_uplot/ulogging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/circuitpython_uplot/umap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/circuitpython_uplot/upie.py
--rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/circuitpython_uplot/uplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/circuitpython_uplot/uscatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:34:55.586005 circuitpython-uplot-0.9.3/circuitpython_uplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-10 14:34:55.000000 circuitpython-uplot-0.9.3/circuitpython_uplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-03-10 14:34:55.000000 circuitpython-uplot-0.9.3/circuitpython_uplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 14:34:55.000000 circuitpython-uplot-0.9.3/circuitpython_uplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-10 14:34:55.000000 circuitpython-uplot-0.9.3/circuitpython_uplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-10 14:34:55.000000 circuitpython-uplot-0.9.3/circuitpython_uplot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:34:55.594005 circuitpython-uplot-0.9.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:34:55.594005 circuitpython-uplot-0.9.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/quick_start.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/quick_start.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/readme.png
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/readme.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)   221907 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_cartesian.gif
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_cartesian.gif.license
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex1.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    22878 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex10.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex10.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex11.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex11.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    13589 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex12.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex12.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex15.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex15.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex16.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex16.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    34215 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex17.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex17.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex3.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex4.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    12133 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex5.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex6.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex6.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    22393 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex7.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex7.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex8.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex8.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex9.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/docs/uplot_ex9.jpg.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:34:55.594005 circuitpython-uplot-0.9.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/examples/uplot_display_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/examples/uplot_integration_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/examples/uplot_plot_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/examples/uplot_readme_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/examples/uplot_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/examples/uplot_sparkline.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/examples/uplot_stackplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/examples/uplot_tickparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/examples/uplot_ubar_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/examples/uplot_uboxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/examples/uplot_ucartesian_advanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/examples/uplot_ucartesian_loggin_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/examples/uplot_ufillbetween.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/examples/uplot_ulogging.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/examples/uplot_umap.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/examples/uplot_upie_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/examples/uplot_uscatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-10 14:34:48.000000 circuitpython-uplot-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-10 14:34:39.000000 circuitpython-uplot-0.9.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 14:34:55.594005 circuitpython-uplot-0.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.885950 circuitpython-uplot-0.9.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.873950 circuitpython-uplot-0.9.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.873950 circuitpython-uplot-0.9.4/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.877950 circuitpython-uplot-0.9.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.877950 circuitpython-uplot-0.9.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-10 14:44:13.885950 circuitpython-uplot-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.877950 circuitpython-uplot-0.9.4/circuitpython_uplot/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/ubar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/ucartesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/ufillbetween.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/ulogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/umap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/upie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/uplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/circuitpython_uplot/uscatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.877950 circuitpython-uplot-0.9.4/circuitpython_uplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-10 14:44:13.000000 circuitpython-uplot-0.9.4/circuitpython_uplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-03-10 14:44:13.000000 circuitpython-uplot-0.9.4/circuitpython_uplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 14:44:13.000000 circuitpython-uplot-0.9.4/circuitpython_uplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-10 14:44:13.000000 circuitpython-uplot-0.9.4/circuitpython_uplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-10 14:44:13.000000 circuitpython-uplot-0.9.4/circuitpython_uplot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.881950 circuitpython-uplot-0.9.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.881950 circuitpython-uplot-0.9.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/quick_start.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/quick_start.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/readme.png
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/readme.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   221907 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_cartesian.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_cartesian.gif.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex1.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)    22878 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex10.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex10.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex11.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex11.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)    13589 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex12.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex12.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex15.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex15.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex16.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex16.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)    34215 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex17.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex17.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex3.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex4.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)    12133 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex5.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex6.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex6.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)    22393 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex7.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex7.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex8.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex8.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex9.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/docs/uplot_ex9.jpg.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:44:13.885950 circuitpython-uplot-0.9.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_display_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_integration_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_plot_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_readme_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_sparkline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_stackplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_tickparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_ubar_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_uboxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_ucartesian_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_ucartesian_loggin_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_ufillbetween.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_ulogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_umap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_upie_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/examples/uplot_uscatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-10 14:44:06.000000 circuitpython-uplot-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-10 14:43:59.000000 circuitpython-uplot-0.9.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 14:44:13.885950 circuitpython-uplot-0.9.4/setup.cfg
```

### Comparing `circuitpython-uplot-0.9.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-uplot-0.9.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/.gitignore` & `circuitpython-uplot-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/.pre-commit-config.yaml` & `circuitpython-uplot-0.9.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/.pylintrc` & `circuitpython-uplot-0.9.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/CODE_OF_CONDUCT.md` & `circuitpython-uplot-0.9.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/LICENSE` & `circuitpython-uplot-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/LICENSES/CC-BY-4.0.txt` & `circuitpython-uplot-0.9.4/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/LICENSES/MIT.txt` & `circuitpython-uplot-0.9.4/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/LICENSES/Unlicense.txt` & `circuitpython-uplot-0.9.4/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/PKG-INFO` & `circuitpython-uplot-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-uplot
-Version: 0.9.3
+Version: 0.9.4
 Summary: framework to display different plots in displayio. similar to widget
 Author-email: "Jose D. Montoya" <uplot@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_uplot
 Keywords: adafruit,blinka,circuitpython,uplot,bar,stackplot,fillbetween,piechart,scatter,displayio,circuitpython,graphics,plot,library,plotting,ulab
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-uplot-0.9.3/README.rst` & `circuitpython-uplot-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/circuitpython_uplot/ubar.py` & `circuitpython-uplot-0.9.4/circuitpython_uplot/ubar.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 try:
     from circuitpython_uplot.uplot import Uplot
 except ImportError:
     pass
 from bitmaptools import draw_line
 from vectorio import Rectangle
 
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 # pylint: disable=too-many-arguments, invalid-name, protected-access
 # pylint: disable=too-few-public-methods, no-self-use
 class ubar:
     """
     Main class to display different graphics
```

### Comparing `circuitpython-uplot-0.9.3/circuitpython_uplot/ucartesian.py` & `circuitpython-uplot-0.9.4/circuitpython_uplot/ucartesian.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     from circuitpython_uplot.uplot import Uplot
 except ImportError:
     pass
 from bitmaptools import draw_line, fill_region
 from ulab import numpy as np
 from vectorio import Polygon
 
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 
 # pylint: disable=too-many-arguments, invalid-name, no-self-use, too-few-public-methods
 # pylint: disable=too-many-locals, too-many-branches
 class ucartesian:
     """
```

### Comparing `circuitpython-uplot-0.9.3/circuitpython_uplot/ufillbetween.py` & `circuitpython-uplot-0.9.4/circuitpython_uplot/ufillbetween.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     from circuitpython_uplot.uplot import Uplot
 except ImportError:
     pass
 from ulab import numpy as np
 from vectorio import Polygon
 
 
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 # pylint: disable=too-many-arguments, invalid-name, no-self-use, too-few-public-methods
 # pylint: disable=too-many-locals
 class ufillbetween:
     """
     Class to draw a fillbetween graph
```

### Comparing `circuitpython-uplot-0.9.3/circuitpython_uplot/ulogging.py` & `circuitpython-uplot-0.9.4/circuitpython_uplot/ulogging.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     from typing import Union
     from circuitpython_uplot.uplot import Uplot
 except ImportError:
     pass
 from bitmaptools import draw_line, fill_region
 from ulab import numpy as np
 
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 
 # pylint: disable=too-many-arguments, invalid-name, no-self-use, too-few-public-methods
 # pylint: disable=too-many-locals, too-many-branches, protected-access
 class ulogging:
     """
```

### Comparing `circuitpython-uplot-0.9.3/circuitpython_uplot/umap.py` & `circuitpython-uplot-0.9.4/circuitpython_uplot/umap.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 except ImportError:
     pass
 
 from ulab import numpy as np
 import displayio
 from vectorio import Rectangle
 
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 
 # pylint: disable=too-few-public-methods, invalid-name, duplicate-code, too-many-locals, too-many-arguments
 # pylint: disable=unused-variable
 class umap:
     """
```

### Comparing `circuitpython-uplot-0.9.3/circuitpython_uplot/upie.py` & `circuitpython-uplot-0.9.4/circuitpython_uplot/upie.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except ImportError:
     pass
 
 
 import math
 from vectorio import Polygon
 
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 # pylint: disable=too-many-arguments, invalid-name, no-self-use
 class upie:
     """
     Class to draw pie
     """
```

### Comparing `circuitpython-uplot-0.9.3/circuitpython_uplot/uplot.py` & `circuitpython-uplot-0.9.4/circuitpython_uplot/uplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import displayio
 import terminalio
 from bitmaptools import draw_line
 from vectorio import Circle
 from ulab import numpy as np
 
 
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 
 # pylint: disable=too-many-arguments, too-many-instance-attributes, too-many-locals
 # pylint: disable=too-many-statements
 # pylint: disable=unused-import, import-outside-toplevel, undefined-variable
```

### Comparing `circuitpython-uplot-0.9.3/circuitpython_uplot/uscatter.py` & `circuitpython-uplot-0.9.4/circuitpython_uplot/uscatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     pass
 
 
 from ulab import numpy as np
 import displayio
 from vectorio import Circle
 
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 
 # pylint: disable=too-few-public-methods, invalid-name, duplicate-code, too-many-locals, too-many-arguments
 class uscatter:
     """
     Main class to display different graphics
```

### Comparing `circuitpython-uplot-0.9.3/circuitpython_uplot.egg-info/PKG-INFO` & `circuitpython-uplot-0.9.4/circuitpython_uplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-uplot
-Version: 0.9.3
+Version: 0.9.4
 Summary: framework to display different plots in displayio. similar to widget
 Author-email: "Jose D. Montoya" <uplot@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_uplot
 Keywords: adafruit,blinka,circuitpython,uplot,bar,stackplot,fillbetween,piechart,scatter,displayio,circuitpython,graphics,plot,library,plotting,ulab
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-uplot-0.9.3/circuitpython_uplot.egg-info/SOURCES.txt` & `circuitpython-uplot-0.9.4/circuitpython_uplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/_static/favicon.ico` & `circuitpython-uplot-0.9.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/api.rst` & `circuitpython-uplot-0.9.4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/conf.py` & `circuitpython-uplot-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/examples.rst` & `circuitpython-uplot-0.9.4/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/index.rst` & `circuitpython-uplot-0.9.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/quick_start.rst` & `circuitpython-uplot-0.9.4/docs/quick_start.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/readme.png` & `circuitpython-uplot-0.9.4/docs/readme.png`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/uplot_cartesian.gif` & `circuitpython-uplot-0.9.4/docs/uplot_cartesian.gif`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/uplot_ex1.jpg` & `circuitpython-uplot-0.9.4/docs/uplot_ex1.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/uplot_ex10.jpg` & `circuitpython-uplot-0.9.4/docs/uplot_ex10.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/uplot_ex11.jpg` & `circuitpython-uplot-0.9.4/docs/uplot_ex11.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/uplot_ex12.jpg` & `circuitpython-uplot-0.9.4/docs/uplot_ex12.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/uplot_ex15.jpg` & `circuitpython-uplot-0.9.4/docs/uplot_ex15.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/uplot_ex16.jpg` & `circuitpython-uplot-0.9.4/docs/uplot_ex16.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/uplot_ex17.jpg` & `circuitpython-uplot-0.9.4/docs/uplot_ex17.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/uplot_ex3.jpg` & `circuitpython-uplot-0.9.4/docs/uplot_ex3.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/uplot_ex4.jpg` & `circuitpython-uplot-0.9.4/docs/uplot_ex4.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/uplot_ex5.jpg` & `circuitpython-uplot-0.9.4/docs/uplot_ex5.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/uplot_ex6.jpg` & `circuitpython-uplot-0.9.4/docs/uplot_ex6.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/uplot_ex7.jpg` & `circuitpython-uplot-0.9.4/docs/uplot_ex7.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/uplot_ex8.jpg` & `circuitpython-uplot-0.9.4/docs/uplot_ex8.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/docs/uplot_ex9.jpg` & `circuitpython-uplot-0.9.4/docs/uplot_ex9.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/examples/uplot_display_shapes.py` & `circuitpython-uplot-0.9.4/examples/uplot_display_shapes.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/examples/uplot_integration_example.py` & `circuitpython-uplot-0.9.4/examples/uplot_integration_example.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/examples/uplot_plot_example.py` & `circuitpython-uplot-0.9.4/examples/uplot_plot_example.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/examples/uplot_readme_example.py` & `circuitpython-uplot-0.9.4/examples/uplot_readme_example.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/examples/uplot_sparkline.py` & `circuitpython-uplot-0.9.4/examples/uplot_sparkline.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/examples/uplot_stackplot.py` & `circuitpython-uplot-0.9.4/examples/uplot_stackplot.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/examples/uplot_tickparameters.py` & `circuitpython-uplot-0.9.4/examples/uplot_tickparameters.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/examples/uplot_ubar_example.py` & `circuitpython-uplot-0.9.4/examples/uplot_ubar_example.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/examples/uplot_uboxplot.py` & `circuitpython-uplot-0.9.4/examples/uplot_uboxplot.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/examples/uplot_ucartesian_advanced.py` & `circuitpython-uplot-0.9.4/examples/uplot_ucartesian_advanced.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/examples/uplot_ucartesian_loggin_data.py` & `circuitpython-uplot-0.9.4/examples/uplot_ucartesian_loggin_data.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/examples/uplot_ufillbetween.py` & `circuitpython-uplot-0.9.4/examples/uplot_ufillbetween.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/examples/uplot_ulogging.py` & `circuitpython-uplot-0.9.4/examples/uplot_ulogging.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/examples/uplot_umap.py` & `circuitpython-uplot-0.9.4/examples/uplot_umap.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/examples/uplot_uscatter.py` & `circuitpython-uplot-0.9.4/examples/uplot_uscatter.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-0.9.3/pyproject.toml` & `circuitpython-uplot-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-uplot"
 description = "framework to display different plots in displayio. similar to widget"
-version = "0.9.3"
+version = "0.9.4"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "uplot@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_uplot"}
 keywords = [
     "adafruit",
```

