# Comparing `tmp/xbrl-us-0.0.31.tar.gz` & `tmp/xbrl-us-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbrl-us-0.0.31.tar", last modified: Fri Jul 14 19:56:34 2023, max compression
+gzip compressed data, was "xbrl-us-0.0.32.tar", last modified: Mon Jul 17 21:31:46 2023, max compression
```

## Comparing `xbrl-us-0.0.31.tar` & `xbrl-us-0.0.32.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:56:34.746403 xbrl-us-0.0.31/
--rw-r--r--   0 hamid      (501) staff       (20)      528 2023-07-14 19:46:19.000000 xbrl-us-0.0.31/.bumpversion.cfg
--rw-r--r--   0 hamid      (501) staff       (20)     2016 2023-07-14 19:46:19.000000 xbrl-us-0.0.31/.cookiecutterrc
--rw-r--r--   0 hamid      (501) staff       (20)      175 2023-06-26 21:38:04.000000 xbrl-us-0.0.31/.coveragerc
--rw-r--r--   0 hamid      (501) staff       (20)      353 2023-06-26 21:38:04.000000 xbrl-us-0.0.31/.editorconfig
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:56:34.697160 xbrl-us-0.0.31/.github/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:56:34.706160 xbrl-us-0.0.31/.github/workflows/
--rw-r--r--   0 hamid      (501) staff       (20)     3400 2023-07-14 19:39:33.000000 xbrl-us-0.0.31/.github/workflows/github-actions.yml
--rw-r--r--   0 hamid      (501) staff       (20)      688 2023-06-26 21:40:12.000000 xbrl-us-0.0.31/.pre-commit-config.yaml
--rw-r--r--   0 hamid      (501) staff       (20)      285 2023-07-08 20:32:20.000000 xbrl-us-0.0.31/.readthedocs.yml
--rw-r--r--   0 hamid      (501) staff       (20)       71 2023-07-06 22:38:13.000000 xbrl-us-0.0.31/AUTHORS.rst
--rw-r--r--   0 hamid      (501) staff       (20)      564 2023-07-14 19:56:27.000000 xbrl-us-0.0.31/CHANGELOG.rst
--rw-r--r--   0 hamid      (501) staff       (20)     2376 2023-06-26 21:38:04.000000 xbrl-us-0.0.31/CONTRIBUTING.rst
--rw-r--r--   0 hamid      (501) staff       (20)     1105 2023-06-26 21:41:13.000000 xbrl-us-0.0.31/LICENSE
--rw-r--r--   0 hamid      (501) staff       (20)      457 2023-07-14 18:26:55.000000 xbrl-us-0.0.31/MANIFEST.in
--rw-r--r--   0 hamid      (501) staff       (20)     9591 2023-07-14 19:56:34.744709 xbrl-us-0.0.31/PKG-INFO
--rw-r--r--   0 hamid      (501) staff       (20)     7762 2023-07-14 19:54:32.000000 xbrl-us-0.0.31/README.rst
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:56:34.707414 xbrl-us-0.0.31/ci/
--rwxr-xr-x   0 hamid      (501) staff       (20)     2867 2023-06-26 21:38:04.000000 xbrl-us-0.0.31/ci/bootstrap.py
--rw-r--r--   0 hamid      (501) staff       (20)       72 2023-06-26 21:38:04.000000 xbrl-us-0.0.31/ci/requirements.txt
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:56:34.697541 xbrl-us-0.0.31/ci/templates/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:56:34.697636 xbrl-us-0.0.31/ci/templates/.github/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:56:34.707957 xbrl-us-0.0.31/ci/templates/.github/workflows/
--rw-r--r--   0 hamid      (501) staff       (20)     1963 2023-06-26 21:38:04.000000 xbrl-us-0.0.31/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:56:34.710615 xbrl-us-0.0.31/docs/
--rw-r--r--   0 hamid      (501) staff       (20)       28 2023-06-26 21:38:04.000000 xbrl-us-0.0.31/docs/authors.rst
--rw-r--r--   0 hamid      (501) staff       (20)       30 2023-06-26 21:38:04.000000 xbrl-us-0.0.31/docs/changelog.rst
--rw-r--r--   0 hamid      (501) staff       (20)     1156 2023-07-14 19:46:19.000000 xbrl-us-0.0.31/docs/conf.py
--rw-r--r--   0 hamid      (501) staff       (20)       33 2023-06-26 21:38:04.000000 xbrl-us-0.0.31/docs/contributing.rst
--rw-r--r--   0 hamid      (501) staff       (20)      219 2023-07-09 12:54:31.000000 xbrl-us-0.0.31/docs/index.rst
--rw-r--r--   0 hamid      (501) staff       (20)       27 2023-06-26 21:38:04.000000 xbrl-us-0.0.31/docs/readme.rst
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:56:34.711266 xbrl-us-0.0.31/docs/reference/
--rw-r--r--   0 hamid      (501) staff       (20)       59 2023-07-09 15:02:31.000000 xbrl-us-0.0.31/docs/reference/index.rst
--rw-r--r--   0 hamid      (501) staff       (20)       98 2023-07-09 15:02:46.000000 xbrl-us-0.0.31/docs/reference/xbrl_us.rst
--rw-r--r--   0 hamid      (501) staff       (20)       35 2023-07-09 00:13:53.000000 xbrl-us-0.0.31/docs/requirements.txt
--rw-r--r--   0 hamid      (501) staff       (20)      109 2023-06-26 21:38:04.000000 xbrl-us-0.0.31/docs/spelling_wordlist.txt
--rw-r--r--   0 hamid      (501) staff       (20)     1194 2023-07-12 22:49:38.000000 xbrl-us-0.0.31/pyproject.toml
--rw-r--r--   0 hamid      (501) staff       (20)      772 2023-06-26 21:38:04.000000 xbrl-us-0.0.31/pytest.ini
--rw-r--r--   0 hamid      (501) staff       (20)       54 2023-07-14 18:22:29.000000 xbrl-us-0.0.31/secrets.yml
--rw-r--r--   0 hamid      (501) staff       (20)       38 2023-07-14 19:56:34.746590 xbrl-us-0.0.31/setup.cfg
--rwxr-xr-x   0 hamid      (501) staff       (20)     3008 2023-07-14 19:46:19.000000 xbrl-us-0.0.31/setup.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:56:34.698256 xbrl-us-0.0.31/src/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:56:34.712945 xbrl-us-0.0.31/src/xbrl_us/
--rw-r--r--   0 hamid      (501) staff       (20)       70 2023-07-14 19:46:19.000000 xbrl-us-0.0.31/src/xbrl_us/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)      372 2023-07-12 22:27:55.000000 xbrl-us-0.0.31/src/xbrl_us/__main__.py
--rw-r--r--   0 hamid      (501) staff       (20)    15086 2023-07-14 18:15:04.000000 xbrl-us-0.0.31/src/xbrl_us/app.py
--rw-r--r--   0 hamid      (501) staff       (20)      373 2023-07-12 22:49:38.000000 xbrl-us-0.0.31/src/xbrl_us/cli.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:56:34.730355 xbrl-us-0.0.31/src/xbrl_us/methods/
--rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:13:32.000000 xbrl-us-0.0.31/src/xbrl_us/methods/assertion search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      297 2023-07-10 18:27:24.000000 xbrl-us-0.0.31/src/xbrl_us/methods/assertion validate.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1002 2023-07-10 12:13:32.000000 xbrl-us-0.0.31/src/xbrl_us/methods/concept name search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1555 2023-07-10 12:13:32.000000 xbrl-us-0.0.31/src/xbrl_us/methods/concept search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1077 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/cube search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/dimension search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      672 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/document search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      480 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/dts id concept label.yml
--rw-r--r--   0 hamid      (501) staff       (20)      870 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/dts id concept name.yml
--rw-r--r--   0 hamid      (501) staff       (20)      589 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/dts id concept reference.yml
--rw-r--r--   0 hamid      (501) staff       (20)      953 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/dts id concept search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1270 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/dts id network search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      850 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/dts id network.yml
--rw-r--r--   0 hamid      (501) staff       (20)      525 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/dts search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1229 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/entity id report search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      343 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/entity id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1273 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/entity report search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      387 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/entity search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1552 2023-07-10 19:53:06.000000 xbrl-us-0.0.31/src/xbrl_us/methods/fact id.yml
--rw-r--r--   0 hamid      (501) staff       (20)      960 2023-07-10 19:53:06.000000 xbrl-us-0.0.31/src/xbrl_us/methods/fact search oim.yml
--rw-r--r--   0 hamid      (501) staff       (20)     9191 2023-07-13 13:17:04.000000 xbrl-us-0.0.31/src/xbrl_us/methods/fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      519 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/label dts id search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      510 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/label search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1332 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/network id relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      394 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/network id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1319 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/network relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1323 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      956 2023-07-10 12:16:52.000000 xbrl-us-0.0.31/src/xbrl_us/methods/relationship tree search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     2923 2023-07-10 21:15:17.000000 xbrl-us-0.0.31/src/xbrl_us/methods/report fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)       99 2023-07-10 19:53:06.000000 xbrl-us-0.0.31/src/xbrl_us/methods/report id delete.yml
--rw-r--r--   0 hamid      (501) staff       (20)     2743 2023-07-10 20:49:26.000000 xbrl-us-0.0.31/src/xbrl_us/methods/report id fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      731 2023-07-10 20:05:31.000000 xbrl-us-0.0.31/src/xbrl_us/methods/report id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1150 2023-07-10 19:53:06.000000 xbrl-us-0.0.31/src/xbrl_us/methods/report search.yml
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:56:34.738492 xbrl-us-0.0.31/src/xbrl_us/schemas/
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:52:58.000000 xbrl-us-0.0.31/src/xbrl_us/schemas/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:14.000000 xbrl-us-0.0.31/src/xbrl_us/schemas/assertion_details.py
--rw-r--r--   0 hamid      (501) staff       (20)     5257 2023-07-07 22:17:57.000000 xbrl-us-0.0.31/src/xbrl_us/schemas/concept_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:14.000000 xbrl-us-0.0.31/src/xbrl_us/schemas/cube_details.py
--rw-r--r--   0 hamid      (501) staff       (20)     1501 2023-07-07 22:17:57.000000 xbrl-us-0.0.31/src/xbrl_us/schemas/dimension_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:36.000000 xbrl-us-0.0.31/src/xbrl_us/schemas/document_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:29.000000 xbrl-us-0.0.31/src/xbrl_us/schemas/dts_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:05.000000 xbrl-us-0.0.31/src/xbrl_us/schemas/entity_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:56:32.000000 xbrl-us-0.0.31/src/xbrl_us/schemas/fact_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:47.000000 xbrl-us-0.0.31/src/xbrl_us/schemas/label_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:54.000000 xbrl-us-0.0.31/src/xbrl_us/schemas/network_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:04.000000 xbrl-us-0.0.31/src/xbrl_us/schemas/relationship_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:41:48.000000 xbrl-us-0.0.31/src/xbrl_us/schemas/report_details.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:56:34.742663 xbrl-us-0.0.31/src/xbrl_us/utils/
--rw-r--r--   0 hamid      (501) staff       (20)       97 2023-07-10 21:39:35.000000 xbrl-us-0.0.31/src/xbrl_us/utils/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)     1377 2023-07-12 17:14:14.000000 xbrl-us-0.0.31/src/xbrl_us/utils/exceptions.py
--rw-r--r--   0 hamid      (501) staff       (20)      464 2023-07-08 23:56:22.000000 xbrl-us-0.0.31/src/xbrl_us/utils/fields.py
--rw-r--r--   0 hamid      (501) staff       (20)    26377 2023-07-07 22:12:20.000000 xbrl-us-0.0.31/src/xbrl_us/utils/paramters.py
--rw-r--r--   0 hamid      (501) staff       (20)    26110 2023-07-14 18:15:12.000000 xbrl-us-0.0.31/src/xbrl_us/xbrl_us.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:56:34.715312 xbrl-us-0.0.31/src/xbrl_us.egg-info/
--rw-r--r--   0 hamid      (501) staff       (20)     9591 2023-07-14 19:56:34.000000 xbrl-us-0.0.31/src/xbrl_us.egg-info/PKG-INFO
--rw-r--r--   0 hamid      (501) staff       (20)     2927 2023-07-14 19:56:34.000000 xbrl-us-0.0.31/src/xbrl_us.egg-info/SOURCES.txt
--rw-r--r--   0 hamid      (501) staff       (20)        1 2023-07-14 19:56:34.000000 xbrl-us-0.0.31/src/xbrl_us.egg-info/dependency_links.txt
--rw-r--r--   0 hamid      (501) staff       (20)       45 2023-07-14 19:56:34.000000 xbrl-us-0.0.31/src/xbrl_us.egg-info/entry_points.txt
--rw-r--r--   0 hamid      (501) staff       (20)        1 2023-07-14 18:18:57.000000 xbrl-us-0.0.31/src/xbrl_us.egg-info/not-zip-safe
--rw-r--r--   0 hamid      (501) staff       (20)      103 2023-07-14 19:56:34.000000 xbrl-us-0.0.31/src/xbrl_us.egg-info/requires.txt
--rw-r--r--   0 hamid      (501) staff       (20)        8 2023-07-14 19:56:34.000000 xbrl-us-0.0.31/src/xbrl_us.egg-info/top_level.txt
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:56:34.743415 xbrl-us-0.0.31/tests/
--rw-r--r--   0 hamid      (501) staff       (20)      515 2023-07-12 23:36:14.000000 xbrl-us-0.0.31/tests/test_xbrl_us.py
--rw-r--r--   0 hamid      (501) staff       (20)     1486 2023-07-14 19:43:01.000000 xbrl-us-0.0.31/tox.ini
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.556568 xbrl-us-0.0.32/
+-rw-r--r--   0 hamid      (501) staff       (20)      528 2023-07-17 21:26:35.000000 xbrl-us-0.0.32/.bumpversion.cfg
+-rw-r--r--   0 hamid      (501) staff       (20)     2016 2023-07-17 21:26:35.000000 xbrl-us-0.0.32/.cookiecutterrc
+-rw-r--r--   0 hamid      (501) staff       (20)      175 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/.coveragerc
+-rw-r--r--   0 hamid      (501) staff       (20)      353 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/.editorconfig
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.502129 xbrl-us-0.0.32/.github/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.509956 xbrl-us-0.0.32/.github/workflows/
+-rw-r--r--   0 hamid      (501) staff       (20)     3400 2023-07-14 19:39:33.000000 xbrl-us-0.0.32/.github/workflows/github-actions.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      688 2023-06-26 21:40:12.000000 xbrl-us-0.0.32/.pre-commit-config.yaml
+-rw-r--r--   0 hamid      (501) staff       (20)      285 2023-07-08 20:32:20.000000 xbrl-us-0.0.32/.readthedocs.yml
+-rw-r--r--   0 hamid      (501) staff       (20)       71 2023-07-06 22:38:13.000000 xbrl-us-0.0.32/AUTHORS.rst
+-rw-r--r--   0 hamid      (501) staff       (20)      694 2023-07-17 21:31:18.000000 xbrl-us-0.0.32/CHANGELOG.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     2376 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/CONTRIBUTING.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     1105 2023-06-26 21:41:13.000000 xbrl-us-0.0.32/LICENSE
+-rw-r--r--   0 hamid      (501) staff       (20)      457 2023-07-14 18:26:55.000000 xbrl-us-0.0.32/MANIFEST.in
+-rw-r--r--   0 hamid      (501) staff       (20)    13345 2023-07-17 21:31:46.555944 xbrl-us-0.0.32/PKG-INFO
+-rw-r--r--   0 hamid      (501) staff       (20)    11286 2023-07-17 21:18:39.000000 xbrl-us-0.0.32/README.rst
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.510751 xbrl-us-0.0.32/ci/
+-rwxr-xr-x   0 hamid      (501) staff       (20)     2867 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/ci/bootstrap.py
+-rw-r--r--   0 hamid      (501) staff       (20)       72 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/ci/requirements.txt
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.502553 xbrl-us-0.0.32/ci/templates/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.502663 xbrl-us-0.0.32/ci/templates/.github/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.511228 xbrl-us-0.0.32/ci/templates/.github/workflows/
+-rw-r--r--   0 hamid      (501) staff       (20)     1963 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.515162 xbrl-us-0.0.32/docs/
+-rw-r--r--   0 hamid      (501) staff       (20)       28 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/docs/authors.rst
+-rw-r--r--   0 hamid      (501) staff       (20)       30 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/docs/changelog.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     1156 2023-07-17 21:26:35.000000 xbrl-us-0.0.32/docs/conf.py
+-rw-r--r--   0 hamid      (501) staff       (20)       33 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/docs/contributing.rst
+-rw-r--r--   0 hamid      (501) staff       (20)      219 2023-07-09 12:54:31.000000 xbrl-us-0.0.32/docs/index.rst
+-rw-r--r--   0 hamid      (501) staff       (20)    10210 2023-07-16 13:55:28.000000 xbrl-us-0.0.32/docs/readme.rst
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.516410 xbrl-us-0.0.32/docs/reference/
+-rw-r--r--   0 hamid      (501) staff       (20)       59 2023-07-09 15:02:31.000000 xbrl-us-0.0.32/docs/reference/index.rst
+-rw-r--r--   0 hamid      (501) staff       (20)       98 2023-07-09 15:02:46.000000 xbrl-us-0.0.32/docs/reference/xbrl_us.rst
+-rw-r--r--   0 hamid      (501) staff       (20)       35 2023-07-09 00:13:53.000000 xbrl-us-0.0.32/docs/requirements.txt
+-rw-r--r--   0 hamid      (501) staff       (20)      109 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/docs/spelling_wordlist.txt
+-rw-r--r--   0 hamid      (501) staff       (20)     1194 2023-07-12 22:49:38.000000 xbrl-us-0.0.32/pyproject.toml
+-rw-r--r--   0 hamid      (501) staff       (20)      772 2023-06-26 21:38:04.000000 xbrl-us-0.0.32/pytest.ini
+-rw-r--r--   0 hamid      (501) staff       (20)       54 2023-07-14 18:22:29.000000 xbrl-us-0.0.32/secrets.yml
+-rw-r--r--   0 hamid      (501) staff       (20)       38 2023-07-17 21:31:46.556721 xbrl-us-0.0.32/setup.cfg
+-rwxr-xr-x   0 hamid      (501) staff       (20)     3004 2023-07-17 21:26:35.000000 xbrl-us-0.0.32/setup.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.503352 xbrl-us-0.0.32/src/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.519187 xbrl-us-0.0.32/src/xbrl_us/
+-rw-r--r--   0 hamid      (501) staff       (20)       70 2023-07-17 21:26:35.000000 xbrl-us-0.0.32/src/xbrl_us/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)      372 2023-07-12 22:27:55.000000 xbrl-us-0.0.32/src/xbrl_us/__main__.py
+-rw-r--r--   0 hamid      (501) staff       (20)    16235 2023-07-15 18:40:11.000000 xbrl-us-0.0.32/src/xbrl_us/app.py
+-rw-r--r--   0 hamid      (501) staff       (20)      373 2023-07-12 22:49:38.000000 xbrl-us-0.0.32/src/xbrl_us/cli.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.544228 xbrl-us-0.0.32/src/xbrl_us/methods/
+-rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:13:32.000000 xbrl-us-0.0.32/src/xbrl_us/methods/assertion search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      297 2023-07-10 18:27:24.000000 xbrl-us-0.0.32/src/xbrl_us/methods/assertion validate.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1002 2023-07-10 12:13:32.000000 xbrl-us-0.0.32/src/xbrl_us/methods/concept name search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1555 2023-07-10 12:13:32.000000 xbrl-us-0.0.32/src/xbrl_us/methods/concept search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1077 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/cube search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/dimension search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      672 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/document search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      480 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/dts id concept label.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      870 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/dts id concept name.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      589 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/dts id concept reference.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      953 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/dts id concept search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1270 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/dts id network search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      850 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/dts id network.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      525 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/dts search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1229 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/entity id report search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      343 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/entity id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1273 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/entity report search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      387 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/entity search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1552 2023-07-10 19:53:06.000000 xbrl-us-0.0.32/src/xbrl_us/methods/fact id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      960 2023-07-10 19:53:06.000000 xbrl-us-0.0.32/src/xbrl_us/methods/fact search oim.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     9377 2023-07-15 18:41:16.000000 xbrl-us-0.0.32/src/xbrl_us/methods/fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      519 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/label dts id search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      510 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/label search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1332 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/network id relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      394 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/network id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1319 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/network relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1323 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      956 2023-07-10 12:16:52.000000 xbrl-us-0.0.32/src/xbrl_us/methods/relationship tree search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     2923 2023-07-10 21:15:17.000000 xbrl-us-0.0.32/src/xbrl_us/methods/report fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)       99 2023-07-10 19:53:06.000000 xbrl-us-0.0.32/src/xbrl_us/methods/report id delete.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     2743 2023-07-10 20:49:26.000000 xbrl-us-0.0.32/src/xbrl_us/methods/report id fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      731 2023-07-10 20:05:31.000000 xbrl-us-0.0.32/src/xbrl_us/methods/report id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1150 2023-07-10 19:53:06.000000 xbrl-us-0.0.32/src/xbrl_us/methods/report search.yml
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.552208 xbrl-us-0.0.32/src/xbrl_us/schemas/
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:52:58.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:14.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/assertion_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)     5257 2023-07-07 22:17:57.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/concept_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:14.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/cube_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1501 2023-07-07 22:17:57.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/dimension_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:36.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/document_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:29.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/dts_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:05.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/entity_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:56:32.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/fact_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:47.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/label_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:54.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/network_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:04.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/relationship_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:41:48.000000 xbrl-us-0.0.32/src/xbrl_us/schemas/report_details.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.554423 xbrl-us-0.0.32/src/xbrl_us/utils/
+-rw-r--r--   0 hamid      (501) staff       (20)       97 2023-07-10 21:39:35.000000 xbrl-us-0.0.32/src/xbrl_us/utils/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1633 2023-07-16 19:19:32.000000 xbrl-us-0.0.32/src/xbrl_us/utils/exceptions.py
+-rw-r--r--   0 hamid      (501) staff       (20)      464 2023-07-08 23:56:22.000000 xbrl-us-0.0.32/src/xbrl_us/utils/fields.py
+-rw-r--r--   0 hamid      (501) staff       (20)    26377 2023-07-07 22:12:20.000000 xbrl-us-0.0.32/src/xbrl_us/utils/paramters.py
+-rw-r--r--   0 hamid      (501) staff       (20)    26901 2023-07-17 21:18:39.000000 xbrl-us-0.0.32/src/xbrl_us/xbrl_us.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.522855 xbrl-us-0.0.32/src/xbrl_us.egg-info/
+-rw-r--r--   0 hamid      (501) staff       (20)    13345 2023-07-17 21:31:46.000000 xbrl-us-0.0.32/src/xbrl_us.egg-info/PKG-INFO
+-rw-r--r--   0 hamid      (501) staff       (20)     2927 2023-07-17 21:31:46.000000 xbrl-us-0.0.32/src/xbrl_us.egg-info/SOURCES.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        1 2023-07-17 21:31:46.000000 xbrl-us-0.0.32/src/xbrl_us.egg-info/dependency_links.txt
+-rw-r--r--   0 hamid      (501) staff       (20)       45 2023-07-17 21:31:46.000000 xbrl-us-0.0.32/src/xbrl_us.egg-info/entry_points.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        1 2023-07-14 20:24:46.000000 xbrl-us-0.0.32/src/xbrl_us.egg-info/not-zip-safe
+-rw-r--r--   0 hamid      (501) staff       (20)      103 2023-07-17 21:31:46.000000 xbrl-us-0.0.32/src/xbrl_us.egg-info/requires.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        8 2023-07-17 21:31:46.000000 xbrl-us-0.0.32/src/xbrl_us.egg-info/top_level.txt
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-17 21:31:46.555143 xbrl-us-0.0.32/tests/
+-rw-r--r--   0 hamid      (501) staff       (20)      515 2023-07-12 23:36:14.000000 xbrl-us-0.0.32/tests/test_xbrl_us.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1486 2023-07-14 19:43:01.000000 xbrl-us-0.0.32/tox.ini
```

### Comparing `xbrl-us-0.0.31/.bumpversion.cfg` & `xbrl-us-0.0.32/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.0.31
+current_version = 0.0.32
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `xbrl-us-0.0.31/.cookiecutterrc` & `xbrl-us-0.0.32/.cookiecutterrc`

 * *Files 0% similar despite different names*

```diff
@@ -50,12 +50,12 @@
     scrutinizer: "no"
     setup_py_uses_setuptools_scm: "no"
     sphinx_docs: "yes"
     sphinx_docs_hosting: "https://python-xbrl-us.readthedocs.io/"
     sphinx_doctest: "no"
     sphinx_theme: "furo"
     test_matrix_separate_coverage: "no"
-    version: "0.0.31"
+    version: "0.0.32"
     version_manager: "bump2version"
     website: "https://hamidvakilzadeh.com"
     year_from: "2023"
     year_to: "2023"
```

### Comparing `xbrl-us-0.0.31/.github/workflows/github-actions.yml` & `xbrl-us-0.0.32/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/.pre-commit-config.yaml` & `xbrl-us-0.0.32/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/CHANGELOG.rst` & `xbrl-us-0.0.32/CHANGELOG.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 
 Changelog
 =========
 
+0.0.32 (2023-07-17)
+~~~~~~~~~~~~~~~~~~~
+
+* Improved Browser Interface
+* Added ``unique`` keyword to ``query`` method
+* Bug fixes
+
 0.0.31 (2023-07-14)
 ~~~~~~~~~~~~~~~~~~~
 
 * fixed dependency issues
 * Bug fixes
```

### Comparing `xbrl-us-0.0.31/CONTRIBUTING.rst` & `xbrl-us-0.0.32/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/LICENSE` & `xbrl-us-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/PKG-INFO` & `xbrl-us-0.0.32/docs/readme.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: xbrl-us
-Version: 0.0.31
-Summary: Python wrapper for xbrl.us API
-Home-page: https://github.com/hamid-vakilzadeh/python-xbrl-us
-Author: hamid-vakilzadeh
-Author-email: vakilzas@uww.edu
-License: MIT
-Project-URL: Documentation, https://python-xbrl-us.readthedocs.io/
-Project-URL: Changelog, https://python-xbrl-us.readthedocs.io/en/latest/changelog.html
-Project-URL: Issue Tracker, https://github.com/hamid-vakilzadeh/python-xbrl-us/issues
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 ======================
 XBRL-US Python Library
 ======================
 
 About
 =====
 
@@ -62,32 +32,32 @@
 
     [FILL: Publication Details]
 
 
 Tutorial ✏️📖📚
 ================
 
-This tutorial will guide you through using the XBRL-US Python library to interact with the XBRL API. The XBRL-US library provides a convenient way to query and retrieve financial data from the XBRL API using Python.
+This tutorial will guide you through using the XBRL-US Python library to interact with the XBRL API.
+The XBRL-US library provides a convenient way to query and retrieve financial data from the XBRL API using Python.
 
-Prerequisites
-~~~~~~~~~~~~~
+1. Prerequisites
+~~~~~~~~~~~~~~~~
 
 Before you begin, ensure you have the following:
 
 * **Python installed on your system**.
   The XBRL-US library supports Python 3.8 and above.
-* **XBRL-US library installed**.
 * **XBRL-US API credentials**.
   You can obtain your credentials by registering for a
   free XBRL-US account at https://xbrl.us/home/use/xbrl-api/.
 * **XBRL-US OAuth2 Access**.
   You can obtain your client ID and client secret by registering for a
   filling the request form at https://xbrl.us/home/use/xbrl-api/access-token/.
 
-You can install it using pip:
+You can install this package using pip:
 
 .. code-block:: bash
 
     pip install xbrl-us
 
 .. caution::
 
@@ -102,50 +72,74 @@
 For detailed information about the XBRL-US Python
 library, you can refer to the documentation at https://python-xbrl-us.readthedocs.io/en/latest/.
 
 **Official Documentation**
 
 For more information about the XBRL API and its endpoints, refer to the original API documentation at https://xbrlus.github.io/xbrl-api.
 
-Step 1: Import the XBRL Library
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+2. Choose Your Preferred Approach
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+There are two distinct ways to use the XBRL-US Python package:
+
+* **Code-Based Approach**: Import the XBRL-US Python package directly into your Python
+  environment for in-depth, custom analysis (see :ref:`Code-Based Approach <code-based approach>`)
+
+* **Browser Interface**: For a no-code experience, navigate to the :ref:`Browser Interface section <browser interface>`.
+  This interface allows for easy exploration and analysis of XBRL data directly in your web
+  browser.
+
+.. _code-based approach:
+
+2.1. Code-Based Approach
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+Import the XBRL Library
+-------------------------------
 
 To start using the XBRL-US library,
-you need to import it into your Python script::
+you need to import it into your Python script:
+
+.. code-block:: python
 
     from xbrl_us import XBRL
 
-Step 2: Create an Instance of XBRL Class
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Create an Instance of XBRL Class
+----------------------------------------
 
 Next, you need to create an instance of the ``XBRL`` class,
 providing your authentication credentials
-(client ID, client secret, username, and password) as parameters::
+(client ID, client secret, username, and password) as parameters:
+
+.. code-block:: python
 
     xbrl = XBRL(
     client_id='Your client id',
     client_secret='Your client secret',
     username='Your username',
     password='Your password'
     )
 
 Make sure to replace ``Your client id``,
 ``Your client secret``, ``Your username``, and
 ``Your password`` with your actual credentials.
 
-Step 3: Query the XBRL API
-~~~~~~~~~~~~~~~~~~~~~~~~~~
+Query the XBRL API
+------------------
 
 The XBRL-US library provides a query method to search
 for data from the XBRL API. You can specify various
 parameters and fields to filter and retrieve the
 desired data.
 
 Here's an example of using the query method to search
-for specific financial facts::
+for specific financial facts:
+
+.. code-block:: python
 
     response = xbrl.query(
         method='fact search',
         parameters={
             "concept.local-name": [
                 'OperatingIncomeLoss',
                 'GrossProfit',
@@ -179,15 +173,17 @@
 We are also specifying the fields we want to retrieve
 in the response. The ``limit`` parameter restricts the
 number of facts returned to 100, and ``as_dataframe=True``
 ensures the response is returned as a ``Pandas DataFrame``.
 
 Alternatively, you can use the ``Parameters`` and ``Fields``
 classes provided by the library to make the query more
-readable, less prone to errors, and easier to maintain::
+readable, less prone to errors, and easier to maintain:
+
+.. code-block:: python
 
     from xbrl_us.utils import Parameters, Fields
 
     response = xbrl.query(
         method='fact search',
         parameters=Parameters(
             concept_local_name=[
@@ -219,23 +215,25 @@
     )
 
 
 This alternative approach also allows you to
 take advantage of the autocomplete feature of your IDE to
 easily find the parameters and fields.
 
-Step 4: Perform Additional Queries
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Perform Additional Queries
+----------------------------------
 
 You can use the same query method to call other API
 endpoints by changing the method parameter and
 providing the relevant parameters and fields.
 
 Here's an example of using the query method to
-search for a specific fact by its ID::
+search for a specific fact by its ID:
+
+.. code-block:: python
 
     response = xbrl.query(
     method='fact id',
     parameters={'fact.id': 123},
     fields=[
         'report.accession',
         'period.fiscal-year',
@@ -253,65 +251,86 @@
     ],
     as_dataframe=False
     )
 
 Congratulations! You have learned how to use the XBRL-US Python library to interact with the XBRL API.
 In this example you will receive the data in json format as the ``as_dataframe`` parameter is set to ``False``.
 
+.. _browser interface:
 
-Development
-===========
+2.2 Browser Interface 🖥️
+~~~~~~~~~~~~~~~~~~~~~~~~
 
-To run all the tests run::
+This feature is designed to make our package even more user-friendly, allowing users to interact and work with XBRL data
+directly through a graphical interface, in addition to the existing code-based methods.
 
-    tox
+The browser interface streamlines data visualization, simplifies navigation, and enhances user interactions.
+With this intuitive, user-friendly interface, you can easily explore, interpret, and analyze XBRL data in real-time,
+right from your web browser.
 
-Note, to combine the coverage data from all the tox environments run:
+Key Features:
 
-.. list-table::
-    :widths: 10 90
-    :stub-columns: 1
+* Create Real-time queries right in your browser
+* Intuitive navigation and search features
+* Filtering and sorting options
+* Seamless integration with the existing XBRL-US Python API
 
-    - - Windows
-      - ::
+Getting started is as simple as ever.
+Update your XBRL-US Python package to the latest version and launch the new Browser Interface from the package menu.
 
-            set PYTEST_ADDOPTS=--cov-append
-            tox
+Getting Started with the Browser Interface
+------------------------------------------
 
-    - - Other
-      - ::
+Getting started is as simple as ever.
+First, ensure you have the latest version of ``xbrl-us`` installed by running the following code:
 
-            PYTEST_ADDOPTS=--cov-append tox
+.. code-block:: bash
+
+    pip install xbrl-us --upgrade
+
+
+Next, launch the new Browser Interface from the package menu:
+
+.. code-block:: bash
+
+    python -m xbrl_us
+
+That is it!
+You should now see the new Browser Interface open in your default web browser.
+
+Happy data exploring!
+
+.. note::
+
+    Please note, while we have tested the interface extensively, this is its initial release.
+    We encourage users to provide feedback to help us further improve the tool. We value your input!
+    You can also find tutorials, example codes, and more resources to help you get started.
 
 
-Changelog
-=========
 
-0.0.31 (2023-07-14)
-~~~~~~~~~~~~~~~~~~~
+Development
+===========
+
+To run all the tests run:
 
-* fixed dependency issues
-* Bug fixes
+.. code-block:: bash
 
+    tox
 
-0.0.3 (2023-07-14)
-~~~~~~~~~~~~~~~~~~
 
-* Backward compatibility with Python 3.8 and 3.9
-* Bug fixes
+Note, to combine the coverage data from all the tox environments run:
 
-0.0.2 (2023-07-12)
-~~~~~~~~~~~~~~~~~~
+.. list-table::
+    :widths: 10 90
+    :stub-columns: 1
 
+    * - Windows
+      - .. code-block:: bash
 
-* Bug fixes
-* Enhanced error handling
-* Improved ``methods`` attributes
-* Added the ability to print the query string
-* Implemented a feature to handle queries with large limits
-* NEW: Introduced a web interface for the API, making it even easier to use
+            set PYTEST_ADDOPTS=--cov-append
+            tox
 
 
-0.0.1 (2023-07-09)
-~~~~~~~~~~~~~~~~~~
+    * - Other
+      - .. code-block:: bash
 
-* First release on PyPI.
+            PYTEST_ADDOPTS=--cov-append tox
```

### Comparing `xbrl-us-0.0.31/ci/bootstrap.py` & `xbrl-us-0.0.32/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/ci/templates/.github/workflows/github-actions.yml` & `xbrl-us-0.0.32/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/docs/conf.py` & `xbrl-us-0.0.32/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "xbrl-us"
 year = "2023"
 author = "hamid-vakilzadeh"
 copyright = f"{year}, {author}"
-version = release = "0.0.31"
+version = release = "0.0.32"
 
 pygments_style = "emacs"
 highlight_language = "python"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/hamid-vakilzadeh/python-xbrl-us/issues/%s", "#"),
     "pr": ("https://github.com/hamid-vakilzadeh/python-xbrl-us/pull/%s", "PR #"),
```

### Comparing `xbrl-us-0.0.31/pyproject.toml` & `xbrl-us-0.0.32/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/pytest.ini` & `xbrl-us-0.0.32/pytest.ini`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/setup.py` & `xbrl-us-0.0.32/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="xbrl-us",
-    version="0.0.31",
+    version="0.0.32",
     license="MIT",
     description="Python wrapper for xbrl.us API",
     long_description_content_type="text/x-rst",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
@@ -37,16 +37,16 @@
         "Operating System :: Unix",
         "Operating System :: POSIX",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         # "Programming Language :: Python :: 3.7",
-        # "Programming Language :: Python :: 3.8",
-        # "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         # uncomment if you test on these interpreters:
         # "Programming Language :: Python :: Implementation :: IronPython",
         # "Programming Language :: Python :: Implementation :: Jython",
```

### Comparing `xbrl-us-0.0.31/src/xbrl_us/app.py` & `xbrl-us-0.0.32/src/xbrl_us/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import streamlit as st
 
-from xbrl_us.xbrl_us import XBRL
+from xbrl_us import XBRL
 
 
 def try_credentials(user_name: str, pass_word: str, client_id: str, client_secret: str):
     try:
         with st.spinner(text="Validating credentials..."):
             XBRL(username=user_name, password=pass_word, client_id=client_id, client_secret=client_secret)._get_token()
             st.session_state.username = user_name
@@ -12,35 +12,29 @@
             st.session_state.client_id = client_id
             st.session_state.client_secret = client_secret
     except Exception as e:
         st.error(f"Invalid credentials. Please try again. {e}")
         st.stop()
 
 
-@st.cache_data(show_spinner="Running query...", max_entries=1000)
-def run_query(params: dict):
-    st.empty()
-    method = params.get("method", None)
-    fields = params.get("fields", None)
-    _parameters = params.get("parameters", None)
-    limit = params.get("limit", None)
-    sort = params.get("sort", None)
-    df = xbrl.query(
-        method=method,
-        fields=fields,
-        parameters=_parameters,
-        limit=limit,
-        sort=sort,
-        as_dataframe=True,
-        print_query=True,
-        streamlit=True,
-    )
+@st.cache_data(show_spinner=False)
+def cache_params(params: dict):
+    cached_params = {
+        "method": params.get("method", None),
+        "fields": params.get("fields", None),
+        "parameters": params.get("parameters", None),
+        "limit": params.get("limit", None),
+        "sort": params.get("sort", None),
+        "unique": params.get("unique", False),
+        "print_query": params.get("print_query", True),
+        "as_dataframe": params.get("as_dataframe", True),
+        "streamlit": params.get("streamlit", True),
+    }
 
-    st.session_state.last_query = df
-    st.session_state.pop("query_params")
+    st.session_state.cached_params = cached_params
 
 
 def show_login():
     # Setup credentials in Streamlit
     username = st.text_input(
         label="Username",
         help="Your username for the [XBRL.US](https://www.xbrl.us) API.",
@@ -151,15 +145,15 @@
                 label_visibility="collapsed",
                 key=f"{key}_selector",
             )
 
             if st.session_state[f"{key}_selector"][0] == st.session_state[f"{key}_selector"][1]:
                 st.error(f"switch to list mode and select {st.session_state[f'{key}'][0]}")
 
-            st.session_state[key] = range(st.session_state[f"{key}_selector"][0], st.session_state[f"{key}_selector"][1])
+            st.session_state[key] = range(st.session_state[f"{key}_selector"][0], st.session_state[f"{key}_selector"][1] + 1)
 
     else:
         st.multiselect(
             label=f"{key}",
             options=list(range(values["min"], values["max"])),
             key=f"{key}",
             label_visibility="collapsed",
@@ -248,14 +242,21 @@
                 options=st.session_state.fields,
                 key="sort",
             )
 
             if len(st.session_state.sort) == 0:
                 sidebar.warning("It is recommended to choose at least one field to sort")
 
+            # check box for unique
+            sidebar.checkbox(
+                label="Unique",
+                key="unique_yes",
+                help="Return unique rows from the results",
+            )
+
             st.session_state.limit_param = None
             # check box for limit
             sidebar.checkbox(
                 label="Limit",
                 key="limit_yes",
             )
             if st.session_state.limit_yes:
@@ -274,74 +275,76 @@
                     st.session_state.limit_param = "all"
                     sidebar.error(
                         """This may take a long time to run. Only use this option if you are sure you want to retrieve all the data."""
                     )
 
         query_button_placeholder = st.empty()
         show_criteria = True
+        show_criteria_placeholder = st.empty()
         if len(st.session_state.parameters) == 0 and len(st.session_state.sort) == 0:
             st.info("No **Sort** or search criteria (**Parameters**) has been selected")
         else:
             # a checkbox to expand the query criteria
-            query_button = st.checkbox(
+            query_button = show_criteria_placeholder.checkbox(
                 label="Show Query Criteria",
                 key="query_button",
                 value=True,
             )
             if not query_button:
                 show_criteria = False
-        if show_criteria:
-            with st.expander(label="**Query Criteria Details**", expanded=True):
-                st.session_state.sort_params = {}
-                if len(st.session_state.sort) > 0:
-                    st.subheader("**Sort**:")
-                    for field in st.session_state.sort:
-                        sort_order = st.radio(
-                            label=f"**{field}**:",
-                            options=("Ascending", "Descending"),
-                            horizontal=True,
-                            key=f"{field}_sort",
-                        )
-                        st.session_state.sort_params[field] = "asc" if sort_order == "Ascending" else "desc"
-                    st.markdown("---")
+        with st.expander(label="**Query Criteria Details**", expanded=show_criteria):
+            st.session_state.sort_params = {}
+            if len(st.session_state.sort) > 0:
+                st.subheader("**Sort**:")
+                for field in st.session_state.sort:
+                    sort_order = st.radio(
+                        label=f"**{field}**:",
+                        options=("Ascending", "Descending"),
+                        horizontal=True,
+                        key=f"{field}_sort",
+                    )
+                    st.session_state.sort_params[field] = "asc" if sort_order == "Ascending" else "desc"
+                st.markdown("---")
 
-                for param in st.session_state.parameters:
-                    st.subheader(f"**{param}**:")
-                    st.write(st.session_state.method_params.parameters[param]["description"])
+            for param in st.session_state.parameters:
+                st.subheader(f"**{param}**:")
+                st.write(st.session_state.method_params.parameters[param]["description"])
+
+                if st.session_state.method_params.parameters[param]["type"] == "boolean":
+                    boolean_input_for_booleans(param)
+
+                elif st.session_state.method_params.parameters[param]["type"] == "integer":
+                    input_number_for_integers(param)
+
+                elif st.session_state.method_params.parameters[param]["type"] == "string":
+                    text_input_for_strings(param)
+
+                elif st.session_state.method_params.parameters[param]["type"] == "array[integer]":
+                    range_and_slider_for_array_integers(
+                        param,
+                        st.session_state.method_params.parameters[param]["values"],
+                    )
 
-                    if st.session_state.method_params.parameters[param]["type"] == "boolean":
-                        boolean_input_for_booleans(param)
+                elif st.session_state.method_params.parameters[param]["type"] == "array[string]":
+                    text_box_for_array_strings_no_ops(param)
 
-                    elif st.session_state.method_params.parameters[param]["type"] == "integer":
-                        input_number_for_integers(param)
+            st.session_state.query_params = {"fields": st.session_state.fields}
+
+            if len(st.session_state.parameters) > 0:
+                st.session_state.query_params["parameters"] = {}
+                for param in st.session_state.parameters:
+                    st.session_state.query_params["parameters"][param] = st.session_state[param]
 
-                    elif st.session_state.method_params.parameters[param]["type"] == "string":
-                        text_input_for_strings(param)
-
-                    elif st.session_state.method_params.parameters[param]["type"] == "array[integer]":
-                        range_and_slider_for_array_integers(
-                            param,
-                            st.session_state.method_params.parameters[param]["values"],
-                        )
-
-                    elif st.session_state.method_params.parameters[param]["type"] == "array[string]":
-                        text_box_for_array_strings_no_ops(param)
-
-                st.session_state.query_params = {"fields": st.session_state.fields}
-
-                if len(st.session_state.parameters) > 0:
-                    st.session_state.query_params["parameters"] = {}
-                    for param in st.session_state.parameters:
-                        st.session_state.query_params["parameters"][param] = st.session_state[param]
-
-                if len(st.session_state.sort_params) > 0:
-                    st.session_state.query_params["sort"] = st.session_state.sort_params
-                if st.session_state.limit_param:
-                    st.session_state.query_params["limit"] = st.session_state.limit_param
-                st.session_state.query_params["method"] = method
+            if len(st.session_state.sort_params) > 0:
+                st.session_state.query_params["sort"] = st.session_state.sort_params
+            if st.session_state.limit_param:
+                st.session_state.query_params["limit"] = st.session_state.limit_param
+            if st.session_state.unique_yes:
+                st.session_state.query_params["unique"] = True
+            st.session_state.query_params["method"] = method
 
     # create a checkbox to show the query parameters
     st.checkbox(
         label="Show Query Parameters",
         key="show_query_params",
         help="Show the query parameters.",
     )
@@ -355,76 +358,93 @@
 
     query_button_placeholder.button(
         label="Run Query",
         key="run_query",
         type="primary",
         use_container_width=True,
         disabled=query_btn_disabled,
-        on_click=run_query,
-        args=(st.session_state.query_params,),
     )
+    new_results_placeholder = st.empty()
+    if st.session_state.run_query:
+        try:
+            with st.spinner("Running query..."):
+                st.session_state.pop("last_query", None)
+                st.session_state.last_query = xbrl.query(
+                    **st.session_state.query_params, as_dataframe=True, print_query=True, streamlit=True
+                )
 
-    # show the dataframe
-    st.subheader("Last Query Results")
-    if "last_query" not in st.session_state:
-        st.info("No **Query** has been run yet.")
-
-    else:
-        # show a download button to get the data in csv format
-        # box for file name
-        filename = st.text_input(
-            label="File Name",
-            value="xbrl data",
-        )
-        dwnld_btn_place, del_btn_place = st.columns(2)
-
-        # show a button to show the full data
-        st.checkbox(
-            label="My computer rocks! 🚀 Show Full Data",
-            help="Show the full data.",
-            key="show_full_data",
-        )
-        if st.session_state.show_full_data:
-            st.success(
-                f"""Viewing full data: **{st.session_state.last_query.shape[0]}**
-                rows and **{st.session_state.last_query.shape[1]}** columns."""
-            )
+        except Exception as e:
+            new_results_placeholder.warning(
+                f"Your query is taking a long time... \n"
+                f"The server may still be working on this query. "
+                f"You can wait and try again in a few minutes. "
+                f"Or try narrowing your search criteria. \n"
+                f"\n {e}"
+            )
+            st.stop()
+
+    with new_results_placeholder.container():
+        # show the dataframe
+        st.subheader("Last Query Results")
+        if "last_query" not in st.session_state:
+            st.info("No **Query** has been run yet.")
 
-            st.dataframe(
-                data=st.session_state.last_query,
-                use_container_width=True,
-                hide_index=True,
-            )
         else:
-            st.success(
-                f"""Query has **{st.session_state.last_query.shape[0]}** rows.
-                You are viewing **{min(100, st.session_state.last_query.shape[0])}** rows
-                and **{st.session_state.last_query.shape[1]}** columns.
-                You can try **Show Full Data** or **Download** the full data instead."""
-            )
+            # show a download button to get the data in csv format
+            # box for file name
+            filename = st.text_input(
+                label="File Name",
+                value="xbrl data",
+            )
+            dwnld_btn_place, del_btn_place = st.columns(2)
+
+            # show a button to show the full data
+            st.checkbox(
+                label="My computer rocks! 🚀 Show Full Data",
+                help="Show the full data.",
+                key="show_full_data",
+            )
+            if st.session_state.show_full_data:
+                st.success(
+                    f"""Viewing full data: **{st.session_state.last_query.shape[0]}**
+                    rows and **{st.session_state.last_query.shape[1]}** columns."""
+                )
 
-            st.dataframe(
-                data=st.session_state.last_query.head(100),
-                use_container_width=True,
-                hide_index=True,
-            )
+                st.dataframe(
+                    data=st.session_state.last_query,
+                    use_container_width=True,
+                    hide_index=True,
+                )
+            else:
+                st.success(
+                    f"""Query has **{st.session_state.last_query.shape[0]}** rows.
+                    You are viewing **{min(100, st.session_state.last_query.shape[0])}** rows
+                    and **{st.session_state.last_query.shape[1]}** columns.
+                    You can try **Show Full Data** or **Download** the full data instead."""
+                )
 
-        with dwnld_btn_place:
-            st.download_button(
-                label="Download as CSV File",
-                use_container_width=True,
-                data=st.session_state.last_query.to_csv(index=False).encode("utf-8"),
-                file_name=f"{filename}.csv",
-                mime="text/csv",
-                key="download_data",
-            )
+                st.dataframe(
+                    data=st.session_state.last_query.head(100),
+                    use_container_width=True,
+                    hide_index=True,
+                )
 
-        with del_btn_place:
-            st.button(
-                label="Delete Query",
-                key="delete_query_btn",
-                on_click=lambda: st.session_state.pop("last_query"),
-                type="primary",
-                use_container_width=True,
-            )
+            with dwnld_btn_place:
+                st.download_button(
+                    label="Download as CSV File",
+                    use_container_width=True,
+                    data=st.session_state.last_query.to_csv(index=False).encode("utf-8"),
+                    file_name=f"{filename}.csv",
+                    mime="text/csv",
+                    key="download_data",
+                )
+
+            with del_btn_place:
+                st.button(
+                    label="Delete Query",
+                    key="delete_query_btn",
+                    on_click=lambda: st.session_state.pop("last_query"),
+                    type="primary",
+                    use_container_width=True,
+                )
 
     # st.write(st.session_state)
```

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/assertion search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/assertion search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/concept name search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/concept name search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/concept search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/concept search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/cube search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/cube search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/dimension search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/dimension search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/document search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/document search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/dts id concept name.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/dts id concept name.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/dts id concept reference.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/dts id concept reference.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/dts id concept search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/dts id concept search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/dts id network search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/dts id network search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/dts id network.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/dts id network.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/dts search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/dts search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/entity id report search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/entity id report search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/entity report search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/entity report search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/fact id.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/fact id.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/fact search oim.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/fact search oim.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/fact search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/fact search.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 description: Search for XBRL facts based on the attributes of the fact, the report it was in, or the source of the data.
 parameters:
   concept.id:
     type: integer
     description: A unique integer for a concept that can be searched. This is a faster way to retrieve the details of a fact, however it is namespace specific and will only search for the use of a concept for a specific schema.
+    values: 0
   concept.is-base:
     type: boolean
     description: Indicates whether the concept is a base element in the reporting taxonomy or a company extension.
   concept.is-monetary:
     type: boolean
     description: Indicates whether the concept represents a monetary value.
   concept.local-name:
     type: array[string]
     description: The name of the concept in the base schema of a taxonomy, excluding the namespace. Use this to search across multiple taxonomies where the local name is known to be consistent over time.
+    vales: "e.g. Revenue,NetIncomeLoss (no spaces allowed)"
   concept.namespace:
     type: string
     description: The namespace of the concept used to identify a fact.
+    values: ""  # TODO: check
   dimension.is-base:
     type: boolean
     description: Indicates whether the dimension (aspect) is a base element in the reporting taxonomy or a company extension.
   dimension.local-name:
     type: array[string]
     description: The local name of the dimension used with the fact.
+    values: ""
   dimension.namespace:
     type: string
     description: The namespace of the dimension used with the fact.
+    values: ""
   dimensions.count:
     type: array[integer]
     description: The number of dimensional qualifiers associated with a given fact. A comma-delimited list will return facts with 0, 1, 2, etc., dimensions.
+    values: {"min":0, "max":1000} # TODO: check max
   dimensions.id:
     type: string
     description: The ID of the dimension.
   dts.entry-point:
     type: string
     description: The URL entry point of a discoverable taxonomy set. Also known as the entry point for a taxonomy.
   dts.id:
```

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/label dts id search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/label dts id search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/network id relationship search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/network id relationship search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/network relationship search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/network relationship search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/relationship search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/relationship search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/relationship tree search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/relationship tree search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/report fact search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/report fact search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/report id fact search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/report id fact search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/report id.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/report id.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/methods/report search.yml` & `xbrl-us-0.0.32/src/xbrl_us/methods/report search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/schemas/concept_details.py` & `xbrl-us-0.0.32/src/xbrl_us/schemas/concept_details.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/schemas/dimension_details.py` & `xbrl-us-0.0.32/src/xbrl_us/schemas/dimension_details.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/utils/exceptions.py` & `xbrl-us-0.0.32/src/xbrl_us/utils/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,7 +29,15 @@
 
 class XBRLRequiredValueError(ValueError):
     """Raised when no method name is provided."""
 
     def __init__(self, key, method):
         message = f"Missing required parameters: required parameter(s) for '{method}' method: '{key}'."
         super().__init__(message)
+
+
+class XBRLTimeOutError(ConnectionError):
+    """Raised when a connection error occurs."""
+
+    def __init__(self, e):
+        message = f"{e}\n\n The query is taking a long time. set timeout to None or try again later."
+        super().__init__(message)
```

### Comparing `xbrl-us-0.0.31/src/xbrl_us/utils/paramters.py` & `xbrl-us-0.0.32/src/xbrl_us/utils/paramters.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/src/xbrl_us/xbrl_us.py` & `xbrl-us-0.0.32/src/xbrl_us/xbrl_us.py`

 * *Files 2% similar despite different names*

```diff
@@ -418,15 +418,15 @@
     def _ensure_access_token(self):
         if not self.access_token or self._is_access_token_expired():
             if self.refresh_token and not self._is_refresh_token_expired():
                 self._get_token(grant_type="refresh_token", refresh_token=self.refresh_token)
             else:
                 self._get_token()
 
-    @retry(exceptions=_query_exceptions, tries=3, delay=2, backoff=2)
+    @retry(exceptions=_query_exceptions, tries=3, delay=2, backoff=2, logger=None)
     def _make_request(self, method, url, **kwargs) -> requests.Response:
         """
         Makes an HTTP request with the provided method, URL, and additional arguments.
 
         Args:
             method (str): The HTTP method for the request.
             url (str): The URL to send the request to.
@@ -436,17 +436,19 @@
             requests.Response: The response object.
         """
         self._ensure_access_token()
 
         headers = kwargs.get("headers", {})
         headers.update({"Authorization": f"Bearer {self.access_token}"})
         kwargs["headers"] = headers
-
-        response = requests.request(method, url, timeout=30, **kwargs)
-        return response
+        try:
+            response = requests.request(method, url, **kwargs)
+            return response
+        except Exception as e:
+            raise e
 
     def _get_account_limit(
         self,
         url: str,
         params: dict,
     ):
         # Query the API with a limit of more than 5000.
@@ -464,15 +466,15 @@
         match = re.search(r"user limit amount is (\d+)", response.text)
         if match:
             self.account_limit = int(match.group(1))
         else:
             print(f"Error: {response.status_code}")
             self.account_limit = None
 
-    def _get_method_url(self, method_name: str, parameters) -> str:
+    def _get_method_url(self, method_name: str, parameters: dict, unique: bool) -> str:
         """
         Get the URL for the specified method from the YAML file.
 
         Args:
             method_name (str): The name of the method.
             parameters: The parameters for the method.
 
@@ -499,26 +501,31 @@
                 for key in missing_keys:
                     raise exceptions.XBRLRequiredValueError(key=key, method=method_name)
 
             # get the required parameters for this method
             for key, value in values.items():
                 placeholder = "{" + key + "}"
                 url = url.replace(placeholder, str(value))
+        if unique:
+            return f"https://api.xbrl.us{url}?unique"
+
         return f"https://api.xbrl.us{url}?"
 
     @_convert_params_to_dict_decorator()
     def query(
         self,
         method: str,
         fields: Optional[list] = None,
         parameters: Optional[Union[Parameters, dict]] = None,
         limit: Optional[int] = None,
         sort: Optional[dict] = None,
+        unique: Optional[bool] = False,
         as_dataframe: bool = False,
         print_query: Optional[bool] = False,
+        timeout: Optional[int] = 5,
         **kwargs,
     ) -> Union[dict, DataFrame]:
         """
 
         Args:
             method (str): The name of the method to query.
             fields (list): The fields query parameter establishes the details of the data to return for the specific query.
@@ -526,23 +533,26 @@
             limit (int): A limit restricts the number of results returned by the query.
                 The limit attribute can only be added to an object type and not a property.
                 For example, to limit the number of facts in a query, {"fact": 10}.
             sort (dict): Any returned value can be sorted in ascending or descending order,
                 using ``ASC`` or ``DESC`` (i.e. {"report.document-type": "DESC"}.
                 Multiple sort criteria can be defined and the sort sequence is determined by
                 the order of the items in the dictionary.
+            unique (bool): If ``True`` returns only unique values.
             as_dataframe (bool): If ``True`` returns the results as a ``DataFrame`` else returns the data
                 as ``json``.
             print_query (bool=False): Whether to print the query.
+            timeout: The number of seconds to wait for a response from the server. Defaults to 5 seconds.
+                If ``None`` will wait indefinitely.
 
         Returns:
             dict | DataFrame: The results of the query.
         """
 
-        method_url = self._get_method_url(method, parameters)
+        method_url = self._get_method_url(method_name=method, parameters=parameters, unique=unique)
         # if limit is all
         if limit == "all":
             # arbitrary large number
             limit = 999999999
 
         query_params = _build_query_params(
             method=method,
@@ -562,33 +572,37 @@
         # ensure the limit is not greater than the account limit
         account_limit = min(limit, self.account_limit) if limit is not None else self.account_limit
 
         streamlit_indicator = kwargs.get("streamlit", False)
         if streamlit_indicator:
             from stqdm import stqdm
 
-            pbar = stqdm(total=None, desc="Downloading Data:", ncols=80)
+            pbar = stqdm(total=None, desc="Matches Found", ncols=80)
         else:
             # create a progress bar
-            pbar = tqdm(total=None, desc="Downloading Data:", ncols=80)
+            pbar = tqdm(total=None, desc="Matches Found", ncols=80, position=0, leave=True)
 
         # update the limit in the query params with the new limit
         query_params = _build_query_params(
             method=method,
             fields=fields,
             parameters=parameters,
             limit=account_limit,
             sort=sort,
         )
 
-        response = self._make_request(
-            method="get",
-            url=method_url,
-            params=query_params,
-        )
+        try:
+            response = self._make_request(
+                method="get",
+                url=method_url,
+                params=query_params,
+                timeout=timeout,
+            )
+        except requests.exceptions.ReadTimeout as e:
+            raise exceptions.XBRLTimeOutError(e) from e
 
         response_data = response.json()
 
         if response.status_code != 200:
             raise response_data["message"]
         elif "data" not in response_data:
             warnings.warn("No data returned from the query.", UserWarning, stacklevel=2)
@@ -627,14 +641,15 @@
                     offset=offset,
                 )
 
                 response = self._make_request(
                     method="get",
                     url=method_url,
                     params=query_params,
+                    timeout=timeout,
                 )
 
                 response_data = response.json()
                 data = response_data["data"]
 
                 # Add the items to the overall collection
                 all_data.extend(data)
@@ -650,14 +665,14 @@
                     # it means we have reached the end
                     # of available items, so we can break out of the loop.
                     break
 
                 # Update the offset for the next request
                 offset += len(data)
 
-            except Exception as e:
-                raise e
+            except requests.exceptions.ReadTimeout as e:
+                raise exceptions.XBRLTimeOutError(e) from e
 
         if as_dataframe:
             return DataFrame.from_dict(all_data)
         else:
             return all_data
```

### Comparing `xbrl-us-0.0.31/src/xbrl_us.egg-info/PKG-INFO` & `xbrl-us-0.0.32/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,33 @@
-Metadata-Version: 2.1
-Name: xbrl-us
-Version: 0.0.31
-Summary: Python wrapper for xbrl.us API
-Home-page: https://github.com/hamid-vakilzadeh/python-xbrl-us
-Author: hamid-vakilzadeh
-Author-email: vakilzas@uww.edu
-License: MIT
-Project-URL: Documentation, https://python-xbrl-us.readthedocs.io/
-Project-URL: Changelog, https://python-xbrl-us.readthedocs.io/en/latest/changelog.html
-Project-URL: Issue Tracker, https://github.com/hamid-vakilzadeh/python-xbrl-us/issues
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 ======================
 XBRL-US Python Library
 ======================
 
+|Workflow| |Docs| |license| |Versions|
+
+
+.. |Workflow| image:: https://img.shields.io/github/actions/workflow/status/hamid-vakilzadeh/python-xbrl-us/github-actions.yml?logo=github&logoColor=white
+   :alt: GitHub Workflow Status (main)
+   :target: https://github.com/hamid-vakilzadeh/python-xbrl-us/actions/workflows/github-actions.yml
+
+.. |Downloads| image:: https://img.shields.io/pypi/dm/xbrl-us?logo=pypi&logoColor=orange&color=blue
+    :alt: PyPI - Downloads
+    :target: https://pypi.org/project/xbrl-us/
+
+.. |Versions| image:: https://img.shields.io/pypi/pyversions/xbrl-us?logo=python&logoColor=yellow&color=yellow
+    :alt: PyPI - Python Version
+    :target: https://pypi.org/project/xbrl-us/
+
+.. |Docs| image:: https://img.shields.io/readthedocs/python-xbrl-us/latest?logo=read-the-docs&logoColor=white
+    :target: https://python-xbrl-us.readthedocs.io/en/latest/?badge=latest
+    :alt: Read the Docs (latest)
+
+.. |license| image:: https://img.shields.io/github/license/hamid-vakilzadeh/python-xbrl-us?logo=github&logoColor=white&color=blue
+   :target: https://github.com/hamid-vakilzadeh/python-xbrl-us/blob/main/LICENSE
+
 About
 =====
 
 The XBRL US Python Wrapper is a powerful tool for interacting with the XBRL US API,
 providing seamless integration of XBRL data into Python applications.
 This wrapper simplifies the process of retrieving and analyzing financial data in XBRL format,
 enabling users to access a wide range of financial information for companies registered with the U.S.
@@ -62,32 +54,32 @@
 
     [FILL: Publication Details]
 
 
 Tutorial ✏️📖📚
 ================
 
-This tutorial will guide you through using the XBRL-US Python library to interact with the XBRL API. The XBRL-US library provides a convenient way to query and retrieve financial data from the XBRL API using Python.
+This tutorial will guide you through using the XBRL-US Python library to interact with the XBRL API.
+The XBRL-US library provides a convenient way to query and retrieve financial data from the XBRL API using Python.
 
-Prerequisites
-~~~~~~~~~~~~~
+1. Prerequisites
+~~~~~~~~~~~~~~~~
 
 Before you begin, ensure you have the following:
 
 * **Python installed on your system**.
   The XBRL-US library supports Python 3.8 and above.
-* **XBRL-US library installed**.
 * **XBRL-US API credentials**.
   You can obtain your credentials by registering for a
   free XBRL-US account at https://xbrl.us/home/use/xbrl-api/.
 * **XBRL-US OAuth2 Access**.
   You can obtain your client ID and client secret by registering for a
   filling the request form at https://xbrl.us/home/use/xbrl-api/access-token/.
 
-You can install it using pip:
+You can install this package using pip:
 
 .. code-block:: bash
 
     pip install xbrl-us
 
 .. caution::
 
@@ -102,50 +94,74 @@
 For detailed information about the XBRL-US Python
 library, you can refer to the documentation at https://python-xbrl-us.readthedocs.io/en/latest/.
 
 **Official Documentation**
 
 For more information about the XBRL API and its endpoints, refer to the original API documentation at https://xbrlus.github.io/xbrl-api.
 
-Step 1: Import the XBRL Library
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+2. Choose Your Preferred Approach
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+There are two distinct ways to use the XBRL-US Python package:
+
+* **Code-Based Approach**: Import the XBRL-US Python package directly into your Python
+  environment for in-depth, custom analysis (see **Code-Based Approach**)
+
+* **Browser Interface**: For a no-code experience, navigate to the **Browser Interface**.
+  This interface allows for easy exploration and analysis of XBRL data directly in your web
+  browser.
+
+.. _code-based approach:
+
+2.1. Code-Based Approach
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+Import the XBRL Library
+-------------------------------
 
 To start using the XBRL-US library,
-you need to import it into your Python script::
+you need to import it into your Python script:
+
+.. code-block:: python
 
     from xbrl_us import XBRL
 
-Step 2: Create an Instance of XBRL Class
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Create an Instance of XBRL Class
+----------------------------------------
 
 Next, you need to create an instance of the ``XBRL`` class,
 providing your authentication credentials
-(client ID, client secret, username, and password) as parameters::
+(client ID, client secret, username, and password) as parameters:
+
+.. code-block:: python
 
     xbrl = XBRL(
     client_id='Your client id',
     client_secret='Your client secret',
     username='Your username',
     password='Your password'
     )
 
 Make sure to replace ``Your client id``,
 ``Your client secret``, ``Your username``, and
 ``Your password`` with your actual credentials.
 
-Step 3: Query the XBRL API
-~~~~~~~~~~~~~~~~~~~~~~~~~~
+Query the XBRL API
+------------------
 
 The XBRL-US library provides a query method to search
 for data from the XBRL API. You can specify various
 parameters and fields to filter and retrieve the
 desired data.
 
 Here's an example of using the query method to search
-for specific financial facts::
+for specific financial facts:
+
+.. code-block:: python
 
     response = xbrl.query(
         method='fact search',
         parameters={
             "concept.local-name": [
                 'OperatingIncomeLoss',
                 'GrossProfit',
@@ -179,15 +195,17 @@
 We are also specifying the fields we want to retrieve
 in the response. The ``limit`` parameter restricts the
 number of facts returned to 100, and ``as_dataframe=True``
 ensures the response is returned as a ``Pandas DataFrame``.
 
 Alternatively, you can use the ``Parameters`` and ``Fields``
 classes provided by the library to make the query more
-readable, less prone to errors, and easier to maintain::
+readable, less prone to errors, and easier to maintain:
+
+.. code-block:: python
 
     from xbrl_us.utils import Parameters, Fields
 
     response = xbrl.query(
         method='fact search',
         parameters=Parameters(
             concept_local_name=[
@@ -219,23 +237,25 @@
     )
 
 
 This alternative approach also allows you to
 take advantage of the autocomplete feature of your IDE to
 easily find the parameters and fields.
 
-Step 4: Perform Additional Queries
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Perform Additional Queries
+----------------------------------
 
 You can use the same query method to call other API
 endpoints by changing the method parameter and
 providing the relevant parameters and fields.
 
 Here's an example of using the query method to
-search for a specific fact by its ID::
+search for a specific fact by its ID:
+
+.. code-block:: python
 
     response = xbrl.query(
     method='fact id',
     parameters={'fact.id': 123},
     fields=[
         'report.accession',
         'period.fiscal-year',
@@ -253,65 +273,86 @@
     ],
     as_dataframe=False
     )
 
 Congratulations! You have learned how to use the XBRL-US Python library to interact with the XBRL API.
 In this example you will receive the data in json format as the ``as_dataframe`` parameter is set to ``False``.
 
+.. _browser interface:
 
-Development
-===========
+2.2 Browser Interface 🖥️
+~~~~~~~~~~~~~~~~~~~~~~~~
 
-To run all the tests run::
+This feature is designed to make our package even more user-friendly, allowing users to interact and work with XBRL data
+directly through a graphical interface, in addition to the existing code-based methods.
 
-    tox
+The browser interface streamlines data visualization, simplifies navigation, and enhances user interactions.
+With this intuitive, user-friendly interface, you can easily explore, interpret, and analyze XBRL data in real-time,
+right from your web browser.
 
-Note, to combine the coverage data from all the tox environments run:
+Key Features:
 
-.. list-table::
-    :widths: 10 90
-    :stub-columns: 1
+* Create Real-time queries right in your browser
+* Intuitive navigation and search features
+* Filtering and sorting options
+* Seamless integration with the existing XBRL-US Python API
 
-    - - Windows
-      - ::
+Getting started is as simple as ever.
+Update your XBRL-US Python package to the latest version and launch the new Browser Interface from the package menu.
 
-            set PYTEST_ADDOPTS=--cov-append
-            tox
+Getting Started with the Browser Interface
+------------------------------------------
 
-    - - Other
-      - ::
+Getting started is as simple as ever.
+First, ensure you have the latest version of ``xbrl-us`` installed by running the following code:
 
-            PYTEST_ADDOPTS=--cov-append tox
+.. code-block:: bash
+
+    pip install xbrl-us --upgrade
+
+
+Next, launch the new Browser Interface from the package menu:
 
+.. code-block:: bash
 
-Changelog
-=========
+    python -m xbrl_us
 
-0.0.31 (2023-07-14)
-~~~~~~~~~~~~~~~~~~~
+That is it!
+You should now see the new Browser Interface open in your default web browser.
 
-* fixed dependency issues
-* Bug fixes
+Happy data exploring!
 
+.. note::
 
-0.0.3 (2023-07-14)
-~~~~~~~~~~~~~~~~~~
+    Please note, while we have tested the interface extensively, this is its initial release.
+    We encourage users to provide feedback to help us further improve the tool. We value your input!
+    You can also find tutorials, example codes, and more resources to help you get started.
 
-* Backward compatibility with Python 3.8 and 3.9
-* Bug fixes
 
-0.0.2 (2023-07-12)
-~~~~~~~~~~~~~~~~~~
 
+Development
+===========
 
-* Bug fixes
-* Enhanced error handling
-* Improved ``methods`` attributes
-* Added the ability to print the query string
-* Implemented a feature to handle queries with large limits
-* NEW: Introduced a web interface for the API, making it even easier to use
+To run all the tests run:
 
+.. code-block:: bash
+
+    tox
 
-0.0.1 (2023-07-09)
-~~~~~~~~~~~~~~~~~~
 
-* First release on PyPI.
+Note, to combine the coverage data from all the tox environments run:
+
+.. list-table::
+    :widths: 10 90
+    :stub-columns: 1
+
+    * - Windows
+      - .. code-block:: bash
+
+            set PYTEST_ADDOPTS=--cov-append
+            tox
+
+
+    * - Other
+      - .. code-block:: bash
+
+            PYTEST_ADDOPTS=--cov-append tox
```

### Comparing `xbrl-us-0.0.31/src/xbrl_us.egg-info/SOURCES.txt` & `xbrl-us-0.0.32/src/xbrl_us.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/tests/test_xbrl_us.py` & `xbrl-us-0.0.32/tests/test_xbrl_us.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.31/tox.ini` & `xbrl-us-0.0.32/tox.ini`

 * *Files identical despite different names*

