# Comparing `tmp/codecov-cli-0.1.8.tar.gz` & `tmp/codecov-cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codecov-cli-0.1.8.tar", last modified: Wed May 10 07:34:28 2023, max compression
+gzip compressed data, was "codecov-cli-0.1.9.tar", last modified: Mon May 15 13:10:32 2023, max compression
```

## Comparing `codecov-cli-0.1.8.tar` & `codecov-cli-0.1.9.tar`

### file list

```diff
@@ -1,109 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:28.005498 codecov-cli-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-10 07:34:28.005498 codecov-cli-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.993497 codecov-cli-0.1.8/codecov_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.993497 codecov-cli-0.1.8/codecov_cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/base_picking.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/create_report_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/get_report_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/labelanalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/staticanalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/fallbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.993497 codecov-cli-0.1.8/codecov_cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/appveyor_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/azure_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/bitbucket_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/bitrise_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/buildkite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/circleci.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/cirrus_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/codebuild.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/droneci.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/github_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/gitlab_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/heroku.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/jenkins.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/teamcity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/travis_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/woodpeckerci.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/folder_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/versioning_systems.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/plugins/gcov.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/plugins/pycoverage.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/plugins/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/plugins/xcode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/runners/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/runners/dan_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/runners/python_standard_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/runners/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/services/commit/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/commit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/commit/base_picking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/services/report/
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/report/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/ecmascriptsix.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/python/
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/finders.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:28.001498 codecov-cli-0.1.8/codecov_cli/services/upload/
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/upload/coverage_file_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/upload/legacy_upload_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/upload/network_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/upload/upload_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/upload/upload_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.993497 codecov-cli-0.1.8/codecov_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-10 07:34:27.000000 codecov-cli-0.1.8/codecov_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-10 07:34:27.000000 codecov-cli-0.1.8/codecov_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 07:34:27.000000 codecov-cli-0.1.8/codecov_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 07:34:27.000000 codecov-cli-0.1.8/codecov_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 07:34:27.000000 codecov-cli-0.1.8/codecov_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 07:34:27.000000 codecov-cli-0.1.8/codecov_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:28.001498 codecov-cli-0.1.8/languages/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/languages/languages.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.993497 codecov-cli-0.1.8/languages/treesitterjavascript/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:28.001498 codecov-cli-0.1.8/languages/treesitterjavascript/src/
--rw-r--r--   0 runner    (1001) docker     (123)  2277994 2023-05-10 07:34:04.000000 codecov-cli-0.1.8/languages/treesitterjavascript/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-10 07:34:04.000000 codecov-cli-0.1.8/languages/treesitterjavascript/src/scanner.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:28.001498 codecov-cli-0.1.8/languages/treesitterjavascript/src/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-10 07:34:04.000000 codecov-cli-0.1.8/languages/treesitterjavascript/src/tree_sitter/parser.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.993497 codecov-cli-0.1.8/languages/treesitterpython/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:28.005498 codecov-cli-0.1.8/languages/treesitterpython/src/
--rw-r--r--   0 runner    (1001) docker     (123)  2658198 2023-05-10 07:34:05.000000 codecov-cli-0.1.8/languages/treesitterpython/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-05-10 07:34:05.000000 codecov-cli-0.1.8/languages/treesitterpython/src/scanner.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:28.005498 codecov-cli-0.1.8/languages/treesitterpython/src/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-10 07:34:05.000000 codecov-cli-0.1.8/languages/treesitterpython/src/tree_sitter/parser.h
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 07:34:28.005498 codecov-cli-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.289603 codecov-cli-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-15 13:10:32.289603 codecov-cli-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.273602 codecov-cli-0.1.9/codecov_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.277603 codecov-cli-0.1.9/codecov_cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/commands/base_picking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/commands/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/commands/create_report_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/commands/empty_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/commands/get_report_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/commands/labelanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/commands/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/commands/staticanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/commands/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/fallbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.277603 codecov-cli-0.1.9/codecov_cli/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.277603 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/appveyor_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/azure_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/bitbucket_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/bitrise_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/buildkite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/circleci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/cirrus_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/codebuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/droneci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/gitlab_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/heroku.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/teamcity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/travis_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/woodpeckerci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/folder_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/helpers/versioning_systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.277603 codecov-cli-0.1.9/codecov_cli/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/plugins/gcov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/plugins/pycoverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/plugins/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/plugins/xcode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.281603 codecov-cli-0.1.9/codecov_cli/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/runners/dan_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/runners/python_standard_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/runners/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.281603 codecov-cli-0.1.9/codecov_cli/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.281603 codecov-cli-0.1.9/codecov_cli/services/commit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/commit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/commit/base_picking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.281603 codecov-cli-0.1.9/codecov_cli/services/empty_upload/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/empty_upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.281603 codecov-cli-0.1.9/codecov_cli/services/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.281603 codecov-cli-0.1.9/codecov_cli/services/staticanalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/staticanalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.281603 codecov-cli-0.1.9/codecov_cli/services/staticanalysis/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/staticanalysis/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/staticanalysis/analyzers/ecmascriptsix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/staticanalysis/analyzers/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.281603 codecov-cli-0.1.9/codecov_cli/services/staticanalysis/analyzers/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/staticanalysis/analyzers/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/staticanalysis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/staticanalysis/finders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/staticanalysis/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.281603 codecov-cli-0.1.9/codecov_cli/services/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/upload/coverage_file_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/upload/legacy_upload_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/upload/network_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/upload/upload_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/services/upload/upload_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/codecov_cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.273602 codecov-cli-0.1.9/codecov_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-15 13:10:32.000000 codecov-cli-0.1.9/codecov_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-15 13:10:32.000000 codecov-cli-0.1.9/codecov_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:10:32.000000 codecov-cli-0.1.9/codecov_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 13:10:32.000000 codecov-cli-0.1.9/codecov_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 13:10:32.000000 codecov-cli-0.1.9/codecov_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 13:10:32.000000 codecov-cli-0.1.9/codecov_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.281603 codecov-cli-0.1.9/languages/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/languages/languages.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.273602 codecov-cli-0.1.9/languages/treesitterjavascript/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.285603 codecov-cli-0.1.9/languages/treesitterjavascript/src/
+-rw-r--r--   0 runner    (1001) docker     (123)  2277994 2023-05-15 13:10:02.000000 codecov-cli-0.1.9/languages/treesitterjavascript/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-15 13:10:02.000000 codecov-cli-0.1.9/languages/treesitterjavascript/src/scanner.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.285603 codecov-cli-0.1.9/languages/treesitterjavascript/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-15 13:10:02.000000 codecov-cli-0.1.9/languages/treesitterjavascript/src/tree_sitter/parser.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.273602 codecov-cli-0.1.9/languages/treesitterpython/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.289603 codecov-cli-0.1.9/languages/treesitterpython/src/
+-rw-r--r--   0 runner    (1001) docker     (123)  2658198 2023-05-15 13:10:05.000000 codecov-cli-0.1.9/languages/treesitterpython/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-05-15 13:10:05.000000 codecov-cli-0.1.9/languages/treesitterpython/src/scanner.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:10:32.289603 codecov-cli-0.1.9/languages/treesitterpython/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-15 13:10:05.000000 codecov-cli-0.1.9/languages/treesitterpython/src/tree_sitter/parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 13:10:32.289603 codecov-cli-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-15 13:09:59.000000 codecov-cli-0.1.9/setup.py
```

### Comparing `codecov-cli-0.1.8/LICENSE` & `codecov-cli-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/PKG-INFO` & `codecov-cli-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecov-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: Codecov Command Line Interface
 Author: Codecov
 Author-email: support@codecov.io
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CodecovCLI
```

### Comparing `codecov-cli-0.1.8/README.md` & `codecov-cli-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/commands/base_picking.py` & `codecov-cli-0.1.9/codecov_cli/commands/base_picking.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/commands/commit.py` & `codecov-cli-0.1.9/codecov_cli/commands/commit.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/commands/create_report_result.py` & `codecov-cli-0.1.9/codecov_cli/commands/create_report_result.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/commands/get_report_results.py` & `codecov-cli-0.1.9/codecov_cli/commands/get_report_results.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/commands/labelanalysis.py` & `codecov-cli-0.1.9/codecov_cli/commands/labelanalysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import time
 
 import click
 import requests
 
 from codecov_cli.fallbacks import CodecovOption, FallbackFieldEnum
 from codecov_cli.runners import get_runner
+from codecov_cli.runners.types import LabelAnalysisRequestResult
 
 logger = logging.getLogger("codecovcli")
 
 
 @click.command()
 @click.option(
     "--token",
@@ -82,20 +83,22 @@
                 "Sorry. Codecov is having problems",
                 extra=dict(extra_log_attributes=dict(status_code=response.status_code)),
             )
             if requested_labels:
                 logger.info(
                     "Could not get set of tests to run. Falling back to running all collected tests."
                 )
-                fake_response = {
-                    "present_report_labels": [],
-                    "absent_labels": requested_labels,
-                    "present_diff_labels": [],
-                    "global_level_labels": [],
-                }
+                fake_response = LabelAnalysisRequestResult(
+                    {
+                        "present_report_labels": [],
+                        "absent_labels": requested_labels,
+                        "present_diff_labels": [],
+                        "global_level_labels": [],
+                    }
+                )
                 return runner.process_labelanalysis_result(fake_response)
             raise click.ClickException("Sorry. Codecov is having problems")
         if response.status_code >= 400:
             logger.warning(
                 "Got a 4XX status code back from Codecov",
                 extra=dict(
                     extra_log_attributes=dict(
@@ -115,26 +118,30 @@
     while not has_result:
         resp_data = requests.get(
             f"https://api.codecov.io/labels/labels-analysis/{eid}",
             headers={"Authorization": token_header},
         )
         resp_json = resp_data.json()
         if resp_json["state"] == "finished":
-            runner.process_labelanalysis_result(resp_data.json()["result"])
+            runner.process_labelanalysis_result(
+                LabelAnalysisRequestResult(resp_data.json()["result"])
+            )
             return
         if resp_json["state"] == "error":
             logger.error(
                 "Request had problems calculating",
                 extra=dict(extra_log_attributes=dict(resp_json=resp_json)),
             )
             if requested_labels:
                 logger.info("Using requested labels as tests to run")
-                fake_response = {
-                    "present_report_labels": [],
-                    "absent_labels": requested_labels,
-                    "present_diff_labels": [],
-                    "global_level_labels": [],
-                }
+                fake_response = LabelAnalysisRequestResult(
+                    {
+                        "present_report_labels": [],
+                        "absent_labels": requested_labels,
+                        "present_diff_labels": [],
+                        "global_level_labels": [],
+                    }
+                )
                 return runner.process_labelanalysis_result(fake_response)
             return
         logger.info("Waiting more time for result")
         time.sleep(5)
```

### Comparing `codecov-cli-0.1.8/codecov_cli/commands/report.py` & `codecov-cli-0.1.9/codecov_cli/commands/report.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/commands/staticanalysis.py` & `codecov-cli-0.1.9/codecov_cli/commands/staticanalysis.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/commands/upload.py` & `codecov-cli-0.1.9/codecov_cli/commands/upload.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/fallbacks.py` & `codecov-cli-0.1.9/codecov_cli/fallbacks.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/__init__.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/appveyor_ci.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/appveyor_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/azure_pipelines.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/azure_pipelines.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/base.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/base.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/bitbucket_ci.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/bitbucket_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/bitrise_ci.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/bitrise_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/buildkite.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/buildkite.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/circleci.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/circleci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/cirrus_ci.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/cirrus_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/codebuild.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/codebuild.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/droneci.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/droneci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/github_actions.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/github_actions.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/gitlab_ci.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/gitlab_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/heroku.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/heroku.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/jenkins.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/jenkins.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/local.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/local.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/teamcity.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/teamcity.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/travis_ci.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/travis_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/woodpeckerci.py` & `codecov-cli-0.1.9/codecov_cli/helpers/ci_adapters/woodpeckerci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/encoder.py` & `codecov-cli-0.1.9/codecov_cli/helpers/encoder.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/folder_searcher.py` & `codecov-cli-0.1.9/codecov_cli/helpers/folder_searcher.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/git.py` & `codecov-cli-0.1.9/codecov_cli/helpers/git.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/logging_utils.py` & `codecov-cli-0.1.9/codecov_cli/helpers/logging_utils.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/request.py` & `codecov-cli-0.1.9/codecov_cli/helpers/request.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/helpers/versioning_systems.py` & `codecov-cli-0.1.9/codecov_cli/helpers/versioning_systems.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/main.py` & `codecov-cli-0.1.9/codecov_cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import typing
 
 import click
 
 from codecov_cli.commands.base_picking import pr_base_picking
 from codecov_cli.commands.commit import create_commit
 from codecov_cli.commands.create_report_result import create_report_results
+from codecov_cli.commands.empty_upload import empty_upload
 from codecov_cli.commands.get_report_results import get_report_results
 from codecov_cli.commands.labelanalysis import label_analysis
 from codecov_cli.commands.report import create_report
 from codecov_cli.commands.staticanalysis import static_analysis
 from codecov_cli.commands.upload import do_upload
 from codecov_cli.helpers.ci_adapters import get_ci_adapter, get_ci_providers_list
 from codecov_cli.helpers.config import load_cli_config
@@ -57,14 +58,15 @@
 cli.add_command(create_commit)
 cli.add_command(create_report)
 cli.add_command(create_report_results)
 cli.add_command(get_report_results)
 cli.add_command(pr_base_picking)
 cli.add_command(label_analysis)
 cli.add_command(static_analysis)
+cli.add_command(empty_upload)
 
 
 def run():
     cli(obj={})
 
 
 if __name__ == "__main__":
```

### Comparing `codecov-cli-0.1.8/codecov_cli/plugins/__init__.py` & `codecov-cli-0.1.9/codecov_cli/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/plugins/gcov.py` & `codecov-cli-0.1.9/codecov_cli/plugins/gcov.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/plugins/pycoverage.py` & `codecov-cli-0.1.9/codecov_cli/plugins/pycoverage.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/plugins/xcode.py` & `codecov-cli-0.1.9/codecov_cli/plugins/xcode.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/runners/__init__.py` & `codecov-cli-0.1.9/codecov_cli/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/runners/dan_runner.py` & `codecov-cli-0.1.9/codecov_cli/runners/dan_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 import subprocess
-from typing import List, TypedDict, Union
+from typing import List, Optional, Union
 
 from codecov_cli.runners.types import (
     LabelAnalysisRequestResult,
     LabelAnalysisRunnerInterface,
 )
 
 
-class DoAnythingNowConfigParams(TypedDict):
-    collect_tests_command: Union[List[str], str]
-    process_labelanalysis_result_command: Union[List[str], str]
+class DoAnythingNowConfigParams(dict):
+    @property
+    def collect_tests_command(self) -> Union[List[str], str]:
+        return self.get("collect_tests_command", None)
+
+    @property
+    def process_labelanalysis_result_command(self) -> Union[List[str], str]:
+        return self.get("process_labelanalysis_result_command", None)
 
 
 class DoAnythingNowRunner(LabelAnalysisRunnerInterface):
-    def __init__(self, config_params: DoAnythingNowConfigParams = None) -> None:
+    def __init__(self, config_params: Optional[dict] = None) -> None:
         super().__init__()
         if config_params is None:
-            config_params = DoAnythingNowConfigParams()
-        self.params = config_params
+            config_params = {}
+        self.params = DoAnythingNowConfigParams(config_params)
 
     def collect_tests(self) -> List[str]:
-        command = self.params.get("collect_tests_command", None)
+        command = self.params.collect_tests_command
         if command is None:
             raise Exception(
                 "DAN runner missing 'collect_tests_command' configuration value"
             )
         return subprocess.run(command, check=True, capture_output=True).stdout.decode()
 
     def process_labelanalysis_result(self, result: LabelAnalysisRequestResult):
-        command = self.params.get("process_labelanalysis_result_command", None)
+        command = self.params.process_labelanalysis_result_command
         if command is None:
             raise Exception(
                 "DAN runner missing 'process_labelanalysis_result_command' configuration value"
             )
         return subprocess.run(command, check=True, capture_output=True).stdout.decode()
```

### Comparing `codecov-cli-0.1.8/codecov_cli/runners/python_standard_runner.py` & `codecov-cli-0.1.9/codecov_cli/runners/python_standard_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 import logging
+import random
 from contextlib import redirect_stdout
 from io import StringIO, TextIOWrapper
 from multiprocessing import Queue, get_context
 from os import getcwd
 from sys import path, stdout
-from typing import List, TypedDict
+from typing import List, Optional
 
 import pytest
 
 from codecov_cli.runners.types import (
     LabelAnalysisRequestResult,
     LabelAnalysisRunnerInterface,
 )
 
 logger = logging.getLogger("codecovcli")
 
 
-class PythonStandardRunnerConfigParams(TypedDict):
-    collect_tests_options: List[str]
-    # include_dirs is to account for the difference described in
-    # https://docs.pytest.org/en/7.1.x/how-to/usage.html#calling-pytest-through-python-m-pytest
-    include_curr_dir: bool
+class PythonStandardRunnerConfigParams(dict):
+    @property
+    def collect_tests_options(self) -> List[str]:
+        return self.get("collect_tests_options", [])
+
+    @property
+    def include_curr_dir(self) -> bool:
+        """ "
+        Account for the difference 'pytest' vs 'python -m pytest'
+        https://docs.pytest.org/en/7.1.x/how-to/usage.html#calling-pytest-through-python-m-pytest
+        """
+        return self.get("include_curr_dir", True)
 
 
 def _include_curr_dir(method):
     def call_method(self, *args, **kwargs):
-        include_curr_dir = self.params["include_curr_dir"]
+        include_curr_dir = self.params.include_curr_dir
         curr_dir = getcwd()
         if include_curr_dir:
             path.append(curr_dir)
         result = method(self, *args, **kwargs)
         if include_curr_dir:
             path.remove(curr_dir)
         return result
@@ -57,23 +65,19 @@
         result = pytest.main(pytest_args)
     if capture_output:
         queue.put(subproces_stdout.getvalue())
     queue.put(result)
 
 
 class PythonStandardRunner(LabelAnalysisRunnerInterface):
-    def __init__(self, config_params: PythonStandardRunnerConfigParams = None) -> None:
+    def __init__(self, config_params: Optional[dict] = None) -> None:
         super().__init__()
-        default_config: PythonStandardRunnerConfigParams = {
-            "collect_tests_options": [],
-            "include_curr_dir": True,
-        }
         if config_params is None:
-            config_params = PythonStandardRunnerConfigParams()
-        self.params = {**default_config, **config_params}
+            config_params = {}
+        self.params = PythonStandardRunnerConfigParams(config_params)
 
     @_include_curr_dir
     def _execute_pytest(
         self, pytest_args: List[str], capture_output: bool = True, numprocess: int = 1
     ) -> str:
         """Handles calling pytest from Python in a subprocess.
         Raises Exception if pytest fails
@@ -98,15 +102,15 @@
                 extra=dict(extra_log_attributes=dict(exit_code=result, output=output)),
             )
             raise Exception("Pytest did not run correctly")
         return output
 
     def collect_tests(self):
         default_options = ["-q", "--collect-only"]
-        extra_args = self.params["collect_tests_options"]
+        extra_args = self.params.collect_tests_options
         options_to_use = default_options + extra_args
         logger.debug(
             "Collecting tests",
             extra=dict(
                 extra_log_attributes=dict(options=options_to_use),
             ),
         )
@@ -139,14 +143,20 @@
             logger.info(
                 "Some tests are being skipped",
                 extra=dict(
                     extra_log_attributes=dict(skipped_tests=sorted(skipped_tests))
                 ),
             )
 
+        if len(all_labels) == 0:
+            all_labels = [random.choice(result["present_report_labels"])]
+            logger.info(
+                "All tests are being skipped. Selected random label to run",
+                extra=dict(extra_log_attributes=dict(selected_label=all_labels[0])),
+            )
         command_array = default_options + [
             label.split("[")[0] if "[" in label else label for label in all_labels
         ]
         logger.info("Running tests")
         logger.debug(
             "Pytest command",
             extra=dict(extra_log_attributes=dict(command_array=command_array)),
```

### Comparing `codecov-cli-0.1.8/codecov_cli/services/commit/__init__.py` & `codecov-cli-0.1.9/codecov_cli/services/commit/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/services/commit/base_picking.py` & `codecov-cli-0.1.9/codecov_cli/services/commit/base_picking.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/services/report/__init__.py` & `codecov-cli-0.1.9/codecov_cli/services/report/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/services/staticanalysis/__init__.py` & `codecov-cli-0.1.9/codecov_cli/services/staticanalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/ecmascriptsix.py` & `codecov-cli-0.1.9/codecov_cli/services/staticanalysis/analyzers/ecmascriptsix.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/python/__init__.py` & `codecov-cli-0.1.9/codecov_cli/services/staticanalysis/analyzers/python/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py` & `codecov-cli-0.1.9/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/services/staticanalysis/finders.py` & `codecov-cli-0.1.9/codecov_cli/services/staticanalysis/finders.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/services/upload/__init__.py` & `codecov-cli-0.1.9/codecov_cli/services/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/services/upload/coverage_file_finder.py` & `codecov-cli-0.1.9/codecov_cli/services/upload/coverage_file_finder.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/services/upload/legacy_upload_sender.py` & `codecov-cli-0.1.9/codecov_cli/services/upload/legacy_upload_sender.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/services/upload/network_finder.py` & `codecov-cli-0.1.9/codecov_cli/services/upload/network_finder.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/services/upload/upload_collector.py` & `codecov-cli-0.1.9/codecov_cli/services/upload/upload_collector.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/services/upload/upload_sender.py` & `codecov-cli-0.1.9/codecov_cli/services/upload/upload_sender.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli/types.py` & `codecov-cli-0.1.9/codecov_cli/types.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/codecov_cli.egg-info/PKG-INFO` & `codecov-cli-0.1.9/codecov_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecov-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: Codecov Command Line Interface
 Author: Codecov
 Author-email: support@codecov.io
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CodecovCLI
```

### Comparing `codecov-cli-0.1.8/codecov_cli.egg-info/SOURCES.txt` & `codecov-cli-0.1.9/codecov_cli.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 codecov_cli.egg-info/entry_points.txt
 codecov_cli.egg-info/requires.txt
 codecov_cli.egg-info/top_level.txt
 codecov_cli/commands/__init__.py
 codecov_cli/commands/base_picking.py
 codecov_cli/commands/commit.py
 codecov_cli/commands/create_report_result.py
+codecov_cli/commands/empty_upload.py
 codecov_cli/commands/get_report_results.py
 codecov_cli/commands/labelanalysis.py
 codecov_cli/commands/report.py
 codecov_cli/commands/staticanalysis.py
 codecov_cli/commands/upload.py
 codecov_cli/helpers/__init__.py
 codecov_cli/helpers/config.py
@@ -56,14 +57,15 @@
 codecov_cli/runners/__init__.py
 codecov_cli/runners/dan_runner.py
 codecov_cli/runners/python_standard_runner.py
 codecov_cli/runners/types.py
 codecov_cli/services/__init__.py
 codecov_cli/services/commit/__init__.py
 codecov_cli/services/commit/base_picking.py
+codecov_cli/services/empty_upload/__init__.py
 codecov_cli/services/report/__init__.py
 codecov_cli/services/staticanalysis/__init__.py
 codecov_cli/services/staticanalysis/exceptions.py
 codecov_cli/services/staticanalysis/finders.py
 codecov_cli/services/staticanalysis/types.py
 codecov_cli/services/staticanalysis/analyzers/__init__.py
 codecov_cli/services/staticanalysis/analyzers/ecmascriptsix.py
```

### Comparing `codecov-cli-0.1.8/languages/treesitterjavascript/src/parser.c` & `codecov-cli-0.1.9/languages/treesitterjavascript/src/parser.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/languages/treesitterjavascript/src/scanner.c` & `codecov-cli-0.1.9/languages/treesitterjavascript/src/scanner.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/languages/treesitterjavascript/src/tree_sitter/parser.h` & `codecov-cli-0.1.9/languages/treesitterjavascript/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/languages/treesitterpython/src/parser.c` & `codecov-cli-0.1.9/languages/treesitterpython/src/parser.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/languages/treesitterpython/src/scanner.cc` & `codecov-cli-0.1.9/languages/treesitterpython/src/scanner.cc`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/languages/treesitterpython/src/tree_sitter/parser.h` & `codecov-cli-0.1.9/languages/treesitterpython/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.8/setup.py` & `codecov-cli-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="codecov-cli",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_packages(exclude=["contrib", "docs", "tests*"]),
     description="Codecov Command Line Interface",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Codecov",
     author_email="support@codecov.io",
     install_requires=["click", "requests", "PyYAML", "tree_sitter", "httpx"],
```

