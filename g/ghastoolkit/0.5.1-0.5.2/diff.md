# Comparing `tmp/ghastoolkit-0.5.1.tar.gz` & `tmp/ghastoolkit-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.5.1.tar", last modified: Sun Jul 16 19:23:06 2023, max compression
+gzip compressed data, was "ghastoolkit-0.5.2.tar", last modified: Mon Jul 17 12:02:40 2023, max compression
```

## Comparing `ghastoolkit-0.5.1.tar` & `ghastoolkit-0.5.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.783336 ghastoolkit-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-16 19:23:06.783336 ghastoolkit-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 19:23:06.783336 ghastoolkit-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.775337 ghastoolkit-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.779337 ghastoolkit-0.5.1/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.779337 ghastoolkit-0.5.1/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.779337 ghastoolkit-0.5.1/src/ghastoolkit/codeql/dataextensions/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/dataextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/dataextensions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/dataextensions/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/dataextensions/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.779337 ghastoolkit-0.5.1/src/ghastoolkit/codeql/packs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/packs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/packs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/packs/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/packs/packs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.783336 ghastoolkit-0.5.1/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.783336 ghastoolkit-0.5.1/src/ghastoolkit/octokit/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.783336 ghastoolkit-0.5.1/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.783336 ghastoolkit-0.5.1/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.779337 ghastoolkit-0.5.1/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-16 19:23:06.000000 ghastoolkit-0.5.1/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-16 19:23:06.000000 ghastoolkit-0.5.1/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 19:23:06.000000 ghastoolkit-0.5.1/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-16 19:23:06.000000 ghastoolkit-0.5.1/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-16 19:23:06.000000 ghastoolkit-0.5.1/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.783336 ghastoolkit-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_codeql_dataext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.337580 ghastoolkit-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-17 12:02:40.337580 ghastoolkit-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 12:02:40.337580 ghastoolkit-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.329580 ghastoolkit-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.329580 ghastoolkit-0.5.2/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.333580 ghastoolkit-0.5.2/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.333580 ghastoolkit-0.5.2/src/ghastoolkit/codeql/dataextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/dataextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/dataextensions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/dataextensions/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/dataextensions/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.333580 ghastoolkit-0.5.2/src/ghastoolkit/codeql/packs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/packs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/packs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/packs/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/packs/packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.333580 ghastoolkit-0.5.2/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.333580 ghastoolkit-0.5.2/src/ghastoolkit/octokit/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.333580 ghastoolkit-0.5.2/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.333580 ghastoolkit-0.5.2/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.333580 ghastoolkit-0.5.2/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-17 12:02:40.000000 ghastoolkit-0.5.2/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-17 12:02:40.000000 ghastoolkit-0.5.2/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:02:40.000000 ghastoolkit-0.5.2/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-17 12:02:40.000000 ghastoolkit-0.5.2/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 12:02:40.000000 ghastoolkit-0.5.2/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.337580 ghastoolkit-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_codeql_dataext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.5.1/LICENSE` & `ghastoolkit-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/PKG-INFO` & `ghastoolkit-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.5.1
+Version: 0.5.2
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.5.1/README.md` & `ghastoolkit-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/pyproject.toml` & `ghastoolkit-0.5.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.5.1"
+version = "0.5.2"
 authors = [{ name = "GeekMasher" }]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/__init__.py` & `ghastoolkit-0.5.2/src/ghastoolkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
```

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/__main__.py` & `ghastoolkit-0.5.2/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/codeql/cli.py` & `ghastoolkit-0.5.2/src/ghastoolkit/codeql/cli.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.5.2/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/codeql/dataextensions/__main__.py` & `ghastoolkit-0.5.2/src/ghastoolkit/codeql/dataextensions/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/codeql/dataextensions/ext.py` & `ghastoolkit-0.5.2/src/ghastoolkit/codeql/dataextensions/ext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/codeql/dataextensions/models.py` & `ghastoolkit-0.5.2/src/ghastoolkit/codeql/dataextensions/models.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/codeql/packs/pack.py` & `ghastoolkit-0.5.2/src/ghastoolkit/codeql/packs/pack.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/codeql/packs/packs.py` & `ghastoolkit-0.5.2/src/ghastoolkit/codeql/packs/packs.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/codeql/results.py` & `ghastoolkit-0.5.2/src/ghastoolkit/codeql/results.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/octokit/clearlydefined.py` & `ghastoolkit-0.5.2/src/ghastoolkit/octokit/clearlydefined.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.5.2/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.5.2/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.5.2/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.5.2/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/octokit/graphql/__init__.py` & `ghastoolkit-0.5.2/src/ghastoolkit/octokit/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.5.2/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.5.2/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.5.2/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/supplychain/advisories.py` & `ghastoolkit-0.5.2/src/ghastoolkit/supplychain/advisories.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 
 from semantic_version import SimpleSpec, Version
 
 from ghastoolkit.octokit.octokit import OctoItem
 
 
 def parseVersion(data: str) -> str:
+    """Parse Version to help semantic_version process the version."""
     stack = data.split(".")
     if len(stack) == 1:
         return f"{data}.0.0"
     elif len(stack) == 2:
         return f"{data}.0"
     return data
 
 
 @dataclass
 class AdvisoryAffect:
-    """Advisory Affected"""
+    """Advisory Affected."""
 
     ecosystem: str
     """Ecosystem / Dependency Manager / PURL type"""
     package: str
     """Package Full Name ([namespace +] name"""
 
     introduced: Optional[str] = None
@@ -41,24 +42,24 @@
         # HACK can we do this a better way?
         if self.ecosystem in ["maven", "nuget"]:
             namespace, name = self.package.rsplit(".", 1)
         else:
             namespace = None
             name = self.package
 
-        self.package_dependency = Dependency(name, namespace, manager="maven")
+        self.package_dependency = Dependency(name, namespace, manager=self.ecosystem)
 
         if self.introduced:
             self.introduced = parseVersion(self.introduced)
         if self.fixed:
             self.fixed = parseVersion(self.fixed)
 
     @staticmethod
     def loadAffect(data: dict) -> "AdvisoryAffect":
-        """Load affects from data
+        """Load affects from data.
 
         https://github.com/github/advisory-database
         """
         # get introduced and fixed versions
         events = data.get("ranges", [{}])[0].get("events", [])
         introduced = None
         fixed = None
@@ -73,15 +74,15 @@
             data.get("package", {}).get("name", "NA"),
             introduced=introduced,
             fixed=fixed,
         )
         return adaff
 
     def check(self, dependency: "Dependency") -> bool:
-        """Check if version is in range"""
+        """Check to see in the dependency is affected by the advisory."""
 
         from ghastoolkit import Dependency
 
         if not isinstance(dependency, Dependency):
             raise Exception(f"Unknown type provided :: {type(dependency)}")
         # None checks
         if not self.package_dependency or not dependency.version:
@@ -91,25 +92,25 @@
             return False
         # name
         if dependency.name != self.package_dependency.name:
             return False
         return self.checkVersion(dependency.version)
 
     def checkVersion(self, version: str) -> bool:
-        """Check version data with"""
+        """Check version data."""
         if not self.introduced or not self.fixed:
             return False
         # print(f"- {self.introduced} > {parseVersion(version)} < {self.fixed}")
         spec = SimpleSpec(f">={self.introduced},<{self.fixed}")
         return Version(parseVersion(version)) in spec
 
 
 @dataclass
 class Advisory(OctoItem):
-    """GitHub Advisory"""
+    """GitHub Advisory."""
 
     ghsa_id: str
     """GitHub Security Advisory Identifier"""
     severity: str
     """Severity level"""
 
     aliases: List[str] = field(default_factory=list)
@@ -124,27 +125,27 @@
     """List of CWEs"""
 
     affected: List[AdvisoryAffect] = field(default_factory=list)
     """Affected versions"""
 
     @staticmethod
     def load(path: str) -> "Advisory":
-        """Load Advisory from path using GitHub Advisory Spec"""
+        """Load Advisory from path using GitHub Advisory Spec."""
         if not os.path.exists(path):
             raise Exception(f"Advisory path does not exist")
 
         _, ext = os.path.splitext(path)
         if ext == ".json":
             return Advisory.loadJson(path)
 
         raise Exception("Unsupported Advisory file type")
 
     @staticmethod
     def loadJson(path: str) -> "Advisory":
-        """Load Advisory from JSON file"""
+        """Load Advisory from JSON file."""
         with open(path, "r") as handle:
             data = json.load(handle)
 
         affected = []
         for affect in data.get("affected", []):
             affected.append(AdvisoryAffect.loadAffect(affect))
 
@@ -154,65 +155,69 @@
             aliases=data.get("aliases", []),
             summary=data.get("summary"),
             affected=affected,
         )
         return advisory
 
     def check(self, dependency: "Dependency") -> Optional["Advisory"]:
-        """Check if dependency is affected by advisory"""
+        """Check if dependency is affected by advisory."""
         for affect in self.affected:
             if affect.check(dependency):
                 return self
         return
 
 
 class Advisories:
+    """GitHub Advisory List."""
+
     def __init__(self) -> None:
+        """Initialise Advisories."""
         self.advisories: List[Advisory] = []
 
     def loadAdvisories(self, path: str):
-        """Load a single file or folder of advisories"""
+        """Load a single file or folder of advisories."""
         if not os.path.exists(path):
             raise Exception("Advisories path does not exist")
         if os.path.isdir(path):
             for root, dirs, files in os.walk(path):
                 for file in files:
                     _, ext = os.path.splitext(file)
                     if ext in [".json"]:
                         fpath = os.path.join(root, file)
                         self.loadAdvisory(fpath)
         else:
             self.loadAdvisory(path)
 
     def loadAdvisory(self, path: str):
-        """Load file with an advisory"""
+        """Load file with an advisory."""
         if not os.path.exists(path):
             raise Exception(f"Path does not exist")
         self.advisories.append(Advisory.load(path))
 
     def find(self, search: str) -> Optional[Advisory]:
-        """Find by id or aliases"""
+        """Find by id or aliases."""
         for advisory in self.advisories:
             if advisory.ghsa_id == search:
                 return advisory
             if search in advisory.aliases:
                 return advisory
         return
 
     def check(self, dependency: "Dependency") -> List[Advisory]:
-        """Check if dependency is affected by any advisory"""
+        """Check if dependency is affected by any advisory in the list of advisories."""
         results = []
         for a in self.advisories:
             result = a.check(dependency)
             if result:
                 results.append(result)
 
         return results
 
     def append(self, advisory: Advisory):
-        """Append advisory"""
+        """Append advisory."""
         if not isinstance(advisory, Advisory):
             raise Exception(f"Non-Advisory type tring to be appended")
         self.advisories.append(advisory)
 
     def __len__(self) -> int:
+        """To String."""
         return len(self.advisories)
```

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.5.2/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.5.2/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.5.2/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.5.2/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.5.1
+Version: 0.5.2
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.5.1/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.5.2/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/tests/test_advisories.py` & `ghastoolkit-0.5.2/tests/test_dependencies.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,69 @@
 
 import unittest
-from semantic_version import Version
-from ghastoolkit.supplychain.advisories import Advisory, Advisories, AdvisoryAffect, parseVersion
-from ghastoolkit.supplychain.dependencies import Dependency
 
+from ghastoolkit import Dependencies, Dependency, Licenses
 
-class TestAdvisories(unittest.TestCase):
+
+class TestDependencies(unittest.TestCase):
     def setUp(self) -> None:
-        self.advisories = Advisories()
+        self.deps = Dependencies()
+        self.deps.append(Dependency("urllib3", manager="pypi", license="MIT"))
+        self.deps.append(Dependency("rich", manager="pypi", license="NOASSERTION"))
+        self.deps.append(Dependency("pyyaml", manager="pypi", license="GPL-3.0"))
+        self.deps.append(Dependency("pyproject-hooks", manager="pypi", license="Apache-2.0"))
+        self.deps.append(Dependency("requests", manager="pypi", license="GPL-2.0"))
         return super().setUp()
 
-    def test_advisories(self):
-        ad = Advisory("rand", "high")
-        self.advisories.append(ad)
-        self.assertEquals(len(self.advisories), 1)
-
-    def test_advisory_check(self):
-        affected = [AdvisoryAffect("maven", "com.geekmasher.ghastoolkit", introduced="0", fixed="1")]
-        ad = Advisory("rand", "high", affected=affected)
-        self.advisories.append(ad)
-        self.assertEquals(len(self.advisories), 1)
-
-        dep = Dependency("ghastoolkit", "com.geekmasher", "0.8", "maven")
+    def test_license(self):
+        mit = self.deps.findLicenses(["MIT"])
+        self.assertEqual(len(mit), 1)
+        self.assertEqual(mit[0].name, "urllib3")
+
+        gpl = self.deps.findLicenses(["GPL-3.0", "GPL-2.0"])
+        self.assertEqual(len(gpl), 2)
+        self.assertEqual(gpl[0].name, "pyyaml")
+        self.assertEqual(gpl[1].name, "requests")
+
+    def test_license_wildcard(self):
+        gpl = self.deps.findLicenses(["GPL-*"])
+        self.assertEqual(len(gpl), 2)
+        self.assertEqual(gpl[0].name, "pyyaml")
+        self.assertEqual(gpl[1].name, "requests")
+
+    def test_findName(self):
+        pys = self.deps.findNames(["py*"])
+        self.assertEqual(len(pys), 2)
+        self.assertEqual(pys[0].name, "pyyaml")
+        self.assertEqual(pys[1].name, "pyproject-hooks")
+
+    def test_find(self):
+        dep = self.deps.find("pyyaml")
+        self.assertIsNotNone(dep)
+        assert dep is not None
+        self.assertEqual(dep.name, "pyyaml")
+
+    def test_apply_license(self):
+        deps = self.deps.findUnknownLicenses()
+        self.assertEqual(len(deps), 1)
 
-        alert = self.advisories.check(dep)
-        self.assertEquals(alert, [ad])
+        licenses = Licenses()
+        licenses.add("pkg:pypi/rich", ["MIT"])
 
-
-    def test_affect_check(self):
-        dep = Dependency("ghastoolkit", "com.geekmasher", "0.8", "maven")
-        affect = AdvisoryAffect("maven", "com.geekmasher.ghastoolkit", introduced="0", fixed="1")
-
-        self.assertTrue(affect.check(dep))
+        self.deps.applyLicenses(licenses)
         
+        deps = self.deps.findUnknownLicenses()
+        self.assertEqual(len(deps), 0)
+
+        dep = self.deps.find("rich")
+        self.assertEqual(dep.name, "rich")
+        self.assertEqual(dep.license, "MIT")
 
-    def test_affect_check_version(self):
-        affect = AdvisoryAffect("", "", introduced="0.2", fixed="1")
+    def test_update_dep(self):
+        dep = Dependency("urllib3", manager="pypi", license="Apache-2")
 
-        # too early
-        self.assertFalse(affect.checkVersion("0.1"))
-        self.assertFalse(affect.checkVersion("0.1.1"))
-        # inside range
-        self.assertTrue(affect.checkVersion("0.2"))
-        self.assertTrue(affect.checkVersion("0.4.2"))
-        self.assertTrue(affect.checkVersion("0.1111"))
-
-        # fixed
-        self.assertFalse(affect.checkVersion("1"))
-        # later versions
-        self.assertFalse(affect.checkVersion("1.1"))
-        self.assertFalse(affect.checkVersion("10"))
-
-    def test_parse_version(self):
-        self.assertEqual(parseVersion("1"), "1.0.0")
-        self.assertEqual(parseVersion("1.0"), "1.0.0")
-        self.assertEqual(parseVersion("1.1.1"), "1.1.1")
-
-    def test_affect_versions(self):
-        affect = AdvisoryAffect("", "", introduced="0.2", fixed="1")
-        self.assertEqual(affect.introduced, "0.2.0")
-        self.assertEqual(affect.fixed, "1.0.0")
+        self.deps.updateDependency(dep)
 
+        urllib_dep = self.deps.find("urllib3")
+        self.assertEqual(urllib_dep.name, "urllib3")
+        self.assertEqual(urllib_dep.license, "Apache-2")
```

### Comparing `ghastoolkit-0.5.1/tests/test_codeql_dataext.py` & `ghastoolkit-0.5.2/tests/test_codeql_dataext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/tests/test_codeqldb.py` & `ghastoolkit-0.5.2/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/tests/test_codescanning.py` & `ghastoolkit-0.5.2/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/tests/test_default.py` & `ghastoolkit-0.5.2/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/tests/test_depgraph.py` & `ghastoolkit-0.5.2/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/tests/test_github.py` & `ghastoolkit-0.5.2/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/tests/test_licenses.py` & `ghastoolkit-0.5.2/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/tests/test_octokit.py` & `ghastoolkit-0.5.2/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.1/tests/test_secretscanning.py` & `ghastoolkit-0.5.2/tests/test_secretscanning.py`

 * *Files identical despite different names*

