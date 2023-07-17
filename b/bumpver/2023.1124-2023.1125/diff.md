# Comparing `tmp/bumpver-2023.1124.tar.gz` & `tmp/bumpver-2023.1125.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bumpver-2023.1124.tar", last modified: Thu May 18 16:42:50 2023, max compression
+gzip compressed data, was "bumpver-2023.1125.tar", last modified: Mon Jul 17 20:43:27 2023, max compression
```

## Comparing `bumpver-2023.1124.tar` & `bumpver-2023.1125.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 16:42:50.614464 bumpver-2023.1124/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     9444 2023-05-18 16:41:41.000000 bumpver-2023.1124/CHANGELOG.md
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     1127 2023-05-18 16:42:39.000000 bumpver-2023.1124/LICENSE
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      148 2023-05-04 13:50:20.000000 bumpver-2023.1124/MANIFEST.in
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    50907 2023-05-18 16:42:50.616801 bumpver-2023.1124/PKG-INFO
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    40281 2023-05-18 16:42:39.000000 bumpver-2023.1124/README.md
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     4053 2023-05-04 13:50:20.000000 bumpver-2023.1124/fastentrypoints.py
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 16:42:48.985055 bumpver-2023.1124/requirements/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      697 2023-05-04 14:52:41.000000 bumpver-2023.1124/requirements/pypi.txt
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2370 2023-05-18 16:42:50.626898 bumpver-2023.1124/setup.cfg
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2457 2023-05-18 16:42:39.000000 bumpver-2023.1124/setup.py
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 16:42:48.781171 bumpver-2023.1124/src/
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 16:42:49.683965 bumpver-2023.1124/src/bumpver/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      262 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/__init__.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      363 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/__main__.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    25865 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/cli.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    21008 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/config.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2548 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/parse.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      793 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/patterns.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     1214 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/pysix.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2267 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/regexfmt.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2290 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/rewrite.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      612 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/utils.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     7915 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/v1patterns.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     5257 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/v1rewrite.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    13411 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/v1version.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    11047 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/v2patterns.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     5736 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/v2rewrite.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    28055 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/v2version.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     8275 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/vcs.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     4177 2023-05-18 16:42:39.000000 bumpver-2023.1124/src/bumpver/version.py
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 16:42:49.948745 bumpver-2023.1124/src/bumpver.egg-info/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    50907 2023-05-18 16:42:48.000000 bumpver-2023.1124/src/bumpver.egg-info/PKG-INFO
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     1262 2023-05-18 16:42:48.000000 bumpver-2023.1124/src/bumpver.egg-info/SOURCES.txt
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        1 2023-05-18 16:42:48.000000 bumpver-2023.1124/src/bumpver.egg-info/dependency_links.txt
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       44 2023-05-18 16:42:48.000000 bumpver-2023.1124/src/bumpver.egg-info/entry_points.txt
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      198 2023-05-18 16:42:48.000000 bumpver-2023.1124/src/bumpver.egg-info/requires.txt
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        8 2023-05-18 16:42:48.000000 bumpver-2023.1124/src/bumpver.egg-info/top_level.txt
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        1 2023-05-18 16:42:48.000000 bumpver-2023.1124/src/bumpver.egg-info/zip-safe
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 16:42:50.125260 bumpver-2023.1124/test/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 13:50:20.000000 bumpver-2023.1124/test/__init__.py
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 16:42:48.848925 bumpver-2023.1124/test/fixtures/
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 16:42:50.188409 bumpver-2023.1124/test/fixtures/project_a/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       66 2023-05-04 13:50:20.000000 bumpver-2023.1124/test/fixtures/project_a/README.md
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      266 2023-05-04 13:50:20.000000 bumpver-2023.1124/test/fixtures/project_a/bumpver.toml
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 16:42:50.304168 bumpver-2023.1124/test/fixtures/project_b/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      219 2023-05-04 13:50:20.000000 bumpver-2023.1124/test/fixtures/project_b/README.rst
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      461 2023-05-04 13:50:20.000000 bumpver-2023.1124/test/fixtures/project_b/setup.cfg
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      136 2023-05-04 13:50:20.000000 bumpver-2023.1124/test/fixtures/project_b/setup.py
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 16:42:48.831925 bumpver-2023.1124/test/fixtures/project_b/src/
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 16:42:50.354074 bumpver-2023.1124/test/fixtures/project_b/src/module_v1/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       34 2023-05-04 13:50:20.000000 bumpver-2023.1124/test/fixtures/project_b/src/module_v1/__init__.py
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 16:42:50.441214 bumpver-2023.1124/test/fixtures/project_b/src/module_v2/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       34 2023-05-04 13:50:20.000000 bumpver-2023.1124/test/fixtures/project_b/src/module_v2/__init__.py
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 16:42:50.514276 bumpver-2023.1124/test/fixtures/project_c/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      135 2023-05-04 13:50:20.000000 bumpver-2023.1124/test/fixtures/project_c/pyproject.toml
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 16:42:50.569576 bumpver-2023.1124/test/fixtures/project_d/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      114 2023-05-04 16:02:18.000000 bumpver-2023.1124/test/fixtures/project_d/pyproject.toml
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    43298 2023-05-18 15:50:02.000000 bumpver-2023.1124/test/test_cli.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    11574 2023-05-04 16:02:18.000000 bumpver-2023.1124/test/test_config.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2381 2023-05-04 13:50:20.000000 bumpver-2023.1124/test/test_parse.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    10418 2023-05-18 15:34:48.000000 bumpver-2023.1124/test/test_patterns.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    12813 2023-05-18 15:17:28.000000 bumpver-2023.1124/test/test_rewrite.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    10996 2023-05-18 14:55:21.000000 bumpver-2023.1124/test/test_version.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2481 2023-05-04 13:50:20.000000 bumpver-2023.1124/test/util.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-07-17 20:43:27.563299 bumpver-2023.1125/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    10066 2023-07-17 20:42:11.000000 bumpver-2023.1125/CHANGELOG.md
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     1127 2023-07-17 20:43:14.000000 bumpver-2023.1125/LICENSE
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      148 2023-05-04 13:50:20.000000 bumpver-2023.1125/MANIFEST.in
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    53224 2023-07-17 20:43:27.565648 bumpver-2023.1125/PKG-INFO
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    41976 2023-07-17 20:43:14.000000 bumpver-2023.1125/README.md
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     4053 2023-05-04 13:50:20.000000 bumpver-2023.1125/fastentrypoints.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-07-17 20:43:25.683695 bumpver-2023.1125/requirements/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      728 2023-07-17 20:42:11.000000 bumpver-2023.1125/requirements/pypi.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2371 2023-07-17 20:43:27.573324 bumpver-2023.1125/setup.cfg
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2457 2023-07-17 20:43:14.000000 bumpver-2023.1125/setup.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-07-17 20:43:25.461789 bumpver-2023.1125/src/
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-07-17 20:43:26.437730 bumpver-2023.1125/src/bumpver/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      262 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/__init__.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      363 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/__main__.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    27519 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/cli.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    22117 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/config.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2548 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/parse.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      793 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/patterns.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     1214 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/pysix.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2267 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/regexfmt.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2290 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/rewrite.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      612 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/utils.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     7915 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/v1patterns.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     5257 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/v1rewrite.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    13425 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/v1version.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    11047 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/v2patterns.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     5736 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/v2rewrite.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    28069 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/v2version.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     9591 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/vcs.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     4177 2023-07-17 20:43:14.000000 bumpver-2023.1125/src/bumpver/version.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-07-17 20:43:26.824980 bumpver-2023.1125/src/bumpver.egg-info/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    53224 2023-07-17 20:43:24.000000 bumpver-2023.1125/src/bumpver.egg-info/PKG-INFO
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     1262 2023-07-17 20:43:25.000000 bumpver-2023.1125/src/bumpver.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        1 2023-07-17 20:43:24.000000 bumpver-2023.1125/src/bumpver.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       44 2023-07-17 20:43:24.000000 bumpver-2023.1125/src/bumpver.egg-info/entry_points.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      232 2023-07-17 20:43:24.000000 bumpver-2023.1125/src/bumpver.egg-info/requires.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        8 2023-07-17 20:43:24.000000 bumpver-2023.1125/src/bumpver.egg-info/top_level.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        1 2023-07-17 17:15:26.000000 bumpver-2023.1125/src/bumpver.egg-info/zip-safe
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-07-17 20:43:27.066573 bumpver-2023.1125/test/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 13:50:20.000000 bumpver-2023.1125/test/__init__.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-07-17 20:43:25.546445 bumpver-2023.1125/test/fixtures/
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-07-17 20:43:27.162176 bumpver-2023.1125/test/fixtures/project_a/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       66 2023-05-04 13:50:20.000000 bumpver-2023.1125/test/fixtures/project_a/README.md
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      266 2023-05-04 13:50:20.000000 bumpver-2023.1125/test/fixtures/project_a/bumpver.toml
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-07-17 20:43:27.309183 bumpver-2023.1125/test/fixtures/project_b/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      219 2023-05-04 13:50:20.000000 bumpver-2023.1125/test/fixtures/project_b/README.rst
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      461 2023-05-04 13:50:20.000000 bumpver-2023.1125/test/fixtures/project_b/setup.cfg
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      136 2023-05-04 13:50:20.000000 bumpver-2023.1125/test/fixtures/project_b/setup.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-07-17 20:43:25.526407 bumpver-2023.1125/test/fixtures/project_b/src/
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-07-17 20:43:27.369097 bumpver-2023.1125/test/fixtures/project_b/src/module_v1/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       34 2023-05-04 13:50:20.000000 bumpver-2023.1125/test/fixtures/project_b/src/module_v1/__init__.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-07-17 20:43:27.426360 bumpver-2023.1125/test/fixtures/project_b/src/module_v2/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       34 2023-05-04 13:50:20.000000 bumpver-2023.1125/test/fixtures/project_b/src/module_v2/__init__.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-07-17 20:43:27.475056 bumpver-2023.1125/test/fixtures/project_c/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      135 2023-05-04 13:50:20.000000 bumpver-2023.1125/test/fixtures/project_c/pyproject.toml
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-07-17 20:43:27.522104 bumpver-2023.1125/test/fixtures/project_d/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      114 2023-05-04 16:02:18.000000 bumpver-2023.1125/test/fixtures/project_d/pyproject.toml
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    50771 2023-07-17 20:42:11.000000 bumpver-2023.1125/test/test_cli.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    12400 2023-07-17 20:42:11.000000 bumpver-2023.1125/test/test_config.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2381 2023-05-04 13:50:20.000000 bumpver-2023.1125/test/test_parse.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    10418 2023-05-18 15:34:48.000000 bumpver-2023.1125/test/test_patterns.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    12813 2023-05-18 15:17:28.000000 bumpver-2023.1125/test/test_rewrite.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    10996 2023-05-18 14:55:21.000000 bumpver-2023.1125/test/test_version.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2481 2023-05-04 13:50:20.000000 bumpver-2023.1125/test/util.py
```

### Comparing `bumpver-2023.1124/CHANGELOG.md` & `bumpver-2023.1125/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,23 @@
 # Changelog for https://github.com/mbarkhau/bumpver
 
+## BumpVer 2023.1125
+
+- Add [#188][gh_i188]: Add `--tag-scope=<SCOPE>` to support separate versioning for branches.
+- Add [#185][gh_i185]: Add `--tag-message=<TMPL>` parameter and `tag_message` configuration option.
+- Fix [#209][gh_i209]: Make `--no-tag-commit` ommit `--follow-tags`.
+
+[gh_i188]: https://github.com/mbarkhau/bumpver/issues/188
+[gh_i185]: https://github.com/mbarkhau/bumpver/issues/185
+[gh_i209]: https://github.com/mbarkhau/bumpver/issues/209
+
+Thank you [Sven Lohrmann](https://github.com/malnvenshorn) for your contributions.
+Thank you [tardis4500](https://github.com/tardis4500) for the issue report.
+
+
 ## BumpVer 2023.1124
 
 - Fix [#208][gh_i208]: Fix handling of versions with PEP440 epoch.
 
 [gh_i208]: https://github.com/mbarkhau/bumpver/issues/208
 
 Thank you [Wen Kokke](https://github.com/wenkokke) for the issue report.
```

### Comparing `bumpver-2023.1124/LICENSE` & `bumpver-2023.1125/LICENSE`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/PKG-INFO` & `bumpver-2023.1125/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bumpver
-Version: 2023.1124
+Version: 2023.1125
 Summary: Bump version numbers in project files.
 Home-page: https://github.com/mbarkhau/bumpver
 Author: Manuel Barkhau
 Author-email: mbarkhau@gmail.com
 License: MIT
 Keywords: version bumpver calver semver versioning bumpversion pep440
 Classifier: Development Status :: 4 - Beta
@@ -47,15 +47,15 @@
 [url_calver_org]: https://calver.org/
 
 
 Project/Repo:
 
 [![MIT License][img_license]][url_license]
 [![Supported Python Versions][img_pyversions]][url_pyversions]
-[![CalVer 2023.1124][img_version]][url_version]
+[![CalVer 2023.1125][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
 [![PyPI Downloads][img_downloads]][url_downloads]
 
 Code Quality/CI:
 
 [![GitHub Build Status][img_github_build]][url_github_build]
 [![GitLab Build Status][img_gitlab_build]][url_gitlab_build]
@@ -81,15 +81,15 @@
 
 [img_style]: https://img.shields.io/badge/code%20style-%20sjfmt-f71.svg
 [url_style]: https://gitlab.com/mbarkhau/straitjacket/
 
 [img_downloads]: https://pepy.tech/badge/bumpver/month
 [url_downloads]: https://pepy.tech/project/bumpver
 
-[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2023.1124&color=blue
+[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2023.1125&color=blue
 [url_version]: https://pypi.org/project/bumpver/
 
 [img_pypi]: https://img.shields.io/badge/PyPI-wheels-green.svg
 [url_pypi]: https://pypi.org/project/bumpver/#files
 
 [img_pyversions]: https://img.shields.io/pypi/pyversions/bumpver.svg
 [url_pyversions]: https://pypi.python.org/pypi/bumpver
@@ -445,15 +445,15 @@
 
 #### Add git hash to version string
 
 If you want to build a package straight from your git repository,
 without making a release first, you can explictly add git hash to
 the version number using ``GITHASH`` version part.
 
-Let's say your ``setup.cfg`` looks like this: 
+Let's say your ``setup.cfg`` looks like this:
 
 ```ini
 [bumpver]
 ...
 version_pattern = "YYYY.BUILD[-TAG][GITHASH]"
 ...
 ```
@@ -631,30 +631,33 @@
                                   uncomitted changes. (WARNING: The commit
                                   will still be aborted if there are
                                   uncomitted to files with version strings.
   --ignore-vcs-tag                Ignore VCS tag invariant and update version
                                   anyway.
   --set-version <VERSION>         Set version explicitly.
   --date <ISODATE>                Set explicit date in format YYYY-0M-0D (e.g.
-                                  2023-05-18).
+                                  2023-07-10).
   --pin-date                      Leave date components unchanged.
   --pin-increments                Leave the auto-increments INC0 and INC1
                                   unchanged.
   --tag-num                       Increment release tag number (rc1, rc2,
                                   rc3..).
   -t, --tag <NAME>                Override release tag of current_version.
                                   Valid options are: alpha, beta, dev, rc,
                                   post, final.
   -p, --patch                     Increment PATCH component.
   -m, --minor                     Increment MINOR component.
   --major                         Increment MAJOR component.
   -c, --commit-message <TMPL>     Set commit message template.
+  --tag-message <TMPL>            Set tag message template.
   --commit / --no-commit          Create a commit with all updated files.
   --tag-commit / --no-tag-commit  Tag the newly created commit.
   --push / --no-push              Push to the default remote.
+  --tag-scope [default|global|branch]
+                                  Tag scope for the current version.
   -h, --help                      Show this message and exit.
 ```
 
 <!-- END bumpver update --help -->
 
 To help with shell script automation, you can use `bumpver show --env`.
 
@@ -826,26 +829,28 @@
 
 The create an initial configuration for project with `bumpver init`.
 
 ```shell
 $ pip install bumpver
 ...
 Installing collected packages: click toml lexid bumpver
-Successfully installed bumpver-2023.1124
+Successfully installed bumpver-2023.1125
 
 $ cd myproject
 ~/myproject/
 
 $ bumpver init --dry
 Exiting because of '-d/--dry'. Would have written to bumpver.toml:
 
     [bumpver]
     current_version = "2020.1001a0"
     version_pattern = "YYYY.BUILD[PYTAGNUM]"
     commit_message = "bump version to {new_version}"
+    tag_message = "{new_version}"
+    tag_scope = "default"
     commit = true
     tag = true
     push = true
 
     [bumpver.file_patterns]
     "README.md" = [
         "{version}",
@@ -867,14 +872,16 @@
 Your `setup.cfg` may now look something like this:
 
 ```ini
 [bumpver]
 current_version = "2019.1001-alpha"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump version to {new_version}"
+tag_message = "{new_version}"
+tag_scope = "default"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
 setup.cfg =
     current_version = "{version}"
@@ -951,25 +958,29 @@
 ## Bump It Up
 
 
 ### Version State
 
 The `current_version` is considered global state and must be stored somewhere. Typically this might be in a `VERSION` file, or some other file which is part of the repository. This creates the risk that parallel branches can have different states. If the `current_version`  were defined only by files in the local checkout, the same version might be generated on different systems for different commits.
 
-To avoid this issue, `bumpver` treats Git/Mercurial tags as the canonical / [SSOT][url_ssot] for the most recent version and attempts to change this state in the most atomic way possible. This is why some actions of the `bumpver` command can take a few seconds, as it is synchronizing with the remote repository to get the most recent versions and to push any new version tags as soon as possible.
-
-[url_ssot]: https://en.wikipedia.org/wiki/Single_source_of_truth
+To avoid this issue, `bumpver` treats Git/Mercurial tags as a second source, depending on the `tag_scope` option, for the most recent version and attempts to change this state in the most atomic way possible. This is why some actions of the `bumpver` command can take a few seconds, as it is synchronizing with the remote repository to get the most recent versions and to push any new version tags as soon as possible.
 
 
 ### The Current Version
 
-The current version is either
+The current version depends on the configured `tag_scope` and is either
+
+| `tag_scope =` |	`current_version =`                                 |
+|---------------|-----------------------------------------------------|
+| `default`     |	`max(config.current_version, max(global_vcs_tags))` |
+| `global`      | `max(global_vcs_tags)`                              |
+| `branch`      | `max(branch_vcs_tags)`                              |
 
- - Typically: The largest Git/Mercurial tag which matches the `version_pattern` from your config, sorted using [`pkg_resources.parse_version`][url_setuptools_pkg_resources].
- - Rarely: Before any tags have been created, the value of `current_version` in `bumpver.toml` / `setup.cfg` / `pyproject.toml`.
+- Before any tags have been created `bumpver` will always default to the value of `current_version` in `bumpver.toml` / `setup.cfg` / `pyproject.toml`.
+- Only Git/Mercurial tags which matches the `version_pattern` from your config will be considered and sorted using [`pkg_resources.parse_version`][url_setuptools_pkg_resources].
 
 [url_setuptools_pkg_resources]: https://setuptools.readthedocs.io/en/latest/pkg_resources.html#parsing-utilities
 
 As part of doing `bumpver update` and `bumpver show`, your local tags are updated using `git fetch --tags`/`hg pull`.
 
 ```shell
 $ bumpver show -vv
@@ -1033,40 +1044,44 @@
 ```
 
 
 ### VCS Parameters (git/mercurial)
 
 The individual steps performed by `bumpver update`:
 
-0. Check that you have no local changes that are uncommitted.
-1. *Fetch* the most recent global VCS tags from origin.
-2. Generate the updated version string.
-3. Replace version strings in all files configured in `file_patterns`.
-4. *Commit* the updated files.
-5. *Tag* the new commit.
-6. *Push* the new commit and tag.
+1. *Fetch* VCS tags from origin.
+2. Get most recent version.
+3. Generate the updated version string.
+4. Check that you have no local changes that are uncommitted.
+5. Replace version strings in all files configured in `file_patterns`.
+6. *Commit* the updated files.
+7. *Tag* the new commit.
+8. *Push* the new commit and tag.
 
 The configuration for these steps can be done with the following parameters:
 
-|    Parameter     |   Type   |               Description               |
-|------------------|----------|-----------------------------------------|
-| `commit_message` | string¹  | Template for commit message in step 4.  |
-| `commit`         | boolean  | Create a commit with all updated files. |
-| `tag`            | boolean² | Tag the newly created commit.           |
-| `push`           | boolean² | Push to the default remote.             |
+|    Parameter     |   Type   |                 Description                |
+|------------------|----------|--------------------------------------------|
+| `tag_scope`      | string   | Scope for the `current_version` in step 2. |
+| `commit_message` | string¹  | Template for commit message in step 6.     |
+| `tag_message`    | string¹  | Template for tag message in step 7.        |
+| `commit`         | boolean  | Create a commit with all updated files.    |
+| `tag`            | boolean² | Tag the newly created commit.              |
+| `push`           | boolean² | Push to the default remote.                |
 
 - ¹ Available placeholders for the `commit_message`: `{new_version}`, `{old_version}`, `{new_version_pep440}`, `{old_version_pep440}`
 - ² Requires `commit = True`
 
 An example configuration might look like this:
 
 ```ini
 [bumpver]
 ...
 commit_message = "bump version to {new_version}"
+tag_message = "{new_version}"
 commit = True
 tag = True
 push = True
 ```
 
 If everything looks OK, you can do `bumpver update`.
 
@@ -1097,15 +1112,15 @@
 In addition to the `commit_message` configuration, you can also override the string used as the the commit message template with the `-c/--commit-message=<TMPL>` parameter:
 
 ```shell
 $ bumpver update --tag final --commit-message 'bump version {old_version} -> {new_version} [ci-publish]' --verbose
 INFO    - Old Version: 2021.1005b0
 INFO    - New Version: 2021.1006
 INFO    - git commit --message 'bump version 2020.1005b0 -> 2021.1006 [ci-publish]'
-INFO    - git tag --annotate 2020.1006 --message 2020.1006
+INFO    - git tag --annotate 2020.1006 --message '2020.1006'
 INFO    - git push origin --follow-tags 2020.1006 HEAD
 ```
 
 As this is a manual operation (rather than a long lived configuration option), you can use the placeholders `OLD` and `NEW` for convenience, instead of the more verbose `{old_version}` and `{new_version}`.
 
 ```shell
 $ bumpver update -f -t final -c '[final-version] OLD -> NEW'
@@ -1113,23 +1128,64 @@
 INFO    - Old Version: 1.2.0b2
 INFO    - New Version: 1.2.0
 INFO    - git commit --message '[final-version] 1.2.0b2 -> 1.2.0'
 ...
 ```
 
 
+### Custom Tag Message
+
+Similarly to `--commit-message` you can provide a tag message template by using the `--tag-message=<TMPL>` parameter or the `tag_message` configuration:
+
+```shell
+$ bumpver update -f -t final --tag-message 'release NEW'
+INFO    - Old Version: 1.2.0b2
+INFO    - New Version: 1.2.0
+...
+INFO    - git tag --annotate 1.2.0 --message 'release 1.2.0'
+...
+```
+
+You can use the same placeholders as in the `--commit-message` template.
+
+If an empty tag message is provided, bumpver uses a lightweight tag in Git. Otherwise, it utilizes an annotated Git tag. You can read more about Git tagging [here](https://git-scm.com/book/en/v2/Git-Basics-Tagging).
+
+```shell
+$ bumpver update -f -t final --tag-message ''
+INFO    - Old Version: 1.2.0b2
+INFO    - New Version: 1.2.0
+...
+INFO    - git tag 1.2.0
+...
+```
+
+
 ## Contributors
 
 |                Name                 |    role           |  since  | until |
 |-------------------------------------|-------------------|---------|-------|
 | Manuel Barkhau (mbarkhau@gmail.com) | author/maintainer | 2018-09 | -     |
 
 
 # Changelog for https://github.com/mbarkhau/bumpver
 
+## BumpVer 2023.1125
+
+- Add [#188][gh_i188]: Add `--tag-scope=<SCOPE>` to support separate versioning for branches.
+- Add [#185][gh_i185]: Add `--tag-message=<TMPL>` parameter and `tag_message` configuration option.
+- Fix [#209][gh_i209]: Make `--no-tag-commit` ommit `--follow-tags`.
+
+[gh_i188]: https://github.com/mbarkhau/bumpver/issues/188
+[gh_i185]: https://github.com/mbarkhau/bumpver/issues/185
+[gh_i209]: https://github.com/mbarkhau/bumpver/issues/209
+
+Thank you [Sven Lohrmann](https://github.com/malnvenshorn) for your contributions.
+Thank you [tardis4500](https://github.com/tardis4500) for the issue report.
+
+
 ## BumpVer 2023.1124
 
 - Fix [#208][gh_i208]: Fix handling of versions with PEP440 epoch.
 
 [gh_i208]: https://github.com/mbarkhau/bumpver/issues/208
 
 Thank you [Wen Kokke](https://github.com/wenkokke) for the issue report.
```

### Comparing `bumpver-2023.1124/README.md` & `bumpver-2023.1125/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [url_calver_org]: https://calver.org/
 
 
 Project/Repo:
 
 [![MIT License][img_license]][url_license]
 [![Supported Python Versions][img_pyversions]][url_pyversions]
-[![CalVer 2023.1124][img_version]][url_version]
+[![CalVer 2023.1125][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
 [![PyPI Downloads][img_downloads]][url_downloads]
 
 Code Quality/CI:
 
 [![GitHub Build Status][img_github_build]][url_github_build]
 [![GitLab Build Status][img_gitlab_build]][url_gitlab_build]
@@ -52,15 +52,15 @@
 
 [img_style]: https://img.shields.io/badge/code%20style-%20sjfmt-f71.svg
 [url_style]: https://gitlab.com/mbarkhau/straitjacket/
 
 [img_downloads]: https://pepy.tech/badge/bumpver/month
 [url_downloads]: https://pepy.tech/project/bumpver
 
-[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2023.1124&color=blue
+[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2023.1125&color=blue
 [url_version]: https://pypi.org/project/bumpver/
 
 [img_pypi]: https://img.shields.io/badge/PyPI-wheels-green.svg
 [url_pypi]: https://pypi.org/project/bumpver/#files
 
 [img_pyversions]: https://img.shields.io/pypi/pyversions/bumpver.svg
 [url_pyversions]: https://pypi.python.org/pypi/bumpver
@@ -416,15 +416,15 @@
 
 #### Add git hash to version string
 
 If you want to build a package straight from your git repository,
 without making a release first, you can explictly add git hash to
 the version number using ``GITHASH`` version part.
 
-Let's say your ``setup.cfg`` looks like this: 
+Let's say your ``setup.cfg`` looks like this:
 
 ```ini
 [bumpver]
 ...
 version_pattern = "YYYY.BUILD[-TAG][GITHASH]"
 ...
 ```
@@ -602,30 +602,33 @@
                                   uncomitted changes. (WARNING: The commit
                                   will still be aborted if there are
                                   uncomitted to files with version strings.
   --ignore-vcs-tag                Ignore VCS tag invariant and update version
                                   anyway.
   --set-version <VERSION>         Set version explicitly.
   --date <ISODATE>                Set explicit date in format YYYY-0M-0D (e.g.
-                                  2023-05-18).
+                                  2023-07-10).
   --pin-date                      Leave date components unchanged.
   --pin-increments                Leave the auto-increments INC0 and INC1
                                   unchanged.
   --tag-num                       Increment release tag number (rc1, rc2,
                                   rc3..).
   -t, --tag <NAME>                Override release tag of current_version.
                                   Valid options are: alpha, beta, dev, rc,
                                   post, final.
   -p, --patch                     Increment PATCH component.
   -m, --minor                     Increment MINOR component.
   --major                         Increment MAJOR component.
   -c, --commit-message <TMPL>     Set commit message template.
+  --tag-message <TMPL>            Set tag message template.
   --commit / --no-commit          Create a commit with all updated files.
   --tag-commit / --no-tag-commit  Tag the newly created commit.
   --push / --no-push              Push to the default remote.
+  --tag-scope [default|global|branch]
+                                  Tag scope for the current version.
   -h, --help                      Show this message and exit.
 ```
 
 <!-- END bumpver update --help -->
 
 To help with shell script automation, you can use `bumpver show --env`.
 
@@ -797,26 +800,28 @@
 
 The create an initial configuration for project with `bumpver init`.
 
 ```shell
 $ pip install bumpver
 ...
 Installing collected packages: click toml lexid bumpver
-Successfully installed bumpver-2023.1124
+Successfully installed bumpver-2023.1125
 
 $ cd myproject
 ~/myproject/
 
 $ bumpver init --dry
 Exiting because of '-d/--dry'. Would have written to bumpver.toml:
 
     [bumpver]
     current_version = "2020.1001a0"
     version_pattern = "YYYY.BUILD[PYTAGNUM]"
     commit_message = "bump version to {new_version}"
+    tag_message = "{new_version}"
+    tag_scope = "default"
     commit = true
     tag = true
     push = true
 
     [bumpver.file_patterns]
     "README.md" = [
         "{version}",
@@ -838,14 +843,16 @@
 Your `setup.cfg` may now look something like this:
 
 ```ini
 [bumpver]
 current_version = "2019.1001-alpha"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump version to {new_version}"
+tag_message = "{new_version}"
+tag_scope = "default"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
 setup.cfg =
     current_version = "{version}"
@@ -922,25 +929,29 @@
 ## Bump It Up
 
 
 ### Version State
 
 The `current_version` is considered global state and must be stored somewhere. Typically this might be in a `VERSION` file, or some other file which is part of the repository. This creates the risk that parallel branches can have different states. If the `current_version`  were defined only by files in the local checkout, the same version might be generated on different systems for different commits.
 
-To avoid this issue, `bumpver` treats Git/Mercurial tags as the canonical / [SSOT][url_ssot] for the most recent version and attempts to change this state in the most atomic way possible. This is why some actions of the `bumpver` command can take a few seconds, as it is synchronizing with the remote repository to get the most recent versions and to push any new version tags as soon as possible.
-
-[url_ssot]: https://en.wikipedia.org/wiki/Single_source_of_truth
+To avoid this issue, `bumpver` treats Git/Mercurial tags as a second source, depending on the `tag_scope` option, for the most recent version and attempts to change this state in the most atomic way possible. This is why some actions of the `bumpver` command can take a few seconds, as it is synchronizing with the remote repository to get the most recent versions and to push any new version tags as soon as possible.
 
 
 ### The Current Version
 
-The current version is either
+The current version depends on the configured `tag_scope` and is either
+
+| `tag_scope =` |	`current_version =`                                 |
+|---------------|-----------------------------------------------------|
+| `default`     |	`max(config.current_version, max(global_vcs_tags))` |
+| `global`      | `max(global_vcs_tags)`                              |
+| `branch`      | `max(branch_vcs_tags)`                              |
 
- - Typically: The largest Git/Mercurial tag which matches the `version_pattern` from your config, sorted using [`pkg_resources.parse_version`][url_setuptools_pkg_resources].
- - Rarely: Before any tags have been created, the value of `current_version` in `bumpver.toml` / `setup.cfg` / `pyproject.toml`.
+- Before any tags have been created `bumpver` will always default to the value of `current_version` in `bumpver.toml` / `setup.cfg` / `pyproject.toml`.
+- Only Git/Mercurial tags which matches the `version_pattern` from your config will be considered and sorted using [`pkg_resources.parse_version`][url_setuptools_pkg_resources].
 
 [url_setuptools_pkg_resources]: https://setuptools.readthedocs.io/en/latest/pkg_resources.html#parsing-utilities
 
 As part of doing `bumpver update` and `bumpver show`, your local tags are updated using `git fetch --tags`/`hg pull`.
 
 ```shell
 $ bumpver show -vv
@@ -1004,40 +1015,44 @@
 ```
 
 
 ### VCS Parameters (git/mercurial)
 
 The individual steps performed by `bumpver update`:
 
-0. Check that you have no local changes that are uncommitted.
-1. *Fetch* the most recent global VCS tags from origin.
-2. Generate the updated version string.
-3. Replace version strings in all files configured in `file_patterns`.
-4. *Commit* the updated files.
-5. *Tag* the new commit.
-6. *Push* the new commit and tag.
+1. *Fetch* VCS tags from origin.
+2. Get most recent version.
+3. Generate the updated version string.
+4. Check that you have no local changes that are uncommitted.
+5. Replace version strings in all files configured in `file_patterns`.
+6. *Commit* the updated files.
+7. *Tag* the new commit.
+8. *Push* the new commit and tag.
 
 The configuration for these steps can be done with the following parameters:
 
-|    Parameter     |   Type   |               Description               |
-|------------------|----------|-----------------------------------------|
-| `commit_message` | string¹  | Template for commit message in step 4.  |
-| `commit`         | boolean  | Create a commit with all updated files. |
-| `tag`            | boolean² | Tag the newly created commit.           |
-| `push`           | boolean² | Push to the default remote.             |
+|    Parameter     |   Type   |                 Description                |
+|------------------|----------|--------------------------------------------|
+| `tag_scope`      | string   | Scope for the `current_version` in step 2. |
+| `commit_message` | string¹  | Template for commit message in step 6.     |
+| `tag_message`    | string¹  | Template for tag message in step 7.        |
+| `commit`         | boolean  | Create a commit with all updated files.    |
+| `tag`            | boolean² | Tag the newly created commit.              |
+| `push`           | boolean² | Push to the default remote.                |
 
 - ¹ Available placeholders for the `commit_message`: `{new_version}`, `{old_version}`, `{new_version_pep440}`, `{old_version_pep440}`
 - ² Requires `commit = True`
 
 An example configuration might look like this:
 
 ```ini
 [bumpver]
 ...
 commit_message = "bump version to {new_version}"
+tag_message = "{new_version}"
 commit = True
 tag = True
 push = True
 ```
 
 If everything looks OK, you can do `bumpver update`.
 
@@ -1068,15 +1083,15 @@
 In addition to the `commit_message` configuration, you can also override the string used as the the commit message template with the `-c/--commit-message=<TMPL>` parameter:
 
 ```shell
 $ bumpver update --tag final --commit-message 'bump version {old_version} -> {new_version} [ci-publish]' --verbose
 INFO    - Old Version: 2021.1005b0
 INFO    - New Version: 2021.1006
 INFO    - git commit --message 'bump version 2020.1005b0 -> 2021.1006 [ci-publish]'
-INFO    - git tag --annotate 2020.1006 --message 2020.1006
+INFO    - git tag --annotate 2020.1006 --message '2020.1006'
 INFO    - git push origin --follow-tags 2020.1006 HEAD
 ```
 
 As this is a manual operation (rather than a long lived configuration option), you can use the placeholders `OLD` and `NEW` for convenience, instead of the more verbose `{old_version}` and `{new_version}`.
 
 ```shell
 $ bumpver update -f -t final -c '[final-version] OLD -> NEW'
@@ -1084,12 +1099,39 @@
 INFO    - Old Version: 1.2.0b2
 INFO    - New Version: 1.2.0
 INFO    - git commit --message '[final-version] 1.2.0b2 -> 1.2.0'
 ...
 ```
 
 
+### Custom Tag Message
+
+Similarly to `--commit-message` you can provide a tag message template by using the `--tag-message=<TMPL>` parameter or the `tag_message` configuration:
+
+```shell
+$ bumpver update -f -t final --tag-message 'release NEW'
+INFO    - Old Version: 1.2.0b2
+INFO    - New Version: 1.2.0
+...
+INFO    - git tag --annotate 1.2.0 --message 'release 1.2.0'
+...
+```
+
+You can use the same placeholders as in the `--commit-message` template.
+
+If an empty tag message is provided, bumpver uses a lightweight tag in Git. Otherwise, it utilizes an annotated Git tag. You can read more about Git tagging [here](https://git-scm.com/book/en/v2/Git-Basics-Tagging).
+
+```shell
+$ bumpver update -f -t final --tag-message ''
+INFO    - Old Version: 1.2.0b2
+INFO    - New Version: 1.2.0
+...
+INFO    - git tag 1.2.0
+...
+```
+
+
 ## Contributors
 
 |                Name                 |    role           |  since  | until |
 |-------------------------------------|-------------------|---------|-------|
 | Manuel Barkhau (mbarkhau@gmail.com) | author/maintainer | 2018-09 | -     |
```

### Comparing `bumpver-2023.1124/fastentrypoints.py` & `bumpver-2023.1125/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/setup.cfg` & `bumpver-2023.1125/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-license_file = LICENSE
+license_files = LICENSE
 
 [bdist_wheel]
 universal = 1
 
 [mypy]
 check_untyped_defs = True
 disallow_untyped_calls = True
@@ -56,15 +56,15 @@
 	dist/
 	.mypy_cache
 
 [tool:pytest]
 addopts = --doctest-modules
 
 [bumpver]
-current_version = "2023.1124"
+current_version = "2023.1125"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump {old_version} -> {new_version}"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
```

### Comparing `bumpver-2023.1124/setup.py` & `bumpver-2023.1125/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 setuptools.setup(
     name="bumpver",
     license="MIT",
     author="Manuel Barkhau",
     author_email="mbarkhau@gmail.com",
     url="https://github.com/mbarkhau/bumpver",
-    version="2023.1124",
+    version="2023.1125",
     keywords="version bumpver calver semver versioning bumpversion pep440",
     description="Bump version numbers in project files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages("src"),
     package_dir=package_dir,
     install_requires=install_requires,
```

### Comparing `bumpver-2023.1124/src/bumpver/cli.py` & `bumpver-2023.1125/src/bumpver/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     import pretty_traceback
 
     pretty_traceback.install()
 except ImportError:
     pass  # no need to fail because of missing dev dependency
 
 
-click.disable_unicode_literals_warning = True  # type: ignore[attr-defined]
+click.disable_unicode_literals_warning = True
 
 logger = logging.getLogger("bumpver.cli")
 
 
 _VERBOSE = 0
 
 
@@ -249,15 +249,15 @@
     decorated = function
     for decorator in decorators:
         decorated = decorator(decorated)
     return decorated
 
 
 @click.group(context_settings={'help_option_names': ["-h", "--help"]})
-@click.version_option(version="2023.1124")
+@click.version_option(version="2023.1125")
 @verbose_option
 def cli(verbose: int = 0) -> None:
     """Automatically update version strings in plaintext files."""
     if verbose:
         _configure_logging(verbose=max(_VERBOSE, verbose))
 
 
@@ -269,15 +269,15 @@
 def test(
     old_version   : str,
     pattern       : str,
     verbose       : int = 0,
     major         : bool = False,
     minor         : bool = False,
     patch         : bool = False,
-    tag           : str = None,
+    tag           : typ.Optional[str] = None,
     tag_num       : bool = False,
     pin_increments: bool = False,
     pin_date      : bool = False,
     date          : typ.Optional[str] = None,
     set_version   : typ.Optional[str] = None,
 ) -> None:
     """Increment a version number for demo purposes."""
@@ -502,42 +502,60 @@
         logger.error(str(err))
         sys.exit(1)
     except rewrite.NoPatternMatch as ex:
         logger.error(str(ex))
         sys.exit(1)
 
 
-def _is_valid_version(raw_pattern: str, old_version: str, new_version: str) -> bool:
+def _parse_version_tags(
+    all_tags: typ.List[str], version_pattern: str, is_new_pattern: bool
+) -> typ.List[str]:
+    version_parser = v2version if is_new_pattern else v1version
+    return [tag for tag in all_tags if version_parser.is_valid(tag, version_pattern)]
+
+
+def _is_valid_version(
+    raw_pattern: str, old_version: str, new_version: str, unique: bool = False
+) -> bool:
     is_new_pattern = "{" not in raw_pattern and "}" not in raw_pattern
+
     try:
         if is_new_pattern:
             v2version.parse_version_info(new_version, raw_pattern)
         else:
             v1version.parse_version_info(new_version, raw_pattern)
     except version.PatternError:
         logger.error(f"Invalid version '{new_version}' for pattern '{raw_pattern}'")
         return False
 
     if version.parse_version(new_version) <= version.parse_version(old_version):
         logger.error("Invariant violated: New version must be greater than old version ")
         logger.error(f"  Failed Invariant: '{new_version}' > '{old_version}'")
         logger.error("If the invariant is from vcs tags try '--ignore-vcs-tag' option.")
         return False
-    else:
-        return True
+
+    if unique:
+        all_tags     = vcs.get_tags(fetch=False, scope=config.TagScope.GLOBAL)
+        version_tags = _parse_version_tags(all_tags, raw_pattern, is_new_pattern)
+
+        if new_version in version_tags:
+            logger.error("Invariant violated: New version must be unique accross all branches")
+            return False
+
+    return True
 
 
 def incr_dispatch(
     old_version: str,
     raw_pattern: str,
     *,
     major         : bool = False,
     minor         : bool = False,
     patch         : bool = False,
-    tag           : str = None,
+    tag           : typ.Optional[str] = None,
     tag_num       : bool = False,
     pin_increments: bool = False,
     pin_date      : bool = False,
     maybe_date    : typ.Optional[dt.date] = None,
 ) -> typ.Optional[str]:
     v1_parts    = list(v1patterns.PART_PATTERNS) + list(v1patterns.FULL_PART_FORMATS)
     has_v1_part = any("{" + part + "}" in raw_pattern for part in v1_parts)
@@ -578,14 +596,15 @@
         )
 
 
 def _update(
     cfg           : config.Config,
     new_version   : str,
     commit_message: str,
+    tag_message   : str,
     allow_dirty   : bool = False,
 ) -> None:
     vcs_api: typ.Optional[vcs.VCSAPI] = None
 
     if cfg.commit:
         try:
             vcs_api = vcs.get_vcs_api()
@@ -605,25 +624,26 @@
             new_v1_vinfo = v1version.parse_version_info(new_version, cfg.version_pattern)
             v1rewrite.rewrite_files(cfg.file_patterns, new_v1_vinfo)
     except rewrite.NoPatternMatch as ex:
         logger.error(str(ex))
         sys.exit(1)
 
     if vcs_api:
-        vcs.commit(cfg, vcs_api, filepaths, new_version, commit_message)
+        vcs.commit(cfg, vcs_api, filepaths, new_version, commit_message, tag_message)
 
 
 def _try_update(
     cfg           : config.Config,
     new_version   : str,
     commit_message: str,
+    tag_message   : str,
     allow_dirty   : bool = False,
 ) -> None:
     try:
-        _update(cfg, new_version, commit_message, allow_dirty)
+        _update(cfg, new_version, commit_message, tag_message, allow_dirty)
     except sp.CalledProcessError as ex:
         logger.error(f"Error running subcommand: {ex.cmd}")
         if ex.stdout:
             sys.stdout.write(ex.stdout.decode('utf-8'))
         if ex.stderr:
             sys.stderr.write(ex.stderr.decode('utf-8'))
         sys.exit(1)
@@ -648,54 +668,56 @@
         click.echo("\n    " + "\n    ".join(cfg_text.splitlines()))
         sys.exit(0)
 
     config.write_content(ctx)
 
 
 def get_latest_vcs_version_tag(cfg: config.Config, fetch: bool) -> typ.Optional[str]:
-    all_tags = vcs.get_tags(fetch=fetch)
-
-    if cfg.is_new_pattern:
-        version_tags = [tag for tag in all_tags if v2version.is_valid(tag, cfg.version_pattern)]
-    else:
-        version_tags = [tag for tag in all_tags if v1version.is_valid(tag, cfg.version_pattern)]
+    all_tags     = vcs.get_tags(fetch=fetch, scope=cfg.tag_scope)
+    version_tags = _parse_version_tags(all_tags, cfg.version_pattern, cfg.is_new_pattern)
 
     if version_tags:
         version_tags.sort(key=version.parse_version, reverse=True)
         _debug_tags = ", ".join(version_tags[:3])
         logger.debug(f"found tags: {_debug_tags} ... ({len(version_tags)} in total)")
         return version_tags[0]
     else:
         return None
 
 
 def _update_cfg_from_vcs(cfg: config.Config, fetch: bool) -> config.Config:
     latest_version_tag = get_latest_vcs_version_tag(cfg, fetch)
+
     if latest_version_tag is None:
         logger.debug("no vcs tags found")
         return cfg
-    else:
-        latest_version_pep440 = version.to_pep440(latest_version_tag)
+
+    latest_version_pep440 = version.to_pep440(latest_version_tag)
+
+    scope_str = f"({cfg.tag_scope.value})" if not cfg.tag_scope == config.TagScope.DEFAULT else ""
+    logger.info(f"Latest version from VCS tag: {latest_version_tag} {scope_str}")
+
+    if cfg.tag_scope == config.TagScope.DEFAULT:
+        logger.info(f"Working dir version        : {cfg.current_version}")
         if version.parse_version(latest_version_tag) <= version.parse_version(cfg.current_version):
             # current_version already newer/up-to-date
             return cfg
-        else:
-            logger.info(f"Working dir version        : {cfg.current_version}")
-            logger.info(f"Latest version from VCS tag: {latest_version_tag}")
-            return cfg._replace(
-                current_version=latest_version_tag,
-                pep440_version=latest_version_pep440,
-            )
+
+    return cfg._replace(
+        current_version=latest_version_tag,
+        pep440_version=latest_version_pep440,
+    )
 
 
 def _parse_vcs_options(
     cfg       : config.Config,
     commit    : typ.Optional[bool] = None,
     tag_commit: typ.Optional[bool] = None,
     push      : typ.Optional[bool] = None,
+    tag_scope : typ.Optional[str] = None,
 ) -> config.Config:
     if commit is False and tag_commit:
         raise ValueError("--no-commit and --tag-commit cannot be used at the same time")
     if commit is False and push:
         raise ValueError("--no-commit and --push cannot be used at the same time")
 
     if commit is not None:
@@ -706,17 +728,24 @@
     if not cfg.commit and push:
         raise ValueError("--push requires either --commit or commit=True in your config")
 
     if tag_commit is not None:
         cfg = cfg._replace(tag=tag_commit)
     if push is not None:
         cfg = cfg._replace(push=push)
+    if tag_scope is not None:
+        cfg = cfg._replace(tag_scope=config.TagScope(tag_scope))
+
     return cfg
 
 
+def _sub_msg_template(message: str) -> str:
+    return re.sub(r"\b(OLD|NEW)\b", r"{\1_VERSION}", message)
+
+
 @cli.command()
 @dry_option
 @fetch_option
 @verbose_option
 @click.option(
     "--allow-dirty",
     default=False,
@@ -738,28 +767,41 @@
     "-c",
     "--commit-message",
     default=None,
     metavar="<TMPL>",
     help="Set commit message template.",
 )
 @click.option(
+    "--tag-message",
+    default=None,
+    metavar="<TMPL>",
+    help="Set tag message template.",
+)
+@click.option(
     "--commit/--no-commit",
     default=None,
     help="Create a commit with all updated files.",
 )
 @click.option(
     "--tag-commit/--no-tag-commit",
     default=None,
     help="Tag the newly created commit.",
 )
 @click.option(
     "--push/--no-push",
     default=None,
     help="Push to the default remote.",
 )
+@click.option(
+    "--tag-scope",
+    default=None,
+    metavar="[default|global|branch]",
+    type=click.Choice([e.value for e in config.TagScope]),
+    help="Tag scope for the current version.",
+)
 def update(
     dry           : bool = False,
     allow_dirty   : bool = False,
     ignore_vcs_tag: bool = False,
     fetch         : bool = True,
     verbose       : int = 0,
     major         : bool = False,
@@ -768,32 +810,34 @@
     tag           : typ.Optional[str] = None,
     tag_num       : bool = False,
     pin_increments: bool = False,
     pin_date      : bool = False,
     date          : typ.Optional[str] = None,
     set_version   : typ.Optional[str] = None,
     commit_message: typ.Optional[str] = None,
+    tag_message   : typ.Optional[str] = None,
     commit        : typ.Optional[bool] = None,
     tag_commit    : typ.Optional[bool] = None,
     push          : typ.Optional[bool] = None,
+    tag_scope     : typ.Optional[str] = None,
 ) -> None:
     """Update project files with the incremented version string."""
     verbose = max(_VERBOSE, verbose)
     _configure_logging(verbose)
     _validate_release_tag(tag)
     maybe_date = _validate_date(date, pin_date)
 
     _, cfg = config.init(project_path=".")
 
     if cfg is None:
         logger.error("Could not parse configuration.")
         sys.exit(1)
 
     try:
-        cfg = _parse_vcs_options(cfg, commit, tag_commit, push)
+        cfg = _parse_vcs_options(cfg, commit, tag_commit, push, tag_scope)
     except ValueError as ex:
         logger.warning(f"Invalid argument: {ex}")
         sys.exit(1)
 
     if not ignore_vcs_tag:
         cfg = _update_cfg_from_vcs(cfg, fetch)
 
@@ -814,42 +858,49 @@
     else:
         new_version = set_version
 
     if new_version is None:
         _log_no_change('update', cfg.version_pattern)
         sys.exit(1)
 
-    if not _is_valid_version(cfg.version_pattern, old_version, new_version):
+    uniqueness_check = cfg.tag_scope == config.TagScope.BRANCH or set_version is not None
+
+    if not _is_valid_version(
+        cfg.version_pattern, old_version, new_version, unique=uniqueness_check
+    ):
         if set_version:
             logger.error(f"Invalid argument --set-version='{set_version}'")
-
         sys.exit(1)
 
     logger.info(f"Old Version: {old_version}")
     logger.info(f"New Version: {new_version}")
 
     if dry or verbose >= 2:
         _print_diff(cfg, new_version)
 
     if commit_message is None:
         commit_msg_template = cfg.commit_message
     else:
-        commit_msg_template, _ = re.subn(r"\b(OLD|NEW)\b", r"{\1_VERSION}", commit_message)
+        commit_msg_template = _sub_msg_template(commit_message)
 
-    commit_message_kwargs = {
+    tag_msg_template = cfg.tag_message if tag_message is None else _sub_msg_template(tag_message)
+
+    tag_and_commit_message_kwargs = {
         'new_version'       : new_version,
         'old_version'       : old_version,
         'NEW_VERSION'       : new_version,
         'OLD_VERSION'       : old_version,
         'new_version_pep440': version.to_pep440(new_version),
         'old_version_pep440': version.to_pep440(old_version),
     }
-    try_commit_message = commit_msg_template.format(**commit_message_kwargs)
+
+    try_commit_message = commit_msg_template.format(**tag_and_commit_message_kwargs)
+    try_tag_message    = tag_msg_template.format(**tag_and_commit_message_kwargs)
 
     if dry:
         return
 
-    _try_update(cfg, new_version, try_commit_message, allow_dirty)
+    _try_update(cfg, new_version, try_commit_message, try_tag_message, allow_dirty)
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `bumpver-2023.1124/src/bumpver/config.py` & `bumpver-2023.1125/src/bumpver/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # https://gitlab.com/mbarkhau/bumpver
 #
 # Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 """Parse bumpver.toml, setup.cfg or pyproject.toml files."""
 
 import re
+import enum
 import typing as typ
 import logging
 import datetime as dt
 import configparser
 
 import toml
 import pathlib2 as pl
@@ -29,15 +30,24 @@
 
 PatternsByFile   = typ.Dict[str, typ.List[Pattern]]
 FilePatternsItem = typ.Tuple[str, typ.List[Pattern]]
 
 
 SUPPORTED_CONFIGS = ["setup.cfg", "pyproject.toml", "pycalver.toml", "bumpver.toml"]
 
+
+class TagScope(str, enum.Enum):
+    DEFAULT = "default"
+    GLOBAL  = "global"
+    BRANCH  = "branch"
+
+
+DEFAULT_TAG_SCOPE      = TagScope.DEFAULT
 DEFAULT_COMMIT_MESSAGE = "bump version to {new_version}"
+DEFAULT_TAG_MESSAGE    = "{new_version}"
 
 
 class ProjectContext(typ.NamedTuple):
     """Container class for project info."""
 
     path           : pl.Path
     config_filepath: pl.Path
@@ -121,14 +131,16 @@
 class Config(typ.NamedTuple):
     """Container for parameters parsed from a config file."""
 
     current_version: str
     version_pattern: str
     pep440_version : str
     commit_message : str
+    tag_message    : str
+    tag_scope      : TagScope
 
     commit        : bool
     tag           : bool
     push          : bool
     is_new_pattern: bool
 
     file_patterns: PatternsByFile
@@ -140,14 +152,16 @@
 def _debug_str(cfg: Config) -> str:
     cfg_str_parts = [
         "Config Parsed: Config(",
         f"\n    current_version='{cfg.current_version}',",
         f"\n    version_pattern='{cfg.version_pattern}',",
         f"\n    pep440_version='{cfg.pep440_version}',",
         f"\n    commit_message='{cfg.commit_message}',",
+        f"\n    tag_message='{cfg.tag_message}',",
+        f"\n    tag_scope='{cfg.tag_scope.value}',",
         f"\n    commit={cfg.commit},",
         f"\n    tag={cfg.tag},",
         f"\n    push={cfg.push},",
         f"\n    is_new_pattern={cfg.is_new_pattern},",
         "\n    file_patterns={",
     ]
 
@@ -360,28 +374,35 @@
 
 def _parse_config(raw_cfg: RawConfig) -> Config:
     """Parse configuration which was loaded from an .ini/.cfg or .toml file."""
 
     commit_message: str = raw_cfg.get('commit_message', DEFAULT_COMMIT_MESSAGE)
     commit_message = raw_cfg['commit_message'] = commit_message.strip("'\" ")
 
+    tag_message: str = raw_cfg.get('tag_message', DEFAULT_TAG_MESSAGE)
+    tag_message = raw_cfg['tag_message'] = tag_message.strip("'\" ")
+
     current_version: str = raw_cfg['current_version']
     current_version = raw_cfg['current_version'] = current_version.strip("'\" ")
 
     version_pattern: str = raw_cfg['version_pattern']
     version_pattern = raw_cfg['version_pattern'] = version_pattern.strip("'\" ")
 
     is_new_pattern = "{" not in version_pattern and "}" not in version_pattern
 
     _validate_version_with_pattern(current_version, version_pattern, is_new_pattern)
 
     pep440_version = version.to_pep440(current_version)
 
     file_patterns = _compile_file_patterns(raw_cfg, is_new_pattern)
 
+    if 'tag_scope' in raw_cfg:
+        raw_cfg['tag_scope'] = raw_cfg['tag_scope'].strip("'\" ").lower()
+    tag_scope: TagScope = TagScope(raw_cfg.get('tag_scope', DEFAULT_TAG_SCOPE))
+
     commit = raw_cfg['commit']
     tag    = raw_cfg['tag']
     push   = raw_cfg['push']
 
     if tag is None:
         tag = raw_cfg['tag'] = False
     if push is None:
@@ -389,19 +410,24 @@
 
     if tag and not commit:
         raise ValueError("commit=True required if tag=True")
 
     if push and not commit:
         raise ValueError("commit=True required if push=True")
 
+    if tag_scope not in list(TagScope):
+        raise ValueError("invalid value for tag_scope")
+
     cfg = Config(
         current_version=current_version,
         version_pattern=version_pattern,
         pep440_version=pep440_version,
         commit_message=commit_message,
+        tag_message=tag_message,
+        tag_scope=tag_scope,
         commit=commit,
         tag=tag,
         push=push,
         is_new_pattern=is_new_pattern,
         file_patterns=file_patterns,
     )
     logger.debug(_debug_str(cfg))
@@ -496,14 +522,16 @@
 
 
 DEFAULT_CONFIGPARSER_BASE_TMPL = """
 [bumpver]
 current_version = "{initial_version}"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump version {{old_version}} -> {{new_version}}"
+tag_message = "{{new_version}}"
+tag_scope = "{default_tag_scope}"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
 """.lstrip()
 
@@ -536,27 +564,31 @@
 
 
 DEFAULT_PYPROJECT_TOML_BASE_TMPL = """
 [tool.bumpver]
 current_version = "{initial_version}"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump version {{old_version}} -> {{new_version}}"
+tag_message = "{{new_version}}"
+tag_scope = "{default_tag_scope}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 """.lstrip()
 
 
 DEFAULT_BUMPVER_TOML_BASE_TMPL = """
 [bumpver]
 current_version = "{initial_version}"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump version {{old_version}} -> {{new_version}}"
+tag_message = "{{new_version}}"
+tag_scope = "{default_tag_scope}"
 commit = true
 tag = true
 push = true
 
 [bumpver.file_patterns]
 """.lstrip()
 
@@ -639,15 +671,18 @@
             "setup.py"      : DEFAULT_TOML_SETUP_PY_STR,
             "README.rst"    : DEFAULT_TOML_README_RST_STR,
             "README.md"     : DEFAULT_TOML_README_MD_STR,
         }
     else:
         raise ValueError(f"Invalid config_format='{fmt}', must be either 'toml' or 'cfg'.")
 
-    cfg_str = base_tmpl.format(initial_version=_initial_version())
+    cfg_str = base_tmpl.format(
+        initial_version=_initial_version(),
+        default_tag_scope=DEFAULT_TAG_SCOPE.value,
+    )
 
     for filename, default_str in default_pattern_strs_by_filename.items():
         if (ctx.path / filename).exists():
             cfg_str += default_str
 
     has_config_file = any((ctx.path / fn).exists() for fn in SUPPORTED_CONFIGS)
```

### Comparing `bumpver-2023.1124/src/bumpver/parse.py` & `bumpver-2023.1125/src/bumpver/parse.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/src/bumpver/patterns.py` & `bumpver-2023.1125/src/bumpver/patterns.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/src/bumpver/pysix.py` & `bumpver-2023.1125/src/bumpver/pysix.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/src/bumpver/regexfmt.py` & `bumpver-2023.1125/src/bumpver/regexfmt.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/src/bumpver/rewrite.py` & `bumpver-2023.1125/src/bumpver/rewrite.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/src/bumpver/utils.py` & `bumpver-2023.1125/src/bumpver/utils.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/src/bumpver/v1patterns.py` & `bumpver-2023.1125/src/bumpver/v1patterns.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/src/bumpver/v1rewrite.py` & `bumpver-2023.1125/src/bumpver/v1rewrite.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/src/bumpver/v1version.py` & `bumpver-2023.1125/src/bumpver/v1version.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         vnfo.dom,
         vnfo.doy,
         vnfo.iso_week,
         vnfo.us_week,
     )
 
 
-def cal_info(date: dt.date = None) -> version.V1CalendarInfo:
+def cal_info(date: typ.Optional[dt.date] = None) -> version.V1CalendarInfo:
     """Generate calendar components for current date.
 
     >>> from datetime import date
 
     >>> c = cal_info(date(2019, 1, 5))
     >>> (c.year, c.quarter, c.month, c.dom, c.doy, c.iso_week, c.us_week)
     (2019, 1, 1, 5, 5, 0, 0)
```

### Comparing `bumpver-2023.1124/src/bumpver/v2patterns.py` & `bumpver-2023.1125/src/bumpver/v2patterns.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/src/bumpver/v2rewrite.py` & `bumpver-2023.1125/src/bumpver/v2rewrite.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/src/bumpver/v2version.py` & `bumpver-2023.1125/src/bumpver/v2version.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         if not (lval is None or rval is None):
             lvals.append(lval)
             rvals.append(rval)
 
     return lvals > rvals
 
 
-def cal_info(date: dt.date = None) -> version.V2CalendarInfo:
+def cal_info(date: typ.Optional[dt.date] = None) -> version.V2CalendarInfo:
     """Generate calendar components for current date.
 
     >>> import datetime as dt
 
     >>> c = cal_info(dt.date(2019, 1, 5))
     >>> (c.year_y, c.quarter, c.month, c.dom, c.doy, c.week_w, c.week_u, c.week_v)
     (2019, 1, 1, 5, 5, 0, 0, 1)
```

### Comparing `bumpver-2023.1124/src/bumpver/vcs.py` & `bumpver-2023.1125/src/bumpver/vcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,53 +40,59 @@
 """
 
 BRANCH_RE = re.compile(BRANCH_PATTERN, flags=re.VERBOSE)
 
 
 VCS_SUBCOMMANDS_BY_NAME = {
     'git': {
-        'is_usable'   : "git rev-parse --git-dir",
-        'fetch'       : "git fetch",
-        'ls_tags'     : "git tag --list",
-        'status'      : "git status --porcelain",
-        'add_path'    : "git add --update '{path}'",
-        'commit'      : "git commit --message '{message}'",
-        'tag'         : "git tag --annotate {tag} --message {tag}",
-        'push_tag'    : "git push {remote} --follow-tags {tag} HEAD",
-        'show_remotes': "git config --get remote.origin.url",
-        'ls_branches' : "git branch -vv",
+        'is_usable'     : "git rev-parse --git-dir",
+        'fetch'         : "git fetch",
+        'ls_tags'       : "git tag --list",
+        'ls_tags_branch': "git tag --list --merged",
+        'status'        : "git status --porcelain",
+        'add_path'      : "git add --update '{path}'",
+        'commit'        : "git commit --message '{message}'",
+        'tag'           : "git tag --annotate {tag} --message '{message}'",
+        'tag_light'     : "git tag {tag}",
+        'push_tag'      : "git push {remote} --follow-tags {tag} HEAD",
+        'push'          : "git push {remote} HEAD",
+        'show_remotes'  : "git config --get remote.origin.url",
+        'ls_branches'   : "git branch -vv",
     },
     'hg': {
-        'is_usable'   : "hg root",
-        'fetch'       : "hg pull",
-        'ls_tags'     : "hg tags",
-        'status'      : "hg status -umard",
-        'add_path'    : "hg add {path}",
-        'commit'      : "hg commit --logfile {path}",
-        'tag'         : "hg tag {tag} --message {tag}",
-        'push_tag'    : "hg push {tag}",
-        'show_remotes': "hg paths",
+        'is_usable'     : "hg root",
+        'fetch'         : "hg pull",
+        'ls_tags'       : "hg tags",
+        'ls_tags_branch': "hg log --branch . --rev='tag()' --template='{{tags}}\\n'",
+        'status'        : "hg status -umard",
+        'add_path'      : "hg add '{path}'",
+        'commit'        : "hg commit --logfile '{path}'",
+        'tag'           : "hg tag {tag} --message '{message}'",
+        'tag_light'     : "hg tag {tag}",
+        'push_tag'      : "hg push {tag}",
+        'push'          : "hg push",
+        'show_remotes'  : "hg paths",
     },
 }
 
 
 Env = typ.Dict[str, str]
 
 
 class VCSAPI:
     """Absraction for git and mercurial."""
 
-    def __init__(self, name: str, subcommands: typ.Dict[str, str] = None):
+    def __init__(self, name: str, subcommands: typ.Optional[typ.Dict[str, str]] = None):
         self.name = name
         if subcommands is None:
             self.subcommands = VCS_SUBCOMMANDS_BY_NAME[name]
         else:
             self.subcommands = subcommands
 
-    def __call__(self, cmd_name: str, env: Env = None, **kwargs: str) -> str:
+    def __call__(self, cmd_name: str, env: typ.Optional[Env] = None, **kwargs: str) -> str:
         """Invoke subcommand and return output."""
         cmd_tmpl = self.subcommands[cmd_name]
         cmd_str  = cmd_tmpl.format(**kwargs)
         if cmd_name in ("commit", "tag", "push_tag"):
             logger.info(cmd_str)
         else:
             logger.debug(cmd_str)
@@ -150,14 +156,20 @@
 
     def ls_tags(self) -> typ.List[str]:
         """List vcs tags on all branches."""
         ls_tag_lines = self('ls_tags').splitlines()
         logger.debug(f"ls_tags output {ls_tag_lines}")
         return [line.strip().split(" ", 1)[0] for line in ls_tag_lines]
 
+    def ls_tags_branch(self) -> typ.List[str]:
+        """List vcs tags on all branches."""
+        ls_tag_lines = self('ls_tags_branch').splitlines()
+        logger.debug(f"ls_tags_branch output {ls_tag_lines}")
+        return [line.strip().split(" ", 1)[0] for line in ls_tag_lines]
+
     def add(self, path: str) -> None:
         """Add updates to be included in next commit."""
         try:
             self('add_path', path=path)
         except sp.CalledProcessError as ex:
             if "already tracked!" in str(ex):
                 # mercurial
@@ -187,24 +199,35 @@
                     fobj.write(message_data)
 
                 env['HGENCODING'] = "utf-8"
                 self('commit', env=env, path=tmp_file.name)
             finally:
                 os.unlink(tmp_file.name)
 
-    def tag(self, tag_name: str) -> None:
-        """Create an annotated tag."""
-        self('tag', tag=tag_name)
+    def tag(self, tag_name: str, tag_message: str) -> None:
+        """Create a tag."""
+        if tag_message:
+            # Annotated
+            self('tag', tag=tag_name, message=tag_message)
+        else:
+            # Lightweight
+            self('tag_light', tag=tag_name)
 
-    def push(self, tag_name: str) -> None:
+    def push_tag(self, tag_name: str) -> None:
         """Push changes to origin."""
         remote = self.get_remote()
         if remote:
             self('push_tag', tag=tag_name, remote=remote)
 
+    def push(self) -> None:
+        """Push changes to origin."""
+        remote = self.get_remote()
+        if remote:
+            self('push', remote=remote)
+
     def __repr__(self) -> str:
         """Generate string representation."""
         return f"VCSAPI(name='{self.name}')"
 
 
 def get_vcs_api() -> VCSAPI:
     """Detect the appropriate VCS for a repository.
@@ -243,32 +266,43 @@
 
 def commit(
     cfg           : config.Config,
     vcs_api       : VCSAPI,
     filepaths     : typ.Set[str],
     new_version   : str,
     commit_message: str,
+    tag_message   : str,
 ) -> None:
     if cfg.commit:
         for filepath in filepaths:
             vcs_api.add(filepath)
 
         vcs_api.commit(commit_message)
 
     if cfg.commit and cfg.tag:
-        vcs_api.tag(new_version)
+        vcs_api.tag(tag_name=new_version, tag_message=tag_message)
 
     if cfg.commit and cfg.push:
-        vcs_api.push(new_version)
+        if cfg.tag:
+            vcs_api.push_tag(tag_name=new_version)
+        else:
+            vcs_api.push()
 
 
-def get_tags(fetch: bool) -> typ.List[str]:
+def get_tags(fetch: bool, scope: config.TagScope) -> typ.List[str]:
     try:
         vcs_api = get_vcs_api()
         logger.debug(f"vcs found: {vcs_api.name}")
+
         if fetch:
             logger.info("fetching tags from remote (to turn off use: -n / --no-fetch)")
             vcs_api.fetch()
-        return vcs_api.ls_tags()
+
+        branch_scope = scope == config.TagScope.BRANCH
+
+        if branch_scope:
+            return vcs_api.ls_tags_branch()
+        else:
+            return vcs_api.ls_tags()
     except OSError:
         logger.debug("No vcs found")
         return []
```

### Comparing `bumpver-2023.1124/src/bumpver/version.py` & `bumpver-2023.1125/src/bumpver/version.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/src/bumpver.egg-info/PKG-INFO` & `bumpver-2023.1125/src/bumpver.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bumpver
-Version: 2023.1124
+Version: 2023.1125
 Summary: Bump version numbers in project files.
 Home-page: https://github.com/mbarkhau/bumpver
 Author: Manuel Barkhau
 Author-email: mbarkhau@gmail.com
 License: MIT
 Keywords: version bumpver calver semver versioning bumpversion pep440
 Classifier: Development Status :: 4 - Beta
@@ -47,15 +47,15 @@
 [url_calver_org]: https://calver.org/
 
 
 Project/Repo:
 
 [![MIT License][img_license]][url_license]
 [![Supported Python Versions][img_pyversions]][url_pyversions]
-[![CalVer 2023.1124][img_version]][url_version]
+[![CalVer 2023.1125][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
 [![PyPI Downloads][img_downloads]][url_downloads]
 
 Code Quality/CI:
 
 [![GitHub Build Status][img_github_build]][url_github_build]
 [![GitLab Build Status][img_gitlab_build]][url_gitlab_build]
@@ -81,15 +81,15 @@
 
 [img_style]: https://img.shields.io/badge/code%20style-%20sjfmt-f71.svg
 [url_style]: https://gitlab.com/mbarkhau/straitjacket/
 
 [img_downloads]: https://pepy.tech/badge/bumpver/month
 [url_downloads]: https://pepy.tech/project/bumpver
 
-[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2023.1124&color=blue
+[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2023.1125&color=blue
 [url_version]: https://pypi.org/project/bumpver/
 
 [img_pypi]: https://img.shields.io/badge/PyPI-wheels-green.svg
 [url_pypi]: https://pypi.org/project/bumpver/#files
 
 [img_pyversions]: https://img.shields.io/pypi/pyversions/bumpver.svg
 [url_pyversions]: https://pypi.python.org/pypi/bumpver
@@ -445,15 +445,15 @@
 
 #### Add git hash to version string
 
 If you want to build a package straight from your git repository,
 without making a release first, you can explictly add git hash to
 the version number using ``GITHASH`` version part.
 
-Let's say your ``setup.cfg`` looks like this: 
+Let's say your ``setup.cfg`` looks like this:
 
 ```ini
 [bumpver]
 ...
 version_pattern = "YYYY.BUILD[-TAG][GITHASH]"
 ...
 ```
@@ -631,30 +631,33 @@
                                   uncomitted changes. (WARNING: The commit
                                   will still be aborted if there are
                                   uncomitted to files with version strings.
   --ignore-vcs-tag                Ignore VCS tag invariant and update version
                                   anyway.
   --set-version <VERSION>         Set version explicitly.
   --date <ISODATE>                Set explicit date in format YYYY-0M-0D (e.g.
-                                  2023-05-18).
+                                  2023-07-10).
   --pin-date                      Leave date components unchanged.
   --pin-increments                Leave the auto-increments INC0 and INC1
                                   unchanged.
   --tag-num                       Increment release tag number (rc1, rc2,
                                   rc3..).
   -t, --tag <NAME>                Override release tag of current_version.
                                   Valid options are: alpha, beta, dev, rc,
                                   post, final.
   -p, --patch                     Increment PATCH component.
   -m, --minor                     Increment MINOR component.
   --major                         Increment MAJOR component.
   -c, --commit-message <TMPL>     Set commit message template.
+  --tag-message <TMPL>            Set tag message template.
   --commit / --no-commit          Create a commit with all updated files.
   --tag-commit / --no-tag-commit  Tag the newly created commit.
   --push / --no-push              Push to the default remote.
+  --tag-scope [default|global|branch]
+                                  Tag scope for the current version.
   -h, --help                      Show this message and exit.
 ```
 
 <!-- END bumpver update --help -->
 
 To help with shell script automation, you can use `bumpver show --env`.
 
@@ -826,26 +829,28 @@
 
 The create an initial configuration for project with `bumpver init`.
 
 ```shell
 $ pip install bumpver
 ...
 Installing collected packages: click toml lexid bumpver
-Successfully installed bumpver-2023.1124
+Successfully installed bumpver-2023.1125
 
 $ cd myproject
 ~/myproject/
 
 $ bumpver init --dry
 Exiting because of '-d/--dry'. Would have written to bumpver.toml:
 
     [bumpver]
     current_version = "2020.1001a0"
     version_pattern = "YYYY.BUILD[PYTAGNUM]"
     commit_message = "bump version to {new_version}"
+    tag_message = "{new_version}"
+    tag_scope = "default"
     commit = true
     tag = true
     push = true
 
     [bumpver.file_patterns]
     "README.md" = [
         "{version}",
@@ -867,14 +872,16 @@
 Your `setup.cfg` may now look something like this:
 
 ```ini
 [bumpver]
 current_version = "2019.1001-alpha"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump version to {new_version}"
+tag_message = "{new_version}"
+tag_scope = "default"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
 setup.cfg =
     current_version = "{version}"
@@ -951,25 +958,29 @@
 ## Bump It Up
 
 
 ### Version State
 
 The `current_version` is considered global state and must be stored somewhere. Typically this might be in a `VERSION` file, or some other file which is part of the repository. This creates the risk that parallel branches can have different states. If the `current_version`  were defined only by files in the local checkout, the same version might be generated on different systems for different commits.
 
-To avoid this issue, `bumpver` treats Git/Mercurial tags as the canonical / [SSOT][url_ssot] for the most recent version and attempts to change this state in the most atomic way possible. This is why some actions of the `bumpver` command can take a few seconds, as it is synchronizing with the remote repository to get the most recent versions and to push any new version tags as soon as possible.
-
-[url_ssot]: https://en.wikipedia.org/wiki/Single_source_of_truth
+To avoid this issue, `bumpver` treats Git/Mercurial tags as a second source, depending on the `tag_scope` option, for the most recent version and attempts to change this state in the most atomic way possible. This is why some actions of the `bumpver` command can take a few seconds, as it is synchronizing with the remote repository to get the most recent versions and to push any new version tags as soon as possible.
 
 
 ### The Current Version
 
-The current version is either
+The current version depends on the configured `tag_scope` and is either
+
+| `tag_scope =` |	`current_version =`                                 |
+|---------------|-----------------------------------------------------|
+| `default`     |	`max(config.current_version, max(global_vcs_tags))` |
+| `global`      | `max(global_vcs_tags)`                              |
+| `branch`      | `max(branch_vcs_tags)`                              |
 
- - Typically: The largest Git/Mercurial tag which matches the `version_pattern` from your config, sorted using [`pkg_resources.parse_version`][url_setuptools_pkg_resources].
- - Rarely: Before any tags have been created, the value of `current_version` in `bumpver.toml` / `setup.cfg` / `pyproject.toml`.
+- Before any tags have been created `bumpver` will always default to the value of `current_version` in `bumpver.toml` / `setup.cfg` / `pyproject.toml`.
+- Only Git/Mercurial tags which matches the `version_pattern` from your config will be considered and sorted using [`pkg_resources.parse_version`][url_setuptools_pkg_resources].
 
 [url_setuptools_pkg_resources]: https://setuptools.readthedocs.io/en/latest/pkg_resources.html#parsing-utilities
 
 As part of doing `bumpver update` and `bumpver show`, your local tags are updated using `git fetch --tags`/`hg pull`.
 
 ```shell
 $ bumpver show -vv
@@ -1033,40 +1044,44 @@
 ```
 
 
 ### VCS Parameters (git/mercurial)
 
 The individual steps performed by `bumpver update`:
 
-0. Check that you have no local changes that are uncommitted.
-1. *Fetch* the most recent global VCS tags from origin.
-2. Generate the updated version string.
-3. Replace version strings in all files configured in `file_patterns`.
-4. *Commit* the updated files.
-5. *Tag* the new commit.
-6. *Push* the new commit and tag.
+1. *Fetch* VCS tags from origin.
+2. Get most recent version.
+3. Generate the updated version string.
+4. Check that you have no local changes that are uncommitted.
+5. Replace version strings in all files configured in `file_patterns`.
+6. *Commit* the updated files.
+7. *Tag* the new commit.
+8. *Push* the new commit and tag.
 
 The configuration for these steps can be done with the following parameters:
 
-|    Parameter     |   Type   |               Description               |
-|------------------|----------|-----------------------------------------|
-| `commit_message` | string¹  | Template for commit message in step 4.  |
-| `commit`         | boolean  | Create a commit with all updated files. |
-| `tag`            | boolean² | Tag the newly created commit.           |
-| `push`           | boolean² | Push to the default remote.             |
+|    Parameter     |   Type   |                 Description                |
+|------------------|----------|--------------------------------------------|
+| `tag_scope`      | string   | Scope for the `current_version` in step 2. |
+| `commit_message` | string¹  | Template for commit message in step 6.     |
+| `tag_message`    | string¹  | Template for tag message in step 7.        |
+| `commit`         | boolean  | Create a commit with all updated files.    |
+| `tag`            | boolean² | Tag the newly created commit.              |
+| `push`           | boolean² | Push to the default remote.                |
 
 - ¹ Available placeholders for the `commit_message`: `{new_version}`, `{old_version}`, `{new_version_pep440}`, `{old_version_pep440}`
 - ² Requires `commit = True`
 
 An example configuration might look like this:
 
 ```ini
 [bumpver]
 ...
 commit_message = "bump version to {new_version}"
+tag_message = "{new_version}"
 commit = True
 tag = True
 push = True
 ```
 
 If everything looks OK, you can do `bumpver update`.
 
@@ -1097,15 +1112,15 @@
 In addition to the `commit_message` configuration, you can also override the string used as the the commit message template with the `-c/--commit-message=<TMPL>` parameter:
 
 ```shell
 $ bumpver update --tag final --commit-message 'bump version {old_version} -> {new_version} [ci-publish]' --verbose
 INFO    - Old Version: 2021.1005b0
 INFO    - New Version: 2021.1006
 INFO    - git commit --message 'bump version 2020.1005b0 -> 2021.1006 [ci-publish]'
-INFO    - git tag --annotate 2020.1006 --message 2020.1006
+INFO    - git tag --annotate 2020.1006 --message '2020.1006'
 INFO    - git push origin --follow-tags 2020.1006 HEAD
 ```
 
 As this is a manual operation (rather than a long lived configuration option), you can use the placeholders `OLD` and `NEW` for convenience, instead of the more verbose `{old_version}` and `{new_version}`.
 
 ```shell
 $ bumpver update -f -t final -c '[final-version] OLD -> NEW'
@@ -1113,23 +1128,64 @@
 INFO    - Old Version: 1.2.0b2
 INFO    - New Version: 1.2.0
 INFO    - git commit --message '[final-version] 1.2.0b2 -> 1.2.0'
 ...
 ```
 
 
+### Custom Tag Message
+
+Similarly to `--commit-message` you can provide a tag message template by using the `--tag-message=<TMPL>` parameter or the `tag_message` configuration:
+
+```shell
+$ bumpver update -f -t final --tag-message 'release NEW'
+INFO    - Old Version: 1.2.0b2
+INFO    - New Version: 1.2.0
+...
+INFO    - git tag --annotate 1.2.0 --message 'release 1.2.0'
+...
+```
+
+You can use the same placeholders as in the `--commit-message` template.
+
+If an empty tag message is provided, bumpver uses a lightweight tag in Git. Otherwise, it utilizes an annotated Git tag. You can read more about Git tagging [here](https://git-scm.com/book/en/v2/Git-Basics-Tagging).
+
+```shell
+$ bumpver update -f -t final --tag-message ''
+INFO    - Old Version: 1.2.0b2
+INFO    - New Version: 1.2.0
+...
+INFO    - git tag 1.2.0
+...
+```
+
+
 ## Contributors
 
 |                Name                 |    role           |  since  | until |
 |-------------------------------------|-------------------|---------|-------|
 | Manuel Barkhau (mbarkhau@gmail.com) | author/maintainer | 2018-09 | -     |
 
 
 # Changelog for https://github.com/mbarkhau/bumpver
 
+## BumpVer 2023.1125
+
+- Add [#188][gh_i188]: Add `--tag-scope=<SCOPE>` to support separate versioning for branches.
+- Add [#185][gh_i185]: Add `--tag-message=<TMPL>` parameter and `tag_message` configuration option.
+- Fix [#209][gh_i209]: Make `--no-tag-commit` ommit `--follow-tags`.
+
+[gh_i188]: https://github.com/mbarkhau/bumpver/issues/188
+[gh_i185]: https://github.com/mbarkhau/bumpver/issues/185
+[gh_i209]: https://github.com/mbarkhau/bumpver/issues/209
+
+Thank you [Sven Lohrmann](https://github.com/malnvenshorn) for your contributions.
+Thank you [tardis4500](https://github.com/tardis4500) for the issue report.
+
+
 ## BumpVer 2023.1124
 
 - Fix [#208][gh_i208]: Fix handling of versions with PEP440 epoch.
 
 [gh_i208]: https://github.com/mbarkhau/bumpver/issues/208
 
 Thank you [Wen Kokke](https://github.com/wenkokke) for the issue report.
```

### Comparing `bumpver-2023.1124/src/bumpver.egg-info/SOURCES.txt` & `bumpver-2023.1125/src/bumpver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/test/test_cli.py` & `bumpver-2023.1125/test/test_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -343,15 +343,16 @@
     assert result.exit_code == 0
 
     assert os.path.exists("bumpver.toml")
     with pl.Path("bumpver.toml").open(mode="r", encoding="utf-8") as fobj:
         cfg_content = fobj.read()
 
     base_str = config.DEFAULT_BUMPVER_TOML_BASE_TMPL.format(
-        initial_version=config._initial_version()
+        initial_version=config._initial_version(),
+        default_tag_scope=config.DEFAULT_TAG_SCOPE.value,
     )
     assert base_str                          in cfg_content
     assert config.DEFAULT_TOML_README_MD_STR in cfg_content
 
     result = runner.invoke(cli.cli, ['show', "-vv"])
     _debug_records(caplog)
     assert result.exit_code == 0
@@ -374,15 +375,16 @@
     result = runner.invoke(cli.cli, ['init', "-vv"])
     assert result.exit_code == 0
 
     with pl.Path("setup.cfg").open(mode="r", encoding="utf-8") as fobj:
         cfg_content = fobj.read()
 
     base_str = config.DEFAULT_CONFIGPARSER_BASE_TMPL.format(
-        initial_version=config._initial_version()
+        initial_version=config._initial_version(),
+        default_tag_scope=config.DEFAULT_TAG_SCOPE.value,
     )
     assert base_str                                  in cfg_content
     assert config.DEFAULT_CONFIGPARSER_README_MD_STR in cfg_content
 
     result = runner.invoke(cli.cli, ['show', "-vv"])
     assert result.exit_code == 0
     assert f"Current Version: {config._initial_version()}\n" in result.output
@@ -413,15 +415,16 @@
     _debug_records(caplog)
     assert result.exit_code == 0
 
     with pl.Path("pyproject.toml").open(mode="r", encoding="utf-8") as fobj:
         cfg_content = fobj.read()
 
     base_str = config.DEFAULT_PYPROJECT_TOML_BASE_TMPL.format(
-        initial_version=config._initial_version()
+        initial_version=config._initial_version(),
+        default_tag_scope=config.DEFAULT_TAG_SCOPE.value,
     )
     assert base_str                          in cfg_content
     assert config.DEFAULT_TOML_README_MD_STR in cfg_content
 
     result = runner.invoke(cli.cli, ['show'])
     assert result.exit_code == 0
     assert f"Current Version: {config._initial_version()}\n" in result.output
@@ -1140,14 +1143,192 @@
 
     commits = shell(*shlex.split("git log -l 2")).decode("utf-8").split("\n\n")
 
     expected = "my custom message (v2019.1001-alpha -> v2019.1002-beta)"
     assert expected in commits[1]
 
 
+def test_hg_tag_message(runner, caplog):
+    _add_project_files("README.md", "setup.cfg")
+    result = runner.invoke(cli.cli, ['init', "-vv"])
+    assert result.exit_code == 0
+
+    tag_message = """
+    "bump: {old_version} ({old_version_pep440}) -> {new_version} ({new_version_pep440})"
+    """
+
+    _update_config_val(
+        "setup.cfg",
+        current_version='"v2019.1001-alpha"',
+        version_pattern="vYYYY.BUILD[-TAG]",
+        tag_message=tag_message.strip(),
+    )
+
+    _vcs_init("hg", ["README.md", "setup.cfg"])
+    assert len(caplog.records) > 0
+
+    cmd = [
+        'update',
+        "-vv",
+        "--pin-date",
+        "--tag",
+        "beta",
+    ]
+
+    result = runner.invoke(cli.cli, cmd)
+    assert result.exit_code == 0
+
+    tags = shell("hg", "tags").decode("utf-8")
+
+    expected_tag = "v2019.1002-beta"
+    assert expected_tag in tags
+
+    latest_changeset = shell("hg", "log", "-l", "1").decode("utf-8")
+
+    expected_message = "bump: v2019.1001-alpha (2019.1001a0) -> v2019.1002-beta (2019.1002b0)"
+    assert expected_message in latest_changeset.split("summery:", 1)[-1]
+
+
+def test_git_tag_message_annotated(runner, caplog):
+    _add_project_files("README.md", "setup.cfg")
+    result = runner.invoke(cli.cli, ['init', "-vv"])
+    assert result.exit_code == 0
+
+    tag_message = """
+    "bump: {old_version} ({old_version_pep440}) -> {new_version} ({new_version_pep440})"
+    """
+
+    _update_config_val(
+        "setup.cfg",
+        current_version='"v2019.1001-alpha"',
+        version_pattern="vYYYY.BUILD[-TAG]",
+        tag_message=tag_message.strip(),
+    )
+
+    _vcs_init("git", ["README.md", "setup.cfg"])
+    assert len(caplog.records) > 0
+
+    cmd = [
+        'update',
+        "-vv",
+        "--pin-date",
+        "--tag",
+        "beta",
+    ]
+
+    result = runner.invoke(cli.cli, cmd)
+    assert result.exit_code == 0
+
+    tags = shell("git", "tag", "--list").decode("utf-8")
+
+    expected_tag = "v2019.1002-beta"
+    assert expected_tag in tags
+
+    objecttype = (
+        shell("git", "tag", "--list", expected_tag, "--format=%(objecttype)")
+        .decode("utf-8")
+        .strip()
+    )
+
+    expected_type = "tag"
+    assert objecttype == expected_type
+
+    message = (
+        shell("git", "tag", "--list", expected_tag, "--format=%(contents:subject)")
+        .decode("utf-8")
+        .strip()
+    )
+
+    expected_message = "bump: v2019.1001-alpha (2019.1001a0) -> v2019.1002-beta (2019.1002b0)"
+    assert expected_message == message
+
+
+def test_git_tag_message_lightweight(runner, caplog):
+    _add_project_files("README.md", "setup.cfg")
+    result = runner.invoke(cli.cli, ['init', "-vv"])
+    assert result.exit_code == 0
+
+    _update_config_val(
+        "setup.cfg",
+        current_version='"v2019.1001-alpha"',
+        version_pattern="vYYYY.BUILD[-TAG]",
+        tag_message='""',
+    )
+
+    _vcs_init("git", ["README.md", "setup.cfg"])
+    assert len(caplog.records) > 0
+
+    cmd = [
+        'update',
+        "-vv",
+        "--pin-date",
+        "--tag",
+        "beta",
+    ]
+
+    result = runner.invoke(cli.cli, cmd)
+    assert result.exit_code == 0
+
+    tags = shell("git", "tag", "--list").decode("utf-8")
+
+    expected_tag = "v2019.1002-beta"
+    assert expected_tag in tags
+
+    objecttype = (
+        shell("git", "tag", "--list", expected_tag, "--format=%(objecttype)")
+        .decode("utf-8")
+        .strip()
+    )
+
+    expected_type = "commit"
+    assert objecttype == expected_type
+
+
+def test_cli_tag_message(runner, caplog):
+    _add_project_files("README.md", "setup.cfg")
+    result = runner.invoke(cli.cli, ['init', "-vv"])
+    assert result.exit_code == 0
+
+    _update_config_val(
+        "setup.cfg",
+        current_version='"v2019.1001-alpha"',
+        version_pattern="vYYYY.BUILD[-TAG]",
+    )
+
+    _vcs_init("git", ["README.md", "setup.cfg"])
+    assert len(caplog.records) > 0
+
+    cmd = [
+        'update',
+        "-vv",
+        "--pin-date",
+        "--tag",
+        "beta",
+        "--tag-message",
+        "my custom message (OLD -> NEW)",
+    ]
+
+    result = runner.invoke(cli.cli, cmd)
+    assert result.exit_code == 0
+
+    tags = shell("git", "tag", "--list").decode("utf-8")
+
+    expected_tag = "v2019.1002-beta"
+    assert expected_tag in tags
+
+    message = (
+        shell("git", "tag", "--list", expected_tag, "--format=%(contents:subject)")
+        .decode("utf-8")
+        .strip()
+    )
+
+    expected_message = "my custom message (v2019.1001-alpha -> v2019.1002-beta)"
+    assert expected_message == message
+
+
 def test_grep(runner):
     _add_project_files("README.md")
 
     search_re = r"^\s+2:\s+Hello World v2017\.1002-alpha !"
 
     cmd1    = r'grep "vYYYY.BUILD[-TAG]" README.md'
     result1 = runner.invoke(cli.cli, shlex.split(cmd1))
@@ -1268,48 +1449,83 @@
     new_version = cli.incr_dispatch(old_version, raw_pattern=version_pattern, **kwargs)
     if new_version is None:
         assert expected is None
     else:
         assert new_version == expected
 
 
-def test_get_latest_vcs_version_tag(runner):
+VCS_VERSION_TAG_CASES = [
+    ("git", None, "0.2.1"),
+    ("git", config.TagScope.GLOBAL, "0.2.1"),
+    ("git", config.TagScope.BRANCH, "0.1.10"),
+    ("git", config.TagScope.DEFAULT, "0.2.1"),
+    ("hg", None, "0.2.1"),
+    ("hg", config.TagScope.GLOBAL, "0.2.1"),
+    ("hg", config.TagScope.BRANCH, "0.1.10"),
+    ("hg", config.TagScope.DEFAULT, "0.2.1"),
+]
+
+
+@pytest.mark.parametrize("vcs_name, tag_scope, expected_version", VCS_VERSION_TAG_CASES)
+def test_get_latest_vcs_version_tag(runner, vcs_name, tag_scope, expected_version):
     result = runner.invoke(cli.cli, ['init', "-vv"])
     assert result.exit_code == 0
 
     _update_config_val("bumpver.toml", push="false")
     _update_config_val("bumpver.toml", current_version='"0.1.8"')
-    _update_config_val("bumpver.toml", version_pattern='"MAJOR.MINOR.PATCH"')
+    _update_config_val("bumpver.toml", version_pattern='"MAJOR.MINOR.PATCH[PYTAGNUM]"')
+
+    if tag_scope is not None:
+        _update_config_val("bumpver.toml", tag_scope=f'"{tag_scope.value}"')
 
-    _vcs_init("git", files=["bumpver.toml"])
+    _vcs_init(vcs_name, files=["bumpver.toml"])
 
     result = runner.invoke(cli.cli, ['update', "--patch"])
     assert result.exit_code == 0
 
     _, cfg = config.init()
     latest_version = cli.get_latest_vcs_version_tag(cfg, fetch=False)
     assert latest_version == "0.1.9"
 
-    result = runner.invoke(cli.cli, ['update', "--patch"])
+    if vcs_name == 'git':
+        shell("git", "branch", "dev")
+        shell("git", "checkout", "dev")
+    else:
+        shell("hg", "branch", "dev")
+
+    result = runner.invoke(cli.cli, ['update', "--minor", "--tag=beta"])
+    assert result.exit_code == 0
+
+    _, cfg = config.init()
+    latest_version = cli.get_latest_vcs_version_tag(cfg, fetch=False)
+    assert latest_version == "0.2.0b0"
+
+    if vcs_name == 'git':
+        shell("git", "checkout", "master")
+    else:
+        shell("hg", "update", "default")
+
+    result = runner.invoke(cli.cli, ['update', "--patch", "--tag=final"])
     assert result.exit_code == 0
 
     _, cfg = config.init()
     latest_version = cli.get_latest_vcs_version_tag(cfg, fetch=False)
-    assert latest_version == "0.1.10"
+    assert latest_version == expected_version
 
 
-def test_ignore_vcs_tag(runner, monkeypatch):
+@pytest.mark.parametrize("vcs_name", ['git', 'hg'])
+def test_ignore_vcs_tag(runner, monkeypatch, vcs_name):
     result = runner.invoke(cli.cli, ['init', "-vv"])
     assert result.exit_code == 0
 
     _update_config_val("bumpver.toml", push="false")
     _update_config_val("bumpver.toml", current_version='"0.1.8"')
     _update_config_val("bumpver.toml", version_pattern='"MAJOR.MINOR.PATCH"')
 
-    _vcs_init("git", files=["bumpver.toml"])
+    _vcs_init(vcs_name, files=["bumpver.toml"])
     _, cfg = config.init()
 
     # mock latest vcs tag 0.2.0 but cfg.current_version is 0.1.8
     monkeypatch.setattr(cli, "get_latest_vcs_version_tag", lambda cfg, fetch: "0.2.0")
     assert cfg.current_version == "0.1.8"
     assert cli.get_latest_vcs_version_tag(cfg, fetch=False) == "0.2.0"
 
@@ -1323,7 +1539,51 @@
 
     out_lines = set(result.output.splitlines())
     assert '-current_version = "0.1.8"' in out_lines
     assert '+current_version = "0.1.9"' in out_lines
 
     latest_version = cli.get_latest_vcs_version_tag(cfg, fetch=False)
     assert latest_version == "0.2.0"
+
+
+@pytest.mark.parametrize("vcs_name", ['git', 'hg'])
+def test_git_tag_scope_branch_version_conflict(runner, caplog, vcs_name):
+    result = runner.invoke(cli.cli, ['init', "-vv"])
+    assert result.exit_code == 0
+
+    _update_config_val("bumpver.toml", push="false")
+    _update_config_val("bumpver.toml", current_version='"0.1.8"')
+    _update_config_val("bumpver.toml", version_pattern='"MAJOR.MINOR.PATCH[PYTAGNUM]"')
+    _update_config_val("bumpver.toml", tag_scope=f'"{config.TagScope.BRANCH.value}"')
+
+    _vcs_init(vcs_name, files=["bumpver.toml"])
+
+    result = runner.invoke(cli.cli, ['update', "--patch"])
+    assert result.exit_code == 0
+
+    _, cfg = config.init()
+    latest_version = cli.get_latest_vcs_version_tag(cfg, fetch=False)
+    assert latest_version == "0.1.9"
+
+    if vcs_name == 'git':
+        shell("git", "branch", "dev")
+        shell("git", "checkout", "dev")
+    else:
+        shell("hg", "branch", "dev")
+
+    result = runner.invoke(cli.cli, ['update', "--minor", "--tag=beta"])
+    assert result.exit_code == 0
+
+    _, cfg = config.init()
+    latest_version = cli.get_latest_vcs_version_tag(cfg, fetch=False)
+    assert latest_version == "0.2.0b0"
+
+    if vcs_name == 'git':
+        shell("git", "checkout", "master")
+    else:
+        shell("hg", "update", "default")
+
+    result = runner.invoke(cli.cli, ['update', "--minor", "--tag=beta"])
+    assert result.exit_code == 1
+
+    error_message = "Invariant violated: New version must be unique accross all branches"
+    assert any(error_message in r.message for r in caplog.records)
```

### Comparing `bumpver-2023.1124/test/test_config.py` & `bumpver-2023.1125/test/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import unicode_literals
 
 import io
 from test import util
 
+import pytest
+
 from bumpver import config
 
 # pylint:disable=redefined-outer-name ; pytest fixtures
 # pylint:disable=protected-access ; allowed for test code
 
 
 PYCALVER_TOML_FIXTURE_1 = """
@@ -87,28 +89,35 @@
 
 
 NEW_PATTERN_CFG_FIXTURE = """
 [bumpver]
 current_version = "v201808.1456-beta"
 version_pattern = "vYYYY0M.BUILD[-TAG]"
 commit_message = "bump version to {new_version}"
+tag_message = "release {new_version}"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
 setup.py =
     {version}
     {pep440_version}
 setup.cfg =
     current_version = "{version}"
 src/project/*.py =
     Copyright (c) 2018-YYYY
 """
 
+MINIMAL_CFG_FIXTURE = """
+[bumpver]
+current_version = "v201808.1456-beta"
+version_pattern = "vYYYY0M.BUILD[-TAG]"
+"""
+
 
 def mk_buf(text):
     buf = io.StringIO()
     buf.write(text)
     buf.seek(0)
     return buf
 
@@ -201,28 +210,49 @@
 def test_parse_v2_cfg():
     buf = mk_buf(NEW_PATTERN_CFG_FIXTURE)
 
     raw_cfg = config._parse_cfg(buf)
     cfg     = config._parse_config(raw_cfg)
     assert cfg.current_version == "v201808.1456-beta"
     assert cfg.commit_message  == "bump version to {new_version}"
+    assert cfg.tag_message     == "release {new_version}"
     assert cfg.commit is True
     assert cfg.tag    is True
     assert cfg.push   is True
 
     files = set(cfg.file_patterns)
     assert "setup.py" in files
     assert "setup.cfg" in files
 
     raw_patterns_by_path = _parse_raw_patterns_by_filepath(cfg)
     assert raw_patterns_by_path["setup.py"] == ["vYYYY0M.BUILD[-TAG]", "YYYY0M.BLD[PYTAGNUM]"]
     assert raw_patterns_by_path["setup.cfg"] == ['current_version = "vYYYY0M.BUILD[-TAG]"']
     assert raw_patterns_by_path["src/project/*.py"] == ["Copyright (c) 2018-YYYY"]
 
 
+@pytest.mark.parametrize("tag_scope", [e.value for e in list(config.TagScope)])
+def test_parse_tag_scope_cfg(tag_scope):
+    buf = mk_buf(f"{MINIMAL_CFG_FIXTURE}\ntag_scope={tag_scope}")
+
+    raw_cfg = config._parse_cfg(buf)
+    cfg     = config._parse_config(raw_cfg)
+
+    assert cfg.tag_scope == tag_scope
+
+
+@pytest.mark.parametrize("tag_scope", ['foobar'])
+def test_parse_tag_scope_cfg_invalid_value(tag_scope):
+    buf = mk_buf(f"{MINIMAL_CFG_FIXTURE}\ntag_scope={tag_scope}")
+
+    raw_cfg = config._parse_cfg(buf)
+
+    with pytest.raises(ValueError):
+        config._parse_config(raw_cfg)
+
+
 def test_parse_default_toml():
     project_path = util.FIXTURES_DIR / "project_a"
 
     ctx          = config.init_project_ctx(project_path)
     default_toml = config.default_config(ctx)
 
     buf     = mk_buf(default_toml)
```

### Comparing `bumpver-2023.1124/test/test_parse.py` & `bumpver-2023.1125/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/test/test_patterns.py` & `bumpver-2023.1125/test/test_patterns.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/test/test_rewrite.py` & `bumpver-2023.1125/test/test_rewrite.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/test/test_version.py` & `bumpver-2023.1125/test/test_version.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1124/test/util.py` & `bumpver-2023.1125/test/util.py`

 * *Files identical despite different names*

