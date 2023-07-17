# Comparing `tmp/scrunch-1689621267.tar.gz` & `tmp/scrunch-1689622832.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scrunch-1689621267.tar", last modified: Mon Jul 17 19:16:03 2023, max compression
+gzip compressed data, was "dist/scrunch-1689622832.tar", last modified: Mon Jul 17 19:42:09 2023, max compression
```

## Comparing `scrunch-1689621267.tar` & `scrunch-1689622832.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:16:03.000000 scrunch-1689621267/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-17 19:15:55.000000 scrunch-1689621267/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-17 19:15:55.000000 scrunch-1689621267/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:16:03.000000 scrunch-1689621267/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:16:03.000000 scrunch-1689621267/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-17 19:15:55.000000 scrunch-1689621267/.github/workflows/test-and-deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-17 19:15:55.000000 scrunch-1689621267/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 19:15:55.000000 scrunch-1689621267/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 19:15:55.000000 scrunch-1689621267/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-17 19:15:55.000000 scrunch-1689621267/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-17 19:15:55.000000 scrunch-1689621267/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-17 19:15:55.000000 scrunch-1689621267/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-17 19:16:03.000000 scrunch-1689621267/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-17 19:15:55.000000 scrunch-1689621267/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-17 19:15:55.000000 scrunch-1689621267/appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 19:15:55.000000 scrunch-1689621267/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:16:03.000000 scrunch-1689621267/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-17 19:15:55.000000 scrunch-1689621267/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-17 19:15:55.000000 scrunch-1689621267/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-17 19:15:55.000000 scrunch-1689621267/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:16:03.000000 scrunch-1689621267/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-17 19:15:55.000000 scrunch-1689621267/integration/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-17 19:15:55.000000 scrunch-1689621267/integration/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-17 19:15:55.000000 scrunch-1689621267/integration/test_backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-17 19:15:55.000000 scrunch-1689621267/integration/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12172 2023-07-17 19:15:55.000000 scrunch-1689621267/integration/test_folders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-17 19:15:55.000000 scrunch-1689621267/integration/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-07-17 19:15:55.000000 scrunch-1689621267/integration/test_recodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-17 19:15:55.000000 scrunch-1689621267/integration/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-17 19:15:55.000000 scrunch-1689621267/integration/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-17 19:15:55.000000 scrunch-1689621267/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-17 19:15:55.000000 scrunch-1689621267/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:16:03.000000 scrunch-1689621267/scrunch/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/crunchboxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/cubes.py
--rw-r--r--   0 runner    (1001) docker     (123)   126327 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29072 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/folders.py
--rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13466 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/mutable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18334 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/streaming_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/subentity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:16:03.000000 scrunch-1689621267/scrunch/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/tests/crunch_test.ini
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/tests/crunch_test_api_key.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:16:03.000000 scrunch-1689621267/scrunch/tests/integration/
--rwxr-xr-x   0 runner    (1001) docker     (123)    38590 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/tests/integration/scrunch_workflow_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/tests/mock_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/tests/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/tests/test_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/tests/test_cubes.py
--rw-r--r--   0 runner    (1001) docker     (123)   283761 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)   100713 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/tests/test_folders.py
--rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/tests/test_recodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/tests/test_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-17 19:15:55.000000 scrunch-1689621267/scrunch/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:16:03.000000 scrunch-1689621267/scrunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-17 19:16:03.000000 scrunch-1689621267/scrunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-17 19:16:03.000000 scrunch-1689621267/scrunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:16:03.000000 scrunch-1689621267/scrunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:16:03.000000 scrunch-1689621267/scrunch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-17 19:16:03.000000 scrunch-1689621267/scrunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 19:16:03.000000 scrunch-1689621267/scrunch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 19:16:03.000000 scrunch-1689621267/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-17 19:15:55.000000 scrunch-1689621267/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-17 19:15:55.000000 scrunch-1689621267/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:42:09.000000 scrunch-1689622832/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-17 19:42:01.000000 scrunch-1689622832/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-17 19:42:01.000000 scrunch-1689622832/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:42:09.000000 scrunch-1689622832/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:42:09.000000 scrunch-1689622832/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-17 19:42:01.000000 scrunch-1689622832/.github/workflows/test-and-deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-17 19:42:01.000000 scrunch-1689622832/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 19:42:01.000000 scrunch-1689622832/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 19:42:01.000000 scrunch-1689622832/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-17 19:42:01.000000 scrunch-1689622832/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-17 19:42:01.000000 scrunch-1689622832/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-17 19:42:01.000000 scrunch-1689622832/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-17 19:42:09.000000 scrunch-1689622832/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-17 19:42:01.000000 scrunch-1689622832/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-17 19:42:01.000000 scrunch-1689622832/appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 19:42:01.000000 scrunch-1689622832/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:42:09.000000 scrunch-1689622832/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-17 19:42:01.000000 scrunch-1689622832/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-17 19:42:01.000000 scrunch-1689622832/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-17 19:42:01.000000 scrunch-1689622832/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:42:09.000000 scrunch-1689622832/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-17 19:42:01.000000 scrunch-1689622832/integration/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-17 19:42:01.000000 scrunch-1689622832/integration/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-17 19:42:01.000000 scrunch-1689622832/integration/test_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-17 19:42:01.000000 scrunch-1689622832/integration/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12172 2023-07-17 19:42:01.000000 scrunch-1689622832/integration/test_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-17 19:42:01.000000 scrunch-1689622832/integration/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-07-17 19:42:01.000000 scrunch-1689622832/integration/test_recodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-17 19:42:01.000000 scrunch-1689622832/integration/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-17 19:42:01.000000 scrunch-1689622832/integration/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-17 19:42:01.000000 scrunch-1689622832/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-17 19:42:01.000000 scrunch-1689622832/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:42:09.000000 scrunch-1689622832/scrunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/crunchboxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/cubes.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126327 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29072 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13466 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/mutable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18334 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/streaming_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/subentity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:42:09.000000 scrunch-1689622832/scrunch/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/tests/crunch_test.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/tests/crunch_test_api_key.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:42:09.000000 scrunch-1689622832/scrunch/tests/integration/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38590 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/tests/integration/scrunch_workflow_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/tests/mock_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/tests/test_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/tests/test_cubes.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283761 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100713 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/tests/test_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/tests/test_recodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/tests/test_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-17 19:42:01.000000 scrunch-1689622832/scrunch/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:42:09.000000 scrunch-1689622832/scrunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-17 19:42:09.000000 scrunch-1689622832/scrunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-17 19:42:09.000000 scrunch-1689622832/scrunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:42:09.000000 scrunch-1689622832/scrunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:42:09.000000 scrunch-1689622832/scrunch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-17 19:42:09.000000 scrunch-1689622832/scrunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 19:42:09.000000 scrunch-1689622832/scrunch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 19:42:09.000000 scrunch-1689622832/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-17 19:42:01.000000 scrunch-1689622832/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-17 19:42:01.000000 scrunch-1689622832/tox.ini
```

### Comparing `scrunch-1689621267/.github/workflows/test-and-deploy.yaml` & `scrunch-1689622832/.github/workflows/test-and-deploy.yaml`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/.gitignore` & `scrunch-1689622832/.gitignore`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/COPYING` & `scrunch-1689622832/COPYING`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/COPYING.LESSER` & `scrunch-1689622832/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/LICENSE` & `scrunch-1689622832/LICENSE`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/PKG-INFO` & `scrunch-1689622832/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrunch
-Version: 1689621267
+Version: 1689622832
 Summary: Pythonic scripting library for cleaning data in Crunch
 Home-page: https://github.com/Crunch-io/scrunch
 Author: Crunch.io
 Author-email: dev@crunch.io
 License: UNKNOWN
 Description: .. image:: https://img.shields.io/pypi/v/scrunch.svg
            :target: https://pypi.org/project/scrunch
```

### Comparing `scrunch-1689621267/README.rst` & `scrunch-1689622832/README.rst`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/docs/conf.py` & `scrunch-1689622832/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/integration/fixtures.py` & `scrunch-1689622832/integration/fixtures.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/integration/test_accounts.py` & `scrunch-1689622832/integration/test_accounts.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/integration/test_backfill.py` & `scrunch-1689622832/integration/test_backfill.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/integration/test_dataset.py` & `scrunch-1689622832/integration/test_dataset.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/integration/test_folders.py` & `scrunch-1689622832/integration/test_folders.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/integration/test_projects.py` & `scrunch-1689622832/integration/test_projects.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/integration/test_recodes.py` & `scrunch-1689622832/integration/test_recodes.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/integration/test_scripts.py` & `scrunch-1689622832/integration/test_scripts.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/integration/test_views.py` & `scrunch-1689622832/integration/test_views.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/accounts.py` & `scrunch-1689622832/scrunch/accounts.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/categories.py` & `scrunch-1689622832/scrunch/categories.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/connections.py` & `scrunch-1689622832/scrunch/connections.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/crunchboxes.py` & `scrunch-1689622832/scrunch/crunchboxes.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/cubes.py` & `scrunch-1689622832/scrunch/cubes.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/datasets.py` & `scrunch-1689622832/scrunch/datasets.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/expressions.py` & `scrunch-1689622832/scrunch/expressions.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/folders.py` & `scrunch-1689622832/scrunch/folders.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/helpers.py` & `scrunch-1689622832/scrunch/helpers.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/mutable_dataset.py` & `scrunch-1689622832/scrunch/mutable_dataset.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/order.py` & `scrunch-1689622832/scrunch/order.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/scripts.py` & `scrunch-1689622832/scrunch/scripts.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/session.py` & `scrunch-1689622832/scrunch/session.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/streaming_dataset.py` & `scrunch-1689622832/scrunch/streaming_dataset.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/subentity.py` & `scrunch-1689622832/scrunch/subentity.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/tests/integration/scrunch_workflow_integration_test.py` & `scrunch-1689622832/scrunch/tests/integration/scrunch_workflow_integration_test.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/tests/mock_session.py` & `scrunch-1689622832/scrunch/tests/mock_session.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/tests/test_accounts.py` & `scrunch-1689622832/scrunch/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/tests/test_categories.py` & `scrunch-1689622832/scrunch/tests/test_categories.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/tests/test_cubes.py` & `scrunch-1689622832/scrunch/tests/test_cubes.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/tests/test_datasets.py` & `scrunch-1689622832/scrunch/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/tests/test_expressions.py` & `scrunch-1689622832/scrunch/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/tests/test_folders.py` & `scrunch-1689622832/scrunch/tests/test_folders.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/tests/test_projects.py` & `scrunch-1689622832/scrunch/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/tests/test_recodes.py` & `scrunch-1689622832/scrunch/tests/test_recodes.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/tests/test_scripts.py` & `scrunch-1689622832/scrunch/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/tests/test_teams.py` & `scrunch-1689622832/scrunch/tests/test_teams.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/tests/test_utilities.py` & `scrunch-1689622832/scrunch/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/tests/test_views.py` & `scrunch-1689622832/scrunch/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/variables.py` & `scrunch-1689622832/scrunch/variables.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch/views.py` & `scrunch-1689622832/scrunch/views.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/scrunch.egg-info/PKG-INFO` & `scrunch-1689622832/scrunch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrunch
-Version: 1689621267
+Version: 1689622832
 Summary: Pythonic scripting library for cleaning data in Crunch
 Home-page: https://github.com/Crunch-io/scrunch
 Author: Crunch.io
 Author-email: dev@crunch.io
 License: UNKNOWN
 Description: .. image:: https://img.shields.io/pypi/v/scrunch.svg
            :target: https://pypi.org/project/scrunch
```

### Comparing `scrunch-1689621267/scrunch.egg-info/SOURCES.txt` & `scrunch-1689622832/scrunch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/setup.py` & `scrunch-1689622832/setup.py`

 * *Files identical despite different names*

### Comparing `scrunch-1689621267/tox.ini` & `scrunch-1689622832/tox.ini`

 * *Files identical despite different names*

