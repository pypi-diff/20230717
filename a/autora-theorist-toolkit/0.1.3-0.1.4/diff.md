# Comparing `tmp/autora-theorist-toolkit-0.1.3.tar.gz` & `tmp/autora-theorist-toolkit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-toolkit-0.1.3.tar", last modified: Thu Jul 13 17:17:45 2023, max compression
+gzip compressed data, was "autora-theorist-toolkit-0.1.4.tar", last modified: Mon Jul 17 19:21:40 2023, max compression
```

## Comparing `autora-theorist-toolkit-0.1.3.tar` & `autora-theorist-toolkit-0.1.4.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:45.691906 autora-theorist-toolkit-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:45.683905 autora-theorist-toolkit-0.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:45.683905 autora-theorist-toolkit-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:45.683905 autora-theorist-toolkit-0.1.3/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/.idea/autora-theorist-toolkit.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:45.683905 autora-theorist-toolkit-0.1.3/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-13 17:17:45.691906 autora-theorist-toolkit-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:45.683905 autora-theorist-toolkit-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/docs/Additional Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:45.683905 autora-theorist-toolkit-0.1.3/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:45.683905 autora-theorist-toolkit-0.1.3/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:17:45.691906 autora-theorist-toolkit-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:45.683905 autora-theorist-toolkit-0.1.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:45.683905 autora-theorist-toolkit-0.1.3/src/autora/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:45.683905 autora-theorist-toolkit-0.1.3/src/autora/theorist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:45.683905 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:45.687906 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/components/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/components/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:45.687906 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/methods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/methods/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/methods/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/methods/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/methods/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:45.687906 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/models/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/models/symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/models/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:45.687906 autora-theorist-toolkit-0.1.3/src/autora_theorist_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-13 17:17:45.000000 autora-theorist-toolkit-0.1.3/src/autora_theorist_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-13 17:17:45.000000 autora-theorist-toolkit-0.1.3/src/autora_theorist_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:17:45.000000 autora-theorist-toolkit-0.1.3/src/autora_theorist_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-13 17:17:45.000000 autora-theorist-toolkit-0.1.3/src/autora_theorist_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 17:17:45.000000 autora-theorist-toolkit-0.1.3/src/autora_theorist_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:45.687906 autora-theorist-toolkit-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-13 17:17:33.000000 autora-theorist-toolkit-0.1.3/tests/test_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:40.499237 autora-theorist-toolkit-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:40.491237 autora-theorist-toolkit-0.1.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:40.491237 autora-theorist-toolkit-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:40.491237 autora-theorist-toolkit-0.1.4/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/.idea/autora-theorist-toolkit.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:40.495237 autora-theorist-toolkit-0.1.4/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-17 19:21:40.499237 autora-theorist-toolkit-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:40.495237 autora-theorist-toolkit-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/docs/Additional Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:40.495237 autora-theorist-toolkit-0.1.4/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:40.495237 autora-theorist-toolkit-0.1.4/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 19:21:40.499237 autora-theorist-toolkit-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:40.495237 autora-theorist-toolkit-0.1.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:40.495237 autora-theorist-toolkit-0.1.4/src/autora/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:40.495237 autora-theorist-toolkit-0.1.4/src/autora/theorist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:40.495237 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:40.495237 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/components/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/components/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:40.495237 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/methods/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/methods/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/methods/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/methods/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:40.495237 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/models/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/models/symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/models/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:40.499237 autora-theorist-toolkit-0.1.4/src/autora_theorist_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-17 19:21:40.000000 autora-theorist-toolkit-0.1.4/src/autora_theorist_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-17 19:21:40.000000 autora-theorist-toolkit-0.1.4/src/autora_theorist_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:21:40.000000 autora-theorist-toolkit-0.1.4/src/autora_theorist_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 19:21:40.000000 autora-theorist-toolkit-0.1.4/src/autora_theorist_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 19:21:40.000000 autora-theorist-toolkit-0.1.4/src/autora_theorist_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:40.499237 autora-theorist-toolkit-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-17 19:21:28.000000 autora-theorist-toolkit-0.1.4/tests/test_toolkit.py
```

### Comparing `autora-theorist-toolkit-0.1.3/.github/pull_request_template.md` & `autora-theorist-toolkit-0.1.4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/.github/workflows/python-publish.yml` & `autora-theorist-toolkit-0.1.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/.gitignore` & `autora-theorist-toolkit-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/.idea/inspectionProfiles/Project_Default.xml` & `autora-theorist-toolkit-0.1.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/.pre-commit-config.yaml` & `autora-theorist-toolkit-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/PKG-INFO` & `autora-theorist-toolkit-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-toolkit
-Version: 0.1.3
+Version: 0.1.4
 Summary: Toolkit to build algorithms for model recovery
 Author-email: "Joshua T. S. Hewson" <joshua_hewson@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/TheLemonPig/autora-theorist-toolkit
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-toolkit-0.1.3/README.md` & `autora-theorist-toolkit-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/docs/Additional Example.ipynb` & `autora-theorist-toolkit-0.1.4/docs/Additional Example.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/docs/Basic Usage.ipynb` & `autora-theorist-toolkit-0.1.4/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/docs/index.md` & `autora-theorist-toolkit-0.1.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/mkdocs/base.yml` & `autora-theorist-toolkit-0.1.4/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/pyproject.toml` & `autora-theorist-toolkit-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/components/nodes.py` & `autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/components/nodes.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/components/primitives.py` & `autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/components/primitives.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/methods/fitting.py` & `autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/methods/fitting.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/methods/metrics.py` & `autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/methods/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from sklearn.metrics import mean_squared_error
-from src.autora.theorist.toolkit.models.symbolic_regression import SymbolicRegressor
+from autora.theorist.toolkit.models.symbolic_regression import SymbolicRegressor
 
 
 def continuous_log_loss(mse):
     return np.log(mse)
 
 
 def continuous_bayesian_information_criterion(y_true, y_pred, n, k):
```

### Comparing `autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/methods/regression.py` & `autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/methods/regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import functools
 import warnings
-from src.autora.theorist.toolkit.methods.fitting import FittingError
+from autora.theorist.toolkit.methods.fitting import FittingError
 from sympy import sympify
 from scipy.optimize import OptimizeWarning
 import functools
 
 
 def regression_handler(func):
     @functools.wraps(func)
```

### Comparing `autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/methods/rules.py` & `autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/methods/rules.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py` & `autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import logging
 from tqdm import tqdm
-from src.autora.theorist.toolkit.components.primitives import Arithmetic, SimpleFunction
-from src.autora.theorist.toolkit.methods.rules import replace_node
-from src.autora.theorist.toolkit.models.bayesian_symbolic_regression import BayesianSymbolicRegressor
-from src.autora.theorist.toolkit.methods.metrics import minimum_description_length
-from src.autora.theorist.toolkit.methods.regression import clean_equation
+from autora.theorist.toolkit.components.primitives import Arithmetic, SimpleFunction
+from autora.theorist.toolkit.methods.rules import replace_node
+from autora.theorist.toolkit.models.bayesian_symbolic_regression import BayesianSymbolicRegressor
+from autora.theorist.toolkit.methods.metrics import minimum_description_length
+from autora.theorist.toolkit.methods.regression import clean_equation
 from sklearn.metrics import mean_squared_error
 import random
 
 logging.basicConfig(level=logging.INFO)
 _logger = logging.getLogger(__name__)
```

### Comparing `autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py` & `autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from src.autora.theorist.toolkit.models.symbolic_regression import SymbolicRegressor
-from src.autora.theorist.toolkit.methods.rules import add_root, remove_root, replace_node
-from src.autora.theorist.toolkit.methods.metrics import minimum_description_length
-from src.autora.theorist.toolkit.methods.fitting import scipy_curve_fit
-from src.autora.theorist.toolkit.methods.regression import regression_handler
+from autora.theorist.toolkit.models.symbolic_regression import SymbolicRegressor
+from autora.theorist.toolkit.methods.rules import add_root, remove_root, replace_node
+from autora.theorist.toolkit.methods.metrics import minimum_description_length
+from autora.theorist.toolkit.methods.fitting import scipy_curve_fit
+from autora.theorist.toolkit.methods.regression import regression_handler
 import random
 
 
 class BayesianSymbolicRegressor(SymbolicRegressor):
 
     def __init__(self, prior_dict, temperature=1.0, tree=None, moves=None):
         super().__init__(tree, moves)
```

### Comparing `autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/models/memory.py` & `autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/models/memory.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py` & `autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import logging
 from tqdm import tqdm
 import random
-from src.autora.theorist.toolkit.components.primitives import Arithmetic, SimpleFunction
-from src.autora.theorist.toolkit.models.symbolic_regression import SymbolicRegressor
-from src.autora.theorist.toolkit.methods.metrics import MinimumDescriptionLength
-from src.autora.theorist.toolkit.methods.rules import replace_node
+from autora.theorist.toolkit.components.primitives import Arithmetic, SimpleFunction
+from autora.theorist.toolkit.models.symbolic_regression import SymbolicRegressor
+from autora.theorist.toolkit.methods.metrics import MinimumDescriptionLength
+from autora.theorist.toolkit.methods.rules import replace_node
 
 logging.basicConfig(level=logging.INFO)
 _logger = logging.getLogger(__name__)
 
 
 class ParallelSymbolicRegressor:
```

### Comparing `autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/models/symbolic_regression.py` & `autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/models/symbolic_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 from tqdm import tqdm
 from inspect import signature
 from typing import List
 from copy import deepcopy
 import pandas as pd
 import random
 
-from src.autora.theorist.toolkit.components.nodes import Variable, Parameter, Operator
-from src.autora.theorist.toolkit.components.primitives import default_primitives
-from src.autora.theorist.toolkit.models.tree import Tree
-from src.autora.theorist.toolkit.models.memory import Stack
-from src.autora.theorist.toolkit.methods.fitting import scipy_curve_fit
-from src.autora.theorist.toolkit.methods.regression import regression_handler, canonical
-from src.autora.theorist.toolkit.methods.rules import less_than
+from autora.theorist.toolkit.components.nodes import Variable, Parameter, Operator
+from autora.theorist.toolkit.components.primitives import default_primitives
+from autora.theorist.toolkit.models.tree import Tree
+from autora.theorist.toolkit.models.memory import Stack
+from autora.theorist.toolkit.methods.fitting import scipy_curve_fit
+from autora.theorist.toolkit.methods.regression import regression_handler, canonical
+from autora.theorist.toolkit.methods.rules import less_than
 
 
 class SymbolicRegressor(BaseEstimator):
 
     # TODO: replace tree=None with expression=None once build_tree() is made
     def __init__(self, tree=None, moves=None, primitives=None,
                  metric=None):
```

### Comparing `autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/models/tree.py` & `autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/models/tree.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/src/autora/theorist/toolkit/utils.py` & `autora-theorist-toolkit-0.1.4/src/autora/theorist/toolkit/utils.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/src/autora_theorist_toolkit.egg-info/PKG-INFO` & `autora-theorist-toolkit-0.1.4/src/autora_theorist_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-toolkit
-Version: 0.1.3
+Version: 0.1.4
 Summary: Toolkit to build algorithms for model recovery
 Author-email: "Joshua T. S. Hewson" <joshua_hewson@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/TheLemonPig/autora-theorist-toolkit
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-toolkit-0.1.3/src/autora_theorist_toolkit.egg-info/SOURCES.txt` & `autora-theorist-toolkit-0.1.4/src/autora_theorist_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/tests/README.md` & `autora-theorist-toolkit-0.1.4/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.1.3/tests/test_toolkit.py` & `autora-theorist-toolkit-0.1.4/tests/test_toolkit.py`

 * *Files identical despite different names*

