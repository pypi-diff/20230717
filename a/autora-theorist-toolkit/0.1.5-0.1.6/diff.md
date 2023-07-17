# Comparing `tmp/autora-theorist-toolkit-0.1.5.tar.gz` & `tmp/autora-theorist-toolkit-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-toolkit-0.1.5.tar", last modified: Mon Jul 17 20:50:46 2023, max compression
+gzip compressed data, was "autora-theorist-toolkit-0.1.6.tar", last modified: Mon Jul 17 20:52:54 2023, max compression
```

## Comparing `autora-theorist-toolkit-0.1.5.tar` & `autora-theorist-toolkit-0.1.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:46.417241 autora-theorist-toolkit-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:46.409240 autora-theorist-toolkit-0.1.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:46.409240 autora-theorist-toolkit-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:46.409240 autora-theorist-toolkit-0.1.5/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/.idea/autora-theorist-toolkit.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:46.413241 autora-theorist-toolkit-0.1.5/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-17 20:50:46.417241 autora-theorist-toolkit-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:46.413241 autora-theorist-toolkit-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/docs/Additional Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:46.413241 autora-theorist-toolkit-0.1.5/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:46.413241 autora-theorist-toolkit-0.1.5/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:50:46.417241 autora-theorist-toolkit-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:46.413241 autora-theorist-toolkit-0.1.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:46.413241 autora-theorist-toolkit-0.1.5/src/autora/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:46.413241 autora-theorist-toolkit-0.1.5/src/autora/theorist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:46.413241 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:46.413241 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/components/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/components/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:46.413241 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/methods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/methods/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/methods/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/methods/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/methods/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:46.417241 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/models/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/models/symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/models/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:46.417241 autora-theorist-toolkit-0.1.5/src/autora_theorist_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-17 20:50:46.000000 autora-theorist-toolkit-0.1.5/src/autora_theorist_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-17 20:50:46.000000 autora-theorist-toolkit-0.1.5/src/autora_theorist_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:50:46.000000 autora-theorist-toolkit-0.1.5/src/autora_theorist_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 20:50:46.000000 autora-theorist-toolkit-0.1.5/src/autora_theorist_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 20:50:46.000000 autora-theorist-toolkit-0.1.5/src/autora_theorist_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:46.417241 autora-theorist-toolkit-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-17 20:50:32.000000 autora-theorist-toolkit-0.1.5/tests/test_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.348922 autora-theorist-toolkit-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.idea/autora-theorist-toolkit.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-17 20:52:54.348922 autora-theorist-toolkit-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/docs/Additional Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:52:54.348922 autora-theorist-toolkit-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.340922 autora-theorist-toolkit-0.1.6/src/autora/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.344922 autora-theorist-toolkit-0.1.6/src/autora/theorist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.344922 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.344922 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/components/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/components/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.344922 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.344922 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.348922 autora-theorist-toolkit-0.1.6/src/autora_theorist_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-17 20:52:54.000000 autora-theorist-toolkit-0.1.6/src/autora_theorist_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-17 20:52:54.000000 autora-theorist-toolkit-0.1.6/src/autora_theorist_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:52:54.000000 autora-theorist-toolkit-0.1.6/src/autora_theorist_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 20:52:54.000000 autora-theorist-toolkit-0.1.6/src/autora_theorist_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 20:52:54.000000 autora-theorist-toolkit-0.1.6/src/autora_theorist_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:54.348922 autora-theorist-toolkit-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-17 20:52:41.000000 autora-theorist-toolkit-0.1.6/tests/test_toolkit.py
```

### Comparing `autora-theorist-toolkit-0.1.5/.github/pull_request_template.md` & `autora-theorist-toolkit-0.1.6/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/.github/workflows/python-publish.yml` & `autora-theorist-toolkit-0.1.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/.gitignore` & `autora-theorist-toolkit-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/.idea/inspectionProfiles/Project_Default.xml` & `autora-theorist-toolkit-0.1.6/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/.pre-commit-config.yaml` & `autora-theorist-toolkit-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/PKG-INFO` & `autora-theorist-toolkit-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-toolkit
-Version: 0.1.5
+Version: 0.1.6
 Summary: Toolkit to build algorithms for model recovery
 Author-email: "Joshua T. S. Hewson" <joshua_hewson@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/TheLemonPig/autora-theorist-toolkit
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-toolkit-0.1.5/README.md` & `autora-theorist-toolkit-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/docs/Additional Example.ipynb` & `autora-theorist-toolkit-0.1.6/docs/Additional Example.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/docs/Basic Usage.ipynb` & `autora-theorist-toolkit-0.1.6/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/docs/index.md` & `autora-theorist-toolkit-0.1.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/mkdocs/base.yml` & `autora-theorist-toolkit-0.1.6/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/pyproject.toml` & `autora-theorist-toolkit-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/components/nodes.py` & `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/components/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Callable
 from inspect import signature
-from src.autora.theorist.toolkit.components.primitives import Arithmetic
+from autora.theorist.toolkit.components.primitives import Arithmetic
 
 ###############
 #       Objects
 ###############
 
 
 ###
```

### Comparing `autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/components/primitives.py` & `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/components/primitives.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/methods/fitting.py` & `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/fitting.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/methods/metrics.py` & `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/metrics.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/methods/regression.py` & `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/methods/rules.py` & `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/methods/rules.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py` & `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py` & `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/models/memory.py` & `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/memory.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py` & `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/models/symbolic_regression.py` & `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/symbolic_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/models/tree.py` & `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/models/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.autora.theorist.toolkit.components.nodes import Symbol, Parameter
+from autora.theorist.toolkit.components.nodes import Symbol, Parameter
 from typing import List
 
 
 ###
 # Tree(Model)
 ###
 # attributes:
```

### Comparing `autora-theorist-toolkit-0.1.5/src/autora/theorist/toolkit/utils.py` & `autora-theorist-toolkit-0.1.6/src/autora/theorist/toolkit/utils.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/src/autora_theorist_toolkit.egg-info/PKG-INFO` & `autora-theorist-toolkit-0.1.6/src/autora_theorist_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-toolkit
-Version: 0.1.5
+Version: 0.1.6
 Summary: Toolkit to build algorithms for model recovery
 Author-email: "Joshua T. S. Hewson" <joshua_hewson@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/TheLemonPig/autora-theorist-toolkit
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-toolkit-0.1.5/src/autora_theorist_toolkit.egg-info/SOURCES.txt` & `autora-theorist-toolkit-0.1.6/src/autora_theorist_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/tests/README.md` & `autora-theorist-toolkit-0.1.6/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.5/tests/test_toolkit.py` & `autora-theorist-toolkit-0.1.6/tests/test_toolkit.py`

 * *Files identical despite different names*

