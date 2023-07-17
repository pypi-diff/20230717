# Comparing `tmp/ghastoolkit-0.5.2.tar.gz` & `tmp/ghastoolkit-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.5.2.tar", last modified: Mon Jul 17 12:02:40 2023, max compression
+gzip compressed data, was "ghastoolkit-0.5.3.tar", last modified: Mon Jul 17 14:30:31 2023, max compression
```

## Comparing `ghastoolkit-0.5.2.tar` & `ghastoolkit-0.5.3.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.337580 ghastoolkit-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-17 12:02:40.337580 ghastoolkit-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 12:02:40.337580 ghastoolkit-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.329580 ghastoolkit-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.329580 ghastoolkit-0.5.2/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.333580 ghastoolkit-0.5.2/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.333580 ghastoolkit-0.5.2/src/ghastoolkit/codeql/dataextensions/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/dataextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/dataextensions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/dataextensions/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/dataextensions/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.333580 ghastoolkit-0.5.2/src/ghastoolkit/codeql/packs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/packs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/packs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/packs/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/packs/packs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/codeql/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.333580 ghastoolkit-0.5.2/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.333580 ghastoolkit-0.5.2/src/ghastoolkit/octokit/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.333580 ghastoolkit-0.5.2/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.333580 ghastoolkit-0.5.2/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.333580 ghastoolkit-0.5.2/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-17 12:02:40.000000 ghastoolkit-0.5.2/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-17 12:02:40.000000 ghastoolkit-0.5.2/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:02:40.000000 ghastoolkit-0.5.2/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-17 12:02:40.000000 ghastoolkit-0.5.2/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 12:02:40.000000 ghastoolkit-0.5.2/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:02:40.337580 ghastoolkit-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_codeql_dataext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-17 12:02:11.000000 ghastoolkit-0.5.2/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.325154 ghastoolkit-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-17 14:30:31.325154 ghastoolkit-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:30:31.325154 ghastoolkit-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.317153 ghastoolkit-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.321153 ghastoolkit-0.5.3/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.321153 ghastoolkit-0.5.3/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.321153 ghastoolkit-0.5.3/src/ghastoolkit/codeql/dataextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/dataextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/dataextensions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/dataextensions/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/dataextensions/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.321153 ghastoolkit-0.5.3/src/ghastoolkit/codeql/packs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/packs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/packs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/packs/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/packs/packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.325154 ghastoolkit-0.5.3/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.325154 ghastoolkit-0.5.3/src/ghastoolkit/octokit/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.325154 ghastoolkit-0.5.3/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.325154 ghastoolkit-0.5.3/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.321153 ghastoolkit-0.5.3/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-17 14:30:31.000000 ghastoolkit-0.5.3/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-17 14:30:31.000000 ghastoolkit-0.5.3/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:30:31.000000 ghastoolkit-0.5.3/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-17 14:30:31.000000 ghastoolkit-0.5.3/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 14:30:31.000000 ghastoolkit-0.5.3/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.325154 ghastoolkit-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_codeql_dataext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.5.2/LICENSE` & `ghastoolkit-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/PKG-INFO` & `ghastoolkit-0.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.5.2
+Version: 0.5.3
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.5.2/README.md` & `ghastoolkit-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/pyproject.toml` & `ghastoolkit-0.5.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.5.2"
+version = "0.5.3"
 authors = [{ name = "GeekMasher" }]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/__init__.py` & `ghastoolkit-0.5.3/src/ghastoolkit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.5.2"
+__version__ = "0.5.3"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
@@ -27,14 +27,16 @@
 
 # Octokit
 from ghastoolkit.octokit.github import GitHub, Repository
 from ghastoolkit.octokit.octokit import Octokit, RestRequest, GraphQLRequest
 from ghastoolkit.octokit.codescanning import CodeScanning, CodeAlert
 from ghastoolkit.octokit.secretscanning import SecretScanning, SecretAlert
 from ghastoolkit.octokit.dependencygraph import DependencyGraph
+from ghastoolkit.octokit.dependabot import Dependabot
+from ghastoolkit.octokit.advisories import SecurityAdvisories
 
 # Supply Chain
 from ghastoolkit.supplychain.advisories import Advisory, Advisories
 from ghastoolkit.supplychain.dependencyalert import DependencyAlert
 from ghastoolkit.supplychain.dependencies import Dependency, Dependencies
 from ghastoolkit.supplychain.licensing import Licenses
```

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/__main__.py` & `ghastoolkit-0.5.3/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/codeql/cli.py` & `ghastoolkit-0.5.3/src/ghastoolkit/codeql/cli.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.5.3/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/codeql/dataextensions/__main__.py` & `ghastoolkit-0.5.3/src/ghastoolkit/codeql/dataextensions/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/codeql/dataextensions/ext.py` & `ghastoolkit-0.5.3/src/ghastoolkit/codeql/dataextensions/ext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/codeql/dataextensions/models.py` & `ghastoolkit-0.5.3/src/ghastoolkit/codeql/dataextensions/models.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/codeql/packs/pack.py` & `ghastoolkit-0.5.3/src/ghastoolkit/codeql/packs/pack.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/codeql/packs/packs.py` & `ghastoolkit-0.5.3/src/ghastoolkit/codeql/packs/packs.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/codeql/results.py` & `ghastoolkit-0.5.3/src/ghastoolkit/codeql/results.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/octokit/clearlydefined.py` & `ghastoolkit-0.5.3/src/ghastoolkit/octokit/clearlydefined.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.5.3/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.5.3/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.5.3/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.5.3/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/octokit/graphql/__init__.py` & `ghastoolkit-0.5.3/src/ghastoolkit/octokit/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.5.3/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.5.3/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.5.3/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/supplychain/advisories.py` & `ghastoolkit-0.5.3/src/ghastoolkit/supplychain/advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.5.3/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.5.3/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.5.3/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.5.3/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.5.2
+Version: 0.5.3
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.5.2/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.5.3/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 src/ghastoolkit/codeql/dataextensions/ext.py
 src/ghastoolkit/codeql/dataextensions/models.py
 src/ghastoolkit/codeql/packs/__init__.py
 src/ghastoolkit/codeql/packs/__main__.py
 src/ghastoolkit/codeql/packs/pack.py
 src/ghastoolkit/codeql/packs/packs.py
 src/ghastoolkit/octokit/__init__.py
+src/ghastoolkit/octokit/advisories.py
 src/ghastoolkit/octokit/clearlydefined.py
 src/ghastoolkit/octokit/codescanning.py
 src/ghastoolkit/octokit/dependabot.py
 src/ghastoolkit/octokit/dependencygraph.py
 src/ghastoolkit/octokit/github.py
 src/ghastoolkit/octokit/octokit.py
 src/ghastoolkit/octokit/secretscanning.py
```

### Comparing `ghastoolkit-0.5.2/tests/test_advisories.py` & `ghastoolkit-0.5.3/tests/test_advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/tests/test_codeql_dataext.py` & `ghastoolkit-0.5.3/tests/test_codeql_dataext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/tests/test_codeqldb.py` & `ghastoolkit-0.5.3/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/tests/test_codescanning.py` & `ghastoolkit-0.5.3/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/tests/test_default.py` & `ghastoolkit-0.5.3/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/tests/test_dependencies.py` & `ghastoolkit-0.5.3/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/tests/test_depgraph.py` & `ghastoolkit-0.5.3/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/tests/test_github.py` & `ghastoolkit-0.5.3/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/tests/test_licenses.py` & `ghastoolkit-0.5.3/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/tests/test_octokit.py` & `ghastoolkit-0.5.3/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.2/tests/test_secretscanning.py` & `ghastoolkit-0.5.3/tests/test_secretscanning.py`

 * *Files identical despite different names*

