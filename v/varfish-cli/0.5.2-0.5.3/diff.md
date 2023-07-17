# Comparing `tmp/varfish_cli-0.5.2.tar.gz` & `tmp/varfish_cli-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varfish_cli-0.5.2.tar", last modified: Mon Jun 12 16:26:03 2023, max compression
+gzip compressed data, was "varfish_cli-0.5.3.tar", last modified: Mon Jul 17 11:38:08 2023, max compression
```

## Comparing `varfish_cli-0.5.2.tar` & `varfish_cli-0.5.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.538033 varfish_cli-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-12 16:26:03.538033 varfish_cli-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.530033 varfish_cli-0.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/docs/cli_docs.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     5264 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.530033 varfish_cli-0.5.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/requirements/develop.txt
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/requirements/test_black.txt
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-12 16:26:03.538033 varfish_cli-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.534033 varfish_cli-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.530033 varfish_cli-0.5.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.534033 varfish_cli-0.5.2/tests/data/config/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/tests/data/config/varfishrc.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.534033 varfish_cli-0.5.2/tests/data/parse_ped/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/tests/data/parse_ped/trio.ped
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/tests/test_parse_ped.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/tests/test_run_case_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.538033 varfish_cli-0.5.2/varfish_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-12 16:26:03.538033 varfish_cli-0.5.2/varfish_cli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.534033 varfish_cli-0.5.2/varfish_cli/api/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39072 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/api/case.py
--rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/api/varannos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.534033 varfish_cli-0.5.2/varfish_cli/case/
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    36213 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/create_case_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/list_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/list_case_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/small_var_query_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/small_var_query_fetch_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/small_var_query_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/small_var_query_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/small_var_query_settings_shortcut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/small_var_query_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/small_var_query_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/parse_ped.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.538033 varfish_cli-0.5.2/varfish_cli/varannos/
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/varannoset_destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/varannoset_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/varannoset_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/varannoset_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/varannosetentry_destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/varannosetentry_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/varannosetentry_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/varannosetentry_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.534033 varfish_cli-0.5.2/varfish_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-12 16:26:03.000000 varfish_cli-0.5.2/varfish_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-12 16:26:03.000000 varfish_cli-0.5.2/varfish_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:26:03.000000 varfish_cli-0.5.2/varfish_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-12 16:26:03.000000 varfish_cli-0.5.2/varfish_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:26:03.000000 varfish_cli-0.5.2/varfish_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-12 16:26:03.000000 varfish_cli-0.5.2/varfish_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 16:26:03.000000 varfish_cli-0.5.2/varfish_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    68448 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:38:08.446080 varfish_cli-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-17 11:38:08.446080 varfish_cli-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:38:08.442080 varfish_cli-0.5.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/docs/cli_docs.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5264 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:38:08.442080 varfish_cli-0.5.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/requirements/develop.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/requirements/test_black.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-17 11:38:08.446080 varfish_cli-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:38:08.442080 varfish_cli-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:38:08.438080 varfish_cli-0.5.3/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:38:08.442080 varfish_cli-0.5.3/tests/data/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/tests/data/config/varfishrc.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:38:08.442080 varfish_cli-0.5.3/tests/data/parse_ped/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/tests/data/parse_ped/trio.ped
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/tests/test_parse_ped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/tests/test_run_case_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:38:08.446080 varfish_cli-0.5.3/varfish_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-17 11:38:08.446080 varfish_cli-0.5.3/varfish_cli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:38:08.442080 varfish_cli-0.5.3/varfish_cli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39072 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/api/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/api/varannos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:38:08.442080 varfish_cli-0.5.3/varfish_cli/case/
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/case/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35513 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/case/create_case_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/case/list_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/case/list_case_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/case/small_var_query_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/case/small_var_query_fetch_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/case/small_var_query_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/case/small_var_query_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/case/small_var_query_settings_shortcut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/case/small_var_query_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/case/small_var_query_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/parse_ped.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:38:08.446080 varfish_cli-0.5.3/varfish_cli/varannos/
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/varannos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/varannos/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/varannos/varannoset_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/varannos/varannoset_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/varannos/varannoset_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/varannos/varannoset_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/varannos/varannosetentry_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/varannos/varannosetentry_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/varannos/varannosetentry_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/varfish_cli/varannos/varannosetentry_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:38:08.442080 varfish_cli-0.5.3/varfish_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-17 11:38:08.000000 varfish_cli-0.5.3/varfish_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-17 11:38:08.000000 varfish_cli-0.5.3/varfish_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:38:08.000000 varfish_cli-0.5.3/varfish_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-17 11:38:08.000000 varfish_cli-0.5.3/varfish_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:38:08.000000 varfish_cli-0.5.3/varfish_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-17 11:38:08.000000 varfish_cli-0.5.3/varfish_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 11:38:08.000000 varfish_cli-0.5.3/varfish_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68448 2023-07-17 11:38:04.000000 varfish_cli-0.5.3/versioneer.py
```

### Comparing `varfish_cli-0.5.2/CHANGELOG.md` & `varfish_cli-0.5.3/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,30 @@
 # Changelog
 
+## [0.5.3](https://github.com/bihealth/varfish-cli/compare/v0.5.2...v0.5.3) (2023-07-17)
+
+
+### Features
+
+* force release of 0.6 ([#46](https://github.com/bihealth/varfish-cli/issues/46)) ([f003be8](https://github.com/bihealth/varfish-cli/commit/f003be8b1f953ff4ab22f7d274264747dd39870d))
+
+
+### Bug Fixes
+
+* allow varfish upload without SV effects ([#43](https://github.com/bihealth/varfish-cli/issues/43)) ([4aead65](https://github.com/bihealth/varfish-cli/commit/4aead65054e97adf7564f8fb3d3a3e0db755c34f))
+* fixing issue with logging ([ab62f24](https://github.com/bihealth/varfish-cli/commit/ab62f242445150c2472aa45ea0c0f6d7782a7b8c))
+
+### [0.5.2](https://www.github.com/bihealth/varfish-cli/compare/v0.5.1...v0.5.2) (2023-07-17)
+
+
+### Bug Fixes
+
+* allow varfish upload without SV effects ([#43](https://www.github.com/bihealth/varfish-cli/issues/43)) ([4aead65](https://www.github.com/bihealth/varfish-cli/commit/4aead65054e97adf7564f8fb3d3a3e0db755c34f))
+* Fixing case list API ([#37](https://www.github.com/bihealth/varfish-cli/issues/37)) ([ccaccfc](https://www.github.com/bihealth/varfish-cli/commit/ccaccfcbec7fb209492f1855b5e740f20ac60bbc))
+
 ### [0.5.2](https://www.github.com/bihealth/varfish-cli/compare/v0.5.1...v0.5.2) (2023-06-12)
 
 
 ### Bug Fixes
 
 * Fixing case list API ([#37](https://www.github.com/bihealth/varfish-cli/issues/37)) ([ccaccfc](https://www.github.com/bihealth/varfish-cli/commit/ccaccfcbec7fb209492f1855b5e740f20ac60bbc))
```

### Comparing `varfish_cli-0.5.2/LICENSE` & `varfish_cli-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/PKG-INFO` & `varfish_cli-0.5.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varfish_cli
-Version: 0.5.2
+Version: 0.5.3
 Summary: Command line interface client for VarFish Server.
 Home-page: https://github.com/bihealth/varfish-cli
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bihealth.de
 License: MIT license
 Keywords: varfish_cli
 Classifier: Development Status :: 4 - Beta
@@ -86,14 +86,35 @@
 varfish_api_token = "XXX"
 EOF
 ```
 
 
 # Changelog
 
+## [0.5.3](https://github.com/bihealth/varfish-cli/compare/v0.5.2...v0.5.3) (2023-07-17)
+
+
+### Features
+
+* force release of 0.6 ([#46](https://github.com/bihealth/varfish-cli/issues/46)) ([f003be8](https://github.com/bihealth/varfish-cli/commit/f003be8b1f953ff4ab22f7d274264747dd39870d))
+
+
+### Bug Fixes
+
+* allow varfish upload without SV effects ([#43](https://github.com/bihealth/varfish-cli/issues/43)) ([4aead65](https://github.com/bihealth/varfish-cli/commit/4aead65054e97adf7564f8fb3d3a3e0db755c34f))
+* fixing issue with logging ([ab62f24](https://github.com/bihealth/varfish-cli/commit/ab62f242445150c2472aa45ea0c0f6d7782a7b8c))
+
+### [0.5.2](https://www.github.com/bihealth/varfish-cli/compare/v0.5.1...v0.5.2) (2023-07-17)
+
+
+### Bug Fixes
+
+* allow varfish upload without SV effects ([#43](https://www.github.com/bihealth/varfish-cli/issues/43)) ([4aead65](https://www.github.com/bihealth/varfish-cli/commit/4aead65054e97adf7564f8fb3d3a3e0db755c34f))
+* Fixing case list API ([#37](https://www.github.com/bihealth/varfish-cli/issues/37)) ([ccaccfc](https://www.github.com/bihealth/varfish-cli/commit/ccaccfcbec7fb209492f1855b5e740f20ac60bbc))
+
 ### [0.5.2](https://www.github.com/bihealth/varfish-cli/compare/v0.5.1...v0.5.2) (2023-06-12)
 
 
 ### Bug Fixes
 
 * Fixing case list API ([#37](https://www.github.com/bihealth/varfish-cli/issues/37)) ([ccaccfc](https://www.github.com/bihealth/varfish-cli/commit/ccaccfcbec7fb209492f1855b5e740f20ac60bbc))
```

### Comparing `varfish_cli-0.5.2/README.md` & `varfish_cli-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/docs/Makefile` & `varfish_cli-0.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/docs/conf.py` & `varfish_cli-0.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/docs/make.bat` & `varfish_cli-0.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/requirements/base.txt` & `varfish_cli-0.5.3/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/requirements/test.txt` & `varfish_cli-0.5.3/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/requirements.txt` & `varfish_cli-0.5.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/setup.cfg` & `varfish_cli-0.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/setup.py` & `varfish_cli-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/tests/test_config.py` & `varfish_cli-0.5.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/tests/test_parse_ped.py` & `varfish_cli-0.5.3/tests/test_parse_ped.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/tests/test_run_case_list.py` & `varfish_cli-0.5.3/tests/test_run_case_list.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/__main__.py` & `varfish_cli-0.5.3/varfish_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/api/case.py` & `varfish_cli-0.5.3/varfish_cli/api/case.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/api/models.py` & `varfish_cli-0.5.3/varfish_cli/api/models.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/api/varannos.py` & `varfish_cli-0.5.3/varfish_cli/api/varannos.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/case/__init__.py` & `varfish_cli-0.5.3/varfish_cli/case/__init__.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/case/config.py` & `varfish_cli-0.5.3/varfish_cli/case/config.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/case/create_case_import.py` & `varfish_cli-0.5.3/varfish_cli/case/create_case_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from ..api import (
     BamQcFile,
     CaseGeneAnnotationFile,
     CaseImportInfo,
     CaseImportState,
     CaseVariantType,
     DatabaseInfoFile,
-    EffectsFile,
     GenomeBuild,
     GenotypeFile,
     PedigreeMember,
     VariantSetImportState,
     models,
 )
 
@@ -471,19 +470,16 @@
             "Guessed file types =\n%s",
             tabulate(guessed, headers=["file type", "file name"], tablefmt="grid"),
         )
 
         issues = []
         if not self.path_ped:
             issues.append("no PED file given")
-        if len(self.paths_genotype_sv) != len(self.paths_effect_sv):
-            issues.append(
-                "different number of SV genotypes (%d)/effects (%d)"
-                % (len(self.paths_genotype_sv), len(self.paths_effect_sv))
-            )
+        if len(self.paths_effect_sv):
+            logger.info("Will ignore any SV effect files")
         if not self.paths_genotype and not self.paths_genotype_sv:
             issues.append("neither small nor SVs given")
         if len(self.paths_genotype) > 1:
             logger.warn("More than one small variant genotype file given.")
         if issues:
             raise MissingFileOnImport("Problem(s) with import files: %s" % ", ".join(issues))
 
@@ -784,26 +780,14 @@
                     api_create_func=api.genotype_file_upload,
                 )
                 for path in self.paths_genotype_sv
             ]
             good_md5s += [
                 self._perform_file_upload(
                     path=path.path,
-                    api_list_func=api.effects_file_list,
-                    func_uuid_arg="variant_set_import_info_uuid",
-                    uuid_value=variant_set_import_info.sodar_uuid,
-                    obj_type="effects file",
-                    file_type=EffectsFile,
-                    api_create_func=api.effects_file_upload,
-                )
-                for path in self.paths_effect_sv
-            ]
-            good_md5s += [
-                self._perform_file_upload(
-                    path=path.path,
                     api_list_func=api.db_info_file_list,
                     func_uuid_arg="variant_set_import_info_uuid",
                     uuid_value=variant_set_import_info.sodar_uuid,
                     obj_type="db info file",
                     file_type=DatabaseInfoFile,
                     api_create_func=api.db_info_file_upload,
                 )
```

### Comparing `varfish_cli-0.5.2/varfish_cli/case/list_case.py` & `varfish_cli-0.5.3/varfish_cli/case/list_case.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/case/list_case_import.py` & `varfish_cli-0.5.3/varfish_cli/case/list_case_import.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/case/small_var_query_create.py` & `varfish_cli-0.5.3/varfish_cli/case/small_var_query_create.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/case/small_var_query_fetch_results.py` & `varfish_cli-0.5.3/varfish_cli/case/small_var_query_fetch_results.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/case/small_var_query_list.py` & `varfish_cli-0.5.3/varfish_cli/case/small_var_query_list.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/case/small_var_query_retrieve.py` & `varfish_cli-0.5.3/varfish_cli/case/small_var_query_retrieve.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/case/small_var_query_settings_shortcut.py` & `varfish_cli-0.5.3/varfish_cli/case/small_var_query_settings_shortcut.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/case/small_var_query_status.py` & `varfish_cli-0.5.3/varfish_cli/case/small_var_query_status.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/case/small_var_query_update.py` & `varfish_cli-0.5.3/varfish_cli/case/small_var_query_update.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/common.py` & `varfish_cli-0.5.3/varfish_cli/common.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/exceptions.py` & `varfish_cli-0.5.3/varfish_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/parse_ped.py` & `varfish_cli-0.5.3/varfish_cli/parse_ped.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/varannos/__init__.py` & `varfish_cli-0.5.3/varfish_cli/varannos/__init__.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/varannos/config.py` & `varfish_cli-0.5.3/varfish_cli/varannos/config.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/varannos/varannoset_destroy.py` & `varfish_cli-0.5.3/varfish_cli/varannos/varannoset_destroy.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/varannos/varannoset_list.py` & `varfish_cli-0.5.3/varfish_cli/varannos/varannoset_list.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/varannos/varannoset_retrieve.py` & `varfish_cli-0.5.3/varfish_cli/varannos/varannoset_retrieve.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/varannos/varannoset_update.py` & `varfish_cli-0.5.3/varfish_cli/varannos/varannoset_update.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/varannos/varannosetentry_destroy.py` & `varfish_cli-0.5.3/varfish_cli/varannos/varannosetentry_destroy.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/varannos/varannosetentry_list.py` & `varfish_cli-0.5.3/varfish_cli/varannos/varannosetentry_list.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/varannos/varannosetentry_retrieve.py` & `varfish_cli-0.5.3/varfish_cli/varannos/varannosetentry_retrieve.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli/varannos/varannosetentry_update.py` & `varfish_cli-0.5.3/varfish_cli/varannos/varannosetentry_update.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/varfish_cli.egg-info/PKG-INFO` & `varfish_cli-0.5.3/varfish_cli.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varfish-cli
-Version: 0.5.2
+Version: 0.5.3
 Summary: Command line interface client for VarFish Server.
 Home-page: https://github.com/bihealth/varfish-cli
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bihealth.de
 License: MIT license
 Keywords: varfish_cli
 Classifier: Development Status :: 4 - Beta
@@ -86,14 +86,35 @@
 varfish_api_token = "XXX"
 EOF
 ```
 
 
 # Changelog
 
+## [0.5.3](https://github.com/bihealth/varfish-cli/compare/v0.5.2...v0.5.3) (2023-07-17)
+
+
+### Features
+
+* force release of 0.6 ([#46](https://github.com/bihealth/varfish-cli/issues/46)) ([f003be8](https://github.com/bihealth/varfish-cli/commit/f003be8b1f953ff4ab22f7d274264747dd39870d))
+
+
+### Bug Fixes
+
+* allow varfish upload without SV effects ([#43](https://github.com/bihealth/varfish-cli/issues/43)) ([4aead65](https://github.com/bihealth/varfish-cli/commit/4aead65054e97adf7564f8fb3d3a3e0db755c34f))
+* fixing issue with logging ([ab62f24](https://github.com/bihealth/varfish-cli/commit/ab62f242445150c2472aa45ea0c0f6d7782a7b8c))
+
+### [0.5.2](https://www.github.com/bihealth/varfish-cli/compare/v0.5.1...v0.5.2) (2023-07-17)
+
+
+### Bug Fixes
+
+* allow varfish upload without SV effects ([#43](https://www.github.com/bihealth/varfish-cli/issues/43)) ([4aead65](https://www.github.com/bihealth/varfish-cli/commit/4aead65054e97adf7564f8fb3d3a3e0db755c34f))
+* Fixing case list API ([#37](https://www.github.com/bihealth/varfish-cli/issues/37)) ([ccaccfc](https://www.github.com/bihealth/varfish-cli/commit/ccaccfcbec7fb209492f1855b5e740f20ac60bbc))
+
 ### [0.5.2](https://www.github.com/bihealth/varfish-cli/compare/v0.5.1...v0.5.2) (2023-06-12)
 
 
 ### Bug Fixes
 
 * Fixing case list API ([#37](https://www.github.com/bihealth/varfish-cli/issues/37)) ([ccaccfc](https://www.github.com/bihealth/varfish-cli/commit/ccaccfcbec7fb209492f1855b5e740f20ac60bbc))
```

### Comparing `varfish_cli-0.5.2/varfish_cli.egg-info/SOURCES.txt` & `varfish_cli-0.5.3/varfish_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.2/versioneer.py` & `varfish_cli-0.5.3/versioneer.py`

 * *Files identical despite different names*

